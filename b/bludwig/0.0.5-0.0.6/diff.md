# Comparing `tmp/bludwig-0.0.5.tar.gz` & `tmp/bludwig-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bludwig-0.0.5.tar", last modified: Sat Jun 17 19:40:01 2023, max compression
+gzip compressed data, was "bludwig-0.0.6.tar", last modified: Wed Jun 21 20:19:28 2023, max compression
```

## Comparing `bludwig-0.0.5.tar` & `bludwig-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 19:40:01.219388 bludwig-0.0.5/
--rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 bludwig-0.0.5/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)      488 2023-06-17 19:40:01.219388 bludwig-0.0.5/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)       58 2023-06-17 19:38:54.000000 bludwig-0.0.5/README.md
--rw-r--r--   0 me        (1000) me        (1000)     1124 2023-06-17 19:38:03.000000 bludwig-0.0.5/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-17 19:40:01.219388 bludwig-0.0.5/setup.cfg
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 19:40:01.199388 bludwig-0.0.5/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 19:40:01.219388 bludwig-0.0.5/src/bludwig/
--rw-r--r--   0 me        (1000) me        (1000)    13727 2023-06-13 20:10:46.000000 bludwig-0.0.5/src/bludwig/LudwigJob.py
--rw-r--r--   0 me        (1000) me        (1000)       82 2023-06-11 18:48:52.000000 bludwig-0.0.5/src/bludwig/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      197 2023-06-10 09:59:04.000000 bludwig-0.0.5/src/bludwig/__main__.py
--rw-r--r--   0 me        (1000) me        (1000)    16867 2023-06-17 14:54:42.000000 bludwig-0.0.5/src/bludwig/helper.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 19:40:01.219388 bludwig-0.0.5/src/bludwig.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)      488 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      339 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       50 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) me        (1000)       17 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-21 20:19:28.138395 bludwig-0.0.6/
+-rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 bludwig-0.0.6/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)      488 2023-06-21 20:19:28.138395 bludwig-0.0.6/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)       58 2023-06-21 20:18:49.000000 bludwig-0.0.6/README.md
+-rw-r--r--   0 me        (1000) me        (1000)     1124 2023-06-21 20:18:39.000000 bludwig-0.0.6/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-21 20:19:28.138395 bludwig-0.0.6/setup.cfg
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-21 20:19:28.138395 bludwig-0.0.6/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-21 20:19:28.138395 bludwig-0.0.6/src/bludwig/
+-rw-r--r--   0 me        (1000) me        (1000)    13529 2023-06-20 20:34:16.000000 bludwig-0.0.6/src/bludwig/LudwigJob.py
+-rw-r--r--   0 me        (1000) me        (1000)       82 2023-06-11 18:48:52.000000 bludwig-0.0.6/src/bludwig/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)      197 2023-06-10 09:59:04.000000 bludwig-0.0.6/src/bludwig/__main__.py
+-rw-r--r--   0 me        (1000) me        (1000)    17565 2023-06-21 20:01:16.000000 bludwig-0.0.6/src/bludwig/helper.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-21 20:19:28.138395 bludwig-0.0.6/src/bludwig.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)      488 2023-06-21 20:19:28.000000 bludwig-0.0.6/src/bludwig.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)      339 2023-06-21 20:19:28.000000 bludwig-0.0.6/src/bludwig.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2023-06-21 20:19:28.000000 bludwig-0.0.6/src/bludwig.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)       50 2023-06-21 20:19:28.000000 bludwig-0.0.6/src/bludwig.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) me        (1000)       17 2023-06-21 20:19:28.000000 bludwig-0.0.6/src/bludwig.egg-info/requires.txt
+-rw-r--r--   0 me        (1000) me        (1000)        8 2023-06-21 20:19:28.000000 bludwig-0.0.6/src/bludwig.egg-info/top_level.txt
```

### Comparing `bludwig-0.0.5/LICENSE` & `bludwig-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bludwig-0.0.5/pyproject.toml` & `bludwig-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pyproject.toml
 
 
 [project]
 name            = "bludwig"
-version         = "0.0.5"        
+version         = "0.0.6"        
 
 requires-python = ">=3.9"
 dependencies    = ['pandasklar','munch']
 
 authors        = [{ name = "djekra", email = "hopsalla@gmail.com" }]
 description     = "Some helper for Ludwig AI"
 readme          = "README.md"
```

### Comparing `bludwig-0.0.5/src/bludwig/LudwigJob.py` & `bludwig-0.0.6/src/bludwig/LudwigJob.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         LudwigJob wird einmal instanziiert, z.B. so:
         ludwig_job = bludwig.LudwigJob( configs=configs, verbose=True) 
         * configs: list of Ludwig-configs as YAML-String, Path to yaml-file or yaml-object
             
         '''
         # Parameter         
         if experiment_name is None:
-            experiment_name = 'ex'
+            experiment_name = 'model'
         self.experiment_name = experiment_name
         self.verbose = verbose        
 
         # configs ggf. in YAML wandeln
         self.configs = []
         for config in configs:
             if isinstance(config, str):
@@ -71,15 +71,16 @@
 
         # job
         self.train_jobs = []
         self.model_names = []
         self.model_paths = []
 
         # train_log
-        self.train_log_raw = pd.DataFrame()
+        self.train_log = pd.DataFrame()
+
 
         # results
         self.train_stats      = []
         self.test_stats       = []
         self.output_dirs      = []       
 
         if len(configs) > 0:
@@ -99,22 +100,25 @@
         model_no:            {self.model_no}   
         cuda:                {self.cuda}             
         '''
         return result
 
 
     
-    def load_from_results(self):    
+    def load_from_results(self, experiment_name=None):    
         '''
         Loads data from results directory
+        * experiment_name: Only load results from this experiment. Otherwise all.
         '''
-        results_dir = os.listdir('results')
+        results_dir = sorted(os.listdir('results'))
+        if experiment_name is not None:
+            results_dir = [rd for rd in results_dir if rd.startswith(experiment_name)]
         self.output_dirs = [ 'results/' + d                for d in results_dir ]
-        self.train_jobs  = [ int(d.split('_')[1])          for d in results_dir ]
-        self.model_names = [ 'model_' + str(j)             for j in self.train_jobs ]    
+        self.train_jobs  = [ int(d.split('_')[-2])         for d in results_dir ]
+        self.model_names = [ self.experiment_name + '_' + str(j)             for j in self.train_jobs ]    
         self.model_paths = [d + '/model'                   for d in self.output_dirs]
         
         train_stats = [ d + '/training_statistics.json'    for d in self.output_dirs ]
         train_stats = [ json.load( open(p) )               for p in train_stats]
         self.train_stats = [ DefaultMunch.fromDict(d)      for d in train_stats]
 
         test_stats = [ d + '/test_statistics.json'         for d in self.output_dirs ]
@@ -180,74 +184,87 @@
 
             
         
 #####################################################################################################
 # experiment
 #
     
-    def experiment(self, train_jobs, dataset):
+    def experiment(self, dataset, train_jobs=None, count_runs=[0] ):
         '''
         train and evaluate a list of Ludwig models
         '''
+        
+        # counts calls of this function
+        count_runs[0]+=1  
+        
+        if train_jobs is None:
+            train_jobs = [ no for (no, _) in enumerate(self.configs)]        
         self.train_jobs = train_jobs
-        self.model_names = ['model_' + str(c) for c in train_jobs]
+        self.model_names = [self.experiment_name + '_' + str(config_no) for config_no in train_jobs]
         
         
         for config_no in train_jobs:
-            experiment_subname = self.experiment_name + '_' + str(config_no) 
-            experiment_path = 'results/' + experiment_subname + '_run'  
+            self.model_name          = self.model_names[config_no]
+            self.model_no            = config_no
+            
+            experiment_path = 'results/' + self.model_name + '_run'  
             print()
-            print( 'Training config_no {} >> {}'.format( config_no, experiment_path) )   
+            print( 'Training model {}'.format(self.model_name) )   
             
             # Zielverzeichnis rekursiv löschen
             try:
                 shutil.rmtree(experiment_path)
             except:
                 pass
 
             logging_level = 20 if self.verbose else 30
 
             # lade model
             self.model               = LudwigModel(config=self.configs[config_no], logging_level=logging_level)   
-            self.model_no            = config_no
+
+            
             self.cuda                = torch.cuda.is_available()
             self.output_feature_name = self.model.config['output_features'][0]['name']
             self.output_feature_type = self.model.config['output_features'][0]['type']
 
             # trainiere
             start_time = time.time()     
-            test_stat, train_stat, _, output_dir = self.model.experiment( dataset=dataset, experiment_name=experiment_subname)
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")            
+                test_stat, train_stat, _, output_dir = self.model.experiment( dataset=dataset, experiment_name=self.model_name)
             self.test_stats  += [test_stat]
             self.train_stats += [train_stat]
             self.output_dirs += [output_dir]
             self.model_paths += [output_dir + '/model']
 
             # logge config
             train_secs        = round( time.time() - start_time )
             train_time        = bpy.human_readable_seconds( train_secs )
             epochs            = len(train_stat.test['combined']['loss']) 
             validation_metric = self.model.config['trainer']['validation_metric']
             log = pak.dataframe([
-                [ config_no, 'train_secs',          train_secs        ],
-                [ config_no, 'train_time',          train_time        ],
-                [ config_no, 'epochs',              epochs            ],
-                [ config_no, 'time/epoch',          bpy.human_readable_seconds( train_secs/epochs ) ],     
-                [ config_no, 'validation_metric',   validation_metric ],     
-                [ config_no, 'experiment_path',     experiment_path   ], 
-                [ config_no, 'output_feature_name', self.output_feature_name   ],    
-                [ config_no, 'output_feature_type', self.output_feature_type   ],                    
+                [ count_runs[0], self.model_name, 'experiment_name',     self.experiment_name   ],                
+                [ count_runs[0], self.model_name, 'train_secs',          train_secs        ],
+                [ count_runs[0], self.model_name, 'train_time',          train_time        ],
+                [ count_runs[0], self.model_name, 'epochs',              epochs            ],
+                [ count_runs[0], self.model_name, 'time/epoch',          bpy.human_readable_seconds( train_secs/epochs ) ],     
+                [ count_runs[0], self.model_name, 'validation_metric',   validation_metric ],     
+                [ count_runs[0], self.model_name, 'experiment_path',     experiment_path   ], 
+                [ count_runs[0], self.model_name, 'output_feature_name', self.output_feature_name   ],    
+                [ count_runs[0], self.model_name, 'output_feature_type', self.output_feature_type   ],                    
                 
             ])
-            log.columns = ['config_no','name','value']
-            self.train_log_raw = pak.add_rows( self.train_log_raw, log ) 
+            log.columns = ['run','model_name','name','value']
+            log2 = analyse_test_stat( count_runs[0], self.model_name, test_stat)
+            self.train_log = pak.add_rows( self.train_log, log  )             
+            self.train_log = pak.add_rows( self.train_log, log2 ) 
+            
             print('train_time:',train_time) 
             print()
-
-        # logge Gesamtprozess
-        self.train_log_raw = pak.add_rows( self.train_log_raw, entwirre_test_stat(self.test_stats))            
+       
 
 
 
         
 #####################################################################################################
 # predict
 #
@@ -260,54 +277,16 @@
         pred.index = data.index
         result = pd.merge( data, pred, left_index=True, right_index=True)
         result = pak.move_cols( result, [self.output_feature_name, self.output_feature_name + '_predictions'])
         result.rename(columns=lambda x: x.replace('_predictions', '_pred').replace('probabilities', 'prob').replace('probability', 'prob'), inplace=True)
         return result        
 
 
-        
-#####################################################################################################
-# train_log
-#
-
-    def train_log(self):
-        ''' returns small log'''
-        if self.train_log_raw.shape[0] > 0:
-            result = prepare_train_log(self.train_log_raw, size='small')
-            return result
-        else:
-            zeilen = ['roc_auc','accuracy','recall','specificity','precision','loss','epochs','time/epoch','train_time']
-            result = pd.DataFrame(zeilen)
-            result.columns = ['name']
-            return result
-
-    
-    
-    def train_log_big(self):
-        ''' returns bigger log'''
-        return prepare_train_log(self.train_log_raw, size='big')        
 
 
-        
-    def train_log_to_csv(self):
-        '''
-        Saves train_log_big to csv file
-        Shows train_log (small version)
-        '''
-        t = self.train_log_big()
-        if self.in_colab:
-            t.to_csv('train_log_colab.csv', index=False)
-        else:
-            if torch.cuda.is_available():
-                t.to_csv('train_log_GPU.csv', index=False)    
-            else:
-                t.to_csv('train_log_CPU.csv', index=False)
-                
-        return self.train_log()
-
 
         
         
 #####################################################################################################
 # Visualisierungen
 #
 
@@ -315,19 +294,22 @@
 
         # Kein bestimmer output_feature_name angefragt >> Default
         if output_feature_name is None:
             output_feature_name = self.output_feature_name
         
         # test_stats_small (verhindert Fehler)
         test_stats_small = []
-        keys_to_keep = list(self.train_log().name)
+        try:
+            keys_to_keep = set(self.train_log.name)
+        except:
+            keys_to_keep = {'accuracy','accuracy_micro','roc_auc','loss'}
         for stat in self.test_stats:
             r = {key: value  for key, value in stat[output_feature_name].items()  if key in keys_to_keep}
             r = { output_feature_name: r }    
-            test_stats_small += [r]        
+            test_stats_small += [r]    
 
         # ausgeben
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             compare_performance( test_stats_small, model_names=self.model_names, output_feature_name=output_feature_name )
```

### Comparing `bludwig-0.0.5/src/bludwig/helper.py` & `bludwig-0.0.6/src/bludwig/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import importlib, yaml, pkg_resources, os, warnings
+import importlib, yaml, pkg_resources, os, warnings, re, requests
 import torch 
 import bpyth as bpy
 import pandas as pd
 import pandasklar as pak
 
     
 #############################################################################################################
@@ -22,118 +22,49 @@
         print('max_memory_reserved:  {}'.format(bpy.human_readable_bytes(torch.cuda.max_memory_reserved( device=device)) )  )  
 
     else:
         print('no CUDA!')    
 
 
 
-def entwirre_test_stat(test_stats):
+#def entwirre_test_stat(test_stats):
+#    result = []
+#    for config_no, test_stat in enumerate(test_stats):
+#        print(config_no)
+#        for output_feature_name, stat in test_stat.items():
+#            if output_feature_name == 'combined':
+#                continue
+#            for key, value in stat.items():
+#                if isinstance(value, (int, float)):
+#                    result += [[config_no, key, bpy.human_readable_number(value,3) ]]    
+#                    
+#    result = pak.dataframe(result)
+#    result.columns = ['config_no','name','value']
+#    return result
+#
+
+
+def analyse_test_stat(run, model_name, test_stat):
     result = []
-    for config_no, test_stat in enumerate(test_stats):
-        print(config_no)
-        for output_feature_name, stat in test_stat.items():
-            if output_feature_name == 'combined':
-                continue
-            for key, value in stat.items():
-                if isinstance(value, (int, float)):
-                    result += [[config_no, key, bpy.human_readable_number(value,3) ]]    
+    for output_feature_name, stat in test_stat.items():
+        if output_feature_name == 'combined':
+            continue
+        for key, value in stat.items():
+            if isinstance(value, (int, float)):
+                result += [[run, model_name, key, bpy.human_readable_number(value,3) ]]    
                     
     result = pak.dataframe(result)
-    result.columns = ['config_no','name','value']
-    return result
-
-
-
-
-def prepare_train_log(train_log_raw, size='small'):
-
-    result = pd.pivot_table( train_log_raw, 
-                              index='name',
-                              columns='config_no',
-                              values='value', 
-                              aggfunc='first')
-    result = pak.drop_multiindex(result).reset_index() 
-    
-    # Namen korrigieren
-    mask = result.name.str.startswith('average')
-    result.loc[mask,'name'] = result[mask].name.str.replace('average_','') + '_avg'   
-
-    # validation_metric ganz nach vorne
-    mask = result.name == 'validation_metric'
-    zeilen_ganzvorne = list(set(result[mask].iloc[0]))    
-    #print(zeilen_ganzvorne)
-
-
-    # Zeilen sortieren
-    if size == 'small':
-        zeilen_vorne =  ['accuracy','recall','specificity','precision','roc_auc','loss',]
-        zeilen_hinten = ['epochs','time/epoch','train_time',]    
-        result = result.set_index('name').T
-        result = pak.move_cols( result, zeilen_vorne )
-        result = pak.move_cols( result, zeilen_ganzvorne )        
-        result = pak.move_cols( result, zeilen_hinten, -1 )    
-        result = result.T.reset_index()
-
-        # Zeilen löschen
-        zeilen_verboten = ['validation_metric']
-        zeilen_erlaubt = [z for z in (zeilen_ganzvorne + zeilen_vorne + zeilen_hinten) if not z in zeilen_verboten ]
-        mask = result.name.isin( zeilen_erlaubt )
-        result = result[mask]
-        
-    else: # size == 'big'
-        result = result.sort_values('name')
-        zeilen_vorne =  ['validation_metric',]
-        zeilen_hinten = ['experiment_path','output_feature_type','output_feature_name','epochs','train_secs','time/epoch','train_time',]     
-        result = result.set_index('name').T
-        result = pak.move_cols( result, zeilen_vorne )         
-        result = pak.move_cols( result, zeilen_hinten, -1 )    
-        result = result.T.reset_index()        
-
-    result = pak.reset_index(result)
-    result.columns = [c if isinstance(c,str) else 'model_' + str(c) for c in result.columns ]
+    result.columns = ['run','model_name','name','value']
     return result
 
 
 
-def list_datasets():
 
-    datasets = [
-#                                                       
-#        dataset_name                    input_field_types   output_field_type    
-#                                    size                                  note
-        ['adult_census_income',      4,  'category, number', 'binary',     'many category fields'], 
-        ['agnews',                   5,  'text',             'category',   ''   ],
-        ['amazon_review_polarity',   6,  'text',             'binary',     '',  ],
-        ['amazon_reviews',           6,  'text',             'category',   '',  ],
-        ['dbpedia',                  5,  'text',             'category',   '',  ],
-        ['electricity',              4,  'number',           'number',     '',  ],
-        ['ethos_binary',             2,  'text',             'binary',     '',  ],
-        ['flickr8k',                 3,  'image',            'text',       '',  ],
-        ['goemotions',               4,  'text',             'category',   '',  ],
-        ['irony',                    3,  'text',             'binary',     '',  ],
-        ['mnist',                    4,  'image',            'category',   'Hello world',  ],
-        ['mushroom_edibility',       3,  'category',         'binary',     '',  ],
-        ['poker_hand',               6,  'category',         'category',   '',  ],
-        ['sarcos',                   4,  'number',           'number',     '',  ],
-        ['sst2',                     3,  'text',             'binary',     '',  ],
-        ['sst3',                     4,  'text',             'category',   '',  ],        
-        ['sst4',                     4,  'text',             'category',   '',  ],       
-        ['yahoo_answers',            6,  'text',             'category',   '',  ],
-        ['yelp_review_polarity',     5,  'text',             'binary',     '',  ],
-        ['yelp_reviews',             5,  'text',             'category',   '',  ],
-        ['yosemite',                 4,  'time',             'number',     '',  ],
-        ['ae_price_prediction',      4,  'category',         'number',     '',  ],     
-        ['bookprice_prediction',     3,  'text,category',    'number',     '',  ],    
 
 
-        
-        ]
-    result = pak.dataframe(datasets)
-    result.columns = ['dataset_name','size','input_field_types','output_field_type','note',]
-    return result
 
 
 
 def load_dataset(dataset_name, verbose=True):
     '''
     Loads a dataset from Ludwig's dataset zoo. 
     * dataset_name: Name of the dataset. Valid names are listed by list_datasets().
@@ -143,17 +74,20 @@
     dataset_loader = getattr(module, dataset_name)
     data_df       = dataset_loader.load(split=False)
         
     #katalog = list_datasets()
     #mask = katalog.dataset_name == dataset_name
     #katalogeintrag = katalog[mask].iloc[0]
 
-    output_feature_names = [col['name'] for col in dataset_loader.config.output_features]   
+    # nacharbeiten
     if dataset_name == 'agnews':
-        output_feature_names = ['class']
+        dataset_loader.config.output_features = [{'name': 'class', 'type': 'category'}]
+        data_df = pak.drop_cols( data_df,'class_index' )
+    
+    output_feature_names = [col['name'] for col in dataset_loader.config.output_features]   
     data_df = pak.move_cols(data_df, output_feature_names)     
     data_df = pak.move_cols(data_df, 'split',-1) 
     data_df = pak.drop_cols(data_df,['Unnamed: 0','Unnamed: 1'])
     data_df = pak.change_datatype(data_df)
 
     if verbose:
         print()
@@ -213,27 +147,39 @@
     analyse.loc[mask,'feature_type'] = 'category'    
 
     # numeric feature_type
     mask1 = analyse['datatype_identified'].isin(['int','float'])
     mask2 = analyse.feature_type == ''
     mask = mask1 & mask2
     analyse.loc[mask,'feature_type'] = 'number'
-
+    
+    # vector feature_type
+    try:
+        pattern = r'^\s*(\d+(\.\d+)?\s*)+$'
+        mask1 = analyse['datatype_identified'].isin(['string'])
+        mask2 = analyse['vmin'].str.match(pattern)
+        mask3 = analyse['vmax'].str.match(pattern)
+        mask4 = analyse.feature_type == ''
+        mask = mask1  &  mask2  &  mask3  &  mask4
+        analyse.loc[mask,'feature_type'] = 'vector'
+    except:
+        pass
+    
     # text feature_type
     mask1 = analyse['datatype_identified'].isin(['string'])
     mask2 = analyse.feature_type == ''
     mask = mask1 & mask2
     analyse.loc[mask,'feature_type'] = 'text'
 
-    
     # image feature_type  
     try:
         mask1 = analyse['feature_type'] == 'text'
         mask2 = analyse['vmin'].str.endswith(('jpg','png'))
-        mask = mask1 & mask2
+        mask3 = analyse['vmin'].str.endswith(('jpg','png'))        
+        mask = mask1  &  mask2  &  mask3
         analyse.loc[mask,'feature_type'] = 'image'
     except:
         pass
 
     # date feature_type  
     mask1 = analyse['datatype_identified'].isin(['datetime'])
     mask2 = analyse.feature_type == ''
@@ -301,139 +247,240 @@
     if use_yaml:
         result = yaml.dump(result)
         result = result.replace( 'null\n...\n', '' )
         
     return result    
 
 
-
-def get_datasets(remove_failed=True):
+def configs(data_df, dataset_loader=None, output_features_size=1, use_yaml=True):
     '''
-    List all datasets available in Ludwig.
+    List of config0, config1
     '''
-    library_location = pkg_resources.get_distribution('ludwig').location
-    directory_within_library = 'ludwig/datasets/configs'
-    directory_path = os.path.join(library_location, directory_within_library)
-    file_list = os.listdir(directory_path)
-    
-    elements_to_remove = ['__pycache__','__init__.py']
-    result = [x.replace('.yaml','') for x in file_list if x not in elements_to_remove]
-    result = sorted(result)
+    c0 = config0(data_df, dataset_loader=dataset_loader, output_features_size=output_features_size, use_yaml=use_yaml)
+    if dataset_loader is not None:
+        c1 = config1(dataset_loader,use_yaml=use_yaml)
+    if dataset_loader is None or c1 is None or c1 == '':
+        return [c0]
+    else:
+        return [c0,c1]
 
-    if not remove_failed:
-        return result
 
-    failed =    ['allstate_claims_severity',
-                 'amazon_employee_access_challenge',
-                 'ames_housing',
-                 'bbcnews',
-                 'bnp_claims_management',
-                 'connect4',
-                 'creditcard_fraud',
-                 'customer_churn_prediction',
-                 'higgs',
-                 'ieee_fraud',
-                 'imbalanced_insurance',
-                 'imdb',
-                 'insurance_lite',
-                 'jigsaw_unintended_bias100k',
-                 'mercedes_benz_greener',
-                 'noshow_appointments',
-                 'numerai28pt6',
-                 'ohsumed_7400',
-                 'otto_group_product',
-                 'porto_seguro_safe_driver',
-                 'reuters_r8',
-                 'rossman_store_sales',
-                 'santander_customer_satisfaction',
-                 'santander_customer_transaction',
-                 'santander_value_prediction',
-                 'sarcastic_headlines',
-                 'synthetic_fraud',
-                 'talkingdata_adtrack_fraud',
-                 'telco_customer_churn',
-                 'temperature',
-                 'titanic',
-                 'twitter_bots',
-                 'walmart_recruiting',
-                 'wmt15',
-                 'fever',
-                 'forest_cover',
-                 'google_quest_qa',
-                 'imdb_genre_prediction',
-                 'kdd_appetency',
-                 'kdd_churn',
-                 'kdd_upselling']    
 
-    result = [x for x in result if x not in failed]
-    return result
+#def list_datasets():
+#    '''
+#    List all datasets available in Ludwig.
+#    '''
+#    def get_filelist(use_github=False):
+#        if use_github:
+#            repository_url = 'https://api.github.com/repos/ludwig-ai/ludwig/contents/ludwig/datasets/configs'
+#            response = requests.get(repository_url)
+#            directory_contents = response.json()
+#            file_list = [item['name'] for item in directory_contents]  
+#            return file_list
+#        else:
+#            library_location = pkg_resources.get_distribution('ludwig').location
+#            directory_within_library = 'ludwig/datasets/configs'
+#            directory_path = os.path.join(library_location, directory_within_library)
+#            file_list = os.listdir(directory_path)       
+#            return file_list            
+#    try:
+#        file_list = get_filelist(use_github=False)
+#    except:
+#        file_list = get_filelist(use_github=True)  
+#        print('using github')
+#    elements_to_remove = ['__pycache__','__init__.py']
+#    result = [x.replace('.yaml','') for x in file_list if x not in elements_to_remove]
+#    result = sorted(result)
+#
+#    return result
+
 
 
 
 
 
-def scan_datasets(dataset_names, get_elements_to_remove=False):
+
+def scan_datasets( dataset_names, use_cache=False ):
     '''
     Scan and analyse Ludwig's database zoo. 
     '''
+    pickle_filename = 'scan_datasets.temp.pickle'
+    if use_cache:
+        try:
+            return pak.load_pickle(pickle_filename)   
+        except:
+            print('cache error')
+            return scan_datasets( dataset_names, use_cache=False )
+        
     result = []
+    
     for dataset in dataset_names:
         
         # load_dataset
         print('loading',dataset)
         try:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")            
                 data_df, dataset_loader = load_dataset(dataset, verbose=False)  
-        except:
-            elements_to_remove += [dataset]
-
-        # analysieren 
-        analyse = analyse_cols(data_df, dataset_loader) 
-        mask = analyse.is_output_feature
-        output_features_size = analyse[mask].shape[0]        
-
-        # output_features and input_features 
-        spalten = ['col_name','feature_type','mem_usage']
-        output_features = analyse[:output_features_size][spalten]           
-        input_features = analyse[output_features_size:][spalten]        
-
-        # Ausgabewerte berechnen
-        input_features_type  = ', '.join(pak.group_and_agg( input_features,  ['feature_type','mem_usage'], ['','sum']).sort_values('mem_usage_sum', ascending=False).feature_type)
-        output_features_type = ', '.join(pak.group_and_agg( output_features, ['feature_type','mem_usage'], ['','sum']).sort_values('mem_usage_sum', ascending=False).feature_type)        
-        config1 = yaml.dump(dataset_loader.default_model_config)
-        config1 = config1.replace('null\n...\n','')
-
-        # Ausgabe
-        result += [{'dataset_name': dataset, 
-                    'rows': bpy.human_readable_number(data_df.shape[0]) ,
-                    'in_size'  : input_features.shape[0],                        
-                    'out_size' : output_features.shape[0],
-
-                    'in_name'  : ', '.join(input_features.col_name),                    
-                    'out_name' : ', '.join(output_features.col_name),                    
-
-                    'in_type'  : input_features_type,  # ', '.join(input_features.feature_type),                      
-                    'out_type' : output_features_type, # ', '.join(output_features.feature_type),                    
-                                 
-                    'description': dataset_loader.description(),
-                    'config1': config1(dataset_loader),
 
-                   }]
+            # analysieren 
+            analyse = analyse_cols(data_df, dataset_loader) 
+            mask = analyse.is_output_feature
+            output_features_size = analyse[mask].shape[0]        
     
+            # output_features and input_features 
+            spalten = ['col_name','feature_type','mem_usage']
+            output_features = analyse[:output_features_size][spalten]           
+            input_features = analyse[output_features_size:][spalten]        
+    
+            # Ausgabewerte berechnen
+            input_features_type  = ', '.join(pak.group_and_agg( input_features,  ['feature_type','mem_usage'], ['','sum']).sort_values('mem_usage_sum', ascending=False).feature_type)
+            output_features_type = ', '.join(pak.group_and_agg( output_features, ['feature_type','mem_usage'], ['','sum']).sort_values('mem_usage_sum', ascending=False).feature_type)        
+    
+            # Ausgabe
+            result += [{'dataset_name': dataset, 
+                        'status'      : 'ok',
+                        'rows'        : bpy.human_readable_number(data_df.shape[0]) ,
+                        'in_size'     : input_features.shape[0],                        
+                        'out_size'    : output_features.shape[0],
+       
+                        'in_name'     : ', '.join(input_features.col_name),                    
+                        'out_name'    : ', '.join(output_features.col_name),                    
+       
+                        'in_type'     : input_features_type,  # ', '.join(input_features.feature_type),                      
+                        'out_type'    : output_features_type, # ', '.join(output_features.feature_type),                    
+                                     
+                        'description' : dataset_loader.description(),
+                        'config1'     : config1(dataset_loader),
+    
+                       }]
 
+        except:
+            result += [{'dataset_name': dataset, 
+                        'status'      : 'Error load',
+                        'rows'        : 0 ,
+                        'in_size'     : 0,                        
+                        'out_size'    : 0,
+       
+                        'in_name'     : '',                    
+                        'out_name'    : '',                    
+       
+                        'in_type'     : '',                       
+                        'out_type'    : '',                    
+                                     
+                        'description' : '',  
+                        'config1'     : '',  
+    
+                       }]
+    
     result = pak.dataframe(result) 
 
-    if get_elements_to_remove:
-        return result, elements_to_remove
+    if not use_cache:
+        pak.dump_pickle(result,pickle_filename)
     return result
 
 
 
+        
+#####################################################################################################
+# train_log
+#
+
+
+def train_log(train_log_raw, T=False):
+    ''' returns small log'''
+    if train_log_raw.shape[0] > 0:
+        result = prepare_train_log(train_log_raw, size='small')
+    else:
+        zeilen = ['validation_metric','loss','roc_auc','accuracy','recall','specificity','precision','epochs','time/epoch','train_time']
+        result = pd.DataFrame(zeilen)
+        result.columns = ['name']
+    if not T:
+        return result
+        
+    result = result.set_index('name')
+    result = result.T.reset_index()
+    result = pak.rename_col(result,'index','model')
+    return result
+
+
+
+def train_log_big(train_log_raw):
+    ''' returns bigger log'''
+    return prepare_train_log(train_log_raw, size='big')        
+
+
+    
+def train_log_to_csv(train_log_raw):
+    '''
+    Saves train_log_big to csv file
+    Saves train_log_raw to csv file
+    Shows train_log (small version)
+    '''
+    t0 = train_log_raw
+    t1 = train_log_big(train_log_raw)
+    t2 = train_log(train_log_raw)
+    
+    t0.to_csv( 'train_log_raw.csv', index=False) 
+    t1.to_csv( 'train_log_big.csv', index=False)  
+    t2.to_csv( 'train_log.csv',     index=False)       
+    return t2
+
+
+
+def prepare_train_log(train_log_raw, size='small'):
+
+    # target_value ergänzen
+    mask = train_log_raw.name == 'validation_metric'  
+    validation_metrics = train_log_raw[mask]
+    
+    mask = pak.isin(train_log_raw, validation_metrics, left_on=['model_name','name'], right_on=['model_name','value'])
+    df = train_log_raw[mask].copy()
+    df['name'] = 'target_value'
+    train_log_raw = pak.add_rows(train_log_raw, df, only_new=['model_name','name','value'])
+    
+    result = pd.pivot_table( train_log_raw, 
+                              index='name',
+                              columns='model_name',
+                              values='value', 
+                              aggfunc='last')
+    result = pak.drop_multiindex(result).reset_index() 
+    
+    # Namen korrigieren
+    mask = result.name.str.startswith('average')
+    result.loc[mask,'name'] = result[mask].name.str.replace('average_','') + '_avg'   
+
+
+    # Zeilen sortieren
+    if size == 'small':
+        zeilen_vorne =  ['target_value','validation_metric','loss','accuracy','recall','specificity','precision','roc_auc',]
+        zeilen_hinten = ['epochs','time/epoch','train_time',]    
+        result = result.set_index('name').T
+        result = pak.move_cols( result, zeilen_vorne )      
+        result = pak.move_cols( result, zeilen_hinten, -1 )    
+        result = result.T.reset_index()
 
+        # Zeilen löschen
+        zeilen_verboten = []
+        zeilen_erlaubt = [z for z in ( zeilen_vorne + zeilen_hinten) if not z in zeilen_verboten ]
+        mask = result.name.isin( zeilen_erlaubt )
+        result = result[mask]
+        
+    else: # size == 'big'
+        result = result.sort_values('name')
+        zeilen_vorne =  ['target_value','validation_metric','loss',]
+        zeilen_hinten = ['experiment_name','experiment_path','output_feature_type','output_feature_name','epochs','train_secs','time/epoch','train_time',]     
+        result = result.set_index('name').T
+        result = pak.move_cols( result, zeilen_vorne )         
+        result = pak.move_cols( result, zeilen_hinten, -1 )    
+        result = result.T.reset_index()        
+
+    result = pak.reset_index(result)
+    result.columns = [c if isinstance(c,str) else 'model_' + str(c) for c in result.columns ]
+    return result
```

