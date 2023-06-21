# Comparing `tmp/conan-server-2.0.6.tar.gz` & `tmp/conan-server-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/conan-server-2.0.6.tar", last modified: Fri May 26 11:31:08 2023, max compression
+gzip compressed data, was "dist/conan-server-2.0.7.tar", last modified: Wed Jun 21 11:09:20 2023, max compression
```

## Comparing `conan-server-2.0.6.tar` & `conan-server-2.0.7.tar`

### file list

```diff
@@ -1,403 +1,403 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.781996 conan-server-2.0.6/
--rw-r--r--   0 root         (0) root         (0)     1084 2023-05-26 11:30:56.000000 conan-server-2.0.6/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-26 11:30:56.000000 conan-server-2.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8156 2023-05-26 11:31:08.781996 conan-server-2.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6041 2023-05-26 11:30:56.000000 conan-server-2.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.741993 conan-server-2.0.6/conan/
--rw-r--r--   0 root         (0) root         (0)      152 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.742993 conan-server-2.0.6/conan/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/conan_api.py
--rw-r--r--   0 root         (0) root         (0)     5892 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/model.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.744993 conan-server-2.0.6/conan/api/subapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4308 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/cache.py
--rw-r--r--   0 root         (0) root         (0)     1101 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/config.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/download.py
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/export.py
--rw-r--r--   0 root         (0) root         (0)    11124 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/graph.py
--rw-r--r--   0 root         (0) root         (0)     3131 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/install.py
--rw-r--r--   0 root         (0) root         (0)     7652 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/list.py
--rw-r--r--   0 root         (0) root         (0)     5110 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/local.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/lockfile.py
--rw-r--r--   0 root         (0) root         (0)     4864 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/new.py
--rw-r--r--   0 root         (0) root         (0)     4426 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/profiles.py
--rw-r--r--   0 root         (0) root         (0)     4478 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/remotes.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/remove.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/search.py
--rw-r--r--   0 root         (0) root         (0)     3907 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/api/subapi/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.744993 conan-server-2.0.6/conan/cli/
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7582 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/args.py
--rw-r--r--   0 root         (0) root         (0)    11009 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     6522 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.747993 conan-server-2.0.6/conan/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3311 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/build.py
--rw-r--r--   0 root         (0) root         (0)     4419 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/cache.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)     8409 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/create.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/download.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/editable.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/export.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/export_pkg.py
--rw-r--r--   0 root         (0) root         (0)     8632 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/graph.py
--rw-r--r--   0 root         (0) root         (0)     2233 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/inspect.py
--rw-r--r--   0 root         (0) root         (0)     4787 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)     5192 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/list.py
--rw-r--r--   0 root         (0) root         (0)     5485 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/lock.py
--rw-r--r--   0 root         (0) root         (0)     4239 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/new.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/profile.py
--rw-r--r--   0 root         (0) root         (0)    11410 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/remote.py
--rw-r--r--   0 root         (0) root         (0)     2595 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/remove.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/search.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/source.py
--rw-r--r--   0 root         (0) root         (0)     3717 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/test.py
--rw-r--r--   0 root         (0) root         (0)     3830 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/commands/upload.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/exit_codes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.747993 conan-server-2.0.6/conan/cli/formatters/
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/formatters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.748993 conan-server-2.0.6/conan/cli/formatters/graph/
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/formatters/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4951 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/formatters/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     1703 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/formatters/graph/graph_info_text.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/formatters/graph/info_graph_dot.py
--rw-r--r--   0 root         (0) root         (0)     5583 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/formatters/graph/info_graph_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.748993 conan-server-2.0.6/conan/cli/formatters/list/
--rw-r--r--   0 root         (0) root         (0)       37 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/formatters/list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/formatters/list/binary_html_table.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/formatters/list/list.py
--rw-r--r--   0 root         (0) root         (0)    12834 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/formatters/list/search_table_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.748993 conan-server-2.0.6/conan/cli/printers/
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/printers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/cli/printers/graph.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.749994 conan-server-2.0.6/conan/internal/
--rw-r--r--   0 root         (0) root         (0)      419 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.749994 conan-server-2.0.6/conan/internal/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.751994 conan-server-2.0.6/conan/internal/api/new/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/alias_new.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/autoools_exe.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/autotools_lib.py
--rw-r--r--   0 root         (0) root         (0)     2843 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/basic.py
--rw-r--r--   0 root         (0) root         (0)     2066 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/bazel_exe.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/bazel_lib.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/cmake_exe.py
--rw-r--r--   0 root         (0) root         (0)     7076 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/cmake_lib.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/meson_exe.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/meson_lib.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/msbuild_exe.py
--rw-r--r--   0 root         (0) root         (0)    12247 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/api/new/msbuild_lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.751994 conan-server-2.0.6/conan/internal/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10247 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/cache/conan_reference_layout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.751994 conan-server-2.0.6/conan/internal/cache/db/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/cache/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3842 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/cache/db/cache_database.py
--rw-r--r--   0 root         (0) root         (0)     7953 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/cache/db/packages_table.py
--rw-r--r--   0 root         (0) root         (0)     5264 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/cache/db/recipes_table.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/cache/db/table.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/conan_app.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/deploy.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/internal/integrity_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.752994 conan-server-2.0.6/conan/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.752994 conan-server-2.0.6/conan/tools/android/
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/android/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1138 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/android/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.752994 conan-server-2.0.6/conan/tools/apple/
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/apple/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11201 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/apple/apple.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/apple/xcodebuild.py
--rw-r--r--   0 root         (0) root         (0)    16380 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/apple/xcodedeps.py
--rw-r--r--   0 root         (0) root         (0)     5683 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/apple/xcodetoolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.753994 conan-server-2.0.6/conan/tools/build/
--rw-r--r--   0 root         (0) root         (0)     4143 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11104 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/build/cppstd.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/build/cpu.py
--rw-r--r--   0 root         (0) root         (0)     2043 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/build/cross_building.py
--rw-r--r--   0 root         (0) root         (0)    15410 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/build/flags.py
--rw-r--r--   0 root         (0) root         (0)      563 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/build/stdcpp_library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.754994 conan-server-2.0.6/conan/tools/cmake/
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9963 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/cmake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.754994 conan-server-2.0.6/conan/tools/cmake/cmakedeps/
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/cmakedeps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8152 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/cmakedeps/cmakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.755994 conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/
--rw-r--r--   0 root         (0) root         (0)     4273 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4451 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/config.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/config_version.py
--rw-r--r--   0 root         (0) root         (0)     5704 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/macros.py
--rw-r--r--   0 root         (0) root         (0)    14925 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/target_configuration.py
--rw-r--r--   0 root         (0) root         (0)    19484 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/target_data.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/targets.py
--rw-r--r--   0 root         (0) root         (0)     5365 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/file_api.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/layout.py
--rw-r--r--   0 root         (0) root         (0)    14423 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/presets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.755994 conan-server-2.0.6/conan/tools/cmake/toolchain/
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/toolchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35919 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/toolchain/blocks.py
--rw-r--r--   0 root         (0) root         (0)    11205 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/toolchain/toolchain.py
--rw-r--r--   0 root         (0) root         (0)      171 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/cmake/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.756994 conan-server-2.0.6/conan/tools/env/
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25389 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/env/environment.py
--rw-r--r--   0 root         (0) root         (0)     3233 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/env/virtualbuildenv.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/env/virtualrunenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.757994 conan-server-2.0.6/conan/tools/files/
--rw-r--r--   0 root         (0) root         (0)      572 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1468 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/files/conandata.py
--rw-r--r--   0 root         (0) root         (0)     6009 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/files/copy_pattern.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/files/cpp_package.py
--rw-r--r--   0 root         (0) root         (0)    24621 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/files/files.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/files/packager.py
--rw-r--r--   0 root         (0) root         (0)     5824 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/files/patches.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.757994 conan-server-2.0.6/conan/tools/files/symlinks/
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/files/symlinks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/files/symlinks/symlinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.758994 conan-server-2.0.6/conan/tools/gnu/
--rw-r--r--   0 root         (0) root         (0)      274 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/gnu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6234 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/gnu/autotools.py
--rw-r--r--   0 root         (0) root         (0)     2954 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/gnu/autotoolsdeps.py
--rw-r--r--   0 root         (0) root         (0)    13228 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/gnu/autotoolstoolchain.py
--rw-r--r--   0 root         (0) root         (0)     3557 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/gnu/get_gnu_triplet.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/gnu/gnudeps_flags.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/gnu/pkgconfig.py
--rw-r--r--   0 root         (0) root         (0)    17816 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/gnu/pkgconfigdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.759995 conan-server-2.0.6/conan/tools/google/
--rw-r--r--   0 root         (0) root         (0)      201 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/google/bazel.py
--rw-r--r--   0 root         (0) root         (0)    10956 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/google/bazeldeps.py
--rw-r--r--   0 root         (0) root         (0)      585 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/google/layout.py
--rw-r--r--   0 root         (0) root         (0)      857 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/google/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.759995 conan-server-2.0.6/conan/tools/intel/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/intel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/intel/intel_cc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.759995 conan-server-2.0.6/conan/tools/layout/
--rw-r--r--   0 root         (0) root         (0)      605 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/layout/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.759995 conan-server-2.0.6/conan/tools/meson/
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/meson/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4073 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/meson/helpers.py
--rw-r--r--   0 root         (0) root         (0)     3880 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/meson/meson.py
--rw-r--r--   0 root         (0) root         (0)    22075 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/meson/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.761995 conan-server-2.0.6/conan/tools/microsoft/
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/microsoft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/microsoft/layout.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/microsoft/msbuild.py
--rw-r--r--   0 root         (0) root         (0)    19194 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/microsoft/msbuilddeps.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/microsoft/nmakedeps.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/microsoft/nmaketoolchain.py
--rw-r--r--   0 root         (0) root         (0)      596 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/microsoft/subsystems.py
--rw-r--r--   0 root         (0) root         (0)    10844 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/microsoft/toolchain.py
--rw-r--r--   0 root         (0) root         (0)    13070 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/microsoft/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.761995 conan-server-2.0.6/conan/tools/premake/
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/premake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/premake/premake.py
--rw-r--r--   0 root         (0) root         (0)    10534 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/premake/premakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.761995 conan-server-2.0.6/conan/tools/qbs/
--rw-r--r--   0 root         (0) root         (0)      152 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/qbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/qbs/qbs.py
--rw-r--r--   0 root         (0) root         (0)     9874 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/qbs/qbsprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.762995 conan-server-2.0.6/conan/tools/scm/
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/scm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8619 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/scm/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.762995 conan-server-2.0.6/conan/tools/system/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16286 2023-05-26 11:30:56.000000 conan-server-2.0.6/conan/tools/system/package_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.763995 conan-server-2.0.6/conan_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8156 2023-05-26 11:31:08.000000 conan-server-2.0.6/conan_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10669 2023-05-26 11:31:08.000000 conan-server-2.0.6/conan_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 11:31:08.000000 conan-server-2.0.6/conan_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-26 11:31:08.000000 conan-server-2.0.6/conan_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      527 2023-05-26 11:31:08.000000 conan-server-2.0.6/conan_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 11:31:08.000000 conan-server-2.0.6/conan_server.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.764995 conan-server-2.0.6/conans/
--rw-r--r--   0 root         (0) root         (0)      201 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.765995 conan-server-2.0.6/conans/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.765995 conan-server-2.0.6/conans/client/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10687 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/cache/editable.py
--rw-r--r--   0 root         (0) root         (0)     6569 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/cache/remote_registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.766995 conan-server-2.0.6/conans/client/cmd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/cmd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7671 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/cmd/export.py
--rw-r--r--   0 root         (0) root         (0)    12827 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/cmd/uploader.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/cmd/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.766995 conan-server-2.0.6/conans/client/conanfile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/conanfile/__init__.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/conanfile/build.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/conanfile/configure.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/conanfile/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.767995 conan-server-2.0.6/conans/client/conf/
--rw-r--r--   0 root         (0) root         (0)     6347 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9195 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/conf/config_installer.py
--rw-r--r--   0 root         (0) root         (0)    14006 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/conf/detect.py
--rw-r--r--   0 root         (0) root         (0)     5473 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/conf/detect_vs.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/conf/required_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.768995 conan-server-2.0.6/conans/client/downloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/downloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9514 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/downloaders/caching_file_downloader.py
--rw-r--r--   0 root         (0) root         (0)     3856 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/downloaders/download_cache.py
--rw-r--r--   0 root         (0) root         (0)     6263 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/downloaders/file_downloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.768995 conan-server-2.0.6/conans/client/generators/
--rw-r--r--   0 root         (0) root         (0)     9520 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/generators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.769995 conan-server-2.0.6/conans/client/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/build_mode.py
--rw-r--r--   0 root         (0) root         (0)     4571 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/compatibility.py
--rw-r--r--   0 root         (0) root         (0)     3832 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/compute_pid.py
--rw-r--r--   0 root         (0) root         (0)    14873 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)    16759 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/graph_binaries.py
--rw-r--r--   0 root         (0) root         (0)    17797 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/graph_builder.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/graph_error.py
--rw-r--r--   0 root         (0) root         (0)    12486 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/install_graph.py
--rw-r--r--   0 root         (0) root         (0)     4163 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/profile_node_definer.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/provides.py
--rw-r--r--   0 root         (0) root         (0)     6536 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/proxy.py
--rw-r--r--   0 root         (0) root         (0)     5806 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/python_requires.py
--rw-r--r--   0 root         (0) root         (0)     4692 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/graph/range_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2595 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/hook_manager.py
--rw-r--r--   0 root         (0) root         (0)    21297 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/installer.py
--rw-r--r--   0 root         (0) root         (0)    15815 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/loader.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/loader_txt.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/migrations.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/pkg_sign.py
--rw-r--r--   0 root         (0) root         (0)    16848 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/profile_loader.py
--rw-r--r--   0 root         (0) root         (0)    11706 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/remote_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.770995 conan-server-2.0.6/conans/client/rest/
--rw-r--r--   0 root         (0) root         (0)      838 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5987 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/rest/auth_manager.py
--rw-r--r--   0 root         (0) root         (0)     6132 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/rest/client_routes.py
--rw-r--r--   0 root         (0) root         (0)     6894 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/rest/conan_requester.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/rest/file_uploader.py
--rw-r--r--   0 root         (0) root         (0)     5388 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/rest/rest_client.py
--rw-r--r--   0 root         (0) root         (0)    10011 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/rest/rest_client_common.py
--rw-r--r--   0 root         (0) root         (0)    13652 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/rest/rest_client_v2.py
--rw-r--r--   0 root         (0) root         (0)     3606 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.771996 conan-server-2.0.6/conans/client/store/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/store/localdb.py
--rw-r--r--   0 root         (0) root         (0)     8798 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/subsystems.py
--rw-r--r--   0 root         (0) root         (0)     5457 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/client/userio.py
--rwxr-xr-x   0 root         (0) root         (0)      118 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/conan.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/conan_server.py
--rw-r--r--   0 root         (0) root         (0)     7817 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/errors.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/migrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.773996 conan-server-2.0.6/conans/model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19600 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/build_info.py
--rw-r--r--   0 root         (0) root         (0)    12420 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/conan_file.py
--rw-r--r--   0 root         (0) root         (0)     2775 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/conanfile_interface.py
--rw-r--r--   0 root         (0) root         (0)    29524 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/conf.py
--rw-r--r--   0 root         (0) root         (0)     5901 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/dependencies.py
--rw-r--r--   0 root         (0) root         (0)    10886 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/graph_lock.py
--rw-r--r--   0 root         (0) root         (0)    13067 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/info.py
--rw-r--r--   0 root         (0) root         (0)     5193 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/layout.py
--rw-r--r--   0 root         (0) root         (0)     4883 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/manifest.py
--rw-r--r--   0 root         (0) root         (0)    17174 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/options.py
--rw-r--r--   0 root         (0) root         (0)     3861 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/package_ref.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/pkg_type.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/profile.py
--rw-r--r--   0 root         (0) root         (0)     7585 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/recipe_ref.py
--rw-r--r--   0 root         (0) root         (0)    24646 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/requires.py
--rw-r--r--   0 root         (0) root         (0)     2171 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/rest_routes.py
--rw-r--r--   0 root         (0) root         (0)    13368 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/settings.py
--rw-r--r--   0 root         (0) root         (0)     6038 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/version.py
--rw-r--r--   0 root         (0) root         (0)     4350 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/model/version_range.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.773996 conan-server-2.0.6/conans/paths/
--rw-r--r--   0 root         (0) root         (0)     2184 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/pylint_plugin.py
--rw-r--r--   0 root         (0) root         (0)      252 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/requirements_dev.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/requirements_server.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.774996 conan-server-2.0.6/conans/search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3814 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/search/query_parse.py
--rw-r--r--   0 root         (0) root         (0)     4384 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.774996 conan-server-2.0.6/conans/server/
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.775996 conan-server-2.0.6/conans/server/conf/
--rw-r--r--   0 root         (0) root         (0)     9523 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2398 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/conf/default_server_conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.775996 conan-server-2.0.6/conans/server/crypto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/crypto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.775996 conan-server-2.0.6/conans/server/crypto/jwt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/crypto/jwt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/crypto/jwt/jwt_credentials_manager.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/crypto/jwt/jwt_manager.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/launcher.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/migrate.py
--rw-r--r--   0 root         (0) root         (0)      315 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/migrations.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/plugin_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.776996 conan-server-2.0.6/conans/server/rest/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/api_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.776996 conan-server-2.0.6/conans/server/rest/bottle_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/bottle_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2844 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/bottle_plugins/authorization_header.py
--rw-r--r--   0 root         (0) root         (0)     1545 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/bottle_plugins/http_basic_authentication.py
--rw-r--r--   0 root         (0) root         (0)     1583 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/bottle_plugins/jwt_authentication.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/bottle_plugins/return_handler.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/bottle_routes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.776996 conan-server-2.0.6/conans/server/rest/controller/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.777996 conan-server-2.0.6/conans/server/rest/controller/v2/
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/controller/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3147 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/controller/v2/conan.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/controller/v2/delete.py
--rw-r--r--   0 root         (0) root         (0)      459 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/controller/v2/ping.py
--rw-r--r--   0 root         (0) root         (0)     3319 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/controller/v2/revisions.py
--rw-r--r--   0 root         (0) root         (0)     1432 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/controller/v2/search.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/controller/v2/users.py
--rw-r--r--   0 root         (0) root         (0)     1761 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/rest/server.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/revision_list.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/server_launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.778996 conan-server-2.0.6/conans/server/service/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/service/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7022 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/service/authorize.py
--rw-r--r--   0 root         (0) root         (0)      210 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/service/mime.py
--rw-r--r--   0 root         (0) root         (0)      591 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/service/user_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.778996 conan-server-2.0.6/conans/server/service/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/service/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/service/v2/search.py
--rw-r--r--   0 root         (0) root         (0)     6315 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/service/v2/service_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.778996 conan-server-2.0.6/conans/server/store/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2429 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/store/disk_adapter.py
--rw-r--r--   0 root         (0) root         (0)    13212 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/store/server_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.779996 conan-server-2.0.6/conans/server/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/server/utils/files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.779996 conan-server-2.0.6/conans/test/
--rw-r--r--   0 root         (0) root         (0)      203 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13174 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.780996 conan-server-2.0.6/conans/test/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/test/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4868 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/test/utils/artifactory.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/test/utils/mocks.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/test/utils/profiles.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/test/utils/scm.py
--rw-r--r--   0 root         (0) root         (0)     3858 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/test/utils/server_launcher.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/test/utils/test_files.py
--rw-r--r--   0 root         (0) root         (0)    35320 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/test/utils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:08.781996 conan-server-2.0.6/conans/util/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/util/config_parser.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/util/dates.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/util/encrypt.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/util/env.py
--rw-r--r--   0 root         (0) root         (0)    11263 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/util/files.py
--rw-r--r--   0 root         (0) root         (0)     3657 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/util/locks.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/util/runners.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/util/sha.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-26 11:30:56.000000 conan-server-2.0.6/conans/util/windows.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-26 11:31:08.782997 conan-server-2.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4943 2023-05-26 11:30:56.000000 conan-server-2.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.583168 conan-server-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-06-21 11:09:09.000000 conan-server-2.0.7/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 11:09:09.000000 conan-server-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8160 2023-06-21 11:09:20.583168 conan-server-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6045 2023-06-21 11:09:09.000000 conan-server-2.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.543165 conan-server-2.0.7/conan/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.544165 conan-server-2.0.7/conan/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/conan_api.py
+-rw-r--r--   0 root         (0) root         (0)     9995 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/model.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.546165 conan-server-2.0.7/conan/api/subapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4888 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/config.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/download.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/export.py
+-rw-r--r--   0 root         (0) root         (0)    10725 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/graph.py
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/install.py
+-rw-r--r--   0 root         (0) root         (0)     7275 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/list.py
+-rw-r--r--   0 root         (0) root         (0)     5110 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/local.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/lockfile.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/new.py
+-rw-r--r--   0 root         (0) root         (0)     4426 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     4478 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/remotes.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/search.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/api/subapi/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.546165 conan-server-2.0.7/conan/cli/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7582 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/args.py
+-rw-r--r--   0 root         (0) root         (0)    10968 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     6240 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.549165 conan-server-2.0.7/conan/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3311 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/build.py
+-rw-r--r--   0 root         (0) root         (0)     4648 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/cache.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)     8291 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/create.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/download.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/editable.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/export.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/export_pkg.py
+-rw-r--r--   0 root         (0) root         (0)     8879 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/inspect.py
+-rw-r--r--   0 root         (0) root         (0)     5003 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)     6454 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/list.py
+-rw-r--r--   0 root         (0) root         (0)     5485 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/lock.py
+-rw-r--r--   0 root         (0) root         (0)     4239 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/new.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/profile.py
+-rw-r--r--   0 root         (0) root         (0)    11410 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/remote.py
+-rw-r--r--   0 root         (0) root         (0)     4862 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/search.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/source.py
+-rw-r--r--   0 root         (0) root         (0)     3884 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/test.py
+-rw-r--r--   0 root         (0) root         (0)     5977 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/upload.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/exit_codes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.549165 conan-server-2.0.7/conan/cli/formatters/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/formatters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.550165 conan-server-2.0.7/conan/cli/formatters/graph/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/formatters/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5593 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/formatters/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/formatters/graph/graph_info_text.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/formatters/graph/info_graph_dot.py
+-rw-r--r--   0 root         (0) root         (0)     7359 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/formatters/graph/info_graph_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.550165 conan-server-2.0.7/conan/cli/formatters/list/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/formatters/list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/formatters/list/binary_html_table.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/formatters/list/list.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/formatters/list/search_table_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.551165 conan-server-2.0.7/conan/cli/printers/
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/printers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/cli/printers/graph.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.551165 conan-server-2.0.7/conan/internal/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.551165 conan-server-2.0.7/conan/internal/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.553166 conan-server-2.0.7/conan/internal/api/new/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/alias_new.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/autoools_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/autotools_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/bazel_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/bazel_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/cmake_exe.py
+-rw-r--r--   0 root         (0) root         (0)     8187 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/cmake_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/meson_exe.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/meson_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/msbuild_exe.py
+-rw-r--r--   0 root         (0) root         (0)    12247 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/api/new/msbuild_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.553166 conan-server-2.0.7/conan/internal/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9923 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/cache/conan_reference_layout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.554166 conan-server-2.0.7/conan/internal/cache/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/cache/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/cache/db/cache_database.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/cache/db/packages_table.py
+-rw-r--r--   0 root         (0) root         (0)     4791 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/cache/db/recipes_table.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/cache/db/table.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/conan_app.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/integrity_check.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/internal/upload_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.554166 conan-server-2.0.7/conan/tools/
+-rw-r--r--   0 root         (0) root         (0)      384 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.554166 conan-server-2.0.7/conan/tools/android/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/android/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/android/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.555166 conan-server-2.0.7/conan/tools/apple/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/apple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11200 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/apple/apple.py
+-rw-r--r--   0 root         (0) root         (0)     2167 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/apple/xcodebuild.py
+-rw-r--r--   0 root         (0) root         (0)    16379 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/apple/xcodedeps.py
+-rw-r--r--   0 root         (0) root         (0)     5683 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/apple/xcodetoolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.555166 conan-server-2.0.7/conan/tools/build/
+-rw-r--r--   0 root         (0) root         (0)     4142 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/build/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11103 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/build/cppstd.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/build/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/build/cross_building.py
+-rw-r--r--   0 root         (0) root         (0)    15391 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/build/flags.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/build/stdcpp_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.556166 conan-server-2.0.7/conan/tools/cmake/
+-rw-r--r--   0 root         (0) root         (0)      217 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11124 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/cmake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.556166 conan-server-2.0.7/conan/tools/cmake/cmakedeps/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/cmakedeps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8168 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/cmakedeps/cmakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.557166 conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/
+-rw-r--r--   0 root         (0) root         (0)     3944 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/config.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/config_version.py
+-rw-r--r--   0 root         (0) root         (0)     5704 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/macros.py
+-rw-r--r--   0 root         (0) root         (0)    14925 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/target_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    19857 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/target_data.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/targets.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/layout.py
+-rw-r--r--   0 root         (0) root         (0)    14422 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/presets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.557166 conan-server-2.0.7/conan/tools/cmake/toolchain/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/toolchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35960 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/toolchain/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    11204 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/toolchain/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/cmake/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.558166 conan-server-2.0.7/conan/tools/env/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25388 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/env/environment.py
+-rw-r--r--   0 root         (0) root         (0)     3233 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/env/virtualbuildenv.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/env/virtualrunenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.559166 conan-server-2.0.7/conan/tools/files/
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/files/conandata.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/files/copy_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    23768 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/files/files.py
+-rw-r--r--   0 root         (0) root         (0)     4177 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/files/packager.py
+-rw-r--r--   0 root         (0) root         (0)     5823 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/files/patches.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.559166 conan-server-2.0.7/conan/tools/files/symlinks/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/files/symlinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/files/symlinks/symlinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.560166 conan-server-2.0.7/conan/tools/gnu/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/gnu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6234 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/gnu/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/gnu/autotoolsdeps.py
+-rw-r--r--   0 root         (0) root         (0)    13227 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/gnu/autotoolstoolchain.py
+-rw-r--r--   0 root         (0) root         (0)     3556 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/gnu/get_gnu_triplet.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/gnu/gnudeps_flags.py
+-rw-r--r--   0 root         (0) root         (0)     4028 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/gnu/pkgconfig.py
+-rw-r--r--   0 root         (0) root         (0)    18557 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/gnu/pkgconfigdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.560166 conan-server-2.0.7/conan/tools/google/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/google/bazel.py
+-rw-r--r--   0 root         (0) root         (0)    10955 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/google/bazeldeps.py
+-rw-r--r--   0 root         (0) root         (0)      585 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/google/layout.py
+-rw-r--r--   0 root         (0) root         (0)      857 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/google/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.561166 conan-server-2.0.7/conan/tools/intel/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/intel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/intel/intel_cc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.561166 conan-server-2.0.7/conan/tools/layout/
+-rw-r--r--   0 root         (0) root         (0)      605 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/layout/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.561166 conan-server-2.0.7/conan/tools/meson/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/meson/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4073 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/meson/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     4954 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/meson/meson.py
+-rw-r--r--   0 root         (0) root         (0)    22060 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/meson/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.562166 conan-server-2.0.7/conan/tools/microsoft/
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/microsoft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/microsoft/layout.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/microsoft/msbuild.py
+-rw-r--r--   0 root         (0) root         (0)    19214 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/microsoft/msbuilddeps.py
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/microsoft/nmakedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/microsoft/nmaketoolchain.py
+-rw-r--r--   0 root         (0) root         (0)      593 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/microsoft/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)    10843 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/microsoft/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)    13069 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/microsoft/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.563166 conan-server-2.0.7/conan/tools/premake/
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/premake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/premake/premake.py
+-rw-r--r--   0 root         (0) root         (0)    10534 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/premake/premakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.563166 conan-server-2.0.7/conan/tools/qbs/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/qbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/qbs/qbs.py
+-rw-r--r--   0 root         (0) root         (0)     9873 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/qbs/qbsprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.563166 conan-server-2.0.7/conan/tools/scm/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/scm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/scm/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.563166 conan-server-2.0.7/conan/tools/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16285 2023-06-21 11:09:09.000000 conan-server-2.0.7/conan/tools/system/package_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.564167 conan-server-2.0.7/conan_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8160 2023-06-21 11:09:20.000000 conan-server-2.0.7/conan_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10670 2023-06-21 11:09:20.000000 conan-server-2.0.7/conan_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 11:09:20.000000 conan-server-2.0.7/conan_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-21 11:09:20.000000 conan-server-2.0.7/conan_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      526 2023-06-21 11:09:20.000000 conan-server-2.0.7/conan_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 11:09:20.000000 conan-server-2.0.7/conan_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.565167 conan-server-2.0.7/conans/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.567167 conan-server-2.0.7/conans/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.567167 conan-server-2.0.7/conans/client/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10525 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/cache/editable.py
+-rw-r--r--   0 root         (0) root         (0)     6569 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/cache/remote_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.568167 conan-server-2.0.7/conans/client/cmd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/cmd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7671 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/cmd/export.py
+-rw-r--r--   0 root         (0) root         (0)    12762 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/cmd/uploader.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/cmd/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.568167 conan-server-2.0.7/conans/client/conanfile/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/conanfile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/conanfile/build.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/conanfile/configure.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/conanfile/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.569167 conan-server-2.0.7/conans/client/conf/
+-rw-r--r--   0 root         (0) root         (0)     6356 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9195 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/conf/config_installer.py
+-rw-r--r--   0 root         (0) root         (0)    14019 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/conf/detect.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/conf/detect_vs.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/conf/required_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.569167 conan-server-2.0.7/conans/client/downloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/downloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9512 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/downloaders/caching_file_downloader.py
+-rw-r--r--   0 root         (0) root         (0)     4228 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/downloaders/download_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/downloaders/file_downloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.569167 conan-server-2.0.7/conans/client/generators/
+-rw-r--r--   0 root         (0) root         (0)     9708 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/generators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.571167 conan-server-2.0.7/conans/client/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4837 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/build_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/compute_pid.py
+-rw-r--r--   0 root         (0) root         (0)    14948 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)    16759 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/graph_binaries.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/graph_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/graph_error.py
+-rw-r--r--   0 root         (0) root         (0)    12486 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/install_graph.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/profile_node_definer.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/provides.py
+-rw-r--r--   0 root         (0) root         (0)     6594 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/python_requires.py
+-rw-r--r--   0 root         (0) root         (0)     4692 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/graph/range_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/hook_manager.py
+-rw-r--r--   0 root         (0) root         (0)    21259 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/installer.py
+-rw-r--r--   0 root         (0) root         (0)    15815 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/loader.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/loader_txt.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/migrations.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/pkg_sign.py
+-rw-r--r--   0 root         (0) root         (0)    16848 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/profile_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13519 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/remote_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.572167 conan-server-2.0.7/conans/client/rest/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5987 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/rest/auth_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6132 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/rest/client_routes.py
+-rw-r--r--   0 root         (0) root         (0)     6894 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/rest/conan_requester.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/rest/file_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     5488 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/rest/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)    10011 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/rest/rest_client_common.py
+-rw-r--r--   0 root         (0) root         (0)    14018 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/rest/rest_client_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3606 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.572167 conan-server-2.0.7/conans/client/store/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/store/localdb.py
+-rw-r--r--   0 root         (0) root         (0)     8798 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)     5457 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/client/userio.py
+-rwxr-xr-x   0 root         (0) root         (0)      118 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/conan.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/conan_server.py
+-rw-r--r--   0 root         (0) root         (0)     7817 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/migrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.575168 conan-server-2.0.7/conans/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20745 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/build_info.py
+-rw-r--r--   0 root         (0) root         (0)    12420 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/conan_file.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/conanfile_interface.py
+-rw-r--r--   0 root         (0) root         (0)    29771 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/conf.py
+-rw-r--r--   0 root         (0) root         (0)     5901 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/dependencies.py
+-rw-r--r--   0 root         (0) root         (0)    10886 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/graph_lock.py
+-rw-r--r--   0 root         (0) root         (0)    13067 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/info.py
+-rw-r--r--   0 root         (0) root         (0)     5247 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/layout.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/options.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/package_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/pkg_type.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/profile.py
+-rw-r--r--   0 root         (0) root         (0)     7612 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/recipe_ref.py
+-rw-r--r--   0 root         (0) root         (0)    24646 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/requires.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/rest_routes.py
+-rw-r--r--   0 root         (0) root         (0)    13368 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/settings.py
+-rw-r--r--   0 root         (0) root         (0)     6038 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/version.py
+-rw-r--r--   0 root         (0) root         (0)     4350 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/model/version_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.575168 conan-server-2.0.7/conans/paths/
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/pylint_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/requirements_dev.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/requirements_server.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.575168 conan-server-2.0.7/conans/search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/search/query_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.576168 conan-server-2.0.7/conans/server/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.576168 conan-server-2.0.7/conans/server/conf/
+-rw-r--r--   0 root         (0) root         (0)     9523 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/conf/default_server_conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.577168 conan-server-2.0.7/conans/server/crypto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/crypto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.577168 conan-server-2.0.7/conans/server/crypto/jwt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/crypto/jwt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/crypto/jwt/jwt_credentials_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/crypto/jwt/jwt_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/migrate.py
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/migrations.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/plugin_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.577168 conan-server-2.0.7/conans/server/rest/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/api_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.578168 conan-server-2.0.7/conans/server/rest/bottle_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/bottle_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/bottle_plugins/authorization_header.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/bottle_plugins/http_basic_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/bottle_plugins/jwt_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/bottle_plugins/return_handler.py
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/bottle_routes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.578168 conan-server-2.0.7/conans/server/rest/controller/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.579168 conan-server-2.0.7/conans/server/rest/controller/v2/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/controller/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/controller/v2/conan.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/controller/v2/delete.py
+-rw-r--r--   0 root         (0) root         (0)      459 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/controller/v2/ping.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/controller/v2/revisions.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/controller/v2/search.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/controller/v2/users.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/rest/server.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/revision_list.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/server_launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.579168 conan-server-2.0.7/conans/server/service/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/service/authorize.py
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/service/mime.py
+-rw-r--r--   0 root         (0) root         (0)      591 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/service/user_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.580168 conan-server-2.0.7/conans/server/service/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/service/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/service/v2/search.py
+-rw-r--r--   0 root         (0) root         (0)     6315 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/service/v2/service_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.580168 conan-server-2.0.7/conans/server/store/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/store/disk_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    13212 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/store/server_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.580168 conan-server-2.0.7/conans/server/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/server/utils/files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.581168 conan-server-2.0.7/conans/test/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13174 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/test/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.581168 conan-server-2.0.7/conans/test/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/test/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4868 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/test/utils/artifactory.py
+-rw-r--r--   0 root         (0) root         (0)     4852 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/test/utils/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/test/utils/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/test/utils/scm.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/test/utils/server_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/test/utils/test_files.py
+-rw-r--r--   0 root         (0) root         (0)    35487 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/test/utils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:20.583168 conan-server-2.0.7/conans/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/util/config_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/util/dates.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/util/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/util/env.py
+-rw-r--r--   0 root         (0) root         (0)    12086 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/util/files.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/util/locks.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/util/runners.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/util/sha.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-06-21 11:09:09.000000 conan-server-2.0.7/conans/util/windows.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-21 11:09:20.584169 conan-server-2.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4943 2023-06-21 11:09:09.000000 conan-server-2.0.7/setup.py
```

### Comparing `conan-server-2.0.6/LICENSE.md` & `conan-server-2.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/PKG-INFO` & `conan-server-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan-server
-Version: 2.0.6
+Version: 2.0.7
 Summary: Conan Server of Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Description: <picture>
           <!-- These are also used for https://github.com/conan-io/.github/blob/main/profile/README.md -->
@@ -30,16 +30,16 @@
         - Portable. Works across all platforms, including Linux, OSX, Windows (with native and first-class support, WSL, MinGW),
           Solaris, FreeBSD, embedded and cross-compiling, docker, WSL
         - Manage binaries. It can create, upload and download binaries for any configuration and platform,
           even cross-compiling, saving lots of time in development and continuous integration. The binary compatibility can be configured
           and customized. Manage all your artifacts in the same way on all platforms.
         - Integrates with any build system, including any proprietary and custom one. Provides tested support for major build systems
           (CMake, MSBuild, Makefiles, Meson, etc).
-        - Extensible: Its python based recipes, together with extensions points allows for great power and flexibility.
-        - Large and active community, especially in Github (https://github.com/conan-io/conan) and Slack (https://cpplang-inviter.cppalliance.org/ #conan channel).
+        - Extensible: Its Python-based recipes, together with extension points allow for great power and flexibility.
+        - Large and active community, especially in GitHub (https://github.com/conan-io/conan) and Slack (https://cpplang-inviter.cppalliance.org/ #conan channel).
           This community also creates and maintains packages in ConanCenter and Bincrafters repositories in Bintray.
         - Stable. Used in production by many companies, since 1.0 there is a commitment not to break package recipes and documented behavior.
         
         
         This is the **developer/maintainer** documentation. For user documentation, go to https://docs.conan.io
         
         
@@ -86,42 +86,42 @@
         ## Contributing to the project
         
         
         Feedback and contribution are always welcome in this project.
         Please read our [contributing guide](https://github.com/conan-io/conan/blob/develop/.github/CONTRIBUTING.md).
         Also, if you plan to contribute, please add some testing for your changes. You can read the [Conan
         tests guidelines section](https://github.com/conan-io/conan/blob/develop/conans/test/README.md) for
-        some advise on how to write tests for Conan.
+        some advice on how to write tests for Conan.
         
         ### Running the tests
         
         
-        **Install python requirements**
+        **Install Python requirements**
         
         ```bash
         $ python -m pip install -r conans/requirements_server.txt
         $ python -m pip install -r conans/requirements_dev.txt
         ```
         
-        If you are not Windows and you are not using a python virtual environment, you will need to run these
+        If you are not on Windows and you are not using a Python virtual environment, you will need to run these
         commands using `sudo`.
         
         Before you can run the tests, you need to set a few environment variables first.
         
         ```bash
         $ export PYTHONPATH=$PYTHONPATH:$(pwd)
         ```
         
         On Windows it would be (while being in the Conan root directory):
         
         ```bash
         $ set PYTHONPATH=.
         ```
         
-        Conan test suite defines and configure some required tools (CMake, Ninja, etc) in the
+        Conan test suite defines and configures some required tools (CMake, Ninja, etc) in the
         ``conftest.py`` and allows to define a custom ``conftest_user.py``.
         Some specific versions, like cmake>=3.15 are necessary.
         
         
         You can run the tests like this:
         
         ```bash
@@ -140,15 +140,15 @@
         
         To run specific tests, you can specify the test name too, something like:
         
         ```bash
         $ python -m pytest conans/test/unittests/client/cmd/export_test.py::ExportTest::test_export_warning -s
         ```
         
-        The `-s` argument can be useful to see some output that otherwise is captured by pytest.
+        The `-s` argument can be useful to see some output that otherwise is captured by *pytest*.
         
         Also, you can run tests against an instance of Artifactory. Those tests should add the attribute
         `artifactory_ready`.
         
         ```bash
         $ python -m pytest . -m artifactory_ready
         ```
@@ -160,15 +160,15 @@
         ```bash
         $ export CONAN_TEST_WITH_ARTIFACTORY=1
         $ export ARTIFACTORY_DEFAULT_URL=http://localhost:8081/artifactory
         $ export ARTIFACTORY_DEFAULT_USER=admin
         $ export ARTIFACTORY_DEFAULT_PASSWORD=password
         ```
         
-        `ARTIFACTORY_DEFAULT_URL` is the base url for the Artifactory repo, not one for a specific
+        `ARTIFACTORY_DEFAULT_URL` is the base URL for the Artifactory repo, not one for a specific
         repository. Running the tests with a real Artifactory instance will create repos on the fly so please
         use a separate server for testing purposes.
         
         ## License
         
         [MIT LICENSE](LICENSE.md)
```

### Comparing `conan-server-2.0.6/README.md` & `conan-server-2.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 - Portable. Works across all platforms, including Linux, OSX, Windows (with native and first-class support, WSL, MinGW),
   Solaris, FreeBSD, embedded and cross-compiling, docker, WSL
 - Manage binaries. It can create, upload and download binaries for any configuration and platform,
   even cross-compiling, saving lots of time in development and continuous integration. The binary compatibility can be configured
   and customized. Manage all your artifacts in the same way on all platforms.
 - Integrates with any build system, including any proprietary and custom one. Provides tested support for major build systems
   (CMake, MSBuild, Makefiles, Meson, etc).
-- Extensible: Its python based recipes, together with extensions points allows for great power and flexibility.
-- Large and active community, especially in Github (https://github.com/conan-io/conan) and Slack (https://cpplang-inviter.cppalliance.org/ #conan channel).
+- Extensible: Its Python-based recipes, together with extension points allow for great power and flexibility.
+- Large and active community, especially in GitHub (https://github.com/conan-io/conan) and Slack (https://cpplang-inviter.cppalliance.org/ #conan channel).
   This community also creates and maintains packages in ConanCenter and Bincrafters repositories in Bintray.
 - Stable. Used in production by many companies, since 1.0 there is a commitment not to break package recipes and documented behavior.
 
 
 This is the **developer/maintainer** documentation. For user documentation, go to https://docs.conan.io
 
 
@@ -78,42 +78,42 @@
 ## Contributing to the project
 
 
 Feedback and contribution are always welcome in this project.
 Please read our [contributing guide](https://github.com/conan-io/conan/blob/develop/.github/CONTRIBUTING.md).
 Also, if you plan to contribute, please add some testing for your changes. You can read the [Conan
 tests guidelines section](https://github.com/conan-io/conan/blob/develop/conans/test/README.md) for
-some advise on how to write tests for Conan.
+some advice on how to write tests for Conan.
 
 ### Running the tests
 
 
-**Install python requirements**
+**Install Python requirements**
 
 ```bash
 $ python -m pip install -r conans/requirements_server.txt
 $ python -m pip install -r conans/requirements_dev.txt
 ```
 
-If you are not Windows and you are not using a python virtual environment, you will need to run these
+If you are not on Windows and you are not using a Python virtual environment, you will need to run these
 commands using `sudo`.
 
 Before you can run the tests, you need to set a few environment variables first.
 
 ```bash
 $ export PYTHONPATH=$PYTHONPATH:$(pwd)
 ```
 
 On Windows it would be (while being in the Conan root directory):
 
 ```bash
 $ set PYTHONPATH=.
 ```
 
-Conan test suite defines and configure some required tools (CMake, Ninja, etc) in the
+Conan test suite defines and configures some required tools (CMake, Ninja, etc) in the
 ``conftest.py`` and allows to define a custom ``conftest_user.py``.
 Some specific versions, like cmake>=3.15 are necessary.
 
 
 You can run the tests like this:
 
 ```bash
@@ -132,15 +132,15 @@
 
 To run specific tests, you can specify the test name too, something like:
 
 ```bash
 $ python -m pytest conans/test/unittests/client/cmd/export_test.py::ExportTest::test_export_warning -s
 ```
 
-The `-s` argument can be useful to see some output that otherwise is captured by pytest.
+The `-s` argument can be useful to see some output that otherwise is captured by *pytest*.
 
 Also, you can run tests against an instance of Artifactory. Those tests should add the attribute
 `artifactory_ready`.
 
 ```bash
 $ python -m pytest . -m artifactory_ready
 ```
@@ -152,14 +152,14 @@
 ```bash
 $ export CONAN_TEST_WITH_ARTIFACTORY=1
 $ export ARTIFACTORY_DEFAULT_URL=http://localhost:8081/artifactory
 $ export ARTIFACTORY_DEFAULT_USER=admin
 $ export ARTIFACTORY_DEFAULT_PASSWORD=password
 ```
 
-`ARTIFACTORY_DEFAULT_URL` is the base url for the Artifactory repo, not one for a specific
+`ARTIFACTORY_DEFAULT_URL` is the base URL for the Artifactory repo, not one for a specific
 repository. Running the tests with a real Artifactory instance will create repos on the fly so please
 use a separate server for testing purposes.
 
 ## License
 
 [MIT LICENSE](LICENSE.md)
```

### Comparing `conan-server-2.0.6/conan/api/conan_api.py` & `conan-server-2.0.7/conan/api/conan_api.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/api/model.py` & `conan-server-2.0.7/conans/client/rest/rest_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,160 +1,137 @@
-import fnmatch
+from conans import CHECKSUM_DEPLOY, REVISIONS, OAUTH_TOKEN
+from conans.client.rest.rest_client_v2 import RestV2Methods
+from conans.errors import AuthenticationException, ConanException
+
+
+class RestApiClientFactory(object):
+
+    def __init__(self, requester, config):
+        self._requester = requester
+        self._config = config
+        self._cached_capabilities = {}
+
+    def new(self, remote, token, refresh_token, custom_headers):
+        tmp = RestApiClient(remote, token, refresh_token, custom_headers,
+                            self._requester, self._config,
+                            self._cached_capabilities)
+        return tmp
+
+
+class RestApiClient(object):
+    """
+        Rest Api Client for handle remote.
+    """
+
+    def __init__(self, remote, token, refresh_token, custom_headers, requester,
+                 config, cached_capabilities):
+
+        # Set to instance
+        self._token = token
+        self._refresh_token = refresh_token
+        self._remote_url = remote.url
+        self._custom_headers = custom_headers
+        self._requester = requester
+
+        self._verify_ssl = remote.verify_ssl
+        self._config = config
+
+        # This dict is shared for all the instances of RestApiClient
+        self._cached_capabilities = cached_capabilities
+
+    def _capable(self, capability, user=None, password=None):
+        capabilities = self._cached_capabilities.get(self._remote_url)
+        if capabilities is None:
+            tmp = RestV2Methods(self._remote_url, self._token, self._custom_headers,
+                                self._requester, self._config, self._verify_ssl)
+            capabilities = tmp.server_capabilities(user, password)
+            self._cached_capabilities[self._remote_url] = capabilities
+        return capability in capabilities
+
+    def _get_api(self):
+        revisions = self._capable(REVISIONS)
+
+        if not revisions:
+            # TODO: port conan_v2_error to 1.X if not revisions
+            raise ConanException("The remote doesn't support revisions. "
+                                 "Conan 2.0 is no longer compatible with "
+                                 "remotes that don't accept revisions.")
+        checksum_deploy = self._capable(CHECKSUM_DEPLOY)
+        return RestV2Methods(self._remote_url, self._token, self._custom_headers,
+                             self._requester, self._config, self._verify_ssl,
+                             checksum_deploy)
+
+    def get_recipe(self, ref, dest_folder, metadata, only_metadata):
+        return self._get_api().get_recipe(ref, dest_folder, metadata, only_metadata)
+
+    def get_recipe_sources(self, ref, dest_folder):
+        return self._get_api().get_recipe_sources(ref, dest_folder)
+
+    def get_package(self, pref, dest_folder, metadata, only_metadata):
+        return self._get_api().get_package(pref, dest_folder, metadata, only_metadata)
+
+    def upload_recipe(self, ref, files_to_upload):
+        return self._get_api().upload_recipe(ref, files_to_upload)
+
+    def upload_package(self, pref, files_to_upload):
+        return self._get_api().upload_package(pref, files_to_upload)
+
+    def authenticate(self, user, password):
+        api_v2 = RestV2Methods(self._remote_url, self._token, self._custom_headers,
+                               self._requester, self._config, self._verify_ssl)
 
-from conans.errors import ConanException
-from conans.model.package_ref import PkgReference
-from conans.model.recipe_ref import RecipeReference
-
-
-class Remote:
-
-    def __init__(self, name, url, verify_ssl=True, disabled=False):
-        self._name = name  # Read only, is the key
-        self.url = url
-        self.verify_ssl = verify_ssl
-        self.disabled = disabled
-
-    @property
-    def name(self):
-        return self._name
-
-    def __eq__(self, other):
-        if other is None:
-            return False
-        return self.name == other.name and \
-               self.url == other.url and \
-               self.verify_ssl == other.verify_ssl and \
-               self.disabled == other.disabled
-
-    def __str__(self):
-        return "{}: {} [Verify SSL: {}, Enabled: {}]".format(self.name, self.url, self.verify_ssl,
-                                                             not self.disabled)
-
-    def __repr__(self):
-        return str(self)
-
-
-class PackagesList:
-    def __init__(self):
-        self.recipes = {}
-
-    def add_refs(self, refs):
-        # RREVS alreday come in ASCENDING order, so upload does older revisions first
-        for ref in refs:
-            ref_dict = self.recipes.setdefault(str(ref), {})
-            if ref.revision:
-                revs_dict = ref_dict.setdefault("revisions", {})
-                rev_dict = revs_dict.setdefault(ref.revision, {})
-                if ref.timestamp:
-                    rev_dict["timestamp"] = ref.timestamp
-
-    def add_prefs(self, rrev, prefs):
-        # Prevs already come in ASCENDING order, so upload does older revisions first
-        revs_dict = self.recipes[str(rrev)]["revisions"]
-        rev_dict = revs_dict[rrev.revision]
-        packages_dict = rev_dict.setdefault("packages", {})
-
-        for pref in prefs:
-            package_dict = packages_dict.setdefault(pref.package_id, {})
-            if pref.revision:
-                prevs_dict = package_dict.setdefault("revisions", {})
-                prev_dict = prevs_dict.setdefault(pref.revision, {})
-                if pref.timestamp:
-                    prev_dict["timestamp"] = pref.timestamp
-
-    def add_configurations(self, confs):
-        for pref, conf in confs.items():
-            rev_dict = self.recipes[str(pref.ref)]["revisions"][pref.ref.revision]
-            try:
-                rev_dict["packages"][pref.package_id]["info"] = conf
-            except KeyError:  # If package_id does not exist, do nothing, only add to existing prefs
-                pass
-
-    def refs(self):
-        result = {}
-        for ref, ref_dict in self.recipes.items():
-            for rrev, rrev_dict in ref_dict.get("revisions", {}).items():
-                t = rrev_dict.get("timestamp")
-                recipe = RecipeReference.loads(f"{ref}#{rrev}%{t}")  # TODO: optimize this
-                result[recipe] = rrev_dict
-        return result.items()
-
-    @staticmethod
-    def prefs(ref, recipe_bundle):
-        result = {}
-        for package_id, pkg_bundle in recipe_bundle.get("packages", {}).items():
-            prevs = pkg_bundle.get("revisions", {})
-            for prev, prev_bundle in prevs.items():
-                t = prev_bundle.get("timestamp")
-                pref = PkgReference(ref, package_id, prev, t)
-                result[pref] = prev_bundle
-        return result.items()
-
-    def serialize(self):
-        return self.recipes
-
-
-class ListPattern:
-
-    def __init__(self, expression, rrev="latest", package_id=None, prev="latest", only_recipe=False):
-        def split(s, c, default=None):
-            if not s:
-                return None, default
-            tokens = s.split(c, 1)
-            if len(tokens) == 2:
-                return tokens[0], tokens[1] or default
-            return tokens[0], default
-
-        recipe, package = split(expression, ":")
-        self.raw = expression
-        self.ref, rrev = split(recipe, "#", rrev)
-        ref, user_channel = split(self.ref, "@")
-        self.name, self.version = split(ref, "/")
-        self.user, self.channel = split(user_channel, "/")
-        self.rrev, _ = split(rrev, "%")
-        self.package_id, prev = split(package, "#", prev)
-        self.prev, _ = split(prev, "%")
-        if only_recipe:
-            if self.package_id:
-                raise ConanException("Do not specify 'package_id' with 'only-recipe'")
+        if self._refresh_token and self._token:
+            token, refresh_token = api_v2.refresh_token(self._token, self._refresh_token)
         else:
-            self.package_id = self.package_id or package_id
+            try:
+                # Check capabilities can raise also 401 until the new Artifactory is released
+                oauth_capable = self._capable(OAUTH_TOKEN, user, password)
+            except AuthenticationException:
+                oauth_capable = False
+
+            if oauth_capable:
+                # Artifactory >= 6.13.X
+                token, refresh_token = api_v2.authenticate_oauth(user, password)
+            else:
+                token = api_v2.authenticate(user, password)
+                refresh_token = None
+
+        return token, refresh_token
+
+    def check_credentials(self):
+        return self._get_api().check_credentials()
+
+    def search(self, pattern=None, ignorecase=True):
+        return self._get_api().search(pattern, ignorecase)
+
+    def search_packages(self, reference):
+        return self._get_api().search_packages(reference)
+
+    def remove_recipe(self, ref):
+        return self._get_api().remove_recipe(ref)
+
+    def remove_all_packages(self, ref):
+        return self._get_api().remove_all_packages(ref)
+
+    def remove_packages(self, prefs):
+        return self._get_api().remove_packages(prefs)
+
+    def server_capabilities(self):
+        return self._get_api().server_capabilities()
+
+    def get_recipe_revisions_references(self, ref):
+        return self._get_api().get_recipe_revisions_references(ref)
+
+    def get_package_revisions_references(self, pref, headers=None):
+        return self._get_api().get_package_revisions_references(pref, headers=headers)
+
+    def get_latest_recipe_reference(self, ref):
+        return self._get_api().get_latest_recipe_reference(ref)
+
+    def get_latest_package_reference(self, pref, headers):
+        return self._get_api().get_latest_package_reference(pref, headers=headers)
+
+    def get_recipe_revision_reference(self, ref):
+        return self._get_api().get_recipe_revision_reference(ref)
 
-    @property
-    def is_latest_rrev(self):
-        return self.rrev == "latest"
-
-    @property
-    def is_latest_prev(self):
-        return self.prev == "latest"
-
-    def check_refs(self, refs):
-        if not refs and self.ref and "*" not in self.ref:
-            raise ConanException(f"Recipe '{self.ref}' not found")
-
-    def filter_rrevs(self, rrevs):
-        if self.rrev == "!latest":
-            return rrevs[1:]
-        rrevs = [r for r in rrevs if fnmatch.fnmatch(r.revision, self.rrev)]
-        if not rrevs:
-            refs_str = f'{self.ref}#{self.rrev}'
-            if "*" not in refs_str:
-                raise ConanException(f"Recipe revision '{refs_str}' not found")
-        return rrevs
-
-    def filter_prefs(self, prefs):
-        prefs = [p for p in prefs if fnmatch.fnmatch(p.package_id, self.package_id)]
-        if not prefs:
-            refs_str = f'{self.ref}#{self.rrev}:{self.package_id}'
-            if "*" not in refs_str:
-                raise ConanException(f"Package ID '{self.raw}' not found")
-        return prefs
-
-    def filter_prevs(self, prevs):
-        if self.prev == "!latest":
-            return prevs[1:]
-        prevs = [p for p in prevs if fnmatch.fnmatch(p.revision, self.prev)]
-        if not prevs:
-            refs_str = f'{self.ref}#{self.rrev}:{self.package_id}#{self.prev}'
-            if "*" not in refs_str:
-                raise ConanException(f"Package revision '{self.raw}' not found")
-        return prevs
+    def get_package_revision_reference(self, pref):
+        return self._get_api().get_package_revision_reference(pref)
```

### Comparing `conan-server-2.0.6/conan/api/output.py` & `conan-server-2.0.7/conan/api/output.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/api/subapi/cache.py` & `conan-server-2.0.7/conan/api/subapi/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,36 +11,48 @@
 class CacheAPI:
 
     def __init__(self, conan_api):
         self.conan_api = conan_api
 
     def export_path(self, ref: RecipeReference):
         app = ConanApp(self.conan_api.cache_folder)
-        ref = _resolve_latest_ref(app, ref)
-        ref_layout = app.cache.ref_layout(ref)
+        ref.revision = None if ref.revision == "latest" else ref.revision
+        ref_layout = app.cache.recipe_layout(ref)
         return ref_layout.export()
 
-    def export_source_path(self, ref: RecipeReference):
+    def recipe_metadata_path(self, ref: RecipeReference):
         app = ConanApp(self.conan_api.cache_folder)
         ref = _resolve_latest_ref(app, ref)
         ref_layout = app.cache.ref_layout(ref)
+        return ref_layout.metadata()
+
+    def export_source_path(self, ref: RecipeReference):
+        app = ConanApp(self.conan_api.cache_folder)
+        ref.revision = None if ref.revision == "latest" else ref.revision
+        ref_layout = app.cache.recipe_layout(ref)
         return ref_layout.export_sources()
 
     def source_path(self, ref: RecipeReference):
         app = ConanApp(self.conan_api.cache_folder)
-        ref = _resolve_latest_ref(app, ref)
-        ref_layout = app.cache.ref_layout(ref)
+        ref.revision = None if ref.revision == "latest" else ref.revision
+        ref_layout = app.cache.recipe_layout(ref)
         return ref_layout.source()
 
     def build_path(self, pref: PkgReference):
         app = ConanApp(self.conan_api.cache_folder)
         pref = _resolve_latest_pref(app, pref)
         ref_layout = app.cache.pkg_layout(pref)
         return ref_layout.build()
 
+    def package_metadata_path(self, pref: PkgReference):
+        app = ConanApp(self.conan_api.cache_folder)
+        pref = _resolve_latest_pref(app, pref)
+        ref_layout = app.cache.pkg_layout(pref)
+        return ref_layout.metadata()
+
     def package_path(self, pref: PkgReference):
         app = ConanApp(self.conan_api.cache_folder)
         pref = _resolve_latest_pref(app, pref)
         ref_layout = app.cache.pkg_layout(pref)
         return ref_layout.package()
 
     def check_integrity(self, package_list):
```

### Comparing `conan-server-2.0.6/conan/api/subapi/config.py` & `conan-server-2.0.7/conan/api/subapi/config.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/api/subapi/download.py` & `conan-server-2.0.7/conan/api/subapi/download.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,44 +8,59 @@
 
 
 class DownloadAPI:
 
     def __init__(self, conan_api):
         self.conan_api = conan_api
 
-    def recipe(self, ref: RecipeReference, remote: Remote):
+    def recipe(self, ref: RecipeReference, remote: Remote, metadata=None):
         output = ConanOutput()
         app = ConanApp(self.conan_api.cache_folder)
-        skip_download = app.cache.exists_rrev(ref)
-        if skip_download:
+        assert ref.revision, f"Reference '{ref}' must have revision"
+        try:
+            app.cache.recipe_layout(ref)  # raises if not found
+        except ConanException:
+            pass
+        else:
             output.info(f"Skip recipe {ref.repr_notime()} download, already in cache")
+            if metadata:
+                app.remote_manager.get_recipe_metadata(ref, remote, metadata)
             return False
 
         output.info(f"Downloading recipe '{ref.repr_notime()}'")
-        app.remote_manager.get_recipe(ref, remote)
+        app.remote_manager.get_recipe(ref, remote, metadata)
+        # Respect the timestamp of the server, the ``get_recipe()`` doesn't do it internally
+        # Best would be that ``get_recipe()`` returns the timestamp in the same call
+        server_ref = app.remote_manager.get_recipe_revision_reference(ref, remote)
+        assert server_ref == ref
+        app.cache.update_recipe_timestamp(server_ref)
 
         layout = app.cache.ref_layout(ref)
         conan_file_path = layout.conanfile()
         conanfile = app.loader.load_basic(conan_file_path, display=ref, remotes=[remote])
 
         # Download the sources too, don't be lazy
         output.info(f"Downloading '{str(ref)}' sources")
         retrieve_exports_sources(app.remote_manager, layout, conanfile, ref, [remote])
         return True
 
-    def package(self, pref: PkgReference, remote: Remote):
+    def package(self, pref: PkgReference, remote: Remote, metadata=None):
         output = ConanOutput()
         app = ConanApp(self.conan_api.cache_folder)
-        if not app.cache.exists_rrev(pref.ref):
+        try:
+            app.cache.recipe_layout(pref.ref)  # raises if not found
+        except ConanException:
             raise ConanException("The recipe of the specified package "
                                  "doesn't exist, download it first")
 
         skip_download = app.cache.exists_prev(pref)
         if skip_download:
             output.info(f"Skip package {pref.repr_notime()} download, already in cache")
+            if metadata:
+                app.remote_manager.get_package_metadata(pref, remote, metadata)
             return False
         layout = app.cache.ref_layout(pref.ref)
         conan_file_path = layout.conanfile()
         conanfile = app.loader.load_basic(conan_file_path, display=pref.ref)
         output.info(f"Downloading package '{pref.repr_notime()}'")
         app.remote_manager.get_package(conanfile, pref, remote)
         return True
```

### Comparing `conan-server-2.0.6/conan/api/subapi/export.py` & `conan-server-2.0.7/conan/api/subapi/export.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/api/subapi/graph.py` & `conan-server-2.0.7/conan/api/subapi/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-import os
-
 from conan.api.output import ConanOutput
 from conan.internal.conan_app import ConanApp
 from conans.client.graph.graph import Node, RECIPE_CONSUMER, CONTEXT_HOST, RECIPE_VIRTUAL, \
     CONTEXT_BUILD
 from conans.client.graph.graph_binaries import GraphBinariesAnalyzer
 from conans.client.graph.graph_builder import DepsGraphBuilder
 from conans.client.graph.profile_node_definer import initialize_conanfile_profile, consumer_definer
-from conans.client.loader import parse_conanfile
-
 from conans.errors import ConanException
-
 from conans.model.recipe_ref import RecipeReference
 
 
 class GraphAPI:
 
     def __init__(self, conan_api):
         self.conan_api = conan_api
@@ -187,14 +182,7 @@
         :param update: (False by default), if Conan should look for newer versions or
             revisions for already existing recipes in the Conan cache
         """
         ConanOutput().title("Computing necessary packages")
         conan_app = ConanApp(self.conan_api.cache_folder)
         binaries_analyzer = GraphBinariesAnalyzer(conan_app)
         binaries_analyzer.evaluate_graph(graph, build_mode, lockfile, remotes, update)
-
-    def load_conanfile_class(self, path):
-        """ Given a path to a conanfile.py file, it loads its class (not instance) to allow
-        inspecting the class attributes, like 'name', 'version', 'description', 'options' etc"""
-        path = os.path.join(os.getcwd(), path)
-        _, ret = parse_conanfile(path)
-        return ret
```

### Comparing `conan-server-2.0.6/conan/api/subapi/install.py` & `conan-server-2.0.7/conan/api/subapi/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from conan.internal.conan_app import ConanApp
 from conan.internal.deploy import do_deploys
 from conans.client.generators import write_generators
 from conans.client.installer import BinaryInstaller
 from conans.errors import ConanInvalidConfiguration
-from conans.util.files import mkdir
 
 
 class InstallAPI:
 
     def __init__(self, conan_api):
         self.conan_api = conan_api
 
@@ -37,15 +36,15 @@
         """
         app = ConanApp(self.conan_api.cache_folder)
         installer = BinaryInstaller(app)
         installer.install_sources(graph, remotes)
 
     # TODO: Look for a better name
     def install_consumer(self, deps_graph, generators=None, source_folder=None, output_folder=None,
-                         deploy=False):
+                         deploy=False, deploy_folder=None):
         """ Once a dependency graph has been installed, there are things to be done, like invoking
         generators for the root consumer.
         This is necessary for example for conanfile.txt/py, or for "conan install <ref> -g
         """
         root_node = deps_graph.root
         conanfile = root_node.conanfile
 
@@ -59,14 +58,13 @@
             msg = "{}: {}: {}".format(conanfile, binary, reason)
             raise ConanInvalidConfiguration(msg)
 
         conanfile.folders.set_base_folders(source_folder, output_folder)
 
         # The previous .set_base_folders has already decided between the source_folder and output
         if deploy:
-            base_folder = conanfile.folders.base_build
-            mkdir(base_folder)
+            base_folder = deploy_folder or conanfile.folders.base_build
             do_deploys(self.conan_api, deps_graph, deploy, base_folder)
 
         conanfile.generators = list(set(conanfile.generators).union(generators or []))
         app = ConanApp(self.conan_api.cache_folder)
         write_generators(conanfile, app)
```

### Comparing `conan-server-2.0.6/conan/api/subapi/list.py` & `conan-server-2.0.7/conan/api/subapi/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     def recipe_revisions(self, ref: RecipeReference, remote=None):
         assert ref.revision is None, "recipe_revisions: ref already have a revision"
         app = ConanApp(self.conan_api.cache_folder)
         if remote:
             results = app.remote_manager.get_recipe_revisions_references(ref, remote=remote)
         else:
-            results = app.cache.get_recipe_revisions_references(ref, only_latest_rrev=False)
+            results = app.cache.get_recipe_revisions_references(ref)
 
         return results
 
     def latest_package_revision(self, pref: PkgReference, remote=None):
         # TODO: This returns None if the given package_id is not existing. It should probably
         #  raise NotFound, but to keep aligned with the above ``latest_recipe_revision`` which
         #  is used as an "exists" check too in other places, lets respect the None return
@@ -52,22 +52,15 @@
     def package_revisions(self, pref: PkgReference, remote=None):
         assert pref.ref.revision is not None, "package_revisions requires a recipe revision, " \
                                               "check latest first if needed"
         app = ConanApp(self.conan_api.cache_folder)
         if remote:
             results = app.remote_manager.get_package_revisions_references(pref, remote=remote)
         else:
-            refs = app.cache.get_package_revisions_references(pref, only_latest_prev=False)
-            results = []
-            for ref in refs:
-                # TODO: Why another call, and why get_package_revisions_references doesn't return
-                #  already the timestamps?
-                timestamp = app.cache.get_package_timestamp(ref)
-                ref.timestamp = timestamp
-                results.append(ref)
+            results = app.cache.get_package_revisions_references(pref, only_latest_prev=False)
         return results
 
     def packages_configurations(self, ref: RecipeReference,
                                 remote=None) -> Dict[PkgReference, dict]:
         assert ref.revision is not None, "packages: ref should have a revision. " \
                                          "Check latest if needed."
         if not remote:
@@ -93,17 +86,18 @@
 
     def select(self, pattern, package_query=None, remote=None):
         if package_query and pattern.package_id and "*" not in pattern.package_id:
             raise ConanException("Cannot specify '-p' package queries, "
                                  "if 'package_id' is not a pattern")
         select_bundle = PackagesList()
         # Avoid doing a ``search`` of recipes if it is an exact ref and it will be used later
-        if "*" in pattern.ref or not pattern.version or \
-                (pattern.package_id is None and pattern.rrev is None):
-            refs = self.conan_api.search.recipes(pattern.ref, remote=remote)
+        search_ref = pattern.search_ref
+        if search_ref:
+            refs = self.conan_api.search.recipes(search_ref, remote=remote)
+            refs = pattern.filter_versions(refs)
             refs = sorted(refs)  # Order alphabetical and older versions first
             pattern.check_refs(refs)
         else:
             refs = [RecipeReference(pattern.name, pattern.version, pattern.user, pattern.channel)]
 
         # Show only the recipe references
         if pattern.package_id is None and pattern.rrev is None:
```

### Comparing `conan-server-2.0.6/conan/api/subapi/local.py` & `conan-server-2.0.7/conan/api/subapi/local.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/api/subapi/lockfile.py` & `conan-server-2.0.7/conan/api/subapi/lockfile.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/api/subapi/new.py` & `conan-server-2.0.7/conan/api/subapi/new.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/api/subapi/profiles.py` & `conan-server-2.0.7/conan/api/subapi/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/api/subapi/remotes.py` & `conan-server-2.0.7/conan/api/subapi/remotes.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/api/subapi/remove.py` & `conan-server-2.0.7/conan/api/subapi/remove.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/api/subapi/search.py` & `conan-server-2.0.7/conan/api/subapi/search.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/api/subapi/upload.py` & `conan-server-2.0.7/conan/api/subapi/upload.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 from conan.api.output import ConanOutput
 from conan.internal.conan_app import ConanApp
+from conan.internal.upload_metadata import gather_metadata
 from conans.client.cmd.uploader import PackagePreparator, UploadExecutor, UploadUpstreamChecker
 from conans.client.downloaders.download_cache import DownloadCache
 from conans.client.pkg_sign import PkgSignaturesPlugin
 from conans.client.rest.file_uploader import FileUploader
 from conans.errors import ConanException, AuthenticationException, ForbiddenException
 
 
@@ -25,21 +26,26 @@
             if conanfile.upload_policy == "skip":
                 ConanOutput().info(f"{ref}: Skipping upload of binaries, "
                                    "because upload_policy='skip'")
                 bundle["packages"] = {}
 
         UploadUpstreamChecker(app).check(package_list, remote, force)
 
-    def prepare(self, package_list, enabled_remotes):
+    def prepare(self, package_list, enabled_remotes, metadata=None):
         """Compress the recipes and packages and fill the upload_data objects
         with the complete information. It doesn't perform the upload nor checks upstream to see
-        if the recipe is still there"""
+        if the recipe is still there
+        :param package_list:
+        :param enabled_remotes:
+        :param metadata: A list of patterns of metadata that should be uploaded. Default None
+        means all metadata will be uploaded together with the pkg artifacts"""
         app = ConanApp(self.conan_api.cache_folder)
         preparator = PackagePreparator(app)
         preparator.prepare(package_list, enabled_remotes)
+        gather_metadata(package_list, app.cache, metadata)
         signer = PkgSignaturesPlugin(app.cache)
         # This might add files entries to package_list with signatures
         signer.sign(package_list)
 
     def upload(self, package_list, remote):
         app = ConanApp(self.conan_api.cache_folder)
         app.remote_manager.check_credentials(remote)
@@ -51,16 +57,18 @@
         config = app.cache.new_config
         url = config.get("core.sources:upload_url")
         if url is None:
             return
         url = url if url.endswith("/") else url + "/"
         download_cache_path = config.get("core.sources:download_cache")
         download_cache_path = download_cache_path or app.cache.default_sources_backup_folder
+        excluded_urls = config.get("core.sources:exclude_urls", check_type=list, default=[])
 
-        files = DownloadCache(download_cache_path).get_backup_sources_files_to_upload(package_list)
+        files = DownloadCache(download_cache_path).get_backup_sources_files_to_upload(package_list,
+                                                                                      excluded_urls)
         # TODO: verify might need a config to force it to False
         uploader = FileUploader(app.requester, verify=True, config=config)
         # TODO: For Artifactory, we can list all files once and check from there instead
         #  of 1 request per file, but this is more general
         for file in files:
             basename = os.path.basename(file)
             full_url = url + basename
```

### Comparing `conan-server-2.0.6/conan/cli/args.py` & `conan-server-2.0.7/conan/cli/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     --build=never      Disallow build for all packages, use binary packages or fail if a binary
                        package is not found. Cannot be combined with other '--build' options.
     --build=missing    Build packages from source whose binary package is not found.
     --build=cascade    Build packages from source that have at least one dependency being built from
                        source.
     --build=[pattern]  Build packages from source whose package reference matches the pattern. The
                        pattern uses 'fnmatch' style wildcards.
-    --build=![pattern] Excluded packages, which will not be built from the source, whose package
+    --build=~[pattern] Excluded packages, which will not be built from the source, whose package
                        reference matches the pattern. The pattern uses 'fnmatch' style wildcards.
     --build=missing:[pattern] Build from source if a compatible binary does not exist, only for
                               packages matching pattern.
 '''
 
 
 def add_lockfile_args(parser):
```

### Comparing `conan-server-2.0.6/conan/cli/cli.py` & `conan-server-2.0.7/conan/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
             output.info("'%s' is not a Conan command. See 'conan --help'." % command_argument)
             output.info("")
             self._print_similar(command_argument)
             raise ConanException("Unknown command %s" % str(exc))
 
         try:
-            command.run(self._conan_api, self._commands[command_argument].parser, args[0][1:])
+            command.run(self._conan_api, args[0][1:])
         except Exception as e:
             # must be a local-import to get updated value
             if ConanOutput.level_allowed(LEVEL_TRACE):
                 print(traceback.format_exc())
             self._conan2_migrate_recipe_msg(e)
             raise
```

### Comparing `conan-server-2.0.6/conan/cli/command.py` & `conan-server-2.0.7/conan/cli/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,64 +25,61 @@
 
 
 class BaseConanCommand:
     def __init__(self, method, formatters=None):
         self._formatters = {"text": lambda x: None}
         self._method = method
         self._name = None
-        self._parser = None
         if formatters:
             for kind, action in formatters.items():
                 if callable(action):
                     self._formatters[kind] = action
                 else:
                     raise ConanException("Invalid formatter for {}. The formatter must be"
                                          "a valid function".format(kind))
         if method.__doc__:
             self._doc = method.__doc__
         else:
             raise ConanException("No documentation string defined for command: '{}'. Conan "
                                  "commands should provide a documentation string explaining "
                                  "its use briefly.".format(self._name))
 
-    def _init_log_levels(self):
-        self._parser.add_argument("-v", default="status", nargs='?',
-                                  help="Level of detail of the output. Valid options from less verbose "
-                                       "to more verbose: -vquiet, -verror, -vwarning, -vnotice, -vstatus, "
-                                       "-v or -vverbose, -vv or -vdebug, -vvv or -vtrace")
+    @staticmethod
+    def _init_log_levels(parser):
+        parser.add_argument("-v", default="status", nargs='?',
+                            help="Level of detail of the output. Valid options from less verbose "
+                                 "to more verbose: -vquiet, -verror, -vwarning, -vnotice, -vstatus, "
+                                 "-v or -vverbose, -vv or -vdebug, -vvv or -vtrace")
 
     @property
     def _help_formatters(self):
         """
         Formatters that are shown as available in help, 'text' formatter
         should not appear
         """
-        return [formatter for formatter in list(self._formatters) if formatter != "text"]
+        return [formatter for formatter in self._formatters if formatter != "text"]
 
-    def _init_formatters(self):
-        if self._help_formatters:
-            help_message = "Select the output format: {}".format(", ".join(list(self._help_formatters)))
-            self._parser.add_argument('-f', '--format', action=OnceArgument, help=help_message)
+    def _init_formatters(self, parser):
+        formatters = self._help_formatters
+        if formatters:
+            help_message = "Select the output format: {}".format(", ".join(formatters))
+            parser.add_argument('-f', '--format', action=OnceArgument, help=help_message)
 
     @property
     def name(self):
         return self._name
 
     @property
     def method(self):
         return self._method
 
     @property
     def doc(self):
         return self._doc
 
-    @property
-    def parser(self):
-        return self._parser
-
     def _format(self, parser, info, *args):
         parser_args, _ = parser.parse_known_args(*args)
 
         default_format = "text"
         try:
             formatarg = parser_args.format or default_format
         except AttributeError:
@@ -108,70 +105,69 @@
         return args
 
 
 class ConanCommand(BaseConanCommand):
     def __init__(self, method, group=None, formatters=None):
         super().__init__(method, formatters=formatters)
         self._subcommands = {}
-        self._subcommand_parser = None
         self._group = group or "Other"
         self._name = method.__name__.replace("_", "-")
-        self._parser = ConanArgumentParser(description=self._doc,
-                                           prog="conan {}".format(self._name),
-                                           formatter_class=SmartFormatter)
-        self._init_formatters()
-        self._init_log_levels()
 
     def add_subcommand(self, subcommand):
-        if not self._subcommand_parser:
-            self._subcommand_parser = self._parser.add_subparsers(dest='subcommand',
-                                                                  help='sub-command help')
-            self._subcommand_parser.required = True
         subcommand.set_name(self.name)
-        subcommand.set_parser(self._parser, self._subcommand_parser)
         self._subcommands[subcommand.name] = subcommand
 
-    def run(self, conan_api, parser, *args):
+    def run(self, conan_api, *args):
+        parser = ConanArgumentParser(description=self._doc, prog="conan {}".format(self._name),
+                                     formatter_class=SmartFormatter)
+        self._init_log_levels(parser)
+        self._init_formatters(parser)
+
         info = self._method(conan_api, parser, *args)
 
         if not self._subcommands:
-            self._format(self._parser, info, *args)
+            self._format(parser, info, *args)
         else:
-            subcommand = args[0][0] if args[0] else None
-            if subcommand in self._subcommands:
-                self._subcommands[subcommand].run(conan_api, *args)
+            subcommand_parser = parser.add_subparsers(dest='subcommand', help='sub-command help')
+            subcommand_parser.required = True
+
+            try:
+                sub = self._subcommands[args[0][0]]
+            except (KeyError, IndexError):  # display help
+                for sub in self._subcommands.values():
+                    sub.set_parser(subcommand_parser)
+                parser.parse_args(*args)
             else:
-                self._parser.parse_args(*args)
+                sub.set_parser(subcommand_parser)
+                sub.run(conan_api, parser, *args)
 
     @property
     def group(self):
         return self._group
 
 
 class ConanSubCommand(BaseConanCommand):
     def __init__(self, method, formatters=None):
         super().__init__(method, formatters=formatters)
-        self._parent_parser = None
         self._parser = None
         self._subcommand_name = method.__name__.replace('_', '-')
 
-    def run(self, conan_api, *args):
-        info = self._method(conan_api, self._parent_parser, self._parser, *args)
+    def run(self, conan_api, parent_parser, *args):
+        info = self._method(conan_api, parent_parser, self._parser, *args)
         # It is necessary to do it after calling the "method" otherwise parser not complete
-        self._format(self._parent_parser, info, *args)
+        self._format(parent_parser, info, *args)
 
     def set_name(self, parent_name):
         self._name = self._subcommand_name.replace(f'{parent_name}-', '', 1)
 
-    def set_parser(self, parent_parser, subcommand_parser):
+    def set_parser(self, subcommand_parser):
         self._parser = subcommand_parser.add_parser(self._name, help=self._doc)
         self._parser.description = self._doc
-        self._parent_parser = parent_parser
-        self._init_formatters()
-        self._init_log_levels()
+        self._init_formatters(self._parser)
+        self._init_log_levels(self._parser)
 
 
 def conan_command(group=None, formatters=None):
     return lambda f: ConanCommand(f, group, formatters=formatters)
 
 
 def conan_subcommand(formatters=None):
```

### Comparing `conan-server-2.0.6/conan/cli/commands/build.py` & `conan-server-2.0.7/conan/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/commands/cache.py` & `conan-server-2.0.7/conan/cli/commands/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 @conan_subcommand(formatters={"text": cli_out_write})
 def cache_path(conan_api: ConanAPI, parser, subparser, *args):
     """
     Show the path to the Conan cache for a given reference.
     """
     subparser.add_argument("reference", help="Recipe reference or Package reference")
-    subparser.add_argument("--folder", choices=['export_source', 'source', 'build'],
+    subparser.add_argument("--folder", choices=['export_source', 'source', 'build', 'metadata'],
                            help="Path to show. The 'build'"
                                 " requires a package reference. If not specified it shows 'exports'"
                                 " path ")
 
     args = parser.parse_args(*args)
     try:
         pref = PkgReference.loads(args.reference)
@@ -36,21 +36,25 @@
         ref = RecipeReference.loads(args.reference)
         if args.folder is None:
             path = conan_api.cache.export_path(ref)
         elif args.folder == "export_source":
             path = conan_api.cache.export_source_path(ref)
         elif args.folder == "source":
             path = conan_api.cache.source_path(ref)
+        elif args.folder == "metadata":
+            path = conan_api.cache.recipe_metadata_path(ref)
         else:
             raise ConanException(f"'--folder {args.folder}' requires a valid package reference")
     else:
         if args.folder is None:
             path = conan_api.cache.package_path(pref)
         elif args.folder == "build":
             path = conan_api.cache.build_path(pref)
+        elif args.folder == "metadata":
+            path = conan_api.cache.package_metadata_path(pref)
         else:
             raise ConanException(f"'--folder {args.folder}' requires a recipe reference")
     return path
 
 
 @conan_subcommand()
 def cache_clean(conan_api: ConanAPI, parser, subparser, *args):
@@ -60,15 +64,15 @@
     """
     subparser.add_argument("pattern", nargs="?", help="Selection pattern for references to clean")
     subparser.add_argument("-s", "--source", action='store_true', default=False,
                            help="Clean source folders")
     subparser.add_argument("-b", "--build", action='store_true', default=False,
                            help="Clean build folders")
     subparser.add_argument("-d", "--download", action='store_true', default=False,
-                           help="Clean download folders")
+                           help="Clean download and metadata folders")
     subparser.add_argument("-t", "--temp", action='store_true', default=False,
                            help="Clean temporary folders")
     subparser.add_argument('-p', '--package-query', action=OnceArgument,
                            help="Remove only the packages matching a specific query, e.g., "
                                 "os=Windows AND (arch=x86 OR compiler=gcc)")
     args = parser.parse_args(*args)
```

### Comparing `conan-server-2.0.6/conan/cli/commands/config.py` & `conan-server-2.0.7/conan/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/commands/create.py` & `conan-server-2.0.7/conan/cli/commands/create.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     lockfile = conan_api.lockfile.update_lockfile_export(lockfile, conanfile, ref,
                                                          args.build_require)
 
     print_profiles(profile_host, profile_build)
 
     deps_graph = None
     if not is_python_require:
-        # TODO: This section might be overlapping with ``graph_compute()``
         requires = [ref] if not args.build_require else None
         tool_requires = [ref] if args.build_require else None
         # FIXME: Dirty: package type still raw, not processed yet
         # TODO: Why not for package_type = "application" like cmake to be used as build-require?
         if conanfile.package_type == "build-scripts" and not args.build_require:
             # swap them
             requires, tool_requires = tool_requires, requires
@@ -85,19 +84,18 @@
                                                       clean=args.lockfile_clean)
 
     if test_conanfile_path:
         # TODO: We need arguments for:
         #  - decide update policy "--test_package_update"
         tested_python_requires = ref.repr_notime() if is_python_require else None
         from conan.cli.commands.test import run_test
-        deps_graph = run_test(conan_api, test_conanfile_path, ref, profile_host, profile_build,
-                              remotes, lockfile, update=False, build_modes=args.build,
-                              tested_python_requires=tested_python_requires)
-        lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
-                                                      clean=args.lockfile_clean)
+        # The test_package do not make the "conan create" command return a different graph or
+        # produce a different lockfile. The result is always the same, irrespective of test_package
+        run_test(conan_api, test_conanfile_path, ref, profile_host, profile_build, remotes, lockfile,
+                 update=False, build_modes=args.build, tested_python_requires=tested_python_requires)
 
     conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, cwd)
     return {"graph": deps_graph,
             "conan_api": conan_api}
 
 
 def _check_tested_reference_matches(deps_graph, tested_ref, out):
```

### Comparing `conan-server-2.0.6/conan/cli/commands/download.py` & `conan-server-2.0.7/conan/cli/commands/download.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,84 @@
 from multiprocessing.pool import ThreadPool
 
 from conan.api.conan_api import ConanAPI
-from conan.api.model import ListPattern
+from conan.api.model import ListPattern, MultiPackagesList
 from conan.api.output import ConanOutput
+from conan.cli import make_abs_path
 from conan.cli.command import conan_command, OnceArgument
+from conan.cli.commands.list import print_list_text, print_list_json
+from conans.errors import ConanException
 
 
-@conan_command(group="Creator")
+@conan_command(group="Creator", formatters={"text": print_list_text,
+                                            "json": print_list_json})
 def download(conan_api: ConanAPI, parser, *args):
     """
     Download (without installing) a single conan package from a remote server.
 
     It downloads just the package, but not its transitive dependencies, and it will not call
     any generate, generators or deployers.
     It can download multiple packages if patterns are used, and also works with
     queries over the package binaries.
     """
 
-    parser.add_argument('reference', help="Recipe reference or package reference, can contain * as "
-                                          "wildcard at any reference field. If revision is not "
-                                          "specified, it is assumed latest one.")
+    parser.add_argument('pattern', nargs="?",
+                        help="A pattern in the form 'pkg/version#revision:package_id#revision', "
+                             "e.g: zlib/1.2.13:* means all binaries for zlib/1.2.13. "
+                             "If revision is not specified, it is assumed latest one.")
     parser.add_argument("--only-recipe", action='store_true', default=False,
                         help='Download only the recipe/s, not the binary packages.')
     parser.add_argument('-p', '--package-query', default=None, action=OnceArgument,
                         help="Only download packages matching a specific query. e.g: os=Windows AND "
                              "(arch=x86 OR compiler=gcc)")
     parser.add_argument("-r", "--remote", action=OnceArgument, required=True,
                         help='Download from this specific remote')
+    parser.add_argument("-m", "--metadata", action='append',
+                        help='Download the metadata matching the pattern, even if the package is '
+                             'already in the cache and not downloaded')
+    parser.add_argument("-l", "--list", help="Package list file")
 
     args = parser.parse_args(*args)
+    if args.pattern is None and args.list is None:
+        raise ConanException("Missing pattern or package list file")
+    if args.pattern and args.list:
+        raise ConanException("Cannot define both the pattern and the package list file")
+
     remote = conan_api.remotes.get(args.remote)
+
+    if args.list:
+        listfile = make_abs_path(args.list)
+        multi_package_list = MultiPackagesList.load(listfile)
+        try:
+            package_list = multi_package_list[remote.name]
+        except KeyError:
+            raise ConanException(f"The current package list does not contain remote '{remote.name}'")
+    else:
+        ref_pattern = ListPattern(args.pattern, package_id="*", only_recipe=args.only_recipe)
+        package_list = conan_api.list.select(ref_pattern, args.package_query, remote)
+
     parallel = conan_api.config.get("core.download:parallel", default=1, check_type=int)
-    ref_pattern = ListPattern(args.reference, package_id="*", only_recipe=args.only_recipe)
-    select_bundle = conan_api.list.select(ref_pattern, args.package_query, remote)
+
     refs = []
     prefs = []
-    for ref, recipe_bundle in select_bundle.refs():
+    for ref, recipe_bundle in package_list.refs():
         refs.append(ref)
-        for pref, _ in select_bundle.prefs(ref, recipe_bundle):
+        for pref, _ in package_list.prefs(ref, recipe_bundle):
             prefs.append(pref)
 
     if parallel <= 1:
         for ref in refs:
-            conan_api.download.recipe(ref, remote)
+            conan_api.download.recipe(ref, remote, args.metadata)
         for pref in prefs:
-            conan_api.download.package(pref, remote)
+            conan_api.download.package(pref, remote, args.metadata)
     else:
         _download_parallel(parallel, conan_api, refs, prefs, remote)
 
+    return {"results": {"Local Cache": package_list.serialize()}}
+
 
 def _download_parallel(parallel, conan_api, refs, prefs, remote):
 
     thread_pool = ThreadPool(parallel)
     # First the recipes in parallel, we have to make sure the recipes are downloaded before the
     # packages
     ConanOutput().info("Downloading recipes in %s parallel threads" % parallel)
```

### Comparing `conan-server-2.0.6/conan/cli/commands/editable.py` & `conan-server-2.0.7/conan/cli/commands/editable.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/commands/export.py` & `conan-server-2.0.7/conan/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/commands/export_pkg.py` & `conan-server-2.0.7/conan/cli/commands/export_pkg.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/commands/graph.py` & `conan-server-2.0.7/conan/cli/commands/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import os
-
 from conan.api.output import ConanOutput, cli_out_write, Color
 from conan.cli import make_abs_path
 from conan.cli.args import common_graph_args, validate_common_graph_args
 from conan.cli.command import conan_command, conan_subcommand
 from conan.cli.formatters.graph import format_graph_html, format_graph_json, format_graph_dot
 from conan.cli.formatters.graph.graph_info_text import format_graph_info
 from conan.cli.printers.graph import print_graph_packages, print_graph_basic
@@ -64,14 +63,16 @@
                                                          args.user, args.channel,
                                                          profile_host, profile_build, lockfile,
                                                          remotes, args.build, args.update)
     else:
         deps_graph = conan_api.graph.load_graph_requires(args.requires, args.tool_requires,
                                                          profile_host, profile_build, lockfile,
                                                          remotes, args.build, args.update)
+    print_graph_basic(deps_graph)
+    deps_graph.report_graph_error()
     conan_api.graph.analyze_binaries(deps_graph, args.build, remotes=remotes, update=args.update,
                                      lockfile=lockfile)
     print_graph_packages(deps_graph)
 
     out = ConanOutput()
     out.title("Computing the build order")
     install_graph = InstallGraph(deps_graph)
@@ -115,14 +116,16 @@
                            help="Check if there are recipe updates")
     subparser.add_argument("--filter", action="append",
                            help="Show only the specified fields")
     subparser.add_argument("--package-filter", action="append",
                            help='Print information only for packages that match the patterns')
     subparser.add_argument("-d", "--deployer", action="append",
                            help='Deploy using the provided deployer to the output folder')
+    subparser.add_argument("-df", "--deployer-folder",
+                           help="Deployer output folder, base build folder by default if not set")
     subparser.add_argument("--build-require", action='store_true', default=False,
                            help='Whether the provided reference is a build-require')
     args = parser.parse_args(*args)
 
     # parameter validation
     validate_common_graph_args(args)
     if args.format in ("html", "dot") and args.filter:
@@ -165,14 +168,14 @@
         conan_api.install.install_system_requires(deps_graph, only_info=True)
         conan_api.install.install_sources(deps_graph, remotes=remotes)
 
         lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
                                                       clean=args.lockfile_clean)
         conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, cwd)
         if args.deployer:
-            base_folder = os.getcwd()
+            base_folder = args.deployer_folder or os.getcwd()
             do_deploys(conan_api, deps_graph, args.deployer, base_folder)
 
     return {"graph": deps_graph,
             "field_filter": args.filter,
             "package_filter": args.package_filter,
             "conan_api": conan_api}
```

### Comparing `conan-server-2.0.6/conan/cli/commands/inspect.py` & `conan-server-2.0.7/conan/cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/commands/install.py` & `conan-server-2.0.7/conan/cli/commands/install.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     common_graph_args(parser)
     parser.add_argument("-g", "--generator", action="append",
                         help='Generators to use')
     parser.add_argument("-of", "--output-folder",
                         help='The root output folder for generated and build files')
     parser.add_argument("-d", "--deployer", action="append",
                         help='Deploy using the provided deployer to the output folder')
+    parser.add_argument("--deployer-folder",
+                        help="Deployer output folder, base build folder by default if not set")
     parser.add_argument("--build-require", action='store_true', default=False,
                         help='Whether the provided reference is a build-require')
     args = parser.parse_args(*args)
 
     validate_common_graph_args(args)
     cwd = os.getcwd()
 
@@ -79,15 +81,16 @@
     conan_api.install.install_binaries(deps_graph=deps_graph, remotes=remotes)
 
     out.title("Finalizing install (deploy, generators)")
     conan_api.install.install_consumer(deps_graph=deps_graph,
                                        generators=args.generator,
                                        output_folder=output_folder,
                                        source_folder=source_folder,
-                                       deploy=args.deployer
+                                       deploy=args.deployer,
+                                       deploy_folder=args.deployer_folder
                                        )
 
     out.success("Install finished successfully")
     lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
                                                   clean=args.lockfile_clean)
     conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, cwd)
     return {"graph": deps_graph,
```

### Comparing `conan-server-2.0.6/conan/cli/commands/list.py` & `conan-server-2.0.7/conan/cli/commands/list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
 
 from conan.api.conan_api import ConanAPI
-from conan.api.model import ListPattern
+from conan.api.model import ListPattern, MultiPackagesList
 from conan.api.output import Color, cli_out_write
+from conan.cli import make_abs_path
 from conan.cli.command import conan_command, OnceArgument
 from conan.cli.formatters.list import list_packages_html
-
-# Keep them so we don't break other commands that import them, but TODO: Remove later
+from conans.errors import ConanException
 from conans.util.dates import timestamp_to_str
 
+
+# Keep them so we don't break other commands that import them, but TODO: Remove later
 remote_color = Color.BRIGHT_BLUE
 recipe_name_color = Color.GREEN
 recipe_color = Color.BRIGHT_WHITE
 reference_color = Color.WHITE
 error_color = Color.BRIGHT_RED
 field_color = Color.BRIGHT_YELLOW
 value_color = Color.CYAN
@@ -89,40 +91,59 @@
 @conan_command(group="Consumer", formatters={"text": print_list_text,
                                              "json": print_list_json,
                                              "html": list_packages_html})
 def list(conan_api: ConanAPI, parser, *args):
     """
     List existing recipes, revisions, or packages in the cache (by default) or the remotes.
     """
-    parser.add_argument('reference', help="Recipe reference or package reference. "
-                                          "Both can contain * as wildcard at any reference field. "
-                                          "If revision is not specified, it is assumed latest one.")
+    parser.add_argument('pattern', nargs="?",
+                        help="A pattern in the form 'pkg/version#revision:package_id#revision', "
+                             "e.g: zlib/1.2.13:* means all binaries for zlib/1.2.13. "
+                             "If revision is not specified, it is assumed latest one.")
     parser.add_argument('-p', '--package-query', default=None, action=OnceArgument,
                         help="List only the packages matching a specific query, e.g, os=Windows AND "
                              "(arch=x86 OR compiler=gcc)")
     parser.add_argument("-r", "--remote", default=None, action="append",
                         help="Remote names. Accepts wildcards ('*' means all the remotes available)")
     parser.add_argument("-c", "--cache", action='store_true', help="Search in the local cache")
+    parser.add_argument("-g", "--graph", help="Graph json file")
+    parser.add_argument("-gb", "--graph-binaries", help="Which binaries are listed", action="append")
+    parser.add_argument("-gr", "--graph-recipes", help="Which recipes are listed", action="append")
 
     args = parser.parse_args(*args)
-    ref_pattern = ListPattern(args.reference, rrev=None, prev=None)
-    # If neither remote nor cache are defined, show results only from cache
-    remotes = []
-    if args.cache or not args.remote:
-        remotes.append(None)
-    if args.remote:
-        remotes.extend(conan_api.remotes.list(args.remote))
-    results = {}
-    for remote in remotes:
-        name = getattr(remote, "name", "Local Cache")
-        try:
-            list_bundle = conan_api.list.select(ref_pattern, args.package_query, remote)
-        except Exception as e:
-            results[name] = {"error": str(e)}
-        else:
-            results[name] = list_bundle.serialize()
+
+    if args.pattern is None and args.graph is None:
+        raise ConanException("Missing pattern or graph json file")
+    if args.pattern and args.graph:
+        raise ConanException("Cannot define both the pattern and the graph json file")
+    if (args.graph_recipes or args.graph_binaries) and not args.graph:
+        raise ConanException("--graph-recipes and --graph-binaries require a --graph input")
+
+    if args.graph:
+        graphfile = make_abs_path(args.graph)
+        pkglist = MultiPackagesList.load_graph(graphfile, args.graph_recipes, args.graph_binaries)
+    else:
+        ref_pattern = ListPattern(args.pattern, rrev=None, prev=None)
+        # If neither remote nor cache are defined, show results only from cache
+        pkglist = MultiPackagesList()
+        if args.cache or not args.remote:
+            try:
+                cache_list = conan_api.list.select(ref_pattern, args.package_query, remote=None)
+            except Exception as e:
+                pkglist.add_error("Local Cache", str(e))
+            else:
+                pkglist.add("Local Cache", cache_list)
+        if args.remote:
+            remotes = conan_api.remotes.list(args.remote)
+            for remote in remotes:
+                try:
+                    remote_list = conan_api.list.select(ref_pattern, args.package_query, remote)
+                except Exception as e:
+                    pkglist.add_error(remote.name, str(e))
+                else:
+                    pkglist.add(remote.name, remote_list)
 
     return {
-        "results": results,
+        "results": pkglist.serialize(),
         "conan_api": conan_api,
         "cli_args": " ".join([f"{arg}={getattr(args, arg)}" for arg in vars(args) if getattr(args, arg)])
     }
```

### Comparing `conan-server-2.0.6/conan/cli/commands/lock.py` & `conan-server-2.0.7/conan/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/commands/new.py` & `conan-server-2.0.7/conan/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/commands/profile.py` & `conan-server-2.0.7/conan/cli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/commands/remote.py` & `conan-server-2.0.7/conan/cli/commands/remote.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/commands/search.py` & `conan-server-2.0.7/conan/cli/commands/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # FIXME: "conan search" == "conan list (*) -r="*"" --> implement @conan_alias_command??
 @conan_command(group="Consumer", formatters={"text": print_list_text,
                                              "json": print_list_json})
 def search(conan_api: ConanAPI, parser, *args):
     """
     Search for package recipes in all the remotes (by default), or a remote.
     """
-    parser.add_argument('reference', help="Recipe reference to search for."
+    parser.add_argument('reference', help="Recipe reference to search for. "
                                           "It can contain * as wildcard at any reference field.")
     parser.add_argument("-r", "--remote", action="append",
                         help="Remote names. Accepts wildcards. If not specified it searches "
                              "in all the remotes")
     args = parser.parse_args(*args)
     ref_pattern = ListPattern(args.reference, rrev=None)
     if ref_pattern.package_id is not None or ref_pattern.rrev is not None:
```

### Comparing `conan-server-2.0.6/conan/cli/commands/source.py` & `conan-server-2.0.7/conan/cli/commands/source.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/commands/test.py` & `conan-server-2.0.7/conan/cli/commands/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 
 from conan.api.output import ConanOutput
 from conan.cli.command import conan_command, OnceArgument
 from conan.cli.commands.create import test_package, _check_tested_reference_matches
 from conan.cli.args import add_lockfile_args, add_common_install_arguments
+from conan.cli.formatters.graph import format_graph_json
 from conan.cli.printers import print_profiles
 from conan.cli.printers.graph import print_graph_basic, print_graph_packages
 from conans.model.recipe_ref import RecipeReference
 
 
-@conan_command(group="Creator")
+@conan_command(group="Creator", formatters={"json": format_graph_json})
 def test(conan_api, parser, *args):
     """
     Test a package from a test_package folder.
     """
     parser.add_argument("path", action=OnceArgument,
                         help="Path to a test_package folder containing a conanfile.py")
     parser.add_argument("reference", action=OnceArgument,
@@ -38,14 +39,17 @@
 
     deps_graph = run_test(conan_api, path, ref, profile_host, profile_build, remotes, lockfile,
                           args.update, build_modes=args.build)
     lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
                                                   clean=args.lockfile_clean)
     conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, cwd)
 
+    return {"graph": deps_graph,
+            "conan_api": conan_api}
+
 
 def run_test(conan_api, path, ref, profile_host, profile_build, remotes, lockfile, update,
              build_modes, tested_python_requires=None):
     root_node = conan_api.graph.load_root_test_conanfile(path, ref,
                                                          profile_host, profile_build,
                                                          remotes=remotes,
                                                          update=update,
```

### Comparing `conan-server-2.0.6/conan/cli/formatters/graph/graph.py` & `conan-server-2.0.7/conan/cli/formatters/graph/graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import os
 
 from jinja2 import Template, select_autoescape
 
-
 from conan.api.output import cli_out_write
 from conan.cli.formatters.graph.graph_info_text import filter_graph
 from conan.cli.formatters.graph.info_graph_dot import graph_info_dot
 from conan.cli.formatters.graph.info_graph_html import graph_info_html
 from conans.client.graph.graph import BINARY_CACHE, \
     BINARY_DOWNLOAD, BINARY_BUILD, BINARY_MISSING, BINARY_UPDATE
+from conans.client.graph.graph_error import GraphConflictError
 from conans.client.installer import build_id
 from conans.util.files import load
 
 
 # FIXME: Check all this code when format_graph_[html/dot] use serialized graph
 
 class _PrinterGraphItem(object):
@@ -82,33 +82,48 @@
                  BINARY_DOWNLOAD: "LightGreen",
                  BINARY_BUILD: "Khaki",
                  BINARY_MISSING: "OrangeRed",
                  BINARY_UPDATE: "SeaGreen"}.get(node.binary, "White")
         return color
 
 
-def _render_graph(graph, template, template_folder):
+def _render_graph(graph, error, template, template_folder):
     graph = _Grapher(graph)
     from conans import __version__ as client_version
     template = Template(template, autoescape=select_autoescape(['html', 'xml']))
-    return template.render(graph=graph, base_template_path=template_folder, version=client_version)
+    return template.render(graph=graph, error=error, base_template_path=template_folder,
+                           version=client_version)
 
 
 def format_graph_html(result):
     graph = result["graph"]
     conan_api = result["conan_api"]
     package_filter = result["package_filter"]
     serial = graph.serialize()
     # TODO: This is not used, it is necessary to update the renderings to use the serialized graph
     #  instead of the native graph
     serial = filter_graph(serial, package_filter)
     template_folder = os.path.join(conan_api.cache_folder, "templates")
     user_template = os.path.join(template_folder, "graph.html")
     template = load(user_template) if os.path.isfile(user_template) else graph_info_html
-    cli_out_write(_render_graph(graph, template, template_folder))
+    if isinstance(graph.error, GraphConflictError):
+        error = {
+            "label": graph.error.require.ref,
+            "type": "conflict",
+            "from": graph.error.node.id or graph.error.base_previous.id,
+            "prev_node": graph.error.prev_node,
+            "should_highlight_node": lambda node: node.id == graph.error.node.id
+        }
+    else:
+        error = {
+            "type": "unknown",
+            "error:": graph.error,
+            "should_highlight_node": lambda node: False
+        }
+    cli_out_write(_render_graph(graph, error, template, template_folder))
     if graph.error:
         raise graph.error
 
 
 def format_graph_dot(result):
     graph = result["graph"]
     conan_api = result["conan_api"]
@@ -116,15 +131,15 @@
     serial = graph.serialize()
     # TODO: This is not used, it is necessary to update the renderings to use the serialized graph
     #  instead of the native graph
     serial = filter_graph(serial, package_filter)
     template_folder = os.path.join(conan_api.cache_folder, "templates")
     user_template = os.path.join(template_folder, "graph.dot")
     template = load(user_template) if os.path.isfile(user_template) else graph_info_dot
-    cli_out_write(_render_graph(graph, template, template_folder))
+    cli_out_write(_render_graph(graph, None, template, template_folder))
     if graph.error:
         raise graph.error
 
 
 def format_graph_json(result):
     graph = result["graph"]
     field_filter = result.get("field_filter")
```

### Comparing `conan-server-2.0.6/conan/cli/formatters/graph/graph_info_text.py` & `conan-server-2.0.7/conan/cli/formatters/graph/graph_info_text.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/formatters/list/binary_html_table.py` & `conan-server-2.0.7/conan/cli/formatters/list/binary_html_table.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/formatters/list/list.py` & `conan-server-2.0.7/conan/cli/formatters/list/list.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/formatters/list/search_table_html.py` & `conan-server-2.0.7/conan/cli/formatters/list/search_table_html.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/cli/printers/graph.py` & `conan-server-2.0.7/conan/cli/printers/graph.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/api/new/autoools_exe.py` & `conan-server-2.0.7/conan/internal/api/new/autoools_exe.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/api/new/autotools_lib.py` & `conan-server-2.0.7/conan/internal/api/new/autotools_lib.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/api/new/basic.py` & `conan-server-2.0.7/conan/internal/api/new/basic.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/api/new/bazel_exe.py` & `conan-server-2.0.7/conan/internal/api/new/bazel_exe.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/api/new/bazel_lib.py` & `conan-server-2.0.7/conan/internal/api/new/bazel_lib.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/api/new/cmake_exe.py` & `conan-server-2.0.7/conan/internal/api/new/cmake_exe.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/api/new/cmake_lib.py` & `conan-server-2.0.7/conan/internal/api/new/cmake_lib.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,22 +87,26 @@
 
 set_target_properties({{name}} PROPERTIES PUBLIC_HEADER "include/{{name}}.h")
 install(TARGETS {{name}})
 """
 
 source_h = """#pragma once
 
+#include <vector>
+#include <string>
+
 {% set define_name = package_name.upper() %}
 #ifdef _WIN32
   #define {{define_name}}_EXPORT __declspec(dllexport)
 #else
   #define {{define_name}}_EXPORT
 #endif
 
 {{define_name}}_EXPORT void {{package_name}}();
+{{define_name}}_EXPORT void {{package_name}}_print_vector(const std::vector<std::string> &strings);
 """
 
 source_cpp = r"""#include <iostream>
 #include "{{name}}.h"
 {% if requires is defined -%}
 {% for require in requires -%}
 #include "{{ as_name(require) }}.h"
@@ -149,14 +153,29 @@
     #endif
 
     // Libstdc++
     #if defined _GLIBCXX_USE_CXX11_ABI
     std::cout << "  {{name}}/{{version}}: _GLIBCXX_USE_CXX11_ABI "<< _GLIBCXX_USE_CXX11_ABI << "\n";
     #endif
 
+    // MSVC runtime
+    #if defined(_DEBUG)
+        #if defined(_MT) && defined(_DLL)
+        std::cout << "  {{name}}/{{version}}: MSVC runtime: MultiThreadedDebugDLL\n";
+        #elif defined(_MT)
+        std::cout << "  {{name}}/{{version}}: MSVC runtime: MultiThreadedDebug\n";
+        #endif
+    #else
+        #if defined(_MT) && defined(_DLL)
+        std::cout << "  {{name}}/{{version}}: MSVC runtime: MultiThreadedDLL\n";
+        #elif defined(_MT)
+        std::cout << "  {{name}}/{{version}}: MSVC runtime: MultiThreaded\n";
+        #endif
+    #endif
+
     // COMPILER VERSIONS
     #if _MSC_VER
     std::cout << "  {{name}}/{{version}}: _MSC_VER" << _MSC_VER<< "\n";
     #endif
 
     #if _MSVC_LANG
     std::cout << "  {{name}}/{{version}}: _MSVC_LANG" << _MSVC_LANG<< "\n";
@@ -204,14 +223,20 @@
     std::cout << "  {{name}}/{{version}}: __MINGW64__" << __MINGW64__<< "\n";
     #endif
 
     #if __CYGWIN__
     std::cout << "  {{name}}/{{version}}: __CYGWIN__" << __CYGWIN__<< "\n";
     #endif
 }
+
+void {{package_name}}_print_vector(const std::vector<std::string> &strings) {
+    for(std::vector<std::string>::const_iterator it = strings.begin(); it != strings.end(); ++it) {
+        std::cout << "{{package_name}}/{{version}} " << *it << std::endl;
+    }
+}
 """
 
 
 test_conanfile_v2 = """import os
 
 from conan import ConanFile
 from conan.tools.cmake import CMake, cmake_layout
@@ -252,17 +277,24 @@
 
 add_executable(example src/example.cpp)
 target_link_libraries(example {{name}}::{{name}})
 """
 
 
 test_main = """#include "{{name}}.h"
+#include <vector>
+#include <string>
 
 int main() {
     {{package_name}}();
+    
+    std::vector<std::string> vec;
+    vec.push_back("test_package");
+
+    {{package_name}}_print_vector(vec);
 }
 """
 
 cmake_lib_files = {"conanfile.py": conanfile_sources_v2,
                    "src/{{name}}.cpp": source_cpp,
                    "include/{{name}}.h": source_h,
                    "CMakeLists.txt": cmake_v2,
```

### Comparing `conan-server-2.0.6/conan/internal/api/new/meson_exe.py` & `conan-server-2.0.7/conan/internal/api/new/meson_exe.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/api/new/meson_lib.py` & `conan-server-2.0.7/conan/internal/api/new/meson_lib.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/api/new/msbuild_exe.py` & `conan-server-2.0.7/conan/internal/api/new/msbuild_exe.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/api/new/msbuild_lib.py` & `conan-server-2.0.7/conan/internal/api/new/msbuild_lib.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/cache/cache.py` & `conan-server-2.0.7/conan/internal/cache/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,37 +86,43 @@
         assert pref.package_id, "Package id must be known to get or create the package layout"
         assert pref.revision is None, "Package revision should be None"
         assert pref.timestamp is None
         package_path = self._get_tmp_path_pref(pref)
         self._create_path(package_path)
         return PackageLayout(pref, os.path.join(self.base_folder, package_path))
 
-    def get_reference_layout(self, ref: RecipeReference):
+    def get_recipe_layout(self, ref: RecipeReference):
         """ the revision must exists, the folder must exist
         """
-        assert ref.revision, "Recipe revision must be known to get the reference layout"
-        ref_data = self._db.try_get_recipe(ref)
+        if ref.revision is None:  # Latest one
+            ref_data = self._db.get_latest_recipe(ref)
+        else:
+            ref_data = self._db.get_recipe(ref)
         ref_path = ref_data.get("path")
+        ref = ref_data.get("ref")  # new revision with timestamp
         return RecipeLayout(ref, os.path.join(self.base_folder, ref_path))
 
+    def get_recipe_revisions_references(self, ref: RecipeReference):
+        return self._db.get_recipe_revisions_references(ref)
+
     def get_package_layout(self, pref: PkgReference):
         """ the revision must exists, the folder must exist
         """
         assert pref.ref.revision, "Recipe revision must be known to get the package layout"
         assert pref.package_id, "Package id must be known to get the package layout"
         assert pref.revision, "Package revision must be known to get the package layout"
         pref_data = self._db.try_get_package(pref)
         pref_path = pref_data.get("path")
         return PackageLayout(pref, os.path.join(self.base_folder, pref_path))
 
     def get_or_create_ref_layout(self, ref: RecipeReference):
         """ called by RemoteManager.get_recipe()
         """
         try:
-            return self.get_reference_layout(ref)
+            return self.get_recipe_layout(ref)
         except ConanReferenceDoesNotExistInDB:
             assert ref.revision, "Recipe revision must be known to create the package layout"
             reference_path = self._get_path(ref)
             self._db.create_recipe(reference_path, ref)
             self._create_path(reference_path, remove_contents=False)
             return RecipeLayout(ref, os.path.join(self.base_folder, reference_path))
 
@@ -138,44 +144,29 @@
         assert ref.revision
         assert ref.timestamp
         self._db.update_recipe_timestamp(ref)
 
     def list_references(self):
         return self._db.list_references()
 
-    def exists_rrev(self, ref):
-        return self._db.exists_rrev(ref)
-
     def exists_prev(self, pref):
         return self._db.exists_prev(pref)
 
-    def get_latest_recipe_reference(self, ref):
-        return self._db.get_latest_recipe_reference(ref)
-
     def get_latest_package_reference(self, pref):
         return self._db.get_latest_package_reference(pref)
 
-    def get_recipe_revisions_references(self, ref: RecipeReference, only_latest_rrev=False):
-        return self._db.get_recipe_revisions_references(ref, only_latest_rrev)
-
     def get_package_references(self, ref: RecipeReference, only_latest_prev=True):
         return self._db.get_package_references(ref, only_latest_prev)
 
     def get_package_revisions_references(self, pref: PkgReference, only_latest_prev=False):
         return self._db.get_package_revisions_references(pref, only_latest_prev)
 
     def get_matching_build_id(self, ref, build_id):
         return self._db.get_matching_build_id(ref, build_id)
 
-    def get_recipe_timestamp(self, ref):
-        return self._db.get_recipe_timestamp(ref)
-
-    def get_package_timestamp(self, pref):
-        return self._db.get_package_timestamp(pref)
-
     def remove_recipe(self, layout: RecipeLayout):
         layout.remove()
         # FIXME: This is clearing package binaries from DB, but not from disk/layout
         self._db.remove_recipe(layout.reference)
 
     def remove_package(self, layout: PackageLayout):
         layout.remove()
```

### Comparing `conan-server-2.0.6/conan/internal/cache/conan_reference_layout.py` & `conan-server-2.0.7/conan/internal/cache/conan_reference_layout.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/cache/db/cache_database.py` & `conan-server-2.0.7/conan/internal/cache/db/cache_database.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,38 +8,19 @@
 
 class CacheDatabase:
 
     def __init__(self, filename):
         self._recipes = RecipesDBTable(filename)
         self._packages = PackagesDBTable(filename)
 
-    def exists_rrev(self, ref):
-        # TODO: This logic could be done directly against DB
-        matching_rrevs = self.get_recipe_revisions_references(ref)
-        return len(matching_rrevs) > 0
-
     def exists_prev(self, ref):
         # TODO: This logic could be done directly against DB
         matching_prevs = self.get_package_revisions_references(ref)
         return len(matching_prevs) > 0
 
-    def get_recipe_timestamp(self, ref):
-        # TODO: Remove this once the ref contains the timestamp
-        ref_data = self.try_get_recipe(ref)
-        return ref_data["ref"].timestamp  # Must exist
-
-    def get_package_timestamp(self, ref):
-        ref_data = self.try_get_package(ref)
-        return ref_data["pref"].timestamp
-
-    def get_latest_recipe_reference(self, ref):
-        # TODO: This logic could be done directly in DB
-        rrevs = self.get_recipe_revisions_references(ref, True)
-        return rrevs[0] if rrevs else None
-
     def get_latest_package_reference(self, ref):
         prevs = self.get_package_revisions_references(ref, True)
         return prevs[0] if prevs else None
 
     def update_recipe_timestamp(self, ref):
         self._recipes.update_timestamp(ref)
 
@@ -59,18 +40,24 @@
         # TODO: This can also be done in a single query in DB
         for d in self._packages.get_package_references(ref):
             existing_build_id = d["build_id"]
             if existing_build_id == build_id:
                 return d["pref"]
         return None
 
-    def try_get_recipe(self, ref: RecipeReference):
+    def get_recipe(self, ref: RecipeReference):
         """ Returns the reference data as a dictionary (or fails) """
-        ref_data = self._recipes.get(ref)
-        return ref_data
+        return self._recipes.get_recipe(ref)
+
+    def get_latest_recipe(self, ref: RecipeReference):
+        """ Returns the reference data as a dictionary (or fails) """
+        return self._recipes.get_latest_recipe(ref)
+
+    def get_recipe_revisions_references(self, ref: RecipeReference):
+        return self._recipes.get_recipe_revisions_references(ref)
 
     def try_get_package(self, ref: PkgReference):
         """ Returns the reference data as a dictionary (or fails) """
         ref_data = self._packages.get(ref)
         return ref_data
 
     def create_recipe(self, path, ref: RecipeReference):
@@ -86,11 +73,7 @@
     def get_package_revisions_references(self, pref: PkgReference, only_latest_prev=False):
         return [d["pref"]
                 for d in self._packages.get_package_revisions_references(pref, only_latest_prev)]
 
     def get_package_references(self, ref: RecipeReference, only_latest_prev=True):
         return [d["pref"]
                 for d in self._packages.get_package_references(ref, only_latest_prev)]
-
-    def get_recipe_revisions_references(self, ref: RecipeReference, only_latest_rrev=False):
-        return [d["ref"]
-                for d in self._recipes.get_recipe_revisions_references(ref, only_latest_rrev)]
```

### Comparing `conan-server-2.0.6/conan/internal/cache/db/packages_table.py` & `conan-server-2.0.7/conan/internal/cache/db/packages_table.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/cache/db/recipes_table.py` & `conan-server-2.0.7/conan/internal/cache/db/recipes_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,57 +29,33 @@
             self.columns.reference: str(ref),
             self.columns.rrev: ref.revision,
         }
         where_expr = ' AND '.join(
             [f'{k}="{v}" ' if v is not None else f'{k} IS NULL' for k, v in where_dict.items()])
         return where_expr
 
-    def _set_clause(self, ref: RecipeReference, path=None):
-        set_dict = {
-            self.columns.reference: str(ref),
-            self.columns.rrev: ref.revision,
-            self.columns.path: path,
-            self.columns.timestamp: ref.timestamp,
-        }
-        set_expr = ', '.join([f'{k} = "{v}"' for k, v in set_dict.items() if v is not None])
-        return set_expr
-
-    def get(self, ref: RecipeReference):
-        """ Returns the row matching the reference or fails """
-        where_clause = self._where_clause(ref)
-        query = f'SELECT * FROM {self.table_name} ' \
-                f'WHERE {where_clause};'
-
-        with self.db_connection() as conn:
-            r = conn.execute(query)
-            row = r.fetchone()
-
-        if not row:
-            raise ConanReferenceDoesNotExistInDB(f"No entry for recipe '{repr(ref)}'")
-        return self._as_dict(self.row_type(*row))
-
     def create(self, path, ref: RecipeReference):
         assert ref is not None
         assert ref.revision is not None
         placeholders = ', '.join(['?' for _ in range(len(self.columns))])
         with self.db_connection() as conn:
             try:
                 conn.execute(f'INSERT INTO {self.table_name} '
-                                 f'VALUES ({placeholders})',
-                                 [str(ref), ref.revision, path, ref.timestamp])
-            except sqlite3.IntegrityError as e:
+                             f'VALUES ({placeholders})',
+                             [str(ref), ref.revision, path, ref.timestamp])
+            except sqlite3.IntegrityError:
                 raise ConanReferenceAlreadyExistsInDB(f"Reference '{repr(ref)}' already exists")
 
     def update_timestamp(self, ref: RecipeReference):
         assert ref.revision is not None
         assert ref.timestamp is not None
-        where_clause = self._where_clause(ref)
         query = f"UPDATE {self.table_name} " \
                 f'SET {self.columns.timestamp} = "{ref.timestamp}" ' \
-                f"WHERE {where_clause};"
+                f'WHERE {self.columns.reference}="{str(ref)}" ' \
+                f'AND {self.columns.rrev} = "{ref.revision}" '
         with self.db_connection() as conn:
             conn.execute(query)
 
     def remove(self, ref: RecipeReference):
         where_clause = self._where_clause(ref)
         query = f"DELETE FROM {self.table_name} " \
                 f"WHERE {where_clause};"
@@ -95,31 +71,46 @@
                     f'FROM {self.table_name} ' \
                     f'ORDER BY {self.columns.timestamp} DESC'
         with self.db_connection() as conn:
             r = conn.execute(query)
             result = [self._as_dict(self.row_type(*row)) for row in r.fetchall()]
         return result
 
-    def get_recipe_revisions_references(self, ref: RecipeReference, only_latest_rrev=False):
-        # FIXME: This is very fragile, we should disambiguate the function and check that revision
-        #        is always None if we want to check the revisions. Do another function to get the
-        #        time or check existence if needed
-        check_rrev = f'AND {self.columns.rrev} = "{ref.revision}" ' if ref.revision else ''
-        if only_latest_rrev:
-            query = f'SELECT {self.columns.reference}, ' \
-                    f'{self.columns.rrev}, ' \
-                    f'{self.columns.path}, ' \
-                    f'MAX({self.columns.timestamp}) ' \
-                    f'FROM {self.table_name} ' \
-                    f'WHERE {self.columns.reference}="{str(ref)}" ' \
-                    f'{check_rrev} '\
-                    f'GROUP BY {self.columns.reference} '  # OTHERWISE IT FAILS THE MAX()
-        else:
-            query = f'SELECT * FROM {self.table_name} ' \
-                    f'WHERE {self.columns.reference} = "{str(ref)}" ' \
-                    f'{check_rrev} ' \
-                    f'ORDER BY {self.columns.timestamp} DESC'
+    def get_recipe(self, ref: RecipeReference):
+        query = f'SELECT * FROM {self.table_name} ' \
+                f'WHERE {self.columns.reference}="{str(ref)}" ' \
+                f'AND {self.columns.rrev} = "{ref.revision}" '
+        with self.db_connection() as conn:
+            r = conn.execute(query)
+            row = r.fetchone()
+            if not row:
+                raise ConanReferenceDoesNotExistInDB(f"Recipe '{ref.repr_notime()}' not found")
+            ret = self._as_dict(self.row_type(*row))
+        return ret
+
+    def get_latest_recipe(self, ref: RecipeReference):
+        query = f'SELECT {self.columns.reference}, ' \
+                f'{self.columns.rrev}, ' \
+                f'{self.columns.path}, ' \
+                f'MAX({self.columns.timestamp}) ' \
+                f'FROM {self.table_name} ' \
+                f'WHERE {self.columns.reference} = "{str(ref)}" ' \
+                f'GROUP BY {self.columns.reference} '  # OTHERWISE IT FAILS THE MAX()
+
+        with self.db_connection() as conn:
+            r = conn.execute(query)
+            row = r.fetchone()
+            if row is None:
+                raise ConanReferenceDoesNotExistInDB(f"Recipe '{ref}' not found")
+            ret = self._as_dict(self.row_type(*row))
+        return ret
+
+    def get_recipe_revisions_references(self, ref: RecipeReference):
+        assert ref.revision is None
+        query = f'SELECT * FROM {self.table_name} ' \
+                f'WHERE {self.columns.reference} = "{str(ref)}" ' \
+                f'ORDER BY {self.columns.timestamp} DESC'
 
         with self.db_connection() as conn:
             r = conn.execute(query)
-            ret = [self._as_dict(self.row_type(*row)) for row in r.fetchall()]
+            ret = [self._as_dict(self.row_type(*row))["ref"] for row in r.fetchall()]
         return ret
```

### Comparing `conan-server-2.0.6/conan/internal/cache/db/table.py` & `conan-server-2.0.7/conan/internal/cache/db/table.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/conan_app.py` & `conan-server-2.0.7/conan/internal/conan_app.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/internal/deploy.py` & `conan-server-2.0.7/conan/internal/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from conans.client.cache.cache import ClientCache
 from conans.client.loader import load_python_file
 from conans.errors import ConanException
-from conans.util.files import rmdir
+from conans.util.files import rmdir, mkdir
 
 
 def _find_deployer(d, cache_deploy_folder):
     """ Implements the logic of finding a deployer, with priority:
     - 1) absolute paths
     - 2) relative to cwd
     - 3) in the cache/extensions/deploy folder
@@ -32,14 +32,15 @@
                       "direct_deploy.py": direct_deploy}.get(d)
     if builtin_deploy is not None:
         return builtin_deploy
     raise ConanException(f"Cannot find deployer '{d}'")
 
 
 def do_deploys(conan_api, graph, deploy, deploy_folder):
+    mkdir(deploy_folder)
     # Handle the deploys
     cache = ClientCache(conan_api.cache_folder)
     for d in deploy or []:
         deployer = _find_deployer(d, cache.deployers_path)
         # IMPORTANT: Use always kwargs to not break if it changes in the future
         deployer(graph=graph, output_folder=deploy_folder)
```

### Comparing `conan-server-2.0.6/conan/internal/integrity_check.py` & `conan-server-2.0.7/conan/internal/integrity_check.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/android/utils.py` & `conan-server-2.0.7/conan/tools/android/utils.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/apple/__init__.py` & `conan-server-2.0.7/conan/tools/apple/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/apple/apple.py` & `conan-server-2.0.7/conan/tools/apple/apple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from conans.util.runners import check_output_runner
 from conan.tools.build import cmd_args_to_string
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 
 def is_apple_os(conanfile):
     """returns True if OS is Apple one (Macos, iOS, watchOS or tvOS"""
     os_ = conanfile.settings.get_safe("os")
     return str(os_) in ['Macos', 'iOS', 'watchOS', 'tvOS']
```

### Comparing `conan-server-2.0.6/conan/tools/apple/xcodedeps.py` & `conan-server-2.0.7/conan/tools/apple/xcodedeps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import textwrap
 from collections import OrderedDict
 
 from jinja2 import Template
 
 from conan.internal import check_duplicated_generator
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.model.dependencies import get_transitive_requires
 from conans.util.files import load, save
 from conan.tools.apple.apple import _to_apple_arch
 
 GLOBAL_XCCONFIG_TEMPLATE = textwrap.dedent("""\
     // Includes both the toolchain and the dependencies
     // files if they exist
```

### Comparing `conan-server-2.0.6/conan/tools/apple/xcodetoolchain.py` & `conan-server-2.0.7/conan/tools/apple/xcodetoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/build/__init__.py` & `conan-server-2.0.7/conan/tools/build/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from shlex import quote
 
 from conan.tools.build.cppstd import check_max_cppstd, check_min_cppstd, \
     valid_max_cppstd, valid_min_cppstd, default_cppstd, supported_cppstd
 from conan.tools.build.cpu import build_jobs
 from conan.tools.build.cross_building import cross_building, can_run
 from conan.tools.build.stdcpp_library import stdcpp_library
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 CONAN_TOOLCHAIN_ARGS_FILE = "conanbuild.conf"
 CONAN_TOOLCHAIN_ARGS_SECTION = "toolchain"
 
 
 def use_win_mingw(conanfile):
     os_build = conanfile.settings_build.get_safe('os')
```

### Comparing `conan-server-2.0.6/conan/tools/build/cppstd.py` & `conan-server-2.0.7/conan/tools/build/cppstd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import operator
 
-from conans.errors import ConanInvalidConfiguration, ConanException
+from conan.errors import ConanInvalidConfiguration, ConanException
 from conans.model.version import Version
 
 
 def check_min_cppstd(conanfile, cppstd, gnu_extensions=False):
     """ Check if current cppstd fits the minimal version required.
 
         In case the current cppstd doesn't fit the minimal version required
```

### Comparing `conan-server-2.0.6/conan/tools/build/cpu.py` & `conan-server-2.0.7/conan/tools/build/cpu.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/build/cross_building.py` & `conan-server-2.0.7/conan/tools/build/cross_building.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/build/flags.py` & `conan-server-2.0.7/conan/tools/build/flags.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     elif compiler in ['gcc', 'apple-clang', 'clang', 'sun-cc']:
         if the_os == 'Macos' and subsystem == 'catalyst':
             # FIXME: This might be conflicting with Autotools --target cli arg
             apple_arch = _to_apple_arch(arch)
             if apple_arch:
                 # TODO: Could we define anything like `to_apple_target()`?
                 #       Check https://github.com/rust-lang/rust/issues/48862
-                return '--target=%s-apple-ios%s-macabi' % (apple_arch, subsystem_ios_version)
+                return f'--target={apple_arch}-apple-ios{subsystem_ios_version}-macabi'
         elif arch in ['x86_64', 'sparcv9', 's390x']:
             return '-m64'
         elif arch in ['x86', 'sparc']:
             return '-m32'
         elif arch in ['s390']:
             return '-m31'
         elif the_os == 'AIX':
@@ -65,29 +65,29 @@
     libcxx = conanfile.settings.get_safe("compiler.libcxx")
     if not libcxx:
         return None, None
     compiler = conanfile.settings.get_safe("compiler")
     lib = stdlib11 = None
     if compiler == "apple-clang":
         # In apple-clang 2 only values atm are "libc++" and "libstdc++"
-        lib = "-stdlib={}".format(libcxx)
+        lib = f'-stdlib={libcxx}'
     elif compiler == "clang" or compiler == "intel-cc":
         if libcxx == "libc++":
             lib = "-stdlib=libc++"
         elif libcxx == "libstdc++" or libcxx == "libstdc++11":
             lib = "-stdlib=libstdc++"
         # FIXME, something to do with the other values? Android c++_shared?
     elif compiler == "sun-cc":
         lib = {"libCstd": "-library=Cstd",
                "libstdcxx": "-library=stdcxx4",
                "libstlport": "-library=stlport4",
                "libstdc++": "-library=stdcpp"
                }.get(libcxx)
     elif compiler == "qcc":
-        lib = "-Y _{}".format(libcxx)
+        lib = f'-Y _{libcxx}'
 
     if compiler in ['clang', 'apple-clang', 'gcc']:
         if libcxx == "libstdc++":
             stdlib11 = "_GLIBCXX_USE_CXX11_ABI=0"
         elif libcxx == "libstdc++11" and conanfile.conf.get("tools.gnu:define_libcxx11_abi",
                                                             check_type=bool):
             stdlib11 = "_GLIBCXX_USE_CXX11_ABI=1"
@@ -174,44 +174,46 @@
         return ""
 
     func = {"gcc": _cppstd_gcc,
             "clang": _cppstd_clang,
             "apple-clang": _cppstd_apple_clang,
             "msvc": _cppstd_msvc,
             "intel-cc": _cppstd_intel_cc,
-            "mcst-lcc": _cppstd_mcst_lcc}.get(compiler, None)
+            "mcst-lcc": _cppstd_mcst_lcc}.get(compiler)
     flag = None
     if func:
         flag = func(Version(compiler_version), str(cppstd))
     return flag
 
 
 def cppstd_msvc_flag(visual_version, cppstd):
     # https://docs.microsoft.com/en-us/cpp/build/reference/std-specify-language-standard-version
-    v14 = None
-    v17 = None
-    v20 = None
-    v23 = None
+    if cppstd == "23":
+        if visual_version >= "193":
+            return "c++latest"
+    elif cppstd == "20":
+        if visual_version >= "192":
+            return "c++20"
+        elif visual_version >= "191":
+            return "c++latest"
+    elif cppstd == "17":
+        if visual_version >= "191":
+            return "c++17"
+        elif visual_version >= "190":
+            return "c++latest"
+    elif cppstd == "14":
+        if visual_version >= "190":
+            return "c++14"
 
-    if visual_version >= "190":
-        v14 = "c++14"
-        v17 = "c++latest"
-    if visual_version >= "191":
-        v17 = "c++17"
-        v20 = "c++latest"
-    if visual_version >= "192":
-        v20 = "c++20"
-    if visual_version >= "193":
-        v23 = "c++latest"
+    return None
 
-    return {"14": v14, "17": v17, "20": v20, "23": v23}.get(str(cppstd), None)
 
 def _cppstd_msvc(visual_version, cppstd):
     flag = cppstd_msvc_flag(visual_version, cppstd)
-    return "/std:%s" % flag if flag else None
+    return f'/std:{flag}' if flag else None
 
 
 def _cppstd_apple_clang(clang_version, cppstd):
     """
     Inspired in:
     https://github.com/Kitware/CMake/blob/master/Modules/Compiler/AppleClang-CXX.cmake
     """
@@ -229,40 +231,40 @@
         vgnu14 = "gnu++14"
     elif clang_version >= "5.1":
         v14 = "c++1y"
         vgnu14 = "gnu++1y"
 
     # Not confirmed that it didn't work before 9.1 but 1z is still valid, so we are ok
     # Note: cmake allows c++17 since version 10.0
-    if Version(clang_version) >= "9.1":
+    if clang_version >= "9.1":
         v17 = "c++17"
         vgnu17 = "gnu++17"
-    elif Version(clang_version) >= "6.1":
+    elif clang_version >= "6.1":
         v17 = "c++1z"
         vgnu17 = "gnu++1z"
 
-    if Version(clang_version) >= "13.0":
+    if clang_version >= "13.0":
         v20 = "c++20"
         vgnu20 = "gnu++20"
-    elif Version(clang_version) >= "10.0":
+    elif clang_version >= "10.0":
         v20 = "c++2a"
         vgnu20 = "gnu++2a"
 
-    if Version(clang_version) >= "13.0":
+    if clang_version >= "13.0":
         v23 = "c++2b"
         vgnu23 = "gnu++2b"
 
     flag = {"98": v98, "gnu98": vgnu98,
             "11": v11, "gnu11": vgnu11,
             "14": v14, "gnu14": vgnu14,
             "17": v17, "gnu17": vgnu17,
             "20": v20, "gnu20": vgnu20,
-            "23": v23, "gnu23": vgnu23}.get(cppstd, None)
+            "23": v23, "gnu23": vgnu23}.get(cppstd)
 
-    return "-std=%s" % flag if flag else None
+    return f'-std={flag}' if flag else None
 
 
 def _cppstd_clang(clang_version, cppstd):
     """
     Inspired in:
     https://github.com/Kitware/CMake/blob/
     1fe2dc5ef2a1f262b125a2ba6a85f624ce150dd2/Modules/Compiler/Clang-CXX.cmake
@@ -308,16 +310,16 @@
         vgnu23 = "gnu++2b"
 
     flag = {"98": v98, "gnu98": vgnu98,
             "11": v11, "gnu11": vgnu11,
             "14": v14, "gnu14": vgnu14,
             "17": v17, "gnu17": vgnu17,
             "20": v20, "gnu20": vgnu20,
-            "23": v23, "gnu23": vgnu23}.get(cppstd, None)
-    return "-std=%s" % flag if flag else None
+            "23": v23, "gnu23": vgnu23}.get(cppstd)
+    return f'-std={flag}' if flag else None
 
 
 def _cppstd_gcc(gcc_version, cppstd):
     """https://github.com/Kitware/CMake/blob/master/Modules/Compiler/GNU-CXX.cmake"""
     # https://gcc.gnu.org/projects/cxx-status.html
     v98 = vgnu98 = v11 = vgnu11 = v14 = vgnu14 = v17 = vgnu17 = v20 = vgnu20 = v23 = vgnu23 = None
 
@@ -351,25 +353,25 @@
         v20 = "c++2a"
         vgnu20 = "gnu++2a"
 
     if gcc_version >= "11":
         v23 = "c++2b"
         vgnu23 = "gnu++2b"
 
-    if Version(gcc_version) >= "12":
+    if gcc_version >= "12":
         v20 = "c++20"
         vgnu20 = "gnu++20"
 
     flag = {"98": v98, "gnu98": vgnu98,
             "11": v11, "gnu11": vgnu11,
             "14": v14, "gnu14": vgnu14,
             "17": v17, "gnu17": vgnu17,
             "20": v20, "gnu20": vgnu20,
             "23": v23, "gnu23": vgnu23}.get(cppstd)
-    return "-std=%s" % flag if flag else None
+    return f'-std={flag}' if flag else None
 
 
 def _cppstd_intel_common(intel_version, cppstd, vgnu98, vgnu0x):
     # https://software.intel.com/en-us/cpp-compiler-developer-guide-and-reference-std-qstd
     # https://software.intel.com/en-us/articles/intel-cpp-compiler-release-notes
     # NOTE: there are only gnu++98 and gnu++0x, and only for Linux/macOS
     v98 = v11 = v14 = v17 = v20 = None
@@ -393,20 +395,20 @@
             "14": v14, "gnu14": vgnu14,
             "17": v17, "gnu17": vgnu17,
             "20": v20, "gnu20": vgnu20}.get(cppstd)
 
 
 def _cppstd_intel_gcc(intel_version, cppstd):
     flag = _cppstd_intel_common(intel_version, cppstd, "gnu++98", "gnu++0x")
-    return "-std=%s" % flag if flag else None
+    return f'-std={flag}' if flag else None
 
 
 def _cppstd_intel_visualstudio(intel_version, cppstd):
     flag = _cppstd_intel_common(intel_version, cppstd, None, None)
-    return "/Qstd=%s" % flag if flag else None
+    return f'/Qstd={flag}' if flag else None
 
 
 def _cppstd_mcst_lcc(mcst_lcc_version, cppstd):
     v11 = vgnu11 = v14 = vgnu14 = v17 = vgnu17 = v20 = vgnu20 = None
 
     if mcst_lcc_version >= "1.21":
         v11 = "c++11"
@@ -425,15 +427,15 @@
     # FIXME: What is this "03"?? that is not a valid cppstd in the settings.yml
     flag = {"98": "c++98", "gnu98": "gnu++98",
             "03": "c++03", "gnu03": "gnu++03",
             "11": v11, "gnu11": vgnu11,
             "14": v14, "gnu14": vgnu14,
             "17": v17, "gnu17": vgnu17,
             "20": v20, "gnu20": vgnu20}.get(cppstd)
-    return "-std=%s" % flag if flag else None
+    return f'-std={flag}' if flag else None
 
 
 def _cppstd_intel_cc(_, cppstd):
     """
     Inspired in:
     https://software.intel.com/content/www/us/en/develop/documentation/
     oneapi-dpcpp-cpp-compiler-dev-guide-and-reference/top/compiler-reference/
@@ -457,9 +459,9 @@
 
     flag = {"98": v98, "gnu98": vgnu98,
             "03": v03, "gnu03": vgnu03,
             "11": v11, "gnu11": vgnu11,
             "14": v14, "gnu14": vgnu14,
             "17": v17, "gnu17": vgnu17,
             "20": v20, "gnu20": vgnu20,
-            "23": v23, "gnu23": vgnu23}.get(cppstd, None)
-    return "-std=%s" % flag if flag else None
+            "23": v23, "gnu23": vgnu23}.get(cppstd)
+    return f'-std={flag}' if flag else None
```

### Comparing `conan-server-2.0.6/conan/tools/build/stdcpp_library.py` & `conan-server-2.0.7/conan/tools/build/stdcpp_library.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/cmake/cmake.py` & `conan-server-2.0.7/conan/tools/cmake/cmake.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from conan.tools.build import build_jobs, cmd_args_to_string
 from conan.tools.cmake.presets import load_cmake_presets
 from conan.tools.cmake.utils import is_multi_configuration
 from conan.tools.files import chdir, mkdir
 from conan.tools.microsoft.msbuild import msbuild_verbosity_cmd_line_arg
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 
 def _cmake_cmd_line_args(conanfile, generator):
     args = []
     if not generator:
         return args
 
@@ -100,14 +100,17 @@
         if not variables:
             variables = {}
         self._cache_variables.update(variables)
 
         arg_list.extend(['-D{}="{}"'.format(k, v) for k, v in self._cache_variables.items()])
         arg_list.append('"{}"'.format(cmakelist_folder))
 
+        if not cli_args or ("--log-level" not in cli_args and "--loglevel" not in cli_args):
+            arg_list.extend(self._cmake_log_levels_args)
+
         if cli_args:
             arg_list.extend(cli_args)
 
         command = " ".join(arg_list)
         with chdir(self, build_folder):
             self._conanfile.run(command)
 
@@ -128,14 +131,17 @@
             args = ["--target", target]
         if cli_args:
             args.extend(cli_args)
 
         cmd_line_args = _cmake_cmd_line_args(self._conanfile, self._generator)
         if build_tool_args:
             cmd_line_args.extend(build_tool_args)
+
+        args.extend(self._compilation_verbosity_arg)
+
         if cmd_line_args:
             args += ['--'] + cmd_line_args
 
         arg_list = ['"{}"'.format(bf), build_config, cmd_args_to_string(args)]
         arg_list = " ".join(filter(None, arg_list))
         command = "%s --build %s" % (self._cmake_program, arg_list)
         self._conanfile.run(command, env=env)
@@ -177,14 +183,15 @@
         build_config = "--config {}".format(bt) if bt and is_multi else ""
 
         pkg_folder = '"{}"'.format(self._conanfile.package_folder.replace("\\", "/"))
         build_folder = '"{}"'.format(self._conanfile.build_folder)
         arg_list = ["--install", build_folder, build_config, "--prefix", pkg_folder]
         if component:
             arg_list.extend(["--component", component])
+        arg_list.extend(self._compilation_verbosity_arg)
         arg_list = " ".join(filter(None, arg_list))
         command = "%s %s" % (self._cmake_program, arg_list)
         self._conanfile.run(command)
 
     def test(self, build_type=None, target=None, cli_args=None, build_tool_args=None, env=""):
         """
         Equivalent to running cmake --build . --target=RUN_TESTS.
@@ -205,7 +212,27 @@
             target = "RUN_TESTS" if is_multi and not is_ninja else "test"
 
         # CTest behavior controlled by CTEST_ env-vars should be directly defined in [buildenv]
         # The default for ``test()`` is both the buildenv and the runenv
         env = ["conanbuild", "conanrun"] if env == "" else env
         self._build(build_type=build_type, target=target, cli_args=cli_args,
                     build_tool_args=build_tool_args, env=env)
+
+    @property
+    def _compilation_verbosity_arg(self):
+        """
+        Controls build tool verbosity, that is, those controlled by -DCMAKE_VERBOSE_MAKEFILE
+        See https://cmake.org/cmake/help/latest/manual/cmake.1.html#cmdoption-cmake-build-v
+        """
+        verbosity = self._conanfile.conf.get("tools.compilation:verbosity",
+                                             choices=("quiet", "verbose"))
+        return ["--verbose"] if verbosity == "verbose" else []
+
+    @property
+    def _cmake_log_levels_args(self):
+        """
+        Controls CMake's own verbosity levels.
+        See https://cmake.org/cmake/help/latest/manual/cmake.1.html#cmdoption-cmake-log-level
+        :return:
+        """
+        log_level = self._conanfile.conf.get("tools.build:verbosity", choices=("quiet", "verbose"))
+        return ["--loglevel=" + log_level.upper()] if log_level is not None else []
```

### Comparing `conan-server-2.0.6/conan/tools/cmake/cmakedeps/cmakedeps.py` & `conan-server-2.0.7/conan/tools/cmake/cmakedeps/cmakedeps.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     FIND_MODE_MODULE
 from conan.tools.cmake.cmakedeps.templates.config import ConfigTemplate
 from conan.tools.cmake.cmakedeps.templates.config_version import ConfigVersionTemplate
 from conan.tools.cmake.cmakedeps.templates.macros import MacrosTemplate
 from conan.tools.cmake.cmakedeps.templates.target_configuration import TargetConfigurationTemplate
 from conan.tools.cmake.cmakedeps.templates.target_data import ConfigDataTemplate
 from conan.tools.cmake.cmakedeps.templates.targets import TargetsTemplate
+from conan.tools.files import save
 from conans.client.generators import relativize_generated_file
-from conans.errors import ConanException
-from conans.util.files import save
+from conan.errors import ConanException
 
 
 class CMakeDeps(object):
 
     def __init__(self, conanfile):
         self._conanfile = conanfile
         self.arch = self._conanfile.settings.get_safe("arch")
@@ -38,15 +38,15 @@
         This method will save the generated files to the conanfile.generators_folder
         """
         check_duplicated_generator(self, self._conanfile)
 
         # Current directory is the generators_folder
         generator_files = self.content
         for generator_file, content in generator_files.items():
-            save(generator_file, content)
+            save(self._conanfile, generator_file, content)
 
     @property
     def content(self):
         macros = MacrosTemplate()
         ret = {macros.filename: macros.render()}
 
         host_req = self._conanfile.dependencies.host
```

### Comparing `conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/__init__.py` & `conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import jinja2
 from jinja2 import Template
 
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 
 class CMakeDepsFileTemplate(object):
 
     def __init__(self, cmakedeps, require, conanfile, generating_module=False):
         self.cmakedeps = cmakedeps
         self.require = require
@@ -26,28 +26,19 @@
 
     @property
     def suffix(self):
         if not self.require.build:
             return ""
         return self.cmakedeps.build_context_suffix.get(self.conanfile.ref.name, "")
 
-    @property
-    def build_modules_activated(self):
-        if self.require.build:
-            return self.conanfile.ref.name in self.cmakedeps.build_context_build_modules
-        else:
-            return self.conanfile.ref.name not in self.cmakedeps.build_context_build_modules
-
     def render(self):
         try:
             context = self.context
         except Exception as e:
             raise ConanException("error generating context for '{}': {}".format(self.conanfile, e))
-        if context is None:
-            return
 
         # Cache the template instance as a class attribute to greatly speed up the rendering
         # NOTE: this assumes that self.template always returns the same string
         template_instance = getattr(type(self), "template_instance", None)
         if template_instance is None:
             template_instance = Template(self.template, trim_blocks=True, lstrip_blocks=True,
                                          undefined=jinja2.StrictUndefined)
```

### Comparing `conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/config.py` & `conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/config.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/config_version.py` & `conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/config_version.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/macros.py` & `conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/macros.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/target_configuration.py` & `conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/target_configuration.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/target_data.py` & `conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/target_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import textwrap
 
 from conan.tools.cmake.cmakedeps import FIND_MODE_NONE, FIND_MODE_CONFIG, FIND_MODE_MODULE, \
     FIND_MODE_BOTH
 from conan.tools.cmake.cmakedeps.templates import CMakeDepsFileTemplate
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.model.dependencies import get_transitive_requires
 
 
 """
 
 foo-release-x86_64-data.cmake
 
@@ -23,17 +23,24 @@
         data_fname += "{}-{}".format(self.file_name, self.configuration.lower())
         if self.arch:
             data_fname += "-{}".format(self.arch)
         data_fname += "-data.cmake"
         return data_fname
 
     @property
+    def _build_modules_activated(self):
+        if self.require.build:
+            return self.conanfile.ref.name in self.cmakedeps.build_context_build_modules
+        else:
+            return self.conanfile.ref.name not in self.cmakedeps.build_context_build_modules
+
+    @property
     def context(self):
         global_cpp = self._get_global_cpp_cmake()
-        if not self.build_modules_activated:
+        if not self._build_modules_activated:
             global_cpp.build_modules_paths = ""
 
         components = self._get_required_components_cpp()
         # using the target names to name components, may change in the future?
         components_names = " ".join([components_target_name for components_target_name, _ in
                                     reversed(components)])
 
@@ -191,30 +198,30 @@
         transitive_requires = get_transitive_requires(self.cmakedeps._conanfile, self.conanfile)
         for comp_name, comp in sorted_comps.items():
             deps_cpp_cmake = _TargetDataContext(comp, pfolder_var_name, self._root_folder,
                                                 self.require, self.cmake_package_type,
                                                 self.is_host_windows)
 
             public_comp_deps = []
-            for require in comp.requires:
-                if "::" in require:  # Points to a component of a different package
-                    pkg, cmp_name = require.split("::")
+            for required_pkg, required_comp in comp.parsed_requires():
+                if required_pkg is not None:  # Points to a component of a different package
                     try:  # Make sure the declared dependency is at least in the recipe requires
-                        self.conanfile.dependencies[pkg]
+                        self.conanfile.dependencies[required_pkg]
                     except KeyError:
                         raise ConanException(f"{self.conanfile}: component '{comp_name}' required "
-                                             f"'{require}', but '{pkg}' is not a direct dependency")
+                                             f"'{required_pkg}::{required_comp}', "
+                                             f"but '{required_pkg}' is not a direct dependency")
                     try:
-                        req = transitive_requires[pkg]
+                        req = transitive_requires[required_pkg]
                     except KeyError:  # The transitive dep might have been skipped
                         pass
                     else:
-                        public_comp_deps.append(self.get_component_alias(req, cmp_name))
+                        public_comp_deps.append(self.get_component_alias(req, required_comp))
                 else:  # Points to a component of same package
-                    public_comp_deps.append(self.get_component_alias(self.conanfile, require))
+                    public_comp_deps.append(self.get_component_alias(self.conanfile, required_comp))
             deps_cpp_cmake.public_deps = " ".join(public_comp_deps)
             component_target_name = self.get_component_alias(self.conanfile, comp_name)
             ret.append((component_target_name, deps_cpp_cmake))
         ret.reverse()
         return ret
 
     def _get_dependency_filenames(self):
```

### Comparing `conan-server-2.0.6/conan/tools/cmake/cmakedeps/templates/targets.py` & `conan-server-2.0.7/conan/tools/cmake/cmakedeps/templates/targets.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/cmake/layout.py` & `conan-server-2.0.7/conan/tools/cmake/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from conans.client.graph.graph import RECIPE_CONSUMER, RECIPE_EDITABLE
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 
 def cmake_layout(conanfile, generator=None, src_folder=".", build_folder="build"):
     """
     :param conanfile: The current recipe object. Always use ``self``.
     :param generator: Allow defining the CMake generator. In most cases it doesn't need to be passed, as it will get the value from the configuration              ``tools.cmake.cmaketoolchain:generator``, or it will automatically deduce the generator from the ``settings``
     :param src_folder: Value for ``conanfile.folders.source``, change it if your source code
```

### Comparing `conan-server-2.0.6/conan/tools/cmake/presets.py` & `conan-server-2.0.7/conan/tools/cmake/presets.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import platform
 
 from conan.api.output import ConanOutput
 from conan.tools.cmake.layout import get_build_folder_custom_vars
 from conan.tools.cmake.utils import is_multi_configuration
 from conan.tools.microsoft import is_msvc
 from conans.client.graph.graph import RECIPE_CONSUMER
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.util.files import save, load
 
 
 def write_cmake_presets(conanfile, toolchain_file, generator, cache_variables,
                         user_presets_path=None, preset_prefix=None):
     preset_path, preset_data = _CMakePresets.generate(conanfile, toolchain_file, generator,
                                                       cache_variables, preset_prefix)
```

### Comparing `conan-server-2.0.6/conan/tools/cmake/toolchain/blocks.py` & `conan-server-2.0.7/conan/tools/cmake/toolchain/blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from conan.tools.build import build_jobs
 from conan.tools.build.flags import architecture_flag, libcxx_flags
 from conan.tools.build.cross_building import cross_building
 from conan.tools.cmake.toolchain import CONAN_TOOLCHAIN_FILENAME
 from conan.tools.intel import IntelCC
 from conan.tools.microsoft.visual import msvc_version_to_toolset_version
 from conans.client.subsystems import deduce_subsystem, WINDOWS
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.util.files import load
 
 
 class Block(object):
     def __init__(self, conanfile, toolchain):
         self._conanfile = conanfile
         self._toolchain = toolchain
@@ -704,15 +704,16 @@
         if settings.get_safe("os") == "WindowsCE":
             return settings.get_safe("os.platform")
 
         if compiler in ("msvc", "clang") and generator and "Visual" in generator:
             return {"x86": "Win32",
                     "x86_64": "x64",
                     "armv7": "ARM",
-                    "armv8": "ARM64"}.get(arch)
+                    "armv8": "ARM64",
+                    "arm64ec": "ARM64EC"}.get(arch)
         return None
 
     def _get_generic_system_name(self):
         os_host = self._conanfile.settings.get_safe("os")
         os_build = self._conanfile.settings_build.get_safe("os")
         arch_host = self._conanfile.settings.get_safe("arch")
         arch_build = self._conanfile.settings_build.get_safe("arch")
```

### Comparing `conan-server-2.0.6/conan/tools/cmake/toolchain/toolchain.py` & `conan-server-2.0.7/conan/tools/cmake/toolchain/toolchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     AndroidSystemBlock, AppleSystemBlock, FPicBlock, ArchitectureBlock, GLibCXXBlock, VSRuntimeBlock, \
     CppStdBlock, ParallelBlock, CMakeFlagsInitBlock, TryCompileBlock, FindFiles, PkgConfigBlock, \
     SkipRPath, SharedLibBock, OutputDirsBlock, ExtraFlagsBlock, CompilersBlock, LinkerScriptsBlock
 from conan.tools.intel import IntelCC
 from conan.tools.microsoft import VCVars
 from conan.tools.microsoft.visual import vs_ide_version
 from conans.client.generators import relativize_generated_file
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.model.options import _PackageOption
 from conans.util.files import save
 
 
 class Variables(OrderedDict):
     _configuration_types = None  # Needed for py27 to avoid infinite recursion
```

### Comparing `conan-server-2.0.6/conan/tools/env/environment.py` & `conan-server-2.0.7/conan/tools/env/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import textwrap
 from collections import OrderedDict
 from contextlib import contextmanager
 
 from conans.client.generators import relativize_generated_file
 from conans.client.subsystems import deduce_subsystem, WINDOWS, subsystem_path
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.model.recipe_ref import ref_matches
 from conans.util.files import save
 
 
 class _EnvVarPlaceHolder:
     pass
```

### Comparing `conan-server-2.0.6/conan/tools/env/virtualbuildenv.py` & `conan-server-2.0.7/conan/tools/env/virtualbuildenv.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/env/virtualrunenv.py` & `conan-server-2.0.7/conan/tools/env/virtualrunenv.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/files/__init__.py` & `conan-server-2.0.7/conan/tools/files/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from conan.tools.files.files import load, save, mkdir, rmdir, rm, ftp_download, download, get, \
     rename, chdir, unzip, replace_in_file, collect_libs, check_md5, check_sha1, check_sha256, \
     move_folder_contents
 
 from conan.tools.files.patches import patch, apply_conandata_patches, export_conandata_patches
-from conan.tools.files.cpp_package import CppPackage
 from conan.tools.files.packager import AutoPackager
 from conan.tools.files.symlinks import symlinks
 from conan.tools.files.copy_pattern import copy
 from conan.tools.files.conandata import update_conandata
```

### Comparing `conan-server-2.0.6/conan/tools/files/conandata.py` & `conan-server-2.0.7/conan/tools/files/conandata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import yaml
 
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.util.files import load, save
 
 
 def update_conandata(conanfile, data):
     """
     Tool to modify the ``conandata.yml`` once it is exported. It can be used, for example:
```

### Comparing `conan-server-2.0.6/conan/tools/files/copy_pattern.py` & `conan-server-2.0.7/conan/tools/files/copy_pattern.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/files/files.py` & `conan-server-2.0.7/conan/tools/files/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import sys
 from contextlib import contextmanager
 from fnmatch import fnmatch
 from shutil import which
 
 
 from conans.client.downloaders.caching_file_downloader import SourcesCachingDownloader
-from conans.errors import ConanException
-from conans.util.files import rmdir as _internal_rmdir
+from conan.errors import ConanException
+from conans.util.files import rmdir as _internal_rmdir, human_size
 from conans.util.sha import check_with_algorithm_sum
 
 
 def load(conanfile, path, encoding="utf-8"):
     """
     Utility function to load files in one line. It will manage the open and close of the file,
     and load binary encodings. Returns the content of the file.
@@ -317,17 +317,17 @@
             zip_info = [m for m in zip_info if m.filename != (common_folder + "/")]
             for member in zip_info:
                 name = member.filename.replace("\\", "/")
                 member.filename = name.split("/", 1)[1]
 
         uncompress_size = sum((file_.file_size for file_ in zip_info))
         if uncompress_size > 100000:
-            output.info("Unzipping %s, this can take a while" % _human_size(uncompress_size))
+            output.info("Unzipping %s, this can take a while" % human_size(uncompress_size))
         else:
-            output.info("Unzipping %s" % _human_size(uncompress_size))
+            output.info("Unzipping %s" % human_size(uncompress_size))
         extracted_size = 0
 
         print_progress.last_size = -1
         if platform.system() == "Windows":
             for file_ in zip_info:
                 extracted_size += file_.file_size
                 print_progress(extracted_size, uncompress_size)
@@ -380,42 +380,14 @@
                         member.linkname = member.linkpath
             if pattern:
                 members = list(filter(lambda m: fnmatch(m.name, pattern),
                                       tarredgzippedFile.getmembers()))
             tarredgzippedFile.extractall(destination, members=members)
 
 
-def _human_size(size_bytes):
-    """
-    format a size in bytes into a 'human' file size, e.g. B, KB, MB, GB, TB, PB
-    Note that bytes will be reported in whole numbers but KB and above will have
-    greater precision.  e.g. 43 B, 443 KB, 4.3 MB, 4.43 GB, etc
-    """
-    UNIT_SIZE = 1000.0
-
-    suffixes_table = [('B', 0), ('KB', 1), ('MB', 1), ('GB', 2), ('TB', 2), ('PB', 2)]
-
-    num = float(size_bytes)
-    the_precision = None
-    the_suffix = None
-    for suffix, precision in suffixes_table:
-        the_precision = precision
-        the_suffix = suffix
-        if num < UNIT_SIZE:
-            break
-        num /= UNIT_SIZE
-
-    if the_precision == 0:
-        formatted_size = "%d" % num
-    else:
-        formatted_size = str(round(num, ndigits=the_precision))
-
-    return "%s%s" % (formatted_size, the_suffix)
-
-
 def check_sha1(conanfile, file_path, signature):
     """
     Check that the specified ``sha1`` of the ``file_path`` matches with signature.
     If doesn’t match it will raise a ``ConanException``.
 
     :param conanfile: Conanfile object.
     :param file_path: Path of the file to check.
@@ -518,19 +490,18 @@
         if ext != ".lib" and name.startswith("lib"):
             name = name[3:]
         result.append(name)
     result.sort()
     return result
 
 
-# TODO: Do NOT document this yet. It is unclear the interface, maybe should be split
-def move_folder_contents(src_folder, dst_folder):
-    """ replaces the current folder contents with the contents of one child folder. This
-    is used in the SCM monorepo flow, when it is necessary to use one subproject subfolder
-    to replace the whole cloned git repo
+def move_folder_contents(conanfile, src_folder, dst_folder):
+    """ replaces the dst_folder contents with the contents of the src_folder, which can be a
+    child folder of dst_folder. This is used in the SCM monorepo flow, when it is necessary
+    to use one subproject subfolder to replace the whole cloned git repo
     /base-folder                       /base-folder
         /pkg  (src folder)                 /other/<otherfiles>
           /other/<otherfiles>              /pkg/<pkgfiles>
           /pkg/<pkgfiles>                  <files>
           <files>
         /siblings
         <siblingsfiles>
```

### Comparing `conan-server-2.0.6/conan/tools/files/packager.py` & `conan-server-2.0.7/conan/tools/files/packager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 
 class _PatternEntry(object):
 
     def __init__(self):
         self.include = []
         self.lib = []
@@ -34,14 +34,17 @@
         self.patterns.source.include = ["*.h", "*.hpp", "*.hxx"]
         self.patterns.source.lib = []
         self.patterns.source.bin = []
 
         self.patterns.build.include = ["*.h", "*.hpp", "*.hxx"]
         self.patterns.build.lib = ["*.so", "*.so.*", "*.a", "*.lib", "*.dylib"]
         self.patterns.build.bin = ["*.exe", "*.dll"]
+        conanfile.output.warning("AutoPackager is **** deprecated ****", warn_tag="deprecated")
+        conanfile.output.warning("AutoPackager **** will be removed ****", warn_tag="deprecated")
+        conanfile.output.warning("Use explicit copy() calls instead", warn_tag="deprecated")
 
     def run(self):
         cf = self._conanfile
         # Check that the components declared in source/build are in package
         cnames = set(cf.cpp.source.components)
         cnames = cnames.union(set(cf.cpp.build.components))
         if cnames.difference(set(cf.cpp.package.components)):
@@ -54,16 +57,16 @@
                 if cname in cf.cpp.source.components:
                     self._package_cppinfo("source", cf.cpp.source.components[cname],
                                           cf.cpp.package.components[cname])
                 if cname in cf.cpp.build.components:
                     self._package_cppinfo("build", cf.cpp.build.components[cname],
                                           cf.cpp.package.components[cname])
         else:  # No components declared
-           self._package_cppinfo("source", cf.cpp.source, cf.cpp.package)
-           self._package_cppinfo("build", cf.cpp.build, cf.cpp.package)
+            self._package_cppinfo("source", cf.cpp.source, cf.cpp.package)
+            self._package_cppinfo("build", cf.cpp.build, cf.cpp.package)
 
     def _package_cppinfo(self, origin_name, origin_cppinfo, dest_cppinfo):
         """
         @param origin_name: one from ["source", "build"]
         @param origin_cppinfo: cpp_info object of an origin (can be a component cppinfo too)
         @param dest_cppinfo: cpp_info object of the package or a component from package
         """
```

### Comparing `conan-server-2.0.6/conan/tools/files/patches.py` & `conan-server-2.0.7/conan/tools/files/patches.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import shutil
 
 import patch_ng
 
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.util.files import mkdir
 
 
 class PatchLogHandler(logging.Handler):
     def __init__(self, scoped_output, patch_file):
         logging.Handler.__init__(self, logging.DEBUG)
         self._scoped_output = scoped_output
```

### Comparing `conan-server-2.0.6/conan/tools/files/symlinks/symlinks.py` & `conan-server-2.0.7/conan/tools/files/symlinks/symlinks.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/gnu/autotools.py` & `conan-server-2.0.7/conan/tools/gnu/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/gnu/autotoolsdeps.py` & `conan-server-2.0.7/conan/tools/gnu/autotoolsdeps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from conan.internal import check_duplicated_generator
+from conan.tools import CppInfo
 from conan.tools.env import Environment
 from conan.tools.gnu.gnudeps_flags import GnuDepsFlags
-from conans.model.build_info import CppInfo
 
 
 class AutotoolsDeps:
     def __init__(self, conanfile):
         self._conanfile = conanfile
         self._environment = None
-        self._ordered_deps = []
+        self._ordered_deps = None
 
     @property
     def ordered_deps(self):
-        if not self._ordered_deps:
+        if self._ordered_deps is None:
             deps = self._conanfile.dependencies.host.topological_sort
             self._ordered_deps = [dep for dep in reversed(deps.values())]
         return self._ordered_deps
 
     def _get_cpp_info(self):
-        ret = CppInfo()
+        ret = CppInfo(self._conanfile)
         for dep in self.ordered_deps:
             dep_cppinfo = dep.cpp_info.aggregated_components()
             # In case we have components, aggregate them, we do not support isolated
             # "targets" with autotools
             ret.merge(dep_cppinfo)
         return ret
 
@@ -51,15 +51,15 @@
             # Ldflags
             ldflags = flags.sharedlinkflags
             ldflags.extend(flags.exelinkflags)
             ldflags.extend(flags.frameworks)
             ldflags.extend(flags.framework_paths)
             ldflags.extend(flags.lib_paths)
 
-            ## set the rpath in Macos so that the library are found in the configure step
+            # set the rpath in Macos so that the library are found in the configure step
             if self._conanfile.settings.get_safe("os") == "Macos":
                 ldflags.extend(self._rpaths_flags())
 
             # libs
             libs = flags.libs
             libs.extend(flags.system_libs)
```

### Comparing `conan-server-2.0.6/conan/tools/gnu/autotoolstoolchain.py` & `conan-server-2.0.7/conan/tools/gnu/autotoolstoolchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from conan.tools.apple.apple import get_apple_sdk_fullname
 from conan.tools.build import cmd_args_to_string, save_toolchain_args
 from conan.tools.build.cross_building import cross_building
 from conan.tools.build.flags import architecture_flag, build_type_flags, cppstd_flag, build_type_link_flags, libcxx_flags
 from conan.tools.env import Environment
 from conan.tools.gnu.get_gnu_triplet import _get_gnu_triplet
 from conan.tools.microsoft import VCVars, msvc_runtime_flag, unix_path
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.model.pkg_type import PackageType
 
 
 class AutotoolsToolchain:
     def __init__(self, conanfile, namespace=None, prefix="/"):
         """
```

### Comparing `conan-server-2.0.6/conan/tools/gnu/get_gnu_triplet.py` & `conan-server-2.0.7/conan/tools/gnu/get_gnu_triplet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 
 def _get_gnu_triplet(os_, arch, compiler=None):
     """
     Returns string with <machine>-<vendor>-<op_system> triplet (<vendor> can be omitted in practice)
 
     :param os_: os to be used to create the triplet
```

### Comparing `conan-server-2.0.6/conan/tools/gnu/gnudeps_flags.py` & `conan-server-2.0.7/conan/tools/gnu/gnudeps_flags.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/gnu/pkgconfig.py` & `conan-server-2.0.7/conan/tools/gnu/pkgconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from conan.tools.build import cmd_args_to_string
 from conan.tools.env import Environment
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.util.runners import check_output_runner
 
 
 class PkgConfig:
 
     def __init__(self, conanfile, library, pkg_config_path=None):
         """
```

### Comparing `conan-server-2.0.6/conan/tools/gnu/pkgconfigdeps.py` & `conan-server-2.0.7/conan/tools/gnu/pkgconfigdeps.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import textwrap
 from collections import namedtuple
 
 from jinja2 import Template, StrictUndefined
 
 from conan.internal import check_duplicated_generator
 from conan.tools.gnu.gnudeps_flags import GnuDepsFlags
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.model.dependencies import get_transitive_requires
 from conans.util.files import save
 
 
 def _get_name_with_namespace(namespace, name):
     """
     Build a name with a namespace, e.g., openssl-crypto
@@ -93,48 +93,51 @@
 
 
 class _PCContentGenerator:
 
     template = textwrap.dedent("""\
         {%- macro get_libs(libdirs, cpp_info, gnudeps_flags) -%}
         {%- for _ in libdirs -%}
-        {{ '-L"${libdir%s}"' % loop.index + " " }}
+        {{ '-L"${libdir%s}"' % (loop.index0 or "") + " " }}
         {%- endfor -%}
         {%- for sys_lib in (cpp_info.libs + cpp_info.system_libs) -%}
         {{ "-l%s" % sys_lib + " " }}
         {%- endfor -%}
         {%- for shared_flag in (cpp_info.sharedlinkflags + cpp_info.exelinkflags) -%}
         {{  shared_flag + " " }}
         {%- endfor -%}
         {%- for framework in (gnudeps_flags.frameworks + gnudeps_flags.framework_paths) -%}
         {{ framework + " " }}
         {%- endfor -%}
         {%- endmacro -%}
 
         {%- macro get_cflags(includedirs, cxxflags, cflags, defines) -%}
         {%- for _ in includedirs -%}
-        {{ '-I"${includedir%s}"' % loop.index + " " }}
+        {{ '-I"${includedir%s}"' % (loop.index0 or "") + " " }}
         {%- endfor -%}
         {%- for cxxflag in cxxflags -%}
         {{ cxxflag + " " }}
         {%- endfor -%}
         {%- for cflag in cflags-%}
         {{ cflag + " " }}
         {%- endfor -%}
         {%- for define in defines-%}
         {{  "-D%s" % define + " " }}
         {%- endfor -%}
         {%- endmacro -%}
 
         prefix={{ prefix_path }}
         {% for path in libdirs %}
-        {{ "libdir{}={}".format(loop.index, path) }}
+        {{ "libdir{}={}".format((loop.index0 or ""), path) }}
         {% endfor %}
         {% for path in includedirs %}
-        {{ "includedir%d=%s" % (loop.index, path) }}
+        {{ "includedir%s=%s" % ((loop.index0 or ""), path) }}
+        {% endfor %}
+        {% for path in bindirs %}
+        {{ "bindir{}={}".format((loop.index0 or ""), path) }}
         {% endfor %}
         {% if pkg_config_custom_content %}
         # Custom PC content
         {{ pkg_config_custom_content }}
         {% endif %}
 
         Name: {{ name }}
@@ -144,43 +147,53 @@
         Cflags: {{ get_cflags(includedirs, cxxflags, cflags, defines) }}
         {% if requires|length %}
         Requires: {{ requires|join(' ') }}
         {% endif %}
     """)
 
     shortened_template = textwrap.dedent("""\
+        prefix={{ prefix_path }}
+        {% if pkg_config_custom_content %}
+        # Custom PC content
+        {{ pkg_config_custom_content }}
+        {% endif %}
+
         Name: {{ name }}
         Description: {{ description }}
         Version: {{ version }}
         {% if requires|length %}
         Requires: {{ requires|join(' ') }}
         {% endif %}
     """)
 
     def __init__(self, conanfile, dep):
         self._conanfile = conanfile
         self._dep = dep
 
-    def content(self, info):
-        assert isinstance(info, _PCInfo) and info.cpp_info is not None
-
+    def _get_prefix_path(self):
         # If editable, package_folder can be None
         root_folder = self._dep.recipe_folder if self._dep.package_folder is None \
             else self._dep.package_folder
-        version = info.cpp_info.get_property("component_version") or self._dep.ref.version
+        return root_folder.replace("\\", "/")
+
+    def content(self, info):
+        assert isinstance(info, _PCInfo) and info.cpp_info is not None
 
-        prefix_path = root_folder.replace("\\", "/")
+        prefix_path = self._get_prefix_path()
+        version = info.cpp_info.get_property("component_version") or self._dep.ref.version
         libdirs = _get_formatted_dirs(info.cpp_info.libdirs, prefix_path)
         includedirs = _get_formatted_dirs(info.cpp_info.includedirs, prefix_path)
+        bindirs = _get_formatted_dirs(info.cpp_info.bindirs, prefix_path)
         custom_content = info.cpp_info.get_property("pkg_config_custom_content")
 
         context = {
             "prefix_path": prefix_path,
             "libdirs": libdirs,
             "includedirs": includedirs,
+            "bindirs": bindirs,
             "pkg_config_custom_content": custom_content,
             "name": info.name,
             "description": info.description,
             "version": version,
             "requires": info.requires,
             "cpp_info": info.cpp_info,
             "cxxflags": [var.replace('"', '\\"') for var in info.cpp_info.cxxflags],
@@ -190,16 +203,19 @@
         }
         template = Template(self.template, trim_blocks=True, lstrip_blocks=True,
                             undefined=StrictUndefined)
         return template.render(context)
 
     def shortened_content(self, info):
         assert isinstance(info, _PCInfo)
-
+        custom_content = info.cpp_info.get_property("pkg_config_custom_content") if info.cpp_info \
+            else None
         context = {
+            "prefix_path": self._get_prefix_path(),
+            "pkg_config_custom_content": custom_content,
             "name": info.name,
             "description": info.description,
             "version": self._dep.ref.version,
             "requires": info.requires
         }
         template = Template(self.shortened_template, trim_blocks=True,
                             lstrip_blocks=True, undefined=StrictUndefined)
@@ -304,15 +320,15 @@
 
     @property
     def pc_files(self):
         """
         Get all the PC files and contents for any dependency:
 
         * If the given dependency does not have components:
-            The PC file will be the depency one.
+            The PC file will be the dependency one.
 
         * If the given dependency has components:
             The PC files will be saved in this order:
                 1- Package components.
                 2- Root component.
 
             Note: If the root-package PC name matches with any other of the components one, the first one
@@ -342,16 +358,16 @@
             pkg_requires.append(component_info.name)
 
         # Second, let's load the root package's PC file ONLY
         # if it does not already exist in components one
         # Issue related: https://github.com/conan-io/conan/issues/10341
         pkg_name = _get_package_name(self._dep, self._build_context_suffix)
         if f"{pkg_name}.pc" not in pc_files:
-            package_info = _PCInfo(pkg_name, pkg_requires, f"Conan package: {pkg_name}", None,
-                                   _get_package_aliases(self._dep))
+            package_info = _PCInfo(pkg_name, pkg_requires, f"Conan package: {pkg_name}",
+                                   self._dep.cpp_info, _get_package_aliases(self._dep))
             # It'll be enough creating a shortened PC file. This file will be like an alias
             pc_files[f"{package_info.name}.pc"] = self._content_generator.shortened_content(package_info)
             for alias in package_info.aliases:
                 alias_info = _PCInfo(alias, [package_info.name],
                                      f"Alias {alias} for {package_info.name}", None, [])
                 pc_files[f"{alias}.pc"] = self._content_generator.shortened_content(alias_info)
```

### Comparing `conan-server-2.0.6/conan/tools/google/bazel.py` & `conan-server-2.0.7/conan/tools/google/bazel.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/google/bazeldeps.py` & `conan-server-2.0.7/conan/tools/google/bazeldeps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import platform
 import textwrap
 
 from jinja2 import Template
 
 from conan.internal import check_duplicated_generator
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.util.files import save
 
 
 class BazelDeps(object):
     def __init__(self, conanfile):
         self._conanfile = conanfile
```

### Comparing `conan-server-2.0.6/conan/tools/google/layout.py` & `conan-server-2.0.7/conan/tools/google/layout.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/google/toolchain.py` & `conan-server-2.0.7/conan/tools/google/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/intel/intel_cc.py` & `conan-server-2.0.7/conan/tools/intel/intel_cc.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         - Compiler: https://software.intel.com/content/www/us/en/develop/documentation/oneapi-dpcpp-cpp-compiler-dev-guide-and-reference/top.html
 """
 import os
 import platform
 import textwrap
 
 from conan.internal import check_duplicated_generator
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 
 def _is_using_intel_oneapi(compiler_version):
     """Check if the Intel compiler to be used belongs to Intel oneAPI
 
     Note: Intel oneAPI Toolkit first version is 2021.1
     """
```

### Comparing `conan-server-2.0.6/conan/tools/layout/__init__.py` & `conan-server-2.0.7/conan/tools/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/meson/helpers.py` & `conan-server-2.0.7/conan/tools/meson/helpers.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/meson/toolchain.py` & `conan-server-2.0.7/conan/tools/meson/toolchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from conan.tools.apple.apple import to_apple_arch, is_apple_os, apple_min_version_flag, \
     apple_sdk_path
 from conan.tools.build.cross_building import cross_building
 from conan.tools.build.flags import libcxx_flags
 from conan.tools.env import VirtualBuildEnv
 from conan.tools.meson.helpers import *
 from conan.tools.microsoft import VCVars, msvc_runtime_flag
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.util.files import save
 
 
 class MesonToolchain(object):
     """
     MesonToolchain generator
     """
@@ -167,23 +167,23 @@
                 os_target = settings_target.get_safe("os")
                 arch_target = settings_target.get_safe("arch")
                 self.cross_build["target"] = to_meson_machine(os_target, arch_target)
             if is_apple_os(self._conanfile):  # default cross-compiler in Apple is common
                 default_comp = "clang"
                 default_comp_cpp = "clang++"
         else:
-            if "Visual" in compiler or compiler == "msvc":
-                default_comp = "cl"
-                default_comp_cpp = "cl"
-            elif "clang" in compiler:
+            if "clang" in compiler:
                 default_comp = "clang"
                 default_comp_cpp = "clang++"
             elif compiler == "gcc":
                 default_comp = "gcc"
                 default_comp_cpp = "g++"
+        if "Visual" in compiler or compiler == "msvc":
+            default_comp = "cl"
+            default_comp_cpp = "cl"
 
         # Read configuration for compilers
         compilers_by_conf = self._conanfile.conf.get("tools.build:compiler_executables", default={},
                                                      check_type=dict)
         # Read the VirtualBuildEnv to update the variables
         # FIXME: This VirtualBuildEnv instance is breaking things!!
         # FIXME: It shouldn't be used here, not intended for this use case
```

### Comparing `conan-server-2.0.6/conan/tools/microsoft/__init__.py` & `conan-server-2.0.7/conan/tools/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/microsoft/layout.py` & `conan-server-2.0.7/conan/tools/microsoft/layout.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from conan.tools.microsoft.msbuild import msbuild_arch
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 
 def vs_layout(conanfile):
     """
     Initialize a layout for a typical Visual Studio project.
 
     :param conanfile: ``< ConanFile object >`` The current recipe object. Always use ``self``.
```

### Comparing `conan-server-2.0.6/conan/tools/microsoft/msbuild.py` & `conan-server-2.0.7/conan/tools/microsoft/msbuild.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 
 def msbuild_verbosity_cmd_line_arg(conanfile):
-    verbosity = conanfile.conf.get("tools.build:verbosity")
-    if verbosity:
-        if verbosity not in ("quiet", "error", "warning", "notice", "status", "verbose",
-                             "normal", "debug", "v", "trace", "vv"):
-            raise ConanException(f"Unknown value '{verbosity}' for 'tools.build:verbosity'")
-        else:
-            # "Quiet", "Minimal", "Normal", "Detailed", "Diagnostic"
-            verbosity = {
-                "quiet": "Quiet",
-                "error": "Minimal",
-                "warning": "Minimal",
-                "notice": "Minimal",
-                "status": "Normal",
-                "verbose": "Normal",
-                "normal": "Normal",
-                "debug": "Detailed",
-                "v": "Detailed",
-                "trace": "Diagnostic",
-                "vv": "Diagnostic"
-            }.get(verbosity)
-            return '/verbosity:{}'.format(verbosity)
+    """
+    Controls msbuild verbosity.
+    See https://learn.microsoft.com/en-us/visualstudio/msbuild/msbuild-command-line-reference
+    :return:
+    """
+    verbosity = conanfile.conf.get("tools.build:verbosity", choices=("quiet", "verbose"))
+    if verbosity is not None:
+        verbosity = {
+            "quiet": "Quiet",
+            "verbose": "Detailed",
+        }.get(verbosity)
+        return f'/verbosity:{verbosity}'
+    return ""
 
 
 def msbuild_arch(arch):
     return {'x86': 'x86',
             'x86_64': 'x64',
             'armv7': 'ARM',
             'armv8': 'ARM64'}.get(str(arch))
```

### Comparing `conan-server-2.0.6/conan/tools/microsoft/msbuilddeps.py` & `conan-server-2.0.7/conan/tools/microsoft/msbuilddeps.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import textwrap
 from xml.dom import minidom
 
 from jinja2 import Template
 
 from conan.internal import check_duplicated_generator
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.model.dependencies import get_transitive_requires
 from conans.util.files import load, save
 
 VALID_LIB_EXTENSIONS = (".so", ".lib", ".a", ".dylib", ".bc")
 
 
 class MSBuildDeps(object):
@@ -315,29 +315,27 @@
         conf_name = self._config_filename()
         condition = self._condition()
         dep_name = self._dep_name(dep, build)
         result = {}
         if dep.cpp_info.has_components:
             pkg_aggregated_content = None
             for comp_name, comp_info in dep.cpp_info.components.items():
-                if comp_name is None:
-                    continue
                 full_comp_name = "{}_{}".format(dep_name, self._get_valid_xml_format(comp_name))
                 vars_filename = "conan_%s_vars%s.props" % (full_comp_name, conf_name)
                 activate_filename = "conan_%s%s.props" % (full_comp_name, conf_name)
                 comp_filename = "conan_%s.props" % full_comp_name
                 pkg_filename = "conan_%s.props" % dep_name
 
                 public_deps = []  # To store the xml dependencies/file names
-                for r in comp_info.requires:
-                    if "::" in r:  # Points to a component of a different package
-                        pkg, cmp_name = r.split("::")
-                        public_deps.append(pkg if pkg == cmp_name else "{}_{}".format(pkg, cmp_name))
+                for required_pkg, required_comp in comp_info.parsed_requires():
+                    if required_pkg is not None:  # Points to a component of a different package
+                        public_deps.append(required_pkg if required_pkg == required_comp
+                                           else "{}_{}".format(required_pkg, required_comp))
                     else:  # Points to a component of same package
-                        public_deps.append("{}_{}".format(dep_name, r))
+                        public_deps.append("{}_{}".format(dep_name, required_comp))
                 public_deps = [self._get_valid_xml_format(d) for d in public_deps]
                 result[vars_filename] = self._vars_props_file(require, dep, full_comp_name,
                                                               comp_info, build=build)
                 result[activate_filename] = self._activate_props_file(full_comp_name, vars_filename,
                                                                       public_deps, build=build)
                 result[comp_filename] = self._dep_props_file(full_comp_name, comp_filename,
                                                              activate_filename, condition)
```

### Comparing `conan-server-2.0.6/conan/tools/microsoft/nmakedeps.py` & `conan-server-2.0.7/conan/tools/microsoft/nmakedeps.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 
 from conan.internal import check_duplicated_generator
+from conan.tools import CppInfo
 from conan.tools.env import Environment
-from conans.model.build_info import CppInfo
 
 
 class NMakeDeps(object):
 
     def __init__(self, conanfile):
         """
         :param conanfile: ``< ConanFile object >`` The current recipe object. Always use ``self``.
         """
         self._conanfile = conanfile
         self._environment = None
 
     # TODO: This is similar from AutotoolsDeps: Refactor and make common
     def _get_cpp_info(self):
-        ret = CppInfo()
+        ret = CppInfo(self._conanfile)
         deps = self._conanfile.dependencies.host.topological_sort
         deps = [dep for dep in reversed(deps.values())]
         for dep in deps:
             dep_cppinfo = dep.cpp_info.aggregated_components()
             # In case we have components, aggregate them, we do not support isolated
             # "targets" with autotools
             ret.merge(dep_cppinfo)
```

### Comparing `conan-server-2.0.6/conan/tools/microsoft/nmaketoolchain.py` & `conan-server-2.0.7/conan/tools/microsoft/nmaketoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/microsoft/subsystems.py` & `conan-server-2.0.7/conan/tools/microsoft/subsystems.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 
 def unix_path(conanfile, path, scope="build"):
     subsystem = deduce_subsystem(conanfile, scope=scope)
     return subsystem_path(subsystem, path)
 
 
 def unix_path_package_info_legacy(conanfile, path, path_flavor=None):
-    message = f"The use of 'unix_path_legacy_compat' is deprecated in Conan 2.0 and does not " \
-              f"perform path conversions. This is retained for compatibility with Conan 1.x " \
-              f"and will be removed in a future version."
+    message = "The use of 'unix_path_legacy_compat' is deprecated in Conan 2.0 and does not " \
+              "perform path conversions. This is retained for compatibility with Conan 1.x " \
+              "and will be removed in a future version."
     conanfile.output.warning(message)
     return path
```

### Comparing `conan-server-2.0.6/conan/tools/microsoft/toolchain.py` & `conan-server-2.0.7/conan/tools/microsoft/toolchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from jinja2 import Template
 
 from conan.internal import check_duplicated_generator
 from conan.tools.build import build_jobs
 from conan.tools.intel.intel_cc import IntelCC
 from conan.tools.microsoft.visual import VCVars, msvs_toolset
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.util.files import save, load
 
 
 class MSBuildToolchain(object):
     """
     MSBuildToolchain class generator
     """
```

### Comparing `conan-server-2.0.6/conan/tools/microsoft/visual.py` & `conan-server-2.0.7/conan/tools/microsoft/visual.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import textwrap
 
 from conan.internal import check_duplicated_generator
 from conans.client.conf.detect_vs import vs_installation_path
-from conans.errors import ConanException, ConanInvalidConfiguration
+from conan.errors import ConanException, ConanInvalidConfiguration
 from conan.tools.scm import Version
 from conan.tools.intel.intel_cc import IntelCC
 
 CONAN_VCVARS_FILE = "conanvcvars.bat"
 
 
 def check_min_vs(conanfile, version, raise_invalid=True):
```

### Comparing `conan-server-2.0.6/conan/tools/premake/premake.py` & `conan-server-2.0.7/conan/tools/premake/premake.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/premake/premakedeps.py` & `conan-server-2.0.7/conan/tools/premake/premakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conan/tools/qbs/qbs.py` & `conan-server-2.0.7/conan/tools/qbs/qbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from conan.tools.build import build_jobs
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 
 def _configuration_dict_to_commandlist(name, config_dict):
     command_list = ['config:%s' % name]
     for key, value in config_dict.items():
         if type(value) is bool:
             if value:
```

### Comparing `conan-server-2.0.6/conan/tools/qbs/qbsprofile.py` & `conan-server-2.0.7/conan/tools/qbs/qbsprofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import platform
 import textwrap
 
 from io import StringIO
 from jinja2 import Template
 
 from conan.internal import check_duplicated_generator
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.util.files import save
 
 _profile_name = 'conan'
 _profiles_prefix_in_config = 'profiles.%s' % _profile_name
 
 _architecture = {
     'x86': 'x86',
```

### Comparing `conan-server-2.0.6/conan/tools/scm/git.py` & `conan-server-2.0.7/conan/tools/scm/git.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from conan.tools.files import chdir
-from conans.errors import ConanException
+from conan.errors import ConanException
 from conans.util.files import mkdir
 from conans.util.runners import check_output_runner
 
 
 class Git(object):
     """
     Git is a wrapper for several common patterns used with *git* tool.
@@ -158,28 +158,29 @@
         :param args: Extra arguments to pass to the git clone as a list.
         """
         args = args or []
         if os.path.exists(url):
             url = url.replace("\\", "/")  # Windows local directory
         mkdir(self.folder)
         self._conanfile.output.info("Cloning git repo")
-        self.run('clone "{}" {} {}'.format(url, " ".join(args), target))
+        target_path = f'"{target}"' if target else ""  # quote in case there are spaces in path
+        self.run('clone "{}" {} {}'.format(url, " ".join(args), target_path))
 
     def fetch_commit(self, url, commit):
         """
         Experimental: does a 1 commit fetch and checkout, instead of a full clone,
         should be faster.
         """
         if os.path.exists(url):
             url = url.replace("\\", "/")  # Windows local directory
         self._conanfile.output.info("Shallow fetch of git repo")
         self.run('init')
         self.run(f'remote add origin "{url}"')
         self.run(f'fetch --depth 1 origin {commit}')
-        self.run(f'checkout FETCH_HEAD')
+        self.run('checkout FETCH_HEAD')
 
     def checkout(self, commit):
         """
         Checkouts the given commit using ``git checkout <commit>``.
 
         :param commit: Commit to checkout.
         """
```

### Comparing `conan-server-2.0.6/conan/tools/system/package_manager.py` & `conan-server-2.0.7/conan/tools/system/package_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import platform
 
 from conan.tools.build import cross_building
 from conans.client.graph.graph import CONTEXT_BUILD
-from conans.errors import ConanException
+from conan.errors import ConanException
 
 
 class _SystemPackageManagerTool(object):
     mode_check = "check"  # Check if installed, fail if not
     mode_install = "install"
     mode_report = "report"  # Only report what would be installed, no check (can run in any system)
     mode_report_installed = "report-installed"  # report installed and missing packages
```

### Comparing `conan-server-2.0.6/conan_server.egg-info/PKG-INFO` & `conan-server-2.0.7/conan_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan-server
-Version: 2.0.6
+Version: 2.0.7
 Summary: Conan Server of Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Description: <picture>
           <!-- These are also used for https://github.com/conan-io/.github/blob/main/profile/README.md -->
@@ -30,16 +30,16 @@
         - Portable. Works across all platforms, including Linux, OSX, Windows (with native and first-class support, WSL, MinGW),
           Solaris, FreeBSD, embedded and cross-compiling, docker, WSL
         - Manage binaries. It can create, upload and download binaries for any configuration and platform,
           even cross-compiling, saving lots of time in development and continuous integration. The binary compatibility can be configured
           and customized. Manage all your artifacts in the same way on all platforms.
         - Integrates with any build system, including any proprietary and custom one. Provides tested support for major build systems
           (CMake, MSBuild, Makefiles, Meson, etc).
-        - Extensible: Its python based recipes, together with extensions points allows for great power and flexibility.
-        - Large and active community, especially in Github (https://github.com/conan-io/conan) and Slack (https://cpplang-inviter.cppalliance.org/ #conan channel).
+        - Extensible: Its Python-based recipes, together with extension points allow for great power and flexibility.
+        - Large and active community, especially in GitHub (https://github.com/conan-io/conan) and Slack (https://cpplang-inviter.cppalliance.org/ #conan channel).
           This community also creates and maintains packages in ConanCenter and Bincrafters repositories in Bintray.
         - Stable. Used in production by many companies, since 1.0 there is a commitment not to break package recipes and documented behavior.
         
         
         This is the **developer/maintainer** documentation. For user documentation, go to https://docs.conan.io
         
         
@@ -86,42 +86,42 @@
         ## Contributing to the project
         
         
         Feedback and contribution are always welcome in this project.
         Please read our [contributing guide](https://github.com/conan-io/conan/blob/develop/.github/CONTRIBUTING.md).
         Also, if you plan to contribute, please add some testing for your changes. You can read the [Conan
         tests guidelines section](https://github.com/conan-io/conan/blob/develop/conans/test/README.md) for
-        some advise on how to write tests for Conan.
+        some advice on how to write tests for Conan.
         
         ### Running the tests
         
         
-        **Install python requirements**
+        **Install Python requirements**
         
         ```bash
         $ python -m pip install -r conans/requirements_server.txt
         $ python -m pip install -r conans/requirements_dev.txt
         ```
         
-        If you are not Windows and you are not using a python virtual environment, you will need to run these
+        If you are not on Windows and you are not using a Python virtual environment, you will need to run these
         commands using `sudo`.
         
         Before you can run the tests, you need to set a few environment variables first.
         
         ```bash
         $ export PYTHONPATH=$PYTHONPATH:$(pwd)
         ```
         
         On Windows it would be (while being in the Conan root directory):
         
         ```bash
         $ set PYTHONPATH=.
         ```
         
-        Conan test suite defines and configure some required tools (CMake, Ninja, etc) in the
+        Conan test suite defines and configures some required tools (CMake, Ninja, etc) in the
         ``conftest.py`` and allows to define a custom ``conftest_user.py``.
         Some specific versions, like cmake>=3.15 are necessary.
         
         
         You can run the tests like this:
         
         ```bash
@@ -140,15 +140,15 @@
         
         To run specific tests, you can specify the test name too, something like:
         
         ```bash
         $ python -m pytest conans/test/unittests/client/cmd/export_test.py::ExportTest::test_export_warning -s
         ```
         
-        The `-s` argument can be useful to see some output that otherwise is captured by pytest.
+        The `-s` argument can be useful to see some output that otherwise is captured by *pytest*.
         
         Also, you can run tests against an instance of Artifactory. Those tests should add the attribute
         `artifactory_ready`.
         
         ```bash
         $ python -m pytest . -m artifactory_ready
         ```
@@ -160,15 +160,15 @@
         ```bash
         $ export CONAN_TEST_WITH_ARTIFACTORY=1
         $ export ARTIFACTORY_DEFAULT_URL=http://localhost:8081/artifactory
         $ export ARTIFACTORY_DEFAULT_USER=admin
         $ export ARTIFACTORY_DEFAULT_PASSWORD=password
         ```
         
-        `ARTIFACTORY_DEFAULT_URL` is the base url for the Artifactory repo, not one for a specific
+        `ARTIFACTORY_DEFAULT_URL` is the base URL for the Artifactory repo, not one for a specific
         repository. Running the tests with a real Artifactory instance will create repos on the fly so please
         use a separate server for testing purposes.
         
         ## License
         
         [MIT LICENSE](LICENSE.md)
```

### Comparing `conan-server-2.0.6/conan_server.egg-info/SOURCES.txt` & `conan-server-2.0.7/conan_server.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 conan/cli/commands/profile.py
 conan/cli/commands/remote.py
 conan/cli/commands/remove.py
 conan/cli/commands/search.py
 conan/cli/commands/source.py
 conan/cli/commands/test.py
 conan/cli/commands/upload.py
+conan/cli/commands/version.py
 conan/cli/formatters/__init__.py
 conan/cli/formatters/graph/__init__.py
 conan/cli/formatters/graph/graph.py
 conan/cli/formatters/graph/graph_info_text.py
 conan/cli/formatters/graph/info_graph_dot.py
 conan/cli/formatters/graph/info_graph_html.py
 conan/cli/formatters/list/__init__.py
@@ -64,14 +65,15 @@
 conan/cli/formatters/list/search_table_html.py
 conan/cli/printers/__init__.py
 conan/cli/printers/graph.py
 conan/internal/__init__.py
 conan/internal/conan_app.py
 conan/internal/deploy.py
 conan/internal/integrity_check.py
+conan/internal/upload_metadata.py
 conan/internal/api/__init__.py
 conan/internal/api/new/__init__.py
 conan/internal/api/new/alias_new.py
 conan/internal/api/new/autoools_exe.py
 conan/internal/api/new/autotools_lib.py
 conan/internal/api/new/basic.py
 conan/internal/api/new/bazel_exe.py
@@ -102,15 +104,14 @@
 conan/tools/build/cppstd.py
 conan/tools/build/cpu.py
 conan/tools/build/cross_building.py
 conan/tools/build/flags.py
 conan/tools/build/stdcpp_library.py
 conan/tools/cmake/__init__.py
 conan/tools/cmake/cmake.py
-conan/tools/cmake/file_api.py
 conan/tools/cmake/layout.py
 conan/tools/cmake/presets.py
 conan/tools/cmake/utils.py
 conan/tools/cmake/cmakedeps/__init__.py
 conan/tools/cmake/cmakedeps/cmakedeps.py
 conan/tools/cmake/cmakedeps/templates/__init__.py
 conan/tools/cmake/cmakedeps/templates/config.py
@@ -125,15 +126,14 @@
 conan/tools/env/__init__.py
 conan/tools/env/environment.py
 conan/tools/env/virtualbuildenv.py
 conan/tools/env/virtualrunenv.py
 conan/tools/files/__init__.py
 conan/tools/files/conandata.py
 conan/tools/files/copy_pattern.py
-conan/tools/files/cpp_package.py
 conan/tools/files/files.py
 conan/tools/files/packager.py
 conan/tools/files/patches.py
 conan/tools/files/symlinks/__init__.py
 conan/tools/files/symlinks/symlinks.py
 conan/tools/gnu/__init__.py
 conan/tools/gnu/autotools.py
```

### Comparing `conan-server-2.0.6/conan_server.egg-info/requires.txt` & `conan-server-2.0.7/conan_server.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 requests<3.0.0,>=2.25
 urllib3<1.27,>=1.26.6
 colorama<0.5.0,>=0.4.3
-PyYAML<=6.0,>=5.1
+PyYAML<7.0,>=6.0
 patch-ng<1.18,>=1.17.4
 fasteners>=0.15
 Jinja2<4.0.0,>=3.0
 python-dateutil<3,>=2.8.0
 bottle<0.13,>=0.12.8
 pluginbase>=0.5
 PyJWT<3.0.0,>=2.4.0
```

### Comparing `conan-server-2.0.6/conans/client/cache/cache.py` & `conan-server-2.0.7/conans/client/cache/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,29 @@
 
     def create_build_pkg_layout(self, ref):
         return self._data_cache.create_build_pkg_layout(ref)
 
     def assign_prev(self, layout: PackageLayout):
         return self._data_cache.assign_prev(layout)
 
-    def ref_layout(self, ref: RecipeReference):
-        return self._data_cache.get_reference_layout(ref)
+    # Recipe methods
+    def recipe_layout(self, ref: RecipeReference):
+        return self._data_cache.get_recipe_layout(ref)
+
+    ref_layout = recipe_layout
+
+    def get_latest_recipe_reference(self, ref):
+        # TODO: We keep this for testing only, to be removed
+        assert ref.revision is None
+        return self._data_cache.get_recipe_layout(ref).reference
+
+    def get_recipe_revisions_references(self, ref):
+        # For listing multiple revisions only
+        assert ref.revision is None
+        return self._data_cache.get_recipe_revisions_references(ref)
 
     def pkg_layout(self, ref: PkgReference):
         return self._data_cache.get_package_layout(ref)
 
     def get_or_create_ref_layout(self, ref: RecipeReference):
         return self._data_cache.get_or_create_ref_layout(ref)
 
@@ -88,32 +101,22 @@
 
     def remove_recipe_layout(self, layout):
         self._data_cache.remove_recipe(layout)
 
     def remove_package_layout(self, layout):
         self._data_cache.remove_package(layout)
 
-    def get_recipe_timestamp(self, ref):
-        return self._data_cache.get_recipe_timestamp(ref)
-
-    def get_package_timestamp(self, ref):
-        return self._data_cache.get_package_timestamp(ref)
-
     def update_recipe_timestamp(self, ref):
         """ when the recipe already exists in cache, but we get a new timestamp from a server
         that would affect its order in our cache """
         return self._data_cache.update_recipe_timestamp(ref)
 
     def all_refs(self):
         return self._data_cache.list_references()
 
-    def exists_rrev(self, ref):
-        # Used just by inspect to check before calling get_recipe()
-        return self._data_cache.exists_rrev(ref)
-
     def exists_prev(self, pref):
         # Used just by download to skip downloads if prev already exists in cache
         return self._data_cache.exists_prev(pref)
 
     def get_package_revisions_references(self, pref: PkgReference, only_latest_prev=False):
         return self._data_cache.get_package_revisions_references(pref, only_latest_prev)
 
@@ -121,20 +124,14 @@
                                only_latest_prev=True) -> List[PkgReference]:
         """Get the latest package references"""
         return self._data_cache.get_package_references(ref, only_latest_prev)
 
     def get_matching_build_id(self, ref, build_id):
         return self._data_cache.get_matching_build_id(ref, build_id)
 
-    def get_recipe_revisions_references(self, ref, only_latest_rrev=False):
-        return self._data_cache.get_recipe_revisions_references(ref, only_latest_rrev)
-
-    def get_latest_recipe_reference(self, ref):
-        return self._data_cache.get_latest_recipe_reference(ref)
-
     def get_latest_package_reference(self, pref):
         return self._data_cache.get_latest_package_reference(pref)
 
     @property
     def store(self):
         return self._store_folder
```

### Comparing `conan-server-2.0.6/conans/client/cache/editable.py` & `conan-server-2.0.7/conans/client/cache/editable.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/cache/remote_registry.py` & `conan-server-2.0.7/conans/client/cache/remote_registry.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/cmd/export.py` & `conan-server-2.0.7/conans/client/cmd/export.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/cmd/uploader.py` & `conan-server-2.0.7/conans/client/cmd/uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,17 +154,16 @@
         add_tgz(EXPORT_TGZ_NAME, files, "Compressing recipe...")
         add_tgz(EXPORT_SOURCES_TGZ_NAME, src_files, "Compressing recipe sources...")
         return result
 
     def _prepare_package(self, pref, prev_bundle):
         pkg_layout = self._app.cache.pkg_layout(pref)
         if pkg_layout.package_is_dirty():
-            raise ConanException("Package %s is corrupted, aborting upload.\n"
-                                 "Remove it with 'conan remove %s -p=%s'"
-                                 % (pref, pref.ref, pref.package_id))
+            raise ConanException(f"Package {pref} is corrupted, aborting upload.\n"
+                                 f"Remove it with 'conan remove {pref}'")
         cache_files = self._compress_package_files(pkg_layout, pref)
         prev_bundle["files"] = cache_files
 
     def _compress_package_files(self, layout, pref):
         download_pkg_folder = layout.download_package()
         package_tgz = os.path.join(download_pkg_folder, PACKAGE_TGZ_NAME)
         if is_dirty(package_tgz):
```

### Comparing `conan-server-2.0.6/conans/client/cmd/user.py` & `conan-server-2.0.7/conans/client/cmd/user.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/conanfile/build.py` & `conan-server-2.0.7/conans/client/conanfile/build.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/conanfile/configure.py` & `conan-server-2.0.7/conans/client/conanfile/configure.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/conanfile/package.py` & `conan-server-2.0.7/conans/client/conanfile/package.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/conf/__init__.py` & `conan-server-2.0.7/conans/client/conf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     Emscripten:
     Neutrino:
         version: ["6.4", "6.5", "6.6", "7.0", "7.1"]
     baremetal:
     VxWorks:
         version: ["7"]
 arch: [x86, x86_64, ppc32be, ppc32, ppc64le, ppc64,
-       armv4, armv4i, armv5el, armv5hf, armv6, armv7, armv7hf, armv7s, armv7k, armv8, armv8_32, armv8.3,
+       armv4, armv4i, armv5el, armv5hf, armv6, armv7, armv7hf, armv7s, armv7k, armv8, armv8_32, armv8.3, arm64ec,
        sparc, sparcv9,
        mips, mips64, avr, s390, s390x, asm.js, wasm, sh4le,
        e2k-v2, e2k-v3, e2k-v4, e2k-v5, e2k-v6, e2k-v7,
        xtensalx6, xtensalx106, xtensalx7]
 compiler:
     sun-cc:
         version: ["5.10", "5.11", "5.12", "5.13", "5.14", "5.15"]
```

### Comparing `conan-server-2.0.6/conans/client/conf/config_installer.py` & `conan-server-2.0.7/conans/client/conf/config_installer.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/conf/detect.py` & `conan-server-2.0.7/conans/client/conf/detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     gcc = _gcc_compiler()
     clang = _clang_compiler()
     if platform.system() == "SunOS":
         sun_cc = _sun_cc_compiler()
 
     if platform.system() == "Windows":
         return vs or cc or gcc or clang
-    elif platform.system() == "Darwin":
+    elif platform.system() in ["Darwin", "FreeBSD"]:
         return clang or cc or gcc
     elif platform.system() == "SunOS":
         return sun_cc or cc or gcc or clang
     else:
         return cc or gcc or clang
```

### Comparing `conan-server-2.0.6/conans/client/conf/detect_vs.py` & `conan-server-2.0.7/conans/client/conf/detect_vs.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/conf/required_version.py` & `conan-server-2.0.7/conans/client/conf/required_version.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/downloaders/caching_file_downloader.py` & `conan-server-2.0.7/conans/client/downloaders/caching_file_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                                    download_cache_folder, backups_urls)
 
     def _caching_download(self, urls, file_path,
                           retry, retry_wait, verify_ssl, auth, headers, md5, sha1, sha256,
                           download_cache_folder, backups_urls):
         """
         this download will first check in the local cache, if not there, it will go to the list
-        of backup_urls defined by user conf (by default ["origin"], and iterate it until
+        of backup_urls defined by user conf (by default ["origin"]), and iterate it until
         something is found.
         """
         # We are going to use the download_urls definition for backups
         download_cache_folder = download_cache_folder or self._cache.default_sources_backup_folder
         # regular local shared download cache, not using Conan backup sources servers
         backups_urls = backups_urls or ["origin"]
         if download_cache_folder and not os.path.isabs(download_cache_folder):
@@ -112,15 +112,15 @@
             self._file_downloader.download(backup_url + sha256 + ".json", cached_path + ".json")
             self._output.info(f"Sources for {urls} found in remote backup {backup_url}")
             return True
         except NotFoundException:
             if is_last:
                 raise NotFoundException(f"File {urls} not found in {backups_urls}")
             else:
-                self._output.warning(f"Sources not found in backup {backup_url}")
+                self._output.warning(f"File {urls} not found in {backup_url}")
         except (AuthenticationException, ForbiddenException) as e:
             raise ConanException(f"The source backup server '{backup_url}' "
                                  f"needs authentication: {e}. "
                                  f"Please provide 'source_credentials.json'")
 
     def _download_from_urls(self, urls, file_path, retry, retry_wait, verify_ssl, auth, headers,
                             md5, sha1, sha256):
```

### Comparing `conan-server-2.0.6/conans/client/downloaders/download_cache.py` & `conan-server-2.0.7/conans/client/downloaders/download_cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,39 +40,47 @@
             thread_lock = self._thread_locks.setdefault(lock, Lock())
             thread_lock.acquire()
             try:
                 yield
             finally:
                 thread_lock.release()
 
-    def get_backup_sources_files_to_upload(self, package_list):
+    def get_backup_sources_files_to_upload(self, package_list, excluded_urls):
         """ from a package_list of packages to upload, collect from the backup-sources cache
         the matching references to upload those backups too
         """
         def should_upload_sources(package):
             return any(prev["upload"] for prev in package["revisions"].values())
 
         files_to_upload = []
         path_backups = os.path.join(self._path, self._SOURCE_BACKUP)
 
         if not os.path.exists(path_backups):
             return []
 
+        if excluded_urls is None:
+            excluded_urls = []
+
         all_refs = {str(k) for k, ref in package_list.refs()
                     if ref.get("upload") or any(should_upload_sources(p)
                                                 for p in ref["packages"].values())}
         for f in os.listdir(path_backups):
             if f.endswith(".json"):
                 f = os.path.join(path_backups, f)
                 content = json.loads(load(f))
                 refs = content["references"]
                 # unknown entries are not uploaded at this moment, the flow is not expected.
-                if any(ref in all_refs for ref in refs):
-                    files_to_upload.append(f)
-                    files_to_upload.append(f[:-5])
+                for ref, urls in refs.items():
+                    is_excluded = all(any(url.startswith(excluded_url)
+                                          for excluded_url in excluded_urls)
+                                      for url in urls)
+                    if not is_excluded and ref in all_refs:
+                        files_to_upload.append(f)
+                        files_to_upload.append(f[:-5])
+                        break
         return files_to_upload
 
     @staticmethod
     def update_backup_sources_json(cached_path, conanfile, urls):
         """ create or update the sha256.json file with the references and new urls used
         """
         summary_path = cached_path + ".json"
```

### Comparing `conan-server-2.0.6/conans/client/downloaders/file_downloader.py` & `conan-server-2.0.7/conans/client/downloaders/file_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 
 
 from conan.api.output import ConanOutput
 from conans.client.rest import response_to_str
 from conans.errors import ConanException, NotFoundException, AuthenticationException, \
     ForbiddenException, ConanConnectionError, RequestErrorException
+from conans.util.files import human_size
 from conans.util.sha import check_with_algorithm_sum
 
 
 class FileDownloader:
 
     def __init__(self, requester, scope=None):
         self._output = ConanOutput(scope=scope)
@@ -98,28 +99,36 @@
                 return int(match.group(3))
             else:
                 total_size = response.headers.get('Content-Length') or len(response.content)
                 return int(total_size)
 
         try:
             total_length = get_total_length()
-            if total_length > 1000000:  # 10 Mb
-                from conan.tools.files.files import _human_size
-                hs = _human_size(total_length)
+            is_large_file = total_length > 10000000  # 10 MB
+            t_start = time.time()
+            base_name = os.path.basename(file_path)
+            if is_large_file:
+                hs = human_size(total_length)
                 action = "Downloading" if range_start == 0 else "Continuing download of"
-                description = f"{action} {hs} {os.path.basename(file_path)}"
-                self._output.info(description)
+                self._output.info(f"{action} {hs} {base_name}")
 
             chunk_size = 1024 * 100
             total_downloaded_size = range_start
             mode = "ab" if range_start else "wb"
             with open(file_path, mode) as file_handler:
                 for chunk in response.iter_content(chunk_size):
                     file_handler.write(chunk)
                     total_downloaded_size += len(chunk)
+                    if is_large_file:
+                        t = time.time()
+                        if t - t_start > 10:  # Every 10 seconds
+                            hs = human_size(total_downloaded_size)
+                            perc = int(total_downloaded_size*100/total_length)
+                            self._output.info(f"Downloaded {hs} {perc}% {base_name}")
+                            t_start = t
 
             gzip = (response.headers.get("content-encoding") == "gzip")
             response.close()
             # it seems that if gzip we don't know the size, cannot resume and shouldn't raise
             if total_downloaded_size != total_length and not gzip:
                 if (total_length > total_downloaded_size > range_start
                         and response.headers.get("Accept-Ranges") == "bytes"):
```

### Comparing `conan-server-2.0.6/conans/client/generators/__init__.py` & `conan-server-2.0.7/conans/client/generators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,13 +195,15 @@
         conanfile.output.info(f"Generated aggregated env files: {generated}")
 
 
 def relativize_generated_file(content, conanfile, placeholder):
     abs_base_path = conanfile.folders._base_generators
     if not abs_base_path or not os.path.isabs(abs_base_path):
         return content
+    abs_base_path = os.path.join(abs_base_path, "")  # For the trailing / to dissambiguate matches
     generators_folder = conanfile.generators_folder
     rel_path = os.path.relpath(abs_base_path, generators_folder)
     new_path = placeholder if rel_path == "." else os.path.join(placeholder, rel_path)
+    new_path = os.path.join(new_path, "")  # For the trailing / to dissambiguate matches
     content = content.replace(abs_base_path, new_path)
     content = content.replace(abs_base_path.replace("\\", "/"), new_path.replace("\\", "/"))
     return content
```

### Comparing `conan-server-2.0.6/conans/client/graph/build_mode.py` & `conan-server-2.0.7/conans/client/graph/build_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class BuildMode:
     """ build_mode => ["*"] if user wrote "--build"
                    => ["hello*", "bye*"] if user wrote "--build hello --build bye"
                    => ["hello/0.1@foo/bar"] if user wrote "--build hello/0.1@foo/bar"
                    => False if user wrote "never"
                    => True if user wrote "missing"
-                   => ["!foo"] means exclude when building all from sources
+                   => ["!foo"] or ["~foo"] means exclude when building all from sources
     """
     def __init__(self, params):
         self.missing = False
         self.never = False
         self.cascade = False
         self.editable = False
         self.patterns = []
@@ -44,15 +44,15 @@
                         clean_pattern = clean_pattern.replace("@#", "#")
                         self.build_missing_patterns.append(clean_pattern)
                     else:
                         # Remove the @ at the end, to match for
                         # "conan install --requires=pkg/0.1@ --build=pkg/0.1@"
                         clean_pattern = param[:-1] if param.endswith("@") else param
                         clean_pattern = clean_pattern.replace("@#", "#")
-                        if clean_pattern and clean_pattern[0] == "!":
+                        if clean_pattern and clean_pattern[0] in ["!", "~"]:
                             self._excluded_patterns.append(clean_pattern[1:])
                         else:
                             self.patterns.append(clean_pattern)
 
             if self.never and (self.missing or self.patterns or self.cascade):
                 raise ConanException("--build=never not compatible with other options")
         self._unused_patterns = list(self.patterns) + self._excluded_patterns
```

### Comparing `conan-server-2.0.6/conans/client/graph/compatibility.py` & `conan-server-2.0.7/conans/client/graph/compatibility.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/graph/compute_pid.py` & `conan-server-2.0.7/conans/client/graph/compute_pid.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/graph/graph.py` & `conan-server-2.0.7/conans/client/graph/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 RECIPE_NEWER = "Newer"  # The local recipe is  modified and newer timestamp than server
 RECIPE_NOT_IN_REMOTE = "Not in remote"
 RECIPE_UPDATEABLE = "Update available"  # The update of recipe is available (only in conan info)
 RECIPE_NO_REMOTE = "No remote"
 RECIPE_EDITABLE = "Editable"
 RECIPE_CONSUMER = "Consumer"  # A conanfile from the user
 RECIPE_VIRTUAL = "Cli"  # A virtual conanfile (dynamic in memory conanfile)
-RECIPE_MISSING = "Missing recipe"  # Impossible to find a recipe for this reference
 RECIPE_SYSTEM_TOOL = "System tool"
 
 BINARY_CACHE = "Cache"
 BINARY_DOWNLOAD = "Download"
 BINARY_UPDATE = "Update"
 BINARY_BUILD = "Build"
 BINARY_MISSING = "Missing"
@@ -210,14 +209,16 @@
     def serialize(self):
         result = OrderedDict()
         result["ref"] = self.ref.repr_notime() if self.ref is not None else "conanfile"
         result["id"] = getattr(self, "id")  # Must be assigned by graph.serialize()
         result["recipe"] = self.recipe
         result["package_id"] = self.package_id
         result["prev"] = self.prev
+        result["remote"] = self.remote.name if self.remote else None
+        result["binary_remote"] = self.binary_remote.name if self.binary_remote else None
         from conans.client.installer import build_id
         result["build_id"] = build_id(self.conanfile)
         result["binary"] = self.binary
         # TODO: This doesn't match the model, check it
         result["invalid_build"] = self.cant_build
         result["info_invalid"] = getattr(getattr(self.conanfile, "info", None), "invalid", None)
         # Adding the conanfile information: settings, options, etc
```

### Comparing `conan-server-2.0.6/conans/client/graph/graph_binaries.py` & `conan-server-2.0.7/conans/client/graph/graph_binaries.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/graph/graph_builder.py` & `conan-server-2.0.7/conans/client/graph/graph_builder.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/graph/graph_error.py` & `conan-server-2.0.7/conans/client/graph/graph_error.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,27 +11,38 @@
         self.node = node
         self.require = require
         self.prev_node = prev_node
         self.prev_require = prev_require
         self.base_previous = base_previous
 
     def __str__(self):
-        return f"Version conflict: {self.node.ref}->{self.require.ref}, "\
-               f"{self.base_previous.ref}->{self.prev_require.ref}."
+        if self.node.ref is not None and self.base_previous.ref is not None:
+            return f"Version conflict: {self.node.ref}->{self.require.ref}, " \
+                   f"{self.base_previous.ref}->{self.prev_require.ref}."
+        else:
+            conflicting_node = self.node.ref or self.base_previous.ref
+            conflicting_node_msg = ""
+            if conflicting_node is not None:
+                conflicting_node_msg = f"\nConflict originates from {conflicting_node}\n"
+            return f"Version conflict: " \
+                   f"Conflict between {self.require.ref} and {self.prev_require.ref} in the graph." \
+                   f"{conflicting_node_msg}" \
+                   f"\nRun conan graph info with your recipe and add --format=html " \
+                   f"to inspect the graph errors in an easier to visualize way."
 
 
 class GraphLoopError(GraphError):
 
     def __init__(self, node, require, ancestor):
         self.node = node
         self.require = require
         self.ancestor = ancestor
 
     def __str__(self):
-        return "There is a cycle/loop in the graph:\n"\
+        return "There is a cycle/loop in the graph:\n" \
                f"    Initial ancestor: {self.ancestor}\n" \
                f"    Require: {self.require.ref}\n" \
                f"    Dependency: {self.node}"
 
 
 class GraphMissingError(GraphError):
```

### Comparing `conan-server-2.0.6/conans/client/graph/install_graph.py` & `conan-server-2.0.7/conans/client/graph/install_graph.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/graph/profile_node_definer.py` & `conan-server-2.0.7/conans/client/graph/profile_node_definer.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/graph/provides.py` & `conan-server-2.0.7/conans/client/graph/provides.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/graph/proxy.py` & `conan-server-2.0.7/conans/client/graph/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,27 +29,27 @@
         output = ConanOutput(scope=str(reference))
 
         conanfile_path = self._cache.editable_packages.get_path(reference)
         if conanfile_path is not None:
             return conanfile_path, RECIPE_EDITABLE, None, reference
 
         # check if it there's any revision of this recipe in the local cache
-        ref = self._cache.get_latest_recipe_reference(reference)
-
-        # NOT in disk, must be retrieved from remotes
-        if not ref:
+        try:
+            recipe_layout = self._cache.recipe_layout(reference)
+            ref = recipe_layout.reference  # latest revision if it was not defined
+        except ConanException:
+            # NOT in disk, must be retrieved from remotes
             # we will only check all servers for latest revision if we did a --update
             remote, new_ref = self._download_recipe(reference, remotes, output, update, check_update)
             recipe_layout = self._cache.ref_layout(new_ref)
             status = RECIPE_DOWNLOADED
             conanfile_path = recipe_layout.conanfile()
             return conanfile_path, status, remote, new_ref
 
         # TODO: cache2.0: check with new --update flows
-        recipe_layout = self._cache.ref_layout(ref)
         conanfile_path = recipe_layout.conanfile()
 
         # TODO: If the revision is given, then we don't need to check for updates?
         if not (check_update or update):
             status = RECIPE_INCACHE
             return conanfile_path, status, None, ref
```

### Comparing `conan-server-2.0.6/conans/client/graph/python_requires.py` & `conan-server-2.0.7/conans/client/graph/python_requires.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/graph/range_resolver.py` & `conan-server-2.0.7/conans/client/graph/range_resolver.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/hook_manager.py` & `conan-server-2.0.7/conans/client/hook_manager.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/installer.py` & `conan-server-2.0.7/conans/client/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,38 +339,39 @@
         node = install_node.nodes[0]
         conanfile = node.conanfile
         ref = node.ref
         editable = self._cache.editable_packages.get(ref)
         conanfile_path = editable["path"]
         output_folder = editable.get("output_folder")
 
-        # TODO: Check, this assumes the folder is always the conanfile one
         base_path = os.path.dirname(conanfile_path)
+
         conanfile.folders.set_base_folders(base_path, output_folder)
         output = conanfile.output
         output.info("Rewriting files of editable package "
                     "'{}' at '{}'".format(conanfile.name, conanfile.generators_folder))
         write_generators(conanfile, self._app)
 
         if node.binary == BINARY_EDITABLE_BUILD:
             run_build_method(conanfile, self._hook_manager)
 
+        rooted_base_path = base_path if conanfile.folders.root is None else \
+            os.path.normpath(os.path.join(base_path, conanfile.folders.root))
+
         for node in install_node.nodes:
             # Get source of information
             conanfile = node.conanfile
             # New editables mechanism based on Folders
-            conanfile.folders.set_base_package(output_folder or base_path)
-            conanfile.folders.set_base_source(base_path)
-            conanfile.folders.set_base_build(output_folder or base_path)
-            conanfile.folders.set_base_generators(output_folder or base_path)
+            conanfile.folders.set_base_package(output_folder or rooted_base_path)
+            conanfile.folders.set_base_folders(base_path, output_folder)
             # Need a temporary package revision for package_revision_mode
             # Cannot be PREV_UNKNOWN otherwise the consumers can't compute their packageID
             node.prev = "editable"
             # TODO: Check this base_path usage for editable when not defined
-            self._call_package_info(conanfile, package_folder=base_path, is_editable=True)
+            self._call_package_info(conanfile, package_folder=rooted_base_path, is_editable=True)
 
     def _handle_node_build(self, package, pkg_layout):
         node = package.nodes[0]
         pref = node.pref
         assert pref.package_id, "Package-ID without value"
         assert pkg_layout, "The pkg_layout should be declared here"
         assert node.binary == BINARY_BUILD
```

### Comparing `conan-server-2.0.6/conans/client/loader.py` & `conan-server-2.0.7/conans/client/loader.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/loader_txt.py` & `conan-server-2.0.7/conans/client/loader_txt.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/migrations.py` & `conan-server-2.0.7/conans/client/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/pkg_sign.py` & `conan-server-2.0.7/conans/client/pkg_sign.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/profile_loader.py` & `conan-server-2.0.7/conans/client/profile_loader.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/remote_manager.py` & `conan-server-2.0.7/conans/client/remote_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 import shutil
 from typing import List
 
 from requests.exceptions import ConnectionError
 
 from conan.api.output import ConanOutput
 from conan.internal.cache.conan_reference_layout import METADATA
-from conan.tools.files.files import _human_size
 from conans.client.cache.remote_registry import Remote
 from conans.client.pkg_sign import PkgSignaturesPlugin
 from conans.errors import ConanConnectionError, ConanException, NotFoundException, \
     PackageNotFoundException
 from conans.model.info import load_binary_info
 from conans.model.package_ref import PkgReference
 from conans.model.recipe_ref import RecipeReference
-from conans.util.files import rmdir
+from conans.util.files import rmdir, human_size
 from conans.paths import EXPORT_SOURCES_TGZ_NAME, EXPORT_TGZ_NAME, PACKAGE_TGZ_NAME
 from conans.util.files import mkdir, tar_extract
 
 
 class RemoteManager(object):
     """ Will handle the remotes to get recipes, packages etc """
 
@@ -36,32 +35,32 @@
         self._call_remote(remote, "upload_recipe", ref, files_to_upload)
 
     def upload_package(self, pref, files_to_upload, remote):
         assert pref.ref.revision, "upload_package requires RREV"
         assert pref.revision, "upload_package requires PREV"
         self._call_remote(remote, "upload_package", pref, files_to_upload)
 
-    def get_recipe(self, ref, remote):
+    def get_recipe(self, ref, remote, metadata=None):
         """
         Read the conans from remotes
         Will iterate the remotes to find the conans unless remote was specified
 
         returns (dict relative_filepath:abs_path , remote_name)"""
 
         assert ref.revision, "get_recipe without revision specified"
 
         layout = self._cache.get_or_create_ref_layout(ref)
         layout.export_remove()
 
         download_export = layout.download_export()
         try:
-            zipped_files = self._call_remote(remote, "get_recipe", ref, download_export)
-            remote_refs = self._call_remote(remote, "get_recipe_revisions_references", ref)
-            ref_time = remote_refs[0].timestamp
-            ref.timestamp = ref_time
+            zipped_files = self._call_remote(remote, "get_recipe", ref, download_export, metadata,
+                                             only_metadata=False)
+            # The timestamp of the ``ref`` from the server has been already obtained by ConanProxy
+            # or it will be obtained explicitly by the ``conan download``
             # filter metadata files
             # This could be also optimized in download, avoiding downloading them, for performance
             zipped_files = {k: v for k, v in zipped_files.items() if not k.startswith(METADATA)}
             # quick server package integrity check:
             if "conanfile.py" not in zipped_files:
                 raise ConanException(f"Corrupted {ref} in '{remote.name}' remote: no conanfile.py")
             if "conanmanifest.txt" not in zipped_files:
@@ -80,45 +79,82 @@
         mkdir(export_folder)
         for file_name, file_path in zipped_files.items():  # copy CONANFILE
             shutil.move(file_path, os.path.join(export_folder, file_name))
 
         # Make sure that the source dir is deleted
         rmdir(layout.source())
 
+    def get_recipe_metadata(self, ref, remote, metadata):
+        """
+        Get only the metadata for a locally existing recipe in Cache
+        """
+        assert ref.revision, "get_recipe without revision specified"
+        output = ConanOutput(scope=str(ref))
+        output.info("Retrieving recipe metadata from remote '%s' " % remote.name)
+        layout = self._cache.ref_layout(ref)
+        download_export = layout.download_export()
+        try:
+            self._call_remote(remote, "get_recipe", ref, download_export, metadata,
+                              only_metadata=True)
+        except BaseException:  # So KeyboardInterrupt also cleans things
+
+            output.error(f"Error downloading metadata from remote '{remote.name}'")
+            raise
+
     def get_recipe_sources(self, ref, layout, remote):
         assert ref.revision, "get_recipe_sources requires RREV"
 
         download_folder = layout.download_export()
         export_sources_folder = layout.export_sources()
         zipped_files = self._call_remote(remote, "get_recipe_sources", ref, download_folder)
         if not zipped_files:
             mkdir(export_sources_folder)  # create the folder even if no source files
             return
 
         tgz_file = zipped_files[EXPORT_SOURCES_TGZ_NAME]
         uncompress_file(tgz_file, export_sources_folder, scope=str(ref))
 
-    def get_package(self, conanfile, pref, remote):
+    def get_package(self, conanfile, pref, remote, metadata=None):
         conanfile.output.info("Retrieving package %s from remote '%s' " % (pref.package_id,
                                                                            remote.name))
 
         assert pref.revision is not None
 
         pkg_layout = self._cache.get_or_create_pkg_layout(pref)
         pkg_layout.package_remove()  # Remove first the destination folder
         with pkg_layout.set_dirty_context_manager():
-            self._get_package(pkg_layout, pref, remote, conanfile.output)
+            self._get_package(pkg_layout, pref, remote, conanfile.output, metadata)
+
+    def get_package_metadata(self, pref, remote, metadata):
+        """
+        only download the metadata, not the packge itself
+        """
+        output = ConanOutput(scope=str(pref.ref))
+        output.info("Retrieving package metadata %s from remote '%s' "
+                    % (pref.package_id, remote.name))
+
+        assert pref.revision is not None
+        pkg_layout = self._cache.pkg_layout(pref)
+        try:
+            download_pkg_folder = pkg_layout.download_package()
+            self._call_remote(remote, "get_package", pref, download_pkg_folder,
+                              metadata, only_metadata=True)
+        except BaseException as e:  # So KeyboardInterrupt also cleans things
+            output.error("Exception while getting package metadata: %s" % str(pref.package_id))
+            output.error("Exception: %s %s" % (type(e), str(e)))
+            raise
 
-    def _get_package(self, layout, pref, remote, scoped_output):
+    def _get_package(self, layout, pref, remote, scoped_output, metadata):
         try:
             assert pref.revision is not None
 
             download_pkg_folder = layout.download_package()
             # Download files to the pkg_tgz folder, not to the final one
-            zipped_files = self._call_remote(remote, "get_package", pref, download_pkg_folder)
+            zipped_files = self._call_remote(remote, "get_package", pref, download_pkg_folder,
+                                             metadata, only_metadata=False)
             zipped_files = {k: v for k, v in zipped_files.items() if not k.startswith(METADATA)}
             # quick server package integrity check:
             for f in ("conaninfo.txt", "conanmanifest.txt", "conan_package.tgz"):
                 if f not in zipped_files:
                     raise ConanException(f"Corrupted {pref} in '{remote.name}' remote: no {f}")
             self._signer.verify(pref, download_pkg_folder)
 
@@ -216,17 +252,17 @@
         except Exception as exc:
             raise ConanException(exc, remote=remote)
 
 
 def uncompress_file(src_path, dest_folder, scope=None):
     try:
         filesize = os.path.getsize(src_path)
-        big_file = filesize > 1000000  # 10 Mb
+        big_file = filesize > 10000000  # 10 MB
         if big_file:
-            hs = _human_size(filesize)
+            hs = human_size(filesize)
             ConanOutput(scope=scope).info(f"Decompressing {hs} {os.path.basename(src_path)}")
         with open(src_path, mode='rb') as file_handler:
             tar_extract(file_handler, dest_folder)
     except Exception as e:
         error_msg = "Error while extracting downloaded file '%s' to %s\n%s\n"\
                     % (src_path, dest_folder, str(e))
         # try to remove the files
```

### Comparing `conan-server-2.0.6/conans/client/rest/__init__.py` & `conan-server-2.0.7/conans/client/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/rest/auth_manager.py` & `conan-server-2.0.7/conans/client/rest/auth_manager.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/rest/client_routes.py` & `conan-server-2.0.7/conans/client/rest/client_routes.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/rest/conan_requester.py` & `conan-server-2.0.7/conans/client/rest/conan_requester.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/rest/file_uploader.py` & `conan-server-2.0.7/conans/client/rest/file_uploader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import time
 from copy import copy
 
 from conan.api.output import ConanOutput
 from conans.client.rest import response_to_str
 from conans.errors import AuthenticationException, ConanException, \
     NotFoundException, ForbiddenException, RequestErrorException, InternalErrorException
@@ -48,50 +47,44 @@
             return response
 
     def exists(self, url, auth):
         response = self._requester.head(url, verify=self._verify_ssl, auth=auth)
         return response
 
     def upload(self, url, abs_path, auth=None, dedup=False, retry=None, retry_wait=None,
-               headers=None, display_name=None):
-        retry = retry if retry is not None else self._config.get("core.upload:retry", default=1, check_type=int)
+               headers=None):
+        retry = retry if retry is not None else self._config.get("core.upload:retry", default=1,
+                                                                 check_type=int)
         retry_wait = retry_wait if retry_wait is not None else \
             self._config.get("core.upload:retry_wait", default=5, check_type=int)
 
         # Send always the header with the Sha1
         headers = copy(headers) or {}
         headers["X-Checksum-Sha1"] = sha1sum(abs_path)
         if dedup:
             response = self._dedup(url, headers, auth)
             if response:
                 return response
 
         for counter in range(retry + 1):
             try:
-                return self._upload_file(url, abs_path, headers, auth, display_name)
+                return self._upload_file(url, abs_path, headers, auth)
             except (NotFoundException, ForbiddenException, AuthenticationException,
                     RequestErrorException):
                 raise
             except ConanException as exc:
                 if counter == retry:
                     raise
                 else:
                     if self._output:
                         self._output.error(exc)
                         self._output.info("Waiting %d seconds to retry..." % retry_wait)
                     time.sleep(retry_wait)
 
-    def _upload_file(self, url, abs_path,  headers, auth, display_name):
-        file_size = os.stat(abs_path).st_size
-        file_name = os.path.basename(abs_path)
-        description = "Uploading {}".format(file_name)
-        post_description = "Uploaded {}".format(
-            file_name) if not display_name else "Uploaded {} -> {}".format(file_name, display_name)
-
-        # self._output.info(description)
+    def _upload_file(self, url, abs_path,  headers, auth):
         with open(abs_path, mode='rb') as file_handler:
             try:
                 response = self._requester.put(url, data=file_handler, verify=self._verify_ssl,
                                                headers=headers, auth=auth)
                 self._handle_400_response(response, auth)
                 response.raise_for_status()  # Raise HTTPError for bad http response status
                 return response
```

### Comparing `conan-server-2.0.6/conans/client/rest/rest_client.py` & `conan-server-2.0.7/conans/test/utils/artifactory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,134 @@
-from conans import CHECKSUM_DEPLOY, REVISIONS, OAUTH_TOKEN
-from conans.client.rest.rest_client_v2 import RestV2Methods
-from conans.errors import AuthenticationException, ConanException
-
-
-class RestApiClientFactory(object):
-
-    def __init__(self, requester, config):
-        self._requester = requester
-        self._config = config
-        self._cached_capabilities = {}
-
-    def new(self, remote, token, refresh_token, custom_headers):
-        tmp = RestApiClient(remote, token, refresh_token, custom_headers,
-                            self._requester, self._config,
-                            self._cached_capabilities)
-        return tmp
+import os
+import time
+import uuid
 
+import requests
 
-class RestApiClient(object):
-    """
-        Rest Api Client for handle remote.
-    """
-
-    def __init__(self, remote, token, refresh_token, custom_headers, requester,
-                 config, cached_capabilities):
-
-        # Set to instance
-        self._token = token
-        self._refresh_token = refresh_token
-        self._remote_url = remote.url
-        self._custom_headers = custom_headers
-        self._requester = requester
-
-        self._verify_ssl = remote.verify_ssl
-        self._config = config
-
-        # This dict is shared for all the instances of RestApiClient
-        self._cached_capabilities = cached_capabilities
-
-    def _capable(self, capability, user=None, password=None):
-        capabilities = self._cached_capabilities.get(self._remote_url)
-        if capabilities is None:
-            tmp = RestV2Methods(self._remote_url, self._token, self._custom_headers,
-                                self._requester, self._config, self._verify_ssl)
-            capabilities = tmp.server_capabilities(user, password)
-            self._cached_capabilities[self._remote_url] = capabilities
-        return capability in capabilities
-
-    def _get_api(self):
-        revisions = self._capable(REVISIONS)
-
-        if not revisions:
-            # TODO: port conan_v2_error to 1.X if not revisions
-            raise ConanException("The remote doesn't support revisions. "
-                                 "Conan 2.0 is no longer compatible with "
-                                 "remotes that don't accept revisions.")
-        checksum_deploy = self._capable(CHECKSUM_DEPLOY)
-        return RestV2Methods(self._remote_url, self._token, self._custom_headers,
-                             self._requester, self._config, self._verify_ssl,
-                             checksum_deploy)
-
-    def get_recipe(self, ref, dest_folder):
-        return self._get_api().get_recipe(ref, dest_folder)
-
-    def get_recipe_sources(self, ref, dest_folder):
-        return self._get_api().get_recipe_sources(ref, dest_folder)
-
-    def get_package(self, pref, dest_folder):
-        return self._get_api().get_package(pref, dest_folder)
-
-    def upload_recipe(self, ref, files_to_upload):
-        return self._get_api().upload_recipe(ref, files_to_upload)
-
-    def upload_package(self, pref, files_to_upload):
-        return self._get_api().upload_package(pref, files_to_upload)
-
-    def authenticate(self, user, password):
-        api_v2 = RestV2Methods(self._remote_url, self._token, self._custom_headers,
-                               self._requester, self._config, self._verify_ssl)
-
-        if self._refresh_token and self._token:
-            token, refresh_token = api_v2.refresh_token(self._token, self._refresh_token)
-        else:
-            try:
-                # Check capabilities can raise also 401 until the new Artifactory is released
-                oauth_capable = self._capable(OAUTH_TOKEN, user, password)
-            except AuthenticationException:
-                oauth_capable = False
-
-            if oauth_capable:
-                # Artifactory >= 6.13.X
-                token, refresh_token = api_v2.authenticate_oauth(user, password)
-            else:
-                token = api_v2.authenticate(user, password)
-                refresh_token = None
-
-        return token, refresh_token
-
-    def check_credentials(self):
-        return self._get_api().check_credentials()
-
-    def search(self, pattern=None, ignorecase=True):
-        return self._get_api().search(pattern, ignorecase)
-
-    def search_packages(self, reference):
-        return self._get_api().search_packages(reference)
-
-    def remove_recipe(self, ref):
-        return self._get_api().remove_recipe(ref)
+from conans.errors import RecipeNotFoundException, PackageNotFoundException
+from conans.server.revision_list import _RevisionEntry
 
-    def remove_all_packages(self, ref):
-        return self._get_api().remove_all_packages(ref)
+ARTIFACTORY_DEFAULT_USER = os.getenv("ARTIFACTORY_DEFAULT_USER", "admin")
+ARTIFACTORY_DEFAULT_PASSWORD = os.getenv("ARTIFACTORY_DEFAULT_PASSWORD", "password")
+ARTIFACTORY_DEFAULT_URL = os.getenv("ARTIFACTORY_DEFAULT_URL", "http://localhost:8090/artifactory")
 
-    def remove_packages(self, prefs):
-        return self._get_api().remove_packages(prefs)
 
-    def server_capabilities(self):
-        return self._get_api().server_capabilities()
+class _ArtifactoryServerStore(object):
 
-    def get_recipe_revisions_references(self, ref):
-        return self._get_api().get_recipe_revisions_references(ref)
+    def __init__(self, repo_url, user, password):
+        self._user = user or ARTIFACTORY_DEFAULT_USER
+        self._password = password or ARTIFACTORY_DEFAULT_PASSWORD
+        self._repo_url = repo_url
 
-    def get_package_revisions_references(self, pref, headers=None):
-        return self._get_api().get_package_revisions_references(pref, headers=headers)
+    @property
+    def _auth(self):
+        return self._user, self._password
 
-    def get_latest_recipe_reference(self, ref):
-        return self._get_api().get_latest_recipe_reference(ref)
+    @staticmethod
+    def _root_recipe(ref):
+        return "{}/{}/{}/{}".format(ref.user, ref.name, ref.version, ref.channel)
 
-    def get_latest_package_reference(self, pref, headers):
-        return self._get_api().get_latest_package_reference(pref, headers=headers)
+    @staticmethod
+    def _ref_index(ref):
+        return "{}/index.json".format(_ArtifactoryServerStore._root_recipe(ref))
 
-    def get_recipe_revision_reference(self, ref):
-        return self._get_api().get_recipe_revision_reference(ref)
+    @staticmethod
+    def _pref_index(pref):
+        tmp = _ArtifactoryServerStore._root_recipe(pref.ref)
+        return "{}/{}/package/{}/index.json".format(tmp, pref.ref.revision, pref.package_id)
+
+    def get_recipe_revisions_references(self, ref):
+        time.sleep(0.1)  # Index appears to not being updated immediately after a remove
+        url = "{}/{}".format(self._repo_url, self._ref_index(ref))
+        response = requests.get(url, auth=self._auth)
+        response.raise_for_status()
+        the_json = response.json()
+        if not the_json["revisions"]:
+            raise RecipeNotFoundException(ref)
+        tmp = [_RevisionEntry(i["revision"], i["time"]) for i in the_json["revisions"]]
+        return tmp
+
+    def get_package_revisions_references(self, pref):
+        time.sleep(0.1)  # Index appears to not being updated immediately
+        url = "{}/{}".format(self._repo_url, self._pref_index(pref))
+        response = requests.get(url, auth=self._auth)
+        response.raise_for_status()
+        the_json = response.json()
+        if not the_json["revisions"]:
+            raise PackageNotFoundException(pref)
+        tmp = [_RevisionEntry(i["revision"], i["time"]) for i in the_json["revisions"]]
+        return tmp
 
-    def get_package_revision_reference(self, pref):
-        return self._get_api().get_package_revision_reference(pref)
+    def get_last_revision(self, ref):
+        revisions = self.get_recipe_revisions_references(ref)
+        return revisions[0]
+
+    def get_last_package_revision(self, ref):
+        revisions = self.get_package_revisions_references(ref)
+        return revisions[0]
+
+
+class ArtifactoryServer(object):
+
+    def __init__(self, *args, **kwargs):
+        self._user = ARTIFACTORY_DEFAULT_USER
+        self._password = ARTIFACTORY_DEFAULT_PASSWORD
+        self._url = ARTIFACTORY_DEFAULT_URL
+        self._repo_name = "conan_{}".format(str(uuid.uuid4()).replace("-", ""))
+        self.create_repository()
+        self.server_store = _ArtifactoryServerStore(self.repo_url, self._user, self._password)
+
+    @property
+    def _auth(self):
+        return self._user, self._password
+
+    @property
+    def repo_url(self):
+        return "{}/{}".format(self._url, self._repo_name)
+
+    @property
+    def repo_api_url(self):
+        return "{}/api/conan/{}".format(self._url, self._repo_name)
+
+    def recipe_revision_time(self, ref):
+        revs = self.server_store.get_recipe_revisions_references(ref)
+        for r in revs:
+            if r.revision == ref.revision:
+                return r.time
+        return None
+
+    def package_revision_time(self, pref):
+        revs = self.server_store.get_package_revisions_references(pref)
+        for r in revs:
+            if r.revision == pref.revision:
+                return r.time
+        return None
+
+    def create_repository(self):
+        url = "{}/api/repositories/{}".format(self._url, self._repo_name)
+        config = {"key": self._repo_name, "rclass": "local", "packageType": "conan"}
+        ret = requests.put(url, auth=self._auth, json=config)
+        ret.raise_for_status()
+
+    def package_exists(self, pref):
+        try:
+            revisions = self.server_store.get_package_revisions_references(pref)
+            if pref.revision:
+                for r in revisions:
+                    if pref.revision == r.revision:
+                        return True
+                return False
+            return True
+        except Exception:  # When resolves the latest and there is no package
+            return False
+
+    def recipe_exists(self, ref):
+        try:
+            revisions = self.server_store.get_recipe_revisions_references(ref)
+            if ref.revision:
+                for r in revisions:
+                    if ref.revision == r.revision:
+                        return True
+                return False
+            return True
+        except Exception:  # When resolves the latest and there is no package
+            return False
```

### Comparing `conan-server-2.0.6/conans/client/rest/rest_client_common.py` & `conan-server-2.0.7/conans/client/rest/rest_client_common.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/rest/rest_client_v2.py` & `conan-server-2.0.7/conans/client/rest/rest_client_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import fnmatch
 import os
 
 from conan.api.output import ConanOutput
 
 from conans.client.downloaders.caching_file_downloader import ConanInternalCacheDownloader
 from conans.client.rest.client_routes import ClientV2Router
 from conans.client.rest.file_uploader import FileUploader
@@ -31,20 +32,25 @@
     def _get_file_list_json(self, url):
         data = self.get_json(url)
         # Discarding (.keys()) still empty metadata for files
         # and make sure the paths like metadata/sign/signature are normalized to /
         data["files"] = list(d.replace("\\", "/") for d in data["files"].keys())
         return data
 
-    def get_recipe(self, ref, dest_folder):
+    def get_recipe(self, ref, dest_folder, metadata, only_metadata):
         url = self.router.recipe_snapshot(ref)
         data = self._get_file_list_json(url)
         files = data["files"]
         accepted_files = ["conanfile.py", "conan_export.tgz", "conanmanifest.txt", "metadata/sign"]
-        files = [f for f in files if any(f.startswith(m) for m in accepted_files)]
+        if only_metadata:
+            accepted_files = []
+        metadata = metadata or []
+        metadata = [f"metadata/{m}" for m in metadata]
+        files = [f for f in files if any(f.startswith(m) for m in accepted_files)
+                 or any(fnmatch.fnmatch(f, m) for m in metadata)]
 
         # If we didn't indicated reference, server got the latest, use absolute now, it's safer
         urls = {fn: self.router.recipe_file(ref, fn) for fn in files}
         self._download_and_save_files(urls, dest_folder, files, parallel=True)
         ret = {fn: os.path.join(dest_folder, fn) for fn in files}
         return ret
 
@@ -61,21 +67,27 @@
 
         # If we didn't indicated reference, server got the latest, use absolute now, it's safer
         urls = {fn: self.router.recipe_file(ref, fn) for fn in files}
         self._download_and_save_files(urls, dest_folder, files, scope=str(ref))
         ret = {fn: os.path.join(dest_folder, fn) for fn in files}
         return ret
 
-    def get_package(self, pref, dest_folder):
+    def get_package(self, pref, dest_folder, metadata, only_metadata):
         url = self.router.package_snapshot(pref)
         data = self._get_file_list_json(url)
         files = data["files"]
         # Download only known files, but not metadata (except sign)
         accepted_files = ["conaninfo.txt", "conan_package.tgz", "conanmanifest.txt", "metadata/sign"]
-        files = [f for f in files if any(f.startswith(m) for m in accepted_files)]
+        if only_metadata:
+            accepted_files = []
+        metadata = metadata or []
+        metadata = [f"metadata/{m}" for m in metadata]
+        files = [f for f in files if any(f.startswith(m) for m in accepted_files)
+                 or any(fnmatch.fnmatch(f, m) for m in metadata)]
+
         # If we didn't indicated reference, server got the latest, use absolute now, it's safer
         urls = {fn: self.router.package_file(pref, fn) for fn in files}
         self._download_and_save_files(urls, dest_folder, files, scope=str(pref.ref))
         ret = {fn: os.path.join(dest_folder, fn) for fn in files}
         return ret
 
     @staticmethod
@@ -114,17 +126,14 @@
         failed = []
         uploader = FileUploader(self.requester, self.verify_ssl, self._config)
         # conan_package.tgz and conan_export.tgz are uploaded first to avoid uploading conaninfo.txt
         # or conanamanifest.txt with missing files due to a network failure
         output = ConanOutput()
         for filename in sorted(files):
             # As the filenames are sorted, the last one is always "conanmanifest.txt"
-            if output and not output.is_terminal:
-                msg = "-> %s" % filename
-                output.info(msg)
             resource_url = urls[filename]
             try:
                 headers = {}
                 uploader.upload(resource_url, files[filename], auth=self.auth,
                                 dedup=self._checksum_deploy,
                                 headers=headers)
             except (AuthenticationException, ForbiddenException):
```

### Comparing `conan-server-2.0.6/conans/client/source.py` & `conan-server-2.0.7/conans/client/source.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/store/localdb.py` & `conan-server-2.0.7/conans/client/store/localdb.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/subsystems.py` & `conan-server-2.0.7/conans/client/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/client/userio.py` & `conan-server-2.0.7/conans/client/userio.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/conan_server.py` & `conan-server-2.0.7/conans/conan_server.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/errors.py` & `conan-server-2.0.7/conans/errors.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/migrations.py` & `conan-server-2.0.7/conans/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/build_info.py` & `conan-server-2.0.7/conans/model/build_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import copy
+import json
 import os
 from collections import OrderedDict, defaultdict
 
 from conan.api.output import ConanOutput
 from conans.errors import ConanException
+from conans.util.files import load, save
 
 _DIRS_VAR_NAMES = ["_includedirs", "_srcdirs", "_libdirs", "_resdirs", "_bindirs", "_builddirs",
                    "_frameworkdirs", "_objects"]
 _FIELD_VAR_NAMES = ["_system_libs", "_frameworks", "_libs", "_defines", "_cflags", "_cxxflags",
                     "_sharedlinkflags", "_exelinkflags"]
 _ALL_NAMES = _DIRS_VAR_NAMES + _FIELD_VAR_NAMES
 
@@ -50,15 +52,15 @@
         return super(MockInfoProperty, self).__setattr__(attr, value)
 
 
 class _Component:
 
     def __init__(self, set_defaults=False):
         # ###### PROPERTIES
-        self._generator_properties = None
+        self._properties = None
 
         # ###### DIRECTORIES
         self._includedirs = None  # Ordered list of include paths
         self._srcdirs = None  # Ordered list of source paths
         self._libdirs = None  # Directories to find libraries
         self._resdirs = None  # Directories to find resources, data, etc
         self._bindirs = None  # Directories to find executables and shared libs
@@ -105,17 +107,46 @@
             "cflags": self._cflags,
             "cxxflags": self._cxxflags,
             "sharedlinkflags": self._sharedlinkflags,
             "exelinkflags": self._exelinkflags,
             "objects": self._objects,
             "sysroot": self._sysroot,
             "requires": self._requires,
-            "properties": self._generator_properties
+            "properties": self._properties
         }
 
+    @staticmethod
+    def deserialize(contents):
+        result = _Component()
+        # TODO: Refactor to avoid this repetition
+        fields = [
+            "includedirs",
+            "srcdirs",
+            "libdirs",
+            "resdirs",
+            "bindirs",
+            "builddirs",
+            "frameworkdirs",
+            "system_libs",
+            "frameworks",
+            "libs",
+            "defines",
+            "cflags",
+            "cxxflags",
+            "sharedlinkflags",
+            "exelinkflags",
+            "objects",
+            "sysroot",
+            "requires",
+            "properties"
+        ]
+        for f in fields:
+            setattr(result, f"_{f}", contents[f])
+        return result
+
     @property
     def includedirs(self):
         if self._includedirs is None:
             self._includedirs = []
         return self._includedirs
 
     @includedirs.setter
@@ -317,23 +348,23 @@
     def required_component_names(self):
         """ Names of the required components of the same package (not scoped with ::)"""
         if self.requires is None:
             return []
         return [r for r in self.requires if "::" not in r]
 
     def set_property(self, property_name, value):
-        if self._generator_properties is None:
-            self._generator_properties = {}
-        self._generator_properties[property_name] = value
+        if self._properties is None:
+            self._properties = {}
+        self._properties[property_name] = value
 
     def get_property(self, property_name):
-        if self._generator_properties is None:
+        if self._properties is None:
             return None
         try:
-            return self._generator_properties[property_name]
+            return self._properties[property_name]
         except KeyError:
             pass
 
     def get_init(self, attribute, default):
         # Similar to dict.setdefault
         item = getattr(self, attribute)
         if item is not None:
@@ -358,24 +389,24 @@
                 else:
                     setattr(self, varname, other_values)
 
         if other.requires:
             current_values = self.get_init("requires", [])
             merge_list(other.requires, current_values)
 
-        if other._generator_properties:
-            current_values = self.get_init("_generator_properties", {})
-            current_values.update(other._generator_properties)
+        if other._properties:
+            current_values = self.get_init("_properties", {})
+            current_values.update(other._properties)
 
     def set_relative_base_folder(self, folder):
         for varname in _DIRS_VAR_NAMES:
             origin = getattr(self, varname)
             if origin is not None:
                 origin[:] = [os.path.join(folder, el) for el in origin]
-        properties = self._generator_properties
+        properties = self._properties
         if properties is not None:
             modules = properties.get("cmake_build_modules")  # Only this prop at this moment
             if modules is not None:
                 assert isinstance(modules, list), "cmake_build_modules must be a list"
                 properties["cmake_build_modules"] = [os.path.join(folder, v) for v in modules]
 
     def deploy_base_folder(self, package_folder, deploy_folder):
@@ -383,29 +414,30 @@
             rel_path = os.path.relpath(el, package_folder)
             return os.path.join(deploy_folder, rel_path)
 
         for varname in _DIRS_VAR_NAMES:
             origin = getattr(self, varname)
             if origin is not None:
                 origin[:] = [relocate(f) for f in origin]
-        properties = self._generator_properties
+        properties = self._properties
         if properties is not None:
             modules = properties.get("cmake_build_modules")  # Only this prop at this moment
             if modules is not None:
                 assert isinstance(modules, list), "cmake_build_modules must be a list"
                 properties["cmake_build_modules"] = [relocate(f) for f in modules]
 
+    def parsed_requires(self):
+        return [r.split("::", 1) if "::" in r else (None, r) for r in self.requires]
+
 
 class CppInfo:
 
     def __init__(self, set_defaults=False):
         self.components = defaultdict(lambda: _Component(set_defaults))
-        # Main package is a component with None key
         self._package = _Component(set_defaults)
-        self._aggregated = None  # A _NewComponent object with all the components aggregated
 
     def __getattr__(self, attr):
         # all cpp_info.xxx of not defined things will go to the global package
         return getattr(self._package, attr)
 
     def __setattr__(self, attr, value):
         if attr in ("components", "_package", "_aggregated"):
@@ -415,14 +447,27 @@
 
     def serialize(self):
         ret = {"root": self._package.serialize()}
         for component_name, info in self.components.items():
             ret[component_name] = info.serialize()
         return ret
 
+    def deserialize(self, content):
+        self._package = _Component.deserialize(content.pop("root"))
+        for component_name, info in content.items():
+            self.components[component_name] = _Component.deserialize(info)
+        return self
+
+    def save(self, path):
+        save(path, json.dumps(self.serialize()))
+
+    def load(self, path):
+        content = json.loads(load(path))
+        return self.deserialize(content)
+
     @property
     def has_components(self):
         return len(self.components) > 0
 
     def merge(self, other, overwrite=False):
         """Merge 'other' into self. 'other' can be an old cpp_info object
         Used to merge Layout source + build cpp objects info (editables)
@@ -484,30 +529,32 @@
             if cached_processed == processed:
                 self._raise_circle_components_requires_error()
 
         return OrderedDict([(cname, self.components[cname]) for cname in processed])
 
     def aggregated_components(self):
         """Aggregates all the components as global values, returning a new CppInfo"""
-        if self._aggregated is None:
-            if self.has_components:
-                result = _Component()
-                # Reversed to make more dependant first
-                for component in reversed(self.get_sorted_components().values()):
-                    result.merge(component)
-                # NOTE: The properties are not aggregated because they might refer only to the
-                # component like "cmake_target_name" describing the target name FOR THE component
-                # not the namespace.
-                # FIXME: What to do about sysroot?
-                result._generator_properties = copy.copy(self._package._generator_properties)
-            else:
-                result = copy.copy(self._package)
-            self._aggregated = CppInfo()
-            self._aggregated._package = result
-        return self._aggregated
+        # This method had caching before, but after a ``--deployer``, the package changes
+        # location, and this caching was invalid, still pointing to the Conan cache instead of
+        # the deployed
+        if self.has_components:
+            result = _Component()
+            # Reversed to make more dependant first
+            for component in reversed(self.get_sorted_components().values()):
+                result.merge(component)
+            # NOTE: The properties are not aggregated because they might refer only to the
+            # component like "cmake_target_name" describing the target name FOR THE component
+            # not the namespace.
+            # FIXME: What to do about sysroot?
+            result._properties = copy.copy(self._package._properties)
+        else:
+            result = copy.copy(self._package)
+        aggregated = CppInfo()
+        aggregated._package = result
+        return aggregated
 
     def check_component_requires(self, conanfile):
         """ quality check for component requires:
         - Check that all recipe ``requires`` are used if consumer recipe explicit opt-in to use
           component requires
         - Check that component external dep::comp dependency "dep" is a recipe "requires"
         - Check that every internal component require actually exist
```

### Comparing `conan-server-2.0.6/conans/model/conan_file.py` & `conan-server-2.0.7/conans/model/conan_file.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/conanfile_interface.py` & `conan-server-2.0.7/conans/model/conanfile_interface.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/conf.py` & `conan-server-2.0.7/conans/model/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 from conans.model.recipe_ref import ref_matches
 
 BUILT_IN_CONFS = {
     "core:required_conan_version": "Raise if current version does not match the defined range.",
     "core:non_interactive": "Disable interactive user input, raises error if input necessary",
     "core:skip_warnings": "Do not show warnings in this list",
     "core:default_profile": "Defines the default host profile ('default' by default)",
-    "core:default_build_profile": "Defines the default build profile (None by default)",
+    "core:default_build_profile": "Defines the default build profile ('default' by default)",
     "core:allow_uppercase_pkg_names": "Temporarily (will be removed in 2.X) allow uppercase names",
     "core.version_ranges:resolve_prereleases": "Whether version ranges can resolve to pre-releases or not",
     "core.upload:retry": "Number of retries in case of failure when uploading to Conan server",
     "core.upload:retry_wait": "Seconds to wait between upload attempts to Conan server",
     "core.download:parallel": "Number of concurrent threads to download packages",
     "core.download:retry": "Number of retries in case of failure when downloading from Conan server",
     "core.download:retry_wait": "Seconds to wait between download attempts from Conan server",
     "core.download:download_cache": "Define path to a file download cache",
     "core.cache:storage_path": "Absolute path where the packages and database are stored",
     # Sources backup
     "core.sources:download_cache": "Folder to store the sources backup",
     "core.sources:download_urls": "List of URLs to download backup sources from",
     "core.sources:upload_url": "Remote URL to upload backup sources to",
+    "core.sources:exclude_urls": "URLs which will not be backed up",
     # Package ID
     "core.package_id:default_unknown_mode": "By default, 'semver_mode'",
     "core.package_id:default_non_embed_mode": "By default, 'minor_mode'",
     "core.package_id:default_embed_mode": "By default, 'full_mode'",
     "core.package_id:default_python_mode": "By default, 'minor_mode'",
     "core.package_id:default_build_mode": "By default, 'None'",
     # General HTTP(python-requests) configuration
@@ -48,16 +49,16 @@
     "tools.android:cmake_legacy_toolchain": "Define to explicitly pass ANDROID_USE_LEGACY_TOOLCHAIN_FILE in CMake toolchain",
     "tools.build:skip_test": "Do not execute CMake.test() and Meson.test() when enabled",
     "tools.build:download_source": "Force download of sources for every package",
     "tools.build:jobs": "Default compile jobs number -jX Ninja, Make, /MP VS (default: max CPUs)",
     "tools.build:sysroot": "Pass the --sysroot=<tools.build:sysroot> flag if available. (None by default)",
     "tools.build.cross_building:can_run": "Bool value that indicates whether is possible to run a non-native "
                                           "app on the same architecture. It's used by 'can_run' tool",
-    "tools.build:verbosity": "Verbosity of MSBuild and XCodeBuild build systems. "
-                             "Possible values are 'quiet', 'error', 'warning', 'notice', 'status', 'verbose', 'normal', 'debug', 'v', 'trace' and 'vv'",
+    "tools.build:verbosity": "Verbosity of build systems if set. Possible values are 'quiet' and 'verbose'",
+    "tools.compilation:verbosity": "Verbosity of compilation tools if set. Possible values are 'quiet' and 'verbose'",
     "tools.cmake.cmaketoolchain:generator": "User defined CMake generator to use instead of default",
     "tools.cmake.cmaketoolchain:find_package_prefer_config": "Argument for the CMAKE_FIND_PACKAGE_PREFER_CONFIG",
     "tools.cmake.cmaketoolchain:toolchain_file": "Use other existing file rather than conan_toolchain.cmake one",
     "tools.cmake.cmaketoolchain:user_toolchain": "Inject existing user toolchains at the beginning of conan_toolchain.cmake",
     "tools.cmake.cmaketoolchain:system_name": "Define CMAKE_SYSTEM_NAME in CMakeToolchain",
     "tools.cmake.cmaketoolchain:system_version": "Define CMAKE_SYSTEM_VERSION in CMakeToolchain",
     "tools.cmake.cmaketoolchain:system_processor": "Define CMAKE_SYSTEM_PROCESSOR in CMakeToolchain",
@@ -271,29 +272,31 @@
             self._check_conf_name(conf)
 
     def items(self):
         # FIXME: Keeping backward compatibility
         for k, v in self._values.items():
             yield k, v.value
 
-    def get(self, conf_name, default=None, check_type=None):
+    def get(self, conf_name, default=None, check_type=None, choices=None):
         """
         Get all the values of the given configuration name.
 
         :param conf_name: Name of the configuration.
         :param default: Default value in case of conf does not have the conf_name key.
         :param check_type: Check the conf type(value) is the same as the given by this param.
                            There are two default smart conversions for bool and str types.
         """
         # Skipping this check only the user.* configurations
         self._check_conf_name(conf_name)
 
         conf_value = self._values.get(conf_name)
         if conf_value:
             v = conf_value.value
+            if choices is not None and v not in choices:
+                raise ConanException(f"Unknown value '{v}' for '{conf_name}'")
             # Some smart conversions
             if check_type is bool and not isinstance(v, bool):
                 # Perhaps, user has introduced a "false", "0" or even "off"
                 return str(v).lower() not in Conf.boolean_false_expressions
             elif check_type is str and not isinstance(v, str):
                 return str(v)
             elif v is None:  # value was unset
@@ -494,21 +497,21 @@
 
     def __repr__(self):
         return "ConfDefinition: " + repr(self._pattern_confs)
 
     def __bool__(self):
         return bool(self._pattern_confs)
 
-    def get(self, conf_name, default=None, check_type=None):
+    def get(self, conf_name, default=None, check_type=None, choices=None):
         """
         Get the value of the conf name requested and convert it to the [type]-like passed.
         """
         pattern, name = self._split_pattern_name(conf_name)
         return self._pattern_confs.get(pattern, Conf()).get(name, default=default,
-                                                            check_type=check_type)
+                                                            check_type=check_type, choices=choices)
 
     def show(self, fnpattern):
         """
         Get the value of the confs that match the requested pattern
         """
         result = {}
```

### Comparing `conan-server-2.0.6/conans/model/dependencies.py` & `conan-server-2.0.7/conans/model/dependencies.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/graph_lock.py` & `conan-server-2.0.7/conans/model/graph_lock.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/info.py` & `conan-server-2.0.7/conans/model/info.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/layout.py` & `conan-server-2.0.7/conans/model/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,30 +87,30 @@
     @property
     def source_folder(self):
         if self._base_source is None:
             return None
         if not self.source:
             return self._base_source
 
-        return os.path.join(self._base_source, self.source)
+        return os.path.normpath(os.path.join(self._base_source, self.source))
 
     @property
     def base_source(self):
         return self._base_source
 
     def set_base_source(self, folder):
         self._base_source = folder
 
     @property
     def build_folder(self):
         if self._base_build is None:
             return None
         if not self.build:
             return self._base_build
-        return os.path.join(self._base_build, self.build)
+        return os.path.normpath(os.path.join(self._base_build, self.build))
 
     @property
     def recipe_metadata_folder(self):
         return self._base_recipe_metadata
 
     def set_base_recipe_metadata(self, folder):
         self._base_recipe_metadata = folder
@@ -143,15 +143,15 @@
 
     @property
     def generators_folder(self):
         if self._base_generators is None:
             return None
         if not self.generators:
             return self._base_generators
-        return os.path.join(self._base_generators, self.generators)
+        return os.path.normpath(os.path.join(self._base_generators, self.generators))
 
     def set_base_generators(self, folder):
         self._base_generators = folder
 
     @property
     def base_export(self):
         return self._base_export
```

### Comparing `conan-server-2.0.6/conans/model/manifest.py` & `conan-server-2.0.7/conans/model/manifest.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/options.py` & `conan-server-2.0.7/conans/model/options.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/package_ref.py` & `conan-server-2.0.7/conans/model/package_ref.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/pkg_type.py` & `conan-server-2.0.7/conans/model/pkg_type.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/profile.py` & `conan-server-2.0.7/conans/model/profile.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/recipe_ref.py` & `conan-server-2.0.7/conans/model/recipe_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
             ConanOutput().warning(f"User containing special chars is discouraged '{self.user}'")
         if self.channel and pattern.search(self.channel):
             ConanOutput().warning(f"Channel containing special chars is discouraged "
                                   f"'{self.channel}'")
 
     def matches(self, pattern, is_consumer):
         negate = False
-        if pattern.startswith("!"):
+        if pattern.startswith("!") or pattern.startswith("~"):
             pattern = pattern[1:]
             negate = True
 
         condition = ((pattern == "&" and is_consumer) or
                       fnmatch.fnmatchcase(str(self), pattern) or
                       fnmatch.fnmatchcase(self.repr_notime(), pattern))
         if negate:
```

### Comparing `conan-server-2.0.6/conans/model/requires.py` & `conan-server-2.0.7/conans/model/requires.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/rest_routes.py` & `conan-server-2.0.7/conans/model/rest_routes.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/settings.py` & `conan-server-2.0.7/conans/model/settings.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/version.py` & `conan-server-2.0.7/conans/model/version.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/model/version_range.py` & `conan-server-2.0.7/conans/model/version_range.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/paths/__init__.py` & `conan-server-2.0.7/conans/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/pylint_plugin.py` & `conan-server-2.0.7/conans/pylint_plugin.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/search/query_parse.py` & `conan-server-2.0.7/conans/search/query_parse.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/search/search.py` & `conan-server-2.0.7/conans/search/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 def filter_packages(query, results: Dict[PkgReference, dict]):
     if query is None:
         return results
     try:
         if "!" in query:
             raise ConanException("'!' character is not allowed")
+        if "~" in query:
+            raise ConanException("'~' character is not allowed")
         if " not " in query or query.startswith("not "):
             raise ConanException("'not' operator is not allowed")
         postfix = infix_to_postfix(query) if query else []
         result = OrderedDict()
         for pref, data in results.items():
             if _evaluate_postfix_with_info(postfix, data):
                 result[pref] = data
```

### Comparing `conan-server-2.0.6/conans/server/conf/__init__.py` & `conan-server-2.0.7/conans/server/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/conf/default_server_conf.py` & `conan-server-2.0.7/conans/server/conf/default_server_conf.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/crypto/jwt/jwt_credentials_manager.py` & `conan-server-2.0.7/conans/server/crypto/jwt/jwt_credentials_manager.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/crypto/jwt/jwt_manager.py` & `conan-server-2.0.7/conans/server/crypto/jwt/jwt_manager.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/launcher.py` & `conan-server-2.0.7/conans/server/launcher.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/migrate.py` & `conan-server-2.0.7/conans/server/migrate.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/plugin_loader.py` & `conan-server-2.0.7/conans/server/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/rest/api_v2.py` & `conan-server-2.0.7/conans/server/rest/api_v2.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/rest/bottle_plugins/authorization_header.py` & `conan-server-2.0.7/conans/server/rest/bottle_plugins/authorization_header.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/rest/bottle_plugins/http_basic_authentication.py` & `conan-server-2.0.7/conans/server/rest/bottle_plugins/http_basic_authentication.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/rest/bottle_plugins/jwt_authentication.py` & `conan-server-2.0.7/conans/server/rest/bottle_plugins/jwt_authentication.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/rest/bottle_plugins/return_handler.py` & `conan-server-2.0.7/conans/server/rest/bottle_plugins/return_handler.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/rest/controller/v2/conan.py` & `conan-server-2.0.7/conans/server/rest/controller/v2/conan.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/rest/controller/v2/delete.py` & `conan-server-2.0.7/conans/server/rest/controller/v2/delete.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/rest/controller/v2/revisions.py` & `conan-server-2.0.7/conans/server/rest/controller/v2/revisions.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/rest/controller/v2/search.py` & `conan-server-2.0.7/conans/server/rest/controller/v2/search.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/rest/controller/v2/users.py` & `conan-server-2.0.7/conans/server/rest/controller/v2/users.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/rest/server.py` & `conan-server-2.0.7/conans/server/rest/server.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/revision_list.py` & `conan-server-2.0.7/conans/server/revision_list.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/service/authorize.py` & `conan-server-2.0.7/conans/server/service/authorize.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,68 +27,68 @@
 
     @abstractmethod
     def check_read_conan(self, username, ref):
         """
         username: User that request to read the conans
         ref: RecipeReference
         """
-        raise NotImplemented()
+        raise NotImplementedError()
 
     @abstractmethod
     def check_write_conan(self, username, ref):
         """
         username: User that request to write the conans
         ref: RecipeReference
         """
-        raise NotImplemented()
+        raise NotImplementedError()
 
     @abstractmethod
     def check_delete_conan(self, username, ref):
         """
         username: User requesting a recipe's deletion
         ref: ConanFileReference
         """
-        raise NotImplemented()
+        raise NotImplementedError()
 
     @abstractmethod
     def check_read_package(self, username, pref):
         """
         username: User that request to read the package
         pref: PackageReference
         """
-        raise NotImplemented()
+        raise NotImplementedError()
 
     @abstractmethod
     def check_write_package(self, username, pref):
         """
         username: User that request to write the package
         pref: PackageReference
         """
-        raise NotImplemented()
+        raise NotImplementedError()
 
     @abstractmethod
     def check_delete_package(self, username, pref):
         """
         username: User requesting a package's deletion
         pref: PackageReference
         """
-        raise NotImplemented()
+        raise NotImplementedError()
 
 
 class Authenticator(object, metaclass=ABCMeta):
     """
     Handles the user authentication
     """
     @abstractmethod
     def valid_user(self, username, plain_password):
         """
         username: User that request to read the conans
         plain_password:
         """
-        raise NotImplemented()
+        raise NotImplementedError()
 
 #  ########################################################
 #  ############ BASIC IMPLEMENTATION CLASSES ##############
 #  ########################################################
 
 
 class BasicAuthenticator(Authenticator):
```

### Comparing `conan-server-2.0.6/conans/server/service/user_service.py` & `conan-server-2.0.7/conans/server/service/user_service.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/service/v2/search.py` & `conan-server-2.0.7/conans/server/service/v2/search.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/service/v2/service_v2.py` & `conan-server-2.0.7/conans/server/service/v2/service_v2.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/store/disk_adapter.py` & `conan-server-2.0.7/conans/server/store/disk_adapter.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/store/server_store.py` & `conan-server-2.0.7/conans/server/store/server_store.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/server/utils/files.py` & `conan-server-2.0.7/conans/server/utils/files.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/test/conftest.py` & `conan-server-2.0.7/conans/test/conftest.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/test/utils/mocks.py` & `conan-server-2.0.7/conans/test/utils/mocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from collections import namedtuple
 from io import StringIO
 
 
 from conan import ConanFile
 from conan.internal.conan_app import ConanFileHelpers
 from conans.model.conf import Conf
 from conans.model.layout import Folders, Infos
@@ -99,26 +98,24 @@
         if self.runner:
             kwargs["output"] = None
             self.runner(*args, **kwargs)
 
 
 class ConanFileMock(ConanFile):
 
-    def __init__(self, shared=None):
-        self.display_name = ""
+    def __init__(self, display_name=""):
+        self.display_name = display_name
         self._conan_node = None
         self.command = None
         self._commands = []
         self.path = None
         self.settings = None
         self.settings_build = MockSettings({"os": "Linux", "arch": "x86_64"})
         self.settings_target = None
         self.options = Options()
-        if shared is not None:
-            self.options = namedtuple("options", "shared")(shared)
         self.generators = []
         self.captured_env = {}
         self.folders = Folders()
         self.folders.set_base_source(".")
         self.folders.set_base_export_sources(".")
         self.folders.set_base_build(".")
         self.folders.set_base_generators(".")
```

### Comparing `conan-server-2.0.6/conans/test/utils/profiles.py` & `conan-server-2.0.7/conans/test/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/test/utils/scm.py` & `conan-server-2.0.7/conans/test/utils/scm.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/test/utils/server_launcher.py` & `conan-server-2.0.7/conans/test/utils/server_launcher.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/test/utils/test_files.py` & `conan-server-2.0.7/conans/test/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/test/utils/tools.py` & `conan-server-2.0.7/conans/test/utils/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,16 +653,15 @@
         # Let's make it easier for all the test clients
         latest_prev = self.cache.get_latest_package_reference(pref)
         pkg_layout = self.cache.pkg_layout(latest_prev)
         return pkg_layout
 
     def get_latest_ref_layout(self, ref) -> RecipeLayout:
         """Get the latest RecipeLayout given a file reference"""
-        latest_rrev = self.cache.get_latest_recipe_reference(ref)
-        ref_layout = self.cache.ref_layout(latest_rrev)
+        ref_layout = self.cache.ref_layout(ref)
         return ref_layout
 
     def get_default_host_profile(self):
         api = ConanAPI(cache_folder=self.cache_folder)
         return api.profiles.get_profile([api.profiles.get_default_host()])
 
     def get_default_build_profile(self):
@@ -762,14 +761,20 @@
         return package_id
 
     def created_package_reference(self, ref):
         pref = re.search(r"{}: Full package reference: (\S+)".format(str(ref)),
                                str(self.out)).group(1)
         return PkgReference.loads(pref)
 
+    def created_package_folder(self, ref):
+        pref = self.created_package_reference(ref)
+        prev = self.cache.get_latest_package_reference(pref)
+        pkg_folder = self.cache.pkg_layout(prev).package()
+        return pkg_folder
+
     def exported_recipe_revision(self):
         return re.search(r": Exported: .*#(\S+)", str(self.out)).group(1)
 
 
 class TurboTestClient(TestClient):
 
     def __init__(self, *args, **kwargs):
```

### Comparing `conan-server-2.0.6/conans/util/config_parser.py` & `conan-server-2.0.7/conans/util/config_parser.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/util/dates.py` & `conan-server-2.0.7/conans/util/dates.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/util/encrypt.py` & `conan-server-2.0.7/conans/util/encrypt.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/util/env.py` & `conan-server-2.0.7/conans/util/env.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/util/files.py` & `conan-server-2.0.7/conans/util/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -347,7 +347,34 @@
 
     with zipfile.ZipFile(filename, "r") as z:
         zip_info = z.infolist()
         extracted_size = 0
         for file_ in zip_info:
             extracted_size += file_.file_size
             z.extract(file_, full_path)
+
+
+def human_size(size_bytes):
+    """
+    format a size in bytes into a 'human' file size, e.g. B, KB, MB, GB, TB, PB
+    Note that bytes will be reported in whole numbers but KB and above will have
+    greater precision.  e.g. 43 B, 443 KB, 4.3 MB, 4.43 GB, etc
+    """
+    unit_size = 1000.0
+    suffixes_table = [('B', 0), ('KB', 1), ('MB', 1), ('GB', 2), ('TB', 2), ('PB', 2)]
+
+    num = float(size_bytes)
+    the_precision = None
+    the_suffix = None
+    for suffix, precision in suffixes_table:
+        the_precision = precision
+        the_suffix = suffix
+        if num < unit_size:
+            break
+        num /= unit_size
+
+    if the_precision == 0:
+        formatted_size = "%d" % num
+    else:
+        formatted_size = str(round(num, ndigits=the_precision))
+
+    return "%s%s" % (formatted_size, the_suffix)
```

### Comparing `conan-server-2.0.6/conans/util/locks.py` & `conan-server-2.0.7/conans/util/locks.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/util/runners.py` & `conan-server-2.0.7/conans/util/runners.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/util/sha.py` & `conan-server-2.0.7/conans/util/sha.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/conans/util/windows.py` & `conan-server-2.0.7/conans/util/windows.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.0.6/setup.py` & `conan-server-2.0.7/setup.py`

 * *Files identical despite different names*

