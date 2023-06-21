# Comparing `tmp/nismod-snail-0.3.1.tar.gz` & `tmp/nismod-snail-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nismod-snail-0.3.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "nismod-snail-0.3.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `nismod-snail-0.3.1.tar` & `nismod-snail-0.3.2.tar`

### file list

```diff
@@ -1,469 +1,469 @@
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/.clang-format
--rw-r--r--   0        0        0      233 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/.environment.yml
--rw-r--r--   0        0        0     2170 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     1497 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1448 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/.github/workflows/package.yml
--rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/.gitignore
--rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/.gitmodules
--rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/CMakeLists.txt
--rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/LICENSE
--rw-r--r--   0        0        0     5877 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/README.md
--rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/docs/Makefile
--rw-r--r--   0        0        0      473 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/docs/source/_static/theme_tweaks.css
--rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/docs/source/api/modules.rst
--rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/docs/source/api/snail.core.rst
--rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/docs/source/api/snail.rst
--rw-r--r--   0        0        0     1444 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/docs/source/conf.py
--rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/docs/source/getting_started.md
--rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/docs/source/index.rst
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/docs/source/license.rst
--rw-r--r--   0        0        0     1550 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/examples.sh
--rw-r--r--   0        0        0      429 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/CMakeLists.txt
--rw-r--r--   0        0        0      628 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.clang-format
--rw-r--r--   0        0        0     3044 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.conan/build.py
--rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.conan/test_package/CMakeLists.txt
--rw-r--r--   0        0        0      551 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.conan/test_package/conanfile.py
--rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.conan/test_package/test_package.cpp
--rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.gitattributes
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.github/FUNDING.yml
--rw-r--r--   0        0        0      711 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      308 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.github/pull_request_template.md
--rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.gitignore
--rw-r--r--   0        0        0     8343 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/.travis.yml
--rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/BUILD.bazel
--rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/CMake/Catch2Config.cmake.in
--rw-r--r--   0        0        0     5086 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/CMake/FindGcov.cmake
--rw-r--r--   0        0        0    12328 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/CMake/FindLcov.cmake
--rw-r--r--   0        0        0     8419 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/CMake/Findcodecov.cmake
--rw-r--r--   0        0        0     1226 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/CMake/MiscFunctions.cmake
--rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/CMake/catch2.pc.in
--rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/CMake/llvm-cov-wrapper
--rw-r--r--   0        0        0     7737 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/CMakeLists.txt
--rw-r--r--   0        0        0     3215 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/LICENSE.txt
--rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/README.md
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/WORKSPACE
--rw-r--r--   0        0        0     2702 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/appveyor.yml
--rw-r--r--   0        0        0    10636 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/artwork/catch2-c-logo.png
--rw-r--r--   0        0        0    33761 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/artwork/catch2-hand-logo.png
--rw-r--r--   0        0        0    20939 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/artwork/catch2-logo-small.png
--rw-r--r--   0        0        0      438 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/codecov.yml
--rw-r--r--   0        0        0     1006 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/conanfile.py
--rw-r--r--   0        0        0     8574 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/contrib/Catch.cmake
--rw-r--r--   0        0        0     3942 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/contrib/CatchAddTests.cmake
--rw-r--r--   0        0        0    15008 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/contrib/ParseAndAddCatchTests.cmake
--rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/contrib/gdbinit
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/contrib/lldbinit
--rw-r--r--   0        0        0     1325 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/Readme.md
--rw-r--r--   0        0        0     8308 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/assertions.md
--rw-r--r--   0        0        0    11499 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/benchmarks.md
--rw-r--r--   0        0        0     5466 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/ci-and-misc.md
--rw-r--r--   0        0        0     9757 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/cmake-integration.md
--rw-r--r--   0        0        0    20867 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/command-line.md
--rw-r--r--   0        0        0     1064 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/commercial-users.md
--rw-r--r--   0        0        0    14426 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/configuration.md
--rw-r--r--   0        0        0     8881 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/contributing.md
--rw-r--r--   0        0        0     4887 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/deprecations.md
--rw-r--r--   0        0        0     2810 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/event-listeners.md
--rw-r--r--   0        0        0     8448 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/generators.md
--rw-r--r--   0        0        0     7211 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/limitations.md
--rw-r--r--   0        0        0     2939 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/list-of-examples.md
--rw-r--r--   0        0        0     4952 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/logging.md
--rw-r--r--   0        0        0     8097 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/matchers.md
--rw-r--r--   0        0        0     6026 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/opensource-users.md
--rw-r--r--   0        0        0     4014 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/other-macros.md
--rw-r--r--   0        0        0     4400 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/own-main.md
--rw-r--r--   0        0        0    56784 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/release-notes.md
--rw-r--r--   0        0        0     3326 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/release-process.md
--rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/reporters.md
--rw-r--r--   0        0        0     5020 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/slow-compiles.md
--rw-r--r--   0        0        0    13228 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/test-cases-and-sections.md
--rw-r--r--   0        0        0     5281 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/test-fixtures.md
--rw-r--r--   0        0        0     4775 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/tostring.md
--rw-r--r--   0        0        0    14790 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/tutorial.md
--rw-r--r--   0        0        0     2513 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/docs/why-catch.md
--rw-r--r--   0        0        0      488 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/000-CatchMain.cpp
--rw-r--r--   0        0        0     1323 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/010-TestCase.cpp
--rw-r--r--   0        0        0     1232 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/020-TestCase-1.cpp
--rw-r--r--   0        0        0     1168 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/020-TestCase-2.cpp
--rw-r--r--   0        0        0     2791 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/030-Asn-Require-Check.cpp
--rw-r--r--   0        0        0     2513 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/100-Fix-Section.cpp
--rw-r--r--   0        0        0     1963 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/110-Fix-ClassFixture.cpp
--rw-r--r--   0        0        0     3040 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/120-Bdd-ScenarioGivenWhenThen.cpp
--rw-r--r--   0        0        0      884 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/200-Rpt-CatchMain.cpp
--rw-r--r--   0        0        0     5701 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/207-Rpt-TeamCityReporter.cpp
--rw-r--r--   0        0        0    14789 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/210-Evt-EventListeners.cpp
--rw-r--r--   0        0        0     1443 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/231-Cfg-OutputStreams.cpp
--rw-r--r--   0        0        0     1965 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/300-Gen-OwnGenerator.cpp
--rw-r--r--   0        0        0     1887 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/301-Gen-MapTypeConversion.cpp
--rw-r--r--   0        0        0     2121 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/302-Gen-Table.cpp
--rw-r--r--   0        0        0     1230 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/310-Gen-VariablesInGenerators.cpp
--rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/311-Gen-CustomCapture.cpp
--rw-r--r--   0        0        0     5425 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/examples/CMakeLists.txt
--rw-r--r--   0        0        0    30046 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/catch.hpp
--rw-r--r--   0        0        0      462 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/catch_with_main.hpp
--rw-r--r--   0        0        0    40644 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/external/clara.hpp
--rw-r--r--   0        0        0     4850 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_benchmark.hpp
--rw-r--r--   0        0        0     1040 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_benchmarking_all.hpp
--rw-r--r--   0        0        0     2292 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_chronometer.hpp
--rw-r--r--   0        0        0     1123 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_clock.hpp
--rw-r--r--   0        0        0     2523 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_constructor.hpp
--rw-r--r--   0        0        0     1164 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_environment.hpp
--rw-r--r--   0        0        0      912 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_estimate.hpp
--rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_execution_plan.hpp
--rw-r--r--   0        0        0     2189 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_optimizer.hpp
--rw-r--r--   0        0        0      987 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_outlier_classification.hpp
--rw-r--r--   0        0        0     1575 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_sample_analysis.hpp
--rw-r--r--   0        0        0     3213 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_analyse.hpp
--rw-r--r--   0        0        0     4019 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_benchmark_function.hpp
--rw-r--r--   0        0        0     2517 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_complete_invoke.hpp
--rw-r--r--   0        0        0     5000 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_estimate_clock.hpp
--rw-r--r--   0        0        0     1132 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_measure.hpp
--rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_repeat.hpp
--rw-r--r--   0        0        0     2545 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_run_for_at_least.hpp
--rw-r--r--   0        0        0     8942 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_stats.cpp
--rw-r--r--   0        0        0     6541 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_stats.hpp
--rw-r--r--   0        0        0      977 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_timing.hpp
--rw-r--r--   0        0        0     2593 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_approx.cpp
--rw-r--r--   0        0        0     5044 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_approx.h
--rw-r--r--   0        0        0     4477 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_assertionhandler.cpp
--rw-r--r--   0        0        0     2714 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_assertionhandler.h
--rw-r--r--   0        0        0      910 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_assertioninfo.h
--rw-r--r--   0        0        0     3313 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_assertionresult.cpp
--rw-r--r--   0        0        0     1800 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_assertionresult.h
--rw-r--r--   0        0        0     7782 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_capture.hpp
--rw-r--r--   0        0        0     1035 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_capture_matchers.cpp
--rw-r--r--   0        0        0     3802 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_capture_matchers.h
--rw-r--r--   0        0        0     1275 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_clara.h
--rw-r--r--   0        0        0    10800 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_commandline.cpp
--rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_commandline.h
--rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_common.cpp
--rw-r--r--   0        0        0     3050 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_common.h
--rw-r--r--   0        0        0    15337 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_compiler_capabilities.h
--rw-r--r--   0        0        0     4161 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_config.cpp
--rw-r--r--   0        0        0     4300 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_config.hpp
--rw-r--r--   0        0        0     1292 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_config_uncaught_exceptions.hpp
--rw-r--r--   0        0        0     8558 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_console_colour.cpp
--rw-r--r--   0        0        0     1797 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_console_colour.h
--rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_context.cpp
--rw-r--r--   0        0        0     1748 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_context.h
--rw-r--r--   0        0        0     1035 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_debug_console.cpp
--rw-r--r--   0        0        0      461 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_debug_console.h
--rw-r--r--   0        0        0     4360 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_debugger.cpp
--rw-r--r--   0        0        0     2159 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_debugger.h
--rw-r--r--   0        0        0      807 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_decomposer.cpp
--rw-r--r--   0        0        0    10336 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_decomposer.h
--rw-r--r--   0        0        0     1238 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_default_main.hpp
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_enforce.cpp
--rw-r--r--   0        0        0     1549 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_enforce.h
--rw-r--r--   0        0        0     2716 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_enum_values_registry.cpp
--rw-r--r--   0        0        0     1055 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_enum_values_registry.h
--rw-r--r--   0        0        0      385 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_errno_guard.cpp
--rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_errno_guard.h
--rw-r--r--   0        0        0     3073 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_exception_translator_registry.cpp
--rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_exception_translator_registry.h
--rw-r--r--   0        0        0      752 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_external_interfaces.h
--rw-r--r--   0        0        0     8920 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_fatal_condition.cpp
--rw-r--r--   0        0        0     2231 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_fatal_condition.h
--rw-r--r--   0        0        0      827 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_generators.cpp
--rw-r--r--   0        0        0     7952 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_generators.hpp
--rw-r--r--   0        0        0     8492 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_generators_generic.hpp
--rw-r--r--   0        0        0     5193 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_generators_specific.hpp
--rw-r--r--   0        0        0      848 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_impl.hpp
--rw-r--r--   0        0        0      108 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_capture.cpp
--rw-r--r--   0        0        0     3656 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_capture.h
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_config.cpp
--rw-r--r--   0        0        0     2802 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_config.h
--rw-r--r--   0        0        0     1537 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_enum_values_registry.h
--rw-r--r--   0        0        0      199 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_exception.cpp
--rw-r--r--   0        0        0     3253 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_exception.h
--rw-r--r--   0        0        0     1273 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_generatortracker.h
--rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_registry_hub.cpp
--rw-r--r--   0        0        0     2216 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_registry_hub.h
--rw-r--r--   0        0        0     4091 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_reporter.cpp
--rw-r--r--   0        0        0     9383 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_reporter.h
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_runner.cpp
--rw-r--r--   0        0        0      552 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_runner.h
--rw-r--r--   0        0        0      881 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_tag_alias_registry.h
--rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_testcase.cpp
--rw-r--r--   0        0        0     1277 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_testcase.h
--rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_leak_detector.cpp
--rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_leak_detector.h
--rw-r--r--   0        0        0     6794 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_list.cpp
--rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_list.h
--rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers.cpp
--rw-r--r--   0        0        0     5752 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers.h
--rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_exception.cpp
--rw-r--r--   0        0        0      932 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_exception.hpp
--rw-r--r--   0        0        0     7563 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_floating.cpp
--rw-r--r--   0        0        0     2739 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_floating.h
--rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_generic.cpp
--rw-r--r--   0        0        0     1698 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_generic.hpp
--rw-r--r--   0        0        0     4847 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_string.cpp
--rw-r--r--   0        0        0     3169 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_string.h
--rw-r--r--   0        0        0     7599 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_vector.h
--rw-r--r--   0        0        0     4838 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_message.cpp
--rw-r--r--   0        0        0     2892 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_message.h
--rw-r--r--   0        0        0     1689 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_meta.hpp
--rw-r--r--   0        0        0     7631 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_objc.hpp
--rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_objc_arc.hpp
--rw-r--r--   0        0        0     2141 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_option.hpp
--rw-r--r--   0        0        0     4116 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_output_redirect.cpp
--rw-r--r--   0        0        0     3335 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_output_redirect.h
--rw-r--r--   0        0        0     1063 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_platform.h
--rw-r--r--   0        0        0      653 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_polyfills.cpp
--rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_polyfills.hpp
--rw-r--r--   0        0        0    22379 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_preprocessor.hpp
--rw-r--r--   0        0        0     1908 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_random_number_generator.cpp
--rw-r--r--   0        0        0     2049 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_random_number_generator.h
--rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_reenable_warnings.h
--rw-r--r--   0        0        0     3870 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_registry_hub.cpp
--rw-r--r--   0        0        0     2487 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_reporter_registrars.hpp
--rw-r--r--   0        0        0     1132 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_reporter_registry.cpp
--rw-r--r--   0        0        0     1086 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_reporter_registry.h
--rw-r--r--   0        0        0      979 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_result_type.cpp
--rw-r--r--   0        0        0     1634 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_result_type.h
--rw-r--r--   0        0        0    23394 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_run_context.cpp
--rw-r--r--   0        0        0     5793 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_run_context.h
--rw-r--r--   0        0        0     1093 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_section.cpp
--rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_section.h
--rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_section_info.cpp
--rw-r--r--   0        0        0     1156 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_section_info.h
--rw-r--r--   0        0        0    11333 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_session.cpp
--rw-r--r--   0        0        0     1692 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_session.h
--rw-r--r--   0        0        0      945 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_singletons.cpp
--rw-r--r--   0        0        0     1215 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_singletons.hpp
--rw-r--r--   0        0        0      916 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_startup_exception_registry.cpp
--rw-r--r--   0        0        0      866 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_startup_exception_registry.h
--rw-r--r--   0        0        0     5972 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_stream.cpp
--rw-r--r--   0        0        0     1235 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_stream.h
--rw-r--r--   0        0        0     3804 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_string_manip.cpp
--rw-r--r--   0        0        0     1646 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_string_manip.h
--rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_stringref.cpp
--rw-r--r--   0        0        0     3435 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_stringref.h
--rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_suppress_warnings.h
--rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tag_alias.cpp
--rw-r--r--   0        0        0      655 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tag_alias.h
--rw-r--r--   0        0        0      590 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tag_alias_autoregistrar.cpp
--rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tag_alias_autoregistrar.h
--rw-r--r--   0        0        0     2198 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tag_alias_registry.cpp
--rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tag_alias_registry.h
--rw-r--r--   0        0        0     6487 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_info.cpp
--rw-r--r--   0        0        0     2502 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_info.h
--rw-r--r--   0        0        0     6533 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_registry_impl.cpp
--rw-r--r--   0        0        0     2415 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_registry_impl.h
--rw-r--r--   0        0        0     7874 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_tracker.cpp
--rw-r--r--   0        0        0     5160 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_tracker.h
--rw-r--r--   0        0        0     1392 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_registry.cpp
--rw-r--r--   0        0        0    28151 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_registry.h
--rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_spec.cpp
--rw-r--r--   0        0        0     2822 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_spec.h
--rw-r--r--   0        0        0     7088 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_spec_parser.cpp
--rw-r--r--   0        0        0     2334 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_spec_parser.h
--rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_text.h
--rw-r--r--   0        0        0     2552 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_timer.cpp
--rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_timer.h
--rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_to_string.hpp
--rw-r--r--   0        0        0     7507 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tostring.cpp
--rw-r--r--   0        0        0    20503 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tostring.h
--rw-r--r--   0        0        0     1695 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_totals.cpp
--rw-r--r--   0        0        0     1063 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_totals.h
--rw-r--r--   0        0        0      713 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_uncaught_exceptions.cpp
--rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_uncaught_exceptions.h
--rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_user_interfaces.h
--rw-r--r--   0        0        0     1298 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_version.cpp
--rw-r--r--   0        0        0     1234 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_version.h
--rw-r--r--   0        0        0     1693 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_wildcard_pattern.cpp
--rw-r--r--   0        0        0     1146 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_wildcard_pattern.h
--rw-r--r--   0        0        0      966 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_windows_h_proxy.h
--rw-r--r--   0        0        0    10496 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_xmlwriter.cpp
--rw-r--r--   0        0        0     3600 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_xmlwriter.h
--rw-r--r--   0        0        0     2206 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_automake.hpp
--rw-r--r--   0        0        0     2606 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_bases.cpp
--rw-r--r--   0        0        0    10972 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_bases.hpp
--rw-r--r--   0        0        0     9970 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_compact.cpp
--rw-r--r--   0        0        0     1093 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_compact.h
--rw-r--r--   0        0        0    23898 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_console.cpp
--rw-r--r--   0        0        0     3105 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_console.h
--rw-r--r--   0        0        0    11374 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_junit.cpp
--rw-r--r--   0        0        0     1949 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_junit.h
--rw-r--r--   0        0        0     5731 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_listening.cpp
--rw-r--r--   0        0        0     2503 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_listening.h
--rw-r--r--   0        0        0     7090 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_sonarqube.hpp
--rw-r--r--   0        0        0     9581 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_tap.hpp
--rw-r--r--   0        0        0     8692 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_teamcity.hpp
--rw-r--r--   0        0        0    11973 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_xml.cpp
--rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_xml.h
--rw-r--r--   0        0        0      416 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/misc/CMakeLists.txt
--rw-r--r--   0        0        0     1031 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/misc/appveyorBuildConfigurationScript.bat
--rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/misc/appveyorMergeCoverageScript.py
--rw-r--r--   0        0        0      530 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/misc/appveyorTestRunScript.bat
--rw-r--r--   0        0        0     3987 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/misc/coverage-helper.cpp
--rw-r--r--   0        0        0     1020 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/misc/installOpenCppCoverage.ps1
--rw-r--r--   0        0        0    23633 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/CMakeLists.txt
--rw-r--r--   0        0        0     7473 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/CMakeLists.txt
--rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/ToDo.txt
--rw-r--r--   0        0        0     3139 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X01-PrefixedMacros.cpp
--rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X02-DisabledMacros.cpp
--rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X03-DisabledExceptions-DefaultHandler.cpp
--rw-r--r--   0        0        0      876 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X04-DisabledExceptions-CustomHandler.cpp
--rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X10-FallbackStringifier.cpp
--rw-r--r--   0        0        0      469 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X11-DisableStringification.cpp
--rw-r--r--   0        0        0      422 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X12-CustomDebugBreakMacro.cpp
--rw-r--r--   0        0        0     3443 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X20-BenchmarkingMacros.cpp
--rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X90-WindowsHeaderInclusion.cpp
--rw-r--r--   0        0        0     9171 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/automake.std.approved.txt
--rw-r--r--   0        0        0   165097 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/compact.sw.approved.txt
--rw-r--r--   0        0        0    49289 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/console.std.approved.txt
--rw-r--r--   0        0        0   457395 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/console.sw.approved.txt
--rw-r--r--   0        0        0    31587 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/console.swa4.approved.txt
--rw-r--r--   0        0        0   115141 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/junit.sw.approved.txt
--rw-r--r--   0        0        0    92599 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/sonarqube.sw.approved.txt
--rw-r--r--   0        0        0   679029 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/xml.sw.approved.txt
--rw-r--r--   0        0        0      351 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/CompileTimePerfTests/10.tests.cpp
--rw-r--r--   0        0        0      341 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/CompileTimePerfTests/100.tests.cpp
--rw-r--r--   0        0        0      695 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/CompileTimePerfTests/All.tests.cpp
--rw-r--r--   0        0        0    21380 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/CmdLine.tests.cpp
--rw-r--r--   0        0        0      848 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Details.tests.cpp
--rw-r--r--   0        0        0    12522 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/GeneratorsImpl.tests.cpp
--rw-r--r--   0        0        0    13268 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/InternalBenchmark.tests.cpp
--rw-r--r--   0        0        0     7755 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/PartTracker.tests.cpp
--rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/RandomNumberGeneration.tests.cpp
--rw-r--r--   0        0        0     4614 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/String.tests.cpp
--rw-r--r--   0        0        0     2857 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/StringManip.tests.cpp
--rw-r--r--   0        0        0     2314 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Tag.tests.cpp
--rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/ToString.tests.cpp
--rw-r--r--   0        0        0     5039 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Xml.tests.cpp
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Misc/invalid-test-names.input
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Misc/plain-old-tests.input
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Misc/special-characters-in-file.input
--rw-r--r--   0        0        0      185 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_console_colour.cpp
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_debugger.cpp
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_interfaces_reporter.cpp
--rw-r--r--   0        0        0      179 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_option.cpp
--rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_stream.cpp
--rw-r--r--   0        0        0      142 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_test_case_tracker.cpp
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_test_spec.cpp
--rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_xmlwriter.cpp
--rw-r--r--   0        0        0     1082 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/TestMain.cpp
--rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/TimingTests/Sleep.tests.cpp
--rw-r--r--   0        0        0     6558 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Approx.tests.cpp
--rw-r--r--   0        0        0     3775 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/BDD.tests.cpp
--rw-r--r--   0        0        0     4149 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Benchmark.tests.cpp
--rw-r--r--   0        0        0     4117 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Class.tests.cpp
--rw-r--r--   0        0        0     6914 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Compilation.tests.cpp
--rw-r--r--   0        0        0     9116 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Condition.tests.cpp
--rw-r--r--   0        0        0      915 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Decomposition.tests.cpp
--rw-r--r--   0        0        0     3440 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/EnumToString.tests.cpp
--rw-r--r--   0        0        0     6230 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Exception.tests.cpp
--rw-r--r--   0        0        0     9475 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Generators.tests.cpp
--rw-r--r--   0        0        0    26943 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Matchers.tests.cpp
--rw-r--r--   0        0        0     8031 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Message.tests.cpp
--rw-r--r--   0        0        0    13943 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Misc.tests.cpp
--rw-r--r--   0        0        0      506 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringByte.tests.cpp
--rw-r--r--   0        0        0     1696 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringChrono.tests.cpp
--rw-r--r--   0        0        0     5928 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringGeneral.tests.cpp
--rw-r--r--   0        0        0      915 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringOptional.tests.cpp
--rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringPair.tests.cpp
--rw-r--r--   0        0        0     1416 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringTuple.tests.cpp
--rw-r--r--   0        0        0     3186 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringVariant.tests.cpp
--rw-r--r--   0        0        0     3172 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringVector.tests.cpp
--rw-r--r--   0        0        0     5390 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringWhich.tests.cpp
--rw-r--r--   0        0        0     9842 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Tricky.tests.cpp
--rw-r--r--   0        0        0      570 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/VariadicMacros.tests.cpp
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/WarnAboutNoTests.cmake
--rw-r--r--   0        0        0     2130 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/TestScripts/testRandomOrder.py
--rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/CatchOCTestCase.h
--rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/CatchOCTestCase.mm
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/Main.mm
--rw-r--r--   0        0        0     3012 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/OCTest.1
--rw-r--r--   0        0        0      546 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/OCTest.mm
--rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/TestObj.h
--rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/TestObj.m
--rw-r--r--   0        0        0    11513 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest.xcodeproj/project.pbxproj
--rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest.xcodeproj/project.xcworkspace/contents.xcworkspacedata
--rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
--rw-r--r--   0        0        0     3990 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/catch_objc_impl.mm
--rw-r--r--   0        0        0     8344 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/approvalTests.py
--rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/approve.py
--rw-r--r--   0        0        0     4646 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/benchmarkCompile.py
--rw-r--r--   0        0        0     1632 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/benchmarkRunner.py
--rw-r--r--   0        0        0      260 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/developBuild.py
--rw-r--r--   0        0        0     2726 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/embed.py
--rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/embedClara.py
--rw-r--r--   0        0        0     3581 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/extractFeaturesFromReleaseNotes.py
--rw-r--r--   0        0        0     1441 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/fixWhitespace.py
--rw-r--r--   0        0        0     6336 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/generateSingleHeader.py
--rw-r--r--   0        0        0      261 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/majorRelease.py
--rw-r--r--   0        0        0      261 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/minorRelease.py
--rw-r--r--   0        0        0      260 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/patchRelease.py
--rw-r--r--   0        0        0     6846 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/releaseCommon.py
--rw-r--r--   0        0        0     1714 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/releaseNotes.py
--rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/scriptCommon.py
--rw-r--r--   0        0        0    13777 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/updateDocumentToC.py
--rw-r--r--   0        0        0     1610 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/scripts/updateWandbox.py
--rw-r--r--   0        0        0   656886 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/single_include/catch2/catch.hpp
--rw-r--r--   0        0        0     2206 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/single_include/catch2/catch_reporter_automake.hpp
--rw-r--r--   0        0        0     7090 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/single_include/catch2/catch_reporter_sonarqube.hpp
--rw-r--r--   0        0        0     9581 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/single_include/catch2/catch_reporter_tap.hpp
--rw-r--r--   0        0        0     8692 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/single_include/catch2/catch_reporter_teamcity.hpp
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/src/catch_with_main.cpp
--rw-r--r--   0        0        0    43554 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/extern/Catch2/third_party/clara.hpp
--rw-r--r--   0        0        0     3918 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/src/geometry.hpp
--rw-r--r--   0        0        0     7180 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/src/grid.hpp
--rw-r--r--   0        0        0     5004 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/src/intersections.cpp
--rw-r--r--   0        0        0     6918 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/src/operations.cpp
--rw-r--r--   0        0        0      523 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/src/operations.hpp
--rw-r--r--   0        0        0     2299 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/src/transform.hpp
--rw-r--r--   0        0        0     1289 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/src/utils.hpp
--rw-r--r--   0        0        0      418 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/tests/README.md
--rw-r--r--   0        0        0      206 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/tests/run_tests.cpp
--rw-r--r--   0        0        0    15640 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/tests/tests_intersections.cpp
--rw-r--r--   0        0        0     3389 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/extension/tests/tests_transform.cpp
--rw-r--r--   0        0        0     3342 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/images/snail.svg
--rw-r--r--   0        0        0     1452 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7752 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/failure_analysis/fragility_damage_analysis.py
--rw-r--r--   0        0        0     8230 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/failure_analysis/results_process_vietnam.py
--rwxr-xr-x   0        0        0     9057 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/network_creation/spatial_and_network_functions.py
--rw-r--r--   0        0        0    19444 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/network_hazard_intersections/hazards_network_intersections_results_collect.py
--rw-r--r--   0        0        0    14854 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/network_hazard_intersections/hazards_networks_intersections.py
--rw-r--r--   0        0        0     5534 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/network_hazard_intersections/intersection_networks.py
--rw-r--r--   0        0        0     5359 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/network_hazard_intersections/intersection_points.py
--rw-r--r--   0        0        0     5382 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/network_hazard_intersections/intersection_polygons.py
--rw-r--r--   0        0        0    24129 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/network_hazard_intersections/network_intersections.py
--rw-r--r--   0        0        0     6246 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/sources_sinks_routing/benchmark_shortest_path.py
--rw-r--r--   0        0        0   337206 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/sources_sinks_routing/igraph.png
--rw-r--r--   0        0        0   367721 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/sources_sinks_routing/pandana.png
--rw-r--r--   0        0        0     5397 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/sources_sinks_routing/shortest_paths_igraph.py
--rw-r--r--   0        0        0     6823 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/scripts/sources_sinks_routing/shortest_paths_pandana.py
--rw-r--r--   0        0        0      504 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/src/snail/__init__.py
--rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/src/snail/__main__.py
--rw-r--r--   0        0        0     9293 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/src/snail/cli.py
--rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/src/snail/core/__init__.py
--rw-r--r--   0        0        0     9058 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/src/snail/intersection.py
--rw-r--r--   0        0        0     3167 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/src/snail/io.py
--rw-r--r--   0        0        0     1009 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/src/snail/routing.py
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/src/snail/tqdm_standin.py
--rw-r--r--   0        0        0     2150 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/core/test_intersections.py
--rw-r--r--   0        0        0   262568 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/climatology-hd35-annual-mean.tif
--rw-r--r--   0        0        0   270586 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/climatology-hd35-historical.tif
--rw-r--r--   0        0        0      127 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/features.csv
--rw-r--r--   0        0        0     2030 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/inunriver_historical_WATCH_1980_rp01000.tif
--rw-r--r--   0        0        0      374 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/inunriver_historical_WATCH_1980_rp01000.tif.aux.xml
--rw-r--r--   0        0        0     3525 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/lines.geojson
--rw-r--r--   0        0        0      626 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/points.geojson
--rw-r--r--   0        0        0     1929 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/polygons.geojson
--rw-r--r--   0        0        0     1654 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/range.tif
--rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/range.tif.aux.xml
--rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/rasters.csv
--rw-r--r--   0        0        0      197 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/integration/run_examples.sh
--rw-r--r--   0        0        0     1134 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/split_polygons_rings.py
--rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/test_init.py
--rw-r--r--   0        0        0     3537 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/test_multi_intersections.py
--rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tests/test_routing.py
--rw-r--r--   0        0        0    15859 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tutorials/01-data-preparation-ghana.ipynb
--rw-r--r--   0        0        0    22516 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tutorials/02-assess-damage-and-disruption.ipynb
--rw-r--r--   0        0        0    20343 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tutorials/03-test-multiple-failures.ipynb
--rw-r--r--   0        0        0    15948 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/tutorials/04-evaluate-adaptation-options.ipynb
--rw-r--r--   0        0        0     8440 2022-11-09 12:37:21.000000 nismod-snail-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/.clang-format
+-rw-r--r--   0        0        0      233 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/.environment.yml
+-rw-r--r--   0        0        0     2170 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1497 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1448 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/.github/workflows/package.yml
+-rw-r--r--   0        0        0      285 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/.gitignore
+-rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/.gitmodules
+-rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/CMakeLists.txt
+-rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5791 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/README.md
+-rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/docs/Makefile
+-rw-r--r--   0        0        0      473 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/docs/source/_static/theme_tweaks.css
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/docs/source/api/modules.rst
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/docs/source/api/snail.core.rst
+-rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/docs/source/api/snail.rst
+-rw-r--r--   0        0        0     1444 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/docs/source/conf.py
+-rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/docs/source/getting_started.md
+-rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/docs/source/index.rst
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/docs/source/license.rst
+-rw-r--r--   0        0        0     1550 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/examples.sh
+-rw-r--r--   0        0        0      429 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/CMakeLists.txt
+-rw-r--r--   0        0        0      628 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.clang-format
+-rw-r--r--   0        0        0     3044 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.conan/build.py
+-rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.conan/test_package/CMakeLists.txt
+-rw-r--r--   0        0        0      551 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.conan/test_package/conanfile.py
+-rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.conan/test_package/test_package.cpp
+-rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.gitattributes
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      711 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      308 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.github/pull_request_template.md
+-rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.gitignore
+-rw-r--r--   0        0        0     8343 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/.travis.yml
+-rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/BUILD.bazel
+-rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/CMake/Catch2Config.cmake.in
+-rw-r--r--   0        0        0     5086 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/CMake/FindGcov.cmake
+-rw-r--r--   0        0        0    12328 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/CMake/FindLcov.cmake
+-rw-r--r--   0        0        0     8419 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/CMake/Findcodecov.cmake
+-rw-r--r--   0        0        0     1226 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/CMake/MiscFunctions.cmake
+-rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/CMake/catch2.pc.in
+-rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/CMake/llvm-cov-wrapper
+-rw-r--r--   0        0        0     7737 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/CMakeLists.txt
+-rw-r--r--   0        0        0     3215 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/LICENSE.txt
+-rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/WORKSPACE
+-rw-r--r--   0        0        0     2702 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/appveyor.yml
+-rw-r--r--   0        0        0    10636 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/artwork/catch2-c-logo.png
+-rw-r--r--   0        0        0    33761 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/artwork/catch2-hand-logo.png
+-rw-r--r--   0        0        0    20939 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/artwork/catch2-logo-small.png
+-rw-r--r--   0        0        0      438 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/codecov.yml
+-rw-r--r--   0        0        0     1006 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/conanfile.py
+-rw-r--r--   0        0        0     8574 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/contrib/Catch.cmake
+-rw-r--r--   0        0        0     3942 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/contrib/CatchAddTests.cmake
+-rw-r--r--   0        0        0    15008 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/contrib/ParseAndAddCatchTests.cmake
+-rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/contrib/gdbinit
+-rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/contrib/lldbinit
+-rw-r--r--   0        0        0     1325 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/Readme.md
+-rw-r--r--   0        0        0     8308 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/assertions.md
+-rw-r--r--   0        0        0    11499 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/benchmarks.md
+-rw-r--r--   0        0        0     5466 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/ci-and-misc.md
+-rw-r--r--   0        0        0     9757 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/cmake-integration.md
+-rw-r--r--   0        0        0    20867 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/command-line.md
+-rw-r--r--   0        0        0     1064 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/commercial-users.md
+-rw-r--r--   0        0        0    14426 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/configuration.md
+-rw-r--r--   0        0        0     8881 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/contributing.md
+-rw-r--r--   0        0        0     4887 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/deprecations.md
+-rw-r--r--   0        0        0     2810 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/event-listeners.md
+-rw-r--r--   0        0        0     8448 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/generators.md
+-rw-r--r--   0        0        0     7211 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/limitations.md
+-rw-r--r--   0        0        0     2939 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/list-of-examples.md
+-rw-r--r--   0        0        0     4952 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/logging.md
+-rw-r--r--   0        0        0     8097 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/matchers.md
+-rw-r--r--   0        0        0     6026 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/opensource-users.md
+-rw-r--r--   0        0        0     4014 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/other-macros.md
+-rw-r--r--   0        0        0     4400 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/own-main.md
+-rw-r--r--   0        0        0    56784 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/release-notes.md
+-rw-r--r--   0        0        0     3326 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/release-process.md
+-rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/reporters.md
+-rw-r--r--   0        0        0     5020 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/slow-compiles.md
+-rw-r--r--   0        0        0    13228 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/test-cases-and-sections.md
+-rw-r--r--   0        0        0     5281 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/test-fixtures.md
+-rw-r--r--   0        0        0     4775 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/tostring.md
+-rw-r--r--   0        0        0    14790 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/tutorial.md
+-rw-r--r--   0        0        0     2513 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/docs/why-catch.md
+-rw-r--r--   0        0        0      488 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/000-CatchMain.cpp
+-rw-r--r--   0        0        0     1323 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/010-TestCase.cpp
+-rw-r--r--   0        0        0     1232 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/020-TestCase-1.cpp
+-rw-r--r--   0        0        0     1168 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/020-TestCase-2.cpp
+-rw-r--r--   0        0        0     2791 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/030-Asn-Require-Check.cpp
+-rw-r--r--   0        0        0     2513 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/100-Fix-Section.cpp
+-rw-r--r--   0        0        0     1963 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/110-Fix-ClassFixture.cpp
+-rw-r--r--   0        0        0     3040 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/120-Bdd-ScenarioGivenWhenThen.cpp
+-rw-r--r--   0        0        0      884 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/200-Rpt-CatchMain.cpp
+-rw-r--r--   0        0        0     5701 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/207-Rpt-TeamCityReporter.cpp
+-rw-r--r--   0        0        0    14789 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/210-Evt-EventListeners.cpp
+-rw-r--r--   0        0        0     1443 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/231-Cfg-OutputStreams.cpp
+-rw-r--r--   0        0        0     1965 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/300-Gen-OwnGenerator.cpp
+-rw-r--r--   0        0        0     1887 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/301-Gen-MapTypeConversion.cpp
+-rw-r--r--   0        0        0     2121 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/302-Gen-Table.cpp
+-rw-r--r--   0        0        0     1230 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/310-Gen-VariablesInGenerators.cpp
+-rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/311-Gen-CustomCapture.cpp
+-rw-r--r--   0        0        0     5425 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/examples/CMakeLists.txt
+-rw-r--r--   0        0        0    30046 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/catch.hpp
+-rw-r--r--   0        0        0      462 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/catch_with_main.hpp
+-rw-r--r--   0        0        0    40644 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/external/clara.hpp
+-rw-r--r--   0        0        0     4850 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_benchmark.hpp
+-rw-r--r--   0        0        0     1040 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_benchmarking_all.hpp
+-rw-r--r--   0        0        0     2292 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_chronometer.hpp
+-rw-r--r--   0        0        0     1123 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_clock.hpp
+-rw-r--r--   0        0        0     2523 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_constructor.hpp
+-rw-r--r--   0        0        0     1164 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_environment.hpp
+-rw-r--r--   0        0        0      912 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_estimate.hpp
+-rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_execution_plan.hpp
+-rw-r--r--   0        0        0     2189 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_optimizer.hpp
+-rw-r--r--   0        0        0      987 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_outlier_classification.hpp
+-rw-r--r--   0        0        0     1575 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_sample_analysis.hpp
+-rw-r--r--   0        0        0     3213 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_analyse.hpp
+-rw-r--r--   0        0        0     4019 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_benchmark_function.hpp
+-rw-r--r--   0        0        0     2517 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_complete_invoke.hpp
+-rw-r--r--   0        0        0     5000 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_estimate_clock.hpp
+-rw-r--r--   0        0        0     1132 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_measure.hpp
+-rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_repeat.hpp
+-rw-r--r--   0        0        0     2545 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_run_for_at_least.hpp
+-rw-r--r--   0        0        0     8942 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_stats.cpp
+-rw-r--r--   0        0        0     6541 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_stats.hpp
+-rw-r--r--   0        0        0      977 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_timing.hpp
+-rw-r--r--   0        0        0     2593 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_approx.cpp
+-rw-r--r--   0        0        0     5044 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_approx.h
+-rw-r--r--   0        0        0     4477 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_assertionhandler.cpp
+-rw-r--r--   0        0        0     2714 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_assertionhandler.h
+-rw-r--r--   0        0        0      910 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_assertioninfo.h
+-rw-r--r--   0        0        0     3313 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_assertionresult.cpp
+-rw-r--r--   0        0        0     1800 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_assertionresult.h
+-rw-r--r--   0        0        0     7782 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_capture.hpp
+-rw-r--r--   0        0        0     1035 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_capture_matchers.cpp
+-rw-r--r--   0        0        0     3802 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_capture_matchers.h
+-rw-r--r--   0        0        0     1275 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_clara.h
+-rw-r--r--   0        0        0    10800 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_commandline.cpp
+-rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_commandline.h
+-rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_common.cpp
+-rw-r--r--   0        0        0     3050 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_common.h
+-rw-r--r--   0        0        0    15337 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_compiler_capabilities.h
+-rw-r--r--   0        0        0     4161 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_config.cpp
+-rw-r--r--   0        0        0     4300 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_config.hpp
+-rw-r--r--   0        0        0     1292 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_config_uncaught_exceptions.hpp
+-rw-r--r--   0        0        0     8558 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_console_colour.cpp
+-rw-r--r--   0        0        0     1797 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_console_colour.h
+-rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_context.cpp
+-rw-r--r--   0        0        0     1748 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_context.h
+-rw-r--r--   0        0        0     1035 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_debug_console.cpp
+-rw-r--r--   0        0        0      461 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_debug_console.h
+-rw-r--r--   0        0        0     4360 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_debugger.cpp
+-rw-r--r--   0        0        0     2159 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_debugger.h
+-rw-r--r--   0        0        0      807 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_decomposer.cpp
+-rw-r--r--   0        0        0    10336 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_decomposer.h
+-rw-r--r--   0        0        0     1238 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_default_main.hpp
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_enforce.cpp
+-rw-r--r--   0        0        0     1549 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_enforce.h
+-rw-r--r--   0        0        0     2716 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_enum_values_registry.cpp
+-rw-r--r--   0        0        0     1055 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_enum_values_registry.h
+-rw-r--r--   0        0        0      385 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_errno_guard.cpp
+-rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_errno_guard.h
+-rw-r--r--   0        0        0     3073 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_exception_translator_registry.cpp
+-rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_exception_translator_registry.h
+-rw-r--r--   0        0        0      752 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_external_interfaces.h
+-rw-r--r--   0        0        0     8920 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_fatal_condition.cpp
+-rw-r--r--   0        0        0     2231 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_fatal_condition.h
+-rw-r--r--   0        0        0      827 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_generators.cpp
+-rw-r--r--   0        0        0     7952 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_generators.hpp
+-rw-r--r--   0        0        0     8492 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_generators_generic.hpp
+-rw-r--r--   0        0        0     5193 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_generators_specific.hpp
+-rw-r--r--   0        0        0      848 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_impl.hpp
+-rw-r--r--   0        0        0      108 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_capture.cpp
+-rw-r--r--   0        0        0     3656 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_capture.h
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_config.cpp
+-rw-r--r--   0        0        0     2802 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_config.h
+-rw-r--r--   0        0        0     1537 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_enum_values_registry.h
+-rw-r--r--   0        0        0      199 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_exception.cpp
+-rw-r--r--   0        0        0     3253 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_exception.h
+-rw-r--r--   0        0        0     1273 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_generatortracker.h
+-rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_registry_hub.cpp
+-rw-r--r--   0        0        0     2216 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_registry_hub.h
+-rw-r--r--   0        0        0     4091 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_reporter.cpp
+-rw-r--r--   0        0        0     9383 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_reporter.h
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_runner.cpp
+-rw-r--r--   0        0        0      552 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_runner.h
+-rw-r--r--   0        0        0      881 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_tag_alias_registry.h
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_testcase.cpp
+-rw-r--r--   0        0        0     1277 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_testcase.h
+-rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_leak_detector.cpp
+-rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_leak_detector.h
+-rw-r--r--   0        0        0     6794 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_list.cpp
+-rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_list.h
+-rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers.cpp
+-rw-r--r--   0        0        0     5752 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers.h
+-rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_exception.cpp
+-rw-r--r--   0        0        0      932 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_exception.hpp
+-rw-r--r--   0        0        0     7563 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_floating.cpp
+-rw-r--r--   0        0        0     2739 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_floating.h
+-rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_generic.cpp
+-rw-r--r--   0        0        0     1698 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_generic.hpp
+-rw-r--r--   0        0        0     4847 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_string.cpp
+-rw-r--r--   0        0        0     3169 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_string.h
+-rw-r--r--   0        0        0     7599 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_vector.h
+-rw-r--r--   0        0        0     4838 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_message.cpp
+-rw-r--r--   0        0        0     2892 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_message.h
+-rw-r--r--   0        0        0     1689 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_meta.hpp
+-rw-r--r--   0        0        0     7631 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_objc.hpp
+-rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_objc_arc.hpp
+-rw-r--r--   0        0        0     2141 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_option.hpp
+-rw-r--r--   0        0        0     4116 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_output_redirect.cpp
+-rw-r--r--   0        0        0     3335 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_output_redirect.h
+-rw-r--r--   0        0        0     1063 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_platform.h
+-rw-r--r--   0        0        0      653 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_polyfills.cpp
+-rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_polyfills.hpp
+-rw-r--r--   0        0        0    22379 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_preprocessor.hpp
+-rw-r--r--   0        0        0     1908 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_random_number_generator.cpp
+-rw-r--r--   0        0        0     2049 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_random_number_generator.h
+-rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_reenable_warnings.h
+-rw-r--r--   0        0        0     3870 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_registry_hub.cpp
+-rw-r--r--   0        0        0     2487 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_reporter_registrars.hpp
+-rw-r--r--   0        0        0     1132 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_reporter_registry.cpp
+-rw-r--r--   0        0        0     1086 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_reporter_registry.h
+-rw-r--r--   0        0        0      979 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_result_type.cpp
+-rw-r--r--   0        0        0     1634 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_result_type.h
+-rw-r--r--   0        0        0    23394 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_run_context.cpp
+-rw-r--r--   0        0        0     5793 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_run_context.h
+-rw-r--r--   0        0        0     1093 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_section.cpp
+-rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_section.h
+-rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_section_info.cpp
+-rw-r--r--   0        0        0     1156 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_section_info.h
+-rw-r--r--   0        0        0    11333 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_session.cpp
+-rw-r--r--   0        0        0     1692 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_session.h
+-rw-r--r--   0        0        0      945 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_singletons.cpp
+-rw-r--r--   0        0        0     1215 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_singletons.hpp
+-rw-r--r--   0        0        0      916 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_startup_exception_registry.cpp
+-rw-r--r--   0        0        0      866 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_startup_exception_registry.h
+-rw-r--r--   0        0        0     5972 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_stream.cpp
+-rw-r--r--   0        0        0     1235 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_stream.h
+-rw-r--r--   0        0        0     3804 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_string_manip.cpp
+-rw-r--r--   0        0        0     1646 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_string_manip.h
+-rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_stringref.cpp
+-rw-r--r--   0        0        0     3435 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_stringref.h
+-rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_suppress_warnings.h
+-rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tag_alias.cpp
+-rw-r--r--   0        0        0      655 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tag_alias.h
+-rw-r--r--   0        0        0      590 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tag_alias_autoregistrar.cpp
+-rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tag_alias_autoregistrar.h
+-rw-r--r--   0        0        0     2198 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tag_alias_registry.cpp
+-rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tag_alias_registry.h
+-rw-r--r--   0        0        0     6487 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_info.cpp
+-rw-r--r--   0        0        0     2502 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_info.h
+-rw-r--r--   0        0        0     6533 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_registry_impl.cpp
+-rw-r--r--   0        0        0     2415 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_registry_impl.h
+-rw-r--r--   0        0        0     7874 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_tracker.cpp
+-rw-r--r--   0        0        0     5160 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_tracker.h
+-rw-r--r--   0        0        0     1392 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_registry.cpp
+-rw-r--r--   0        0        0    28151 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_registry.h
+-rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_spec.cpp
+-rw-r--r--   0        0        0     2822 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_spec.h
+-rw-r--r--   0        0        0     7088 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_spec_parser.cpp
+-rw-r--r--   0        0        0     2334 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_spec_parser.h
+-rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_text.h
+-rw-r--r--   0        0        0     2552 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_timer.cpp
+-rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_timer.h
+-rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_to_string.hpp
+-rw-r--r--   0        0        0     7507 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tostring.cpp
+-rw-r--r--   0        0        0    20503 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tostring.h
+-rw-r--r--   0        0        0     1695 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_totals.cpp
+-rw-r--r--   0        0        0     1063 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_totals.h
+-rw-r--r--   0        0        0      713 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_uncaught_exceptions.cpp
+-rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_uncaught_exceptions.h
+-rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_user_interfaces.h
+-rw-r--r--   0        0        0     1298 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_version.cpp
+-rw-r--r--   0        0        0     1234 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_version.h
+-rw-r--r--   0        0        0     1693 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_wildcard_pattern.cpp
+-rw-r--r--   0        0        0     1146 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_wildcard_pattern.h
+-rw-r--r--   0        0        0      966 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_windows_h_proxy.h
+-rw-r--r--   0        0        0    10496 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_xmlwriter.cpp
+-rw-r--r--   0        0        0     3600 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_xmlwriter.h
+-rw-r--r--   0        0        0     2206 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_automake.hpp
+-rw-r--r--   0        0        0     2606 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_bases.cpp
+-rw-r--r--   0        0        0    10972 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_bases.hpp
+-rw-r--r--   0        0        0     9970 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_compact.cpp
+-rw-r--r--   0        0        0     1093 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_compact.h
+-rw-r--r--   0        0        0    23898 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_console.cpp
+-rw-r--r--   0        0        0     3105 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_console.h
+-rw-r--r--   0        0        0    11374 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_junit.cpp
+-rw-r--r--   0        0        0     1949 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_junit.h
+-rw-r--r--   0        0        0     5731 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_listening.cpp
+-rw-r--r--   0        0        0     2503 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_listening.h
+-rw-r--r--   0        0        0     7090 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_sonarqube.hpp
+-rw-r--r--   0        0        0     9581 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_tap.hpp
+-rw-r--r--   0        0        0     8692 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_teamcity.hpp
+-rw-r--r--   0        0        0    11973 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_xml.cpp
+-rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_xml.h
+-rw-r--r--   0        0        0      416 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/misc/CMakeLists.txt
+-rw-r--r--   0        0        0     1031 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/misc/appveyorBuildConfigurationScript.bat
+-rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/misc/appveyorMergeCoverageScript.py
+-rw-r--r--   0        0        0      530 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/misc/appveyorTestRunScript.bat
+-rw-r--r--   0        0        0     3987 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/misc/coverage-helper.cpp
+-rw-r--r--   0        0        0     1020 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/misc/installOpenCppCoverage.ps1
+-rw-r--r--   0        0        0    23633 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/CMakeLists.txt
+-rw-r--r--   0        0        0     7473 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/CMakeLists.txt
+-rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/ToDo.txt
+-rw-r--r--   0        0        0     3139 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X01-PrefixedMacros.cpp
+-rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X02-DisabledMacros.cpp
+-rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X03-DisabledExceptions-DefaultHandler.cpp
+-rw-r--r--   0        0        0      876 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X04-DisabledExceptions-CustomHandler.cpp
+-rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X10-FallbackStringifier.cpp
+-rw-r--r--   0        0        0      469 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X11-DisableStringification.cpp
+-rw-r--r--   0        0        0      422 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X12-CustomDebugBreakMacro.cpp
+-rw-r--r--   0        0        0     3443 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X20-BenchmarkingMacros.cpp
+-rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X90-WindowsHeaderInclusion.cpp
+-rw-r--r--   0        0        0     9171 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/automake.std.approved.txt
+-rw-r--r--   0        0        0   165097 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/compact.sw.approved.txt
+-rw-r--r--   0        0        0    49289 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/console.std.approved.txt
+-rw-r--r--   0        0        0   457395 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/console.sw.approved.txt
+-rw-r--r--   0        0        0    31587 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/console.swa4.approved.txt
+-rw-r--r--   0        0        0   115141 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/junit.sw.approved.txt
+-rw-r--r--   0        0        0    92599 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/sonarqube.sw.approved.txt
+-rw-r--r--   0        0        0   679029 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/xml.sw.approved.txt
+-rw-r--r--   0        0        0      351 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/CompileTimePerfTests/10.tests.cpp
+-rw-r--r--   0        0        0      341 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/CompileTimePerfTests/100.tests.cpp
+-rw-r--r--   0        0        0      695 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/CompileTimePerfTests/All.tests.cpp
+-rw-r--r--   0        0        0    21380 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/CmdLine.tests.cpp
+-rw-r--r--   0        0        0      848 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Details.tests.cpp
+-rw-r--r--   0        0        0    12522 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/GeneratorsImpl.tests.cpp
+-rw-r--r--   0        0        0    13268 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/InternalBenchmark.tests.cpp
+-rw-r--r--   0        0        0     7755 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/PartTracker.tests.cpp
+-rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/RandomNumberGeneration.tests.cpp
+-rw-r--r--   0        0        0     4614 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/String.tests.cpp
+-rw-r--r--   0        0        0     2857 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/StringManip.tests.cpp
+-rw-r--r--   0        0        0     2314 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Tag.tests.cpp
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/ToString.tests.cpp
+-rw-r--r--   0        0        0     5039 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Xml.tests.cpp
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Misc/invalid-test-names.input
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Misc/plain-old-tests.input
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Misc/special-characters-in-file.input
+-rw-r--r--   0        0        0      185 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_console_colour.cpp
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_debugger.cpp
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_interfaces_reporter.cpp
+-rw-r--r--   0        0        0      179 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_option.cpp
+-rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_stream.cpp
+-rw-r--r--   0        0        0      142 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_test_case_tracker.cpp
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_test_spec.cpp
+-rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/SurrogateCpps/catch_xmlwriter.cpp
+-rw-r--r--   0        0        0     1082 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/TestMain.cpp
+-rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/TimingTests/Sleep.tests.cpp
+-rw-r--r--   0        0        0     6558 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Approx.tests.cpp
+-rw-r--r--   0        0        0     3775 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/BDD.tests.cpp
+-rw-r--r--   0        0        0     4149 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Benchmark.tests.cpp
+-rw-r--r--   0        0        0     4117 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Class.tests.cpp
+-rw-r--r--   0        0        0     6914 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Compilation.tests.cpp
+-rw-r--r--   0        0        0     9116 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Condition.tests.cpp
+-rw-r--r--   0        0        0      915 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Decomposition.tests.cpp
+-rw-r--r--   0        0        0     3440 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/EnumToString.tests.cpp
+-rw-r--r--   0        0        0     6230 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Exception.tests.cpp
+-rw-r--r--   0        0        0     9475 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Generators.tests.cpp
+-rw-r--r--   0        0        0    26943 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Matchers.tests.cpp
+-rw-r--r--   0        0        0     8031 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Message.tests.cpp
+-rw-r--r--   0        0        0    13943 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Misc.tests.cpp
+-rw-r--r--   0        0        0      506 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringByte.tests.cpp
+-rw-r--r--   0        0        0     1696 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringChrono.tests.cpp
+-rw-r--r--   0        0        0     5928 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringGeneral.tests.cpp
+-rw-r--r--   0        0        0      915 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringOptional.tests.cpp
+-rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringPair.tests.cpp
+-rw-r--r--   0        0        0     1416 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringTuple.tests.cpp
+-rw-r--r--   0        0        0     3186 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringVariant.tests.cpp
+-rw-r--r--   0        0        0     3172 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringVector.tests.cpp
+-rw-r--r--   0        0        0     5390 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringWhich.tests.cpp
+-rw-r--r--   0        0        0     9842 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Tricky.tests.cpp
+-rw-r--r--   0        0        0      570 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/VariadicMacros.tests.cpp
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/WarnAboutNoTests.cmake
+-rw-r--r--   0        0        0     2130 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/TestScripts/testRandomOrder.py
+-rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/CatchOCTestCase.h
+-rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/CatchOCTestCase.mm
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/Main.mm
+-rw-r--r--   0        0        0     3012 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/OCTest.1
+-rw-r--r--   0        0        0      546 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/OCTest.mm
+-rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/TestObj.h
+-rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/TestObj.m
+-rw-r--r--   0        0        0    11513 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest.xcodeproj/project.pbxproj
+-rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+-rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-r--r--   0        0        0     3990 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/catch_objc_impl.mm
+-rw-r--r--   0        0        0     8344 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/approvalTests.py
+-rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/approve.py
+-rw-r--r--   0        0        0     4646 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/benchmarkCompile.py
+-rw-r--r--   0        0        0     1632 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/benchmarkRunner.py
+-rw-r--r--   0        0        0      260 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/developBuild.py
+-rw-r--r--   0        0        0     2726 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/embed.py
+-rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/embedClara.py
+-rw-r--r--   0        0        0     3581 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/extractFeaturesFromReleaseNotes.py
+-rw-r--r--   0        0        0     1441 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/fixWhitespace.py
+-rw-r--r--   0        0        0     6336 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/generateSingleHeader.py
+-rw-r--r--   0        0        0      261 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/majorRelease.py
+-rw-r--r--   0        0        0      261 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/minorRelease.py
+-rw-r--r--   0        0        0      260 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/patchRelease.py
+-rw-r--r--   0        0        0     6846 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/releaseCommon.py
+-rw-r--r--   0        0        0     1714 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/releaseNotes.py
+-rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/scriptCommon.py
+-rw-r--r--   0        0        0    13777 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/updateDocumentToC.py
+-rw-r--r--   0        0        0     1610 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/scripts/updateWandbox.py
+-rw-r--r--   0        0        0   656886 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/single_include/catch2/catch.hpp
+-rw-r--r--   0        0        0     2206 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/single_include/catch2/catch_reporter_automake.hpp
+-rw-r--r--   0        0        0     7090 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/single_include/catch2/catch_reporter_sonarqube.hpp
+-rw-r--r--   0        0        0     9581 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/single_include/catch2/catch_reporter_tap.hpp
+-rw-r--r--   0        0        0     8692 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/single_include/catch2/catch_reporter_teamcity.hpp
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/src/catch_with_main.cpp
+-rw-r--r--   0        0        0    43554 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/extern/Catch2/third_party/clara.hpp
+-rw-r--r--   0        0        0     3918 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/src/geometry.hpp
+-rw-r--r--   0        0        0     7180 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/src/grid.hpp
+-rw-r--r--   0        0        0     5004 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/src/intersections.cpp
+-rw-r--r--   0        0        0     6918 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/src/operations.cpp
+-rw-r--r--   0        0        0      523 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/src/operations.hpp
+-rw-r--r--   0        0        0     2299 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/src/transform.hpp
+-rw-r--r--   0        0        0     1289 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/src/utils.hpp
+-rw-r--r--   0        0        0      420 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/tests/README.md
+-rw-r--r--   0        0        0      206 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/tests/run_tests.cpp
+-rw-r--r--   0        0        0    15640 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/tests/tests_intersections.cpp
+-rw-r--r--   0        0        0     3389 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/extension/tests/tests_transform.cpp
+-rw-r--r--   0        0        0     3342 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/images/snail.svg
+-rw-r--r--   0        0        0     1452 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7752 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/failure_analysis/fragility_damage_analysis.py
+-rw-r--r--   0        0        0     8230 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/failure_analysis/results_process_vietnam.py
+-rwxr-xr-x   0        0        0     9057 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/network_creation/spatial_and_network_functions.py
+-rw-r--r--   0        0        0    19444 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/network_hazard_intersections/hazards_network_intersections_results_collect.py
+-rw-r--r--   0        0        0    14854 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/network_hazard_intersections/hazards_networks_intersections.py
+-rw-r--r--   0        0        0     5534 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/network_hazard_intersections/intersection_networks.py
+-rw-r--r--   0        0        0     5359 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/network_hazard_intersections/intersection_points.py
+-rw-r--r--   0        0        0     5382 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/network_hazard_intersections/intersection_polygons.py
+-rw-r--r--   0        0        0    24129 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/network_hazard_intersections/network_intersections.py
+-rw-r--r--   0        0        0     6246 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/sources_sinks_routing/benchmark_shortest_path.py
+-rw-r--r--   0        0        0   337206 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/sources_sinks_routing/igraph.png
+-rw-r--r--   0        0        0   367721 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/sources_sinks_routing/pandana.png
+-rw-r--r--   0        0        0     5397 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/sources_sinks_routing/shortest_paths_igraph.py
+-rw-r--r--   0        0        0     6823 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/scripts/sources_sinks_routing/shortest_paths_pandana.py
+-rw-r--r--   0        0        0      504 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/src/snail/__init__.py
+-rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/src/snail/__main__.py
+-rw-r--r--   0        0        0     9293 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/src/snail/cli.py
+-rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/src/snail/core/__init__.py
+-rw-r--r--   0        0        0     9247 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/src/snail/intersection.py
+-rw-r--r--   0        0        0     3167 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/src/snail/io.py
+-rw-r--r--   0        0        0     1009 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/src/snail/routing.py
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/src/snail/tqdm_standin.py
+-rw-r--r--   0        0        0     2150 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/core/test_intersections.py
+-rw-r--r--   0        0        0   262568 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/climatology-hd35-annual-mean.tif
+-rw-r--r--   0        0        0   270586 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/climatology-hd35-historical.tif
+-rw-r--r--   0        0        0      127 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/features.csv
+-rw-r--r--   0        0        0     2030 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/inunriver_historical_WATCH_1980_rp01000.tif
+-rw-r--r--   0        0        0      374 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/inunriver_historical_WATCH_1980_rp01000.tif.aux.xml
+-rw-r--r--   0        0        0     3525 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/lines.geojson
+-rw-r--r--   0        0        0      626 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/points.geojson
+-rw-r--r--   0        0        0     1929 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/polygons.geojson
+-rw-r--r--   0        0        0     1654 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/range.tif
+-rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/range.tif.aux.xml
+-rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/rasters.csv
+-rw-r--r--   0        0        0      197 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/integration/run_examples.sh
+-rw-r--r--   0        0        0     1134 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/split_polygons_rings.py
+-rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/test_init.py
+-rw-r--r--   0        0        0     3537 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/test_multi_intersections.py
+-rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tests/test_routing.py
+-rw-r--r--   0        0        0    15859 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tutorials/01-data-preparation-ghana.ipynb
+-rw-r--r--   0        0        0    22516 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tutorials/02-assess-damage-and-disruption.ipynb
+-rw-r--r--   0        0        0    20343 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tutorials/03-test-multiple-failures.ipynb
+-rw-r--r--   0        0        0    15948 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/tutorials/04-evaluate-adaptation-options.ipynb
+-rw-r--r--   0        0        0     8354 2022-11-09 12:37:21.000000 nismod-snail-0.3.2/PKG-INFO
```

### Comparing `nismod-snail-0.3.1/.github/workflows/build.yml` & `nismod-snail-0.3.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/.github/workflows/docs.yml` & `nismod-snail-0.3.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/.github/workflows/package.yml` & `nismod-snail-0.3.2/.github/workflows/package.yml`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/CMakeLists.txt` & `nismod-snail-0.3.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/LICENSE` & `nismod-snail-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/README.md` & `nismod-snail-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -163,25 +163,25 @@
 This may need some includes for `pybind11` - which will vary depending on your
 python installation. For example, with python via miniconda:
 
     clang-tidy --checks 'cppcoreguidelines-*' extension/src/* -- \
         -I/home/username/miniconda3/include/python3.11/ \
         -I./pybind11/include/
 
-Or with c++ headers installed on a Linux machine:
+Or with C++ headers installed on a Linux machine:
 
-    clang-tidy --checks 'cppcoreguidelines-*' \
-        extension/src/*  \
-        -- -std=c++11  -I/usr/include/x86_64-linux-gnu/c++/11 -I/usr/include/c++/11
+    clang-tidy --checks 'cppcoreguidelines-*' extension/src/* -- \
+        -std=c++14  \
+        -I/usr/include/x86_64-linux-gnu/c++/11 \
+        -I/usr/include/c++/11 \
+        -I{$PWD}/extension/extern/pybind11/include \
+        -I/usr/include/python3.10
 
 ### Integration of C++ and Python using pybind11
 
 The `snail.core.intersections` module is built using `pybind11` with
-`setuptools` (see [docs](https://pybind11.readthedocs.io/en/stable/compiling.html#building-with-setuptools))
+`scikit-build-core` (see [docs](https://scikit-build-core.readthedocs.io/en/latest/))
 
 - `extension/src/intersections.cpp` defines the module interface using the
   `PYBIND11_MODULE` macro
 - `pyproject.toml` defines the build requirements for snail, which includes
-  pybind11, wheel and setuptools
-- `setup.py` defines the `Pybind11Extension` module to build - both the C++
-  files to compile, and the location of the built module within the python
-  package
+  pybind11 and scikit-build-core
```

#### html2text {}

```diff
@@ -56,18 +56,17 @@
 update --init --recursive Build the library and run tests: cmake -Bbuild ./
 extension cmake --build build/ ./build/run_tests Run code style auto-
 formatting: clang-format -i extension/src/*.{cpp,hpp} Run lints and checks:
 clang-tidy --checks 'cppcoreguidelines-*' extension/src/*.{cpp,hpp} This may
 need some includes for `pybind11` - which will vary depending on your python
 installation. For example, with python via miniconda: clang-tidy --checks
 'cppcoreguidelines-*' extension/src/* -- \ -I/home/username/miniconda3/include/
-python3.11/ \ -I./pybind11/include/ Or with c++ headers installed on a Linux
-machine: clang-tidy --checks 'cppcoreguidelines-*' \ extension/src/* \ -- -
-std=c++11 -I/usr/include/x86_64-linux-gnu/c++/11 -I/usr/include/c++/11 ###
+python3.11/ \ -I./pybind11/include/ Or with C++ headers installed on a Linux
+machine: clang-tidy --checks 'cppcoreguidelines-*' extension/src/* -- \ -
+std=c++14 \ -I/usr/include/x86_64-linux-gnu/c++/11 \ -I/usr/include/c++/11 \ -I
+{$PWD}/extension/extern/pybind11/include \ -I/usr/include/python3.10 ###
 Integration of C++ and Python using pybind11 The `snail.core.intersections`
-module is built using `pybind11` with `setuptools` (see [docs](https://
-pybind11.readthedocs.io/en/stable/compiling.html#building-with-setuptools)) -
-`extension/src/intersections.cpp` defines the module interface using the
-`PYBIND11_MODULE` macro - `pyproject.toml` defines the build requirements for
-snail, which includes pybind11, wheel and setuptools - `setup.py` defines the
-`Pybind11Extension` module to build - both the C++ files to compile, and the
-location of the built module within the python package
+module is built using `pybind11` with `scikit-build-core` (see [docs](https://
+scikit-build-core.readthedocs.io/en/latest/)) - `extension/src/
+intersections.cpp` defines the module interface using the `PYBIND11_MODULE`
+macro - `pyproject.toml` defines the build requirements for snail, which
+includes pybind11 and scikit-build-core
```

### Comparing `nismod-snail-0.3.1/docs/Makefile` & `nismod-snail-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/docs/source/api/snail.rst` & `nismod-snail-0.3.2/docs/source/api/snail.rst`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/docs/source/conf.py` & `nismod-snail-0.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/docs/source/index.rst` & `nismod-snail-0.3.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/examples.sh` & `nismod-snail-0.3.2/examples.sh`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/.clang-format` & `nismod-snail-0.3.2/extension/extern/Catch2/.clang-format`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/.conan/build.py` & `nismod-snail-0.3.2/extension/extern/Catch2/.conan/build.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/.conan/test_package/conanfile.py` & `nismod-snail-0.3.2/extension/extern/Catch2/.conan/test_package/conanfile.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/.gitattributes` & `nismod-snail-0.3.2/extension/extern/Catch2/.gitattributes`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/.github/ISSUE_TEMPLATE/bug_report.md` & `nismod-snail-0.3.2/extension/extern/Catch2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/.github/pull_request_template.md` & `nismod-snail-0.3.2/extension/extern/Catch2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/.gitignore` & `nismod-snail-0.3.2/extension/extern/Catch2/.gitignore`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/.travis.yml` & `nismod-snail-0.3.2/extension/extern/Catch2/.travis.yml`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/CMake/FindGcov.cmake` & `nismod-snail-0.3.2/extension/extern/Catch2/CMake/FindGcov.cmake`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/CMake/FindLcov.cmake` & `nismod-snail-0.3.2/extension/extern/Catch2/CMake/FindLcov.cmake`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/CMake/Findcodecov.cmake` & `nismod-snail-0.3.2/extension/extern/Catch2/CMake/Findcodecov.cmake`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/CMake/MiscFunctions.cmake` & `nismod-snail-0.3.2/extension/extern/Catch2/CMake/MiscFunctions.cmake`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/CMake/llvm-cov-wrapper` & `nismod-snail-0.3.2/extension/extern/Catch2/CMake/llvm-cov-wrapper`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/CMakeLists.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/CODE_OF_CONDUCT.md` & `nismod-snail-0.3.2/extension/extern/Catch2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/LICENSE.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/README.md` & `nismod-snail-0.3.2/extension/extern/Catch2/README.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/appveyor.yml` & `nismod-snail-0.3.2/extension/extern/Catch2/appveyor.yml`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/artwork/catch2-c-logo.png` & `nismod-snail-0.3.2/extension/extern/Catch2/artwork/catch2-c-logo.png`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/artwork/catch2-hand-logo.png` & `nismod-snail-0.3.2/extension/extern/Catch2/artwork/catch2-hand-logo.png`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/artwork/catch2-logo-small.png` & `nismod-snail-0.3.2/extension/extern/Catch2/artwork/catch2-logo-small.png`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/conanfile.py` & `nismod-snail-0.3.2/extension/extern/Catch2/conanfile.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/contrib/Catch.cmake` & `nismod-snail-0.3.2/extension/extern/Catch2/contrib/Catch.cmake`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/contrib/CatchAddTests.cmake` & `nismod-snail-0.3.2/extension/extern/Catch2/contrib/CatchAddTests.cmake`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/contrib/ParseAndAddCatchTests.cmake` & `nismod-snail-0.3.2/extension/extern/Catch2/contrib/ParseAndAddCatchTests.cmake`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/contrib/gdbinit` & `nismod-snail-0.3.2/extension/extern/Catch2/contrib/gdbinit`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/contrib/lldbinit` & `nismod-snail-0.3.2/extension/extern/Catch2/contrib/lldbinit`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/Readme.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/Readme.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/assertions.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/assertions.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/benchmarks.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/ci-and-misc.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/ci-and-misc.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/cmake-integration.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/cmake-integration.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/command-line.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/command-line.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/commercial-users.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/commercial-users.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/configuration.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/contributing.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/deprecations.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/deprecations.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/event-listeners.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/event-listeners.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/generators.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/generators.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/limitations.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/limitations.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/list-of-examples.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/list-of-examples.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/logging.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/logging.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/matchers.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/matchers.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/opensource-users.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/opensource-users.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/other-macros.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/other-macros.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/own-main.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/own-main.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/release-notes.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/release-notes.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/release-process.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/release-process.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/reporters.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/reporters.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/slow-compiles.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/slow-compiles.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/test-cases-and-sections.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/test-cases-and-sections.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/test-fixtures.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/test-fixtures.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/tostring.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/tostring.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/tutorial.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/docs/why-catch.md` & `nismod-snail-0.3.2/extension/extern/Catch2/docs/why-catch.md`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/010-TestCase.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/010-TestCase.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/020-TestCase-1.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/020-TestCase-1.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/020-TestCase-2.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/020-TestCase-2.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/030-Asn-Require-Check.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/030-Asn-Require-Check.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/100-Fix-Section.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/100-Fix-Section.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/110-Fix-ClassFixture.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/110-Fix-ClassFixture.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/120-Bdd-ScenarioGivenWhenThen.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/120-Bdd-ScenarioGivenWhenThen.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/200-Rpt-CatchMain.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/200-Rpt-CatchMain.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/207-Rpt-TeamCityReporter.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/207-Rpt-TeamCityReporter.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/210-Evt-EventListeners.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/210-Evt-EventListeners.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/231-Cfg-OutputStreams.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/231-Cfg-OutputStreams.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/300-Gen-OwnGenerator.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/300-Gen-OwnGenerator.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/301-Gen-MapTypeConversion.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/301-Gen-MapTypeConversion.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/302-Gen-Table.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/302-Gen-Table.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/310-Gen-VariablesInGenerators.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/310-Gen-VariablesInGenerators.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/311-Gen-CustomCapture.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/311-Gen-CustomCapture.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/examples/CMakeLists.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/catch.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/catch.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/external/clara.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/external/clara.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_benchmark.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_benchmark.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_benchmarking_all.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_benchmarking_all.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_chronometer.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_chronometer.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_clock.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_clock.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_constructor.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_constructor.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_environment.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_environment.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_estimate.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_estimate.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_execution_plan.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_execution_plan.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_optimizer.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_optimizer.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_outlier_classification.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_outlier_classification.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/catch_sample_analysis.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/catch_sample_analysis.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_analyse.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_analyse.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_benchmark_function.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_benchmark_function.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_complete_invoke.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_complete_invoke.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_estimate_clock.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_estimate_clock.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_measure.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_measure.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_repeat.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_repeat.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_run_for_at_least.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_run_for_at_least.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_stats.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_stats.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_stats.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_stats.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/benchmark/detail/catch_timing.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/benchmark/detail/catch_timing.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_approx.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_approx.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_approx.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_approx.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_assertionhandler.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_assertionhandler.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_assertionhandler.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_assertionhandler.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_assertioninfo.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_assertioninfo.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_assertionresult.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_assertionresult.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_assertionresult.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_assertionresult.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_capture.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_capture.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_capture_matchers.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_capture_matchers.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_capture_matchers.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_capture_matchers.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_clara.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_clara.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_commandline.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_commandline.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_commandline.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_commandline.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_common.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_common.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_common.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_common.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_compiler_capabilities.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_compiler_capabilities.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_config.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_config.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_config.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_config.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_config_uncaught_exceptions.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_config_uncaught_exceptions.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_console_colour.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_console_colour.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_console_colour.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_console_colour.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_context.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_context.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_context.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_context.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_debug_console.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_debug_console.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_debugger.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_debugger.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_debugger.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_debugger.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_decomposer.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_decomposer.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_decomposer.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_decomposer.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_default_main.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_default_main.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_enforce.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_enforce.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_enforce.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_enforce.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_enum_values_registry.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_enum_values_registry.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_enum_values_registry.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_enum_values_registry.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_exception_translator_registry.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_exception_translator_registry.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_exception_translator_registry.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_exception_translator_registry.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_external_interfaces.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_external_interfaces.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_fatal_condition.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_fatal_condition.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_fatal_condition.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_fatal_condition.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_generators.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_generators.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_generators.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_generators.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_generators_generic.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_generators_generic.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_generators_specific.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_generators_specific.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_impl.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_impl.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_capture.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_capture.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_config.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_config.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_enum_values_registry.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_enum_values_registry.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_exception.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_exception.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_generatortracker.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_generatortracker.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_registry_hub.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_registry_hub.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_reporter.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_reporter.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_reporter.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_reporter.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_runner.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_runner.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_tag_alias_registry.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_tag_alias_registry.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_interfaces_testcase.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_interfaces_testcase.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_leak_detector.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_leak_detector.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_list.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_list.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_list.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_list.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_exception.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_exception.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_exception.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_exception.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_floating.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_floating.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_floating.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_floating.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_generic.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_generic.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_string.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_string.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_string.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_string.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_matchers_vector.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_matchers_vector.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_message.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_message.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_message.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_message.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_meta.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_meta.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_objc.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_objc.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_objc_arc.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_objc_arc.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_option.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_option.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_output_redirect.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_output_redirect.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_output_redirect.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_output_redirect.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_platform.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_platform.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_polyfills.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_polyfills.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_preprocessor.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_preprocessor.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_random_number_generator.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_random_number_generator.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_random_number_generator.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_random_number_generator.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_reenable_warnings.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_reenable_warnings.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_registry_hub.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_registry_hub.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_reporter_registrars.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_reporter_registrars.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_reporter_registry.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_reporter_registry.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_reporter_registry.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_reporter_registry.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_result_type.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_result_type.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_result_type.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_result_type.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_run_context.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_run_context.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_run_context.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_run_context.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_section.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_section.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_section.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_section.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_section_info.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_section_info.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_session.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_session.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_session.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_session.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_singletons.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_singletons.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_singletons.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_singletons.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_startup_exception_registry.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_startup_exception_registry.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_startup_exception_registry.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_startup_exception_registry.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_stream.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_stream.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_stream.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_stream.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_string_manip.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_string_manip.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_string_manip.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_string_manip.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_stringref.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_stringref.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_stringref.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_stringref.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_suppress_warnings.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_suppress_warnings.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tag_alias.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tag_alias.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tag_alias_autoregistrar.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tag_alias_autoregistrar.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tag_alias_autoregistrar.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tag_alias_autoregistrar.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tag_alias_registry.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tag_alias_registry.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tag_alias_registry.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tag_alias_registry.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_info.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_info.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_info.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_info.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_registry_impl.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_registry_impl.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_registry_impl.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_registry_impl.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_tracker.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_tracker.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_case_tracker.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_case_tracker.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_registry.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_registry.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_registry.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_registry.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_spec.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_spec.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_spec.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_spec.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_spec_parser.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_spec_parser.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_test_spec_parser.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_test_spec_parser.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_timer.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_timer.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_timer.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_timer.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_to_string.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_to_string.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tostring.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tostring.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_tostring.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_tostring.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_totals.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_totals.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_totals.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_totals.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_uncaught_exceptions.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_uncaught_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_user_interfaces.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_user_interfaces.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_version.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_version.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_version.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_version.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_wildcard_pattern.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_wildcard_pattern.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_wildcard_pattern.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_wildcard_pattern.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_windows_h_proxy.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_windows_h_proxy.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_xmlwriter.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_xmlwriter.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/internal/catch_xmlwriter.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/internal/catch_xmlwriter.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_automake.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_automake.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_bases.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_bases.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_bases.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_bases.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_compact.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_compact.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_compact.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_compact.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_console.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_console.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_console.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_console.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_junit.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_junit.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_junit.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_junit.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_listening.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_listening.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_listening.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_listening.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_sonarqube.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_sonarqube.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_tap.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_tap.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_teamcity.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_teamcity.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_xml.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_xml.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/include/reporters/catch_reporter_xml.h` & `nismod-snail-0.3.2/extension/extern/Catch2/include/reporters/catch_reporter_xml.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/misc/appveyorBuildConfigurationScript.bat` & `nismod-snail-0.3.2/extension/extern/Catch2/misc/appveyorBuildConfigurationScript.bat`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/misc/appveyorTestRunScript.bat` & `nismod-snail-0.3.2/extension/extern/Catch2/misc/appveyorTestRunScript.bat`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/misc/coverage-helper.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/misc/coverage-helper.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/misc/installOpenCppCoverage.ps1` & `nismod-snail-0.3.2/extension/extern/Catch2/misc/installOpenCppCoverage.ps1`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/CMakeLists.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/CMakeLists.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/ToDo.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/ToDo.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X01-PrefixedMacros.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X01-PrefixedMacros.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X02-DisabledMacros.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X02-DisabledMacros.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X03-DisabledExceptions-DefaultHandler.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X03-DisabledExceptions-DefaultHandler.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X04-DisabledExceptions-CustomHandler.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X04-DisabledExceptions-CustomHandler.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/ExtraTests/X20-BenchmarkingMacros.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/ExtraTests/X20-BenchmarkingMacros.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/automake.std.approved.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/automake.std.approved.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/compact.sw.approved.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/compact.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/console.std.approved.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/console.std.approved.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/console.sw.approved.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/console.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/console.swa4.approved.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/console.swa4.approved.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/junit.sw.approved.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/junit.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/sonarqube.sw.approved.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/sonarqube.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/Baselines/xml.sw.approved.txt` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/Baselines/xml.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/CompileTimePerfTests/All.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/CompileTimePerfTests/All.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/CmdLine.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/CmdLine.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Details.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Details.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/GeneratorsImpl.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/GeneratorsImpl.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/InternalBenchmark.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/InternalBenchmark.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/PartTracker.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/PartTracker.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/RandomNumberGeneration.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/RandomNumberGeneration.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/String.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/String.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/StringManip.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/StringManip.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Tag.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Tag.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/ToString.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/ToString.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Xml.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/IntrospectiveTests/Xml.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/TestMain.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/TestMain.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/TimingTests/Sleep.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/TimingTests/Sleep.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Approx.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Approx.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/BDD.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/BDD.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Benchmark.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Benchmark.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Class.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Class.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Compilation.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Compilation.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Condition.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Condition.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Decomposition.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Decomposition.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/EnumToString.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/EnumToString.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Exception.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Exception.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Generators.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Generators.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Matchers.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Matchers.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Message.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Message.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Misc.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Misc.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringChrono.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringChrono.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringGeneral.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringGeneral.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringOptional.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringOptional.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringPair.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringPair.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringTuple.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringTuple.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringVariant.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringVariant.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringVector.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringVector.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringWhich.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/ToStringWhich.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/Tricky.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/Tricky.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/UsageTests/VariadicMacros.tests.cpp` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/UsageTests/VariadicMacros.tests.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/SelfTest/WarnAboutNoTests.cmake` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/SelfTest/WarnAboutNoTests.cmake`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/TestScripts/testRandomOrder.py` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/TestScripts/testRandomOrder.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/CatchOCTestCase.h` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/CatchOCTestCase.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/CatchOCTestCase.mm` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/CatchOCTestCase.mm`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/OCTest.1` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/OCTest.1`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/OCTest.mm` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/OCTest.mm`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest/TestObj.h` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest/TestObj.h`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/OCTest.xcodeproj/project.pbxproj` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/OCTest.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/projects/XCode/OCTest/catch_objc_impl.mm` & `nismod-snail-0.3.2/extension/extern/Catch2/projects/XCode/OCTest/catch_objc_impl.mm`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/approvalTests.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/approvalTests.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/approve.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/approve.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/benchmarkCompile.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/benchmarkCompile.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/benchmarkRunner.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/benchmarkRunner.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/embed.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/embed.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/embedClara.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/embedClara.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/extractFeaturesFromReleaseNotes.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/extractFeaturesFromReleaseNotes.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/fixWhitespace.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/fixWhitespace.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/generateSingleHeader.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/generateSingleHeader.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/releaseCommon.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/releaseCommon.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/releaseNotes.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/releaseNotes.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/scriptCommon.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/scriptCommon.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/updateDocumentToC.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/updateDocumentToC.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/scripts/updateWandbox.py` & `nismod-snail-0.3.2/extension/extern/Catch2/scripts/updateWandbox.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/single_include/catch2/catch.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/single_include/catch2/catch.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/single_include/catch2/catch_reporter_automake.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/single_include/catch2/catch_reporter_automake.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/single_include/catch2/catch_reporter_sonarqube.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/single_include/catch2/catch_reporter_sonarqube.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/single_include/catch2/catch_reporter_tap.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/single_include/catch2/catch_reporter_tap.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/single_include/catch2/catch_reporter_teamcity.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/single_include/catch2/catch_reporter_teamcity.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/extern/Catch2/third_party/clara.hpp` & `nismod-snail-0.3.2/extension/extern/Catch2/third_party/clara.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/src/geometry.hpp` & `nismod-snail-0.3.2/extension/src/geometry.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/src/grid.hpp` & `nismod-snail-0.3.2/extension/src/grid.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/src/intersections.cpp` & `nismod-snail-0.3.2/extension/src/intersections.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/src/operations.cpp` & `nismod-snail-0.3.2/extension/src/operations.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/src/operations.hpp` & `nismod-snail-0.3.2/extension/src/operations.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/src/transform.hpp` & `nismod-snail-0.3.2/extension/src/transform.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/src/utils.hpp` & `nismod-snail-0.3.2/extension/src/utils.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/tests/tests_intersections.cpp` & `nismod-snail-0.3.2/extension/tests/tests_intersections.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/extension/tests/tests_transform.cpp` & `nismod-snail-0.3.2/extension/tests/tests_transform.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/images/snail.svg` & `nismod-snail-0.3.2/images/snail.svg`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/pyproject.toml` & `nismod-snail-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="nismod-snail"
-version="0.3.1"
+version="0.3.2"
 license={file = "LICENSE"}
 description="The spatial networks impact assessment library"
 readme="README.md"
 authors=[
     {name="Tom Russell", email="tomalrussell@gmail.com"},
     {name="Thibault Lestang"},
     {name="Raghav Pant"},
```

### Comparing `nismod-snail-0.3.1/scripts/failure_analysis/fragility_damage_analysis.py` & `nismod-snail-0.3.2/scripts/failure_analysis/fragility_damage_analysis.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/failure_analysis/results_process_vietnam.py` & `nismod-snail-0.3.2/scripts/failure_analysis/results_process_vietnam.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/network_creation/spatial_and_network_functions.py` & `nismod-snail-0.3.2/scripts/network_creation/spatial_and_network_functions.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/network_hazard_intersections/hazards_network_intersections_results_collect.py` & `nismod-snail-0.3.2/scripts/network_hazard_intersections/hazards_network_intersections_results_collect.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/network_hazard_intersections/hazards_networks_intersections.py` & `nismod-snail-0.3.2/scripts/network_hazard_intersections/hazards_networks_intersections.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/network_hazard_intersections/intersection_networks.py` & `nismod-snail-0.3.2/scripts/network_hazard_intersections/intersection_networks.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/network_hazard_intersections/intersection_points.py` & `nismod-snail-0.3.2/scripts/network_hazard_intersections/intersection_points.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/network_hazard_intersections/intersection_polygons.py` & `nismod-snail-0.3.2/scripts/network_hazard_intersections/intersection_polygons.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/network_hazard_intersections/network_intersections.py` & `nismod-snail-0.3.2/scripts/network_hazard_intersections/network_intersections.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/sources_sinks_routing/benchmark_shortest_path.py` & `nismod-snail-0.3.2/scripts/sources_sinks_routing/benchmark_shortest_path.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/sources_sinks_routing/igraph.png` & `nismod-snail-0.3.2/scripts/sources_sinks_routing/igraph.png`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/sources_sinks_routing/pandana.png` & `nismod-snail-0.3.2/scripts/sources_sinks_routing/pandana.png`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/sources_sinks_routing/shortest_paths_igraph.py` & `nismod-snail-0.3.2/scripts/sources_sinks_routing/shortest_paths_igraph.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/scripts/sources_sinks_routing/shortest_paths_pandana.py` & `nismod-snail-0.3.2/scripts/sources_sinks_routing/shortest_paths_pandana.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/src/snail/cli.py` & `nismod-snail-0.3.2/src/snail/cli.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/src/snail/intersection.py` & `nismod-snail-0.3.2/src/snail/intersection.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,14 +169,15 @@
     # half-line pieces within the polygon interior, plus the boundary
     # split into pieces, then passed to shapely (GEOS) polygonize
     # - doesn't handle polygons with holes
     # - polygonize doesn't always piece back together correctly, or leaves
     #   gaps - perhaps especially for coarse grids (vs shape size)
     # - should be possible to write all at the lower level
     ##
+    polygon_features["split"] = 0
     for i in tqdm(range(len(polygon_features))):
         # split area
         geom_splits = split_polygon(
             polygon_features.geometry[i], t.width, t.height, t.transform
         )
         # round to high precision (avoid floating point errors)
         geom_splits = [
@@ -232,17 +233,22 @@
             to look up raster pixel. Indices must be stored under columns with
             names referenced by index_i and index_j.
         fname: Filename of raster file to read data from
     Returns:
         pd.Series: Series of raster values, with same row indexing as df.
     """
     # 2D numpy indexing is j, i (i.e. row, column)
-    return pandas.Series(
+    with_data = pandas.Series(
         index=features.index, data=data[features[index_j], features[index_i]]
     )
+    # set NaN for out-of-bounds
+    with_data[
+        (features[index_i] == -1) | (features[index_j] == -1)
+    ] = numpy.nan
+    return with_data
 
 
 def apply_indices(
     features: geopandas.GeoDataFrame,
     transform: Transform,
     index_i="index_i",
     index_j="index_j",
@@ -265,11 +271,11 @@
     i, j = get_cell_indices(geom, t.height, t.width, t.transform)
 
     # Raise error if cell index would be out of bounds
     # assert 0 <= i < t.width
     # assert 0 <= j < t.height
 
     # Or - special value (-1,-1) if cell would be out of bounds
-    if i > t.width or i < 0 or j > t.height or j < 0:
+    if i >= t.width or i < 0 or j >= t.height or j < 0:
         i = -1
         j = -1
     return pandas.Series(index=(index_i, index_j), data=[i, j])
```

### Comparing `nismod-snail-0.3.1/src/snail/io.py` & `nismod-snail-0.3.2/src/snail/io.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/src/snail/routing.py` & `nismod-snail-0.3.2/src/snail/routing.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tests/core/test_intersections.py` & `nismod-snail-0.3.2/tests/core/test_intersections.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tests/integration/climatology-hd35-annual-mean.tif` & `nismod-snail-0.3.2/tests/integration/climatology-hd35-annual-mean.tif`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tests/integration/climatology-hd35-historical.tif` & `nismod-snail-0.3.2/tests/integration/climatology-hd35-historical.tif`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tests/integration/inunriver_historical_WATCH_1980_rp01000.tif` & `nismod-snail-0.3.2/tests/integration/inunriver_historical_WATCH_1980_rp01000.tif`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tests/integration/lines.geojson` & `nismod-snail-0.3.2/tests/integration/lines.geojson`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tests/integration/points.geojson` & `nismod-snail-0.3.2/tests/integration/points.geojson`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tests/integration/polygons.geojson` & `nismod-snail-0.3.2/tests/integration/polygons.geojson`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tests/integration/range.tif` & `nismod-snail-0.3.2/tests/integration/range.tif`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tests/split_polygons_rings.py` & `nismod-snail-0.3.2/tests/split_polygons_rings.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tests/test_multi_intersections.py` & `nismod-snail-0.3.2/tests/test_multi_intersections.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tests/test_routing.py` & `nismod-snail-0.3.2/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tutorials/01-data-preparation-ghana.ipynb` & `nismod-snail-0.3.2/tutorials/01-data-preparation-ghana.ipynb`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tutorials/02-assess-damage-and-disruption.ipynb` & `nismod-snail-0.3.2/tutorials/02-assess-damage-and-disruption.ipynb`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tutorials/03-test-multiple-failures.ipynb` & `nismod-snail-0.3.2/tutorials/03-test-multiple-failures.ipynb`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/tutorials/04-evaluate-adaptation-options.ipynb` & `nismod-snail-0.3.2/tutorials/04-evaluate-adaptation-options.ipynb`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.3.1/PKG-INFO` & `nismod-snail-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nismod-snail
-Version: 0.3.1
+Version: 0.3.2
 Summary: The spatial networks impact assessment library
 Author: Thibault Lestang, Raghav Pant, Lena Fuldauer
 Author-Email: Tom Russell <tomalrussell@gmail.com>
 Maintainer-Email: Tom Russell <tomalrussell@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Tom Russell and snail contributors
@@ -219,25 +219,25 @@
 This may need some includes for `pybind11` - which will vary depending on your
 python installation. For example, with python via miniconda:
 
     clang-tidy --checks 'cppcoreguidelines-*' extension/src/* -- \
         -I/home/username/miniconda3/include/python3.11/ \
         -I./pybind11/include/
 
-Or with c++ headers installed on a Linux machine:
+Or with C++ headers installed on a Linux machine:
 
-    clang-tidy --checks 'cppcoreguidelines-*' \
-        extension/src/*  \
-        -- -std=c++11  -I/usr/include/x86_64-linux-gnu/c++/11 -I/usr/include/c++/11
+    clang-tidy --checks 'cppcoreguidelines-*' extension/src/* -- \
+        -std=c++14  \
+        -I/usr/include/x86_64-linux-gnu/c++/11 \
+        -I/usr/include/c++/11 \
+        -I{$PWD}/extension/extern/pybind11/include \
+        -I/usr/include/python3.10
 
 ### Integration of C++ and Python using pybind11
 
 The `snail.core.intersections` module is built using `pybind11` with
-`setuptools` (see [docs](https://pybind11.readthedocs.io/en/stable/compiling.html#building-with-setuptools))
+`scikit-build-core` (see [docs](https://scikit-build-core.readthedocs.io/en/latest/))
 
 - `extension/src/intersections.cpp` defines the module interface using the
   `PYBIND11_MODULE` macro
 - `pyproject.toml` defines the build requirements for snail, which includes
-  pybind11, wheel and setuptools
-- `setup.py` defines the `Pybind11Extension` module to build - both the C++
-  files to compile, and the location of the built module within the python
-  package
+  pybind11 and scikit-build-core
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nismod-snail Version: 0.3.1 Summary: The spatial
+Metadata-Version: 2.1 Name: nismod-snail Version: 0.3.2 Summary: The spatial
 networks impact assessment library Author: Thibault Lestang, Raghav Pant, Lena
 Fuldauer Author-Email: Tom Russell
 gmail.com> Maintainer-Email: Tom Russell
 gmail.com> License: MIT License Copyright (c) 2020 Tom Russell and snail
 contributors Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
@@ -89,18 +89,17 @@
 update --init --recursive Build the library and run tests: cmake -Bbuild ./
 extension cmake --build build/ ./build/run_tests Run code style auto-
 formatting: clang-format -i extension/src/*.{cpp,hpp} Run lints and checks:
 clang-tidy --checks 'cppcoreguidelines-*' extension/src/*.{cpp,hpp} This may
 need some includes for `pybind11` - which will vary depending on your python
 installation. For example, with python via miniconda: clang-tidy --checks
 'cppcoreguidelines-*' extension/src/* -- \ -I/home/username/miniconda3/include/
-python3.11/ \ -I./pybind11/include/ Or with c++ headers installed on a Linux
-machine: clang-tidy --checks 'cppcoreguidelines-*' \ extension/src/* \ -- -
-std=c++11 -I/usr/include/x86_64-linux-gnu/c++/11 -I/usr/include/c++/11 ###
+python3.11/ \ -I./pybind11/include/ Or with C++ headers installed on a Linux
+machine: clang-tidy --checks 'cppcoreguidelines-*' extension/src/* -- \ -
+std=c++14 \ -I/usr/include/x86_64-linux-gnu/c++/11 \ -I/usr/include/c++/11 \ -I
+{$PWD}/extension/extern/pybind11/include \ -I/usr/include/python3.10 ###
 Integration of C++ and Python using pybind11 The `snail.core.intersections`
-module is built using `pybind11` with `setuptools` (see [docs](https://
-pybind11.readthedocs.io/en/stable/compiling.html#building-with-setuptools)) -
-`extension/src/intersections.cpp` defines the module interface using the
-`PYBIND11_MODULE` macro - `pyproject.toml` defines the build requirements for
-snail, which includes pybind11, wheel and setuptools - `setup.py` defines the
-`Pybind11Extension` module to build - both the C++ files to compile, and the
-location of the built module within the python package
+module is built using `pybind11` with `scikit-build-core` (see [docs](https://
+scikit-build-core.readthedocs.io/en/latest/)) - `extension/src/
+intersections.cpp` defines the module interface using the `PYBIND11_MODULE`
+macro - `pyproject.toml` defines the build requirements for snail, which
+includes pybind11 and scikit-build-core
```

