# Comparing `tmp/cemconvert-0.5.4.tar.gz` & `tmp/cemconvert-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cemconvert-0.5.4.tar", last modified: Tue Jun 20 17:21:59 2023, max compression
+gzip compressed data, was "dist/cemconvert-0.5.5.tar", last modified: Wed Jun 21 13:33:14 2023, max compression
```

## Comparing `cemconvert-0.5.4.tar` & `cemconvert-0.5.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-20 17:21:59.000000 cemconvert-0.5.4/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      671 2023-06-20 17:21:54.000000 cemconvert-0.5.4/setup.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-20 17:21:59.000000 cemconvert-0.5.4/PKG-INFO
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-20 17:21:59.000000 cemconvert-0.5.4/bin/
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     5195 2023-05-12 16:05:11.000000 cemconvert-0.5.4/bin/get_camd_cems
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3996 2023-02-08 15:41:07.000000 cemconvert-0.5.4/bin/cemconvert
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6349 2023-05-12 16:11:03.000000 cemconvert-0.5.4/bin/get_camd_cems_bulk
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2597 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/tz.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3821 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/temporal.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)    10129 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/ff10.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     1995 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/qa.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      283 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/__init__.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     7071 2023-05-22 20:25:07.000000 cemconvert-0.5.4/cemconvert/cemcorrect.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     5273 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/proc.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6781 2023-05-19 20:23:16.000000 cemconvert-0.5.4/cemconvert/cem.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     4818 2023-06-20 16:36:27.000000 cemconvert-0.5.4/cemconvert/run_parse.py
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-20 17:21:59.000000 cemconvert-0.5.4/examples/
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)      307 2023-06-20 16:30:32.000000 cemconvert-0.5.4/examples/get_camd_cems.csh
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     1188 2023-06-16 19:57:48.000000 cemconvert-0.5.4/examples/cemconvert_2021.csh
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)       38 2023-06-20 17:21:59.000000 cemconvert-0.5.4/setup.cfg
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2499 2023-06-20 16:44:51.000000 cemconvert-0.5.4/README.md
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      484 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/SOURCES.txt
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/PKG-INFO
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)        1 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/dependency_links.txt
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)       11 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/top_level.txt
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)       28 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/requires.txt
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 13:33:14.000000 cemconvert-0.5.5/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      671 2023-06-21 13:33:00.000000 cemconvert-0.5.5/setup.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-21 13:33:14.000000 cemconvert-0.5.5/PKG-INFO
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 13:33:14.000000 cemconvert-0.5.5/bin/
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     5195 2023-05-12 16:05:11.000000 cemconvert-0.5.5/bin/get_camd_cems
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3996 2023-02-08 15:41:07.000000 cemconvert-0.5.5/bin/cemconvert
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6349 2023-05-12 16:11:03.000000 cemconvert-0.5.5/bin/get_camd_cems_bulk
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 13:33:14.000000 cemconvert-0.5.5/cemconvert/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2597 2023-05-17 15:23:53.000000 cemconvert-0.5.5/cemconvert/tz.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3821 2023-05-17 15:23:53.000000 cemconvert-0.5.5/cemconvert/temporal.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)    10736 2023-06-21 13:31:52.000000 cemconvert-0.5.5/cemconvert/ff10.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     1995 2023-05-17 15:23:53.000000 cemconvert-0.5.5/cemconvert/qa.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      283 2023-05-17 15:23:53.000000 cemconvert-0.5.5/cemconvert/__init__.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     7071 2023-05-22 20:25:07.000000 cemconvert-0.5.5/cemconvert/cemcorrect.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     5273 2023-05-17 15:23:53.000000 cemconvert-0.5.5/cemconvert/proc.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6781 2023-05-19 20:23:16.000000 cemconvert-0.5.5/cemconvert/cem.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     4818 2023-06-20 16:36:27.000000 cemconvert-0.5.5/cemconvert/run_parse.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 13:33:14.000000 cemconvert-0.5.5/examples/
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)      307 2023-06-20 16:30:32.000000 cemconvert-0.5.5/examples/get_camd_cems.csh
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     1188 2023-06-16 19:57:48.000000 cemconvert-0.5.5/examples/cemconvert_2021.csh
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       38 2023-06-21 13:33:14.000000 cemconvert-0.5.5/setup.cfg
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2499 2023-06-20 16:44:51.000000 cemconvert-0.5.5/README.md
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 13:33:14.000000 cemconvert-0.5.5/cemconvert.egg-info/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      484 2023-06-21 13:33:13.000000 cemconvert-0.5.5/cemconvert.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-21 13:33:13.000000 cemconvert-0.5.5/cemconvert.egg-info/PKG-INFO
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)        1 2023-06-21 13:33:13.000000 cemconvert-0.5.5/cemconvert.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       11 2023-06-21 13:33:13.000000 cemconvert-0.5.5/cemconvert.egg-info/top_level.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       28 2023-06-21 13:33:13.000000 cemconvert-0.5.5/cemconvert.egg-info/requires.txt
```

### Comparing `cemconvert-0.5.4/setup.py` & `cemconvert-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages, Extension
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name="cemconvert",
-    version="0.5.4",
+    version="0.5.5",
     packages = find_packages(),
     python_requires='>=3.5',
     scripts=['bin/cemconvert','bin/get_camd_cems','bin/get_camd_cems_bulk'],
     setup_requires=['numpy>=1.19.5','pandas>=1.1.0'],
     install_requires=['numpy>=1.19.5','pandas>=1.1.0'],
     package_data={'cemconvert': ['examples/*.csh']},
     data_files=[('examples', ['examples/cemconvert_2021.csh','examples/get_camd_cems.csh'])],
```

### Comparing `cemconvert-0.5.4/bin/get_camd_cems` & `cemconvert-0.5.5/bin/get_camd_cems`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.4/bin/cemconvert` & `cemconvert-0.5.5/bin/cemconvert`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.4/bin/get_camd_cems_bulk` & `cemconvert-0.5.5/bin/get_camd_cems_bulk`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.4/cemconvert/tz.py` & `cemconvert-0.5.5/cemconvert/tz.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.4/cemconvert/temporal.py` & `cemconvert-0.5.5/cemconvert/temporal.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.4/cemconvert/ff10.py` & `cemconvert-0.5.5/cemconvert/ff10.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,42 +9,53 @@
     Class for FF10 and inventory related variables and processes
     '''
 
     def __init__(self, opts):
         # Variable name to use in the FF10 pollutant field for the temporalizer
         self.temporalvar = opts.temporalvar
         self.year = opts.year
+        # Annual FF10 columns in order
         self.ann_cols = ('country_cd','region_cd','tribal_code','facility_id','unit_id','rel_point_id',
           'process_id','agy_facility_id','agy_unit_id','agy_rel_point_id','agy_process_id','scc','poll','ann_value',
           'ann_pct_red','facility_name','erptype','stkhgt','stkdiam','stktemp','stkflow','stkvel','naics',
           'longitude','latitude','ll_datum','horiz_coll_mthd','design_capacity','design_capacity_units',
           'reg_codes','fac_source_type','unit_type_code','control_ids','control_measures','current_cost',
           'cumulative_cost','projection_factor','submitter_id','calc_method','data_set_id',
           'facil_category_code','oris_facility_code','oris_boiler_id','ipm_yn','calc_year','date_updated',
           'fug_height','fug_width_xdim','fug_length_ydim','fug_angle','zipcode','annual_avg_hours_per_year',
           'jan_value','feb_value','mar_value','apr_value','may_value','jun_value','jul_value','aug_value',
           'sep_value','oct_value','nov_value','dec_value','jan_pctred','feb_pctred','mar_pctred',
           'apr_pctred','may_pctred','jun_pctred','jul_pctred','aug_pctred','sep_pctred','oct_pctred',
           'nov_pctred','dec_pctred','comment')
+        # Data type for FF10 columns
         self.ff10_dtype = {'region_cd': str, 'tribal_code': str, 'facility_id': str, 'unit_id': str,
           'process_id': str, 'scc': str, 'poll': str, 'erptype': str, 'naics': str, 'll_datum': str,
           'fac_source_type': str, 'unit_type_code': str, 'submitter_id': str, 'data_set_id': str,
           'facil_category_code': str, 'oris_facility_code': str, 'oris_boiler_id': str, 'ipm_yn': str,
           'calc_year': str, 'date_updated': str, 'zipcode': str, 'comment': str, 'facility_name': str, 
           'agy_facility_id': str, 'agy_unit_id': str, 'agy_rel_point_id': str, 'agy_process_id': str,
           'reg_codes': str, 'control_ids': str, 'design_capacity_units': str, 'rel_point_id': str,
           'calc_method': str}
+        # 24 hour value column names
         self.hrvals = ['hrval%s' %hr for hr in range(24)]
+        # Hourly FF10 columns in order
         self.hourly_cols = ['country_cd','region_cd','tribal_code','facility_id','unit_id','rel_point_id',
           'process_id','scc','poll','op_type_cd','calc_method','date_updated','date','daytot'] + \
           self.hrvals + ['comment',]
+        # Monthly column names
         self.month_vals = ['jan_value','feb_value','mar_value','apr_value','may_value','jun_value',
           'jul_value','aug_value','sep_value','oct_value','nov_value','dec_value']
+        # Source identifier columns 
         self.id_cols = ['facility_id','unit_id','rel_point_id','process_id','oris_facility_code',
           'oris_boiler_id']
+        # Stack and source parameter columns
+        self.param_cols = ['scc','latitude','longitude','erptype','region_cd','facility_name',
+          'ipm_yn','country_cd','stkhgt','stkvel','stkflow','stktemp','stkdiam','naics',
+          'fac_source_type','fug_height','fug_width_xdim','fug_length_ydim','fug_angle',
+          'unit_type_code']
         self.ann_ff10 = pd.DataFrame()
         # FIPS by facility
         self.fips = pd.DataFrame()
         self.oris_fips = pd.DataFrame()
         # SCCs by unit/process
         self.sccs = pd.DataFrame()
         self.ann_head = []
@@ -105,35 +116,38 @@
         fn = os.path.join(opts.output_path, 'ptinv_%s_%s.csv' %(opts.year, opts.label))
         monthly = self.calc_monthly_vals(annual)
         annual = annual.groupby(self.id_cols+['poll',], as_index=False).sum()
         annual = annual.merge(monthly, on=self.id_cols+['poll',], how='left', suffixes=['_old',''])
         annual.rename(columns={'daytot': 'ann_value'}, inplace=True)
         # Fill FF10 fields for HOURACT values
         temp = annual[annual['poll'] == self.temporalvar].copy()
-        ann_cols = self.id_cols + ['scc','latitude','longitude','erptype','region_cd',
-          'facility_name','ipm_yn','country_cd']
+        ann_cols = self.id_cols + self.param_cols 
         temp = temp.merge(self.ann_ff10[ann_cols].drop_duplicates(self.id_cols), 
           on=self.id_cols, how='left')
         # Fill FF10 fields for non-HOURACT values
         annual = annual[annual['poll'] != self.temporalvar].merge(self.ann_ff10, 
           on=self.id_cols+['poll',], how='outer', suffixes=['_cem',''])
         annual = pd.concat((annual, temp))
         idx = annual['ann_value_cem'].notnull()
         annual.loc[idx, 'ann_value'] = annual.loc[idx, 'ann_value_cem']
         annual = annual.merge(monthly, on=self.id_cols+['poll',], how='left', suffixes=['_f',''])
+        # Fill in a single country
         country = str(annual['country_cd'].values[0])
+        # Round these fields
         round_cols = ['ann_value','latitude','longitude']
         annual[round_cols] = annual[round_cols].round(8)
         for col in self.ann_cols:
             if col not in list(annual.columns):
                 annual[col] = None
+        # Write the annual FF10 header
         with open(fn, 'w') as f:
             head = '#FORMAT=FF10_POINT\n#COUNTRY=%s\n#YEAR=%s\n' %(country, self.year)
             f.write(head)
             f.write('%s\n' %','.join(self.ann_cols))
+            # And data
             annual.to_csv(f, columns=self.ann_cols, index=False, quoting=csv.QUOTE_NONNUMERIC,
               header=False)
         fn = os.path.join(os.path.dirname(fn), 'qa_%s'  %os.path.basename(fn))
         write_annual_qa(fn, annual, self.ann_ff10, self.temporalvar)  
 
     def calc_monthly_vals(self, df):
         '''
```

### Comparing `cemconvert-0.5.4/cemconvert/qa.py` & `cemconvert-0.5.5/cemconvert/qa.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.4/cemconvert/cemcorrect.py` & `cemconvert-0.5.5/cemconvert/cemcorrect.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.4/cemconvert/proc.py` & `cemconvert-0.5.5/cemconvert/proc.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.4/cemconvert/cem.py` & `cemconvert-0.5.5/cemconvert/cem.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.4/cemconvert/run_parse.py` & `cemconvert-0.5.5/cemconvert/run_parse.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.4/examples/cemconvert_2021.csh` & `cemconvert-0.5.5/examples/cemconvert_2021.csh`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.4/README.md` & `cemconvert-0.5.5/README.md`

 * *Files identical despite different names*

