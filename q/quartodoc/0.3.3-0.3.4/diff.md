# Comparing `tmp/quartodoc-0.3.3.tar.gz` & `tmp/quartodoc-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartodoc-0.3.3.tar", last modified: Fri Jun  2 14:27:05 2023, max compression
+gzip compressed data, was "quartodoc-0.3.4.tar", last modified: Wed Jun 21 17:58:07 2023, max compression
```

## Comparing `quartodoc-0.3.3.tar` & `quartodoc-0.3.4.tar`

### file list

```diff
@@ -1,135 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.784204 quartodoc-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.764204 quartodoc-0.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-02 14:26:52.000000 quartodoc-0.3.3/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.764204 quartodoc-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-02 14:26:52.000000 quartodoc-0.3.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-02 14:26:52.000000 quartodoc-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-02 14:26:52.000000 quartodoc-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-02 14:26:52.000000 quartodoc-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-02 14:26:52.000000 quartodoc-0.3.3/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-02 14:26:52.000000 quartodoc-0.3.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-02 14:27:05.784204 quartodoc-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-02 14:26:52.000000 quartodoc-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-02 14:26:52.000000 quartodoc-0.3.3/README.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.760203 quartodoc-0.3.3/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.764204 quartodoc-0.3.3/_extensions/interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 14:26:52.000000 quartodoc-0.3.3/_extensions/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 14:26:52.000000 quartodoc-0.3.3/_extensions/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-02 14:26:52.000000 quartodoc-0.3.3/_extensions/interlinks/interlinks.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.764204 quartodoc-0.3.3/case_studies/
--rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-06-02 14:26:52.000000 quartodoc-0.3.3/case_studies/objects_sqla.inv
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-02 14:26:52.000000 quartodoc-0.3.3/case_studies/parsing.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-02 14:26:52.000000 quartodoc-0.3.3/case_studies/some_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-02 14:26:52.000000 quartodoc-0.3.3/case_studies/sphinx-inventory.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-02 14:26:52.000000 quartodoc-0.3.3/case_studies/sphinx-inventory.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.768204 quartodoc-0.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/about.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.768204 quartodoc-0.3.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/advanced-layouts.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/architecture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/basic-building.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/basic-content.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/basic-docs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/crossrefs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/dev-big-picture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/dev-dataclasses.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/dev-docstrings.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/dev-prepare.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/dev-renderers.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/docstring-examples.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/docstring-style.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/extending.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/extra-build-sequence.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/interlinks.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/sidebar.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/dascore/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/dascore/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/dascore/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/dascore/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/dascore/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/pkgdown/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/pkgdown/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/reference/Builder.build.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/reference/Builder.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/reference/get_object.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/reference/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/reference/preview.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/single-page/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/single-page/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/single-page/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/single-page/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/single-page/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/single-page/reference/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/weird-install/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/weird-install/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.776203 quartodoc-0.3.3/examples/weird-install/src/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/weird-install/src/some_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-02 14:26:52.000000 quartodoc-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.776203 quartodoc-0.3.3/quartodoc/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/autosummary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.776203 quartodoc-0.3.3/quartodoc/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/write.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.780204 quartodoc-0.3.3/quartodoc/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19955 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/renderers/md_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.780204 quartodoc-0.3.3/quartodoc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_alias_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.784204 quartodoc-0.3.3/quartodoc/tests/example_interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.784204 quartodoc-0.3.3/quartodoc/tests/example_interlinks/_inv/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/_inv/other_objects.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/interlinks.lua
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/objects.json
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/spec.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/test.md
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/test.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_builder_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_renderers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.776203 quartodoc-0.3.3/quartodoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-02 14:26:52.000000 quartodoc-0.3.3/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.760203 quartodoc-0.3.3/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.784204 quartodoc-0.3.3/scripts/filter-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-02 14:26:52.000000 quartodoc-0.3.3/scripts/filter-spec/generate_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-02 14:26:52.000000 quartodoc-0.3.3/scripts/filter-spec/generate_test_qmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-02 14:27:05.784204 quartodoc-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.468516 quartodoc-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-21 17:57:57.000000 quartodoc-0.3.4/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-21 17:57:57.000000 quartodoc-0.3.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-21 17:57:57.000000 quartodoc-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-21 17:57:57.000000 quartodoc-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-21 17:57:57.000000 quartodoc-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-21 17:57:57.000000 quartodoc-0.3.4/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-21 17:57:57.000000 quartodoc-0.3.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-21 17:58:07.468516 quartodoc-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-21 17:57:57.000000 quartodoc-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-21 17:57:57.000000 quartodoc-0.3.4/README.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.452516 quartodoc-0.3.4/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/_extensions/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 17:57:57.000000 quartodoc-0.3.4/_extensions/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-21 17:57:57.000000 quartodoc-0.3.4/_extensions/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-21 17:57:57.000000 quartodoc-0.3.4/_extensions/interlinks/interlinks.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/case_studies/
+-rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-06-21 17:57:57.000000 quartodoc-0.3.4/case_studies/objects_sqla.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-21 17:57:57.000000 quartodoc-0.3.4/case_studies/parsing.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-21 17:57:57.000000 quartodoc-0.3.4/case_studies/some_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-21 17:57:57.000000 quartodoc-0.3.4/case_studies/sphinx-inventory.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 17:57:57.000000 quartodoc-0.3.4/case_studies/sphinx-inventory.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/about.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.460516 quartodoc-0.3.4/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/advanced-layouts.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/architecture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/basic-building.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/basic-content.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/basic-docs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/crossrefs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/dev-big-picture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/dev-dataclasses.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/dev-docstrings.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/dev-prepare.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/dev-renderers.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/docstring-examples.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/docstring-style.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/extending.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/extra-build-sequence.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/interlinks.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/sidebar.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.460516 quartodoc-0.3.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.460516 quartodoc-0.3.4/examples/dascore/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/dascore/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/dascore/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/dascore/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/dascore/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.460516 quartodoc-0.3.4/examples/pkgdown/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.460516 quartodoc-0.3.4/examples/pkgdown/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/reference/Builder.build.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/reference/Builder.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/reference/get_object.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/reference/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/reference/preview.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/examples/single-page/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/single-page/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/single-page/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/single-page/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/examples/single-page/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/single-page/reference/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/examples/weird-install/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/weird-install/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/examples/weird-install/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/weird-install/src/some_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-21 17:57:57.000000 quartodoc-0.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/quartodoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20618 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/autosummary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/quartodoc/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/quartodoc/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20066 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/renderers/md_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.468516 quartodoc-0.3.4/quartodoc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_alias_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.468516 quartodoc-0.3.4/quartodoc/tests/example_interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.468516 quartodoc-0.3.4/quartodoc/tests/example_interlinks/_inv/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/_inv/other_objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/interlinks.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/test.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_builder_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/quartodoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-21 17:57:57.000000 quartodoc-0.3.4/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.468516 quartodoc-0.3.4/scripts/filter-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-21 17:57:57.000000 quartodoc-0.3.4/scripts/filter-spec/generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-21 17:57:57.000000 quartodoc-0.3.4/scripts/filter-spec/generate_test_qmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-21 17:58:07.468516 quartodoc-0.3.4/setup.cfg
```

### Comparing `quartodoc-0.3.3/.github/CODE_OF_CONDUCT.md` & `quartodoc-0.3.4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/.github/workflows/ci.yml` & `quartodoc-0.3.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/.gitignore` & `quartodoc-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/LICENSE` & `quartodoc-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/Makefile` & `quartodoc-0.3.4/Makefile`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/PKG-INFO` & `quartodoc-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.3.3
+Version: 0.3.4
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quartodoc-0.3.3/README.md` & `quartodoc-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/README.qmd` & `quartodoc-0.3.4/README.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/_extensions/interlinks/interlinks.lua` & `quartodoc-0.3.4/_extensions/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/case_studies/objects_sqla.inv` & `quartodoc-0.3.4/case_studies/objects_sqla.inv`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/case_studies/parsing.qmd` & `quartodoc-0.3.4/case_studies/parsing.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/case_studies/some_package.py` & `quartodoc-0.3.4/case_studies/some_package.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/case_studies/sphinx-inventory.md` & `quartodoc-0.3.4/case_studies/sphinx-inventory.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/case_studies/sphinx-inventory.qmd` & `quartodoc-0.3.4/case_studies/sphinx-inventory.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/_quarto.yml` & `quartodoc-0.3.4/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/examples/index.qmd` & `quartodoc-0.3.4/docs/examples/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/architecture.qmd` & `quartodoc-0.3.4/docs/get-started/architecture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/basic-building.qmd` & `quartodoc-0.3.4/docs/get-started/basic-building.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/basic-content.qmd` & `quartodoc-0.3.4/docs/get-started/basic-content.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/basic-docs.qmd` & `quartodoc-0.3.4/docs/get-started/basic-docs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/crossrefs.qmd` & `quartodoc-0.3.4/docs/get-started/crossrefs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/dev-big-picture.qmd` & `quartodoc-0.3.4/docs/get-started/dev-big-picture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/dev-docstrings.qmd` & `quartodoc-0.3.4/docs/get-started/dev-docstrings.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/dev-prepare.qmd` & `quartodoc-0.3.4/docs/get-started/dev-prepare.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/dev-renderers.qmd` & `quartodoc-0.3.4/docs/get-started/dev-renderers.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/docstring-examples.qmd` & `quartodoc-0.3.4/docs/get-started/docstring-examples.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/extending.qmd` & `quartodoc-0.3.4/docs/get-started/extending.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/extra-build-sequence.qmd` & `quartodoc-0.3.4/docs/get-started/extra-build-sequence.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/interlinks.qmd` & `quartodoc-0.3.4/docs/get-started/interlinks.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/overview.qmd` & `quartodoc-0.3.4/docs/get-started/overview.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/get-started/sidebar.qmd` & `quartodoc-0.3.4/docs/get-started/sidebar.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/docs/styles.css` & `quartodoc-0.3.4/docs/styles.css`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/examples/dascore/_quarto.yml` & `quartodoc-0.3.4/examples/dascore/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/examples/dascore/generate_api.py` & `quartodoc-0.3.4/examples/dascore/generate_api.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/examples/pkgdown/_quarto.yml` & `quartodoc-0.3.4/examples/pkgdown/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/examples/pkgdown/objects.json` & `quartodoc-0.3.4/examples/pkgdown/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/examples/pkgdown/reference/Builder.qmd` & `quartodoc-0.3.4/examples/pkgdown/reference/Builder.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/examples/pkgdown/reference/get_object.qmd` & `quartodoc-0.3.4/examples/pkgdown/reference/get_object.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/examples/single-page/_quarto.yml` & `quartodoc-0.3.4/examples/single-page/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/examples/single-page/objects.json` & `quartodoc-0.3.4/examples/single-page/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/examples/single-page/reference/index.qmd` & `quartodoc-0.3.4/examples/single-page/reference/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/__main__.py` & `quartodoc-0.3.4/quartodoc/__main__.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/ast.py` & `quartodoc-0.3.4/quartodoc/ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/autosummary.py` & `quartodoc-0.3.4/quartodoc/autosummary.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 from griffe.dataclasses import Alias
 from griffe.docstrings.parsers import Parser, parse
 from griffe.docstrings import dataclasses as ds  # noqa
 from griffe import dataclasses as dc
 from plum import dispatch  # noqa
 from pathlib import Path
 from types import ModuleType
+from pydantic import ValidationError
 
 from .inventory import create_inventory, convert_inventory
 from . import layout
 from .renderers import Renderer
+from .validation import fmt
 
 from typing import Any
 
 
 _log = logging.getLogger(__name__)
 
 
@@ -374,14 +376,17 @@
         The output path for a sidebar yaml config (by default no config generated).
     rewrite_all_pages:
         Whether to rewrite all rendered doc pages, or only those with changes.
     source_dir:
         A directory where source files to be documented live. This is only necessary
         if you are not documenting a package, but collection of scripts. Use a "."
         to refer to the current directory.
+    dynamic:
+        Whether to dynamically load all python objects. By default, objects are
+        loaded using static analysis.
 
     """
 
     # builder dispatching ----
     style: str
     _registry: "dict[str, Builder]" = {}
 
@@ -416,14 +421,15 @@
         dir: str = "reference",
         title: str = "Function reference",
         renderer: "dict | Renderer | str" = "markdown",
         out_index: str = None,
         sidebar: "str | None" = None,
         rewrite_all_pages=False,
         source_dir: "str | None" = None,
+        dynamic: bool | None = None,
     ):
         self.layout = self.load_layout(sections=sections, package=package)
 
         self.package = package
         self.version = None
         self.dir = dir
         self.title = title
@@ -432,20 +438,28 @@
         self.renderer = Renderer.from_config(renderer)
 
         if out_index is not None:
             self.out_index = out_index
 
         self.rewrite_all_pages = rewrite_all_pages
         self.source_dir = str(Path(source_dir).absolute()) if source_dir else None
+        self.dynamic = dynamic
 
     def load_layout(self, sections: dict, package: str):
         # TODO: currently returning the list of sections, to make work with
         # previous code. We should make Layout a first-class citizen of the
         # process.
-        return layout.Layout(sections=sections, package=package)
+        try:
+            return layout.Layout(sections=sections, package=package)
+        except ValidationError as e:
+            msg = 'Configuration error for YAML:\n - '
+            errors = [fmt(err) for err in e.errors() if fmt(err)]
+            first_error = errors[0] # we only want to show one error at a time b/c it is confusing otherwise
+            msg += first_error           
+            raise ValueError(msg) from None
 
     # building ----------------------------------------------------------------
 
     def build(self, filter: str = "*"):
         """Build index page, sphinx inventory, and individual doc pages.
 
         Parameters
@@ -462,15 +476,15 @@
             import sys
 
             sys.path.append(self.source_dir)
 
         # shaping and collection ----
 
         _log.info("Generating blueprint.")
-        blueprint = blueprint(self.layout)
+        blueprint = blueprint(self.layout, dynamic=self.dynamic)
 
         _log.info("Collecting pages and inventory items.")
         pages, items = collect(blueprint, base_dir=self.dir)
 
         # writing pages ----
 
         _log.info("Writing index")
@@ -556,15 +570,16 @@
         for section in blueprint.sections:
             links = []
             for entry in section.contents:
                 links.extend(self._page_to_links(entry))
 
             contents.append({"section": section.title, "contents": links})
 
-        return {"website": {"sidebar": {"id": self.dir, "contents": contents}}}
+        entries = [{"id": self.dir, "contents": contents}, {"id": "dummy-sidebar"}]
+        return {"website": {"sidebar": entries}}
 
     def write_sidebar(self, blueprint: layout.Layout):
         """Write a yaml config file for API sidebar."""
 
         d_sidebar = self._generate_sidebar(blueprint)
         yaml.dump(d_sidebar, open(self.sidebar, "w"))
```

### Comparing `quartodoc-0.3.3/quartodoc/builder/blueprint.py` & `quartodoc-0.3.4/quartodoc/builder/blueprint.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
                 lines_collection=LinesCollection(),
             )
             self.get_object = partial(_get_object, loader=loader)
         else:
             self.get_object = get_object
 
         self.crnt_package = None
+        self.dynamic = None
 
     @staticmethod
     def _append_member_path(path: str, new: str):
         if ":" in path:
             return f"{path}.{new}"
 
         return f"{path}:{new}"
@@ -105,28 +106,30 @@
         if pkg is None:
             path = el.name
         else:
             path = f"{pkg}.{el.name}" if ":" in el.name else f"{pkg}:{el.name}"
 
         _log.info(f"Getting object for {path}")
 
-        obj = self.get_object_fixed(path, dynamic=el.dynamic)
+        dynamic = el.dynamic if el.dynamic is not None else self.dynamic
+
+        obj = self.get_object_fixed(path, dynamic=dynamic)
         raw_members = self._fetch_members(el, obj)
 
         # Three cases for structuring child methods ----
 
         children = []
         for entry in raw_members:
             # Note that we could have iterated over obj.members, but currently
             # if obj is an Alias to a class, then its members are not Aliases,
             # but the actual objects on the target.
             # On the other hand, we've wired get_object up to make sure getting
             # the member of an Alias also returns an Alias.
             member_path = self._append_member_path(path, entry)
-            obj_member = self.get_object_fixed(member_path, dynamic=el.dynamic)
+            obj_member = self.get_object_fixed(member_path, dynamic=dynamic)
 
             # do no document submodules
             if obj_member.kind.value == "module":
                 continue
 
             # create element for child ----
             doc = Doc.from_griffe(obj_member.name, obj_member)
@@ -194,23 +197,25 @@
 
 
 @overload
 def blueprint(el: Auto, package: str) -> Doc:
     ...
 
 
-def blueprint(el: _Base, package: str = None) -> _Base:
+def blueprint(el: _Base, package: str = None, dynamic: None | bool = None) -> _Base:
     """Convert a configuration element to something that is ready to render.
 
     Parameters
     ----------
     el:
         An element, like layout.Auto, to transform.
     package:
         A base package name. If specified, this is prepended to the names of any objects.
+    dynamic:
+        Whether to dynamically load objects. Defaults to using static analysis.
 
     Examples
     --------
 
     >>> from quartodoc import blueprint
     >>> from quartodoc.layout import Auto
     >>> blueprint(Auto(name = "quartodoc.get_object"))
@@ -222,14 +227,17 @@
     """
 
     trans = BlueprintTransformer()
 
     if package is not None:
         trans.crnt_package = package
 
+    if dynamic is not None:
+        trans.dynamic = dynamic
+
     return trans.visit(el)
 
 
 def strip_package_name(el: _Base, package: str):
     """Removes leading package name from layout Pages."""
 
     stripper = _PagePackageStripper(package)
```

### Comparing `quartodoc-0.3.3/quartodoc/builder/collect.py` & `quartodoc-0.3.4/quartodoc/builder/collect.py`

 * *Files 25% similar despite different names*

```diff
@@ -35,18 +35,33 @@
 
     @dispatch
     def exit(self, el: layout.Doc):
         page_node = self.find_page_node()
         p_el = page_node.value
 
         uri = f"{self.base_dir}/{p_el.path}.html#{el.anchor}"
+
+        name_path = el.obj.path
+        canonical_path = el.obj.canonical_path
+
+        # item corresponding to the specified path ----
+        # e.g. this might be a top-level import
         self.items.append(
-            layout.Item(name=el.obj.path, obj=el.obj, uri=uri, dispname=None)
+            layout.Item(name=name_path, obj=el.obj, uri=uri, dispname=None)
         )
 
+        if name_path != canonical_path:
+            # item corresponding to the canonical path ----
+            # this is where the object is defined (which may be deep in a submodule)
+            self.items.append(
+                layout.Item(
+                    name=canonical_path, obj=el.obj, uri=uri, dispname=name_path
+                )
+            )
+
         return el
 
     @dispatch
     def exit(self, el: layout.Page):
         self.pages.append(el)
 
         return el
```

### Comparing `quartodoc-0.3.3/quartodoc/builder/utils.py` & `quartodoc-0.3.4/quartodoc/builder/utils.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/interlinks.py` & `quartodoc-0.3.4/quartodoc/interlinks.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/inventory.py` & `quartodoc-0.3.4/quartodoc/inventory.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/layout.py` & `quartodoc-0.3.4/quartodoc/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 
     kind: Literal["auto"] = "auto"
     name: str
     members: Optional[list[str]] = None
     include_private: bool = False
     include: Optional[str] = None
     exclude: Optional[str] = None
-    dynamic: Union[bool, str] = False
+    dynamic: Union[None, bool, str] = None
     children: ChoicesChildren = ChoicesChildren.embedded
     package: Union[str, None, MISSING] = MISSING()
 
 
 # TODO: rename to Default or something
 class _AutoDefault(_Base):
     """This hacky class allows creating Auto as a default option in Pages and Sections."""
```

### Comparing `quartodoc-0.3.3/quartodoc/renderers/base.py` & `quartodoc-0.3.4/quartodoc/renderers/base.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/renderers/md_renderer.py` & `quartodoc-0.3.4/quartodoc/renderers/md_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,19 @@
         elif self.display_name == "full":
             return el.path
 
         elif self.display_name == "canonical":
             return el.canonical_path
 
         raise ValueError(f"Unsupported display_name: `{self.display_name}`")
+    
+    def _render_table(self, rows, headers):
+        table = tabulate(rows, headers=headers, tablefmt="github")
+
+        return table
 
     def render_annotation(self, el: "str | expr.Name | expr.Expression | None"):
         """Special hook for rendering a type annotation.
 
         Parameters
         ----------
         el:
@@ -407,15 +412,15 @@
     # parameters ----
 
     @dispatch
     def render(self, el: ds.DocstringSectionParameters):
         rows = list(map(self.render, el.value))
         header = ["Name", "Type", "Description", "Default"]
 
-        return tabulate(rows, header, tablefmt="github")
+        return self._render_table(rows, header)
 
     @dispatch
     def render(self, el: ds.DocstringParameter) -> Tuple[str]:
         # TODO: if default is not, should return the word "required" (unescaped)
         default = "required" if el.default is None else escape(el.default)
 
         annotation = self.render_annotation(el.annotation)
@@ -425,15 +430,15 @@
     # attributes ----
 
     @dispatch
     def render(self, el: ds.DocstringSectionAttributes):
         header = ["Name", "Type", "Description"]
         rows = list(map(self.render, el.value))
 
-        return tabulate(rows, header, tablefmt="github")
+        return self._render_table(rows, header)
 
     @dispatch
     def render(self, el: ds.DocstringAttribute):
         annotation = self.render_annotation(el.annotation)
         row = [
             sanitize(el.name),
             self.render_annotation(annotation),
@@ -481,15 +486,15 @@
     # returns ----
 
     @dispatch
     def render(self, el: Union[ds.DocstringSectionReturns, ds.DocstringSectionRaises]):
         rows = list(map(self.render, el.value))
         header = ["Type", "Description"]
 
-        return tabulate(rows, header, tablefmt="github")
+        return self._render_table(rows, header)
 
     @dispatch
     def render(self, el: Union[ds.DocstringReturn, ds.DocstringRaise]):
         # similar to DocstringParameter, but no name or default
         annotation = self.render_annotation(el.annotation)
         return (annotation, sanitize(el.description, allow_markdown=True))
```

### Comparing `quartodoc-0.3.3/quartodoc/tests/example_dynamic.py` & `quartodoc-0.3.4/quartodoc/tests/example_dynamic.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/tests/example_interlinks/interlinks.lua` & `quartodoc-0.3.4/quartodoc/tests/example_interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/tests/example_interlinks/objects.json` & `quartodoc-0.3.4/quartodoc/tests/example_interlinks/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/tests/example_interlinks/spec.yml` & `quartodoc-0.3.4/quartodoc/tests/example_interlinks/spec.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/tests/example_interlinks/test.md` & `quartodoc-0.3.4/quartodoc/tests/example_interlinks/test.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/tests/example_interlinks/test.qmd` & `quartodoc-0.3.4/quartodoc/tests/example_interlinks/test.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/tests/test_ast.py` & `quartodoc-0.3.4/quartodoc/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/tests/test_basic.py` & `quartodoc-0.3.4/quartodoc/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/tests/test_builder.py` & `quartodoc-0.3.4/quartodoc/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/tests/test_builder_blueprint.py` & `quartodoc-0.3.4/quartodoc/tests/test_builder_blueprint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from quartodoc import get_object
 from quartodoc import layout as lo
-from quartodoc.builder.blueprint import BlueprintTransformer
+from quartodoc.builder.blueprint import BlueprintTransformer, blueprint
 import pytest
 
 TEST_MOD = "quartodoc.tests.example"
 
 
 @pytest.fixture
 def lay():
@@ -68,14 +68,25 @@
 
     assert isinstance(res, lo.DocModule)
     assert len(res.members) == 1
     assert res.members[0].name == "a_func"
     assert res.members[0].obj.path == path.replace(":", ".") + ".a_func"
 
 
+def test_blueprint_default_dynamic(bp):
+    from quartodoc.tests.example_dynamic import NOTE
+
+    path = "quartodoc.tests.example_dynamic:f"
+    auto = lo.Auto(name=path)
+
+    res = blueprint(auto, dynamic=True)
+    assert isinstance(res, lo.DocFunction)
+    assert NOTE in res.obj.docstring.value
+
+
 def test_blueprint_auto_package(bp):
     auto = lo.Auto(name="a_func", package="quartodoc.tests.example")
     res = bp.visit(auto)
 
     assert isinstance(res, lo.DocFunction)
     assert res.name == "a_func"
     assert res.anchor == "quartodoc.tests.example.a_func"
```

### Comparing `quartodoc-0.3.3/quartodoc/tests/test_interlinks.py` & `quartodoc-0.3.4/quartodoc/tests/test_interlinks.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/tests/test_layout.py` & `quartodoc-0.3.4/quartodoc/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc/tests/test_renderers.py` & `quartodoc-0.3.4/quartodoc/tests/test_renderers.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/quartodoc.egg-info/PKG-INFO` & `quartodoc-0.3.4/quartodoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.3.3
+Version: 0.3.4
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quartodoc-0.3.3/quartodoc.egg-info/SOURCES.txt` & `quartodoc-0.3.4/quartodoc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 quartodoc/__init__.py
 quartodoc/__main__.py
 quartodoc/ast.py
 quartodoc/autosummary.py
 quartodoc/interlinks.py
 quartodoc/inventory.py
 quartodoc/layout.py
+quartodoc/validation.py
 quartodoc.egg-info/PKG-INFO
 quartodoc.egg-info/SOURCES.txt
 quartodoc.egg-info/dependency_links.txt
 quartodoc.egg-info/entry_points.txt
 quartodoc.egg-info/requires.txt
 quartodoc.egg-info/top_level.txt
 quartodoc/builder/__init__.py
@@ -91,14 +92,15 @@
 quartodoc/tests/test_ast.py
 quartodoc/tests/test_basic.py
 quartodoc/tests/test_builder.py
 quartodoc/tests/test_builder_blueprint.py
 quartodoc/tests/test_interlinks.py
 quartodoc/tests/test_layout.py
 quartodoc/tests/test_renderers.py
+quartodoc/tests/test_validation.py
 quartodoc/tests/example_interlinks/.gitignore
 quartodoc/tests/example_interlinks/README.md
 quartodoc/tests/example_interlinks/_quarto.yml
 quartodoc/tests/example_interlinks/interlinks.lua
 quartodoc/tests/example_interlinks/objects.json
 quartodoc/tests/example_interlinks/spec.yml
 quartodoc/tests/example_interlinks/test.md
```

### Comparing `quartodoc-0.3.3/requirements-dev.txt` & `quartodoc-0.3.4/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/scripts/filter-spec/generate_files.py` & `quartodoc-0.3.4/scripts/filter-spec/generate_files.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.3/setup.cfg` & `quartodoc-0.3.4/setup.cfg`

 * *Files identical despite different names*

