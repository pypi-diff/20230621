# Comparing `tmp/mediagrains-3.5.1.tar.gz` & `tmp/mediagrains-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediagrains-3.5.1.tar", last modified: Wed Jan 11 10:35:23 2023, max compression
+gzip compressed data, was "mediagrains-3.5.2.tar", last modified: Wed Jun 21 07:45:54 2023, max compression
```

## Comparing `mediagrains-3.5.1.tar` & `mediagrains-3.5.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.496645 mediagrains-3.5.1/
--rw-r--r--   0 root         (0) root         (0)      573 2023-01-11 10:22:34.000000 mediagrains-3.5.1/COPYING
--rw-r--r--   0 root         (0) root         (0)     6607 2023-01-11 10:22:34.000000 mediagrains-3.5.1/ICLA.md
--rw-r--r--   0 root         (0) root         (0)    11362 2023-01-11 10:22:34.000000 mediagrains-3.5.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      147 2023-01-11 10:22:34.000000 mediagrains-3.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      358 2023-01-11 10:35:23.496645 mediagrains-3.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10548 2023-01-11 10:22:34.000000 mediagrains-3.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.480645 mediagrains-3.5.1/examples/
--rw-r--r--   0 root         (0) root         (0)    62845 2023-01-11 10:22:34.000000 mediagrains-3.5.1/examples/audio.gsf
--rw-r--r--   0 root         (0) root         (0)     8295 2023-01-11 10:22:34.000000 mediagrains-3.5.1/examples/coded_audio.gsf
--rw-r--r--   0 root         (0) root         (0)    68457 2023-01-11 10:22:34.000000 mediagrains-3.5.1/examples/coded_video.gsf
--rw-r--r--   0 root         (0) root         (0)    37610 2023-01-11 10:22:34.000000 mediagrains-3.5.1/examples/event.gsf
--rw-r--r--   0 root         (0) root         (0) 25011059 2023-01-11 10:22:34.000000 mediagrains-3.5.1/examples/interleaved.gsf
--rw-r--r--   0 root         (0) root         (0)  1946205 2023-01-11 10:22:34.000000 mediagrains-3.5.1/examples/video.gsf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.484645 mediagrains-3.5.1/mediagrains/
--rw-r--r--   0 root         (0) root         (0)     1904 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/__init__.py
--rw-r--r--   0 root         (0) root         (0)      100 2023-01-11 10:29:01.000000 mediagrains-3.5.1/mediagrains/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.484645 mediagrains-3.5.1/mediagrains/asyncio/
--rw-r--r--   0 root         (0) root         (0)    29394 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4464 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/asyncio/aiobytes.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/asyncio/bytesaio.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/asyncio/py.typed
--rw-r--r--   0 root         (0) root         (0)     5644 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/cogenums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.484645 mediagrains-3.5.1/mediagrains/comparison/
--rw-r--r--   0 root         (0) root         (0)     2321 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/comparison/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1435 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/comparison/__main__.py
--rw-r--r--   0 root         (0) root         (0)    41713 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/comparison/_internal.py
--rw-r--r--   0 root         (0) root         (0)     8221 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/comparison/options.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/comparison/psnr.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/comparison/py.typed
--rw-r--r--   0 root         (0) root         (0)     1432 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/grain.py
--rw-r--r--   0 root         (0) root         (0)    31876 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/grain_constructors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.484645 mediagrains-3.5.1/mediagrains/grains/
--rw-r--r--   0 root         (0) root         (0)     8158 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/grains/AudioGrain.py
--rw-r--r--   0 root         (0) root         (0)     8807 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/grains/CodedAudioGrain.py
--rw-r--r--   0 root         (0) root         (0)    16187 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/grains/CodedVideoGrain.py
--rw-r--r--   0 root         (0) root         (0)    11074 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/grains/EventGrain.py
--rw-r--r--   0 root         (0) root         (0)    27612 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/grains/Grain.py
--rw-r--r--   0 root         (0) root         (0)    19821 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/grains/VideoGrain.py
--rw-r--r--   0 root         (0) root         (0)      986 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/grains/__init__.py
--rw-r--r--   0 root         (0) root         (0)   100429 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/gsf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.488645 mediagrains-3.5.1/mediagrains/hypothesis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/hypothesis/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/hypothesis/py.typed
--rw-r--r--   0 root         (0) root         (0)    35973 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/hypothesis/strategies.py
--rw-r--r--   0 root         (0) root         (0)    35626 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/hypothesis/strategies_new.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.488645 mediagrains-3.5.1/mediagrains/numpy/
--rw-r--r--   0 root         (0) root         (0)      856 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/numpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/numpy/audiograin.py
--rw-r--r--   0 root         (0) root         (0)    21284 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/numpy/convert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.488645 mediagrains-3.5.1/mediagrains/numpy/numpy_grains/
--rw-r--r--   0 root         (0) root         (0)     8748 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/numpy/numpy_grains/AudioGrain.py
--rw-r--r--   0 root         (0) root         (0)    18775 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/numpy/numpy_grains/VideoGrain.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/numpy/numpy_grains/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/numpy/py.typed
--rw-r--r--   0 root         (0) root         (0)     3518 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/numpy/videograin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.488645 mediagrains-3.5.1/mediagrains/patterngenerators/
--rw-r--r--   0 root         (0) root         (0)      968 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4538 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.488645 mediagrains-3.5.1/mediagrains/patterngenerators/audio/
--rw-r--r--   0 root         (0) root         (0)      747 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/audio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/audio/abc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/audio/py.typed
--rw-r--r--   0 root         (0) root         (0)     8613 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/audio/tone.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.488645 mediagrains-3.5.1/mediagrains/patterngenerators/video/
--rw-r--r--   0 root         (0) root         (0)      905 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/video/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/video/abc.py
--rw-r--r--   0 root         (0) root         (0)     3126 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/video/colourbars.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/video/constants.py
--rw-r--r--   0 root         (0) root         (0)     3275 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/video/lumasteps.py
--rw-r--r--   0 root         (0) root         (0)     4772 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/video/movingbaroverlay.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/video/py.typed
--rw-r--r--   0 root         (0) root         (0)     1639 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/patterngenerators/video/still.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/py.typed
--rw-r--r--   0 root         (0) root         (0)    15613 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/testsignalgenerator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.488645 mediagrains-3.5.1/mediagrains/tools/
--rw-r--r--   0 root         (0) root         (0)      866 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2463 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/tools/_file_or_pipe.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/tools/extract_from_gsf.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/tools/py.typed
--rw-r--r--   0 root         (0) root         (0)     7917 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/tools/wrap_in_gsf.py
--rw-r--r--   0 root         (0) root         (0)     8857 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.492645 mediagrains-3.5.1/mediagrains/utils/
--rw-r--r--   0 root         (0) root         (0)      855 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4375 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/utils/adts_aac_grain_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2685 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/utils/adts_aac_parser.py
--rw-r--r--   0 root         (0) root         (0)    12975 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/utils/asyncbinaryio.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/utils/grain_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     7023 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/utils/h264_grain_wrapper.py
--rw-r--r--   0 root         (0) root         (0)    31576 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/utils/h264_parser.py
--rw-r--r--   0 root         (0) root         (0)     6642 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/utils/iobytes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/utils/py.typed
--rw-r--r--   0 root         (0) root         (0)     6270 2023-01-11 10:22:34.000000 mediagrains-3.5.1/mediagrains/utils/synchronise.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.484645 mediagrains-3.5.1/mediagrains.egg-info/
--rw-r--r--   0 root         (0) root         (0)      358 2023-01-11 10:35:23.000000 mediagrains-3.5.1/mediagrains.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3437 2023-01-11 10:35:23.000000 mediagrains-3.5.1/mediagrains.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-11 10:35:23.000000 mediagrains-3.5.1/mediagrains.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      230 2023-01-11 10:35:23.000000 mediagrains-3.5.1/mediagrains.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-01-11 10:35:23.000000 mediagrains-3.5.1/mediagrains.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-01-11 10:35:23.000000 mediagrains-3.5.1/mediagrains.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-11 10:35:23.496645 mediagrains-3.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2565 2023-01-11 10:22:34.000000 mediagrains-3.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:35:23.496645 mediagrains-3.5.1/tests/
--rw-r--r--   0 root         (0) root         (0)     4625 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/audio_utils.py
--rw-r--r--   0 root         (0) root         (0)     4575 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/fixtures.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_adts_aac_parser.py
--rw-r--r--   0 root         (0) root         (0)    30682 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_asyncio_gsf.py
--rw-r--r--   0 root         (0) root         (0)    30683 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_asyncio_gsf_newcode.py
--rw-r--r--   0 root         (0) root         (0)     7054 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_audio_psnr.py
--rw-r--r--   0 root         (0) root         (0)     7042 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_audio_psnr_newcode.py
--rw-r--r--   0 root         (0) root         (0)     8498 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_comparison.py
--rw-r--r--   0 root         (0) root         (0)     8753 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_comparison_newcode.py
--rw-r--r--   0 root         (0) root         (0)    83405 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_grain.py
--rw-r--r--   0 root         (0) root         (0)    84060 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_grain_newcode.py
--rw-r--r--   0 root         (0) root         (0)   121022 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_gsf.py
--rw-r--r--   0 root         (0) root         (0)   122049 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_gsf_newcode.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_iobytes.py
--rw-r--r--   0 root         (0) root         (0)     8681 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_numpy_audiograin.py
--rw-r--r--   0 root         (0) root         (0)     8693 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_numpy_audiograin_newcode.py
--rw-r--r--   0 root         (0) root         (0)    41394 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_numpy_videograin.py
--rw-r--r--   0 root         (0) root         (0)    41533 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_numpy_videograin_newcode.py
--rw-r--r--   0 root         (0) root         (0)    29844 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_patterngenerators.py
--rw-r--r--   0 root         (0) root         (0)    33788 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_testsignalgenerator.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_video_psnr.py
--rw-r--r--   0 root         (0) root         (0)     8273 2023-01-11 10:22:34.000000 mediagrains-3.5.1/tests/test_video_psnr_newcode.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.918506 mediagrains-3.5.2/
+-rw-r--r--   0 root         (0) root         (0)      573 2023-03-04 06:59:09.000000 mediagrains-3.5.2/COPYING
+-rw-r--r--   0 root         (0) root         (0)     6607 2023-03-04 06:59:09.000000 mediagrains-3.5.2/ICLA.md
+-rw-r--r--   0 root         (0) root         (0)    11362 2023-03-04 06:59:09.000000 mediagrains-3.5.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      147 2023-03-04 06:59:09.000000 mediagrains-3.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-21 07:45:54.918506 mediagrains-3.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10377 2023-03-29 08:10:32.000000 mediagrains-3.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.906506 mediagrains-3.5.2/examples/
+-rw-r--r--   0 root         (0) root         (0)    62845 2023-03-04 06:59:09.000000 mediagrains-3.5.2/examples/audio.gsf
+-rw-r--r--   0 root         (0) root         (0)     8295 2023-03-04 06:59:09.000000 mediagrains-3.5.2/examples/coded_audio.gsf
+-rw-r--r--   0 root         (0) root         (0)    68457 2023-03-04 06:59:09.000000 mediagrains-3.5.2/examples/coded_video.gsf
+-rw-r--r--   0 root         (0) root         (0)    37610 2023-03-04 06:59:09.000000 mediagrains-3.5.2/examples/event.gsf
+-rw-r--r--   0 root         (0) root         (0) 25011059 2023-03-04 06:59:09.000000 mediagrains-3.5.2/examples/interleaved.gsf
+-rw-r--r--   0 root         (0) root         (0)  1946205 2023-03-04 06:59:09.000000 mediagrains-3.5.2/examples/video.gsf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.910507 mediagrains-3.5.2/mediagrains/
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-21 07:41:41.000000 mediagrains-3.5.2/mediagrains/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.910507 mediagrains-3.5.2/mediagrains/asyncio/
+-rw-r--r--   0 root         (0) root         (0)    29394 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4464 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/asyncio/aiobytes.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/asyncio/bytesaio.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/asyncio/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5644 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/cogenums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.910507 mediagrains-3.5.2/mediagrains/comparison/
+-rw-r--r--   0 root         (0) root         (0)     2321 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/comparison/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/comparison/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    41713 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/comparison/_internal.py
+-rw-r--r--   0 root         (0) root         (0)     8221 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/comparison/options.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/comparison/psnr.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/comparison/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/grain.py
+-rw-r--r--   0 root         (0) root         (0)    31876 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/grain_constructors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.910507 mediagrains-3.5.2/mediagrains/grains/
+-rw-r--r--   0 root         (0) root         (0)     8158 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/grains/AudioGrain.py
+-rw-r--r--   0 root         (0) root         (0)     8807 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/grains/CodedAudioGrain.py
+-rw-r--r--   0 root         (0) root         (0)    16187 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/grains/CodedVideoGrain.py
+-rw-r--r--   0 root         (0) root         (0)    11074 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/grains/EventGrain.py
+-rw-r--r--   0 root         (0) root         (0)    27612 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/grains/Grain.py
+-rw-r--r--   0 root         (0) root         (0)    19821 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/grains/VideoGrain.py
+-rw-r--r--   0 root         (0) root         (0)      986 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/grains/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   100481 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/gsf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.910507 mediagrains-3.5.2/mediagrains/hypothesis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/hypothesis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/hypothesis/py.typed
+-rw-r--r--   0 root         (0) root         (0)    35973 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/hypothesis/strategies.py
+-rw-r--r--   0 root         (0) root         (0)    35626 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/hypothesis/strategies_new.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.914507 mediagrains-3.5.2/mediagrains/numpy/
+-rw-r--r--   0 root         (0) root         (0)      856 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/numpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/numpy/audiograin.py
+-rw-r--r--   0 root         (0) root         (0)    21764 2023-06-21 07:39:31.000000 mediagrains-3.5.2/mediagrains/numpy/convert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.914507 mediagrains-3.5.2/mediagrains/numpy/numpy_grains/
+-rw-r--r--   0 root         (0) root         (0)     8748 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/numpy/numpy_grains/AudioGrain.py
+-rw-r--r--   0 root         (0) root         (0)    18775 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/numpy/numpy_grains/VideoGrain.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/numpy/numpy_grains/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/numpy/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/numpy/videograin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.914507 mediagrains-3.5.2/mediagrains/patterngenerators/
+-rw-r--r--   0 root         (0) root         (0)      968 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4538 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.914507 mediagrains-3.5.2/mediagrains/patterngenerators/audio/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/audio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/audio/abc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/audio/py.typed
+-rw-r--r--   0 root         (0) root         (0)     8613 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/audio/tone.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.914507 mediagrains-3.5.2/mediagrains/patterngenerators/video/
+-rw-r--r--   0 root         (0) root         (0)      905 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/video/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/video/abc.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/video/colourbars.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/video/constants.py
+-rw-r--r--   0 root         (0) root         (0)     3275 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/video/lumasteps.py
+-rw-r--r--   0 root         (0) root         (0)     4772 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/video/movingbaroverlay.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/video/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/patterngenerators/video/still.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/py.typed
+-rw-r--r--   0 root         (0) root         (0)    15613 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/testsignalgenerator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.914507 mediagrains-3.5.2/mediagrains/tools/
+-rw-r--r--   0 root         (0) root         (0)      866 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/tools/_file_or_pipe.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/tools/extract_from_gsf.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/tools/py.typed
+-rw-r--r--   0 root         (0) root         (0)     7917 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/tools/wrap_in_gsf.py
+-rw-r--r--   0 root         (0) root         (0)     8857 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.918506 mediagrains-3.5.2/mediagrains/utils/
+-rw-r--r--   0 root         (0) root         (0)      855 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4375 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/utils/adts_aac_grain_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/utils/adts_aac_parser.py
+-rw-r--r--   0 root         (0) root         (0)    12975 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/utils/asyncbinaryio.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/utils/grain_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     7023 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/utils/h264_grain_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)    31542 2023-05-09 10:01:31.000000 mediagrains-3.5.2/mediagrains/utils/h264_parser.py
+-rw-r--r--   0 root         (0) root         (0)     6642 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/utils/iobytes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/utils/py.typed
+-rw-r--r--   0 root         (0) root         (0)     6270 2023-03-04 06:59:09.000000 mediagrains-3.5.2/mediagrains/utils/synchronise.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.910507 mediagrains-3.5.2/mediagrains.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-21 07:45:54.000000 mediagrains-3.5.2/mediagrains.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3437 2023-06-21 07:45:54.000000 mediagrains-3.5.2/mediagrains.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 07:45:54.000000 mediagrains-3.5.2/mediagrains.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-21 07:45:54.000000 mediagrains-3.5.2/mediagrains.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-21 07:45:54.000000 mediagrains-3.5.2/mediagrains.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-21 07:45:54.000000 mediagrains-3.5.2/mediagrains.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 07:45:54.922507 mediagrains-3.5.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-05-09 10:01:31.000000 mediagrains-3.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:45:54.918506 mediagrains-3.5.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     4625 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/audio_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4575 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_adts_aac_parser.py
+-rw-r--r--   0 root         (0) root         (0)    30682 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_asyncio_gsf.py
+-rw-r--r--   0 root         (0) root         (0)    30683 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_asyncio_gsf_newcode.py
+-rw-r--r--   0 root         (0) root         (0)     7054 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_audio_psnr.py
+-rw-r--r--   0 root         (0) root         (0)     7042 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_audio_psnr_newcode.py
+-rw-r--r--   0 root         (0) root         (0)     8498 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_comparison.py
+-rw-r--r--   0 root         (0) root         (0)     8753 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_comparison_newcode.py
+-rw-r--r--   0 root         (0) root         (0)    83405 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_grain.py
+-rw-r--r--   0 root         (0) root         (0)    84060 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_grain_newcode.py
+-rw-r--r--   0 root         (0) root         (0)   121022 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_gsf.py
+-rw-r--r--   0 root         (0) root         (0)   122049 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_gsf_newcode.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_iobytes.py
+-rw-r--r--   0 root         (0) root         (0)     8681 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_numpy_audiograin.py
+-rw-r--r--   0 root         (0) root         (0)     8693 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_numpy_audiograin_newcode.py
+-rw-r--r--   0 root         (0) root         (0)    41394 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_numpy_videograin.py
+-rw-r--r--   0 root         (0) root         (0)    41533 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_numpy_videograin_newcode.py
+-rw-r--r--   0 root         (0) root         (0)    29844 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_patterngenerators.py
+-rw-r--r--   0 root         (0) root         (0)    33788 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_testsignalgenerator.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_video_psnr.py
+-rw-r--r--   0 root         (0) root         (0)     8273 2023-03-04 06:59:09.000000 mediagrains-3.5.2/tests/test_video_psnr_newcode.py
```

### Comparing `mediagrains-3.5.1/COPYING` & `mediagrains-3.5.2/COPYING`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/ICLA.md` & `mediagrains-3.5.2/ICLA.md`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/LICENSE.md` & `mediagrains-3.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/README.md` & `mediagrains-3.5.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -216,33 +216,25 @@
 To do the same with a sine wave:
 ```bash
 ffmpeg -f lavfi -i "sine=frequency=1000:duration=5" -f s16le -ac 2 - | wrap_audio_in_gsf - output_audio.gsf --sample-rate 44100
 gsf_probe output_audio.gsf
 extract_gsf_essence output_audio.gsf - | ffplay -f s16le -ac 2 -ar 44100 pipe:0
 ```
 
-The tools have been packaged into docker images for convenience. Images for all the tools can be built using:
+The tools have been packaged into the `mediagrains` docker image for convenience. The `mediagrains` image containing all the tools can be built using:
 ```bash
 make tools
 ```
 
-Or individual tool images can be built using one of the following:
+You can make use of the tools image with the following command:
 ```bash
-make tool-gsf_probe
-make tool-extract_gsf_essence
-make tool-tool-wrap_audio_in_gsf
-make tool-tool-wrap_video_in_gsf
+$(make -s run-cmd) <TOOL> <ARGS>
 ```
 
-You can make use of the tools images with the following command, replacing the source data directory, image name and build tag as required:
-```bash
-$(make -s run-cmd-extract_gsf_essence) <ARGS>
-```
-
-Running the command without ARGS will provide help
+Running the command without `<TOOL>` or `<ARGS>` will list the available tools. Running without `<ARGS>` will provide help.
 
 ## Development
 ### Commontooling
 
 This repository uses a library of makefiles, templates, and other tools for development tooling and CI workflows. To discover operations that may be run against this repo, run the following in the top level of the repo:
 
 ```bash
```

### Comparing `mediagrains-3.5.1/examples/audio.gsf` & `mediagrains-3.5.2/examples/audio.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/examples/coded_audio.gsf` & `mediagrains-3.5.2/examples/coded_audio.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/examples/coded_video.gsf` & `mediagrains-3.5.2/examples/coded_video.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/examples/event.gsf` & `mediagrains-3.5.2/examples/event.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/examples/interleaved.gsf` & `mediagrains-3.5.2/examples/interleaved.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/examples/video.gsf` & `mediagrains-3.5.2/examples/video.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/__init__.py` & `mediagrains-3.5.2/mediagrains/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/asyncio/__init__.py` & `mediagrains-3.5.2/mediagrains/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/asyncio/aiobytes.py` & `mediagrains-3.5.2/mediagrains/asyncio/aiobytes.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/asyncio/bytesaio.py` & `mediagrains-3.5.2/mediagrains/asyncio/bytesaio.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/cogenums.py` & `mediagrains-3.5.2/mediagrains/cogenums.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/comparison/__init__.py` & `mediagrains-3.5.2/mediagrains/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/comparison/__main__.py` & `mediagrains-3.5.2/mediagrains/comparison/__main__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/comparison/_internal.py` & `mediagrains-3.5.2/mediagrains/comparison/_internal.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/comparison/options.py` & `mediagrains-3.5.2/mediagrains/comparison/options.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/comparison/psnr.py` & `mediagrains-3.5.2/mediagrains/comparison/psnr.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/grain.py` & `mediagrains-3.5.2/mediagrains/grain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/grain_constructors.py` & `mediagrains-3.5.2/mediagrains/grain_constructors.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/grains/AudioGrain.py` & `mediagrains-3.5.2/mediagrains/grains/AudioGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/grains/CodedAudioGrain.py` & `mediagrains-3.5.2/mediagrains/grains/CodedAudioGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/grains/CodedVideoGrain.py` & `mediagrains-3.5.2/mediagrains/grains/CodedVideoGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/grains/EventGrain.py` & `mediagrains-3.5.2/mediagrains/grains/EventGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/grains/Grain.py` & `mediagrains-3.5.2/mediagrains/grains/Grain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/grains/VideoGrain.py` & `mediagrains-3.5.2/mediagrains/grains/VideoGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/grains/__init__.py` & `mediagrains-3.5.2/mediagrains/grains/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/gsf.py` & `mediagrains-3.5.2/mediagrains/gsf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1559,15 +1559,15 @@
 
     @property
     def tags(self) -> Tuple["GSFEncoderTag", ...]:
         return tuple(self._tags)
 
     @property
     def segments(self) -> Mapping[int, "GSFEncoderSegment"]:
-        return frozendict(self._segments)
+        return frozendict(self._segments)  # type: ignore[operator]
 
     def add_tag(self, key: str, value: str):
         """Add a tag to the file"""
         if self._active_dump:
             raise GSFEncodeAddToActiveDump("Cannot add a new tag to an encoder that is currently dumping")
 
         self._tags.append(GSFEncoderTag(key, value))
@@ -1965,15 +1965,15 @@
 
     @property
     def tags(self) -> Tuple["GSFEncoderTag", ...]:
         return tuple(self._tags)
 
     @property
     def segments(self) -> Mapping[int, "GSFEncoderSegment"]:
-        return frozendict(self._segments)
+        return frozendict(self._segments)  # type: ignore[operator]
 
     def add_tag(self, key: str, value: str):
         """Add a tag to the file"""
         if self._open_encoder is not None:
             raise GSFEncodeAddToActiveDump("Cannot add a new tag to an encoder that is currently dumping")
 
         self._tags.append(GSFEncoderTag(key, value))
```

### Comparing `mediagrains-3.5.1/mediagrains/hypothesis/strategies.py` & `mediagrains-3.5.2/mediagrains/hypothesis/strategies.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/hypothesis/strategies_new.py` & `mediagrains-3.5.2/mediagrains/hypothesis/strategies_new.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/numpy/__init__.py` & `mediagrains-3.5.2/mediagrains/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/numpy/audiograin.py` & `mediagrains-3.5.2/mediagrains/numpy/audiograin.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/numpy/convert.py` & `mediagrains-3.5.2/mediagrains/numpy/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,30 +148,36 @@
 # Colourspace conversions (based on rec.709)
 def _convert_rgb_to_yuv444(grain_in: VideoGrain, grain_out: VideoGrain) -> None:
     bd = COG_FRAME_FORMAT_ACTIVE_BITS(grain_out.format)
     (R, G, B) = (grain_in.component_data.R,
                  grain_in.component_data.G,
                  grain_in.component_data.B)
 
-    np.clip((R*0.2126 + G*0.7152 + B*0.0722), 0, 1 << bd, out=grain_out.component_data.Y)
-    np.clip((R*-0.114572 - G*0.385428 + B*0.5 + (1 << (bd - 1))),
-            0, 1 << bd, out=grain_out.component_data.U)
-    np.clip((R*0.5 - G*0.454153 - B*0.045847 + (1 << (bd - 1))),
-            0, 1 << bd, out=grain_out.component_data.V)
+    # Note that NumPy requires the `unsafe` cast here due to the slight loss of precision in RGB<->YUV conversion
+    np.clip((R*0.2126 + G*0.7152 + B*0.0722),
+            0, 1 << bd, out=grain_out.component_data.Y, casting="unsafe")  # type: ignore
+    np.clip((R*-0.114572 - G*0.385428 + B*0.5 + (1 << (bd - 1))),  # type: ignore
+            0, 1 << bd, out=grain_out.component_data.U, casting="unsafe")
+    np.clip((R*0.5 - G*0.454153 - B*0.045847 + (1 << (bd - 1))),  # type: ignore
+            0, 1 << bd, out=grain_out.component_data.V, casting="unsafe")
 
 
 def _convert_yuv444_to_rgb(grain_in: VideoGrain, grain_out: VideoGrain) -> None:
     bd = COG_FRAME_FORMAT_ACTIVE_BITS(grain_in.format)
     (Y, U, V) = (grain_in.component_data.Y.astype(np.dtype(np.double)),
                  grain_in.component_data.U.astype(np.dtype(np.double)) - (1 << (bd - 1)),
                  grain_in.component_data.V.astype(np.dtype(np.double)) - (1 << (bd - 1)))
 
-    np.clip((Y + V*1.5748), 0, 1 << bd, out=grain_out.component_data.R)
-    np.clip((Y - U*0.187324 - V*0.468124), 0, 1 << bd, out=grain_out.component_data.G)
-    np.clip((Y + U*1.8556), 0, 1 << bd, out=grain_out.component_data.B)
+    # Note that NumPy requires the `unsafe` cast here due to the slight loss of precision in RGB<->YUV conversion
+    np.clip((Y + V*1.5748),
+            0, 1 << bd, out=grain_out.component_data.R, casting="unsafe")  # type: ignore
+    np.clip((Y - U*0.187324 - V*0.468124),
+            0, 1 << bd, out=grain_out.component_data.G, casting="unsafe")  # type: ignore
+    np.clip((Y + U*1.8556),
+            0, 1 << bd, out=grain_out.component_data.B, casting="unsafe")  # type: ignore
 
 
 def _convert_v210_to_yuv422_10bit(grain_in: VideoGrain, grain_out: VideoGrain) -> None:
     # This is a v210 -> planar descramble. It's not super fast, but it should be correct
     #
     # Input data is array of 32-bit words, arranged as a 1d array in repeating blocks of 4 like:
     # lsb ->       ->msb
```

### Comparing `mediagrains-3.5.1/mediagrains/numpy/numpy_grains/AudioGrain.py` & `mediagrains-3.5.2/mediagrains/numpy/numpy_grains/AudioGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/numpy/numpy_grains/VideoGrain.py` & `mediagrains-3.5.2/mediagrains/numpy/numpy_grains/VideoGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/numpy/videograin.py` & `mediagrains-3.5.2/mediagrains/numpy/videograin.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/__init__.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/abc.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/abc.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/audio/__init__.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/audio/abc.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/audio/abc.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/audio/tone.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/audio/tone.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/video/__init__.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/video/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/video/abc.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/video/abc.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/video/colourbars.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/video/colourbars.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/video/constants.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/video/constants.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/video/lumasteps.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/video/lumasteps.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/video/movingbaroverlay.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/video/movingbaroverlay.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/patterngenerators/video/still.py` & `mediagrains-3.5.2/mediagrains/patterngenerators/video/still.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/testsignalgenerator.py` & `mediagrains-3.5.2/mediagrains/testsignalgenerator.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/tools/__init__.py` & `mediagrains-3.5.2/mediagrains/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/tools/_file_or_pipe.py` & `mediagrains-3.5.2/mediagrains/tools/_file_or_pipe.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/tools/extract_from_gsf.py` & `mediagrains-3.5.2/mediagrains/tools/extract_from_gsf.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/tools/wrap_in_gsf.py` & `mediagrains-3.5.2/mediagrains/tools/wrap_in_gsf.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/typing.py` & `mediagrains-3.5.2/mediagrains/typing.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/utils/__init__.py` & `mediagrains-3.5.2/mediagrains/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/utils/adts_aac_grain_wrapper.py` & `mediagrains-3.5.2/mediagrains/utils/adts_aac_grain_wrapper.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/utils/adts_aac_parser.py` & `mediagrains-3.5.2/mediagrains/utils/adts_aac_parser.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/utils/asyncbinaryio.py` & `mediagrains-3.5.2/mediagrains/utils/asyncbinaryio.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/utils/grain_wrapper.py` & `mediagrains-3.5.2/mediagrains/utils/grain_wrapper.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/utils/h264_grain_wrapper.py` & `mediagrains-3.5.2/mediagrains/utils/h264_grain_wrapper.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/utils/h264_parser.py` & `mediagrains-3.5.2/mediagrains/utils/h264_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 
 """H.264 raw bitstream parser"""
 
 from typing import Optional, Dict, Iterator, Iterable, List, Tuple
 from enum import IntEnum
 from itertools import chain
-from bitstring import BitStream, ReadError
+from bitstring import BitStream, ReadError, Bits
 from fractions import Fraction
 
 
 class UnavailableParamSets(ValueError):
     """SPS or PPS referenced by a Slice are not available in the parsed bitstream"""
     pass
 
@@ -431,29 +431,29 @@
         if sps.aspect_ratio_idc == 255:  # extended SAR
             return Fraction(sps.sar_width, sps.sar_height)
         elif sps.aspect_ratio_idc < len(aspect_ratios):
             return Fraction(aspect_ratios[sps.aspect_ratio_idc][0], aspect_ratios[sps.aspect_ratio_idc][1])
         else:
             return None
 
-    def _parse_nal_unit_type(self, bits: BitStream) -> int:
+    def _parse_nal_unit_type(self, bits: Bits) -> int:
         """Peek NALU for NAL Unit Type
 
         :param bits: NALU bits
         :returns: NAL Unit Type
         """
         self._parse_start_code_prefix(bits)
 
         bits.read('uint:1')  # forbidden_zero_bit
         bits.read('uint:2')  # nal_ref_idc
         nal_unit_type = bits.read('uint:5')
 
         return nal_unit_type
 
-    def _parse_sps(self, rbsp_bits: BitStream) -> SPS:
+    def _parse_sps(self, rbsp_bits: Bits) -> SPS:
         """Parse SPS NALU
 
         :param bits: RBSP bits
         :returns: parsed SPS
         :raises ValueError: if a parse failure occurs
         """
         sps = SPS()
@@ -556,15 +556,15 @@
                 sps.time_scale = rbsp_bits.read('uint:32')
                 sps.fixed_frame_rate_flag = rbsp_bits.read('uint:1')
 
         # Ignore the rest
 
         return sps
 
-    def _parse_pps(self, rbsp_bits: BitStream) -> PPS:
+    def _parse_pps(self, rbsp_bits: Bits) -> PPS:
         """Parse PPS NALU
 
         :param bits: RBSP bits
         :returns: parsed PPS
         :raises ValueError: if a parse failure occurs
         """
         pps = PPS()
@@ -609,15 +609,15 @@
         rbsp_bits.read('uint:1')  # constrained_intra_pred_flag
         pps.redundant_pic_cnt_present_flag = rbsp_bits.read('uint:1')
 
         # Ignore the rest
 
         return pps
 
-    def _parse_slice_header(self, rbsp_bits: BitStream) -> SliceHeader:
+    def _parse_slice_header(self, rbsp_bits: Bits) -> SliceHeader:
         """Parse slice header NALU
 
         :param bits: RBSP bits
         :returns: parsed slice header
         :raises ValueError: if a parse failure occurs
         """
         slice_header = SliceHeader()
@@ -659,25 +659,25 @@
         if pps.redundant_pic_cnt_present_flag:
             slice_header.redundant_pic_cnt = rbsp_bits.read('ue')
 
         # Ignore the rest
 
         return slice_header
 
-    def _get_nalu_offsets(self, bits: BitStream) -> Iterator[int]:
+    def _get_nalu_offsets(self, bits: Bits) -> Iterator[int]:
         """Returns a generator of NALU offsets in the frame
 
         The offsets are at the prefix 0x000001.
 
         :param bits: the frame bits
         :returns: a generator of bit offsets
         """
         return bits.findall('0x000001', bytealigned=True)
 
-    def _parse_rbsp_bits(self, bits: BitStream) -> BitStream:
+    def _parse_rbsp_bits(self, bits: Bits) -> Bits:
         """Return raw byte sequence payload that excludes emulation prevention bytes
 
         :param bits: the NALU bits
         :returns: the raw byte sequence payload
         """
         self._parse_start_code_prefix(bits)
         rbsp_start = bits.pos
@@ -691,15 +691,15 @@
         for next_emu_offset in emu_offsets:
             rbsp_bits.append(bits[emu_offset+3*8:next_emu_offset+2*8])
             emu_offset = next_emu_offset
         rbsp_bits.append(bits[emu_offset+3*8:])
 
         return rbsp_bits
 
-    def _parse_start_code_prefix(self, bits: BitStream) -> List[int]:
+    def _parse_start_code_prefix(self, bits: Bits) -> List[int]:
         """Parse the 3 or 4 byte start code prefix
 
         :param bits: the NALU bits
         :returns: the start code prefix bytes
         """
         start_code_prefix = bits.readlist('3*uint:8')  # start code prefix
         if start_code_prefix == [0x00, 0x00, 0x00]:
```

### Comparing `mediagrains-3.5.1/mediagrains/utils/iobytes.py` & `mediagrains-3.5.2/mediagrains/utils/iobytes.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains/utils/synchronise.py` & `mediagrains-3.5.2/mediagrains/utils/synchronise.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/mediagrains.egg-info/SOURCES.txt` & `mediagrains-3.5.2/mediagrains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/setup.py` & `mediagrains-3.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 packages_required = [
     "mediajson >=2.0.0",
     "mediatimestamp >=2.1.0",
     "frozendict >= 1.2",
     'numpy >= 1.23.0',
     'deprecated >= 1.2.6',
-    "bitstring"
+    "bitstring >= 4.0.1",
 ]
 
 console_scripts = [
     'wrap_video_in_gsf=mediagrains.tools:wrap_video_in_gsf',
     'wrap_audio_in_gsf=mediagrains.tools:wrap_audio_in_gsf',
     'extract_gsf_essence=mediagrains.tools:extract_gsf_essence',
     'gsf_probe=mediagrains.tools:gsf_probe'
```

### Comparing `mediagrains-3.5.1/tests/audio_utils.py` & `mediagrains-3.5.2/tests/audio_utils.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/fixtures.py` & `mediagrains-3.5.2/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_adts_aac_parser.py` & `mediagrains-3.5.2/tests/test_adts_aac_parser.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_asyncio_gsf.py` & `mediagrains-3.5.2/tests/test_asyncio_gsf.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_asyncio_gsf_newcode.py` & `mediagrains-3.5.2/tests/test_asyncio_gsf_newcode.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_audio_psnr.py` & `mediagrains-3.5.2/tests/test_audio_psnr.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_audio_psnr_newcode.py` & `mediagrains-3.5.2/tests/test_audio_psnr_newcode.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_comparison.py` & `mediagrains-3.5.2/tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_comparison_newcode.py` & `mediagrains-3.5.2/tests/test_comparison_newcode.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_grain.py` & `mediagrains-3.5.2/tests/test_grain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_grain_newcode.py` & `mediagrains-3.5.2/tests/test_grain_newcode.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_gsf.py` & `mediagrains-3.5.2/tests/test_gsf.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_gsf_newcode.py` & `mediagrains-3.5.2/tests/test_gsf_newcode.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_iobytes.py` & `mediagrains-3.5.2/tests/test_iobytes.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_numpy_audiograin.py` & `mediagrains-3.5.2/tests/test_numpy_audiograin.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_numpy_audiograin_newcode.py` & `mediagrains-3.5.2/tests/test_numpy_audiograin_newcode.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_numpy_videograin.py` & `mediagrains-3.5.2/tests/test_numpy_videograin.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_numpy_videograin_newcode.py` & `mediagrains-3.5.2/tests/test_numpy_videograin_newcode.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_patterngenerators.py` & `mediagrains-3.5.2/tests/test_patterngenerators.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_testsignalgenerator.py` & `mediagrains-3.5.2/tests/test_testsignalgenerator.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_video_psnr.py` & `mediagrains-3.5.2/tests/test_video_psnr.py`

 * *Files identical despite different names*

### Comparing `mediagrains-3.5.1/tests/test_video_psnr_newcode.py` & `mediagrains-3.5.2/tests/test_video_psnr_newcode.py`

 * *Files identical despite different names*

