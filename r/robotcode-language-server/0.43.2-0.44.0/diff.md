# Comparing `tmp/robotcode_language_server-0.43.2.tar.gz` & `tmp/robotcode_language_server-0.44.0.tar.gz`

## Comparing `robotcode_language_server-0.43.2.tar` & `robotcode_language_server-0.44.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    18981 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    38247 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    58384 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    67010 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83614 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    85311 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    42861 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/pyproject.toml
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    19251 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    38247 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    58384 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    67010 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83614 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    85370 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    42861 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/pyproject.toml
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     TextDocumentSyncKind,
     TextDocumentSyncOptions,
     TraceValues,
     Unregistration,
     UnregistrationParams,
     WorkspaceFolder,
 )
+from robotcode.core.utils.process import pid_exists
 from robotcode.jsonrpc2.protocol import (
     JsonRPCErrorException,
     JsonRPCErrors,
     JsonRPCException,
     JsonRPCProtocol,
     ProtocolPartDescriptor,
     rpc_method,
@@ -110,15 +111,15 @@
 
     file_extensions: ClassVar[Set[str]] = set()
     languages: ClassVar[List[LanguageDefinition]] = []
 
     def __init__(self, server: JsonRPCServer[Any]):
         super().__init__()
         self.server = server
-
+        self.parent_process_id: Optional[int] = None
         self.initialization_options: Any = None
         self.client_info: Optional[InitializeParamsClientInfoType] = None
         self._workspace: Optional[Workspace] = None
         self.client_capabilities: Optional[ClientCapabilities] = None
         self.shutdown_received = False
         self._capabilities: Optional[ServerCapabilities] = None
         self._base_capabilities = ServerCapabilities(
@@ -170,29 +171,48 @@
 
         for p in self.registry.parts:
             if isinstance(p, HasExtendCapabilities):
                 p.extend_capabilities(base_capabilities)
 
         return base_capabilities
 
+    PARENT_PROCESS_WATCHER_INTERVAL = 5
+
+    def start_parent_process_watcher(self) -> None:
+        if self.parent_process_id and self.loop:
+            self.loop.call_later(self.PARENT_PROCESS_WATCHER_INTERVAL, self._parent_process_watcher)
+
+    def _parent_process_watcher(self) -> None:
+        if not self.parent_process_id:
+            return
+        if not pid_exists(self.parent_process_id):
+            self.__logger.error(lambda: f"Parent process {self.parent_process_id} is dead, exiting...")
+            exit(2)
+        self.start_parent_process_watcher()
+
     @rpc_method(name="initialize", param_type=InitializeParams)
     @__logger.call
     async def _initialize(
         self,
         capabilities: ClientCapabilities,
         root_path: Optional[str] = None,
         root_uri: Optional[str] = None,
         initialization_options: Optional[Any] = None,
         trace: Optional[TraceValues] = None,
         client_info: Optional[InitializeParamsClientInfoType] = None,
         workspace_folders: Optional[List[WorkspaceFolder]] = None,
         work_done_token: Optional[ProgressToken] = None,
+        process_id: Optional[int] = None,
         *args: Any,
         **kwargs: Any,
     ) -> InitializeResult:
+        self.parent_process_id = process_id
+        if self.parent_process_id and pid_exists(self.parent_process_id):
+            self.start_parent_process_watcher()
+
         self.trace = trace or TraceValues.OFF
         self.client_info = client_info
 
         self.client_capabilities = capabilities
 
         self._workspace = Workspace(self, root_uri=root_uri, root_path=root_path, workspace_folders=workspace_folders)
```

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,10 +157,8 @@
                     results.append(result)
 
         if not results:
             return params
 
         if len(results) > 1:
             self._logger.warning("More then one resolve result. Use the last one.")
-        result = results[-1]
-
-        return result
+        return results[-1]
```

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,20 @@
             document = self._documents.get(uri, None)
 
             normalized_text = self._normalize_line_endings(text_document.text)
 
             if document is None:
                 text_changed = False
                 document = await self._create_document(
-                    text_document.uri, normalized_text, text_document.language_id, text_document.version
+                    text_document.uri,
+                    normalized_text,
+                    text_document.language_id
+                    if text_document.language_id
+                    else self.detect_language_id(text_document.uri),
+                    text_document.version,
                 )
 
                 self._documents[uri] = document
             else:
                 text_changed = document.text() != normalized_text
                 if text_changed:
                     document.apply_full_change(text_document.version, normalized_text)
```

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     WorkspaceFoldersServerCapabilities,
 )
 from robotcode.core.lsp.types import (
     WorkspaceFolder as TypesWorkspaceFolder,
 )
 from robotcode.core.uri import Uri
 from robotcode.core.utils.path import path_is_relative_to
-from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.jsonrpc2.protocol import JsonRPCErrorException, rpc_method
 from robotcode.language_server.common.has_extend_capabilities import (
     HasExtendCapabilities,
 )
 
 from .protocol_part import LanguageServerProtocolPart
 
 if TYPE_CHECKING:
@@ -347,28 +347,34 @@
     ) -> Optional[Any]:
         if (
             self.parent.client_capabilities
             and self.parent.client_capabilities.workspace
             and self.parent.client_capabilities.workspace.configuration
             and request
         ):
-            r = await self.parent.send_request_async(
-                "workspace/configuration",
-                ConfigurationParams(
-                    items=[
-                        ConfigurationItem(
-                            scope_uri=str(scope_uri) if isinstance(scope_uri, Uri) else scope_uri,
-                            section=section,
-                        )
-                    ]
-                ),
-                list,
-            )
-
-            return r[0] if r is not None else None
+            try:
+                r = await self.parent.send_request_async(
+                    "workspace/configuration",
+                    ConfigurationParams(
+                        items=[
+                            ConfigurationItem(
+                                scope_uri=str(scope_uri) if isinstance(scope_uri, Uri) else scope_uri,
+                                section=section,
+                            )
+                        ]
+                    ),
+                    list,
+                )
+
+                return r[0] if r is not None else None
+            except asyncio.CancelledError:
+                raise
+            except JsonRPCErrorException as e:
+                self._logger.warning(str(e))
+                pass
 
         result = self.settings
         for sub_key in str(section).split("."):
             if sub_key in result:
                 result = result.get(sub_key, None)
             else:
                 result = {}
```

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, Final, List, Optional
+from typing import TYPE_CHECKING, Any, ClassVar, Dict, Final, List, Optional, Set
 
 from robotcode.core.dataclasses import CamelSnakeMixin, from_dict
 from robotcode.core.logging import LoggingDescriptor
 from robotcode.core.lsp.types import InitializeError
 from robotcode.jsonrpc2.protocol import JsonRPCErrorException, JsonRPCErrors, ProtocolPartDescriptor
 from robotcode.language_server.common.parts.document_symbols import symbol_information_label
 from robotcode.language_server.common.protocol import LanguageDefinition, LanguageServerProtocol
@@ -102,17 +102,17 @@
 
     robot_debugging_utils = ProtocolPartDescriptor(RobotDebuggingUtilsProtocolPart)
 
     name = "RobotCode Language Server"
     short_name = "RobotCode"
     version = __version__
 
-    file_extensions = {"robot", "resource", "py", "yaml", "yml"}
+    file_extensions: ClassVar[Set[str]] = {"robot", "resource", "py", "yaml", "yml"}
 
-    languages = [
+    languages: ClassVar[List[LanguageDefinition]] = [
         LanguageDefinition(
             id="robotframework",
             extensions=[".robot", ".resource"],
             aliases=["Robot Framework", "robotframework"],
         ),
         # LanguageDefinition(
         #     id="feature",
```

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/server.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                         "...",
                         "editor.action.showReferences",
                         [str(document.uri), code_lens.range.start, []],
                     )
 
                     async def find_refs() -> None:
                         if document is None or kw_doc is None:
-                            return
+                            return  #  type: ignore[unreachable]
 
                         await self.parent.robot_references.find_keyword_references(
                             document, kw_doc, include_declaration=False
                         )
 
                         await self.parent.code_lens.refresh()
```

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
+    ClassVar,
     Dict,
     Iterable,
     Iterator,
     List,
     Optional,
     Tuple,
     Type,
@@ -447,15 +448,15 @@
                 )
                 if range is not None
                 else None,
             )
             for s in self.namespace.imports_manager.environment.keys()
         ]
 
-    _VARIABLE_COMPLETION_SORT_TEXT_PREFIX = {
+    _VARIABLE_COMPLETION_SORT_TEXT_PREFIX: ClassVar[Dict[VariableDefinitionType, str]] = {
         VariableDefinitionType.LOCAL_VARIABLE: "033",
         VariableDefinitionType.ARGUMENT: "034",
         VariableDefinitionType.VARIABLE: "035",
         VariableDefinitionType.IMPORTED_VARIABLE: "036",
         VariableDefinitionType.COMMAND_LINE_VARIABLE: "037",
         VariableDefinitionType.BUILTIN_VARIABLE: "038",
         VariableDefinitionType.ENVIRONMENT_VARIABLE: "039",
```

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.44.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/.gitignore` & `robotcode_language_server-0.44.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/LICENSE.txt` & `robotcode_language_server-0.44.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/README.md` & `robotcode_language_server-0.44.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.2/pyproject.toml` & `robotcode_language_server-0.44.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.43.2",
-  "robotcode==0.43.2",
+  "robotcode-jsonrpc2==0.44.0",
+  "robotcode==0.44.0",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 langserver = "robotcode.language_server.hooks"
 
 [project.urls]
```

### Comparing `robotcode_language_server-0.43.2/PKG-INFO` & `robotcode_language_server-0.44.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.43.2
+Version: 0.44.0
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.43.2
-Requires-Dist: robotcode==0.43.2
+Requires-Dist: robotcode-jsonrpc2==0.44.0
+Requires-Dist: robotcode==0.44.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

