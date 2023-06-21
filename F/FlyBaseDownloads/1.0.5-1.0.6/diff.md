# Comparing `tmp/FlyBaseDownloads-1.0.5.tar.gz` & `tmp/FlyBaseDownloads-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyBaseDownloads-1.0.5.tar", last modified: Fri Jun 16 00:24:28 2023, max compression
+gzip compressed data, was "FlyBaseDownloads-1.0.6.tar", last modified: Wed Jun 21 00:20:51 2023, max compression
```

## Comparing `FlyBaseDownloads-1.0.5.tar` & `FlyBaseDownloads-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-16 00:24:28.967659 FlyBaseDownloads-1.0.5/
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-16 00:24:28.963659 FlyBaseDownloads-1.0.5/FlyBaseDownloads/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     5250 2023-06-16 00:22:09.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/Downloads.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     1497 2023-06-15 22:52:26.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/FBD.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      616 2023-06-15 23:09:00.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/__init__.py
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-16 00:24:28.967659 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     1163 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Alleles_Stocks.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      782 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Clones.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     1216 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Gene_Ontology_annotation.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      890 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Gene_groups.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     3621 2023-06-15 22:55:14.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Genes.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      761 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Homologs.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      821 2023-06-15 21:36:31.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Human_disease.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      798 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Insertions.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     1277 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Ontology_Terms.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      522 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Organisms.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      572 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/References.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      513 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Synonyms.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       10 2023-06-15 23:11:35.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/__init__.py
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-16 00:24:28.967659 FlyBaseDownloads-1.0.5/FlyBaseDownloads.egg-info/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26511 2023-06-16 00:24:28.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      827 2023-06-16 00:24:28.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-16 00:24:28.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-16 00:24:28.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads.egg-info/requires.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-16 00:24:28.000000 FlyBaseDownloads-1.0.5/FlyBaseDownloads.egg-info/top_level.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26511 2023-06-16 00:24:28.967659 FlyBaseDownloads-1.0.5/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.5/README.md
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-16 00:24:28.967659 FlyBaseDownloads-1.0.5/setup.cfg
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      945 2023-06-16 00:19:09.000000 FlyBaseDownloads-1.0.5/setup.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-21 00:20:51.442672 FlyBaseDownloads-1.0.6/
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-21 00:20:51.438671 FlyBaseDownloads-1.0.6/FlyBaseDownloads/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     5500 2023-06-20 19:01:36.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/Downloads.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     1497 2023-06-15 22:52:26.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/FBD.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      616 2023-06-15 23:09:00.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/__init__.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-21 00:20:51.442672 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     1163 2023-06-20 23:51:59.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Alleles_Stocks.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      782 2023-06-20 23:50:13.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Clones.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     1504 2023-06-20 18:16:23.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Gene_Ontology_annotation.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      974 2023-06-20 19:03:57.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Gene_groups.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     3621 2023-06-20 23:52:31.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Genes.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      761 2023-06-20 23:51:36.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Homologs.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      821 2023-06-20 23:52:14.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Human_disease.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      798 2023-06-20 23:51:03.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Insertions.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     1186 2023-06-20 23:46:52.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Ontology_Terms.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      522 2023-06-20 23:51:19.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Organisms.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      572 2023-06-20 23:50:28.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/References.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      513 2023-06-20 23:51:50.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Synonyms.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)        9 2023-06-20 23:52:40.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/__init__.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-21 00:20:51.438671 FlyBaseDownloads-1.0.6/FlyBaseDownloads.egg-info/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    49645 2023-06-21 00:20:51.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      827 2023-06-21 00:20:51.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-21 00:20:51.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-21 00:20:51.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads.egg-info/requires.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-21 00:20:51.000000 FlyBaseDownloads-1.0.6/FlyBaseDownloads.egg-info/top_level.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    49645 2023-06-21 00:20:51.442672 FlyBaseDownloads-1.0.6/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    49074 2023-06-21 00:16:20.000000 FlyBaseDownloads-1.0.6/README.md
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-21 00:20:51.442672 FlyBaseDownloads-1.0.6/setup.cfg
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      945 2023-06-21 00:05:49.000000 FlyBaseDownloads-1.0.6/setup.py
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/Downloads.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/Downloads.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jun 15 17:04:19 2023
 
-@author: usuario
+@author: javiera.quiroz
 """
 
 
 import pandas as pd
 import fnmatch
 import gzip
 from ftplib import FTP
@@ -26,158 +26,175 @@
         
     def download_file(self):
         
         url = self.url
         
         ftp = FTP(url.split('/')[2])
         ftp.login()
-        ruta_directorio = '/'.join(url.split('/')[3:-1])
-
-
-        ftp.cwd(ruta_directorio)
-
-        archivos_remotos = ftp.nlst()
-
-        archivos_filtrados = list(fnmatch.filter(archivos_remotos, url.split('/')[-1]))
-
-        archivos = []
-        for archivo in archivos_filtrados:
-            ruta_archivo = '../' + archivo
-            if not os.path.exists(archivo):
-                with open(ruta_archivo, 'wb') as archivo_local:
-                    ftp.retrbinary('RETR ' + archivo, archivo_local.write)
-    
-                    archivos.append(archivo)
+        directory_path = '/'.join(url.split('/')[3:-1])
+        
+        ftp.cwd(directory_path)
+        
+        remote_files = ftp.nlst()
+        
+        filtered_files = list(fnmatch.filter(remote_files, url.split('/')[-1]))
+        
+        files = []
+        for file in filtered_files:
+            file_path = '../' + file
+            if not os.path.exists(file):
+                with open(file_path, 'wb') as local_file:
+                    ftp.retrbinary('RETR ' + file, local_file.write)
+        
+                files.append(file)
             else:
-                archivos.append(archivo)
-
+                files.append(file)
+        
         ftp.quit()
-        if len(archivos) > 0:
-            return archivos
+        if len(files) > 0:
+            return files
         else:
             print('Failed to download the file')
             return []
         
     
     
     
-    def open_file_tsv(self, ruta_archivo, header):
+    def open_file_tsv(self, file_path, header):
         a = []
 
-        if re.search(r'gz', ruta_archivo):
+        if re.search(r'gz', file_path):
             
             try: 
-                with gzip.open('../' + ruta_archivo, 'rt') as archivo:
-                   df = pd.read_csv(archivo, sep='\t', header=header)
+                with gzip.open('../' + file_path, 'rt') as file:
+                   df = pd.read_csv(file, sep='\t', header=header)
                    a.append(df)
                 return (a[0])
             
             except: 
                 try:
-                    with gzip.open('../' + ruta_archivo, 'rt') as archivo:
-                        df = csv.reader(archivo, delimiter='\t')
+                    with gzip.open('../' + file_path, 'rt') as file:
+                        df = csv.reader(file, delimiter='\t')
                         a.append(pd.DataFrame(df))
                 
                     df = a[0]
                     columns = df.iloc[header, :].tolist()
         
-                    # Elimina la fila del encabezado del DataFrame
                     df = df.iloc[header + 1:, :]
                     
-                    # Asigna los nuevos nombres de columna al DataFrame
                     df.columns = columns
                     df = df.dropna(axis='columns')
                   
   
                     return (df)
                 except:
                     print('Failed to download the file') 
                     
-    def open_file_json(self, ruta_archivo):
+    def open_file_json(self, file_path):
         
         a = []
 
-        if re.search(r'gz', ruta_archivo):
+        if re.search(r'gz', file_path):
             
             try: 
-                with gzip.open('../' + ruta_archivo, 'rt') as archivo:
-                    d = json.load(archivo)
+                with gzip.open('../' + file_path, 'rt') as file:
+                    d = json.load(file)
                     d_ = d['data']
-                    datos = pd.DataFrame(d_)
-                    a.append(datos)
+                    data = pd.DataFrame(d_)
+                    a.append(data)
                    
             except:
                 try:
-                    with gzip.open('../' + ruta_archivo, 'rt') as archivo:
-                        return json.load(archivo)
+                    with gzip.open('../' + file_path, 'rt') as file:
+                        return json.load(file)
                 except:
                     print('Failed to download the file') 
             
         
         return a[0]
                     
-    def open_obo(self, ruta_archivo):
+    def open_obo(self, file_path):
     
         a = []
         
         try:
-            if re.search(r'gz', ruta_archivo):
-                with gzip.open('../' + ruta_archivo, 'rt') as archivo:
-                   if re.search(r'obo', ruta_archivo):
+            if re.search(r'gz', file_path):
+                with gzip.open('../' + file_path, 'rt') as file:
+                   if re.search(r'obo', file_path):
                        
-                      graph = obonet.read_obo(archivo)
+                      graph = obonet.read_obo(file)
                       
                       a.append(graph)
 
             return a[0]
         
         except:
             print('Failed to download the file') 
+            
+    def open_fb(self, file_path,start_line, columns):
+        a = []
+
+        if re.search(r'gz', file_path):
+            
+            try:
+                with gzip.open('../' + file_path, 'rt') as file:
+                    df = csv.reader(file, delimiter='\t')
+                    a.append(pd.DataFrame(df))
+            
+                df = a[0]
+                
+                df = df.iloc[start_line:, :-2]
+                df.columns = columns
+              
+
+                return (df)
+                            
+            except:
+                    print('Failed to download the file') 
         
     
     def get(self, header = None):
         
-        archivos = []
+        files = []
         
         try:
-            archivos = self.download_file()
+            files = self.download_file()
         except:
             print('Failed to download the file') 
         patron = r"##?\s?\w+"
         
         def df_r(df):
             if re.search(r"FB\w{9}", df.columns[0]):
                 df_columns = pd.DataFrame(df.columns).T
 
                 df.columns = range(len(df.columns))
                 
-                # Unir la fila de columnas con el resto del DataFrame
+               
                 df = pd.concat([df_columns, df], ignore_index=True, axis = 0)
             
             if re.search(patron, df.iloc[-1,0]):
                 df = df.iloc[:-1, :]
             
             return df
         
         
-        if len(archivos) > 0:
+        if len(files) > 0:
             if re.search('.obo', self.url):
-                return self.open_obo(archivos[0])
+                return self.open_obo(files[0])
             elif re.search('.json', self.url):
                 try:
-                    return df_r(self.open_file_json(archivos[0]))
+                    return df_r(self.open_file_json(files[0]))
                     
                 except:
                     try:
-                        df = self.open_file_json(archivos[0])
+                        df = self.open_file_json(files[0])
                         df = pd.concat([df.drop(['driver'], axis=1), df['driver'].apply(pd.Series)], axis=1)
 
-                        # Reemplazar los valores None por NaN
                         df = df.replace({None: pd.NA})
                         return df_r(df)
                     except:
-                        return self.open_file_json(archivos[0])
+                        return self.open_file_json(files[0])
                     
             else:
-                return df_r(self.open_file_tsv(archivos[0], header))
+                return df_r(self.open_file_tsv(files[0], header))
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/FBD.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/FBD.py`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/__init__.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/__init__.py`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Alleles_Stocks.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Alleles_Stocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     
         self.main_url = main_url
         self.gen_url = ''
         
     def get(self):
         
         url = self.main_url + self.gen_url + self.un_url
-        descargas = Downloads(url)
+        downloads = Downloads(url)
         
-        return descargas.get(self.header)
+        return downloads.get(self.header)
         
     def Stock(self):
         self.gen_url = 'stocks/'
         self.un_url = 'stocks_*.tsv.gz'
         self.header = 0
         return self.get()
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Clones.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Clones.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,11 +25,11 @@
         self.header = 3
         return self.get()
     
     
     def get(self):    
         url = self.main_url + self.cl_url + self.un_url
         
-        descargas = Downloads(url)
+        downloads = Downloads(url)
         
-        return descargas.get(self.header)
+        return downloads.get(self.header)
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Gene_Ontology_annotation.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Ontology_Terms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,53 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Thu Jun 15 17:25:55 2023
+Created on Thu Jun 15 17:32:48 2023
 
 @author: usuario
 """
 
 from FlyBaseDownloads.Downloads import Downloads 
-import pandas as pd
 
 
-class Gene_Ontology_annotation():
+class Ontology_Terms():
     
     def __init__(self, main_url):
     
         self.main_url = main_url
-        self.go_url = 'go/gene_association.fb.gz'
-        self.header = 5
-        self.df_columns = ['DB', 'DB_Object_ID', 'DB_Object_Symbol',
-                           'Qualifier', 'GO ID', 'DB:Reference',
-                           'Evidence', 'With (or) From', 'Aspect',
-                           'DB_Object_Name', 'DB_Object_Synonym', 'DB_Object_Type',
-                           'taxon', 'Date', 'Assigned_by']
+        self.go_url = 'ontologies/'
+        self.header = None
         
     def get(self):
         
-        url = self.main_url + self.go_url
-        descargas = Downloads(url)
+        url = self.main_url + self.go_url + self.un_url
+        downloads = Downloads(url)
         
-        archivos = []
+        return downloads.get(self.header)
         
-        archivos = descargas.download_file()
-        
-        if len(archivos) > 0:
-            df = descargas.open_file_tsv(archivos[0], self.header)
-            df = df.iloc[:, :-2]
-            df_ = pd.DataFrame(df.columns).T
-            df_.columns = self.df_columns
-            df.columns = self.df_columns
-            return pd.concat([df_, df])
+    def FBbt(self):
+        self.un_url = 'fly_anatomy.obo.gz'
+        return self.get()
+    
+    def FBdv(self):
+        self.un_url = 'fly_development.obo.gz'
+        return self.get()
+    
+    def FBcv(self):
+        self.un_url = 'flybase_controlled_vocabulary.obo.gz'
+        return self.get()
+    
+    def FBsv(self):
+        self.un_url = 'flybase_stock_vocabulary.obo.gz'
+        return self.get()
+    
+    def GO(self):
+        self.un_url = 'go-basic.obo.gz'
+        return self.get()
+    
+    def FBbi(self):
+        self.un_url = 'image.obo.gz'
+        return self.get()
+    
+    def DO(self):
+        self.un_url = 'so-simple.obo.gz'
+        return self.get()
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Gene_groups.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Human_disease.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Thu Jun 15 17:27:27 2023
+Created on Thu Jun 15 18:34:38 2023
 
 @author: usuario
 """
 
-from FlyBaseDownloads.Downloads import Downloads 
-
-class Gene_groups():
+class Human_disease():
     
     def __init__(self, main_url):
-    
         self.main_url = main_url
-        self.gen_url = 'genes/'
+        self.gen_url = 'human_disease/'
         
     def get(self):
         
         url = self.main_url + self.gen_url + self.un_url
-        descargas = Downloads(url)
+        downloads = self.db.Downloads(url)
         
-        return descargas.get(self.header)
+        return downloads.get(self.header)
         
-    def Gene_group(self):
-        self.un_url = 'gene_group_data_fb_*.tsv.gz'
-        self.header = 6
+    def Disease_model_annotations(self):
+        self.gen_url = 'human_disease/'
+        self.un_url = 'disease_model_annotations_fb_*.tsv.gz'
+        self.header = 4
         return self.get()
     
-    def Gene_groups_HGNC(self):
-        self.un_url = 'gene_groups_HGNC_fb_*.tsv.gz'
-        self.header = 6
-        return self.get()
-        
-    def Pathway_group(self):
-        self.un_url = 'pathway_group_data_fb_*.tsv.gz'
-        self.header = 6
+    def Human_Orthologs(self):
+        self.gen_url = 'orthologs/'
+        self.un_url = 'dmel_human_orthologs_disease_fb_*.tsv.gz'
+        self.header = 3
         return self.get()
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Genes.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Genes.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,11 +122,11 @@
         self.header = 4
         return self.get()
 
     
     def get(self):
         
         url = self.main_url + self.gen_url + self.un_url
-        descargas = Downloads(url)
+        downloads = Downloads(url)
         
-        return descargas.get(self.header)
+        return downloads.get(self.header)
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Homologs.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Organisms.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Thu Jun 15 17:28:43 2023
+Created on Thu Jun 15 17:33:17 2023
 
 @author: usuario
 """
 
 from FlyBaseDownloads.Downloads import Downloads 
 
-class Homologs():
+class Organisms():
     
     def __init__(self, main_url):
         self.main_url = main_url
-        self.gen_url = 'orthologs/'
+        self.org_url = 'species/organism_list_fb*.tsv.gz'
+        self.header = 4
         
-    def get(self):
+    
+    def Species_list(self):
         
-        url = self.main_url + self.gen_url + self.un_url
-        descargas = Downloads(url)
+        url = self.main_url + self.org_url
         
-        return descargas.get(self.header)
+        downloads = Downloads(url)
         
-    def Drosophila_Paralogs(self):
-        self.un_url = 'dmel_paralogs_fb_*.tsv.gz'
-        self.header = 4
-        return self.get()
-    
-    def Human_Orthologs(self):
-        self.un_url = 'dmel_human_orthologs_disease_fb_*.tsv.gz'
-        self.header = 3
-        return self.get()
+        return downloads.get(self.header)
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Human_disease.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Insertions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Thu Jun 15 18:34:38 2023
+Created on Thu Jun 15 17:34:00 2023
 
 @author: usuario
 """
 
-class Human_disease():
+from FlyBaseDownloads.Downloads import Downloads 
+
+class Insertions():
     
     def __init__(self, main_url):
+    
         self.main_url = main_url
-        self.gen_url = 'human_disease/'
+        self.in_url = 'insertions/'
+        self.header = 0
         
-    def get(self):
+    def GAL4_drivers(self):
+        self.un_url = 'fu_gal4_table_fb_2023_03.json.gz'
+        df = self.get()
         
-        url = self.main_url + self.gen_url + self.un_url
-        descargas = self.db.Downloads(url)
+        return df
         
-        return descargas.get(self.header)
         
-    def Disease_model_annotations(self):
-        self.gen_url = 'human_disease/'
-        self.un_url = 'disease_model_annotations_fb_*.tsv.gz'
-        self.header = 4
-        return self.get()
     
-    def Human_Orthologs(self):
-        self.gen_url = 'orthologs/'
-        self.un_url = 'dmel_human_orthologs_disease_fb_*.tsv.gz'
+    def Map_insertions(self):
+        self.un_url = 'insertion_mapping_fb_*.tsv.gz'
         self.header = 3
-        return self.get()
+        return self.get()
+        
+    def get(self):
+        url = self.main_url + self.in_url + self.un_url
+        
+        downloads = Downloads(url)
+        
+        return downloads.get(self.header)
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/Organisms.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/References.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Thu Jun 15 17:33:17 2023
+Created on Thu Jun 15 17:35:38 2023
 
 @author: usuario
 """
 
 from FlyBaseDownloads.Downloads import Downloads 
 
-class Organisms():
+class References():
     
     def __init__(self, main_url):
+    
         self.main_url = main_url
-        self.org_url = 'species/organism_list_fb*.tsv.gz'
-        self.header = 4
+        self.org_url = 'references/fbrf_pmid_pmcid_doi_fb*.tsv.gz'
+        self.header = 2
         
     
-    def Species_list(self):
+    def FBrf_PMid_PMCid_doi(self):
         
         url = self.main_url + self.org_url
         
-        descargas = Downloads(url)
+        downloads = Downloads(url)
         
-        return descargas.get(self.header)
+        df = downloads.get(self.header)
+        return df.iloc[1:, :]
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads/classes/References.py` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads/classes/Synonyms.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Thu Jun 15 17:35:38 2023
+Created on Thu Jun 15 17:04:57 2023
 
 @author: usuario
 """
 
 from FlyBaseDownloads.Downloads import Downloads 
 
-class References():
+class Synonyms():
     
     def __init__(self, main_url):
     
         self.main_url = main_url
-        self.org_url = 'references/fbrf_pmid_pmcid_doi_fb*.tsv.gz'
-        self.header = 2
+        self.syn_url = 'synonyms/fb_synonym_*.tsv.gz'
+        self.header = 3
         
     
-    def FBrf_PMid_PMCid_doi(self):
+    def get(self):
         
-        url = self.main_url + self.org_url
+        url = self.main_url + self.syn_url
         
-        descargas = Downloads(url)
+        downloads = Downloads(url)
         
-        df = descargas.get(self.header)
-        return df.iloc[1:, :]
+        return downloads.get(self.header)
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads.egg-info/PKG-INFO` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,89 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.5
+Version: 1.0.6
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
+
 # FlyBaseDownloads
 
 Python package to facilitate the data download from FlyBase. Most of the available data from their official wiki can be downloaded. One of the purposes of this library is to organize the data as closely as possible to the source, **FlyBase**. Despite not being the official package, it is organized by data class/type and provides direct downloads of the current bulk data files from the FTP site.
 For more information, visit the [official FlyBase wiki](https://wiki.flybase.org/wiki/FlyBase:Downloads_Overview).
 
+- [Usage and Installation](#usageninstallation)
+- [Synonyms](#synonyms)
+- [Genes](#genes)
+    - [Genetic interaction table](#git) 
+    - [RNA-Seq RPKM values](#rnaseq-v)
+    - [RNA-Seq RPKM values matrix](#rnaseq-m) 
+    - [Single Cell RNA-Seq Gene Expression](#single-cell)
+    - [Physical interaction MITAB file](#mitab)
+    - [Functional complementation table](#fct)
+    - [FBgn to DB Accession IDs](#fbgn-db)
+    - [FBgn to Annotation ID](#fbgn-ann)
+    - [FBgn to GLEANR IDs](#fbgn-gl)
+    - [FBgn to FBtr to FBpp IDs ](#fbgn-fbpp)
+    - [FBgn to FBtr to FBpp IDs (expanded)](#fbgn-fbpp-e)
+    - [FBgn exons to Affy1](#fbgn-af1)
+    - [FBgn exons to Affy2](#fbgn-af2)
+    - [Genes Sequence Ontology (SO) data](#go-gene)
+    - [Genes map table](#genes-map)
+    - [Best gene summaries](#bgs)
+    - [Automated gene summaries](#ags)
+    - [Gene Snapshots](#gss)
+    - [Unique protein isoforms](#upi)
+    - [Non-coding RNAs](#non-cod)
+    - [Enzyme](#enzyme)
+ - [Gene Ontology annotation files GO](#go-file)
+	  - [Gene Association File - GAF](#gaf) 
+ - [Gene Groups](#gene-groups)
+	  - [Gene group data](#ggd) 
+	  - [Gene groups with HGNC IDs](#hgnc) 
+	  - [Pathway group](#pathway) 
+ - [Alleles and Stocks](#aands)
+	  - [Stock](#stock)
+	  - [Genetic interactions](#genint)
+	  - [Phenotypic](#pheno) 
+	  - [Alleles to Genes](#alltoge)
+ - [Homologs](#homs)
+	  - [Drosophila Paralogs](#paral)
+	  - [Human Orthologs](#hort-d) 
+ - [Human disease](#hudss)
+	  - [Human disease model](#hdm) 
+	  - [Human Orthologs](#hort-h) 
+ - [Organisms](#orgs)
+	  - [Species list](#species) 
+ - [Ontology Terms](#ont-tr)
+	  - [Fly Anatomy](#f-bt-on)
+	  - [Fly Development](#f-dv-on)
+	  - [Flybase Controlled Vocabulary](#f-cv-on) 
+	  - [Fly Stock Ontology](#f-sv-on)
+	  - [Gene Ontology](#f-go-on)
+	  - [Image Ontology](#f-bi-on) 
+	  - [Human Disease Ontology](#f-do-on)
+ - [Insertions](#insr)
+	  - [Map data for insertions](#mp-insr)
+	  - [Frequently-used GAL4 drivers table](#gal4)
+ - [Clones](#clones)
+	  - [cDNAs: FBcl to acc. ID](#dna-fbcl-acc) 
+	  - [Genomic: FBcl to acc. ID](#gen-fbcl-acc) 
+ - [References](#ref)
+	  - [FlyBase FBrf to PubMed ID to PMCID to DOI](#ref-get) 
 
-# Bulk data files
+# Usage and Installation <a name="usageninstallation"></a>
 
 In order to simplify the download of FlyBase files, the names have been kept as close as possible. To access the data, follow these steps:
 
 1. Install the library using the pip command.
 
     > pip install FlyBaseDownloads
 
@@ -31,15 +91,15 @@
 
     > import FlyBaseDownloads as FBD
 
 3. Access the different classes of the library described below.
 
 
 
-## Synonyms
+## Synonyms <a name="synonyms"></a>
 
 To download the file, execute the following command.
 
     Synonyms = FBD.Synonyms.get()
 
 The file reports current symbols and synonyms for the following objects in FlyBase: genes (FBgn), alleles (FBal), balancers (FBba), aberrations (FBab), transgenic constructs (FBtp), insertions (FBti), transcripts (FBtr), and proteins (FBpp).
 
@@ -51,23 +111,23 @@
 | organism_abbreviation   | Abbreviation (from the Species Abbreviations list) indicating the species of origin |
 | current_symbol   | Current symbol used in FlyBase for the object |
 | current_fullname   | Current full name used in FlyBase for the object|
 | fullname_synonym(s)   | 	Non-current full name(s) associated with the object (pipe separated values) |
 | symbol_synonym(s)   | Non-current symbol(s) associated with the object (pipe separated values) |
 
 
-## Genes
+## Genes <a name="genes"></a>
 
 To facilitate its usage, it is suggested to access the data using the following command.
 
     Genes = FBD.Genes
 
 Then, enter the specific method according to the desired data
 
-#### Genetic interaction table
+#### Genetic interaction table <a name="git"></a>
 
 To download the file, execute the following command.
 
     Genetic_interaction_table = Genes.Genetic_interaction_table()
 
 Columns Description
 
@@ -77,15 +137,15 @@
 | Starting_gene(s)_FBgn | Current FlyBase identifier (FBgn#) of gene(s) involved in the starting genotype |
 | Interacting_gene(s)_symbol | Current FlyBase symbol of gene(s) involved in the interacting genotype |
 | Interacting_gene(s)_FBgn | Current FlyBase identifier (FBgn#) of gene(s) involved in the interacting genotype |
 | Interaction_type | Type of interaction observed, either 'suppressible' or 'enhanceable' |
 |Publication_FBrf | Current FlyBase identifier (FBrf#) of publication from which the data came |
 
 
-#### RNA-Seq RPKM values
+#### RNA-Seq RPKM values <a name="rnaseq-v"></a>
 
 To download the file, execute the following command.
 
     RNASeq_values = Genes.RNASeq_values()
 
 Columns Description
 
@@ -100,15 +160,15 @@
 | RNASource_name	| The official FlyBase symbol for the RNA-Seq experiment used for RPKM expression calculation |
 | RPKM_value	| The RPKM expression value for the gene in the specified RNA-Seq experiment |
 | Bin_value	| The expression bin classification of this gene in this RNA-Seq experiment, based on RPKM value. Bins range from 1 (no/extremely low expression) to 8 (extremely high expression)| 
 | Unique_exon_base_count	T| he number of exonic bases unique to the gene (not overlapping exons of other genes). Field will be blank for genes derived from dicistronic/polycistronic transcripts |
 | Total_exon_base_count	| The number of bases in all exons of this gene |
 | Count_used	| Indicates if the RPKM expression value was calculated using only the exonic regions unique to the gene and not overlapping exons of other genes (Unique), or, if the RPKM expression value was calculated based on all exons of the gene regardless of overlap with other genes (Total). RPKM expression values are typically reported for the "Unique" count, except for genes on dicistronic/polycistronic transcripts, in which case the "Total" count is reported |
 
-#### RNA-Seq RPKM values matrix
+#### RNA-Seq RPKM values matrix <a name="rnaseq-m"></a>
 
 To download the file, execute the following command.
 
     RNASeq_values_matrix = Genes.RNASeq_values_matrix()
 
 Columns Description
 
@@ -117,15 +177,15 @@
 | gene_primary_id	| The unique FlyBase gene ID for this gene.
 |gene_symbol	| The official FlyBase symbol for this gene.|
 | gene_fullname	| The official full name for this gene.|
 | gene_type	| The type of gene: e.g., protein_coding_gene, non_protein_coding_gene.|
 | DATASAMPLE_NAME_(DATASET_ID)	| Each subsequent column reports the gene RPKM values for the sample listed in the header. The dataset "FBlc" ID is listed in parentheses, and can be pasted into FlyBase search to access more information on the sample from the "dataset" report.|
 
 
-#### Single Cell RNA-Seq Gene Expression
+#### Single Cell RNA-Seq Gene Expression <a name="single-cell"></a>
 
 To download the file, execute the following command.
 
     SingleCellRNASeq_Gene_Expression = Genes.Single_Cell_RNA_Gene_Expression()
 
 Columns Description
 
@@ -143,51 +203,51 @@
 | Cluster_Cell_Type_ID	| The FlyBase FBbt ID for the cell type represented by the cell cluster.| 
 | Cluster_Cell_Type_Name	| The FlyBase name for the cell type represented by the cell cluster.| 
 | Gene_ID	| The FlyBase FBgn ID for the expressed gene.| 
 | Gene_Symbol	| The FlyBase symbol for the expressed gene (ASCII-format).|
 | Mean_Expression	| The average level of expression of the gene across all cells of the cluster in which the gene is detected at all.|
 | Spread	| The proportion of cells in the cluster in which the gene is detected.| 
 
-#### Physical interaction MITAB file
+#### Physical interaction MITAB file <a name="mitab"></a>
 
 To download the file, execute the following command.
 
     Physical_interaction_MITAB = Genes.Physical_interaction_MITAB()
 
 Columns Description
 
 | Column number	| Column heading	| General format	| FlyBase example	| Content description | 
 |----------------------|--------------------|----------------------|--------------------|----------------------|
 | 1 | ID(s) Interactor A                   | database:identifier            | flybase:FBgn0002121| The unique Flybase identifier for the first gene of the interacting pair.              |                           |
 | 2 | ID(s) Interactor B                   | -                              | -                  | The unique Flybase identifier for the second gene of the interacting pair.             |                           |
 | 3 | Alt ID(s) Interactor A               | database:identifier            | flybase:CG2671\| entrez gene/locuslink:33156 | The alternative gene identifiers currently provided are Flybase annotation IDs (CG#) and NCBI’s Entrez Gene ID separated by “\|“                           |
 | 4 | Alt ID(s) Interactor B               | -                              | -                  |                        -                          |
 | 5 | Alias(es) Interactor A               | database:name(alias type)      | flybase:l(2)gl(gene name) | The official Flybase gene symbol. It is referred to as “gene name” to adhere to the psi-mi ontology. |                           |
-| 6 | Alias(es) Interactor B               | -                              | ”-                  |                    -      |                       
+| 6 | Alias(es) Interactor B               | -                              | -                  |                    -      | 
 | 7 | Interaction Detection Method(s)      | ontology:identifier(method name) | psi-mi:"MI:0006"(anti bait coimmunoprecipitation) | The assay used to detect the interaction, taken from the psi-mi ontology. |                           |
 | 8 | Publication 1st Author(s)            | surname initial(s) (publication year) | Betschinger K. (2003) | The first author and year of the publication where the interaction is described. |                           |
 | 9 | Publication ID(s)                    | database:identifier            | flybase:FBrf0157155\|pubmed:12629552 | The unique FlyBase identifier for the publication followed by the unique PubMed identifier (if there is one) separated by “\|”. |                           |
 | 10| Taxid Interactor A                   | taxid:identifier               | taxid:7227("Drosophila melanogaster") | The NCBI taxonomy identifier for the source organism of the interactor. The vast majority of interactors in FlyBase come from D. melanogaster. There are, however, a few interspecies interactions consisting of a D. melanogaster interactor and an interactor of a different species. |                           |
-| 11| Taxid Interactor B                   | -                              | -                  |           -                |                           
+| 11| Taxid Interactor B                   | -                              | -                  |           -                | 
 | 12| Interaction Type(s)                  | ontology:identifier(interaction type) | psi-mi:"MI:0915"(physical association) | Taken from the psi-mi ontology. Most often “physical association” for FlyBase. |                           |
-| 13| Source Database(s)                   | ontology:identifier(database name) | psi-mi:"MI:0478"(flybase) | All interactions are curated by FlyBase. |                           
-| 14| Interaction Identifier(s)            | database:identifier            | flybase:FBrf0157155-13.coIP.WB | The unique FlyBase identifier for this interaction. |                                             
+| 13| Source Database(s)                   | ontology:identifier(database name) | psi-mi:"MI:0478"(flybase) | All interactions are curated by FlyBase. | 
+| 14| Interaction Identifier(s)            | database:identifier            | flybase:FBrf0157155-13.coIP.WB | The unique FlyBase identifier for this interaction. | 
 | 15	| Confidence Value(s) |	-|-|		Not applicable	
 | 16	| Expansion Method(s) |-|-| Not applicable
 | 17	| Biological Role(s)  Interactor A	| -|-|		Not applicable	
 | 18	| Biological Role(s) Interactor B	| -|-|		Not applicable	
 | 19	| Experimental Role(s) Interactor A	| ontology:identifier(experimental role name) |	psi-mi:"MI:0496"(bait)	| The role played by the interactor in the experiment. Taken from the psi-mi ontology.	|
 | 20	| Experimental Role(s) Interactor B | -|-|	-|	
 | 21	| Type(s) Interactor A |	ontology:identifier(interactor type name)	| psi-mi:"MI:0326"(protein)	| The molecule type. For FlyBase, these are limited to protein or ribonucleic acid. Taken from the psi-mi ontology.	|
-| 22	| Type(s) Interactor B	| -|-|-|		
+| 22	| Type(s) Interactor B	| -|-|-| 
 | 23	| Xref(s) Interactor A	|-|-|	Not applicable	
 | 24	| Xref(s) Interactor B	|	-|-|	Not applicable	
 | 25	| Interaction Xref(s) |	database:identifier	| flybase:FBig0000000103	| Cross references for the interactions. For Flybase, these include an interaction group identifier (FBig) and possibly a collection identifier (FBlc) separated by “\|”. All experiments that show an interaction between the products of gene A and gene B are compiled into an A-B interaction group, such that all interactions are associated with an interaction group identified by an FBig number. Interactions identified as part of a large scale study are also associated with the collection identifier, or FBlc number.	|
 | 26	| Annotation(s) Interactor A |	topic:text	isoform-| comment:a isoform	| Information on whether the interaction is specific to a particular interactor isoform.	
-| 27	| Annotation(s) Interactor B |	- | - | -| 	
+| 27	| Annotation(s) Interactor B |	- | - | -|
 | 28	| Interaction Annotation(s) |	topic:text	| comment:Phosphorylated isoforms of @l(2)gl@ are absent when @aPKC@ is knocked down by RNAi.	| Describes the source(s) of the interaction participants and includes free text comments about the interaction.	|
 | 29	| Host Organism(s)	|	- | - | Not applicable	|
 | 30	| Interaction Parameters  | - | -	|	Not applicable	|
 | 31	| Creation Date	| - | - |	Not applicable	|
 | 32	| Update Date	| - | - |		Not applicable	|
 | 33	| Checksum Interactor A	| - | -	|	Not applicable	|
 | 34	| Checksum Interactor B	| - | -	|	Not applicable	|
@@ -197,15 +257,15 @@
 | 38	| Feature(s) Interactor B	| -	| - | -|
 | 39	| Stoichiometry Interactor A |-|-| Not applicable	|
 | 40	| Stoichiometry Interactor B |-|-| Not applicable| 
 | 41	| Identification Method(s) Participant A	|-|-|	Not applicable| 
 | 42	| Identification Method(s) Participant B |-|-|	Not applicable| 
 
 
-#### Functional complementation table
+#### Functional complementation table <a name="fct"></a>
 
 To download the file, execute the following command.
 
     Functional_complementation = Genes.Functional_complementation()
 
 Columns Description
 
@@ -213,15 +273,15 @@
 |----------------------|--------------------|
 | Dmel gene (symbol)	|Current FlyBase symbol of Dmel gene.|
 | Dmel gene (FBgn)	| Current FlyBase identifier (FBgn#) of Dmel gene in column 1.|
 | Functionally complementing ortholog (symbol)	| Current FlyBase symbol of a non-Dmel ortholog of the Dmel gene in column 1 where this non-Dmel gene has been show to functionally complement the Dmel gene.|
 | Functionally complementing ortholog (FBgn#)	| Current FlyBase identifier (FBgn#) of a non-Dmel ortholog of the Dmel gene in column 1 where this non-Dmel gene has been show to functionally complement the Dmel gene.|
 | Supporting_FBrf	| Current FlyBase identifier (FBrf#) of the publication that provides support for the functional complementation statement (the publication that reported the suppression of a mutant phenotype of the Dmel gene by a transgenic construct/mutant allele of the non-Dmel ortholog).|
 
-#### FBgn to DB Accession IDs
+#### FBgn to DB Accession IDs <a name="fbgn-db"></a>
 
 To download the file, execute the following command.
 
     FBgn_toDB_Accession_IDs = Genes.FBgn_toDB_Accession_IDs()
 
 Columns Description
 
@@ -233,15 +293,15 @@
 nucleotide_accession	| EMBL/GenBank/DDBJ nucleotide accession associated with the gene.|
 | na_based_protein_accession	| EMBL/GenBank/DDBJ protein accession associated with the gene and the nucleotide accession in the preceeding 'nucleotide_accession' column|
 | UniprotKB/Swiss-Prot/TrEMBL_accession	| UniProtKB/SwissProt/TrEMBL protein accession associated with the gene.|
 |EntrezGene_ID	| NCBI Entrez ID associated with the gene.
 |RefSeq_transcripts	| NCBI RefSeq transcript accession associated with the gene.|
 RefSeq_proteins	| NCBI RefSeq protein accession associated with the gene and the transcript accession in the preceeding 'RefSeq_transcripts' column.|
 
-#### FBgn to Annotation ID
+#### FBgn to Annotation ID <a name="fbgn-ann"></a>
 
 To download the file, execute the following command.
 
     FBgn_toAnnotation_ID = Genes.FBgn_toAnnotation_ID()
 
 Columns Description
 
@@ -250,44 +310,44 @@
 | gene_symbol	| Current symbol of gene.|
 | organism_abbreviation	| Abbreviation (from the Species Abbreviations list) indicating the species of origin of the gene.|
 | primary_FBgn#	| Current FlyBase identifier (FBgn#) of gene.|
 | secondary_FBgn#(s)	| Secondary FlyBase identifier(s) (FBgn#) associated with the gene (comma separated values).| 
 | annotation_ID	| Current annotation identifier associated with the gene.|
 | secondary_annotation_ID(s)	|Secondary annotation identifier(s) associated with the gene (comma separated values).|
 
-#### FBgn to GLEANR IDs
+#### FBgn to GLEANR IDs <a name="fbgn-gl"></a>
 
 To download the file, execute the following command.
 
     FBgn_toGLEANR_IDs = Genes.FBgn_toGLEANR_IDs()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |organism_abbreviation	| Abbreviation (from the Species Abbreviations list) indicating the species of origin of the gene.|
 |gene_symbol	| Current FlyBase gene symbol.|
 |primary_FBgn#	| Current FlyBase identifier (FBgn#) of the gene.|
 |GLEANR_ID	| GLEANR identifier assigned by the AAA Consortium.|
 
-#### FBgn to FBtr to FBpp IDs
+#### FBgn to FBtr to FBpp IDs <a name="fbgn-fbpp"></a>
 
 To download the file, execute the following command.
 
     FBgn_to_FBtr_to_FBpp = Genes.FBgn_to_FBtr_to_FBpp()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FlyBase_FBgn	|Current FlyBase identifier (FBgn#) of the gene.|
 |FlyBase_FBtr	|Current FlyBase identifier (FBtr#) of a transcript encoded by the gene listed in the preceeding 'FlyBase_FBgn' column.|
 |FlyBase_FBpp	|Current FlyBase identifier (FBpp#) of a polypeptide encoded by the transcript listed in the preceeding 'FlyBase_FBtr' column, where this is relevant.|
 
-#### FBgn to FBtr to FBpp IDs (expanded)
+#### FBgn to FBtr to FBpp IDs (expanded) <a name="fbgn-fbpp-e"></a>
 
 To download the file, execute the following command.
 
     FBgn_to_FBtr_to_FBpp_exp = Genes.FBgn_to_FBtr_to_FBpp_expanded()
 
 Columns Description
 
@@ -301,15 +361,15 @@
 |annotation_ID	|Current FlyBase annotation identifier of the gene.|
 |transcript_type	|The type of transcript, represented by a Sequence Ontology term.|
 |transcript_ID	|Current FlyBase annotation identifier of the transcript.|
 |transcript_symbol	|Current symbol of the transcript.|
 |polypeptide_ID	|Current FlyBase annotation identifier of the polypeptide.|
 |polypeptide_symbol	|Current symbol of the polypeptide.|
 
-#### FBgn exons to Affy1 
+#### FBgn exons to Affy1 <a name="fbgn-af1"></a>
 
 To download the file, execute the following command.
 
     FBgn_exons2affy1 = Genes.FBgn_exons2affy1()
 
 The file is generated by testing for overlaps, no matter how small, of the locations of Affy1 oligos in the genome with the locations of gene exons, as defined by the Dmel gene models for the current release of FlyBase. If the location of an Affy1 oligo shows any kind of overlap with an exon of a gene, a Gene=>Affy reference is recorded in this file.
 
@@ -322,38 +382,38 @@
 
 it excludes:
  - genes not located to the sequence
  - mitochondrial genes
 
 The first column of a line it is the FBgn ID, and the second one is the Affy1 ID that overlaps with an exon of the gene.
 
-#### FBgn exons to Affy2
+#### FBgn exons to Affy2 <a name="fbgn-af2"></a>
 
 To download the file, execute the following command.
 
     FBgn_exons2affy2 = Genes.FBgn_exons2affy2()
 
 Similar to the Affy1 but with Affy2.
 
-#### Genes Sequence Ontology (SO) data
+#### Genes Sequence Ontology (SO) data <a name="go-gene"></a>
 
 To download the file, execute the following command.
 
     Genes_Sequence_Ontology = Genes.Genes_Sequence_Ontology()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |gene_primary_id	|The unique FlyBase gene ID for this gene.|
 |gene_symbol	|The official FlyBase symbol for this gene.|
 |so_term_name	|The SO term name.|
 |so_term_id	|The SO term primary identifier.|
 
-#### Genes map table
+#### Genes map table <a name="genes-map"></a>
 
 To download the file, execute the following command.
 
     Genes_map = Genes.Genes_map()
 
 Columns Description
 
@@ -362,43 +422,43 @@
 |organism_abbreviation	|Abbreviation (from the Species Abbreviations list) indicating the species of origin of the gene.|
 |current_symbol	|Current FlyBase gene symbol.|
 |primary_FBid	|Current FlyBase identifier (FBgn#) of gene.|
 |recombination_loc	|Recombination map location.|
 |cytogenetic_loc	|Cytogenetic location.|
 |sequence_loc	|Genomic location.|
 
-#### Best gene summaries
+#### Best gene summaries <a name="bgs"></a>
 
 To download the file, execute the following command.
 
     Best_gene_summaries = Genes.Best_gene_summaries()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FBgn_ID	|Current FlyBase identifier number for the gene.|
 |Gene_Symbol	|Current FlyBase symbol of the gene.|
 |Summary_Source	|The source of the gene summary.|
 |Summary	|The gene summary text.|
 
-### Automated_gene_summaries
+### Automated gene summaries <a name="ags"></a>
 
 To download the file, execute the following command.
 
 `Automated_gene_summaries = Genes.Automated_gene_summaries()`
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FlyBase ID. | The Valid FlyBase identifier number for the gene.|
 |Summary| The gene summary as a string of plain text.|
 
-#### Gene Snapshots
+#### Gene Snapshots <a name="gss"></a>
 
 To download the file, execute the following command.
 
     Gene_Snapshots = Genes.Gene_Snapshots()
 
 Columns Description
 
@@ -407,52 +467,458 @@
 |FBgn_ID	|Current FlyBase identifier number for the gene.|
 |GeneSymbol	|Current FlyBase symbol of the gene.|
 |GeneName	|Current FlyBase name of the gene.|
 |datestamp	|Date on which the information was last reviewed.|
 |gene_snapshot_text	| Gene snapshot information for the gene. Cases that are in progress or are deemed to have insufficient data to summarize are stated as such|
 
 
-#### Unique protein isoforms
+#### Unique protein isoforms <a name="upi"></a>
 
 To download the file, execute the following command.
 
     Unique_protein_isoforms = Genes.Unique_protein_isoforms()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FBgn	|Current FlyBase identifier (FBgn#) of the gene.|
 |FB_gene_symbol	|Current FlyBase gene symbol of the gene.|
 |representative_protein	|Current FlyBase protein symbol of the representative protein isoform.|
 |identical_protein(s)	|Current FlyBase protein symbol(s) of identical protein isoforms.|
 
-### Non-coding RNAs
+### Non-coding RNAs <a name="non-cod"></a>
 
 To download the file, execute the following command.
 
     Noncoding_RNAs = Genes.Noncoding_RNAs()
 
 This file reports all ncRNAs with gene models supported by FlyBase in JSON format, as submitted to [RNAcentral](http://rnacentral.org/). Pseudogenes are excluded. In addition to the symbols and IDs for ncRNAs, this file also includes their associated gene, genomic location, sequence, Sequence Ontology classification, etc.
 
 
-#### Enzyme data
+#### Enzyme data <a name="enzyme"></a>
 
 To download the file, execute the following command.
 
     Enzyme = Genes.Enzyme()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
-|group_id	|FlyBase gene group (FBgg) ID of the relevant terminal group within the ENZYMES (FBgg0001715) hierarchy (only terminal groups contain members).
+|group_id	|FlyBase gene group (FBgg) ID of the relevant terminal group within the ENZYMES (FBgg0001715) hierarchy (only terminal groups contain members).|
 |group_name	|FlyBase gene group (FBgg) name of relevant terminal group within the ENZYMES (FBgg0001715) hierarchy (only terminal groups contain members).|
 |group_GO_ID	|The GO molecular function term ID on the given gene group. Multiple entries are separated with a pipe.|
 |group_GO_name	|The GO molecular function term name on the given gene group. Multiple entries are separated with a pipe.|
 |group_EC_number	|The EC number on the given gene group, if present. (This is computed, corresponding to the EC cross-reference on the GO molecular function term.)|
 |group_EC_name	|The EC name on the given gene group, if present. (This is computed, corresponding to the EC cross-reference on the GO molecular function term.)|
 |gene_id	|The current FlyBase gene ID (FBgn) of the gene.|
 |gene_symbol	|The current FlyBase symbol of the gene.|
 |gene_name	|The current FlyBase name of the gene.|
-|gene_EC_number	|The EC number(s) associated with the gene, if present. Multiple entries are separated with a pipe. (This is computed, corresponding to the EC cross-reference(s) on any positive GO molecular function term(s) annotated to the gene.)
+|gene_EC_number	|The EC number(s) associated with the gene, if present. Multiple entries are separated with a pipe. (This is computed, corresponding to the EC cross-reference(s) on any positive GO molecular function term(s) annotated to the gene.)|
 |gene_EC_name	|The EC name(s) associated with the gene, if present. Multiple entries are separated with a pipe. (This is computed, corresponding to the EC cross-reference(s) on any positive GO molecular function term(s) annotated to the gene.)|
+
+## Gene Ontology annotation files <a name="go-file"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    GOAnn = FBD.GOAnn
+
+Then, enter the specific method according to the desired data
+
+#### Gene Association File - GAF <a name="gaf"></a>
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|DB	|The database contributing the gene_association file FB File: always "FB" for gene_association.fb.|
+|DB Object ID |A unique identifier in the database for the item being annotated. FB File: This is always the primary FlyBase identifier number for a Drosophila gene. Example: FBgn0000490|
+|DB Object Symbol |A (unique and valid) symbol to which the DB Object ID is matched. FB File: This is always the valid gene symbol for a Drosophila gene. Example: dpp|
+|Qualifier | For each GO annotation, one of the following as gene product to term relations are used: 'acts_upstream_of', 'acts_upstream_of_negative_effect', 'acts_upstream_of_positive_effect', 'colocalizes_with', 'contributes_to', 'enables', 'involved_in', 'is_active_in', 'located_in', 'part_of'. This column may also contain the 'NOT' qualifier, separated by a pipe (“\|”) from the gene product to term relation, which makes the annotation statement a negation. |
+|GO ID | The unique GO identifier for the GO term attributed to the DB_Object_ID. Example: GO:0005160|
+|DB:Reference | The unique identifier for the reference to which the GO annotation is attributed. FB File: Each FlyBase reference including published literature, conference abstracts, personal communications, sequence records and computer files has a unique 7 digit identifier (an FBrf). Where this reference is a published paper with a PubMed identifier, the PubMed ID is also listed in column 6, separated from the FBrf with a pipe (“\|”). Example: FB:FBrf0136863\|PMID:11432817 |
+|Evidence | The evidence code for the GO annotation; one of IMP, IGI, IPI, ISS, IDA, IEP, IEA, TAS, NAS, ND, IC, RCA, HDA, HMP, HGI, HEP, IBA|
+|With (or) From | FB File: This column contains the identifier for annotations where the evidence code is IGI, IPI, ISS, IEA or IC. For IGI the database gene symbol and identifier is listed. For ISS and IPI the identifier can be a gene symbol and identifier, or a sequence (protein or nucleic acid) identifier. For IC, the GO identifier of the term used as the basis of a curator inference is given. IGI example: FLYBASE:rpr; FB:FBgn0011706, ISS example: UniProt:P35569, ISS example: EMBL:AF064523, ISS example: SGD_LOCUS:COP1; SGD:S0002304, IC example: GO:0045298|
+|Aspect | Which ontology the GO term belongs to: Function ( F ), Process ( P ) or Component ( C ). Example: P| 
+|DB Object Name | FB File: The full name of the FlyBase gene. Example: decapentaplegic Where a FlyBase gene has no full name (eg Pten), this field is left blank.|
+|DB Object Synonym | Alternative names by which the database object is known. FB File: Multiple synonyms of a FlyBase gene are separated by a pipe (“\|”). Example: M(2)LS1\|shortvein\|Dm-DPP\|dpp\|Dpp\|DPP\|CG9885\|TGF-beta\|TGF-&bgr\|TGF-b\|Hin-d\|l(2)10638\|shv\|DPP-C\|ho\|M(2)23AB\|blk\|l(2)22Fa\|l(2)k17036\|Tg\|TGF&bgr |
+| DB Object Type |The type of object being annotated. Always a gene for FlyBase data. FB file: always "gene" for gene_association.fb.|
+|Taxon | The taxonomic identifier of the species encoding the gene product Example: taxon:7227|
+|Date|The date of last annotation update, in the format 'YYYYMMDD'. At present this date is the same for all annotations and corresponds to the date of the latest FlyBase update; we are in the process of changing our system so that dates more accurately reflect the date the annotation is made. Example: 20040821|
+|Assigned by |The source of the GO annotation.|
+
+## Gene groups <a name="gene-groups"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Gene_groups = FBD.Gene_groups
+
+Then, enter the specific method according to the desired data
+
+#### Gene group <a name="ggd"></a>
+
+To download the file, execute the following command.
+
+    Gene_groups_data = Gene_groups.Gene_group() 
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FB_group_id	|Current FlyBase identifier (FBgg##) of Gene Group.|
+|FB_group_symbol	|Current FlyBase symbol of Gene Group.|
+|FB_group_name	|Current FlyBase full name of Gene Group.|
+|Parent_FB_group_id	|Current FlyBase identifier (FBgg##) of parent of given Gene Group (if relevant).|
+|Parent_FB_group_symbol	|Current FlyBase symbol of parent of given Gene Group (if relevant).|
+|Group_member_FB_gene_id	|Current FlyBase identifier (FBgn##) of member gene (if terminal group).|
+|Group_member_FB_gene_symbol	|Current FlyBase symbol of member gene (if terminal group).|
+
+#### Gene groups with HGNC IDs  <a name="hgnc"></a>
+
+To download the file, execute the following command.
+
+    Gene_groups_HGNC= Gene_groups.Gene_groups_HGNC()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FB_group_id	|Current FlyBase identifier (FBgg##) of Gene Group.|
+|FB_group_symbol	|Current FlyBase symbol of Gene Group.|
+|FB_group_name	|Current FlyBase full name of Gene Group.|
+|HGNC_family_ID	|HGNC ID of equivalent human 'gene family'.|
+
+
+#### Pathway group <a name="pathway"></a>
+
+To download the file, execute the following command.
+
+    Pathway_group = Gene_groups.Pathway_group()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FB_group_id	|Current FlyBase identifier (FBgg##) of Pathway Gene Group.|
+|FB_group_symbol	|Current FlyBase symbol of Pathway Gene Group.|
+|FB_group_name	|Current FlyBase full name of Pathway Gene Group.|
+|Parent_FB_group_id	|Current FlyBase identifier (FBgg##) of parent of given Pathway Gene Group (if relevant).|
+|Parent_FB_group_symbol	|Current FlyBase symbol of parent of given Pathway Gene Group (if relevant).|
+|Group_member_FB_gene_id	|Current FlyBase identifier (FBgn##) of member gene (if terminal group).|
+|Group_member_FB_gene_symbol	|Current FlyBase symbol of member gene (if terminal group).|
+
+## Alleles and Stocks <a name="aands"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Alleles_Stocks = FBD.Alleles_Stocks
+
+Then, enter the specific method according to the desired data
+
+#### Stock data <a name="stock"></a>
+
+To download the file, execute the following command.
+
+    Stock = Alleles_Stocks.Stock()
+
+Columns Description
+
+| Column heading           | Content Description          | Example |
+|----------------------|--------------------|--------------------|
+|FBst	|The unique identifier assigned to this stock by FlyBase.|	FBst0000002|
+|collection_short_name	|A short name for the stock collection that holds the stock.	|Bloomington|
+|stock_type_cv	|The controlled vocabulary term and unique identifier that describe the state of the stock.|	living stock ; FBsv:0000002|
+|species	|Abbreviation (from the Species Abbreviations list) indicating the species of the stock.	|Dmel|
+|FB_genotype	|Genetic components of the stock corresponding to alleles, aberrations, balancers, or insertions in FlyBase. May be empty.|	w[*]; betaTub60D[2] Kr[If-1]/CyO|
+|description	|Genetic components of the stock as provided to FlyBase by the collection that holds the stock.	|FlyTrap: ZCL1796 III|
+|stock_number	|The stock identifier provided to FlyBase by the collection that holds the stock. May be empty.	|110818|
+
+#### Genetic interactions <a name="genint"></a>
+
+To download the file, execute the following command.
+
+    Genetic_interactions = Alleles_Stocks.Allele_genetic_interactions()
+ 
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|allele_symbol	|Current FlyBase allele symbol.|
+|allele_FBal#	|Current FlyBase identifier (FBal#) of allele.|
+|interaction	|Interaction information associated with allele.|
+|FBrf#	|Current FlyBase identifer (FBrf#) of publication from which data came.|
+
+
+#### Phenotypic data <a name="pheno"></a>
+
+To download the file, execute the following command.
+
+    Phenotypic_data = Alleles_Stocks.Phenotypic()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|genotype_symbols	|Current FlyBase symbol(s) of the components that make up the genotype.|
+|genotype_FBids	|Current FlyBase identifier(s) of the components that make up the genotype.|
+|phenotype_name	|Phenotypic name associated with the genotype.|
+|phenotype_id	|Phenotypic identifier associated with the genotype.|
+|qualifier_names	|Qualifier name(s) associated with phenotypic data for genotype.|
+|qualifier_ids	|Qualifier identifier(s) associated with phenotypic data for genotype.|
+|reference	|Current FlyBase identifer (FBrf#) of publication from which data came.|
+
+#### Alleles to Genes <a name="alltoge"></a>
+
+To download the file, execute the following command.
+
+    Alleles_toGenes = Alleles_Stocks.FBal_to_FBgn()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|AlleleID	|Current FlyBase identifier (FBal#) of the allele.|
+|AlleleSymbol	|Current symbol of the allele.|
+|GeneID	|Current FlyBase identifier (FBgn#) of the gene.|
+|GeneSymbol	|Current symbol of the gene.|
+
+## Homologs <a name="homs"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Homologs = FBD.Homologs
+
+Then, enter the specific method according to the desired data
+
+#### Drosophila Paralogs <a name="paral"></a>
+
+To download the file, execute the following command.
+
+    Dmel_Paralog = Homologs.Drosophila_Paralogs()
+
+Columns Description
+
+| Column heading           | Content Description          | 
+|----------------------|--------------------|
+|FBgn_ID	|Current FlyBase identifier (FBgn#) of the D. melanogaster gene.|
+|GeneSymbol	|Current FlyBase gene symbol of the D. melanogaster gene.|
+|Arm/Scaffold	|Arm upon which the D. melanogaster gene is localized.|
+|Location	|Location of D. melanogaster gene on the arm.|
+|Strand	|Strand of D. melanogaster gene ('1' indicates the positive strand, '-1' indicates the negative strand).|
+|Paralog_FBgn_ID	|Current FlyBase identifier (FBgn#) of the paralogous gene.|
+|Paralog_GeneSymbol	|Current FlyBase gene symbol of the paralogous gene.|
+|Paralog_Arm/Scaffold	|Arm upon which the paralogous gene is localized.|
+|Paralog_Location	|Location of paralogous gene on the arm.|
+|Paralog_Strand	|Strand of paralogous gene ('1' indicates the positive strand, '-1' indicates the negative strand).|
+|DIOPT_score	|DIOPT 'score' for the paralog call (i.e. the number of individual algorithms that support the call).|
+
+#### Human Orthologs <a name="hort-d"></a>
+
+To download the file, execute the following command.
+
+    Hman_Orthologs = Homologs.Human_Orthologs()
+ 
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|Dmel_gene_ID	|Current FlyBase identifier (FBgn#) of the D. melanogaster gene.|
+|Dmel_gene_symbol	|Current FlyBase gene symbol of the D. melanogaster gene.|
+|Human_gene_HGNC_ID	|HGNC ID of orthologous human gene.|
+|Human_gene_OMIM_ID	|OMIM ID of orthologous human gene.|
+|Human_gene_symbol	|HGNC gene symbol of orthologous human gene.|
+|DIOPT_score	|DIOPT 'score' for orthology call (i.e. the number of individual algorithms that support the call).|
+|OMIM_Phenotype_IDs	|OMIM Phenotype ID of orthologous human gene (comma separated values).|
+|OMIM_Phenotype_IDs[name]	|OMIM Phenotype ID of orthologous human gene (with the corresponding OMIM name in square brackets).| |Multiple phenotype[name] entries are separated by a comma.|
+
+
+## Human disease <a name="hudss"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Human_disease = FBD.Human_disease
+
+#### Human disease model data <a name="hdm"></a>
+
+To download the file, execute the following command.
+
+    Human_disease_model = Human_disease.Disease_model_annotations()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBgn ID	|Current FlyBase identifier (FBgn#) of the gene associated with the allele of an experimental annotation, or the D. melanogaster ortholog of a human gene associated with a disease in OMIM.|
+|Gene symbol	|Current FlyBase symbol of the gene in column 1.|
+HGNC ID	|HGNC ID of the gene identified in column 1 where it is a human gene (experimental-based annotations only).|
+|DO qualifier	|Type of association between the object of annotation and the disease - one of 'model of', 'ameliorates', 'exacerbates', 'DOES NOT model', 'DOES NOT ameliorate' or 'DOES NOT exacerbate'.|
+|DO ID	|Disease Ontology (DO) ID.|
+|DO term	|Disease Ontology (DO) term.|
+|Allele used in model (FBal ID)	|Current FlyBase identifier (FBal#) of allele (experimental-based annotations only).|
+|Allele used in model (symbol)	|Current FlyBase symbol of allele (experimental-based annotations only).|
+|Based on orthology with (HGNC ID)	|HGNC ID of the human ortholog used for annotations based on orthology to human disease genes.|
+|Based on orthology with (symbol)	|HGNC gene symbol of the human ortholog used for annotations based on orthology to human disease genes.|
+|Evidence/interacting alleles	|Evidence code, with interacting allele(s) where appropriate. For experimental-based annotations, the evidence code is one of: 'inferred from mutant phenotype', 'in combination with', 'modeled by', 'is ameliorated by', 'is exacerbated by', 'is NOT ameliorated by' or 'is NOT exacerbated by'. Interacting alleles are give as 'FLYBASE:<allele_symbol>; FB:<FBal_ID>', with multiple alleles separated by a comma. For orthology-based annotations, the evidence code is 'inferred from electronic annotation'.|
+|Reference (FBrf ID)	|Current FlyBase identifier (FBrf#) of the source publication.|
+
+#### Human orthologs <a name="hort-h"></a>
+
+To download the file, execute the following command.
+
+    Hman_Orthologs = Human_disease.Human_Orthologs()
+
+This is identical to the file of the same name listed under the 'Orthologs' section above.
+
+## Organisms <a name="orgs"></a>
+
+#### Species list <a name="species"></a>
+
+To download the file, execute the following command.
+
+    Species = FBD.Organisms.Species_list()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|Genus	|The genus designation of the organism.|
+|Species name	|The species designation of the organism.|
+|Abbreviation	|The standard FlyBase prefix for the species. This abbreviation is used in FlyBase as the first part of the symbol (before the '\') of any object, e.g. a gene or allele, that originates from this species. This column may be blank, if no individual report page exists for that species in FlyBase.|
+|Common name	|The NCBI Taxonomy Database common name of the organism. This column may be blank.|
+|Ncbi-taxon-id	|The NCBI Taxonomy Database Taxon ID for the organism. This column may be blank.|
+|drosophilid	|If the species is from the family Drosophilidae, this column is filled in with 'y'.|
+
+## Ontology Terms <a name="ont-tr"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Ontology = FBD.Ontology_Terms
+
+#### Fly anatomy <a name="f-bt-on"></a>
+
+
+    FBbt = Ontology.FBbt()
+
+#### Fly development <a name="f-dv-on"></a>
+
+
+    FBdv = Ontology.FBdv()
+
+#### Flybase controlled vocabulary <a name="f-cv-on"></a>
+
+
+    FBcv = Ontology.FBcv()
+
+#### Stock ontology <a name="f-sv-on"></a>
+
+
+    FBsv = Ontology.FBsv()
+
+#### Gene ontology <a name="f-go-on"></a>
+
+
+    GO = Ontology.G0()
+
+#### Image ontology <a name="f-bi-on"></a>
+
+
+    FBbi= Ontology.FBbi()
+
+#### Human disease ontology <a name="f-do-on"></a>
+
+
+    DO = Ontology.DO()
+
+## Insertions <a name="insr"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Insertions = FBD.Insertions
+
+#### Map data for insertions <a name="mp-insr"></a>
+
+   To download the file, execute the following command.
+
+    map_Insertions = Insertions.Map_insertions()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|insertion_symbol	|Current symbol of insertion.|
+|FBti#	|Current FlyBase identifier (FBti#) of insertion.|
+genomic_location	|Genomic location of insertion.|
+|range	|Range (t/f) indicates whether genomic location is range or single base|.
+|orientation	|Orientation (1/0) indicates orientation of insertion on chromosome.|
+|estimated_cytogenetic_location	|Estimated cytogenetic location based on correlation of genomic location and estimated genomic location of cytological bands.|
+|observed_cytogenetic_location	|Observed cytogenetic location reported in the literature.|
+
+
+#### Frequently-used GAL4 drivers <a name="gal4"></a>
+
+   To download the file, execute the following command.
+
+    Gal4 = Insertions.GAL4_drivers()
+
+This file reports a list of all GAL4 drivers that have been curated to at least 21 references and/or are among 150 most frequently requested GAL4 stocks from the [Bloomington Drosophila Stock Center](https://bdsc.indiana.edu/), in JSON format. In addition to the symbols and IDs for Scer\GAL4 alleles, this file also includes their associated transposon or insertion, associated gene, expression pattern in controlled vocabulary stage and anatomy terms, stocks, and publications, all with IDs, as well as free text expression pattern descriptions. This file, except for publications and stocks, is also available in TSV format [here](http://flybase.org/GAL4/freq_used_drivers.tsv).
+
+## Clones <a name="clones"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Clones = FBD.Clones
+
+#### cDNAs: FBcl to acc. ID <a name="dna-fbcl-acc"></a>
+
+   To download the file, execute the following command.
+
+    c_cDNAs = Clones.cDNA_clone_data()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBcl#	|Current FlyBase identifier (FBcl#) of cDNA clone.|
+organism_abbreviation	|Abbreviation (from the Species |Abbreviations list) indicating the species of origin of the clone.|
+|clone_name	|Clone name.|
+|dataset_metadata_name	|Name of dataset associated with clone.|
+|cDNA_accession(s)	|EMBL/GenBank/DDBJ cDNA accession number.|
+|EST_accession(s)	|EMBL/GenBank/DDBJ EST accession number.|
+
+#### Genomic: FBcl to acc. ID <a name="gen-fbcl-acc"></a>
+
+   To download the file, execute the following command.
+
+    c_genomic = Clones.genomic_clone_data()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBcl#	|Current FlyBase identifier (FBcl#) of genomic clone.|
+|organism_abbreviation	|Abbreviation (from the Species Abbreviations list) indicating the species of origin of the clone.|
+|clone_name	|Clone name.|
+|accession	|EMBL/GenBank/DDBJ cDNA accession number.|
+
+## References <a name="ref"></a>
+
+#### FlyBase FBrf to PubMed ID to PMCID to DOI <a name="ref-get"></a>
+
+   To download the file, execute the following command.
+
+    References = FBD.References.FBrf_PMid_PMCid_doi()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBrf	|The unique FlyBase ID for this publication.|
+|PMID	|The unique PubMed ID for this publication.|
+|PMCID	|The unique PubMed Central ID for this publication, if applicable.|
+|DOI	|The digital object identifier assigned to the publication.
+|pub_type	|The publication type (for example, paper, review, erratum, abstract, book, etc.)|
+|miniref	|A short citation listing the first author, year of publication, journal, volume, issue and page numbers.|
+|pmid_added	|The FlyBase release in which the publication was first incorporated into the FlyBase bibliography. Note: as this report first generated for fb_2012_01 release, all publications associated with a Pub Med ID prior to this release have pmid_added = fb_2011_10.|
+
+## Autor: 
+Javiera Quiroz, [email](javiera.quiroz@biomedica.udec.cl).
```

### Comparing `FlyBaseDownloads-1.0.5/FlyBaseDownloads.egg-info/SOURCES.txt` & `FlyBaseDownloads-1.0.6/FlyBaseDownloads.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.5/PKG-INFO` & `FlyBaseDownloads-1.0.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,89 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.5
+Version: 1.0.6
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
+
 # FlyBaseDownloads
 
 Python package to facilitate the data download from FlyBase. Most of the available data from their official wiki can be downloaded. One of the purposes of this library is to organize the data as closely as possible to the source, **FlyBase**. Despite not being the official package, it is organized by data class/type and provides direct downloads of the current bulk data files from the FTP site.
 For more information, visit the [official FlyBase wiki](https://wiki.flybase.org/wiki/FlyBase:Downloads_Overview).
 
+- [Usage and Installation](#usageninstallation)
+- [Synonyms](#synonyms)
+- [Genes](#genes)
+    - [Genetic interaction table](#git) 
+    - [RNA-Seq RPKM values](#rnaseq-v)
+    - [RNA-Seq RPKM values matrix](#rnaseq-m) 
+    - [Single Cell RNA-Seq Gene Expression](#single-cell)
+    - [Physical interaction MITAB file](#mitab)
+    - [Functional complementation table](#fct)
+    - [FBgn to DB Accession IDs](#fbgn-db)
+    - [FBgn to Annotation ID](#fbgn-ann)
+    - [FBgn to GLEANR IDs](#fbgn-gl)
+    - [FBgn to FBtr to FBpp IDs ](#fbgn-fbpp)
+    - [FBgn to FBtr to FBpp IDs (expanded)](#fbgn-fbpp-e)
+    - [FBgn exons to Affy1](#fbgn-af1)
+    - [FBgn exons to Affy2](#fbgn-af2)
+    - [Genes Sequence Ontology (SO) data](#go-gene)
+    - [Genes map table](#genes-map)
+    - [Best gene summaries](#bgs)
+    - [Automated gene summaries](#ags)
+    - [Gene Snapshots](#gss)
+    - [Unique protein isoforms](#upi)
+    - [Non-coding RNAs](#non-cod)
+    - [Enzyme](#enzyme)
+ - [Gene Ontology annotation files GO](#go-file)
+	  - [Gene Association File - GAF](#gaf) 
+ - [Gene Groups](#gene-groups)
+	  - [Gene group data](#ggd) 
+	  - [Gene groups with HGNC IDs](#hgnc) 
+	  - [Pathway group](#pathway) 
+ - [Alleles and Stocks](#aands)
+	  - [Stock](#stock)
+	  - [Genetic interactions](#genint)
+	  - [Phenotypic](#pheno) 
+	  - [Alleles to Genes](#alltoge)
+ - [Homologs](#homs)
+	  - [Drosophila Paralogs](#paral)
+	  - [Human Orthologs](#hort-d) 
+ - [Human disease](#hudss)
+	  - [Human disease model](#hdm) 
+	  - [Human Orthologs](#hort-h) 
+ - [Organisms](#orgs)
+	  - [Species list](#species) 
+ - [Ontology Terms](#ont-tr)
+	  - [Fly Anatomy](#f-bt-on)
+	  - [Fly Development](#f-dv-on)
+	  - [Flybase Controlled Vocabulary](#f-cv-on) 
+	  - [Fly Stock Ontology](#f-sv-on)
+	  - [Gene Ontology](#f-go-on)
+	  - [Image Ontology](#f-bi-on) 
+	  - [Human Disease Ontology](#f-do-on)
+ - [Insertions](#insr)
+	  - [Map data for insertions](#mp-insr)
+	  - [Frequently-used GAL4 drivers table](#gal4)
+ - [Clones](#clones)
+	  - [cDNAs: FBcl to acc. ID](#dna-fbcl-acc) 
+	  - [Genomic: FBcl to acc. ID](#gen-fbcl-acc) 
+ - [References](#ref)
+	  - [FlyBase FBrf to PubMed ID to PMCID to DOI](#ref-get) 
 
-# Bulk data files
+# Usage and Installation <a name="usageninstallation"></a>
 
 In order to simplify the download of FlyBase files, the names have been kept as close as possible. To access the data, follow these steps:
 
 1. Install the library using the pip command.
 
     > pip install FlyBaseDownloads
 
@@ -31,15 +91,15 @@
 
     > import FlyBaseDownloads as FBD
 
 3. Access the different classes of the library described below.
 
 
 
-## Synonyms
+## Synonyms <a name="synonyms"></a>
 
 To download the file, execute the following command.
 
     Synonyms = FBD.Synonyms.get()
 
 The file reports current symbols and synonyms for the following objects in FlyBase: genes (FBgn), alleles (FBal), balancers (FBba), aberrations (FBab), transgenic constructs (FBtp), insertions (FBti), transcripts (FBtr), and proteins (FBpp).
 
@@ -51,23 +111,23 @@
 | organism_abbreviation   | Abbreviation (from the Species Abbreviations list) indicating the species of origin |
 | current_symbol   | Current symbol used in FlyBase for the object |
 | current_fullname   | Current full name used in FlyBase for the object|
 | fullname_synonym(s)   | 	Non-current full name(s) associated with the object (pipe separated values) |
 | symbol_synonym(s)   | Non-current symbol(s) associated with the object (pipe separated values) |
 
 
-## Genes
+## Genes <a name="genes"></a>
 
 To facilitate its usage, it is suggested to access the data using the following command.
 
     Genes = FBD.Genes
 
 Then, enter the specific method according to the desired data
 
-#### Genetic interaction table
+#### Genetic interaction table <a name="git"></a>
 
 To download the file, execute the following command.
 
     Genetic_interaction_table = Genes.Genetic_interaction_table()
 
 Columns Description
 
@@ -77,15 +137,15 @@
 | Starting_gene(s)_FBgn | Current FlyBase identifier (FBgn#) of gene(s) involved in the starting genotype |
 | Interacting_gene(s)_symbol | Current FlyBase symbol of gene(s) involved in the interacting genotype |
 | Interacting_gene(s)_FBgn | Current FlyBase identifier (FBgn#) of gene(s) involved in the interacting genotype |
 | Interaction_type | Type of interaction observed, either 'suppressible' or 'enhanceable' |
 |Publication_FBrf | Current FlyBase identifier (FBrf#) of publication from which the data came |
 
 
-#### RNA-Seq RPKM values
+#### RNA-Seq RPKM values <a name="rnaseq-v"></a>
 
 To download the file, execute the following command.
 
     RNASeq_values = Genes.RNASeq_values()
 
 Columns Description
 
@@ -100,15 +160,15 @@
 | RNASource_name	| The official FlyBase symbol for the RNA-Seq experiment used for RPKM expression calculation |
 | RPKM_value	| The RPKM expression value for the gene in the specified RNA-Seq experiment |
 | Bin_value	| The expression bin classification of this gene in this RNA-Seq experiment, based on RPKM value. Bins range from 1 (no/extremely low expression) to 8 (extremely high expression)| 
 | Unique_exon_base_count	T| he number of exonic bases unique to the gene (not overlapping exons of other genes). Field will be blank for genes derived from dicistronic/polycistronic transcripts |
 | Total_exon_base_count	| The number of bases in all exons of this gene |
 | Count_used	| Indicates if the RPKM expression value was calculated using only the exonic regions unique to the gene and not overlapping exons of other genes (Unique), or, if the RPKM expression value was calculated based on all exons of the gene regardless of overlap with other genes (Total). RPKM expression values are typically reported for the "Unique" count, except for genes on dicistronic/polycistronic transcripts, in which case the "Total" count is reported |
 
-#### RNA-Seq RPKM values matrix
+#### RNA-Seq RPKM values matrix <a name="rnaseq-m"></a>
 
 To download the file, execute the following command.
 
     RNASeq_values_matrix = Genes.RNASeq_values_matrix()
 
 Columns Description
 
@@ -117,15 +177,15 @@
 | gene_primary_id	| The unique FlyBase gene ID for this gene.
 |gene_symbol	| The official FlyBase symbol for this gene.|
 | gene_fullname	| The official full name for this gene.|
 | gene_type	| The type of gene: e.g., protein_coding_gene, non_protein_coding_gene.|
 | DATASAMPLE_NAME_(DATASET_ID)	| Each subsequent column reports the gene RPKM values for the sample listed in the header. The dataset "FBlc" ID is listed in parentheses, and can be pasted into FlyBase search to access more information on the sample from the "dataset" report.|
 
 
-#### Single Cell RNA-Seq Gene Expression
+#### Single Cell RNA-Seq Gene Expression <a name="single-cell"></a>
 
 To download the file, execute the following command.
 
     SingleCellRNASeq_Gene_Expression = Genes.Single_Cell_RNA_Gene_Expression()
 
 Columns Description
 
@@ -143,51 +203,51 @@
 | Cluster_Cell_Type_ID	| The FlyBase FBbt ID for the cell type represented by the cell cluster.| 
 | Cluster_Cell_Type_Name	| The FlyBase name for the cell type represented by the cell cluster.| 
 | Gene_ID	| The FlyBase FBgn ID for the expressed gene.| 
 | Gene_Symbol	| The FlyBase symbol for the expressed gene (ASCII-format).|
 | Mean_Expression	| The average level of expression of the gene across all cells of the cluster in which the gene is detected at all.|
 | Spread	| The proportion of cells in the cluster in which the gene is detected.| 
 
-#### Physical interaction MITAB file
+#### Physical interaction MITAB file <a name="mitab"></a>
 
 To download the file, execute the following command.
 
     Physical_interaction_MITAB = Genes.Physical_interaction_MITAB()
 
 Columns Description
 
 | Column number	| Column heading	| General format	| FlyBase example	| Content description | 
 |----------------------|--------------------|----------------------|--------------------|----------------------|
 | 1 | ID(s) Interactor A                   | database:identifier            | flybase:FBgn0002121| The unique Flybase identifier for the first gene of the interacting pair.              |                           |
 | 2 | ID(s) Interactor B                   | -                              | -                  | The unique Flybase identifier for the second gene of the interacting pair.             |                           |
 | 3 | Alt ID(s) Interactor A               | database:identifier            | flybase:CG2671\| entrez gene/locuslink:33156 | The alternative gene identifiers currently provided are Flybase annotation IDs (CG#) and NCBI’s Entrez Gene ID separated by “\|“                           |
 | 4 | Alt ID(s) Interactor B               | -                              | -                  |                        -                          |
 | 5 | Alias(es) Interactor A               | database:name(alias type)      | flybase:l(2)gl(gene name) | The official Flybase gene symbol. It is referred to as “gene name” to adhere to the psi-mi ontology. |                           |
-| 6 | Alias(es) Interactor B               | -                              | ”-                  |                    -      |                       
+| 6 | Alias(es) Interactor B               | -                              | -                  |                    -      | 
 | 7 | Interaction Detection Method(s)      | ontology:identifier(method name) | psi-mi:"MI:0006"(anti bait coimmunoprecipitation) | The assay used to detect the interaction, taken from the psi-mi ontology. |                           |
 | 8 | Publication 1st Author(s)            | surname initial(s) (publication year) | Betschinger K. (2003) | The first author and year of the publication where the interaction is described. |                           |
 | 9 | Publication ID(s)                    | database:identifier            | flybase:FBrf0157155\|pubmed:12629552 | The unique FlyBase identifier for the publication followed by the unique PubMed identifier (if there is one) separated by “\|”. |                           |
 | 10| Taxid Interactor A                   | taxid:identifier               | taxid:7227("Drosophila melanogaster") | The NCBI taxonomy identifier for the source organism of the interactor. The vast majority of interactors in FlyBase come from D. melanogaster. There are, however, a few interspecies interactions consisting of a D. melanogaster interactor and an interactor of a different species. |                           |
-| 11| Taxid Interactor B                   | -                              | -                  |           -                |                           
+| 11| Taxid Interactor B                   | -                              | -                  |           -                | 
 | 12| Interaction Type(s)                  | ontology:identifier(interaction type) | psi-mi:"MI:0915"(physical association) | Taken from the psi-mi ontology. Most often “physical association” for FlyBase. |                           |
-| 13| Source Database(s)                   | ontology:identifier(database name) | psi-mi:"MI:0478"(flybase) | All interactions are curated by FlyBase. |                           
-| 14| Interaction Identifier(s)            | database:identifier            | flybase:FBrf0157155-13.coIP.WB | The unique FlyBase identifier for this interaction. |                                             
+| 13| Source Database(s)                   | ontology:identifier(database name) | psi-mi:"MI:0478"(flybase) | All interactions are curated by FlyBase. | 
+| 14| Interaction Identifier(s)            | database:identifier            | flybase:FBrf0157155-13.coIP.WB | The unique FlyBase identifier for this interaction. | 
 | 15	| Confidence Value(s) |	-|-|		Not applicable	
 | 16	| Expansion Method(s) |-|-| Not applicable
 | 17	| Biological Role(s)  Interactor A	| -|-|		Not applicable	
 | 18	| Biological Role(s) Interactor B	| -|-|		Not applicable	
 | 19	| Experimental Role(s) Interactor A	| ontology:identifier(experimental role name) |	psi-mi:"MI:0496"(bait)	| The role played by the interactor in the experiment. Taken from the psi-mi ontology.	|
 | 20	| Experimental Role(s) Interactor B | -|-|	-|	
 | 21	| Type(s) Interactor A |	ontology:identifier(interactor type name)	| psi-mi:"MI:0326"(protein)	| The molecule type. For FlyBase, these are limited to protein or ribonucleic acid. Taken from the psi-mi ontology.	|
-| 22	| Type(s) Interactor B	| -|-|-|		
+| 22	| Type(s) Interactor B	| -|-|-| 
 | 23	| Xref(s) Interactor A	|-|-|	Not applicable	
 | 24	| Xref(s) Interactor B	|	-|-|	Not applicable	
 | 25	| Interaction Xref(s) |	database:identifier	| flybase:FBig0000000103	| Cross references for the interactions. For Flybase, these include an interaction group identifier (FBig) and possibly a collection identifier (FBlc) separated by “\|”. All experiments that show an interaction between the products of gene A and gene B are compiled into an A-B interaction group, such that all interactions are associated with an interaction group identified by an FBig number. Interactions identified as part of a large scale study are also associated with the collection identifier, or FBlc number.	|
 | 26	| Annotation(s) Interactor A |	topic:text	isoform-| comment:a isoform	| Information on whether the interaction is specific to a particular interactor isoform.	
-| 27	| Annotation(s) Interactor B |	- | - | -| 	
+| 27	| Annotation(s) Interactor B |	- | - | -|
 | 28	| Interaction Annotation(s) |	topic:text	| comment:Phosphorylated isoforms of @l(2)gl@ are absent when @aPKC@ is knocked down by RNAi.	| Describes the source(s) of the interaction participants and includes free text comments about the interaction.	|
 | 29	| Host Organism(s)	|	- | - | Not applicable	|
 | 30	| Interaction Parameters  | - | -	|	Not applicable	|
 | 31	| Creation Date	| - | - |	Not applicable	|
 | 32	| Update Date	| - | - |		Not applicable	|
 | 33	| Checksum Interactor A	| - | -	|	Not applicable	|
 | 34	| Checksum Interactor B	| - | -	|	Not applicable	|
@@ -197,15 +257,15 @@
 | 38	| Feature(s) Interactor B	| -	| - | -|
 | 39	| Stoichiometry Interactor A |-|-| Not applicable	|
 | 40	| Stoichiometry Interactor B |-|-| Not applicable| 
 | 41	| Identification Method(s) Participant A	|-|-|	Not applicable| 
 | 42	| Identification Method(s) Participant B |-|-|	Not applicable| 
 
 
-#### Functional complementation table
+#### Functional complementation table <a name="fct"></a>
 
 To download the file, execute the following command.
 
     Functional_complementation = Genes.Functional_complementation()
 
 Columns Description
 
@@ -213,15 +273,15 @@
 |----------------------|--------------------|
 | Dmel gene (symbol)	|Current FlyBase symbol of Dmel gene.|
 | Dmel gene (FBgn)	| Current FlyBase identifier (FBgn#) of Dmel gene in column 1.|
 | Functionally complementing ortholog (symbol)	| Current FlyBase symbol of a non-Dmel ortholog of the Dmel gene in column 1 where this non-Dmel gene has been show to functionally complement the Dmel gene.|
 | Functionally complementing ortholog (FBgn#)	| Current FlyBase identifier (FBgn#) of a non-Dmel ortholog of the Dmel gene in column 1 where this non-Dmel gene has been show to functionally complement the Dmel gene.|
 | Supporting_FBrf	| Current FlyBase identifier (FBrf#) of the publication that provides support for the functional complementation statement (the publication that reported the suppression of a mutant phenotype of the Dmel gene by a transgenic construct/mutant allele of the non-Dmel ortholog).|
 
-#### FBgn to DB Accession IDs
+#### FBgn to DB Accession IDs <a name="fbgn-db"></a>
 
 To download the file, execute the following command.
 
     FBgn_toDB_Accession_IDs = Genes.FBgn_toDB_Accession_IDs()
 
 Columns Description
 
@@ -233,15 +293,15 @@
 nucleotide_accession	| EMBL/GenBank/DDBJ nucleotide accession associated with the gene.|
 | na_based_protein_accession	| EMBL/GenBank/DDBJ protein accession associated with the gene and the nucleotide accession in the preceeding 'nucleotide_accession' column|
 | UniprotKB/Swiss-Prot/TrEMBL_accession	| UniProtKB/SwissProt/TrEMBL protein accession associated with the gene.|
 |EntrezGene_ID	| NCBI Entrez ID associated with the gene.
 |RefSeq_transcripts	| NCBI RefSeq transcript accession associated with the gene.|
 RefSeq_proteins	| NCBI RefSeq protein accession associated with the gene and the transcript accession in the preceeding 'RefSeq_transcripts' column.|
 
-#### FBgn to Annotation ID
+#### FBgn to Annotation ID <a name="fbgn-ann"></a>
 
 To download the file, execute the following command.
 
     FBgn_toAnnotation_ID = Genes.FBgn_toAnnotation_ID()
 
 Columns Description
 
@@ -250,44 +310,44 @@
 | gene_symbol	| Current symbol of gene.|
 | organism_abbreviation	| Abbreviation (from the Species Abbreviations list) indicating the species of origin of the gene.|
 | primary_FBgn#	| Current FlyBase identifier (FBgn#) of gene.|
 | secondary_FBgn#(s)	| Secondary FlyBase identifier(s) (FBgn#) associated with the gene (comma separated values).| 
 | annotation_ID	| Current annotation identifier associated with the gene.|
 | secondary_annotation_ID(s)	|Secondary annotation identifier(s) associated with the gene (comma separated values).|
 
-#### FBgn to GLEANR IDs
+#### FBgn to GLEANR IDs <a name="fbgn-gl"></a>
 
 To download the file, execute the following command.
 
     FBgn_toGLEANR_IDs = Genes.FBgn_toGLEANR_IDs()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |organism_abbreviation	| Abbreviation (from the Species Abbreviations list) indicating the species of origin of the gene.|
 |gene_symbol	| Current FlyBase gene symbol.|
 |primary_FBgn#	| Current FlyBase identifier (FBgn#) of the gene.|
 |GLEANR_ID	| GLEANR identifier assigned by the AAA Consortium.|
 
-#### FBgn to FBtr to FBpp IDs
+#### FBgn to FBtr to FBpp IDs <a name="fbgn-fbpp"></a>
 
 To download the file, execute the following command.
 
     FBgn_to_FBtr_to_FBpp = Genes.FBgn_to_FBtr_to_FBpp()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FlyBase_FBgn	|Current FlyBase identifier (FBgn#) of the gene.|
 |FlyBase_FBtr	|Current FlyBase identifier (FBtr#) of a transcript encoded by the gene listed in the preceeding 'FlyBase_FBgn' column.|
 |FlyBase_FBpp	|Current FlyBase identifier (FBpp#) of a polypeptide encoded by the transcript listed in the preceeding 'FlyBase_FBtr' column, where this is relevant.|
 
-#### FBgn to FBtr to FBpp IDs (expanded)
+#### FBgn to FBtr to FBpp IDs (expanded) <a name="fbgn-fbpp-e"></a>
 
 To download the file, execute the following command.
 
     FBgn_to_FBtr_to_FBpp_exp = Genes.FBgn_to_FBtr_to_FBpp_expanded()
 
 Columns Description
 
@@ -301,15 +361,15 @@
 |annotation_ID	|Current FlyBase annotation identifier of the gene.|
 |transcript_type	|The type of transcript, represented by a Sequence Ontology term.|
 |transcript_ID	|Current FlyBase annotation identifier of the transcript.|
 |transcript_symbol	|Current symbol of the transcript.|
 |polypeptide_ID	|Current FlyBase annotation identifier of the polypeptide.|
 |polypeptide_symbol	|Current symbol of the polypeptide.|
 
-#### FBgn exons to Affy1 
+#### FBgn exons to Affy1 <a name="fbgn-af1"></a>
 
 To download the file, execute the following command.
 
     FBgn_exons2affy1 = Genes.FBgn_exons2affy1()
 
 The file is generated by testing for overlaps, no matter how small, of the locations of Affy1 oligos in the genome with the locations of gene exons, as defined by the Dmel gene models for the current release of FlyBase. If the location of an Affy1 oligo shows any kind of overlap with an exon of a gene, a Gene=>Affy reference is recorded in this file.
 
@@ -322,38 +382,38 @@
 
 it excludes:
  - genes not located to the sequence
  - mitochondrial genes
 
 The first column of a line it is the FBgn ID, and the second one is the Affy1 ID that overlaps with an exon of the gene.
 
-#### FBgn exons to Affy2
+#### FBgn exons to Affy2 <a name="fbgn-af2"></a>
 
 To download the file, execute the following command.
 
     FBgn_exons2affy2 = Genes.FBgn_exons2affy2()
 
 Similar to the Affy1 but with Affy2.
 
-#### Genes Sequence Ontology (SO) data
+#### Genes Sequence Ontology (SO) data <a name="go-gene"></a>
 
 To download the file, execute the following command.
 
     Genes_Sequence_Ontology = Genes.Genes_Sequence_Ontology()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |gene_primary_id	|The unique FlyBase gene ID for this gene.|
 |gene_symbol	|The official FlyBase symbol for this gene.|
 |so_term_name	|The SO term name.|
 |so_term_id	|The SO term primary identifier.|
 
-#### Genes map table
+#### Genes map table <a name="genes-map"></a>
 
 To download the file, execute the following command.
 
     Genes_map = Genes.Genes_map()
 
 Columns Description
 
@@ -362,43 +422,43 @@
 |organism_abbreviation	|Abbreviation (from the Species Abbreviations list) indicating the species of origin of the gene.|
 |current_symbol	|Current FlyBase gene symbol.|
 |primary_FBid	|Current FlyBase identifier (FBgn#) of gene.|
 |recombination_loc	|Recombination map location.|
 |cytogenetic_loc	|Cytogenetic location.|
 |sequence_loc	|Genomic location.|
 
-#### Best gene summaries
+#### Best gene summaries <a name="bgs"></a>
 
 To download the file, execute the following command.
 
     Best_gene_summaries = Genes.Best_gene_summaries()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FBgn_ID	|Current FlyBase identifier number for the gene.|
 |Gene_Symbol	|Current FlyBase symbol of the gene.|
 |Summary_Source	|The source of the gene summary.|
 |Summary	|The gene summary text.|
 
-### Automated_gene_summaries
+### Automated gene summaries <a name="ags"></a>
 
 To download the file, execute the following command.
 
 `Automated_gene_summaries = Genes.Automated_gene_summaries()`
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FlyBase ID. | The Valid FlyBase identifier number for the gene.|
 |Summary| The gene summary as a string of plain text.|
 
-#### Gene Snapshots
+#### Gene Snapshots <a name="gss"></a>
 
 To download the file, execute the following command.
 
     Gene_Snapshots = Genes.Gene_Snapshots()
 
 Columns Description
 
@@ -407,52 +467,458 @@
 |FBgn_ID	|Current FlyBase identifier number for the gene.|
 |GeneSymbol	|Current FlyBase symbol of the gene.|
 |GeneName	|Current FlyBase name of the gene.|
 |datestamp	|Date on which the information was last reviewed.|
 |gene_snapshot_text	| Gene snapshot information for the gene. Cases that are in progress or are deemed to have insufficient data to summarize are stated as such|
 
 
-#### Unique protein isoforms
+#### Unique protein isoforms <a name="upi"></a>
 
 To download the file, execute the following command.
 
     Unique_protein_isoforms = Genes.Unique_protein_isoforms()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FBgn	|Current FlyBase identifier (FBgn#) of the gene.|
 |FB_gene_symbol	|Current FlyBase gene symbol of the gene.|
 |representative_protein	|Current FlyBase protein symbol of the representative protein isoform.|
 |identical_protein(s)	|Current FlyBase protein symbol(s) of identical protein isoforms.|
 
-### Non-coding RNAs
+### Non-coding RNAs <a name="non-cod"></a>
 
 To download the file, execute the following command.
 
     Noncoding_RNAs = Genes.Noncoding_RNAs()
 
 This file reports all ncRNAs with gene models supported by FlyBase in JSON format, as submitted to [RNAcentral](http://rnacentral.org/). Pseudogenes are excluded. In addition to the symbols and IDs for ncRNAs, this file also includes their associated gene, genomic location, sequence, Sequence Ontology classification, etc.
 
 
-#### Enzyme data
+#### Enzyme data <a name="enzyme"></a>
 
 To download the file, execute the following command.
 
     Enzyme = Genes.Enzyme()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
-|group_id	|FlyBase gene group (FBgg) ID of the relevant terminal group within the ENZYMES (FBgg0001715) hierarchy (only terminal groups contain members).
+|group_id	|FlyBase gene group (FBgg) ID of the relevant terminal group within the ENZYMES (FBgg0001715) hierarchy (only terminal groups contain members).|
 |group_name	|FlyBase gene group (FBgg) name of relevant terminal group within the ENZYMES (FBgg0001715) hierarchy (only terminal groups contain members).|
 |group_GO_ID	|The GO molecular function term ID on the given gene group. Multiple entries are separated with a pipe.|
 |group_GO_name	|The GO molecular function term name on the given gene group. Multiple entries are separated with a pipe.|
 |group_EC_number	|The EC number on the given gene group, if present. (This is computed, corresponding to the EC cross-reference on the GO molecular function term.)|
 |group_EC_name	|The EC name on the given gene group, if present. (This is computed, corresponding to the EC cross-reference on the GO molecular function term.)|
 |gene_id	|The current FlyBase gene ID (FBgn) of the gene.|
 |gene_symbol	|The current FlyBase symbol of the gene.|
 |gene_name	|The current FlyBase name of the gene.|
-|gene_EC_number	|The EC number(s) associated with the gene, if present. Multiple entries are separated with a pipe. (This is computed, corresponding to the EC cross-reference(s) on any positive GO molecular function term(s) annotated to the gene.)
+|gene_EC_number	|The EC number(s) associated with the gene, if present. Multiple entries are separated with a pipe. (This is computed, corresponding to the EC cross-reference(s) on any positive GO molecular function term(s) annotated to the gene.)|
 |gene_EC_name	|The EC name(s) associated with the gene, if present. Multiple entries are separated with a pipe. (This is computed, corresponding to the EC cross-reference(s) on any positive GO molecular function term(s) annotated to the gene.)|
+
+## Gene Ontology annotation files <a name="go-file"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    GOAnn = FBD.GOAnn
+
+Then, enter the specific method according to the desired data
+
+#### Gene Association File - GAF <a name="gaf"></a>
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|DB	|The database contributing the gene_association file FB File: always "FB" for gene_association.fb.|
+|DB Object ID |A unique identifier in the database for the item being annotated. FB File: This is always the primary FlyBase identifier number for a Drosophila gene. Example: FBgn0000490|
+|DB Object Symbol |A (unique and valid) symbol to which the DB Object ID is matched. FB File: This is always the valid gene symbol for a Drosophila gene. Example: dpp|
+|Qualifier | For each GO annotation, one of the following as gene product to term relations are used: 'acts_upstream_of', 'acts_upstream_of_negative_effect', 'acts_upstream_of_positive_effect', 'colocalizes_with', 'contributes_to', 'enables', 'involved_in', 'is_active_in', 'located_in', 'part_of'. This column may also contain the 'NOT' qualifier, separated by a pipe (“\|”) from the gene product to term relation, which makes the annotation statement a negation. |
+|GO ID | The unique GO identifier for the GO term attributed to the DB_Object_ID. Example: GO:0005160|
+|DB:Reference | The unique identifier for the reference to which the GO annotation is attributed. FB File: Each FlyBase reference including published literature, conference abstracts, personal communications, sequence records and computer files has a unique 7 digit identifier (an FBrf). Where this reference is a published paper with a PubMed identifier, the PubMed ID is also listed in column 6, separated from the FBrf with a pipe (“\|”). Example: FB:FBrf0136863\|PMID:11432817 |
+|Evidence | The evidence code for the GO annotation; one of IMP, IGI, IPI, ISS, IDA, IEP, IEA, TAS, NAS, ND, IC, RCA, HDA, HMP, HGI, HEP, IBA|
+|With (or) From | FB File: This column contains the identifier for annotations where the evidence code is IGI, IPI, ISS, IEA or IC. For IGI the database gene symbol and identifier is listed. For ISS and IPI the identifier can be a gene symbol and identifier, or a sequence (protein or nucleic acid) identifier. For IC, the GO identifier of the term used as the basis of a curator inference is given. IGI example: FLYBASE:rpr; FB:FBgn0011706, ISS example: UniProt:P35569, ISS example: EMBL:AF064523, ISS example: SGD_LOCUS:COP1; SGD:S0002304, IC example: GO:0045298|
+|Aspect | Which ontology the GO term belongs to: Function ( F ), Process ( P ) or Component ( C ). Example: P| 
+|DB Object Name | FB File: The full name of the FlyBase gene. Example: decapentaplegic Where a FlyBase gene has no full name (eg Pten), this field is left blank.|
+|DB Object Synonym | Alternative names by which the database object is known. FB File: Multiple synonyms of a FlyBase gene are separated by a pipe (“\|”). Example: M(2)LS1\|shortvein\|Dm-DPP\|dpp\|Dpp\|DPP\|CG9885\|TGF-beta\|TGF-&bgr\|TGF-b\|Hin-d\|l(2)10638\|shv\|DPP-C\|ho\|M(2)23AB\|blk\|l(2)22Fa\|l(2)k17036\|Tg\|TGF&bgr |
+| DB Object Type |The type of object being annotated. Always a gene for FlyBase data. FB file: always "gene" for gene_association.fb.|
+|Taxon | The taxonomic identifier of the species encoding the gene product Example: taxon:7227|
+|Date|The date of last annotation update, in the format 'YYYYMMDD'. At present this date is the same for all annotations and corresponds to the date of the latest FlyBase update; we are in the process of changing our system so that dates more accurately reflect the date the annotation is made. Example: 20040821|
+|Assigned by |The source of the GO annotation.|
+
+## Gene groups <a name="gene-groups"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Gene_groups = FBD.Gene_groups
+
+Then, enter the specific method according to the desired data
+
+#### Gene group <a name="ggd"></a>
+
+To download the file, execute the following command.
+
+    Gene_groups_data = Gene_groups.Gene_group() 
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FB_group_id	|Current FlyBase identifier (FBgg##) of Gene Group.|
+|FB_group_symbol	|Current FlyBase symbol of Gene Group.|
+|FB_group_name	|Current FlyBase full name of Gene Group.|
+|Parent_FB_group_id	|Current FlyBase identifier (FBgg##) of parent of given Gene Group (if relevant).|
+|Parent_FB_group_symbol	|Current FlyBase symbol of parent of given Gene Group (if relevant).|
+|Group_member_FB_gene_id	|Current FlyBase identifier (FBgn##) of member gene (if terminal group).|
+|Group_member_FB_gene_symbol	|Current FlyBase symbol of member gene (if terminal group).|
+
+#### Gene groups with HGNC IDs  <a name="hgnc"></a>
+
+To download the file, execute the following command.
+
+    Gene_groups_HGNC= Gene_groups.Gene_groups_HGNC()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FB_group_id	|Current FlyBase identifier (FBgg##) of Gene Group.|
+|FB_group_symbol	|Current FlyBase symbol of Gene Group.|
+|FB_group_name	|Current FlyBase full name of Gene Group.|
+|HGNC_family_ID	|HGNC ID of equivalent human 'gene family'.|
+
+
+#### Pathway group <a name="pathway"></a>
+
+To download the file, execute the following command.
+
+    Pathway_group = Gene_groups.Pathway_group()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FB_group_id	|Current FlyBase identifier (FBgg##) of Pathway Gene Group.|
+|FB_group_symbol	|Current FlyBase symbol of Pathway Gene Group.|
+|FB_group_name	|Current FlyBase full name of Pathway Gene Group.|
+|Parent_FB_group_id	|Current FlyBase identifier (FBgg##) of parent of given Pathway Gene Group (if relevant).|
+|Parent_FB_group_symbol	|Current FlyBase symbol of parent of given Pathway Gene Group (if relevant).|
+|Group_member_FB_gene_id	|Current FlyBase identifier (FBgn##) of member gene (if terminal group).|
+|Group_member_FB_gene_symbol	|Current FlyBase symbol of member gene (if terminal group).|
+
+## Alleles and Stocks <a name="aands"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Alleles_Stocks = FBD.Alleles_Stocks
+
+Then, enter the specific method according to the desired data
+
+#### Stock data <a name="stock"></a>
+
+To download the file, execute the following command.
+
+    Stock = Alleles_Stocks.Stock()
+
+Columns Description
+
+| Column heading           | Content Description          | Example |
+|----------------------|--------------------|--------------------|
+|FBst	|The unique identifier assigned to this stock by FlyBase.|	FBst0000002|
+|collection_short_name	|A short name for the stock collection that holds the stock.	|Bloomington|
+|stock_type_cv	|The controlled vocabulary term and unique identifier that describe the state of the stock.|	living stock ; FBsv:0000002|
+|species	|Abbreviation (from the Species Abbreviations list) indicating the species of the stock.	|Dmel|
+|FB_genotype	|Genetic components of the stock corresponding to alleles, aberrations, balancers, or insertions in FlyBase. May be empty.|	w[*]; betaTub60D[2] Kr[If-1]/CyO|
+|description	|Genetic components of the stock as provided to FlyBase by the collection that holds the stock.	|FlyTrap: ZCL1796 III|
+|stock_number	|The stock identifier provided to FlyBase by the collection that holds the stock. May be empty.	|110818|
+
+#### Genetic interactions <a name="genint"></a>
+
+To download the file, execute the following command.
+
+    Genetic_interactions = Alleles_Stocks.Allele_genetic_interactions()
+ 
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|allele_symbol	|Current FlyBase allele symbol.|
+|allele_FBal#	|Current FlyBase identifier (FBal#) of allele.|
+|interaction	|Interaction information associated with allele.|
+|FBrf#	|Current FlyBase identifer (FBrf#) of publication from which data came.|
+
+
+#### Phenotypic data <a name="pheno"></a>
+
+To download the file, execute the following command.
+
+    Phenotypic_data = Alleles_Stocks.Phenotypic()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|genotype_symbols	|Current FlyBase symbol(s) of the components that make up the genotype.|
+|genotype_FBids	|Current FlyBase identifier(s) of the components that make up the genotype.|
+|phenotype_name	|Phenotypic name associated with the genotype.|
+|phenotype_id	|Phenotypic identifier associated with the genotype.|
+|qualifier_names	|Qualifier name(s) associated with phenotypic data for genotype.|
+|qualifier_ids	|Qualifier identifier(s) associated with phenotypic data for genotype.|
+|reference	|Current FlyBase identifer (FBrf#) of publication from which data came.|
+
+#### Alleles to Genes <a name="alltoge"></a>
+
+To download the file, execute the following command.
+
+    Alleles_toGenes = Alleles_Stocks.FBal_to_FBgn()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|AlleleID	|Current FlyBase identifier (FBal#) of the allele.|
+|AlleleSymbol	|Current symbol of the allele.|
+|GeneID	|Current FlyBase identifier (FBgn#) of the gene.|
+|GeneSymbol	|Current symbol of the gene.|
+
+## Homologs <a name="homs"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Homologs = FBD.Homologs
+
+Then, enter the specific method according to the desired data
+
+#### Drosophila Paralogs <a name="paral"></a>
+
+To download the file, execute the following command.
+
+    Dmel_Paralog = Homologs.Drosophila_Paralogs()
+
+Columns Description
+
+| Column heading           | Content Description          | 
+|----------------------|--------------------|
+|FBgn_ID	|Current FlyBase identifier (FBgn#) of the D. melanogaster gene.|
+|GeneSymbol	|Current FlyBase gene symbol of the D. melanogaster gene.|
+|Arm/Scaffold	|Arm upon which the D. melanogaster gene is localized.|
+|Location	|Location of D. melanogaster gene on the arm.|
+|Strand	|Strand of D. melanogaster gene ('1' indicates the positive strand, '-1' indicates the negative strand).|
+|Paralog_FBgn_ID	|Current FlyBase identifier (FBgn#) of the paralogous gene.|
+|Paralog_GeneSymbol	|Current FlyBase gene symbol of the paralogous gene.|
+|Paralog_Arm/Scaffold	|Arm upon which the paralogous gene is localized.|
+|Paralog_Location	|Location of paralogous gene on the arm.|
+|Paralog_Strand	|Strand of paralogous gene ('1' indicates the positive strand, '-1' indicates the negative strand).|
+|DIOPT_score	|DIOPT 'score' for the paralog call (i.e. the number of individual algorithms that support the call).|
+
+#### Human Orthologs <a name="hort-d"></a>
+
+To download the file, execute the following command.
+
+    Hman_Orthologs = Homologs.Human_Orthologs()
+ 
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|Dmel_gene_ID	|Current FlyBase identifier (FBgn#) of the D. melanogaster gene.|
+|Dmel_gene_symbol	|Current FlyBase gene symbol of the D. melanogaster gene.|
+|Human_gene_HGNC_ID	|HGNC ID of orthologous human gene.|
+|Human_gene_OMIM_ID	|OMIM ID of orthologous human gene.|
+|Human_gene_symbol	|HGNC gene symbol of orthologous human gene.|
+|DIOPT_score	|DIOPT 'score' for orthology call (i.e. the number of individual algorithms that support the call).|
+|OMIM_Phenotype_IDs	|OMIM Phenotype ID of orthologous human gene (comma separated values).|
+|OMIM_Phenotype_IDs[name]	|OMIM Phenotype ID of orthologous human gene (with the corresponding OMIM name in square brackets).| |Multiple phenotype[name] entries are separated by a comma.|
+
+
+## Human disease <a name="hudss"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Human_disease = FBD.Human_disease
+
+#### Human disease model data <a name="hdm"></a>
+
+To download the file, execute the following command.
+
+    Human_disease_model = Human_disease.Disease_model_annotations()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBgn ID	|Current FlyBase identifier (FBgn#) of the gene associated with the allele of an experimental annotation, or the D. melanogaster ortholog of a human gene associated with a disease in OMIM.|
+|Gene symbol	|Current FlyBase symbol of the gene in column 1.|
+HGNC ID	|HGNC ID of the gene identified in column 1 where it is a human gene (experimental-based annotations only).|
+|DO qualifier	|Type of association between the object of annotation and the disease - one of 'model of', 'ameliorates', 'exacerbates', 'DOES NOT model', 'DOES NOT ameliorate' or 'DOES NOT exacerbate'.|
+|DO ID	|Disease Ontology (DO) ID.|
+|DO term	|Disease Ontology (DO) term.|
+|Allele used in model (FBal ID)	|Current FlyBase identifier (FBal#) of allele (experimental-based annotations only).|
+|Allele used in model (symbol)	|Current FlyBase symbol of allele (experimental-based annotations only).|
+|Based on orthology with (HGNC ID)	|HGNC ID of the human ortholog used for annotations based on orthology to human disease genes.|
+|Based on orthology with (symbol)	|HGNC gene symbol of the human ortholog used for annotations based on orthology to human disease genes.|
+|Evidence/interacting alleles	|Evidence code, with interacting allele(s) where appropriate. For experimental-based annotations, the evidence code is one of: 'inferred from mutant phenotype', 'in combination with', 'modeled by', 'is ameliorated by', 'is exacerbated by', 'is NOT ameliorated by' or 'is NOT exacerbated by'. Interacting alleles are give as 'FLYBASE:<allele_symbol>; FB:<FBal_ID>', with multiple alleles separated by a comma. For orthology-based annotations, the evidence code is 'inferred from electronic annotation'.|
+|Reference (FBrf ID)	|Current FlyBase identifier (FBrf#) of the source publication.|
+
+#### Human orthologs <a name="hort-h"></a>
+
+To download the file, execute the following command.
+
+    Hman_Orthologs = Human_disease.Human_Orthologs()
+
+This is identical to the file of the same name listed under the 'Orthologs' section above.
+
+## Organisms <a name="orgs"></a>
+
+#### Species list <a name="species"></a>
+
+To download the file, execute the following command.
+
+    Species = FBD.Organisms.Species_list()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|Genus	|The genus designation of the organism.|
+|Species name	|The species designation of the organism.|
+|Abbreviation	|The standard FlyBase prefix for the species. This abbreviation is used in FlyBase as the first part of the symbol (before the '\') of any object, e.g. a gene or allele, that originates from this species. This column may be blank, if no individual report page exists for that species in FlyBase.|
+|Common name	|The NCBI Taxonomy Database common name of the organism. This column may be blank.|
+|Ncbi-taxon-id	|The NCBI Taxonomy Database Taxon ID for the organism. This column may be blank.|
+|drosophilid	|If the species is from the family Drosophilidae, this column is filled in with 'y'.|
+
+## Ontology Terms <a name="ont-tr"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Ontology = FBD.Ontology_Terms
+
+#### Fly anatomy <a name="f-bt-on"></a>
+
+
+    FBbt = Ontology.FBbt()
+
+#### Fly development <a name="f-dv-on"></a>
+
+
+    FBdv = Ontology.FBdv()
+
+#### Flybase controlled vocabulary <a name="f-cv-on"></a>
+
+
+    FBcv = Ontology.FBcv()
+
+#### Stock ontology <a name="f-sv-on"></a>
+
+
+    FBsv = Ontology.FBsv()
+
+#### Gene ontology <a name="f-go-on"></a>
+
+
+    GO = Ontology.G0()
+
+#### Image ontology <a name="f-bi-on"></a>
+
+
+    FBbi= Ontology.FBbi()
+
+#### Human disease ontology <a name="f-do-on"></a>
+
+
+    DO = Ontology.DO()
+
+## Insertions <a name="insr"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Insertions = FBD.Insertions
+
+#### Map data for insertions <a name="mp-insr"></a>
+
+   To download the file, execute the following command.
+
+    map_Insertions = Insertions.Map_insertions()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|insertion_symbol	|Current symbol of insertion.|
+|FBti#	|Current FlyBase identifier (FBti#) of insertion.|
+genomic_location	|Genomic location of insertion.|
+|range	|Range (t/f) indicates whether genomic location is range or single base|.
+|orientation	|Orientation (1/0) indicates orientation of insertion on chromosome.|
+|estimated_cytogenetic_location	|Estimated cytogenetic location based on correlation of genomic location and estimated genomic location of cytological bands.|
+|observed_cytogenetic_location	|Observed cytogenetic location reported in the literature.|
+
+
+#### Frequently-used GAL4 drivers <a name="gal4"></a>
+
+   To download the file, execute the following command.
+
+    Gal4 = Insertions.GAL4_drivers()
+
+This file reports a list of all GAL4 drivers that have been curated to at least 21 references and/or are among 150 most frequently requested GAL4 stocks from the [Bloomington Drosophila Stock Center](https://bdsc.indiana.edu/), in JSON format. In addition to the symbols and IDs for Scer\GAL4 alleles, this file also includes their associated transposon or insertion, associated gene, expression pattern in controlled vocabulary stage and anatomy terms, stocks, and publications, all with IDs, as well as free text expression pattern descriptions. This file, except for publications and stocks, is also available in TSV format [here](http://flybase.org/GAL4/freq_used_drivers.tsv).
+
+## Clones <a name="clones"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Clones = FBD.Clones
+
+#### cDNAs: FBcl to acc. ID <a name="dna-fbcl-acc"></a>
+
+   To download the file, execute the following command.
+
+    c_cDNAs = Clones.cDNA_clone_data()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBcl#	|Current FlyBase identifier (FBcl#) of cDNA clone.|
+organism_abbreviation	|Abbreviation (from the Species |Abbreviations list) indicating the species of origin of the clone.|
+|clone_name	|Clone name.|
+|dataset_metadata_name	|Name of dataset associated with clone.|
+|cDNA_accession(s)	|EMBL/GenBank/DDBJ cDNA accession number.|
+|EST_accession(s)	|EMBL/GenBank/DDBJ EST accession number.|
+
+#### Genomic: FBcl to acc. ID <a name="gen-fbcl-acc"></a>
+
+   To download the file, execute the following command.
+
+    c_genomic = Clones.genomic_clone_data()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBcl#	|Current FlyBase identifier (FBcl#) of genomic clone.|
+|organism_abbreviation	|Abbreviation (from the Species Abbreviations list) indicating the species of origin of the clone.|
+|clone_name	|Clone name.|
+|accession	|EMBL/GenBank/DDBJ cDNA accession number.|
+
+## References <a name="ref"></a>
+
+#### FlyBase FBrf to PubMed ID to PMCID to DOI <a name="ref-get"></a>
+
+   To download the file, execute the following command.
+
+    References = FBD.References.FBrf_PMid_PMCid_doi()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBrf	|The unique FlyBase ID for this publication.|
+|PMID	|The unique PubMed ID for this publication.|
+|PMCID	|The unique PubMed Central ID for this publication, if applicable.|
+|DOI	|The digital object identifier assigned to the publication.
+|pub_type	|The publication type (for example, paper, review, erratum, abstract, book, etc.)|
+|miniref	|A short citation listing the first author, year of publication, journal, volume, issue and page numbers.|
+|pmid_added	|The FlyBase release in which the publication was first incorporated into the FlyBase bibliography. Note: as this report first generated for fb_2012_01 release, all publications associated with a Pub Med ID prior to this release have pmid_added = fb_2011_10.|
+
+## Autor: 
+Javiera Quiroz, [email](javiera.quiroz@biomedica.udec.cl).
```

### Comparing `FlyBaseDownloads-1.0.5/README.md` & `FlyBaseDownloads-1.0.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,74 @@
+
 # FlyBaseDownloads
 
 Python package to facilitate the data download from FlyBase. Most of the available data from their official wiki can be downloaded. One of the purposes of this library is to organize the data as closely as possible to the source, **FlyBase**. Despite not being the official package, it is organized by data class/type and provides direct downloads of the current bulk data files from the FTP site.
 For more information, visit the [official FlyBase wiki](https://wiki.flybase.org/wiki/FlyBase:Downloads_Overview).
 
+- [Usage and Installation](#usageninstallation)
+- [Synonyms](#synonyms)
+- [Genes](#genes)
+    - [Genetic interaction table](#git) 
+    - [RNA-Seq RPKM values](#rnaseq-v)
+    - [RNA-Seq RPKM values matrix](#rnaseq-m) 
+    - [Single Cell RNA-Seq Gene Expression](#single-cell)
+    - [Physical interaction MITAB file](#mitab)
+    - [Functional complementation table](#fct)
+    - [FBgn to DB Accession IDs](#fbgn-db)
+    - [FBgn to Annotation ID](#fbgn-ann)
+    - [FBgn to GLEANR IDs](#fbgn-gl)
+    - [FBgn to FBtr to FBpp IDs ](#fbgn-fbpp)
+    - [FBgn to FBtr to FBpp IDs (expanded)](#fbgn-fbpp-e)
+    - [FBgn exons to Affy1](#fbgn-af1)
+    - [FBgn exons to Affy2](#fbgn-af2)
+    - [Genes Sequence Ontology (SO) data](#go-gene)
+    - [Genes map table](#genes-map)
+    - [Best gene summaries](#bgs)
+    - [Automated gene summaries](#ags)
+    - [Gene Snapshots](#gss)
+    - [Unique protein isoforms](#upi)
+    - [Non-coding RNAs](#non-cod)
+    - [Enzyme](#enzyme)
+ - [Gene Ontology annotation files GO](#go-file)
+	  - [Gene Association File - GAF](#gaf) 
+ - [Gene Groups](#gene-groups)
+	  - [Gene group data](#ggd) 
+	  - [Gene groups with HGNC IDs](#hgnc) 
+	  - [Pathway group](#pathway) 
+ - [Alleles and Stocks](#aands)
+	  - [Stock](#stock)
+	  - [Genetic interactions](#genint)
+	  - [Phenotypic](#pheno) 
+	  - [Alleles to Genes](#alltoge)
+ - [Homologs](#homs)
+	  - [Drosophila Paralogs](#paral)
+	  - [Human Orthologs](#hort-d) 
+ - [Human disease](#hudss)
+	  - [Human disease model](#hdm) 
+	  - [Human Orthologs](#hort-h) 
+ - [Organisms](#orgs)
+	  - [Species list](#species) 
+ - [Ontology Terms](#ont-tr)
+	  - [Fly Anatomy](#f-bt-on)
+	  - [Fly Development](#f-dv-on)
+	  - [Flybase Controlled Vocabulary](#f-cv-on) 
+	  - [Fly Stock Ontology](#f-sv-on)
+	  - [Gene Ontology](#f-go-on)
+	  - [Image Ontology](#f-bi-on) 
+	  - [Human Disease Ontology](#f-do-on)
+ - [Insertions](#insr)
+	  - [Map data for insertions](#mp-insr)
+	  - [Frequently-used GAL4 drivers table](#gal4)
+ - [Clones](#clones)
+	  - [cDNAs: FBcl to acc. ID](#dna-fbcl-acc) 
+	  - [Genomic: FBcl to acc. ID](#gen-fbcl-acc) 
+ - [References](#ref)
+	  - [FlyBase FBrf to PubMed ID to PMCID to DOI](#ref-get) 
 
-# Bulk data files
+# Usage and Installation <a name="usageninstallation"></a>
 
 In order to simplify the download of FlyBase files, the names have been kept as close as possible. To access the data, follow these steps:
 
 1. Install the library using the pip command.
 
     > pip install FlyBaseDownloads
 
@@ -16,15 +76,15 @@
 
     > import FlyBaseDownloads as FBD
 
 3. Access the different classes of the library described below.
 
 
 
-## Synonyms
+## Synonyms <a name="synonyms"></a>
 
 To download the file, execute the following command.
 
     Synonyms = FBD.Synonyms.get()
 
 The file reports current symbols and synonyms for the following objects in FlyBase: genes (FBgn), alleles (FBal), balancers (FBba), aberrations (FBab), transgenic constructs (FBtp), insertions (FBti), transcripts (FBtr), and proteins (FBpp).
 
@@ -36,23 +96,23 @@
 | organism_abbreviation   | Abbreviation (from the Species Abbreviations list) indicating the species of origin |
 | current_symbol   | Current symbol used in FlyBase for the object |
 | current_fullname   | Current full name used in FlyBase for the object|
 | fullname_synonym(s)   | 	Non-current full name(s) associated with the object (pipe separated values) |
 | symbol_synonym(s)   | Non-current symbol(s) associated with the object (pipe separated values) |
 
 
-## Genes
+## Genes <a name="genes"></a>
 
 To facilitate its usage, it is suggested to access the data using the following command.
 
     Genes = FBD.Genes
 
 Then, enter the specific method according to the desired data
 
-#### Genetic interaction table
+#### Genetic interaction table <a name="git"></a>
 
 To download the file, execute the following command.
 
     Genetic_interaction_table = Genes.Genetic_interaction_table()
 
 Columns Description
 
@@ -62,15 +122,15 @@
 | Starting_gene(s)_FBgn | Current FlyBase identifier (FBgn#) of gene(s) involved in the starting genotype |
 | Interacting_gene(s)_symbol | Current FlyBase symbol of gene(s) involved in the interacting genotype |
 | Interacting_gene(s)_FBgn | Current FlyBase identifier (FBgn#) of gene(s) involved in the interacting genotype |
 | Interaction_type | Type of interaction observed, either 'suppressible' or 'enhanceable' |
 |Publication_FBrf | Current FlyBase identifier (FBrf#) of publication from which the data came |
 
 
-#### RNA-Seq RPKM values
+#### RNA-Seq RPKM values <a name="rnaseq-v"></a>
 
 To download the file, execute the following command.
 
     RNASeq_values = Genes.RNASeq_values()
 
 Columns Description
 
@@ -85,15 +145,15 @@
 | RNASource_name	| The official FlyBase symbol for the RNA-Seq experiment used for RPKM expression calculation |
 | RPKM_value	| The RPKM expression value for the gene in the specified RNA-Seq experiment |
 | Bin_value	| The expression bin classification of this gene in this RNA-Seq experiment, based on RPKM value. Bins range from 1 (no/extremely low expression) to 8 (extremely high expression)| 
 | Unique_exon_base_count	T| he number of exonic bases unique to the gene (not overlapping exons of other genes). Field will be blank for genes derived from dicistronic/polycistronic transcripts |
 | Total_exon_base_count	| The number of bases in all exons of this gene |
 | Count_used	| Indicates if the RPKM expression value was calculated using only the exonic regions unique to the gene and not overlapping exons of other genes (Unique), or, if the RPKM expression value was calculated based on all exons of the gene regardless of overlap with other genes (Total). RPKM expression values are typically reported for the "Unique" count, except for genes on dicistronic/polycistronic transcripts, in which case the "Total" count is reported |
 
-#### RNA-Seq RPKM values matrix
+#### RNA-Seq RPKM values matrix <a name="rnaseq-m"></a>
 
 To download the file, execute the following command.
 
     RNASeq_values_matrix = Genes.RNASeq_values_matrix()
 
 Columns Description
 
@@ -102,15 +162,15 @@
 | gene_primary_id	| The unique FlyBase gene ID for this gene.
 |gene_symbol	| The official FlyBase symbol for this gene.|
 | gene_fullname	| The official full name for this gene.|
 | gene_type	| The type of gene: e.g., protein_coding_gene, non_protein_coding_gene.|
 | DATASAMPLE_NAME_(DATASET_ID)	| Each subsequent column reports the gene RPKM values for the sample listed in the header. The dataset "FBlc" ID is listed in parentheses, and can be pasted into FlyBase search to access more information on the sample from the "dataset" report.|
 
 
-#### Single Cell RNA-Seq Gene Expression
+#### Single Cell RNA-Seq Gene Expression <a name="single-cell"></a>
 
 To download the file, execute the following command.
 
     SingleCellRNASeq_Gene_Expression = Genes.Single_Cell_RNA_Gene_Expression()
 
 Columns Description
 
@@ -128,51 +188,51 @@
 | Cluster_Cell_Type_ID	| The FlyBase FBbt ID for the cell type represented by the cell cluster.| 
 | Cluster_Cell_Type_Name	| The FlyBase name for the cell type represented by the cell cluster.| 
 | Gene_ID	| The FlyBase FBgn ID for the expressed gene.| 
 | Gene_Symbol	| The FlyBase symbol for the expressed gene (ASCII-format).|
 | Mean_Expression	| The average level of expression of the gene across all cells of the cluster in which the gene is detected at all.|
 | Spread	| The proportion of cells in the cluster in which the gene is detected.| 
 
-#### Physical interaction MITAB file
+#### Physical interaction MITAB file <a name="mitab"></a>
 
 To download the file, execute the following command.
 
     Physical_interaction_MITAB = Genes.Physical_interaction_MITAB()
 
 Columns Description
 
 | Column number	| Column heading	| General format	| FlyBase example	| Content description | 
 |----------------------|--------------------|----------------------|--------------------|----------------------|
 | 1 | ID(s) Interactor A                   | database:identifier            | flybase:FBgn0002121| The unique Flybase identifier for the first gene of the interacting pair.              |                           |
 | 2 | ID(s) Interactor B                   | -                              | -                  | The unique Flybase identifier for the second gene of the interacting pair.             |                           |
 | 3 | Alt ID(s) Interactor A               | database:identifier            | flybase:CG2671\| entrez gene/locuslink:33156 | The alternative gene identifiers currently provided are Flybase annotation IDs (CG#) and NCBI’s Entrez Gene ID separated by “\|“                           |
 | 4 | Alt ID(s) Interactor B               | -                              | -                  |                        -                          |
 | 5 | Alias(es) Interactor A               | database:name(alias type)      | flybase:l(2)gl(gene name) | The official Flybase gene symbol. It is referred to as “gene name” to adhere to the psi-mi ontology. |                           |
-| 6 | Alias(es) Interactor B               | -                              | ”-                  |                    -      |                       
+| 6 | Alias(es) Interactor B               | -                              | -                  |                    -      | 
 | 7 | Interaction Detection Method(s)      | ontology:identifier(method name) | psi-mi:"MI:0006"(anti bait coimmunoprecipitation) | The assay used to detect the interaction, taken from the psi-mi ontology. |                           |
 | 8 | Publication 1st Author(s)            | surname initial(s) (publication year) | Betschinger K. (2003) | The first author and year of the publication where the interaction is described. |                           |
 | 9 | Publication ID(s)                    | database:identifier            | flybase:FBrf0157155\|pubmed:12629552 | The unique FlyBase identifier for the publication followed by the unique PubMed identifier (if there is one) separated by “\|”. |                           |
 | 10| Taxid Interactor A                   | taxid:identifier               | taxid:7227("Drosophila melanogaster") | The NCBI taxonomy identifier for the source organism of the interactor. The vast majority of interactors in FlyBase come from D. melanogaster. There are, however, a few interspecies interactions consisting of a D. melanogaster interactor and an interactor of a different species. |                           |
-| 11| Taxid Interactor B                   | -                              | -                  |           -                |                           
+| 11| Taxid Interactor B                   | -                              | -                  |           -                | 
 | 12| Interaction Type(s)                  | ontology:identifier(interaction type) | psi-mi:"MI:0915"(physical association) | Taken from the psi-mi ontology. Most often “physical association” for FlyBase. |                           |
-| 13| Source Database(s)                   | ontology:identifier(database name) | psi-mi:"MI:0478"(flybase) | All interactions are curated by FlyBase. |                           
-| 14| Interaction Identifier(s)            | database:identifier            | flybase:FBrf0157155-13.coIP.WB | The unique FlyBase identifier for this interaction. |                                             
+| 13| Source Database(s)                   | ontology:identifier(database name) | psi-mi:"MI:0478"(flybase) | All interactions are curated by FlyBase. | 
+| 14| Interaction Identifier(s)            | database:identifier            | flybase:FBrf0157155-13.coIP.WB | The unique FlyBase identifier for this interaction. | 
 | 15	| Confidence Value(s) |	-|-|		Not applicable	
 | 16	| Expansion Method(s) |-|-| Not applicable
 | 17	| Biological Role(s)  Interactor A	| -|-|		Not applicable	
 | 18	| Biological Role(s) Interactor B	| -|-|		Not applicable	
 | 19	| Experimental Role(s) Interactor A	| ontology:identifier(experimental role name) |	psi-mi:"MI:0496"(bait)	| The role played by the interactor in the experiment. Taken from the psi-mi ontology.	|
 | 20	| Experimental Role(s) Interactor B | -|-|	-|	
 | 21	| Type(s) Interactor A |	ontology:identifier(interactor type name)	| psi-mi:"MI:0326"(protein)	| The molecule type. For FlyBase, these are limited to protein or ribonucleic acid. Taken from the psi-mi ontology.	|
-| 22	| Type(s) Interactor B	| -|-|-|		
+| 22	| Type(s) Interactor B	| -|-|-| 
 | 23	| Xref(s) Interactor A	|-|-|	Not applicable	
 | 24	| Xref(s) Interactor B	|	-|-|	Not applicable	
 | 25	| Interaction Xref(s) |	database:identifier	| flybase:FBig0000000103	| Cross references for the interactions. For Flybase, these include an interaction group identifier (FBig) and possibly a collection identifier (FBlc) separated by “\|”. All experiments that show an interaction between the products of gene A and gene B are compiled into an A-B interaction group, such that all interactions are associated with an interaction group identified by an FBig number. Interactions identified as part of a large scale study are also associated with the collection identifier, or FBlc number.	|
 | 26	| Annotation(s) Interactor A |	topic:text	isoform-| comment:a isoform	| Information on whether the interaction is specific to a particular interactor isoform.	
-| 27	| Annotation(s) Interactor B |	- | - | -| 	
+| 27	| Annotation(s) Interactor B |	- | - | -|
 | 28	| Interaction Annotation(s) |	topic:text	| comment:Phosphorylated isoforms of @l(2)gl@ are absent when @aPKC@ is knocked down by RNAi.	| Describes the source(s) of the interaction participants and includes free text comments about the interaction.	|
 | 29	| Host Organism(s)	|	- | - | Not applicable	|
 | 30	| Interaction Parameters  | - | -	|	Not applicable	|
 | 31	| Creation Date	| - | - |	Not applicable	|
 | 32	| Update Date	| - | - |		Not applicable	|
 | 33	| Checksum Interactor A	| - | -	|	Not applicable	|
 | 34	| Checksum Interactor B	| - | -	|	Not applicable	|
@@ -182,15 +242,15 @@
 | 38	| Feature(s) Interactor B	| -	| - | -|
 | 39	| Stoichiometry Interactor A |-|-| Not applicable	|
 | 40	| Stoichiometry Interactor B |-|-| Not applicable| 
 | 41	| Identification Method(s) Participant A	|-|-|	Not applicable| 
 | 42	| Identification Method(s) Participant B |-|-|	Not applicable| 
 
 
-#### Functional complementation table
+#### Functional complementation table <a name="fct"></a>
 
 To download the file, execute the following command.
 
     Functional_complementation = Genes.Functional_complementation()
 
 Columns Description
 
@@ -198,15 +258,15 @@
 |----------------------|--------------------|
 | Dmel gene (symbol)	|Current FlyBase symbol of Dmel gene.|
 | Dmel gene (FBgn)	| Current FlyBase identifier (FBgn#) of Dmel gene in column 1.|
 | Functionally complementing ortholog (symbol)	| Current FlyBase symbol of a non-Dmel ortholog of the Dmel gene in column 1 where this non-Dmel gene has been show to functionally complement the Dmel gene.|
 | Functionally complementing ortholog (FBgn#)	| Current FlyBase identifier (FBgn#) of a non-Dmel ortholog of the Dmel gene in column 1 where this non-Dmel gene has been show to functionally complement the Dmel gene.|
 | Supporting_FBrf	| Current FlyBase identifier (FBrf#) of the publication that provides support for the functional complementation statement (the publication that reported the suppression of a mutant phenotype of the Dmel gene by a transgenic construct/mutant allele of the non-Dmel ortholog).|
 
-#### FBgn to DB Accession IDs
+#### FBgn to DB Accession IDs <a name="fbgn-db"></a>
 
 To download the file, execute the following command.
 
     FBgn_toDB_Accession_IDs = Genes.FBgn_toDB_Accession_IDs()
 
 Columns Description
 
@@ -218,15 +278,15 @@
 nucleotide_accession	| EMBL/GenBank/DDBJ nucleotide accession associated with the gene.|
 | na_based_protein_accession	| EMBL/GenBank/DDBJ protein accession associated with the gene and the nucleotide accession in the preceeding 'nucleotide_accession' column|
 | UniprotKB/Swiss-Prot/TrEMBL_accession	| UniProtKB/SwissProt/TrEMBL protein accession associated with the gene.|
 |EntrezGene_ID	| NCBI Entrez ID associated with the gene.
 |RefSeq_transcripts	| NCBI RefSeq transcript accession associated with the gene.|
 RefSeq_proteins	| NCBI RefSeq protein accession associated with the gene and the transcript accession in the preceeding 'RefSeq_transcripts' column.|
 
-#### FBgn to Annotation ID
+#### FBgn to Annotation ID <a name="fbgn-ann"></a>
 
 To download the file, execute the following command.
 
     FBgn_toAnnotation_ID = Genes.FBgn_toAnnotation_ID()
 
 Columns Description
 
@@ -235,44 +295,44 @@
 | gene_symbol	| Current symbol of gene.|
 | organism_abbreviation	| Abbreviation (from the Species Abbreviations list) indicating the species of origin of the gene.|
 | primary_FBgn#	| Current FlyBase identifier (FBgn#) of gene.|
 | secondary_FBgn#(s)	| Secondary FlyBase identifier(s) (FBgn#) associated with the gene (comma separated values).| 
 | annotation_ID	| Current annotation identifier associated with the gene.|
 | secondary_annotation_ID(s)	|Secondary annotation identifier(s) associated with the gene (comma separated values).|
 
-#### FBgn to GLEANR IDs
+#### FBgn to GLEANR IDs <a name="fbgn-gl"></a>
 
 To download the file, execute the following command.
 
     FBgn_toGLEANR_IDs = Genes.FBgn_toGLEANR_IDs()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |organism_abbreviation	| Abbreviation (from the Species Abbreviations list) indicating the species of origin of the gene.|
 |gene_symbol	| Current FlyBase gene symbol.|
 |primary_FBgn#	| Current FlyBase identifier (FBgn#) of the gene.|
 |GLEANR_ID	| GLEANR identifier assigned by the AAA Consortium.|
 
-#### FBgn to FBtr to FBpp IDs
+#### FBgn to FBtr to FBpp IDs <a name="fbgn-fbpp"></a>
 
 To download the file, execute the following command.
 
     FBgn_to_FBtr_to_FBpp = Genes.FBgn_to_FBtr_to_FBpp()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FlyBase_FBgn	|Current FlyBase identifier (FBgn#) of the gene.|
 |FlyBase_FBtr	|Current FlyBase identifier (FBtr#) of a transcript encoded by the gene listed in the preceeding 'FlyBase_FBgn' column.|
 |FlyBase_FBpp	|Current FlyBase identifier (FBpp#) of a polypeptide encoded by the transcript listed in the preceeding 'FlyBase_FBtr' column, where this is relevant.|
 
-#### FBgn to FBtr to FBpp IDs (expanded)
+#### FBgn to FBtr to FBpp IDs (expanded) <a name="fbgn-fbpp-e"></a>
 
 To download the file, execute the following command.
 
     FBgn_to_FBtr_to_FBpp_exp = Genes.FBgn_to_FBtr_to_FBpp_expanded()
 
 Columns Description
 
@@ -286,15 +346,15 @@
 |annotation_ID	|Current FlyBase annotation identifier of the gene.|
 |transcript_type	|The type of transcript, represented by a Sequence Ontology term.|
 |transcript_ID	|Current FlyBase annotation identifier of the transcript.|
 |transcript_symbol	|Current symbol of the transcript.|
 |polypeptide_ID	|Current FlyBase annotation identifier of the polypeptide.|
 |polypeptide_symbol	|Current symbol of the polypeptide.|
 
-#### FBgn exons to Affy1 
+#### FBgn exons to Affy1 <a name="fbgn-af1"></a>
 
 To download the file, execute the following command.
 
     FBgn_exons2affy1 = Genes.FBgn_exons2affy1()
 
 The file is generated by testing for overlaps, no matter how small, of the locations of Affy1 oligos in the genome with the locations of gene exons, as defined by the Dmel gene models for the current release of FlyBase. If the location of an Affy1 oligo shows any kind of overlap with an exon of a gene, a Gene=>Affy reference is recorded in this file.
 
@@ -307,38 +367,38 @@
 
 it excludes:
  - genes not located to the sequence
  - mitochondrial genes
 
 The first column of a line it is the FBgn ID, and the second one is the Affy1 ID that overlaps with an exon of the gene.
 
-#### FBgn exons to Affy2
+#### FBgn exons to Affy2 <a name="fbgn-af2"></a>
 
 To download the file, execute the following command.
 
     FBgn_exons2affy2 = Genes.FBgn_exons2affy2()
 
 Similar to the Affy1 but with Affy2.
 
-#### Genes Sequence Ontology (SO) data
+#### Genes Sequence Ontology (SO) data <a name="go-gene"></a>
 
 To download the file, execute the following command.
 
     Genes_Sequence_Ontology = Genes.Genes_Sequence_Ontology()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |gene_primary_id	|The unique FlyBase gene ID for this gene.|
 |gene_symbol	|The official FlyBase symbol for this gene.|
 |so_term_name	|The SO term name.|
 |so_term_id	|The SO term primary identifier.|
 
-#### Genes map table
+#### Genes map table <a name="genes-map"></a>
 
 To download the file, execute the following command.
 
     Genes_map = Genes.Genes_map()
 
 Columns Description
 
@@ -347,43 +407,43 @@
 |organism_abbreviation	|Abbreviation (from the Species Abbreviations list) indicating the species of origin of the gene.|
 |current_symbol	|Current FlyBase gene symbol.|
 |primary_FBid	|Current FlyBase identifier (FBgn#) of gene.|
 |recombination_loc	|Recombination map location.|
 |cytogenetic_loc	|Cytogenetic location.|
 |sequence_loc	|Genomic location.|
 
-#### Best gene summaries
+#### Best gene summaries <a name="bgs"></a>
 
 To download the file, execute the following command.
 
     Best_gene_summaries = Genes.Best_gene_summaries()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FBgn_ID	|Current FlyBase identifier number for the gene.|
 |Gene_Symbol	|Current FlyBase symbol of the gene.|
 |Summary_Source	|The source of the gene summary.|
 |Summary	|The gene summary text.|
 
-### Automated_gene_summaries
+### Automated gene summaries <a name="ags"></a>
 
 To download the file, execute the following command.
 
 `Automated_gene_summaries = Genes.Automated_gene_summaries()`
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FlyBase ID. | The Valid FlyBase identifier number for the gene.|
 |Summary| The gene summary as a string of plain text.|
 
-#### Gene Snapshots
+#### Gene Snapshots <a name="gss"></a>
 
 To download the file, execute the following command.
 
     Gene_Snapshots = Genes.Gene_Snapshots()
 
 Columns Description
 
@@ -392,52 +452,458 @@
 |FBgn_ID	|Current FlyBase identifier number for the gene.|
 |GeneSymbol	|Current FlyBase symbol of the gene.|
 |GeneName	|Current FlyBase name of the gene.|
 |datestamp	|Date on which the information was last reviewed.|
 |gene_snapshot_text	| Gene snapshot information for the gene. Cases that are in progress or are deemed to have insufficient data to summarize are stated as such|
 
 
-#### Unique protein isoforms
+#### Unique protein isoforms <a name="upi"></a>
 
 To download the file, execute the following command.
 
     Unique_protein_isoforms = Genes.Unique_protein_isoforms()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
 |FBgn	|Current FlyBase identifier (FBgn#) of the gene.|
 |FB_gene_symbol	|Current FlyBase gene symbol of the gene.|
 |representative_protein	|Current FlyBase protein symbol of the representative protein isoform.|
 |identical_protein(s)	|Current FlyBase protein symbol(s) of identical protein isoforms.|
 
-### Non-coding RNAs
+### Non-coding RNAs <a name="non-cod"></a>
 
 To download the file, execute the following command.
 
     Noncoding_RNAs = Genes.Noncoding_RNAs()
 
 This file reports all ncRNAs with gene models supported by FlyBase in JSON format, as submitted to [RNAcentral](http://rnacentral.org/). Pseudogenes are excluded. In addition to the symbols and IDs for ncRNAs, this file also includes their associated gene, genomic location, sequence, Sequence Ontology classification, etc.
 
 
-#### Enzyme data
+#### Enzyme data <a name="enzyme"></a>
 
 To download the file, execute the following command.
 
     Enzyme = Genes.Enzyme()
 
 Columns Description
 
 | Column heading           | Content Description          |
 |----------------------|--------------------|
-|group_id	|FlyBase gene group (FBgg) ID of the relevant terminal group within the ENZYMES (FBgg0001715) hierarchy (only terminal groups contain members).
+|group_id	|FlyBase gene group (FBgg) ID of the relevant terminal group within the ENZYMES (FBgg0001715) hierarchy (only terminal groups contain members).|
 |group_name	|FlyBase gene group (FBgg) name of relevant terminal group within the ENZYMES (FBgg0001715) hierarchy (only terminal groups contain members).|
 |group_GO_ID	|The GO molecular function term ID on the given gene group. Multiple entries are separated with a pipe.|
 |group_GO_name	|The GO molecular function term name on the given gene group. Multiple entries are separated with a pipe.|
 |group_EC_number	|The EC number on the given gene group, if present. (This is computed, corresponding to the EC cross-reference on the GO molecular function term.)|
 |group_EC_name	|The EC name on the given gene group, if present. (This is computed, corresponding to the EC cross-reference on the GO molecular function term.)|
 |gene_id	|The current FlyBase gene ID (FBgn) of the gene.|
 |gene_symbol	|The current FlyBase symbol of the gene.|
 |gene_name	|The current FlyBase name of the gene.|
-|gene_EC_number	|The EC number(s) associated with the gene, if present. Multiple entries are separated with a pipe. (This is computed, corresponding to the EC cross-reference(s) on any positive GO molecular function term(s) annotated to the gene.)
+|gene_EC_number	|The EC number(s) associated with the gene, if present. Multiple entries are separated with a pipe. (This is computed, corresponding to the EC cross-reference(s) on any positive GO molecular function term(s) annotated to the gene.)|
 |gene_EC_name	|The EC name(s) associated with the gene, if present. Multiple entries are separated with a pipe. (This is computed, corresponding to the EC cross-reference(s) on any positive GO molecular function term(s) annotated to the gene.)|
+
+## Gene Ontology annotation files <a name="go-file"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    GOAnn = FBD.GOAnn
+
+Then, enter the specific method according to the desired data
+
+#### Gene Association File - GAF <a name="gaf"></a>
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|DB	|The database contributing the gene_association file FB File: always "FB" for gene_association.fb.|
+|DB Object ID |A unique identifier in the database for the item being annotated. FB File: This is always the primary FlyBase identifier number for a Drosophila gene. Example: FBgn0000490|
+|DB Object Symbol |A (unique and valid) symbol to which the DB Object ID is matched. FB File: This is always the valid gene symbol for a Drosophila gene. Example: dpp|
+|Qualifier | For each GO annotation, one of the following as gene product to term relations are used: 'acts_upstream_of', 'acts_upstream_of_negative_effect', 'acts_upstream_of_positive_effect', 'colocalizes_with', 'contributes_to', 'enables', 'involved_in', 'is_active_in', 'located_in', 'part_of'. This column may also contain the 'NOT' qualifier, separated by a pipe (“\|”) from the gene product to term relation, which makes the annotation statement a negation. |
+|GO ID | The unique GO identifier for the GO term attributed to the DB_Object_ID. Example: GO:0005160|
+|DB:Reference | The unique identifier for the reference to which the GO annotation is attributed. FB File: Each FlyBase reference including published literature, conference abstracts, personal communications, sequence records and computer files has a unique 7 digit identifier (an FBrf). Where this reference is a published paper with a PubMed identifier, the PubMed ID is also listed in column 6, separated from the FBrf with a pipe (“\|”). Example: FB:FBrf0136863\|PMID:11432817 |
+|Evidence | The evidence code for the GO annotation; one of IMP, IGI, IPI, ISS, IDA, IEP, IEA, TAS, NAS, ND, IC, RCA, HDA, HMP, HGI, HEP, IBA|
+|With (or) From | FB File: This column contains the identifier for annotations where the evidence code is IGI, IPI, ISS, IEA or IC. For IGI the database gene symbol and identifier is listed. For ISS and IPI the identifier can be a gene symbol and identifier, or a sequence (protein or nucleic acid) identifier. For IC, the GO identifier of the term used as the basis of a curator inference is given. IGI example: FLYBASE:rpr; FB:FBgn0011706, ISS example: UniProt:P35569, ISS example: EMBL:AF064523, ISS example: SGD_LOCUS:COP1; SGD:S0002304, IC example: GO:0045298|
+|Aspect | Which ontology the GO term belongs to: Function ( F ), Process ( P ) or Component ( C ). Example: P| 
+|DB Object Name | FB File: The full name of the FlyBase gene. Example: decapentaplegic Where a FlyBase gene has no full name (eg Pten), this field is left blank.|
+|DB Object Synonym | Alternative names by which the database object is known. FB File: Multiple synonyms of a FlyBase gene are separated by a pipe (“\|”). Example: M(2)LS1\|shortvein\|Dm-DPP\|dpp\|Dpp\|DPP\|CG9885\|TGF-beta\|TGF-&bgr\|TGF-b\|Hin-d\|l(2)10638\|shv\|DPP-C\|ho\|M(2)23AB\|blk\|l(2)22Fa\|l(2)k17036\|Tg\|TGF&bgr |
+| DB Object Type |The type of object being annotated. Always a gene for FlyBase data. FB file: always "gene" for gene_association.fb.|
+|Taxon | The taxonomic identifier of the species encoding the gene product Example: taxon:7227|
+|Date|The date of last annotation update, in the format 'YYYYMMDD'. At present this date is the same for all annotations and corresponds to the date of the latest FlyBase update; we are in the process of changing our system so that dates more accurately reflect the date the annotation is made. Example: 20040821|
+|Assigned by |The source of the GO annotation.|
+
+## Gene groups <a name="gene-groups"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Gene_groups = FBD.Gene_groups
+
+Then, enter the specific method according to the desired data
+
+#### Gene group <a name="ggd"></a>
+
+To download the file, execute the following command.
+
+    Gene_groups_data = Gene_groups.Gene_group() 
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FB_group_id	|Current FlyBase identifier (FBgg##) of Gene Group.|
+|FB_group_symbol	|Current FlyBase symbol of Gene Group.|
+|FB_group_name	|Current FlyBase full name of Gene Group.|
+|Parent_FB_group_id	|Current FlyBase identifier (FBgg##) of parent of given Gene Group (if relevant).|
+|Parent_FB_group_symbol	|Current FlyBase symbol of parent of given Gene Group (if relevant).|
+|Group_member_FB_gene_id	|Current FlyBase identifier (FBgn##) of member gene (if terminal group).|
+|Group_member_FB_gene_symbol	|Current FlyBase symbol of member gene (if terminal group).|
+
+#### Gene groups with HGNC IDs  <a name="hgnc"></a>
+
+To download the file, execute the following command.
+
+    Gene_groups_HGNC= Gene_groups.Gene_groups_HGNC()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FB_group_id	|Current FlyBase identifier (FBgg##) of Gene Group.|
+|FB_group_symbol	|Current FlyBase symbol of Gene Group.|
+|FB_group_name	|Current FlyBase full name of Gene Group.|
+|HGNC_family_ID	|HGNC ID of equivalent human 'gene family'.|
+
+
+#### Pathway group <a name="pathway"></a>
+
+To download the file, execute the following command.
+
+    Pathway_group = Gene_groups.Pathway_group()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FB_group_id	|Current FlyBase identifier (FBgg##) of Pathway Gene Group.|
+|FB_group_symbol	|Current FlyBase symbol of Pathway Gene Group.|
+|FB_group_name	|Current FlyBase full name of Pathway Gene Group.|
+|Parent_FB_group_id	|Current FlyBase identifier (FBgg##) of parent of given Pathway Gene Group (if relevant).|
+|Parent_FB_group_symbol	|Current FlyBase symbol of parent of given Pathway Gene Group (if relevant).|
+|Group_member_FB_gene_id	|Current FlyBase identifier (FBgn##) of member gene (if terminal group).|
+|Group_member_FB_gene_symbol	|Current FlyBase symbol of member gene (if terminal group).|
+
+## Alleles and Stocks <a name="aands"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Alleles_Stocks = FBD.Alleles_Stocks
+
+Then, enter the specific method according to the desired data
+
+#### Stock data <a name="stock"></a>
+
+To download the file, execute the following command.
+
+    Stock = Alleles_Stocks.Stock()
+
+Columns Description
+
+| Column heading           | Content Description          | Example |
+|----------------------|--------------------|--------------------|
+|FBst	|The unique identifier assigned to this stock by FlyBase.|	FBst0000002|
+|collection_short_name	|A short name for the stock collection that holds the stock.	|Bloomington|
+|stock_type_cv	|The controlled vocabulary term and unique identifier that describe the state of the stock.|	living stock ; FBsv:0000002|
+|species	|Abbreviation (from the Species Abbreviations list) indicating the species of the stock.	|Dmel|
+|FB_genotype	|Genetic components of the stock corresponding to alleles, aberrations, balancers, or insertions in FlyBase. May be empty.|	w[*]; betaTub60D[2] Kr[If-1]/CyO|
+|description	|Genetic components of the stock as provided to FlyBase by the collection that holds the stock.	|FlyTrap: ZCL1796 III|
+|stock_number	|The stock identifier provided to FlyBase by the collection that holds the stock. May be empty.	|110818|
+
+#### Genetic interactions <a name="genint"></a>
+
+To download the file, execute the following command.
+
+    Genetic_interactions = Alleles_Stocks.Allele_genetic_interactions()
+ 
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|allele_symbol	|Current FlyBase allele symbol.|
+|allele_FBal#	|Current FlyBase identifier (FBal#) of allele.|
+|interaction	|Interaction information associated with allele.|
+|FBrf#	|Current FlyBase identifer (FBrf#) of publication from which data came.|
+
+
+#### Phenotypic data <a name="pheno"></a>
+
+To download the file, execute the following command.
+
+    Phenotypic_data = Alleles_Stocks.Phenotypic()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|genotype_symbols	|Current FlyBase symbol(s) of the components that make up the genotype.|
+|genotype_FBids	|Current FlyBase identifier(s) of the components that make up the genotype.|
+|phenotype_name	|Phenotypic name associated with the genotype.|
+|phenotype_id	|Phenotypic identifier associated with the genotype.|
+|qualifier_names	|Qualifier name(s) associated with phenotypic data for genotype.|
+|qualifier_ids	|Qualifier identifier(s) associated with phenotypic data for genotype.|
+|reference	|Current FlyBase identifer (FBrf#) of publication from which data came.|
+
+#### Alleles to Genes <a name="alltoge"></a>
+
+To download the file, execute the following command.
+
+    Alleles_toGenes = Alleles_Stocks.FBal_to_FBgn()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|AlleleID	|Current FlyBase identifier (FBal#) of the allele.|
+|AlleleSymbol	|Current symbol of the allele.|
+|GeneID	|Current FlyBase identifier (FBgn#) of the gene.|
+|GeneSymbol	|Current symbol of the gene.|
+
+## Homologs <a name="homs"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Homologs = FBD.Homologs
+
+Then, enter the specific method according to the desired data
+
+#### Drosophila Paralogs <a name="paral"></a>
+
+To download the file, execute the following command.
+
+    Dmel_Paralog = Homologs.Drosophila_Paralogs()
+
+Columns Description
+
+| Column heading           | Content Description          | 
+|----------------------|--------------------|
+|FBgn_ID	|Current FlyBase identifier (FBgn#) of the D. melanogaster gene.|
+|GeneSymbol	|Current FlyBase gene symbol of the D. melanogaster gene.|
+|Arm/Scaffold	|Arm upon which the D. melanogaster gene is localized.|
+|Location	|Location of D. melanogaster gene on the arm.|
+|Strand	|Strand of D. melanogaster gene ('1' indicates the positive strand, '-1' indicates the negative strand).|
+|Paralog_FBgn_ID	|Current FlyBase identifier (FBgn#) of the paralogous gene.|
+|Paralog_GeneSymbol	|Current FlyBase gene symbol of the paralogous gene.|
+|Paralog_Arm/Scaffold	|Arm upon which the paralogous gene is localized.|
+|Paralog_Location	|Location of paralogous gene on the arm.|
+|Paralog_Strand	|Strand of paralogous gene ('1' indicates the positive strand, '-1' indicates the negative strand).|
+|DIOPT_score	|DIOPT 'score' for the paralog call (i.e. the number of individual algorithms that support the call).|
+
+#### Human Orthologs <a name="hort-d"></a>
+
+To download the file, execute the following command.
+
+    Hman_Orthologs = Homologs.Human_Orthologs()
+ 
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|Dmel_gene_ID	|Current FlyBase identifier (FBgn#) of the D. melanogaster gene.|
+|Dmel_gene_symbol	|Current FlyBase gene symbol of the D. melanogaster gene.|
+|Human_gene_HGNC_ID	|HGNC ID of orthologous human gene.|
+|Human_gene_OMIM_ID	|OMIM ID of orthologous human gene.|
+|Human_gene_symbol	|HGNC gene symbol of orthologous human gene.|
+|DIOPT_score	|DIOPT 'score' for orthology call (i.e. the number of individual algorithms that support the call).|
+|OMIM_Phenotype_IDs	|OMIM Phenotype ID of orthologous human gene (comma separated values).|
+|OMIM_Phenotype_IDs[name]	|OMIM Phenotype ID of orthologous human gene (with the corresponding OMIM name in square brackets).| |Multiple phenotype[name] entries are separated by a comma.|
+
+
+## Human disease <a name="hudss"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Human_disease = FBD.Human_disease
+
+#### Human disease model data <a name="hdm"></a>
+
+To download the file, execute the following command.
+
+    Human_disease_model = Human_disease.Disease_model_annotations()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBgn ID	|Current FlyBase identifier (FBgn#) of the gene associated with the allele of an experimental annotation, or the D. melanogaster ortholog of a human gene associated with a disease in OMIM.|
+|Gene symbol	|Current FlyBase symbol of the gene in column 1.|
+HGNC ID	|HGNC ID of the gene identified in column 1 where it is a human gene (experimental-based annotations only).|
+|DO qualifier	|Type of association between the object of annotation and the disease - one of 'model of', 'ameliorates', 'exacerbates', 'DOES NOT model', 'DOES NOT ameliorate' or 'DOES NOT exacerbate'.|
+|DO ID	|Disease Ontology (DO) ID.|
+|DO term	|Disease Ontology (DO) term.|
+|Allele used in model (FBal ID)	|Current FlyBase identifier (FBal#) of allele (experimental-based annotations only).|
+|Allele used in model (symbol)	|Current FlyBase symbol of allele (experimental-based annotations only).|
+|Based on orthology with (HGNC ID)	|HGNC ID of the human ortholog used for annotations based on orthology to human disease genes.|
+|Based on orthology with (symbol)	|HGNC gene symbol of the human ortholog used for annotations based on orthology to human disease genes.|
+|Evidence/interacting alleles	|Evidence code, with interacting allele(s) where appropriate. For experimental-based annotations, the evidence code is one of: 'inferred from mutant phenotype', 'in combination with', 'modeled by', 'is ameliorated by', 'is exacerbated by', 'is NOT ameliorated by' or 'is NOT exacerbated by'. Interacting alleles are give as 'FLYBASE:<allele_symbol>; FB:<FBal_ID>', with multiple alleles separated by a comma. For orthology-based annotations, the evidence code is 'inferred from electronic annotation'.|
+|Reference (FBrf ID)	|Current FlyBase identifier (FBrf#) of the source publication.|
+
+#### Human orthologs <a name="hort-h"></a>
+
+To download the file, execute the following command.
+
+    Hman_Orthologs = Human_disease.Human_Orthologs()
+
+This is identical to the file of the same name listed under the 'Orthologs' section above.
+
+## Organisms <a name="orgs"></a>
+
+#### Species list <a name="species"></a>
+
+To download the file, execute the following command.
+
+    Species = FBD.Organisms.Species_list()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|Genus	|The genus designation of the organism.|
+|Species name	|The species designation of the organism.|
+|Abbreviation	|The standard FlyBase prefix for the species. This abbreviation is used in FlyBase as the first part of the symbol (before the '\') of any object, e.g. a gene or allele, that originates from this species. This column may be blank, if no individual report page exists for that species in FlyBase.|
+|Common name	|The NCBI Taxonomy Database common name of the organism. This column may be blank.|
+|Ncbi-taxon-id	|The NCBI Taxonomy Database Taxon ID for the organism. This column may be blank.|
+|drosophilid	|If the species is from the family Drosophilidae, this column is filled in with 'y'.|
+
+## Ontology Terms <a name="ont-tr"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Ontology = FBD.Ontology_Terms
+
+#### Fly anatomy <a name="f-bt-on"></a>
+
+
+    FBbt = Ontology.FBbt()
+
+#### Fly development <a name="f-dv-on"></a>
+
+
+    FBdv = Ontology.FBdv()
+
+#### Flybase controlled vocabulary <a name="f-cv-on"></a>
+
+
+    FBcv = Ontology.FBcv()
+
+#### Stock ontology <a name="f-sv-on"></a>
+
+
+    FBsv = Ontology.FBsv()
+
+#### Gene ontology <a name="f-go-on"></a>
+
+
+    GO = Ontology.G0()
+
+#### Image ontology <a name="f-bi-on"></a>
+
+
+    FBbi= Ontology.FBbi()
+
+#### Human disease ontology <a name="f-do-on"></a>
+
+
+    DO = Ontology.DO()
+
+## Insertions <a name="insr"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Insertions = FBD.Insertions
+
+#### Map data for insertions <a name="mp-insr"></a>
+
+   To download the file, execute the following command.
+
+    map_Insertions = Insertions.Map_insertions()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|insertion_symbol	|Current symbol of insertion.|
+|FBti#	|Current FlyBase identifier (FBti#) of insertion.|
+genomic_location	|Genomic location of insertion.|
+|range	|Range (t/f) indicates whether genomic location is range or single base|.
+|orientation	|Orientation (1/0) indicates orientation of insertion on chromosome.|
+|estimated_cytogenetic_location	|Estimated cytogenetic location based on correlation of genomic location and estimated genomic location of cytological bands.|
+|observed_cytogenetic_location	|Observed cytogenetic location reported in the literature.|
+
+
+#### Frequently-used GAL4 drivers <a name="gal4"></a>
+
+   To download the file, execute the following command.
+
+    Gal4 = Insertions.GAL4_drivers()
+
+This file reports a list of all GAL4 drivers that have been curated to at least 21 references and/or are among 150 most frequently requested GAL4 stocks from the [Bloomington Drosophila Stock Center](https://bdsc.indiana.edu/), in JSON format. In addition to the symbols and IDs for Scer\GAL4 alleles, this file also includes their associated transposon or insertion, associated gene, expression pattern in controlled vocabulary stage and anatomy terms, stocks, and publications, all with IDs, as well as free text expression pattern descriptions. This file, except for publications and stocks, is also available in TSV format [here](http://flybase.org/GAL4/freq_used_drivers.tsv).
+
+## Clones <a name="clones"></a>
+
+To facilitate its usage, it is suggested to access the data using the following command.
+
+    Clones = FBD.Clones
+
+#### cDNAs: FBcl to acc. ID <a name="dna-fbcl-acc"></a>
+
+   To download the file, execute the following command.
+
+    c_cDNAs = Clones.cDNA_clone_data()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBcl#	|Current FlyBase identifier (FBcl#) of cDNA clone.|
+organism_abbreviation	|Abbreviation (from the Species |Abbreviations list) indicating the species of origin of the clone.|
+|clone_name	|Clone name.|
+|dataset_metadata_name	|Name of dataset associated with clone.|
+|cDNA_accession(s)	|EMBL/GenBank/DDBJ cDNA accession number.|
+|EST_accession(s)	|EMBL/GenBank/DDBJ EST accession number.|
+
+#### Genomic: FBcl to acc. ID <a name="gen-fbcl-acc"></a>
+
+   To download the file, execute the following command.
+
+    c_genomic = Clones.genomic_clone_data()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBcl#	|Current FlyBase identifier (FBcl#) of genomic clone.|
+|organism_abbreviation	|Abbreviation (from the Species Abbreviations list) indicating the species of origin of the clone.|
+|clone_name	|Clone name.|
+|accession	|EMBL/GenBank/DDBJ cDNA accession number.|
+
+## References <a name="ref"></a>
+
+#### FlyBase FBrf to PubMed ID to PMCID to DOI <a name="ref-get"></a>
+
+   To download the file, execute the following command.
+
+    References = FBD.References.FBrf_PMid_PMCid_doi()
+
+Columns Description
+
+| Column heading           | Content Description          |
+|----------------------|--------------------|
+|FBrf	|The unique FlyBase ID for this publication.|
+|PMID	|The unique PubMed ID for this publication.|
+|PMCID	|The unique PubMed Central ID for this publication, if applicable.|
+|DOI	|The digital object identifier assigned to the publication.
+|pub_type	|The publication type (for example, paper, review, erratum, abstract, book, etc.)|
+|miniref	|A short citation listing the first author, year of publication, journal, volume, issue and page numbers.|
+|pmid_added	|The FlyBase release in which the publication was first incorporated into the FlyBase bibliography. Note: as this report first generated for fb_2012_01 release, all publications associated with a Pub Med ID prior to this release have pmid_added = fb_2011_10.|
+
+## Autor: 
+Javiera Quiroz, [email](javiera.quiroz@biomedica.udec.cl).
```

### Comparing `FlyBaseDownloads-1.0.5/setup.py` & `FlyBaseDownloads-1.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: javiera.quiroz
 """
 
 from setuptools import setup
 
 setup(
     name='FlyBaseDownloads',
-    version='1.0.5',
+    version='1.0.6',
     license='MIT',
     author='Javiera Quiroz Olave',
     url= 'https://github.com/JavieraQuirozO/FlyBaseDownloads',
     author_email='javiera.quiroz@biomedica.udec.cl',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=open('requirements.txt').readlines(),
```

