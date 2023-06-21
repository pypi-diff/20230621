# Comparing `tmp/skelly_synchronize-2023.6.1018.tar.gz` & `tmp/skelly_synchronize-2023.6.1019.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_synchronize-2023.6.1018.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skelly_synchronize-2023.6.1019.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skelly_synchronize-2023.6.1018.tar` & `skelly_synchronize-2023.6.1019.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0       65 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/.gitattributes
--rw-r--r--   0        0        0      146 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/.github/workflows/lint-with-black.yml
--rw-r--r--   0        0        0     1087 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1025 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2783 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/.gitignore
--rw-r--r--   0        0        0    34523 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/LICENSE
--rw-r--r--   0        0        0     3030 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/README.md
--rw-r--r--   0        0        0     1639 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/requirements.txt
--rw-r--r--   0        0        0       50 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/setup.py
--rw-r--r--   0        0        0     1056 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/__init__.py
--rw-r--r--   0        0        0      333 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/__main__.py
--rw-r--r--   0        0        0     3401 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/audio_utilities.py
--rw-r--r--   0        0        0     2758 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/correlation_functions.py
--rw-r--r--   0        0        0      616 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/debugging/debug_output.py
--rw-r--r--   0        0        0     2136 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/debugging/debug_plots.py
--rw-r--r--   0        0        0     1557 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
--rw-r--r--   0        0        0     3438 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
--rw-r--r--   0        0        0     5993 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/video_functions/video_utilities.py
--rw-r--r--   0        0        0     1873 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/gui/skelly_synchronize_gui.py
--rw-r--r--   0        0        0      420 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/gui/widgets/run_button_widget.py
--rw-r--r--   0        0        0     5326 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/skelly_synchronize.py
--rw-r--r--   0        0        0        0 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/system/__init__.py
--rw-r--r--   0        0        0     1479 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/system/default_paths.py
--rw-r--r--   0        0        0     1402 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/system/logging_configuration.py
--rw-r--r--   0        0        0      599 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/system/paths_and_file_names.py
--rw-r--r--   0        0        0     1085 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/conftest.py
--rw-r--r--   0        0        0      656 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/test_normalize_lag_dict.py
--rw-r--r--   0        0        0      847 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/test_trim_single_video_deffcode.py
--rw-r--r--   0        0        0      577 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
--rw-r--r--   0        0        0      262 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
--rw-r--r--   0        0        0     1263 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0     1061 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/load_sample_data.py
--rw-r--r--   0        0        0     2048 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
--rw-r--r--   0        0        0     1348 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/utils/get_video_files.py
--rw-r--r--   0        0        0     1103 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/utils/path_handling_utilities.py
--rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 skelly_synchronize-2023.6.1018/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/.gitattributes
+-rw-r--r--   0        0        0      146 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/.github/workflows/lint-with-black.yml
+-rw-r--r--   0        0        0     1087 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1025 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2783 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/.gitignore
+-rw-r--r--   0        0        0    34523 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/LICENSE
+-rw-r--r--   0        0        0     3030 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/README.md
+-rw-r--r--   0        0        0     1639 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/requirements.txt
+-rw-r--r--   0        0        0       50 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/setup.py
+-rw-r--r--   0        0        0     1056 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/__init__.py
+-rw-r--r--   0        0        0      333 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/__main__.py
+-rw-r--r--   0        0        0     3401 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/audio_utilities.py
+-rw-r--r--   0        0        0     2758 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/correlation_functions.py
+-rw-r--r--   0        0        0      616 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/debugging/debug_output.py
+-rw-r--r--   0        0        0     2136 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/debugging/debug_plots.py
+-rw-r--r--   0        0        0     1557 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
+-rw-r--r--   0        0        0     3438 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
+-rw-r--r--   0        0        0     5993 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/video_functions/video_utilities.py
+-rw-r--r--   0        0        0     1873 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/gui/skelly_synchronize_gui.py
+-rw-r--r--   0        0        0      420 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/gui/widgets/run_button_widget.py
+-rw-r--r--   0        0        0     5389 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/skelly_synchronize.py
+-rw-r--r--   0        0        0        0 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/system/__init__.py
+-rw-r--r--   0        0        0     1479 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/system/default_paths.py
+-rw-r--r--   0        0        0     1402 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/system/logging_configuration.py
+-rw-r--r--   0        0        0      646 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/system/paths_and_file_names.py
+-rw-r--r--   0        0        0     1487 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/tests/conftest.py
+-rw-r--r--   0        0        0     1593 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/tests/test_all_files_created.py
+-rw-r--r--   0        0        0      656 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/tests/test_normalize_lag_dict.py
+-rw-r--r--   0        0        0      522 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/tests/test_number_of_videos_is_preserved.py
+-rw-r--r--   0        0        0      847 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/tests/test_trim_single_video_deffcode.py
+-rw-r--r--   0        0        0      712 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/tests/test_videos_are_same_length.py
+-rw-r--r--   0        0        0      577 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
+-rw-r--r--   0        0        0      262 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
+-rw-r--r--   0        0        0     1263 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0     1044 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/tests/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     2048 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
+-rw-r--r--   0        0        0     1348 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/utils/get_video_files.py
+-rw-r--r--   0        0        0     1103 2023-06-21 19:17:50.777538 skelly_synchronize-2023.6.1019/skelly_synchronize/utils/path_handling_utilities.py
+-rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 skelly_synchronize-2023.6.1019/PKG-INFO
```

### Comparing `skelly_synchronize-2023.6.1018/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_synchronize-2023.6.1019/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/.github/workflows/python-testing.yml` & `skelly_synchronize-2023.6.1019/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/.gitignore` & `skelly_synchronize-2023.6.1019/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/LICENSE` & `skelly_synchronize-2023.6.1019/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/README.md` & `skelly_synchronize-2023.6.1019/README.md`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/pyproject.toml` & `skelly_synchronize-2023.6.1019/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.06.1018"
+current_version = "v2023.06.1019"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/__init__.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_synchronize"
-__version__ = "v2023.06.1018"
+__version__ = "v2023.06.1019"
 
 __author__ = """Philip Queen"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
```

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/audio_utilities.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/correlation_functions.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/correlation_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/debugging/debug_output.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/debugging/debug_output.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/debugging/debug_plots.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/debugging/debug_plots.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/video_functions/deffcode_functions.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/video_functions/deffcode_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/video_functions/video_utilities.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/core_processes/video_functions/video_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/gui/skelly_synchronize_gui.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/gui/skelly_synchronize_gui.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/skelly_synchronize.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/skelly_synchronize.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     synchronized_video_folder_path: Path = None,
     file_type: str = ".mp4",
     video_handler: str = "deffcode",
 ):
     """Run the functions from the VideoSynchronize class to synchronize all videos with the given file type in the base path folder.
     Uses deffcode and to handle the video files as default, set "video_handler" to "ffmpeg" to use ffmpeg methods instead.
     ffmpeg is used to get audio from the video files with either method.
+
+    Returns the folder path of the synchronized video folder.
     """
     start_timer = time.time()
 
     video_file_list = get_video_file_list(
         folder_path=raw_video_folder_path, file_type=file_type
     )
     if synchronized_video_folder_path is None:
```

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/system/default_paths.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/system/logging_configuration.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/system/paths_and_file_names.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/system/paths_and_file_names.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # directory names
 SYNCHRONIZED_VIDEOS_FOLDER_NAME = "synchronized_videos"
+RAW_VIDEOS_FOLDER_NAME = "raw_videos"
 AUDIO_FILES_FOLDER_NAME = "audio_files"
 TRIMMED_AUDIO_FOLDER_NAME = "trimmed_audio"
 
 # file names
 DEBUG_TOML_NAME = "synchronization_debug.toml"
 DEBUG_PLOT_NAME = "debug_plot.png"
 
 # debug dictionary keys
 RAW_VIDEO_NAME = "Raw_video_information"
 SYNCHRONIZED_VIDEO_NAME = "Synchronized_video_information"
 AUDIO_NAME = "Audio_information"
 LAG_DICTIONARY_NAME = "Lag_dictionary"
 
 # figshare info
-FIGSHARE_ZIP_FILE_URL = "https://figshare.com/ndownloader/files/40293973"
-FIGSHARE_SAMPLE_DATA_FILE_NAME = "freemocap_sample_data"
+FIGSHARE_ZIP_FILE_URL = "https://figshare.com/ndownloader/files/41066489"
+FIGSHARE_SAMPLE_DATA_FILE_NAME = "skelly_synchronize_sample_data"
```

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/conftest.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 import sys
 import pytest
 from pathlib import Path
 
-
 print(f"Thank you for using skelly_synchronize!")
 print(f"This is printing from: {__file__}")
 
 base_package_path = Path(__file__).parent.parent.parent
 print(f"adding base_package_path: {base_package_path} : to sys.path")
 sys.path.insert(0, str(base_package_path))  # add parent directory to sys.path
 
+from skelly_synchronize.skelly_synchronize import synchronize_videos_from_audio
 from skelly_synchronize.tests.utilities.load_sample_data import (
-    find_synchronized_videos_folder_path,
+    find_raw_videos_folder_path,
     load_sample_data,
 )
 from skelly_synchronize.utils.get_video_files import get_video_file_list
 
 
 def pytest_sessionstart():
     pytest.sample_session_folder_path = load_sample_data()
-    video_folder_path = find_synchronized_videos_folder_path(
+    pytest.raw_video_folder_path = find_raw_videos_folder_path(
         pytest.sample_session_folder_path
     )
+    pytest.synchronized_video_folder_path = synchronize_videos_from_audio(
+        pytest.raw_video_folder_path
+    )
     pytest.video_file_list = get_video_file_list(
-        folder_path=video_folder_path, file_type=".mp4"
+        folder_path=pytest.synchronized_video_folder_path, file_type=".mp4"
     )
 
 
 @pytest.fixture
+def raw_video_folder_path():
+    return pytest.raw_video_folder_path
+
+
+@pytest.fixture
+def synchronized_video_folder_path():
+    return pytest.synchronized_video_folder_path
+
+
+@pytest.fixture
 def test_video_pathstring():
     return str(pytest.video_file_list[0])
 
 
 @pytest.fixture
 def output_video_pathstring():
     return str(pytest.sample_session_folder_path / "trimmed_sample_video.mp4")
```

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/test_normalize_lag_dict.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/tests/test_normalize_lag_dict.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/test_trim_single_video_deffcode.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/tests/test_trim_single_video_deffcode.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/check_list_values_are_equal.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/tests/utilities/check_list_values_are_equal.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/load_sample_data.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/tests/utilities/load_sample_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 import requests
 import zipfile
 from pathlib import Path
 
 from skelly_synchronize.system.paths_and_file_names import (
     FIGSHARE_SAMPLE_DATA_FILE_NAME,
     FIGSHARE_ZIP_FILE_URL,
-    SYNCHRONIZED_VIDEOS_FOLDER_NAME,
+    RAW_VIDEOS_FOLDER_NAME,
 )
 
 
 def load_sample_data() -> Path:
     extract_to_path = Path.home()
     extract_to_path.mkdir(exist_ok=True)
 
     figshare_sample_data_path = extract_to_path / FIGSHARE_SAMPLE_DATA_FILE_NAME
 
     if not Path.exists(figshare_sample_data_path):
         r = requests.get(FIGSHARE_ZIP_FILE_URL)
         z = zipfile.ZipFile(io.BytesIO(r.content))
-        z.extractall(extract_to_path)
+        z.extractall(figshare_sample_data_path)
 
     return figshare_sample_data_path
 
 
-def find_synchronized_videos_folder_path(session_folder_path: Path) -> Path:
+def find_raw_videos_folder_path(session_folder_path: Path) -> Path:
     for subfolder_path in session_folder_path.iterdir():
-        if subfolder_path.name == SYNCHRONIZED_VIDEOS_FOLDER_NAME:
+        if subfolder_path.name == RAW_VIDEOS_FOLDER_NAME:
             return subfolder_path
 
     raise Exception(
         f"Could not find a videos folder in path {str(session_folder_path)}"
     )
```

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/utils/get_video_files.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/utils/get_video_files.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/skelly_synchronize/utils/path_handling_utilities.py` & `skelly_synchronize-2023.6.1019/skelly_synchronize/utils/path_handling_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1018/PKG-INFO` & `skelly_synchronize-2023.6.1019/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_synchronize
-Version: 2023.6.1018
+Version: 2023.6.1019
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skelly_synchronize <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
```

