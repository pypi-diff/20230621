# Comparing `tmp/pydoc_markdown-4.8.0.tar.gz` & `tmp/pydoc_markdown-4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoc_markdown-4.8.0.tar", max compression
+gzip compressed data, was "pydoc_markdown-4.8.1.tar", max compression
```

## Comparing `pydoc_markdown-4.8.0.tar` & `pydoc_markdown-4.8.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1002 2022-11-12 22:49:35.853142 pydoc_markdown-4.8.0/LICENSE
--rw-r--r--   0        0        0     4037 2023-05-28 19:40:12.890883 pydoc_markdown-4.8.0/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-05-28 00:16:10.151072 pydoc_markdown-4.8.0/readme.md
--rw-r--r--   0        0        0     8446 2023-05-28 19:40:12.898883 pydoc_markdown-4.8.0/src/pydoc_markdown/__init__.py
--rw-r--r--   0        0        0       81 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/__init__.py
--rw-r--r--   0        0        0       81 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/loaders/__init__.py
--rw-r--r--   0        0        0     5722 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/loaders/python.py
--rw-r--r--   0        0        0       81 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/__init__.py
--rw-r--r--   0        0        0     5520 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/crossref.py
--rw-r--r--   0        0        0     3954 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/filter.py
--rw-r--r--   0        0        0     5971 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/google.py
--rw-r--r--   0        0        0     3875 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/pydocmd.py
--rw-r--r--   0        0        0     2740 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/smart.py
--rw-r--r--   0        0        0     5622 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/sphinx.py
--rw-r--r--   0        0        0       81 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/__init__.py
--rw-r--r--   0        0        0     6840 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/docusaurus.py
--rw-r--r--   0        0        0    16957 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/hugo.py
--rw-r--r--   0        0        0     3947 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/jinja2.py
--rw-r--r--   0        0        0    22500 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/markdown.py
--rw-r--r--   0        0        0     7848 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/mkdocs.py
--rw-r--r--   0        0        0       81 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/source_linkers/__init__.py
--rw-r--r--   0        0        0     6636 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/source_linkers/git.py
--rw-r--r--   0        0        0     7085 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/interfaces.py
--rw-r--r--   0        0        0    13878 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/main.py
--rw-r--r--   0        0        0     6467 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/novella/preprocessor.py
--rw-r--r--   0        0        0        0 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/py.typed
--rw-r--r--   0        0        0     3375 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/static.py
--rw-r--r--   0        0        0        5 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/__init__.py
--rw-r--r--   0        0        0     4013 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/docspec.py
--rw-r--r--   0        0        0     4545 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/knownfiles.py
--rw-r--r--   0        0        0      930 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/misc.py
--rw-r--r--   0        0        0      378 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/misc_test.py
--rw-r--r--   0        0        0     6851 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/pages.py
--rw-r--r--   0        0        0     2492 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/watchdog.py
--rw-r--r--   0        0        0     2998 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/util/ytemplate.py
--rw-r--r--   0        0        0     5787 1970-01-01 00:00:00.000000 pydoc_markdown-4.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-06-10 09:05:27.603322 pydoc_markdown-4.8.1/LICENSE
+-rw-r--r--   0        0        0     4379 2023-06-10 09:05:27.603820 pydoc_markdown-4.8.1/README.md
+-rw-r--r--   0        0        0     4042 2023-06-21 15:48:21.555580 pydoc_markdown-4.8.1/pyproject.toml
+-rw-r--r--   0        0        0     8757 2023-06-21 15:48:21.555767 pydoc_markdown-4.8.1/src/pydoc_markdown/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-10 09:05:27.631119 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-10 09:05:27.631455 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/loaders/__init__.py
+-rw-r--r--   0        0        0     5722 2023-06-10 09:05:27.631691 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/loaders/python.py
+-rw-r--r--   0        0        0       81 2023-06-10 09:05:27.632045 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/__init__.py
+-rw-r--r--   0        0        0     5520 2023-06-10 09:05:27.632255 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/crossref.py
+-rw-r--r--   0        0        0     3954 2023-06-10 09:05:27.632449 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/filter.py
+-rw-r--r--   0        0        0     5971 2023-06-10 09:05:27.632657 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/google.py
+-rw-r--r--   0        0        0     3875 2023-06-10 09:05:27.632836 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/pydocmd.py
+-rw-r--r--   0        0        0     2740 2023-06-10 09:05:27.633020 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/smart.py
+-rw-r--r--   0        0        0     5622 2023-06-10 09:05:27.633206 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/sphinx.py
+-rw-r--r--   0        0        0       81 2023-06-10 09:05:27.633857 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/__init__.py
+-rw-r--r--   0        0        0     6840 2023-06-10 09:05:27.634098 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/docusaurus.py
+-rw-r--r--   0        0        0    16977 2023-06-21 15:48:17.310736 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/hugo.py
+-rw-r--r--   0        0        0     3947 2023-06-10 09:05:27.634568 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/jinja2.py
+-rw-r--r--   0        0        0    22500 2023-06-10 09:05:27.634852 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/markdown.py
+-rw-r--r--   0        0        0     7848 2023-06-21 15:19:12.008743 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/mkdocs.py
+-rw-r--r--   0        0        0       81 2023-06-10 09:05:27.635527 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/source_linkers/__init__.py
+-rw-r--r--   0        0        0     6636 2023-06-10 09:05:27.635845 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/source_linkers/git.py
+-rw-r--r--   0        0        0     6841 2023-06-21 15:48:17.311484 pydoc_markdown-4.8.1/src/pydoc_markdown/interfaces.py
+-rw-r--r--   0        0        0    13878 2023-06-10 09:05:27.636497 pydoc_markdown-4.8.1/src/pydoc_markdown/main.py
+-rw-r--r--   0        0        0     6467 2023-06-10 09:05:27.637084 pydoc_markdown-4.8.1/src/pydoc_markdown/novella/preprocessor.py
+-rw-r--r--   0        0        0        0 2023-06-10 09:05:27.637221 pydoc_markdown-4.8.1/src/pydoc_markdown/py.typed
+-rw-r--r--   0        0        0     3375 2023-06-10 09:05:27.637431 pydoc_markdown-4.8.1/src/pydoc_markdown/static.py
+-rw-r--r--   0        0        0        5 2023-06-10 09:05:27.637750 pydoc_markdown-4.8.1/src/pydoc_markdown/util/__init__.py
+-rw-r--r--   0        0        0     4013 2023-06-10 09:05:27.638093 pydoc_markdown-4.8.1/src/pydoc_markdown/util/docspec.py
+-rw-r--r--   0        0        0     4545 2023-06-10 09:05:27.638318 pydoc_markdown-4.8.1/src/pydoc_markdown/util/knownfiles.py
+-rw-r--r--   0        0        0      930 2023-06-10 09:05:27.638499 pydoc_markdown-4.8.1/src/pydoc_markdown/util/misc.py
+-rw-r--r--   0        0        0      378 2023-06-10 09:05:27.638686 pydoc_markdown-4.8.1/src/pydoc_markdown/util/misc_test.py
+-rw-r--r--   0        0        0     7215 2023-06-21 15:48:17.312065 pydoc_markdown-4.8.1/src/pydoc_markdown/util/pages.py
+-rw-r--r--   0        0        0      706 2023-06-21 15:48:17.312634 pydoc_markdown-4.8.1/src/pydoc_markdown/util/pages_test.py
+-rw-r--r--   0        0        0     2492 2023-06-10 09:05:27.639621 pydoc_markdown-4.8.1/src/pydoc_markdown/util/watchdog.py
+-rw-r--r--   0        0        0     2998 2023-06-10 09:05:27.639948 pydoc_markdown-4.8.1/src/pydoc_markdown/util/ytemplate.py
+-rw-r--r--   0        0        0     5907 1970-01-01 00:00:00.000000 pydoc_markdown-4.8.1/PKG-INFO
```

### Comparing `pydoc_markdown-4.8.0/LICENSE` & `pydoc_markdown-4.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/pyproject.toml` & `pydoc_markdown-4.8.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "pydoc-markdown"
-version = "4.8.0"
+version = "4.8.1"
 description = "Create Python API documentation in Markdown format."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
-readme = "readme.md"
+readme = "README.md"
 packages = [{ include = "pydoc_markdown", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Topic :: Software Development :: Code Generators",
     "Topic :: Utilities",
@@ -22,16 +22,16 @@
 
 [tool.poetry.urls]
 Homepage = "https://github.com/NiklasRosenstein/pydoc-markdown"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = ">=7.1,<9.0"
-"databind.core" = "^4.3.0"
-"databind.json" = "^4.3.0"
+"databind.core" = "^4.4.0"
+"databind.json" = "^4.4.0"
 docspec = "^2.2.1"
 docspec-python = "^2.2.1"
 docstring-parser = "^0.11"
 "nr.util" = ">=0.7.5,<1.0.0"
 jinja2 = "^3.0.0"
 requests = "^2.23.0"
 PyYAML = ">=5.0,<7.0"
@@ -105,15 +105,15 @@
 [tool.slap.release]
 tag-format = "v{version}"
 
 [tool.slap.install]
 dev-extras = []
 
 [tool.slap.test]
-pytest = "pytest test/ --cov=./src/pydoc_markdown --cov-report html:htmlcov -vv"
+pytest = "pytest src/ test/ --cov=./src/pydoc_markdown --cov-report html:htmlcov -vv"
 mypy = "mypy src/ --check-untyped-defs --namespace-packages --exclude src/pydoc_markdown/novella"
 isort = "isort src test --check-only"
 black = "black src test --check"
 
 [tool.slap.run]
 "docs:build" = "cd docs && novella --base-url pydoc-markdown/"
 "docs:dev" = "cd docs && novella --serve"
```

### Comparing `pydoc_markdown-4.8.0/readme.md` & `pydoc_markdown-4.8.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -81,9 +81,11 @@
 Feel free to open a topic on [GitHub Discussions](https://github.com/NiklasRosenstein/pydoc-markdown/discussions)!
 
 ### Projects using Pydoc-Markdown 📚
 
 An incomplete list of projects that use Pydoc-Markdown to generate their API documentation. Feel free to open a
 pull request to add your project to this list!
 
+* [CosmPy](https://docs.fetch.ai/CosmPy/)
+* [haystack by deepset](https://docs.haystack.deepset.ai/reference/agent-api)
 * [tensorchord/envd](https://envd.tensorchord.ai/api/starlark/v0/config.html)
 * [tqdm](https://tqdm.github.io/)
```

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/__init__.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from pydoc_markdown.contrib.processors.filter import FilterProcessor
 from pydoc_markdown.contrib.processors.smart import SmartProcessor
 from pydoc_markdown.contrib.renderers.markdown import MarkdownRenderer
 from pydoc_markdown.interfaces import Builder, Context, Loader, Processor, Renderer, Resolver
 from pydoc_markdown.util import ytemplate
 
 __author__ = "Niklas Rosenstein <rosensteinniklas@gmail.com>"
-__version__ = "4.8.0"
+__version__ = "4.8.1"
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class Hooks:
     pre_render: t.List[str] = dataclasses.field(default_factory=list, metadata={"alias": "pre-render"})
@@ -101,15 +101,21 @@
             filename = arg
             logger.info('Loading configuration file "%s".', filename)
             if filename.endswith(".toml"):
                 data = tomli.loads(Path(filename).read_text())
             else:
                 data = ytemplate.load(filename, {"env": ytemplate.Attributor(os.environ)})
             if filename == "pyproject.toml":
-                data = data["tool"]["pydoc-markdown"]
+                try:
+                    data = data["tool"]["pydoc-markdown"]
+                except KeyError:
+                    raise RuntimeError(
+                        "Could not find configuration in pyproject.toml. Make sure you have a [tool.pydoc-markdown] "
+                        "section, or create a pydoc-markdown.yaml file."
+                    )
         else:
             data = arg
 
         unknown_keys: t.List[t.Tuple[DatabindContext, t.Set[str]]] = []
         result = databind.json.load(
             data,
             type(self),
```

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/loaders/python.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/loaders/python.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/crossref.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/crossref.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/filter.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/filter.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/google.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/google.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/pydocmd.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/pydocmd.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/smart.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/smart.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/sphinx.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/sphinx.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/docusaurus.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/docusaurus.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/hugo.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/hugo.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,28 +42,28 @@
 import yaml
 from databind.core import Remainder
 from nr.util.fs import chmod
 
 from pydoc_markdown.contrib.renderers.markdown import MarkdownRenderer
 from pydoc_markdown.interfaces import Builder, Context, Renderer, Resolver, Server
 from pydoc_markdown.util.knownfiles import KnownFiles
-from pydoc_markdown.util.pages import Page, Pages
+from pydoc_markdown.util.pages import GenericPage, Page, Pages
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class GetHugo:
     enabled: bool = True
     version: t.Optional[str] = None
     extended: bool = True
 
 
 @dataclasses.dataclass
-class HugoPage(Page["HugoPage"]):
+class HugoPage(GenericPage["HugoPage"]):
     """
     A subclass of #Page which adds Hugo-specific overrides.
 
     ### Options
     """
 
     children: t.List["HugoPage"] = dataclasses.field(default_factory=list)
```

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/jinja2.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/jinja2.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/markdown.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/markdown.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/mkdocs.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/mkdocs.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/source_linkers/git.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/source_linkers/git.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/interfaces.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
 
 class PluginBase(abc.ABC):
     def init(self, context: Context) -> None:
         pass
 
 
-# TODO(@NiklasRosenstein): Test that this works as expected.
 @Union(
     [
         "!pydoc_markdown.interfaces.Loader",
         "<import>",
     ],
     style=Union.FLAT,
 )
@@ -91,15 +90,14 @@
     """
 
     @abc.abstractmethod
     def resolve_reference(self, suite: "ApiSuite", scope: docspec.ApiObject, ref: str) -> t.Optional[docspec.ApiObject]:
         ...
 
 
-# TODO(@NiklasRosenstein): Test that this works as expected.
 @Union(
     [
         "!pydoc_markdown.interfaces.Processor",
         "<import>",
     ],
     style=Union.FLAT,
 )
@@ -111,15 +109,14 @@
     """
 
     @abc.abstractmethod
     def process(self, modules: t.List[docspec.Module], resolver: t.Optional[Resolver]) -> None:
         ...
 
 
-# TODO(@NiklasRosenstein): Test that this works as expected.
 @Union(
     [
         "!pydoc_markdown.interfaces.Renderer",
         "<import>",
     ],
     style=Union.FLAT,
 )
@@ -206,15 +203,14 @@
     def build(self, site_dir: str) -> None:
         """
         Invoke the build. The *site_dir* is the directory in which the output files should be
         placed. Otherwise, the directory may be determined by the builder.
         """
 
 
-# TODO(@NiklasRosenstein): Test that this works as expected.
 @Union(
     [
         "!pydoc_markdown.interfaces.SourceLinker",
         "<import>",
     ],
     style=Union.FLAT,
 )
```

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/main.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/main.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/novella/preprocessor.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/novella/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/static.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/static.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/util/docspec.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/util/docspec.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/util/knownfiles.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/util/knownfiles.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/util/misc.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/util/misc.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/util/pages.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/util/pages.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 import shutil
 import typing as t
 
 import docspec
 
 from pydoc_markdown.interfaces import SinglePageRenderer
 
-T_Page = t.TypeVar("T_Page", bound="Page")
+T_Page = t.TypeVar("T_Page", bound="GenericPage")
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class IterHierarchyItem(t.Generic[T_Page]):
     page: "T_Page"
     parent_chain: t.List["T_Page"]
@@ -71,15 +71,15 @@
 class Pages(t.List[T_Page]):
     def iter_hierarchy(self) -> t.Iterable[IterHierarchyItem[T_Page]]:
         for page in self:
             yield from page.iter_hierarchy()
 
 
 @dataclasses.dataclass
-class Page(t.Generic[T_Page]):
+class GenericPage(t.Generic[T_Page]):
     """
     Metadata for a page that a renderer implementation should understand
     in order to produce multiple output files. The page hierarchy defines
     the site navigation as well as the generated files.
     """
 
     #: The title of the page.
@@ -108,15 +108,15 @@
     def __post_init__(self) -> None:
         if not self.name:
             self.name = re.sub(r"\s+", "-", self.title.lower())
 
     def has_content(self) -> bool:
         return bool(self.source or self.contents)
 
-    def iter_hierarchy(self, parent_chain: t.List[Page] | None = None) -> t.Iterable[IterHierarchyItem]:
+    def iter_hierarchy(self, parent_chain: t.List[GenericPage] | None = None) -> t.Iterable[IterHierarchyItem]:
         if parent_chain is None:
             parent_chain = []
         yield IterHierarchyItem(self, parent_chain)
         for child in self.children:
             yield from child.iter_hierarchy(parent_chain + [self])
 
     def filtered_modules(self, modules: t.List[docspec.Module]) -> t.List[docspec.Module]:
@@ -171,11 +171,21 @@
         with open(filename, "w") as fp:
             if write_prefix:
                 write_prefix(fp)
             if self.source:
                 src_path = os.path.join(context_directory, self.source)
                 logger.info('Writing "%s" (source: "%s")', filename, src_path)
                 with open(src_path, "rb") as src:
-                    shutil.copyfileobj(src, fp.buffer)  # type: ignore[misc]  # See https://github.com/python/mypy/issues/15031  # noqa: E501
+                    shutil.copyfileobj(src, fp.buffer)  # type: ignore[misc]  # Fixed in https://github.com/python/mypy/pull/14975  # noqa: E501
             else:
                 logger.info('Rendering "%s"', filename)
                 renderer.render_single_page(fp, self.filtered_modules(modules), self.title)
+
+
+class Page(GenericPage["Page"]):
+    def __class_getitem__(self, item: t.Type[T_Page]) -> t.Type[T_Page]:
+        """
+        For runtime backwards compatibility before Pydoc-Markdown 4.8.1, when the #GenericPage class
+        was still called #Page.
+        """
+
+        return GenericPage[item]  # type: ignore[valid-type,return-value]
```

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/util/watchdog.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/util/watchdog.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/src/pydoc_markdown/util/ytemplate.py` & `pydoc_markdown-4.8.1/src/pydoc_markdown/util/ytemplate.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.0/PKG-INFO` & `pydoc_markdown-4.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoc-markdown
-Version: 4.8.0
+Version: 4.8.1
 Summary: Create Python API documentation in Markdown format.
 License: MIT
 Keywords: documentation,docs,generator,markdown,pydoc
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -17,16 +17,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
 Requires-Dist: PyYAML (>=5.0,<7.0)
 Requires-Dist: click (>=7.1,<9.0)
-Requires-Dist: databind.core (>=4.3.0,<5.0.0)
-Requires-Dist: databind.json (>=4.3.0,<5.0.0)
+Requires-Dist: databind.core (>=4.4.0,<5.0.0)
+Requires-Dist: databind.json (>=4.4.0,<5.0.0)
 Requires-Dist: docspec (>=2.2.1,<3.0.0)
 Requires-Dist: docspec-python (>=2.2.1,<3.0.0)
 Requires-Dist: docstring-parser (>=0.11,<0.12)
 Requires-Dist: jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: nr.util (>=0.7.5,<1.0.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: tomli (>=2.0.0,<3.0.0)
@@ -119,10 +119,12 @@
 Feel free to open a topic on [GitHub Discussions](https://github.com/NiklasRosenstein/pydoc-markdown/discussions)!
 
 ### Projects using Pydoc-Markdown 📚
 
 An incomplete list of projects that use Pydoc-Markdown to generate their API documentation. Feel free to open a
 pull request to add your project to this list!
 
+* [CosmPy](https://docs.fetch.ai/CosmPy/)
+* [haystack by deepset](https://docs.haystack.deepset.ai/reference/agent-api)
 * [tensorchord/envd](https://envd.tensorchord.ai/api/starlark/v0/config.html)
 * [tqdm](https://tqdm.github.io/)
```

