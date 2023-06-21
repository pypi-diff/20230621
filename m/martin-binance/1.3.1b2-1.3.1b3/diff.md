# Comparing `tmp/martin-binance-1.3.1b2.tar.gz` & `tmp/martin-binance-1.3.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin-binance-1.3.1b2.tar", last modified: Tue Jun 20 14:29:28 2023, max compression
+gzip compressed data, was "martin-binance-1.3.1b3.tar", last modified: Tue Jun 20 15:14:34 2023, max compression
```

## Comparing `martin-binance-1.3.1b2.tar` & `martin-binance-1.3.1b3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.1b2/.deepsource.toml
--rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.1b2/.dockerignore
--rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.1b2/.github/FUNDING.yml
--rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.1b2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.1b2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.1b2/.github/workflows/codeql.yml
--rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.1b2/.gitignore
--rwxr-xr-x   0        0        0    18795 2023-06-20 11:01:32.418813 martin-binance-1.3.1b2/CHANGELOG.md
--rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.1b2/Dockerfile
--rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.1b2/LICENSE
--rwxr-xr-x   0        0        0     3944 2023-06-19 19:17:03.912066 martin-binance-1.3.1b2/README.md
--rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.1b2/doc/Create_strategy.png
--rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.1b2/doc/Model of logarithmic grid.ods
--rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.1b2/doc/Modified martingale.svg
--rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.1b2/doc/graf1.png
--rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.1b2/doc/tlg_notify.png
--rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.1b2/doc/tmux.png
--rw-r--r--   0        0        0     1968 2023-06-20 14:29:09.195846 martin-binance-1.3.1b2/martin_binance/__init__.py
--rw-r--r--   0        0        0     3882 2023-06-19 19:16:08.328313 martin-binance-1.3.1b2/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2946 2023-06-10 10:09:47.513439 martin-binance-1.3.1b2/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-06-10 10:09:47.513439 martin-binance-1.3.1b2/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    14050 2023-06-19 19:16:08.304258 martin-binance-1.3.1b2/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6721 2023-06-19 17:47:04.745501 martin-binance-1.3.1b2/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6716 2023-06-19 17:47:04.745501 martin-binance-1.3.1b2/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6722 2023-06-19 17:47:04.745501 martin-binance-1.3.1b2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4707 2023-06-10 10:09:47.517442 martin-binance-1.3.1b2/martin_binance/client.py
--rw-r--r--   0        0        0   185525 2023-06-20 10:20:51.033666 martin-binance-1.3.1b2/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.1b2/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.1b2/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.1b2/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.1b2/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    85764 2023-06-19 21:29:05.366900 martin-binance-1.3.1b2/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.1b2/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.1b2/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.1b2/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16369 2023-06-19 17:47:04.749497 martin-binance-1.3.1b2/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-06-10 10:09:47.517442 martin-binance-1.3.1b2/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1274 2023-06-20 08:42:34.849378 martin-binance-1.3.1b2/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.1b2/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.1b2/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1303 2023-06-20 14:29:25.379899 martin-binance-1.3.1b2/pyproject.toml
--rw-r--r--   0        0        0      335 2023-06-19 19:16:08.288221 martin-binance-1.3.1b2/requirements.txt
--rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.1b2/uml/architecture.puml
--rw-r--r--   0        0        0     5151 1970-01-01 00:00:00.000000 martin-binance-1.3.1b2/PKG-INFO
+-rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.1b3/.deepsource.toml
+-rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.1b3/.dockerignore
+-rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.1b3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.1b3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.1b3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.1b3/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.1b3/.gitignore
+-rwxr-xr-x   0        0        0    18795 2023-06-20 11:01:32.418813 martin-binance-1.3.1b3/CHANGELOG.md
+-rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.1b3/Dockerfile
+-rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.1b3/LICENSE
+-rwxr-xr-x   0        0        0     3944 2023-06-19 19:17:03.912066 martin-binance-1.3.1b3/README.md
+-rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.1b3/doc/Create_strategy.png
+-rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.1b3/doc/Model of logarithmic grid.ods
+-rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.1b3/doc/Modified martingale.svg
+-rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.1b3/doc/graf1.png
+-rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.1b3/doc/tlg_notify.png
+-rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.1b3/doc/tmux.png
+-rw-r--r--   0        0        0     1968 2023-06-20 14:54:56.871877 martin-binance-1.3.1b3/martin_binance/__init__.py
+-rw-r--r--   0        0        0     4187 2023-06-20 15:14:30.461764 martin-binance-1.3.1b3/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2946 2023-06-10 10:09:47.513439 martin-binance-1.3.1b3/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:09:47.513439 martin-binance-1.3.1b3/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    14050 2023-06-19 19:16:08.304258 martin-binance-1.3.1b3/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6721 2023-06-19 17:47:04.745501 martin-binance-1.3.1b3/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6716 2023-06-19 17:47:04.745501 martin-binance-1.3.1b3/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6722 2023-06-19 17:47:04.745501 martin-binance-1.3.1b3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4707 2023-06-10 10:09:47.517442 martin-binance-1.3.1b3/martin_binance/client.py
+-rw-r--r--   0        0        0   185525 2023-06-20 10:20:51.033666 martin-binance-1.3.1b3/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.1b3/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.1b3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.1b3/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.1b3/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    85764 2023-06-19 21:29:05.366900 martin-binance-1.3.1b3/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.1b3/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.1b3/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.1b3/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16369 2023-06-19 17:47:04.749497 martin-binance-1.3.1b3/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-06-10 10:09:47.517442 martin-binance-1.3.1b3/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1274 2023-06-20 08:42:34.849378 martin-binance-1.3.1b3/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.1b3/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.1b3/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1360 2023-06-20 15:04:52.248056 martin-binance-1.3.1b3/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-06-19 19:16:08.288221 martin-binance-1.3.1b3/requirements.txt
+-rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.1b3/uml/architecture.puml
+-rw-r--r--   0        0        0     5151 1970-01-01 00:00:00.000000 martin-binance-1.3.1b3/PKG-INFO
```

### Comparing `martin-binance-1.3.1b2/.github/ISSUE_TEMPLATE/bug_report.md` & `martin-binance-1.3.1b3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/.github/ISSUE_TEMPLATE/feature_request.md` & `martin-binance-1.3.1b3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/.github/workflows/codeql.yml` & `martin-binance-1.3.1b3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/CHANGELOG.md` & `martin-binance-1.3.1b3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/Dockerfile` & `martin-binance-1.3.1b3/Dockerfile`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/LICENSE` & `martin-binance-1.3.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/README.md` & `martin-binance-1.3.1b3/README.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/doc/Create_strategy.png` & `martin-binance-1.3.1b3/doc/Create_strategy.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/doc/Model of logarithmic grid.ods` & `martin-binance-1.3.1b3/doc/Model of logarithmic grid.ods`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/doc/Modified martingale.svg` & `martin-binance-1.3.1b3/doc/Modified martingale.svg`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/doc/graf1.png` & `martin-binance-1.3.1b3/doc/graf1.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/doc/tlg_notify.png` & `martin-binance-1.3.1b3/doc/tlg_notify.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/doc/tmux.png` & `martin-binance-1.3.1b3/doc/tmux.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/__init__.py` & `martin-binance-1.3.1b3/martin_binance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.1b2"
+__version__ = "1.3.1b3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 #
 import platform
```

### Comparing `martin-binance-1.3.1b2/martin_binance/backtest/OoTSP.py` & `martin-binance-1.3.1b3/martin_binance/backtest/OoTSP.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,98 +2,103 @@
 # -*- coding: utf-8 -*-
 """
 Optimization of Trading Strategy Parameters
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0-2"
+__version__ = "1.3.0-3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 import importlib.util
 from decimal import Decimal
 import optuna
 import inquirer
 from inquirer.themes import GreenPassion
 from martin_binance import BACKTEST_PATH
 
-questions = [
-    inquirer.List(
-        "path",
-        message="Select from saved: exchange_PAIR with the strategy you want to optimize",
-        choices=[f.name for f in BACKTEST_PATH.iterdir() if f.is_dir() and f.name.count('_') == 1],
-    ),
-    inquirer.List(
-        "mode",
-        message="New study session or optimization history plot from saved one",
-        choices=["New", "Plot from saved"],
-    ),
-    inquirer.Text(
-        "n_trials",
-        message="Enter number of cycles, from 50 to 500",
-        ignore=lambda x: x["mode"] == "Plot from saved",
-        default='150',
-        validate=lambda _, c: 50 <= int(c) < 500,
-    ),
-]
 
-answers = inquirer.prompt(questions, theme=GreenPassion())
+PARAMS_FLOAT = ['PRICE_SHIFT', 'KBB']
 
-study_name = answers.get('path')  # Unique identifier of the study
-storage_name = f"sqlite:///{Path(BACKTEST_PATH, study_name, f'{study_name}.db')}"
+def try_trade(mbs, **kwargs):
+    for key, value in kwargs.items():
+        print(key, value)
+        setattr(mbs.ex, key, value if isinstance(value, int) or key in PARAMS_FLOAT else Decimal(f"{value}"))
+    mbs.ex.MODE = 'S'
+    mbs.ex.SAVE_DS = False
+    mbs.trade()
+    result = float(mbs.session_result.get('profit', 0)) + float(mbs.session_result.get('free', 0))
+    return result
 
-if answers.get('mode') == 'New':
-    Path(BACKTEST_PATH, study_name, f'{study_name}.db').unlink(missing_ok=True)
-    try:
-        strategy = next(Path(BACKTEST_PATH, answers.get('path')).glob("cli_*.py"))
-    except StopIteration:
-        raise UserWarning(f"Can't find cli_*.py in {Path(BACKTEST_PATH, answers.get('path'))}")
-    spec = importlib.util.spec_from_file_location("strategy", strategy)
-    mbs = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(mbs)
-
-    PARAMS_FLOAT = ['PRICE_SHIFT', 'KBB']
-
-    def try_trade(**kwargs):
-        for key, value in kwargs.items():
-            print(key, value)
-            setattr(mbs.ex, key, value if isinstance(value, int) or key in PARAMS_FLOAT else Decimal(f"{value}"))
-        mbs.ex.MODE = 'S'
-        mbs.ex.SAVE_DS = False
-        mbs.trade()
-        result = float(mbs.session_result.get('profit', 0)) + float(mbs.session_result.get('free', 0))
-        return result
 
+def main():
     def objective(trial):
         params = {
             'GRID_MAX_COUNT': trial.suggest_int('GRID_MAX_COUNT', 3, 5),
             'PRICE_SHIFT': trial.suggest_float('PRICE_SHIFT', 0, 0.05, step=0.01),
             'PROFIT': trial.suggest_float('PROFIT', 0.05, 0.15, step=0.05),
             'PROFIT_MAX': trial.suggest_float('PROFIT_MAX', 0.25, 1.0, step=0.05),
             'OVER_PRICE': trial.suggest_float('OVER_PRICE', 0.1, 1, step=0.1),
             'ORDER_Q': trial.suggest_int('ORDER_Q', 6, 12),
             'MARTIN': trial.suggest_float('MARTIN', 5, 15, step=1),
             'SHIFT_GRID_DELAY': trial.suggest_int('SHIFT_GRID_DELAY', 10, 60, step=10),
             'KBB': trial.suggest_float('KBB', 1, 5, step=0.5),
             'LINEAR_GRID_K': trial.suggest_int('LINEAR_GRID_K', 0, 100, step=20),
         }
-        return try_trade(**params)
+        return try_trade(mbs, **params)
 
-    study = optuna.create_study(study_name=study_name, storage=storage_name, direction="maximize")
-    study.optimize(objective, n_trials=int(answers.get('n_trials', '0')))
+    questions = [
+        inquirer.List(
+            "path",
+            message="Select from saved: exchange_PAIR with the strategy you want to optimize",
+            choices=[f.name for f in BACKTEST_PATH.iterdir() if f.is_dir() and f.name.count('_') == 1],
+        ),
+        inquirer.List(
+            "mode",
+            message="New study session or optimization history plot from saved one",
+            choices=["New", "Plot from saved"],
+        ),
+        inquirer.Text(
+            "n_trials",
+            message="Enter number of cycles, from 50 to 500",
+            ignore=lambda x: x["mode"] == "Plot from saved",
+            default='150',
+            validate=lambda _, c: 10 <= int(c) < 500,
+        ),
+    ]
+
+    answers = inquirer.prompt(questions, theme=GreenPassion())
+
+    study_name = answers.get('path')  # Unique identifier of the study
+    storage_name = f"sqlite:///{Path(BACKTEST_PATH, study_name, f'{study_name}.db')}"
+
+    if answers.get('mode') == 'New':
+        Path(BACKTEST_PATH, study_name, f'{study_name}.db').unlink(missing_ok=True)
+        try:
+            strategy = next(Path(BACKTEST_PATH, answers.get('path')).glob("cli_*.py"))
+        except StopIteration:
+            raise UserWarning(f"Can't find cli_*.py in {Path(BACKTEST_PATH, answers.get('path'))}")
+        spec = importlib.util.spec_from_file_location("strategy", strategy)
+        mbs = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(mbs)
+        study = optuna.create_study(study_name=study_name, storage=storage_name, direction="maximize")
+        study.optimize(objective, n_trials=int(answers.get('n_trials', '0')))
+        print(f"Optimal parameters: {study.best_params} for get {study.best_value}")
+        importance_params = optuna.importance.get_param_importances(study)
+        print("Evaluate parameter importance based on completed trials in the given study:")
+        for p in importance_params.items():
+            print(p)
+        print(f"Study instance saved to {storage_name} for later use")
+    else:
+        study = optuna.load_study(study_name=study_name, storage=storage_name)
+    #
+    try:
+        fig = optuna.visualization.plot_optimization_history(study)
+        fig.show()
+    except ImportError:
+        print("Can't find GUI, you can copy study instance to another environment for analyze it")
 
-    print(f"Optimal parameters: {study.best_params} for get {study.best_value}")
 
-    importance_params = optuna.importance.get_param_importances(study)
-    print("Evaluate parameter importance based on completed trials in the given study:")
-    for p in importance_params.items():
-        print(p)
-else:
-    study = optuna.load_study(study_name=study_name, storage=storage_name)
-
-try:
-    fig = optuna.visualization.plot_optimization_history(study)
-    fig.show()
-except ImportError:
-    print(f"Study instance saved to {storage_name} for later use")
+if __name__ == '__main__':
+    main()
```

### Comparing `martin-binance-1.3.1b2/martin_binance/backtest/VCoSEL.py` & `martin-binance-1.3.1b3/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/backtest/exchange_simulator.py` & `martin-binance-1.3.1b3/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/cli_0_BTCUSDT.py.template` & `martin-binance-1.3.1b3/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/cli_1_BTCUSDT.py.template` & `martin-binance-1.3.1b3/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin-binance-1.3.1b3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/client.py` & `martin-binance-1.3.1b3/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/executor.py` & `martin-binance-1.3.1b3/martin_binance/executor.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/funds_rate.db.template` & `martin-binance-1.3.1b3/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin-binance-1.3.1b3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/margin_wrapper.py` & `martin-binance-1.3.1b3/martin_binance/margin_wrapper.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/ms_cfg.toml.template` & `martin-binance-1.3.1b3/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/service/funds_rate_exporter.py` & `martin-binance-1.3.1b3/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/service/grafana.json` & `martin-binance-1.3.1b3/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/martin_binance/service/relaunch.py` & `martin-binance-1.3.1b3/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/pyproject.toml` & `martin-binance-1.3.1b3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -40,9 +40,10 @@
 
 [tool.flit.module]
 name = "martin_binance"
 
 [project.urls]
 Source = "https://github.com/DogsTailFarmer/martin-binance"
 
-[project.entry-points.init]
-console_scripts = "martin_binance.__init__:init"
+[project.scripts]
+martin-binance-init = "martin_binance.__init__:init"
+martin-binance-backtest = "martin_binance.backtest.OoTSP:main"
```

### Comparing `martin-binance-1.3.1b2/uml/architecture.puml` & `martin-binance-1.3.1b3/uml/architecture.puml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b2/PKG-INFO` & `martin-binance-1.3.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.3.1b2
+Version: 1.3.1b3
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 1.3.1b2 Summary: Free
+Metadata-Version: 2.1 Name: martin-binance Version: 1.3.1b3 Summary: Free
 trading system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
 Dist: exchanges-wrapper==1.3.0.post2 Requires-Dist: margin-strategy-sdk==0.0.11
```

