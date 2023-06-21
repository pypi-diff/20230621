# Comparing `tmp/getpaper-0.0.5.tar.gz` & `tmp/getpaper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.0.5.tar", last modified: Wed Jun 21 00:15:39 2023, max compression
+gzip compressed data, was "getpaper-0.0.6.tar", last modified: Wed Jun 21 13:47:05 2023, max compression
```

## Comparing `getpaper-0.0.5.tar` & `getpaper-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 00:15:39.092116 getpaper-0.0.5/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.0.5/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1959 2023-06-21 00:15:39.092116 getpaper-0.0.5/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1344 2023-06-20 23:35:34.000000 getpaper-0.0.5/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 00:15:39.088116 getpaper-0.0.5/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.0.5/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3544 2023-06-20 22:10:24.000000 getpaper-0.0.5/getpaper/download.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1306 2023-06-21 00:13:24.000000 getpaper-0.0.5/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     4810 2023-06-21 00:06:28.000000 getpaper-0.0.5/getpaper/parse.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 00:15:39.092116 getpaper-0.0.5/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1959 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      298 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       78 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      142 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-21 00:15:39.092116 getpaper-0.0.5/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1472 2023-06-21 00:06:39.000000 getpaper-0.0.5/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 13:47:05.744694 getpaper-0.0.6/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.0.6/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2280 2023-06-21 13:47:05.744694 getpaper-0.0.6/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1665 2023-06-21 13:18:25.000000 getpaper-0.0.6/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 13:47:05.740694 getpaper-0.0.6/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.0.6/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     4033 2023-06-21 12:30:05.000000 getpaper-0.0.6/getpaper/download.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4415 2023-06-21 12:58:00.000000 getpaper-0.0.6/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     5452 2023-06-21 12:24:40.000000 getpaper-0.0.6/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1068 2023-06-21 10:50:13.000000 getpaper-0.0.6/getpaper/splitter.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 13:47:05.744694 getpaper-0.0.6/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2280 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       78 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-21 13:47:05.744694 getpaper-0.0.6/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1535 2023-06-21 13:45:20.000000 getpaper-0.0.6/setup.py
```

### Comparing `getpaper-0.0.5/LICENSE` & `getpaper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.5/PKG-INFO` & `getpaper-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.0.5
+Version: 0.0.6
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -46,13 +46,22 @@
 getpaper/parse.py parse_folder --folder /home/antonkulaga/sources/getpaper/test
 ```
 You can also parse papers on a per file basis, for example:
 ```bash
 getpaper/parse.py parse_paper --paper /home/antonkulaga/sources/getpaper/test/22266545.pdf
 ```
 
+## Indexing papers
+
+We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
+For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
+
+# Examples
+
+You can run examples.py to see usage examples
+
 # Additional requirements
 
 Detectron2 is required for using models from the layoutparser model zoo but is not automatically installed with this package. 
 For MacOS and Linux, build from source with:
 
 pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
```

### Comparing `getpaper-0.0.5/README.md` & `getpaper-0.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -28,13 +28,22 @@
 getpaper/parse.py parse_folder --folder /home/antonkulaga/sources/getpaper/test
 ```
 You can also parse papers on a per file basis, for example:
 ```bash
 getpaper/parse.py parse_paper --paper /home/antonkulaga/sources/getpaper/test/22266545.pdf
 ```
 
+## Indexing papers
+
+We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
+For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
+
+# Examples
+
+You can run examples.py to see usage examples
+
 # Additional requirements
 
 Detectron2 is required for using models from the layoutparser model zoo but is not automatically installed with this package. 
 For MacOS and Linux, build from source with:
 
 pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
```

### Comparing `getpaper-0.0.5/getpaper/download.py` & `getpaper-0.0.6/getpaper/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,25 +38,42 @@
     """
     doi_from_pubmed wrapped in try
     :param pubmed:
     :return:
     """
     return Try.of(lambda: doi_from_pubmed(pubmed))
 
-def try_download(doi: str, papers: Path, skip_if_exist: bool = True, name: Optional[str] = None) -> Try[Path]:
+def try_download(doi: str, destination: Path, skip_if_exist: bool = True, name: Optional[str] = None) -> Try[Path]:
+    """
+    downloads the paper by doi
+    :param doi:
+    :param destination: where to put the results
+    :param skip_if_exist:
+    :param name:
+    :return: Try monad with the result
+    """
     doi_url = f"https://doi.org/{doi}"
-    paper = (papers / f"{doi}.pdf").absolute().resolve() if name is None else (papers / f"{name.replace(',pdf', '')}.pdf").absolute().resolve()
+    paper = (destination / f"{doi}.pdf").absolute().resolve() if name is None else (destination / f"{name.replace(',pdf', '')}.pdf").absolute().resolve()
     if skip_if_exist and paper.exists():
         print(f"Paper {paper} for {doi} already exists!")
-        return paper
+        return Try.of(lambda: paper)
     return Try.of(lambda: scihub_download(doi_url, paper_type="doi", out=str(paper))).map(lambda _: paper)
 
-def download_pubmed(pubmed: str, papers: Path, skip_if_exist: bool = True, name: Optional[str] = None):
+
+def download_pubmed(pubmed: str, destination: Path, skip_if_exist: bool = True, name: Optional[str] = None):
+    """
+    downloads paper by its pubmed id
+    :param pubmed: pubmed id
+    :param destination: where to store the result
+    :param skip_if_exist:
+    :param name:
+    :return:
+    """
     try_resolve = try_doi_from_pubmed(pubmed)
-    return try_resolve.flat_map(lambda doi: try_download(doi, papers, skip_if_exist, name))
+    return try_resolve.flat_map(lambda doi: try_download(doi, destination, skip_if_exist, name))
 
 
 @click.group(invoke_without_command=False)
 @click.pass_context
 def app(ctx: Context):
     #if ctx.invoked_subcommand is None:
     #    click.echo('Running the default command...')
@@ -64,15 +81,16 @@
     pass
 
 @app.command("download_doi")
 @click.option('--doi', type=click.STRING, help="download doi")
 @click.option('--folder', type=click.Path(), default=".", help="where to download the paper")
 @click.option('--skip_existing', type=click.BOOL, default=True, help="if it should skip downloading if the paper exists")
 @click.option('--name', type=click.STRING, default=None, help="custom name, used doi of none")
-def download_doi_command(doi: str, folder: str, skip_existing: bool, name: Optional[str]):
+def download_doi_command(doi: str, folder: str, skip_existing: bool = True, name: Optional[str] = None) -> Try:
+    print(f"downloading {doi} to {folder}")
     where = Path(folder)
     where.mkdir(exist_ok=True, parents=True)
     return try_download(doi, where, skip_existing, name)
 
 @app.command("download_pubmed")
 @click.option('--pubmed', type=click.STRING, help="download doi")
 @click.option('--folder', type=click.Path(), default=".", help="where to download the paper")
```

### Comparing `getpaper-0.0.5/getpaper/parse.py` & `getpaper-0.0.6/getpaper/parse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
-from typing import Optional
+from typing import Optional, List
 
 import click
 import requests
 from click import Context
 from langchain.document_loaders import UnstructuredPDFLoader
 from langchain.schema import Document
 from pycomfort.files import traverse
 
 def parse_paper(paper: Path, folder: Optional[Path] = None,
-                mode: str = "single", strategy: str = "hi_res",
+                mode: str = "single", strategy: str = "auto",
                 pdf_infer_table_structure: bool = True,
                 include_page_breaks: bool = False
                 ):
     """
     Parses the paper using Unstructured paper parser
     :param paper:
     :param folder:
@@ -40,54 +40,71 @@
             f = (where / f"{paper.stem}_{i}.txt")
             print(f"writing {f}")
             f.write_text(doc.page_content)
             acc.append(f)
         return acc
 
 def parse_papers(parse_folder: Path, destination: Optional[Path] = None,
-                 mode: str = "single", strategy: str = "hi_res",
+                 mode: str = "single", strategy: str = "auto",
                  pdf_infer_table_structure: bool = True,
                  include_page_breaks: bool = False):
     papers: list[Path] = traverse(parse_folder, lambda p: "pdf" in p.suffix)
     print(f"indexing {len(papers)} papers")
     acc = []
     for i, paper in enumerate(papers):
         where = destination if destination is not None else paper.parent
         print(f"adding paper {paper} which is {i} out of {len(papers)}. It will be saved to {where}")
         acc = acc + parse_paper(paper, where, mode, strategy, pdf_infer_table_structure, include_page_breaks)
     print("papers parsing finished!")
     return acc
 
+def papers_to_documents(folder: Path, suffix: str = ""):
+    txt = traverse(folder, lambda p: "txt" in p.suffix)
+    texts = [t for t in txt if suffix in t.name] if suffix != "" else txt
+    docs: List[Document] = []
+    for t in texts:
+        doi = f"http://doi.org/{t.parent.name}/{t.stem}"
+        with open(t, 'r') as file:
+            text = file.read()
+            if len(text)<10:
+                print("TOO SHORT TEXT")
+            else:
+                doc = Document(
+                    page_content = text,
+                    metadata={"source": doi}
+                )
+                docs.append(doc)
+    return docs
 
 @click.group(invoke_without_command=False)
 @click.pass_context
 def app(ctx: Context):
     #if ctx.invoked_subcommand is None:
     #    click.echo('Running the default command...')
     #    test_index()
     pass
 
 @app.command("parse_paper")
 @click.option('--paper', type=click.Path(exists=True), help="paper pdf to parse")
 @click.option('--destination', type=click.STRING, default=".", help="destination folder")
 @click.option('--mode', type=click.Choice(["single", "elements", "paged"]), default="single", help="paper mode to be used")
-@click.option('--strategy', type=click.Choice(["auto", "hi_res"]), default="hi_res", help="parsing strategy to be used, hi-res by default")
+@click.option('--strategy', type=click.Choice(["auto", "hi_res", "fast"]), default="auto", help="parsing strategy to be used, auto by default")
 @click.option('--infer_tables', type=click.BOOL, default=True, help="if the table structure should be inferred")
 @click.option('--include_page_breaks', type=click.BOOL, default=False, help="if page breaks should be included")
 def parse_paper_command(paper: str, destination: str, mode: str, strategy: str, infer_tables: bool, include_page_breaks: bool):
     paper_file = Path(paper)
     destination_folder = Path(destination)
     print(f"parsing paper {paper} with mode={mode} {'' if destination_folder is None else 'destination folder ' + destination}")
     return parse_paper(paper_file, None, mode, strategy, infer_tables, include_page_breaks)
 
 @app.command("parse_folder")
 @click.option('--folder', type=click.Path(exists=True), help="folder to parse papers in")
 @click.option('--destination', type=click.STRING, default=None, help="destination folder")
 @click.option('--mode', type=click.Choice(["single", "elements", "paged"]), default="single", help="paper mode to be used")
-@click.option('--strategy', type=click.Choice(["auto", "hi_res"]), default="hi_res", help="parsing strategy to be used, hi-res by default")
+@click.option('--strategy', type=click.Choice(["auto", "hi_res", "fast"]), default="auto", help="parsing strategy to be used, auto by default")
 @click.option('--infer_tables', type=click.BOOL, default=True, help="if the table structure should be inferred")
 @click.option('--include_page_breaks', type=click.BOOL, default=False, help="if page breaks should be included")
 def parse_paper_command(folder: str,destination: str, mode: str, strategy: str, infer_tables: bool, include_page_breaks: bool):
     parse_folder = Path(folder)
     destination_folder = Path(destination) if destination is not None else None
     print(f"parsing paper {folder} with mode={mode} {'' if destination_folder is None else 'destination folder ' + destination}")
     return parse_papers(parse_folder, destination_folder, mode, strategy, infer_tables, include_page_breaks)
```

### Comparing `getpaper-0.0.5/getpaper.egg-info/PKG-INFO` & `getpaper-0.0.6/getpaper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.0.5
+Version: 0.0.6
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -46,13 +46,22 @@
 getpaper/parse.py parse_folder --folder /home/antonkulaga/sources/getpaper/test
 ```
 You can also parse papers on a per file basis, for example:
 ```bash
 getpaper/parse.py parse_paper --paper /home/antonkulaga/sources/getpaper/test/22266545.pdf
 ```
 
+## Indexing papers
+
+We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
+For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
+
+# Examples
+
+You can run examples.py to see usage examples
+
 # Additional requirements
 
 Detectron2 is required for using models from the layoutparser model zoo but is not automatically installed with this package. 
 For MacOS and Linux, build from source with:
 
 pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
```

### Comparing `getpaper-0.0.5/setup.py` & `getpaper-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
     author="antonkulaga (Anton Kulaga)",
     author_email="<antonkulaga@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['pyfunctional', 'more-itertools', 'click',
+    install_requires=['pyfunctional', 'more-itertools', 'click', 'python-dotenv', 'tiktoken', 'pynction',
                       'unstructured', 'unstructured-inference', 'unstructured[local-inference]', 'unstructured.PaddleOCR',
-                      'scidownl', 'langchain'],
+                      'scidownl', 'langchain', 'openai', 'chromadb'],
     keywords=['python', 'utils', 'files', 'papers', 'download'],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         "Operating System :: Unix",
```

