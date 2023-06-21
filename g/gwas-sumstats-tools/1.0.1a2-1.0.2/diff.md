# Comparing `tmp/gwas_sumstats_tools-1.0.1a2.tar.gz` & `tmp/gwas_sumstats_tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwas_sumstats_tools-1.0.1a2.tar", max compression
+gzip compressed data, was "gwas_sumstats_tools-1.0.2.tar", max compression
```

## Comparing `gwas_sumstats_tools-1.0.1a2.tar` & `gwas_sumstats_tools-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-03-14 16:27:27.618973 gwas_sumstats_tools-1.0.1a2/LICENSE
--rw-r--r--   0        0        0     4846 2023-04-11 15:51:21.526207 gwas_sumstats_tools-1.0.1a2/README.md
--rw-r--r--   0        0        0    11560 2023-04-11 15:51:21.557208 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/cli.py
--rw-r--r--   0        0        0     1387 2023-03-14 16:27:27.619973 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/config.py
--rw-r--r--   0        0        0     5817 2023-05-16 16:41:20.816328 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/format.py
--rw-r--r--   0        0        0    10291 2023-04-11 15:51:21.558208 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/interfaces/data_table.py
--rw-r--r--   0        0        0     7574 2023-05-16 16:41:20.816328 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/interfaces/metadata.py
--rw-r--r--   0        0        0     3913 2023-03-14 16:27:27.619973 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/read.py
--rw-r--r--   0        0        0     5754 2023-03-14 16:27:27.619973 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/schema/data_table.py
--rw-r--r--   0        0        0     1816 2023-05-12 16:09:12.400946 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/schema/metadata.py
--rw-r--r--   0        0        0     4773 2023-05-12 13:51:16.163417 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/utils.py
--rw-r--r--   0        0        0     8337 2023-04-11 15:51:21.558208 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/validate.py
--rw-r--r--   0        0        0      679 2023-05-16 16:41:20.824328 gwas_sumstats_tools-1.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-14 16:27:27.618973 gwas_sumstats_tools-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5207 2023-06-06 14:58:15.047099 gwas_sumstats_tools-1.0.2/README.md
+-rwxr-xr-x   0        0        0    11560 2023-06-06 14:58:15.062099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/cli.py
+-rwxr-xr-x   0        0        0     1387 2023-06-06 14:58:15.062099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/config.py
+-rwxr-xr-x   0        0        0     5380 2023-06-06 14:58:15.062099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/format.py
+-rwxr-xr-x   0        0        0    10291 2023-06-06 14:58:15.071099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/interfaces/data_table.py
+-rwxr-xr-x   0        0        0     7574 2023-06-06 14:58:15.084099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/interfaces/metadata.py
+-rwxr-xr-x   0        0        0     3913 2023-06-06 14:58:15.084099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/read.py
+-rwxr-xr-x   0        0        0     5754 2023-06-06 14:58:15.084099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/schema/data_table.py
+-rwxr-xr-x   0        0        0     1816 2023-06-06 14:58:15.099099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/schema/metadata.py
+-rwxr-xr-x   0        0        0     4773 2023-06-06 14:58:15.118099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/utils.py
+-rwxr-xr-x   0        0        0     8337 2023-06-06 14:58:15.119099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/validate.py
+-rw-r--r--   0        0        0      695 2023-06-21 12:34:18.075637 gwas_sumstats_tools-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5888 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.2/PKG-INFO
```

### Comparing `gwas_sumstats_tools-1.0.1a2/LICENSE` & `gwas_sumstats_tools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a2/README.md` & `gwas_sumstats_tools-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,17 +31,28 @@
   * Create metadata from the GWAS Catalog (internal use, requires authenticated API): `-g`
   * Edit/add the values to the metadata: `-e` with `--<FIELD>=<VALUE>`
 
 ## Requirements
 - python >= 3.9
 
 ## Installation
+### Local installation with pip
 ```console
-$ pip install gwas-sumstats-tools
+$ pip3 install gwas-sumstats-tools
 ```
+### Run with Docker
+The following Docker command is the equivalent to running `gwas-ssf`. 
+```console
+$ docker run -it -v ${PWD}:/application ebispot/gwas-sumstats-tools:latest
+```
+Just append any subcommands or arguments e.g.:
+```console
+$ docker run -it -v ${PWD}:/application ebispot/gwas-sumstats-tools:latest validate
+```
+
 
 ## Usage
 
 <p align="center"><img src="gwas-demo.gif"/></p>
 
 ```console
 $ gwas-ssf [OPTIONS] COMMAND [ARGS]...
```

### Comparing `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/cli.py` & `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/cli.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/config.py` & `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/config.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/format.py` & `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/format.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,79 @@
 from pathlib import Path
 from rich import print
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
 from gwas_sumstats_tools.interfaces.data_table import SumStatsTable
-from gwas_sumstats_tools.interfaces.metadata import (MetadataClient,
-                                                     metadata_dict_from_gwas_cat,
-                                                     get_file_metadata)
-from gwas_sumstats_tools.utils import (parse_accession_id,
-                                       append_to_path,
-                                       exit_if_no_data)
+from gwas_sumstats_tools.interfaces.metadata import (
+    MetadataClient,
+    metadata_dict_from_gwas_cat,
+    get_file_metadata,
+)
+from gwas_sumstats_tools.utils import (
+    parse_accession_id,
+    append_to_path,
+    exit_if_no_data,
+)
 
 
 class Formatter:
-    def __init__(self,
-                 data_infile: Path,
-                 data_outfile: Path = None,
-                 metadata_infile: Path = None,
-                 metadata_outfile: Path = None,
-                 format_data: bool = False,
-                 ) -> None:
+    def __init__(
+        self,
+        data_infile: Path,
+        data_outfile: Path = None,
+        metadata_infile: Path = None,
+        metadata_outfile: Path = None,
+        format_data: bool = False,
+    ) -> None:
         self.format_data = format_data
         self.data_infile = Path(data_infile)
-        self.data_outfile = Path(self._set_data_outfile_name()
-                                 if not data_outfile
-                                 else data_outfile)
-        self.metadata_outfile = Path(self._set_metadata_outfile_name()
-                                     if not metadata_outfile
-                                     else metadata_outfile)
-        self.data = SumStatsTable(sumstats_file=self.data_infile) \
-            if self.data_infile else None
-        self.meta = MetadataClient(in_file=metadata_infile,
-                                   out_file=self.metadata_outfile)
+        self.data_outfile = Path(
+            self._set_data_outfile_name() if not data_outfile else data_outfile
+        )
+        self.metadata_outfile = Path(
+            self._set_metadata_outfile_name()
+            if not metadata_outfile
+            else metadata_outfile
+        )
+        self.data = (
+            SumStatsTable(sumstats_file=self.data_infile) if self.data_infile else None
+        )
+        self.meta = MetadataClient(
+            in_file=metadata_infile, out_file=self.metadata_outfile
+        )
 
     def _set_data_outfile_name(self) -> str:
-        """Set the data outfile name. 
+        """Set the data outfile name.
         This method only runs if the data outfile is not
         set. Then if the data is not to be reformatted, the
-        outfile is the same as the infile. If the data is 
-        to be formatted, the outfile name is configured based 
+        outfile is the same as the infile. If the data is
+        to be formatted, the outfile name is configured based
         on infile name accession ID parsing.
 
         Returns:
             data outfile name string
         """
         if self.format_data:
             accession_id = parse_accession_id(filename=self.data_infile)
             if accession_id:
                 self.data_outfile = accession_id + ".tsv.gz"
             else:
-                self.data_outfile = append_to_path(self.data_infile, "-FORMATTED.tsv.gz")
+                self.data_outfile = append_to_path(
+                    self.data_infile, "-FORMATTED.tsv.gz"
+                )
         else:
             self.data_outfile = self.data_infile
         return self.data_outfile
 
     def _set_metadata_outfile_name(self) -> str:
         return append_to_path(self.data_outfile, "-meta.yaml")
 
-    def set_metadata(self,
-                     from_gwas_cat: bool = False,
-                     custom_metadata: dict = None) -> MetadataClient:
+    def set_metadata(
+        self, from_gwas_cat: bool = False, custom_metadata: dict = None
+    ) -> MetadataClient:
         """Set metadata.
         The hierarchy of where metadata is set is as follows:
         1. custom_metadata map (overwrites anything below)
         2. metadata from the GWAS Catalog
         3. metadata from the original input file
         4. metadata inferred from the datafile
 
@@ -70,63 +81,71 @@
             from_gwas_cat -- update with data from GWAS catalog (default: {False})
             custom_metadata -- Update with this map (default: {None})
 
         Returns:
             metadata object
         """
         self.meta.from_file()
-        meta_dict = get_file_metadata(in_file=self.data_infile,
-                                      out_file=self.data_outfile,
-                                      meta_dict=self.meta.as_dict())
+        meta_dict = get_file_metadata(
+            in_file=self.data_infile,
+            out_file=self.data_outfile,
+            meta_dict=self.meta.as_dict(),
+        )
         if from_gwas_cat:
             accession_id = parse_accession_id(filename=self.data_infile)
             meta_dict.update(metadata_dict_from_gwas_cat(accession_id=accession_id))
         if custom_metadata:
             meta_dict.update(custom_metadata)
         self.meta.update_metadata(meta_dict)
         return self.meta
 
 
-def format(filename: Path,
-           data_outfile: Path = None,
-           minimal_to_standard: bool = False,
-           generate_metadata: bool = False,
-           metadata_outfile: Path = None,
-           metadata_infile: Path = None,
-           metadata_from_gwas_cat: bool = False,
-           header_map: dict = None,
-           metadata_dict: dict = None,
-           ) -> None:
-
-    formatter = Formatter(data_infile=filename,
-                          data_outfile=data_outfile,
-                          metadata_infile=metadata_infile,
-                          metadata_outfile=metadata_outfile,
-                          format_data=minimal_to_standard)
+def format(
+    filename: Path,
+    data_outfile: Path = None,
+    minimal_to_standard: bool = False,
+    generate_metadata: bool = False,
+    metadata_outfile: Path = None,
+    metadata_infile: Path = None,
+    metadata_from_gwas_cat: bool = False,
+    header_map: dict = None,
+    metadata_dict: dict = None,
+) -> None:
+    formatter = Formatter(
+        data_infile=filename,
+        data_outfile=data_outfile,
+        metadata_infile=metadata_infile,
+        metadata_outfile=metadata_outfile,
+        format_data=minimal_to_standard,
+    )
     if minimal_to_standard:
         exit_if_no_data(table=formatter.data.sumstats)
         print("[bold]\n-------- SUMSTATS DATA --------\n[/bold]")
         print(formatter.data.sumstats)
         if header_map:
             formatter.data.reformat_header(header_map=header_map)
         else:
             formatter.data.reformat_header()
         formatter.data.normalise_missing_values()
         print("[bold]\n-------- REFORMATTED DATA --------\n[/bold]")
         print(formatter.data.sumstats)
-        print(f"[green]Formatting and writing sumstats data --> {str(formatter.data_outfile)}[/green]")
-        with Progress(SpinnerColumn(finished_text="Complete!"),
-                      TextColumn("[progress.description]{task.description}"),
-                      transient=True
-                      ) as progress:
+        print(
+            f"[green]Formatting and writing sumstats data --> {str(formatter.data_outfile)}[/green]"
+        )
+        with Progress(
+            SpinnerColumn(finished_text="Complete!"),
+            TextColumn("[progress.description]{task.description}"),
+            transient=True,
+        ) as progress:
             progress.add_task(description="Processing...", total=None)
             formatter.data.to_file(outfile=formatter.data_outfile)
     # Get metadata
     if generate_metadata:
         print("[bold]\n---------- METADATA ----------\n[/bold]")
-        metadata = formatter.set_metadata(from_gwas_cat=metadata_from_gwas_cat,
-                                          custom_metadata=metadata_dict)
+        metadata = formatter.set_metadata(
+            from_gwas_cat=metadata_from_gwas_cat, custom_metadata=metadata_dict
+        )
         print(metadata)
         print(f"[green]Writing metadata --> {str(metadata._out_file)}[/green]")
         metadata.to_file()
     if not any([minimal_to_standard, generate_metadata]):
-        print("Nothing to do.")
+        print("Nothing to do.")
```

### Comparing `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/interfaces/data_table.py` & `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/interfaces/data_table.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/interfaces/metadata.py` & `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/interfaces/metadata.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/read.py` & `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/read.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/schema/data_table.py` & `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/schema/data_table.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/schema/metadata.py` & `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/utils.py` & `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/utils.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/validate.py` & `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/validate.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a2/pyproject.toml` & `gwas_sumstats_tools-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "gwas-sumstats-tools"
-version = "1.0.1a2"
+version = "1.0.2"
 description = ""
 authors = ["jdhayhurst <jhayhurst@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "gwas_sumstats_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 petl = "^1.7.12"
 requests = "^2.28.2"
 pyyaml = "^6.0"
 pydantic = "^1.10.4"
 typer = {extras = ["all"], version = "^0.7.0"}
 pandera = {extras = ["io"], version = "^0.13.4"}
+pandas = "^2.0.2"
 
 [tool.poetry.scripts]
 gwas-ssf = "gwas_sumstats_tools.cli:app"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 pytest = "^7.2.1"
```

### Comparing `gwas_sumstats_tools-1.0.1a2/PKG-INFO` & `gwas_sumstats_tools-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: gwas-sumstats-tools
-Version: 1.0.1a2
+Version: 1.0.2
 Summary: 
 Author: jdhayhurst
 Author-email: jhayhurst@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pandera[io] (>=0.13.4,<0.14.0)
 Requires-Dist: petl (>=1.7.12,<2.0.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
@@ -50,17 +51,28 @@
   * Create metadata from the GWAS Catalog (internal use, requires authenticated API): `-g`
   * Edit/add the values to the metadata: `-e` with `--<FIELD>=<VALUE>`
 
 ## Requirements
 - python >= 3.9
 
 ## Installation
+### Local installation with pip
 ```console
-$ pip install gwas-sumstats-tools
+$ pip3 install gwas-sumstats-tools
 ```
+### Run with Docker
+The following Docker command is the equivalent to running `gwas-ssf`. 
+```console
+$ docker run -it -v ${PWD}:/application ebispot/gwas-sumstats-tools:latest
+```
+Just append any subcommands or arguments e.g.:
+```console
+$ docker run -it -v ${PWD}:/application ebispot/gwas-sumstats-tools:latest validate
+```
+
 
 ## Usage
 
 <p align="center"><img src="gwas-demo.gif"/></p>
 
 ```console
 $ gwas-ssf [OPTIONS] COMMAND [ARGS]...
```

