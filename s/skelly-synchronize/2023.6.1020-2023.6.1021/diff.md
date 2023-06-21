# Comparing `tmp/skelly_synchronize-2023.6.1020.tar.gz` & `tmp/skelly_synchronize-2023.6.1021.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_synchronize-2023.6.1020.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skelly_synchronize-2023.6.1021.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skelly_synchronize-2023.6.1020.tar` & `skelly_synchronize-2023.6.1021.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0       65 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/.gitattributes
--rw-r--r--   0        0        0      146 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/.github/workflows/lint-with-black.yml
--rw-r--r--   0        0        0     1087 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1025 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2783 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/.gitignore
--rw-r--r--   0        0        0    34523 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/LICENSE
--rw-r--r--   0        0        0     3030 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/README.md
--rw-r--r--   0        0        0     1646 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/pyproject.toml
--rw-r--r--   0        0        0      162 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/requirements.txt
--rw-r--r--   0        0        0       50 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/setup.py
--rw-r--r--   0        0        0     1056 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/skelly_synchronize/__init__.py
--rw-r--r--   0        0        0      333 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/skelly_synchronize/__main__.py
--rw-r--r--   0        0        0     3401 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/audio_utilities.py
--rw-r--r--   0        0        0     2758 2023-06-21 19:18:18.651880 skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/correlation_functions.py
--rw-r--r--   0        0        0      616 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/debugging/debug_output.py
--rw-r--r--   0        0        0     3015 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/debugging/debug_plots.py
--rw-r--r--   0        0        0     1558 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
--rw-r--r--   0        0        0     3438 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
--rw-r--r--   0        0        0     5993 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/video_functions/video_utilities.py
--rw-r--r--   0        0        0     1873 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/gui/skelly_synchronize_gui.py
--rw-r--r--   0        0        0      420 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/gui/widgets/run_button_widget.py
--rw-r--r--   0        0        0     5488 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/skelly_synchronize.py
--rw-r--r--   0        0        0        0 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/system/__init__.py
--rw-r--r--   0        0        0     1479 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/system/default_paths.py
--rw-r--r--   0        0        0     1402 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/system/logging_configuration.py
--rw-r--r--   0        0        0      646 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/system/paths_and_file_names.py
--rw-r--r--   0        0        0     1487 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/tests/conftest.py
--rw-r--r--   0        0        0     1593 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/tests/test_all_files_created.py
--rw-r--r--   0        0        0      656 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/tests/test_normalize_lag_dict.py
--rw-r--r--   0        0        0      522 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/tests/test_number_of_videos_is_preserved.py
--rw-r--r--   0        0        0      847 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/tests/test_trim_single_video_deffcode.py
--rw-r--r--   0        0        0      712 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/tests/test_videos_are_same_length.py
--rw-r--r--   0        0        0      577 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
--rw-r--r--   0        0        0      262 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
--rw-r--r--   0        0        0     1263 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0     1044 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/tests/utilities/load_sample_data.py
--rw-r--r--   0        0        0     2048 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
--rw-r--r--   0        0        0     1348 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/utils/get_video_files.py
--rw-r--r--   0        0        0     1103 2023-06-21 19:18:18.655880 skelly_synchronize-2023.6.1020/skelly_synchronize/utils/path_handling_utilities.py
--rw-r--r--   0        0        0     3980 1970-01-01 00:00:00.000000 skelly_synchronize-2023.6.1020/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/.gitattributes
+-rw-r--r--   0        0        0      146 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/.github/workflows/lint-with-black.yml
+-rw-r--r--   0        0        0     1087 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1010 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2783 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/.gitignore
+-rw-r--r--   0        0        0    34523 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/LICENSE
+-rw-r--r--   0        0        0     3030 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/README.md
+-rw-r--r--   0        0        0     1646 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/setup.py
+-rw-r--r--   0        0        0     1056 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/__init__.py
+-rw-r--r--   0        0        0      333 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/__main__.py
+-rw-r--r--   0        0        0     3401 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/audio_utilities.py
+-rw-r--r--   0        0        0     2758 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/correlation_functions.py
+-rw-r--r--   0        0        0      616 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/debugging/debug_output.py
+-rw-r--r--   0        0        0     3015 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/debugging/debug_plots.py
+-rw-r--r--   0        0        0     1558 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
+-rw-r--r--   0        0        0     3438 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
+-rw-r--r--   0        0        0     5993 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/video_utilities.py
+-rw-r--r--   0        0        0     1873 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/gui/skelly_synchronize_gui.py
+-rw-r--r--   0        0        0      420 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/gui/widgets/run_button_widget.py
+-rw-r--r--   0        0        0     5488 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/skelly_synchronize.py
+-rw-r--r--   0        0        0        0 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/system/__init__.py
+-rw-r--r--   0        0        0     1479 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/system/default_paths.py
+-rw-r--r--   0        0        0     1402 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/system/logging_configuration.py
+-rw-r--r--   0        0        0      646 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/system/paths_and_file_names.py
+-rw-r--r--   0        0        0     1487 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/conftest.py
+-rw-r--r--   0        0        0     1593 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_all_files_created.py
+-rw-r--r--   0        0        0      656 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_normalize_lag_dict.py
+-rw-r--r--   0        0        0      522 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_number_of_videos_is_preserved.py
+-rw-r--r--   0        0        0      847 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_trim_single_video_deffcode.py
+-rw-r--r--   0        0        0      712 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_videos_are_same_length.py
+-rw-r--r--   0        0        0      577 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
+-rw-r--r--   0        0        0      262 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
+-rw-r--r--   0        0        0     1263 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0     1044 2023-06-21 19:45:06.654786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     1853 2023-06-21 19:45:06.654786 skelly_synchronize-2023.6.1021/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
+-rw-r--r--   0        0        0     1348 2023-06-21 19:45:06.654786 skelly_synchronize-2023.6.1021/skelly_synchronize/utils/get_video_files.py
+-rw-r--r--   0        0        0     1103 2023-06-21 19:45:06.654786 skelly_synchronize-2023.6.1021/skelly_synchronize/utils/path_handling_utilities.py
+-rw-r--r--   0        0        0     3980 1970-01-01 00:00:00.000000 skelly_synchronize-2023.6.1021/PKG-INFO
```

### Comparing `skelly_synchronize-2023.6.1020/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_synchronize-2023.6.1021/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/.github/workflows/python-testing.yml` & `skelly_synchronize-2023.6.1021/.github/workflows/python-testing.yml`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,15 @@
           python-version: '3.9'
           # Optional - x64 or x86 architecture, defaults to x64
           architecture: 'x64'
           cache: 'pip'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -r requirements.txt
+          pip install -e .
       - name: Install FFmpeg
         run: |
           sudo apt-get update
           sudo apt-get install -y ffmpeg
       - name: Run tests with pytest
         run: |
           pip install pytest
```

### Comparing `skelly_synchronize-2023.6.1020/.gitignore` & `skelly_synchronize-2023.6.1021/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/LICENSE` & `skelly_synchronize-2023.6.1021/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/README.md` & `skelly_synchronize-2023.6.1021/README.md`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/pyproject.toml` & `skelly_synchronize-2023.6.1021/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.06.1020"
+current_version = "v2023.06.1021"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/__init__.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_synchronize"
-__version__ = "v2023.06.1020"
+__version__ = "v2023.06.1021"
 
 __author__ = """Philip Queen"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
```

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/audio_utilities.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/correlation_functions.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/correlation_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/debugging/debug_output.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/debugging/debug_output.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/debugging/debug_plots.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/debugging/debug_plots.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/video_functions/deffcode_functions.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/deffcode_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/core_processes/video_functions/video_utilities.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/video_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/gui/skelly_synchronize_gui.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/gui/skelly_synchronize_gui.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/skelly_synchronize.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/skelly_synchronize.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/system/default_paths.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/system/logging_configuration.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/system/paths_and_file_names.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/system/paths_and_file_names.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/tests/conftest.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/tests/test_all_files_created.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_all_files_created.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/tests/test_normalize_lag_dict.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_normalize_lag_dict.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/tests/test_number_of_videos_is_preserved.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_number_of_videos_is_preserved.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/tests/test_trim_single_video_deffcode.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_trim_single_video_deffcode.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/tests/test_videos_are_same_length.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_videos_are_same_length.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/tests/utilities/check_list_values_are_equal.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/check_list_values_are_equal.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/tests/utilities/load_sample_data.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/load_sample_data.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,19 +28,14 @@
     sourcer = Sourcer(video_pathstring).probe_stream()
 
     metadata_dictionary = sourcer.retrieve_metadata()
 
     deffcode_width = metadata_dictionary["source_video_resolution"][0]
     deffcode_height = metadata_dictionary["source_video_resolution"][1]
 
-    logging.info(f"opencv width is {opencv_width}, opencv height is {opencv_height}")
-    logging.info(
-        f"deffcode width is {deffcode_width}, deffcode height is {deffcode_height}"
-    )
-
     if (opencv_width != deffcode_width) & (opencv_height != deffcode_height):
         return True
     else:
         return False
 
 
 if __name__ == "__main__":
```

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/utils/get_video_files.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/utils/get_video_files.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/skelly_synchronize/utils/path_handling_utilities.py` & `skelly_synchronize-2023.6.1021/skelly_synchronize/utils/path_handling_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1020/PKG-INFO` & `skelly_synchronize-2023.6.1021/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_synchronize
-Version: 2023.6.1020
+Version: 2023.6.1021
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skelly_synchronize <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
```

