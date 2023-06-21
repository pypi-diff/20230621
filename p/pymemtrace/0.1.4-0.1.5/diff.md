# Comparing `tmp/pymemtrace-0.1.4.tar.gz` & `tmp/pymemtrace-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemtrace-0.1.4.tar", last modified: Sat Mar 19 10:49:28 2022, max compression
+gzip compressed data, was "pymemtrace-0.1.5.tar", last modified: Wed Jun 21 12:12:26 2023, max compression
```

## Comparing `pymemtrace-0.1.4.tar` & `pymemtrace-0.1.5.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.299527 pymemtrace-0.1.4/
--rw-r--r--   0 engun      (501) staff       (20)      146 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/AUTHORS.rst
--rw-r--r--   0 engun      (501) staff       (20)     3250 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 engun      (501) staff       (20)      754 2022-03-19 09:12:15.000000 pymemtrace-0.1.4/HISTORY.rst
--rw-r--r--   0 engun      (501) staff       (20)     1065 2017-12-04 13:23:31.000000 pymemtrace-0.1.4/LICENSE
--rw-r--r--   0 engun      (501) staff       (20)      298 2022-03-17 09:41:31.000000 pymemtrace-0.1.4/MANIFEST.in
--rw-r--r--   0 engun      (501) staff       (20)     6993 2022-03-19 10:49:28.299644 pymemtrace-0.1.4/PKG-INFO
--rw-r--r--   0 engun      (501) staff       (20)     5314 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/README.rst
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.195775 pymemtrace-0.1.4/docs/
--rw-r--r--   0 engun      (501) staff       (20)     6783 2018-01-18 10:19:00.000000 pymemtrace-0.1.4/docs/Makefile
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.185985 pymemtrace-0.1.4/docs/_build/
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.186227 pymemtrace-0.1.4/docs/_build/html/
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.205699 pymemtrace-0.1.4/docs/_build/html/_images/
--rw-r--r--   0 engun      (501) staff       (20)    57321 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_20328.svg
--rw-r--r--   0 engun      (501) staff       (20)    33545 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_3938.svg
--rw-r--r--   0 engun      (501) staff       (20)   203722 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_4147.svg
--rw-r--r--   0 engun      (501) staff       (20)    30456 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_76753.svg
--rw-r--r--   0 engun      (501) staff       (20)    26786 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_77077.svg
--rw-r--r--   0 engun      (501) staff       (20)   186964 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_77633.svg
--rw-r--r--   0 engun      (501) staff       (20)    34351 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_8631.svg
--rw-r--r--   0 engun      (501) staff       (20)    57467 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_8692.svg
--rw-r--r--   0 engun      (501) staff       (20)    40610 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_9236.svg
--rw-r--r--   0 engun      (501) staff       (20)    30809 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_9434.svg
--rw-r--r--   0 engun      (501) staff       (20)    39081 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_9552.svg
--rw-r--r--   0 engun      (501) staff       (20)    39339 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_9685.svg
--rw-r--r--   0 engun      (501) staff       (20)    32943 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/_build/html/_images/process.log_14129.svg
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.228963 pymemtrace-0.1.4/docs/_build/html/_static/
--rw-r--r--   0 engun      (501) staff       (20)      673 2020-10-31 12:33:19.000000 pymemtrace-0.1.4/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 engun      (501) staff       (20)     3500 2020-10-31 12:33:19.000000 pymemtrace-0.1.4/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 engun      (501) staff       (20)     3578 2020-10-31 12:33:19.000000 pymemtrace-0.1.4/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 engun      (501) staff       (20)     3445 2020-10-31 12:33:19.000000 pymemtrace-0.1.4/docs/_build/html/_static/comment.png
--rw-r--r--   0 engun      (501) staff       (20)      347 2020-10-31 12:33:19.000000 pymemtrace-0.1.4/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 engun      (501) staff       (20)      347 2020-10-31 12:33:19.000000 pymemtrace-0.1.4/docs/_build/html/_static/down.png
--rw-r--r--   0 engun      (501) staff       (20)      286 2020-11-09 16:32:13.000000 pymemtrace-0.1.4/docs/_build/html/_static/file.png
--rw-r--r--   0 engun      (501) staff       (20)       90 2020-11-09 16:32:13.000000 pymemtrace-0.1.4/docs/_build/html/_static/minus.png
--rw-r--r--   0 engun      (501) staff       (20)       90 2020-11-09 16:32:13.000000 pymemtrace-0.1.4/docs/_build/html/_static/plus.png
--rw-r--r--   0 engun      (501) staff       (20)      345 2020-10-31 12:33:19.000000 pymemtrace-0.1.4/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 engun      (501) staff       (20)      345 2020-10-31 12:33:19.000000 pymemtrace-0.1.4/docs/_build/html/_static/up.png
--rw-r--r--   0 engun      (501) staff       (20)     6467 2017-12-04 13:28:23.000000 pymemtrace-0.1.4/docs/make.bat
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.235002 pymemtrace-0.1.4/docs/source/
--rw-r--r--   0 engun      (501) staff       (20)       31 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/authors.rst
--rwxr-xr-x   0 engun      (501) staff       (20)     8762 2022-03-19 09:13:04.000000 pymemtrace-0.1.4/docs/source/conf.py
--rw-r--r--   0 engun      (501) staff       (20)       36 2020-11-11 14:53:24.000000 pymemtrace-0.1.4/docs/source/contributing.rst
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.238072 pymemtrace-0.1.4/docs/source/examples/
--rw-r--r--   0 engun      (501) staff       (20)     5431 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/examples/c_py_mem_trace.rst
--rw-r--r--   0 engun      (501) staff       (20)     4514 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/examples/debug_malloc_stats.rst
--rw-r--r--   0 engun      (501) staff       (20)    40512 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/examples/dtrace.rst
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.239102 pymemtrace-0.1.4/docs/source/examples/images/
--rw-r--r--   0 engun      (501) staff       (20)    32943 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/examples/images/process.log_14129.svg
--rw-r--r--   0 engun      (501) staff       (20)     8532 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/examples/process.rst
--rw-r--r--   0 engun      (501) staff       (20)     7986 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/examples/trace_malloc.rst
--rw-r--r--   0 engun      (501) staff       (20)      219 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/examples.rst
--rw-r--r--   0 engun      (501) staff       (20)       31 2020-11-11 14:53:24.000000 pymemtrace-0.1.4/docs/source/history.rst
--rw-r--r--   0 engun      (501) staff       (20)      374 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/index.rst
--rw-r--r--   0 engun      (501) staff       (20)     1202 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/installation.rst
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.240568 pymemtrace-0.1.4/docs/source/memory_leaks/
--rw-r--r--   0 engun      (501) staff       (20)    11560 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/memory_leaks/introduction.rst
--rw-r--r--   0 engun      (501) staff       (20)     2416 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/memory_leaks/techniques.rst
--rw-r--r--   0 engun      (501) staff       (20)     9777 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/memory_leaks/tools.rst
--rw-r--r--   0 engun      (501) staff       (20)      205 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/memory_leaks.rst
--rw-r--r--   0 engun      (501) staff       (20)       30 2020-11-11 14:53:24.000000 pymemtrace-0.1.4/docs/source/readme.rst
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.256955 pymemtrace-0.1.4/docs/source/ref/
--rw-r--r--   0 engun      (501) staff       (20)      789 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/ref/c_mem_leak.rst
--rw-r--r--   0 engun      (501) staff       (20)      610 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/ref/c_py_mem_trace.rst
--rw-r--r--   0 engun      (501) staff       (20)      191 2020-11-11 14:53:24.000000 pymemtrace-0.1.4/docs/source/ref/debug_malloc_stats.rst
--rw-r--r--   0 engun      (501) staff       (20)      151 2020-11-11 14:53:24.000000 pymemtrace-0.1.4/docs/source/ref/process.rst
--rw-r--r--   0 engun      (501) staff       (20)      185 2020-11-11 14:53:24.000000 pymemtrace-0.1.4/docs/source/ref/redirect_stdout.rst
--rw-r--r--   0 engun      (501) staff       (20)      256 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/ref/trace_malloc.rst
--rw-r--r--   0 engun      (501) staff       (20)      233 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/reference.rst
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.259390 pymemtrace-0.1.4/docs/source/tech_notes/
--rw-r--r--   0 engun      (501) staff       (20)    23952 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/cPyMemTrace.rst
--rw-r--r--   0 engun      (501) staff       (20)     9117 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/dtrace.rst
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.270666 pymemtrace-0.1.4/docs/source/tech_notes/images/
--rw-r--r--   0 engun      (501) staff       (20)    57321 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_20328.svg
--rw-r--r--   0 engun      (501) staff       (20)    33545 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_3938.svg
--rw-r--r--   0 engun      (501) staff       (20)   203722 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_4147.svg
--rw-r--r--   0 engun      (501) staff       (20)    30456 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_76753.svg
--rw-r--r--   0 engun      (501) staff       (20)    26786 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_77077.svg
--rw-r--r--   0 engun      (501) staff       (20)   186964 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_77633.svg
--rw-r--r--   0 engun      (501) staff       (20)    34351 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_8631.svg
--rw-r--r--   0 engun      (501) staff       (20)    57467 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_8692.svg
--rw-r--r--   0 engun      (501) staff       (20)    40610 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_9236.svg
--rw-r--r--   0 engun      (501) staff       (20)    30809 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_9434.svg
--rw-r--r--   0 engun      (501) staff       (20)    39081 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_9552.svg
--rw-r--r--   0 engun      (501) staff       (20)    39339 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_9685.svg
--rw-r--r--   0 engun      (501) staff       (20)     1799 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/tech_notes/rss_cost.rst
--rw-r--r--   0 engun      (501) staff       (20)      174 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/docs/source/technical_notes.rst
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.272526 pymemtrace-0.1.4/pymemtrace/
--rw-r--r--   0 engun      (501) staff       (20)      151 2022-03-19 09:12:15.000000 pymemtrace-0.1.4/pymemtrace/__init__.py
--rw-r--r--   0 engun      (501) staff       (20)    30319 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/debug_malloc_stats.py
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.295202 pymemtrace-0.1.4/pymemtrace/examples/
--rw-r--r--   0 engun      (501) staff       (20)        0 2020-11-09 16:31:52.000000 pymemtrace-0.1.4/pymemtrace/examples/__init__.py
--rw-r--r--   0 engun      (501) staff       (20)     1641 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/examples/ex_cPyMemTrace.py
--rw-r--r--   0 engun      (501) staff       (20)     7152 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/examples/ex_debug_malloc_stats.py
--rw-r--r--   0 engun      (501) staff       (20)     3685 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/examples/ex_dtrace.py
--rw-r--r--   0 engun      (501) staff       (20)     3510 2020-11-11 14:53:24.000000 pymemtrace-0.1.4/pymemtrace/examples/ex_memory_exercise.py
--rw-r--r--   0 engun      (501) staff       (20)     1028 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/examples/ex_process.py
--rw-r--r--   0 engun      (501) staff       (20)     7094 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/examples/ex_trace_malloc.py
--rw-r--r--   0 engun      (501) staff       (20)      519 2020-11-09 16:31:52.000000 pymemtrace-0.1.4/pymemtrace/examples/example.py
--rw-r--r--   0 engun      (501) staff       (20)     3952 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/parse_dtrace_output.py
--rw-r--r--   0 engun      (501) staff       (20)    14196 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/process.py
--rw-r--r--   0 engun      (501) staff       (20)     3488 2020-11-09 16:31:52.000000 pymemtrace-0.1.4/pymemtrace/redirect_stdout.py
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.189999 pymemtrace-0.1.4/pymemtrace/src/
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.295940 pymemtrace-0.1.4/pymemtrace/src/c/
--rw-r--r--   0 engun      (501) staff       (20)     5246 2022-03-18 16:25:32.000000 pymemtrace-0.1.4/pymemtrace/src/c/get_rss.c
--rw-r--r--   0 engun      (501) staff       (20)      964 2022-03-19 09:10:26.000000 pymemtrace-0.1.4/pymemtrace/src/c/pymemtrace_util.c
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.296763 pymemtrace-0.1.4/pymemtrace/src/cpy/
--rw-r--r--   0 engun      (501) staff       (20)     4985 2020-11-01 12:49:01.000000 pymemtrace-0.1.4/pymemtrace/src/cpy/cCustom.c
--rw-r--r--   0 engun      (501) staff       (20)    12226 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/src/cpy/cMemLeak.c
--rw-r--r--   0 engun      (501) staff       (20)    17170 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/src/cpy/cPyMemTrace.c
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.297524 pymemtrace-0.1.4/pymemtrace/src/include/
--rw-r--r--   0 engun      (501) staff       (20)      251 2020-11-03 12:59:19.000000 pymemtrace-0.1.4/pymemtrace/src/include/get_rss.h
--rw-r--r--   0 engun      (501) staff       (20)      231 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/src/include/pymemtrace_util.h
--rw-r--r--   0 engun      (501) staff       (20)     3751 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/pymemtrace/trace_malloc.py
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.274004 pymemtrace-0.1.4/pymemtrace.egg-info/
--rw-r--r--   0 engun      (501) staff       (20)     6993 2022-03-19 10:49:27.000000 pymemtrace-0.1.4/pymemtrace.egg-info/PKG-INFO
--rw-r--r--   0 engun      (501) staff       (20)     3819 2022-03-19 10:49:28.000000 pymemtrace-0.1.4/pymemtrace.egg-info/SOURCES.txt
--rw-r--r--   0 engun      (501) staff       (20)        1 2022-03-19 10:49:27.000000 pymemtrace-0.1.4/pymemtrace.egg-info/dependency_links.txt
--rw-r--r--   0 engun      (501) staff       (20)        1 2017-12-23 10:03:36.000000 pymemtrace-0.1.4/pymemtrace.egg-info/not-zip-safe
--rw-r--r--   0 engun      (501) staff       (20)        7 2022-03-19 10:49:27.000000 pymemtrace-0.1.4/pymemtrace.egg-info/requires.txt
--rw-r--r--   0 engun      (501) staff       (20)       17 2022-03-19 10:49:27.000000 pymemtrace-0.1.4/pymemtrace.egg-info/top_level.txt
--rw-r--r--   0 engun      (501) staff       (20)      407 2022-03-19 10:49:28.300149 pymemtrace-0.1.4/setup.cfg
--rw-r--r--   0 engun      (501) staff       (20)     3821 2022-03-19 10:47:59.000000 pymemtrace-0.1.4/setup.py
-drwxr-xr-x   0 engun      (501) staff       (20)        0 2022-03-19 10:49:28.299227 pymemtrace-0.1.4/tests/
--rw-r--r--   0 engun      (501) staff       (20)       65 2017-12-04 13:28:23.000000 pymemtrace-0.1.4/tests/__init__.py
--rw-r--r--   0 engun      (501) staff       (20)     1925 2020-11-09 16:31:52.000000 pymemtrace-0.1.4/tests/_test_redirect_stdout.py
--rw-r--r--   0 engun      (501) staff       (20)      151 2020-11-20 09:57:02.000000 pymemtrace-0.1.4/tests/test_cMemLeak.py
--rw-r--r--   0 engun      (501) staff       (20)    22503 2020-11-11 14:53:24.000000 pymemtrace-0.1.4/tests/test_debug_malloc_stats.py
--rw-r--r--   0 engun      (501) staff       (20)     8845 2020-11-09 16:31:52.000000 pymemtrace-0.1.4/tests/test_process.py
--rw-r--r--   0 engun      (501) staff       (20)    12868 2017-12-13 09:04:19.000000 pymemtrace-0.1.4/tests/test_settrace.py
--rw-r--r--   0 engun      (501) staff       (20)      610 2022-03-17 21:13:49.000000 pymemtrace-0.1.4/tests/test_trace_malloc.py
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.589478 pymemtrace-0.1.5/
+-rw-r--r--   0 engun      (501) staff       (20)      146 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/AUTHORS.rst
+-rw-r--r--   0 engun      (501) staff       (20)     3250 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 engun      (501) staff       (20)      896 2023-06-21 12:04:41.000000 pymemtrace-0.1.5/HISTORY.rst
+-rw-r--r--   0 engun      (501) staff       (20)     1065 2017-12-04 13:23:31.000000 pymemtrace-0.1.5/LICENSE
+-rw-r--r--   0 engun      (501) staff       (20)      298 2022-03-17 09:41:31.000000 pymemtrace-0.1.5/MANIFEST.in
+-rw-r--r--   0 engun      (501) staff       (20)     7167 2023-06-21 12:12:26.589591 pymemtrace-0.1.5/PKG-INFO
+-rw-r--r--   0 engun      (501) staff       (20)     5314 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/README.rst
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.522465 pymemtrace-0.1.5/docs/
+-rw-r--r--   0 engun      (501) staff       (20)     6783 2018-01-18 10:19:00.000000 pymemtrace-0.1.5/docs/Makefile
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.516799 pymemtrace-0.1.5/docs/_build/
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.517041 pymemtrace-0.1.5/docs/_build/html/
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.532622 pymemtrace-0.1.5/docs/_build/html/_images/
+-rw-r--r--   0 engun      (501) staff       (20)    57321 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_20328.svg
+-rw-r--r--   0 engun      (501) staff       (20)    33545 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_3938.svg
+-rw-r--r--   0 engun      (501) staff       (20)   203722 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_4147.svg
+-rw-r--r--   0 engun      (501) staff       (20)    30456 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_76753.svg
+-rw-r--r--   0 engun      (501) staff       (20)    26786 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_77077.svg
+-rw-r--r--   0 engun      (501) staff       (20)   186964 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_77633.svg
+-rw-r--r--   0 engun      (501) staff       (20)    34351 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_8631.svg
+-rw-r--r--   0 engun      (501) staff       (20)    57467 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_8692.svg
+-rw-r--r--   0 engun      (501) staff       (20)    40610 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_9236.svg
+-rw-r--r--   0 engun      (501) staff       (20)    30809 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_9434.svg
+-rw-r--r--   0 engun      (501) staff       (20)    39081 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_9552.svg
+-rw-r--r--   0 engun      (501) staff       (20)    39339 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_9685.svg
+-rw-r--r--   0 engun      (501) staff       (20)    32943 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/_build/html/_images/process.log_14129.svg
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.538296 pymemtrace-0.1.5/docs/_build/html/_static/
+-rw-r--r--   0 engun      (501) staff       (20)      673 2020-10-31 12:33:19.000000 pymemtrace-0.1.5/docs/_build/html/_static/ajax-loader.gif
+-rw-r--r--   0 engun      (501) staff       (20)     3500 2020-10-31 12:33:19.000000 pymemtrace-0.1.5/docs/_build/html/_static/comment-bright.png
+-rw-r--r--   0 engun      (501) staff       (20)     3578 2020-10-31 12:33:19.000000 pymemtrace-0.1.5/docs/_build/html/_static/comment-close.png
+-rw-r--r--   0 engun      (501) staff       (20)     3445 2020-10-31 12:33:19.000000 pymemtrace-0.1.5/docs/_build/html/_static/comment.png
+-rw-r--r--   0 engun      (501) staff       (20)      347 2020-10-31 12:33:19.000000 pymemtrace-0.1.5/docs/_build/html/_static/down-pressed.png
+-rw-r--r--   0 engun      (501) staff       (20)      347 2020-10-31 12:33:19.000000 pymemtrace-0.1.5/docs/_build/html/_static/down.png
+-rw-r--r--   0 engun      (501) staff       (20)      286 2020-11-09 16:32:13.000000 pymemtrace-0.1.5/docs/_build/html/_static/file.png
+-rw-r--r--   0 engun      (501) staff       (20)       90 2020-11-09 16:32:13.000000 pymemtrace-0.1.5/docs/_build/html/_static/minus.png
+-rw-r--r--   0 engun      (501) staff       (20)       90 2020-11-09 16:32:13.000000 pymemtrace-0.1.5/docs/_build/html/_static/plus.png
+-rw-r--r--   0 engun      (501) staff       (20)      345 2020-10-31 12:33:19.000000 pymemtrace-0.1.5/docs/_build/html/_static/up-pressed.png
+-rw-r--r--   0 engun      (501) staff       (20)      345 2020-10-31 12:33:19.000000 pymemtrace-0.1.5/docs/_build/html/_static/up.png
+-rw-r--r--   0 engun      (501) staff       (20)     6467 2017-12-04 13:28:23.000000 pymemtrace-0.1.5/docs/make.bat
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.543867 pymemtrace-0.1.5/docs/source/
+-rw-r--r--   0 engun      (501) staff       (20)       31 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/authors.rst
+-rwxr-xr-x   0 engun      (501) staff       (20)     8762 2023-06-21 12:03:47.000000 pymemtrace-0.1.5/docs/source/conf.py
+-rw-r--r--   0 engun      (501) staff       (20)       36 2020-11-11 14:53:24.000000 pymemtrace-0.1.5/docs/source/contributing.rst
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.565472 pymemtrace-0.1.5/docs/source/examples/
+-rw-r--r--   0 engun      (501) staff       (20)     5431 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/examples/c_py_mem_trace.rst
+-rw-r--r--   0 engun      (501) staff       (20)     4514 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/examples/debug_malloc_stats.rst
+-rw-r--r--   0 engun      (501) staff       (20)    40512 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/examples/dtrace.rst
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.565940 pymemtrace-0.1.5/docs/source/examples/images/
+-rw-r--r--   0 engun      (501) staff       (20)    32943 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/examples/images/process.log_14129.svg
+-rw-r--r--   0 engun      (501) staff       (20)     8532 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/examples/process.rst
+-rw-r--r--   0 engun      (501) staff       (20)     7986 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/examples/trace_malloc.rst
+-rw-r--r--   0 engun      (501) staff       (20)      219 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/examples.rst
+-rw-r--r--   0 engun      (501) staff       (20)       31 2020-11-11 14:53:24.000000 pymemtrace-0.1.5/docs/source/history.rst
+-rw-r--r--   0 engun      (501) staff       (20)      374 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/index.rst
+-rw-r--r--   0 engun      (501) staff       (20)     1202 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/installation.rst
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.567247 pymemtrace-0.1.5/docs/source/memory_leaks/
+-rw-r--r--   0 engun      (501) staff       (20)    11560 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/memory_leaks/introduction.rst
+-rw-r--r--   0 engun      (501) staff       (20)     2416 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/memory_leaks/techniques.rst
+-rw-r--r--   0 engun      (501) staff       (20)     9777 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/memory_leaks/tools.rst
+-rw-r--r--   0 engun      (501) staff       (20)      205 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/memory_leaks.rst
+-rw-r--r--   0 engun      (501) staff       (20)       30 2020-11-11 14:53:24.000000 pymemtrace-0.1.5/docs/source/readme.rst
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.569730 pymemtrace-0.1.5/docs/source/ref/
+-rw-r--r--   0 engun      (501) staff       (20)      789 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/ref/c_mem_leak.rst
+-rw-r--r--   0 engun      (501) staff       (20)      610 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/ref/c_py_mem_trace.rst
+-rw-r--r--   0 engun      (501) staff       (20)      191 2020-11-11 14:53:24.000000 pymemtrace-0.1.5/docs/source/ref/debug_malloc_stats.rst
+-rw-r--r--   0 engun      (501) staff       (20)      151 2020-11-11 14:53:24.000000 pymemtrace-0.1.5/docs/source/ref/process.rst
+-rw-r--r--   0 engun      (501) staff       (20)      185 2020-11-11 14:53:24.000000 pymemtrace-0.1.5/docs/source/ref/redirect_stdout.rst
+-rw-r--r--   0 engun      (501) staff       (20)      256 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/ref/trace_malloc.rst
+-rw-r--r--   0 engun      (501) staff       (20)      233 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/reference.rst
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.570852 pymemtrace-0.1.5/docs/source/tech_notes/
+-rw-r--r--   0 engun      (501) staff       (20)    23952 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/cPyMemTrace.rst
+-rw-r--r--   0 engun      (501) staff       (20)     9117 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/dtrace.rst
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.580040 pymemtrace-0.1.5/docs/source/tech_notes/images/
+-rw-r--r--   0 engun      (501) staff       (20)    57321 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_20328.svg
+-rw-r--r--   0 engun      (501) staff       (20)    33545 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_3938.svg
+-rw-r--r--   0 engun      (501) staff       (20)   203722 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_4147.svg
+-rw-r--r--   0 engun      (501) staff       (20)    30456 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_76753.svg
+-rw-r--r--   0 engun      (501) staff       (20)    26786 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_77077.svg
+-rw-r--r--   0 engun      (501) staff       (20)   186964 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_77633.svg
+-rw-r--r--   0 engun      (501) staff       (20)    34351 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_8631.svg
+-rw-r--r--   0 engun      (501) staff       (20)    57467 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_8692.svg
+-rw-r--r--   0 engun      (501) staff       (20)    40610 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_9236.svg
+-rw-r--r--   0 engun      (501) staff       (20)    30809 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_9434.svg
+-rw-r--r--   0 engun      (501) staff       (20)    39081 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_9552.svg
+-rw-r--r--   0 engun      (501) staff       (20)    39339 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_9685.svg
+-rw-r--r--   0 engun      (501) staff       (20)     1799 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/tech_notes/rss_cost.rst
+-rw-r--r--   0 engun      (501) staff       (20)      174 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/docs/source/technical_notes.rst
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.582378 pymemtrace-0.1.5/pymemtrace/
+-rw-r--r--   0 engun      (501) staff       (20)      151 2023-06-21 12:03:47.000000 pymemtrace-0.1.5/pymemtrace/__init__.py
+-rw-r--r--   0 engun      (501) staff       (20)    30319 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/pymemtrace/debug_malloc_stats.py
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.585959 pymemtrace-0.1.5/pymemtrace/examples/
+-rw-r--r--   0 engun      (501) staff       (20)        0 2020-11-09 16:31:52.000000 pymemtrace-0.1.5/pymemtrace/examples/__init__.py
+-rw-r--r--   0 engun      (501) staff       (20)     1641 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/pymemtrace/examples/ex_cPyMemTrace.py
+-rw-r--r--   0 engun      (501) staff       (20)     7152 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/pymemtrace/examples/ex_debug_malloc_stats.py
+-rw-r--r--   0 engun      (501) staff       (20)     3685 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/pymemtrace/examples/ex_dtrace.py
+-rw-r--r--   0 engun      (501) staff       (20)     3510 2020-11-11 14:53:24.000000 pymemtrace-0.1.5/pymemtrace/examples/ex_memory_exercise.py
+-rw-r--r--   0 engun      (501) staff       (20)     1028 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/pymemtrace/examples/ex_process.py
+-rw-r--r--   0 engun      (501) staff       (20)     7094 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/pymemtrace/examples/ex_trace_malloc.py
+-rw-r--r--   0 engun      (501) staff       (20)      519 2020-11-09 16:31:52.000000 pymemtrace-0.1.5/pymemtrace/examples/example.py
+-rw-r--r--   0 engun      (501) staff       (20)     3952 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/pymemtrace/parse_dtrace_output.py
+-rw-r--r--   0 engun      (501) staff       (20)    14196 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/pymemtrace/process.py
+-rw-r--r--   0 engun      (501) staff       (20)     3488 2020-11-09 16:31:52.000000 pymemtrace-0.1.5/pymemtrace/redirect_stdout.py
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.518633 pymemtrace-0.1.5/pymemtrace/src/
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.586476 pymemtrace-0.1.5/pymemtrace/src/c/
+-rw-r--r--   0 engun      (501) staff       (20)     5246 2022-03-18 16:25:32.000000 pymemtrace-0.1.5/pymemtrace/src/c/get_rss.c
+-rw-r--r--   0 engun      (501) staff       (20)      964 2022-03-19 09:10:26.000000 pymemtrace-0.1.5/pymemtrace/src/c/pymemtrace_util.c
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.587211 pymemtrace-0.1.5/pymemtrace/src/cpy/
+-rw-r--r--   0 engun      (501) staff       (20)     4985 2020-11-01 12:49:01.000000 pymemtrace-0.1.5/pymemtrace/src/cpy/cCustom.c
+-rw-r--r--   0 engun      (501) staff       (20)    12226 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/pymemtrace/src/cpy/cMemLeak.c
+-rw-r--r--   0 engun      (501) staff       (20)    17681 2023-06-21 12:08:59.000000 pymemtrace-0.1.5/pymemtrace/src/cpy/cPyMemTrace.c
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.587682 pymemtrace-0.1.5/pymemtrace/src/include/
+-rw-r--r--   0 engun      (501) staff       (20)      251 2020-11-03 12:59:19.000000 pymemtrace-0.1.5/pymemtrace/src/include/get_rss.h
+-rw-r--r--   0 engun      (501) staff       (20)      231 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/pymemtrace/src/include/pymemtrace_util.h
+-rw-r--r--   0 engun      (501) staff       (20)     3751 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/pymemtrace/trace_malloc.py
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.584028 pymemtrace-0.1.5/pymemtrace.egg-info/
+-rw-r--r--   0 engun      (501) staff       (20)     7167 2023-06-21 12:12:26.000000 pymemtrace-0.1.5/pymemtrace.egg-info/PKG-INFO
+-rw-r--r--   0 engun      (501) staff       (20)     3819 2023-06-21 12:12:26.000000 pymemtrace-0.1.5/pymemtrace.egg-info/SOURCES.txt
+-rw-r--r--   0 engun      (501) staff       (20)        1 2023-06-21 12:12:26.000000 pymemtrace-0.1.5/pymemtrace.egg-info/dependency_links.txt
+-rw-r--r--   0 engun      (501) staff       (20)        1 2017-12-23 10:03:36.000000 pymemtrace-0.1.5/pymemtrace.egg-info/not-zip-safe
+-rw-r--r--   0 engun      (501) staff       (20)        7 2023-06-21 12:12:26.000000 pymemtrace-0.1.5/pymemtrace.egg-info/requires.txt
+-rw-r--r--   0 engun      (501) staff       (20)       17 2023-06-21 12:12:26.000000 pymemtrace-0.1.5/pymemtrace.egg-info/top_level.txt
+-rw-r--r--   0 engun      (501) staff       (20)      407 2023-06-21 12:12:26.590038 pymemtrace-0.1.5/setup.cfg
+-rw-r--r--   0 engun      (501) staff       (20)     3872 2023-06-21 12:03:47.000000 pymemtrace-0.1.5/setup.py
+drwxr-xr-x   0 engun      (501) staff       (20)        0 2023-06-21 12:12:26.589300 pymemtrace-0.1.5/tests/
+-rw-r--r--   0 engun      (501) staff       (20)       65 2017-12-04 13:28:23.000000 pymemtrace-0.1.5/tests/__init__.py
+-rw-r--r--   0 engun      (501) staff       (20)     1925 2020-11-09 16:31:52.000000 pymemtrace-0.1.5/tests/_test_redirect_stdout.py
+-rw-r--r--   0 engun      (501) staff       (20)      151 2020-11-20 09:57:02.000000 pymemtrace-0.1.5/tests/test_cMemLeak.py
+-rw-r--r--   0 engun      (501) staff       (20)    22503 2020-11-11 14:53:24.000000 pymemtrace-0.1.5/tests/test_debug_malloc_stats.py
+-rw-r--r--   0 engun      (501) staff       (20)     8845 2020-11-09 16:31:52.000000 pymemtrace-0.1.5/tests/test_process.py
+-rw-r--r--   0 engun      (501) staff       (20)    13376 2023-06-21 11:49:49.000000 pymemtrace-0.1.5/tests/test_settrace.py
+-rw-r--r--   0 engun      (501) staff       (20)      766 2023-06-21 11:15:43.000000 pymemtrace-0.1.5/tests/test_trace_malloc.py
```

### Comparing `pymemtrace-0.1.4/CONTRIBUTING.rst` & `pymemtrace-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/HISTORY.rst` & `pymemtrace-0.1.5/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+0.1.5 (2023-06-21)
+------------------
+
+* Add support for Python versions 3.10, 3.11. Now supports Python versions 3.7, 3.8, 3.9, 3.10, 3.11.
+
 0.1.4 (2022-03-19)
 ------------------
 
 * Fix Linux build.
 
 0.1.3 (2022-03-17)
 ------------------
```

### Comparing `pymemtrace-0.1.4/LICENSE` & `pymemtrace-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/PKG-INFO` & `pymemtrace-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pymemtrace
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python memory tracing.
 Home-page: https://github.com/paulross/pymemtrace
 Author: Paul Ross
 Author-email: apaulross@gmail.com
 License: MIT license
 Keywords: pymemtrace
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 *******************
 Introduction
@@ -151,14 +151,19 @@
 
 
 
 =======
 History
 =======
 
+0.1.5 (2023-06-21)
+------------------
+
+* Add support for Python versions 3.10, 3.11. Now supports Python versions 3.7, 3.8, 3.9, 3.10, 3.11.
+
 0.1.4 (2022-03-19)
 ------------------
 
 * Fix Linux build.
 
 0.1.3 (2022-03-17)
 ------------------
@@ -182,9 +187,7 @@
 * Includes extensive documentation and performance measurement.
 * First release on PyPI.
 
 0.1.0 (2017-12-04)
 ------------------
 
 * Initial idea and implementation, never released.
-
-
```

### Comparing `pymemtrace-0.1.4/README.rst` & `pymemtrace-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/Makefile` & `pymemtrace-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_20328.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_20328.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_3938.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_3938.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_4147.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_4147.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_76753.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_76753.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_77077.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_77077.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_77633.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_77633.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_8631.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_8631.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_8692.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_8692.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_9236.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_9236.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_9434.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_9434.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_9552.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_9552.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/LASToHTML.log_9685.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/LASToHTML.log_9685.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_images/process.log_14129.svg` & `pymemtrace-0.1.5/docs/_build/html/_images/process.log_14129.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_static/ajax-loader.gif` & `pymemtrace-0.1.5/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_static/comment-bright.png` & `pymemtrace-0.1.5/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_static/comment-close.png` & `pymemtrace-0.1.5/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/_build/html/_static/comment.png` & `pymemtrace-0.1.5/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/make.bat` & `pymemtrace-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/conf.py` & `pymemtrace-0.1.5/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'pymemtrace'
-copyright = u"2017-2022, Paul Ross"
+copyright = u"2017-2023, Paul Ross"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = pymemtrace.__version__
```

### Comparing `pymemtrace-0.1.4/docs/source/examples/c_py_mem_trace.rst` & `pymemtrace-0.1.5/docs/source/examples/c_py_mem_trace.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/examples/debug_malloc_stats.rst` & `pymemtrace-0.1.5/docs/source/examples/debug_malloc_stats.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/examples/dtrace.rst` & `pymemtrace-0.1.5/docs/source/examples/dtrace.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/examples/images/process.log_14129.svg` & `pymemtrace-0.1.5/docs/source/examples/images/process.log_14129.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/examples/process.rst` & `pymemtrace-0.1.5/docs/source/examples/process.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/examples/trace_malloc.rst` & `pymemtrace-0.1.5/docs/source/examples/trace_malloc.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/installation.rst` & `pymemtrace-0.1.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/memory_leaks/introduction.rst` & `pymemtrace-0.1.5/docs/source/memory_leaks/introduction.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/memory_leaks/techniques.rst` & `pymemtrace-0.1.5/docs/source/memory_leaks/techniques.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/memory_leaks/tools.rst` & `pymemtrace-0.1.5/docs/source/memory_leaks/tools.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/ref/c_mem_leak.rst` & `pymemtrace-0.1.5/docs/source/ref/c_mem_leak.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/ref/c_py_mem_trace.rst` & `pymemtrace-0.1.5/docs/source/ref/c_py_mem_trace.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/cPyMemTrace.rst` & `pymemtrace-0.1.5/docs/source/tech_notes/cPyMemTrace.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/dtrace.rst` & `pymemtrace-0.1.5/docs/source/tech_notes/dtrace.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_20328.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_20328.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_3938.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_3938.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_4147.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_4147.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_76753.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_76753.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_77077.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_77077.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_77633.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_77633.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_8631.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_8631.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_8692.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_8692.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_9236.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_9236.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_9434.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_9434.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_9552.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_9552.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/images/LASToHTML.log_9685.svg` & `pymemtrace-0.1.5/docs/source/tech_notes/images/LASToHTML.log_9685.svg`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/docs/source/tech_notes/rss_cost.rst` & `pymemtrace-0.1.5/docs/source/tech_notes/rss_cost.rst`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/debug_malloc_stats.py` & `pymemtrace-0.1.5/pymemtrace/debug_malloc_stats.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/examples/ex_cPyMemTrace.py` & `pymemtrace-0.1.5/pymemtrace/examples/ex_cPyMemTrace.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/examples/ex_debug_malloc_stats.py` & `pymemtrace-0.1.5/pymemtrace/examples/ex_debug_malloc_stats.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/examples/ex_dtrace.py` & `pymemtrace-0.1.5/pymemtrace/examples/ex_dtrace.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/examples/ex_memory_exercise.py` & `pymemtrace-0.1.5/pymemtrace/examples/ex_memory_exercise.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/examples/ex_process.py` & `pymemtrace-0.1.5/pymemtrace/examples/ex_process.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/examples/ex_trace_malloc.py` & `pymemtrace-0.1.5/pymemtrace/examples/ex_trace_malloc.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/examples/example.py` & `pymemtrace-0.1.5/pymemtrace/examples/example.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/parse_dtrace_output.py` & `pymemtrace-0.1.5/pymemtrace/parse_dtrace_output.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/process.py` & `pymemtrace-0.1.5/pymemtrace/process.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/redirect_stdout.py` & `pymemtrace-0.1.5/pymemtrace/redirect_stdout.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/src/c/get_rss.c` & `pymemtrace-0.1.5/pymemtrace/src/c/get_rss.c`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/src/c/pymemtrace_util.c` & `pymemtrace-0.1.5/pymemtrace/src/c/pymemtrace_util.c`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/src/cpy/cCustom.c` & `pymemtrace-0.1.5/pymemtrace/src/cpy/cCustom.c`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/src/cpy/cMemLeak.c` & `pymemtrace-0.1.5/pymemtrace/src/cpy/cMemLeak.c`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace/src/cpy/cPyMemTrace.c` & `pymemtrace-0.1.5/pymemtrace/src/cpy/cPyMemTrace.c`

 * *Files 2% similar despite different names*

```diff
@@ -110,21 +110,31 @@
 static int
 trace_or_profile_function(PyObject *pobj, PyFrameObject *frame, int what, PyObject *arg) {
     assert(Py_TYPE(pobj) == &TraceFileWrapperType && "trace_wrapper is not a TraceFileWrapperType.");
 
     TraceFileWrapper *trace_wrapper = (TraceFileWrapper *)pobj;
     size_t rss = getCurrentRSS_alternate();
 #ifdef PY_MEM_TRACE_WRITE_OUTPUT
+#if PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION >= 11
+    /* See https://docs.python.org/3.11/whatsnew/3.11.html#pyframeobject-3-11-hiding */
+    const unsigned char *file_name = PyUnicode_1BYTE_DATA(PyFrame_GetCode(frame)->co_filename);
+#else
     const unsigned char *file_name = PyUnicode_1BYTE_DATA(frame->f_code->co_filename);
+#endif
     int line_number = PyFrame_GetLineNumber(frame);
     const char *func_name = NULL;
     if (what == PyTrace_C_CALL || what == PyTrace_C_EXCEPTION || what == PyTrace_C_RETURN) {
         func_name = PyEval_GetFuncName(arg);
     } else {
+#if PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION >= 11
+        /* See https://docs.python.org/3.11/whatsnew/3.11.html#pyframeobject-3-11-hiding */
+        func_name = (const char *)PyUnicode_1BYTE_DATA(PyFrame_GetCode(frame)->co_name);
+#else
         func_name = (const char *)PyUnicode_1BYTE_DATA(frame->f_code->co_name);
+#endif
     }
     long d_rss = rss - trace_wrapper->rss;
     if (labs(d_rss) >= trace_wrapper->d_rss_trigger
         && trace_wrapper->event_number > 0
         && (trace_wrapper->event_number - trace_wrapper->previous_event_number) > 1) {
         // Previous event.
 #ifdef PY_MEM_TRACE_WRITE_OUTPUT_PREV_NEXT
@@ -231,15 +241,15 @@
         Py_RETURN_NONE;
     }
     PyErr_SetString(PyExc_RuntimeError, "Could not attach profile function.");
     return NULL;
 }
 
 static PyObject *
-py_detach_profile_function() {
+py_detach_profile_function(void) {
     if (profile_wrapper) {
         TraceFileWrapper_dealloc(profile_wrapper);
         profile_wrapper = NULL;
     }
     PyEval_SetProfile(NULL, NULL);
     Py_RETURN_NONE;
 }
@@ -252,30 +262,30 @@
         Py_RETURN_NONE;
     }
     PyErr_SetString(PyExc_RuntimeError, "Could not attach trace function.");
     return NULL;
 }
 
 static PyObject *
-py_detach_trace_function() {
+py_detach_trace_function(void) {
     if (trace_wrapper) {
         TraceFileWrapper_dealloc(trace_wrapper);
         trace_wrapper = NULL;
     }
     PyEval_SetTrace(NULL, NULL);
     Py_RETURN_NONE;
 }
 
 static PyObject *
-py_rss() {
+py_rss(void) {
     return PyLong_FromSize_t(getCurrentRSS_alternate());
 }
 
 static PyObject *
-py_rss_peak() {
+py_rss_peak(void) {
     return PyLong_FromSize_t(getPeakRSS());
 }
 
 static PyMethodDef cPyMemTraceMethods[] = {
     {"rss",   (PyCFunction) py_rss, METH_NOARGS, "Return the current RSS in bytes."},
     {"rss_peak",   (PyCFunction) py_rss_peak, METH_NOARGS, "Return the peak RSS in bytes."},
     {NULL, NULL, 0, NULL}        /* Sentinel */
```

### Comparing `pymemtrace-0.1.4/pymemtrace/trace_malloc.py` & `pymemtrace-0.1.5/pymemtrace/trace_malloc.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/pymemtrace.egg-info/PKG-INFO` & `pymemtrace-0.1.5/pymemtrace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pymemtrace
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python memory tracing.
 Home-page: https://github.com/paulross/pymemtrace
 Author: Paul Ross
 Author-email: apaulross@gmail.com
 License: MIT license
 Keywords: pymemtrace
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 *******************
 Introduction
@@ -151,14 +151,19 @@
 
 
 
 =======
 History
 =======
 
+0.1.5 (2023-06-21)
+------------------
+
+* Add support for Python versions 3.10, 3.11. Now supports Python versions 3.7, 3.8, 3.9, 3.10, 3.11.
+
 0.1.4 (2022-03-19)
 ------------------
 
 * Fix Linux build.
 
 0.1.3 (2022-03-17)
 ------------------
@@ -182,9 +187,7 @@
 * Includes extensive documentation and performance measurement.
 * First release on PyPI.
 
 0.1.0 (2017-12-04)
 ------------------
 
 * Initial idea and implementation, never released.
-
-
```

### Comparing `pymemtrace-0.1.4/pymemtrace.egg-info/SOURCES.txt` & `pymemtrace-0.1.5/pymemtrace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/setup.py` & `pymemtrace-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 if DEBUG:
     extra_compile_args.extend(['-g3', '-O0', '-DDEBUG=1', '-UNDEBUG'])
 else:
     extra_compile_args.extend(['-O3', '-UDEBUG', '-DNDEBUG'])
 
 setup(
     name='pymemtrace',
-    version='0.1.4',
+    version='0.1.5',
     description="Python memory tracing.",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/x-rst',
     author="Paul Ross",
     author_email='apaulross@gmail.com',
     url='https://github.com/paulross/pymemtrace',
     packages=find_packages(),  # include=['pymemtrace']),
@@ -78,18 +78,19 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: C',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development',
     ],
     test_suite='tests',
     tests_require=test_requirements,
     setup_requires=setup_requirements,
     # Extensions
     ext_modules=[
```

### Comparing `pymemtrace-0.1.4/tests/_test_redirect_stdout.py` & `pymemtrace-0.1.5/tests/_test_redirect_stdout.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/tests/test_debug_malloc_stats.py` & `pymemtrace-0.1.5/tests/test_debug_malloc_stats.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/tests/test_process.py` & `pymemtrace-0.1.5/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `pymemtrace-0.1.4/tests/test_settrace.py` & `pymemtrace-0.1.5/tests/test_settrace.py`

 * *Files 7% similar despite different names*

```diff
@@ -301,15 +301,19 @@
             results.append(v)
         assert results == [0, 2, 4]
     if TRACE_TO_STDOUT:
         print()
 #         pprint.pprint(rte.records)
         print(rte)
         print('Code line numbers:', sorted(set([r.lineno_code for r in rte.records])))
-    assert len(rte.records) == 17
+    assert sys.version_info.major == 3
+    if sys.version_info.minor < 10:
+        assert len(rte.records) == 17
+    else:
+        assert len(rte.records) == 16
 
 def test_generator_grandparent_parent_child():
     def child_generator(n):
         for i in range(n):
             yield i
 
     def parent_generator(n):
@@ -327,15 +331,19 @@
             results.append(v)
         assert results == [0, 4, 8]
     if TRACE_TO_STDOUT:
         print()
 #         pprint.pprint(rte.records)
         print(rte)
         print('Code line numbers:', sorted(set([r.lineno_code for r in rte.records])))
-    assert len(rte.records) == 26
+    assert sys.version_info.major == 3
+    if sys.version_info.minor < 10:
+        assert len(rte.records) == 26
+    else:
+        assert len(rte.records) == 24
 
 def test_generator_class_different_named_methods():
     class ChildGenerator:
         def child_generate(self, n):
             yield n
             yield n * 2
             yield n * 4
@@ -354,15 +362,19 @@
             results.append(v)
         assert results == [9, 18, 36]
     if TRACE_TO_STDOUT:
         print()
 #         pprint.pprint(rte.records)
         print(rte)
         print('Code line numbers:', sorted(set([r.lineno_code for r in rte.records])))
-    assert len(rte.records) == 17
+    assert sys.version_info.major == 3
+    if sys.version_info.minor < 10:
+        assert len(rte.records) == 17
+    else:
+        assert len(rte.records) == 16
 
 def test_generator_class_same_named_methods():
     class ChildGenerator:
         def generate(self, n):
             yield n
             yield n * 2
             yield n * 4
@@ -381,8 +393,12 @@
             results.append(v)
         assert results == [9, 18, 36]
     if TRACE_TO_STDOUT:
         print()
 #         pprint.pprint(rte.records)
         print(rte)
         print('Code line numbers:', sorted(set([r.lineno_code for r in rte.records])))
-    assert len(rte.records) == 17
+    assert sys.version_info.major == 3
+    if sys.version_info.minor < 10:
+        assert len(rte.records) == 17
+    else:
+        assert len(rte.records) == 16
```

### Comparing `pymemtrace-0.1.4/tests/test_trace_malloc.py` & `pymemtrace-0.1.5/tests/test_trace_malloc.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 
 
 def test_trace_malloc_simple():
     list_of_strings = []
     # with trace_malloc.TraceMalloc('filename') as tm:
     with trace_malloc.TraceMalloc('lineno') as tm:
         list_of_strings.append(' ' * 1024)
-    print(f'tm.memory_start={tm.memory_start}')
-    print(f'tm.memory_finish={tm.memory_finish}')
+    # print()
+    # print(f'tm.memory_start={tm.memory_start}')
+    # print(f'tm.memory_finish={tm.memory_finish}')
+    # print(f'tm.net_statistics(): {tm.net_statistics()}')
     # for stat in tm.net_statistics():
     #     print(stat)
     # assert tm.diff == 0, f'tm.diff={tm.diff}'
-    assert len(tm.net_statistics()) in (3, 5, 6,)
+    # Different versions of Python will have a different number of entries.
+    assert len(tm.net_statistics()) in (3, 4, 5, 6,)
     assert len(tm.statistics) > 3
 
 
 if __name__ == '__main__':
     test_trace_malloc_simple()
```

