# Comparing `tmp/myokit-1.34.0.tar.gz` & `tmp/myokit-1.35.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myokit-1.34.0.tar", last modified: Wed Jun  7 22:21:18 2023, max compression
+gzip compressed data, was "myokit-1.35.0.tar", last modified: Wed Jun 21 11:10:29 2023, max compression
```

## Comparing `myokit-1.34.0.tar` & `myokit-1.35.0.tar`

### file list

```diff
@@ -1,456 +1,454 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.397337 myokit-1.34.0/
--rw-r--r--   0 michael   (1000) michael   (1000)     1833 2023-06-07 13:48:59.000000 myokit-1.34.0/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-06-07 13:48:23.000000 myokit-1.34.0/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     5086 2023-06-07 22:21:18.397337 myokit-1.34.0/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     3821 2023-06-07 13:48:59.000000 myokit-1.34.0/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.361337 myokit-1.34.0/myokit/
--rw-r--r--   0 michael   (1000) michael   (1000)    14696 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59821 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23902 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_aux.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.362337 myokit-1.34.0/myokit/_bin/
--rw-r--r--   0 michael   (1000) michael   (1000)     6226 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/example.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.364337 myokit-1.34.0/myokit/_bin/gui/
--rw-r--r--   0 michael   (1000) michael   (1000)      784 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/find.png
--rw-r--r--   0 michael   (1000) michael   (1000)    96412 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-128.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     3528 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-16.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-24.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   233500 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-256.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    12232 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-32.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    23817 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-48.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    36761 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-64.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    65257 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-96.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer.ico
--rw-r--r--   0 michael   (1000) michael   (1000)    30396 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer.png
--rw-r--r--   0 michael   (1000) michael   (1000)    47406 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-128.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     2987 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-16.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     4971 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-24.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   152751 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-256.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     7355 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-32.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     9835 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-48.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    16235 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-64.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    30683 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-96.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide.ico
--rw-r--r--   0 michael   (1000) michael   (1000)    15096 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide.png
--rw-r--r--   0 michael   (1000) michael   (1000)      571 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/new.png
--rw-r--r--   0 michael   (1000) michael   (1000)      544 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/open.png
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/redo.png
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/run.png
--rw-r--r--   0 michael   (1000) michael   (1000)      565 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/save.png
--rw-r--r--   0 michael   (1000) michael   (1000)      284 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/undo.png
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.364337 myokit-1.34.0/myokit/_bin/install-lin/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      254 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_bin/install-lin/myokit-datablock-viewer.desktop
--rwxr-xr-x   0 michael   (1000) michael   (1000)      266 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_bin/install-lin/myokit-datalog-viewer.desktop
--rwxr-xr-x   0 michael   (1000) michael   (1000)      264 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/install-lin/myokit-ide.desktop
--rw-r--r--   0 michael   (1000) michael   (1000)     4338 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_bin/install-lin/myokit.lang
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-07 13:47:50.000000 myokit-1.34.0/myokit/_bin/install-lin/x-abf.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      246 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/install-lin/x-cellml.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      247 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_bin/install-lin/x-myokit.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      275 2023-06-07 13:47:50.000000 myokit-1.34.0/myokit/_bin/install-lin/x-wcp.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.365337 myokit-1.34.0/myokit/_bin/install-win/
--rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-06-07 22:09:55.000000 myokit-1.34.0/myokit/_bin/install-win/menu.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.365337 myokit-1.34.0/myokit/_bin/sundials-win-vs/
--rw-r--r--   0 michael   (1000) michael   (1000)     1758 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/LICENSE
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.358337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.365337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/
--rw-r--r--   0 michael   (1000) michael   (1000)    27506 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h
--rw-r--r--   0 michael   (1000) michael   (1000)     2427 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h
--rw-r--r--   0 michael   (1000) michael   (1000)    12344 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.365337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/nvector/
--rw-r--r--   0 michael   (1000) michael   (1000)     8934 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.366337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/
--rw-r--r--   0 michael   (1000) michael   (1000)     5785 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h
--rw-r--r--   0 michael   (1000) michael   (1000)     8997 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h
--rw-r--r--   0 michael   (1000) michael   (1000)    13330 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h
--rw-r--r--   0 michael   (1000) michael   (1000)     1024 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h
--rw-r--r--   0 michael   (1000) michael   (1000)    10283 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h
--rw-r--r--   0 michael   (1000) michael   (1000)     9385 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5420 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h
--rw-r--r--   0 michael   (1000) michael   (1000)     9190 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h
--rw-r--r--   0 michael   (1000) michael   (1000)    12559 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5165 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h
--rw-r--r--   0 michael   (1000) michael   (1000)     1266 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.366337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunlinsol/
--rw-r--r--   0 michael   (1000) michael   (1000)     2983 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.366337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunmatrix/
--rw-r--r--   0 michael   (1000) michael   (1000)     3647 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.367337 myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/
--rw-r--r--   0 michael   (1000) michael   (1000)   677888 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll
--rw-r--r--   0 michael   (1000) michael   (1000)   169196 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib
--rw-r--r--   0 michael   (1000) michael   (1000)   160768 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll
--rw-r--r--   0 michael   (1000) michael   (1000)    59576 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib
--rw-r--r--   0 michael   (1000) michael   (1000)    12309 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_config.py
--rw-r--r--   0 michael   (1000) michael   (1000)    68704 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_datablock.py
--rw-r--r--   0 michael   (1000) michael   (1000)    68982 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_datalog.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11462 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_err.py
--rw-r--r--   0 michael   (1000) michael   (1000)      438 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_exec_new.py
--rw-r--r--   0 michael   (1000) michael   (1000)      448 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_exec_old.py
--rw-r--r--   0 michael   (1000) michael   (1000)   105065 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_expressions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9545 2023-06-07 18:58:09.000000 myokit-1.34.0/myokit/_io.py
--rw-r--r--   0 michael   (1000) michael   (1000)   193828 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_model_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-06-07 22:19:30.000000 myokit-1.34.0/myokit/_myokit_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)    74425 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_parsing.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4566 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_progress.py
--rw-r--r--   0 michael   (1000) michael   (1000)    30748 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_protocol.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.369337 myokit-1.34.0/myokit/_sim/
--rw-r--r--   0 michael   (1000) michael   (1000)    13853 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19220 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)    18933 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/cable.py
--rw-r--r--   0 michael   (1000) michael   (1000)    38822 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/cmodel.h
--rw-r--r--   0 michael   (1000) michael   (1000)    15889 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/cmodel.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4047 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/compiler.c
--rw-r--r--   0 michael   (1000) michael   (1000)     2784 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/compiler.py
--rw-r--r--   0 michael   (1000) michael   (1000)    71394 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/cvodessim.c
--rw-r--r--   0 michael   (1000) michael   (1000)    42629 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/cvodessim.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15446 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/differential.hpp
--rw-r--r--   0 michael   (1000) michael   (1000)    47578 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/fiber_tissue.c
--rw-r--r--   0 michael   (1000) michael   (1000)    50826 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/fiber_tissue.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8012 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/jacobian.cpp
--rw-r--r--   0 michael   (1000) michael   (1000)    13105 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/jacobian.py
--rw-r--r--   0 michael   (1000) michael   (1000)    31548 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/mcl.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5037 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/opencl.c
--rw-r--r--   0 michael   (1000) michael   (1000)    16825 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/opencl.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46683 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/openclsim.c
--rw-r--r--   0 michael   (1000) michael   (1000)    19360 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/openclsim.cl
--rw-r--r--   0 michael   (1000) michael   (1000)    69345 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/openclsim.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29825 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/pacing.h
--rw-r--r--   0 michael   (1000) michael   (1000)    11126 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/rhs.c
--rw-r--r--   0 michael   (1000) michael   (1000)     7634 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/rhs.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1720 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/sundials.c
--rw-r--r--   0 michael   (1000) michael   (1000)     3092 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/sundials.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4835 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_system.py
--rw-r--r--   0 michael   (1000) michael   (1000)    30095 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_unit.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3172 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/float.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.369337 myokit-1.34.0/myokit/formats/
--rw-r--r--   0 michael   (1000) michael   (1000)    20284 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.369337 myokit-1.34.0/myokit/formats/ansic/
--rw-r--r--   0 michael   (1000) michael   (1000)     3453 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/ansic/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3698 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/ansic/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5467 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/formats/ansic/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.369337 myokit-1.34.0/myokit/formats/ansic/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    11965 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/ansic/template/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)     6044 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/ansic/template/euler.c
--rw-r--r--   0 michael   (1000) michael   (1000)    14244 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/ansic/template/sim.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.370337 myokit-1.34.0/myokit/formats/axon/
--rw-r--r--   0 michael   (1000) michael   (1000)      643 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/axon/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    70187 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/axon/_abf.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10277 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/axon/_atf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      939 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/axon/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.370337 myokit-1.34.0/myokit/formats/cellml/
--rw-r--r--   0 michael   (1000) michael   (1000)     1572 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cellml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2909 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2451 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cellml/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2355 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cellml/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.370337 myokit-1.34.0/myokit/formats/cellml/v1/
--rw-r--r--   0 michael   (1000) michael   (1000)      715 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cellml/v1/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59236 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v1/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)    43692 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v1/_parser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15320 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v1/_writer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.371337 myokit-1.34.0/myokit/formats/cellml/v2/
--rw-r--r--   0 michael   (1000) michael   (1000)      704 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cellml/v2/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59303 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v2/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29674 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v2/_parser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    12108 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v2/_writer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.371337 myokit-1.34.0/myokit/formats/channelml/
--rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/channelml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    14840 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/formats/channelml/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.371337 myokit-1.34.0/myokit/formats/cpp/
--rw-r--r--   0 michael   (1000) michael   (1000)      631 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cpp/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      527 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cpp/_ewriter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.371337 myokit-1.34.0/myokit/formats/cuda/
--rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cuda/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4603 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cuda/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2165 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cuda/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.371337 myokit-1.34.0/myokit/formats/cuda/template/
--rw-r--r--   0 michael   (1000) michael   (1000)     8863 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/cuda/template/kernel.cu
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.372337 myokit-1.34.0/myokit/formats/easyml/
--rw-r--r--   0 michael   (1000) michael   (1000)      942 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/easyml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3811 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/easyml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15877 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/easyml/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.372337 myokit-1.34.0/myokit/formats/html/
--rw-r--r--   0 michael   (1000) michael   (1000)      563 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/html/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2449 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/html/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7184 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/html/_flatten.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.372337 myokit-1.34.0/myokit/formats/latex/
--rw-r--r--   0 michael   (1000) michael   (1000)      788 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/latex/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6823 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/latex/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5259 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/latex/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.372337 myokit-1.34.0/myokit/formats/mathml/
--rw-r--r--   0 michael   (1000) michael   (1000)      743 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/mathml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    12444 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/mathml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)    34419 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/formats/mathml/_parser.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.373337 myokit-1.34.0/myokit/formats/matlab/
--rw-r--r--   0 michael   (1000) michael   (1000)      801 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3306 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2974 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/matlab/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.373337 myokit-1.34.0/myokit/formats/matlab/template/
--rw-r--r--   0 michael   (1000) michael   (1000)      528 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/template/constants.m
--rw-r--r--   0 michael   (1000) michael   (1000)      374 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/template/ifthenelse.m
--rw-r--r--   0 michael   (1000) michael   (1000)     2095 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/matlab/template/main.m
--rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/template/model.m
--rw-r--r--   0 michael   (1000) michael   (1000)      461 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/template/model_wrapper.m
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.373337 myokit-1.34.0/myokit/formats/opencl/
--rw-r--r--   0 michael   (1000) michael   (1000)     7068 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/opencl/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5394 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/opencl/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4009 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/opencl/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.374337 myokit-1.34.0/myokit/formats/opencl/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    11633 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/opencl/template/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)     8158 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/opencl/template/kernel.cl
--rw-r--r--   0 michael   (1000) michael   (1000)     9018 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/opencl/template/minilog.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1042 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/formats/opencl/template/plot.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      162 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/opencl/template/test.sh
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.374337 myokit-1.34.0/myokit/formats/python/
--rw-r--r--   0 michael   (1000) michael   (1000)     1155 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/python/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6912 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/python/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/python/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.374337 myokit-1.34.0/myokit/formats/python/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    10489 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/python/template/sim.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.375337 myokit-1.34.0/myokit/formats/sbml/
--rw-r--r--   0 michael   (1000) michael   (1000)      759 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/sbml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59422 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/sbml/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1111 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/sbml/_importer.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29317 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/sbml/_parser.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.375337 myokit-1.34.0/myokit/formats/stan/
--rw-r--r--   0 michael   (1000) michael   (1000)     2983 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/stan/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3233 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/stan/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3869 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/stan/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.375337 myokit-1.34.0/myokit/formats/stan/template/
--rw-r--r--   0 michael   (1000) michael   (1000)     5305 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/stan/template/cell.stan
--rwxr-xr-x   0 michael   (1000) michael   (1000)       92 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/formats/stan/template/run.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.376337 myokit-1.34.0/myokit/formats/sympy/
--rw-r--r--   0 michael   (1000) michael   (1000)     1744 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/sympy/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6872 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/sympy/_ereader.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5008 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/sympy/_ewriter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.376337 myokit-1.34.0/myokit/formats/wcp/
--rw-r--r--   0 michael   (1000) michael   (1000)      360 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/wcp/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10510 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/wcp/_wcp.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.376337 myokit-1.34.0/myokit/formats/xml/
--rw-r--r--   0 michael   (1000) michael   (1000)      551 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/xml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1600 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/xml/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)      499 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/xml/_split.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.377337 myokit-1.34.0/myokit/gui/
--rw-r--r--   0 michael   (1000) michael   (1000)    12173 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/gui/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46626 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/gui/datablock_viewer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    32941 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/gui/datalog_viewer.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8607 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/gui/explorer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)   108635 2023-06-07 22:09:55.000000 myokit-1.34.0/myokit/gui/ide.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2174 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/gui/progress.py
--rw-r--r--   0 michael   (1000) michael   (1000)    50887 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/gui/source.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6270 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/gui/vargrapher.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.378337 myokit-1.34.0/myokit/lib/
--rw-r--r--   0 michael   (1000) michael   (1000)      216 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/lib/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    24002 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/lib/deps.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28160 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/lib/guess.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46838 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/lib/hh.py
--rw-r--r--   0 michael   (1000) michael   (1000)    67969 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/lib/markov.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4513 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/lib/multi.py
--rw-r--r--   0 michael   (1000) michael   (1000)    13979 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/lib/plots.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4658 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/pacing.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8504 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/pype.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.385337 myokit-1.34.0/myokit/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)     7898 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2830 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/ansic_event_based_pacing.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1376 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/ansic_fixed_form_pacing.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.387337 myokit-1.34.0/myokit/tests/data/
--rw-r--r--   0 michael   (1000) michael   (1000)     3022 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-model-compare-a.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     2889 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-model-compare-b.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3137 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-model.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-protocol.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-script.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3287 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-units.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     5091 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/clancy-1999-fitting.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3128 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/conditional.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6067 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/cv1d.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/cv1d.zip
--rw-r--r--   0 michael   (1000) michael   (1000)    23916 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/decker-2009.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)    18350 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/decker.model
--rw-r--r--   0 michael   (1000) michael   (1000)    10416 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/dn-1985-normalised.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      800 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/dom-markov.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.388337 myokit-1.34.0/myokit/tests/data/formats/
--rw-r--r--   0 michael   (1000) michael   (1000)     8192 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/abf-protocol.pro
--rw-r--r--   0 michael   (1000) michael   (1000)    98376 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/abf-v1.abf
--rw-r--r--   0 michael   (1000) michael   (1000)    24576 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/abf-v2.abf
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.389337 myokit-1.34.0/myokit/tests/data/formats/cellml/
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)    59093 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/br-1977-dot.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    58593 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/br-1977.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)   117223 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/corrias.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)   221953 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/decker-2009.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)     1595 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/documentation.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/invalid-file.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    44837 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    44947 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.391337 myokit-1.34.0/myokit/tests/data/formats/channelml/
--rw-r--r--   0 michael   (1000) michael   (1000)     2648 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      557 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     2702 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     2369 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1258 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1539 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1290 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1374 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1373 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      675 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1398 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1317 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.391337 myokit-1.34.0/myokit/tests/data/formats/sbml/
--rw-r--r--   0 michael   (1000) michael   (1000)     8719 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     9801 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml
--rw-r--r--   0 michael   (1000) michael   (1000)    31408 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/HodgkinHuxley.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/LICENSE
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.391337 myokit-1.34.0/myokit/tests/data/formats/sbml/model/
--rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     2952 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     1226 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.391337 myokit-1.34.0/myokit/tests/data/formats/sbml/result/
--rw-r--r--   0 michael   (1000) michael   (1000)     2457 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/result/00001-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     2206 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/result/00004-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/result/01103-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)    25600 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/wcp-file.wcp
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.396337 myokit-1.34.0/myokit/tests/data/io/
--rw-r--r--   0 michael   (1000) michael   (1000)      735 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-1-not-enough-files.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109429 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-2-no-header.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   104768 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-3-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-4-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109458 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-5-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1549 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-6-time-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-7-0d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-8-1d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)      739 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-1-not-enough-files.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346240 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-2-no-header.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   333091 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-3-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-4-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346257 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-5-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1553 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-6-time-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1588 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-7-0d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-8-2d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)      623 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-1-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1281 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-2-no-structure.zip
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-3-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-4-invalid-n-fields.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-5-invalid-data-size.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1457 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-6-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-7-not-enough-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     6031 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/io/block2d.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/block2d.zip
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-1-empty.csv
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-10-just-spaces.csv
--rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-11-just-a-semicolon.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-12-bad-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-13-header-with-empty-1.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-14-header-with-empty-2.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-15-header-with-empty-3.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-16-wrong-columns-in-data.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-17-non-float-data.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      112 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-2-windows.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      103 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-3-old-mac.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-4-empty-lines.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-5-semicolons.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-6-open-string.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-7-empty-lines-2.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-8-unquoted-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      114 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-9-double-quoted-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     1421 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/goodlog.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     4992 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/lr-1991-dep.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     2315 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/lr-1991-fitting.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     4571 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/lr-1991-testing.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6124 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/lr-1991.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.397337 myokit-1.34.0/myokit/tests/data/multi/
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/beeler-1977-protocol.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/beeler-1977-script.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/beeler-no-name.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6013 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/lr-1991.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/not-a-model.csv
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.397337 myokit-1.34.0/myokit/tests/data/multi/subdir/
--rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/subdir/beeler-no-name.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3754 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/noble-1962.mmt
--rwxr-xr-x   0 michael   (1000) michael   (1000)    22939 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_aux.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    57389 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v1_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    42270 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v1_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12819 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v1_writer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    73727 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v2_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    26746 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v2_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11264 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v2_writer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4345 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cmodel.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      704 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/test_compiler_detection.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14384 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_component.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12599 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_config.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    50041 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_datablock.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    83227 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_datalog.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    61106 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_dependency_checking.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)   138795 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_expressions.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5053 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_float.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4523 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    15162 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_axon.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    19483 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_cellml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     7137 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_channelml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11791 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_easyml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     9610 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_exporters.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    41242 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_expression_writers.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3645 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/test_formats_html.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1972 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_importers.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    37731 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_mathml_content.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     9013 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_mathml_presentation.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    17615 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/test_formats_opencl.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5106 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_sbml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10611 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_sympy.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1891 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_wcp.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14562 2023-06-07 18:58:09.000000 myokit-1.34.0/myokit/tests/test_io.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2107 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_jacobian_calculator.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2054 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_jacobian_tracer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     7763 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/test_lib_deps.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    42620 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_lib_guess.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    31300 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_lib_hh.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    40269 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_lib_markov.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5432 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_lib_multi.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6168 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/tests/test_lib_plots.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2935 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_meta.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    85260 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_model.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    17109 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_model_building.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4068 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_opencl_info.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8299 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_pacing_factory.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5448 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_pacing_system_c.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3235 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/test_pacing_system_py.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    51305 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_parsing.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2868 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_progress_reporters.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    15379 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_protocol.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12852 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/tests/test_protocol_floating_point.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2606 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_protocol_time_series.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2689 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_pype.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     7640 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_quantity.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3738 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_rhs_benchmarker.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    72067 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_sbml_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    54976 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_sbml_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    18000 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_1d.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    42412 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_cvodes.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1959 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_cvodes_from_disk.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    35708 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_fiber_tissue.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14320 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_log_interval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    59482 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/tests/test_simulation_opencl.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3110 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_opencl_log_interval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    20401 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_opencl_vs_cvode.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5503 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_opencl_vs_sim1d.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      790 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_system_info.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10578 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_tools.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    13922 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/tests/test_unit.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2009 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_user_functions.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    33619 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_variable.py
--rw-r--r--   0 michael   (1000) michael   (1000)    17487 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tools.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8609 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/units.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.362337 myokit-1.34.0/myokit.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)     5086 2023-06-07 22:21:17.000000 myokit-1.34.0/myokit.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)    15047 2023-06-07 22:21:18.000000 myokit-1.34.0/myokit.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-06-07 22:21:17.000000 myokit-1.34.0/myokit.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       48 2023-06-07 22:21:18.000000 myokit-1.34.0/myokit.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-01-04 14:18:38.000000 myokit-1.34.0/myokit.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      182 2023-06-07 22:21:18.000000 myokit-1.34.0/myokit.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        7 2023-06-07 22:21:18.000000 myokit-1.34.0/myokit.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-07 22:21:18.397337 myokit-1.34.0/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     3290 2023-06-07 22:09:50.000000 myokit-1.34.0/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.836466 myokit-1.35.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1833 2023-06-07 13:48:59.000000 myokit-1.35.0/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-06-07 13:48:23.000000 myokit-1.35.0/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     5059 2023-06-21 11:10:29.836466 myokit-1.35.0/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     3821 2023-06-07 13:48:59.000000 myokit-1.35.0/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.803465 myokit-1.35.0/myokit/
+-rw-r--r--   0 michael   (1000) michael   (1000)    14173 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    58017 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23743 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_aux.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.803465 myokit-1.35.0/myokit/_bin/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6226 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/example.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.806465 myokit-1.35.0/myokit/_bin/gui/
+-rw-r--r--   0 michael   (1000) michael   (1000)      784 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/find.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    96412 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-128.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     3528 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-16.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-24.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   233500 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-256.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    12232 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-32.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    23817 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-48.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    36761 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-64.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    65257 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-96.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)    30396 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    47406 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-128.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     2987 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-16.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     4971 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-24.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   152751 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-256.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     7355 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-32.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     9835 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-48.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    16235 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-64.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    30683 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-96.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)    15096 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      571 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/new.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      544 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/open.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/redo.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/run.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      565 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/save.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      284 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/undo.png
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.807466 myokit-1.35.0/myokit/_bin/install-lin/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      254 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/_bin/install-lin/myokit-datablock-viewer.desktop
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      266 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/_bin/install-lin/myokit-datalog-viewer.desktop
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      264 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/install-lin/myokit-ide.desktop
+-rw-r--r--   0 michael   (1000) michael   (1000)     4338 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/_bin/install-lin/myokit.lang
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-07 13:47:50.000000 myokit-1.35.0/myokit/_bin/install-lin/x-abf.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      246 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/install-lin/x-cellml.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      247 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/_bin/install-lin/x-myokit.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      275 2023-06-07 13:47:50.000000 myokit-1.35.0/myokit/_bin/install-lin/x-wcp.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.807466 myokit-1.35.0/myokit/_bin/install-win/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_bin/install-win/menu.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.807466 myokit-1.35.0/myokit/_bin/sundials-win-vs/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1758 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/LICENSE
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.799466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.807466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/
+-rw-r--r--   0 michael   (1000) michael   (1000)    27506 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     2427 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    12344 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.807466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/nvector/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8934 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.808466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5785 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     8997 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    13330 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     1024 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    10283 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     9385 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5420 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     9190 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    12559 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5165 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     1266 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.808466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunlinsol/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2983 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.808466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunmatrix/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3647 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.809466 myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/
+-rw-r--r--   0 michael   (1000) michael   (1000)   677888 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll
+-rw-r--r--   0 michael   (1000) michael   (1000)   169196 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib
+-rw-r--r--   0 michael   (1000) michael   (1000)   160768 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll
+-rw-r--r--   0 michael   (1000) michael   (1000)    59576 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib
+-rw-r--r--   0 michael   (1000) michael   (1000)    12048 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_config.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    66499 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_datablock.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    67472 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_datalog.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11060 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_err.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   103962 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_expressions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8948 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_io.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   193097 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_model_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      726 2023-06-21 10:54:06.000000 myokit-1.35.0/myokit/_myokit_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    74065 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_parsing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4410 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_progress.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    30572 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_protocol.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.811466 myokit-1.35.0/myokit/_sim/
+-rw-r--r--   0 michael   (1000) michael   (1000)    13412 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19150 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    18810 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cable.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    38703 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cmodel.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    15775 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cmodel.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4047 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_sim/compiler.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     2664 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/compiler.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    71253 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cvodessim.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    42507 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cvodessim.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15446 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/differential.hpp
+-rw-r--r--   0 michael   (1000) michael   (1000)    47438 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/fiber_tissue.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    50694 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/fiber_tissue.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8012 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/jacobian.cpp
+-rw-r--r--   0 michael   (1000) michael   (1000)    12957 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/jacobian.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    32352 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/mcl.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5037 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_sim/opencl.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    16446 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/opencl.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46535 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/openclsim.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    19360 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/openclsim.cl
+-rw-r--r--   0 michael   (1000) michael   (1000)    69220 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/openclsim.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29511 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/pacing.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    10914 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/rhs.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     7392 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/rhs.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1720 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_sim/sundials.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     2972 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/sundials.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4602 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_system.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29848 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_unit.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3066 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/float.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.811466 myokit-1.35.0/myokit/formats/
+-rw-r--r--   0 michael   (1000) michael   (1000)    20096 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.812466 myokit-1.35.0/myokit/formats/ansic/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3347 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/ansic/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3566 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/ansic/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5361 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/ansic/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.812466 myokit-1.35.0/myokit/formats/ansic/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11965 2023-06-20 10:29:46.000000 myokit-1.35.0/myokit/formats/ansic/template/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     6044 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/ansic/template/euler.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    14244 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/ansic/template/sim.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.812466 myokit-1.35.0/myokit/formats/axon/
+-rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/axon/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    69921 2023-06-21 10:30:12.000000 myokit-1.35.0/myokit/formats/axon/_abf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10165 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/axon/_atf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      833 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/axon/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.812466 myokit-1.35.0/myokit/formats/cellml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1466 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2719 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2283 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2229 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.813466 myokit-1.35.0/myokit/formats/cellml/v1/
+-rw-r--r--   0 michael   (1000) michael   (1000)      608 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v1/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59011 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v1/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    43554 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v1/_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15055 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v1/_writer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.813466 myokit-1.35.0/myokit/formats/cellml/v2/
+-rw-r--r--   0 michael   (1000) michael   (1000)      598 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v2/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59012 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v2/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29536 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v2/_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11994 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v2/_writer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.813466 myokit-1.35.0/myokit/formats/channelml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      443 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/channelml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    14605 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/channelml/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.814466 myokit-1.35.0/myokit/formats/cpp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cpp/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      421 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cpp/_ewriter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.814466 myokit-1.35.0/myokit/formats/cuda/
+-rw-r--r--   0 michael   (1000) michael   (1000)      816 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cuda/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4472 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cuda/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2059 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cuda/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.814466 myokit-1.35.0/myokit/formats/cuda/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8863 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cuda/template/kernel.cu
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.814466 myokit-1.35.0/myokit/formats/easyml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/easyml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3482 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/easyml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15771 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/easyml/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.814466 myokit-1.35.0/myokit/formats/html/
+-rw-r--r--   0 michael   (1000) michael   (1000)      457 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/html/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2343 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/html/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6606 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/html/_flatten.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.815466 myokit-1.35.0/myokit/formats/latex/
+-rw-r--r--   0 michael   (1000) michael   (1000)      682 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/latex/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6690 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/latex/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5117 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/latex/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.815466 myokit-1.35.0/myokit/formats/mathml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      637 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/mathml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    12194 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/mathml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    34289 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/mathml/_parser.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.815466 myokit-1.35.0/myokit/formats/matlab/
+-rw-r--r--   0 michael   (1000) michael   (1000)      695 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/matlab/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3172 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/matlab/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2868 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/matlab/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.815466 myokit-1.35.0/myokit/formats/matlab/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)      528 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/formats/matlab/template/constants.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      374 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/formats/matlab/template/ifthenelse.m
+-rw-r--r--   0 michael   (1000) michael   (1000)     2095 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/formats/matlab/template/main.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/formats/matlab/template/model.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      461 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/formats/matlab/template/model_wrapper.m
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.816466 myokit-1.35.0/myokit/formats/opencl/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6962 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/opencl/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5261 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/opencl/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3903 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/opencl/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.816466 myokit-1.35.0/myokit/formats/opencl/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11633 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/formats/opencl/template/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     8158 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/opencl/template/kernel.cl
+-rw-r--r--   0 michael   (1000) michael   (1000)     9018 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/formats/opencl/template/minilog.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1042 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/formats/opencl/template/plot.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      162 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/formats/opencl/template/test.sh
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.816466 myokit-1.35.0/myokit/formats/python/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1049 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/python/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6751 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/python/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      969 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/python/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.816466 myokit-1.35.0/myokit/formats/python/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    10311 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/python/template/sim.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.817466 myokit-1.35.0/myokit/formats/sbml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      653 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sbml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59396 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sbml/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      987 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sbml/_importer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29181 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sbml/_parser.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.817466 myokit-1.35.0/myokit/formats/stan/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2877 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/stan/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3102 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/stan/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3745 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/stan/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.817466 myokit-1.35.0/myokit/formats/stan/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5305 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/stan/template/cell.stan
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       92 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/formats/stan/template/run.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.817466 myokit-1.35.0/myokit/formats/sympy/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1638 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sympy/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6758 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sympy/_ereader.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4875 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sympy/_ewriter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.818466 myokit-1.35.0/myokit/formats/wcp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      254 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/wcp/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10234 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/wcp/_wcp.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.818466 myokit-1.35.0/myokit/formats/xml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/xml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1494 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/xml/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      393 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/xml/_split.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.819466 myokit-1.35.0/myokit/gui/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6154 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46576 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/datablock_viewer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    32560 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/datalog_viewer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8588 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/explorer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)   108238 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/ide.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2157 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/progress.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    52418 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/source.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6072 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/vargrapher.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.819466 myokit-1.35.0/myokit/lib/
+-rw-r--r--   0 michael   (1000) michael   (1000)      216 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/lib/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23859 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/deps.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28056 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/guess.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46678 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/hh.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    67773 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/markov.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4408 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/multi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    13874 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/plots.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4552 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/pacing.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8230 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/pype.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.826466 myokit-1.35.0/myokit/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2697 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/ansic_event_based_pacing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1244 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/ansic_fixed_form_pacing.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.827466 myokit-1.35.0/myokit/tests/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3022 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-model-compare-a.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2889 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-model-compare-b.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3137 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-model.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-protocol.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-script.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3287 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-units.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     5091 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/clancy-1999-fitting.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3128 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/conditional.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6067 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/cv1d.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/cv1d.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)    23916 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/decker-2009.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)    18350 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/decker.model
+-rw-r--r--   0 michael   (1000) michael   (1000)    10416 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/dn-1985-normalised.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      800 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/dom-markov.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.828466 myokit-1.35.0/myokit/tests/data/formats/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8192 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/abf-protocol.pro
+-rw-r--r--   0 michael   (1000) michael   (1000)    98376 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/abf-v1.abf
+-rw-r--r--   0 michael   (1000) michael   (1000)    24576 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/abf-v2.abf
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.829466 myokit-1.35.0/myokit/tests/data/formats/cellml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)    59093 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/br-1977-dot.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    58593 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/br-1977.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)   117223 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/corrias.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)   221953 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/decker-2009.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1595 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/documentation.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/invalid-file.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    44837 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    44947 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.830466 myokit-1.35.0/myokit/tests/data/formats/channelml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2648 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      557 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2702 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2369 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1258 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1539 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1290 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1374 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1373 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      675 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1398 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1317 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.831466 myokit-1.35.0/myokit/tests/data/formats/sbml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8719 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     9801 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)    31408 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/HodgkinHuxley.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/LICENSE
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.831466 myokit-1.35.0/myokit/tests/data/formats/sbml/model/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2952 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1226 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.831466 myokit-1.35.0/myokit/tests/data/formats/sbml/result/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2457 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/result/00001-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     2206 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/result/00004-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/result/01103-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)    25600 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/wcp-file.wcp
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.836466 myokit-1.35.0/myokit/tests/data/io/
+-rw-r--r--   0 michael   (1000) michael   (1000)      735 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-1-not-enough-files.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109429 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-2-no-header.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   104768 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-3-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-4-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109458 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-5-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1549 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-6-time-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-7-0d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-8-1d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)      739 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-1-not-enough-files.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346240 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-2-no-header.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   333091 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-3-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-4-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346257 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-5-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1553 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-6-time-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1588 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-7-0d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-8-2d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)      623 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-1-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1281 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-2-no-structure.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-3-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-4-invalid-n-fields.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-5-invalid-data-size.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1457 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-6-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-7-not-enough-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     6031 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/io/block2d.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/block2d.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-1-empty.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-10-just-spaces.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-11-just-a-semicolon.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-12-bad-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-13-header-with-empty-1.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-14-header-with-empty-2.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-15-header-with-empty-3.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-16-wrong-columns-in-data.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-17-non-float-data.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      112 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-2-windows.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      103 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-3-old-mac.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-4-empty-lines.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-5-semicolons.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-6-open-string.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-7-empty-lines-2.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-8-unquoted-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      114 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-9-double-quoted-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     1421 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/goodlog.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     4992 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/lr-1991-dep.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2315 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/lr-1991-fitting.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4571 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/lr-1991-testing.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6124 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/lr-1991.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.836466 myokit-1.35.0/myokit/tests/data/multi/
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/beeler-1977-protocol.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/beeler-1977-script.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/beeler-no-name.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6013 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/lr-1991.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/not-a-model.csv
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.836466 myokit-1.35.0/myokit/tests/data/multi/subdir/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/subdir/beeler-no-name.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3754 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/noble-1962.mmt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    22536 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_aux.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    56981 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v1_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    41869 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v1_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12532 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v1_writer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    73319 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v2_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    26345 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v2_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10977 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v2_writer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4058 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cmodel.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      476 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_compiler_detection.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14096 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_component.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11511 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_config.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    49755 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_datablock.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    82813 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_datalog.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    60654 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_dependency_checking.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)   138508 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_expressions.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4882 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_float.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4236 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14876 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_axon.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    19078 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_cellml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6703 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_channelml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11358 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_easyml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     9169 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_exporters.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    40800 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_expression_writers.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3539 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_html.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1531 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_importers.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    37444 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_mathml_content.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8726 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_mathml_presentation.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    17298 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_opencl.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4672 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_sbml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10324 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_sympy.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1786 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_wcp.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14334 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_io.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1821 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_jacobian_calculator.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1767 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_jacobian_tracer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7476 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_deps.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    42333 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_guess.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    31014 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_hh.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    39983 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_markov.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5145 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_multi.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6062 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_plots.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2829 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_meta.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    84972 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_model.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    16720 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_model_building.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3834 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_opencl_info.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8193 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_pacing_factory.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5161 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_pacing_system_c.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2948 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_pacing_system_py.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    50865 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_parsing.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2762 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_progress_reporters.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    15092 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_protocol.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12565 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_protocol_floating_point.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2318 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_protocol_time_series.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2402 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_pype.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7353 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_quantity.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3452 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_rhs_benchmarker.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    71633 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_sbml_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    54542 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_sbml_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    17713 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_1d.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    42191 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_cvodes.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1853 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_cvodes_from_disk.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    35421 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_fiber_tissue.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14033 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_log_interval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    59195 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_opencl.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3005 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_opencl_log_interval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    20114 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_opencl_vs_cvode.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5216 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_opencl_vs_sim1d.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      562 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_system_info.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10358 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_tools.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    13635 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_unit.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1721 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_user_functions.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    33331 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_variable.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    16868 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tools.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8503 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/units.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.803465 myokit-1.35.0/myokit.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5059 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15007 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       48 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-01-04 14:18:38.000000 myokit-1.35.0/myokit.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      176 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        7 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-21 11:10:29.837466 myokit-1.35.0/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     3183 2023-06-21 10:33:11.000000 myokit-1.35.0/setup.py
```

### Comparing `myokit-1.34.0/LICENSE.txt` & `myokit-1.35.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/PKG-INFO` & `myokit-1.35.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: myokit
-Version: 1.34.0
+Version: 1.35.0
 Summary: A simple interface to cardiac cellular electrophysiology
 Home-page: http://myokit.org
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/MichaelClerx/myokit/issues
 Project-URL: Documentation, http://docs.myokit.org
 Project-URL: Source Code, https://github.com/MichaelClerx/myokit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: optional
 Provides-Extra: gui
 Provides-Extra: pyqt
 Provides-Extra: pyside
```

### Comparing `myokit-1.34.0/README.md` & `myokit-1.35.0/README.md`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/__init__.py` & `myokit-1.35.0/myokit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,59 +16,41 @@
 #
 # __all__ should NOT be provided! Doing so removes all methods below from
 # the content imported by "from myokit import *".
 #
 # Without an explicit __all__, importing * will result in importing all
 # functions and classes described below. No submodules of myokit will be
 # loaded!
-
-
 #
 # GUI and graphical modules should not be auto-included because they define a
 # matplotlib backend to use. If the user requires a different backend, this
 # will generate an error.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 
 #
 # Check python version
 #
 # Hexversion guide:
 #  0x   Hex
 #  02   PY_MAJOR_VERSION
 #  07   PY_MINOR_VERSION
 #  0F   PY_MICRO_VERSION, in hex, so 0F is 15, 10 is 16, etc.
 #  F    PY_RELEASE_LEVEL, A for alpha, B for beta, C for candidate, F for final
 #  0    PY_RELEASE_SERIAL, increments with every release
 #
 import sys  # noqa
 if sys.hexversion < 0x03000000:  # pragma: no cover
+    raise Exception('This version of Myokit does not support Python 2.')
+elif sys.hexversion < 0x03070000:  # pragma: no cover
     import logging  # noqa
     log = logging.getLogger(__name__)
     log.warning(
-        'Myokit support for Python 2.7 is nearing the end of its lifetime.'
-        ' Please upgrade as soon as possible! Detected Python version: '
-        + sys.version)
-    del logging, log
-elif sys.hexversion < 0x03060000:  # pragma: no cover
-    import logging  # noqa
-    log = logging.getLogger(__name__)
-    log.warning(
-        'Myokit is not tested on Python 3 versions older than 3.6. Detected'
+        'Myokit is not tested on Python 3 versions older than 3.7. Detected'
         ' Python version: ' + sys.version)
     del logging, log
-
-
-# Exec() that works with Python 2 versions before 2.7.9
-if sys.hexversion < 0x020709F0:     # pragma: no python 3 cover
-    from ._exec_old import _exec    # noqa
-else:
-    from ._exec_new import _exec    # noqa
 del sys
 
 
 #
 # Version information
 #
 from ._myokit_version import (  # noqa
@@ -285,17 +267,17 @@
 #
 DATE_FORMAT = '%Y-%m-%d %H:%M:%S'
 TIME_FORMAT = '%H:%M:%S'
 
 #
 # GUI: Favor PySide or PyQt
 #
+FORCE_PYQT6 = False
 FORCE_PYQT5 = False
-FORCE_PYQT4 = False
-FORCE_PYSIDE = False
+FORCE_PYSIDE6 = False
 FORCE_PYSIDE2 = False
 
 
 #
 # Library paths and settings
 #
```

### Comparing `myokit-1.34.0/myokit/__main__.py` & `myokit-1.35.0/myokit/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Command line tools.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import warnings
 
 _line_width = 79
 
 
 def printline():
     """ Utility method for printing horizontal lines. """
@@ -25,14 +22,63 @@
         'fail': '\033[91m',
         'bold': '\033[1m',
         'underline': '\033[4m',
     }
     return colors[color] + str(text) + colors['normal']
 
 
+def qtforce(pyqt6=False, pyqt5=False, pyside6=False, pyside2=False):
+    """ Enforce a chosen Qt version. """
+
+    if pyqt6 or pyqt5 or pyside6 or pyside2:
+        import myokit
+
+        myokit.FORCE_PYQT6 = False
+        myokit.FORCE_PYQT5 = False
+        myokit.FORCE_PYSIDE6 = False
+        myokit.FORCE_PYSIDE2 = False
+
+        if pyqt6:
+            myokit.FORCE_PYQT6 = True
+        elif pyside6:
+            myokit.FORCE_PYSIDE6 = True
+        elif pyqt5:
+            myokit.FORCE_PYQT5 = True
+        elif pyside2:
+            myokit.FORCE_PYSIDE2 = True
+
+        import myokit.gui
+        print('Using backend: ' + myokit.gui.backend)
+
+
+def add_qtforce_arguments(parser):
+    """ Updates a parser with arguments to force a Qt version. """
+
+    parser.add_argument(
+        '--pyqt6',
+        action='store_true',
+        help='Run using the PyQt6 backend.',
+    )
+    parser.add_argument(
+        '--pyqt5',
+        action='store_true',
+        help='Run using the PyQt5 backend.',
+    )
+    parser.add_argument(
+        '--pyside6',
+        action='store_true',
+        help='Run using the PySide6 backend.',
+    )
+    parser.add_argument(
+        '--pyside2',
+        action='store_true',
+        help='Run using the PySide2 backend.',
+    )
+
+
 def main():
     """
     Parses command line arguments.
     """
     import sys
 
     # Create parser
@@ -84,44 +130,21 @@
         # Call the selected function with the parsed arguments
         func(**args)
 
 
 #
 # Data block viewer
 #
-
-def block(filename, pyqt4=False, pyqt5=False, pyside=False, pyside2=False):
+def block(filename, pyqt6=False, pyqt5=False, pyside6=False, pyside2=False):
     """
     Runs the DataBlock viewer.
     """
-    import myokit
-    if pyqt5:
-        myokit.FORCE_PYQT5 = True
-        myokit.FORCE_PYQT4 = False
-        myokit.FORCE_PYSIDE = False
-        myokit.FORCE_PYSIDE2 = False
-    elif pyqt4:
-        myokit.FORCE_PYQT5 = False
-        myokit.FORCE_PYQT4 = True
-        myokit.FORCE_PYSIDE = False
-        myokit.FORCE_PYSIDE2 = False
-    elif pyside:
-        myokit.FORCE_PYQT5 = False
-        myokit.FORCE_PYQT4 = False
-        myokit.FORCE_PYSIDE = True
-        myokit.FORCE_PYSIDE2 = False
-    elif pyside2:
-        myokit.FORCE_PYQT5 = False
-        myokit.FORCE_PYQT4 = False
-        myokit.FORCE_PYSIDE = False
-        myokit.FORCE_PYSIDE2 = True
-    import myokit.gui
+    qtforce(pyqt6, pyqt5, pyside6, pyside2)
+
     import myokit.gui.datablock_viewer
-    if pyqt5 or pyqt4 or pyside or pyside2:
-        print('Using backend: ' + myokit.gui.backend)
     myokit.gui.run(myokit.gui.datablock_viewer.DataBlockViewer, filename)
 
 
 def add_block_parser(subparsers):
     """
     Adds a subcommand parser for `block`.
     """
@@ -133,34 +156,15 @@
     parser.add_argument(
         'filename',
         default=None,
         nargs='?',
         metavar='filename',
         help='The DataBlock zip file to open (optional).',
     )
-    parser.add_argument(
-        '--pyqt5',
-        action='store_true',
-        help='Run the DataBlock Viewer using the PyQt5 backend.',
-    )
-    parser.add_argument(
-        '--pyqt4',
-        action='store_true',
-        help='Run the DataBlock Viewer using the PyQt4 backend.',
-    )
-    parser.add_argument(
-        '--pyside',
-        action='store_true',
-        help='Run the DataBlock Viewer using the PySide backend.',
-    )
-    parser.add_argument(
-        '--pyside2',
-        action='store_true',
-        help='Run the DataBlock Viewer using the PySide2 backend.',
-    )
+    add_qtforce_arguments(parser)
     parser.set_defaults(func=block)
 
 
 #
 # Compare
 #
 
@@ -417,29 +421,23 @@
     """
     import platform
 
     plat = platform.system()
     if plat == 'Linux':
         yesno = \
             'Install launcher icons and file type associations for Gnome/KDE? '
-        try:
-            yesno = raw_input(yesno)
-        except NameError:   # pragma: no python 2 cover
-            yesno = input(yesno)
+        yesno = input(yesno)
         yesno = (yesno.strip().lower())[:1] == 'y'
 
         if yesno:
             install_gnome_kde()
 
     elif plat == 'Windows':
         yesno = 'Install start menu shortcuts? '
-        try:
-            yesno = raw_input(yesno)
-        except NameError:   # pragma: no python 2 cover
-            yesno = input(yesno)
+        yesno = input(yesno)
         yesno = (yesno.strip().lower())[:1] == 'y'
 
         if yesno:
             install_windows()
 
     elif plat == 'Darwin':
         print(
@@ -583,46 +581,25 @@
     parser.set_defaults(func=install)
 
 
 #
 # IDE
 #
 
-def ide(filename, pyqt4=False, pyqt5=False, pyside=False, pyside2=False):
+def ide(filename, pyqt6=False, pyqt5=False, pyside6=False, pyside2=False):
     """
     Runs the Myokit IDE.
     """
+    qtforce(pyqt6, pyqt5, pyside6, pyside2)
+
     import os
-    import myokit
-    if pyqt5:
-        myokit.FORCE_PYQT5 = True
-        myokit.FORCE_PYQT4 = False
-        myokit.FORCE_PYSIDE = False
-        myokit.FORCE_PYSIDE2 = False
-    elif pyqt4:
-        myokit.FORCE_PYQT5 = False
-        myokit.FORCE_PYQT4 = True
-        myokit.FORCE_PYSIDE = False
-        myokit.FORCE_PYSIDE2 = False
-    elif pyside:
-        myokit.FORCE_PYQT5 = False
-        myokit.FORCE_PYQT4 = False
-        myokit.FORCE_PYSIDE = True
-        myokit.FORCE_PYSIDE2 = False
-    elif pyside2:
-        myokit.FORCE_PYQT5 = False
-        myokit.FORCE_PYQT4 = False
-        myokit.FORCE_PYSIDE = False
-        myokit.FORCE_PYSIDE2 = True
-    import myokit.gui
-    import myokit.gui.ide
-    if pyqt5 or pyqt4 or pyside or pyside2:
-        print('Using backend: ' + myokit.gui.backend)
     if filename is not None:
         filename = os.path.abspath(os.path.expanduser(filename))
+
+    import myokit.gui.ide
     myokit.gui.run(myokit.gui.ide.MyokitIDE, filename)
 
 
 def add_ide_parser(subparsers):
     """
     Adds a subcommand parser for the ``compare`` command.
     """
@@ -634,34 +611,15 @@
     parser.add_argument(
         'filename',
         default=None,
         nargs='?',
         metavar='filename',
         help='The mmt file to open (optional).',
     )
-    parser.add_argument(
-        '--pyqt5',
-        action='store_true',
-        help='Run the IDE using the PyQt5 backend.',
-    )
-    parser.add_argument(
-        '--pyqt4',
-        action='store_true',
-        help='Run the IDE using the PyQt4 backend.',
-    )
-    parser.add_argument(
-        '--pyside',
-        action='store_true',
-        help='Run the IDE using the PySide backend.',
-    )
-    parser.add_argument(
-        '--pyside2',
-        action='store_true',
-        help='Run the DataBlock Viewer using the PySide2 backend.',
-    )
+    add_qtforce_arguments(parser)
     parser.set_defaults(func=ide)
 
 
 #
 # Import
 #
 
@@ -737,19 +695,20 @@
     parser.set_defaults(func=mmt_import)
 
 
 #
 # Log viewer
 #
 
-def log(filenames):
+def log(filenames, pyqt6=False, pyqt5=False, pyside6=False, pyside2=False):
     """
     Runs the DataLog Viewer.
     """
-    import myokit.gui
+    qtforce(pyqt6, pyqt5, pyside6, pyside2)
+
     import myokit.gui.datalog_viewer
     myokit.gui.run(myokit.gui.datalog_viewer.DataLogViewer, *filenames)
 
 
 def add_log_parser(subparsers):
     """
     Adds a subcommand parser for the ``log`` command.
@@ -757,14 +716,15 @@
     import argparse
 
     parser = subparsers.add_parser(
         'log',
         description='Runs the DataLog Viewer (PROTOTYPE).',
         help='Runs the DataLog Viewer (PROTOTYPE).',
     )
+    add_qtforce_arguments(parser)
     parser.add_argument(
         'filenames',
         default=None,
         nargs=argparse.REMAINDER,
         metavar='filename',
         help='The DataLog zip file to open (optional).',
     )
@@ -863,18 +823,15 @@
 
     print('Please select an OpenCL device by typing ' + q)
     print('Leave blank to keep current selection.')
 
     try:
         while True:
             x = 'Select device: '
-            try:
-                x = raw_input(x)
-            except NameError:   # pragma: no python 2 cover
-                x = input(x)    # lgtm [py/use-of-input]
+            x = input(x)
             x = x.strip()
             if x == '':
                 x = None
                 break
             try:
                 x = int(x)
                 if x > 0 and x <= n:
@@ -928,18 +885,15 @@
     import myokit
 
     # Ask user if settings should be deleted
     if force:
         remove = True
     else:
         yesno = 'Remove all Myokit settings files? '
-        try:
-            yesno = raw_input(yesno)
-        except NameError:           # pragma: no python 2 cover
-            yesno = input(yesno)    # lgtm [py/use-of-input]
+        yesno = input(yesno)
         yesno = yesno.strip().lower()
         remove = (yesno[:1] == 'y')
     if remove:
         print('Removing')
         print('  ' + myokit.DIR_USER)
         myokit.tools.rmtree(myokit.DIR_USER)
         print('Done')
@@ -1325,15 +1279,15 @@
     import os
     import subprocess
     import sys
 
     try:
         print('Gathering coverage data')
         p = subprocess.Popen([
-            'python3',
+            sys.executable,
             '-m',
             'coverage',
             'run',
             'myokit',
             'test',
             'unit',
         ])
@@ -1349,15 +1303,15 @@
             sys.exit(1)
         if ret != 0:
             print('FAILED')
             sys.exit(ret)
 
         print('Generating coverage report.')
         p = subprocess.Popen([
-            'python3',
+            sys.executable,
             '-m',
             'coverage',
             'report',
             '-m',
             '--skip-covered',
         ])
         p.wait()
@@ -1780,16 +1734,15 @@
     cmd = [sys.executable, '-c', code]
     curdir = os.getcwd()
     try:
         os.chdir(root)
         p = subprocess.Popen(
             cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, env=env
         )
-        stdout, stderr = p.communicate()
-        # TODO: Use p.communicate(timeout=3600) if Python3 only
+        stdout, stderr = p.communicate(timeout=3600)
         if p.returncode != 0:
             # Show failing code, output and errors before returning
             print('ERROR')
             print('-- script ' + '-' * (79 - 10))
             for i, line in enumerate(code.splitlines()):
                 j = str(1 + i)
                 print(j + ' ' * (5 - len(j)) + line)
```

### Comparing `myokit-1.34.0/myokit/_aux.py` & `myokit-1.35.0/myokit/_aux.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 # Myokit auxillary functions: This module can be used to gather any
 # functions that are important enough to warrant inclusion in the main
 # myokit module but don't belong to any specific hidden module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
 
 import sys
 
 # Globally shared numpy expression writer
 _numpywriter_ = None
 
@@ -25,15 +22,15 @@
 
     def __init__(self):
         # Deprecated since 2021-03-24
         import warnings
         warnings.warn(
             'The class `myokit.Benchmarker` is deprecated.'
             ' Please use `myokit.tools.Benchmarker` instead.')
-        super(Benchmarker, self).__init__()
+        super().__init__()
 
 
 def date():
     """
     Returns the current date and time, in the format used throughout Myokit.
     """
     import time
@@ -146,15 +143,15 @@
     import warnings
     warnings.warn(
         'The method `myokit.format_path` is deprecated.'
         ' Please use `myokit.tools.format_path` instead.')
     return myokit.tools.format_path(path, root)
 
 
-class ModelComparison(object):
+class ModelComparison:
     """
     Compares two models.
 
     The resulting diff text can be iterated over::
 
         for line in ModelComparison(m1, m2):
             print(line)
@@ -516,17 +513,17 @@
     #   3 x = 1/0
     #
     # will raise an exception on line 3.
     #
     script = '\n' + script
 
     # Class to run scripts
-    class Runner(object):
+    class Runner:
         def __init__(self, model, protocol, script, stdout, stderr, progress):
-            super(Runner, self).__init__()
+            super().__init__()
             self.model = model
             self.protocol = protocol
             self.script = script
             self.stdout = stdout
             self.stderr = stderr
             self.progress = progress
             self.exc_info = None
@@ -551,15 +548,15 @@
                 if self.stderr is not None:
                     oldstderr = sys.stderr
                     sys.stderr = self.stderr
                 environment = {
                     'get_model': get_model,
                     'get_protocol': get_protocol,
                 }
-                myokit._exec(self.script, environment)
+                exec(self.script, environment)
             finally:
                 if oldstdout is not None:
                     sys.stdout = oldstdout
                 if oldstderr is not None:
                     sys.stderr = oldstderr
                 myokit._Simulation_progress = oldprogress
```

### Comparing `myokit-1.34.0/myokit/_bin/example.mmt` & `myokit-1.35.0/myokit/_bin/example.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/find.png` & `myokit-1.35.0/myokit/_bin/gui/find.png`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-128.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-128.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-16.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-16.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-24.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-24.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-256.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-256.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-32.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-32.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-48.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-48.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-64.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-64.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-96.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-96.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer.ico` & `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer.ico`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer.png` & `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer.png`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-ide-128.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-ide-128.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-ide-16.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-ide-16.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-ide-24.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-ide-24.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-ide-256.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-ide-256.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-ide-32.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-ide-32.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-ide-48.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-ide-48.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-ide-64.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-ide-64.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-ide-96.xpm` & `myokit-1.35.0/myokit/_bin/gui/icon-ide-96.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-ide.ico` & `myokit-1.35.0/myokit/_bin/gui/icon-ide.ico`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/icon-ide.png` & `myokit-1.35.0/myokit/_bin/gui/icon-ide.png`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/new.png` & `myokit-1.35.0/myokit/_bin/gui/new.png`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/open.png` & `myokit-1.35.0/myokit/_bin/gui/open.png`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/gui/save.png` & `myokit-1.35.0/myokit/_bin/gui/save.png`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/install-lin/myokit.lang` & `myokit-1.35.0/myokit/_bin/install-lin/myokit.lang`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/install-win/menu.json` & `myokit-1.35.0/myokit/_bin/install-win/menu.json`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/LICENSE` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/LICENSE`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib` & `myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_config.py` & `myokit-1.35.0/myokit/_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 #
 # Loads settings from configuration file in user home directory or attempts to
 # guess best settings.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-# Load Myokit, at least, the bit that's been setup so far. This just means
-# this method will add a link to the myokit module already being loaded
-# into this method's namespace. This allows us to use the constants defined
-# before this method was called.
-import myokit
-
-# Load standard library modules
+import configparser
 import logging
 import os
 import platform
 import sys
 import warnings
 
-# ConfigParser in Python 2 and 3
-try:
-    from ConfigParser import ConfigParser
-except ImportError:
-    from configparser import RawConfigParser as ConfigParser
+# Load Myokit, at least, the bit that's been setup so far. This just means
+# this method will add a link to the myokit module already being loaded
+# into this method's namespace. This allows us to use the constants defined
+# before this method was called.
+import myokit
 
 
 def _create(path):
     """
     Attempts to guess the best settings and stores them in a new configuration
     file.
     """
     # Get operating system
     system = platform.system()
 
     # Create config parser
-    config = ConfigParser(allow_no_value=True)
+    config = configparser.RawConfigParser(allow_no_value=True)
 
     # Make the parser case sensitive (need for unix paths!)
     config.optionxform = str
 
     # General information
     config.add_section('myokit')
     config.set(
@@ -67,20 +58,20 @@
     config.set('time', '# Time format used throughout Myokit')
     config.set('time', '# The format should be acceptable for time.strftime')
     config.set('time', 'time_format', myokit.TIME_FORMAT)
 
     # GUI Backend
     config.add_section('gui')
     config.set('gui', '# Backend to use for graphical user interface.')
-    config.set('gui', '# Valid options are pyqt5, pyqt4, pyside2 and pyside.')
+    config.set('gui', '# Valid options are pyqt6, pyqt5, pyside6 and pyside2.')
     config.set('gui', '# Leave unset for automatic selection.')
+    config.set('gui', '#backend = pyqt6')
     config.set('gui', '#backend = pyqt5')
-    config.set('gui', '#backend = pyqt4')
+    config.set('gui', '#backend = pyside6')
     config.set('gui', '#backend = pyside2')
-    config.set('gui', '#backend = pyside')
 
     # Locations of sundials library
     config.add_section('sundials')
     config.set(
         'sundials', '# Location of sundials shared libary files'
         ' (.so, .dll, or .dylib).')
     config.set('sundials', '# Multiple paths can be set using ; as separator.')
@@ -219,15 +210,15 @@
                     'Unsupported syntax found in ' + str(path) + ' on line '
                     + str(1 + i) + ', character ' + str(x) + ', semicolons (;)'
                     + ' must not be preceded by whitespace: ```'
                     + line.strip() + '```.')
         del lines, inline_comment
 
     # Create the config parser (no value allows comments)
-    config = ConfigParser(allow_no_value=True)
+    config = configparser.RawConfigParser(allow_no_value=True)
 
     # Make the parser case sensitive (need for unix paths!)
     config.optionxform = str
 
     # Parse the config file
     config.read(path)
 
@@ -266,38 +257,38 @@
         x = config.get('time', 'time_format')
         if x:
             myokit.TIME_FORMAT = str(x)
 
     # GUI Backend
     if config.has_option('gui', 'backend'):
         x = config.get('gui', 'backend').strip().lower()
-        if x == 'pyqt' or x == 'pyqt4':
-            myokit.FORCE_PYQT4 = True
+        if x == 'pyqt6':
+            myokit.FORCE_PYQT6 = True
             myokit.FORCE_PYQT5 = False
-            myokit.FORCE_PYSIDE = False
+            myokit.FORCE_PYSIDE6 = False
             myokit.FORCE_PYSIDE2 = False
         elif x == 'pyqt5':
-            myokit.FORCE_PYQT4 = False
+            myokit.FORCE_PYQT6 = False
             myokit.FORCE_PYQT5 = True
-            myokit.FORCE_PYSIDE = False
+            myokit.FORCE_PYSIDE6 = False
             myokit.FORCE_PYSIDE2 = False
-        elif x == 'pyside':
-            myokit.FORCE_PYQT4 = False
+        elif x == 'pyside6':
+            myokit.FORCE_PYQT6 = False
             myokit.FORCE_PYQT5 = False
-            myokit.FORCE_PYSIDE = True
+            myokit.FORCE_PYSIDE6 = True
             myokit.FORCE_PYSIDE2 = False
         elif x == 'pyside2':
-            myokit.FORCE_PYQT4 = False
+            myokit.FORCE_PYQT6 = False
             myokit.FORCE_PYQT5 = False
-            myokit.FORCE_PYSIDE = False
+            myokit.FORCE_PYSIDE6 = False
             myokit.FORCE_PYSIDE2 = True
         elif x != '':
             warnings.warn(
                 'Invalid setting in myokit.ini. Expected values for backend'
-                ' are pyqt, pyqt4, pyqt5, pyside, or pyside2. Got: ' + x)
+                ' are pyqt6, pyqt5, pyside6, or pyside2. Got: ' + x)
 
     # Sundials libraries, header files, and version
     if config.has_option('sundials', 'lib'):
         myokit.SUNDIALS_LIB.extend(_path_list(config.get('sundials', 'lib')))
     if config.has_option('sundials', 'inc'):
         myokit.SUNDIALS_INC.extend(_path_list(config.get('sundials', 'inc')))
```

### Comparing `myokit-1.34.0/myokit/_datablock.py` & `myokit-1.35.0/myokit/_datablock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #
 # Containers for time-series of 1d and 2d rectangular data arrays.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
+import array
 import os
 import sys
-import array
-import numpy as np
+
 import myokit
 
+import numpy as np
+
 
 # Readme file for DataBlock1d binary files
 README_SAVE_1D = """
 Myokit DataBlock1d Binary File
 ==============================
 This zip file contains simulation data in the form of multiple time series.
 Zero-dimensional time series, such as time or a global pace variable are
@@ -81,15 +80,15 @@
 
 """.strip()
 
 # Encoding used for text portions of zip files
 ENC = 'utf-8'
 
 
-class DataBlock1d(object):
+class DataBlock1d:
     """
     Container for time-series of 1d rectangular data arrays.
 
     Each ``DataBlock1d`` has a fixed width ``w``, and a 0d time series vector
     containing a sequence of ``n`` times.
 
     One-dimensional time series can be added to the block, provided the data
@@ -472,25 +471,18 @@
             import zlib
             del zlib
         except ImportError:
             raise Exception(
                 'This method requires the ``zlib`` module to be installed.')
 
         # Get size of single and double types on this machine
-        try:
-            dsize = {
-                'd': len(array.array('d', [1]).tobytes()),
-                'f': len(array.array('f', [1]).tobytes()),
-            }
-        except (AttributeError, TypeError):  # pragma: no python 3 cover
-            # List dtype as str for Python 2.7.10 (see #225)
-            dsize = {
-                b'd': len(array.array(b'd', [1]).tostring()),
-                b'f': len(array.array(b'f', [1]).tostring()),
-            }
+        dsize = {
+            'd': len(array.array('d', [1]).tobytes()),
+            'f': len(array.array('f', [1]).tobytes()),
+        }
 
         # Read data from file
         try:
             f = None
             f = zipfile.ZipFile(filename, 'r')
             info = f.infolist()
             if len(info) < 3:
@@ -540,16 +532,14 @@
                     fraction = 1.0 / fraction
                 iprogress = 0
                 progress.update(iprogress * fraction)
             head = iter(head)
             nt = int(next(head))
             nx = int(next(head))
             dtype = next(head)[1:-1]
-            # Convert dtype to str for Python 2.7.10 (see #225)
-            dtype = str(dtype)
             if dtype not in dsize:
                 raise myokit.DataBlockReadError(
                     'Unable to read DataBlock1d: Unrecognized data type "'
                     + dtype + '".')
             names_0d = []
             names_1d = []
             name = next(head)
@@ -569,18 +559,15 @@
             # Read time
             end += n0
             if end > nb:
                 raise myokit.DataBlockReadError(
                     'Unable to read DataBlock1d: Header indicates larger data'
                     ' than found in the body.')
             data = array.array(dtype)
-            try:
-                data.frombytes(body[start:end])
-            except AttributeError:  # pragma: no python 3 cover
-                data.fromstring(body[start:end])
+            data.frombytes(body[start:end])
             if sys.byteorder == 'big':  # pragma: no cover
                 data.byteswap()
             data = np.array(data)
             if progress:
                 iprogress += 1
                 if not progress.update(iprogress * fraction):
                     return
@@ -593,18 +580,15 @@
                 start = end
                 end += n0
                 if end > nb:
                     raise myokit.DataBlockReadError(
                         'Unable to read DataBlock1d: Header indicates larger'
                         ' data than found in the body.')
                 data = array.array(dtype)
-                try:
-                    data.frombytes(body[start:end])
-                except AttributeError:  # pragma: no python 3 cover
-                    data.fromstring(body[start:end])
+                data.frombytes(body[start:end])
                 if sys.byteorder == 'big':  # pragma: no cover
                     data.byteswap()
                 data = np.array(data)
                 block.set0d(name, data, copy=False)
                 if progress:
                     iprogress += 1
                     if not progress.update(iprogress * fraction):
@@ -615,18 +599,15 @@
                 start = end
                 end += n1
                 if end > nb:
                     raise myokit.DataBlockReadError(
                         'Unable to read DataBlock1d: Header indicates larger'
                         ' data than found in the body.')
                 data = array.array(dtype)
-                try:
-                    data.frombytes(body[start:end])
-                except AttributeError:  # pragma: no python 3 cover
-                    data.fromstring(body[start:end])
+                data.frombytes(body[start:end])
                 if sys.byteorder == 'big':  # pragma: no cover
                     data.byteswap()
                 data = np.array(data).reshape(nt, nx, order='C')
                 block.set1d(name, data, copy=False)
                 if progress:
                     iprogress += 1
                     if not progress.update(iprogress * fraction):
@@ -676,16 +657,15 @@
             import zlib
             del zlib
         except ImportError:
             raise Exception(
                 'This method requires the ``zlib`` module to be installed.')
 
         # Data type
-        # Create dtype as str for Python 2.7.10 (see #225)
-        dtype = str('d')     # Only supporting doubles right now
+        dtype = 'd'     # Only supporting doubles right now
 
         # Create header
         head_str = []
         head_str.append(str(self._nt))
         head_str.append(str(self._nx))
         head_str.append('"' + dtype + '"')
         for name in self._0d:
@@ -702,18 +682,15 @@
         for name, data in self._0d.items():
             body_str.append(array.array(dtype, data))
         for name, data in self._1d.items():
             body_str.append(array.array(dtype, data.reshape(n, order='C')))
         if sys.byteorder == 'big':  # pragma: no cover
             for ar in body_str:
                 ar.byteswap()
-        try:
-            body_str = b''.join([ar.tobytes() for ar in body_str])
-        except AttributeError:  # pragma: no python 3 cover
-            body_str = b''.join([ar.tostring() for ar in body_str])
+        body_str = b''.join([ar.tobytes() for ar in body_str])
 
         # Write
         head = zipfile.ZipInfo('header_block1d.txt')
         head.compress_type = zipfile.ZIP_DEFLATED
         body = zipfile.ZipInfo('data.bin')
         body.compress_type = zipfile.ZIP_DEFLATED
         read = zipfile.ZipInfo('readme.txt')
@@ -799,15 +776,15 @@
         Returns a 0d time series of the value ``variable``, corresponding to
         the cell at position ``x``. The data is returned directly, no copy is
         made.
         """
         return self._1d[variable][:, x]
 
 
-class DataBlock2d(object):
+class DataBlock2d:
     """
     Container for time-series of 2d rectangular data arrays.
 
     Each ``DataBlock2d`` has a fixed width ``w`` and height ``h``, and a 0d
     time series vector containing a sequence of ``n`` times.
 
     Two-dimensional time series can be added to the block, provided the data
@@ -1270,25 +1247,18 @@
             import zlib
             del zlib
         except ImportError:
             raise Exception(
                 'This method requires the ``zlib`` module to be installed.')
 
         # Get size of single and double types on this machine
-        try:
-            dsize = {
-                'd': len(array.array('d', [1]).tobytes()),
-                'f': len(array.array('f', [1]).tobytes()),
-            }
-        except (AttributeError, TypeError):  # pragma: no python 3 cover
-            # List dtype as str for Python 2.7.10 (see #225)
-            dsize = {
-                b'd': len(array.array(b'd', [1]).tostring()),
-                b'f': len(array.array(b'f', [1]).tostring()),
-            }
+        dsize = {
+            'd': len(array.array('d', [1]).tobytes()),
+            'f': len(array.array('f', [1]).tobytes()),
+        }
 
         # Read data from file
         try:
             f = None
             f = zipfile.ZipFile(filename, 'r')
             info = f.infolist()
             if len(info) < 3:
@@ -1349,16 +1319,15 @@
                 progress.update(iprogress * fraction)
             head = iter(head)
             nt = int(next(head))
             ny = int(next(head))
             nx = int(next(head))
 
             # Get dtype
-            # Convert dtype to str for Python 2.7.10 (see #225)
-            dtype = str(next(head))[1:-1]
+            dtype = next(head)[1:-1]
             if dtype not in dsize:
                 raise myokit.DataBlockReadError(
                     'Unable to read DataBlock2d: Unrecognized data type "'
                     + str(dtype) + '".')
 
             names_0d = []
             names_2d = []
@@ -1380,18 +1349,15 @@
             end += n0
             if end > nb:
                 raise myokit.DataBlockReadError(
                     'Unable to read DataBlock2d: Header indicates larger data'
                     ' than found in the body.')
 
             data = array.array(dtype)
-            try:
-                data.frombytes(body[start:end])
-            except AttributeError:  # pragma: no python 3 cover
-                data.fromstring(body[start:end])
+            data.frombytes(body[start:end])
             if sys.byteorder == 'big':  # pragma: no cover
                 data.byteswap()
             data = np.array(data)
             if progress:
                 iprogress += 1
                 if not progress.update(iprogress * fraction):
                     return
@@ -1404,18 +1370,15 @@
                 start = end
                 end += n0
                 if end > nb:
                     raise myokit.DataBlockReadError(
                         'Unable to read DataBlock2d: Header indicates larger'
                         ' data than found in the body.')
                 data = array.array(dtype)
-                try:
-                    data.frombytes(body[start:end])
-                except AttributeError:  # pragma: no python 3 cover
-                    data.fromstring(body[start:end])
+                data.frombytes(body[start:end])
                 if sys.byteorder == 'big':  # pragma: no cover
                     data.byteswap()
                 data = np.array(data)
                 block.set0d(name, data, copy=False)
                 if progress:
                     iprogress += 1
                     if not progress.update(iprogress * fraction):
@@ -1426,18 +1389,15 @@
                 start = end
                 end += n2
                 if end > nb:
                     raise myokit.DataBlockReadError(
                         'Unable to read DataBlock2d: Header indicates larger'
                         ' data than found in the body.')
                 data = array.array(dtype)
-                try:
-                    data.frombytes(body[start:end])
-                except AttributeError:  # pragma: no python 3 cover
-                    data.fromstring(body[start:end])
+                data.frombytes(body[start:end])
                 if sys.byteorder == 'big':  # pragma: no cover
                     data.byteswap()
                 data = np.array(data).reshape(nt, ny, nx, order='C')
                 block.set2d(name, data, copy=False)
                 if progress:
                     iprogress += 1
                     if not progress.update(iprogress * fraction):
@@ -1492,16 +1452,15 @@
             import zlib
             del zlib
         except ImportError:
             raise Exception(
                 'This method requires the ``zlib`` module to be installed.')
 
         # Data type
-        # Create dtype as str for Python 2.7.10 (see #225)
-        dtype = str('d')  # Only supporting doubles right now
+        dtype = 'd'     # Only supporting doubles right now
 
         # Create header
         head_str = []
         head_str.append(str(self._nt))
         head_str.append(str(self._ny))
         head_str.append(str(self._nx))
         head_str.append('"' + dtype + '"')
@@ -1519,18 +1478,15 @@
         for name, data in self._0d.items():
             body_str.append(array.array(dtype, data))
         for name, data in self._2d.items():
             body_str.append(array.array(dtype, data.reshape(n, order='C')))
         if sys.byteorder == 'big':  # pragma: no cover
             for ar in body_str:
                 ar.byteswap()
-        try:
-            body_str = b''.join([ar.tobytes() for ar in body_str])
-        except AttributeError:  # pragma: no python 3 cover
-            body_str = b''.join([ar.tostring() for ar in body_str])
+        body_str = b''.join([ar.tobytes() for ar in body_str])
 
         # Write
         head = zipfile.ZipInfo('header_block2d.txt')
         head.compress_type = zipfile.ZIP_DEFLATED
         body = zipfile.ZipInfo('data.bin')
         body.compress_type = zipfile.ZIP_DEFLATED
         read = zipfile.ZipInfo('readme.txt')
@@ -1667,15 +1623,15 @@
         Returns a 0d time series of the value ``variable``, corresponding to
         the cell at position ``x``, ``y``. The data is returned directly, no
         copy is made.
         """
         return self._2d[variable][:, y, x]
 
 
-class ColorMap(object):
+class ColorMap:
     """
     *Abstract class*
 
     Applies colormap transformations to floating point data and returns RGB
     data.
 
     :class:`ColorMaps <ColorMap>` are callable objects and take the following
```

### Comparing `myokit-1.34.0/myokit/_datalog.py` & `myokit-1.35.0/myokit/_datalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 #
 # Functions relating to the DataLog class for storing time series data.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import re
 import sys
 import array
+
 import numpy as np
+
 from collections import OrderedDict
-import myokit
 
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
+import myokit
 
 
 # Function to split keys into dimension-key,qname-key pairs
 ID_NAME_PATTERN = re.compile(r'(\d+.)+')
 
 # Readme file for DataLog binary files
 README_SAVE_BIN = """
@@ -97,19 +91,19 @@
         the ``time`` argument will overwrite the cloned value.
 
     """
 
     def __init__(self, other=None, time=None):
         if other is None:
             # Create new
-            super(DataLog, self).__init__()
+            super().__init__()
             self._time = None
         else:
             # Clone
-            super(DataLog, self).__init__(other)
+            super().__init__(other)
             try:
                 self._time = str(other._time)
             except Exception:
                 self._time = None
         if time is not None:
             self.set_time_key(time)
 
@@ -212,18 +206,18 @@
                 log[str(k)] = np.array(v, copy=True, dtype=float)
         else:
             for k, v in self.items():
                 log[str(k)] = list(v)
         return log
 
     def __contains__(self, key):
-        return super(DataLog, self).__contains__(self._parse_key(key))
+        return super().__contains__(self._parse_key(key))
 
     def __delitem__(self, key):
-        return super(DataLog, self).__delitem__(self._parse_key(key))
+        return super().__delitem__(self._parse_key(key))
 
     def extend(self, other):
         """
         Returns a copy of this log, extended with the data of another.
 
         Both logs must have the same keys and the same time key. The added data
         must be from later time points than in the log being extended.
@@ -324,15 +318,15 @@
         for i, log in enumerate(logs):
             for k, v in log.items():
                 if k != self._time:
                     out[k, i] = v
         return out
 
     def __getitem__(self, key):
-        return super(DataLog, self).__getitem__(self._parse_key(key))
+        return super().__getitem__(self._parse_key(key))
 
     def has_nan(self):
         """
         Returns True if one of the variables in this DataLog has a ``NaN`` as
         its final logged value.
         """
         for k, d in self.items():
@@ -513,25 +507,18 @@
             import zlib
             del zlib
         except ImportError:
             raise Exception(
                 'This method requires the ``zlib`` module to be installed.')
 
         # Get size of single and double types on this machine
-        try:
-            dsize = {
-                'd': len(array.array('d', [1]).tobytes()),
-                'f': len(array.array('f', [1]).tobytes()),
-            }
-        except (AttributeError, TypeError):  # pragma: no python 3 cover
-            # List dtype as str for Python 2.7.10 (see #225)
-            dsize = {
-                b'd': len(array.array(b'd', [1]).tostring()),
-                b'f': len(array.array(b'f', [1]).tostring()),
-            }
+        dsize = {
+            'd': len(array.array('d', [1]).tobytes()),
+            'f': len(array.array('f', [1]).tobytes()),
+        }
 
         # Read data
         try:
             f = None
             f = zipfile.ZipFile(filename, 'r')
             # Get ZipInfo objects
             try:
@@ -559,15 +546,15 @@
         log = DataLog()
 
         # Parse header
         # Number of fields, length of data arrays, data type, time, fields
         head = iter(head.splitlines())
         n = int(next(head))
         data_size = int(next(head))
-        data_type = str(next(head))  # Cast to str for Python 2.7.10 (see #225)
+        data_type = next(head)
         time = next(head)
         if time:
             # Note, this field doesn't have to be present in the log!
             log._time = time
         fields = [x for x in head]
         if len(fields) != n:
             raise myokit.DataLogReadError(
@@ -600,18 +587,15 @@
                 if end > nbody:
                     raise myokit.DataLogReadError(
                         'Header indicates larger data size than found in body.'
                     )
 
                 # Read data
                 ar = array.array(data_type)
-                try:
-                    ar.frombytes(body[start:end])
-                except AttributeError:  # pragma: no python 3 cover
-                    ar.fromstring(body[start:end])
+                ar.frombytes(body[start:end])
                 if sys.byteorder == 'big':  # pragma: no cover
                     ar.byteswap()
                 log[field] = ar
         finally:
             if progress:
                 progress.exit()
         return log
@@ -634,33 +618,25 @@
         safely be read.
         """
         log = DataLog()
         # Check filename
         filename = os.path.expanduser(filename)
 
         # Typecode dependent on precision
-        # Typecode must be str for Python 2.7.10 (see #225)
-        typecode = str('d' if precision == myokit.DOUBLE_PRECISION else 'f')
+        typecode = 'd' if precision == myokit.DOUBLE_PRECISION else 'f'
 
         # Error raising function
         def e(line, char, msg):
             raise myokit.DataLogReadError(
                 'Syntax error on line ' + str(line) + ', character '
                 + str(1 + char) + ': ' + msg)
 
-        def uopen(filename):
-            # Open a filename in 'universal newline' mode, python 2 and 3
-            try:
-                return open(filename, 'r', newline=None)
-            except TypeError:   # pragma: no python 3 cover
-                return open(filename, 'U')
-
         quote = '"'
         delim = ','
-        with uopen(filename) as f:
+        with open(filename, 'r', newline=None) as f:
             # Read header
             keys = []   # The log keys, in order of appearance
 
             # Read first line
             line = f.readline()
 
             # Ignore comments
@@ -932,16 +908,15 @@
             import zlib
             del zlib
         except ImportError:
             raise Exception(
                 'This method requires the `zlib` module to be installed.')
 
         # Data type
-        # dtype must be str for Python 2.7.10 (see #225)
-        dtype = str('d' if precision == myokit.DOUBLE_PRECISION else 'f')
+        dtype = 'd' if precision == myokit.DOUBLE_PRECISION else 'f'
 
         # Create data strings
         head_str = []
         body_str = []   # Will be filled with bytes
 
         # Number of fields, length of data arrays, data type, time, fields
         head_str.append(str(len(self)))
@@ -955,18 +930,15 @@
         enc = 'utf8'
         for k, v in self.items():
             head_str.append(k)
             # Create array, ensure it's litte-endian
             ar = array.array(dtype, v)
             if sys.byteorder == 'big':  # pragma: no cover
                 ar.byteswap()
-            try:
-                body_str.append(ar.tobytes())
-            except AttributeError:   # pragma: no python 3 cover
-                body_str.append(ar.tostring())
+            body_str.append(ar.tobytes())
         head_str = '\n'.join(head_str)
         body_str = b''.join(body_str)
 
         # 2018-07-15: Wondering why I chose body-head-readme ordering now...
 
         # Write
         head = zipfile.ZipInfo('structure.txt')
@@ -1002,15 +974,15 @@
         ``filename``
             The file to write (existing files will be overwritten without
             warning.
         ``precision``
             If a precision argument (for example ``myokit.DOUBLE_PRECISION``)
             is given, the output will be stored in such a way that this amount
             of precision is guaranteed to be present in the string. If the
-            precision argument is set to ``None`` python's default formatting
+            precision argument is set to ``None`` Python's default formatting
             is used, which may lead to smaller files.
         ``order``
             To specify the ordering of the log's arguments, pass in a sequence
             ``order`` with the log's keys.
         ``delimiter``
             This field can be used to set an alternative delimiter. To use
             spaces set ``delimiter=' '``, for tabs: ``delimiter='\\t'``. Note
@@ -1103,15 +1075,15 @@
     def set_time_key(self, key):
         """
         Sets the key under which the time data is stored.
         """
         self._time = None if key is None else str(key)
 
     def __setitem__(self, key, value):
-        return super(DataLog, self).__setitem__(
+        return super().__setitem__(
             self._parse_key(key), value)
 
     def split(self, value):
         """
         Splits the log into a part before and after the time ``value``::
 
             s = myokit.Simulation(m, p)
@@ -1418,15 +1390,15 @@
             # Add sorted keys
             s = '.' + name if id_list[0] else name
             info._keys = ['.'.join([str(x) for x in y]) + s for y in id_list]
 
         return infos
 
 
-class LoggedVariableInfo(object):
+class LoggedVariableInfo:
     """
     Contains information about the log entries for each variable. These objects
     should only be created by :meth:`DataLog.variable_info()`.
     """
     def __init__(self):
         self._dimension = None
         self._ids = None
@@ -1625,17 +1597,15 @@
     type of variables are allowed in this log.
 
     When a new DataLog is created by this method, the internal storage
     uses arrays from the array module. The data type for these new arrays can
     be specified using the ``precision`` argument.
     """
     # Typecode dependent on precision
-    # Note: Cast to str() here makes it work with older versions of 2.7.x,
-    # where unicode isn't accepted (Python 3 of course doesn't accept bytes)
-    typecode = str('d' if precision == myokit.DOUBLE_PRECISION else 'f')
+    typecode = 'd' if precision == myokit.DOUBLE_PRECISION else 'f'
 
     # Get all options for dimensionality
     if dims is None:
         dims = ()
     ndims = len(dims)
     if ndims == 0:
         dcombos = ['']
@@ -1870,15 +1840,15 @@
         if len(log) > 0:
             log[0]
     except Exception:
         raise ValueError(
             'Argument `log` has unexpected type. Expecting None, integer flag,'
             ' sequence of names, dict or DataLog.')
 
-    if isinstance(log, basestring):
+    if isinstance(log, str):
         raise ValueError(
             'String passed in as `log` argument, should be list'
             ' or other sequence containing strings.')
 
     # Parse log argument as list
     lst = log
     log = myokit.DataLog()
```

### Comparing `myokit-1.34.0/myokit/_err.py` & `myokit-1.35.0/myokit/_err.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #
 # Non-standard exceptions raised by myokit.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
 
 
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 #
 # Base classes
 #
 #
@@ -20,28 +18,28 @@
     Note that myokit classes and functions may raise any type of exception, for
     example a :class:``KeyError`` or a :class:`ValueError`. Only new classes of
     exception *defined* by Myokit will extend this base class.
 
     *Extends:* ``Exception``
     """
     def __init__(self, message):
-        super(MyokitError, self).__init__(message)
+        super().__init__(message)
 
 
 class IntegrityError(MyokitError):
     """
     Raised if an integrity error is found in a model.
 
     The error message is stored in the property ``message``. An optional parser
     token may be obtained with :meth:`token()`.
 
     *Extends:* :class:`myokit.MyokitError`
     """
     def __init__(self, message, token=None):
-        super(IntegrityError, self).__init__(message)
+        super().__init__(message)
         self._token = token
 
     def token(self):
         """
         Returns a parser token associated with this error, or ``None`` if no
         such token was given.
         """
@@ -73,15 +71,15 @@
     def __init__(self, cycle):
         # Set message
         msg = 'Cyclical reference found: (' + ' > '.join(
             [v.var().qname() for v in cycle]) + ').'
         # Set token: First item in cycle is model's defining lhs
         tok = cycle[0].var()._token
         # Raise
-        super(CyclicalDependencyError, self).__init__(msg, tok)
+        super().__init__(msg, tok)
 
 
 class DataBlockReadError(MyokitError):
     """
     Raised when an error is encountered while reading a
     :class:`myokit.DataBlock1d` or :class:`myokit.DataBlock2d`.
 
@@ -163,27 +161,27 @@
     """
     Raised when a reference is found to a variable ``reference`` that isn't
     accessible from the owning variable ``owner``'s scope.
 
     *Extends:* :class:`myokit.IntegrityError`
     """
     def __init__(self, reference, owner):
-        super(IllegalReferenceError, self).__init__(
+        super().__init__(
             'Illegal reference: The referenced variable <' + reference.qname()
             + '> is outside the scope of <' + owner.qname() + '>.')
 
 
 class IllegalReferenceInInitialValueError(IllegalReferenceError):
     """
     Raised when an illegal reference is made in an initial value.
 
     The only way this can occur is if the reference is to a nested variable.
     """
     def __init__(self, reference, owner):
-        super(IllegalReferenceError, self).__init__(
+        super(IntegrityError, self).__init__(
             'Illegal reference made in initial value: The referenced variable'
             ' <' + reference.qname() + '> is nested.')
 
 
 class ImportError(MyokitError):
     """
     Raised when an import from another format fails.
@@ -199,25 +197,25 @@
     *Extends:* :class:`myokit.MyokitError`.
     """
     def __init__(self, model_name, message):
         msg = 'Incompatible model'
         if model_name:
             msg += ' <' + str(model_name) + '>'
         msg += ': ' + str(message)
-        super(IncompatibleModelError, self).__init__(msg)
+        super().__init__(msg)
 
 
 class IncompatibleUnitError(MyokitError):
     """
     Raised when a unit incompatibility is detected.
 
     *Extends:* :class:`myokit.MyokitError`.
     """
     def __init__(self, message, token=None):
-        super(MyokitError, self).__init__(message)
+        super().__init__(message)
         self._token = token
 
     def token(self):
         """
         Returns a parser token associated with this error, or ``None`` if no
         such token was given.
         """
@@ -284,27 +282,27 @@
     The first argument ``var`` should be the invalid variable.
 
     *Extends:* :class:`myokit.IntegrityError`
     """
     def __init__(self, var):
         msg = 'No rhs set for <' + var.qname() + '>.'
         tok = var._token
-        super(MissingRhsError, self).__init__(msg, tok)
+        super().__init__(msg, tok)
 
 
 class MissingTimeVariableError(IntegrityError):
     """
     Raised when no variable was bound to time.
 
     *Extends:* :class:`myokit.IntegrityError`
     """
     def __init__(self):
         msg = 'No variable bound to time. At least one of the model\'s' \
               ' variables must be bound to "time".'
-        super(MissingTimeVariableError, self).__init__(msg)
+        super().__init__(msg)
 
 
 class NumericalError(MyokitError):
     """
     Raised when a numerical error occurs during the evaluation of a myokit
     :class:`Expression`.
 
@@ -335,15 +333,15 @@
         self.name = str(name)
         self.line = int(line)
         self.char = int(char)
         self.value = self.name + ' on line ' + str(self.line)
         self.desc = str(desc)
         self.value += ': ' + self.desc
         self.cause = cause
-        super(ParseError, self).__init__(self.value)
+        super().__init__(self.value)
 
 
 class ProtocolEventError(MyokitError):
     """
     Raised when a :class:`ProtocolEvent` is created with invalid parameters.
 
     *Extends:* :class:`myokit.MyokitError`
@@ -379,15 +377,15 @@
 class SimulationCancelledError(MyokitError):
     """
     Raised when a user terminates a simulation.
 
     *Extends:* :class:`myokit.MyokitError`
     """
     def __init__(self, message='Operation cancelled by user.'):
-        super(SimulationCancelledError, self).__init__(message)
+        super().__init__(message)
 
 
 class SimultaneousProtocolEventError(MyokitError):
     """
     Raised if two events in a protocol happen at the same time. Raised when
     creating a protocol or when running one.
 
@@ -398,15 +396,15 @@
 class UnresolvedReferenceError(IntegrityError):
     """
     Raised when a reference to a variable cannot be resolved.
 
     *Extends:* :class:`myokit.IntegrityError`
     """
     def __init__(self, reference, extra_message=None):
-        super(UnresolvedReferenceError, self).__init__(
+        super().__init__(
             'Unknown variable: <' + reference + '>.'
             + ((' ' + extra_message) if extra_message else '')
         )
 
 
 class UnusedVariableError(IntegrityError):
     """
@@ -415,15 +413,15 @@
     The unused variable must be passed in as the first argument ``var``.
 
     *Extends:* :class:`myokit.IntegrityError`
     """
     def __init__(self, var):
         msg = 'Unused variable: <' + var.qname() + '>.'
         tok = var.lhs()._token
-        super(UnusedVariableError, self).__init__(msg, tok)
+        super().__init__(msg, tok)
 
 
 class VariableMappingError(MyokitError):
     """
     Raised when a method needs to map variables from one model onto another,
     but no valid mapping can be made.
```

### Comparing `myokit-1.34.0/myokit/_expressions.py` & `myokit-1.35.0/myokit/_expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,35 @@
 #
 # Myokit symbolic expression classes. Defines different expressions, equations
 # and the unit system.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
+import io
 import math
 import numpy
 
 import myokit
+
 from myokit import IntegrityError
 
-# StringIO in Python 2 and 3
-try:
-    from cStringIO import StringIO
-except ImportError:
-    from io import StringIO
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
 
 # Expression precedence levels
 FUNCTION_CALL = 70
 POWER = 60
 PREFIX = 50
 PRODUCT = 40
 SUM = 30
 CONDITIONAL = 20
 CONDITION_AND = 10
 LITERAL = 0
 
 
-class Expression(object):
+class Expression:
     """
     Myokit's most generic interface for expressions. All expressions extend
     this class.
 
     Expressions are immutable objects.
 
     Expression objects have an ``_rbp`` property determining their *right
@@ -81,16 +69,16 @@
         # to way until a first request.
         self._cached_hash = None
         self._cached_polish = None
         self._cached_validation = None
         self._cached_unit_tolerant = None
         self._cached_unit_strict = None
 
-    def __bool__(self):     # pragma: no python 2 cover
-        """ Python 3 method to determine the outcome of "if expression". """
+    def __bool__(self):
+        # Determines the outcome of "if expression".
         return True
 
     def bracket(self, op=None):
         """
         Checks if the given operand (which should be an operand of this
         expression) needs brackets around it when writing a mathematical
         expression.
@@ -138,15 +126,15 @@
         - if the variable's component matches the argument ``component`` or the
           variable is nested, then the local variable name is used
         - if the given ``component`` has an alias for the variable, this alias
           is used.
         """
         # Note: Because variable and component names can change, the output of
         # code can not be cached (for non-literal expressions).
-        b = StringIO()
+        b = io.StringIO()
         self._code(b, component)
         return b.getvalue()
 
     def _code(self, b, c):
         """
         Internal version of ``code()``, should write the generated code to the
         stringbuffer ``b``, from the context of component ``c``.
@@ -536,28 +524,24 @@
         return result
 
     def _eval_unit(self, mode):
         """ Internal version of eval_unit(). """
         raise NotImplementedError
 
     def __float__(self):
-        # Cast to float is required in Python 3: numpy float etc. are ok, but
-        # this is deprecated.
         return float(self.eval())
 
     def __getitem__(self, key):
         return self._operands[key]
 
     def __hash__(self):
         if self._cached_hash is None:
             self._cached_hash = hash(self._polish())
         return self._cached_hash
-        # Note for Python3:
-        #   In Python3, anything that has an __eq__ stops inheriting this hash
-        #   method!
+        # Note: anything that has an __eq__ stops inheriting this hash method!
         # From: https://docs.python.org/3.1/reference/datamodel.html
         # > If a class that overrides __eq__() needs to retain the
         #   implementation of __hash__() from a parent class, the interpreter
         #   must be told this explicitly by setting
         #   __hash__ = <ParentClass>.__hash__. Otherwise the inheritance of
         #   __hash__() will be blocked, just as if __hash__ had been explicitly
         #   set to None.
@@ -627,18 +611,14 @@
 
     def __len__(self):
         return len(self._operands)
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
-    def __nonzero__(self):  # pragma: no python 3 cover
-        """ Python 2 method to determine the outcome of "if expression". """
-        return True
-
     def operator_rep(self):
         """
         Returns a representation of this expression's type. (For example '+' or
         '*')
         """
         return self._rep
 
@@ -649,15 +629,15 @@
         unambiguous expressions.
 
         Note that id's are immutable _during the Variable's lifetime_. Since a
         Name object stores a reference to the Variable, this means the
         variable id is immutable in the expression's lifetime.
         """
         if self._cached_polish is None:
-            b = StringIO()
+            b = io.StringIO()
             self._polishb(b)
             self._cached_polish = b.getvalue()
         return self._cached_polish
 
     def _polishb(self, b):
         """
         Recursive part of _polish(). Should write the generated code to the
@@ -666,15 +646,15 @@
         Because hash() and others use _polish(), this function should never
         use eval() or other advanced functions.
         """
         raise NotImplementedError
 
     def pyfunc(self, use_numpy=True):
         """
-        Converts this expression to python and returns the new function's
+        Converts this expression to Python and returns the new function's
         handle.
 
         By default, when converting mathematical functions such as ``log``, the
         version from ``numpy`` (i.e. ``numpy.log``) is used. To use the
         built-in ``math`` module instead, set ``use_numpy=False``.
         """
         # Get expression writer
@@ -687,27 +667,27 @@
         args = [w.ex(x) for x in self._references]
         c = 'def ex_pyfunc_generated(' + ','.join(args) + '):\n    return ' \
             + w.ex(self)
 
         # Create function
         local = {}
         if use_numpy:
-            myokit._exec(c, {'numpy': numpy}, local)
+            exec(c, {'numpy': numpy}, local)
         else:
-            myokit._exec(c, {'math': math}, local)
+            exec(c, {'math': math}, local)
 
         # Return
         return local['ex_pyfunc_generated']
 
     def pystr(self, use_numpy=False):
         """
-        Returns a string representing this expression in python syntax.
+        Returns a string representing this expression in Python syntax.
 
         By default, built-in functions such as 'exp' are converted to the
-        python version 'math.exp'. To use the numpy versions, set
+        Python version 'math.exp'. To use the numpy versions, set
         ``numpy=True``.
         """
         # Get expression writer
         if use_numpy:
             w = myokit.numpy_writer()
         else:
             w = myokit.python_writer()
@@ -738,15 +718,15 @@
         return self.code()
 
     def tree_str(self):
         """
         Returns a string representing the parse tree corresponding to this
         expression.
         """
-        b = StringIO()
+        b = io.StringIO()
         self._tree_str(b, 0)
         return b.getvalue()
 
     def _tree_str(self, b, n):
         raise NotImplementedError
 
     def validate(self):
@@ -851,29 +831,29 @@
         number's unit will be left undefined.
 
     *Extends:* :class:`Expression`
     """
     _rbp = LITERAL
 
     def __init__(self, value, unit=None):
-        super(Number, self).__init__()
+        super().__init__()
         if isinstance(value, myokit.Quantity):
             # Conversion from Quantity class
             if unit is not None:
                 raise ValueError(
                     'myokit.Number created from a myokit.Quantity cannot'
                     ' specify an additional unit.')
             self._value = value.value()
             self._unit = value.unit()
         else:
             # Basic creation with number and unit
             self._value = float(value) if value else 0.0
             if unit is None or isinstance(unit, myokit.Unit):
                 self._unit = unit
-            elif isinstance(unit, basestring):
+            elif isinstance(unit, str):
                 self._unit = myokit.parse_unit(unit)
             else:
                 raise ValueError(
                     'Unit in myokit.Number should be a myokit.Unit or None.')
         # Create nice string representation
         self._str = myokit.float.str(self._value)
         if self._str[-2:] == '.0':
@@ -1009,18 +989,18 @@
 class Name(LhsExpression):
     """
     Represents a reference to a variable.
 
     *Extends:* :class:`LhsExpression`
     """
     _rbp = LITERAL
-    __hash__ = LhsExpression.__hash__   # For Python3, when __eq__ is present
+    __hash__ = LhsExpression.__hash__
 
     def __init__(self, value):
-        super(Name, self).__init__()
+        super().__init__()
         self._value = value
         self._references = set([self])
         self._proper = isinstance(self._value, myokit.Variable)
 
     def bracket(self, op=None):
         """See :meth:`Expression.bracket()`."""
         if op is not None:
@@ -1050,15 +1030,15 @@
                 if c:
                     try:
                         b.write(c.alias_for(self._value))
                         return
                     except KeyError:
                         pass
                 b.write(self._value.qname(c))
-        elif isinstance(self._value, basestring):
+        elif isinstance(self._value, str):
             # Allow strings for debugging
             b.write('str:' + str(self._value))
         else:
             # Allow "misusing" the expression system by storing other types as
             # values.
             b.write(str(self._value))
 
@@ -1121,15 +1101,15 @@
         return (var is None) or (var == self._value)
 
     def is_state_value(self):
         """See: meth:`Expression.is_state_value()`."""
         return self._proper and self._value.is_state()
 
     def _polishb(self, b):
-        if isinstance(self._value, basestring):
+        if isinstance(self._value, str):
             # Allow an exception for strings
             b.write('str:')
             b.write(self._value)
         else:
             # Use object id here to make immutable references. This is fine
             # since references should always be to variable objects, and
             # variables are unique this way (one Variable('x') doesn't equal
@@ -1149,15 +1129,15 @@
                 return self._value.rhs()
         return None
 
     def _tree_str(self, b, n):
         b.write(' ' * n + str(self._value) + '\n')
 
     def _validate(self, trail):
-        super(Name, self)._validate(trail)
+        super()._validate(trail)
         # Check value: String is allowed at construction for debugging, but
         # not here!
         if not self._proper:
             raise IntegrityError(
                 'Name value "' + repr(self._value) + '" is not an instance of'
                 ' class myokit.Variable', self._token)
 
@@ -1170,18 +1150,18 @@
     """
     Represents a reference to the time-derivative of a variable.
 
     *Extends:* :class:`LhsExpression`
     """
     _rbp = FUNCTION_CALL
     _nargs = [1]    # Allows parsing as a function
-    __hash__ = LhsExpression.__hash__   # For Python3, when __eq__ is present
+    __hash__ = LhsExpression.__hash__
 
     def __init__(self, op):
-        super(Derivative, self).__init__((op,))
+        super().__init__((op,))
         if not isinstance(op, Name):
             raise IntegrityError(
                 'The dot() operator can only be used on variables.',
                 self._token)
         self._op = op
         self._proper = self._op._proper
         self._references = set([self])
@@ -1270,15 +1250,15 @@
         b.write(' ' * n + 'dot(' + str(self._op._value) + ')\n')
 
     def var(self):
         """See :meth:`LhsExpression.var()`."""
         return self._op._value
 
     def _validate(self, trail):
-        super(Derivative, self)._validate(trail)
+        super()._validate(trail)
         # Check that value is a variable has already been performed by name
         # Check if value is the name of a state variable
         if not self._op._value.is_state():
             raise IntegrityError(
                 'Derivatives can only be defined for state variables.',
                 self._token)
 
@@ -1291,26 +1271,26 @@
     This class is used when writing out derivatives of equations, but may _not_
     appear in right-hand-side expressions for model variables!
 
     *Extends:* :class:`LhsExpression`
     """
     _rbp = FUNCTION_CALL
     _nargs = [2]    # Allows parsing as a function
-    __hash__ = LhsExpression.__hash__   # For Python3, when __eq__ is present
+    __hash__ = LhsExpression.__hash__
 
     def __init__(self, var1, var2):
         if not isinstance(var1, (Name, Derivative)):
             raise IntegrityError(
                 'The first argument to a partial derivative must be a'
                 ' variable name or a dot() expression.')
         if not isinstance(var2, (Name, InitialValue)):
             raise IntegrityError(
                 'The second argument to a partial derivative must be a'
                 ' variable name or an initial value.')
-        super(PartialDerivative, self).__init__((var1, var2))
+        super().__init__((var1, var2))
 
         self._var1 = var1
         self._var2 = var2
         self._references = set([self])
         self._has_partials = True
 
     def bracket(self, op=None):
@@ -1402,18 +1382,18 @@
     This class is used when writing out derivatives of equations, but may _not_
     appear in right-hand-side expressions for model variables!
 
     *Extends:* :class:`LhsExpression`
     """
     _rbp = FUNCTION_CALL
     _nargs = [1]    # Allows parsing as a function
-    __hash__ = LhsExpression.__hash__   # For Python3, when __eq__ is present
+    __hash__ = LhsExpression.__hash__
 
     def __init__(self, var):
-        super(InitialValue, self).__init__((var, ))
+        super().__init__((var, ))
         if not isinstance(var, Name):
             raise IntegrityError(
                 'The first argument to an initial value must be a variable'
                 ' name.', self._token)
 
         self._var = var
         self._references = set([self])
@@ -1464,15 +1444,15 @@
         b.write(' ' * n + 'init(' + str(self._var._value) + ')\n')
 
     def var(self):
         """See :meth:`LhsExpression.var()`."""
         return self._var._value
 
     def _validate(self, trail):
-        super(InitialValue, self)._validate(trail)
+        super()._validate(trail)
         # Check if value is the name of a state variable
         var = self._var._value
         if not (isinstance(var, myokit.Variable) and var.is_state()):
             raise IntegrityError(
                 'Initial values can only be defined for state variables.',
                 self._token)
 
@@ -1483,15 +1463,15 @@
 
     *Abstract class, extends:* :class:`Expression`
     """
     _rbp = PREFIX
     _rep = None
 
     def __init__(self, op):
-        super(PrefixExpression, self).__init__((op,))
+        super().__init__((op,))
         self._op = op
 
     def bracket(self, op):
         """See :meth:`Expression.bracket()`."""
         if op != self._op:
             raise ValueError('Given operand is not used in this expression.')
         return (self._op._rbp > LITERAL) and (self._op._rbp < self._rbp)
@@ -1582,15 +1562,15 @@
 
     *Abstract class, extends:* :class:`Expression`
     """
     _rep = None      # Operator representation (+, *, et)
     _spaces_round_operator = True
 
     def __init__(self, left, right):
-        super(InfixExpression, self).__init__((left, right))
+        super().__init__((left, right))
         self._op1 = left
         self._op2 = right
 
     def bracket(self, op):
         """See :meth:`Expression.bracket()`."""
         if op == self._op1:
             return (op._rbp > LITERAL and (op._rbp < self._rbp))
@@ -2085,15 +2065,15 @@
     *Abstract class, extends:* :class:`Expression`
     """
     _nargs = [1]
     _fname = None
     _rbp = FUNCTION_CALL
 
     def __init__(self, *ops):
-        super(Function, self).__init__(ops)
+        super().__init__(ops)
         if self._nargs is not None:
             if not len(ops) in self._nargs:
                 raise IntegrityError(
                     'Function (' + str(self._fname) + ') created with wrong'
                     ' number of arguments (' + str(len(ops)) + ', expecting '
                     + ' or '.join([str(x) for x in self._nargs]) + ').',
                     self._token)
@@ -2656,15 +2636,15 @@
 
     *Extends:* :class:`Function`
     """
     _nargs = [3]
     _fname = 'if'
 
     def __init__(self, i, t, e):
-        super(If, self).__init__(i, t, e)
+        super().__init__(i, t, e)
         self._i = i     # if
         self._t = t     # then
         self._e = e     # else
 
     def condition(self):
         """
         Returns this if-function's condition.
@@ -2762,15 +2742,15 @@
 
     *Extends:* :class:`Function`
     """
     _nargs = None
     _fname = 'piecewise'
 
     def __init__(self, *ops):
-        super(Piecewise, self).__init__(*ops)
+        super().__init__(*ops)
 
         # Check number of arguments
         n = len(self._operands)
         if n % 2 == 0:
             raise IntegrityError(
                 'Piecewise function must have odd number of arguments:'
                 ' ([condition, value]+, else_value).', self._token)
@@ -2850,15 +2830,15 @@
     def pieces(self):
         """
         Returns an iterator over the pieces in this Piecewise.
         """
         return iter(self._e)
 
 
-class Condition(object):
+class Condition:
     """
     *Abstract class*
 
     Interface for conditional expressions that can be evaluated to True or
     False. Doesn't add any methods but simply indicates that this is a
     condition.
     """
```

### Comparing `myokit-1.34.0/myokit/_io.py` & `myokit-1.35.0/myokit/_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,19 @@
 # Myokit auxillary functions: This module can be used to gather any
 # functions that are important enough to warrant inclusion in the main
 # myokit module but don't belong to any specific hidden module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import array
+import io
 import os
 import sys
 
-# StringIO in Python 2 and 3
-try:
-    from cStringIO import StringIO
-except ImportError:  # pragma: no python 2 cover
-    from io import StringIO
-
 import myokit
 
 
 def _examplify(filename):
     """
     If ``filename`` is equal to "example" and there isn't a file with that
     name, this function returns the file specified by myokit.EXAMPLE. In all
@@ -141,27 +133,22 @@
 
         if parts[0] != 'state':     # pragma: no cover
             raise Exception('Invalid state file format [30].')
 
         code = parts[1]
         if code not in ['d', 'f']:  # pragma: no cover
             raise Exception('Invalid state file format [40].')
-        # Convert code to str for Python 2.7.10 (see #225)
-        code = str(code)
 
         size = int(parts[2])
         if size < 0:    # pragma: no cover
             raise Exception('Invalid state file format [50].')
 
         # Create array, read bytes into array
         ar = array.array(code)
-        try:
-            ar.frombytes(f.read(info))
-        except AttributeError:  # pragma: no python 3 cover
-            ar.fromstring(f.read(info))
+        ar.frombytes(f.read(info))
 
         # Always store as little endian
         if sys.byteorder == 'big':  # pragma: no cover
             ar.byteswap()
 
     return list(ar)
 
@@ -180,15 +167,15 @@
         raise ValueError(
             'At least one of [model, protocol, script] must not be None.')
 
     if filename:
         filename = os.path.expanduser(filename)
         f = open(filename, 'w')
     else:
-        f = StringIO()
+        f = io.StringIO()
     out = None
     try:
         if model is not None:
             if isinstance(model, myokit.Model):
                 model = model.code()
             else:
                 model = model.strip()
@@ -293,28 +280,24 @@
         import zlib
         del zlib
     except ImportError:
         raise Exception(
             'This method requires the `zlib` module to be installed.')
 
     # Data type
-    # Convert code to str for Python 2.7.10 (see #225)
-    code = str('d' if precision == myokit.DOUBLE_PRECISION else 'f')
+    code = 'd' if precision == myokit.DOUBLE_PRECISION else 'f'
 
     # Create array, ensure it's little-endian
     ar = array.array(code, state)
     if sys.byteorder == 'big':  # pragma: no cover
         ar.byteswap()
 
     # Store precision and data type in internal filename
     name = 'state_' + code + '_' + str(len(state))
     info = zipfile.ZipInfo(name)
     info.compress_type = zipfile.ZIP_DEFLATED
 
     # Write to compressed file
-    try:
-        ar = ar.tobytes()
-    except AttributeError:  # pragma: no python 3 cover
-        ar = ar.tostring()
+    ar = ar.tobytes()
     with zipfile.ZipFile(filename, 'w') as f:
         f.writestr(info, ar)
```

### Comparing `myokit-1.34.0/myokit/_model_api.py` & `myokit-1.35.0/myokit/_model_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,45 +1,32 @@
 #
 # Defines the python classes that represent a Myokit model.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-from collections import OrderedDict
+import io
 import math
 import re
+
+from collections import OrderedDict
+
 import myokit
 
-# StringIO in Python 2 and 3
-try:
-    from cStringIO import StringIO
-except ImportError:
-    from io import StringIO
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
 
 TAB = ' ' * 4
 NAME = re.compile(r'^[a-zA-Z]\w*$')
 META = re.compile(r'^[a-zA-Z]\w*(:[a-zA-Z]\w*)*$')
 
 
 def check_name(name):
     """
     Tests if the given name is a valid myokit name and raises a
     :class:`myokit.InvalidNameError` if it isn't.
     """
-    # Note: Names are stored as str (so unicode in Python3)
-    # But the regex restriction means their format is compatible with ascii.
     # Check str compatibility
     name = str(name)
 
     # Check name syntax
     if NAME.match(name) is None:
         raise myokit.InvalidNameError(
             'The name <' + str(name) + '> is  invalid. The first character of'
@@ -61,37 +48,37 @@
 
     def __getitem__(self, key):
         # Check key
         if META.match(key) is None:
             raise myokit.InvalidMetaDataNameError(
                 'The key <' + str(key) + '>'
                 ' is not a valid meta-data property identifier.')
-        return super(MetaDataContainer, self).__getitem__(key)
+        return super().__getitem__(key)
 
     def __setitem__(self, key, item):
         # Check item
         item = str(item)
         # Check key
         if META.match(key) is None:
             raise myokit.InvalidMetaDataNameError(
                 'The key <' + str(key) + '>'
                 ' is not a valid meta-data property identifier.')
-        super(MetaDataContainer, self).__setitem__(key, item)
+        super().__setitem__(key, item)
 
 
-class ObjectWithMeta(object):
+class ObjectWithMeta:
     """
     Base class for objects with meta data.
 
     Meta-data properties are all stored in a dict and should be string:string
     mappings.
     """
 
     def __init__(self):
-        super(ObjectWithMeta, self).__init__()
+        super().__init__()
         self.meta = MetaDataContainer()
 
     def _clone_metadata(self, clone):
         """
         Clones this object's metadata into ``clone``.
         """
         for k, v in self.meta.items():
@@ -131,15 +118,15 @@
     def __init__(self, parent, name):
         """
         Creates a new ModelPart
 
         The given parent should be a ModelPart or None. The name should be
         unique within the set of children for the given parent.
         """
-        super(ModelPart, self).__init__()
+        super().__init__()
         self._parent = parent   # This object's parent
         self._model = None      # The model this object belongs to
         self._name = str(name)  # Local name
         self._uname = None      # Globally unique name
         self._token = None      # Parser token for errors, not always set
 
     def _clone_modelpart_data(self, clone):
@@ -149,24 +136,24 @@
         clone._uname = str(self._uname)
         self._clone_metadata(clone)
 
     def code(self):
         """
         Returns this object in ``mmt`` syntax.
         """
-        b = StringIO()
+        b = io.StringIO()
         self._code(b, 0)
         return b.getvalue()
 
     def _code(self, b, t):
         """
         Internal version of _code(), to be implemented by all subclasses.
 
         The argument ``t`` specifies the number of tabs to indent the code
-        with. The argument ``b`` is a cStringIO buffer.
+        with. The argument ``b`` is a StringIO buffer.
         """
         raise NotImplementedError
 
     def _delete(self):
         """
         Tells this object it's being deleted. Removes links to parent and/or
         model.
@@ -245,15 +232,15 @@
     def uname(self):
         """
         Returns a globally unique name for this object.
         """
         return self._uname
 
 
-class VarProvider(object):
+class VarProvider:
     """
     *Abstract class*
 
     This class provides an iterator over variables and equations for any object
     that can provide access to an iterator over its variables.
     """
 
@@ -459,15 +446,15 @@
     Minimal dictionary support is provided: A variable named "x" can be
     obtained from an owner ``m`` using ``m["x"]``. The number of variables in
     ``m`` is given by ``len(m)`` and the presence of "x" in ``m`` can be tested
     using ``if "x" in m:``.
     """
 
     def __init__(self, parent, name):
-        super(VarOwner, self).__init__(parent, name)
+        super().__init__(parent, name)
         self._variables = {}
         # Set component
         self._component = self
         while type(self._component) != Component:
             self._component = self._component.parent()
 
     def add_variable(self, name):
@@ -785,15 +772,15 @@
     For consistency with components, variables, and expressions, models cannot
     be compared with ``==`` (which will only return ``True`` if both operands
     are the same object). Checking if models are the same in other senses can
     be done with :meth:`is_similar`. Models can be serialized with ``pickle``.
     """
 
     def __init__(self, name=None):
-        super(Model, self).__init__()
+        super().__init__()
 
         # A dictionary of components
         self._components = {}
 
         # The model's state variables
         self._state_vars = []
 
@@ -1120,15 +1107,15 @@
 
     def code(self, line_numbers=False):
         """
         Returns this model in ``mmt`` syntax.
 
         Line numbers can be added by setting ``line_numbers=True``.
         """
-        b = StringIO()
+        b = io.StringIO()
         b.write('[[model]]\n')
         self._code(b, 0)
         if line_numbers:
             lines = b.getvalue().strip().split('\n')
             out = []
             n = int(math.ceil(math.log10(len(lines))))
             for k, line in enumerate(lines):
@@ -1745,23 +1732,23 @@
                 new_name.append(comp.name())
 
         new_name_error_str = (
             'new_name must be a list of strings the same length '
             'as external_component, or a string if only one '
             'component is provided'
         )
-        if isinstance(new_name, basestring):
+        if isinstance(new_name, str):
             if len(external_component) != 1:
                 raise TypeError(new_name_error_str)
             new_name = [new_name]
         else:
             try:
                 ok = (
                     len(new_name) == len(external_component) and
-                    all(isinstance(name, basestring) for name in new_name)
+                    all(isinstance(name, str) for name in new_name)
                 )
                 if not ok:
                     raise TypeError(new_name_error_str)
             except TypeError:
                 raise TypeError(new_name_error_str)
 
         # Get external model
@@ -1832,15 +1819,15 @@
                 # Check target vars in var map are variables and exist in self
                 if isinstance(self_var, myokit.Variable):
                     if not self_var.has_ancestor(self):
                         raise myokit.VariableMappingError(
                             'The variable <' + self_var.qname() + '> in the'
                             ' given var_map\'s values is not part of this'
                             ' model.')
-                elif isinstance(self_var, basestring):
+                elif isinstance(self_var, str):
                     try:
                         self_var = self.var(self_var)
                     except KeyError:
                         raise myokit.VariableMappingError(
                             'The variable name <' + self_var + '> appears in'
                             ' the var_map\'s values but was not found in this'
                             ' model.')
@@ -1854,15 +1841,15 @@
                 # in external model
                 if isinstance(ext_var, myokit.Variable):
                     if not ext_var.has_ancestor(ext_model):
                         raise myokit.VariableMappingError(
                             'The variable <' + ext_var.qname() + '> in the'
                             ' given var_map\'s keys but is not part of the'
                             ' source model.')
-                elif isinstance(ext_var, basestring):
+                elif isinstance(ext_var, str):
                     try:
                         ext_var = ext_model.var(ext_var)
                     except KeyError:
                         raise myokit.VariableMappingError(
                             'The variable name <' + ext_var + '> appears in'
                             ' the var_map\'s keys but was not found in the'
                             ' source model.')
@@ -2593,15 +2580,15 @@
            delimited list of floats.
          - A list of scalars. In this case, the list length will be
            checked and all values converted to float. No re-ordering takes
            place.
 
         """
         n = self.count_states()
-        if isinstance(state, basestring):
+        if isinstance(state, str):
             # String given. Parse into name:float map or list
             state = myokit.parse_state(state)
         if isinstance(state, dict):
             # Dictionary (sub)types. Parse into list of floats
             ini = [0] * n
             for k, v in enumerate(self.states()):
                 if v in state:
@@ -2908,15 +2895,15 @@
         Sets this model's initial values.
 
         The ``values`` must be specified as either a list of floats,
         expressions, and/or strings; or as a dict or string in a format
         accepted by :meth:`map_to_state`.
         """
         # Use map to state?
-        if isinstance(values, basestring) or isinstance(values, dict):
+        if isinstance(values, str) or isinstance(values, dict):
             self._state_init = [
                 myokit.Number(x) for x in self.map_to_state(values)]
         elif len(values) != len(self._state_vars):
             raise ValueError('Wrong number of initial values, expecting '
                              + str(len(self._state_vars)) + '.')
         else:
             # Parsing of arguments without making changes, in case it fails.
@@ -3651,15 +3638,15 @@
     the iterator methods.
 
     Meta-data properties can be accessed via the property ``meta``, for example
     ``model.meta['key']= 'value'``.
     """
 
     def __init__(self, model, name):
-        super(Component, self).__init__(model, name)
+        super().__init__(model, name)
         self._alias_map = {}    # Maps variable names to other variables names
 
     def _clone1(self, model, new_name=None):
         """
         Performs the first part of component cloning: Clones this component's
         variables into the :class:`Model` given as ``model``, but doesn't set
         any references (such as in aliases or expressions.)
@@ -3737,15 +3724,15 @@
                 + ' and '.join(['<' + c.qname() + '>' for c in reffers]))
 
         # No problems? Then delete all variables from component
         for var in self.variables():
             var._delete(recursive=True, ignore_siblings=True)
 
         # Delete links to parent
-        super(Component, self)._delete()
+        super()._delete()
 
     def alias(self, name):
         """
         Returns the :class:`Variable` referred to using the alias ``name``.
         """
         return self._alias_map[name]
 
@@ -3869,15 +3856,15 @@
     input is not available.
 
     Meta-data properties can be accessed via the property ``meta``, for example
     ``model.meta['key']= 'value'``.
     """
 
     def __init__(self, parent, name):
-        super(Variable, self).__init__(parent, name)
+        super().__init__(parent, name)
 
         # Index, only set if this is a state variable
         self._index = None
 
         # This variable's unit, if given, else dimensionless
         self._unit = None
 
@@ -4276,15 +4263,15 @@
             for kid in kids:
                 # Call this method for each kid (and cascade to their kids)
                 kid._delete(recursive=True, ignore_siblings=True)
                 # Remove kid from list of nested variables
                 self._remove_variable_internal(kid)
 
         # Remove parent links
-        super(Variable, self)._delete()
+        super()._delete()
 
     def demote(self):
         """
         Turns a state variable into an intermediary variable.
 
         This will reset the validation status of the model this variable
         belongs to.
@@ -4494,15 +4481,15 @@
             import warnings
             warnings.warn('The keyword argument `state_value` is deprecated.'
                           ' Please use `initial_value` instead.')
 
         # Handle string and number rhs's
         model = self.model()
         if not isinstance(initial_value, myokit.Expression):
-            if isinstance(initial_value, basestring):
+            if isinstance(initial_value, str):
                 # Expressions are evaluated in model context
                 initial_value = myokit.parse_expression(
                     initial_value, context=model)
             elif initial_value is not None:
                 initial_value = myokit.Number(initial_value)
 
         try:
@@ -4584,17 +4571,17 @@
             func.append(tab + w.eq(eq))
         func.append(tab + 'return ' + w.ex(eqs[-1].lhs))
         func = '\n'.join(func) + '\n'
 
         # Create function
         local = {}
         if use_numpy:
-            myokit._exec(func, {'numpy': numpy}, local)
+            exec(func, {'numpy': numpy}, local)
         else:
-            myokit._exec(func, {'math': math}, local)
+            exec(func, {'math': math}, local)
         handle = local['var_pyfunc_generated']
 
         # Return
         if arguments:
             return (handle, args)
         else:
             return handle
@@ -4762,15 +4749,15 @@
         self._set_initial_value(value, True)
 
     def _set_initial_value(self, value, make_the_change):
         """ Internal version of `set_initial_value`. """
         # Handle strings and floats
         model = self.model()
         if not isinstance(value, myokit.Expression):
-            if isinstance(value, basestring):
+            if isinstance(value, str):
                 value = myokit.parse_expression(value, context=model)
             else:
                 value = myokit.Number(value)
 
         # Allow internal calls to parse `value` without making a change
         if not make_the_change:
             return value
@@ -4830,15 +4817,15 @@
             x.set_rhs('1 + y')
 
         Calling `set_rhs` will reset the validation status of the model this
         variable belongs to.
         """
         # Handle string and number rhs's
         if not isinstance(rhs, myokit.Expression):
-            if isinstance(rhs, basestring):
+            if isinstance(rhs, str):
                 rhs = myokit.parse_expression(rhs, context=self)
             elif rhs is not None:
                 rhs = myokit.Number(rhs)
 
         # Update the refs-by stored in the old dependencies
         for ref in self._refs_to:
             ref._refs_by.remove(self)
@@ -4881,15 +4868,15 @@
     def set_unit(self, unit=None):
         """
         Changes this variable's unit. The unit can be set to any valid Unit
         object, or ``None`` to remove the unit.
         """
         if unit is None or isinstance(unit, myokit.Unit):
             self._unit = unit
-        elif isinstance(unit, basestring):
+        elif isinstance(unit, str):
             self._unit = myokit.parse_unit(unit)
         else:
             raise TypeError('Method set_unit() expects a myokit.Unit or None.')
         # No need to reset validation status or cache. Units are checked only
         # by the model.
 
     def state_value(self):
@@ -5064,15 +5051,15 @@
         """
         Will return the value of this variable's defining right-hand side
         expression.
         """
         return self._rhs.eval()
 
 
-class Equation(object):
+class Equation:
     """
     Defines an equation: a statement that a left-hand side (LHS) is equal to a
     right-hand side (RHS) expression.
 
     The sides of an equation are stored in the properties ``lhs`` and ``rhs``.
     Equations are immutable: once created, their LHS and RHS cannot be changed.
 
@@ -5099,15 +5086,15 @@
         return Equation(
             self._lhs.clone(subst, expand, retain),
             self._rhs.clone(subst, expand, retain),
         )
 
     def code(self):
         """ Returns an ``.mmt`` representation of this equation. """
-        b = StringIO()
+        b = io.StringIO()
         self._lhs._code(b, None)
         b.write(' = ')
         self._rhs._code(b, None)
         return b.getvalue()
 
     def __hash__(self):
         # Note: Hash should never change during object's lifetime. This is
@@ -5145,15 +5132,15 @@
         # Always sorted
         def stream(lst):
             for eq in lst:
                 yield eq.lhs.var()
         return stream(self)
 
 
-class UserFunction(object):
+class UserFunction:
     """
     Represents a user function.
 
     ``UserFunction`` objects should not be created directly, but only via
     :meth:`Model.add_function()`.
 
     User functions are not ``Expression`` objects, but template expressions
```

### Comparing `myokit-1.34.0/myokit/_myokit_version.py` & `myokit-1.35.0/myokit/_myokit_version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 #
 # Myokit's version info
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-import sys
 
 # True if this is a release, False for a development version
 __release__ = True
 
 # Version as a tuple (major, minor, revision)
 #  - Changes to major are rare
 #  - Changes to minor indicate new features, possible slight backwards
 #    incompatibility
 #  - Changes to revision indicate bugfixes, tiny new features
 #  - There is no significance to odd/even numbers
-__version_tuple__ = 1, 34, 0
+__version_tuple__ = 1, 35, 0
 
 # String version of the version number
 __version__ = '.'.join([str(x) for x in __version_tuple__])
 if not __release__:  # pragma: no cover
     __version_tuple__ += ('dev', )
     __version__ += '.dev'
 
-# Don't expose x on Python2
-if sys.hexversion < 0x03000000:  # pragma: no python 3 cover
-    del x
```

### Comparing `myokit-1.34.0/myokit/_parsing.py` & `myokit-1.35.0/myokit/_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 #
 # Parser for .mmt files
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import re
-#import unicodedata
+
 from collections import OrderedDict
 
 import myokit
-from myokit import ParseError, ProtocolParseError
 
-# Strings in Python2 and Python3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
+from myokit import ParseError, ProtocolParseError
 
 
 def parse(source):
     """
     Parses strings in ``mmt`` format and returns a tuple ``(model,
     protocol, embedded script)``.
 
     ``None`` may be returned for any segment not appearing in the source.
 
     The source to parse can be given as a plain string, a sequence of lines
     or a stream of lines.
     """
     # Get raw stream
     raw = source
-    if isinstance(raw, basestring):
+    if isinstance(raw, str):
         raw = raw.splitlines()
     raw = iter(raw)
 
     # Create tokenizer
     stream = Tokenizer(raw)
 
     # Start parsing
@@ -74,15 +66,15 @@
 
 def parse_model(source):
     """
     Parses a model in ``mmt`` format.
     """
     # Get raw stream
     raw = source
-    if isinstance(raw, basestring):
+    if isinstance(raw, str):
         raw = raw.splitlines()
     raw = iter(raw)
 
     # Parse and return
     stream = Tokenizer(raw)
     token = expect(stream.peek(), SEGMENT_HEADER)
     if token[1] != '[[model]]':
@@ -96,15 +88,15 @@
 
 def parse_protocol(source):
     """
     Parses a protocol in ``mmt`` format.
     """
     # Get raw stream
     raw = source
-    if isinstance(raw, basestring):
+    if isinstance(raw, str):
         raw = raw.splitlines()
     raw = iter(raw)
 
     # Parse and return
     stream = Tokenizer(raw)
     token = expect(stream.peek(), SEGMENT_HEADER)
     if token[1] != '[[protocol]]':
@@ -118,15 +110,15 @@
 
 def parse_script(source):
     """
     Parses a script in ``mmt`` format.
     """
     # Get raw stream
     raw = source
-    if isinstance(raw, basestring):
+    if isinstance(raw, str):
         raw = raw.splitlines()
     raw = iter(raw)
 
     # Parse and return
     stream = Tokenizer(raw)
     token = expect(stream.peek(), SEGMENT_HEADER)
     if token[1] != '[[script]]':
@@ -158,15 +150,15 @@
         ...
 
     Parsed data from this input format is returned as a list of floating point
     numbers.
     """
     # Get raw stream
     raw = state
-    if isinstance(raw, basestring):
+    if isinstance(raw, str):
         raw = raw.splitlines()
     raw = iter(raw)
 
     # Create tokenizer
     stream = Tokenizer(raw, check_indenting=False)
 
     # Start parsing
@@ -201,15 +193,15 @@
 def split(source):
     """
     Attempts to split the ``source`` into model, protocol and script segments.
     Any content before the [[model]] tag is discarded.
     """
     # Get raw stream
     raw = source
-    if isinstance(raw, basestring):
+    if isinstance(raw, str):
         raw = raw.splitlines()
     raw = iter(raw)
     segments = ['', '', '']
     prot_or_script = ('[[protocol]]', '[[script]]')
 
     # Gather lines in stream
     lines = [line for line in raw]
@@ -313,15 +305,15 @@
     hide = [EOL, EOF, INDENT, DEDENT, AND, OR, NOT]
     if code not in hide:
         got += ' "' + text + '"'
 
     # Parse expected token(s) or string
     if type(expected) == int:
         expected = [expected]
-    if not isinstance(expected, basestring):
+    if not isinstance(expected, str):
         if len(expected) > 2:
             expected = 'one of [' \
                 + ', '.join([token_str[i] for i in expected]) + ']'
         elif len(expected) == 2:
             expected = token_str[expected[0]] + ' or ' + token_str[expected[1]]
         else:
             expected = token_str[expected[0]]
@@ -344,15 +336,15 @@
         if token[2] not in info.model._tokens:
             d = info.model._tokens[token[2]] = {}
         else:
             d = info.model._tokens[token[2]]
         d[token[3]] = (token, obj)
 
 
-class ParseInfo(object):
+class ParseInfo:
     def __init__(self):
         self.model = None
         self.initial_values = OrderedDict()
         self.initial_value_tokens = {}
         self.alias_map = {}
         self.user_functions = {}
 
@@ -1067,15 +1059,15 @@
 
     By default, constants defined for variables whose RHS is a single number
     will keep their units. To disable this, set ``skip_literals=False``.
 
     This method will raise a :class:`myokit.ParseError` if the given code
     cannot be parsed to a valid model.
     """
-    if isinstance(model_text, basestring):
+    if isinstance(model_text, str):
         lines = model_text.splitlines()
     else:
         lines = model_text
     stream = Tokenizer(lines)
     m = parse_model_from_stream(stream)
     # Collect positions of fake unit tokens
     cuts = []
@@ -1263,15 +1255,15 @@
     PLUS, MINUS, STAR, SLASH, POWER, REMAINDER]
 
 # Map of equals-comparators (==, !=, >=, <=)
 _COMPEQ = '=!><'
 _COMPEQ_MAP = [EQEQUAL, NOTEQUAL, MOREEQUAL, LESSEQUAL]
 
 
-class Tokenizer(object):
+class Tokenizer:
     """
     Takes a stream of lines as input and provides a stream interface returning
     tokens.
 
     Strips comments and concatenates lines with open parentheses (anything
     between round brackets is counted as a single line). Blank lines (or lines
     with nothing but comments) are ignored. Leading whitespace is converted
@@ -1308,15 +1300,15 @@
         self._has_last_value = False
 
         # Catchers and catcher handle index
         self._catchers = {}
         self._catcheri = 0
 
         # String given instead of stream of lines? Convert
-        if isinstance(stream_of_lines, basestring):
+        if isinstance(stream_of_lines, str):
             stream_of_lines = iter(stream_of_lines.splitlines())
 
         # Create tokenizer
         self._tokenizer = self._tizer(stream_of_lines, check_indenting)
 
         # Grab first token
         self._advance()
@@ -1961,15 +1953,15 @@
     out = [ex.name]
     if ex.desc is not None:
         out.append('  ' + ex.desc)
     out.append('On line ' + str(ex.line) + ' character ' + str(ex.char))
     line = None
 
     if ex.line > 0 and source is not None:
-        if isinstance(source, basestring) and os.path.isfile(source):
+        if isinstance(source, str) and os.path.isfile(source):
             # Re-open file, find line
             with open(source, 'r') as f:
                 for i in range(0, ex.line):
                     line = next(f)
             line = line.rstrip()
         else:
             i = 0
@@ -2011,15 +2003,15 @@
 
         # Add error indication
         out.append(' ' * (2 + char) + '^')
 
     return '\n'.join(out)
 
 
-class NudParser(object):
+class NudParser:
     """
     Expression parser for nud operators.
 
     An expression parser to use when parsing a token as the first element
     of an expression. The term nud stands for 'null denotation' as it has no
     previous expression bound to it.
     """
@@ -2080,15 +2072,15 @@
 
 
 class FunctionParser(NudParser):
     """
     Parser for function calls.
     """
     def __init__(self):
-        super(FunctionParser, self).__init__()
+        super().__init__()
         self._rbp = myokit.Function._rbp
 
     def parse(self, stream, info):
         name = next(stream)
         ops = []
         token = next(stream)
         while token[0] != PAREN_CLOSE:
@@ -2121,15 +2113,15 @@
                 + ' argument(s) could not be found.')
 
         # Found function, return template, arguments and tokens. "func" is
         # now a (template) Expression object.
         return (func, ops, (name,))
 
 
-class LedParser(object):
+class LedParser:
     """
     Expression parser for led operators.
 
     An expression parser to use when parsing a token with an existing
     expression. The term led stands for 'left denotation' as it is bound to
     an existing expression on its left.
```

### Comparing `myokit-1.34.0/myokit/_progress.py` & `myokit-1.35.0/myokit/_progress.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 #
 # Contains classes for progress reporting during long operations.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import timeit
 
 import myokit
 
 
-class ProgressReporter(object):
+class ProgressReporter:
     """
     Interface for progress updates in Simulations. Also allows some job types
     to be cancelled by the user.
 
     Many simulation types take an argument ``progress`` that can be used to
     pass in an object implementing this interface. The simulation will use this
     object to report on its progress.
@@ -58,15 +55,15 @@
         ``progress``, which will have a value in the range ``[0, 1]``.
 
         The return value of this update can be used to signal a job should be
         cancelled: Return ``True`` to keep going, ``False`` to cancel.
         """
         pass
 
-    class _Job(object):
+    class _Job:
         def __init__(self, parent, msg):
             self._parent = parent
             self._msg = msg
 
         def __enter__(self):
             self._parent.enter(self._msg)
 
@@ -93,15 +90,15 @@
 
     Output is only written if the new percentage done differs from the old one,
     in a string format specified by the number of ``digits`` to display. The
     ``digits`` parameter accepts the special value ``-1`` to only print out a
     status every ten percent.
     """
     def __init__(self, digits=1):
-        super(ProgressPrinter, self).__init__()
+        super().__init__()
         self._b = myokit.tools.Benchmarker()
         self._f = None
         self._d = int(digits)
 
     def enter(self, msg=None):
         # Reset
         self._b.reset()
@@ -134,15 +131,15 @@
 
 
 class Timeout(ProgressReporter):
     """
     Progress reporter that cancels a simulation after ``timeout`` seconds.
     """
     def __init__(self, timeout):
-        super(Timeout, self).__init__()
+        super().__init__()
         self._timeout = float(timeout)
 
     def enter(self, msg=None):
         self._max_time = timeit.default_timer() + self._timeout
 
     def update(self, progress):
         return timeit.default_timer() < self._max_time
```

### Comparing `myokit-1.34.0/myokit/_protocol.py` & `myokit-1.35.0/myokit/_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 #
 # Defines the python classes that represent pacing protocols.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
 
 import numpy as np
 
 from bisect import bisect_right
 
 
-class Protocol(object):
+class Protocol:
     """
     Represents a pacing protocol as a sequence of :class:`events
     <ProtocolEvent>`.
 
     Every event represents a time span during which the stimulus is non-zero.
     All events specify a stimulus level, a starting time and a duration. The
     stimulus level is given as a dimensionless number where 0 is no stimulus
@@ -45,15 +42,15 @@
     is not.
 
     Protocols can be compared with ``==``, which will check if the :meth:`code`
     for both protocols is the same. Protocols can be serialized with
     ``pickle``.
     """
     def __init__(self):
-        super(Protocol, self).__init__()
+        super().__init__()
         self._head = None
 
     def add(self, e):
         """
         (Re-)schedules an :class:`event <ProtocolEvent>`.
         """
         # No head? Then set as head
@@ -532,15 +529,15 @@
             raise ValueError('Times cannot be negative.')
 
         # Create a pacing system, calculate the values, and return
         p = PacingSystem(self)
         return [p.advance(t) for t in times]
 
 
-class ProtocolEvent(object):
+class ProtocolEvent:
     """
     Describes an event occurring as part of a protocol.
     """
     def __init__(self, level, start, duration, period=0, multiplier=0):
         """
         Creates a new event
 
@@ -715,15 +712,15 @@
         """
         return self._start + self._duration
 
     def __str__(self):
         return self.in_words()
 
 
-class PacingSystem(object):
+class PacingSystem:
     """
     This class uses a :class:`myokit.Protocol` to update the value of a
     pacing variable over time.
 
     A pacing system is created by passing in a protocol:
 
         import myokit
@@ -849,15 +846,15 @@
 
 
 class NotAnUnbrokenSequenceError(myokit.MyokitError):
     """ Error raised exclusively by is_unbroken_sequence_exception(). """
     pass
 
 
-class TimeSeriesProtocol(object):
+class TimeSeriesProtocol:
     """
     Represents a pacing protocol as a sequence of time value pairs and an
     interpolation method (currently only linear interpolation is supported).
 
     A 1D time-series should be given as input. During the simulation, the value
     of the pacing variable will be determined by interpolating between the two
     nearest points in the series. If the simulation time is outside the bounds
@@ -866,15 +863,15 @@
     Protocols can be compared with ``==``, which will check if the sequence of
     time value pairs is the same, and the interpolation method is the same.
     Protocols can be serialized with ``pickle``.
 
     """
 
     def __init__(self, times, values, method=None):
-        super(TimeSeriesProtocol, self).__init__()
+        super().__init__()
 
         if len(times) != len(values):
             raise ValueError('Times and values array must have same size.')
         times_tpl, values_tpl = zip(*[
             (float(t), float(v)) for t, v in sorted(zip(times, values))
         ])
         self._times = list(times_tpl)
```

### Comparing `myokit-1.34.0/myokit/_sim/__init__.py` & `myokit-1.35.0/myokit/_sim/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 #
 # This hidden module contains the core functions dealing with simulations and
 # the data they generate.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-# Library imports
 import os
 import platform
 import sys
 import tempfile
 import threading
 import timeit
 import traceback
@@ -32,44 +28,31 @@
             ).stdout
         else:
             return subprocess.Popen(
                 command, shell=True, bufsize=bufsize, stdin=subprocess.PIPE
             ).stdin
     os.popen = _ospop
 
-
-# Setuptools imports
 from setuptools import setup, Extension  # noqa
 
-
-# Myokit imports
 import myokit       # noqa
 import myokit.pype  # noqa
 
 
-# Dynamic module finding and loading in Python 3.5+ and younger
-if sys.hexversion >= 0x03050000:
-    import importlib.machinery
+def load_module(name, path):
+    """ Dynamically find and load a module (Python 3.5+). """
     import importlib
+    import importlib.machinery
 
-    def load_module(name, path):
-        spec = importlib.machinery.PathFinder.find_spec(name, [path])
-        module = importlib.util.module_from_spec(spec)
-        return module
-
-else:  # pragma: no python 3 cover
-    import imp
-
-    def load_module(name, path):
-        (f, pathname, description) = imp.find_module(name, [path])
-        f.close()
-        return imp.load_dynamic(name, pathname)
+    spec = importlib.machinery.PathFinder.find_spec(name, [path])
+    module = importlib.util.module_from_spec(spec)
+    return module
 
 
-class CModule(object):
+class CModule:
     """
     Abstract base class for classes that dynamically create and compile a
     back-end C-module.
     """
     def __init__(self):
         self._debug_file_count = 0
```

### Comparing `myokit-1.34.0/myokit/_sim/cable.c` & `myokit-1.35.0/myokit/_sim/cable.c`

 * *Files 1% similar despite different names*

```diff
@@ -363,17 +363,15 @@
     if (PyList_Size(state_out) != ncells * N_STATE) {
         PyErr_SetString(PyExc_Exception, "'state_out' must have size ncells * n_states.");
         return sim_clean();
     }
     for(i_state=0; i_state<ncells * N_STATE; i_state++) {
         flt = PyList_GetItem(state_in, i_state);    /* Borrowed reference */
         if (!PyFloat_Check(flt)) {
-            char errstr[200];
-            sprintf(errstr, "Item %d in state vector is not a float.", i_state);
-            PyErr_SetString(PyExc_Exception, errstr);
+            PyErr_Format(PyExc_Exception, "Item %d in state vector is not a float.", i_state);
             return sim_clean();
         }
     }
 
     /* Set minimum step size */
     dt_min = 1e-2 * default_dt;
```

### Comparing `myokit-1.34.0/myokit/_sim/cable.py` & `myokit-1.35.0/myokit/_sim/cable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #
 # Cable simulation using a simple forward Euler implementation
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
-import myokit
 import platform
 
+import myokit
+
 # Location of source file
 SOURCE_FILE = 'cable.c'
 
 
 class Simulation1d(myokit.CModule):
     """
     Can run 1d cable simulations based on a :class:`model <Model>`.
@@ -97,15 +95,15 @@
     [3] Cellular cardiac electrophysiology modelling with Chaste and CellML
     Cooper, Spiteri, Mirams (2015) Frontiers in Physiology
 
     """
     _index = 0      # Unique id for generated module
 
     def __init__(self, model, protocol=None, ncells=50, rl=False):
-        super(Simulation1d, self).__init__()
+        super().__init__()
 
         # Require a valid model
         model.validate()
 
         # Set protocol
         self.set_protocol(protocol)
```

### Comparing `myokit-1.34.0/myokit/_sim/cmodel.h` & `myokit-1.35.0/myokit/_sim/cmodel.h`

 * *Files 0% similar despite different names*

```diff
@@ -914,17 +914,15 @@
     return Model_OK;
 }
 
 /*
  * Private method: Add a variable to the logging lists. Returns 1 if
  * successful.
  *
- * Note: The variable names are all ascii compatible. In Python2, the strings
- * inside log_dict are either unicode or bytes, but they can be matched
- * without conversion.
+ * Note: The variable names are all ascii compatible.
  *
  * Arguments
  *  log_dict : A dictionary mapping variable names to sequences.
  *  i : The next index to add logs and vars.
  *  name : The name to check.
  *  var : A pointer to the variable.
  *
```

### Comparing `myokit-1.34.0/myokit/_sim/cmodel.py` & `myokit-1.35.0/myokit/_sim/cmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 #
 # Myokit symbolic expression classes. Defines different expressions, equations
 # and the unit system.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import traceback
 
 from collections import OrderedDict
 
 import myokit
 import myokit.formats.ansic
 import myokit.pype
 
 # Location of source file
 SOURCE_FILE = 'cmodel.h'
 
 
-class CModel(object):
+class CModel:
     """
     Generates ansi-C code for a model.
 
     Example::
 
         model = myokit.parse_model('example')
         cmodel = CModel(model)
```

### Comparing `myokit-1.34.0/myokit/_sim/compiler.c` & `myokit-1.35.0/myokit/_sim/compiler.c`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_sim/compiler.py` & `myokit-1.35.0/myokit/_sim/compiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # C Compiler information class
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 
 import myokit
 
 # Path to C Source for Compiler info module
 SOURCE_FILE = 'compiler.c'
 
@@ -28,15 +25,15 @@
     # Cached compilation error messages
     _message = None
 
     # Guess at compiler
     _compiler = None
 
     def __init__(self):
-        super(Compiler, self).__init__()
+        super().__init__()
         # Create and cache back-end
         Compiler._index += 1
 
         # Define libraries
         libd = list()
         incd = list()
         incd.append(myokit.DIR_CFUNC)
```

### Comparing `myokit-1.34.0/myokit/_sim/cvodessim.c` & `myokit-1.35.0/myokit/_sim/cvodessim.c`

 * *Files 0% similar despite different names*

```diff
@@ -169,19 +169,16 @@
  * Warnings are passed to Python's warning system, where they can be
  * caught or suppressed using the warnings module.
  */
 void
 ErrorHandler(int error_code, const char *module, const char *function,
              char *msg, void *eh_data)
 {
-    char errstr[1024];
     if (error_code > 0) {
-        sprintf(errstr, "CVODES: %s", msg);
-        PyErr_WarnEx(PyExc_RuntimeWarning, errstr, 1);
-        /* Python 3.2+: PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "CVODES: %s", msg); */
+        PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "CVODES: %s", msg);
     }
 }
 
 /*
  * Initialisation status.
  * Proper sequence is init(), repeated step() calls till finished, then clean.
  */
```

### Comparing `myokit-1.34.0/myokit/_sim/cvodessim.py` & `myokit-1.35.0/myokit/_sim/cvodessim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #
 # CVODES-driven single cell simulation with optional sensitivities and root
 # finding
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import platform
 import tempfile
 
 from collections import OrderedDict
 
 import myokit
@@ -148,15 +145,15 @@
     solvers. Hindmarsh, Brown, Woodward, et al. (2005) ACM Transactions on
     Mathematical Software.
 
     """
     _index = 0  # Simulation id
 
     def __init__(self, model, protocol=None, sensitivities=None, path=None):
-        super(Simulation, self).__init__()
+        super().__init__()
 
         # Require a valid model
         if not model.is_valid():
             model.validate()
         self._model = model.clone()
         del model
```

### Comparing `myokit-1.34.0/myokit/_sim/differential.hpp` & `myokit-1.35.0/myokit/_sim/differential.hpp`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_sim/fiber_tissue.c` & `myokit-1.35.0/myokit/_sim/fiber_tissue.c`

 * *Files 1% similar despite different names*

```diff
@@ -538,33 +538,29 @@
 
     // Create state vectors, set initial values
     dsize_state_f = nfx * nfy * n_state_f * sizeof(Real);
     rvec_state_f = (Real*)malloc(dsize_state_f);
     for(i=0; i < nfx * nfy * n_state_f; i++) {
         flt = PyList_GetItem(state_in_f, i);    // Don't decref!
         if(!PyFloat_Check(flt)) {
-            char errstr[200];
-            sprintf(errstr, "Item %u in fiber state vector is not a float.", (unsigned int)i);
-            PyErr_SetString(PyExc_Exception, errstr);
+            PyErr_Format(PyExc_Exception, "Item %u in fiber state vector is not a float.", (unsigned int)i);
             return sim_clean();
         }
         rvec_state_f[i] = (Real)PyFloat_AsDouble(flt);
     }
     #ifdef MYOKIT_DEBUG_MESSAGES
     printf("Created fiber state vector, set initial values.\n");
     #endif
 
     dsize_state_t = ntx * nty * n_state_t * sizeof(Real);
     rvec_state_t = (Real*)malloc(dsize_state_t);
     for(i=0; i < ntx * nty * n_state_t; i++) {
         flt = PyList_GetItem(state_in_t, i);
         if(!PyFloat_Check(flt)) {
-            char errstr[200];
-            sprintf(errstr, "Item %u in tissue state vector is not a float.", (unsigned int)i);
-            PyErr_SetString(PyExc_Exception, errstr);
+            PyErr_Format(PyExc_Exception, "Item %u in tissue state vector is not a float.", (unsigned int)i);
             return sim_clean();
         }
         rvec_state_t[i] = (Real)PyFloat_AsDouble(flt);
     }
     #ifdef MYOKIT_DEBUG_MESSAGES
     printf("Created tissue state vector, set initial values.\n");
     #endif
```

### Comparing `myokit-1.34.0/myokit/_sim/fiber_tissue.py` & `myokit-1.35.0/myokit/_sim/fiber_tissue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #
 # OpenCL driven fiber-tissue simulation.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
-import myokit
 import platform
 
+import myokit
+
 # Location of C and OpenCL sources
 SOURCE_FILE = 'fiber_tissue.c'
 KERNEL_FILE = 'openclsim.cl'
 
 
 class FiberTissueSimulation(myokit.CModule):
     """
@@ -118,15 +116,15 @@
     _index = 0  # Unique id for the created simulation module
 
     def __init__(
             self, fiber_model, tissue_model, protocol=None,
             ncells_fiber=(128, 2), ncells_tissue=(128, 128), nx_paced=5,
             g_fiber=(9, 6), g_tissue=(9, 6), g_fiber_tissue=9,
             dt=0.005, precision=myokit.SINGLE_PRECISION, native_maths=False):
-        super(FiberTissueSimulation, self).__init__()
+        super().__init__()
 
         # Deprecated since 2021-05-28
         # Un-deprecated on 2022-04-20, following Adam's request
         #import warnings
         #warnings.warn(
         #    'The class `myokit.FiberTissueSimulation` is deprecated, and will'
         #    ' be removed in future versions of Myokit.')
```

### Comparing `myokit-1.34.0/myokit/_sim/jacobian.cpp` & `myokit-1.35.0/myokit/_sim/jacobian.cpp`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_sim/jacobian.py` & `myokit-1.35.0/myokit/_sim/jacobian.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #
 # Two Jacobian calculating tools sharing the same C++ source code.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
-import myokit
-import numpy as np
 import platform
 
+import numpy as np
+
+import myokit
+
 # Location of C source file
 SOURCE_FILE = 'jacobian.cpp'
 
 
 class JacobianTracer(myokit.CppModule):
     """
     Given a model and a simulation log, this class can revisit every logged
@@ -41,15 +40,15 @@
     However, in many cases, these functions will only occur as part of a
     condition in an if statement, so the ``NaN``'s won't propagate to the final
     result.
     """
     _index = 0  # Unique id
 
     def __init__(self, model):
-        super(JacobianTracer, self).__init__()
+        super().__init__()
 
         # Require a valid model
         model.validate()
 
         # Clone model
         self._model = model.clone()
 
@@ -212,15 +211,15 @@
     However, in many cases, these functions will only occur as part of a
     condition in an if statement, so the ``NaN``'s won't propagate to the final
     result.
     """
     _index = 0  # Unique id
 
     def __init__(self, model):
-        super(JacobianCalculator, self).__init__()
+        super().__init__()
         # Require a valid model
         model.validate()
 
         # Clone model
         self._model = model.clone()
 
         # Store the initial values (won't be able to access once time binding
```

### Comparing `myokit-1.34.0/myokit/_sim/mcl.h` & `myokit-1.35.0/myokit/_sim/mcl.h`

 * *Files 18% similar despite different names*

```diff
@@ -63,187 +63,185 @@
  *
  * An extra note about the error can be passed in as msg.
  */
 static int
 mcl_flag2(const char* msg, const cl_int flag)
 {
     char sub[1024];
-    char err[2048];
 
     if(flag == CL_SUCCESS) {
         return 0;
     }
 
     if(strcmp(msg, "")) {
         sprintf(sub, " (%s)", msg);
     } else {
         sub[0] = 0;
     }
 
     switch(flag) {
         // OpenCL 1.0 Errors
         case CL_DEVICE_NOT_FOUND:
-            sprintf(err, "OpenCL error%s: CL_DEVICE_NOT_FOUND", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_DEVICE_NOT_FOUND", sub);
             break;
         case CL_DEVICE_NOT_AVAILABLE:
-            sprintf(err, "OpenCL error%s: CL_DEVICE_NOT_AVAILABLE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_DEVICE_NOT_AVAILABLE", sub);
             break;
         case CL_COMPILER_NOT_AVAILABLE:
-            sprintf(err, "OpenCL error%s: CL_COMPILER_NOT_AVAILABLE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_COMPILER_NOT_AVAILABLE", sub);
             break;
         case CL_MEM_OBJECT_ALLOCATION_FAILURE:
-            sprintf(err, "OpenCL error%s: CL_MEM_OBJECT_ALLOCATION_FAILURE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_MEM_OBJECT_ALLOCATION_FAILURE", sub);
             break;
         case CL_OUT_OF_RESOURCES:
-            sprintf(err, "OpenCL error%s: CL_OUT_OF_RESOURCES", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_OUT_OF_RESOURCES", sub);
             break;
         case CL_OUT_OF_HOST_MEMORY:
-            sprintf(err, "OpenCL error%s: CL_OUT_OF_HOST_MEMORY", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_OUT_OF_HOST_MEMORY", sub);
             break;
         case CL_PROFILING_INFO_NOT_AVAILABLE:
-            sprintf(err, "OpenCL error%s: CL_PROFILING_INFO_NOT_AVAILABLE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_PROFILING_INFO_NOT_AVAILABLE", sub);
             break;
         case CL_MEM_COPY_OVERLAP:
-            sprintf(err, "OpenCL error%s: CL_MEM_COPY_OVERLAP", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_MEM_COPY_OVERLAP", sub);
             break;
         case CL_IMAGE_FORMAT_MISMATCH:
-            sprintf(err, "OpenCL error%s: CL_IMAGE_FORMAT_MISMATCH", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_IMAGE_FORMAT_MISMATCH", sub);
             break;
         case CL_IMAGE_FORMAT_NOT_SUPPORTED:
-            sprintf(err, "OpenCL error%s: CL_IMAGE_FORMAT_NOT_SUPPORTED", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_IMAGE_FORMAT_NOT_SUPPORTED", sub);
             break;
         case CL_BUILD_PROGRAM_FAILURE:
-            sprintf(err, "OpenCL error%s: CL_BUILD_PROGRAM_FAILURE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_BUILD_PROGRAM_FAILURE", sub);
             break;
         case CL_MAP_FAILURE:
-            sprintf(err, "OpenCL error%s: CL_MAP_FAILURE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_MAP_FAILURE", sub);
             break;
         case CL_MISALIGNED_SUB_BUFFER_OFFSET:
-            sprintf(err, "OpenCL error%s: CL_MISALIGNED_SUB_BUFFER_OFFSET", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_MISALIGNED_SUB_BUFFER_OFFSET", sub);
             break;
         case CL_EXEC_STATUS_ERROR_FOR_EVENTS_IN_WAIT_LIST:
-            sprintf(err, "OpenCL error%s: CL_EXEC_STATUS_ERROR_FOR_EVENTS_IN_WAIT_LIST", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_EXEC_STATUS_ERROR_FOR_EVENTS_IN_WAIT_LIST", sub);
             break;
         case CL_INVALID_VALUE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_VALUE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_VALUE", sub);
             break;
         case CL_INVALID_DEVICE_TYPE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_DEVICE_TYPE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_DEVICE_TYPE", sub);
             break;
         case CL_INVALID_PLATFORM:
-            sprintf(err, "OpenCL error%s: CL_INVALID_PLATFORM", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_PLATFORM", sub);
             break;
         case CL_INVALID_DEVICE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_DEVICE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_DEVICE", sub);
             break;
         case CL_INVALID_CONTEXT:
-            sprintf(err, "OpenCL error%s: CL_INVALID_CONTEXT", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_CONTEXT", sub);
             break;
         case CL_INVALID_QUEUE_PROPERTIES:
-            sprintf(err, "OpenCL error%s: CL_INVALID_QUEUE_PROPERTIES", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_QUEUE_PROPERTIES", sub);
             break;
         case CL_INVALID_COMMAND_QUEUE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_COMMAND_QUEUE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_COMMAND_QUEUE", sub);
             break;
         case CL_INVALID_HOST_PTR:
-            sprintf(err, "OpenCL error%s: CL_INVALID_HOST_PTR", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_HOST_PTR", sub);
             break;
         case CL_INVALID_MEM_OBJECT:
-            sprintf(err, "OpenCL error%s: CL_INVALID_MEM_OBJECT", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_MEM_OBJECT", sub);
             break;
         case CL_INVALID_IMAGE_FORMAT_DESCRIPTOR:
-            sprintf(err, "OpenCL error%s: CL_INVALID_IMAGE_FORMAT_DESCRIPTOR", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_IMAGE_FORMAT_DESCRIPTOR", sub);
             break;
         case CL_INVALID_IMAGE_SIZE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_IMAGE_SIZE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_IMAGE_SIZE", sub);
             break;
         case CL_INVALID_SAMPLER:
-            sprintf(err, "OpenCL error%s: CL_INVALID_SAMPLER", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_SAMPLER", sub);
             break;
         case CL_INVALID_BINARY:
-            sprintf(err, "OpenCL error%s: CL_INVALID_BINARY", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_BINARY", sub);
             break;
         case CL_INVALID_BUILD_OPTIONS:
-            sprintf(err, "OpenCL error%s: CL_INVALID_BUILD_OPTIONS", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_BUILD_OPTIONS", sub);
             break;
         case CL_INVALID_PROGRAM:
-            sprintf(err, "OpenCL error%s: CL_INVALID_PROGRAM", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_PROGRAM", sub);
             break;
         case CL_INVALID_PROGRAM_EXECUTABLE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_PROGRAM_EXECUTABLE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_PROGRAM_EXECUTABLE", sub);
             break;
         case CL_INVALID_KERNEL_NAME:
-            sprintf(err, "OpenCL error%s: CL_INVALID_KERNEL_NAME", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_KERNEL_NAME", sub);
             break;
         case CL_INVALID_KERNEL_DEFINITION:
-            sprintf(err, "OpenCL error%s: CL_INVALID_KERNEL_DEFINITION", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_KERNEL_DEFINITION", sub);
             break;
         case CL_INVALID_KERNEL:
-            sprintf(err, "OpenCL error%s: CL_INVALID_KERNEL", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_KERNEL", sub);
             break;
         case CL_INVALID_ARG_INDEX:
-            sprintf(err, "OpenCL error%s: CL_INVALID_ARG_INDEX", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_ARG_INDEX", sub);
             break;
         case CL_INVALID_ARG_VALUE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_ARG_VALUE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_ARG_VALUE", sub);
             break;
         case CL_INVALID_ARG_SIZE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_ARG_SIZE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_ARG_SIZE", sub);
             break;
         case CL_INVALID_KERNEL_ARGS:
-            sprintf(err, "OpenCL error%s: CL_INVALID_KERNEL_ARGS", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_KERNEL_ARGS", sub);
             break;
         case CL_INVALID_WORK_DIMENSION:
-            sprintf(err, "OpenCL error%s: CL_INVALID_WORK_DIMENSION", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_WORK_DIMENSION", sub);
             break;
         case CL_INVALID_WORK_GROUP_SIZE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_WORK_GROUP_SIZE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_WORK_GROUP_SIZE", sub);
             break;
         case CL_INVALID_WORK_ITEM_SIZE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_WORK_ITEM_SIZE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_WORK_ITEM_SIZE", sub);
             break;
         case CL_INVALID_GLOBAL_OFFSET:
-            sprintf(err, "OpenCL error%s: CL_INVALID_GLOBAL_OFFSET", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_GLOBAL_OFFSET", sub);
             break;
         case CL_INVALID_EVENT_WAIT_LIST:
-            sprintf(err, "OpenCL error%s: CL_INVALID_EVENT_WAIT_LIST", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_EVENT_WAIT_LIST", sub);
             break;
         case CL_INVALID_EVENT:
-            sprintf(err, "OpenCL error%s: CL_INVALID_EVENT", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_EVENT", sub);
             break;
         case CL_INVALID_OPERATION:
-            sprintf(err, "OpenCL error%s: CL_INVALID_OPERATION", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_OPERATION", sub);
             break;
         case CL_INVALID_GL_OBJECT:
-            sprintf(err, "OpenCL error%s: CL_INVALID_GL_OBJECT", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_GL_OBJECT", sub);
             break;
         case CL_INVALID_BUFFER_SIZE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_BUFFER_SIZE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_BUFFER_SIZE", sub);
             break;
         case CL_INVALID_MIP_LEVEL:
-            sprintf(err, "OpenCL error%s: CL_INVALID_MIP_LEVEL", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_MIP_LEVEL", sub);
             break;
         case CL_INVALID_GLOBAL_WORK_SIZE:
-            sprintf(err, "OpenCL error%s: CL_INVALID_GLOBAL_WORK_SIZE", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_GLOBAL_WORK_SIZE", sub);
             break;
         case CL_INVALID_PROPERTY:
-            sprintf(err, "OpenCL error%s: CL_INVALID_PROPERTY", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_INVALID_PROPERTY", sub);
             break;
         // OpenCL 1.1 etc. codes can not be assumed to be defined
         // Might be good to have ifdefs or something
         // OpenCL extensions
         case -1001:     // CL_PLATFORM_NOT_FOUND_KHR
-            sprintf(err, "OpenCL error%s: CL_PLATFORM_NOT_FOUND_KHR", sub);
+            PyErr_Format(PyExc_Exception, "OpenCL error%s: CL_PLATFORM_NOT_FOUND_KHR", sub);
             break;
         // Unknown error
         default:
-            sprintf(err, "Unknown OpenCL error%s: %i", sub, (int)flag);
+            PyErr_Format(PyExc_Exception, "Unknown OpenCL error%s: %i", sub, (int)flag);
             break;
     };
-    PyErr_SetString(PyExc_Exception, err);
     return 1;
 }
 
 /*
  * Checks the given flag for an opencl error, returns 1 if found and sets the
  * error message, else, returns 0.
  */
```

### Comparing `myokit-1.34.0/myokit/_sim/opencl.c` & `myokit-1.35.0/myokit/_sim/opencl.c`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_sim/opencl.py` & `myokit-1.35.0/myokit/_sim/opencl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 #
 # OpenCL information class
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
+import configparser
 import os
-import myokit
-
-try:
-    # Python2
-    from ConfigParser import ConfigParser
-except ImportError:
-    # Python 3
-    from configparser import RawConfigParser as ConfigParser
 
+import myokit
 
 # Settings file
 SETTINGS_FILE = os.path.join(myokit.DIR_USER, 'preferred-opencl-device.ini')
 
-
 # Location of C source for OpenCL info module
 SOURCE_FILE = 'opencl.c'
 
 
 class OpenCL(myokit.CModule):
     """
     Tests for OpenCL support and can return information about opencl
@@ -37,15 +27,15 @@
     # Cached back-end object if compiled, False if compilation failed
     _instance = None
 
     # Cached compilation error message
     _message = None
 
     def __init__(self):
-        super(OpenCL, self).__init__()
+        super().__init__()
         # Create back-end and cache it
         OpenCL._index += 1
         mname = 'myokit_opencl_info_' + str(OpenCL._index)
         mname += '_' + str(myokit.pid_hash())
         fname = os.path.join(myokit.DIR_CFUNC, SOURCE_FILE)
         args = {'module_name': mname}
 
@@ -161,19 +151,16 @@
         with the platform/device name, or ``None`` if no preference was set.
         """
         platform = device = None
 
         # Read ini file
         inifile = os.path.expanduser(SETTINGS_FILE)
         if os.path.isfile(inifile):
-            config = ConfigParser()
-            try:
-                config.read(inifile, encoding='ascii')  # Python 3
-            except TypeError:   # pragma: no python 3 cover
-                config.read(inifile)
+            config = configparser.RawConfigParser()
+            config.read(inifile, encoding='ascii')
 
             def get(section, option):
                 x = None
                 if config.has_section(section):
                     if config.has_option(section, option):
                         x = config.get(section, option).strip()
                         if x:
@@ -201,15 +188,15 @@
         # Make sure platform and device can be stored as ascii
         if platform:
             platform = platform.encode('ascii').decode('ascii')
         if device:
             device = device.encode('ascii').decode('ascii')
 
         # Create configuration
-        config = ConfigParser()
+        config = configparser.RawConfigParser()
         config.add_section('selection')
         if platform:
             config.set('selection', 'platform', platform)
         if device:
             config.set('selection', 'device', device)
 
         # Write configuration to ini file
@@ -267,15 +254,15 @@
         platform, device = myokit.OpenCL.load_selection_bytes()
 
         # Build and return
         return cl.build(platform, device, code)
     '''
 
 
-class OpenCLInfo(object):
+class OpenCLInfo:
     """
     Represents information about the available OpenCL platforms and devices.
 
     Each ``OpenCLInfo`` object has a property ``platforms``, containing a tuple
     of :class:`OpenCLPlatformInfo` objects.
 
     ``OpenCLInfo`` objects are created and returned by :class:`myokit.OpenCL`.
@@ -295,15 +282,15 @@
             if platform.name == selected_platform:  # pragma: no cover
                 pname += '  <-- Selected platform in myokit.ini'
             b.append(pname)
             platform._format(b, selected_platform, selected_device, pre=' ')
         return '\n'.join(b)
 
 
-class OpenCLPlatformInfo(object):
+class OpenCLPlatformInfo:
     """
     Represents information about an OpenCL platform.
 
     An ``OpenCLPlatformInfo`` object has the following properties:
 
     ``name`` (string)
         This platform's name.
@@ -372,15 +359,15 @@
             b.append(pre[:-1] + 'Device: ' + self.device.name)
             self.device._format(b, pre, name=False)
 
     def has_extension(self, extension):
         return extension in self.extensions
 
 
-class OpenCLDeviceInfo(object):
+class OpenCLDeviceInfo:
     """
     Represents information about an OpenCL device.
 
     An ``OpenCLDeviceInfo`` object has the following properties:
 
     ``name`` (string)
         This device's name.
```

### Comparing `myokit-1.34.0/myokit/_sim/openclsim.c` & `myokit-1.35.0/myokit/_sim/openclsim.c`

 * *Files 0% similar despite different names*

```diff
@@ -511,17 +511,15 @@
 
     // Create state vector, set initial values
     dsize_state = nx * ny * n_state * sizeof(Real);
     rvec_state = (Real*)malloc(dsize_state);
     for(i=0; i<nx * ny * n_state; i++) {
         flt = PyList_GetItem(state_in, (Py_ssize_t)i);    // Don't decref!
         if(!PyFloat_Check(flt)) {
-            char errstr[200];
-            sprintf(errstr, "Item %u in state vector is not a float.", (unsigned int)i);
-            PyErr_SetString(PyExc_Exception, errstr);
+            PyErr_Format(PyExc_Exception, "Item %u in state vector is not a float.", (unsigned int)i);
             return sim_clean();
         }
         rvec_state[i] = (Real)PyFloat_AsDouble(flt);
     }
 
     // Create diffusion current vector
     if (diffusion) {
@@ -548,17 +546,15 @@
     // Create vector of field data
     if(n_field_data) {
         dsize_field_data = n_field_data * sizeof(Real);
         rvec_field_data = (Real*)malloc(dsize_field_data);
         for(i=0; i<n_field_data; i++) {
             flt = PyList_GetItem(field_data, (Py_ssize_t)i);    // No need to decref
             if(!PyFloat_Check(flt)) {
-                char errstr[200];
-                sprintf(errstr, "Item %u in field data is not a float.", (unsigned int)i);
-                PyErr_SetString(PyExc_Exception, errstr);
+                PyErr_Format(PyExc_Exception, "Item %u in field data is not a float.", (unsigned int)i);
                 return sim_clean();
             }
             rvec_field_data[i] = (Real)PyFloat_AsDouble(flt);
         }
     } else {
         dsize_field_data = sizeof(Real);
         rvec_field_data = (Real*)malloc(dsize_field_data);
```

### Comparing `myokit-1.34.0/myokit/_sim/openclsim.cl` & `myokit-1.35.0/myokit/_sim/openclsim.cl`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_sim/openclsim.py` & `myokit-1.35.0/myokit/_sim/openclsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: UTF-8 -*-
 #
 # OpenCL driven simulation, 1d or 2d
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
-import myokit
-import numpy as np
 import platform
+
 from collections import OrderedDict
 
+import numpy as np
+
+import myokit
+
 
 # Location of C and OpenCL sources
 SOURCE_FILE = 'openclsim.c'
 KERNEL_FILE = 'openclsim.cl'
 
 
 class SimulationOpenCL(myokit.CModule):
@@ -144,15 +144,15 @@
 
     """
     _index = 0  # Unique id for the generated module
 
     def __init__(
             self, model, protocol=None, ncells=256, diffusion=True,
             precision=myokit.SINGLE_PRECISION, native_maths=False, rl=False):
-        super(SimulationOpenCL, self).__init__()
+        super().__init__()
 
         # Require a valid model
         if not model.is_valid():
             model.validate()
 
         # Require independent components
         if model.has_interdependent_components():
```

### Comparing `myokit-1.34.0/myokit/_sim/pacing.h` & `myokit-1.35.0/myokit/_sim/pacing.h`

 * *Files 2% similar despite different names*

```diff
@@ -349,17 +349,15 @@
     // Default values
     n = 0;
     events = 0;
 
     if (protocol != Py_None) {
 
         // Get PyList from protocol (will need to decref!)
-        // Cast to (char*) happens because CallMethod accepts a mutable char*
-        // This should have been const char* and has been fixed in python 3
-        PyObject* list = PyObject_CallMethod(protocol, (char*)"events", NULL); // Returns a new reference
+        PyObject* list = PyObject_CallMethod(protocol, "events", NULL); // Returns a new reference
         if(list == NULL) return ESys_POPULATE_INVALID_PROTOCOL;
         if(!PyList_Check(list)) {
             Py_DECREF(list);
             return ESys_POPULATE_INVALID_PROTOCOL;
         }
         n = PyList_Size(list);
 
@@ -762,17 +760,15 @@
 
     // Check ESys
     if(sys == 0) return FSys_INVALID_SYSTEM;
     if (sys->n_points != -1) return FSys_POPULATED_SYSTEM;
     if (protocol == Py_None) return FSys_POPULATE_INVALID_PROTOCOL;
 
     // Get PyList from protocol (will need to decref!)
-    // Cast to (char*) happens because CallMethod accepts a mutable char*
-    // This should have been const char* and has been fixed in python 3
-    times_list = PyObject_CallMethod(protocol, (char*)"times", NULL); // Returns a new reference
+    times_list = PyObject_CallMethod(protocol, "times", NULL); // Returns a new reference
     if(times_list == NULL) return FSys_POPULATE_INVALID_PROTOCOL;
     if(!PyList_Check(times_list)) {
         Py_DECREF(times_list);
         return FSys_POPULATE_INVALID_TIMES;
     }
 
     // Check and convert times list
```

### Comparing `myokit-1.34.0/myokit/_sim/rhs.c` & `myokit-1.35.0/myokit/_sim/rhs.c`

 * *Files 6% similar despite different names*

```diff
@@ -131,46 +131,39 @@
  */
 static int
 log_extract(PyObject* data, const char* name, const int position, double* var)
 {
     PyObject* key;
     PyObject* list;
     PyObject* item;
-    char errstr[1000];
 
     // Get sequence from dict
     key = PyUnicode_FromString(name);
     if (!PyDict_Contains(data, key)) {
         Py_DECREF(key);
-        // Raise exception
-        sprintf(errstr, "Variable %s not found in log.", name);
-        PyErr_SetString(PyExc_Exception, errstr);
+        PyErr_Format(PyExc_Exception, "Variable %s not found in log.", name);
         return 0;
     }
     list = PyDict_GetItem(data, key); // Borrowed ref, don't decref
     Py_DECREF(key);
 
     // Get float from sequence
     key = PyLong_FromLong(position);
     item = PySequence_GetItem(list, position); // New reference, decref
     if (item == NULL) {
         Py_DECREF(key);
-        // Raise exception
-        sprintf(errstr, "No item found at position %i of log for %s.", position, name);
-        PyErr_SetString(PyExc_Exception, errstr);
+        PyErr_Format(PyExc_Exception, "No item found at position %i of log for %s.", position, name);
         return 0;
     }
     Py_DECREF(key);
 
     // Get double from float
     if (!PyFloat_Check(item)) {
         Py_XDECREF(item);
-        // Raise exception
-        sprintf(errstr, "Log for %s can only contain floats (error at index %i).", name, position);
-        PyErr_SetString(PyExc_Exception, errstr);
+        PyErr_Format(PyExc_Exception, "Log for %s can only contain floats (error at index %i).", name, position);
         return 0;
     }
 
     // Assign value to variable
     *var = PyFloat_AsDouble(item);
 
     // Decrease reference count of float object
```

### Comparing `myokit-1.34.0/myokit/_sim/rhs.py` & `myokit-1.35.0/myokit/_sim/rhs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 #
 # Right-hand-side equation benchmarking tool.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
-import timeit
-import myokit
 import platform
+import timeit
 
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
-
+import myokit
 
 # Location of C source file
 SOURCE_FILE = 'rhs.c'
 
 
 class RhsBenchmarker(myokit.CModule):
     """
@@ -38,15 +29,15 @@
     the given list will be tested.
 
     A valid myokit model should be provided as the ``model`` argument.
     """
     _index = 0  # Unique id for the generated module
 
     def __init__(self, model, variables=None, exclude_selected=False):
-        super(RhsBenchmarker, self).__init__()
+        super().__init__()
 
         # Require a valid model
         model.validate()
 
         # Clone model
         self._model = model.clone()
 
@@ -197,15 +188,15 @@
         and stores a result in self._variables.
         """
         if variables is None:
             self._variables = []
         else:
             self._variables = set()
             for var in variables:
-                if isinstance(var, basestring):
+                if isinstance(var, str):
                     # String? Then get variable from model
                     var = self._model.get(var)
                 else:
                     # Variable object? Then replace by equivalent form internal
                     # cloned model.
                     var = self._model.get(var.qname())
                 if var.is_constant():
```

### Comparing `myokit-1.34.0/myokit/_sim/sundials.c` & `myokit-1.35.0/myokit/_sim/sundials.c`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/_sim/sundials.py` & `myokit-1.35.0/myokit/_sim/sundials.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Sundials information class
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 
 import myokit
 
 # Path to C Source for Sundials info module
 SOURCE_FILE = 'sundials.c'
 
@@ -28,15 +25,15 @@
     # Cached compilation error messages
     _message = None
 
     # Version of Sundials found
     _version = None
 
     def __init__(self):
-        super(Sundials, self).__init__()
+        super().__init__()
         # Create and cache back-end
         Sundials._index += 1
 
         # Define libraries
         libd = list(myokit.SUNDIALS_LIB)
         incd = list(myokit.SUNDIALS_INC)
         incd.append(myokit.DIR_CFUNC)
```

### Comparing `myokit-1.34.0/myokit/_system.py` & `myokit-1.35.0/myokit/_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 #
 # System information class.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
+import importlib
 import os
-import sys
 import platform
-import importlib
+import sys
 
 import myokit
 
 
 def system(live_printing=False):
     """
     Returns a (long) string with system information.
@@ -24,15 +21,15 @@
     """
 
     # Print directly to screen or store in array
     if not live_printing:
         out = []
     else:
         # Create fake list interface that just prints
-        class Out(object):
+        class Out:
             def append(self, x):
                 print(x)
 
             def extend(self, xs):
                 print('\n'.join(xs))
 
         out = Out()
@@ -64,33 +61,30 @@
     out.append('MoviePy: ' + _module_version('moviepy'))
     out.append('')
 
     # GUI toolkits
     out.append('== GUI ==')
 
     try:    # pragma: no cover
-        from PyQt5.QtCore import QT_VERSION_STR
-        out.append('PyQt5: ' + QT_VERSION_STR)
+        from PyQt6.QtCore import QT_VERSION_STR
+        out.append('PyQt6: ' + QT_VERSION_STR)
         out.append('  Sip: ' + _module_version('sip'))
         del QT_VERSION_STR
     except ImportError:
-        out.append('PyQt5: Not found')
+        out.append('PyQt6: Not found')
 
     try:    # pragma: no cover
-        from PyQt4.QtCore import QT_VERSION_STR
-        out.append('PyQt4: ' + QT_VERSION_STR)
+        from PyQt5.QtCore import QT_VERSION_STR
+        out.append('PyQt5: ' + QT_VERSION_STR)
         out.append('  Sip: ' + _module_version('sip'))
         del QT_VERSION_STR
     except ImportError:
-        out.append('PyQt4: Not found')
-    except RuntimeError:    # pragma: no cover
-        # Happens if PyQt5 was also found
-        out.append('PyQt4: OK')
+        out.append('PyQt5: Not found')
 
-    out.append('PySide: ' + _module_version('PySide'))
+    out.append('PySide6: ' + _module_version('PySide6'))
     out.append('PySide2: ' + _module_version('PySide2'))
     out.append('')
 
     # Development tools
     out.append('== Development tools ==')
     out.append('Sphinx: ' + _module_version('sphinx'))
     out.append('Flake8: ' + _module_version('flake8'))
```

### Comparing `myokit-1.34.0/myokit/_unit.py` & `myokit-1.35.0/myokit/_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 #
 # Myokit symbolic expression classes. Defines different expressions, equations
 # and the unit system.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import math
 
 import myokit
 
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
-
 
-class Unit(object):
+class Unit:
     """
     Represents a unit.
 
     Most users won't want to create units, but instead use e.g.
     ``myokit.parse_unit('kg/mV')`` or ``myokit.units.mV``.
 
     Each Unit consists of
@@ -518,15 +509,15 @@
             more obscure units (furlong, parsec). Having ``output`` set to
             ``False`` will cause one-way behavior: Myokit will recognise the
             unit name but never use it in output.
             Setting this to ``True`` will also register the given name as a
             preferred representation format.
 
         """
-        if not isinstance(name, basestring):
+        if not isinstance(name, str):
             raise TypeError('Given name must be a string.')
         if not isinstance(unit, Unit):
             raise TypeError('Given unit must be myokit.Unit')
         Unit._units[name] = unit
         if quantifiable:
             # Overwrite existing entries without warning
             Unit._quantifiable.add(name)
@@ -675,15 +666,15 @@
         if not isinstance(other, Unit):
             return Unit(list(self._x), self._m - math.log10(float(other)))
         return Unit(
             [a - b for a, b in zip(self._x, other._x)],
             self._m - other._m)
 
 
-class Quantity(object):
+class Quantity:
     """
     Represents a quantity with a :class:`unit <myokit.Unit>`. Can be used to
     perform unit-safe arithmetic.
 
     Example::
 
         >>> from myokit import Quantity as Q
```

### Comparing `myokit-1.34.0/myokit/float.py` & `myokit-1.35.0/myokit/float.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Functions related to floating point numbers. Imported by default.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import sys
 
 import myokit
 
 # Store ref to built-in `round` and `str` functions
 _round = round
 _str = str
```

### Comparing `myokit-1.34.0/myokit/formats/__init__.py` & `myokit-1.35.0/myokit/formats/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 #
 # Contains functions for the import and export of Myokit objects.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-import myokit
 import os
 import sys
 import traceback
 import warnings
 
+import myokit
+
 # Constants
 DIR_FORMATS = os.path.join(myokit.DIR_MYOKIT, 'formats')
 
 # Hidden lists
 _IMPORTERS = None
 _EXPORTERS = None
 _EWRITERS = None
 
 
 # Classes & methods
-class Exporter(object):
+class Exporter:
     """
     Abstract base class for exporters.
     """
     def __init__(self):
-        super(Exporter, self).__init__()
+        super().__init__()
 
     def post_export_info(self):
         """
         Optional method that returns a string containing information about this
         exporter, to be shown after the export is completed.
         """
         return ''
@@ -102,15 +100,15 @@
     Returns a list of available exporters by name.
     """
     if _EXPORTERS is None:  # pragma: no cover
         _scan_for_internal_formats()
     return sorted(_EXPORTERS.keys())
 
 
-class ExpressionWriter(object):
+class ExpressionWriter:
     """
     Base class for expression writers, that take myokit expressions as input
     and convert them to text or other formats.
     """
     def __init__(self):
         self._op_map = self._build_op_map()
 
@@ -318,20 +316,20 @@
     Returns a list of available expression writers by name.
     """
     if _EWRITERS is None:   # pragma: no cover
         _scan_for_internal_formats()
     return sorted(_EWRITERS.keys())
 
 
-class Importer(object):
+class Importer:
     """
     Abstract base class for importers.
     """
     def __init__(self):
-        super(Importer, self).__init__()
+        super().__init__()
 
     def component(self, path, model):
         """
         Imports a component from the given ``path`` and adds it to the given
         model.
 
         The importer may pose restraints on the used model. For example, the
@@ -407,15 +405,15 @@
     """
     *Abstract class, extends:* :class:`Exporter`
 
     Abstract base class for exporters that turn a model (and optionally a
     protocol) into a runnable chunk of code.
     """
     def __init__(self):
-        super(TemplatedRunnableExporter, self).__init__()
+        super().__init__()
 
     def runnable(self, path, model, protocol=None, *args):
         """
         Exports a :class:`myokit.Model` and optionally a
         :class:`myokit.Protocol` to something that can be run or compiled.
 
         The output will be stored in the **directory** ``path``.
```

### Comparing `myokit-1.34.0/myokit/formats/ansic/__init__.py` & `myokit-1.35.0/myokit/formats/ansic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Provides Ansi-C support
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from ._exporter import AnsiCExporter, AnsiCCableExporter, AnsiCEulerExporter
 from ._ewriter import AnsiCExpressionWriter
 
 
 # Importers
 
 # Exporters
```

### Comparing `myokit-1.34.0/myokit/formats/ansic/_ewriter.py` & `myokit-1.35.0/myokit/formats/matlab/_ewriter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 #
-# Ansi-C expression writer
+# Matlab expression writer and keywords
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-import myokit
 from myokit.formats.python import PythonExpressionWriter
 
 
-class AnsiCExpressionWriter(PythonExpressionWriter):
+class MatlabExpressionWriter(PythonExpressionWriter):
     """
-    This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` writes
-    equations for variables in a C-style syntax.
+    This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` translates
+    Myokit :class:`expressions <myokit.Expression>` to a Matlab syntax.
     """
     def __init__(self):
-        super(AnsiCExpressionWriter, self).__init__()
+        super().__init__()
         self._function_prefix = ''
-        self._fcond = None
+        self._fcond = 'ifthenelse'
 
     def set_condition_function(self, func=None):
         """
         Sets a function name to use for if statements
 
         By setting func to None you can revert back to the default behavior
          (the ternary operator). Any other value will be interpreted as the
-         name of a C function taking arguments (condition, value_if_true,
+         name of a function taking arguments (condition, value_if_true,
          value_if_false).
         """
         self._fcond = func
 
     #def _ex_name(self, e):
     #def _ex_derivative(self, e):
     #def _ex_number(self, e):
@@ -39,48 +35,47 @@
     #def _ex_prefix_minus(self, e):
     #def _ex_plus(self, e):
     #def _ex_minus(self, e):
     #def _ex_multiply(self, e):
     #def _ex_divide(self, e):
 
     def _ex_quotient(self, e):
-        # Note that this _must_ round towards minus infinity!
-        # See myokit.Quotient !
-        return self.ex(myokit.Floor(myokit.Divide(e[0], e[1])))
+        # Round towards minus infinity
+        return 'floor(' + self._ex_infix(e, '/') + ')'
 
     def _ex_remainder(self, e):
-        # Note that this _must_ use the same round-to-neg-inf convention as
-        # myokit.Quotient! Implementation below is consistent with Python
-        # convention:
-        return self.ex(myokit.Minus(
-            e[0], myokit.Multiply(e[1], myokit.Quotient(e[0], e[1]))))
+        # Uses the round-towards-minus-infinity convention!
+        return 'mod(' + self.ex(e[0]) + ', ' + self.ex(e[1]) + ')'
 
     def _ex_power(self, e):
-        return 'pow(' + self.ex(e[0]) + ', ' + self.ex(e[1]) + ')'
+        return self._ex_infix(e, '^')
 
     #def _ex_sqrt(self, e):
+    #    Ignore imaginary part
+    #    return 'real(' + self._ex_function(e, 'sqrt') + ')'
     #def _ex_sin(self, e):
     #def _ex_cos(self, e):
     #def _ex_tan(self, e):
     #def _ex_asin(self, e):
     #def _ex_acos(self, e):
     #def _ex_atan(self, e):
     #def _ex_exp(self, e):
 
     def _ex_log(self, e):
         if len(e) == 1:
             return self._ex_function(e, 'log')
-        return '(log(' + self.ex(e[0]) + ') / log(' + self.ex(e[1]) + '))'
+        else:
+            return '(log(' + self.ex(e[0]) + ') / log(' + self.ex(e[1]) + '))'
 
     #def _ex_log10(self, e):
     #def _ex_floor(self, e):
     #def _ex_ceil(self, e):
 
     def _ex_abs(self, e):
-        return self._ex_function(e, 'fabs')
+        return self._ex_function(e, 'abs')
 
     def _ex_not(self, e):
         return '!(' + self.ex(e[0]) + ')'
 
     #def _ex_equal(self, e):
     #def _ex_not_equal(self, e):
     #def _ex_more(self, e):
@@ -91,30 +86,24 @@
     def _ex_and(self, e):
         return self._ex_infix_condition(e, '&&')
 
     def _ex_or(self, e):
         return self._ex_infix_condition(e, '||')
 
     def _ex_if(self, e):
-        ite = (self.ex(e._i), self.ex(e._t), self.ex(e._e))
-        if self._fcond is None:
-            return '(%s ? %s : %s)' % ite
-        else:
-            return '%s(%s, %s, %s)' % ((self._fcond,) + ite)
+        return '%s(%s, %s, %s)' % (
+            self._fcond, self.ex(e._i), self.ex(e._t), self.ex(e._e))
 
     def _ex_piecewise(self, e):
         s = []
         n = len(e._i)
-        if self._fcond is None:
-            for i in range(0, n):
-                s.append('(%s ? %s : ' % (self.ex(e._i[i]), self.ex(e._e[i])))
-            s.append(self.ex(e._e[n]))
-            s.append(')' * n)
-        else:
-            for i in range(0, n):
-                s.append(
-                    '%s(%s, %s, ' % (
-                        self._fcond, self.ex(e._i[i]), self.ex(e._e[i])))
-            s.append(self.ex(e._e[n]))
-            s.append(')' * n)
+        for i in range(0, n):
+            s.append(self._fcond)
+            s.append('(')
+            s.append(self.ex(e._i[i]))
+            s.append(', ')
+            s.append(self.ex(e._e[i]))
+            s.append(', ')
+        s.append(self.ex(e._e[n]))
+        s.append(')' * n)
         return ''.join(s)
```

### Comparing `myokit-1.34.0/myokit/formats/ansic/_exporter.py` & `myokit-1.35.0/myokit/formats/ansic/_exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Exports to Ansi C, using the CVODE libraries for integration
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 
 import myokit.formats
 
 
 class AnsiCExporter(myokit.formats.TemplatedRunnableExporter):
     """
```

### Comparing `myokit-1.34.0/myokit/formats/ansic/template/cable.c` & `myokit-1.35.0/myokit/formats/ansic/template/cable.c`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/ansic/template/euler.c` & `myokit-1.35.0/myokit/formats/ansic/template/euler.c`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/ansic/template/sim.c` & `myokit-1.35.0/myokit/formats/ansic/template/sim.c`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/axon/_abf.py` & `myokit-1.35.0/myokit/formats/axon/_abf.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,31 +135,30 @@
 #-----------------------------------  end  ------------------------------------
 # The abf2load script is available from:
 #  http://www.mathworks.com/matlabcentral/fileexchange/22114-abf2load
 #------------------------------------------------------------------------------
 # Information - but no direct code - from the matlab script get_abf_header.m
 # was also used: http://neurodata.hg.sourceforge.net/hgweb/neurodata/neurodata/
 #------------------------------------------------------------------------------
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-from collections import OrderedDict
-import numpy as np
-import traceback
 import datetime
 import logging
-import struct
 import os
+import struct
+import traceback
+
+import numpy as np
+
+from collections import OrderedDict
 
 
 # Encoding for text parts of files
 _ENC = 'latin-1'
 
 
-class AbfFile(object):
+class AbfFile:
     """
     Represents a read-only Axon Binary Format file (``.abf``), stored at the
     location pointed to by ``filepath``.
 
     Files in the "ABF" format and the newer "ABF2" format can be read. If the
     given ``filepath`` ends in ``.pro`` a protocol file is assumed. This
     assumption can be overruled by setting the ``is_protocol_file`` argument
@@ -195,15 +194,14 @@
     :class:`myokit.DataLog` version of the file's data, use:meth:`myokit_log`.
 
     In some cases, a myokit protocol can be created from a stored stimulus
     protocol. To do this, use the method:meth:`myokit_protocol`.
     """
     def __init__(self, filepath, is_protocol_file=None):
         # The path to the file and its basename
-        # Ensure it's a `str` for Python2/3 compatibility
         filepath = str(filepath)
         self._filepath = os.path.abspath(filepath)
         self._filename = os.path.basename(filepath)
 
         # Abf format version
         self._version = None
 
@@ -698,15 +696,14 @@
         Reads the file's header.
         """
 
         def read_f(f, form, offset=None):
             """
             Read and unpack a file section using the given format ``form``.
             """
-            # Form must be a str (so bytes on Python 2)
             form = str(form)
             if offset is not None:
                 f.seek(offset)
             return struct.unpack(form, f.read(struct.calcsize(form)))
 
         def ups(val):
             """
@@ -1302,22 +1299,22 @@
                     if h['nSignalType'] != 0:
                         s -= a[i]['fSignalOffset']
 
                 # Set final offset
                 self._adc_offsets.append(s)
 
 
-class Sweep(object):
+class Sweep:
     """
     Represents a single sweep (also called an 'episode')
 
     A sweep is represented as a fixed-size list of channels.
     """
     def __init__(self, n):
-        super(Sweep, self).__init__()
+        super().__init__()
         n = int(n)
         if n < 0:   # pragma: no cover
             raise ValueError('Number channels cannot be negative.')
         self._nc = n    # Number of channels
         self._channels = [None] * n
 
     def __getitem__(self, key):
@@ -1332,22 +1329,22 @@
     def __setitem__(self, key, value):
         if type(key) == slice:
             raise NotImplementedError(
                 'Assignment with slices is not supported.')
         self._channels[key] = value
 
 
-class Channel(object):
+class Channel:
     """
     Represents an analog signal for a single channel.
 
     To obtain this channel's formatted data, use times() and trace()
     """
     def __init__(self, parent_file):
-        super(Channel, self).__init__()
+        super().__init__()
         self._parent_file = parent_file  # The abf file this channel is from
         self._type = TYPE_UNKNOWN   # Type of recording
 
         # This channel's name
         self._name = None
 
         # This channel's index (see note below)
@@ -1382,15 +1379,15 @@
         Returns the name set for this channel.
         """
         return self._name
 
     def number(self):
         """
         Returns the channel index used by pClamp. Note that this does not
-        necessarily equal its index in the python sweep data!
+        necessarily equal its index in the Python sweep data!
         """
         return self._numb
 
     def __str__(self):
         return 'Channel(' + str(self._numb) + ' "' + str(self._name) \
             + '"); ' + str(len(self._data)) + ' points sampled at ' \
             + str(self._rate) + 'Hz, starts at t=' + str(self._start)
```

### Comparing `myokit-1.34.0/myokit/formats/axon/_atf.py` & `myokit-1.35.0/myokit/formats/axon/_atf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #
 # This module reads files in Axon Text File format.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-from collections import OrderedDict
-import numpy as np
 import os
 import re
 
+import numpy as np
+
+from collections import OrderedDict
+
 
 # Format used for any text
 _ENC = 'ascii'
 
 
-class AtfFile(object):
+class AtfFile:
     """
     Represents an Axon Text File (ATF) stored on disk.
 
     This method provides access to the data stored in the ATF as well as any
     meta data stored in the header.
 
     Access to the data is provided using a dict-like interface: to iterate over
```

### Comparing `myokit-1.34.0/myokit/formats/axon/_importer.py` & `myokit-1.35.0/myokit/formats/axon/_importer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Imports selected types of protocols from files in Axon Binary Format
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit.formats
 
 
 class AbfImporter(myokit.formats.Importer):
     """
     This :class:`Importer <myokit.formats.Importer>` can import protocols from
     files in Axon Binary Format.
```

### Comparing `myokit-1.34.0/myokit/formats/cellml/__init__.py` & `myokit-1.35.0/myokit/formats/cellml/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Provides CellML support
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from ._exporter import CellMLExporter, CellML1Exporter, CellML2Exporter
 from ._ewriter import CellMLExpressionWriter
 from ._importer import CellMLImporter, CellMLImporterError  # noqa
 
 
 # Namespaces
 NS_BQBIOL = 'http://biomodels.net/biology-qualifiers/'
```

### Comparing `myokit-1.34.0/myokit/formats/cellml/_ewriter.py` & `myokit-1.35.0/myokit/formats/cellml/_ewriter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # CellML expression writer
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from lxml import etree
 
 import myokit
 import myokit.formats.cellml
 
 from myokit.formats.mathml import MathMLExpressionWriter
 
@@ -20,16 +17,16 @@
     Writes equations for variables using CellML's version of MathML.
 
     To use, create an expression writer, then pass in a method to set good
     variable names with :meth:`set_lhs_function()`, and a method to look up
     unit names with :meth:`set_unit_function()`.
     """
     def __init__(self, version='1.0'):
-        super(CellMLExpressionWriter, self).__init__()
-        super(CellMLExpressionWriter, self).set_mode(presentation=False)
+        super().__init__()
+        super().set_mode(presentation=False)
 
         # Units lookup method
         self._funits = None
 
         # Use unames by default
         self._flhs = lambda x: x.var().uname()
 
@@ -50,15 +47,15 @@
         """
         Sets a unit lookup function, which will be used to convert a
         :class:`myokit.Unit` to a CellML units name.
         """
         self._funits = f
 
     def _ex_number(self, e, t):
-        x = super(CellMLExpressionWriter, self)._ex_number(e, t)
+        x = super()._ex_number(e, t)
         unit = e.unit()
         if self._funits is not None and unit is not None:
             units = self._funits(e.unit())
         else:
             units = 'dimensionless'
         x.attrib[etree.QName(self._ns, 'units')] = units
```

### Comparing `myokit-1.34.0/myokit/formats/cellml/_exporter.py` & `myokit-1.35.0/myokit/formats/cellml/_exporter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 #
 # Exports to CellML.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
 import myokit.lib.guess
 
 import warnings
 
 
 class CellMLExporter(myokit.formats.Exporter):
     """
     This:class:`Exporter <myokit.formats.Exporter>` creates a CellML model.
     """
     def __init__(self):
-        super(CellMLExporter, self).__init__()
+        super().__init__()
 
     def model(self, path, model, protocol=None, version='1.0'):
         """
         Writes a CellML model to the given filename.
 
         Arguments:
 
@@ -65,17 +62,17 @@
 
 
 class CellML1Exporter(CellMLExporter):
     """
     This:class:`Exporter <myokit.formats.Exporter>` creates a CellML 1.0 model.
     """
     def model(self, path, model, protocol=None):
-        super(CellML1Exporter, self).model(path, model, protocol, '1.0')
+        super().model(path, model, protocol, '1.0')
 
 
 class CellML2Exporter(CellMLExporter):
     """
     This:class:`Exporter <myokit.formats.Exporter>` creates a CellML 2.0 model.
     """
     def model(self, path, model, protocol=None):
-        super(CellML2Exporter, self).model(path, model, protocol, '2.0')
+        super().model(path, model, protocol, '2.0')
```

### Comparing `myokit-1.34.0/myokit/formats/cellml/_importer.py` & `myokit-1.35.0/myokit/formats/cellml/_importer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #
 # Imports a model definition from a CellML file
 # Only partial CellML support is provided.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from lxml import etree
 
 import myokit
 import myokit.formats
 
 from myokit.formats.xml import split
 
@@ -24,15 +21,15 @@
 
 class CellMLImporter(myokit.formats.Importer):
     """
     This :class:`Importer <myokit.formats.Importer>` imports a model definition
     from CellML.
     """
     def __init__(self, verbose=False):
-        super(CellMLImporter, self).__init__()
+        super().__init__()
 
     def model(self, path):
         """
         Reads a CellML file and returns a:class:`myokit.Model`.
         """
         import myokit.formats.cellml as cellml
         import myokit.formats.cellml.v1 as v1
```

### Comparing `myokit-1.34.0/myokit/formats/cellml/v1/_api.py` & `myokit-1.35.0/myokit/formats/cellml/v1/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # CellML 1.0/1.1 API
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import collections
 import re
 import warnings
 
 import myokit
 
 
@@ -112,15 +109,15 @@
         multiplier = multiplier.replace('-', '_minus_')
         multiplier = multiplier.replace('.', '_dot_')
         name += '_times_' + multiplier
 
     return name
 
 
-class AnnotatableElement(object):
+class AnnotatableElement:
     """
     Represents a CellML 1.0 or 1.1 element that can have a cmeta:id.
 
     Each ``AnnotatableElement`` also has a public dict ``meta`` that can be
     used to story key:value (string:string) pairs, for storing meta data.
     """
 
@@ -183,34 +180,34 @@
 
 class UnsupportedBaseUnitsError(UnitsError):
     """
     Raised when unsupported base units are used.
     """
     def __init__(self, units):
         self.units = units
-        super(UnsupportedBaseUnitsError, self).__init__(
+        super().__init__(
             'Unsupported base units "' + units + '".')
 
 
 class UnsupportedUnitOffsetError(UnitsError):
     """
     Raised when units with non-zero offsets are used.
     """
     def __init__(self):
-        super(UnsupportedUnitOffsetError, self).__init__(
+        super().__init__(
             'Units with non-zero offsets are not supported.')
 
 
 class Component(AnnotatableElement):
     """
     Represents a model component, should not be created directly but only via
     :meth:`Model.add_component()`.
     """
     def __init__(self, model, name):
-        super(Component, self).__init__(model)
+        super().__init__(model)
 
         # Store model
         self._model = model
 
         # Check and store name
         if not is_valid_identifier(name):
             raise CellMLError(
@@ -470,15 +467,15 @@
         A valid CellML identifier string.
     ``version``
         A string representing the CellML version this model is in (must be
         '1.0' or '1.1').
 
     """
     def __init__(self, name, version='1.0'):
-        super(Model, self).__init__(self)
+        super().__init__(self)
 
         # Check and store name
         if not is_valid_identifier(name):
             raise CellMLError(
                 'Model name must be a valid CellML identifier (3.4.1.2).')
         self._name = name
 
@@ -1161,15 +1158,15 @@
     def version(self):
         """
         Returns the CellML version this model is in.
         """
         return self._version
 
 
-class Units(object):
+class Units:
     """
     Represents a CellML units definition, should not be created directly but
     only via :meth:`Model.add_units()` or :meth:`Component.add_units()`.
 
     Arguments:
 
     ``name``
@@ -1466,15 +1463,15 @@
         The variable's public interface.
     ``private_interface``
         The variable's private interface.
 
     """
     def __init__(self, component, name, units, public_interface='none',
                  private_interface='none'):
-        super(Variable, self).__init__(component.model())
+        super().__init__(component.model())
 
         # Store component
         self._component = component
 
         # Check and store name
         if not is_valid_identifier(name):
             raise CellMLError(
```

### Comparing `myokit-1.34.0/myokit/formats/cellml/v1/_parser.py` & `myokit-1.35.0/myokit/formats/cellml/v1/_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Parses a CellML 1.0 or 1.1 document.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import collections
 import warnings
 
 from lxml import etree
 
 import myokit
 import myokit.formats.mathml
@@ -56,18 +53,18 @@
     def __init__(self, message, element=None):
         if element is not None:
             try:    # pragma: no cover
                 line = str(element.sourceline)
                 message = 'Error on line ' + line + '. ' + message
             except AttributeError:
                 pass
-        super(CellMLParsingError, self).__init__(message)
+        super().__init__(message)
 
 
-class CellMLParser(object):
+class CellMLParser:
     """
     Parses CellML 1.0 and 1.1 documents, and performs (partial) validation of a
     CellML document.
 
     For notes about CellML 1.0/1.1 support, see
     :class:`myokit.formats.cellml.v1.Model`.
     """
```

### Comparing `myokit-1.34.0/myokit/formats/cellml/v1/_writer.py` & `myokit-1.35.0/myokit/formats/cellml/v1/_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 #
 # CellML 1.0/1.1 Writer: Writes a CellML Model to disk
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from lxml import etree
+from urllib.parse import quote
 
 import myokit
 import myokit.formats.cellml as cellml
 
-# Quoting URI strings in Python2 and Python3
-try:
-    from urllib.parse import quote
-except ImportError:     # pragma: no python 3 cover
-    # Python 2
-    from urllib import quote
-
 
 # Left-over from old exporter. Not sure if this had any function.
 # Add name in 'tmp-documentation' format
 # emodel.attrib['name'] = 'generated_model'
 # if 'name' in model.meta:
 #     dtag = et.SubElement(emodel, 'documentation')
 #     dtag.attrib['xmlns'] = NS_TMP_DOC
@@ -41,15 +32,15 @@
 def write_string(model):
     """
     Writes a CellML 1.0 or 1.1 model to a string and returns it.
     """
     return CellMLWriter().write_string(model)
 
 
-class CellMLWriter(object):
+class CellMLWriter:
     """
     Writes CellML 1.0 or 1.1 documents.
     """
 
     # List of si unit names corresponding to myokit.Unit exponents
     _exp_si = None
```

### Comparing `myokit-1.34.0/myokit/formats/cellml/v2/__init__.py` & `myokit-1.35.0/myokit/formats/cellml/v1/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 #
-# CellML 2.0 support.
+# CellML 1.0 and 1.1 support.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from ._api import (     # noqa
     AnnotatableElement,
     CellMLError,
     clean_identifier,
     create_unit_name,
     Component,
     Model,
     Units,
+    UnitsError,
+    UnsupportedBaseUnitsError,
+    UnsupportedUnitOffsetError,
     Variable,
-    is_basic_real_number_string,
-    is_identifier,
-    is_integer_string,
-    is_real_number_string,
+    is_valid_identifier,
 )
 
 from ._parser import (  # noqa
     parse_file,
     parse_string,
     CellMLParser,
     CellMLParsingError,
```

### Comparing `myokit-1.34.0/myokit/formats/cellml/v2/_api.py` & `myokit-1.35.0/myokit/formats/cellml/v2/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 #
 # CellML 2.0 API
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import collections
 import re
 import warnings
 
 import myokit
 
-# Strings in Python2 and Python3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
-
 
 # Data types
 _cellml_identifier = re.compile(r'^[a-zA-Z][a-zA-Z0-9_]*$')
 _cellml_integer = re.compile(r'^[+-]?[0-9]+$')
 _real = r'[+-]?(([0-9]*\.[0-9]+)|([0-9]+\.?[0-9]*))'
 _cellml_basic_real = re.compile(r'^' + _real + r'$')
 _cellml_real = re.compile(r'^' + _real + r'([eE][+-]?[0-9]+)?$')
@@ -138,15 +129,15 @@
         multiplier = multiplier.replace('-', '_minus_')
         multiplier = multiplier.replace('.', '_dot_')
         name += '_times_' + multiplier
 
     return name
 
 
-class AnnotatableElement(object):
+class AnnotatableElement:
     """
     Represents a CellML 2.0 element that can be annotated (using a public dict
     ``meta`` that stores key:value pairs).
     """
 
     def __init__(self):
 
@@ -163,15 +154,15 @@
 
 class Component(AnnotatableElement):
     """
     Represents a model component; should not be created directly but only via
     :meth:`Model.add_component()`.
     """
     def __init__(self, model, name):
-        super(Component, self).__init__()
+        super().__init__()
 
         # Store model
         self._model = model
 
         # Check and store name
         if not is_identifier(name):
             raise CellMLError(
@@ -319,15 +310,15 @@
         A valid CellML identifier string.
     ``version``
         A string representing the CellML version this model is in (must be
         '2.0').
 
     """
     def __init__(self, name, version='2.0'):
-        super(Model, self).__init__()
+        super().__init__()
 
         # Check and store name
         if not is_identifier(name):
             raise CellMLError(
                 'Model name must be a valid CellML identifier.')
         self._name = name
 
@@ -1064,15 +1055,15 @@
     def version(self):
         """
         Returns the CellML version this model is in.
         """
         return self._version
 
 
-class Units(object):
+class Units:
     """
     Represents a CellML units definition; should not be created directly but
     only via :meth:`Model.add_units()` or :meth:`Component.add_units()`.
 
     Arguments:
 
     ``name``
@@ -1355,15 +1346,15 @@
     ``units``
         The string name of a units object known to this variable's model.
     ``interface``
         The variable's interface.
 
     """
     def __init__(self, component, name, units, interface='none'):
-        super(Variable, self).__init__()
+        super().__init__()
 
         # Store model and component
         self._model = component.model()
         self._component = component
 
         # Check and store name
         if not is_identifier(name):
@@ -1611,15 +1602,15 @@
         """
         Sets this variable's intial value (must be a number or ``None``).
         """
         # Allow unsetting with ``None``
         if value is not None:
 
             # Check value is a real number string
-            if isinstance(value, basestring):
+            if isinstance(value, str):
                 if is_real_number_string(value):
                     value = float(value)
                 else:
                     raise CellMLError(
                         'If given, a variable initial_value must be a real'
                         ' number (using variables as initial values is not'
                         ' supported).')
@@ -1638,15 +1629,15 @@
     def units(self):
         """
         Returns the units this variable is in (as a :class:`Units` object).
         """
         return self._units
 
 
-class ConnectedVariableSet(object):
+class ConnectedVariableSet:
     """
     Represents a set of connected variables.
 
     Arguments:
 
     ``variable=None``
         An optional first variable in this set.
```

### Comparing `myokit-1.34.0/myokit/formats/cellml/v2/_parser.py` & `myokit-1.35.0/myokit/formats/cellml/v2/_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Parses a CellML 2.0 document.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import warnings
 
 from lxml import etree
 
 import myokit
 import myokit.formats.mathml
 import myokit.formats.cellml as cellml
@@ -55,18 +52,18 @@
     def __init__(self, message, element=None):
         if element is not None:
             try:    # pragma: no cover
                 line = str(element.sourceline)
                 message = 'Error on line ' + line + '. ' + message
             except AttributeError:
                 pass
-        super(CellMLParsingError, self).__init__(message)
+        super().__init__(message)
 
 
-class CellMLParser(object):
+class CellMLParser:
     """
     Parses CellML 2.0 documents, and performs (partial) validation.
 
     For notes about CellML 2.0 support, see
     :class:`myokit.formats.cellml.v2.Model`.
     """
```

### Comparing `myokit-1.34.0/myokit/formats/cellml/v2/_writer.py` & `myokit-1.35.0/myokit/formats/cellml/v2/_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # CellML 2.0 Writer: Writes a CellML Model to disk
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from lxml import etree
 
 import myokit
 import myokit.formats.cellml as cellml
 
 
 def write_file(path, model):
@@ -23,15 +20,15 @@
 def write_string(model):
     """
     Writes a CellML 2.0 model to a string and returns it.
     """
     return CellMLWriter().write_string(model)
 
 
-class CellMLWriter(object):
+class CellMLWriter:
     """
     Writes CellML 2.0 documents.
     """
 
     # List of si unit names corresponding to myokit.Unit exponents
     _exp_si = None
```

### Comparing `myokit-1.34.0/myokit/formats/channelml/_importer.py` & `myokit-1.35.0/myokit/formats/channelml/_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 #
 # Imports a channel model from a ChannelML file.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
+import io
 import os
 import textwrap
+import warnings
 import xml.dom
 import xml.dom.minidom
 
-import warnings
-
-try:
-    # Python 2
-    from cStringIO import StringIO
-except ImportError:
-    # Python3
-    from io import StringIO
-
 import myokit
 from myokit import formats
 from myokit import Name, Number, Minus, Multiply, Divide, Power
 
 
 def dom_child(node):
     """
@@ -67,15 +57,15 @@
 
 class ChannelMLImporter(formats.Importer):
     """
     This :class:`Importer <myokit.formats.Importer>` imports model definitions
     from the ChannelML format.
     """
     def __init__(self, verbose=False):
-        super(ChannelMLImporter, self).__init__()
+        super().__init__()
         self.generated_name_index = 0
 
     def component(self, path, model):
         """
         Imports a channel component from the ChannelML file at ``path`` and
         adds it to the given model.
 
@@ -369,15 +359,15 @@
         """
         Coarsely extracts any meta data from the model and returns it as a text
         file.
         """
         if not root.hasAttribute('xmlns:meta'):
             return None
         ns = root.getAttribute('xmlns:meta')
-        b = StringIO()
+        b = io.StringIO()
 
         def scan(parent):
             kid = dom_child(parent)
             while kid is not None:
                 t = None
                 if kid.namespaceURI == ns:
                     t = self._flatten(kid)
```

### Comparing `myokit-1.34.0/myokit/formats/cuda/__init__.py` & `myokit-1.35.0/myokit/formats/cuda/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Provides an export to a CUDA kernel
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from ._exporter import CudaKernelExporter, CudaKernelRLExporter
 from ._ewriter import CudaExpressionWriter
 from myokit.formats import ansic
 
 
 # Importers
 # Exporters
```

### Comparing `myokit-1.34.0/myokit/formats/cuda/_ewriter.py` & `myokit-1.35.0/myokit/formats/cuda/_ewriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 #
 # CUDA expression writer
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
+
 from myokit.formats.python import PythonExpressionWriter
 
 
 class CudaExpressionWriter(PythonExpressionWriter):
     """
     This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` translates
     Myokit :class:`expressions <myokit.Expression>` to their CUDA equivalents.
     """
     def __init__(self, precision=myokit.SINGLE_PRECISION):
-        super(CudaExpressionWriter, self).__init__()
+        super().__init__()
         self._function_prefix = ''
         self._sp = (precision == myokit.SINGLE_PRECISION)
 
     #def _ex_name(self, e):
     #def _ex_derivative(self, e):
 
     def _ex_number(self, e):
```

### Comparing `myokit-1.34.0/myokit/formats/cuda/_exporter.py` & `myokit-1.35.0/myokit/formats/cuda/_exporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Exports to a CUDA kernel
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 
 import myokit.formats
 
 
 class CudaKernelExporter(myokit.formats.TemplatedRunnableExporter):
     """
```

### Comparing `myokit-1.34.0/myokit/formats/cuda/template/kernel.cu` & `myokit-1.35.0/myokit/formats/cuda/template/kernel.cu`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/easyml/__init__.py` & `myokit-1.35.0/myokit/formats/easyml/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Provides EasyML (CARP/CARPentry) support
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from ._exporter import EasyMLExporter
 from ._ewriter import EasyMLExpressionWriter
 
 
 # Importers
 
 # Exporters
```

### Comparing `myokit-1.34.0/myokit/formats/easyml/_ewriter.py` & `myokit-1.35.0/myokit/formats/easyml/_ewriter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 #
 # EasyML expression writer
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import warnings
 
 import myokit
+
 from myokit.formats.python import PythonExpressionWriter
 
 
 class EasyMLExpressionWriter(PythonExpressionWriter):
     """
     This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` writes
     equations for variables in EasyML syntax.
     """
     def __init__(self):
-        super(EasyMLExpressionWriter, self).__init__()
+        super().__init__()
         self._function_prefix = ''
 
     #def _ex_name(self, e):
     #def _ex_derivative(self, e):
 
     def _ex_number(self, e):
         return myokit.float.str(e)
@@ -35,15 +33,15 @@
     def _ex_minus(self, e):
         if isinstance(e[0], myokit.Exp) and isinstance(e[1], myokit.Number):
             if e[1].eval() == 1:
                 return 'expm1(' + self.ex(e[0][0]) + ')'
         if isinstance(e[1], myokit.Exp) and isinstance(e[0], myokit.Number):
             if e[0].eval() == 1:
                 return '-expm1(' + self.ex(e[1][0]) + ')'
-        return super(EasyMLExpressionWriter, self)._ex_minus(e)
+        return super()._ex_minus(e)
 
     #def _ex_multiply(self, e):
     #def _ex_divide(self, e):
 
     def _ex_quotient(self, e):
         return self.ex(myokit.Floor(myokit.Divide(e[0], e[1])))
 
@@ -54,48 +52,48 @@
     def _ex_power(self, e):
         return 'pow(' + self.ex(e[0]) + ', ' + self.ex(e[1]) + ')'
 
     #def _ex_sqrt(self, e):
 
     def _ex_sin(self, e):
         warnings.warn('Potentially unsupported function: sin()')
-        return super(EasyMLExpressionWriter, self)._ex_sin(e)
+        return super()._ex_sin(e)
 
     #def _ex_cos(self, e):
 
     def _ex_tan(self, e):
         warnings.warn('Potentially unsupported function: tan()')
-        return super(EasyMLExpressionWriter, self)._ex_tan(e)
+        return super()._ex_tan(e)
 
     def _ex_asin(self, e):
         warnings.warn('Potentially unsupported function: asin()')
-        return super(EasyMLExpressionWriter, self)._ex_asin(e)
+        return super()._ex_asin(e)
 
     #def _ex_acos(self, e):
 
     def _ex_atan(self, e):
         warnings.warn('Potentially unsupported function: atan()')
-        return super(EasyMLExpressionWriter, self)._ex_atan(e)
+        return super()._ex_atan(e)
 
     #def _ex_exp(self, e):
 
     def _ex_log(self, e):
         if len(e) == 1:
             return self._ex_function(e, 'log')
         return '(log(' + self.ex(e[0]) + ') / log(' + self.ex(e[1]) + '))'
 
     #def _ex_log10(self, e):
 
     def _ex_floor(self, e):
         warnings.warn('Potentially unsupported function: floor()')
-        return super(EasyMLExpressionWriter, self)._ex_floor(e)
+        return super()._ex_floor(e)
 
     def _ex_ceil(self, e):
         warnings.warn('Potentially unsupported function: ceil()')
-        return super(EasyMLExpressionWriter, self)._ex_ceil(e)
+        return super()._ex_ceil(e)
 
     def _ex_abs(self, e):
         return self._ex_function(e, 'fabs')
 
     def _ex_not(self, e):
         return '!(' + self.ex(e[0]) + ')'
```

### Comparing `myokit-1.34.0/myokit/formats/easyml/_exporter.py` & `myokit-1.35.0/myokit/formats/easyml/_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Export as an EasyML model.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import collections
 import os
 import warnings
 
 import myokit.formats
 import myokit.lib.guess as guess
 import myokit.lib.hh as hh
```

### Comparing `myokit-1.34.0/myokit/formats/html/_exporter.py` & `myokit-1.35.0/myokit/formats/html/_exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Exports to MathML based formats.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from lxml import etree
 
 import myokit
 
 
 class HTMLExporter(myokit.formats.Exporter):
     """
```

### Comparing `myokit-1.34.0/myokit/formats/html/_flatten.py` & `myokit-1.35.0/myokit/formats/html/_flatten.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 #
 # Flattens HTML and attempts to create readable ASCII code.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
+import html
+import html.parser
 import re
-import sys
 import textwrap
 
-# HTML Parser in Python 2 and 3
-try:
-    from HTMLParser import HTMLParser
-except ImportError:
-    from html.parser import HTMLParser
-
 
 def html2ascii(html, width=79, indent='  '):
     """
     Flattens HTML and attempts to create readable ASCII code.
 
     The output will be text-wrapped after ``width`` characters. Each new level
     of nesting will be indented with the text given as ``indent``.
@@ -28,29 +20,21 @@
     # Create asciifier and go!
     f = Asciifier(width, indent)
     f.feed(html)
     f.close()
     return f.get_text()
 
 
-class Asciifier(HTMLParser):
+class Asciifier(html.parser.HTMLParser):
     INDENT = 1
     DEDENT = -1
     WHITE = [' ', '\t', '\f', '\r', '\n']
 
     def __init__(self, line_width=79, indent='  '):
-        if sys.hexversion < 0x03000000:     # pragma: no python 3 cover
-            # HTMLParser requires old-school constructor
-            HTMLParser.__init__(self)
-        else:                               # pragma: no python 2 cover
-            super(Asciifier, self).__init__(convert_charrefs=False)
-
-            # Unescape method is deprecated
-            import html
-            self.unescape = html.unescape
+        super().__init__(convert_charrefs=False)
 
         # In <head> yes/no
         self.inhead = False
 
         self.text = []  # Current document
         self.line = []  # Current (unwrapped) line
 
@@ -222,15 +206,15 @@
 
     def handle_entityref(self, name):
         # Ignore content while in head
         if self.inhead:
             return
 
         # Convert html characters
-        data = self.unescape('&' + name + ';')
+        data = html.unescape('&' + name + ';')
 
         # Convert to ascii and back to strip out non-ascii content
         data = data.encode('ascii', 'ignore').decode('ascii')
 
         # Non-empty? Then add to line
         if data:
             self.line.append(data)
```

### Comparing `myokit-1.34.0/myokit/formats/latex/__init__.py` & `myokit-1.35.0/myokit/formats/cpp/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 #
-# Provides latex export
+# Provides C++ support
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
+import myokit.formats.ansic
 
-from ._exporter import PdfExporter, PosterExporter
-from ._ewriter import LatexExpressionWriter
-
-_exporters = {
-    'latex-article': PdfExporter,
-    'latex-poster': PosterExporter,
-}
-
-
-def exporters():
-    """
-    Returns a dict of all exporters available in this module.
-    """
-    return dict(_exporters)
+from ._ewriter import CppExpressionWriter
 
 
+# Importers
+# Exporters
 # Expression writers
-
 _ewriters = {
-    'latex': LatexExpressionWriter,
+    'cpp': CppExpressionWriter,
 }
 
 
 def ewriters():
     """
     Returns a dict of all expression writers available in this module.
     """
     return dict(_ewriters)
 
 
-#
 # Language keywords
-#
-# None!
+keywords = list(myokit.formats.ansic.keywords)
+# TODO Append more keywords
```

### Comparing `myokit-1.34.0/myokit/formats/latex/_ewriter.py` & `myokit-1.35.0/myokit/formats/latex/_ewriter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 #
 # Latex expression writer
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit.formats
 
 
 class LatexExpressionWriter(myokit.formats.ExpressionWriter):
     """
     This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` translates
     Myokit :class:`expressions <myokit.Expression>` to their Tex equivalent.
     """
     def __init__(self):
-        super(LatexExpressionWriter, self).__init__()
+        super().__init__()
 
         # Default time variable
         self._time = None
         self.set_time_variable_name()
 
         # Default lhs function
         def fhls(lhs):
```

### Comparing `myokit-1.34.0/myokit/formats/latex/_exporter.py` & `myokit-1.35.0/myokit/formats/latex/_exporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 #
 # Exports model definitions to Latex files.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 
 import myokit
+
 from ._ewriter import LatexExpressionWriter
 
 
 class PdfExporter(myokit.formats.Exporter):
     """
     This :class:`Exporter <myokit.formats.Exporter>` exports model equations to
     a simple latex document.
     """
     def __init__(self):
-        super(PdfExporter, self).__init__()
+        super().__init__()
 
     def _clean(self, text):
         """
         Cleans some text for use in latex.
         """
         return text.replace('_', '\_')
 
@@ -107,15 +105,15 @@
 class PosterExporter(myokit.formats.Exporter):
     """
     This :class:`Exporter <myokit.formats.Exporter>` exports model equations to
     a terrifying poster format, designed to strike fear into the heart of its
     beholders.
     """
     def __init__(self):
-        super(PosterExporter, self).__init__()
+        super().__init__()
 
     def post_export_info(self):
         return '\n'.join((
             'To create a pdf using pdflatex::',
             '',
             '  pdflatex filename.tex',
             '',
```

### Comparing `myokit-1.34.0/myokit/formats/mathml/_ewriter.py` & `myokit-1.35.0/myokit/formats/mathml/_ewriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 #
 # MathML expression writer
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from lxml import etree
 
 import myokit.formats
 
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
-
 
 class MathMLExpressionWriter(myokit.formats.ExpressionWriter):
     """
     This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` translates
     Myokit :class:`expressions <myokit.Expression>` to Content MathML or
     Presentation MathML.
     """
     def __init__(self):
-        super(MathMLExpressionWriter, self).__init__()
+        super().__init__()
 
         # Default mode
         self._pres = False
 
         # Default lhs conversion function
         def flhs(lhs):
             var = lhs.var()
-            if isinstance(var, basestring):
+            if isinstance(var, str):
                 # This can happen with time variable of derivative if the
                 # proper variable isn't set!
                 return var
             return var.qname()
         self._flhs = flhs
 
         # Default number-to-string conversion function (outputs e.g. "1.0")
```

### Comparing `myokit-1.34.0/myokit/formats/mathml/_parser.py` & `myokit-1.35.0/myokit/formats/mathml/_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 #
 # Converts MathML to Myokit expressions, using an ElementTree implementation.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
+
 from myokit.formats.xml import split
 
 
 def parse_mathml_string(s):
     """
     Parses a MathML string that should contain a single expression.
     """
@@ -59,18 +57,18 @@
     def __init__(self, message, element=None):
         if element is not None:
             try:    # pragma: no cover
                 line = str(element.sourceline)
                 message = 'Error on line ' + line + '. ' + message
             except AttributeError:
                 pass
-        super(MathMLError, self).__init__(message)
+        super().__init__(message)
 
 
-class MathMLParser(object):
+class MathMLParser:
     """
     Parses MathML expressions into :class:`myokit.Expression` objects.
 
     Arguments:
 
     ``name_factory``
         A callable with arguments ``(name_as_string, element)`` that returns
```

### Comparing `myokit-1.34.0/myokit/formats/matlab/__init__.py` & `myokit-1.35.0/myokit/formats/matlab/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Provides Matlab/Octave support
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from ._exporter import MatlabExporter
 from ._ewriter import MatlabExpressionWriter
 
 
 # Importers
 # Exporters
 _exporters = {
```

### Comparing `myokit-1.34.0/myokit/formats/matlab/_ewriter.py` & `myokit-1.35.0/myokit/formats/stan/_ewriter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 #
-# Matlab expression writer and keywords
+# Stan expression writer and keywords
+#
+# cell.stan:: This will become the stan model definition file
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
+import myokit
 
 from myokit.formats.python import PythonExpressionWriter
 
 
-class MatlabExpressionWriter(PythonExpressionWriter):
+class StanExpressionWriter(PythonExpressionWriter):
     """
-    This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` translates
-    Myokit :class:`expressions <myokit.Expression>` to a Matlab syntax.
+    This:class:`ExpressionWriter <myokit.formats.ExpressionWriter>` translates
+    Myokit:class:`expressions <myokit.Expression>` to a Stan syntax.
     """
     def __init__(self):
-        super(MatlabExpressionWriter, self).__init__()
+        super().__init__()
         self._function_prefix = ''
-        self._fcond = 'ifthenelse'
+
+        self._fcond = None
+        self.set_condition_function('ifthenelse')
 
     def set_condition_function(self, func=None):
         """
         Sets a function name to use for if statements
 
         By setting func to None you can revert back to the default behavior
          (the ternary operator). Any other value will be interpreted as the
@@ -38,42 +41,42 @@
     #def _ex_prefix_minus(self, e):
     #def _ex_plus(self, e):
     #def _ex_minus(self, e):
     #def _ex_multiply(self, e):
     #def _ex_divide(self, e):
 
     def _ex_quotient(self, e):
-        # Round towards minus infinity
-        return 'floor(' + self._ex_infix(e, '/') + ')'
+        # Use floor to round towards minus infinity
+        return self.ex(myokit.Floor(myokit.Divide(e[0], e[1])))
 
     def _ex_remainder(self, e):
-        # Uses the round-towards-minus-infinity convention!
-        return 'mod(' + self.ex(e[0]) + ', ' + self.ex(e[1]) + ')'
+        # fmod uses correct convention
+        return self._ex_function(e, 'fmod')
 
     def _ex_power(self, e):
         return self._ex_infix(e, '^')
 
     #def _ex_sqrt(self, e):
-    #    Ignore imaginary part
-    #    return 'real(' + self._ex_function(e, 'sqrt') + ')'
     #def _ex_sin(self, e):
     #def _ex_cos(self, e):
     #def _ex_tan(self, e):
     #def _ex_asin(self, e):
     #def _ex_acos(self, e):
     #def _ex_atan(self, e):
     #def _ex_exp(self, e):
 
     def _ex_log(self, e):
         if len(e) == 1:
             return self._ex_function(e, 'log')
         else:
             return '(log(' + self.ex(e[0]) + ') / log(' + self.ex(e[1]) + '))'
 
-    #def _ex_log10(self, e):
+    def _ex_log10(self, e):
+        return 'log10(' + self.ex(e[0]) + ')'
+
     #def _ex_floor(self, e):
     #def _ex_ceil(self, e):
 
     def _ex_abs(self, e):
         return self._ex_function(e, 'abs')
 
     def _ex_not(self, e):
@@ -89,24 +92,19 @@
     def _ex_and(self, e):
         return self._ex_infix_condition(e, '&&')
 
     def _ex_or(self, e):
         return self._ex_infix_condition(e, '||')
 
     def _ex_if(self, e):
-        return '%s(%s, %s, %s)' % (
-            self._fcond, self.ex(e._i), self.ex(e._t), self.ex(e._e))
+        return ('(' + self.ex(e._i) + ' ? ' + self.ex(e._t) + ' : ' +
+                self.ex(e._e) + ')')
 
     def _ex_piecewise(self, e):
         s = []
         n = len(e._i)
         for i in range(0, n):
-            s.append(self._fcond)
-            s.append('(')
-            s.append(self.ex(e._i[i]))
-            s.append(', ')
-            s.append(self.ex(e._e[i]))
-            s.append(', ')
+            s.append('(%s ? %s : ' % (self.ex(e._i[i]), self.ex(e._e[i])))
         s.append(self.ex(e._e[n]))
         s.append(')' * n)
         return ''.join(s)
```

### Comparing `myokit-1.34.0/myokit/formats/matlab/_exporter.py` & `myokit-1.35.0/myokit/formats/matlab/_exporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Exports to matlab/octave
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 
 import myokit.formats
 
 
 class MatlabExporter(myokit.formats.TemplatedRunnableExporter):
     """
```

### Comparing `myokit-1.34.0/myokit/formats/matlab/template/constants.m` & `myokit-1.35.0/myokit/formats/matlab/template/constants.m`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/matlab/template/main.m` & `myokit-1.35.0/myokit/formats/matlab/template/main.m`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/matlab/template/model.m` & `myokit-1.35.0/myokit/formats/matlab/template/model.m`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/opencl/__init__.py` & `myokit-1.35.0/myokit/formats/opencl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Provides an export to OpenCL
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from ._exporter import OpenCLExporter, OpenCLRLExporter
 from ._ewriter import OpenCLExpressionWriter
 from myokit.formats import ansic
 
 
 # Importers
 # Exporters
```

### Comparing `myokit-1.34.0/myokit/formats/opencl/_ewriter.py` & `myokit-1.35.0/myokit/formats/opencl/_ewriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 #
 # OpenCL expression writer
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
+
 from myokit.formats.python import PythonExpressionWriter
 
 
 class OpenCLExpressionWriter(PythonExpressionWriter):
     """
     This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` translates
     Myokit :class:`expressions <myokit.Expression>` to OpenCL syntax.
     """
     def __init__(self, precision=myokit.SINGLE_PRECISION, native_math=True):
-        super(OpenCLExpressionWriter, self).__init__()
+        super().__init__()
         self._function_prefix = ''
         self._sp = (precision == myokit.SINGLE_PRECISION)
         self._nm = bool(native_math)
 
     def _exc(self, e):
         """Returns ``ex(e)`` if ``e`` is a Condition, else ``ex(e != 0)``."""
         if isinstance(e, myokit.Condition):
```

### Comparing `myokit-1.34.0/myokit/formats/opencl/_exporter.py` & `myokit-1.35.0/myokit/formats/opencl/_exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Exports to Ansi-C using OpenCL for parallelization
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 
 import myokit.formats
 
 
 class OpenCLExporter(myokit.formats.TemplatedRunnableExporter):
     """
```

### Comparing `myokit-1.34.0/myokit/formats/opencl/template/cable.c` & `myokit-1.35.0/myokit/formats/opencl/template/cable.c`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/opencl/template/kernel.cl` & `myokit-1.35.0/myokit/formats/opencl/template/kernel.cl`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/opencl/template/minilog.py` & `myokit-1.35.0/myokit/formats/opencl/template/minilog.py`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/opencl/template/plot.py` & `myokit-1.35.0/myokit/formats/opencl/template/plot.py`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/python/__init__.py` & `myokit-1.35.0/myokit/formats/python/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Provides Python support
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from ._exporter import PythonExporter
 from ._ewriter import PythonExpressionWriter, NumPyExpressionWriter
 
 # Importers
 # Exporters
 
 _exporters = {
```

### Comparing `myokit-1.34.0/myokit/formats/python/_ewriter.py` & `myokit-1.35.0/myokit/formats/python/_ewriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #
 # Python expression writer and keywords
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit.formats
 
 
 class PythonExpressionWriter(myokit.formats.ExpressionWriter):
     """
     This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` translates
     Myokit :class:`expressions <myokit.Expression>` to their Python
     equivalent.
     """
     def __init__(self):
-        super(PythonExpressionWriter, self).__init__()
+        super().__init__()
 
         self._flhs = None
         self.set_lhs_function(lambda v: str(v))
 
         self._function_prefix = 'math.'
 
     def set_lhs_function(self, f):
@@ -188,15 +185,15 @@
 class NumPyExpressionWriter(PythonExpressionWriter):
     """
     This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` translates
     Myokit :class:`expressions <myokit.Expression>` to Python expressions
     intended for use in NumPy arrays.
     """
     def __init__(self):
-        super(NumPyExpressionWriter, self).__init__()
+        super().__init__()
         self._function_prefix = 'numpy.'
     #def _ex_name(self, e):
     #def _ex_derivative(self, e):
     #def _ex_number(self, e):
     #def _ex_prefix_plus(self, e):
     #def _ex_prefix_minus(self, e):
     #def _ex_plus(self, e):
```

### Comparing `myokit-1.34.0/myokit/formats/python/_exporter.py` & `myokit-1.35.0/myokit/formats/python/_exporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Exports to plain python
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 
 import myokit.formats
 
 
 class PythonExporter(myokit.formats.TemplatedRunnableExporter):
     """
```

### Comparing `myokit-1.34.0/myokit/formats/python/template/sim.py` & `myokit-1.35.0/myokit/formats/python/template/sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 <?
 # Generate class per component
 for comp in components:
     names = c(comp)
     w.set_lhs_function(lambda x: v(x, comp))
 
     ?>
-class <?= names[1] ?>(object):
+class <?= names[1] ?>:
     def __init__(self):
 <?
     for var in comp.variables(deep=True):
         print(tab2 + v(var, comp) + ' = None')
         if var.is_state():
             print(tab2 + v(var.lhs(), comp) + ' = None')
     ?>
@@ -114,15 +114,15 @@
             print(tab2 + e(eq))
     if not printed:
         print(tab2 + 'pass')
 ?>
 #
 # Engine component
 #
-class Engine(object):
+class Engine:
     """
     Calculates the derivatives in the current state
     """
     def __init__(self):
         self.pace = 0.0
         self.time = 0.0
 <?
@@ -209,18 +209,18 @@
     init()
     engine.update()
     print_state()
 
 #
 # Pacing
 #
-class Protocol(object):
+class Protocol:
     """ Holds an ordered set of ProtocolEvent objects """
     def __init__(self):
-        super(Protocol, self).__init__()
+        super().__init__()
         self.head = None
     def add(self, e):
         """ Schedules an event """
         if self.head is None:
             self.head = e
             return
         if e.start < self.head.start:
@@ -234,17 +234,19 @@
         f.next = e
     def pop(self):
         """ Returns the next event """
         e = self.head
         if self.head is not None:
             self.head = self.head.next
         return e
-class ProtocolEvent(object):
+
+
+class ProtocolEvent:
     def __init__(self, level, start, duration, period=0, multiplier=0):
-        super(ProtocolEvent, self).__init__()
+        super().__init__()
         self.level = float(level)
         self.start = float(start)
         self.duration = float(duration)
         if self.duration <= 0:
             raise Exception('Duration must be greater than zero')
         self.period = float(period)
         if self.period < 0:
@@ -252,14 +254,15 @@
         self.multiplier = int(multiplier)
         if self.multiplier < 0:
             raise Exception('Multiplier must be zero or greater')
         if self.period == 0 and self.multiplier > 0:
             raise Exception('Non-periodic event cannot occur more than once')
         self.next = None
 
+
 def pacing_protocol():
     pacing = Protocol()
 <?
 nxt = protocol.head()
 while nxt:
     x = [
         nxt.level(),
@@ -373,18 +376,15 @@
         try:
             init()
             data = beat(small, large)
             done = True
         except ArithmeticError as e:
             print('Arithmetic error occurred')
             y = 'Continue with smaller stepsize? (y/n): '
-            try:
-                y = raw_input(y)    # Python 2
-            except NameError:
-                y = input(y)        # Python 3
+            y = input(y)
             if y.lower()[0:1] == 'y':
                 small /= 2
                 large /= 2
                 go = True
     if done:
         print('Showing result...')
         x = []
```

### Comparing `myokit-1.34.0/myokit/formats/sbml/_api.py` & `myokit-1.35.0/myokit/formats/sbml/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# SBML API
+#
+# This file is part of Myokit.
+# See http://myokit.org for copyright, sharing, and licensing details.
+#
 import collections
 import warnings
 import re
 
 import myokit
 import myokit.units
 
@@ -12,15 +18,15 @@
 _SBML_TIME = 'http://www.sbml.org/sbml/symbols/time'
 
 
 class SBMLError(Exception):
     """Raised if something goes wrong when working with an SBML model."""
 
 
-class Quantity(object):
+class Quantity:
     """
     Base class for anything that has a numerical value in an SBML model, and
     can be set by rules, reactions, or initial assignments.
     """
     def __init__(self):
 
         # Expression for initial value (myokit.Expression)
@@ -85,15 +91,15 @@
         """
         Returns a :class:`myokit.Expression` for this quantity's value, or
         ``None`` if not set.
         """
         return self._value
 
 
-class CSymbolVariable(object):
+class CSymbolVariable:
     """
     Represents a CSymbol that can appear in SBML expressions, but which has a
     predetermind value and/or meaning, e.g. "time".
     """
     def __init__(self, definition_url):
         self._definition_url = str(definition_url)
 
@@ -118,15 +124,15 @@
     ``model``
         The :class:`myokit.formats.sbml.Model` this compartment is in.
     ``sid``
         This compartment's SId.
 
     """
     def __init__(self, model, sid):
-        super(Compartment, self).__init__()
+        super().__init__()
 
         if not isinstance(model, Model):
             raise SBMLError(
                 '<' + str(model) + '> needs to be an instance of'
                 ' myokit.formats.sbml.Model.')
 
         self._model = model
@@ -181,15 +187,15 @@
         """
         return self._spatial_dimensions
 
     def __str__(self):
         return '<Compartment ' + self._sid + '>'
 
 
-class Model(object):
+class Model:
     """
     Represents a model in SBML.
 
     Arguments:
 
     ``name``
         A user-friendly name for this model.
@@ -577,15 +583,15 @@
     ``model``
         The model this parameter is in.
     ``sid``
         This parameter's SId.
 
     """
     def __init__(self, model, sid):
-        super(Parameter, self).__init__()
+        super().__init__()
 
         if not isinstance(model, Model):
             raise SBMLError(
                 '<' + str(model) + '> needs to be an instance of'
                 ' myokit.formats.sbml.Model.')
 
         self._model = model
@@ -608,15 +614,15 @@
         return '<Parameter ' + self._sid + '>'
 
     def units(self):
         """Returns the units this parameter is in, or ``None`` if not set."""
         return self._units
 
 
-class Reaction(object):
+class Reaction:
     """
     Represents an SBML reaction; to create a reaction use
     :meth:`Model.add_reaction()`.
 
     Arguments:
 
     ``model``
@@ -768,15 +774,15 @@
     ``is_constant``
         Whether or not this species is constant.
     ``is_boundary``
         Whether or not this species is at the boundary of a reaction.
 
     """
     def __init__(self, compartment, sid, is_amount, is_constant, is_boundary):
-        super(Species, self).__init__()
+        super().__init__()
 
         if not isinstance(compartment, Compartment):
             raise SBMLError(
                 '<' + compartment + '> needs to be instance of'
                 ' myokit.formats.sbml.Compartment')
         if not isinstance(is_amount, bool):
             raise SBMLError(
@@ -910,15 +916,15 @@
     the species' stoichiometry.
     """
     REACTANT = 0
     PRODUCT = 1
     MODIFIER = 2
 
     def __init__(self, species, sid=None):
-        super(SpeciesReference, self).__init__()
+        super().__init__()
 
         if not isinstance(species, Species):
             raise SBMLError(
                 '<' + species + '> needs to be instance of'
                 ' myokit.formats.sbml.Species')
 
         self._species = species
@@ -932,19 +938,19 @@
         """Returns this species reference's SId, or ``None`` if not set."""
         return self._sid
 
     def __str__(self):
         return '<SpeciesReference ' + self._sid + '>'
 
 
-class ModifierSpeciesReference(object):
+class ModifierSpeciesReference:
     """Represents a reference to a modifier species in an SBML reaction."""
 
     def __init__(self, species, sid=None):
-        super(ModifierSpeciesReference, self).__init__()
+        super().__init__()
 
         if not isinstance(species, Species):
             raise SBMLError(
                 '<' + species + '> needs to be instance of'
                 ' myokit.formats.sbml.Species')
 
         self._species = species
@@ -967,15 +973,15 @@
     underscore.
     """
     if name[:1] == '_':
         name = 'underscore' + name
     return name
 
 
-class _MyokitConverter(object):
+class _MyokitConverter:
     """
     Converts SBML Models to Myokit models.
     """
     @staticmethod
     def convert(sbml_model):
         """Converts the given SBML model to a Myokit model."""
```

### Comparing `myokit-1.34.0/myokit/formats/sbml/_importer.py` & `myokit-1.35.0/myokit/formats/sbml/_importer.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,30 +3,27 @@
 # Only partial SBML support (Based on SBML level 3 version 2) is provided.
 # The file format specifications can be found here
 # http://sbml.org/Documents/Specifications.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit.formats
 
 
 class SBMLImporter(myokit.formats.Importer):
     """
     This :class:`Importer <myokit.formats.Importer>` loads model definitions
     from files in SBML format.
 
     Not all SBML features are supported, see
     :class:`myokit.formats.sbml.SBMLParser`.
     """
     def __init__(self):
-        super(SBMLImporter, self).__init__()
+        super().__init__()
 
     def supports_model(self):
         """Returns ``True``."""
         return True
 
     def model(self, path):
         """
```

### Comparing `myokit-1.34.0/myokit/formats/sbml/_parser.py` & `myokit-1.35.0/myokit/formats/sbml/_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 # Only partial SBML support (based on SBML level 3 version 2) is provided.
 # The SBML file format specifications can be found here
 # http://sbml.org/Documents/Specifications.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import re
 import warnings
 
 from lxml import etree
 
 import myokit
 import myokit.units
@@ -72,18 +69,18 @@
     def __init__(self, message, element=None):
         if element is not None:
             try:
                 line = str(element.sourceline)
                 message = 'Error on line ' + line + '. ' + message
             except AttributeError:  # pragma: no cover
                 pass
-        super(SBMLParsingError, self).__init__(message)
+        super().__init__(message)
 
 
-class SBMLParser(object):
+class SBMLParser:
     """
     Parses SBML models, creating an SBML Model structure that can be converted
     to a :class:`myokit.Model` object.
 
     Support notes:
 
     - SBML older than Level 2 version 1 is unlikely to work.
```

### Comparing `myokit-1.34.0/myokit/formats/stan/__init__.py` & `myokit-1.35.0/myokit/formats/stan/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Provides Stan support (see: http://mc-stan.org/)
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from ._exporter import StanExporter
 from ._ewriter import StanExpressionWriter
 
 
 # Importers
 # Exporters
 _exporters = {
```

### Comparing `myokit-1.34.0/myokit/formats/stan/_ewriter.py` & `myokit-1.35.0/myokit/formats/ansic/_ewriter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 #
-# Stan expression writer and keywords
-#
-# cell.stan:: This will become the stan model definition file
+# Ansi-C expression writer
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
+
 from myokit.formats.python import PythonExpressionWriter
 
 
-class StanExpressionWriter(PythonExpressionWriter):
+class AnsiCExpressionWriter(PythonExpressionWriter):
     """
-    This:class:`ExpressionWriter <myokit.formats.ExpressionWriter>` translates
-    Myokit:class:`expressions <myokit.Expression>` to a Stan syntax.
+    This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` writes
+    equations for variables in a C-style syntax.
     """
     def __init__(self):
-        super(StanExpressionWriter, self).__init__()
+        super().__init__()
         self._function_prefix = ''
-
         self._fcond = None
-        self.set_condition_function('ifthenelse')
 
     def set_condition_function(self, func=None):
         """
         Sets a function name to use for if statements
 
         By setting func to None you can revert back to the default behavior
          (the ternary operator). Any other value will be interpreted as the
-         name of a function taking arguments (condition, value_if_true,
+         name of a C function taking arguments (condition, value_if_true,
          value_if_false).
         """
         self._fcond = func
 
     #def _ex_name(self, e):
     #def _ex_derivative(self, e):
     #def _ex_number(self, e):
@@ -43,47 +37,48 @@
     #def _ex_prefix_minus(self, e):
     #def _ex_plus(self, e):
     #def _ex_minus(self, e):
     #def _ex_multiply(self, e):
     #def _ex_divide(self, e):
 
     def _ex_quotient(self, e):
-        # Use floor to round towards minus infinity
+        # Note that this _must_ round towards minus infinity!
+        # See myokit.Quotient !
         return self.ex(myokit.Floor(myokit.Divide(e[0], e[1])))
 
     def _ex_remainder(self, e):
-        # fmod uses correct convention
-        return self._ex_function(e, 'fmod')
+        # Note that this _must_ use the same round-to-neg-inf convention as
+        # myokit.Quotient! Implementation below is consistent with Python
+        # convention:
+        return self.ex(myokit.Minus(
+            e[0], myokit.Multiply(e[1], myokit.Quotient(e[0], e[1]))))
 
     def _ex_power(self, e):
-        return self._ex_infix(e, '^')
+        return 'pow(' + self.ex(e[0]) + ', ' + self.ex(e[1]) + ')'
 
     #def _ex_sqrt(self, e):
     #def _ex_sin(self, e):
     #def _ex_cos(self, e):
     #def _ex_tan(self, e):
     #def _ex_asin(self, e):
     #def _ex_acos(self, e):
     #def _ex_atan(self, e):
     #def _ex_exp(self, e):
 
     def _ex_log(self, e):
         if len(e) == 1:
             return self._ex_function(e, 'log')
-        else:
-            return '(log(' + self.ex(e[0]) + ') / log(' + self.ex(e[1]) + '))'
-
-    def _ex_log10(self, e):
-        return 'log10(' + self.ex(e[0]) + ')'
+        return '(log(' + self.ex(e[0]) + ') / log(' + self.ex(e[1]) + '))'
 
+    #def _ex_log10(self, e):
     #def _ex_floor(self, e):
     #def _ex_ceil(self, e):
 
     def _ex_abs(self, e):
-        return self._ex_function(e, 'abs')
+        return self._ex_function(e, 'fabs')
 
     def _ex_not(self, e):
         return '!(' + self.ex(e[0]) + ')'
 
     #def _ex_equal(self, e):
     #def _ex_not_equal(self, e):
     #def _ex_more(self, e):
@@ -94,19 +89,30 @@
     def _ex_and(self, e):
         return self._ex_infix_condition(e, '&&')
 
     def _ex_or(self, e):
         return self._ex_infix_condition(e, '||')
 
     def _ex_if(self, e):
-        return ('(' + self.ex(e._i) + ' ? ' + self.ex(e._t) + ' : ' +
-                self.ex(e._e) + ')')
+        ite = (self.ex(e._i), self.ex(e._t), self.ex(e._e))
+        if self._fcond is None:
+            return '(%s ? %s : %s)' % ite
+        else:
+            return '%s(%s, %s, %s)' % ((self._fcond,) + ite)
 
     def _ex_piecewise(self, e):
         s = []
         n = len(e._i)
-        for i in range(0, n):
-            s.append('(%s ? %s : ' % (self.ex(e._i[i]), self.ex(e._e[i])))
-        s.append(self.ex(e._e[n]))
-        s.append(')' * n)
+        if self._fcond is None:
+            for i in range(0, n):
+                s.append('(%s ? %s : ' % (self.ex(e._i[i]), self.ex(e._e[i])))
+            s.append(self.ex(e._e[n]))
+            s.append(')' * n)
+        else:
+            for i in range(0, n):
+                s.append(
+                    '%s(%s, %s, ' % (
+                        self._fcond, self.ex(e._i[i]), self.ex(e._e[i])))
+            s.append(self.ex(e._e[n]))
+            s.append(')' * n)
         return ''.join(s)
```

### Comparing `myokit-1.34.0/myokit/formats/stan/_exporter.py` & `myokit-1.35.0/myokit/formats/stan/_exporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Exports to stan (a package for statistical inference)
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 
 import myokit.formats
 
 
 class StanExporter(myokit.formats.TemplatedRunnableExporter):
     """
@@ -57,15 +54,15 @@
             A list of variables or variable names, specifying the model
             variables to be estimated by stan.
         ``output``
             A single variable to be used as the model output (for example an
             ion current).
 
         """
-        super(StanExporter, self).runnable(
+        super().runnable(
             path, model, protocol, parameters, output)
 
     def _vars(self, model, protocol, parameters, output):
         import myokit.formats.stan as stan
 
         # Check parameter list
         if parameters is None:
```

### Comparing `myokit-1.34.0/myokit/formats/stan/template/cell.stan` & `myokit-1.35.0/myokit/formats/stan/template/cell.stan`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/formats/sympy/__init__.py` & `myokit-1.35.0/myokit/formats/sympy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Provides interaction with the computer algebra system Sympy
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 from ._ereader import SymPyExpressionReader
 from ._ewriter import SymPyExpressionWriter
 
 
 # Importers
 # Exporters
 # Expression writers
```

### Comparing `myokit-1.34.0/myokit/formats/sympy/_ereader.py` & `myokit-1.35.0/myokit/formats/sympy/_ereader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 #
 # Sympy expression reader
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
 import myokit.formats
 
 
-class SymPyExpressionReader(object):
+class SymPyExpressionReader:
     """
     Converts Sympy expressions to Myokit expressions.
 
     Any variable names will be resolved against the given model. If no model is
     given, string names will be used instead of myokit Variable objects.
     """
     def __init__(self, model=None):
```

### Comparing `myokit-1.34.0/myokit/formats/sympy/_ewriter.py` & `myokit-1.35.0/myokit/formats/sympy/_ewriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 #
 # SymPy expression writer
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
+import myokit.formats
 
 try:
     import sympy as sp
 except ImportError:
     pass
 
-import myokit.formats
-
 
 class SymPyExpressionWriter(myokit.formats.ExpressionWriter):
     """
     This :class:`ExpressionWriter <myokit.formats.ExpressionWriter>` converts
     Myokit :class:`expressions <myokit.Expression>` to SymPy expressions.
 
     The returned type is a SymPy object, not a string!
     """
     def __init__(self):
-        super(SymPyExpressionWriter, self).__init__()
+        super().__init__()
 
         self._flhs = None
         self.set_lhs_function(lambda lhs: str(lhs))
 
         # Import sympy again, will trigger error if can't be done.
         import sympy
         del sympy
```

### Comparing `myokit-1.34.0/myokit/formats/wcp/_wcp.py` & `myokit-1.35.0/myokit/formats/wcp/_wcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #
 # This module reads files in WCP format
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import struct
 import numpy as np
 
 import myokit
 
 # Encoding of text portions of wcp file
 _ENC = 'ascii'
 
 
-class WcpFile(object):
+class WcpFile:
     """
     Represents a read-only WinWCP file (``.wcp``), stored at the location
     pointed to by ``filepath``.
 
     Only files in the newer file format version 9 can be read. This version of
     the format was introduced in 2010. New versions of WinWCP can read older
     files and will convert them to the new format automatically when opened.
@@ -31,15 +28,14 @@
 
     WinWCP files contain a number of records ``NR``, each containing data from
     ``NC`` channels. Every channel has the same length, ``NP`` samples.
     Sampling happens at a fixed sampling rate.
     """
     def __init__(self, filepath):
         # The path to the file and its basename
-        # Ensure it's a `str` for Python2/3 compatibility
         filepath = str(filepath)
         self._filepath = os.path.abspath(filepath)
         self._filename = os.path.basename(filepath)
 
         # Records
         self._records = None
         self._channel_names = None
@@ -156,16 +152,14 @@
             # Status of signal (Accepted or rejected, as string)
             rstatus = f.read(8)
 
             # Type of recording, as string
             rtype = f.read(4)
 
             # Group number (float set by the user)
-            # Note: First argument to struct.unpack must be a str (so bytes on
-            # Python 2).
             group_number = struct.unpack(str('<f'), f.read(4))[0]
 
             # Time of recording, as float, not sure how to interpret
             rtime = struct.unpack(str('<f'), f.read(4))[0]
 
             # Sampling interval: pretty sure this should be the same as the
             # file wide one in header[b'dt']
```

### Comparing `myokit-1.34.0/myokit/formats/xml/_exporter.py` & `myokit-1.35.0/myokit/formats/xml/_exporter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Exports to a generic XML format.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 
 from lxml import etree
 
 import myokit
```

### Comparing `myokit-1.34.0/myokit/gui/datablock_viewer.py` & `myokit-1.35.0/myokit/gui/datablock_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 #
 # Qt gui for viewing DataBlock2d data files.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
+import collections
+import configparser
 import os
 import sys
-import numpy as np
 import traceback
-import collections
+
+import numpy as np
 
 import myokit
 import myokit.gui
-from myokit.gui import QtWidgets, QtGui, QtCore, Qt
 
-# ConfigParser in Python 2 and 3
-try:
-    import ConfigParser as configparser
-except ImportError:
-    import configparser
+from myokit.gui import QtWidgets, QtGui, QtCore, Qt
 
 
 # Application title
 TITLE = 'Myokit DataBlock Viewer'
 
 # Settings file
 SETTINGS_FILE = os.path.join(myokit.DIR_USER, 'DataBlockViewer.ini')
@@ -88,171 +82,199 @@
 
 class DataBlockViewer(myokit.gui.MyokitApplication):
     """
     Graphical interface for viewing DataBlock data.
     """
 
     def __init__(self, filename=None):
-        super(DataBlockViewer, self).__init__()
+        super().__init__()
         # Set application icon
         self.setWindowIcon(icon())
+
         # Set size, center
         self.resize(800, 600)
         self.setMinimumSize(600, 400)
         qr = self.frameGeometry()
-        cp = QtWidgets.QDesktopWidget().availableGeometry().center()
+        cp = QtGui.QGuiApplication.primaryScreen().availableGeometry().center()
         qr.moveCenter(cp)
         self.move(qr.topLeft())
+
         # Status bar
         self._label_cursor = QtWidgets.QLabel()
         self.statusBar().addPermanentWidget(self._label_cursor)
         self.statusBar().showMessage('Ready')
+
         # Menu bar
         self.create_menu()
+
         # Timer
         self._timer_interval = 50
         self._timer = QtCore.QTimer(self)
         self._timer.setInterval(self._timer_interval)
         self._timer.setSingleShot(False)
         self._timer.timeout.connect(self.action_next_frame)
         self._timer_paused = False
-        try:
-            self._timer.setTimerType(Qt.PreciseTimer)
-        except AttributeError:
-            pass    # Qt4 uses precise timer by default
+        self._timer.setTimerType(Qt.TimerType.PreciseTimer)
+
         # Video widget
         self._video_scene = VideoScene()
         self._video_scene.mouse_moved.connect(self.event_video_mouse_move)
         self._video_scene.single_click.connect(self.event_video_single_click)
         self._video_scene.double_click.connect(self.event_video_double_click)
         self._video_view = VideoView(self._video_scene)
         self._video_view.setMouseTracking(True)
-        self._video_view.setCursor(Qt.CrossCursor)
+        self._video_view.setCursor(Qt.CursorShape.CrossCursor)
         #self._video_view.setViewport(QtOpenGL.QGLWidget())
         self._video_pixmap = None
         self._video_item = None
         self._video_frames = None
         self._video_iframe = None
+
         # Colorbar widget
         self._colorbar_width = 20
         self._colorbar_height = 256
         self._colorbar_scene = VideoScene()
         self._colorbar_view = VideoView(self._colorbar_scene)
         self._colorbar_view.setMaximumWidth(self._colorbar_width)
         self._colorbar_pixmap = None
         self._colorbar_item = None
+
         # Video slider
-        self._slider = QtWidgets.QSlider(Qt.Horizontal)
-        self._slider.setTickPosition(QtWidgets.QSlider.NoTicks)
-        #self._slider.setTickPosition(QtWidgets.QSlider.TicksBothSides)
+        self._slider = QtWidgets.QSlider(Qt.Orientation.Horizontal)
+        self._slider.setTickPosition(QtWidgets.QSlider.TickPosition.NoTicks)
         self._slider.setSingleStep(1)
         self._slider.setMinimum(0)
         self._slider.setMaximum(0)
         self._slider.sliderPressed.connect(self.action_pause_timer)
         self._slider.sliderReleased.connect(self.action_depause_timer)
         self._slider.valueChanged.connect(self.action_set_frame)
+
         # Controls
         style = QtWidgets.QApplication.style()
+
         # Play button
-        self._play_icon_play = style.standardIcon(style.SP_MediaPlay)
-        self._play_icon_pause = style.standardIcon(style.SP_MediaPause)
+        self._play_icon_play = style.standardIcon(
+            style.StandardPixmap.SP_MediaPlay)
+        self._play_icon_pause = style.standardIcon(
+            style.StandardPixmap.SP_MediaPause)
         self._play_button = QtWidgets.QPushButton()
         self._play_button.setIcon(self._play_icon_play)
         self._play_button.pressed.connect(self.action_start_stop)
+
         # Frame indicator
         self._frame_label = QtWidgets.QLabel('Frame')
         self._frame_field = QtWidgets.QLineEdit('0')
         self._frame_field.setReadOnly(True)
         self._frame_field.setMaxLength(6)
         self._frame_field.setMaximumWidth(100)
-        self._frame_label.setAlignment(Qt.AlignRight | Qt.AlignVCenter)
+        self._frame_label.setAlignment(
+            Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignVCenter)
+
         # Time indicator
         self._time_label = QtWidgets.QLabel('Time')
         self._time_field = QtWidgets.QLineEdit('0')
         self._time_field.setReadOnly(True)
         self._time_field.setMaxLength(6)
         self._time_field.setMaximumWidth(100)
-        self._time_label.setAlignment(Qt.AlignRight | Qt.AlignVCenter)
+        self._time_label.setAlignment(
+            Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignVCenter)
+
         # Speed indicator
         self._rate_label = QtWidgets.QLabel('Delay')
         self._rate_field = QtWidgets.QLineEdit(str(self._timer_interval))
         self._rate_field.setValidator(QtGui.QIntValidator(1, 2**20, self))
         self._rate_field.editingFinished.connect(self.event_rate_changed)
         self._rate_field.setMaximumWidth(100)
-        self._rate_label.setAlignment(Qt.AlignRight | Qt.AlignVCenter)
+        self._rate_label.setAlignment(
+            Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignVCenter)
+
         # Graph controls
         self._graph_clear_button = QtWidgets.QPushButton('Clear graphs')
         self._graph_clear_button.pressed.connect(self.action_clear_graphs)
+
         # Variable selection
         self._variable_select = QtWidgets.QComboBox()
         self._variable_select.activated.connect(self.event_variable_selected)
         self._variable_select.setMinimumWidth(120)
+
         # Colormap selection
         self._colormap = next(iter(myokit.ColorMap.names()))
         self._colormap_select = QtWidgets.QComboBox()
         for cmap in myokit.ColorMap.names():
             self._colormap_select.addItem(cmap)
         self._colormap_select.activated.connect(self.event_colormap_selected)
         self._colormap_select.setMinimumWidth(120)
+
         # Control layout
         self._control_layout = QtWidgets.QHBoxLayout()
         self._control_layout.addWidget(self._play_button)
         self._control_layout.addWidget(self._frame_label)
         self._control_layout.addWidget(self._frame_field)
         self._control_layout.addWidget(self._time_label)
         self._control_layout.addWidget(self._time_field)
         self._control_layout.addWidget(self._rate_label)
         self._control_layout.addWidget(self._rate_field)
         self._control_layout.addWidget(self._graph_clear_button)
         self._control_layout.addWidget(self._variable_select)
         self._control_layout.addWidget(self._colormap_select)
+
         # Graph area
         self._graph_area = GraphArea()
         self._graph_area.mouse_moved.connect(self.event_graph_mouse_move)
         self._graph_area.setMouseTracking(True)
-        self._graph_area.setCursor(Qt.CrossCursor)
+        self._graph_area.setCursor(Qt.CursorShape.CrossCursor)
+
         # Video and colorbar layout
         self._video_plus_layout = QtWidgets.QHBoxLayout()
         self._video_plus_layout.addWidget(self._video_view)
         self._video_plus_layout.addWidget(self._colorbar_view)
+
         # Video Layout
         self._video_layout = QtWidgets.QVBoxLayout()
         self._video_layout.addLayout(self._video_plus_layout)
         self._video_layout.addWidget(self._slider)
         self._video_layout.addLayout(self._control_layout)
         self._video_widget = QtWidgets.QWidget()
         self._video_widget.setLayout(self._video_layout)
+
         # Central layout
-        self._central_widget = QtWidgets.QSplitter(Qt.Vertical)
+        self._central_widget = QtWidgets.QSplitter(Qt.Orientation.Vertical)
         self._central_widget.addWidget(self._video_widget)
         self._central_widget.addWidget(self._graph_area)
         self.setCentralWidget(self._central_widget)
+
         # Current path, current file, recent files
         self._path = QtCore.QDir.currentPath()
         self._file = None
         self._recent_files = []
+
         # Current data block, display variable
         self._data = None
         self._variable = None
+
         # Load settings from ini file
         self.load_config()
         self.update_window_title()
+
         # Set controls to correct values
         self._colormap_select.setCurrentIndex(self._colormap_select.findText(
             self._colormap))
         self._rate_field.setText(str(self._timer_interval))
         self._timer.setInterval(self._timer_interval)
+
         # Pause video playback during resize
         self._resize_timer = QtCore.QTimer()
         self._resize_timer.timeout.connect(self._resize_timeout)
         self._video_view.resize_event.connect(self._resize_started)
         self._colorbar_view.resize_event.connect(self._resize_started)
+
         # Attempt to load selected file
         if filename and os.path.isfile(filename):
             self.load_data_file(filename)
+
         # Focus on play button
         self._play_button.setFocus()
 
     def action_about(self):
         """
         Displays the about dialog.
         """
@@ -302,15 +324,16 @@
             data = self._data.get2d(self._variable)
             lower = np.min(data)
             upper = np.max(data)
             # Create image
             nx = 200
             ny = 800
             image = myokit.ColorMap.image(self._colormap, nx, ny)
-            image = QtGui.QImage(image, nx, ny, QtGui.QImage.Format_ARGB32)
+            image = QtGui.QImage(
+                image, nx, ny, QtGui.QImage.Format.Format_ARGB32)
             painter = QtGui.QPainter(image)
             painter.drawText(10, 15, str(upper))
             painter.drawText(10, ny - 5, str(lower))
             painter.end()
             # Save
             image.save(fname, ext)
 
@@ -356,15 +379,16 @@
                 QtWidgets.QMessageBox.warning(
                     self, TITLE,
                     '<h1>Image type not recognized.</h1>'
                     '<p>Unknown image type "' + str(ext) + '".</p>')
                 return
             nt, ny, nx = self._data.shape()
             image = self._video_frames[self._video_iframe]
-            image = QtGui.QImage(image, nx, ny, QtGui.QImage.Format_ARGB32)
+            image = QtGui.QImage(
+                image, nx, ny, QtGui.QImage.Format.Format_ARGB32)
             image.save(fname, ext)
 
     def action_extract_graphs(self):
         """
         Extracts the currently displayed graphs to a csv file.
         """
         if self._data is None:
@@ -460,15 +484,16 @@
         self._colormap_select.setCurrentIndex(self._colormap_select.findText(
             self._colormap))
         if self._data is not None:
             # Update colorbar
             nx = self._colorbar_width
             ny = self._colorbar_height
             image = myokit.ColorMap.image(self._colormap, nx, ny)
-            image = QtGui.QImage(image, nx, ny, QtGui.QImage.Format_ARGB32)
+            image = QtGui.QImage(
+                image, nx, ny, QtGui.QImage.Format.Format_ARGB32)
             self._colorbar_pixmap.convertFromImage(image)
             self._colorbar_item.setPixmap(self._colorbar_pixmap)  # qt5
             self.action_set_variable(self._variable)
 
     def action_set_variable(self, var):
         """
         Loads the variable specified by the name ``var`` into the main display.
@@ -500,15 +525,16 @@
             if self._slider.value() != frame:
                 self._slider.setValue(self._video_iframe)
             # Update frame/time information
             self._frame_field.setText(str(frame))
             self._time_field.setText(str(self._data.time()[frame]))
             # Update scene
             image = self._video_frames[self._video_iframe]
-            image = QtGui.QImage(image, nx, ny, QtGui.QImage.Format_ARGB32)
+            image = QtGui.QImage(
+                image, nx, ny, QtGui.QImage.Format.Format_ARGB32)
             self._video_pixmap.convertFromImage(image)
             self._video_item.setPixmap(self._video_pixmap)   # qt5
         # Update graph area
         self._graph_area.set_position(self._video_iframe)
 
     def action_start_timer(self):
         """
@@ -536,74 +562,73 @@
         """
         Creates this widget's menu.
         """
         self._menu = self.menuBar()
         # File menu
         self._menu_file = self._menu.addMenu('&File')
         # File > Open
-        self._tool_open = QtWidgets.QAction('&Open', self)
+        self._tool_open = QtGui.QAction('&Open', self)
         self._tool_open.setShortcut('Ctrl+O')
         self._tool_open.setStatusTip('Open a DataLog for inspection.')
         self._tool_open.setIcon(QtGui.QIcon.fromTheme('document-open'))
         self._tool_open.triggered.connect(self.action_open)
         self._menu_file.addAction(self._tool_open)
         # File > ----
         self._menu_file.addSeparator()
         # File > Recent files
         self._recent_file_tools = []
         for i in range(N_RECENT_FILES):
-            tool = QtWidgets.QAction(self, visible=False)
+            tool = QtGui.QAction(self, visible=False)
             tool.triggered.connect(self.action_recent_file)
             self._recent_file_tools.append(tool)
             self._menu_file.addAction(tool)
         # File > ----
         self._menu_file.addSeparator()
         # File > Quit
-        self._tool_exit = QtWidgets.QAction('&Quit', self)
+        self._tool_exit = QtGui.QAction('&Quit', self)
         self._tool_exit.setShortcut('Ctrl+Q')
         self._tool_exit.setStatusTip('Exit application.')
         self._tool_exit.setIcon(QtGui.QIcon.fromTheme('application-exit'))
         self._tool_exit.triggered.connect(self.close)
         self._menu_file.addAction(self._tool_exit)
         # Data menu
         self._menu_data = self._menu.addMenu('&Data')
         # Data > Extract frame
-        self._tool_exframe = QtWidgets.QAction('Extract &frame', self)
+        self._tool_exframe = QtGui.QAction('Extract &frame', self)
         self._tool_exframe.setStatusTip(
             'Extract the current frame as csv file.')
         self._tool_exframe.triggered.connect(self.action_extract_frame)
         self._menu_data.addAction(self._tool_exframe)
         # Data > Extract graphs
-        self._tool_exgraph = QtWidgets.QAction('Extract &graphs', self)
+        self._tool_exgraph = QtGui.QAction('Extract &graphs', self)
         self._tool_exgraph.setStatusTip('Extract the current graphs.')
         self._tool_exgraph.triggered.connect(self.action_extract_graphs)
         self._menu_data.addAction(self._tool_exgraph)
         # Data > ----
         self._menu_data.addSeparator()
         # Data > Extract frame as image
-        self._tool_imgframe = QtWidgets.QAction('Save frame as &image', self)
+        self._tool_imgframe = QtGui.QAction('Save frame as &image', self)
         self._tool_imgframe.setStatusTip(
             'Save the current frame as an image file.')
         self._tool_imgframe.triggered.connect(self.action_extract_frame_image)
         self._menu_data.addAction(self._tool_imgframe)
         # Data > Extract colormap as image
-        self._tool_imgcolor = QtWidgets.QAction(
-            'Save &colormap as image', self)
+        self._tool_imgcolor = QtGui.QAction('Save &colormap as image', self)
         self._tool_imgcolor.setStatusTip('Save the colormap as an image file.')
         self._tool_imgcolor.triggered.connect(
             self.action_extract_colormap_image)
         self._menu_data.addAction(self._tool_imgcolor)
         # Help menu
         self._menu_help = self._menu.addMenu('&Help')
         # Help > About
-        self._tool_about = QtWidgets.QAction('&About', self)
+        self._tool_about = QtGui.QAction('&About', self)
         self._tool_about.setStatusTip('View information about this program.')
         self._tool_about.triggered.connect(self.action_about)
         self._menu_help.addAction(self._tool_about)
-        self._tool_license = QtWidgets.QAction('&License', self)
+        self._tool_license = QtGui.QAction('&License', self)
         self._tool_license.setStatusTip('View this program\'s license info.')
         self._tool_license.triggered.connect(self.action_license)
         self._menu_help.addAction(self._tool_license)
 
     def display_exception(self):
         """
         Displays the last exception.
@@ -673,15 +698,15 @@
             x, y = F.format(x), F.format(y)
             self._label_cursor.setText('(' + x + ', ' + y + ', ' + z + ')')
 
     def keyPressEvent(self, e):
         """
         Catch key presses?
         """
-        if e.key() == Qt.Key_Space:
+        if e.key() == Qt.Key.Key_Space:
             self.action_start_stop()
 
     def load_config(self):
         """
         Loads the user configuration from an ini file.
         """
         # Read ini file
@@ -747,15 +772,15 @@
         # Fix path
         fname = os.path.abspath(str(fname))
         self._path = os.path.dirname(fname)
         # Try loading file.
         self.statusBar().showMessage('Loading ' + str(fname))
         n = 1000000
         pd = QtWidgets.QProgressDialog('Loading data file...', 'Cancel', 0, n)
-        pd.setWindowModality(Qt.WindowModal)
+        pd.setWindowModality(Qt.WindowModality.WindowModal)
         pd.setValue(0)
 
         class Reporter(myokit.ProgressReporter):
             def __init__(self, pd):
                 self._pd = pd
 
             def enter(self, msg=None):
@@ -947,39 +972,39 @@
     # Attributes: cell x, cell y
     single_click = QtCore.Signal(float, float)
     # Double click!
     # Attributes: cell x, cell y
     double_click = QtCore.Signal(float, float)
 
     def __init__(self, *args):
-        super(VideoScene, self).__init__(*args)
+        super().__init__(*args)
         self.setBackgroundBrush(QtGui.QColor(192, 192, 192))
         self._w = None
         self._h = None
         self._p = None
         self.resize(1, 1)
 
     def mousePressEvent(self, event):
         """
         Single-click
         """
-        if event.button() == QtCore.Qt.LeftButton:
-            if event.modifiers() == Qt.NoModifier:
+        if event.button() == Qt.MouseButton.LeftButton:
+            if event.modifiers() == Qt.KeyBoardModifier.NoModifier:
                 p = event.scenePos()
                 x, y = int(p.x()), int(p.y())
                 if x >= 0 and x < self._w and y >= 0 and y < self._h:
                     self.single_click.emit(x, y)
                     return
 
     def mouseDoubleClickEvent(self, event):
         """
         Double-click
         """
-        if event.button() == QtCore.Qt.LeftButton:
-            if event.modifiers() == Qt.NoModifier:
+        if event.button() == Qt.MouseButton.LeftButton:
+            if event.modifiers() == Qt.KeyBoardModifier.NoModifier:
                 p = event.scenePos()
                 x, y = int(p.x()), int(p.y())
                 if x >= 0 and x < self._w and y >= 0 and y < self._h:
                     self.double_click.emit(x, y)
                     return
 
     def mouseMoveEvent(self, event):
@@ -1004,27 +1029,28 @@
     Views a color data scene.
     """
     # Signals
     # The view was resized
     resize_event = QtCore.Signal()
 
     def __init__(self, scene):
-        super(VideoView, self).__init__(scene)
+        super().__init__(scene)
         # Disable scrollbars
-        self.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
-        self.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
+        self.setHorizontalScrollBarPolicy(
+            Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+        self.setVerticalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
 
         # Set rendering hints
-        self.setRenderHint(QtGui.QPainter.Antialiasing)
+        self.setRenderHint(QtGui.QPainter.RenderHint.Antialiasing)
         self.setViewportUpdateMode(
-            QtWidgets.QGraphicsView.BoundingRectViewportUpdate)
+            QtWidgets.QGraphicsView.ViewportUpdateMode.BoundingRectViewportUpdate)  # noqa
 
         # Fit scene rect in view
         self.fitInView(self.sceneRect(), keepAspect=True)
-        self.setAlignment(Qt.AlignCenter)
+        self.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
         # Delayed resizing
         self._resize_timer = QtCore.QTimer()
         self._resize_timer.timeout.connect(self._resize_timeout)
 
         # No focus (no keyboard, no border)
         self.setFocusPolicy(Qt.FocusPolicy.NoFocus)
@@ -1034,30 +1060,21 @@
         For some reason, Qt has a stupid bug in it that gives the scene a
         (hardcoded) margin of 2px. To remove, this is a re-implementation of
         the fitInView method, loosely based on the original C.
 
         https://bugreports.qt-project.org/browse/QTBUG-11945
         """
         # Reset the view scale
-        try:
-            # PyQt5 / PySide
-            unity = self.transform().mapRect(QtCore.QRectF(0, 0, 1, 1))
-        except AttributeError:
-            # PyQt4
-            unity = self.matrix().mapRect(QtCore.QRectF(0, 0, 1, 1))
+        unity = self.transform().mapRect(QtCore.QRectF(0, 0, 1, 1))
         w, h = max(1, unity.width()), max(1, unity.height())
         self.scale(1. / w, 1 / h)
 
         # Find the ideal scaling ratio
         viewRect = self.viewport().rect()
-        try:
-            sceneRect = self.transform().mapRect(rect)
-        except AttributeError:
-            # PyQt4
-            sceneRect = self.matrix().mapRect(rect)
+        sceneRect = self.transform().mapRect(rect)
         xr = viewRect.width() / sceneRect.width()
         yr = viewRect.height() / sceneRect.height()
         if keepAspect:
             xr = min(xr, yr)
 
         # Scale and center
         self.scale(xr, yr)
@@ -1087,15 +1104,15 @@
     """
     # Signals
     # Somebody moved the mouse
     # Attributes: cell x, cell y
     mouse_moved = QtCore.Signal(float, float)
 
     def __init__(self):
-        super(GraphArea, self).__init__()
+        super().__init__()
         # DataBlock 2d, and its time vector
         self._data = None
         self._time = None
 
         # Index (x, y, variable) of temporary graph (if any)
         self._temp_index = None
         self._temp_path = None
@@ -1116,28 +1133,28 @@
         self._tmax = 1
         self._trange = self._tmax - self._tmin
 
         # Current position in time
         self._position = self._tmin
 
         # Colors for drawing
-        self._color_temp = Qt.black
+        self._color_temp = Qt.GlobalColor.black
         self._color_cycle = [
-            Qt.red,
-            #Qt.green,
-            Qt.blue,
-            #Qt.cyan,
-            Qt.magenta,
-            #Qt.yellow,
-            Qt.darkRed,
-            Qt.darkGreen,
-            Qt.darkBlue,
-            Qt.darkCyan,
-            Qt.darkMagenta,
-            Qt.darkYellow,
+            Qt.GlobalColor.red,
+            #Qt.GlobalColor.green,
+            Qt.GlobalColor.blue,
+            #Qt.GlobalColor.cyan,
+            Qt.GlobalColor.magenta,
+            #Qt.GlobalColor.yellow,
+            Qt.GlobalColor.darkRed,
+            Qt.GlobalColor.darkGreen,
+            Qt.GlobalColor.darkBlue,
+            Qt.GlobalColor.darkCyan,
+            Qt.GlobalColor.darkMagenta,
+            Qt.GlobalColor.darkYellow,
         ]
 
         # Scaling factors from pixels to normalized (0, 1) coordinates. Updated
         # after every resize.
         self._sw = 1.0
         self._sh = 1.0
 
@@ -1261,19 +1278,19 @@
             return
 
         # Create painter
         painter = QtGui.QPainter()
         painter.begin(self)
 
         # Fill background
-        painter.fillRect(self.rect(), QtGui.QBrush(Qt.white))
+        painter.fillRect(self.rect(), QtGui.QBrush(Qt.GlobalColor.white))
 
         # Create coordinate system for graphs
         painter.scale(self.width(), self.height())
-        painter.setRenderHint(QtGui.QPainter.Antialiasing)
+        painter.setRenderHint(QtGui.QPainter.RenderHint.Antialiasing)
 
         # Create pen
         pen = QtGui.QPen()
         pen.setWidth(0)
 
         # Draw frozen graphs
         colors = iter(self._color_cycle)
@@ -1289,15 +1306,15 @@
         # Draw temp graph
         if self._temp_path:
             pen.setColor(self._color_temp)
             painter.setPen(pen)
             painter.drawPath(self._temp_path)
 
         # Show time indicator
-        pen.setColor(Qt.red)
+        pen.setColor(Qt.GlobalColor.red)
         painter.setPen(pen)
         t = (self._position - self._tmin) / self._trange
         painter.drawLine(QtCore.QLineF(t, 0, t, 1))
 
         # Finish
         painter.end()
```

### Comparing `myokit-1.34.0/myokit/gui/datalog_viewer.py` & `myokit-1.35.0/myokit/gui/datalog_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 #
 # Qt gui for viewing DataBlock2d data files.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-# Standard library imports
+import configparser
 import gc
 import os
 import sys
 import traceback
 
-# Qt imports
 from myokit.gui import QtWidgets, QtGui, QtCore, Qt
 
-# Myokit
 import myokit
 import myokit.gui
-
-# Myokit components
 import myokit.formats.axon
 import myokit.formats.wcp
 
 # Matplotlib (must be imported _after_ gui has had chance to set backend)
 import matplotlib
 import matplotlib.figure
 from myokit.gui import matplotlib_backend as backend
@@ -35,20 +28,14 @@
 # SciPy: Only used to load matlab files.
 try:
     import scipy.io
     has_scipy = True
 except ImportError:
     has_scipy = False
 
-# ConfigParser in Python 2 and 3
-try:
-    import ConfigParser as configparser
-except ImportError:
-    import configparser
-
 
 # Application title
 TITLE = 'Myokit DataLog Viewer (PROTOTYPE)'
 
 # Application icon
 # def icon():
 #    icons = [
@@ -111,23 +98,23 @@
 
 
 class DataLogViewer(myokit.gui.MyokitApplication):
     """
     Graphical interface for viewing DataLog data.
     """
     def __init__(self, *filenames):
-        super(DataLogViewer, self).__init__()
+        super().__init__()
 
         # Set Title, icon
         self.setWindowTitle(TITLE + ' ' + myokit.__version__)
 
         # Set size, center
         self.resize(800, 600)
         qr = self.frameGeometry()
-        cp = QtWidgets.QDesktopWidget().availableGeometry().center()
+        cp = QtGui.QGuiApplication.primaryScreen().availableGeometry().center()
         qr.moveCenter(cp)
         self.move(qr.topLeft())
 
         # Add widget for file tabs
         self._tabs = TabWidget()
         self._tabs.setTabsClosable(True)
         self._tabs.tabCloseRequested.connect(self.action_close)
@@ -272,81 +259,82 @@
         """
         Creates this widget's menu.
         """
         self._menu = self.menuBar()
         # File menu
         self._menu_file = self._menu.addMenu('&File')
         # File > Open
-        self._tool_open = QtWidgets.QAction('&Open', self)
+        self._tool_open = QtGui.QAction('&Open', self)
         self._tool_open.setShortcut('Ctrl+O')
         self._tool_open.setStatusTip('Open a file')
         self._tool_open.setIcon(QtGui.QIcon.fromTheme('document-open'))
         self._tool_open.triggered.connect(self.action_open)
         self._menu_file.addAction(self._tool_open)
         # File > ----
         self._menu_file.addSeparator()
         # File > Quit
-        self._tool_exit = QtWidgets.QAction('&Quit', self)
+        self._tool_exit = QtGui.QAction('&Quit', self)
         self._tool_exit.setShortcut('Ctrl+Q')
         self._tool_exit.setStatusTip('Exit application.')
         self._tool_exit.setIcon(QtGui.QIcon.fromTheme('application-exit'))
         self._tool_exit.triggered.connect(self.close)
         self._menu_file.addAction(self._tool_exit)
         # View menu
         self._menu_view = self._menu.addMenu('&View')
         # View > Next file
-        self._tool_next_file = QtWidgets.QAction('Next file', self)
+        self._tool_next_file = QtGui.QAction('Next file', self)
         self._tool_next_file.setShortcut('Ctrl+PgDown')
         self._tool_next_file.setStatusTip('Select the next open file')
         self._tool_next_file.triggered.connect(self.action_next_file)
         self._tool_next_file.setEnabled(False)
         self._menu_view.addAction(self._tool_next_file)
         # View > Previous file
         self._menu_view.addAction(self._tool_next_file)
-        self._tool_prev_file = QtWidgets.QAction('Previous file', self)
+        self._tool_prev_file = QtGui.QAction('Previous file', self)
         self._tool_prev_file.setShortcut('Ctrl+PgUp')
         self._tool_prev_file.setStatusTip('Select the previous open file')
         self._tool_prev_file.triggered.connect(self.action_prev_file)
         self._tool_prev_file.setEnabled(False)
         self._menu_view.addAction(self._tool_prev_file)
         # View > Next variable
-        self._tool_next_var = QtWidgets.QAction('Next variable', self)
+        self._tool_next_var = QtGui.QAction('Next variable', self)
         self._tool_next_var.setShortcut('PgDown')
         self._tool_next_var.setStatusTip('Show the next variable')
         self._tool_next_var.triggered.connect(self.action_next_var)
         self._tool_next_var.setEnabled(False)
         self._menu_view.addAction(self._tool_next_var)
         # View > Previous var
-        self._tool_prev_var = QtWidgets.QAction('Previous variable', self)
+        self._tool_prev_var = QtGui.QAction('Previous variable', self)
         self._tool_prev_var.setShortcut('PgUp')
         self._tool_prev_var.setStatusTip('Show the previous variable')
         self._tool_prev_var.triggered.connect(self.action_prev_var)
         self._tool_prev_var.setEnabled(False)
         self._menu_view.addAction(self._tool_prev_var)
         # Help menu
         self._menu_help = self._menu.addMenu('&Help')
         # Help > About
-        self._tool_about = QtWidgets.QAction('&About', self)
+        self._tool_about = QtGui.QAction('&About', self)
         self._tool_about.setStatusTip('View information about this program.')
         self._tool_about.triggered.connect(self.action_about)
         self._menu_help.addAction(self._tool_about)
         # Help > License
-        self._tool_license = QtWidgets.QAction('&License', self)
+        self._tool_license = QtGui.QAction('&License', self)
         self._tool_license.setStatusTip('View this program\'s license info.')
         self._tool_license.triggered.connect(self.action_license)
         self._menu_help.addAction(self._tool_license)
 
     def create_toolbar(self):
         """
         Creates this widget's toolbar
         """
         self._toolbar = self.addToolBar('tools')
         self._toolbar.setFloatable(False)
         self._toolbar.setMovable(False)
-        self._toolbar.setToolButtonStyle(Qt.ToolButtonTextBesideIcon)
+        self._toolbar.setToolButtonStyle(
+            Qt.ToolButtonStyle.ToolButtonTextBesideIcon)
         self._toolbar.addAction(self._tool_open)
         #self._toolbar.addSeparator()
 
     def load_config(self):
         """
         Loads the user configuration from an ini file.
         """
@@ -504,15 +492,15 @@
         with open(inifile, 'w') as configfile:
             config.write(configfile)
 
     def show(self):
         """
         Shows this viewer.
         """
-        super(DataLogViewer, self).show()
+        super().show()
         QtWidgets.QApplication.processEvents()
 
     def fileTabChangeEvent(self, index):
         """
         Different file tab selected.
         """
         if index >= 0:
@@ -551,17 +539,17 @@
 
 
 class AbfTab(TabWidget):
     """
     A widget displaying an ABF file.
     """
     def __init__(self, parent, abf):
-        super(AbfTab, self).__init__(parent)
+        super().__init__(parent)
         self.setTabsClosable(False)
-        self.setTabPosition(self.East)
+        self.setTabPosition(self.TabPosition.East)
         self._abf = abf
         self._figures = []
         self._axes = []
         for i in range(self._abf.data_channels()):
             tab, name = self.create_graph_tab(i)
             self.addTab(tab, name)
         for i in range(self._abf.protocol_channels()):
@@ -645,27 +633,27 @@
         """
         for figure in self._figures:
             figure.clear()
         for axes in self._axes:
             axes.cla()
         del self._figures, self._axes
         gc.collect()
-        super(AbfTab, self).deleteLater()
+        super().deleteLater()
 
 
 class AtfTab(TabWidget):
     """
     A widget displaying an AGF file.
     """
     def __init__(self, parent, atf):
-        super(AtfTab, self).__init__(parent)
+        super().__init__(parent)
         self._atf = atf
 
         self.setTabsClosable(False)
-        self.setTabPosition(self.East)
+        self.setTabPosition(self.TabPosition.East)
 
         self._figures = []
         self._axes = []
         keys = list(self._atf.keys())
         if len(keys) > 1:
             time = keys[0]  # Time is always first (and regularly sampled)
             for key in keys[1:]:
@@ -716,27 +704,27 @@
         """
         for figure in self._figures:
             figure.clear()
         for axes in self._axes:
             axes.cla()
         del self._figures, self._axes
         gc.collect()
-        super(AtfTab, self).deleteLater()
+        super().deleteLater()
 
 
 class CsvTab(TabWidget):
     """
     A widget displaying a CSV file.
 
     The given log must have a time variable set.
     """
     def __init__(self, parent, log, filename):
-        super(CsvTab, self).__init__(parent)
+        super().__init__(parent)
         self.setTabsClosable(False)
-        self.setTabPosition(self.East)
+        self.setTabPosition(self.TabPosition.East)
         self._log = log.npview()
         self._filename = filename
         self._figures = []
         self._axes = []
 
         # Check time key was found
         time = log.time_key()
@@ -815,25 +803,25 @@
         """
         for figure in self._figures:
             figure.clear()
         for axes in self._axes:
             axes.cla()
         del self._figures, self._axes
         gc.collect()
-        super(CsvTab, self).deleteLater()
+        super().deleteLater()
 
 
 class MatTab(TabWidget):
     """
     A widget displaying a MAT file.
     """
     def __init__(self, parent, mat, filename):
-        super(MatTab, self).__init__(parent)
+        super().__init__(parent)
         self.setTabsClosable(False)
-        self.setTabPosition(self.East)
+        self.setTabPosition(self.TabPosition.East)
         self._figures = []
         self._filename = filename
         self._axes = []
 
         # Find usable data
         for key in mat.keys():
             if key[:1] == '_':
@@ -903,25 +891,25 @@
         """
         for figure in self._figures:
             figure.clear()
         for axes in self._axes:
             axes.cla()
         del self._figures, self._axes
         gc.collect()
-        super(MatTab, self).deleteLater()
+        super().deleteLater()
 
 
 class TxtTab(TabWidget):
     """
     A widget displaying a TXT file (with lots of heuristics!).
     """
     def __init__(self, parent, data, filename):
-        super(TxtTab, self).__init__(parent)
+        super().__init__(parent)
         self.setTabsClosable(False)
-        self.setTabPosition(self.East)
+        self.setTabPosition(self.TabPosition.East)
         self._figures = []
         self._filename = filename
         self._axes = []
 
         # Find usable data
         if np.prod(data.shape) == np.max(data.shape):
             # 1d data
@@ -985,25 +973,25 @@
         """
         for figure in self._figures:
             figure.clear()
         for axes in self._axes:
             axes.cla()
         del self._figures, self._axes
         gc.collect()
-        super(TxtTab, self).deleteLater()
+        super().deleteLater()
 
 
 class WcpTab(TabWidget):
     """
     A widget displaying a WCP file.
     """
     def __init__(self, parent, wcp):
-        super(WcpTab, self).__init__(parent)
+        super().__init__(parent)
         self.setTabsClosable(False)
-        self.setTabPosition(self.East)
+        self.setTabPosition(self.TabPosition.East)
         self._wcp = wcp
         self._figures = []
         self._axes = []
         for i in range(self._wcp.records()):
             self.addTab(self.create_graph_tab(i), 'Record ' + str(i))
         del self._wcp
 
@@ -1040,9 +1028,9 @@
         """
         for figure in self._figures:
             figure.clear()
         for axes in self._axes:
             axes.cla()
         del self._figures, self._axes
         gc.collect()
-        super(WcpTab, self).deleteLater()
+        super().deleteLater()
```

### Comparing `myokit-1.34.0/myokit/gui/explorer.py` & `myokit-1.35.0/myokit/gui/explorer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 #
 # Temporary Qt explorer for Myokit
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-# Standard library imports
-
-# Myokit
 import myokit
+import myokit.gui
 
-# Qt imports
 from myokit.gui import QtCore, QtGui, QtWidgets
-
-# GUI components
-import myokit.gui
+from myokit.gui import matplotlib_backend as backend
 from . import progress
 
 # Matplotlib (must be imported _after_ gui has had chance to set backend)
 import matplotlib
 import matplotlib.figure
-from myokit.gui import matplotlib_backend as backend
 
 
 # Constants
 # Classes & methods
 class Explorer(QtWidgets.QDialog):
     """
     Runs simulations with a model and allows all variables to be graphed.
@@ -40,15 +31,15 @@
         :class:`myokit.Protocol`, :class:`myokit.Simulation`).
     ``output_stream``
         Something with a write() method.
 
     *Extends:* ``QtWidgets.QDialog``
     """
     def __init__(self, parent, sim_method, output_stream, duration=1000):
-        super(Explorer, self).__init__(parent)
+        super().__init__(parent)
         self.setWindowTitle('Myokit Explorer')
         self._sim_method = sim_method
         self._stream = output_stream
         # Set guess for run times
         guess_pre = 0
         guess_run = duration
         # Explorer data
@@ -80,31 +71,34 @@
         self._select_x.currentIndexChanged.connect(self.combo_changed)
         self._select_y = QtWidgets.QComboBox()
         self._select_y.currentIndexChanged.connect(self.combo_changed)
         # Create bottom widgets
         self._close_button = QtWidgets.QPushButton('Close')
         self._close_button.clicked.connect(self.action_close)
         # Create button layout
-        button_layout = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.LeftToRight)
+        button_layout = QtWidgets.QBoxLayout(
+            QtWidgets.QBoxLayout.Direction.LeftToRight)
         button_layout.addWidget(label1)
         button_layout.addWidget(self._pre_field)
         button_layout.addWidget(label2)
         button_layout.addWidget(self._run_field)
         button_layout.addWidget(self._clear_button)
         button_layout.addWidget(self._run_button)
         # Create graph options layout
         graph_option_layout = QtWidgets.QBoxLayout(
-            QtWidgets.QBoxLayout.LeftToRight)
+            QtWidgets.QBoxLayout.Direction.LeftToRight)
         graph_option_layout.addWidget(self._select_x)
         graph_option_layout.addWidget(self._select_y)
         # Create bottom layout
-        bottom_layout = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.LeftToRight)
+        bottom_layout = QtWidgets.QBoxLayout(
+            QtWidgets.QBoxLayout.Direction.LeftToRight)
         bottom_layout.addWidget(self._close_button)
         # Create central layout
-        layout = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.TopToBottom)
+        layout = QtWidgets.QBoxLayout(
+            QtWidgets.QBoxLayout.Direction.TopToBottom)
         layout.addLayout(button_layout)
         layout.addLayout(graph_option_layout)
         layout.addWidget(self._canvas)
         layout.addWidget(self._toolbar)
         layout.addLayout(bottom_layout)
         self.setLayout(layout)
 
@@ -151,49 +145,49 @@
 
     def action_run(self):
         """
         Runs a simulation and updates the explorer data.
         """
         pbar = progress.ProgressBar(self, 'Creating simulation')
         QtWidgets.QApplication.processEvents(
-            QtCore.QEventLoop.ExcludeUserInputEvents)
+            QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
         try:
             pbar.show()
             QtWidgets.QApplication.processEvents(
-                QtCore.QEventLoop.ExcludeUserInputEvents)
+                QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
             # Create and run simulation
             out = self._sim_method()
             if type(out) == str:
                 self._stream.write(out)
                 return
             else:
                 m, p, s = out
             QtWidgets.QApplication.processEvents(
-                QtCore.QEventLoop.ExcludeUserInputEvents)
+                QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
             pre = float(self._pre_field.text())
             run = float(self._run_field.text())
             if pre:
                 s.pre(pre, progress=pbar.reporter())
             d = s.run(run, progress=pbar.reporter()).npview()
             self._stream.write('Final state: \n' + m.format_state(s.state()))
             QtWidgets.QApplication.processEvents(
-                QtCore.QEventLoop.ExcludeUserInputEvents)
+                QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
         except myokit.SimulationCancelledError:
             return
         except myokit.MyokitError as e:
             self._stream.write(str(e))
             return
         except Exception as e:
             self._stream.write(str(e))
             return
         finally:
             pbar.close()
             pbar.deleteLater()
             QtWidgets.QApplication.processEvents(
-                QtCore.QEventLoop.ExcludeUserInputEvents)
+                QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
         # Reset combo-box keys?
         reset_keys = True
         if self._keys:
             # Only reset keys if the old set differs from the new
             if self._keys == set(d.keys()):
                 reset_keys = False
         # Append or reset old data
```

### Comparing `myokit-1.34.0/myokit/gui/ide.py` & `myokit-1.35.0/myokit/gui/ide.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,40 @@
 #
 # Graphical interface to myokit. Allows mmt files to be created, modified and
 # run.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-# Standard library imports
+import configparser
 import gc
 import os
 import sys
 import textwrap
 import traceback
 import warnings
 
-# Myokit
 import myokit
 import myokit.formats
+import myokit.gui
 import myokit.lib.deps
 import myokit.lib.guess
 
-# Qt imports
 from myokit.gui import QtWidgets, QtGui, QtCore, Qt
 
-# GUI components
-import myokit.gui
 from . import source
 from . import explorer
 from . import progress
 from . import vargrapher
 
 # Matplotlib imports
 # Matplotlib.pyplot must be imported _after_ myokit.gui has set the backend
 import matplotlib
 matplotlib.interactive(True)        # Allows plt.show()
 
-# ConfigParser in Python 2 and 3
-try:
-    import ConfigParser as configparser
-except ImportError:
-    import configparser
-
 
 # Application title
 TITLE = 'Myokit IDE'
 
 # Settings file
 SETTINGS_FILE = os.path.join(myokit.DIR_USER, 'myokit-ide.ini')
 
@@ -106,24 +94,28 @@
 
 # Classes & functions
 class MyokitIDE(myokit.gui.MyokitApplication):
     """
     New GUI for editing ``.mmt`` files.
     """
     def __init__(self, filename=None):
-        super(MyokitIDE, self).__init__()
+        super().__init__()
+
+        # Regular expression for navigator
+        self._nav_query = QtCore.QRegularExpression(
+            r'^\[[a-zA-Z]{1}[a-zA-Z0-9_]*\]')
 
         # Set application icon
         self.setWindowIcon(icon())
 
         # Set size, center
         self.resize(950, 720)
         self.setMinimumSize(600, 440)
         qr = self.frameGeometry()
-        cp = QtWidgets.QDesktopWidget().availableGeometry().center()
+        cp = QtGui.QGuiApplication.primaryScreen().availableGeometry().center()
         qr.moveCenter(cp)
         self.move(qr.topLeft())
 
         # Status bar
         self._label_cursor = QtWidgets.QLabel()
         self.statusBar().addPermanentWidget(self._label_cursor)
         self.statusBar().showMessage('Ready')
@@ -180,33 +172,33 @@
         self._protocol_tools.add(self._protocol_search, 'Find/Replace')
 
         self._script_tools = TabbedToolBar()
         self._script_tools.tab_toggled.connect(self.change_tool_visibility)
         self._script_tools.add(self._script_search, 'Find/Replace')
 
         # Create editor tabs
-        self._model_tab = QtWidgets.QSplitter(Qt.Horizontal)
+        self._model_tab = QtWidgets.QSplitter(Qt.Orientation.Horizontal)
         self._model_tab.editor = self._model_editor
         self._model_tab.search = self._model_search
         self._model_tab.addWidget(self._model_editor)
         self._model_tab.addWidget(self._model_tools)
         self._model_tab.setSizes([400, 100])
         self._model_tab.setCollapsible(0, False)
         self._model_tab.setCollapsible(1, False)
 
-        self._protocol_tab = QtWidgets.QSplitter(Qt.Horizontal)
+        self._protocol_tab = QtWidgets.QSplitter(Qt.Orientation.Horizontal)
         self._protocol_tab.editor = self._protocol_editor
         self._protocol_tab.search = self._protocol_search
         self._protocol_tab.addWidget(self._protocol_editor)
         self._protocol_tab.addWidget(self._protocol_tools)
         self._protocol_tab.setSizes([400, 100])
         self._protocol_tab.setCollapsible(0, False)
         self._protocol_tab.setCollapsible(1, False)
 
-        self._script_tab = QtWidgets.QSplitter(Qt.Horizontal)
+        self._script_tab = QtWidgets.QSplitter(Qt.Orientation.Horizontal)
         self._script_tab.editor = self._script_editor
         self._script_tab.search = self._script_search
         self._script_tab.addWidget(self._script_editor)
         self._script_tab.addWidget(self._script_tools)
         self._script_tab.setSizes([400, 100])
         self._script_tab.setCollapsible(0, False)
         self._script_tab.setCollapsible(1, False)
@@ -241,15 +233,15 @@
         self._script_editor.copyAvailable.connect(self.change_copy_script)
 
         # Create console
         self._console = Console()
         self._console.write('Loading Myokit IDE')
 
         # Create central layout: vertical splitter
-        self._central_splitter = QtWidgets.QSplitter(Qt.Vertical)
+        self._central_splitter = QtWidgets.QSplitter(Qt.Orientation.Vertical)
         self._central_splitter.addWidget(self._editor_tabs)
         self._central_splitter.addWidget(self._console)
         self._central_splitter.setSizes([580, 120])
         self.setCentralWidget(self._central_splitter)
 
         # Timer to bundle operations after the model text has changed
         self._model_changed_timer = QtCore.QTimer()
@@ -377,18 +369,18 @@
     def action_clear_units(self):
         """
         Remove all units from expressions in this model.
         """
         try:
             # Ask are you sure?
             msg = 'Remove all units from expressions in model?'
-            box = QtWidgets.QMessageBox
-            options = box.Yes | box.No
-            reply = box.question(self, TITLE, msg, options)
-            if reply == box.No:
+            sb = QtWidgets.QMessageBox.StandardButton
+            reply = QtWidgets.QMessageBox.question(
+                self, TITLE, msg, sb.Yes | sb.No)
+            if reply == sb.No:
                 return
             # Strip units
             # Note: lines are used in error handling!
             lines = self._model_editor.get_text().splitlines()
             text = myokit.strip_expression_units(lines)
             self._model_editor.replace(text)
             self._console.write('Removed all expression units.')
@@ -462,29 +454,29 @@
     def action_explore(self):
         """
         Opens the explorer
         """
         # Simulation creation method
         def sim():
             QtWidgets.QApplication.processEvents(
-                QtCore.QEventLoop.ExcludeUserInputEvents)
+                QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
             try:
                 # Get model and protocol
                 m = self.model(errors_in_console=True)
                 if m is False:
                     return 'Errors in model'
                 elif m is None:
                     return 'Empty model definition'
                 QtWidgets.QApplication.processEvents(
-                    QtCore.QEventLoop.ExcludeUserInputEvents)
+                    QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
                 p = self.protocol(errors_in_console=True)
                 if p is False:
                     return 'Errors in protocol'
                 QtWidgets.QApplication.processEvents(
-                    QtCore.QEventLoop.ExcludeUserInputEvents)
+                    QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
                 # Create and return simulation
                 self.statusBar().showMessage('Creating simulation...')
                 return m, p, myokit.Simulation(m, p)
             except Exception:
                 self.show_exception()
         try:
             # Guess duration
@@ -1002,38 +994,38 @@
         """
         pbar = None
         try:
             # Prepare interface
             #self.setEnabled(False)
             self._console.write('Running embedded script.')
             QtWidgets.QApplication.setOverrideCursor(
-                QtGui.QCursor(Qt.WaitCursor))
+                QtGui.QCursor(Qt.CursorShape.WaitCursor))
             # Create progress bar
             pbar = progress.ProgressBar(self, 'Running embedded script')
             pbar.show()
             QtWidgets.QApplication.processEvents(
-                QtCore.QEventLoop.ExcludeUserInputEvents)
+                QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
             # Get model and protocol
             m = self.model(errors_in_console=True)
             if m is False:
                 return
             p = self.protocol(errors_in_console=True)
             if p is False:
                 return
             QtWidgets.QApplication.processEvents(
-                QtCore.QEventLoop.ExcludeUserInputEvents)
+                QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
             # Clone model & protocol: the script may modify them!
             if m:
                 m = m.clone()
             QtWidgets.QApplication.processEvents(
-                QtCore.QEventLoop.ExcludeUserInputEvents)
+                QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
             if p:
                 p = p.clone()
             QtWidgets.QApplication.processEvents(
-                QtCore.QEventLoop.ExcludeUserInputEvents)
+                QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
             # Get embedded script
             x = self._script_editor.get_text()
             # Run
             try:
                 myokit.run(
                     m, p, x,
                     stdout=self._console,
@@ -1047,15 +1039,15 @@
             except myokit.SimulationCancelledError:
                 self._console.write('Simulation cancelled by user.')
             except Exception:
                 self._console.write('An error has occurred')
                 self._console.write(traceback.format_exc())
         finally:
             QtWidgets.QApplication.processEvents(
-                QtCore.QEventLoop.ExcludeUserInputEvents)
+                QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
             # Hide progress bar
             if pbar is not None:
                 pbar.close()
                 pbar.deleteLater()
             # Work-around for cursor bug on linux
             #pos = QtGui.QCursor.pos()
             #QtGui.QCursor.setPos(0, 0)
@@ -1542,16 +1534,18 @@
             pass
         # Save changes?
         if not self.prompt_save_changes(cancel=False):
             # Something went wrong when saving changes or use wants to abort
             if event:
                 event.ignore()
             return
+
         # Close all windows, including matplotlib plots
-        QtWidgets.qApp.closeAllWindows()
+        QtWidgets.QApplication.instance().closeAllWindows()
+
         # Accept event, closing this window
         if event:
             event.accept()
 
     def close_explorer(self):
         """
         Closes the explorer, if any.
@@ -1566,550 +1560,538 @@
         """
         Creates this widget's menu.
         """
         self._menu = self.menuBar()
         # File menu
         self._menu_file = self._menu.addMenu('&File')
         # File > New
-        self._tool_new = QtWidgets.QAction('&New', self)
+        self._tool_new = QtGui.QAction('&New', self)
         self._tool_new.setShortcut('Ctrl+N')
         self._tool_new.setStatusTip('Create a new mmt file.')
         self._tool_new.setIcon(myokit.gui.icon('document-new'))
         self._tool_new.triggered.connect(self.action_new)
         self._menu_file.addAction(self._tool_new)
         # File > Open
-        self._tool_open = QtWidgets.QAction('&Open', self)
+        self._tool_open = QtGui.QAction('&Open', self)
         self._tool_open.setShortcut('Ctrl+O')
         self._tool_open.setStatusTip('Open an existing mmt file.')
         self._tool_open.setIcon(myokit.gui.icon('document-open'))
         self._tool_open.triggered.connect(self.action_open)
         self._menu_file.addAction(self._tool_open)
         # File > ----
         self._menu_file.addSeparator()
         # File > Save
-        self._tool_save = QtWidgets.QAction('&Save', self)
+        self._tool_save = QtGui.QAction('&Save', self)
         self._tool_save.setShortcut('Ctrl+S')
         self._tool_save.setStatusTip('Save the current file')
         self._tool_save.setIcon(myokit.gui.icon('document-save'))
         self._tool_save.triggered.connect(self.action_save)
         self._tool_save.setEnabled(False)
         self._menu_file.addAction(self._tool_save)
         # File > Save as
-        self._tool_save_as = QtWidgets.QAction('Save &as', self)
+        self._tool_save_as = QtGui.QAction('Save &as', self)
         self._tool_save_as.setShortcut('Ctrl+Shift+S')
         self._tool_save_as.setStatusTip(
             'Save the current file under a different name.')
         self._tool_save_as.triggered.connect(self.action_save_as)
         self._menu_file.addAction(self._tool_save_as)
         # File > ----
         self._menu_file.addSeparator()
         # File > Recent files
         self._recent_file_tools = []
         for i in range(N_RECENT_FILES):
-            tool = QtWidgets.QAction(self, visible=False)
+            tool = QtGui.QAction(self, visible=False)
             tool.triggered.connect(self.action_open_recent)
             self._recent_file_tools.append(tool)
             self._menu_file.addAction(tool)
         # File > ----
         self._menu_file.addSeparator()
         # File > Quit
-        self._tool_exit = QtWidgets.QAction('&Quit', self)
+        self._tool_exit = QtGui.QAction('&Quit', self)
         self._tool_exit.setShortcut('Ctrl+Q')
         self._tool_exit.setStatusTip('Exit application.')
         self._tool_exit.triggered.connect(self.close)
         self._menu_file.addAction(self._tool_exit)
         #
         # Edit menu
         #
         self._menu_edit = self._menu.addMenu('&Edit')
         # Edit > Undo
-        self._tool_undo = QtWidgets.QAction('&Undo', self)
+        self._tool_undo = QtGui.QAction('&Undo', self)
         self._tool_undo.setShortcut('Ctrl+Z')
         self._tool_undo.setStatusTip('Undo the last edit.')
         self._tool_undo.setIcon(myokit.gui.icon('edit-undo'))
         self._tool_undo.triggered.connect(self.action_undo)
         self._tool_undo.setEnabled(False)
         self._menu_edit.addAction(self._tool_undo)
         # Edit > Redo
-        self._tool_redo = QtWidgets.QAction('&Redo', self)
+        self._tool_redo = QtGui.QAction('&Redo', self)
         self._tool_redo.setShortcut('Ctrl+Shift+Z')
         self._tool_redo.setStatusTip('Redo the last undone edit.')
         self._tool_redo.setIcon(myokit.gui.icon('edit-redo'))
         self._tool_redo.triggered.connect(self.action_redo)
         self._tool_redo.setEnabled(False)
         self._menu_edit.addAction(self._tool_redo)
         # Edit > ----
         self._menu_edit.addSeparator()
         # Edit > Cut
-        self._tool_cut = QtWidgets.QAction('&Cut', self)
+        self._tool_cut = QtGui.QAction('&Cut', self)
         self._tool_cut.setShortcut('Ctrl+X')
         self._tool_cut.setStatusTip(
             'Cut the selected text and copy it to the clipboard.')
         #self._tool_cut.setIcon(myokit.gui.icon('edit-cut'))
         self._tool_cut.triggered.connect(self.action_cut)
         self._tool_cut.setEnabled(False)
         self._menu_edit.addAction(self._tool_cut)
         # Edit > Copy
-        self._tool_copy = QtWidgets.QAction('&Copy', self)
+        self._tool_copy = QtGui.QAction('&Copy', self)
         self._tool_copy.setShortcut('Ctrl+C')
         self._tool_copy.setStatusTip(
             'Copy the selected text to the clipboard.')
         #self._tool_copy.setIcon(myokit.gui.icon('edit-copy'))
         self._tool_copy.triggered.connect(self.action_copy)
         self._tool_copy.setEnabled(False)
         self._menu_edit.addAction(self._tool_copy)
         # Edit > Paste
-        self._tool_paste = QtWidgets.QAction('&Paste', self)
+        self._tool_paste = QtGui.QAction('&Paste', self)
         self._tool_paste.setShortcut('Ctrl+V')
         self._tool_paste.setStatusTip(
             'Paste text from the clipboard into the editor.')
         #self._tool_paste.setIcon(myokit.gui.icon('edit-paste'))
         self._tool_paste.triggered.connect(self.action_paste)
         self._menu_edit.addAction(self._tool_paste)
         # Edit > ----
         self._menu_edit.addSeparator()
         # Edit > Find and replace
-        self._tool_find = QtWidgets.QAction('&Find and replace', self)
+        self._tool_find = QtGui.QAction('&Find and replace', self)
         self._tool_find.setShortcut('Ctrl+F')
         self._tool_find.setStatusTip('Find and/or replace some text.')
         self._tool_find.setIcon(myokit.gui.icon('edit-find'))
         self._tool_find.triggered.connect(self.action_find)
         self._menu_edit.addAction(self._tool_find)
         # Edit > ----
         self._menu_edit.addSeparator()
         # Edit > Format protocol
-        self._tool_format_protocol = QtWidgets.QAction(
-            'Format protocol', self)
+        self._tool_format_protocol = QtGui.QAction('Format protocol', self)
         self._tool_format_protocol.setStatusTip(
             'Standardise the formatting of the protocol section.')
         self._tool_format_protocol.triggered.connect(
             self.action_format_protocol)
         self._menu_edit.addAction(self._tool_format_protocol)
         self._protocol_widgets.append(self._tool_format_protocol)
         # Edit > ----
         self._menu_edit.addSeparator()
         # Edit > Comment or uncomment
-        self._tool_comment = QtWidgets.QAction(
+        self._tool_comment = QtGui.QAction(
             '&Comment/uncomment selected lines', self)
         self._tool_comment.setShortcut('Ctrl+;')
         self._tool_comment.setStatusTip(
             'Comments or uncomments the currently selected lines.')
         self._tool_comment.triggered.connect(self.action_comment)
         self._menu_edit.addAction(self._tool_comment)
         # Edit > Remove units from expressions
-        self._tool_remove_units = QtWidgets.QAction(
+        self._tool_remove_units = QtGui.QAction(
             'Remove units from &expressions', self)
         self._tool_remove_units.setStatusTip(
             'Remove all units inside expressions.')
         self._tool_remove_units.triggered.connect(self.action_clear_units)
         self._menu_edit.addAction(self._tool_remove_units)
         self._model_widgets.append(self._tool_remove_units)
         # Edit > Trim whitespace
-        self._tool_trim_whitespace = QtWidgets.QAction(
+        self._tool_trim_whitespace = QtGui.QAction(
             'Trim trailing &whitespace', self)
         self._tool_trim_whitespace.setStatusTip(
             'Remove trailing whitespace from each line.')
         self._tool_trim_whitespace.triggered.connect(
             self.action_trim_whitespace)
         self._menu_edit.addAction(self._tool_trim_whitespace)
         #
         # View menu
         #
         self._menu_view = self._menu.addMenu('&View')
         # View > View model definition
-        self._tool_view_model = QtWidgets.QAction(
-            'View &model definition', self)
+        self._tool_view_model = QtGui.QAction('View &model definition', self)
         self._tool_view_model.setShortcut('Alt+1')
         self._tool_view_model.setStatusTip('View the model definition tab')
         self._tool_view_model.triggered.connect(self.action_view_model)
         self._menu_view.addAction(self._tool_view_model)
         # View > View protocol definition
-        self._tool_view_protocol = QtWidgets.QAction(
+        self._tool_view_protocol = QtGui.QAction(
             'View &protocol definition', self)
         self._tool_view_protocol.setShortcut('Alt+2')
         self._tool_view_protocol.setStatusTip(
             'View the protocol definition tab')
         self._tool_view_protocol.triggered.connect(self.action_view_protocol)
         self._menu_view.addAction(self._tool_view_protocol)
         # View > View embedded script
-        self._tool_view_script = QtWidgets.QAction(
-            'View embedded &script', self)
+        self._tool_view_script = QtGui.QAction('View embedded &script', self)
         self._tool_view_script.setShortcut('Alt+3')
         self._tool_view_script.setStatusTip('View the embedded script tab')
         self._tool_view_script.triggered.connect(self.action_view_script)
         self._menu_view.addAction(self._tool_view_script)
         # View > ----
         self._menu_view.addSeparator()
         # View > Show model components (navigator)
-        self._tool_view_navigator = QtWidgets.QAction(
+        self._tool_view_navigator = QtGui.QAction(
             'Show model &components', self)
         self._tool_view_navigator.setCheckable(True)
         self._tool_view_navigator.setStatusTip(
             'Shows or hides the model navigator pane.')
         self._tool_view_navigator.triggered.connect(
             self.action_toggle_navigator)
         self._menu_view.addAction(self._tool_view_navigator)
         self._model_widgets.append(self._tool_view_navigator)
         # View > ----
         self._menu_view.addSeparator()
         # View > Preview protocol
-        self._tool_preview_protocol = QtWidgets.QAction(
-            '&Preview protocol', self)
+        self._tool_preview_protocol = QtGui.QAction('&Preview protocol', self)
         self._tool_preview_protocol.setShortcut('Ctrl+P')
         self._tool_preview_protocol.setStatusTip(
             'Show a preview of the current protocol.')
         self._tool_preview_protocol.triggered.connect(
             self.action_preview_protocol)
         self._menu_view.addAction(self._tool_preview_protocol)
 
         #
         # Convert menu
         #
         self._menu_convert = self._menu.addMenu('&Convert')
 
         # Convert > Import CellML
-        self._tool_import_cellml = QtWidgets.QAction(
+        self._tool_import_cellml = QtGui.QAction(
             'Import model from CellML', self)
         self._tool_import_cellml.setStatusTip(
             'Import a model definition from a CellML file.')
         self._tool_import_cellml.triggered.connect(
             lambda: self.action_import_model('cellml', FILTER_CELLML))
         self._menu_convert.addAction(self._tool_import_cellml)
         # Convert > Export CellML 1
-        self._tool_export_cellml1 = QtWidgets.QAction(
+        self._tool_export_cellml1 = QtGui.QAction(
             'Export model to CellML 1.0', self)
         self._tool_export_cellml1.setStatusTip(
             'Export a model definition to a CellML 1.0 document.')
         self._tool_export_cellml1.triggered.connect(
             lambda: self.action_export_model(
                 'cellml1', '.cellml', FILTER_CELLML))
         self._menu_convert.addAction(self._tool_export_cellml1)
         # Convert > Export CellML 2
-        self._tool_export_cellml2 = QtWidgets.QAction(
+        self._tool_export_cellml2 = QtGui.QAction(
             'Export model to CellML 2.0', self)
         self._tool_export_cellml2.setStatusTip(
             'Export a model definition to a CellML 2.0 document.')
         self._tool_export_cellml2.triggered.connect(
             lambda: self.action_export_model(
                 'cellml2', '.cellml', FILTER_CELLML))
         self._menu_convert.addAction(self._tool_export_cellml2)
 
         # Convert > ----
         self._menu_convert.addSeparator()
         # Convert > Import ABF
-        self._tool_import_abf = QtWidgets.QAction(
-            'Import protocol from ABF', self)
+        self._tool_import_abf = QtGui.QAction('Import protocol from ABF', self)
         self._tool_import_abf.setStatusTip(
             'Import a protocol definition from an ABF file.')
         self._tool_import_abf.triggered.connect(
             self.action_import_abf_protocol)
         self._menu_convert.addAction(self._tool_import_abf)
         # Convert > Import ChannelML
-        self._tool_import_channelml = QtWidgets.QAction(
+        self._tool_import_channelml = QtGui.QAction(
             'Import model from ChannelML', self)
         self._tool_import_channelml.setStatusTip(
             'Import a channel model from ChannelML.')
         self._tool_import_channelml.triggered.connect(
             lambda: self.action_import_model('channelml', FILTER_CHANNELML))
         self._menu_convert.addAction(self._tool_import_channelml)
         # Convert > Import SBML
-        self._tool_import_sbml = QtWidgets.QAction(
-            'Import model from SBML', self)
+        self._tool_import_sbml = QtGui.QAction('Import model from SBML', self)
         self._tool_import_sbml.setStatusTip(
             'Import a model from SBML.')
         self._tool_import_sbml.triggered.connect(
             lambda: self.action_import_model('sbml', FILTER_SBML))
         self._menu_convert.addAction(self._tool_import_sbml)
 
         # Convert > ----
         self._menu_convert.addSeparator()
         # Convert > Export HTML
-        self._tool_export_html = QtWidgets.QAction(
-            'Export model to HTML', self)
+        self._tool_export_html = QtGui.QAction('Export model to HTML', self)
         self._tool_export_html.setStatusTip(
             'Export a model definition to an HTML document using presentation'
             ' MathML.')
         self._tool_export_html.triggered.connect(
             lambda: self.action_export_model('html', '.html', FILTER_HTML))
         self._menu_convert.addAction(self._tool_export_html)
         # Convert > Export Latex
-        self._tool_export_latex = QtWidgets.QAction(
-            'Export model to Latex', self)
+        self._tool_export_latex = QtGui.QAction('Export model to Latex', self)
         self._tool_export_latex.setStatusTip(
             'Export a model definition to a Latex document.')
         self._tool_export_latex.triggered.connect(
             lambda: self.action_export_model(
                 'latex-article', '.tex', FILTER_LATEX))
         self._menu_convert.addAction(self._tool_export_latex)
 
         # Convert > ----
         self._menu_convert.addSeparator()
 
         # Convert > Ansic
-        self._tool_export_ansic = QtWidgets.QAction('Export to Ansi C', self)
+        self._tool_export_ansic = QtGui.QAction('Export to Ansi C', self)
         self._tool_export_ansic.setStatusTip(
             'Export to a runnable Ansi C program.')
         self._tool_export_ansic.triggered.connect(
             lambda: self.action_export_runnable('ansic'))
         self._menu_convert.addAction(self._tool_export_ansic)
 
         # Convert > CUDA
-        self._tool_export_cuda = QtWidgets.QAction(
-            'Export to CUDA kernel', self)
+        self._tool_export_cuda = QtGui.QAction('Export to CUDA kernel', self)
         self._tool_export_cuda.setStatusTip(
             'Export a model definition to a CUDA kernel program.')
         self._tool_export_cuda.triggered.connect(
             lambda: self.action_export_runnable('cuda-kernel'))
         self._menu_convert.addAction(self._tool_export_cuda)
 
         # Convert > CUDA RL
-        self._tool_export_cuda_rl = QtWidgets.QAction(
+        self._tool_export_cuda_rl = QtGui.QAction(
             'Export to CUDA kernel with RL updates', self)
         self._tool_export_cuda_rl.setStatusTip(
             'Export a model definition to a CUDA kernel program using'
             ' Rush-Larsen updates where possible.')
         self._tool_export_cuda_rl.triggered.connect(
             lambda: self.action_export_runnable('cuda-kernel-rl'))
         self._menu_convert.addAction(self._tool_export_cuda_rl)
 
         # Convert > EasyML
-        self._tool_export_easyml = QtWidgets.QAction(
+        self._tool_export_easyml = QtGui.QAction(
             'Export to EasyML (Carp)', self)
         self._tool_export_easyml.setStatusTip(
             'Export to an EasyML script for use with Carp/Carpentry.')
         self._tool_export_easyml.triggered.connect(
             lambda: self.action_export_model('easyml', '.model'))
         self._menu_convert.addAction(self._tool_export_easyml)
 
         # Convert > Matlab
-        self._tool_export_matlab = QtWidgets.QAction(
+        self._tool_export_matlab = QtGui.QAction(
             'Export to Matlab/Octave', self)
         self._tool_export_matlab.setStatusTip(
             'Export to a runnable Matlab/Octave script.')
         self._tool_export_matlab.triggered.connect(
             lambda: self.action_export_runnable('matlab'))
         self._menu_convert.addAction(self._tool_export_matlab)
 
         # Convert > OpenCL
-        self._tool_export_opencl = QtWidgets.QAction(
+        self._tool_export_opencl = QtGui.QAction(
             'Export to OpenCL kernel', self)
         self._tool_export_opencl.setStatusTip(
             'Export a model definition to an OpenCL kernel program using')
         self._tool_export_opencl.triggered.connect(
             lambda: self.action_export_runnable('opencl'))
         self._menu_convert.addAction(self._tool_export_opencl)
 
         # Convert > OpenCL RL
-        self._tool_export_opencl_rl = QtWidgets.QAction(
+        self._tool_export_opencl_rl = QtGui.QAction(
             'Export to OpenCL kernel with RL updates', self)
         self._tool_export_opencl_rl.setStatusTip(
             'Export a model definition to an OpenCL kernel program using'
             ' Rush-Larsen updates where possible.')
         self._tool_export_opencl_rl.triggered.connect(
             lambda: self.action_export_runnable('opencl-rl'))
         self._menu_convert.addAction(self._tool_export_opencl_rl)
 
         # Convert > Python
-        self._tool_export_python = QtWidgets.QAction('Export to Python', self)
+        self._tool_export_python = QtGui.QAction('Export to Python', self)
         self._tool_export_python.setStatusTip(
             'Export a model definition to a runnable Python script.')
         self._tool_export_python.triggered.connect(
             lambda: self.action_export_runnable('python'))
         self._menu_convert.addAction(self._tool_export_python)
 
         #
         # Analysis menu
         #
         self._menu_analysis = self._menu.addMenu('&Analysis')
         # Analysis > Model statistics
-        self._tool_stats = QtWidgets.QAction('Show model statistics', self)
+        self._tool_stats = QtGui.QAction('Show model statistics', self)
         self._tool_stats.setStatusTip(
             'Displays some basic statistics about the current model.')
         self._tool_stats.triggered.connect(self.action_model_stats)
         self._menu_analysis.addAction(self._tool_stats)
         # Analysis > ----
         self._menu_analysis.addSeparator()
         # Analysis > Check units strict
-        self._tool_units_strict = QtWidgets.QAction(
-            'Check units (&strict)', self)
+        self._tool_units_strict = QtGui.QAction('Check units (&strict)', self)
         self._tool_units_strict.setShortcut('F9')
         self._tool_units_strict.setStatusTip(
             'Check this model\'s units in strict mode.')
         self._tool_units_strict.triggered.connect(
             self.action_check_units_strict)
         self._menu_analysis.addAction(self._tool_units_strict)
         # Analysis > Check units tolerant
-        self._tool_units_tolerant = QtWidgets.QAction(
+        self._tool_units_tolerant = QtGui.QAction(
             'Check units (&tolerant)', self)
         self._tool_units_tolerant.setShortcut('F10')
         self._tool_units_tolerant.setStatusTip(
             'Check this model\'s units in tolerant mode.')
         self._tool_units_tolerant.triggered.connect(
             self.action_check_units_tolerant)
         self._menu_analysis.addAction(self._tool_units_tolerant)
         # Analysis > ----
         self._menu_analysis.addSeparator()
         # Analysis > Show variable info
-        self._tool_variable_info = QtWidgets.QAction(
+        self._tool_variable_info = QtGui.QAction(
             'Show quick variable info', self)
         self._tool_variable_info.setShortcut('Ctrl+R')
         self._tool_variable_info.setStatusTip(
             'Shows this variable\'s type and where it is defined.')
         self._tool_variable_info.triggered.connect(self.action_variable_info)
         self._menu_analysis.addAction(self._tool_variable_info)
         self._model_widgets.append(self._tool_variable_info)
         # Analysis > Show variable evaluation
-        self._tool_variable_evaluation = QtWidgets.QAction(
+        self._tool_variable_evaluation = QtGui.QAction(
             'Show variable evaluation', self)
         self._tool_variable_evaluation.setShortcut('Ctrl+E')
         self._tool_variable_evaluation.setStatusTip(
             'Show how the selected variable is evaluated.')
         self._tool_variable_evaluation.triggered.connect(
             self.action_variable_evaluation)
         self._menu_analysis.addAction(self._tool_variable_evaluation)
         self._model_widgets.append(self._tool_variable_evaluation)
         # Analysis > Show variable dependencies
-        self._tool_variable_dependencies = QtWidgets.QAction(
+        self._tool_variable_dependencies = QtGui.QAction(
             'Show variable dependencies', self)
         self._tool_variable_dependencies.setShortcut('Ctrl+D')
         self._tool_variable_dependencies.setStatusTip(
             'Show all expressions needed to calculate the selected variable.')
         self._tool_variable_dependencies.triggered.connect(
             self.action_variable_dependencies)
         self._menu_analysis.addAction(self._tool_variable_dependencies)
         self._model_widgets.append(self._tool_variable_dependencies)
         # Analysis > Show variable users
-        self._tool_variable_users = QtWidgets.QAction(
+        self._tool_variable_users = QtGui.QAction(
             'Show variable users', self)
         self._tool_variable_users.setShortcut('Ctrl+U')
         self._tool_variable_users.setStatusTip(
             'Show all expressions dependent on the selected variable.')
         self._tool_variable_users.triggered.connect(
             self.action_variable_users)
         self._menu_analysis.addAction(self._tool_variable_users)
         self._model_widgets.append(self._tool_variable_users)
         # Analysis > Graph variable
-        self._tool_variable_graph = QtWidgets.QAction(
+        self._tool_variable_graph = QtGui.QAction(
             'Graph selected variable', self)
         self._tool_variable_graph.setShortcut('Ctrl+G')
         self._tool_variable_graph.setStatusTip(
             'Display a graph of the selected variable.')
         self._tool_variable_graph.triggered.connect(self.action_variable_graph)
         self._menu_analysis.addAction(self._tool_variable_graph)
         self._model_widgets.append(self._tool_variable_graph)
         # Analysis > Jump to variable definition
-        self._tool_variable_jump = QtWidgets.QAction(
+        self._tool_variable_jump = QtGui.QAction(
             'Jump to variable definition', self)
         self._tool_variable_jump.setShortcut('Ctrl+J')
         self._tool_variable_jump.setStatusTip(
             'Jump to the selected variable\'s definition.')
         self._tool_variable_jump.triggered.connect(
             self.action_variable_definition)
         self._menu_analysis.addAction(self._tool_variable_jump)
         self._model_widgets.append(self._tool_variable_jump)
 
         # Analysis > ----
         self._menu_analysis.addSeparator()
         # Analysis > Evaluate state derivatives
-        self._tool_state_derivatives = QtWidgets.QAction(
+        self._tool_state_derivatives = QtGui.QAction(
             'Evaluate state derivatives', self)
         self._tool_state_derivatives.setShortcut('F7')
         self._tool_state_derivatives.setStatusTip(
             'Evaluate all state derivatives and display the results.')
         self._tool_state_derivatives.triggered.connect(
             self.action_state_derivatives)
         self._menu_analysis.addAction(self._tool_state_derivatives)
         # Analysis > Evaluate state derivatives without error checking
-        self._tool_state_derivatives2 = QtWidgets.QAction(
+        self._tool_state_derivatives2 = QtGui.QAction(
             'Evaluate state derivatives (no error checking)', self)
         self._tool_state_derivatives2.setShortcut('F8')
         self._tool_state_derivatives2.setStatusTip(
             'Evaluate all state derivatives without checking for numerical'
             ' errors.')
         self._tool_state_derivatives2.triggered.connect(
             self.action_state_derivatives2)
         self._menu_analysis.addAction(self._tool_state_derivatives2)
         # Analysis > ----
         self._menu_analysis.addSeparator()
         # Analysis > Show component dependency graph
-        self._tool_component_dependency_graph = QtWidgets.QAction(
+        self._tool_component_dependency_graph = QtGui.QAction(
             'Show component dependency graph', self)
         self._tool_component_dependency_graph.setStatusTip(
             'Display a graph of the dependencies between components.')
         self._tool_component_dependency_graph.triggered.connect(
             self.action_component_dependency_graph)
         self._menu_analysis.addAction(self._tool_component_dependency_graph)
         # Analysis > Show variable dependency graph
-        self._tool_variable_dependency_graph = QtWidgets.QAction(
+        self._tool_variable_dependency_graph = QtGui.QAction(
             'Show variable dependency graph', self)
         self._tool_variable_dependency_graph.setStatusTip(
             'Display a graph of the dependencies between variables.')
         self._tool_variable_dependency_graph.triggered.connect(
             self.action_variable_dependency_graph)
         self._menu_analysis.addAction(self._tool_variable_dependency_graph)
         # Analysis > Show state dependency matrix
-        self._tool_state_matrix = QtWidgets.QAction(
+        self._tool_state_matrix = QtGui.QAction(
             'Show state dependency matrix', self)
         self._tool_state_matrix.setStatusTip(
             'Display a matrix graph of the dependencies between states.')
         self._tool_state_matrix.triggered.connect(self.action_state_matrix)
         self._menu_analysis.addAction(self._tool_state_matrix)
         # Analysis > Show component dependency cycles
-        self._tool_component_cycles = QtWidgets.QAction(
+        self._tool_component_cycles = QtGui.QAction(
             'Show cyclical component dependencies', self)
         self._tool_component_cycles.setStatusTip(
             'Display a list of cyclical dependencies between components.')
         self._tool_component_cycles.triggered.connect(
             self.action_component_cycles)
         self._menu_analysis.addAction(self._tool_component_cycles)
         #
         # Run menu
         #
         self._menu_run = self._menu.addMenu('&Run')
         # Run > Validate
-        self._tool_validate = QtWidgets.QAction(
-            '&Validate model', self)
+        self._tool_validate = QtGui.QAction('&Validate model', self)
         self._tool_validate.setShortcut('Ctrl+B')
         self._tool_validate.setStatusTip('Validate the model.')
         self._tool_validate.triggered.connect(self.action_validate)
         self._menu_run.addAction(self._tool_validate)
         # Run > Jump to error
-        self._tool_jump_to_error = QtWidgets.QAction(
-            '&Jump to last error', self)
+        self._tool_jump_to_error = QtGui.QAction('&Jump to last error', self)
         self._tool_jump_to_error.setShortcut('Ctrl+Space')
         self._tool_jump_to_error.setStatusTip(
             'Jump to the last model error found.')
         self._tool_jump_to_error.triggered.connect(self.action_jump_to_error)
         self._menu_run.addAction(self._tool_jump_to_error)
         # Run > Run embedded script
-        self._tool_run = QtWidgets.QAction('&Run embedded script', self)
+        self._tool_run = QtGui.QAction('&Run embedded script', self)
         self._tool_run.setShortcut('F5')
         self._tool_run.setStatusTip('Run the embedded script.')
         self._tool_run.setIcon(myokit.gui.icon('media-playback-start'))
         self._tool_run.triggered.connect(self.action_run)
         self._menu_run.addAction(self._tool_run)
         # Run > Run explorer
-        self._tool_explore = QtWidgets.QAction('&Run explorer', self)
+        self._tool_explore = QtGui.QAction('&Run explorer', self)
         self._tool_explore.setShortcut('F6')
         self._tool_explore.setStatusTip(
             'Run a simulation and display the results in the explorer.')
         self._tool_explore.setIcon(myokit.gui.icon('media-playback-start'))
         self._tool_explore.triggered.connect(self.action_explore)
         self._menu_run.addAction(self._tool_explore)
         #
         # Help menu
         #
         self._menu_help = self._menu.addMenu('&Help')
         # Help > About
-        self._tool_about = QtWidgets.QAction('&About', self)
+        self._tool_about = QtGui.QAction('&About', self)
         self._tool_about.setStatusTip('View information about this program.')
         self._tool_about.triggered.connect(self.action_about)
         self._menu_help.addAction(self._tool_about)
         # Help > License
-        self._tool_license = QtWidgets.QAction('&License', self)
+        self._tool_license = QtGui.QAction('&License', self)
         self._tool_license.setStatusTip('View this program\'s license info.')
         self._tool_license.triggered.connect(self.action_license)
         self._menu_help.addAction(self._tool_license)
 
     def create_toolbar(self):
         """
         Creates the shared toolbar.
@@ -2356,23 +2338,23 @@
         """
         if not self._have_changes:
             return True
         if self._file:
             msg = 'Save changes to ' + str(self._file) + '?'
         else:
             msg = 'Save changes to new file?'
-        box = QtWidgets.QMessageBox
-        options = box.Yes | box.No
+        sb = QtWidgets.QMessageBox.StandardButton
+        options = sb.Yes | sb.No
         if cancel:
-            options |= box.Cancel
-        reply = box.question(self, TITLE, msg, options)
-        if reply == box.Yes:
+            options |= sb.Cancel
+        reply = QtWidgets.QMessageBox.question(self, TITLE, msg, options)
+        if reply == sb.Yes:
             # Only allow quitting if save succesful
             return self.save_file(save_as=False)
-        elif reply == box.No:
+        elif reply == sb.No:
             return True
         else:
             return False
 
     def protocol(self, force=False, console=False, errors_in_console=False):
         """
         Validates the entered pacing protocol and returns it.
@@ -2586,24 +2568,21 @@
             self, TITLE,
             '<h1>An error has occurred.</h1>'
             '<pre>' + text + '</pre>')
 
     def update_navigator(self):
         """ Updates the model navigator contents. """
         # Find all components and store their positions in a list (name, line)
-        #Sloppy version: query = QtCore.QRegExp(r'^\[') could be faster?
-        query = QtCore.QRegExp(r'^\[[a-zA-Z]{1}[a-zA-Z0-9_]*\]')
         pos = 0
-        found = self._model_editor.document().find(query, pos)
+        found = self._model_editor.document().find(self._nav_query, pos)
         positions = []
         while not found.isNull():
             pos = found.position()
-            block = found.block()
-            positions.append((block.text(), pos))
-            found = self._model_editor.document().find(query, pos)
+            positions.append((found.selectedText(), pos))
+            found = self._model_editor.document().find(self._nav_query, pos)
         self._model_navigator.set_positions(positions)
 
     def update_recent_files_menu(self):
         """
         Updates the recent files menu.
         """
         for k, filename in enumerate(self._recent_files):
@@ -2633,15 +2612,15 @@
     request, and hidden using the "close" button.
     """
     # Signal: Tab show (added) or hidden (removed)
     # Attributes: (widget, status)
     tab_toggled = QtCore.Signal(QtWidgets.QWidget, bool)
 
     def __init__(self, parent=None):
-        super(TabbedToolBar, self).__init__(parent)
+        super().__init__(parent)
 
         self.setTabsClosable(True)
         self.tabCloseRequested.connect(self._close_button_hit)
 
         # Mapping from widgets to their labels
         self._tabs = {}
 
@@ -2658,19 +2637,19 @@
     def _close_button_hit(self, index):
         """ Called when the user clicks a "close tab" button. """
         self.toggle(self.widget(index), False)
 
     def keyPressEvent(self, event):
         """ Qt event: A key-press reaches the widget. """
         key = event.key()
-        if key == Qt.Key_Escape:
+        if key == Qt.Key.Key_Escape:
             self.setFocus()
             self.focusPreviousChild()
         else:
-            super(TabbedToolBar, self).keyPressEvent(event)
+            super().keyPressEvent(event)
 
     def toggle(self, widget, new_status=None):
         """
         Toggles the visibility of the given widget (which must previously have
         been added with :meth:`add`), and returns its updated visibility
         status.
 
@@ -2716,15 +2695,15 @@
     Model navigator window used to jump to different model components.
     """
     # Signal: Component selected
     # Attributes: (description)
     item_changed = QtCore.Signal(int)
 
     def __init__(self, parent=None):
-        super(ModelNavigator, self).__init__(parent)
+        super().__init__(parent)
 
         # List widget
         self._list_widget = QtWidgets.QListWidget()
         self._list_widget.currentItemChanged.connect(self.current_item_changed)
 
         layout = QtWidgets.QVBoxLayout()
         layout.addWidget(self._list_widget)
@@ -2732,15 +2711,15 @@
 
         # List contents
         self._positions = []
 
     def current_item_changed(self, item, previous_item):
         """ Called if the navigator item is changed. """
         if item is not None:
-            line = item.data(Qt.UserRole)
+            line = item.data(Qt.ItemDataRole.UserRole)
             self.item_changed.emit(line)
 
     def set_positions(self, positions):
         """ Updates the component list """
 
         # Check if update is required
         if positions == self._positions:
@@ -2748,32 +2727,33 @@
         self._positions = list(positions)
 
         # Create new items
         self._list_widget.clear()
         self._list_widget.setSortingEnabled(True)
         for text, pos in self._positions:
             item = QtWidgets.QListWidgetItem(text[1:-1])
-            item.setData(Qt.UserRole, pos)
+            item.setData(Qt.ItemDataRole.UserRole, pos)
             self._list_widget.addItem(item)
 
 
 class Console(QtWidgets.QPlainTextEdit):
     """
     Console window used to write plain text output to in the IDE. Shows model
     parsing states and output of running explorations / scripts.
 
     *Extends*: ``QtWidgets.QPlainTextEdit``
     """
     def __init__(self, parent=None):
-        super(Console, self).__init__(parent)
+        super().__init__(parent)
         self.setReadOnly(True)
         font = myokit.gui.qtMonospaceFont()
         font.setPointSize(10)
         self.setFont(font)
-        self.setFrameStyle(QtWidgets.QFrame.WinPanel | QtWidgets.QFrame.Sunken)
+        self.setFrameStyle(
+            QtWidgets.QFrame.Shape.WinPanel | QtWidgets.QFrame.Shadow.Sunken)
 
     def clear(self):
         """
         Clears the console.
         """
         self.setPlainText('')
 
@@ -2807,8 +2787,8 @@
         #    return
         # Write text
         self.appendPlainText('[' + myokit.time() + '] ' + str(text))
         # Autoscroll
         self.verticalScrollBar().setValue(self.verticalScrollBar().maximum())
         # Autoflush
         QtWidgets.QApplication.processEvents(
-            QtCore.QEventLoop.ExcludeUserInputEvents)
+            QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
```

### Comparing `myokit-1.34.0/myokit/gui/progress.py` & `myokit-1.35.0/myokit/gui/progress.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Progress bar for Myokit
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
 from myokit.gui import Qt, QtCore, QtWidgets
 
 # GUI components
 # Constants
 N = 100000000
 
@@ -18,17 +15,18 @@
 class ProgressBar(QtWidgets.QProgressDialog):
     """
     Progress bar dialog for Myokit. Has a method :meth:`reporter()` that will
     return a :class:`myokit.ProgressReporter` for interfacing with simulations
     and other tasks implementing the ``ProgressReporter`` interface.
     """
     def __init__(self, parent, message):
-        super(ProgressBar, self).__init__(
-            message, 'Cancel', 0, N, parent=parent)
-        self.setWindowModality(Qt.WindowModal)
+        super().__init__(
+            message, 'Cancel', 0, N, parent)
+        self.setWindowTitle(' ')
+        self.setWindowModality(Qt.WindowModality.WindowModal)
         self.setAutoClose(False)
         self.setAutoReset(False)
         self._reporter = ProgressBarReporter(self)
 
     def reporter(self):
         """
         Returns a :class:`ProgressReporter` for his progress bar.
@@ -47,27 +45,29 @@
     A :class:`myokit.ProgressReporter` that sends updates to a
     :class:`ProgressBar`. To use, create a ``ProgressBar`` and then call its
     :meth:`reporter() <ProgressBar.reporter>` method to obtain a linked
     ``ProgressBarReporter``.
     """
 
     def __init__(self, pd):
-        super(ProgressBarReporter, self).__init__()
+        super().__init__()
         self._pd = pd
 
     def enter(self, msg=None):
         self._pd.setEnabled(True)
         self._pd.reset()
         if msg is not None:
             self._pd.setLabelText(str(msg))
         self._pd.setValue(0)
+        self._pd.repaint()
         QtWidgets.QApplication.processEvents(
-            QtCore.QEventLoop.ExcludeUserInputEvents)
+            QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
 
     def exit(self):
         self._pd.setEnabled(False)
 
     def update(self, f):
         self._pd.setValue((int)(N * f))
         QtWidgets.QApplication.processEvents(
-            QtCore.QEventLoop.ExcludeUserInputEvents)
+            QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents)
+        self._pd.repaint()
         return not self._pd.wasCanceled()
```

### Comparing `myokit-1.34.0/myokit/gui/source.py` & `myokit-1.35.0/myokit/gui/source.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 # Source code editor for Myokit.
 #
 # This code is based in part on examples provided by the PyQt project.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
+
 from myokit.gui import Qt, QtCore, QtGui, QtWidgets
 
+
 # GUI components
 # Constants
 SPACE = ' '
 TABS = 4
 INDENT = SPACE * TABS
 BRACKETS = {
     '(': ')',
@@ -64,25 +63,25 @@
     # Don't mess with these directly: Use the SVG in myokit-docs
     if not dark:
         STYLE_HEADER.setForeground(QtGui.QColor(0, 31, 231))
         STYLE_COMMENT.setForeground(QtGui.QColor(103, 161, 107))
         STYLE_ANNOT_KEY.setForeground(QtGui.QColor(0, 31, 231))
         STYLE_ANNOT_VAL.setForeground(QtGui.QColor(57, 115, 214))
         STYLE_KEYWORD_1.setForeground(QtGui.QColor(0, 128, 0))
-        STYLE_KEYWORD_1.setFontWeight(QtGui.QFont.Bold)
+        STYLE_KEYWORD_1.setFontWeight(QtGui.QFont.Weight.Bold)
         STYLE_KEYWORD_2.setForeground(QtGui.QColor(0, 128, 128))
         STYLE_LITERAL.setForeground(QtGui.QColor(255, 20, 215))
         STYLE_INLINE_UNIT.setForeground(QtGui.QColor(128, 0, 128))
     else:
         STYLE_HEADER.setForeground(QtGui.QColor(98, 178, 255))
         STYLE_COMMENT.setForeground(QtGui.QColor(153, 153, 153))
         STYLE_ANNOT_KEY.setForeground(QtGui.QColor(179, 179, 179))
         STYLE_ANNOT_VAL.setForeground(QtGui.QColor(171, 177, 205))
         STYLE_KEYWORD_1.setForeground(QtGui.QColor(10, 195, 87))
-        STYLE_KEYWORD_1.setFontWeight(QtGui.QFont.Bold)
+        STYLE_KEYWORD_1.setFontWeight(QtGui.QFont.Weight.Bold)
         STYLE_KEYWORD_2.setForeground(QtGui.QColor(10, 195, 87))
         STYLE_LITERAL.setForeground(QtGui.QColor(255, 223, 12))
         STYLE_INLINE_UNIT.setForeground(QtGui.QColor(168, 152, 33))
 
         global COLOR_SELECTED_LINE
         COLOR_SELECTED_LINE = QtGui.QColor(70, 70, 70)
 
@@ -93,15 +92,15 @@
     Source code editor used in Myokit.
 
     Provides the signal ``find_action(str)`` which is fired everything a find
     action occurred with a description that can be used in an application's
     status bar.
     """
     def __init__(self, parent=None):
-        super(Editor, self).__init__(parent)
+        super().__init__(parent)
 
         # Current style
         self._palette = QtGui.QGuiApplication.palette()
         _check_for_dark_mode(self._palette)
 
         # Apply default settings
         self._default_settings()
@@ -111,15 +110,20 @@
         self._line_number_area.update_width(0)
 
         # Add current line highlighting and bracket matching
         self.cursorPositionChanged.connect(self.cursor_changed)
         self.cursor_changed()
 
         # Line position
-        self._line_offset = self.fontMetrics().width(' ' * 79)
+        try:
+            # https://doc.qt.io/qt-5/qfontmetrics.html#horizontalAdvance
+            # Qt 5.5.11 and onwards
+            self._line_offset = self.fontMetrics().horizontalAdvance(' ' * 79)
+        except AttributeError:
+            self._line_offset = self.fontMetrics().width(' ' * 79)
 
         # Number of blocks in page up/down
         self._blocks_per_page = 1
 
         # Last position in line, used for smart up/down buttons
         self._last_column = None
         self.textChanged.connect(self._text_has_changed)
@@ -127,50 +131,51 @@
     def cursor_changed(self):
         """ Slot: Called when the cursor position is changed """
         # Highlight current line
         extra_selections = []
         selection = QtWidgets.QTextEdit.ExtraSelection()
         selection.format.setBackground(COLOR_SELECTED_LINE)
         selection.format.setProperty(
-            QtGui.QTextFormat.FullWidthSelection, True)
+            QtGui.QTextFormat.Property.FullWidthSelection, True)
         selection.cursor = self.textCursor()
         selection.cursor.clearSelection()
         extra_selections.append(selection)
 
         # Bracket matching
         cursor = self.textCursor()
         if not cursor.hasSelection():
             # Test if in front of or behind an opening or closing bracket
             pos = cursor.position()
             bracket = None
             if not cursor.atEnd():
-                cursor.setPosition(pos + 1, QtGui.QTextCursor.KeepAnchor)
+                cursor.setPosition(
+                    pos + 1, QtGui.QTextCursor.MoveMode.KeepAnchor)
                 text = cursor.selectedText()
                 if text in BRACKETS:
                     bracket = cursor
             elif bracket is None and not cursor.atStart():
                 cursor.setPosition(pos - 1)
-                cursor.setPosition(pos, QtGui.QTextCursor.KeepAnchor)
+                cursor.setPosition(pos, QtGui.QTextCursor.MoveMode.KeepAnchor)
                 text = cursor.selectedText()
                 if text in BRACKETS:
                     bracket = cursor
 
             if bracket:
                 # Find matching partner
                 doc = self.document()
                 depth = 1
                 start = bracket.position()
                 while depth > 0:
                     if text in BRACKETS_CLOSE:
                         other = doc.find(
                             text, start - 1,
-                            QtGui.QTextDocument.FindBackward)
+                            QtGui.QTextDocument.FindFlag.FindBackward)
                         match = doc.find(
                             BRACKETS[text], start - 1,
-                            QtGui.QTextDocument.FindBackward)
+                            QtGui.QTextDocument.FindFlag.FindBackward)
                     else:
                         other = doc.find(text, start)
                         match = doc.find(BRACKETS[text], start)
                     if match.isNull():
                         break
                     if other.isNull():
                         depth -= 1
@@ -218,19 +223,28 @@
         return (line, char)
 
     def _default_settings(self):
         """ Applies this editor's default settings. """
         # Set font
         self.setFont(FONT)
         # Set frame
-        self.setFrameStyle(QtWidgets.QFrame.WinPanel | QtWidgets.QFrame.Sunken)
+        self.setFrameStyle(
+            QtWidgets.QFrame.Shape.WinPanel | QtWidgets.QFrame.Shadow.Sunken)
         # Disable wrapping
-        self.setLineWrapMode(self.NoWrap)
+        self.setLineWrapMode(QtWidgets.QPlainTextEdit.LineWrapMode.NoWrap)
         # Set tab width (if ever seen) to 4 spaces
-        self.setTabStopWidth(self.fontMetrics().width(' ' * 4))
+        try:
+            # https://doc.qt.io/qt-5/qtextedit-obsolete.html
+            # https://doc.qt.io/qt-5/qfontmetrics.html#horizontalAdvance
+            # Qt 5.10/5.11 and onwards
+            ts = self.fontMetrics().horizontalAdvance(' ' * 4)
+            self.setTabStopDistance(ts)
+        except AttributeError:
+            ts = self.fontMetrics().width(' ' * 4)
+            self.setTabStopWidth(ts)
 
     def get_text(self):
         """ Returns the text in this editor. """
         return self.toPlainText()
 
     def jump_to(self, line, char):
         """ Jumps to the given line and row (with indices starting at 0). """
@@ -238,28 +252,35 @@
         cursor = self.textCursor()
         cursor.setPosition(block.position() + char)
         self.setTextCursor(cursor)
         self.centerCursor()
 
     def keyPressEvent(self, event):
         """ Qt event: A key was pressed. """
+        K = Qt.Key
+        KM = Qt.KeyboardModifier
+        MM = QtGui.QTextCursor.MoveMode
+        MO = QtGui.QTextCursor.MoveOperation
+
         # Get key and modifiers
         key = event.key()
         mod = event.modifiers()
         # Possible modifiers:
         #  NoModifier
         #  ShiftModifier, ControlModifier, AltModifiier
         #  MetaModifier (i.e. super key)
         #  KeyPadModifier (button is part of keypad)
         #  GroupSwitchModifier (x11 thing)
+
         # Ignore the keypad modifier, we don't care!
-        if mod & Qt.KeypadModifier:
-            mod = mod ^ Qt.KeypadModifier   # xor!
+        if mod & KM.KeypadModifier:
+            mod = mod ^ KM.KeypadModifier   # xor!
+
         # Actions per key/modifier combination
-        if key == Qt.Key_Tab and mod == Qt.NoModifier:
+        if key == K.Key_Tab and mod == KM.NoModifier:
             # Indent
             cursor = self.textCursor()
             start, end = cursor.selectionStart(), cursor.selectionEnd()
             if cursor.hasSelection():
                 # Add single tab to all lines in selection
                 cursor.beginEditBlock()     # Undo grouping
                 doc = self.document()
@@ -271,15 +292,15 @@
                     b = b.next()
                 cursor.endEditBlock()
             else:
                 # Insert spaces until next tab stop
                 pos = cursor.positionInBlock()
                 cursor.insertText((TABS - pos % TABS) * SPACE)
 
-        elif key == Qt.Key_Backtab and mod == Qt.ShiftModifier:
+        elif key == K.Key_Backtab and mod == KM.ShiftModifier:
             # Dedent all lines in selection (or single line if no selection)
             '''
             cursor = self.textCursor()
             start, end = cursor.selectionStart(), cursor.selectionEnd()
             cursor.beginEditBlock() # Undo grouping
             doc = self.document()
             # Get blocks in selection
@@ -291,19 +312,19 @@
             # Dedent
             for b in blocks:
                 t = b.text()
                 p1 = b.position()
                 p2 = p1 + min(4, len(t) - len(t.lstrip()))
                 c = self.textCursor()
                 c.setPosition(p1)
-                c.setPosition(p2, QtGui.QTextCursor.KeepAnchor)
+                c.setPosition(p2, MM.KeepAnchor)
                 c.removeSelectedText()
             cursor.endEditBlock()
             '''
-            # This silly method is required because of a bug in qt4/qt5
+            # This silly method is required because of a bug in qt5 (and 6?)
             cursor = self.textCursor()
             start, end = cursor.selectionStart(), cursor.selectionEnd()
             first = self.document().findBlock(start)
             q = 0
             new_text = []
             new_start, new_end = start, end
             b = QtGui.QTextBlock(first)
@@ -320,30 +341,29 @@
             new_start = max(new_start, first.position())
             new_end = max(new_end, new_start)
             if q > 0:
                 # Cut text, replace with new
                 cursor.beginEditBlock()
                 cursor.setPosition(first.position())
                 cursor.setPosition(
-                    last.position() + last.length() - 1,
-                    QtGui.QTextCursor.KeepAnchor)
+                    last.position() + last.length() - 1, MM.KeepAnchor)
                 cursor.removeSelectedText()
                 cursor.insertText('\n'.join(new_text))
                 cursor.endEditBlock()
                 # Set new cursor
                 cursor.setPosition(new_start)
-                cursor.setPosition(new_end, QtGui.QTextCursor.KeepAnchor)
+                cursor.setPosition(new_end, MM.KeepAnchor)
                 self.setTextCursor(cursor)
 
-        elif key == Qt.Key_Enter or key == Qt.Key_Return:
+        elif key == K.Key_Enter or key == K.Key_Return:
             # Enter/Return with modifier is overruled here to mean nothing
             # This is very important as the default for shift-enter is to
             # start a new line within the same block (this can't happen with
             # copy-pasting, so it's safe to just catch it here).
-            if mod == Qt.NoModifier:
+            if mod == KM.NoModifier:
                 # "Smart" enter:
                 #   - If selection, selection is deleted
                 #   - Else, autoindenting is performed
                 cursor = self.textCursor()
                 cursor.beginEditBlock()
                 if cursor.hasSelection():
                     # Replace selection with newline,
@@ -357,16 +377,16 @@
                     i = i[:cursor.positionInBlock()]
                     cursor.insertBlock()
                     cursor.insertText(i)
                 cursor.endEditBlock()
                 # Scroll if necessary
                 self.ensureCursorVisible()
 
-        elif key == Qt.Key_Home and (
-                mod == Qt.NoModifier or mod == Qt.ShiftModifier):
+        elif key == K.Key_Home and (
+                mod == KM.NoModifier or mod == KM.ShiftModifier):
             # Plain home button: move to start of line
             # If Control is used: Jump to start of document
             # Ordinary home button: Jump to first column or first
             # non-whitespace character
             cursor = self.textCursor()
             block = cursor.block()
             cp = cursor.position()
@@ -381,33 +401,30 @@
                 # end of line if all whitespace
                 t = block.text()
                 indent = len(t) - len(t.lstrip())
                 newpos = bp + indent
                 # Smart up/down:
                 self._last_column = indent
             # If Shift is used: only move position (keep anchor, i.e. select)
-            anchor = (
-                QtGui.QTextCursor.KeepAnchor if mod == Qt.ShiftModifier
-                else QtGui.QTextCursor.MoveAnchor)
-            cursor.setPosition(newpos, anchor)
+            cursor.setPosition(
+                newpos,
+                MM.KeepAnchor if mod == KM.ShiftModifier else MM.MoveAnchor)
             self.setTextCursor(cursor)
 
-        elif key == Qt.Key_Home and (
-                mod == Qt.ControlModifier
-                or mod == Qt.ControlModifier & Qt.ShiftModifier):
+        elif key == K.Key_Home and (
+                mod == KM.ControlModifier
+                or mod == KM.ControlModifier & KM.ShiftModifier):
             # Move to start of document
             # If Shift is used: only move position (keep anchor, i.e. select)
-            anchor = (
-                QtGui.QTextCursor.KeepAnchor if mod == Qt.ShiftModifier
-                else QtGui.QTextCursor.MoveAnchor)
             cursor = self.textCursor()
-            cursor.setPosition(0, anchor)
+            cursor.setPosition(
+                0, MM.KeepAnchor if mod == KM.ShiftModifier else MM.MoveAnchor)
             self.setTextCursor(cursor)
 
-        elif key in (Qt.Key_Up, Qt.Key_Down) and mod == Qt.AltModifier:
+        elif key in (K.Key_Up, K.Key_Down) and mod == KM.AltModifier:
             # Move selected lines up or down
             # Get current selection
             doc = self.document()
             cursor = self.textCursor()
             start, end = cursor.selectionStart(), cursor.selectionEnd()
             block1 = doc.findBlock(start)
             if start == end:
@@ -416,88 +433,85 @@
                 block2 = doc.findBlock(end)
                 # Whole line selection? Then move end back 1 position
                 if end == block2.position():
                     end -= 1
                     block2 = block2.previous()  # always valid
             block2 = block1 if start == end else doc.findBlock(end)
             # Check if we can move
-            if key == Qt.Key_Up:
+            if key == K.Key_Up:
                 if not block1.previous().isValid():
                     return
             elif not block2.next().isValid():
                 return
             # Select full line(s)
             b1pos = block1.position()
             cursor.beginEditBlock()
             cursor.setPosition(b1pos)
-            cursor.setPosition(end, QtGui.QTextCursor.KeepAnchor)
-            cursor.movePosition(
-                QtGui.QTextCursor.EndOfLine, QtGui.QTextCursor.KeepAnchor)
+            cursor.setPosition(end, MM.KeepAnchor)
+            cursor.movePosition(MO.EndOfLine, MM.KeepAnchor)
             line = cursor.selectedText()
             size = cursor.selectionEnd() - cursor.selectionStart()
             cursor.removeSelectedText()
-            if key == Qt.Key_Up:
+            if key == K.Key_Up:
                 cursor.deletePreviousChar()
-                cursor.movePosition(QtGui.QTextCursor.StartOfLine)
+                cursor.movePosition(MO.StartOfLine)
                 cursor.insertText(line + '\n')
-                cursor.movePosition(QtGui.QTextCursor.Left)
+                cursor.movePosition(MO.Left)
             else:
                 cursor.deleteChar()
-                cursor.movePosition(QtGui.QTextCursor.EndOfLine)
+                cursor.movePosition(MO.EndOfLine)
                 cursor.insertText('\n' + line)
             cursor.endEditBlock()
             # Cursor is at the end of the moved lines.
             # Set moved lines as selection
-            cursor.movePosition(
-                QtGui.QTextCursor.Left, QtGui.QTextCursor.KeepAnchor, size)
+            cursor.movePosition(MO.Left, MM.KeepAnchor, size)
             self.setTextCursor(cursor)
 
-        elif key in (Qt.Key_Up, Qt.Key_Down, Qt.Key_PageUp, Qt.Key_PageDown) \
-                and (mod == Qt.NoModifier or mod == Qt.ShiftModifier):
+        elif key in (K.Key_Up, K.Key_Down, K.Key_PageUp, K.Key_PageDown) \
+                and (mod == KM.NoModifier or mod == KM.ShiftModifier):
             # Move cursor up/down
             # Maintain the column position, even when the current row doesn't
             # have as many characters. Reset this behavior as soon as a
             # left/right home/end action is made or whenever the text is
             # changed.
             # Set up operation
             anchor = (
-                QtGui.QTextCursor.KeepAnchor if mod == Qt.ShiftModifier
-                else QtGui.QTextCursor.MoveAnchor)
-            operation = \
-                QtGui.QTextCursor.PreviousBlock if key in (
-                    Qt.Key_Up, Qt.Key_PageUp) else QtGui.QTextCursor.NextBlock
-            n = 1 if key in (Qt.Key_Up, Qt.Key_Down) else (
+                MM.KeepAnchor if mod == KM.ShiftModifier else MM.MoveAnchor)
+            operation = (MO.PreviousBlock if key in (K.Key_Up, K.Key_PageUp)
+                         else MO.NextBlock)
+            n = 1 if key in (K.Key_Up, K.Key_Down) else (
                 self._blocks_per_page - 3)
+
             # Move
             cursor = self.textCursor()
             if self._last_column is None:
                 # Update "smart" column
                 self._last_column = cursor.positionInBlock()
             if cursor.movePosition(operation, anchor, n):
                 column = min(cursor.block().length() - 1, self._last_column)
                 cursor.setPosition(cursor.position() + column, anchor)
             else:
                 # Up/Down beyond document start/end? Move cursor to document
                 # start/end and update last column
-                if operation == QtGui.QTextCursor.NextBlock:
-                    cursor.movePosition(QtGui.QTextCursor.EndOfBlock, anchor)
+                if operation == MO.NextBlock:
+                    cursor.movePosition(MO.EndOfBlock, anchor)
                 else:
-                    cursor.movePosition(QtGui.QTextCursor.StartOfBlock, anchor)
+                    cursor.movePosition(MO.StartOfBlock, anchor)
                 self._last_column = cursor.positionInBlock()
             self.setTextCursor(cursor)
 
-        elif key in (Qt.Key_Left, Qt.Key_Right, Qt.Key_End) and not (
-                mod & Qt.AltModifier):
+        elif key in (K.Key_Left, K.Key_Right, K.Key_End) and not (
+                mod & KM.AltModifier):
             # Allow all modifiers except alt
             # Reset smart up/down behavior
             self._last_column = None
             # Pass to parent class
-            super(Editor, self).keyPressEvent(event)
+            super().keyPressEvent(event)
 
-        elif key == Qt.Key_Insert and mod == Qt.NoModifier:
+        elif key == K.Key_Insert and mod == KM.NoModifier:
             # Insert/replace
             self.setOverwriteMode(not self.overwriteMode())
 
         else:
             # Default keyboard shortcuts / functions:
             # Backspace             OK
             # Delete                OK
@@ -526,28 +540,34 @@
             # Alt+Wheel             OK (Horizontal scrolling)
             # Control+Wheel         OK (Fast scrolling)
             # Control+K             Removed
             # Not listed, but very important:
             # Shift-Enter           Starts new line within the same block!
             #                       Definitely removed
             # Ctrl-i                Undocumented, but inserts tab...
-            ctrl_ignore = (Qt.Key_K, Qt.Key_I)
-            if mod == Qt.ControlModifier and key in ctrl_ignore:
+            ctrl_ignore = (K.Key_K, K.Key_I)
+            if mod == KM.ControlModifier and key in ctrl_ignore:
                 # Control-K: ignore
                 pass
-            elif key == Qt.Key_Up or key == Qt.Key_Down:
+            elif key == K.Key_Up or key == K.Key_Down:
                 # Up/down with modifiers: ignore
                 pass
             else:
                 # Let parent class handle it
-                super(Editor, self).keyPressEvent(event)
+                super().keyPressEvent(event)
 
     def _line_number_area_width(self):
         """ Returns the required width for the number area. """
-        return 8 + self.fontMetrics().width(str(max(1, self.blockCount())))
+        text = str(max(1, self.blockCount()))
+        try:
+            # https://doc.qt.io/qt-5/qfontmetrics.html#horizontalAdvance
+            # Qt 5.5.11 and onwards
+            return 8 + self.fontMetrics().horizontalAdvance(text)
+        except AttributeError:
+            return 8 + self.fontMetrics().width(text)
 
     def _line_number_area_paint(self, area, event):
         """ Repaints the line number area. """
         # Area to repaint
         rect = event.rect()
         etop = rect.top()
         ebot = rect.bottom()
@@ -569,25 +589,25 @@
         bbot = int(btop + geom.height())
 
         # Iterate over visible blocks
         count = block.blockNumber()
         while block.isValid() and btop <= ebot:
             count += 1
             if block.isVisible() and bbot >= etop:
-                painter.drawText(
-                    0, btop, width - 4, height, Qt.AlignRight, str(count))
+                painter.drawText(0, btop, width - 4, height,
+                                 Qt.AlignmentFlag.AlignRight, str(count))
             block = block.next()
             btop = bbot
             bbot += int(self.blockBoundingRect(block).height())
 
     def paintEvent(self, e):
         """ Paints this editor. """
 
         # Paint the editor
-        super(Editor, self).paintEvent(e)
+        super().paintEvent(e)
 
         # Paint a line between the editor and the line number area
         x = int(
             self.contentOffset().x()
             + self.document().documentMargin()
             + self._line_offset
         )
@@ -606,15 +626,15 @@
         cursor.beginEditBlock()
         cursor.removeSelectedText()
         self.appendPlainText(str(text))
         cursor.endEditBlock()
 
     def resizeEvent(self, event):
         """ Qt event: Editor is resized. """
-        super(Editor, self).resizeEvent(event)
+        super().resizeEvent(event)
         # Update line number area
         rect = self.contentsRect()
         self._line_number_area.setGeometry(
             rect.left(), rect.top(),
             self._line_number_area_width(), rect.height())
         # Set number of "blocks" per page
         font = self.fontMetrics()
@@ -673,24 +693,26 @@
                 remove = False
                 break
         cursor.beginEditBlock()
         if remove:
             for block in blocks:
                 p = block.position() + indent
                 cursor.setPosition(p)
-                cursor.setPosition(p + 1, QtGui.QTextCursor.KeepAnchor)
+                cursor.setPosition(
+                    p + 1, QtGui.QTextCursor.MoveMode.KeepAnchor)
                 cursor.removeSelectedText()
         else:
 
             for block in blocks:
                 p = block.position()
                 n = len(block.text())
                 if len(block.text()) < indent:
                     cursor.setPosition(p)
-                    cursor.setPosition(p + n, QtGui.QTextCursor.KeepAnchor)
+                    cursor.setPosition(
+                        p + n, QtGui.QTextCursor.MoveMode.KeepAnchor)
                     cursor.removeSelectedText()
                     cursor.insertText(' ' * indent + '#')
                 else:
                     cursor.setPosition(p + indent)
                     cursor.insertText('#')
         cursor.endEditBlock()
 
@@ -701,16 +723,16 @@
         cursor.beginEditBlock()     # Undo grouping
         while block.isValid():
             t = block.text()
             a = len(t)
             b = len(t.rstrip())
             if a > b:
                 cursor.setPosition(block.position() + b)
-                cursor.setPosition(
-                    block.position() + a, QtGui.QTextCursor.KeepAnchor)
+                cursor.setPosition(block.position() + a,
+                                   QtGui.QTextCursor.MoveMode.KeepAnchor)
                 cursor.removeSelectedText()
             block = block.next()
         cursor.endEditBlock()
 
 
 class LineNumberArea(QtWidgets.QWidget):
     """
@@ -718,15 +740,15 @@
     the text area class.
 
     The line number is drawn in the left margin of the :class:`Editor` widget,
     the space to do so is created by setting the editor's viewport margins.
     """
 
     def __init__(self, editor):
-        super(LineNumberArea, self).__init__(editor)
+        super().__init__(editor)
         self._editor = editor
         self._editor.blockCountChanged.connect(self.update_width)
         self._editor.updateRequest.connect(self.update_contents)
 
     def paintEvent(self, event):
         """ Qt event: Paint this area. """
         self._editor._line_number_area_paint(self, event)
@@ -762,15 +784,15 @@
     Find/replace widget for :class:`Editor`.
     """
     # Signal: Find action happened, update with text
     # Attributes: (description)
     find_action = QtCore.Signal(str)
 
     def __init__(self, parent, editor):
-        super(FindReplaceWidget, self).__init__(parent)
+        super().__init__(parent)
         self._editor = editor
 
         # Create widgets
         self._replace_all_button = QtWidgets.QPushButton('Replace all')
         self._replace_all_button.clicked.connect(self.action_replace_all)
         self._replace_button = QtWidgets.QPushButton('Replace')
         self._replace_button.clicked.connect(self.action_replace)
@@ -785,23 +807,25 @@
 
         # Create layout
         text_layout = QtWidgets.QGridLayout()
         text_layout.addWidget(self._search_label, 0, 0)
         text_layout.addWidget(self._search_field, 0, 1)
         text_layout.addWidget(self._replace_label, 1, 0)
         text_layout.addWidget(self._replace_field, 1, 1)
-        check_layout = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.TopToBottom)
+        check_layout = QtWidgets.QBoxLayout(
+            QtWidgets.QBoxLayout.Direction.TopToBottom)
         check_layout.addWidget(self._case_check)
         check_layout.addWidget(self._whole_check)
         button_layout = QtWidgets.QGridLayout()
         button_layout.addWidget(self._replace_all_button, 0, 1)
         button_layout.addWidget(self._replace_button, 0, 2)
         button_layout.addWidget(self._find_button, 0, 3)
 
-        layout = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.TopToBottom)
+        layout = QtWidgets.QBoxLayout(
+            QtWidgets.QBoxLayout.Direction.TopToBottom)
         layout.addLayout(text_layout)
         layout.addLayout(check_layout)
         layout.addLayout(button_layout)
         layout.addStretch(1)
         self.setLayout(layout)
 
         # Accept keyboard focus on search and replace fields
@@ -810,19 +834,19 @@
 
     def action_find(self):
         """ Qt slot: Find (next) item. """
         query = self._search_field.text()
         if query == '':
             self.find_action.emit('No query set')
             return
-        flags = 0x0
+        flags = QtGui.QTextDocument.FindFlag(0)
         if self._case_check.isChecked():
-            flags |= QtGui.QTextDocument.FindCaseSensitively
+            flags |= QtGui.QTextDocument.FindFlag.FindCaseSensitively
         if self._whole_check.isChecked():
-            flags |= QtGui.QTextDocument.FindWholeWords
+            flags |= QtGui.QTextDocument.FindFlag.FindWholeWords
         if flags:
             found = self._editor.find(query, flags)
         else:
             found = self._editor.find(query)
         if found is False:
             # Not found? Try from top of document
             previous_cursor = self._editor.textCursor()
@@ -863,19 +887,19 @@
     def action_replace_all(self):
         """ Qt slot: Replace all found items with replacement """
         query = self._search_field.text()
         replacement = self._replace_field.text()
         if query == '':
             self.find_action.emit('No query set')
             return
-        flags = 0x0
+        flags = QtGui.QTextDocument.FindFlag(0)
         if self._case_check.isChecked():
-            flags |= QtGui.QTextDocument.FindCaseSensitively
+            flags |= QtGui.QTextDocument.FindFlag.FindCaseSensitively
         if self._whole_check.isChecked():
-            flags |= QtGui.QTextDocument.FindWholeWords
+            flags |= QtGui.QTextDocument.FindFlag.FindWholeWords
         n = 0
         found = True
         scrollpos = self._editor.verticalScrollBar().value()
         grouping = self._editor.textCursor()
         grouping.beginEditBlock()
         continue_from_top = True
         while found:
@@ -913,18 +937,18 @@
             self._search_field.setText(cursor.selectedText())
         self._search_field.selectAll()
         self._search_field.setFocus()
 
     def keyPressEvent(self, event):
         """ Qt event: A key-press reaches the widget. """
         key = event.key()
-        if key == Qt.Key_Enter or key == Qt.Key_Return:
+        if key == Qt.Key.Key_Enter or key == Qt.Key.Key_Return:
             self.action_find()
         else:
-            super(FindReplaceWidget, self).keyPressEvent(event)
+            super().keyPressEvent(event)
 
     def load_config(self, config, section):
         """
         Loads this search's configuration using the given :class:`ConfigParser`
         ``config``. Loads all settings from the section ``section``.
         """
         if config.has_section(section):
@@ -952,401 +976,408 @@
     Syntax highlighter for ``mmt`` model definitions.
     """
     KEYWORD_1 = ['use', 'as']
     KEYWORD_2 = ['and', 'or', 'not']
     ANNOT_KEYS = ['in', 'bind', 'label']
 
     def __init__(self, document):
-        super(ModelHighlighter, self).__init__(document)
+        super().__init__(document)
 
         # Expressions used to find strings & comments
-        self._string_start = QtCore.QRegExp(r'"""')
-        self._string_stop = QtCore.QRegExp(r'"""')
-        self._comment_start = QtCore.QRegExp(r'#[^\n]*')
+        R = QtCore.QRegularExpression
+        self._string = R(r'"""')
 
         # Headers
         name = r'[a-zA-Z]+[a-zA-Z0-9_]*'
-        self._rule_head = QtCore.QRegExp(r'^(\s*)\[{1,2}' + name + '\]{1,2}')
+        self._rule_head = R(r'^\s*(\[{1,2}' + name + '\]{1,2})')
 
         # Simple rules
         self._rules = []
 
         # Numbers
-        pattern = QtCore.QRegExp(r'\b[+-]?[0-9]*\.?[0-9]+([eE][+-]?[0-9]+)?\b')
+        pattern = R(r'\b[+-]?[0-9]*\.?[0-9]+([eE][+-]?[0-9]+)?\b')
         self._rules.append((pattern, STYLE_LITERAL))
-        unit = r'\[[a-zA-Z0-9/^-*]+\]'
-        self._rules.append((QtCore.QRegExp(unit), STYLE_INLINE_UNIT))
+        unit = r'\[([a-zA-Z0-9/^-]|\*)+\]'
+        self._rules.append((R(unit), STYLE_INLINE_UNIT))
 
         # Keywords
         for keyword in self.KEYWORD_1:
-            pattern = QtCore.QRegExp(r'\b' + keyword + r'\b')
-            self._rules.append((pattern, STYLE_KEYWORD_1))
+            self._rules.append((R(r'\b' + keyword + r'\b'), STYLE_KEYWORD_1))
         for keyword in self.KEYWORD_2:
-            pattern = QtCore.QRegExp(r'\b' + keyword + r'\b')
-            self._rules.append((pattern, STYLE_KEYWORD_2))
+            self._rules.append((R(r'\b' + keyword + r'\b'), STYLE_KEYWORD_2))
 
         # Meta-data coloring
         self._rules_labels = [
-            QtCore.QRegExp(r'(\s*)(bind)\s+(' + name + ')'),
-            QtCore.QRegExp(r'(\s*)(label)\s+(' + name + ')'),
+            R(r'(\s*)(bind)\s+(' + name + ')'),
+            R(r'(\s*)(label)\s+(' + name + ')'),
         ]
-        self._rule_meta_key = QtCore.QRegExp(name + r':')
-        self._rule_meta_val = QtCore.QRegExp(r':(\s*)(.+)')
-        self._rule_var_unit = QtCore.QRegExp(r'^(\s*)(in)(\s*)(' + unit + ')')
+        self._rule_meta = R(r'^\s*(' + name + r':)(\s*)(.+)')
+        self._rule_var_unit = R(r'^(\s*)(in)(\s*)(' + unit + ')')
 
-        # Comments
-        # Note: For some reason this can _not_ use self._comment_start
-        self._comments = QtCore.QRegExp(r'#[^\n]*')
+        # Comment
+        self._comment = R(r'#')
+
+    def _highlight_ok(self, strings, start, length):
+        """ Checks if the string ``start`` to ``length`` needs formatted. """
+        for lo, hi in strings:
+            if lo <= start < hi or lo <= start + length < hi:
+                return False
+        return True
 
     def highlightBlock(self, text):
         """ Qt: Called whenever a block should be highlighted. """
-        # Simple rules
-        for (pattern, style) in self._rules:
-            i = pattern.indexIn(text)
-            while i >= 0:
-                # Note: Can't use matchedLength() here because it does quirky
-                # things with the subgroup for the numbers regex.
-                n = len(pattern.cap(0))
-                self.setFormat(i, n, style)
-                i = pattern.indexIn(text, i + n)
-
-        # Model and component headers
-        i = self._rule_head.indexIn(text)
-        while i >= 0:
-            m = len(self._rule_head.cap(1))
-            n = len(self._rule_head.cap(0))
-            self.setFormat(i + m, n - m, STYLE_HEADER)
-            i = self._rule_head.indexIn(text, i + n)
 
-        # Annotations
-        # Labels
-        for pattern in self._rules_labels:
-            i = pattern.indexIn(text)
-            while i >= 0:
-                n0 = len(pattern.cap(0))
-                n1 = len(pattern.cap(1))
-                n2 = len(pattern.cap(2))
-                n3 = len(pattern.cap(3))
-                self.setFormat(i + n1, n2, STYLE_ANNOT_KEY)
-                self.setFormat(i + n0 - n3, n3, STYLE_ANNOT_VAL)
-                i = pattern.indexIn(text, i + n0)
-
-        # Units
-        i = self._rule_var_unit.indexIn(text)
-        if i == 0:
-            n1 = len(self._rule_var_unit.cap(1))
-            n2 = len(self._rule_var_unit.cap(2))
-            n3 = len(self._rule_var_unit.cap(3))
-            n4 = len(self._rule_var_unit.cap(4))
-            self.setFormat(n1, n2, STYLE_ANNOT_KEY)
-            self.setFormat(n1 + n2 + n3, n4, STYLE_ANNOT_VAL)
-
-        # Meta properties
-        i = self._rule_meta_key.indexIn(text)
-        if i >= 0:
-            n0 = len(self._rule_meta_key.cap(0))
-            self.setFormat(i, n0, STYLE_ANNOT_KEY)
-        i = self._rule_meta_val.indexIn(text)
-        if i >= 0:
-            n1 = len(self._rule_meta_val.cap(1))
-            n2 = len(self._rule_meta_val.cap(2))
-            self.setFormat(i, 1, STYLE_ANNOT_KEY)
-            self.setFormat(1 + i + n1, n2, STYLE_ANNOT_VAL)
-
-        # Comments (overrule all other formatting except multi-line strings)
-        i = self._comments.indexIn(text)
-        while i >= 0:
-            n = len(self._comments.cap(0))
-            self.setFormat(i, n, STYLE_COMMENT)
-            i = self._comments.indexIn(text, i + n)
-
-        # Multi-line strings
-        # Block states:
-        #  0 Normal
-        #  1 Multi-line string (meta)
+        # To avoid formatting within strings each is stored as a (start, end).
+        strings = []
+        # If the start has been handled, set the offset.
+        offset = 0
+        # If the end has been handled, chop it off the string
+
+        # Multi-line strings are done first, because they overrule a lot of
+        # things and we can skip formatting if we're inside one.
+        # Block states: 0=No string, 1=A """ string
         self.setCurrentBlockState(0)
 
-        # Check state of previous block
-        if self.previousBlockState() != 1:
-            # Normal block
-            next = start = self._string_start.indexIn(text)
-            comment = self._comment_start.indexIn(text)
-            if next >= 0 and (comment < 0 or comment > next):
-                next += self._string_start.matchedLength()
+        # Continuing a multi-line string?
+        if self.previousBlockState() == 1:
+            # Search for string stop
+            ms = self._string.match(text)
+            if ms.hasMatch():
+                # Terminate the multi-line string
+                offset = ms.capturedEnd(0)
+                self.setFormat(0, offset, STYLE_ANNOT_VAL)
             else:
-                start = next = -1
+                # Whole line in the string
+                self.setCurrentBlockState(1)
+                self.setFormat(0, len(text), STYLE_ANNOT_VAL)
+                return
         else:
-            start = next = 0
+            # Search for string start
+            ms = self._string.match(text)
+            if ms.hasMatch():
+                # Potential start, but check that it's not commented out
+                start = ms.capturedStart()
+                mc = self._comment.match(text)
+                if not (mc.hasMatch() and mc.capturedStart() < start):
+                    # Definitely a string start. See if it ends on this line
+                    me = self._string.match(text, offset=ms.capturedEnd())
+                    if me.hasMatch():
+                        # Terminate the single-line string
+                        end = me.capturedEnd()
+                        self.setFormat(start, end - start, STYLE_ANNOT_VAL)
+                        strings.append((start, end))
+                    else:
+                        # Multi-line string
+                        self.setCurrentBlockState(1)
+                        self.setFormat(start, len(text), STYLE_ANNOT_VAL)
+
+        # Comment
+        i = self._comment.globalMatch(text, offset=offset)
+        while i.hasNext():
+            m = i.next()
+            x = m.capturedStart()
+            if self._highlight_ok(strings, x, 1):
+                self.setFormat(x, len(text) - x, STYLE_COMMENT)
+                text = text[:x]
+                break
 
-        # Find any occurrences of string start / stop
-        while next >= 0:
-            stop = self._string_stop.indexIn(text, next)
-            if stop < 0:
-                # Continuing multi-line string
-                self.setCurrentBlockState(1)
-                self.setFormat(start, len(text) - start, STYLE_ANNOT_VAL)
-                next = -1
-            else:
-                # Ending single-line or multi-line string
-                # Format until stop token
-                next = stop = stop + self._string_stop.matchedLength()
-                self.setFormat(start, stop - start, STYLE_ANNOT_VAL)
-                # Find next string in block, if any
-                next = start = self._string_start.indexIn(text, next)
-                if next >= 0:
-                    next += self._string_start.matchedLength()
+        # Rule-based formatting
+        for (pattern, style) in self._rules:
+            i = pattern.globalMatch(text, offset=offset)
+            while i.hasNext():
+                m = i.next()
+                x, w = m.capturedStart(), m.capturedLength()
+                if self._highlight_ok(strings, x, w):
+                    self.setFormat(x, w, style)
+
+        # Model and component headers (must be at start of string)
+        if offset == 0:
+            m = self._rule_head.match(text)
+            if m.hasMatch():
+                x, w = m.capturedStart(1), m.capturedLength(1)
+                self.setFormat(x, w, STYLE_HEADER)
+
+        # Variable units (must be at start of string)
+        if offset == 0:
+            m = self._rule_var_unit.match(text)
+            if m.hasMatch():
+                self.setFormat(
+                    m.capturedStart(2), m.capturedLength(2), STYLE_ANNOT_KEY)
+                self.setFormat(
+                    m.capturedStart(4), m.capturedLength(4), STYLE_ANNOT_VAL)
+
+        # Binds and labels
+        for pattern in self._rules_labels:
+            i = pattern.globalMatch(text, offset=offset)
+            while i.hasNext():
+                m = i.next()
+                x, w = m.capturedStart(), m.capturedLength()
+                if self._highlight_ok(strings, x, w):
+                    self.setFormat(m.capturedStart(2), m.capturedLength(2),
+                                   STYLE_ANNOT_KEY)
+                    self.setFormat(m.capturedStart(3), m.capturedLength(3),
+                                   STYLE_ANNOT_VAL)
+
+        # Meta properties (must be at start of string)
+        if offset == 0:
+            m = self._rule_meta.match(text)
+            if m.hasMatch():
+                self.setFormat(
+                    m.capturedStart(1), m.capturedLength(1), STYLE_ANNOT_KEY)
+                # Don't reformat strings (or bits after string end!)
+                if m.captured(3)[:3] != '"""':
+                    self.setFormat(m.capturedStart(3), m.capturedLength(3),
+                                   STYLE_ANNOT_VAL)
 
 
 class ProtocolHighlighter(QtGui.QSyntaxHighlighter):
     """
     Syntax highlighter for ``mmt`` protocol definitions.
     """
     def __init__(self, document):
-        super(ProtocolHighlighter, self).__init__(document)
+        super().__init__(document)
 
         # Headers and units
-        self._rule_head = QtCore.QRegExp(r'^(\s*)\[\[[a-zA-Z0-9_]+\]\]')
+        R = QtCore.QRegularExpression
+        self._rule_head = R(r'^\s*(\[\[[a-zA-Z0-9_]+\]\])')
 
         # Highlighting rules
         self._rules = []
 
         # Numbers
-        pattern = QtCore.QRegExp(r'\b[+-]?[0-9]*\.?[0-9]+([eE][+-]?[0-9]+)?\b')
-        self._rules.append((pattern, STYLE_LITERAL))
+        self._rules.append(
+            (R(r'\b[+-]?[0-9]*\.?[0-9]+([eE][+-]?[0-9]+)?\b'), STYLE_LITERAL))
 
         # Keyword "next"
-        pattern = QtCore.QRegExp(r'\bnext\b')
-        self._rules.append((pattern, STYLE_KEYWORD_1))
+        self._rules.append((R(r'\bnext\b'), STYLE_KEYWORD_1))
 
         # Comments
-        pattern = QtCore.QRegExp(r'#[^\n]*')
-        self._rules.append((pattern, STYLE_COMMENT))
+        self._rules.append((R(r'#[^\n]*'), STYLE_COMMENT))
 
     def highlightBlock(self, text):
         """ Qt: Called whenever a block should be highlighted. """
+
         # Rule based formatting
         for (pattern, style) in self._rules:
-            i = pattern.indexIn(text)
-            while i >= 0:
-                n = len(pattern.cap(0))
-                self.setFormat(i, n, style)
-                i = pattern.indexIn(text, i + n)
-
-        # Protocol header
-        i = self._rule_head.indexIn(text)
-        while i >= 0:
-            m = len(self._rule_head.cap(1))
-            n = len(self._rule_head.cap(0))
-            self.setFormat(i + m, n - m, STYLE_HEADER)
-            i = self._rule_head.indexIn(text, i + n)
+            i = pattern.globalMatch(text)
+            while i.hasNext():
+                m = i.next()
+                self.setFormat(m.capturedStart(), m.capturedLength(), style)
+
+        # Protocol header (must be at strart of string)
+        m = self._rule_head.match(text)
+        if m.hasMatch():
+            self.setFormat(
+                m.capturedStart(1), m.capturedLength(1), STYLE_HEADER)
 
 
 class ScriptHighlighter(QtGui.QSyntaxHighlighter):
     """
     Syntax highlighter for ``mmt`` script files.
     """
     def __init__(self, document):
-        super(ScriptHighlighter, self).__init__(document)
+        super().__init__(document)
 
-        # Headers and units
-        self._rule_head = QtCore.QRegExp(r'^(\s*)\[\[[a-zA-Z0-9_]+\]\]')
+        # Script header
+        R = QtCore.QRegularExpression
+        self._rule_head = R(r'^\s*(\[\[[a-zA-Z0-9_]+\]\])')
 
         # Highlighting rules
         self._rules = []
 
         # Keywords
         import keyword
         for kw in keyword.kwlist:
-            pattern = QtCore.QRegExp(r'\b' + kw + r'\b')
-            self._rules.append((pattern, STYLE_KEYWORD_1))
+            self._rules.append((R(r'\b' + kw + r'\b'), STYLE_KEYWORD_1))
 
         # Built-in essential functions
         for func in _PYFUNC:
-            pattern = QtCore.QRegExp(r'\b' + str(func) + r'\b')
-            self._rules.append((pattern, STYLE_KEYWORD_2))
+            self._rules.append((R(r'\b' + str(func) + r'\b'), STYLE_KEYWORD_2))
 
         # Literals: numbers, True, False, None
         # Override some keywords
-        pattern = QtCore.QRegExp(r'\b[+-]?[0-9]*\.?[0-9]+([eE][+-]?[0-9]+)?\b')
-        self._rules.append((pattern, STYLE_LITERAL))
-        pattern = QtCore.QRegExp(r'\bTrue\b')
-        self._rules.append((pattern, STYLE_LITERAL))
-        pattern = QtCore.QRegExp(r'\bFalse\b')
-        self._rules.append((pattern, STYLE_LITERAL))
-        pattern = QtCore.QRegExp(r'\bNone\b')
-        self._rules.append((pattern, STYLE_LITERAL))
+        self._rules.append((R(r'\b[+-]?[0-9]*\.?[0-9]+([eE][+-]?[0-9]+)?\b'),
+                            STYLE_LITERAL))
+        self._rules.append((R(r'\bTrue\b'), STYLE_LITERAL))
+        self._rules.append((R(r'\bFalse\b'), STYLE_LITERAL))
+        self._rules.append((R(r'\bNone\b'), STYLE_LITERAL))
 
         # Strings
-        pattern = QtCore.QRegExp(r'"([^"\\]|\\")*"')
-        self._rules.append((pattern, STYLE_LITERAL))
-        pattern = QtCore.QRegExp(r"'([^'\\]|\\')*'")
-        self._rules.append((pattern, STYLE_LITERAL))
-
-        # Multi-line strings
-        self._string1 = QtCore.QRegExp(r"'''")
-        self._string2 = QtCore.QRegExp(r'"""')
+        self._s1 = R(r'"')
+        self._s2 = R(r"'")
+        self._ms1 = R(r'"""')
+        self._ms2 = R(r"'''")
+        self._s_start = R(r'"""|\'\'\'|"|\'')
+        self._s_end = {
+            '"': self._s1, "'": self._s2, '"""': self._ms1, "'''": self._ms2}
 
         # Comments
-        pattern = QtCore.QRegExp(r'#[^\n]*')
-        self._rules.append((pattern, STYLE_COMMENT))
+        self._comment = R(r'#')
+
+    def _highlight_ok(self, strings, start, length):
+        """ Checks if the string ``start`` to ``length`` needs formatted. """
+        for lo, hi in strings:
+            if lo <= start < hi or lo <= start + length < hi:
+                return False
+        return True
 
     def highlightBlock(self, text):
         """ Qt: Called whenever a block should be highlighted. """
-        # Rule based formatting
-        for (pattern, style) in self._rules:
-            i = pattern.indexIn(text)
-            while i >= 0:
-                # Note: Can't use matchedLength() here because it does quirky
-                # things with the subgroup for the numbers regex.
-                n = len(pattern.cap(0))
-                self.setFormat(i, n, style)
-                i = pattern.indexIn(text, i + n)
 
-        # Script header
-        i = self._rule_head.indexIn(text)
-        while i >= 0:
-            m = len(self._rule_head.cap(1))
-            n = len(self._rule_head.cap(0))
-            self.setFormat(i + m, n - m, STYLE_HEADER)
-            i = self._rule_head.indexIn(text, i + n)
-
-        # Block states:
-        #  0 Normal
-        #  1 Multi-line string 1
-        #  2 Multi-line string 2
+        # To avoid formatting within strings each is stored as a (start, end).
+        strings = []
+        # If the start has been handled, set the offset.
+        offset = 0
+        # If the end has been handled, chop it off the string
+
+        # Multi-line strings are done first, because they overrule a lot of
+        # things and we can skip formatting if we're inside one.
+        # Block states: 0=No string, 1=A " " " string, 2=A ' ' ' string
         self.setCurrentBlockState(0)
 
-        # Multi-line formats
-        def find_start(text, next):
-            s1 = self._string1.indexIn(text, next)
-            s2 = self._string2.indexIn(text, next)
-            if s1 < 0 and s2 < 0:
-                current = 0
-                start = -1
-                next = -1
-            else:
-                if s1 >= 0 and s2 >= 0:
-                    current = 1 if s1 < s2 else 2
-                    start = min(s1, s2)
-                elif s1 >= 0:
-                    current = 1
-                    start = s1
-                else:   # (s2 >= 0)
-                    current = 2
-                    start = s2
-                next = start + 3
-
-                # Check we're not in a comment
-                i = text.rfind('\n', start) + 1
-                if text[i:i + 1] == '#':
-                    current = 0
-                    start = next = -1
-
-            return current, start, next
-
-        # Check state of previous block
+        # Continuing a multi-line string?
         previous = self.previousBlockState()
         if previous == 1 or previous == 2:
-            current, start, next = previous, 0, 0
-        else:
-            current, start, next = find_start(text, 0)
-
-        # Find any occurrences of string start / stop
-        while next >= 0:
-            if current == 1:
-                stop = self._string1.indexIn(text, next)
+            # Search for string stop
+            r = self._ms1 if previous == 1 else self._ms2
+            ms = r.match(text)
+            if ms.hasMatch():
+                # Terminate the multi-line string, and increase global offset
+                offset = ms.capturedEnd(0)
+                self.setFormat(0, offset, STYLE_LITERAL)
             else:
-                stop = self._string2.indexIn(text, next)
-            if stop < 0:
-                # Continuing multi-line string
-                self.setCurrentBlockState(current)
-                self.setFormat(start, len(text) - start, STYLE_LITERAL)
-                next = -1
+                # Whole line in the string
+                self.setCurrentBlockState(previous)
+                self.setFormat(0, len(text), STYLE_LITERAL)
+                return
+
+        # Search for string starts (single or multi-line)
+        stroff = offset     # Offset for string start/end searching
+        m1 = self._s_start.match(text, offset=stroff)
+        while m1.hasMatch():
+            stroff = m1.capturedEnd()
+            start = m1.capturedStart()
+            # Are we in a comment?
+            mc = self._comment.match(text)
+            if (mc.hasMatch() and mc.capturedStart() < start):
+                # No point searching for further string starts
+                stroff = len(text)
             else:
-                # Ending single-line or multi-line string
-                # Format until stop token
-                stop += 3
-                self.setFormat(start, stop - start, STYLE_LITERAL)
-                # Find next string in block, if any
-                next = stop + 3
-                current, start, next = find_start(text, next)
+                # Find string end
+                m2 = self._s_end[m1.captured()].match(text, offset=stroff)
+                if m2.hasMatch():
+                    stroff = m2.capturedEnd()
+                    # Ignore if escaped
+                    if text[m2.capturedStart() - 1] != '\\':
+                        # Terminate the single line string and move on
+                        self.setFormat(start, stroff - start, STYLE_LITERAL)
+                        strings.append((start, stroff))
+                elif m1.capturedLength() > 1:
+                    # Multi-line string start. Block finished!
+                    self.setCurrentBlockState(
+                        1 if m1.captured() == '"""' else 2)
+                    self.setFormat(start, len(text) - start, STYLE_LITERAL)
+                    return
+                # No Match? Then not a string so ignore and continue
+            m1 = self._s_start.match(text, offset=stroff)
+
+        # Comment
+        i = self._comment.globalMatch(text, offset=offset)
+        while i.hasNext():
+            m = i.next()
+            x = m.capturedStart()
+            if self._highlight_ok(strings, x, 1):
+                self.setFormat(x, len(text) - x, STYLE_COMMENT)
+                text = text[:x]
+                break
+
+        # Script header (must be at start of string)
+        if offset == 0:
+            m = self._rule_head.match(text)
+            if m.hasMatch():
+                self.setFormat(
+                    m.capturedStart(1), m.capturedLength(1), STYLE_HEADER)
+
+        # Rule based formatting
+        for (pattern, style) in self._rules:
+            i = pattern.globalMatch(text, offset=offset)
+            while i.hasNext():
+                m = i.next()
+                x, w = m.capturedStart(), m.capturedLength()
+                if self._highlight_ok(strings, x, w):
+                    self.setFormat(x, w, style)
 
 
 # List of essential built-in python functions
 _PYFUNC = [
     'abs()',
-    'divmod()',
-    'input()',
-    'open()',
-    'staticmethod()',
+    'aiter()',
     'all()',
-    'enumerate()',
-    'int()',
-    'ord()',
-    'str()',
     'any()',
-    'eval()',
-    'isinstance()',
-    'pow()',
-    'sum()',
-    'basestring()',
-    'execfile()',
-    'issubclass()',
-    'print()',
-    'super()',
+    'anext()',
+    'ascii()',
     'bin()',
-    'file()',
-    'iter()',
-    'property()',
-    'tuple()',
     'bool()',
-    'filter()',
-    'len()',
-    'range()',
-    'type()',
+    'breakpoint()',
     'bytearray()',
-    'float()',
-    'list()',
-    'raw_input()',
-    'unichr()',
+    'bytes()',
     'callable()',
-    'format()',
-    'locals()',
-    'reduce()',
-    'unicode()',
     'chr()',
-    'frozenset()',
-    'long()',
-    'reload()',
-    'vars()',
     'classmethod()',
+    'compile()',
+    'complex()',
+    'delattr()',
+    'dict()',
+    'dir()',
+    'divmod()',
+    'enumerate()',
+    'eval()',
+    'exec()',
+    'filter()',
+    'float()',
+    'format()',
+    'frozenset()',
     'getattr()',
-    'map()',
-    'repr()',
-    'range()',
-    'cmp()',
     'globals()',
-    'max()',
-    'reversed()',
-    'zip()',
-    'compile()',
     'hasattr()',
-    'memoryview()',
-    'round()',
-    '__import__()',
-    'complex()',
     'hash()',
-    'min()',
-    'set()',
-    'delattr()',
     'help()',
-    'next()',
-    'setattr()',
-    'dict()',
     'hex()',
-    'object()',
-    'slice()',
-    'dir()',
     'id()',
+    'input()',
+    'int()',
+    'isinstance()',
+    'issubclass()',
+    'iter()',
+    'len()',
+    'list()',
+    'locals()',
+    'map()',
+    'max()',
+    'memoryview()',
+    'min()',
+    'next()',
+    'object()',
     'oct()',
+    'open()',
+    'ord()',
+    'pow()',
+    'print()',
+    'property()',
+    'range()',
+    'repr()',
+    'reversed()',
+    'round()',
+    'set()',
+    'setattr()',
+    'slice()',
     'sorted()',
+    'staticmethod()',
+    'str()',
+    'sum()',
+    'super()',
+    'tuple()',
+    'type()',
+    'vars()',
+    'zip()',
+    '__import__()',
 ]
```

### Comparing `myokit-1.34.0/myokit/gui/vargrapher.py` & `myokit-1.35.0/myokit/gui/vargrapher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 #
 # Widget to display graphs of variable's equations.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-# Standard library imports
-
-# Myokit
 import myokit
+import myokit.gui
 
-# Qt imports
 from myokit.gui import QtGui, QtWidgets
 
-# NumPy
 import numpy as np
 
-# GUI components
-import myokit.gui
-
 # Matplotlib (must be imported _after_ gui has had chance to set backend)
 import matplotlib
 import matplotlib.figure
 from myokit.gui import matplotlib_backend as backend
 from mpl_toolkits.mplot3d import axes3d     # noqa
 
 
@@ -46,15 +36,15 @@
         The python function that calculates ``var``
     ``args``
         The arguments to func, i.e. the LhsExpressions that ``var`` depends on.
 
     *Extends:* ``QtWidgets.QDialog``
     """
     def __init__(self, parent, title, var, func, args):
-        super(VarGrapher, self).__init__(parent)
+        super().__init__(parent)
         self.setFixedSize(700, 600)
         self.setWindowTitle(title)
 
         # Figure panel
         self._figure = matplotlib.figure.Figure()
         self._canvas = backend.FigureCanvasQTAgg(self._figure)
         self._toolbar = backend.NavigationToolbar2QT(self._canvas, self)
```

### Comparing `myokit-1.34.0/myokit/lib/deps.py` & `myokit-1.35.0/myokit/lib/deps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #
 # Dependency graphing: creates graphical representations of myokit models
 # Uses matplotlib.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
-import random
 import collections
+import random
+
 import myokit
+
 # Don't import pyplot yet, this will crash if no window environment is loaded
 
 
 def create_state_dependency_matrix(model, direct=False, knockout=None):
     """
     Creates a matrix showing state variable dependency distances.
 
@@ -170,23 +169,23 @@
     a.set_xlabel('Affecting variable')
     a.set_ylabel('Affected variable')
 
     # Return
     return a
 
 
-class DiGraph(object):
+class DiGraph:
     """
     A simple directed graph implementation.
 
     If desired, a digraph can be created from an n-by-n connectivity matrix,
     for example ``matrix=[[0, 1, 1], [0, 1, 0], [0, 0, 0]]``
     """
     def __init__(self, matrix=None):
-        super(DiGraph, self).__init__()
+        super().__init__()
         if isinstance(matrix, DiGraph):
             # Clone
             self.nodes = collections.OrderedDict()
             for node in matrix:
                 self.add_node(node.uid)
             for node in matrix:
                 for edge in node.edgo:
@@ -522,23 +521,23 @@
             return self.node(test)
         if test.graph != self:
             raise ValueError('Node from another graph: "' + str(test) + '"')
         assert (test.uid in self.nodes and self.nodes[test.uid] == test)
         return test
 
 
-class Node(object):
+class Node:
     """
     Defines a node in a graph
     """
     def __init__(self, uid):
         """
         Creates a new, graphless node with the given identifier
         """
-        super(Node, self).__init__()
+        super().__init__()
         self.graph = None
         self.uid = uid
         self.edgo = set()
         self.edgi = set()
         # Graphical
         self.x = 0
         self.y = 0
```

### Comparing `myokit-1.34.0/myokit/lib/guess.py` & `myokit-1.35.0/myokit/lib/guess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #
 # Methods for guessing the meaning of model variables (and manipulating models
 # based on those guesses).
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
 import collections
+
 import myokit
 
 
 def _compatible_units(unit, options):
     """ Checks if ``unit`` is compatible with one of the given ``options``. """
     if unit is None:
         return False
```

### Comparing `myokit-1.34.0/myokit/lib/hh.py` & `myokit-1.35.0/myokit/lib/hh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 #
 # Tools for working with Hodgkin-Huxley style ion channel models
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import numpy as np
+
 import myokit
 
 
-class HHModel(object):
+class HHModel:
     """
     Represents a Hodgkin-Huxley (HH)-style model of an ion channel, extracted
     from a :class:`myokit.Model`.
 
     The class assumes the HH model can be (re)written as::
 
         I = prod(x[i]**n[i]) * f(V, p)
@@ -90,15 +88,15 @@
     """
     # NOTE: A HHModel must be immutable!
     # This ensures that the simulations don't have to clone it (which would be
     # costly and difficult).
     # A HHModel can return a function to calculate state values, but it never
     # updates its internal state in any way.
     def __init__(self, model, states, parameters=None, current=None, vm=None):
-        super(HHModel, self).__init__()
+        super().__init__()
 
         #
         # Check input
         #
         if not isinstance(model, myokit.Model):
             raise ValueError('First argument must be a myokit.Model.')
 
@@ -529,15 +527,15 @@
 
         Returns a list of steady state values.
         """
         inputs = self._parse_inputs(membrane_potential, parameters)
         return self._steady_state_function(*inputs)
 
 
-class AnalyticalSimulation(object):
+class AnalyticalSimulation:
     """
     Analytically evaluates a :class:`HHModel`'s state for a given set of points
     in time.
 
     Each simulation object maintains an internal state consisting of
 
     * The current simulation time
@@ -579,15 +577,15 @@
         plt.legend(loc='center right')
         plt.subplot(212)
         plt.plot(d.time(), d[m.current()])
         plt.show()
 
     """
     def __init__(self, model, protocol=None):
-        super(AnalyticalSimulation, self).__init__()
+        super().__init__()
 
         # Check model
         if not isinstance(model, HHModel):
             raise ValueError('First parameter must be a `HHModel`.')
         self._model = model
 
         # Check protocol
```

### Comparing `myokit-1.34.0/myokit/lib/markov.py` & `myokit-1.35.0/myokit/lib/markov.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #
 # Tools for working with Markov models of ion channels.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import collections
+
 import numpy as np
 
 import myokit
 
 
-class LinearModel(object):
+class LinearModel:
     """
     Represents a linear Markov model of an ion channel extracted from a
     :class:`myokit.Model`.
 
     The class assumes the markov model can be written as::
 
         dot(x) = A(V,p) * x
@@ -116,15 +114,15 @@
     # NOTE: A LinearModel must be immutable!
     # This ensures that the simulations don't have to clone it (which would be
     # costly and difficult).
     # A LinearModel has a method "matrices()" which can evaluate A and B
     # for its default values or newly passed in values, but it never updates
     # its internal state in any way!
     def __init__(self, model, states, parameters=None, current=None, vm=None):
-        super(LinearModel, self).__init__()
+        super().__init__()
 
         # Get a clone of the model, with all markov models written in full ODE
         # form.
         self._model = convert_markov_models_to_full_ode_form(model)
         del model
 
         #
@@ -385,15 +383,15 @@
             if e != zero:
                 body.append('B[' + str(j) + '] = ' + w(e))
         body.append('return A, B')
         code = head + '\n' + '\n'.join(['    ' + line for line in body])
         globl = {'numpy': np, 'n': n}
         local = {}
 
-        myokit._exec(code, globl, local)
+        exec(code, globl, local)
         self._matrix_function = local['matrix_function']
 
         #
         # Create function to return list of transition rates
         #
         self._model.reserve_unique_names('R', 'n', 'numpy')
         head = 'def rate_list_function('
@@ -404,15 +402,15 @@
         for i, j, e in R:
             body.append(
                 'R.append((' + str(i) + ',' + str(j) + ',' + w(e) + '))')
         body.append('return R')
         code = head + '\n' + '\n'.join(['    ' + line for line in body])
         globl = {'numpy': np}
         local = {}
-        myokit._exec(code, globl, local)
+        exec(code, globl, local)
         self._rate_list_function = local['rate_list_function']
 
     def current(self):
         """
         Returns the name of the current variable used by this model, or None if
         no current variable was specified.
         """
@@ -631,15 +629,15 @@
 
         # Recreate full state vector and return
         x = np.array(x).reshape((len(x),))
         x = np.concatenate((x, [1 - np.sum(x)]))
         return x
 
 
-class AnalyticalSimulation(object):
+class AnalyticalSimulation:
     """
     Analytically evaluates a :class:`LinearModel`'s state over a given set of
     points in time.
 
     Solutions are calculated for the "law of large numbers" case, i.e. without
     stochastic behavior. The solution algorithm is based on eigenvalue
     decomposition.
@@ -685,15 +683,15 @@
         plt.legend(loc='center right')
         plt.subplot(212)
         plt.plot(d.time(), d[m.current()])
         plt.show()
 
     """
     def __init__(self, model, protocol=None):
-        super(AnalyticalSimulation, self).__init__()
+        super().__init__()
         # Check model
         if not isinstance(model, LinearModel):
             raise ValueError('First parameter must be a `LinearModel`.')
         self._model = model
 
         # Check protocol
         if protocol is None:
@@ -1089,15 +1087,15 @@
     def state(self):
         """
         Returns the initial state used by this simulation.
         """
         return list(self._state)
 
 
-class DiscreteSimulation(object):
+class DiscreteSimulation:
     """
     Performs stochastic simulations of a :class:`LinearModel`'s behavior for a
     finite number of channels.
 
     Simulations are run using the "Direct method" proposed by Gillespie [1].
 
     Each simulation object maintains an internal state consisting of
@@ -1559,15 +1557,15 @@
     def state(self):
         """
         Returns the current simulation state.
         """
         return list(self._state)
 
 
-class MarkovModel(object):
+class MarkovModel:
     """
     **Deprecated**: This class has been replaced by the classes
     :class:`LinearModel` and :class:`AnalyticalSimulation`. Please update your
     code to use these classes instead. This class will be removed in
     future versions of Myokit.
     """
```

### Comparing `myokit-1.34.0/myokit/lib/multi.py` & `myokit-1.35.0/myokit/lib/multi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # Tools for running experiments on multiple models.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
+import os
 
 import myokit
-import os
 
 
 #
 # Deprecated since 2020-06-14
 #
 import warnings
 warnings.warn(
```

### Comparing `myokit-1.34.0/myokit/lib/plots.py` & `myokit-1.35.0/myokit/lib/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # Creates common graphs
 # Uses matplotlib
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import numpy as np
+
 # Don't import pyplot yet, this will cause a crash if no window environment
 # is loaded.
 
 
 def simulation_times(
         time=None, realtime=None, evaluations=None, mode='stair', axes=None,
         nbuckets=50, label=None):
```

### Comparing `myokit-1.34.0/myokit/pacing.py` & `myokit-1.35.0/myokit/pacing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Factory methods for pacing protocols
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
 """
 This module contains factory methods to create Protocol objects
 programmatically.
 """
```

### Comparing `myokit-1.34.0/myokit/pype.py` & `myokit-1.35.0/myokit/pype.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 #
 # A tiny templating engine using a php style syntax.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import ast
+import io
 import re
 import sys
 import traceback
 
-import myokit
-
-try:
-    # Python 2
-    from cStringIO import StringIO
-except ImportError:
-    # Python3
-    from io import StringIO
-
 
-class TemplateEngine(object):
+class TemplateEngine:
     """
     A tiny templating engine using a php style syntax.
 
     Not intended for use in websites or with untrusted templates.
 
     Basic syntax::
 
@@ -36,15 +25,15 @@
 
         Hello <?= "world" ?>
 
     All processed template data is printed to the standard output stream or a
     stream specified by the user.
     """
     def __init__(self):
-        super(TemplateEngine, self).__init__()
+        super().__init__()
         self.stream = None
         self.error = None
 
     def error_details(self):
         """
         After a PypeError has been thrown, calling this will method will return
         a detailed (multi-line) error message.
@@ -67,28 +56,28 @@
                 'Second argument passed to process() must be dict'
                 ' (variable_name : value)')
 
         # Convert script, any exceptions are thrown as PypeErrors
         script = self._convert(filename)
 
         # Get or create output stream
-        stdout = self.stream if self.stream else StringIO()
-        stderr = StringIO()
+        stdout = self.stream if self.stream else io.StringIO()
+        stderr = io.StringIO()
 
         # Run and handle errors
         error = None
         try:
             # Run, but catch any output + any occurring exception
             sysout = syserr = None
             try:
                 sysout = sys.stdout
                 syserr = sys.stderr
                 sys.stdout = stdout
                 sys.stderr = stderr
-                myokit._exec(script, variables)
+                exec(script, variables)
             except Exception:
                 error = sys.exc_info()
             finally:
                 if sysout:
                     sys.stdout = sysout
                 if syserr:
                     sys.stderr = syserr    # Ignore error output
@@ -241,9 +230,9 @@
 class PypeError(Exception):
     """
     An error thrown by the :class:`TemplateEngine`
 
     *Extends:* Exception
     """
     def __init__(self, message):
-        super(PypeError, self).__init__(message)
+        super().__init__(message)
```

### Comparing `myokit-1.34.0/myokit/tests/__init__.py` & `myokit-1.35.0/myokit/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 # The TemporaryDirectory class was adapted from Pints
 # See: https://github.com/pints-team/pints
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import tempfile
 import warnings
 
 import myokit
 
 
@@ -39,22 +36,22 @@
     OpenCL_DOUBLE_PRECISION = info.has_extension('cl_khr_fp64')
     if OpenCL_DOUBLE_PRECISION:
         OpenCL_DOUBLE_PRECISION_CONNECTIONS = info.has_extension(
             'cl_khr_int64_base_atomics')
     del info
 
 
-class TemporaryDirectory(object):
+class TemporaryDirectory:
     """
     ContextManager that provides a temporary directory to create temporary
     files in. Deletes the directory and its contents when the context is
     exited.
     """
     def __init__(self):
-        super(TemporaryDirectory, self).__init__()
+        super().__init__()
         self._dir = None
 
     def __enter__(self):
         self._dir = os.path.realpath(tempfile.mkdtemp())
         return self
 
     def path(self, path=None):
@@ -134,15 +131,15 @@
         pass
 
     def update(self, f):
         self.okays -= 1
         return self.okays >= 0
 
 
-class WarningCollector(object):
+class WarningCollector:
     """
     Wrapper around warnings.catch_warnings() that gathers all messages into a
     single string.
     """
     def __init__(self):
         self._warnings = []
         self._w = warnings.catch_warnings(record=True)
```

### Comparing `myokit-1.34.0/myokit/tests/ansic_event_based_pacing.py` & `myokit-1.35.0/myokit/tests/ansic_event_based_pacing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 #
 # Class for testing the event-based pacing system.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 
 import myokit
 
 from myokit.tests import DIR_TEST
 
 
@@ -22,15 +19,15 @@
 class AnsicEventBasedPacing(myokit.CModule):
     """
     Class for testing the event-based pacing system.
     """
     _index = 0
 
     def __init__(self, protocol):
-        super(AnsicEventBasedPacing, self).__init__()
+        super().__init__()
 
         # Unique id
         AnsicEventBasedPacing._index += 1
         module_name = 'myokit_ansic_pacing_' \
             + str(AnsicEventBasedPacing._index)
 
         # Arguments
```

### Comparing `myokit-1.34.0/myokit/tests/data/beeler-1977-model-compare-a.mmt` & `myokit-1.35.0/myokit/tests/data/beeler-1977-model-compare-a.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/beeler-1977-model-compare-b.mmt` & `myokit-1.35.0/myokit/tests/data/beeler-1977-model-compare-b.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/beeler-1977-model.mmt` & `myokit-1.35.0/myokit/tests/data/beeler-1977-model.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/beeler-1977-units.mmt` & `myokit-1.35.0/myokit/tests/data/beeler-1977-units.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/clancy-1999-fitting.mmt` & `myokit-1.35.0/myokit/tests/data/clancy-1999-fitting.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/conditional.mmt` & `myokit-1.35.0/myokit/tests/data/conditional.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/cv1d.mmt` & `myokit-1.35.0/myokit/tests/data/cv1d.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/cv1d.zip` & `myokit-1.35.0/myokit/tests/data/cv1d.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/decker-2009.mmt` & `myokit-1.35.0/myokit/tests/data/decker-2009.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/decker.model` & `myokit-1.35.0/myokit/tests/data/decker.model`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/dn-1985-normalised.mmt` & `myokit-1.35.0/myokit/tests/data/dn-1985-normalised.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/dom-markov.mmt` & `myokit-1.35.0/myokit/tests/data/dom-markov.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/abf-protocol.pro` & `myokit-1.35.0/myokit/tests/data/formats/abf-protocol.pro`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/abf-v1.abf` & `myokit-1.35.0/myokit/tests/data/formats/abf-v1.abf`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/abf-v2.abf` & `myokit-1.35.0/myokit/tests/data/formats/abf-v2.abf`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/cellml/br-1977-dot.cellml` & `myokit-1.35.0/myokit/tests/data/formats/cellml/br-1977-dot.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/cellml/br-1977.cellml` & `myokit-1.35.0/myokit/tests/data/formats/cellml/br-1977.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/cellml/corrias.cellml` & `myokit-1.35.0/myokit/tests/data/formats/cellml/corrias.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/cellml/decker-2009.cellml` & `myokit-1.35.0/myokit/tests/data/formats/cellml/decker-2009.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/cellml/documentation.cellml` & `myokit-1.35.0/myokit/tests/data/formats/cellml/documentation.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml` & `myokit-1.35.0/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml` & `myokit-1.35.0/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml` & `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml` & `myokit-1.35.0/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml` & `myokit-1.35.0/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/sbml/HodgkinHuxley.xml` & `myokit-1.35.0/myokit/tests/data/formats/sbml/HodgkinHuxley.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml` & `myokit-1.35.0/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml` & `myokit-1.35.0/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml` & `myokit-1.35.0/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/sbml/result/00001-results.csv` & `myokit-1.35.0/myokit/tests/data/formats/sbml/result/00001-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/sbml/result/00004-results.csv` & `myokit-1.35.0/myokit/tests/data/formats/sbml/result/00004-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/sbml/result/01103-results.csv` & `myokit-1.35.0/myokit/tests/data/formats/sbml/result/01103-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/formats/wcp-file.wcp` & `myokit-1.35.0/myokit/tests/data/formats/wcp-file.wcp`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad1d-1-not-enough-files.zip` & `myokit-1.35.0/myokit/tests/data/io/bad1d-1-not-enough-files.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad1d-2-no-header.zip` & `myokit-1.35.0/myokit/tests/data/io/bad1d-2-no-header.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad1d-3-no-data.zip` & `myokit-1.35.0/myokit/tests/data/io/bad1d-3-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad1d-4-not-a-zip.zip` & `myokit-1.35.0/myokit/tests/data/io/bad1d-4-not-a-zip.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad1d-5-bad-data-type.zip` & `myokit-1.35.0/myokit/tests/data/io/bad1d-5-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad1d-6-time-too-short.zip` & `myokit-1.35.0/myokit/tests/data/io/bad1d-6-time-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad1d-7-0d-too-short.zip` & `myokit-1.35.0/myokit/tests/data/io/bad1d-7-0d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad1d-8-1d-too-short.zip` & `myokit-1.35.0/myokit/tests/data/io/bad1d-8-1d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad2d-1-not-enough-files.zip` & `myokit-1.35.0/myokit/tests/data/io/bad2d-1-not-enough-files.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad2d-2-no-header.zip` & `myokit-1.35.0/myokit/tests/data/io/bad2d-2-no-header.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad2d-3-no-data.zip` & `myokit-1.35.0/myokit/tests/data/io/bad2d-3-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad2d-4-not-a-zip.zip` & `myokit-1.35.0/myokit/tests/data/io/bad2d-4-not-a-zip.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad2d-5-bad-data-type.zip` & `myokit-1.35.0/myokit/tests/data/io/bad2d-5-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad2d-6-time-too-short.zip` & `myokit-1.35.0/myokit/tests/data/io/bad2d-6-time-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad2d-7-0d-too-short.zip` & `myokit-1.35.0/myokit/tests/data/io/bad2d-7-0d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/bad2d-8-2d-too-short.zip` & `myokit-1.35.0/myokit/tests/data/io/bad2d-8-2d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/badlog-1-no-data.zip` & `myokit-1.35.0/myokit/tests/data/io/badlog-1-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/badlog-2-no-structure.zip` & `myokit-1.35.0/myokit/tests/data/io/badlog-2-no-structure.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/badlog-4-invalid-n-fields.zip` & `myokit-1.35.0/myokit/tests/data/io/badlog-4-invalid-n-fields.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/badlog-5-invalid-data-size.zip` & `myokit-1.35.0/myokit/tests/data/io/badlog-5-invalid-data-size.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/badlog-6-bad-data-type.zip` & `myokit-1.35.0/myokit/tests/data/io/badlog-6-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/badlog-7-not-enough-data.zip` & `myokit-1.35.0/myokit/tests/data/io/badlog-7-not-enough-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/block2d.mmt` & `myokit-1.35.0/myokit/tests/data/io/block2d.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/block2d.zip` & `myokit-1.35.0/myokit/tests/data/io/block2d.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/io/goodlog.zip` & `myokit-1.35.0/myokit/tests/data/io/goodlog.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/lr-1991-dep.mmt` & `myokit-1.35.0/myokit/tests/data/lr-1991-dep.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/lr-1991-fitting.mmt` & `myokit-1.35.0/myokit/tests/data/lr-1991-fitting.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/lr-1991-testing.mmt` & `myokit-1.35.0/myokit/tests/data/lr-1991-testing.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/lr-1991.mmt` & `myokit-1.35.0/myokit/tests/data/lr-1991.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/multi/beeler-no-name.mmt` & `myokit-1.35.0/myokit/tests/data/multi/beeler-no-name.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/multi/lr-1991.mmt` & `myokit-1.35.0/myokit/tests/data/multi/lr-1991.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/multi/subdir/beeler-no-name.mmt` & `myokit-1.35.0/myokit/tests/data/multi/subdir/beeler-no-name.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/data/noble-1962.mmt` & `myokit-1.35.0/myokit/tests/data/noble-1962.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.34.0/myokit/tests/test_aux.py` & `myokit-1.35.0/myokit/tests/test_aux.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,19 @@
 #!/usr/bin/env python3
 #
 # Tests the myokit._aux module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
+import io
 import os
 import re
 import unittest
 
-# StringIO in Python 2 and 3
-try:
-    from cStringIO import StringIO
-except ImportError:  # pragma: no python 2 cover
-    from io import StringIO
-
-# Strings in Python2 and Python3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
-
 import myokit
 
 from myokit.tests import DIR_DATA, WarningCollector
 
 
 class AuxTest(unittest.TestCase):
     """
@@ -83,45 +69,45 @@
         self.assertEqual(protocol.head().period(), 1000)
 
     def test_default_script(self):
         # Test default script
 
         # Test without a model
         script = myokit.default_script()
-        self.assertTrue(isinstance(script, basestring))
+        self.assertTrue(isinstance(script, str))
         self.assertIn('run(1000)', script)
 
         # Test adapting the time unit
         model = myokit.Model()
         t = model.add_component('c').add_variable('t')
         t.set_rhs(0)
         script = myokit.default_script(model)
-        self.assertTrue(isinstance(script, basestring))
+        self.assertTrue(isinstance(script, str))
         self.assertIn('run(1000)', script)
 
         t.set_binding('time')
         script = myokit.default_script(model)
-        self.assertTrue(isinstance(script, basestring))
+        self.assertTrue(isinstance(script, str))
         self.assertIn('run(1000)', script)
 
         t.set_unit('s')
         script = myokit.default_script(model)
-        self.assertTrue(isinstance(script, basestring))
+        self.assertTrue(isinstance(script, str))
         self.assertIn('run(1.0)', script)
 
         t.set_unit('ms')
         script = myokit.default_script(model)
-        self.assertTrue(isinstance(script, basestring))
+        self.assertTrue(isinstance(script, str))
         self.assertIn('run(1000)', script)
 
         # Test plotting membrane potential
         v = model.get('c').add_variable('v')
         v.set_label('membrane_potential')
         script = myokit.default_script(model)
-        self.assertTrue(isinstance(script, basestring))
+        self.assertTrue(isinstance(script, str))
         self.assertIn("var = 'c.v'", script)
 
         # TODO: Run with tiny model?
 
     def test_format_float_dict(self):
         # Test myokit.format_float_dict, which is deprecated
         d = {'one': 1, 'Definitely two': 2, 'Three-ish': 3.1234567}
@@ -279,15 +265,15 @@
             myokit.run(m, p, x)
         with myokit.tools.capture():
             myokit.run(m, p, '[[script]]\n' + x)
         self.assertRaises(ZeroDivisionError, myokit.run, m, p, 'print(1 / 0)')
 
         # Test with stringio
         x = "print('Hi there')"
-        s = StringIO()
+        s = io.StringIO()
         with myokit.tools.capture() as c:
             myokit.run(m, p, x, stderr=s, stdout=s)
         self.assertEqual(c.text(), '')
         self.assertEqual(s.getvalue(), 'Hi there\n')
 
     def test_step(self):
         # Test the step() method.
@@ -559,15 +545,15 @@
         self.assertEqual(a, b)
 
     def test_version(self):
         # Test the version() method.
 
         # Raw version
         raw = myokit.version(raw=True)
-        self.assertIsInstance(raw, basestring)
+        self.assertIsInstance(raw, str)
         parts = raw.split('.')
         self.assertTrue(len(parts) in [3, 4])
 
         # Formatted version
         v = myokit.version()
         v = v.splitlines()
         self.assertEqual(len(v), 3)
```

### Comparing `myokit-1.34.0/myokit/tests/test_cellml_v1_api.py` & `myokit-1.35.0/myokit/tests/test_cellml_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,21 @@
 #!/usr/bin/env python3
 #
 # Tests the CellML 1.0/1.1 API.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 import myokit.formats.cellml.v1 as cellml
 
 from myokit.tests import WarningCollector
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python2 and Python3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
-
 
 class TestCellML1AnnotatedElement(unittest.TestCase):
     """ Tests for cellml.AnnotatableElement. """
 
     def test_cmeta_id(self):
         # Tests the cmeta_id methods.
 
@@ -1499,15 +1484,15 @@
 
     def test_si_unit_names(self):
         # Tests Units.si_unit_names()
 
         names = [x for x in cellml.Units.si_unit_names()]
         self.assertTrue(len(names) > 10)
         for name in names:
-            self.assertTrue(isinstance(name, basestring))
+            self.assertTrue(isinstance(name, str))
             if name == 'celsius':
                 continue
             self.assertTrue(
                 isinstance(cellml.Units.find_units(name), cellml.Units))
 
     def test_string_conversion(self):
         # Test __str__
```

### Comparing `myokit-1.34.0/myokit/tests/test_cellml_v1_parser.py` & `myokit-1.35.0/myokit/tests/test_cellml_v1_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,26 @@
 #!/usr/bin/env python3
 #
 # Tests the CellML 1.0/1.1 parser.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 import myokit.formats.cellml as cellml
 import myokit.formats.cellml.v1 as v1
 
 from myokit.tests import TemporaryDirectory, DIR_FORMATS, WarningCollector
 
 # CellML directory
 DIR = os.path.join(DIR_FORMATS, 'cellml')
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python2 and Python3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
-
 
 class TestCellMLParser(unittest.TestCase):
     """ Tests the CellML 1.0/1.1 parser (mostly for errors). """
 
     def assertBad(self, xml, message, version='1.0'):
         """
         Inserts the given ``xml`` into a <model> element, parses it, and checks
```

### Comparing `myokit-1.34.0/myokit/tests/test_cellml_v1_writer.py` & `myokit-1.35.0/myokit/tests/test_cellml_v1_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 #!/usr/bin/env python3
 #
 # Tests the CellML 1.0/1.1 writer
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import re
 import unittest
 
 import myokit
 import myokit.formats.cellml.v1 as cellml
 
 from myokit.tests import TemporaryDirectory, WarningCollector
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class TestCellMLWriter(unittest.TestCase):
     """ Tests for cellml.Writer. """
 
     def test_cmeta_ids(self):
         # Tests cmeta ids are written for models, components, and variables
```

### Comparing `myokit-1.34.0/myokit/tests/test_cellml_v2_api.py` & `myokit-1.35.0/myokit/tests/test_cellml_v2_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,21 @@
 #!/usr/bin/env python3
 #
 # Tests the CellML 2.0 API.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 import myokit.formats.cellml.v2 as cellml
 
 from myokit.tests import WarningCollector
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python2 and Python3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
-
 
 class TestCellML2AnnotatableElement(unittest.TestCase):
     """ Tests for ``cellml.v2.AnnotatableElement``. """
 
     def test_annotatable(self):
         # Test making an annotation
 
@@ -1806,15 +1791,15 @@
 
     def test_si_unit_names(self):
         # Tests Units.si_unit_names()
 
         names = [x for x in cellml.Units.si_unit_names()]
         self.assertTrue(len(names) > 10)
         for name in names:
-            self.assertTrue(isinstance(name, basestring))
+            self.assertTrue(isinstance(name, str))
             self.assertTrue(
                 isinstance(cellml.Units.find_units(name), cellml.Units))
 
     def test_string_conversion(self):
         # Test __str__
 
         u = cellml.Units('Numpty', myokit.units.ampere)
```

### Comparing `myokit-1.34.0/myokit/tests/test_cellml_v2_parser.py` & `myokit-1.35.0/myokit/tests/test_cellml_v2_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,25 @@
 #!/usr/bin/env python3
 #
 # Tests the CellML 2.0 parser.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 import myokit.formats.cellml.v2 as v2
 
 from myokit.tests import TemporaryDirectory, DIR_FORMATS, WarningCollector
 
 # CellML directory
 DIR = os.path.join(DIR_FORMATS, 'cellml')
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python2 and Python3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
-
 
 class TestCellMLParser(unittest.TestCase):
     """ Tests the CellML 2.0 parser (mostly for errors / model validation). """
 
     def assertBad(self, xml, message, version='2.0'):
         """
         Inserts the given ``xml`` into a <model> element, parses it, and checks
```

### Comparing `myokit-1.34.0/myokit/tests/test_cellml_v2_writer.py` & `myokit-1.35.0/myokit/tests/test_cellml_v2_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 #!/usr/bin/env python3
 #
 # Tests the CellML 2.0 writer.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import re
 import unittest
 
 import myokit
 import myokit.formats.cellml.v2 as cellml
 
 from myokit.tests import TemporaryDirectory, WarningCollector
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class TestCellMLWriter(unittest.TestCase):
     """ Tests for cellml.Writer. """
 
     def test_component(self):
         # Tests if components are written
```

### Comparing `myokit-1.34.0/myokit/tests/test_cmodel.py` & `myokit-1.35.0/myokit/tests/test_cmodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 #!/usr/bin/env python3
 #
 # Tests the CModel class.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 
 from myokit.tests import DIR_DATA
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class CModelTest(unittest.TestCase):
     """
     Tests the CModel class.
     """
 
     @classmethod
```

### Comparing `myokit-1.34.0/myokit/tests/test_component.py` & `myokit-1.35.0/myokit/tests/test_component.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,18 @@
 #!/usr/bin/env python3
 #
 # Tests the Component and VarOwner classes.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
 import unittest
 
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
 class VarOwnerTest(unittest.TestCase):
     """
     Tests parts of :class:`myokit.VarOwner`.
     """
     def test_move_variable(self):
         # Test the method to move component variables to another component.
```

### Comparing `myokit-1.34.0/myokit/tests/test_config.py` & `myokit-1.35.0/myokit/tests/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 #!/usr/bin/env python3
 #
 # Tests the exporters from the format module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import sys
 import unittest
 
 import myokit
 
 from myokit.tests import TemporaryDirectory, WarningCollector
 
-
 debug = False
 
 
 # Simple test
 config_basic = """
 [myokit]
 [time]
@@ -40,33 +36,23 @@
 [extra]
 setting = 12
 sotting=2
 str=String value
 """
 
 # Config with empty paths and spaces
-config_paths_1 = """
+config_paths = """
 [sundials]
 lib = five
 inc = three;four;
 [opencl]
 lib = one;;   two point five;three;
 inc =
 """
 
-# Config with empty paths and " ;", which in Python 2 is ignored
-config_paths_2 = """
-[sundials]
-lib = five ; six
-inc = three;four;
-[opencl]
-lib = one ;;   two point five ;three;
-inc =
-"""
-
 
 class TestConfig(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
 
         # Import hidden _config module
@@ -78,18 +64,18 @@
             sys.path = path
 
         # Back-up current settings
         cls._compat_no_capture = myokit.COMPAT_NO_CAPTURE
         cls._compat_no_fd_capture = myokit.COMPAT_NO_FD_CAPTURE
         cls._date_format = myokit.DATE_FORMAT
         cls._time_format = myokit.TIME_FORMAT
-        cls._force_pyside = myokit.FORCE_PYSIDE
-        cls._force_pyside2 = myokit.FORCE_PYSIDE2
-        cls._force_pyqt4 = myokit.FORCE_PYQT4
+        cls._force_pyqt6 = myokit.FORCE_PYQT6
         cls._force_pyqt5 = myokit.FORCE_PYQT5
+        cls._force_pyside6 = myokit.FORCE_PYSIDE6
+        cls._force_pyside2 = myokit.FORCE_PYSIDE2
         cls._sundials_lib = myokit.SUNDIALS_LIB
         cls._sundials_inc = myokit.SUNDIALS_INC
         cls._opencl_lib = myokit.OPENCL_LIB
         cls._opencl_inc = myokit.OPENCL_INC
 
         # Temporarily change myokit config dir
         cls._dir_user = myokit.DIR_USER
@@ -110,35 +96,35 @@
         myokit.DIR_USER = cls._dir_user
 
         # Reset data and time
         myokit.COMPAT_NO_CAPTURE = cls._compat_no_capture
         myokit.COMPAT_NO_FD_CAPTURE = cls._compat_no_fd_capture
         myokit.DATE_FORMAT = cls._date_format
         myokit.TIME_FORMAT = cls._time_format
-        myokit.FORCE_PYSIDE = cls._force_pyside
-        myokit.FORCE_PYSIDE2 = cls._force_pyside2
-        myokit.FORCE_PYQT4 = cls._force_pyqt4
+        myokit.FORCE_PYQT6 = cls._force_pyqt6
         myokit.FORCE_PYQT5 = cls._force_pyqt5
+        myokit.FORCE_PYSIDE6 = cls._force_pyside6
+        myokit.FORCE_PYSIDE2 = cls._force_pyside2
         myokit.SUNDIALS_LIB = cls._sundials_lib
         myokit.SUNDIALS_INC = cls._sundials_inc
         myokit.OPENCL_LIB = cls._opencl_lib
         myokit.OPENCL_INC = cls._opencl_inc
 
         # Reload local settings
         cls._config_module._load()
 
         # Sanity check
         assert myokit.COMPAT_NO_CAPTURE == cls._compat_no_capture
         assert myokit.COMPAT_NO_FD_CAPTURE == cls._compat_no_fd_capture
         assert myokit.DATE_FORMAT != 'TEST_DATE_FORMAT'
         assert myokit.TIME_FORMAT != 'TEST_TIME_FORMAT'
-        assert myokit.FORCE_PYSIDE == cls._force_pyside
-        assert myokit.FORCE_PYSIDE2 == cls._force_pyside2
-        assert myokit.FORCE_PYQT4 == cls._force_pyqt4
+        assert myokit.FORCE_PYQT6 == cls._force_pyqt6
         assert myokit.FORCE_PYQT5 == cls._force_pyqt5
+        assert myokit.FORCE_PYSIDE6 == cls._force_pyside6
+        assert myokit.FORCE_PYSIDE2 == cls._force_pyside2
         assert myokit.SUNDIALS_LIB != ['one', 'two']
         assert myokit.SUNDIALS_INC != ['three', 'four']
         assert myokit.OPENCL_LIB != ['five', 'six']
         assert myokit.OPENCL_INC != ['three', 'eight']
 
         if debug:
             print('tearDownClass completed')
@@ -164,25 +150,25 @@
 
     def test_load_basic(self):
         # Tests basic entries are loaded.
         myokit.SUNDIALS_LIB = []
         myokit.SUNDIALS_INC = []
         myokit.OPENCL_LIB = []
         myokit.OPENCL_INC = []
-        myokit.FORCE_PYSIDE = myokit.FORCE_PYSIDE2 = False
-        myokit.FORCE_PYQT4 = myokit.FORCE_PYQT5 = False
+        myokit.FORCE_PYSIDE6 = myokit.FORCE_PYSIDE2 = False
+        myokit.FORCE_PYQT6 = myokit.FORCE_PYQT5 = False
         with open(self._temp_dir.path('myokit.ini'), 'w') as f:
             f.write(config_basic)
         self._config_module._load()
         self.assertEqual(myokit.DATE_FORMAT, 'TEST_DATE_FORMAT')
         self.assertEqual(myokit.TIME_FORMAT, 'TEST_TIME_FORMAT')
-        self.assertFalse(myokit.FORCE_PYSIDE)
-        self.assertFalse(myokit.FORCE_PYSIDE2)
-        self.assertFalse(myokit.FORCE_PYQT4)
+        self.assertFalse(myokit.FORCE_PYQT6)
         self.assertFalse(myokit.FORCE_PYQT5)
+        self.assertFalse(myokit.FORCE_PYSIDE6)
+        self.assertFalse(myokit.FORCE_PYSIDE2)
         self.assertEqual(myokit.SUNDIALS_LIB, ['one', 'two'])
         self.assertEqual(myokit.SUNDIALS_INC, ['three', 'four'])
         self.assertEqual(myokit.OPENCL_LIB, ['five', 'six'])
         self.assertEqual(myokit.OPENCL_INC, ['three', 'eight'])
 
         # Unknown settings are ignored
         with open(self._temp_dir.path('myokit.ini'), 'w') as f:
@@ -201,88 +187,69 @@
 
         # Lists of paths should be filtered for empty values and trimmed
         myokit.SUNDIALS_LIB = []
         myokit.SUNDIALS_INC = []
         myokit.OPENCL_LIB = []
         myokit.OPENCL_INC = []
         with open(self._temp_dir.path('myokit.ini'), 'w') as f:
-            f.write(config_paths_1)
+            f.write(config_paths)
         self._config_module._load()
         self.assertEqual(myokit.SUNDIALS_LIB, ['five'])
         self.assertEqual(myokit.SUNDIALS_INC, ['three', 'four'])
         self.assertEqual(
             myokit.OPENCL_LIB,
             ['one', 'two point five', 'three'])
         self.assertEqual(myokit.OPENCL_INC, [])
 
-        # Even if the list contains " ;", which Python 2's config parser treats
-        # as a comment
-        myokit.SUNDIALS_LIB = []
-        myokit.SUNDIALS_INC = []
-        myokit.OPENCL_LIB = []
-        myokit.OPENCL_INC = []
-        with open(self._temp_dir.path('myokit.ini'), 'w') as f:
-            f.write(config_paths_2)
-        if sys.hexversion < 0x03020000:
-            self.assertRaises(ImportError, self._config_module._load)
-        else:
-            self._config_module._load()
-            self.assertEqual(myokit.SUNDIALS_LIB, ['five', 'six'])
-            self.assertEqual(myokit.SUNDIALS_INC, ['three', 'four'])
-            self.assertEqual(
-                myokit.OPENCL_LIB,
-                ['one', 'two point five', 'three'])
-            self.assertEqual(myokit.OPENCL_INC, [])
-
     def test_load_gui_backend(self):
         # Tests setting the GUI back end
 
         # Qt gui options
         with open(self._temp_dir.path('myokit.ini'), 'w') as f:
-            f.write('[gui]\nbackend=pyqt4\n')
+            f.write('[gui]\nbackend=pyqt6\n')
         self._config_module._load()
-        self.assertFalse(myokit.FORCE_PYSIDE)
-        self.assertFalse(myokit.FORCE_PYSIDE2)
-        self.assertTrue(myokit.FORCE_PYQT4)
+        self.assertTrue(myokit.FORCE_PYQT6)
         self.assertFalse(myokit.FORCE_PYQT5)
+        self.assertFalse(myokit.FORCE_PYSIDE6)
+        self.assertFalse(myokit.FORCE_PYSIDE2)
 
         with open(self._temp_dir.path('myokit.ini'), 'w') as f:
             f.write('[gui]\nbackend=pyqt5\n')
         self._config_module._load()
-        self.assertFalse(myokit.FORCE_PYSIDE)
-        self.assertFalse(myokit.FORCE_PYSIDE2)
-        self.assertFalse(myokit.FORCE_PYQT4)
+        self.assertFalse(myokit.FORCE_PYQT6)
         self.assertTrue(myokit.FORCE_PYQT5)
+        self.assertFalse(myokit.FORCE_PYSIDE6)
+        self.assertFalse(myokit.FORCE_PYSIDE2)
 
         with open(self._temp_dir.path('myokit.ini'), 'w') as f:
-            f.write('[gui]\nbackend=pyside\n')
+            f.write('[gui]\nbackend=pyside6\n')
         self._config_module._load()
-        self.assertTrue(myokit.FORCE_PYSIDE)
-        self.assertFalse(myokit.FORCE_PYSIDE2)
-        self.assertFalse(myokit.FORCE_PYQT4)
+        self.assertFalse(myokit.FORCE_PYQT6)
         self.assertFalse(myokit.FORCE_PYQT5)
+        self.assertTrue(myokit.FORCE_PYSIDE6)
+        self.assertFalse(myokit.FORCE_PYSIDE2)
 
         with open(self._temp_dir.path('myokit.ini'), 'w') as f:
             f.write('[gui]\nbackend=pyside2\n')
         self._config_module._load()
-        self.assertFalse(myokit.FORCE_PYSIDE)
-        self.assertTrue(myokit.FORCE_PYSIDE2)
-        self.assertFalse(myokit.FORCE_PYQT4)
+        self.assertFalse(myokit.FORCE_PYQT6)
         self.assertFalse(myokit.FORCE_PYQT5)
+        self.assertFalse(myokit.FORCE_PYSIDE6)
+        self.assertTrue(myokit.FORCE_PYSIDE2)
 
         # Empty has no effect
         with open(self._temp_dir.path('myokit.ini'), 'w') as f:
             f.write('[gui]\nbackend=\n')
         with WarningCollector() as c:
             self._config_module._load()
         self.assertEqual(c.text(), '')
-        self.assertFalse(myokit.FORCE_PYSIDE)
-        self.assertTrue(myokit.FORCE_PYSIDE2)
-        self.assertFalse(myokit.FORCE_PYQT4)
+        self.assertFalse(myokit.FORCE_PYQT6)
         self.assertFalse(myokit.FORCE_PYQT5)
+        self.assertFalse(myokit.FORCE_PYSIDE6)
+        self.assertTrue(myokit.FORCE_PYSIDE2)
 
         # Invalid raises warning
         with open(self._temp_dir.path('myokit.ini'), 'w') as f:
             f.write('[gui]\nbackend=lalala\n')
         with WarningCollector() as c:
             self._config_module._load()
         self.assertIn('Expected values for backend are', c.text())
```

### Comparing `myokit-1.34.0/myokit/tests/test_datablock.py` & `myokit-1.35.0/myokit/tests/test_datablock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 #!/usr/bin/env python3
 #
 # Tests the DataBlock1d and DataBlock2d classes
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 
 from myokit.tests import (
     TemporaryDirectory,
     DIR_DATA,
     DIR_IO,
     TestReporter,
     CancellingReporter,
     WarningCollector,
 )
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class DataBlock1dTest(unittest.TestCase):
     """
     Tests the DataBlock1d
     """
     def test_combined(self):
         # Runs a combined test of:
```

### Comparing `myokit-1.34.0/myokit/tests/test_datalog.py` & `myokit-1.35.0/myokit/tests/test_datalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,47 +1,30 @@
 #!/usr/bin/env python3
 #
 # Tests the DataLog class
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 
 from myokit.tests import (
     DIR_DATA,
     DIR_IO,
     TemporaryDirectory,
     TestReporter,
     CancellingReporter,
     WarningCollector,
 )
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
-# Universal newline mode in Python 2 and 3
-def uopen(filename):
-    try:
-        return open(filename, 'r', newline=None)
-    except TypeError:
-        return open(filename, 'U')
-
-
 # Extra output
 debug = False
 
 
 class DataLogTest(unittest.TestCase):
     """
     Tests the DataLog's functions.
@@ -1391,20 +1374,20 @@
         d = myokit.DataLog(time='a.b')
         d['a.b'] = np.arange(0, 100)
         d['c.d'] = np.sqrt(np.arange(0, 100) * 1.2)
         d['e.f'] = np.arange(0, 100) + 1
         with TemporaryDirectory() as td:
             fname = td.path('test.csv')
             d.save_csv(fname, order=['a.b', 'c.d', 'e.f'])
-            with uopen(fname) as f:
+            with open(fname, 'r', newline=None) as f:
                 header = f.readline()
             self.assertEqual(header, '"a.b","c.d","e.f"\n')
 
             d.save_csv(fname, order=['e.f', 'a.b', 'c.d'])
-            with uopen(fname) as f:
+            with open(fname, 'r', newline=None) as f:
                 header = f.readline()
             self.assertEqual(header, '"e.f","a.b","c.d"\n')
 
             # Test invalid order
             self.assertRaises(
                 ValueError, d.save_csv, fname, order=['e.f', 'a.b', 'c.e'])
 
@@ -1418,15 +1401,15 @@
         d['100.z.a'] = np.arange(10) * 100
         d['2.z.a'] = np.arange(10) * 2
         d['11.z.a'] = np.arange(10) * 11
         d['14.z.a'] = np.arange(10) * 10
         with TemporaryDirectory() as td:
             fname = td.path('test.csv')
             d.save_csv(fname)
-            with uopen(fname) as f:
+            with open(fname, 'r', newline=None) as f:
                 order = [x[1:-1] for x in f.readline().strip().split(',')]
             self.assertEqual(len(order), 9)
             self.assertEqual(order[0], 'e.t')
             self.assertEqual(order[1], '0.z.a')
             self.assertEqual(order[2], '1.z.a')
             self.assertEqual(order[3], '2.z.a')
             self.assertEqual(order[4], '11.z.a')
```

### Comparing `myokit-1.34.0/myokit/tests/test_dependency_checking.py` & `myokit-1.35.0/myokit/tests/test_dependency_checking.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,36 +2,21 @@
 #
 # Tests the dependency resolving and sorting to solvable order in the myokit
 # core.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 
 from myokit.tests import DIR_DATA
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
-
 
 # Extra output
 debug = False
 
 
 class DepTest(unittest.TestCase):
     """
@@ -51,24 +36,24 @@
     def has_lhs(self, depmap, key, *deps):
         """
         Check if the depmap entry for lhs contains all deps, and only those
         deps.
         """
         # If a string lhs is given, interpret it as a variable name and get
         # the lhs of its defining equation
-        if isinstance(key, basestring):
+        if isinstance(key, str):
             key = self.m.get(key)
             if isinstance(key, myokit.Variable):
                 key = key.lhs()
 
         # Convert deps list to list of objects. If a string name is given,
         # convert it to a Name. Ensure no duplicates are given.
         deps = list(set(deps))
         for k, dep in enumerate(deps):
-            if isinstance(dep, basestring):
+            if isinstance(dep, str):
                 deps[k] = self.n(dep)
 
         # Get dep map
         self.assertIn(key, depmap)
         dmap = depmap[key]
 
         # Show what will be tested
@@ -445,15 +430,15 @@
         head = self.head
         depmap = m.map_deep_dependencies(omit_states=True)
 
         def has(lhs, *deps):
             return self.has_lhs(depmap, lhs, *deps)
 
         def nhas(lhs):
-            if isinstance(lhs, basestring):
+            if isinstance(lhs, str):
                 lhs = self.m.get(lhs).lhs()
             self.assertNotIn(lhs, depmap)
 
         # Start testing
         head('Deep dependency mapping')
         head('Testing engine component')
         has('engine.time')
@@ -590,15 +575,15 @@
         head = self.head
         depmap = m.map_deep_dependencies(omit_states=False, collapse=True)
 
         def has(lhs, *deps):
             return self.has_lhs(depmap, lhs, *deps)
 
         def nhas(lhs):
-            if isinstance(lhs, basestring):
+            if isinstance(lhs, str):
                 lhs = self.m.get(lhs).lhs()
             self.assertNotIn(lhs, depmap)
 
         # Start testing
         head('Deep dependency mapping')
         head('Testing engine component')
         has('engine.time')
@@ -1356,18 +1341,18 @@
                 lhs = self.m.get(lhs).lhs()
             for eq in self.order[self.ccomp]:
                 if eq.lhs == lhs:
                     return eq
 
         def before(lhs1, *lhs2s):
             """ Asserts lhs1 comes before lhs2 in the current component """
-            if isinstance(lhs1, basestring):
+            if isinstance(lhs1, str):
                 lhs1 = self.m.get(self.ccomp + '.' + lhs1).lhs()
             for lhs2 in lhs2s:
-                if isinstance(lhs2, basestring):
+                if isinstance(lhs2, str):
                     lhs2 = self.m.get(self.ccomp + '.' + lhs2).lhs()
                 i1 = i2 = None
                 for i, eq in enumerate(self.order[self.ccomp]):
                     if eq.lhs == lhs1:
                         i1 = i
                         if i2:
                             break
@@ -1504,22 +1489,22 @@
         self.assertTrue(m.has_interdependent_components())
 
     def test_expressions_for(self):
         # Test Model.expressions_for().
 
         def before(lhs1, *lhs2s):
             """ Asserts lhs2 comes before lhs1 """
-            if isinstance(lhs1, basestring):
+            if isinstance(lhs1, str):
                 if lhs1.startswith('dot('):
                     lhs1 = myokit.Derivative(myokit.Name(
                         self.m.get(lhs1[4:-1])))
                 else:
                     lhs1 = myokit.Name(self.m.get(lhs1))
             for lhs2 in lhs2s:
-                if isinstance(lhs2, basestring):
+                if isinstance(lhs2, str):
                     if lhs2.startswith('dot('):
                         lhs2 = myokit.Derivative(myokit.Name(
                             self.m.get(lhs2[4:-1])))
                     else:
                         lhs2 = myokit.Name(self.m.get(lhs2))
                 i1 = i2 = None
                 for i, eq in enumerate(self.eqs):
```

### Comparing `myokit-1.34.0/myokit/tests/test_expressions.py` & `myokit-1.35.0/myokit/tests/test_expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 #!/usr/bin/env python3
 #
 # Tests the expression classes.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import pickle
 import unittest
 
 import numpy as np
 
 import myokit
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 # Unit --> See test_units.py
 # Quantity --> See test_units.py
 
 
 # Tiny model for partial derivative testing.
 pd_model = myokit.parse_model("""
```

### Comparing `myokit-1.34.0/myokit/tests/test_float.py` & `myokit-1.35.0/myokit/tests/test_float.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 #
 # Tests the methods and classes in myokit.floats
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import sys
 import unittest
 
 import myokit
 
 
 class FloatTest(unittest.TestCase):
@@ -87,16 +84,15 @@
         self.assertNotEqual(-49, myokit.float.round(-x))
         self.assertEqual(-0.5, myokit.float.round(-0.5))
 
     def test_str(self):
         # Test float to string conversion.
 
         # String should be passed through
-        # Note: convert to str() to test in python 2 and 3.
-        self.assertEqual(myokit.float.str(str('123')), '123')
+        self.assertEqual(myokit.float.str('123'), '123')
 
         # Simple numbers
         self.assertEqual(myokit.float.str(0), '0')
         self.assertEqual(myokit.float.str(0.0000), '0.0')
         self.assertEqual(myokit.float.str(1.234), '1.234')
         self.assertEqual(
             myokit.float.str(0.12432656245e12), ' 1.24326562450000000e+11')
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats.py` & `myokit-1.35.0/myokit/tests/test_formats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 #!/usr/bin/env python3
 #
 # Tests shared infrastructure in myokit.formats.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 import myokit.formats
 
 from myokit.tests import TemporaryDirectory
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class FormatsTest(unittest.TestCase):
     """
     Test infrastructure from the formats module.
     """
 
     def test_register_external_importer(self):
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_axon.py` & `myokit-1.35.0/myokit/tests/test_formats_axon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 #!/usr/bin/env python3
 #
 # Tests the Axon format module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 import myokit.formats.axon as axon
 
 from myokit.tests import TemporaryDirectory, DIR_FORMATS
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class AbfTest(unittest.TestCase):
     """
     Tests the ABF format support.
     """
 
     def test_read_v1(self):
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_cellml.py` & `myokit-1.35.0/myokit/tests/test_formats_cellml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 #
 # Tests the CellML importer, exporter, and expression writer.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import re
 import unittest
 
 import myokit
 import myokit.formats as formats
 import myokit.formats.cellml as cellml
@@ -19,26 +16,14 @@
 from myokit.formats.cellml import CellMLImporterError
 
 from myokit.tests import TemporaryDirectory, DIR_FORMATS, WarningCollector
 
 # CellML dir
 DIR = os.path.join(DIR_FORMATS, 'cellml')
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
-
 
 class CellMLExporterTest(unittest.TestCase):
     """
     Tests for :class:`myokit.formats.cellml.CellMLExporter`.
     """
 
     def test_capability_reporting(self):
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_channelml.py` & `myokit-1.35.0/myokit/tests/test_formats_channelml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,26 @@
 #!/usr/bin/env python3
 #
 # Tests the importers for various formats
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 import myokit.formats
 import myokit.formats.channelml
 
 from myokit.tests import DIR_FORMATS, WarningCollector
 
 # ChannelML dir
 DIR = os.path.join(DIR_FORMATS, 'channelml')
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:  # pragma: no python 3 cover
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
-
 
 class ChannelMLTest(unittest.TestCase):
     """ Test ChannelML importing. """
 
     def test_capability_reporting(self):
         # Test if the right capabilities are reported.
         i = myokit.formats.importer('channelml')
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_easyml.py` & `myokit-1.35.0/myokit/tests/test_formats_easyml.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,23 @@
 #!/usr/bin/env python3
 #
 # Tests the EasyML module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 import myokit.formats
 import myokit.formats.easyml
 
 from myokit.tests import TemporaryDirectory, WarningCollector, DIR_DATA
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:  # pragma: no python 3 cover
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
 
 # Model that requires unit conversion
 units_model = """
 [[model]]
 membrane.V = -0.08
 hh.x = 0.1
 hh.y = 0.9
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_exporters.py` & `myokit-1.35.0/myokit/tests/test_formats_exporters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,33 @@
 #!/usr/bin/env python3
 #
 # Tests the exporters from the format module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 import myokit.formats
 
 from myokit.tests import TemporaryDirectory
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:  # pragma: no python 3 cover
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
-
 
 class ExportTest(unittest.TestCase):
     """
     Tests various exporters.
     """
 
     def _test(self, e, model=None, protocol=None):
         """ Test a given exporter `e`. """
 
         # Test info method.
-        self.assertIsInstance(e.post_export_info(), basestring)
+        self.assertIsInstance(e.post_export_info(), str)
 
         # Load model, protocol
         m, p = model, protocol
         if m is None:
             m = myokit.load_model('example')
         if p is None:
             p = myokit.load_protocol('example')
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_expression_writers.py` & `myokit-1.35.0/myokit/tests/test_formats_expression_writers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,55 +1,39 @@
 #!/usr/bin/env python3
 #
 # Tests the expression writer classes.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 import myokit.formats
 import myokit.formats.ansic
 import myokit.formats.cpp
 import myokit.formats.latex
 import myokit.formats.matlab
 import myokit.formats.python
 import myokit.formats.stan
 
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:  # pragma: no python 3 cover
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
-
-
 class ExpressionWriterTest(unittest.TestCase):
     """ Test shared expression writer functionality. """
 
     def test_ewriter_interface(self):
         # Test listing and creating expression writers.
 
         # Test listing
         es = myokit.formats.ewriters()
         self.assertTrue(len(es) > 0)
 
         # Create one of each
         for e in es:
-            self.assertIsInstance(e, basestring)
+            self.assertIsInstance(e, str)
             e = myokit.formats.ewriter(e)
             self.assertTrue(isinstance(e, myokit.formats.ExpressionWriter))
 
     def test_unknown(self):
         # Test requesting an unknown expression writer.
         # Test fetching using ewriter method
         self.assertRaisesRegex(
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_html.py` & `myokit-1.35.0/myokit/tests/test_formats_html.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 #
 # Tests the HTML support functions.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit.formats.html
 
 
 html = """
 <!DOCTYPE html>
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_importers.py` & `myokit-1.35.0/myokit/tests/test_formats_importers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,32 @@
 #!/usr/bin/env python3
 #
 # Tests the importers for various formats
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 import myokit.formats as formats
 
 from myokit.tests import DIR_FORMATS
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:  # pragma: no python 3 cover
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
-
 
 class ImporterTest(unittest.TestCase):
     """ Test shared importer functionality. """
 
     def test_importer_interface(self):
         # Test listing and creating importers.
         ims = myokit.formats.importers()
         self.assertTrue(len(ims) > 0)
         for i in ims:
-            self.assertIsInstance(i, basestring)
+            self.assertIsInstance(i, str)
             i = myokit.formats.importer(i)
             self.assertTrue(isinstance(i, myokit.formats.Importer))
 
     def test_unknown(self):
         # Test requesting an unknown importer.
         # Test fetching using importer method
         self.assertRaisesRegex(
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_mathml_content.py` & `myokit-1.35.0/myokit/tests/test_formats_mathml_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 #!/usr/bin/env python3
 #
 # Tests the parser and expression writer for content MathML.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import re
 import unittest
 
 import lxml.etree as etree
 
 import myokit
 import myokit.formats.mathml as mathml
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class ContentMathMLParserTest(unittest.TestCase):
     """ Tests content MathML parsing. """
 
     def p(self, xml):
         """ Parses a MathML string and returns a myokit.Expression. """
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_mathml_presentation.py` & `myokit-1.35.0/myokit/tests/test_formats_mathml_presentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 #!/usr/bin/env python3
 #
 # Tests the MathML expression writer in presentation mode.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import re
 import unittest
 
 import myokit
 import myokit.formats.mathml as mathml
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class PresentationMathMLTest(unittest.TestCase):
     """
     Tests export of presentation MathML.
     """
 
     @classmethod
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_opencl.py` & `myokit-1.35.0/myokit/tests/test_formats_opencl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 #!/usr/bin/env python3
 #
 # Tests the expression writer for OpenCL.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 import myokit.formats
 import myokit.formats.opencl
 
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:  # pragma: no python 3 cover
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
 class OpenCLExpressionWriterTest(unittest.TestCase):
     """ Test the OpenCL ewriter class. """
 
     def test_basic(self):
 
         # Single and double precision and native maths
         ws = myokit.formats.opencl.OpenCLExpressionWriter()
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_sbml.py` & `myokit-1.35.0/myokit/tests/test_formats_sbml.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,26 @@
 #!/usr/bin/env python3
 #
 # Tests Myokit's SBML support.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import numpy as np
 
 import myokit
 import myokit.formats
 import myokit.formats.sbml
 
 # from shared import DIR_FORMATS, WarningCollector
 from myokit.tests import DIR_FORMATS, WarningCollector
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:  # pragma: no python 3 cover
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
-
 
 class SBMLImporterTest(unittest.TestCase):
     """
     Tests the SBMLImporter.
     """
 
     def test_capability_reporting(self):
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_sympy.py` & `myokit-1.35.0/myokit/tests/test_formats_sympy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 #!/usr/bin/env python3
 #
 # Tests the importers for various formats
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 import myokit.formats.sympy as mypy
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class SymPyReadWriteTest(unittest.TestCase):
     """
     Tests the SymPy ewriter and ereader classes.
     """
 
     @classmethod
```

### Comparing `myokit-1.34.0/myokit/tests/test_formats_wcp.py` & `myokit-1.35.0/myokit/tests/test_formats_wcp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/env python3
 #
 # Tests the WCP format module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit.formats.wcp as wcp
 
 from myokit.tests import DIR_FORMATS
```

### Comparing `myokit-1.34.0/myokit/tests/test_io.py` & `myokit-1.35.0/myokit/tests/test_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,23 @@
 #
 # Tests the loading/saveing mmt files and states.
 # See also test_parsing.py
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 
 from myokit.tests import DIR_DATA, TemporaryDirectory
 
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:
-    basestring = str
-
 
 class LoadSaveMmtTest(unittest.TestCase):
     """Tests load/save functions for mmt files."""
 
     def test_examplify(self):
         # Test _examplify.
         self.assertEqual(myokit._io._examplify('test.txt'), 'test.txt')
@@ -101,15 +93,15 @@
         self.assertIsNone(m)
         self.assertIsInstance(p, myokit.Protocol)
         self.assertIsNone(x)
 
         m, p, x = myokit.load(spath)
         self.assertIsNone(m)
         self.assertIsNone(p)
-        self.assertTrue(isinstance(x, basestring))
+        self.assertTrue(isinstance(x, str))
 
         self.assertRaises(
             myokit.SectionNotFoundError, myokit.load_model, ppath)
         self.assertRaises(
             myokit.SectionNotFoundError, myokit.load_model, spath)
         self.assertRaises(
             myokit.SectionNotFoundError, myokit.load_protocol, mpath)
@@ -124,15 +116,15 @@
         # Test if the correct parts are saved/loaded from disk using the
         # ``save()`` method.
 
         # Test example loading
         m, p, x = myokit.load('example')
         self.assertIsInstance(m, myokit.Model)
         self.assertIsInstance(p, myokit.Protocol)
-        self.assertTrue(isinstance(x, basestring))
+        self.assertTrue(isinstance(x, str))
 
         # Save all three and reload
         with TemporaryDirectory() as d:
             opath = d.path('test.mmt')
             myokit.save(opath, m, p, x)
             mm, pp, xx = myokit.load(opath)
             self.assertEqual(m.code(), mm.code())
@@ -314,30 +306,30 @@
     def test_save_script(self):
         # Test if the correct parts are saved/loaded from disk using the
         # ``save_script()`` method.
 
         ipath = os.path.join(DIR_DATA, 'lr-1991.mmt')
         # Test example loading
         x = myokit.load_script('example')
-        self.assertTrue(isinstance(x, basestring))
+        self.assertTrue(isinstance(x, str))
         # Test file loading
         x = myokit.load_script(ipath)
-        self.assertTrue(isinstance(x, basestring))
+        self.assertTrue(isinstance(x, str))
         with TemporaryDirectory() as d:
             opath = d.path('test.mmt')
             myokit.save_script(opath, x)
             # Test no other parts were written
             with open(opath, 'r') as f:
                 text = f.read()
             self.assertFalse('[[model]]' in text)
             self.assertFalse('[[protocol]]' in text)
             self.assertTrue('[[script]]' in text)
             # Test reloading
             xx = myokit.load_script(opath)
-            self.assertTrue(isinstance(xx, basestring))
+            self.assertTrue(isinstance(xx, str))
             self.assertEqual(x, xx)
 
 
 class LoadSaveStateTest(unittest.TestCase):
     """Tests loading and saving states."""
 
     def test_load_save_state(self):
```

### Comparing `myokit-1.34.0/myokit/tests/test_jacobian_calculator.py` & `myokit-1.35.0/myokit/tests/test_jacobian_calculator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 #!/usr/bin/env python3
 #
 # Tests the Jacobian calculator.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 
 from myokit.tests import DIR_DATA
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class JacobianCalculatorTest(unittest.TestCase):
     """
     Tests the JacobianCalculator.
     """
     def test_simple(self):
         # Load model
```

### Comparing `myokit-1.34.0/myokit/tests/test_jacobian_tracer.py` & `myokit-1.35.0/myokit/tests/test_jacobian_tracer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 #!/usr/bin/env python3
 #
 # Tests the Jacobian tracer.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 
 from myokit.tests import DIR_DATA
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class JacobianTracerTest(unittest.TestCase):
     """
     Tests the JacobianTracer.
     """
     def test_simple(self):
         # Load model
```

### Comparing `myokit-1.34.0/myokit/tests/test_lib_deps.py` & `myokit-1.35.0/myokit/tests/test_lib_deps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 #!/usr/bin/env python3
 #
 # Tests the lib.deps dependency graphing module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import random
 import unittest
 
 import myokit
 import myokit.lib.deps as deps
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class LibDepsTest(unittest.TestCase):
 
     def test_state_dependency_matrix(self):
         # Test create_ and plot_ state dependency matrix method, to create
         # matrix plot of state interdependencies.
```

### Comparing `myokit-1.34.0/myokit/tests/test_lib_guess.py` & `myokit-1.35.0/myokit/tests/test_lib_guess.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 #!/usr/bin/env python3
 #
 # Tests the lib.guess variable meaning guessing module
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 import myokit.lib.guess as guess
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class LibGuessTest(unittest.TestCase):
     """
     Tests for ``myokit.lib.guess``.
     """
 
     def test_add_embedded_protocol_pacing(self):
```

### Comparing `myokit-1.34.0/myokit/tests/test_lib_hh.py` & `myokit-1.35.0/myokit/tests/test_lib_hh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 #!/usr/bin/env python3
 #
 # Tests the lib.hh module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 import myokit.lib.hh as hh
 
 from myokit.tests import DIR_DATA
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 MODEL = """
 [[model]]
 membrane.V = -80
 ikr.a = 4.5e-4
 ikr.r = 0.15
 ina.r = 0.15
```

### Comparing `myokit-1.34.0/myokit/tests/test_lib_markov.py` & `myokit-1.35.0/myokit/tests/test_lib_markov.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 #!/usr/bin/env python3
 #
 # Tests the lib.markov module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 import myokit.lib.markov as markov
 
 from myokit.tests import DIR_DATA, WarningCollector
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class LinearModelTest(unittest.TestCase):
     """
     Tests the linear model class.
     """
 
     def test_manual_creation(self):
```

### Comparing `myokit-1.34.0/myokit/tests/test_lib_multi.py` & `myokit-1.35.0/myokit/tests/test_lib_multi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 #!/usr/bin/env python3
 #
 # Tests the myokit.lib.multi module.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 
 from myokit.tests import DIR_DATA, WarningCollector
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 # Path to multi-model testing files
 DIR_MULTI = os.path.join(DIR_DATA, 'multi')
 
 
 class LibMultiTest(unittest.TestCase):
     """
     Tests the myokit.lib.multi module.
```

### Comparing `myokit-1.34.0/myokit/tests/test_lib_plots.py` & `myokit-1.35.0/myokit/tests/test_lib_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 #
 # Tests if the myokit.lib.plots module runs without exceptions, doesn't inspect
 # the output.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 import myokit.lib.plots as plots
 
 from myokit.tests import DIR_DATA, WarningCollector
```

### Comparing `myokit-1.34.0/myokit/tests/test_meta.py` & `myokit-1.35.0/myokit/tests/test_meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 #
 # Tests meta data functions in myokit.Model
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 
 
 class MetaTest(unittest.TestCase):
     """
```

### Comparing `myokit-1.34.0/myokit/tests/test_model.py` & `myokit-1.35.0/myokit/tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,33 +4,23 @@
 #
 # Notes:
 #  - Tests for dependency checking in models are in `test_dependency_checking`.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import pickle
 import re
 import unittest
 
 import myokit
 
 from myokit.tests import TemporaryDirectory, WarningCollector
 
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
 class ModelTest(unittest.TestCase):
     """
     Tests parts of :class:`myokit.Model`.
     """
 
     def test_add_component_allow_renamining(self):
         # Test the ``Model.add_component_allow_renaming`` method.
```

### Comparing `myokit-1.34.0/myokit/tests/test_model_building.py` & `myokit-1.35.0/myokit/tests/test_model_building.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,17 @@
 #
 # NOTE: THESE TESTS SHOULD SLOWLY BE MERGED INTO test_model, test_variable, etc
 #
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
 import unittest
 
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:
-    basestring = str
-
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 # Further model API tests are found in:
 #  - test_dependency_checking.py
 
 
 class ModelBuildTest(unittest.TestCase):
 
     def test_model_creation(self):
@@ -296,18 +281,18 @@
         eq = [eq for eq in m.equations(deep=False)]
         self.assertEqual(len(eq), 8)
         eq = [eq for eq in m.equations(deep=True)]
         self.assertEqual(len(eq), 10)
 
         # Test dependency mapping
         def has(var, *dps):
-            lst = vrs[m.get(var).lhs() if isinstance(var, basestring) else var]
+            lst = vrs[m.get(var).lhs() if isinstance(var, str) else var]
             self.assertEqual(len(lst), len(dps))
             for d in dps:
-                d = m.get(d).lhs() if isinstance(d, basestring) else d
+                d = m.get(d).lhs() if isinstance(d, str) else d
                 self.assertIn(d, lst)
 
         vrs = m.map_shallow_dependencies(omit_states=False)
         self.assertEqual(len(vrs), 12)
         has('X.a')
         has('X.b', 'X.b.b1', 'X.b.b2')
         has('X.b.b1')
```

### Comparing `myokit-1.34.0/myokit/tests/test_opencl_info.py` & `myokit-1.35.0/myokit/tests/test_opencl_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 #!/usr/bin/env python3
 #
 # Tests the OpenCL info class.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 
 from myokit.tests import TemporaryDirectory, OpenCL_FOUND
 
-# Strings in Python2 and Python3
-try:
-    basestring
-except NameError:
-    basestring = str
-
 
 @unittest.skipIf(not OpenCL_FOUND, 'OpenCL not found on this system.')
 class OpenCLTest(unittest.TestCase):
     """
     Tests the OpenCL info class.
     """
 
@@ -31,20 +22,20 @@
         # Tested as condition to get in, so must be true
         self.assertTrue(myokit.OpenCL.available())
 
     def test_current_info(self):
         # Tests the method to query the current device
         self.assertIsInstance(
             myokit.OpenCL.current_info(), myokit.OpenCLPlatformInfo)
-        self.assertIsInstance(myokit.OpenCL.current_info(True), basestring)
+        self.assertIsInstance(myokit.OpenCL.current_info(True), str)
 
     def test_info(self):
         # Tests the method to query the current device
         self.assertIsInstance(myokit.OpenCL.info(), myokit.OpenCLInfo)
-        self.assertIsInstance(myokit.OpenCL.info(True), basestring)
+        self.assertIsInstance(myokit.OpenCL.info(True), str)
 
     def test_load_save_selection(self):
         # Tests the load_selection method
         import myokit._sim.opencl
         org_name = myokit._sim.opencl.SETTINGS_FILE
         try:
             with TemporaryDirectory() as d:
@@ -79,17 +70,17 @@
         # Tests getting info about devices, specifically for device selection
         info = myokit.OpenCL.selection_info()
         self.assertIsInstance(info, list)
         self.assertGreater(len(info), 0)
         item = info[0]
         self.assertEqual(len(item), 3)
         platform, device, specs = item
-        self.assertIsInstance(platform, basestring)
-        self.assertIsInstance(device, basestring)
-        self.assertIsInstance(specs, basestring)
+        self.assertIsInstance(platform, str)
+        self.assertIsInstance(device, str)
+        self.assertIsInstance(specs, str)
 
     def test_supported(self):
         # Tested as condition to get in, so must be true
         self.assertTrue(myokit.OpenCL.supported())
 
     def test_hidden(self):
         # Tests some private methods of the opencl module
```

### Comparing `myokit-1.34.0/myokit/tests/test_pacing_factory.py` & `myokit-1.35.0/myokit/tests/test_pacing_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 #
 # Tests protocol creation via myokit.pacing
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 
 
 class PacingFactoryTest(unittest.TestCase):
     """
```

### Comparing `myokit-1.34.0/myokit/tests/test_pacing_system_c.py` & `myokit-1.35.0/myokit/tests/test_pacing_system_c.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 #!/usr/bin/env python3
 #
 # Tests the C implementation of the Pacing System
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 import numpy as np
 
 import myokit
 
 from myokit.tests.ansic_event_based_pacing import AnsicEventBasedPacing
 from myokit.tests.ansic_fixed_form_pacing import AnsicFixedFormPacing
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class EventBasedPacingAnsicTest(unittest.TestCase):
     """
     Tests the C implementation of event based pacing.
     """
     def test_with_event_at_t_0(self):
         # Test with event starting at t=0
```

### Comparing `myokit-1.34.0/myokit/tests/test_pacing_system_py.py` & `myokit-1.35.0/myokit/tests/test_pacing_system_py.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 #!/usr/bin/env python3
 #
 # Tests the pure Python implementation of the Pacing System
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class EventBasedPacingPythonTest(unittest.TestCase):
     """
     Tests the pure python PacingSystem class.
     """
     def test_with_event_at_t_0(self):
         # Test with event starting at t=0
```

### Comparing `myokit-1.34.0/myokit/tests/test_parsing.py` & `myokit-1.35.0/myokit/tests/test_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,22 @@
 #
 # Tests the parsing module.
 # See also test_io.py
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import myokit
 import myokit.units
 
 from myokit.tests import DIR_DATA, TemporaryDirectory
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
-
 
 class TokenizerTest(unittest.TestCase):
     """
     Tests the tokenizer class.
     """
 
     def test_tokenizer(self):
@@ -904,37 +889,37 @@
         from myokit._parsing import parse_script
 
         # Test simple
         code = (
             '[[script]]',
         )
         script = parse_script(code)
-        self.assertIsInstance(script, basestring)
+        self.assertIsInstance(script, str)
         script = parse_script(''.join(code))
-        self.assertIsInstance(script, basestring)
+        self.assertIsInstance(script, str)
 
         code = (
             '[[script]]\n',
         )
         script = parse_script(code)
-        self.assertIsInstance(script, basestring)
+        self.assertIsInstance(script, str)
 
         code = (
             '[[script]]\n',
             'print("hi")',
         )
         script = parse_script(code)
-        self.assertIsInstance(script, basestring)
+        self.assertIsInstance(script, str)
 
         code = (
             '[[script]]\n',
             'print("hi")\n',
         )
         script = parse_script(code)
-        self.assertIsInstance(script, basestring)
+        self.assertIsInstance(script, str)
 
         # Not a script
         code = (
             '[[hello]]\n',
             'print("hi")\n',
         )
         self.assertRaisesRegex(
```

### Comparing `myokit-1.34.0/myokit/tests/test_progress_reporters.py` & `myokit-1.35.0/myokit/tests/test_progress_reporters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 #
 # Tests some of the ProgressReporter classes.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 import re
 import time
 
 import myokit
```

### Comparing `myokit-1.34.0/myokit/tests/test_protocol.py` & `myokit-1.35.0/myokit/tests/test_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 #!/usr/bin/env python3
 #
 # Tests protocol creation and pacing
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import pickle
 import unittest
 
 import myokit
 
 from myokit.tests import WarningCollector
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class ProtocolTest(unittest.TestCase):
     """
     Tests the Protocol class.
     """
 
     def test_characteristic_time(self):
```

### Comparing `myokit-1.34.0/myokit/tests/test_protocol_floating_point.py` & `myokit-1.35.0/myokit/tests/test_protocol_floating_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,20 @@
 #
 # To avoid this, we should use slightly more careful ways of comparing floating
 # point numbers if all protocol handling code.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 
 from myokit.tests.ansic_event_based_pacing import AnsicEventBasedPacing
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class ProtocolFloatingPointTest(unittest.TestCase):
 
     def test_is_sequence_and_length_floats_1(self):
 
         # Tests how float issues are handled in characteristic_time,
         # is_sequence, and is_unbroken_sequence
```

### Comparing `myokit-1.34.0/myokit/tests/test_protocol_time_series.py` & `myokit-1.35.0/myokit/tests/test_protocol_time_series.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 #!/usr/bin/env python3
 #
 # Tests the time series protocol class
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 import pickle
 
 import myokit
 
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
 class TimeSeriesProtocolTest(unittest.TestCase):
     """
     Tests the TimeSeriesProtocol class.
     """
 
     def test_eq(self):
         # Equality testing
```

### Comparing `myokit-1.34.0/myokit/tests/test_pype.py` & `myokit-1.35.0/myokit/tests/test_pype.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 #!/usr/bin/env python3
 #
 # Tests the parser
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 import myokit.pype
 
 from myokit.tests import TemporaryDirectory
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class PypeTest(unittest.TestCase):
 
     def test_process_errors(self):
         # Test error handling in the ``process`` method.
 
         # Process method takes a dict
```

### Comparing `myokit-1.34.0/myokit/tests/test_quantity.py` & `myokit-1.35.0/myokit/tests/test_quantity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 #!/usr/bin/env python3
 #
 # Tests the Quantity class
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class QuantityTest(unittest.TestCase):
     """
     Tests the Quantity class for unit arithmetic.
     """
 
     def test_as_rhs(self):
```

### Comparing `myokit-1.34.0/myokit/tests/test_rhs_benchmarker.py` & `myokit-1.35.0/myokit/tests/test_rhs_benchmarker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 #!/usr/bin/env python3
 #
 # Tests the RhsBenchmarker
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
+
 import numpy as np
 
 import myokit
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class RhsBenchmarkerTest(unittest.TestCase):
     """
     Tests :class:`RhsBenchmarker`.
     """
     def test_simple(self):
         # Test basic functionality.
```

### Comparing `myokit-1.34.0/myokit/tests/test_sbml_api.py` & `myokit-1.35.0/myokit/tests/test_sbml_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,24 @@
 #!/usr/bin/env python3
 #
 # Tests Myokit's SBML api.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 import myokit.formats
 import myokit.formats.sbml as sbml
 
 from myokit.formats.sbml._api import _MyokitConverter as X
 
 from myokit.tests import WarningCollector
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:  # pragma: no python 3 cover
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
-
 
 class TestCompartment(unittest.TestCase):
     """
     Unit tests for :class:`Compartment`.
     """
 
     @classmethod
```

### Comparing `myokit-1.34.0/myokit/tests/test_sbml_parser.py` & `myokit-1.35.0/myokit/tests/test_sbml_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,23 @@
 #!/usr/bin/env python3
 #
 # Tests Myokit's SBML support.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 import myokit.formats
 import myokit.formats.sbml
 from myokit.formats.sbml import SBMLParser, SBMLParsingError
 
 from myokit.tests import WarningCollector
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:  # pragma: no python 3 cover
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-# Strings in Python 2 and 3
-try:
-    basestring
-except NameError:   # pragma: no python 2 cover
-    basestring = str
-
 
 class TestSBMLParser(unittest.TestCase):
     """
     Unit tests for the SBMLParser class.
     """
 
     @classmethod
```

### Comparing `myokit-1.34.0/myokit/tests/test_simulation_1d.py` & `myokit-1.35.0/myokit/tests/test_simulation_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 #!/usr/bin/env python3
 #
 # Tests the Simulation1d class.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 
 from myokit.tests import DIR_DATA, CancellingReporter
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
 # Show simulation output
 debug = False
 
 
 class Simulation1dTest(unittest.TestCase):
     """
     Test the non-parallel 1d simulation.
```

### Comparing `myokit-1.34.0/myokit/tests/test_simulation_cvodes.py` & `myokit-1.35.0/myokit/tests/test_simulation_cvodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 #
 # Tests the CVODES simulation class.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import pickle
 import platform
 import re
 import sys
 import unittest
 
@@ -22,20 +19,14 @@
 from myokit.tests import (
     CancellingReporter,
     DIR_DATA,
     test_case_pk_model,
     WarningCollector,
 )
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class SimulationTest(unittest.TestCase):
     """
     Tests the CVODES simulation class.
     """
 
     @classmethod
@@ -293,21 +284,22 @@
         with WarningCollector() as w:
             self.sim.set_fixed_form_protocol(times, values)
         self.assertIn('eprecated', w.text())
         self.sim.reset()
         d = self.sim.run(n, log_interval=1)
         self.assertEqual(list(d.time()), times)
         self.assertEqual(list(d['engine.pace']), values)
-        self.assertRaisesRegex(
-            ValueError, 'No times',
-            self.sim.set_fixed_form_protocol, values=values)
-        self.assertRaisesRegex(
-            ValueError, 'No values',
-            self.sim.set_fixed_form_protocol, times=times)
-        self.sim.set_fixed_form_protocol(None)
+        with WarningCollector() as w:
+            self.assertRaisesRegex(
+                ValueError, 'No times',
+                self.sim.set_fixed_form_protocol, values=values)
+            self.assertRaisesRegex(
+                ValueError, 'No values',
+                self.sim.set_fixed_form_protocol, times=times)
+            self.sim.set_fixed_form_protocol(None)
         self.sim.reset()
         d = self.sim.run(n, log_interval=1)
         self.assertEqual(list(d['engine.pace']), [0] * n)
 
         # Reset original protocol
         self.sim.set_protocol(self.protocol)
         self.sim.reset()
```

### Comparing `myokit-1.34.0/myokit/tests/test_simulation_cvodes_from_disk.py` & `myokit-1.35.0/myokit/tests/test_simulation_cvodes_from_disk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 #
 # Tests the CVODES simulation class, when using a precompiled simulation.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import numpy as np
 
 import myokit
```

### Comparing `myokit-1.34.0/myokit/tests/test_simulation_fiber_tissue.py` & `myokit-1.35.0/myokit/tests/test_simulation_fiber_tissue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 #!/usr/bin/env python3
 #
 # Tests the Fiber-tissue OpenCL simulation
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 
 from myokit.tests import (
     CancellingReporter,
     DIR_DATA,
     OpenCL_FOUND,
     WarningCollector,
 )
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
 # Show simulation output
 debug = False
 
 
 @unittest.skipIf(not OpenCL_FOUND, 'OpenCL not found on this system.')
 class FiberTissueSimulationTest(unittest.TestCase):
     """
```

### Comparing `myokit-1.34.0/myokit/tests/test_simulation_log_interval.py` & `myokit-1.35.0/myokit/tests/test_simulation_log_interval.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 #!/usr/bin/env python3
 #
 # Tests the simulation classes' interpretation of log_interval
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
 
 import numpy as np
 
 import myokit
 
 from myokit.tests import DIR_DATA
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 # Extra output
 debug = False
 
 
 class PeriodicTest(unittest.TestCase):
     """
     Tests a simulation class for consistent log entry timing.
```

### Comparing `myokit-1.34.0/myokit/tests/test_simulation_opencl.py` & `myokit-1.35.0/myokit/tests/test_simulation_opencl.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,38 +4,29 @@
 #
 # Comparisons against CVODE and Simulation1d (with various options e.g. rush
 # larsen and native maths) are given in other files.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 
 from myokit.tests import (
     CancellingReporter,
     DIR_DATA,
     OpenCL_FOUND,
     OpenCL_DOUBLE_PRECISION_CONNECTIONS,
     WarningCollector,
 )
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
 # Show simulation output
 debug = False
 
 
 @unittest.skipIf(not OpenCL_FOUND, 'OpenCL not found on this system.')
 class SimulationOpenCLTest(unittest.TestCase):
     """
```

### Comparing `myokit-1.34.0/myokit/tests/test_simulation_opencl_log_interval.py` & `myokit-1.35.0/myokit/tests/test_simulation_opencl_log_interval.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/env python3
 #
 # Tests the OpenCL simulation classes' interpretation of log_interval
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 
 from myokit.tests import OpenCL_FOUND, DIR_DATA, WarningCollector
 from myokit.tests.test_simulation_log_interval import PeriodicTest
```

### Comparing `myokit-1.34.0/myokit/tests/test_simulation_opencl_vs_cvode.py` & `myokit-1.35.0/myokit/tests/test_simulation_opencl_vs_cvode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 #!/usr/bin/env python3
 #
 # Tests the OpenCL simulation classes
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 
 from myokit.tests import OpenCL_DOUBLE_PRECISION, DIR_DATA
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
 # Show simulation output
 debug = False
 
 
 @unittest.skipIf(
     not OpenCL_DOUBLE_PRECISION,
     'OpenCL double precision extension not supported on selected device.')
```

### Comparing `myokit-1.34.0/myokit/tests/test_simulation_opencl_vs_sim1d.py` & `myokit-1.35.0/myokit/tests/test_simulation_opencl_vs_sim1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 #!/usr/bin/env python3
 #
 # Tests the OpenCL simulation classes
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import unittest
+
 import numpy as np
 
 import myokit
 
 from myokit.tests import OpenCL_DOUBLE_PRECISION, DIR_DATA
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
 # Show simulation output
 debug = False
 
 
 @unittest.skipIf(
     not OpenCL_DOUBLE_PRECISION,
     'OpenCL double precision extension not supported on selected device.')
```

### Comparing `myokit-1.34.0/myokit/tests/test_system_info.py` & `myokit-1.35.0/myokit/tests/test_system_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 #!/usr/bin/env python3
 #
 # Tests the system() method
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 
 
-# Strings in Python2 and Python3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
-
-
 class SystemInfoTest(unittest.TestCase):
     """
     Tests the system info method.
     """
 
     def test_system_info(self):
         import matplotlib
         matplotlib.use('template')
 
-        self.assertIsInstance(myokit.system(), basestring)
+        self.assertIsInstance(myokit.system(), str)
         with myokit.tools.capture():
             myokit.system(live_printing=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `myokit-1.34.0/myokit/tests/test_tools.py` & `myokit-1.35.0/myokit/tests/test_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 #!/usr/bin/env python3
 #
 # Tests the methods and classes in myokit.tools
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import os
 import re
 import sys
 import threading
 import time
 import unittest
 
-# Strings in Python2 and Python3
-try:
-    basestring
-except NameError:   # pragma: no cover
-    basestring = str
-
 import myokit
 
 from myokit.tests import TemporaryDirectory
 
 
 class BenchmarkerTest(unittest.TestCase):
     """Tests the ``Benchmarker``."""
```

### Comparing `myokit-1.34.0/myokit/tests/test_unit.py` & `myokit-1.35.0/myokit/tests/test_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 #!/usr/bin/env python3
 #
 # Tests the Unit class
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import myokit
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
 
 class MyokitUnitTest(unittest.TestCase):
 
     def test_create(self):
         # Test basic unit creation.
 
         myokit.Unit.parse_simple('mV')
```

### Comparing `myokit-1.34.0/myokit/tests/test_user_functions.py` & `myokit-1.35.0/myokit/tests/test_user_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,17 @@
 #!/usr/bin/env python
 #
 # Tests the UserFunction class.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 import myokit
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
 # Further testing in test_model.py
 
 
 class UserFunctionTest(unittest.TestCase):
     """ Tests :class:`UserFunction`. """
 
     def test_user_function(self):
```

### Comparing `myokit-1.34.0/myokit/tests/test_variable.py` & `myokit-1.35.0/myokit/tests/test_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 #!/usr/bin/env python3
 #
 # Tests the Variable class.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import unittest
 
 import numpy as np
 
 import myokit
 
 from myokit.tests import WarningCollector
 
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
-
-
 class VariableTest(unittest.TestCase):
     """
     Tests parts of :class:`myokit.Variable`.
     """
 
     def test_clamp(self):
         # Tests clamping a variable to a fixed value
```

### Comparing `myokit-1.34.0/myokit/tools.py` & `myokit-1.35.0/myokit/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,38 +2,30 @@
 # Myokit utility functions. This module gathers functions that are used in
 # Myokit, but are not particularly Myokit-dependent, i.e. they could easily be
 # stand-alone. Imported by default.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
+import io
 import os
 import re
 import shutil
 import stat
 import sys
 import tempfile
 import threading
 import timeit
 
-# StringIO in Python 2 and 3
-try:
-    from cStringIO import StringIO
-except ImportError:  # pragma: no python 2 cover
-    from io import StringIO
-
 
 # Natural sort regex
 _natural_sort_regex = re.compile('([0-9]+)')
 
 
-class Benchmarker(object):
+class Benchmarker:
     """
     Allows benchmarking using the with statement.
 
     Example::
 
         m,p,x = myokit.load('example')
         s = myokit.Simulation(m, p)
@@ -93,15 +85,15 @@
     def time(self):
         """
         Returns the time since benchmarking started (as a float, in seconds).
         """
         return timeit.default_timer() - self._start
 
 
-class capture(object):
+class capture:
     """
     Context manager that temporarily redirects the current standard output and
     error streams, and captures anything that's written to them.
 
     Example::
 
         with myokit.tools.capture() as a:
@@ -220,16 +212,16 @@
         # Save the current output / error streams
         self._org_out = sys.stdout
         self._org_err = sys.stderr
 
         # Redirect
         if not self._fd:
             # Create temporary output and error streams
-            self._tmp_out = StringIO()
-            self._tmp_err = StringIO()
+            self._tmp_out = io.StringIO()
+            self._tmp_err = io.StringIO()
 
             # Redirect, attempting to flush first
             try:
                 sys.stdout.flush()
             except AttributeError:  # pragma: no cover
                 pass
             finally:
@@ -387,33 +379,25 @@
         Returns the text captured from stderr, or an empty string if nothing
         was captured or capturing is still active.
         """
         if self._txt_err is None:
             return ''
         text = self._txt_err
 
-        # In Python 2, the text needs to be decoded from ascii
-        if sys.hexversion < 0x03000000:  # pragma: no python 3 cover
-            text = text.decode('ascii', 'ignore')
-
         return text
 
     def out(self):
         """
         Returns the text captured from stdout, or an empty string if nothing
         was captured or capturing is still active.
         """
         if self._txt_out is None:
             return ''
         text = self._txt_out
 
-        # In Python 2, the text needs to be decoded from ascii
-        if sys.hexversion < 0x03000000:  # pragma: no python 3 cover
-            text = text.decode('ascii', 'ignore')
-
         return text
 
     def text(self):
         """
         Returns the combined text captured from output and error text, if any
         (output first, then error text).
         """
```

### Comparing `myokit-1.34.0/myokit/units.py` & `myokit-1.35.0/myokit/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #
 # Easy access to predefined myokit units.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
-
 import myokit
 
 
 def _add(name, unit, quantifiable=False, output=False):
     """
     Adds the given unit to the local namespace and registers it with the myokit
     unit system.
```

### Comparing `myokit-1.34.0/myokit.egg-info/PKG-INFO` & `myokit-1.35.0/myokit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: myokit
-Version: 1.34.0
+Version: 1.35.0
 Summary: A simple interface to cardiac cellular electrophysiology
 Home-page: http://myokit.org
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/MichaelClerx/myokit/issues
 Project-URL: Documentation, http://docs.myokit.org
 Project-URL: Source Code, https://github.com/MichaelClerx/myokit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: optional
 Provides-Extra: gui
 Provides-Extra: pyqt
 Provides-Extra: pyside
```

### Comparing `myokit-1.34.0/myokit.egg-info/SOURCES.txt` & `myokit-1.35.0/myokit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 myokit/__init__.py
 myokit/__main__.py
 myokit/_aux.py
 myokit/_config.py
 myokit/_datablock.py
 myokit/_datalog.py
 myokit/_err.py
-myokit/_exec_new.py
-myokit/_exec_old.py
 myokit/_expressions.py
 myokit/_io.py
 myokit/_model_api.py
 myokit/_myokit_version.py
 myokit/_parsing.py
 myokit/_progress.py
 myokit/_protocol.py
```

### Comparing `myokit-1.34.0/setup.py` & `myokit-1.35.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #
 # SetupTools script for Myokit
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-from __future__ import absolute_import, division
-from __future__ import print_function, unicode_literals
 from setuptools import setup, find_packages
 
 
 # Get version number
 import os
 import sys
 sys.path.append(os.path.abspath('myokit'))
@@ -54,15 +52,14 @@
 
     # Classifiers for pypi
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Scientific/Engineering :: Chemistry',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering :: Medical Science Apps.',
         'Topic :: Scientific/Engineering :: Physics',
@@ -75,41 +72,44 @@
     include_package_data=True,
 
     # Register myokit as a shell script
     entry_points={
         'console_scripts': ['myokit = myokit.__main__:main']
     },
 
+    # Python version
+    python_requires='>=3.7',
+
     # List of dependencies
     install_requires=[
         'configparser',
         'lxml',
-        'matplotlib>=1.5',
+        'matplotlib>=2.2',
         'numpy',
         'setuptools',
         # PyQT or PySide?
         # (PySide is pip installable, Actions can get PyQt from apt)
     ],
 
     # Optional extras
     extras_require={
         'docs': [
-            'sphinx>=1.5, !=1.7.3',     # Doc generation
+            'sphinx>=1.7.4',        # Doc generation
         ],
         'dev': [
             'coverage',             # Coverage checking
             'flake8>=3',            # Style checking
         ],
         'optional': [
             'scipy',            # Used in data log, and data log viewer
             'sympy',            # Used in formats.sympy
         ],
-        'gui': ['pyqt5', 'sip'],
-        'pyqt': ['pyqt5', 'sip'],
-        'pyside': ['pyside2'],
+        'gui': ['pyqt6', 'sip'],
+        'pyqt': ['pyqt6', 'sip'],
+        'pyside': ['pyside6'],
     },
 
     # Unit tests
     test_suite='myokit.tests',
 
     # See: https://setuptools.pypa.io/en/latest/userguide/miscellaneous.html
     #      #setting-the-zip-safe-flag
```

