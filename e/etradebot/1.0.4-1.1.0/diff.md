# Comparing `tmp/etradebot-1.0.4.tar.gz` & `tmp/etradebot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etradebot-1.0.4.tar", last modified: Tue Apr 18 19:36:27 2023, max compression
+gzip compressed data, was "etradebot-1.1.0.tar", last modified: Wed Jun 21 01:28:11 2023, max compression
```

## Comparing `etradebot-1.0.4.tar` & `etradebot-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 19:36:27.034000 etradebot-1.0.4/
--rw-rw-rw-   0        0        0     1097 2023-03-20 03:24:40.000000 etradebot-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     4944 2023-04-18 19:36:26.656000 etradebot-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4398 2023-04-16 01:46:23.000000 etradebot-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.086000 etradebot-1.0.4/authentication/
--rw-rw-rw-   0        0        0       31 2023-02-19 07:12:36.000000 etradebot-1.0.4/authentication/__init__.py
--rw-rw-rw-   0        0        0     5885 2023-04-02 17:21:30.000000 etradebot-1.0.4/authentication/authentication.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.100000 etradebot-1.0.4/etrade/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.4/etrade/__init__.py
--rw-rw-rw-   0        0        0     9912 2023-04-02 17:36:50.000000 etradebot-1.0.4/etrade/etrade.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.559000 etradebot-1.0.4/etradebot.egg-info/
--rw-rw-rw-   0        0        0     4944 2023-04-18 19:36:25.000000 etradebot-1.0.4/etradebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      742 2023-04-18 19:36:25.000000 etradebot-1.0.4/etradebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       46 2023-04-18 19:36:25.000000 etradebot-1.0.4/etradebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      267 2023-04-18 19:36:25.000000 etradebot-1.0.4/etradebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       59 2023-04-18 19:36:25.000000 etradebot-1.0.4/etradebot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.568000 etradebot-1.0.4/execute/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.4/execute/__init__.py
--rw-rw-rw-   0        0        0    15723 2023-04-11 04:37:00.000000 etradebot-1.0.4/execute/execute.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.580000 etradebot-1.0.4/model/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.4/model/__init__.py
--rw-rw-rw-   0        0        0     3144 2023-03-29 05:54:46.000000 etradebot-1.0.4/model/investor_views.py
--rw-rw-rw-   0        0        0    30850 2023-04-12 05:02:10.000000 etradebot-1.0.4/model/model.py
--rw-rw-rw-   0        0        0       42 2023-04-18 19:36:27.032000 etradebot-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1375 2023-04-18 19:34:10.000000 etradebot-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.602000 etradebot-1.0.4/strategies/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.4/strategies/__init__.py
--rw-rw-rw-   0        0        0     3038 2023-04-18 19:12:36.000000 etradebot-1.0.4/strategies/cape_strategy.py
--rw-rw-rw-   0        0        0     3050 2023-03-18 21:04:05.000000 etradebot-1.0.4/strategies/example_strategy.py
--rw-rw-rw-   0        0        0     1397 2023-04-18 19:13:26.000000 etradebot-1.0.4/strategies/strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.631000 etradebot-1.0.4/tests/
--rw-rw-rw-   0        0        0        0 2023-02-19 06:56:31.000000 etradebot-1.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0    25834 2023-03-16 04:10:47.000000 etradebot-1.0.4/tests/mock_responses.py
--rw-rw-rw-   0        0        0     3857 2023-03-03 23:39:46.000000 etradebot-1.0.4/tests/test_authentication.py
--rw-rw-rw-   0        0        0     7079 2023-02-26 05:02:38.000000 etradebot-1.0.4/tests/test_etrade.py
--rw-rw-rw-   0        0        0     5658 2023-03-04 00:28:00.000000 etradebot-1.0.4/tests/test_execute.py
--rw-rw-rw-   0        0        0     7062 2023-03-16 04:10:47.000000 etradebot-1.0.4/tests/test_model.py
--rw-rw-rw-   0        0        0        0 2023-02-19 00:45:57.000000 etradebot-1.0.4/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.653000 etradebot-1.0.4/utils/
--rw-rw-rw-   0        0        0        0 2023-02-17 04:26:08.000000 etradebot-1.0.4/utils/__init__.py
--rw-rw-rw-   0        0        0     1126 2023-04-17 04:03:16.000000 etradebot-1.0.4/utils/credentials.py
--rw-rw-rw-   0        0        0     2185 2023-04-03 02:19:14.000000 etradebot-1.0.4/utils/fake_data.py
--rw-rw-rw-   0        0        0      989 2023-02-19 02:01:31.000000 etradebot-1.0.4/utils/logging_config.py
--rw-rw-rw-   0        0        0     3763 2023-02-20 04:32:22.000000 etradebot-1.0.4/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:28:11.102496 etradebot-1.1.0/
+-rw-rw-rw-   0        0        0     1097 2023-05-01 17:23:42.000000 etradebot-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0   247181 2023-05-15 17:13:49.000000 etradebot-1.1.0/LICENSE.chromedriver
+-rw-rw-rw-   0        0        0     4975 2023-06-21 01:28:11.100368 etradebot-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4393 2023-05-01 17:23:42.000000 etradebot-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 01:28:10.901995 etradebot-1.1.0/authentication/
+-rw-rw-rw-   0        0        0       31 2023-05-01 17:23:42.000000 etradebot-1.1.0/authentication/__init__.py
+-rw-rw-rw-   0        0        0     5885 2023-05-01 17:23:42.000000 etradebot-1.1.0/authentication/authentication.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:28:10.903292 etradebot-1.1.0/etrade/
+-rw-rw-rw-   0        0        0        0 2023-05-01 17:23:43.000000 etradebot-1.1.0/etrade/__init__.py
+-rw-rw-rw-   0        0        0    12657 2023-06-21 00:01:29.000000 etradebot-1.1.0/etrade/etrade.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:28:10.972971 etradebot-1.1.0/etradebot.egg-info/
+-rw-rw-rw-   0        0        0     4975 2023-06-21 01:28:09.000000 etradebot-1.1.0/etradebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-06-21 01:28:09.000000 etradebot-1.1.0/etradebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       46 2023-06-21 01:28:09.000000 etradebot-1.1.0/etradebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      267 2023-06-21 01:28:09.000000 etradebot-1.1.0/etradebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       59 2023-06-21 01:28:09.000000 etradebot-1.1.0/etradebot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 01:28:10.976958 etradebot-1.1.0/execute/
+-rw-rw-rw-   0        0        0        0 2023-05-01 17:23:43.000000 etradebot-1.1.0/execute/__init__.py
+-rw-rw-rw-   0        0        0    15723 2023-05-01 17:23:43.000000 etradebot-1.1.0/execute/execute.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:28:10.977954 etradebot-1.1.0/model/
+-rw-rw-rw-   0        0        0        0 2023-05-01 17:23:43.000000 etradebot-1.1.0/model/__init__.py
+-rw-rw-rw-   0        0        0     3144 2023-05-01 17:23:43.000000 etradebot-1.1.0/model/investor_views.py
+-rw-rw-rw-   0        0        0    30808 2023-06-20 22:15:33.000000 etradebot-1.1.0/model/model.py
+-rw-rw-rw-   0        0        0       42 2023-06-21 01:28:11.102496 etradebot-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1375 2023-06-21 01:18:43.000000 etradebot-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:28:11.025700 etradebot-1.1.0/strategies/
+-rw-rw-rw-   0        0        0        0 2023-05-01 17:23:43.000000 etradebot-1.1.0/strategies/__init__.py
+-rw-rw-rw-   0        0        0     3019 2023-06-20 22:20:00.000000 etradebot-1.1.0/strategies/cape_strategy.py
+-rw-rw-rw-   0        0        0     3050 2023-05-01 17:23:43.000000 etradebot-1.1.0/strategies/example_strategy.py
+-rw-rw-rw-   0        0        0     1397 2023-05-01 17:23:43.000000 etradebot-1.1.0/strategies/strategy.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:28:11.030684 etradebot-1.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-01 17:23:43.000000 etradebot-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    25834 2023-05-01 17:23:43.000000 etradebot-1.1.0/tests/mock_responses.py
+-rw-rw-rw-   0        0        0     3857 2023-05-01 17:23:43.000000 etradebot-1.1.0/tests/test_authentication.py
+-rw-rw-rw-   0        0        0     7079 2023-05-01 17:23:43.000000 etradebot-1.1.0/tests/test_etrade.py
+-rw-rw-rw-   0        0        0     5658 2023-05-01 17:23:43.000000 etradebot-1.1.0/tests/test_execute.py
+-rw-rw-rw-   0        0        0     7062 2023-05-01 17:23:43.000000 etradebot-1.1.0/tests/test_model.py
+-rw-rw-rw-   0        0        0        0 2023-05-01 17:23:43.000000 etradebot-1.1.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:28:11.100368 etradebot-1.1.0/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-01 17:23:43.000000 etradebot-1.1.0/utils/__init__.py
+-rw-rw-rw-   0        0        0     1126 2023-05-01 17:23:43.000000 etradebot-1.1.0/utils/credentials.py
+-rw-rw-rw-   0        0        0     2185 2023-05-01 17:23:43.000000 etradebot-1.1.0/utils/fake_data.py
+-rw-rw-rw-   0        0        0      989 2023-05-01 17:23:43.000000 etradebot-1.1.0/utils/logging_config.py
+-rw-rw-rw-   0        0        0     3763 2023-05-01 17:23:43.000000 etradebot-1.1.0/utils/portfolio.py
```

### Comparing `etradebot-1.0.4/LICENSE` & `etradebot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/PKG-INFO` & `etradebot-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: etradebot
-Version: 1.0.4
+Version: 1.1.0
 Summary: A Python-based trading bot for the E-Trade platform
 Home-page: https://github.com/nathanramoscfa/etradebot
 Author: Nathan Ramos, CFA®
 Author-email: info@nrcapitalmanagement.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE.chromedriver
 
 # ETradeBot
 
 ETradeBot is an automated trading software written in Python for E-Trade accounts that allows users to execute trades based on custom trading strategies. ETradeBot is strategy-agnostic and will execute any strategy given to it. This project is not affiliated with E-Trade or any other financial institution. By using ETradeBot, you agree to the [disclaimer](https://etradebot.readthedocs.io/en/latest/disclaimer.html).
 
 ## Features
 
@@ -27,15 +28,15 @@
 -   Manages portfolio: tracks positions, balance, and performance
 -   Trades: common stocks and ETFs
 
 ## Getting Started
 
 Refer to the [ETradeBot documentation](https://etradebot.readthedocs.io/en/latest/index.html) for instructions on installing, configuring, and using the software. 
 
-1. [Install](https://etradebot.readthedocs.io/en/latest/bloomberg.html) the Bloomberg SDK and C++ Build Tools.
+1. [Install](https://etradebot.readthedocs.io/en/latest/data.html) the Bloomberg SDK and C++ Build Tools.
 2. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
 3. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
 4. [Obtain](https://etradebot.readthedocs.io/en/latest/credentials.html) and securely store your E-Trade credentials.
 5. [Insert](https://etradebot.readthedocs.io/en/latest/strategies.html) your strategy into the strategies directory as a .py file.
 6. [Configure](https://etradebot.readthedocs.io/en/latest/batch.html) a batch file to run ETradeBot.
 7. [Run](https://etradebot.readthedocs.io/en/latest/running.html) ETradeBot in either preview or live trading mode.
 8. [Schedule](https://etradebot.readthedocs.io/en/latest/scheduling.html) ETradeBot to run automatically.
```

### Comparing `etradebot-1.0.4/README.md` & `etradebot-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 -   Manages portfolio: tracks positions, balance, and performance
 -   Trades: common stocks and ETFs
 
 ## Getting Started
 
 Refer to the [ETradeBot documentation](https://etradebot.readthedocs.io/en/latest/index.html) for instructions on installing, configuring, and using the software. 
 
-1. [Install](https://etradebot.readthedocs.io/en/latest/bloomberg.html) the Bloomberg SDK and C++ Build Tools.
+1. [Install](https://etradebot.readthedocs.io/en/latest/data.html) the Bloomberg SDK and C++ Build Tools.
 2. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
 3. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
 4. [Obtain](https://etradebot.readthedocs.io/en/latest/credentials.html) and securely store your E-Trade credentials.
 5. [Insert](https://etradebot.readthedocs.io/en/latest/strategies.html) your strategy into the strategies directory as a .py file.
 6. [Configure](https://etradebot.readthedocs.io/en/latest/batch.html) a batch file to run ETradeBot.
 7. [Run](https://etradebot.readthedocs.io/en/latest/running.html) ETradeBot in either preview or live trading mode.
 8. [Schedule](https://etradebot.readthedocs.io/en/latest/scheduling.html) ETradeBot to run automatically.
```

### Comparing `etradebot-1.0.4/authentication/authentication.py` & `etradebot-1.1.0/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/etrade/etrade.py` & `etradebot-1.1.0/etrade/etrade.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import xmltodict
 import pandas as pd
+import numpy as np
 from authentication.authentication import Authentication
 
 
 class ETrade:
     """
     :description: ETrade class
 
@@ -31,14 +32,15 @@
     :type browser: str, optional
     :param retries: Number of retries for failed requests, defaults to 3
     :type retries: int, optional
     :param sleep: Sleep time between retries, defaults to 30
     :type sleep: int, optional
     :EtradeRef: https://apisb.etrade.com/docs/api/authorization/request_token.html
     """
+
     def __init__(
             self, consumer_key, consumer_secret, web_username, web_password, account_id, etrade_cookie,
             sandbox_key=None, sandbox_secret=None, dev=True, headless=True, browser='chrome', retries=3, sleep=30
     ):
         self.auth = Authentication(
             consumer_key, consumer_secret, web_username, web_password, account_id, etrade_cookie,
             sandbox_key, sandbox_secret, dev, headless, browser, retries, sleep
@@ -227,16 +229,93 @@
         except xmltodict.expat.ExpatError:
             return pd.DataFrame()
 
         fields = ['symbolDescription', 'positionType', 'quantity', 'costPerShare', 'marketValue', 'totalCost',
                   'daysGain', 'daysGainPct', 'totalGain', 'totalGainPct', 'pctOfPortfolio']
         portfolio_data = pd.DataFrame(account_portfolio['PortfolioResponse']['AccountPortfolio']['Position'])[fields]
         portfolio_data = portfolio_data.apply(pd.to_numeric, errors='ignore')
-        numeric_cols = portfolio_data.columns[portfolio_data.dtypes != 'object']
-        numeric_cols = numeric_cols.drop('pctOfPortfolio')
-        portfolio_data[numeric_cols] = portfolio_data[numeric_cols].round(4)
-        portfolio_data[['daysGainPct', 'totalGainPct', 'pctOfPortfolio']] = portfolio_data[
-                                                                                   ['daysGainPct', 'totalGainPct',
-                                                                                    'pctOfPortfolio']] / 100
         portfolio_data = portfolio_data.sort_values(by=sort_by, ascending=ascending).set_index('symbolDescription')
 
         return portfolio_data
+
+    @staticmethod
+    def compute_portfolio_performance(portfolio_data):
+        """
+        :description: Compute portfolio performance
+
+        :param portfolio_data: Portfolio data
+        :type portfolio_data: pandas.DataFrame
+        :return: Portfolio performance
+        :rtype: pandas.Series
+        """
+        dollar_cols = ['marketValue', 'totalCost', 'daysGain', 'totalGain']
+        percent_cols = ['daysGainPct', 'totalGainPct']
+
+        # Remove dollar sign and convert to float
+        for col in dollar_cols:
+            portfolio_data[col] = portfolio_data[col].replace(r'[\$,]', '', regex=True).astype(float)
+
+        # Convert percentage strings to float numbers
+        portfolio_data[percent_cols] = portfolio_data[percent_cols].replace('%', '', regex=True).astype('float')
+
+        # Compute sum for dollar_cols
+        dollar_sum = portfolio_data[dollar_cols].sum()
+
+        # Compute the performance metrics as defined
+        portfolio_performance = dollar_sum.copy()
+        portfolio_performance['daysGainPct'] = dollar_sum['daysGain'] / (
+                    dollar_sum['totalCost'] - dollar_sum['daysGain'])
+        portfolio_performance['totalGainPct'] = dollar_sum['totalGain'] / dollar_sum['totalCost']
+
+        # Now convert to string format
+        portfolio_performance[dollar_cols] = portfolio_performance[dollar_cols].apply(lambda x: '${:,.2f}'.format(x))
+        for col in percent_cols:
+            if col in portfolio_performance:
+                portfolio_performance[col] = '{:.2f}%'.format(
+                    portfolio_performance[col] * 100)  # multiplying by 100 to convert ratio to percentage
+
+        return portfolio_performance
+
+    @staticmethod
+    def format_portfolio_data(portfolio_data):
+        """
+        :description: Format portfolio data
+
+        :param portfolio_data: Portfolio data
+        :type portfolio_data: pandas.DataFrame
+        :return: Formatted portfolio data
+        :rtype: pandas.DataFrame
+        """
+        # Copy the original dataframe to avoid altering it
+        formatted_portfolio = portfolio_data.copy()
+
+        # Define the columns to be formatted
+        dollar_cols = ['costPerShare', 'marketValue', 'totalCost', 'daysGain', 'totalGain']
+        percent_cols = ['daysGainPct', 'totalGainPct', 'pctOfPortfolio']
+
+        # Apply formatting
+        for col in dollar_cols:
+            formatted_portfolio[col] = formatted_portfolio[col].apply(
+                lambda x: '${:,.2f}'.format(x) if isinstance(x, float) else x)
+
+        for col in percent_cols:
+            formatted_portfolio[col] = formatted_portfolio[col].apply(
+                lambda x: '{:.2f}%'.format(x) if isinstance(x, float) else x)
+
+        return formatted_portfolio
+
+    @staticmethod
+    def get_current_portfolio(portfolio_data):
+        """
+        :description: Get current portfolio
+
+        :param portfolio_data: Portfolio data
+        :type portfolio_data: pandas.DataFrame
+        :return: Current portfolio
+        :rtype: pandas.DataFrame
+        """
+
+        current_portfolio = portfolio_data[[
+            'pctOfPortfolio', 'quantity', 'positionType'
+        ]]
+
+        return current_portfolio
```

### Comparing `etradebot-1.0.4/etradebot.egg-info/PKG-INFO` & `etradebot-1.1.0/etradebot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: etradebot
-Version: 1.0.4
+Version: 1.1.0
 Summary: A Python-based trading bot for the E-Trade platform
 Home-page: https://github.com/nathanramoscfa/etradebot
 Author: Nathan Ramos, CFA®
 Author-email: info@nrcapitalmanagement.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE.chromedriver
 
 # ETradeBot
 
 ETradeBot is an automated trading software written in Python for E-Trade accounts that allows users to execute trades based on custom trading strategies. ETradeBot is strategy-agnostic and will execute any strategy given to it. This project is not affiliated with E-Trade or any other financial institution. By using ETradeBot, you agree to the [disclaimer](https://etradebot.readthedocs.io/en/latest/disclaimer.html).
 
 ## Features
 
@@ -27,15 +28,15 @@
 -   Manages portfolio: tracks positions, balance, and performance
 -   Trades: common stocks and ETFs
 
 ## Getting Started
 
 Refer to the [ETradeBot documentation](https://etradebot.readthedocs.io/en/latest/index.html) for instructions on installing, configuring, and using the software. 
 
-1. [Install](https://etradebot.readthedocs.io/en/latest/bloomberg.html) the Bloomberg SDK and C++ Build Tools.
+1. [Install](https://etradebot.readthedocs.io/en/latest/data.html) the Bloomberg SDK and C++ Build Tools.
 2. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
 3. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
 4. [Obtain](https://etradebot.readthedocs.io/en/latest/credentials.html) and securely store your E-Trade credentials.
 5. [Insert](https://etradebot.readthedocs.io/en/latest/strategies.html) your strategy into the strategies directory as a .py file.
 6. [Configure](https://etradebot.readthedocs.io/en/latest/batch.html) a batch file to run ETradeBot.
 7. [Run](https://etradebot.readthedocs.io/en/latest/running.html) ETradeBot in either preview or live trading mode.
 8. [Schedule](https://etradebot.readthedocs.io/en/latest/scheduling.html) ETradeBot to run automatically.
```

### Comparing `etradebot-1.0.4/etradebot.egg-info/SOURCES.txt` & `etradebot-1.1.0/etradebot.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+LICENSE.chromedriver
 README.md
 setup.py
 authentication/__init__.py
 authentication/authentication.py
 etrade/__init__.py
 etrade/etrade.py
 etradebot.egg-info/PKG-INFO
```

### Comparing `etradebot-1.0.4/execute/execute.py` & `etradebot-1.1.0/execute/execute.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/model/investor_views.py` & `etradebot-1.1.0/model/investor_views.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/model/model.py` & `etradebot-1.1.0/model/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,17 +384,15 @@
         :param confidences: Confidences
         :type confidences: pandas.core.series.Series, required
         :param prints: Prints, default is False
         :type prints: bool, optional
         :return: posterior covariance matrix, posterior expected returns
         :rtype: tuple
         """
-        delta = self.market_implied_risk_aversion(market_prices, risk_free_rate)
-        print('Delta:')
-        print(round(delta, 2))
+        delta = self.market_implied_risk_aversion(market_prices, risk_free_rate, prints=prints)
 
         prior_returns = black_litterman.market_implied_prior_returns(
             market_caps.loc[symbols],
             delta,
             covariance_matrix,
             risk_free_rate
         )
```

### Comparing `etradebot-1.0.4/setup.py` & `etradebot-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='etradebot',
-    version='1.0.4',
+    version='1.1.0',
     url='https://github.com/nathanramoscfa/etradebot',
     license='MIT',
     author='Nathan Ramos, CFA®',
     author_email='info@nrcapitalmanagement.com',
     description='A Python-based trading bot for the E-Trade platform',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `etradebot-1.0.4/strategies/cape_strategy.py` & `etradebot-1.1.0/strategies/cape_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pandas as pd
 import model.investor_views as views
 from model.model import Model
 
 
-def get_nrcapital_forecast(filepath, min_long_return=0.15, max_short_return=0.0):
+def get_cape_forecast(filepath, min_long_return=0.15, max_short_return=0.0):
     """
     :description: Get equity ETF data and filter ETFs by expected return
 
-    :param filepath: Filepath to nrcapital forecasts
+    :param filepath: Filepath to cape forecasts
     :type filepath: str, required
     :param min_long_return: Minimum required long return, default is 0.15
     :type min_long_return: float, optional
     :param max_short_return: Maximum tolerable short return, default is 0.0
     :type max_short_return: float, optional
     :return: Selected equity ETFs
     :rtype: pd.DataFrame
@@ -29,16 +29,16 @@
 def strategy():
     """
     :description: Strategy to be run by the backtester
 
     :return: Portfolio weights
     :rtype: pd.Series
     """
-    etf_path = 'https://raw.githubusercontent.com/nathanramoscfa/nrcapital/main/data/etf_cape_return_forecast.csv'
-    selected_equity_etfs = get_nrcapital_forecast(etf_path)
+    etf_path = 'https://raw.githubusercontent.com/nathanramoscfa/cape/main/data/etf_cape_return_forecast.csv'
+    selected_equity_etfs = get_cape_forecast(etf_path)
     symbols = list(selected_equity_etfs.TICKER)
 
     model = Model(
         symbols,
         num_years=100,  # years
         bounds=(-0.3, 1.0),  # percent
         gamma=0.0,  # decimal
@@ -55,15 +55,15 @@
     risk_free_rate = model.get_risk_free_rate(prints=True)
     market_caps = model.get_market_caps(prints=True)
 
     vif_symbols = model.vif_filter(historical_prices, market_caps, threshold=50, prints=True)
     investor_views, confidences = views.investor_views_confidences(selected_equity_etfs, vif_symbols, prints=True)
 
     market_symbol, market_name, market_prices = model.get_market_prices(historical_prices, symbols, prints=True)
-    market_implied_risk_aversion = model.market_implied_risk_aversion(market_prices, risk_free_rate, prints=True)
+    market_implied_risk_aversion = model.market_implied_risk_aversion(market_prices, risk_free_rate, prints=False)
     covariance_matrix = model.calculate_covariance_matrix(historical_prices, symbols, prints=False)
     posterior_covariance_matrix, posterior_expected_returns = model.calculate_black_litterman(
         covariance_matrix,
         market_prices,
         risk_free_rate,
         market_caps,
         symbols,
```

### Comparing `etradebot-1.0.4/strategies/example_strategy.py` & `etradebot-1.1.0/strategies/example_strategy.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/strategies/strategy.py` & `etradebot-1.1.0/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/tests/mock_responses.py` & `etradebot-1.1.0/tests/mock_responses.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/tests/test_authentication.py` & `etradebot-1.1.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/tests/test_etrade.py` & `etradebot-1.1.0/tests/test_etrade.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/tests/test_execute.py` & `etradebot-1.1.0/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/tests/test_model.py` & `etradebot-1.1.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/utils/credentials.py` & `etradebot-1.1.0/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/utils/fake_data.py` & `etradebot-1.1.0/utils/fake_data.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/utils/logging_config.py` & `etradebot-1.1.0/utils/logging_config.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.4/utils/portfolio.py` & `etradebot-1.1.0/utils/portfolio.py`

 * *Files identical despite different names*

