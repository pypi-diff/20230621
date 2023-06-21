# Comparing `tmp/uproot-5.0.8.tar.gz` & `tmp/uproot-5.0.9.tar.gz`

## Comparing `uproot-5.0.8.tar` & `uproot-5.0.9.tar`

### file list

```diff
@@ -1,238 +1,238 @@
--rw-r--r--   0        0        0    13217 2020-02-02 00:00:00.000000 uproot-5.0.8/.all-contributorsrc
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 uproot-5.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 uproot-5.0.8/.readthedocs.yml
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.0.8/CITATION.cff
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/workflows/build-test.yml
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/workflows/semantic-pr-title.yml
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 uproot-5.0.8/dev/example-objects.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 uproot-5.0.8/dev/make-models.py
--rw-r--r--   0        0        0    95009 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/diagrams/abstraction-layers.png
--rw-r--r--   0        0        0    39940 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/diagrams/abstraction-layers.svg
--rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/diagrams/example-dask-graph.png
--rw-r--r--   0        0        0    70413 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/diagrams/uproot-awkward-timeline.png
--rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/diagrams/uproot-awkward-timeline.svg
--rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/logo/logo.svg
--rw-r--r--   0        0        0   223219 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/photos/switcheroo.jpg
--rw-r--r--   0        0        0    69252 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/basic.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/conf.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/index.rst
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/make_changelog.py
--rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/prepare_docstrings.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/requirements.txt
--rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/uproot3-to-4.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/_templates/breadcrumbs.html
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/__init__.py
--rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/_awkward_forth.py
--rw-r--r--   0        0        0    41220 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/_dask.py
--rw-r--r--   0        0        0    34514 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/_util.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behavior.py
--rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/cache.py
--rw-r--r--   0        0        0    16839 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/compression.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/const.py
--rw-r--r--   0        0        0    71187 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/containers.py
--rw-r--r--   0        0        0    20423 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/deserialization.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/dynamic.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/exceptions.py
--rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/extras.py
--rw-r--r--   0        0        0    65811 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/model.py
--rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/pyroot.py
--rw-r--r--   0        0        0    98265 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/reading.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/serialization.py
--rw-r--r--   0        0        0    69210 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/streamers.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/version.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/RooCurve.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/RooHist.py
--rw-r--r--   0        0        0    10049 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TAxis.py
--rw-r--r--   0        0        0   130424 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TBranch.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TBranchElement.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TDatime.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TGraph.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TGraphAsymmErrors.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TGraphErrors.py
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TH1.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TH2.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TH2Poly.py
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TH3.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TParameter.py
--rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TProfile.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TProfile2D.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TProfile3D.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TTree.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/__init__.py
--rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/__init__.py
--rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/grouped.py
--rw-r--r--   0        0        0    40728 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/identify.py
--rw-r--r--   0        0        0    14973 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/jagged.py
--rw-r--r--   0        0        0    37252 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/library.py
--rw-r--r--   0        0        0    23068 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/numerical.py
--rw-r--r--   0        0        0    34143 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/objects.py
--rw-r--r--   0        0        0    18835 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/strings.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/language/__init__.py
--rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/language/python.py
--rw-r--r--   0        0        0    25744 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/RNTuple.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TArray.py
--rw-r--r--   0        0        0    25379 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TAtt.py
--rw-r--r--   0        0        0    11179 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TBasket.py
--rw-r--r--   0        0        0    37043 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TBranch.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TClonesArray.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TDatime.py
--rw-r--r--   0        0        0    35595 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TGraph.py
--rw-r--r--   0        0        0   213682 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TH.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/THashList.py
--rw-r--r--   0        0        0    33898 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TLeaf.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TList.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TMatrixT.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TNamed.py
--rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TObjArray.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TObjString.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TObject.py
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TRef.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TString.py
--rw-r--r--   0        0        0     7255 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TTable.py
--rw-r--r--   0        0        0    46956 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TTree.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/sink/__init__.py
--rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/sink/file.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/__init__.py
--rw-r--r--   0        0        0    16003 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/chunk.py
--rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/cursor.py
--rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/file.py
--rw-r--r--   0        0        0    14154 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/futures.py
--rw-r--r--   0        0        0    25910 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/http.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/object.py
--rw-r--r--   0        0        0    15697 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/xrootd.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/__init__.py
--rw-r--r--   0        0        0    82851 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/_cascade.py
--rw-r--r--   0        0        0    31855 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/_cascadentuple.py
--rw-r--r--   0        0        0    56422 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/_cascadetree.py
--rw-r--r--   0        0        0    79676 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/identify.py
--rw-r--r--   0        0        0    80251 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/writable.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/__init__.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/conftest.py
--rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0001-source-class.py
--rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0006-notify-when-downloaded.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0007-single-chunk-interface.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0008-start-interpretation.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0009-nested-directories.py
--rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0010-start-streamers.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0011-generate-classes-from-streamers.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0013-rntuple-anchor.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0014-all-ttree-versions.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0016-interpretations.py
--rw-r--r--   0        0        0     9682 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0017-multi-basket-multi-branch-fetch.py
--rw-r--r--   0        0        0    33935 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0018-array-fetching-interface.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0022-number-of-branches.py
--rw-r--r--   0        0        0    13960 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0023-more-interpretations-1.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0023-ttree-versions.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0028-fallback-to-read-streamer.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0029-more-string-types.py
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0031-test-stl-containers.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0033-more-interpretations-2.py
--rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0034-generic-objects-in-ttrees.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0035-datatype-generality.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0038-memberwise-serialization.py
--rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0043-iterate-function.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0044-concatenate-function.py
--rw-r--r--   0        0        0    68981 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0046-histograms-bh-hist.py
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0053-parents-should-not-be-bases.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0058-detach-model-objects-from-files.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0066-fix-http-fallback-freeze.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0067-common-entry-offsets.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0081-dont-parse-colons.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0087-memberwise-splitting-not-implemented-messages.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0088-read-with-http.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0099-read-from-file-object.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0112-fix-pandas-with-cut.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0118-fix-name-fetch-again.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0123-atlas-issues.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0126-turn-unknown-emptyarrays-into-known-types.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0167-use-the-common-histogram-interface.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0172-allow-allocators-in-vector-typenames.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0173-empty-and-multiprocessing-bugs.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0182-complain-about-missing-files.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0194-fix-lost-cuts-in-iterate.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0220-contiguous-byte-ranges-in-http.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0228_read-TProfiles.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0240-read_TGraphAsymmErrors.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0278-specializations-for-TParameter.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0302-pickle.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0303-empty-jagged-array.py
--rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0320-start-working-on-ROOT-writing.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0322-writablefile-infrastructure.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0325-fix-windows-file-uris.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0329-update-existing-root-files.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0335-empty-ttree-division-by-zero.py
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0341-manipulate-streamer-info.py
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0344-writabledirectory-can-read.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0345-bulk-copy-method.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0349-write-TObjString.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0350-read-RooCurve-RooHist.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0351-write-TList.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0352-write-THashList.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0384-move-behavior_of-and-fix-383.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0398-dimensions-in-leaflist.py
--rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0405-write-a-histogram.py
--rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0406-write-a-ttree.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0407-read-TDatime.py
--rw-r--r--   0        0        0    17062 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0412-write-multidimensional-numpy-to-ttree.py
--rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0414-write-jagged-arrays.py
--rw-r--r--   0        0        0    16674 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0416-writing-compressed-data.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0418-read-TTable.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0420-pyroot-uproot-interoperability.py
--rw-r--r--   0        0        0    17479 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0422-hist-integration.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0430-global_index-for-tuples-of-DataFrames.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0438-TClonesArray-is-not-AsGrouped.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0439-check-awkward-before-numpy.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0442-regular-TClonesArray.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0472-tstreamerinfo-for-ttree.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0475-remember-to-update-freesegments.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0484-manually-add-model-for-TMatrixTSym_double_.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0487-implement-asdtypeinplace.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0498-create-leaf-branch-in-extend.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0519-remove-memmap-copy.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0520-dynamic-classes-cant-be-abc-subclasses.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0569-fBits-is-4-bytes.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0576-unicode-in-names.py
--rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0578-dask-for-numpy.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0580-round-trip-for-no-flow-histograms.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0589-explicitly-interpret-RVec-type.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0603-dask-delayed-open.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0609-num-enteries-func.py
--rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0610-awkward-form.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0630-rntuple-basics.py
--rw-r--r--   0        0        0    58430 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0637-setup-tests-for-AwkwardForth.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0643-reading-vector-pair-TLorentzVector-int.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0651-implement-transformed-axis.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0652_dask-for-awkward.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0662-rntuple-stl-containers.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0700-dask-empty-arrays.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0705-rntuple-writing-metadata.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0750-avoid-empty-TBasket-issue.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0755-dask-awkward-column-projection.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0791-protect-uproot-project_columns-from-dask-node-names.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0798_DAOD_PHYSLITE.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0808-fix_awkward_form_for_AsStridedObjects.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0816-separate-AwkwardForth-machines-by-TBranch.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0832-ak_add_doc-should-also-add-to-typetracer.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0840-support-tleafG.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0841-fix-814.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0844-fix-delete-hist-from-root.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0852-fix-strided-interp-extra-offsets.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0870-writing-arrays-of-type-unknown-fix-822.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0876-uproot-dask-blind-steps.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0886-fix-awkward-form-breadcrumbs.py
--rw-r--r--   0        0        0   128147 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/samples/h_dynamic.pkl
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 uproot-5.0.8/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 uproot-5.0.8/LICENSE
--rw-r--r--   0        0        0    25899 2020-02-02 00:00:00.000000 uproot-5.0.8/README.md
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 uproot-5.0.8/pyproject.toml
--rw-r--r--   0        0        0    28208 2020-02-02 00:00:00.000000 uproot-5.0.8/PKG-INFO
+-rw-r--r--   0        0        0    13217 2020-02-02 00:00:00.000000 uproot-5.0.9/.all-contributorsrc
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 uproot-5.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 uproot-5.0.9/.readthedocs.yml
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.0.9/CITATION.cff
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 uproot-5.0.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 uproot-5.0.9/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 uproot-5.0.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 uproot-5.0.9/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 uproot-5.0.9/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 uproot-5.0.9/.github/workflows/build-test.yml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 uproot-5.0.9/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 uproot-5.0.9/.github/workflows/semantic-pr-title.yml
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 uproot-5.0.9/dev/example-objects.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 uproot-5.0.9/dev/make-models.py
+-rw-r--r--   0        0        0    95009 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-img/diagrams/abstraction-layers.png
+-rw-r--r--   0        0        0    39940 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-img/diagrams/abstraction-layers.svg
+-rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-img/diagrams/example-dask-graph.png
+-rw-r--r--   0        0        0    70413 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-img/diagrams/uproot-awkward-timeline.png
+-rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-img/diagrams/uproot-awkward-timeline.svg
+-rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0   223219 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-img/photos/switcheroo.jpg
+-rw-r--r--   0        0        0    69252 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-sphinx/basic.rst
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-sphinx/conf.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-sphinx/index.rst
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-sphinx/make_changelog.py
+-rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-sphinx/prepare_docstrings.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-sphinx/requirements.txt
+-rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-sphinx/uproot3-to-4.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 uproot-5.0.9/docs-sphinx/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/__init__.py
+-rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/_awkward_forth.py
+-rw-r--r--   0        0        0    41600 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/_dask.py
+-rw-r--r--   0        0        0    34514 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/_util.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behavior.py
+-rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/cache.py
+-rw-r--r--   0        0        0    16839 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/compression.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/const.py
+-rw-r--r--   0        0        0    71187 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/containers.py
+-rw-r--r--   0        0        0    20423 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/deserialization.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/dynamic.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/exceptions.py
+-rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/extras.py
+-rw-r--r--   0        0        0    65811 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/model.py
+-rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/pyroot.py
+-rw-r--r--   0        0        0    98265 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/reading.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/serialization.py
+-rw-r--r--   0        0        0    69210 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/streamers.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/version.py
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/RooCurve.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/RooHist.py
+-rw-r--r--   0        0        0    10049 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TAxis.py
+-rw-r--r--   0        0        0   130424 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TBranch.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TBranchElement.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TDatime.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TGraph.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TGraphAsymmErrors.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TGraphErrors.py
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TH1.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TH2.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TH2Poly.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TH3.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TParameter.py
+-rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TProfile.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TProfile2D.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TProfile3D.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/TTree.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/behaviors/__init__.py
+-rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/interpretation/__init__.py
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/interpretation/grouped.py
+-rw-r--r--   0        0        0    40728 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/interpretation/identify.py
+-rw-r--r--   0        0        0    14973 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/interpretation/jagged.py
+-rw-r--r--   0        0        0    37252 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/interpretation/library.py
+-rw-r--r--   0        0        0    23068 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/interpretation/numerical.py
+-rw-r--r--   0        0        0    34143 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/interpretation/objects.py
+-rw-r--r--   0        0        0    18835 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/interpretation/strings.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/language/__init__.py
+-rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/language/python.py
+-rw-r--r--   0        0        0    25744 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/RNTuple.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TArray.py
+-rw-r--r--   0        0        0    25379 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TAtt.py
+-rw-r--r--   0        0        0    11179 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TBasket.py
+-rw-r--r--   0        0        0    37043 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TBranch.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TClonesArray.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TDatime.py
+-rw-r--r--   0        0        0    35595 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TGraph.py
+-rw-r--r--   0        0        0   213682 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TH.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/THashList.py
+-rw-r--r--   0        0        0    33898 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TLeaf.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TList.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TMatrixT.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TNamed.py
+-rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TObjArray.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TObjString.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TObject.py
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TRef.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TString.py
+-rw-r--r--   0        0        0     7255 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TTable.py
+-rw-r--r--   0        0        0    46956 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/TTree.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/models/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/sink/__init__.py
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/sink/file.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/source/__init__.py
+-rw-r--r--   0        0        0    16003 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/source/chunk.py
+-rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/source/cursor.py
+-rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/source/file.py
+-rw-r--r--   0        0        0    14154 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/source/futures.py
+-rw-r--r--   0        0        0    25910 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/source/http.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/source/object.py
+-rw-r--r--   0        0        0    15697 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/source/xrootd.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/writing/__init__.py
+-rw-r--r--   0        0        0    82851 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/writing/_cascade.py
+-rw-r--r--   0        0        0    31855 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/writing/_cascadentuple.py
+-rw-r--r--   0        0        0    56422 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/writing/_cascadetree.py
+-rw-r--r--   0        0        0    79676 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/writing/identify.py
+-rw-r--r--   0        0        0    80251 2020-02-02 00:00:00.000000 uproot-5.0.9/src/uproot/writing/writable.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/conftest.py
+-rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0001-source-class.py
+-rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0006-notify-when-downloaded.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0007-single-chunk-interface.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0008-start-interpretation.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0009-nested-directories.py
+-rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0010-start-streamers.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0011-generate-classes-from-streamers.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0013-rntuple-anchor.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0014-all-ttree-versions.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0016-interpretations.py
+-rw-r--r--   0        0        0     9682 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0017-multi-basket-multi-branch-fetch.py
+-rw-r--r--   0        0        0    33935 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0018-array-fetching-interface.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0022-number-of-branches.py
+-rw-r--r--   0        0        0    13960 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0023-more-interpretations-1.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0023-ttree-versions.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0028-fallback-to-read-streamer.py
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0029-more-string-types.py
+-rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0031-test-stl-containers.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0033-more-interpretations-2.py
+-rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0034-generic-objects-in-ttrees.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0035-datatype-generality.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0038-memberwise-serialization.py
+-rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0043-iterate-function.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0044-concatenate-function.py
+-rw-r--r--   0        0        0    68981 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0046-histograms-bh-hist.py
+-rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0053-parents-should-not-be-bases.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0058-detach-model-objects-from-files.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0066-fix-http-fallback-freeze.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0067-common-entry-offsets.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0081-dont-parse-colons.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0087-memberwise-splitting-not-implemented-messages.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0088-read-with-http.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0099-read-from-file-object.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0112-fix-pandas-with-cut.py
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0118-fix-name-fetch-again.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0123-atlas-issues.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0126-turn-unknown-emptyarrays-into-known-types.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0167-use-the-common-histogram-interface.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0172-allow-allocators-in-vector-typenames.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0173-empty-and-multiprocessing-bugs.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0182-complain-about-missing-files.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0194-fix-lost-cuts-in-iterate.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0220-contiguous-byte-ranges-in-http.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0228_read-TProfiles.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0240-read_TGraphAsymmErrors.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0278-specializations-for-TParameter.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0302-pickle.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0303-empty-jagged-array.py
+-rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0320-start-working-on-ROOT-writing.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0322-writablefile-infrastructure.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0325-fix-windows-file-uris.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0329-update-existing-root-files.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0335-empty-ttree-division-by-zero.py
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0341-manipulate-streamer-info.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0344-writabledirectory-can-read.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0345-bulk-copy-method.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0349-write-TObjString.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0350-read-RooCurve-RooHist.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0351-write-TList.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0352-write-THashList.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0384-move-behavior_of-and-fix-383.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0398-dimensions-in-leaflist.py
+-rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0405-write-a-histogram.py
+-rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0406-write-a-ttree.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0407-read-TDatime.py
+-rw-r--r--   0        0        0    17062 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0412-write-multidimensional-numpy-to-ttree.py
+-rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0414-write-jagged-arrays.py
+-rw-r--r--   0        0        0    16674 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0416-writing-compressed-data.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0418-read-TTable.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0420-pyroot-uproot-interoperability.py
+-rw-r--r--   0        0        0    17479 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0422-hist-integration.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0430-global_index-for-tuples-of-DataFrames.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0438-TClonesArray-is-not-AsGrouped.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0439-check-awkward-before-numpy.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0442-regular-TClonesArray.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0472-tstreamerinfo-for-ttree.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0475-remember-to-update-freesegments.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0484-manually-add-model-for-TMatrixTSym_double_.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0487-implement-asdtypeinplace.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0498-create-leaf-branch-in-extend.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0519-remove-memmap-copy.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0520-dynamic-classes-cant-be-abc-subclasses.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0569-fBits-is-4-bytes.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0576-unicode-in-names.py
+-rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0578-dask-for-numpy.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0580-round-trip-for-no-flow-histograms.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0589-explicitly-interpret-RVec-type.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0603-dask-delayed-open.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0609-num-enteries-func.py
+-rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0610-awkward-form.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0630-rntuple-basics.py
+-rw-r--r--   0        0        0    58430 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0637-setup-tests-for-AwkwardForth.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0643-reading-vector-pair-TLorentzVector-int.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0651-implement-transformed-axis.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0652_dask-for-awkward.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0662-rntuple-stl-containers.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0700-dask-empty-arrays.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0705-rntuple-writing-metadata.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0750-avoid-empty-TBasket-issue.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0755-dask-awkward-column-projection.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0791-protect-uproot-project_columns-from-dask-node-names.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0798_DAOD_PHYSLITE.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0808-fix_awkward_form_for_AsStridedObjects.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0816-separate-AwkwardForth-machines-by-TBranch.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0832-ak_add_doc-should-also-add-to-typetracer.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0840-support-tleafG.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0841-fix-814.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0844-fix-delete-hist-from-root.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0852-fix-strided-interp-extra-offsets.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0870-writing-arrays-of-type-unknown-fix-822.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0876-uproot-dask-blind-steps.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/test_0886-fix-awkward-form-breadcrumbs.py
+-rw-r--r--   0        0        0   128147 2020-02-02 00:00:00.000000 uproot-5.0.9/tests/samples/h_dynamic.pkl
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 uproot-5.0.9/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 uproot-5.0.9/LICENSE
+-rw-r--r--   0        0        0    25899 2020-02-02 00:00:00.000000 uproot-5.0.9/README.md
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 uproot-5.0.9/pyproject.toml
+-rw-r--r--   0        0        0    28208 2020-02-02 00:00:00.000000 uproot-5.0.9/PKG-INFO
```

### Comparing `uproot-5.0.8/.all-contributorsrc` & `uproot-5.0.9/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/.pre-commit-config.yaml` & `uproot-5.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/CITATION.cff` & `uproot-5.0.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/.github/ISSUE_TEMPLATE/bug-report.md` & `uproot-5.0.9/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/.github/ISSUE_TEMPLATE/feature-request.md` & `uproot-5.0.9/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/.github/workflows/build-test.yml` & `uproot-5.0.9/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/.github/workflows/deploy.yml` & `uproot-5.0.9/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/dev/example-objects.py` & `uproot-5.0.9/dev/example-objects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/dev/make-models.py` & `uproot-5.0.9/dev/make-models.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-img/diagrams/abstraction-layers.png` & `uproot-5.0.9/docs-img/diagrams/abstraction-layers.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-img/diagrams/abstraction-layers.svg` & `uproot-5.0.9/docs-img/diagrams/abstraction-layers.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-img/diagrams/example-dask-graph.png` & `uproot-5.0.9/docs-img/diagrams/example-dask-graph.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-img/diagrams/uproot-awkward-timeline.png` & `uproot-5.0.9/docs-img/diagrams/uproot-awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-img/diagrams/uproot-awkward-timeline.svg` & `uproot-5.0.9/docs-img/diagrams/uproot-awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-img/logo/logo-300px-white.png` & `uproot-5.0.9/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-img/logo/logo-300px.png` & `uproot-5.0.9/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-img/logo/logo-600px.png` & `uproot-5.0.9/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-img/logo/logo.svg` & `uproot-5.0.9/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-img/photos/switcheroo.jpg` & `uproot-5.0.9/docs-img/photos/switcheroo.jpg`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-sphinx/basic.rst` & `uproot-5.0.9/docs-sphinx/basic.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-sphinx/conf.py` & `uproot-5.0.9/docs-sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-sphinx/index.rst` & `uproot-5.0.9/docs-sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-sphinx/make_changelog.py` & `uproot-5.0.9/docs-sphinx/make_changelog.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-sphinx/prepare_docstrings.py` & `uproot-5.0.9/docs-sphinx/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/docs-sphinx/uproot3-to-4.rst` & `uproot-5.0.9/docs-sphinx/uproot3-to-4.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/__init__.py` & `uproot-5.0.9/src/uproot/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/_awkward_forth.py` & `uproot-5.0.9/src/uproot/_awkward_forth.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/_dask.py` & `uproot-5.0.9/src/uproot/_dask.py`

 * *Files 2% similar despite different names*

```diff
@@ -761,15 +761,18 @@
 
     def __call__(self, i_start_stop):
         i, start, stop = i_start_stop
 
         if self.form_mapping is not None:
             awkward = uproot.extras.awkward()
 
-            actual_form = self.rendered_form.select_columns(self.common_keys)
+            if set(self.common_keys) != set(self.rendered_form.columns()):
+                actual_form = self.rendered_form.select_columns(self.common_keys)
+            else:
+                actual_form = self.rendered_form
 
             mapping, buffer_key = self.form_mapping.create_column_mapping_and_key(
                 self.ttrees[i], start, stop, self.interp_options
             )
 
             return awkward.from_buffers(
                 actual_form,
@@ -876,15 +879,18 @@
 
 which has {num_entries} entries"""
             )
 
         if self.form_mapping is not None:
             awkward = uproot.extras.awkward()
 
-            actual_form = self.rendered_form.select_columns(self.common_keys)
+            if set(self.common_keys) != set(self.rendered_form.columns()):
+                actual_form = self.rendered_form.select_columns(self.common_keys)
+            else:
+                actual_form = self.rendered_form
 
             mapping, buffer_key = self.form_mapping.create_column_mapping_and_key(
                 ttree, start, stop, self.interp_options
             )
 
             return awkward.from_buffers(
                 actual_form,
@@ -1135,15 +1141,15 @@
     if len(partition_args) == 0:
         divisions.append(0)
         partition_args.append((0, 0, 0))
 
     return dask_awkward.from_map(
         _UprootRead(
             ttrees,
-            common_keys,
+            common_keys if form_mapping is None else form.columns(),
             common_keys,
             interp_options,
             form_mapping=form_mapping,
             rendered_form=None if form_mapping is None else form,
         ),
         partition_args,
         divisions=tuple(divisions),
@@ -1226,15 +1232,15 @@
                 )
 
     return dask_awkward.from_map(
         _UprootOpenAndRead(
             custom_classes,
             allow_missing,
             real_options,
-            common_keys,
+            common_keys if form_mapping is None else form.columns(),
             common_keys,
             interp_options,
             form_mapping=form_mapping,
             rendered_form=None if form_mapping is None else form,
         ),
         partition_args,
         divisions=None if divisions is None else tuple(divisions),
```

### Comparing `uproot-5.0.8/src/uproot/_util.py` & `uproot-5.0.9/src/uproot/_util.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behavior.py` & `uproot-5.0.9/src/uproot/behavior.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/cache.py` & `uproot-5.0.9/src/uproot/cache.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/compression.py` & `uproot-5.0.9/src/uproot/compression.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/const.py` & `uproot-5.0.9/src/uproot/const.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/containers.py` & `uproot-5.0.9/src/uproot/containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/deserialization.py` & `uproot-5.0.9/src/uproot/deserialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/dynamic.py` & `uproot-5.0.9/src/uproot/dynamic.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/exceptions.py` & `uproot-5.0.9/src/uproot/exceptions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/extras.py` & `uproot-5.0.9/src/uproot/extras.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/model.py` & `uproot-5.0.9/src/uproot/model.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/pyroot.py` & `uproot-5.0.9/src/uproot/pyroot.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/reading.py` & `uproot-5.0.9/src/uproot/reading.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/serialization.py` & `uproot-5.0.9/src/uproot/serialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/streamers.py` & `uproot-5.0.9/src/uproot/streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/RooCurve.py` & `uproot-5.0.9/src/uproot/behaviors/RooCurve.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/RooHist.py` & `uproot-5.0.9/src/uproot/behaviors/RooHist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TAxis.py` & `uproot-5.0.9/src/uproot/behaviors/TAxis.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TBranch.py` & `uproot-5.0.9/src/uproot/behaviors/TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TBranchElement.py` & `uproot-5.0.9/src/uproot/behaviors/TBranchElement.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TGraph.py` & `uproot-5.0.9/src/uproot/behaviors/TGraph.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TGraphAsymmErrors.py` & `uproot-5.0.9/src/uproot/behaviors/TGraphAsymmErrors.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TH1.py` & `uproot-5.0.9/src/uproot/behaviors/TH1.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TH2.py` & `uproot-5.0.9/src/uproot/behaviors/TH2.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TH2Poly.py` & `uproot-5.0.9/src/uproot/behaviors/TH2Poly.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TH3.py` & `uproot-5.0.9/src/uproot/behaviors/TH3.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TParameter.py` & `uproot-5.0.9/src/uproot/behaviors/TParameter.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TProfile.py` & `uproot-5.0.9/src/uproot/behaviors/TProfile.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TProfile2D.py` & `uproot-5.0.9/src/uproot/behaviors/TProfile2D.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TProfile3D.py` & `uproot-5.0.9/src/uproot/behaviors/TProfile3D.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/TTree.py` & `uproot-5.0.9/src/uproot/behaviors/TTree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/behaviors/__init__.py` & `uproot-5.0.9/src/uproot/behaviors/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/interpretation/__init__.py` & `uproot-5.0.9/src/uproot/interpretation/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/interpretation/grouped.py` & `uproot-5.0.9/src/uproot/interpretation/grouped.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/interpretation/identify.py` & `uproot-5.0.9/src/uproot/interpretation/identify.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/interpretation/jagged.py` & `uproot-5.0.9/src/uproot/interpretation/jagged.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/interpretation/library.py` & `uproot-5.0.9/src/uproot/interpretation/library.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/interpretation/numerical.py` & `uproot-5.0.9/src/uproot/interpretation/numerical.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/interpretation/objects.py` & `uproot-5.0.9/src/uproot/interpretation/objects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/interpretation/strings.py` & `uproot-5.0.9/src/uproot/interpretation/strings.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/language/__init__.py` & `uproot-5.0.9/src/uproot/language/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/language/python.py` & `uproot-5.0.9/src/uproot/language/python.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/RNTuple.py` & `uproot-5.0.9/src/uproot/models/RNTuple.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TArray.py` & `uproot-5.0.9/src/uproot/models/TArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TAtt.py` & `uproot-5.0.9/src/uproot/models/TAtt.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TBasket.py` & `uproot-5.0.9/src/uproot/models/TBasket.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TBranch.py` & `uproot-5.0.9/src/uproot/models/TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TClonesArray.py` & `uproot-5.0.9/src/uproot/models/TClonesArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TDatime.py` & `uproot-5.0.9/src/uproot/models/TDatime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TGraph.py` & `uproot-5.0.9/src/uproot/models/TGraph.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TH.py` & `uproot-5.0.9/src/uproot/models/TH.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/THashList.py` & `uproot-5.0.9/src/uproot/models/THashList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TLeaf.py` & `uproot-5.0.9/src/uproot/models/TLeaf.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TList.py` & `uproot-5.0.9/src/uproot/models/TList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TMatrixT.py` & `uproot-5.0.9/src/uproot/models/TMatrixT.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TNamed.py` & `uproot-5.0.9/src/uproot/models/TNamed.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TObjArray.py` & `uproot-5.0.9/src/uproot/models/TObjArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TObjString.py` & `uproot-5.0.9/src/uproot/models/TObjString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TObject.py` & `uproot-5.0.9/src/uproot/models/TObject.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TRef.py` & `uproot-5.0.9/src/uproot/models/TRef.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TString.py` & `uproot-5.0.9/src/uproot/models/TString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TTable.py` & `uproot-5.0.9/src/uproot/models/TTable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/TTree.py` & `uproot-5.0.9/src/uproot/models/TTree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/models/__init__.py` & `uproot-5.0.9/src/uproot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/sink/__init__.py` & `uproot-5.0.9/src/uproot/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/sink/file.py` & `uproot-5.0.9/src/uproot/sink/file.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/source/__init__.py` & `uproot-5.0.9/src/uproot/source/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/source/chunk.py` & `uproot-5.0.9/src/uproot/source/chunk.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/source/cursor.py` & `uproot-5.0.9/src/uproot/source/cursor.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/source/file.py` & `uproot-5.0.9/src/uproot/source/file.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/source/futures.py` & `uproot-5.0.9/src/uproot/source/futures.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/source/http.py` & `uproot-5.0.9/src/uproot/source/http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/source/object.py` & `uproot-5.0.9/src/uproot/source/object.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/source/xrootd.py` & `uproot-5.0.9/src/uproot/source/xrootd.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/writing/__init__.py` & `uproot-5.0.9/src/uproot/writing/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/writing/_cascade.py` & `uproot-5.0.9/src/uproot/writing/_cascade.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/writing/_cascadentuple.py` & `uproot-5.0.9/src/uproot/writing/_cascadentuple.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/writing/_cascadetree.py` & `uproot-5.0.9/src/uproot/writing/_cascadetree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/writing/identify.py` & `uproot-5.0.9/src/uproot/writing/identify.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/src/uproot/writing/writable.py` & `uproot-5.0.9/src/uproot/writing/writable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0001-source-class.py` & `uproot-5.0.9/tests/test_0001-source-class.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0006-notify-when-downloaded.py` & `uproot-5.0.9/tests/test_0006-notify-when-downloaded.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0007-single-chunk-interface.py` & `uproot-5.0.9/tests/test_0007-single-chunk-interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0008-start-interpretation.py` & `uproot-5.0.9/tests/test_0008-start-interpretation.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0009-nested-directories.py` & `uproot-5.0.9/tests/test_0009-nested-directories.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0010-start-streamers.py` & `uproot-5.0.9/tests/test_0010-start-streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0011-generate-classes-from-streamers.py` & `uproot-5.0.9/tests/test_0011-generate-classes-from-streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0013-rntuple-anchor.py` & `uproot-5.0.9/tests/test_0013-rntuple-anchor.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0014-all-ttree-versions.py` & `uproot-5.0.9/tests/test_0014-all-ttree-versions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0016-interpretations.py` & `uproot-5.0.9/tests/test_0016-interpretations.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0017-multi-basket-multi-branch-fetch.py` & `uproot-5.0.9/tests/test_0017-multi-basket-multi-branch-fetch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0018-array-fetching-interface.py` & `uproot-5.0.9/tests/test_0018-array-fetching-interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0022-number-of-branches.py` & `uproot-5.0.9/tests/test_0022-number-of-branches.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0023-more-interpretations-1.py` & `uproot-5.0.9/tests/test_0023-more-interpretations-1.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0023-ttree-versions.py` & `uproot-5.0.9/tests/test_0023-ttree-versions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0029-more-string-types.py` & `uproot-5.0.9/tests/test_0029-more-string-types.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0031-test-stl-containers.py` & `uproot-5.0.9/tests/test_0031-test-stl-containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0033-more-interpretations-2.py` & `uproot-5.0.9/tests/test_0033-more-interpretations-2.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0034-generic-objects-in-ttrees.py` & `uproot-5.0.9/tests/test_0034-generic-objects-in-ttrees.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0035-datatype-generality.py` & `uproot-5.0.9/tests/test_0035-datatype-generality.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0038-memberwise-serialization.py` & `uproot-5.0.9/tests/test_0038-memberwise-serialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0043-iterate-function.py` & `uproot-5.0.9/tests/test_0043-iterate-function.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0044-concatenate-function.py` & `uproot-5.0.9/tests/test_0044-concatenate-function.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0046-histograms-bh-hist.py` & `uproot-5.0.9/tests/test_0046-histograms-bh-hist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0053-parents-should-not-be-bases.py` & `uproot-5.0.9/tests/test_0053-parents-should-not-be-bases.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0058-detach-model-objects-from-files.py` & `uproot-5.0.9/tests/test_0058-detach-model-objects-from-files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0067-common-entry-offsets.py` & `uproot-5.0.9/tests/test_0067-common-entry-offsets.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0081-dont-parse-colons.py` & `uproot-5.0.9/tests/test_0081-dont-parse-colons.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0087-memberwise-splitting-not-implemented-messages.py` & `uproot-5.0.9/tests/test_0087-memberwise-splitting-not-implemented-messages.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0088-read-with-http.py` & `uproot-5.0.9/tests/test_0088-read-with-http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0099-read-from-file-object.py` & `uproot-5.0.9/tests/test_0099-read-from-file-object.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0112-fix-pandas-with-cut.py` & `uproot-5.0.9/tests/test_0112-fix-pandas-with-cut.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0118-fix-name-fetch-again.py` & `uproot-5.0.9/tests/test_0118-fix-name-fetch-again.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0167-use-the-common-histogram-interface.py` & `uproot-5.0.9/tests/test_0167-use-the-common-histogram-interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0173-empty-and-multiprocessing-bugs.py` & `uproot-5.0.9/tests/test_0173-empty-and-multiprocessing-bugs.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0182-complain-about-missing-files.py` & `uproot-5.0.9/tests/test_0182-complain-about-missing-files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0220-contiguous-byte-ranges-in-http.py` & `uproot-5.0.9/tests/test_0220-contiguous-byte-ranges-in-http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0228_read-TProfiles.py` & `uproot-5.0.9/tests/test_0228_read-TProfiles.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0240-read_TGraphAsymmErrors.py` & `uproot-5.0.9/tests/test_0240-read_TGraphAsymmErrors.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0278-specializations-for-TParameter.py` & `uproot-5.0.9/tests/test_0278-specializations-for-TParameter.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0302-pickle.py` & `uproot-5.0.9/tests/test_0302-pickle.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0303-empty-jagged-array.py` & `uproot-5.0.9/tests/test_0303-empty-jagged-array.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0320-start-working-on-ROOT-writing.py` & `uproot-5.0.9/tests/test_0320-start-working-on-ROOT-writing.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0322-writablefile-infrastructure.py` & `uproot-5.0.9/tests/test_0322-writablefile-infrastructure.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0325-fix-windows-file-uris.py` & `uproot-5.0.9/tests/test_0325-fix-windows-file-uris.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0329-update-existing-root-files.py` & `uproot-5.0.9/tests/test_0329-update-existing-root-files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0341-manipulate-streamer-info.py` & `uproot-5.0.9/tests/test_0341-manipulate-streamer-info.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0344-writabledirectory-can-read.py` & `uproot-5.0.9/tests/test_0344-writabledirectory-can-read.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0345-bulk-copy-method.py` & `uproot-5.0.9/tests/test_0345-bulk-copy-method.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0349-write-TObjString.py` & `uproot-5.0.9/tests/test_0349-write-TObjString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0350-read-RooCurve-RooHist.py` & `uproot-5.0.9/tests/test_0350-read-RooCurve-RooHist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0351-write-TList.py` & `uproot-5.0.9/tests/test_0351-write-TList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0352-write-THashList.py` & `uproot-5.0.9/tests/test_0352-write-THashList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0384-move-behavior_of-and-fix-383.py` & `uproot-5.0.9/tests/test_0384-move-behavior_of-and-fix-383.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0398-dimensions-in-leaflist.py` & `uproot-5.0.9/tests/test_0398-dimensions-in-leaflist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0405-write-a-histogram.py` & `uproot-5.0.9/tests/test_0405-write-a-histogram.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0406-write-a-ttree.py` & `uproot-5.0.9/tests/test_0406-write-a-ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0407-read-TDatime.py` & `uproot-5.0.9/tests/test_0407-read-TDatime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0412-write-multidimensional-numpy-to-ttree.py` & `uproot-5.0.9/tests/test_0412-write-multidimensional-numpy-to-ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0414-write-jagged-arrays.py` & `uproot-5.0.9/tests/test_0414-write-jagged-arrays.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0416-writing-compressed-data.py` & `uproot-5.0.9/tests/test_0416-writing-compressed-data.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0418-read-TTable.py` & `uproot-5.0.9/tests/test_0418-read-TTable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0420-pyroot-uproot-interoperability.py` & `uproot-5.0.9/tests/test_0420-pyroot-uproot-interoperability.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0422-hist-integration.py` & `uproot-5.0.9/tests/test_0422-hist-integration.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0438-TClonesArray-is-not-AsGrouped.py` & `uproot-5.0.9/tests/test_0438-TClonesArray-is-not-AsGrouped.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0442-regular-TClonesArray.py` & `uproot-5.0.9/tests/test_0442-regular-TClonesArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0472-tstreamerinfo-for-ttree.py` & `uproot-5.0.9/tests/test_0472-tstreamerinfo-for-ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0475-remember-to-update-freesegments.py` & `uproot-5.0.9/tests/test_0475-remember-to-update-freesegments.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0487-implement-asdtypeinplace.py` & `uproot-5.0.9/tests/test_0487-implement-asdtypeinplace.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0498-create-leaf-branch-in-extend.py` & `uproot-5.0.9/tests/test_0498-create-leaf-branch-in-extend.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0576-unicode-in-names.py` & `uproot-5.0.9/tests/test_0576-unicode-in-names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0578-dask-for-numpy.py` & `uproot-5.0.9/tests/test_0578-dask-for-numpy.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0580-round-trip-for-no-flow-histograms.py` & `uproot-5.0.9/tests/test_0580-round-trip-for-no-flow-histograms.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0589-explicitly-interpret-RVec-type.py` & `uproot-5.0.9/tests/test_0589-explicitly-interpret-RVec-type.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0603-dask-delayed-open.py` & `uproot-5.0.9/tests/test_0603-dask-delayed-open.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0609-num-enteries-func.py` & `uproot-5.0.9/tests/test_0609-num-enteries-func.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0610-awkward-form.py` & `uproot-5.0.9/tests/test_0610-awkward-form.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0630-rntuple-basics.py` & `uproot-5.0.9/tests/test_0630-rntuple-basics.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0637-setup-tests-for-AwkwardForth.py` & `uproot-5.0.9/tests/test_0637-setup-tests-for-AwkwardForth.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0643-reading-vector-pair-TLorentzVector-int.py` & `uproot-5.0.9/tests/test_0643-reading-vector-pair-TLorentzVector-int.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0651-implement-transformed-axis.py` & `uproot-5.0.9/tests/test_0651-implement-transformed-axis.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0652_dask-for-awkward.py` & `uproot-5.0.9/tests/test_0652_dask-for-awkward.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0662-rntuple-stl-containers.py` & `uproot-5.0.9/tests/test_0662-rntuple-stl-containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0700-dask-empty-arrays.py` & `uproot-5.0.9/tests/test_0700-dask-empty-arrays.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0705-rntuple-writing-metadata.py` & `uproot-5.0.9/tests/test_0705-rntuple-writing-metadata.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0755-dask-awkward-column-projection.py` & `uproot-5.0.9/tests/test_0755-dask-awkward-column-projection.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0791-protect-uproot-project_columns-from-dask-node-names.py` & `uproot-5.0.9/tests/test_0791-protect-uproot-project_columns-from-dask-node-names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0798_DAOD_PHYSLITE.py` & `uproot-5.0.9/tests/test_0798_DAOD_PHYSLITE.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0808-fix_awkward_form_for_AsStridedObjects.py` & `uproot-5.0.9/tests/test_0808-fix_awkward_form_for_AsStridedObjects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0816-separate-AwkwardForth-machines-by-TBranch.py` & `uproot-5.0.9/tests/test_0816-separate-AwkwardForth-machines-by-TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0832-ak_add_doc-should-also-add-to-typetracer.py` & `uproot-5.0.9/tests/test_0832-ak_add_doc-should-also-add-to-typetracer.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0840-support-tleafG.py` & `uproot-5.0.9/tests/test_0840-support-tleafG.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0841-fix-814.py` & `uproot-5.0.9/tests/test_0841-fix-814.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0844-fix-delete-hist-from-root.py` & `uproot-5.0.9/tests/test_0844-fix-delete-hist-from-root.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/test_0876-uproot-dask-blind-steps.py` & `uproot-5.0.9/tests/test_0876-uproot-dask-blind-steps.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/tests/samples/h_dynamic.pkl` & `uproot-5.0.9/tests/samples/h_dynamic.pkl`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/.gitignore` & `uproot-5.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/LICENSE` & `uproot-5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/README.md` & `uproot-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/pyproject.toml` & `uproot-5.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uproot-5.0.8/PKG-INFO` & `uproot-5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uproot
-Version: 5.0.8
+Version: 5.0.9
 Summary: ROOT I/O in pure Python and NumPy.
 Project-URL: Download, https://github.com/scikit-hep/uproot5/releases
 Project-URL: Homepage, https://github.com/scikit-hep/uproot5
 Author-email: Jim Pivarski <pivarski@princeton.edu>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

