# Comparing `tmp/cemconvert-0.5.6.tar.gz` & `tmp/cemconvert-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cemconvert-0.5.6.tar", last modified: Wed Jun 21 14:13:28 2023, max compression
+gzip compressed data, was "dist/cemconvert-0.5.7.tar", last modified: Wed Jun 21 18:59:03 2023, max compression
```

## Comparing `cemconvert-0.5.6.tar` & `cemconvert-0.5.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      628 2023-06-21 14:13:02.000000 cemconvert-0.5.6/setup.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-21 14:13:28.000000 cemconvert-0.5.6/PKG-INFO
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/bin/
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     5195 2023-05-12 16:05:11.000000 cemconvert-0.5.6/bin/get_camd_cems
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3996 2023-02-08 15:41:07.000000 cemconvert-0.5.6/bin/cemconvert
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6349 2023-05-12 16:11:03.000000 cemconvert-0.5.6/bin/get_camd_cems_bulk
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)       38 2023-06-21 14:13:28.000000 cemconvert-0.5.6/setup.cfg
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2499 2023-06-20 16:44:51.000000 cemconvert-0.5.6/README.md
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2597 2023-05-17 15:23:53.000000 cemconvert-0.5.6/src/cemconvert/tz.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3821 2023-05-17 15:23:53.000000 cemconvert-0.5.6/src/cemconvert/temporal.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)    10736 2023-06-21 13:31:52.000000 cemconvert-0.5.6/src/cemconvert/ff10.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     1995 2023-05-17 15:23:53.000000 cemconvert-0.5.6/src/cemconvert/qa.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      283 2023-05-17 15:23:53.000000 cemconvert-0.5.6/src/cemconvert/__init__.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     7071 2023-05-22 20:25:07.000000 cemconvert-0.5.6/src/cemconvert/cemcorrect.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     5273 2023-05-17 15:23:53.000000 cemconvert-0.5.6/src/cemconvert/proc.py
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert/examples/
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)      307 2023-06-20 16:30:32.000000 cemconvert-0.5.6/src/cemconvert/examples/get_camd_cems.csh
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     1188 2023-06-16 19:57:48.000000 cemconvert-0.5.6/src/cemconvert/examples/cemconvert_2021.csh
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6781 2023-05-19 20:23:16.000000 cemconvert-0.5.6/src/cemconvert/cem.py
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert/data/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)    95049 2023-02-08 15:30:00.000000 cemconvert-0.5.6/src/cemconvert/data/county_fips_tz.csv
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     4818 2023-06-20 16:36:27.000000 cemconvert-0.5.6/src/cemconvert/run_parse.py
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      609 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/SOURCES.txt
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/PKG-INFO
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)        1 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/dependency_links.txt
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)       11 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/top_level.txt
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)       28 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/requires.txt
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 18:59:03.000000 cemconvert-0.5.7/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      628 2023-06-21 18:58:45.000000 cemconvert-0.5.7/setup.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-21 18:59:03.000000 cemconvert-0.5.7/PKG-INFO
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 18:59:03.000000 cemconvert-0.5.7/bin/
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     5195 2023-05-12 16:05:11.000000 cemconvert-0.5.7/bin/get_camd_cems
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3996 2023-02-08 15:41:07.000000 cemconvert-0.5.7/bin/cemconvert
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6349 2023-05-12 16:11:03.000000 cemconvert-0.5.7/bin/get_camd_cems_bulk
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       38 2023-06-21 18:59:03.000000 cemconvert-0.5.7/setup.cfg
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2499 2023-06-20 16:44:51.000000 cemconvert-0.5.7/README.md
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 18:59:03.000000 cemconvert-0.5.7/src/
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 18:59:03.000000 cemconvert-0.5.7/src/cemconvert/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2597 2023-05-17 15:23:53.000000 cemconvert-0.5.7/src/cemconvert/tz.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3821 2023-05-17 15:23:53.000000 cemconvert-0.5.7/src/cemconvert/temporal.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)    10736 2023-06-21 13:31:52.000000 cemconvert-0.5.7/src/cemconvert/ff10.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     1995 2023-05-17 15:23:53.000000 cemconvert-0.5.7/src/cemconvert/qa.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      283 2023-05-17 15:23:53.000000 cemconvert-0.5.7/src/cemconvert/__init__.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     7071 2023-05-22 20:25:07.000000 cemconvert-0.5.7/src/cemconvert/cemcorrect.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     5273 2023-05-17 15:23:53.000000 cemconvert-0.5.7/src/cemconvert/proc.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 18:59:03.000000 cemconvert-0.5.7/src/cemconvert/examples/
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)      307 2023-06-20 16:30:32.000000 cemconvert-0.5.7/src/cemconvert/examples/get_camd_cems.csh
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     1188 2023-06-16 19:57:48.000000 cemconvert-0.5.7/src/cemconvert/examples/cemconvert_2021.csh
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6844 2023-06-21 18:58:14.000000 cemconvert-0.5.7/src/cemconvert/cem.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 18:59:03.000000 cemconvert-0.5.7/src/cemconvert/data/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)    95049 2023-02-08 15:30:00.000000 cemconvert-0.5.7/src/cemconvert/data/county_fips_tz.csv
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     4818 2023-06-20 16:36:27.000000 cemconvert-0.5.7/src/cemconvert/run_parse.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 18:59:03.000000 cemconvert-0.5.7/src/cemconvert.egg-info/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      609 2023-06-21 18:59:02.000000 cemconvert-0.5.7/src/cemconvert.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-21 18:59:01.000000 cemconvert-0.5.7/src/cemconvert.egg-info/PKG-INFO
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)        1 2023-06-21 18:59:01.000000 cemconvert-0.5.7/src/cemconvert.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       11 2023-06-21 18:59:01.000000 cemconvert-0.5.7/src/cemconvert.egg-info/top_level.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       28 2023-06-21 18:59:01.000000 cemconvert-0.5.7/src/cemconvert.egg-info/requires.txt
```

### Comparing `cemconvert-0.5.6/setup.py` & `cemconvert-0.5.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages, Extension
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name="cemconvert",
-    version="0.5.6",
+    version="0.5.7",
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     python_requires='>=3.5',
     scripts=['bin/cemconvert','bin/get_camd_cems','bin/get_camd_cems_bulk'],
     setup_requires=['numpy>=1.19.5','pandas>=1.1.0'],
     install_requires=['numpy>=1.19.5','pandas>=1.1.0'],
     package_data={'cemconvert': ['examples/*.csh','data/*.csv']},
```

### Comparing `cemconvert-0.5.6/bin/get_camd_cems` & `cemconvert-0.5.7/bin/get_camd_cems`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/bin/cemconvert` & `cemconvert-0.5.7/bin/cemconvert`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/bin/get_camd_cems_bulk` & `cemconvert-0.5.7/bin/get_camd_cems_bulk`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/README.md` & `cemconvert-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/src/cemconvert/tz.py` & `cemconvert-0.5.7/src/cemconvert/tz.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/src/cemconvert/temporal.py` & `cemconvert-0.5.7/src/cemconvert/temporal.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/src/cemconvert/ff10.py` & `cemconvert-0.5.7/src/cemconvert/ff10.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/src/cemconvert/qa.py` & `cemconvert-0.5.7/src/cemconvert/qa.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/src/cemconvert/cemcorrect.py` & `cemconvert-0.5.7/src/cemconvert/cemcorrect.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/src/cemconvert/proc.py` & `cemconvert-0.5.7/src/cemconvert/proc.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/src/cemconvert/examples/cemconvert_2021.csh` & `cemconvert-0.5.7/src/cemconvert/examples/cemconvert_2021.csh`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/src/cemconvert/cem.py` & `cemconvert-0.5.7/src/cemconvert/cem.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.valcols = ['GLOAD','SLOAD','HTINPUT','SO2','CO2','NOX','OPTIME']#,'SO2MEAS','NOXMEAS','CO2MEAS']
         # Measurement names to integer codes
         self.measxref = {'Measured': 1, 'Calculated': 2, 'Substitute': 3,
           'Measured and Substitute': 4, 'LME': 5, 'Other': 6}
         # Old CEM columns
         self.oldcem = ['oris_facility_code','oris_boiler_id','date','hour','NOX','SO2','noxrate',
          'OPTIME','GLOAD','SLOAD','HTINPUT','htinputmeas','SO2MEAS','NOXMEAS','noxrmeasure','flow']
-        # List of months nmaes used in the CEMS monthly file
+        # List of months names used in the CEMS monthly file
         self.months = ('jan','feb','mar','apr','may','jun','jul','aug','sep','oct','nov','dec')
         # Initialize the dataframe to hold the hourly values for the period
         self.hourly = pd.DataFrame()
 
     def set_measure_codes(self, df):
         '''
         Set the measurement string to an integer for cemcorrect
@@ -62,14 +62,15 @@
         dtype = {'Facility ID': str, 'Unit ID': str, 'SO2 Mass Measure Indicator': str,
           'NOx Mass Measure Indicator': str, 'CO2 Mass Measure Indicator': str,
           'NOx Rate Measure Indicator': str, 'Heat Input Measure Indicator': str}
         df = pd.read_csv(fn, usecols=self.cemcols, dtype=dtype)
         # Rename columns to shorten names and fit formats
         df.rename(columns=self.colmap, inplace=True)
         df['date'] = pd.to_datetime(df.date + ' ' + df.hour.astype(str).str.zfill(2), format='%Y-%m-%d %H')
+        df['month'] = df.date.dt.month.astype(int).astype(str)
         df = self.set_measure_codes(df)
         dupes = df.duplicated(['oris_facility_code','oris_boiler_id','date','hour'], keep=False)
         if len(df[dupes]) > 0:
             raise ValueError('Duplicate ORIS/Date/Hour combinations found in CEMS')
         print('Records read: %s  NOX sum (lb): %s' %(len(df), sum(df['NOX'].fillna(0).round(6))))
         return df
```

### Comparing `cemconvert-0.5.6/src/cemconvert/data/county_fips_tz.csv` & `cemconvert-0.5.7/src/cemconvert/data/county_fips_tz.csv`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/src/cemconvert/run_parse.py` & `cemconvert-0.5.7/src/cemconvert/run_parse.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.6/src/cemconvert.egg-info/SOURCES.txt` & `cemconvert-0.5.7/src/cemconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

