# Comparing `tmp/wxdat-1.1.2.tar.gz` & `tmp/wxdat-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxdat-1.1.2.tar", max compression
+gzip compressed data, was "wxdat-1.2.0.tar", max compression
```

## Comparing `wxdat-1.1.2.tar` & `wxdat-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1071 2023-01-13 00:29:27.479547 wxdat-1.1.2/LICENSE
--rw-r--r--   0        0        0     2199 2023-02-02 03:36:47.988129 wxdat-1.1.2/README.md
--rw-r--r--   0        0        0      662 2023-03-19 15:11:46.511536 wxdat-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       33 2023-01-07 17:38:26.117864 wxdat-1.1.2/src/wxdat/__init__.py
--rw-r--r--   0        0        0     2260 2023-03-18 01:57:51.853658 wxdat-1.1.2/src/wxdat/__main__.py
--rw-r--r--   0        0        0     6398 2023-03-18 01:57:51.853658 wxdat-1.1.2/src/wxdat/config.py
--rw-r--r--   0        0        0     3640 2023-03-18 01:57:51.853658 wxdat-1.1.2/src/wxdat/database.py
--rw-r--r--   0        0        0     5515 2023-03-18 01:57:51.853658 wxdat-1.1.2/src/wxdat/metrics.py
--rw-r--r--   0        0        0     6502 2023-03-19 15:11:46.511536 wxdat-1.1.2/src/wxdat/providers/__init__.py
--rw-r--r--   0        0        0     4457 2023-01-18 06:11:54.826609 wxdat-1.1.2/src/wxdat/providers/accuweather.py
--rw-r--r--   0        0        0     3986 2023-01-18 06:11:54.826609 wxdat-1.1.2/src/wxdat/providers/ambientwx.py
--rw-r--r--   0        0        0     6663 2023-03-08 17:17:04.761626 wxdat-1.1.2/src/wxdat/providers/darksky.py
--rw-r--r--   0        0        0     4104 2023-01-18 06:11:54.826609 wxdat-1.1.2/src/wxdat/providers/noaa.py
--rw-r--r--   0        0        0     6862 2023-01-18 06:11:54.826609 wxdat-1.1.2/src/wxdat/providers/openweather.py
--rw-r--r--   0        0        0     3736 2023-01-18 06:11:54.826609 wxdat-1.1.2/src/wxdat/providers/wunderground.py
--rw-r--r--   0        0        0     3097 2023-01-21 19:51:10.218285 wxdat-1.1.2/src/wxdat/units/__init__.py
--rw-r--r--   0        0        0     3392 2023-01-13 00:29:27.479547 wxdat-1.1.2/src/wxdat/units/distance.py
--rw-r--r--   0        0        0     1931 2023-01-13 00:29:27.479547 wxdat-1.1.2/src/wxdat/units/pressure.py
--rw-r--r--   0        0        0     2798 2023-01-13 00:29:27.479547 wxdat-1.1.2/src/wxdat/units/quantity.py
--rw-r--r--   0        0        0     1209 2023-01-21 19:51:10.218285 wxdat-1.1.2/src/wxdat/units/rate.py
--rw-r--r--   0        0        0     1484 2023-01-13 00:29:27.479547 wxdat-1.1.2/src/wxdat/units/temperature.py
--rw-r--r--   0        0        0     2652 2023-01-13 00:29:27.479547 wxdat-1.1.2/src/wxdat/units/velocity.py
--rw-r--r--   0        0        0      936 2023-01-13 00:29:27.479547 wxdat-1.1.2/src/wxdat/units/volume.py
--rw-r--r--   0        0        0      881 2023-01-13 00:29:27.479547 wxdat-1.1.2/src/wxdat/units/weight.py
--rw-r--r--   0        0        0     1650 2023-03-18 01:57:51.877659 wxdat-1.1.2/src/wxdat/version.py
--rw-r--r--   0        0        0     3312 1970-01-01 00:00:00.000000 wxdat-1.1.2/setup.py
--rw-r--r--   0        0        0     2995 1970-01-01 00:00:00.000000 wxdat-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-10 14:02:30.444482 wxdat-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2199 2023-01-24 14:38:03.133133 wxdat-1.2.0/README.md
+-rw-r--r--   0        0        0      663 2023-06-21 03:13:56.848313 wxdat-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-01-07 17:38:11.743809 wxdat-1.2.0/src/wxdat/__init__.py
+-rw-r--r--   0        0        0     2260 2023-03-19 14:53:46.007655 wxdat-1.2.0/src/wxdat/__main__.py
+-rw-r--r--   0        0        0     6398 2023-03-19 14:53:46.008303 wxdat-1.2.0/src/wxdat/config.py
+-rw-r--r--   0        0        0     3683 2023-06-21 03:18:47.374073 wxdat-1.2.0/src/wxdat/database.py
+-rw-r--r--   0        0        0     5515 2023-03-19 14:53:46.009092 wxdat-1.2.0/src/wxdat/metrics.py
+-rw-r--r--   0        0        0     6504 2023-03-19 15:23:37.615963 wxdat-1.2.0/src/wxdat/providers/__init__.py
+-rw-r--r--   0        0        0     4457 2023-01-19 01:01:56.989878 wxdat-1.2.0/src/wxdat/providers/accuweather.py
+-rw-r--r--   0        0        0     4075 2023-06-21 03:18:47.374242 wxdat-1.2.0/src/wxdat/providers/ambientwx.py
+-rw-r--r--   0        0        0     6663 2023-02-14 14:12:56.230852 wxdat-1.2.0/src/wxdat/providers/darksky.py
+-rw-r--r--   0        0        0     4104 2023-01-19 01:01:56.991629 wxdat-1.2.0/src/wxdat/providers/noaa.py
+-rw-r--r--   0        0        0     6862 2023-01-19 01:01:56.991956 wxdat-1.2.0/src/wxdat/providers/openweather.py
+-rw-r--r--   0        0        0     3736 2023-01-19 01:01:56.992601 wxdat-1.2.0/src/wxdat/providers/wunderground.py
+-rw-r--r--   0        0        0     3097 2023-01-21 19:50:22.876646 wxdat-1.2.0/src/wxdat/units/__init__.py
+-rw-r--r--   0        0        0     3392 2023-01-13 00:50:28.105958 wxdat-1.2.0/src/wxdat/units/distance.py
+-rw-r--r--   0        0        0     1931 2023-01-13 00:50:28.106131 wxdat-1.2.0/src/wxdat/units/pressure.py
+-rw-r--r--   0        0        0     2798 2023-01-13 00:50:28.106343 wxdat-1.2.0/src/wxdat/units/quantity.py
+-rw-r--r--   0        0        0     1209 2023-01-21 19:50:22.876902 wxdat-1.2.0/src/wxdat/units/rate.py
+-rw-r--r--   0        0        0     1484 2023-01-13 00:50:28.106471 wxdat-1.2.0/src/wxdat/units/temperature.py
+-rw-r--r--   0        0        0     2652 2023-01-13 00:50:28.106680 wxdat-1.2.0/src/wxdat/units/velocity.py
+-rw-r--r--   0        0        0      936 2023-01-13 00:50:28.106805 wxdat-1.2.0/src/wxdat/units/volume.py
+-rw-r--r--   0        0        0      881 2023-01-13 00:50:28.107000 wxdat-1.2.0/src/wxdat/units/weight.py
+-rw-r--r--   0        0        0     1650 2023-03-19 14:53:46.010256 wxdat-1.2.0/src/wxdat/version.py
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 wxdat-1.2.0/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 wxdat-1.2.0/PKG-INFO
```

### Comparing `wxdat-1.1.2/LICENSE` & `wxdat-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/README.md` & `wxdat-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/pyproject.toml` & `wxdat-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "wxdat"
-version = "1.1.2"
+version = "1.2.0"
 description = "Weather data explorer."
 authors = ["jheddings <jheddings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-requests = "^2.28.2"
+requests = "^2.31.0"
 click = "^8.1.3"
 prometheus-client = "^0.16.0"
-pydantic = "^1.10.6"
-sqlalchemy = "^2.0.7"
-psycopg2 = "^2.9.5"
+pydantic = "^1.10.9"
+sqlalchemy = "^2.0.16"
+psycopg2 = "^2.9.6"
 ratelimit = "^2.2.1"
 pyyaml = "^6.0"
 gitpython = "^3.1.31"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.1.1"
-pytest = "^7.2.2"
+pre-commit = "^3.3.3"
+pytest = "^7.3.2"
 pytest-vcr = "^1.0.2"
-coverage = "^7.2.2"
+coverage = "^7.2.7"
 
 [tool.poetry.scripts]
 wxdat = "wxdat.__main__:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wxdat-1.1.2/src/wxdat/__main__.py` & `wxdat-1.2.0/src/wxdat/__main__.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/config.py` & `wxdat-1.2.0/src/wxdat/config.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/database.py` & `wxdat-1.2.0/src/wxdat/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     humidity = sql.Column(sql.Float())
 
     precip_hour = sql.Column(sql.Float())
     precip_day = sql.Column(sql.Float())
     precip_week = sql.Column(sql.Float())
     precip_month = sql.Column(sql.Float())
     precip_year = sql.Column(sql.Float())
+    precip_total = sql.Column(sql.Float())
 
     rel_pressure = sql.Column(sql.Float())
     abs_pressure = sql.Column(sql.Float())
 
     cloud_cover = sql.Column(sql.Float())
     visibility = sql.Column(sql.Float())
     uv_index = sql.Column(sql.Float())
```

### Comparing `wxdat-1.1.2/src/wxdat/metrics.py` & `wxdat-1.2.0/src/wxdat/metrics.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/providers/__init__.py` & `wxdat-1.2.0/src/wxdat/providers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     def record_current_conditions(self):
         """Record the current conditions from the internal station."""
 
         self.logger.info("Reading current condition -- %s", self.station.name)
         wx_data = self.station.current_conditions
 
         if wx_data is None:
-            self.logger.info(
+            self.logger.debug(
                 "Station '%s' did not provide current weather.",
                 self.station.name,
             )
             return False
 
         self.metrics(wx_data)
 
@@ -189,15 +189,15 @@
     def record_hourly_forecast(self):
         """Record the hourly forecast from the internal station."""
 
         self.logger.info("Reading hourly forecast -- %s", self.station.name)
         forecast = self.station.hourly_forecast
 
         if forecast is None:
-            self.logger.info(
+            self.logger.debug(
                 "Station '%s' did not provide an hourly forecast.",
                 self.station.name,
             )
             return False
 
         for hour in forecast:
             self.logger.debug("-- saving hourly forecast @ %s", hour.timestamp)
```

### Comparing `wxdat-1.1.2/src/wxdat/providers/accuweather.py` & `wxdat-1.2.0/src/wxdat/providers/accuweather.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/providers/ambientwx.py` & `wxdat-1.2.0/src/wxdat/providers/ambientwx.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
     hourlyrainin: Optional[float] = None
     dailyrainin: Optional[float] = None
     weeklyrainin: Optional[float] = None
     monthlyrainin: Optional[float] = None
     yearlyrainin: Optional[float] = None
     eventrainin: Optional[float] = None
+    totalrainin: Optional[float] = None
 
     uv: Optional[float] = None
 
     tempinf: Optional[float] = None
     humidityin: Optional[float] = None
     feelsLikein: Optional[float] = None
     dewPointin: Optional[float] = None
@@ -99,14 +100,15 @@
             humidity=conditions.humidity,
             dew_point=conditions.dewPoint,
             precip_hour=conditions.hourlyrainin,
             precip_day=conditions.dailyrainin,
             precip_week=conditions.weeklyrainin,
             precip_month=conditions.monthlyrainin,
             precip_year=conditions.yearlyrainin,
+            precip_total=conditions.totalrainin,
             rel_pressure=conditions.baromrelin,
             abs_pressure=conditions.baromabsin,
             solar_rad=conditions.solarradiation,
             uv_index=conditions.uv,
         )
 
     @property
```

### Comparing `wxdat-1.1.2/src/wxdat/providers/darksky.py` & `wxdat-1.2.0/src/wxdat/providers/darksky.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/providers/noaa.py` & `wxdat-1.2.0/src/wxdat/providers/noaa.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/providers/openweather.py` & `wxdat-1.2.0/src/wxdat/providers/openweather.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/providers/wunderground.py` & `wxdat-1.2.0/src/wxdat/providers/wunderground.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/units/__init__.py` & `wxdat-1.2.0/src/wxdat/units/__init__.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/units/distance.py` & `wxdat-1.2.0/src/wxdat/units/distance.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/units/pressure.py` & `wxdat-1.2.0/src/wxdat/units/pressure.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/units/quantity.py` & `wxdat-1.2.0/src/wxdat/units/quantity.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/units/rate.py` & `wxdat-1.2.0/src/wxdat/units/rate.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/units/temperature.py` & `wxdat-1.2.0/src/wxdat/units/temperature.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/units/velocity.py` & `wxdat-1.2.0/src/wxdat/units/velocity.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/units/volume.py` & `wxdat-1.2.0/src/wxdat/units/volume.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/units/weight.py` & `wxdat-1.2.0/src/wxdat/units/weight.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/src/wxdat/version.py` & `wxdat-1.2.0/src/wxdat/version.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.1.2/setup.py` & `wxdat-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'gitpython>=3.1.31,<4.0.0',
  'prometheus-client>=0.16.0,<0.17.0',
- 'psycopg2>=2.9.5,<3.0.0',
- 'pydantic>=1.10.6,<2.0.0',
+ 'psycopg2>=2.9.6,<3.0.0',
+ 'pydantic>=1.10.9,<2.0.0',
  'pyyaml>=6.0,<7.0',
  'ratelimit>=2.2.1,<3.0.0',
- 'requests>=2.28.2,<3.0.0',
- 'sqlalchemy>=2.0.7,<3.0.0']
+ 'requests>=2.31.0,<3.0.0',
+ 'sqlalchemy>=2.0.16,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['wxdat = wxdat.__main__:main']}
 
 setup_kwargs = {
     'name': 'wxdat',
-    'version': '1.1.2',
+    'version': '1.2.0',
     'description': 'Weather data explorer.',
     'long_description': "# wxdat #\n\n[![PyPI](https://img.shields.io/pypi/v/wxdat.svg)](https://pypi.org/project/wxdat)\n[![LICENSE](https://img.shields.io/github/license/jheddings/wxdat)](LICENSE)\n[![Style](https://img.shields.io/badge/style-black-black)](https://github.com/ambv/black)\n\nA general purpose weather data recorder & explorer.\n\n![dashboard](docs/images/dashboard.png)\n\nWhile the primary purpose of this library is to record weather data, it can also be\nused as a framework for collecting weather information in other apps.\n\n## Installation ##\n\nInstall the published package using pip:\n\n```shell\npip3 install wxdat\n```\n\nThis project uses `poetry` to manage dependencies and a local virtual environment.  To\nget started, clone the repository and install the dependencies with the following:\n\n```shell\npoetry install\n```\n\n## Usage ##\n\nRun the module and tell it which config file to use.\n\n```shell\npython3 -m wxdat --config wxdat.yaml\n```\n\nIf you are using `poetry` to manage the virtual environment, use the following:\n\n```shell\npoetry run python -m wxdat --config wxdat.yaml\n```\n\n## Configuration ##\n\nThe configuration file is a YAML document with a list of stations to export.  See the\nincluded default file for more details.\n\nAll stations have the following configuration values:\n* name - must be unique\n* type - the support station type\n\n## Supported Stations ##\n\nEventually, I'd like to add local stations, not just online sources.  Please see\nthe example configuration file for details on each provider.\n\n* AccuWeather\n* Ambient Weather Network\n* OpenWeatherMap\n* National Weather Service (NOAA)\n* Weather Underground\n\n## Unit Conversion ##\n\n`wxdat` also includes a limited set of conversion helpers for working with units.  In\ngeneral, the pattern for using them is:\n\n```python\nfrom wxdat import units\n\n# convert 100.0 from celsius to fahrenheit\ntemp = units.degC(100).degf\n```\n\n## Contributing ##\n\nTo submit a new issue, please visit the [Issues](https://github.com/jheddings/wxdat/issues)\npage.\n\nIf you are unsure where to start, create a post in the\n[Discussions](https://github.com/jheddings/wxdat/discussions) area.\n\nAdditionally, [Pull Requests](https://github.com/jheddings/wxdat/pulls) are welcome.\n",
     'author': 'jheddings',
     'author_email': 'jheddings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `wxdat-1.1.2/PKG-INFO` & `wxdat-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: wxdat
-Version: 1.1.2
+Version: 1.2.0
 Summary: Weather data explorer.
 License: MIT
 Author: jheddings
 Author-email: jheddings@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
-Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
-Requires-Dist: pydantic (>=1.10.6,<2.0.0)
+Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: sqlalchemy (>=2.0.7,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.16,<3.0.0)
 Description-Content-Type: text/markdown
 
 # wxdat #
 
 [![PyPI](https://img.shields.io/pypi/v/wxdat.svg)](https://pypi.org/project/wxdat)
 [![LICENSE](https://img.shields.io/github/license/jheddings/wxdat)](LICENSE)
 [![Style](https://img.shields.io/badge/style-black-black)](https://github.com/ambv/black)
```

