# Comparing `tmp/aidentified-matching-api-1.1.3.tar.gz` & `tmp/aidentified-matching-api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aidentified-matching-api-1.1.3.tar", last modified: Wed Mar 29 12:39:33 2023, max compression
+gzip compressed data, was "aidentified-matching-api-1.2.0.tar", last modified: Wed Jun 21 16:58:48 2023, max compression
```

## Comparing `aidentified-matching-api-1.1.3.tar` & `aidentified-matching-api-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 david      (502) staff       (20)        0 2023-03-29 12:39:33.653211 aidentified-matching-api-1.1.3/
--rw-r--r--   0 david      (502) staff       (20)    11358 2022-02-16 18:15:20.000000 aidentified-matching-api-1.1.3/LICENSE
--rw-r--r--   0 david      (502) staff       (20)       24 2022-02-16 18:15:20.000000 aidentified-matching-api-1.1.3/MANIFEST.in
--rw-r--r--   0 david      (502) staff       (20)      224 2023-03-29 12:39:33.652742 aidentified-matching-api-1.1.3/PKG-INFO
--rw-r--r--   0 david      (502) staff       (20)    10637 2022-03-03 15:14:55.000000 aidentified-matching-api-1.1.3/README.md
-drwxr-xr-x   0 david      (502) staff       (20)        0 2023-03-29 12:39:33.647522 aidentified-matching-api-1.1.3/aidentified_matching_api/
--rw-r--r--   0 david      (502) staff       (20)    10639 2022-10-25 22:37:50.000000 aidentified-matching-api-1.1.3/aidentified_matching_api/__init__.py
--rw-r--r--   0 david      (502) staff       (20)      917 2022-08-24 18:08:14.000000 aidentified-matching-api-1.1.3/aidentified_matching_api/constants.py
--rw-r--r--   0 david      (502) staff       (20)     2080 2022-02-16 18:15:20.000000 aidentified-matching-api-1.1.3/aidentified_matching_api/daily_files.py
--rw-r--r--   0 david      (502) staff       (20)     1403 2022-02-16 18:15:20.000000 aidentified-matching-api-1.1.3/aidentified_matching_api/dataset.py
--rw-r--r--   0 david      (502) staff       (20)     9256 2023-03-29 12:34:13.000000 aidentified-matching-api-1.1.3/aidentified_matching_api/dataset_file.py
--rw-r--r--   0 david      (502) staff       (20)     1508 2022-02-16 18:15:20.000000 aidentified-matching-api-1.1.3/aidentified_matching_api/get_id.py
--rw-r--r--   0 david      (502) staff       (20)     5250 2022-02-16 18:15:20.000000 aidentified-matching-api-1.1.3/aidentified_matching_api/token_service.py
--rw-r--r--   0 david      (502) staff       (20)     6428 2022-10-03 15:18:41.000000 aidentified-matching-api-1.1.3/aidentified_matching_api/validation.py
-drwxr-xr-x   0 david      (502) staff       (20)        0 2023-03-29 12:39:33.651209 aidentified-matching-api-1.1.3/aidentified_matching_api.egg-info/
--rw-r--r--   0 david      (502) staff       (20)      224 2023-03-29 12:39:33.000000 aidentified-matching-api-1.1.3/aidentified_matching_api.egg-info/PKG-INFO
--rw-r--r--   0 david      (502) staff       (20)      677 2023-03-29 12:39:33.000000 aidentified-matching-api-1.1.3/aidentified_matching_api.egg-info/SOURCES.txt
--rw-r--r--   0 david      (502) staff       (20)        1 2023-03-29 12:39:33.000000 aidentified-matching-api-1.1.3/aidentified_matching_api.egg-info/dependency_links.txt
--rw-r--r--   0 david      (502) staff       (20)       68 2023-03-29 12:39:33.000000 aidentified-matching-api-1.1.3/aidentified_matching_api.egg-info/entry_points.txt
--rw-r--r--   0 david      (502) staff       (20)       27 2023-03-29 12:39:33.000000 aidentified-matching-api-1.1.3/aidentified_matching_api.egg-info/requires.txt
--rw-r--r--   0 david      (502) staff       (20)       25 2023-03-29 12:39:33.000000 aidentified-matching-api-1.1.3/aidentified_matching_api.egg-info/top_level.txt
--rw-r--r--   0 david      (502) staff       (20)       27 2022-02-16 18:15:20.000000 aidentified-matching-api-1.1.3/requirements.in
--rw-r--r--   0 david      (502) staff       (20)       38 2023-03-29 12:39:33.653415 aidentified-matching-api-1.1.3/setup.cfg
--rw-r--r--   0 david      (502) staff       (20)     1322 2023-03-29 12:35:12.000000 aidentified-matching-api-1.1.3/setup.py
-drwxr-xr-x   0 david      (502) staff       (20)        0 2023-03-29 12:39:33.651919 aidentified-matching-api-1.1.3/tests/
--rw-r--r--   0 david      (502) staff       (20)     3358 2022-10-03 15:18:41.000000 aidentified-matching-api-1.1.3/tests/test_validation.py
+drwxr-xr-x   0 david      (502) staff       (20)        0 2023-06-21 16:58:48.069771 aidentified-matching-api-1.2.0/
+-rw-r--r--   0 david      (502) staff       (20)    11358 2022-02-16 18:15:20.000000 aidentified-matching-api-1.2.0/LICENSE
+-rw-r--r--   0 david      (502) staff       (20)       24 2022-02-16 18:15:20.000000 aidentified-matching-api-1.2.0/MANIFEST.in
+-rw-r--r--   0 david      (502) staff       (20)      224 2023-06-21 16:58:48.069337 aidentified-matching-api-1.2.0/PKG-INFO
+-rw-r--r--   0 david      (502) staff       (20)    10637 2022-03-03 15:14:55.000000 aidentified-matching-api-1.2.0/README.md
+drwxr-xr-x   0 david      (502) staff       (20)        0 2023-06-21 16:58:48.065379 aidentified-matching-api-1.2.0/aidentified_matching_api/
+-rw-r--r--   0 david      (502) staff       (20)    11075 2023-06-13 19:04:32.000000 aidentified-matching-api-1.2.0/aidentified_matching_api/__init__.py
+-rw-r--r--   0 david      (502) staff       (20)      917 2022-08-24 18:08:14.000000 aidentified-matching-api-1.2.0/aidentified_matching_api/constants.py
+-rw-r--r--   0 david      (502) staff       (20)     2080 2022-02-16 18:15:20.000000 aidentified-matching-api-1.2.0/aidentified_matching_api/daily_files.py
+-rw-r--r--   0 david      (502) staff       (20)     1403 2022-02-16 18:15:20.000000 aidentified-matching-api-1.2.0/aidentified_matching_api/dataset.py
+-rw-r--r--   0 david      (502) staff       (20)     9482 2023-06-21 16:58:10.000000 aidentified-matching-api-1.2.0/aidentified_matching_api/dataset_file.py
+-rw-r--r--   0 david      (502) staff       (20)     1618 2023-06-21 16:58:10.000000 aidentified-matching-api-1.2.0/aidentified_matching_api/get_id.py
+-rw-r--r--   0 david      (502) staff       (20)     5250 2022-02-16 18:15:20.000000 aidentified-matching-api-1.2.0/aidentified_matching_api/token_service.py
+-rw-r--r--   0 david      (502) staff       (20)     8901 2023-06-21 16:58:10.000000 aidentified-matching-api-1.2.0/aidentified_matching_api/validation.py
+drwxr-xr-x   0 david      (502) staff       (20)        0 2023-06-21 16:58:48.068009 aidentified-matching-api-1.2.0/aidentified_matching_api.egg-info/
+-rw-r--r--   0 david      (502) staff       (20)      224 2023-06-21 16:58:48.000000 aidentified-matching-api-1.2.0/aidentified_matching_api.egg-info/PKG-INFO
+-rw-r--r--   0 david      (502) staff       (20)      677 2023-06-21 16:58:48.000000 aidentified-matching-api-1.2.0/aidentified_matching_api.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (502) staff       (20)        1 2023-06-21 16:58:48.000000 aidentified-matching-api-1.2.0/aidentified_matching_api.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (502) staff       (20)       68 2023-06-21 16:58:48.000000 aidentified-matching-api-1.2.0/aidentified_matching_api.egg-info/entry_points.txt
+-rw-r--r--   0 david      (502) staff       (20)       27 2023-06-21 16:58:48.000000 aidentified-matching-api-1.2.0/aidentified_matching_api.egg-info/requires.txt
+-rw-r--r--   0 david      (502) staff       (20)       25 2023-06-21 16:58:48.000000 aidentified-matching-api-1.2.0/aidentified_matching_api.egg-info/top_level.txt
+-rw-r--r--   0 david      (502) staff       (20)       27 2022-02-16 18:15:20.000000 aidentified-matching-api-1.2.0/requirements.in
+-rw-r--r--   0 david      (502) staff       (20)       38 2023-06-21 16:58:48.069948 aidentified-matching-api-1.2.0/setup.cfg
+-rw-r--r--   0 david      (502) staff       (20)     1322 2023-06-21 16:58:10.000000 aidentified-matching-api-1.2.0/setup.py
+drwxr-xr-x   0 david      (502) staff       (20)        0 2023-06-21 16:58:48.068450 aidentified-matching-api-1.2.0/tests/
+-rw-r--r--   0 david      (502) staff       (20)     5010 2023-06-14 16:52:30.000000 aidentified-matching-api-1.2.0/tests/test_validation.py
```

### Comparing `aidentified-matching-api-1.1.3/LICENSE` & `aidentified-matching-api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aidentified-matching-api-1.1.3/README.md` & `aidentified-matching-api-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aidentified-matching-api-1.1.3/aidentified_matching_api/__init__.py` & `aidentified-matching-api-1.2.0/aidentified_matching_api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,16 +60,18 @@
 #
 
 dataset_parser = subparser.add_parser("dataset", help="Manage datasets")
 dataset_subparser = dataset_parser.add_subparsers()
 
 
 _dataset_parent = argparse.ArgumentParser(add_help=False)
-_dataset_parent_group = _dataset_parent.add_argument_group(title="required arguments")
-_dataset_parent_group.add_argument("--name", help="Dataset name", required=True)
+_dataset_parent_arg_group = _dataset_parent.add_argument_group(
+    title="required arguments"
+)
+_dataset_parent_arg_group.add_argument("--name", help="Dataset name", required=True)
 
 dataset_list = dataset_subparser.add_parser("list", help="List datasets")
 dataset_list.set_defaults(func=dataset.list_datasets)
 
 dataset_create = dataset_subparser.add_parser(
     "create", help="Create new dataset", parents=[_dataset_parent]
 )
@@ -196,52 +198,63 @@
 dataset_file_list.set_defaults(func=dataset_file.list_dataset_files)
 
 dataset_file_create = dataset_files_subparser.add_parser(
     "create",
     help="Create new dataset file",
     parents=[_get_dataset_file_parent(dataset_file_name=True)],
 )
+dataset_file_create.add_argument(
+    "--include-households",
+    help="Add household members of matches to output",
+    action="store_true",
+)
+dataset_file_create.add_argument(
+    "--match-logic",
+    help="Choose matching technique. See API documentation for details. Default is OPPORTUNISTIC",
+    choices=["OPPORTUNISTIC", "ADDRESS", "EMAIL"],
+    default="OPPORTUNISTIC",
+)
 dataset_file_create.set_defaults(func=dataset_file.create_dataset_file)
 
-dataset_file_create = dataset_files_subparser.add_parser(
+dataset_file_upload_group = dataset_files_subparser.add_parser(
     "upload",
     help="Upload dataset file",
     parents=[
         _get_dataset_file_parent(
             dataset_file_name=True, dataset_file_upload=True, validation=True
         )
     ],
 )
-dataset_file_create.add_argument(
+dataset_file_upload_group.add_argument(
     "--upload-part-size",
     help="Size of upload chunk in megabytes",
     type=int,
     default=100,
 )
-dataset_file_create.add_argument(
+dataset_file_upload_group.add_argument(
     "--concurrent-uploads", help="Max number of concurrent uploads", type=int, default=4
 )
-dataset_file_create.set_defaults(func=dataset_file.upload_dataset_file)
-dataset_file_create.set_defaults(upload_dataset_file_lock=threading.Lock())
+dataset_file_upload_group.set_defaults(func=dataset_file.upload_dataset_file)
+dataset_file_upload_group.set_defaults(upload_dataset_file_lock=threading.Lock())
 
 dataset_file_abort = dataset_files_subparser.add_parser(
     "abort",
     help="Abort dataset file upload",
     parents=[_get_dataset_file_parent(dataset_file_name=True)],
 )
 dataset_file_abort.set_defaults(func=dataset_file.abort_dataset_file)
 
-dataset_file_download = dataset_files_subparser.add_parser(
+dataset_file_download_group = dataset_files_subparser.add_parser(
     "download",
     help="Download matched dataset file",
     parents=[
         _get_dataset_file_parent(dataset_file_name=True, dataset_file_download=True)
     ],
 )
-dataset_file_download.set_defaults(func=dataset_file.download_dataset_file)
+dataset_file_download_group.set_defaults(func=dataset_file.download_dataset_file)
 
 
 dataset_file_delete = dataset_files_subparser.add_parser(
     "delete",
     help="Delete dataset file",
     parents=[_get_dataset_file_parent(dataset_file_name=True)],
 )
```

### Comparing `aidentified-matching-api-1.1.3/aidentified_matching_api/constants.py` & `aidentified-matching-api-1.2.0/aidentified_matching_api/constants.py`

 * *Files identical despite different names*

### Comparing `aidentified-matching-api-1.1.3/aidentified_matching_api/daily_files.py` & `aidentified-matching-api-1.2.0/aidentified_matching_api/daily_files.py`

 * *Files identical despite different names*

### Comparing `aidentified-matching-api-1.1.3/aidentified_matching_api/dataset.py` & `aidentified-matching-api-1.2.0/aidentified_matching_api/dataset.py`

 * *Files identical despite different names*

### Comparing `aidentified-matching-api-1.1.3/aidentified_matching_api/dataset_file.py` & `aidentified-matching-api-1.2.0/aidentified_matching_api/dataset_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,20 @@
     constants.pretty(resp_obj)
 
 
 def create_dataset_file(args):
     # create files under name.
     dataset_id = get_id.get_dataset_id_from_dataset_name(args)
 
-    dataset_file_payload = {"dataset_id": dataset_id, "name": args.dataset_file_name}
+    dataset_file_payload = {
+        "dataset_id": dataset_id,
+        "name": args.dataset_file_name,
+        "include_households": args.include_households,
+        "match_logic": args.match_logic,
+    }
     resp_obj = token.token_service.api_call(
         args, requests.post, "/v1/dataset-file/", json=dataset_file_payload
     )
 
     constants.pretty(resp_obj)
 
 
@@ -235,20 +240,22 @@
         raise Exception(f"Error(s) while uploading file: {exc_strings}")
 
 
 def upload_dataset_file(args):
     if args.upload_part_size < 5:
         raise Exception("--upload-part-size must be greater than 5 Mb")
 
+    dataset_file = get_id.get_dataset_file_from_dataset_file_name(args)
+    dataset_file_id = dataset_file["dataset_file_id"]
+    match_logic = dataset_file["match_logic"]
+
     logger.info("Starting validation")
-    csv_args = validation.validate(args)
+    csv_args = validation.validate(args, match_logic)
     logger.info("Validation complete")
 
-    dataset_file_id = get_id.get_dataset_file_id_from_dataset_file_name(args)
-
     token.token_service.api_call(
         args, requests.post, f"/v1/dataset-file/{dataset_file_id}/initiate-upload/"
     )
 
     loop = asyncio.new_event_loop()
     with upload_abort_ctxmgr(args, dataset_file_id):
         loop.run_until_complete(manage_uploads(args, dataset_file_id, csv_args))
```

### Comparing `aidentified-matching-api-1.1.3/aidentified_matching_api/get_id.py` & `aidentified-matching-api-1.2.0/aidentified_matching_api/get_id.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,20 +25,24 @@
 
     if resp_obj["count"] == 0:
         raise Exception(f"No dataset with name '{args.dataset_name}' found")
 
     return resp_obj["results"][0]["dataset_id"]
 
 
-def get_dataset_file_id_from_dataset_file_name(args):
+def get_dataset_file_from_dataset_file_name(args):
     dataset_params = {
         "dataset_name": args.dataset_name,
         "name": args.dataset_file_name,
     }
     resp_obj = token.token_service.api_call(
         args, requests.get, "/v1/dataset-file/", params=dataset_params
     )
 
     if resp_obj["count"] == 0:
         raise Exception(f"No dataset file with name '{args.dataset_file_name}' found")
 
-    return resp_obj["results"][0]["dataset_file_id"]
+    return resp_obj["results"][0]
+
+
+def get_dataset_file_id_from_dataset_file_name(args):
+    return get_dataset_file_from_dataset_file_name(args)["dataset_file_id"]
```

### Comparing `aidentified-matching-api-1.1.3/aidentified_matching_api/token_service.py` & `aidentified-matching-api-1.2.0/aidentified_matching_api/token_service.py`

 * *Files identical despite different names*

### Comparing `aidentified-matching-api-1.1.3/aidentified_matching_api/validation.py` & `aidentified-matching-api-1.2.0/aidentified_matching_api/validation.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import codecs
 import csv
 import io
+from typing import List
 
 import aidentified_matching_api.constants as constants
 
 # first_name - string - required
 # last_name - string - required
 # id - string - optional; unique
 # street_address_1 - string - optional; home street
@@ -53,14 +54,30 @@
     "linkedin",
     *[f"school_{idx}" for idx in range(1, 11)],
     *[f"email_{idx}" for idx in range(1, 11)],
     *[f"phone_{idx}" for idx in range(1, 11)],
     *[f"domain_{idx}" for idx in range(1, 11)],
     *[f"linkedin_{idx}" for idx in range(1, 11)],
 }
+HEADERS_ADDRESS_ONLY = {
+    "id",
+    "street_address_1",
+    "street_address_2",
+    "postal_code",
+    "city",
+}
+HEADERS_EMAIL_ONLY = {
+    "id",
+    "email",
+    *[f"email_{idx}" for idx in range(1, 11)],
+}
+
+
+class ValidationError(Exception):
+    pass
 
 
 class CsvArgs:
     __slots__ = [
         "raw_fd",
         "codec_info",
         "delimiter",
@@ -92,26 +109,26 @@
         self.skipinitialspace = skipinitialspace
 
 
 def _csv_read(csv_reader, record_idx):
     try:
         return next(csv_reader)
     except csv.Error as e:
-        raise Exception(f"Bad CSV format in row {record_idx}: {e}") from None
+        raise ValidationError(f"Bad CSV format in row {record_idx}: {e}") from None
     except UnicodeError as e:
-        raise Exception(f"Bad character encoding at byte {e.start}") from None
+        raise ValidationError(f"Bad character encoding at byte {e.start}") from None
 
 
-def validate(args) -> CsvArgs:
+def validate(args, match_logic) -> CsvArgs:
     # Validate choice of csv encoding, even if they don't do
     # the rest of the validation.
     try:
         codec_info = codecs.lookup(args.csv_encoding)
     except LookupError:
-        raise Exception(f"Unknown csv-encoding '{args.csv_encoding}'") from None
+        raise ValidationError(f"Unknown csv-encoding '{args.csv_encoding}'") from None
 
     csv_args = CsvArgs(
         args.dataset_file_path,
         codec_info,
         args.csv_delimiter,
         args.csv_no_doublequotes,
         args.csv_escapechar,
@@ -119,103 +136,163 @@
         constants.QUOTE_METHODS[args.csv_quoting],
         args.csv_skip_initial_space,
     )
 
     if not args.validate:
         return csv_args
 
-    validate_fd(csv_args)
-    args.dataset_file_path.seek(0)
+    if match_logic == "OPPORTUNISTIC":
+        validator = OpportunisticCsvValidator(csv_args)
+    elif match_logic == "ADDRESS":
+        validator = AddressCsvValidator(csv_args)
+    elif match_logic == "EMAIL":
+        validator = EmailCsvValidator(csv_args)
+    else:
+        raise ValidationError(f"Unknown match_logic '{args.match_logic}'")
 
-    return csv_args
+    validator.validate()
 
+    args.dataset_file_path.seek(0)
 
-def validate_fd(csv_args: CsvArgs):
-    potential_bom = csv_args.raw_fd.read(3)
-    # Python drops the BOM from UTF16/UTF32 but not UTF8
-    if potential_bom == codecs.BOM_UTF8:
-        skip_len = 3
-    else:
-        skip_len = 0
-    csv_args.raw_fd.seek(0)
-    csv_args.raw_fd.read(skip_len)
-
-    text_fd = csv_args.codec_info.streamreader(csv_args.raw_fd)
-
-    csv_reader = csv.reader(
-        text_fd,
-        delimiter=csv_args.delimiter,
-        doublequote=csv_args.doublequotes,
-        escapechar=csv_args.escapechar,
-        quotechar=csv_args.quotechar,
-        quoting=csv_args.quoting,
-        skipinitialspace=csv_args.skipinitialspace,
-        strict=True,
-    )
+    return csv_args
 
-    record_idx = 1
 
-    try:
-        headers = _csv_read(csv_reader, record_idx)
-    except StopIteration:
-        raise Exception("No headers in file") from None
-
-    for header in headers:
-        if header not in HEADERS:
-            raise Exception(f"Invalid header '{header}'")
-
-    sentinel = object()
-    if (
-        next(
-            (
-                header
-                for header in headers
-                if header not in ("id", "first_name", "last_name")
-            ),
-            sentinel,
+class CsvValidator:
+    valid_headers: List[str]
+    required_headers: List[str]
+
+    def __init__(self, csv_args: CsvArgs):
+        potential_bom = csv_args.raw_fd.read(3)
+        # Python drops the BOM from UTF16/UTF32 but not UTF8
+        if potential_bom == codecs.BOM_UTF8:
+            skip_len = 3
+        else:
+            skip_len = 0
+        csv_args.raw_fd.seek(0)
+        csv_args.raw_fd.read(skip_len)
+
+        text_fd = csv_args.codec_info.streamreader(csv_args.raw_fd)
+
+        csv_reader = csv.reader(
+            text_fd,
+            delimiter=csv_args.delimiter,
+            doublequote=csv_args.doublequotes,
+            escapechar=csv_args.escapechar,
+            quotechar=csv_args.quotechar,
+            quoting=csv_args.quoting,
+            skipinitialspace=csv_args.skipinitialspace,
+            strict=True,
         )
-        is sentinel
-    ):
-        raise Exception("Needs at least one of the extra attribute headers")
 
-    record_len = len(headers)
+        self.csv_reader = csv_reader
+        self.required_header_idxes = []
 
-    try:
-        id_idx = headers.index("id")
-    except ValueError:
-        id_idx = None
-    id_uniqueness = set()
+    def validate(self):
+        """Raises ValidationError when stuff goes wrong"""
+        record_idx = 1
+
+        try:
+            headers = _csv_read(self.csv_reader, record_idx)
+        except StopIteration:
+            raise ValidationError("No headers in file") from None
 
-    required_header_idxes = []
-    for required_header in ("first_name", "last_name"):
-        if required_header not in headers:
-            raise Exception(f"Required header {required_header} not in headers")
+        for header in headers:
+            if header not in self.valid_headers:
+                raise ValidationError(f"Invalid header '{header}'")
 
-        required_header_idxes.append((required_header, headers.index(required_header)))
+        self.validate_extra_attr_headers(headers)
 
-    record_idx += 1
+        record_len = len(headers)
 
-    while True:
         try:
-            record = _csv_read(csv_reader, record_idx)
-        except StopIteration:
-            break
+            id_idx = headers.index("id")
+        except ValueError:
+            id_idx = None
+        id_uniqueness = set()
 
-        if record_idx > 500_001:
-            raise Exception("CSV has more than 500,000 data rows")
+        self.calculate_required_header_idxes(headers)
 
-        if len(record) != record_len:
-            raise Exception(f"Row {record_idx} does not match header length")
+        record_idx += 1
 
-        if id_idx is not None:
-            cust_id = record[id_idx]
-            if cust_id in id_uniqueness:
-                raise Exception(f"Row {record_idx} has duplicate id '{cust_id}'")
-            id_uniqueness.add(cust_id)
-
-        for required_header, required_header_idx in required_header_idxes:
-            if not record[required_header_idx]:
-                raise Exception(
-                    f"Row {record_idx} has invalid value for {required_header}"
+        while True:
+            try:
+                record = _csv_read(self.csv_reader, record_idx)
+            except StopIteration:
+                break
+
+            if record_idx > 500_001:
+                raise ValidationError("CSV has more than 500,000 data rows")
+
+            if len(record) != record_len:
+                raise ValidationError(f"Row {record_idx} does not match header length")
+
+            if id_idx is not None:
+                cust_id = record[id_idx]
+                if cust_id in id_uniqueness:
+                    raise ValidationError(
+                        f"Row {record_idx} has duplicate id '{cust_id}'"
+                    )
+                id_uniqueness.add(cust_id)
+
+            for required_header, required_header_idx in self.required_header_idxes:
+                if not record[required_header_idx]:
+                    raise ValidationError(
+                        f"Row {record_idx} has invalid value for {required_header}"
+                    )
+
+            record_idx += 1
+
+    def validate_extra_attr_headers(self, headers: List[str]):
+        sentinel = object()
+        if (
+            next(
+                (
+                    header
+                    for header in headers
+                    if header not in ["id"] + self.required_headers
+                ),
+                sentinel,
+            )
+            is sentinel
+        ):
+            raise ValidationError("Needs at least one of the extra attribute headers")
+
+    def calculate_required_header_idxes(self, headers: List[str]):
+        for required_header in self.required_headers:
+            if required_header not in headers:
+                raise ValidationError(
+                    f"Required header {required_header} not in headers"
                 )
 
-        record_idx += 1
+            self.required_header_idxes.append(
+                (required_header, headers.index(required_header))
+            )
+
+
+class OpportunisticCsvValidator(CsvValidator):
+    valid_headers = HEADERS
+    required_headers = ["first_name", "last_name"]
+
+
+class AddressCsvValidator(CsvValidator):
+    valid_headers = HEADERS_ADDRESS_ONLY
+    required_headers = ["street_address_1"]
+
+    def validate_extra_attr_headers(self, headers: List[str]):
+        return
+
+
+class EmailCsvValidator(CsvValidator):
+    valid_headers = HEADERS_EMAIL_ONLY
+    required_headers = []
+
+    def validate_extra_attr_headers(self, headers: List[str]):
+        return
+
+    def calculate_required_header_idxes(self, headers: List[str]):
+        for header in ("email", "email_1"):
+            if header in headers:
+                self.required_header_idxes.append((header, headers.index(header)))
+                return
+
+        if not self.required_header_idxes:
+            raise ValidationError("Required header email_N not in headers")
```

### Comparing `aidentified-matching-api-1.1.3/aidentified_matching_api.egg-info/SOURCES.txt` & `aidentified-matching-api-1.2.0/aidentified_matching_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aidentified-matching-api-1.1.3/setup.py` & `aidentified-matching-api-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open("requirements.in", "r") as fd:
     requirements = [x.strip() for x in fd.readlines()]
 
 setup(
     name="aidentified-matching-api",
-    version="1.1.3",
+    version="1.2.0",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
     ],
     packages=["aidentified_matching_api"],
     python_requires=">=3.7",
     # Let's not force all the hard requirements out from requirements.txt
```

