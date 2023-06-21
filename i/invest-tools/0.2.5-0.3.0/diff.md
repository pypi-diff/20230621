# Comparing `tmp/invest_tools-0.2.5.tar.gz` & `tmp/invest_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest_tools-0.2.5.tar", max compression
+gzip compressed data, was "invest_tools-0.3.0.tar", max compression
```

## Comparing `invest_tools-0.2.5.tar` & `invest_tools-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-06-20 16:13:34.001514 invest_tools-0.2.5/LICENSE
--rw-r--r--   0        0        0     2748 2023-06-20 16:13:34.001514 invest_tools-0.2.5/README.md
--rw-r--r--   0        0        0      106 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/analysis.py
--rw-r--r--   0        0        0      198 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/currency.py
--rw-r--r--   0        0        0      572 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/log.py
--rw-r--r--   0        0        0     1102 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/plot.py
--rw-r--r--   0        0        0    10736 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/portfolio.py
--rw-r--r--   0        0        0     1887 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/validation.py
--rw-r--r--   0        0        0      682 2023-06-20 16:13:34.001514 invest_tools-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3614 1970-01-01 00:00:00.000000 invest_tools-0.2.5/setup.py
--rw-r--r--   0        0        0     3436 1970-01-01 00:00:00.000000 invest_tools-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-21 16:25:15.500255 invest_tools-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2229 2023-06-21 16:25:15.500255 invest_tools-0.3.0/README.md
+-rw-r--r--   0        0        0      106 2023-06-21 16:25:15.500255 invest_tools-0.3.0/invest_tools/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-21 16:25:15.500255 invest_tools-0.3.0/invest_tools/analysis.py
+-rw-r--r--   0        0        0      198 2023-06-21 16:25:15.500255 invest_tools-0.3.0/invest_tools/currency.py
+-rw-r--r--   0        0        0      572 2023-06-21 16:25:15.500255 invest_tools-0.3.0/invest_tools/log.py
+-rw-r--r--   0        0        0     1102 2023-06-21 16:25:15.500255 invest_tools-0.3.0/invest_tools/plot.py
+-rw-r--r--   0        0        0    10951 2023-06-21 16:25:15.500255 invest_tools-0.3.0/invest_tools/portfolio.py
+-rw-r--r--   0        0        0     1887 2023-06-21 16:25:15.500255 invest_tools-0.3.0/invest_tools/validation.py
+-rw-r--r--   0        0        0      682 2023-06-21 16:25:30.876430 invest_tools-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3080 1970-01-01 00:00:00.000000 invest_tools-0.3.0/setup.py
+-rw-r--r--   0        0        0     2917 1970-01-01 00:00:00.000000 invest_tools-0.3.0/PKG-INFO
```

### Comparing `invest_tools-0.2.5/LICENSE` & `invest_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invest_tools-0.2.5/README.md` & `invest_tools-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -67,30 +67,14 @@
 port.build()
 port.analyse()
 print(port.analysis)
 port.plot_correlation_heatmap()
 port.plot_returns_data()
 ```
 
-## Roadmap
-
-- [x] Add an input validator
-- [x] Add logging
-- [ ] Update risk free calculation to use new data outputs
-- [ ] Add deeper analysis methods
-    - [ ] Coppock Curve
-    - [ ] Fama French
-    - [ ] Excess Returns
-    - [ ] Maximum Drawdown
-    - [ ] Calculate Moments
-- [ ] Add further testing
-- [ ] Make the package more generic
-- [ ] Investigate using [Polars](https://www.pola.rs/)
-- [ ] Add func to calculate number of shares to buy to achieve portfolio make up (need to take in cash total for portfolio)
-
 ## License
 
 [MIT](LICENSE)
 
 ## Contact
 
-Just open an issue I guess?
+Just open an issue I guess?
```

### Comparing `invest_tools-0.2.5/invest_tools/analysis.py` & `invest_tools-0.3.0/invest_tools/analysis.py`

 * *Files identical despite different names*

### Comparing `invest_tools-0.2.5/invest_tools/log.py` & `invest_tools-0.3.0/invest_tools/log.py`

 * *Files identical despite different names*

### Comparing `invest_tools-0.2.5/invest_tools/plot.py` & `invest_tools-0.3.0/invest_tools/plot.py`

 * *Files identical despite different names*

### Comparing `invest_tools-0.2.5/invest_tools/portfolio.py` & `invest_tools-0.3.0/invest_tools/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing
+from datetime import datetime, timedelta
 
 import pandas as pd
 
 from invest_tools import analysis, currency, plot, validation
 from invest_tools.log import logger
 
 PRICES_DATATYPES = {
@@ -257,28 +258,33 @@
         self.percentage_returns = percentage_returns
 
         logger.info("Analysis loaded")
         return analysis_results
 
     def benchmark_analysis(self) -> pd.DataFrame:
         cumulative_returns = self.backtest[["portfolio_returns", "benchmark_returns"]]
+        cumulative_returns = cumulative_returns.loc[
+            datetime.now() - timedelta(days=365) : datetime.now()
+        ]
         cumulative_returns = cumulative_returns.assign(
             excess_returns=cumulative_returns.portfolio_returns
             - cumulative_returns.benchmark_returns
         )
         cumulative_returns = (
             1 + cumulative_returns[["portfolio_returns", "excess_returns"]]
         ).cumprod() - 1
         self.benchmark = cumulative_returns
         return cumulative_returns
 
     def plot_correlation_heatmap(self, save=False) -> None:
         if len(self.backtest) < 1:
             logger.warn("please run `.build()` before plotting")
-        stock_returns = self.backtest.drop("portfolio_returns", axis=1)
+        stock_returns = self.backtest.drop(
+            columns=["portfolio_returns", "benchmark_returns"]
+        )
         correlation_matrix = stock_returns.corr()
         logger.info("calculating portfolio correlation")
         plot.plot_heatmap(correlation_matrix, "Portfolio Correlation", save)
 
     def plot_returns_data(self, save=False) -> None:
         if len(self.backtest) < 1:
             logger.warn("please run `.build()` before plotting")
```

### Comparing `invest_tools-0.2.5/invest_tools/validation.py` & `invest_tools-0.3.0/invest_tools/validation.py`

 * *Files identical despite different names*

### Comparing `invest_tools-0.2.5/pyproject.toml` & `invest_tools-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "invest-tools"
-version = "0.2.5"
+version = "0.3.0"
 description = "Tools to manage portfolio risk analysis"
 authors = ["leo <leojpedwards@gmail.com>"]
 readme = "README.md"
 packages = [{include = "invest_tools"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `invest_tools-0.2.5/setup.py` & `invest_tools-0.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  'pandas>=1.5.3,<2.0.0',
  'scipy>=1.10.1,<2.0.0',
  'seaborn>=0.12.2,<0.13.0',
  'statsmodels>=0.13.5,<0.14.0']
 
 setup_kwargs = {
     'name': 'invest-tools',
-    'version': '0.2.5',
+    'version': '0.3.0',
     'description': 'Tools to manage portfolio risk analysis',
-    'long_description': '# invest-tools\n\n[![PyPI version](https://badge.fury.io/py/invest-tools.svg)](https://badge.fury.io/py/invest-tools)\n[![codecov](https://codecov.io/gh/leo-jp-edwards/invest-tools/graph/badge.svg?token=C1W8MZFS80)](https://codecov.io/gh/leo-jp-edwards/invest-tools)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**Tools to manage portfolio risk analysis**\n\n## Installation\n\nAs a python package this should be installable through:\n\n> `pip install invest-tools`\n\nOr:\n\n> `poetry add invest-tools`\n\n### Dependencies\n\nThe dependencies of this project can be seen in the `pyproject.toml` file. However for completeness there is a dependcy on `pandas`, `statsmodels` and `matplotlib` as the basics.\n\n## Data Inputs\n\nThere are three data inputs which should be present for the package to work as expected. \n\nThe path strings to the csvs can be passed in. \n\n1. Portfolio price data as a CSV\n\n| TIDM | Date | Open | High | Low | Close | Volume | Adjustment |\n|------|------|------|------|-----|-------|--------|------------|\n| EG | 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n| EG2 | 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n\n2. Currency data as a CSV\n\n| Date | Open | High | Low | Close | Adj Close | Volume |\n|------|------|------|-----|-------|-----------|--------|\n| 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n\n## Example\n\nBuild a portfolio of two securities called `EG` and `EG2` with the weighting split 50:50 between the two. One is denominated in GBP and one in USD.\n\nThis will output the mean returns of such a portfolio.\n\n```python\nimport numpy as np\nfrom invest_tools import portfolio\n\nportfolio_definition = {\n    "EG": {\n        "weight": 0.5,\n        "currency": "gbp"\n    },\n    "EG2": {\n        "weight": 0.5,\n        "currency": "usd"\n    }\n}\n\nport = portfolio.Portfolio(portfolio_definition, portfolio.Currency.GBP)\nport.get_usd_converter("path/to/csv")\nport.get_prices("path/to/csv")\nport.build()\nport.analyse()\nprint(port.analysis)\nport.plot_correlation_heatmap()\nport.plot_returns_data()\n```\n\n## Roadmap\n\n- [x] Add an input validator\n- [x] Add logging\n- [ ] Update risk free calculation to use new data outputs\n- [ ] Add deeper analysis methods\n    - [ ] Coppock Curve\n    - [ ] Fama French\n    - [ ] Excess Returns\n    - [ ] Maximum Drawdown\n    - [ ] Calculate Moments\n- [ ] Add further testing\n- [ ] Make the package more generic\n- [ ] Investigate using [Polars](https://www.pola.rs/)\n- [ ] Add func to calculate number of shares to buy to achieve portfolio make up (need to take in cash total for portfolio)\n\n## License\n\n[MIT](LICENSE)\n\n## Contact\n\nJust open an issue I guess?',
+    'long_description': '# invest-tools\n\n[![PyPI version](https://badge.fury.io/py/invest-tools.svg)](https://badge.fury.io/py/invest-tools)\n[![codecov](https://codecov.io/gh/leo-jp-edwards/invest-tools/graph/badge.svg?token=C1W8MZFS80)](https://codecov.io/gh/leo-jp-edwards/invest-tools)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**Tools to manage portfolio risk analysis**\n\n## Installation\n\nAs a python package this should be installable through:\n\n> `pip install invest-tools`\n\nOr:\n\n> `poetry add invest-tools`\n\n### Dependencies\n\nThe dependencies of this project can be seen in the `pyproject.toml` file. However for completeness there is a dependcy on `pandas`, `statsmodels` and `matplotlib` as the basics.\n\n## Data Inputs\n\nThere are three data inputs which should be present for the package to work as expected. \n\nThe path strings to the csvs can be passed in. \n\n1. Portfolio price data as a CSV\n\n| TIDM | Date | Open | High | Low | Close | Volume | Adjustment |\n|------|------|------|------|-----|-------|--------|------------|\n| EG | 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n| EG2 | 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n\n2. Currency data as a CSV\n\n| Date | Open | High | Low | Close | Adj Close | Volume |\n|------|------|------|-----|-------|-----------|--------|\n| 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n\n## Example\n\nBuild a portfolio of two securities called `EG` and `EG2` with the weighting split 50:50 between the two. One is denominated in GBP and one in USD.\n\nThis will output the mean returns of such a portfolio.\n\n```python\nimport numpy as np\nfrom invest_tools import portfolio\n\nportfolio_definition = {\n    "EG": {\n        "weight": 0.5,\n        "currency": "gbp"\n    },\n    "EG2": {\n        "weight": 0.5,\n        "currency": "usd"\n    }\n}\n\nport = portfolio.Portfolio(portfolio_definition, portfolio.Currency.GBP)\nport.get_usd_converter("path/to/csv")\nport.get_prices("path/to/csv")\nport.build()\nport.analyse()\nprint(port.analysis)\nport.plot_correlation_heatmap()\nport.plot_returns_data()\n```\n\n## License\n\n[MIT](LICENSE)\n\n## Contact\n\nJust open an issue I guess?\n',
     'author': 'leo',
     'author_email': 'leojpedwards@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `invest_tools-0.2.5/PKG-INFO` & `invest_tools-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-tools
-Version: 0.2.5
+Version: 0.3.0
 Summary: Tools to manage portfolio risk analysis
 License: MIT
 Author: leo
 Author-email: leojpedwards@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -87,30 +87,15 @@
 port.build()
 port.analyse()
 print(port.analysis)
 port.plot_correlation_heatmap()
 port.plot_returns_data()
 ```
 
-## Roadmap
-
-- [x] Add an input validator
-- [x] Add logging
-- [ ] Update risk free calculation to use new data outputs
-- [ ] Add deeper analysis methods
-    - [ ] Coppock Curve
-    - [ ] Fama French
-    - [ ] Excess Returns
-    - [ ] Maximum Drawdown
-    - [ ] Calculate Moments
-- [ ] Add further testing
-- [ ] Make the package more generic
-- [ ] Investigate using [Polars](https://www.pola.rs/)
-- [ ] Add func to calculate number of shares to buy to achieve portfolio make up (need to take in cash total for portfolio)
-
 ## License
 
 [MIT](LICENSE)
 
 ## Contact
 
 Just open an issue I guess?
+
```

