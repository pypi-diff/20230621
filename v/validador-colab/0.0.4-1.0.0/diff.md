# Comparing `tmp/validador_colab-0.0.4.tar.gz` & `tmp/validador_colab-1.0.0.tar.gz`

## Comparing `validador_colab-0.0.4.tar` & `validador_colab-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 validador_colab-0.0.4/main.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 validador_colab-0.0.4/requirements.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/__init__.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/colab_counter.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/natural_one.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/sakura.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/smarket_counter.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/validation_detail.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/errors/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/errors/divergent_data.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/errors/no_data_found.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/repositories/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/repositories/colab_counters.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/repositories/smarket_analytics.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/usecases/__init__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/usecases/colab_service.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/usecases/smarket_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/configs/__init__.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/configs/configs.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/database/__init__.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/database/postgres.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/database/postgres_controle.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/repositories/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/repositories/colab_counters_repository.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/repositories/smarket_analytics_repository.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/routes/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/routes/daily_conf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/utils/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/loop/__init__.py
--rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/loop/first_block.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 validador_colab-0.0.4/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.4/README.md
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 validador_colab-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 validador_colab-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 validador_colab-1.0.0/main.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 validador_colab-1.0.0/requirements.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/__init__.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/colab_counter.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/natural_one.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/sakura.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/smarket_counter.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/validation_detail.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/errors/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/errors/divergent_data.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/errors/no_data_found.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/repositories/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/repositories/colab_counters.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/repositories/smarket_analytics.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/usecases/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/usecases/colab_service.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/usecases/smarket_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/configs/__init__.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/configs/configs.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/database/__init__.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/database/postgres.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/database/postgres_controle.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/repositories/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/repositories/colab_counters_repository.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/repositories/smarket_analytics_repository.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/routes/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/routes/daily_conf.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/utils/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/utils/break_no_data_found.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/utils/clean_old_data.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/loop/__init__.py
+-rw-r--r--   0        0        0    15078 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/loop/first_block.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/loop/reprocessing_first_block.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 validador_colab-1.0.0/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.0.0/README.md
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 validador_colab-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 validador_colab-1.0.0/PKG-INFO
```

### Comparing `validador_colab-0.0.4/main.py` & `validador_colab-1.0.0/main.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.4/requirements.txt` & `validador_colab-1.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.4/validador_colab/core/entities/sakura.py` & `validador_colab-1.0.0/validador_colab/core/entities/sakura.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,10 +3,11 @@
     def __init__(self):
         self.products = [1949, 1950, 1951, 1952, 1955, 1956, 1957, 1958, 1961, 1962, 1964, 1968, 1969, 27719, 88000,
                          88001, 91601, 111886, 181951, 209716, 209717, 225496, 236720, 287201, 287202, 287203, 287204,
                          287205, 287206, 287207, 287208,
                          325000, 325001, 325099, 325101, 325955, 330471, 330472, 332822, 287201, 287202, 287203, 287207,
                          287208]
         self.clients = [20, 70]
+        self.id = 13
 
     def __repr__(self):
         return "Sakura"
```

### Comparing `validador_colab-0.0.4/validador_colab/core/usecases/colab_service.py` & `validador_colab-1.0.0/validador_colab/core/usecases/colab_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,8 +21,8 @@
         data = self.colab_counters_repository.get_data(industry_id, date_start, date_end)
         if len(data) > 0:
             for unit in data:
                 colab_counters.append(ColabCounter(unit[0], unit[1], unit[2], unit[3]))
             return colab_counters
         else:
             print(f"Sem dados para a industria {industry_id}, na data {date_start} até {date_end}")
-            raise NoDataFound
+            return []
```

### Comparing `validador_colab-0.0.4/validador_colab/core/usecases/smarket_service.py` & `validador_colab-1.0.0/validador_colab/core/usecases/smarket_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,10 +19,15 @@
             date_end = datetime.strptime(date_end, "%Y-%m-%d").strftime("%Y-%m-%d")
         #data = []
         for client_id in industry.clients:
             data = self.smarket_analytics_repository.get_data(industry, date_start, date_end, client_id)
             if len(data) > 0:
                 for unit in data:
                     smarket_counters.append(SmarketCounter(unit[0], unit[1], unit[2], unit[3], unit[4], client_id))
-        return smarket_counters
+
+        if len(smarket_counters) > 0:
+
+            return smarket_counters
+        else:
+            return []
```

### Comparing `validador_colab-0.0.4/validador_colab/infra/configs/configs.py` & `validador_colab-1.0.0/validador_colab/infra/configs/configs.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.4/validador_colab/infra/database/postgres.py` & `validador_colab-1.0.0/validador_colab/infra/database/postgres.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from sqlalchemy import pool
 from validador_colab.infra.configs import CONFIGS
 import psycopg2
-import os
-import sshtunnel
 
 
 class DBConnectionHandlerPostgres:
 
     # def start_smarket_tunnel(self):
     #     """Somente utilizar em caso de dev"""
     #     self.ssh_tunnel = sshtunnel.SSHTunnelForwarder(
@@ -44,56 +41,65 @@
             database=CONFIGS.CLIENT_ID)
         return c
 
     def __init__(self):
         # self.ssh_tunnel = None
         # if CONFIGS.MODE == 'DEV':
         #     self.start_smarket_tunnel()
-
-        pool_colab = pool.QueuePool(
-            self.getconn_colab, max_overflow=0, pool_size=2)
-        pool_smarket = pool.QueuePool(
-            self.getconn_smarket, max_overflow=0, pool_size=2)
-        self.conn_colab = pool_colab.connect()
-        self.conn_smarket = pool_smarket.connect()
-        self.cursor_colab = self.conn_colab.cursor()
-        self.cursor_smarket = self.conn_smarket.cursor()
+        # pool_colab = pool.QueuePool(
+        #     self.getconn_colab, max_overflow=0, pool_size=2)
+        # pool_smarket = pool.QueuePool(
+        #     self.getconn_smarket, max_overflow=0, pool_size=2)
+        # self.conn_colab = pool_colab.connect()
+        # self.conn_smarket = pool_smarket.connect()
+        # self.cursor_colab = self.conn_colab.cursor()
+        # self.cursor_smarket = self.conn_smarket.cursor()
+        pass
 
     def get(self, mode: str, sql: str):
 
         values = [()]
 
         if mode.upper() == 'COLAB':
-            self.cursor_colab.execute(sql)
-            try:
-                values = self.cursor_colab.fetchall()
-            except Exception as e:
-                self.cursor_colab.execute('rollback')
-            finally:
-                self.cursor_colab.execute('commit')
-            return values
+            conn_clb = self.getconn_colab()
+            with conn_clb.cursor() as colab_curs:
+                colab_curs.execute(sql)
+                try:
+                    values = colab_curs.fetchall()
+                except Exception as e:
+                    colab_curs.execute('rollback')
+                finally:
+                    colab_curs.execute('commit')
+                conn_clb.close()
+                return values
 
         elif mode.upper() == 'SMARKET':
-            self.cursor_smarket.execute(sql)
-            try:
-                values = self.cursor_smarket.fetchall()
-            except Exception as e:
-                self.cursor_smarket.execute('rollback')
-            finally:
-                self.cursor_smarket.execute('commit')
-            return values
+            conn_smkt = self.getconn_smarket()
+            with conn_smkt.cursor() as smkt_curs:
+                smkt_curs.execute(sql)
+                try:
+                    values = smkt_curs.fetchall()
+                except Exception as e:
+                    smkt_curs.execute('rollback')
+                finally:
+                    smkt_curs.execute('commit')
+                conn_smkt.close()
+                return values
 
     def insert(self, sql, mode='COLAB'):
         if mode.upper() == "COLAB":
-            try:
-                self.cursor_colab.execute(sql)
-            except Exception as e:
-                self.cursor_colab.execute('rollback')
-            finally:
-                self.cursor_colab.execute('commit')
+            conn_clb = self.conn_colab()
+            with conn_clb.cursor() as colab_curs:
+                try:
+                    colab_curs.execute(sql)
+                except Exception as e:
+                    colab_curs.execute('rollback')
+                finally:
+                    colab_curs.execute('commit')
+                conn_clb.close()
 
 
 
 if __name__ == "__main__":
 
     db = DBConnectionHandlerPostgres()
     print(db.get('smarket', 'select now();'))
```

### Comparing `validador_colab-0.0.4/validador_colab/infra/database/postgres_controle.py` & `validador_colab-1.0.0/validador_colab/infra/database/postgres_controle.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,21 +15,36 @@
             host=CONFIGS.COLAB_PROD_HOST,
             database=CONFIGS.COLAB_PROD_NAME,
             port=CONFIGS.COLAB_PROD_PORT
         )
         return c
 
     def __init__(self):
-        pool_colab = pool.QueuePool(
-            self.getconn_colab, max_overflow=0, pool_size=2)
-        self.conn_colab = pool_colab.connect()
-        self.cursor_colab = self.conn_colab.cursor()
+        # pool_colab = pool.QueuePool(
+        #     self.getconn_colab, max_overflow=0, pool_size=2)
+        # self.conn_colab = pool_colab.connect()
+        # self.cursor_colab = self.conn_colab.cursor()
+        pass
+
+    # def get(self, sql):
+    #     conn_colab = self.getconn_colab()
+    #     with conn_colab.cursor() as colab_curs:
+    #         try:
+    #             colab_curs.execute(sql)
+    #         except Exception as e:
+    #             colab_curs.execute("rollback")
+    #         finally:
+    #             colab_curs.execute("commit")
+    #     conn_colab.close()
 
     def insert(self, sql, mode='COLAB'):
         if mode.upper() == "COLAB":
-            try:
-                self.cursor_colab.execute(sql)
-            except Exception as e:
-                print(e)
-                self.cursor_colab.execute('rollback')
-            finally:
-                self.cursor_colab.execute('commit')
+            conn_colab = self.getconn_colab()
+            with conn_colab.cursor() as colab_curs:
+                try:
+                    colab_curs.execute(sql)
+                except Exception as e:
+                    print(e)
+                    colab_curs.execute('rollback')
+                finally:
+                    colab_curs.execute('commit')
+                conn_colab.close()
```

### Comparing `validador_colab-0.0.4/validador_colab/infra/repositories/colab_counters_repository.py` & `validador_colab-1.0.0/validador_colab/infra/repositories/colab_counters_repository.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.4/validador_colab/infra/repositories/smarket_analytics_repository.py` & `validador_colab-1.0.0/validador_colab/infra/repositories/smarket_analytics_repository.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.4/validador_colab/infra/routes/daily_conf.py` & `validador_colab-1.0.0/validador_colab/infra/routes/daily_conf.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.4/validador_colab/loop/first_block.py` & `validador_colab-1.0.0/validador_colab/loop/first_block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,83 @@
 from validador_colab.infra.repositories import SmarketAnalyticsRepositoryPostgres, ColabCountersRepositoryPostgres
 from validador_colab.core.usecases import SmarketService, ColabService
 from validador_colab.core.entities import Sakura, NaturalOne, ValidationDetail
 from validador_colab.core.errors import NoDataFound
-from validador_colab.infra.database import DBConnectionHandlerPostgres, DBConnectionHandlerPostgresControle
+from validador_colab.infra.database import DBConnectionHandlerPostgres, DBConnectionHandlerPostgresControle, DB_CONTROLE
+from validador_colab.infra.utils import break_no_data_found
 import pickle
 import os
 import asyncio
 import datetime
 
 temp_data_folder = os.path.join(os.getcwd(), 'temp_data')
 
 db = DBConnectionHandlerPostgresControle()
 
 
-async def first_block(industry_id: int, date_start, date_end, print_corretos=True):
+async def first_block(industry_id: int, date_start, date_end, print_corretos=True, pickle_use=False):
     if not os.path.exists(temp_data_folder):
         os.makedirs(temp_data_folder)
 
     if industry_id == 11: #Natural One
         industry = NaturalOne()
     elif industry_id == 13: #Sakura
         industry = Sakura()
 
     pickle_colab_name = "colab_data_" + industry.__repr__() + "_" + date_start + "_" + date_end + ".pkl"
     pickle_smarket_name = "smarket_data_" + industry.__repr__() + "_" + date_start + "_" + date_end + ".pkl"
 
-    try:
-        if not os.path.exists(os.path.join(temp_data_folder, pickle_smarket_name)):
-            print("Getting data from smarket")
-            smarket_data = SmarketService(SmarketAnalyticsRepositoryPostgres()).get_smarket_counters(industry, date_start, date_end)
-            with open(os.path.join(temp_data_folder, pickle_smarket_name), 'wb') as f:
-                pickle.dump(smarket_data, f)
-            print("Data saved")
-        else:
-            print("Loading data from smarket")
-            with open(os.path.join(temp_data_folder, pickle_smarket_name), 'rb') as f:
-                smarket_data = pickle.load(f)
-            print("Data loaded")
-
-        if not os.path.exists(os.path.join(temp_data_folder, pickle_colab_name)):
-            print("Getting data from colab")
-            colab_data = ColabService(ColabCountersRepositoryPostgres()).get_colab_counters(industry_id, date_start, date_end)
-            with open(os.path.join(temp_data_folder, pickle_colab_name), 'wb') as f:
-                pickle.dump(colab_data, f)
-            print("Data saved")
-        else:
-            print("Loading data from colab")
-            with open(os.path.join(temp_data_folder, pickle_colab_name), 'rb') as f:
-                colab_data = pickle.load(f)
-            print("Data loaded")
-    except NoDataFound:
-        print(f"Sem dados cadastrados para a industria no dia {date_start} até o dia {date_end}")
+    if pickle_use:
+
+        try:
+            if not os.path.exists(os.path.join(temp_data_folder, pickle_smarket_name)):
+                print("Getting data from smarket")
+                smarket_data = SmarketService(SmarketAnalyticsRepositoryPostgres()).get_smarket_counters(industry, date_start, date_end)
+                with open(os.path.join(temp_data_folder, pickle_smarket_name), 'wb') as f:
+                    pickle.dump(smarket_data, f)
+                print("Data saved")
+            else:
+                print("Loading data from smarket")
+                with open(os.path.join(temp_data_folder, pickle_smarket_name), 'rb') as f:
+                    smarket_data = pickle.load(f)
+                print("Data loaded")
+
+            if not os.path.exists(os.path.join(temp_data_folder, pickle_colab_name)):
+                print("Getting data from colab")
+                colab_data = ColabService(ColabCountersRepositoryPostgres()).get_colab_counters(industry_id, date_start, date_end)
+                with open(os.path.join(temp_data_folder, pickle_colab_name), 'wb') as f:
+                    pickle.dump(colab_data, f)
+                print("Data saved")
+            else:
+                print("Loading data from colab")
+                with open(os.path.join(temp_data_folder, pickle_colab_name), 'rb') as f:
+                    colab_data = pickle.load(f)
+                print("Data loaded")
+        except NoDataFound:
+            print(f"Sem dados cadastrados para a industria no dia {date_start} até o dia {date_end}")
+
+    else:
+        print("Getting data from smarket")
+        smarket_data = SmarketService(SmarketAnalyticsRepositoryPostgres()).get_smarket_counters(industry, date_start,
+                                                                                                 date_end)
+        print("Getting data from colab")
+        colab_data = ColabService(ColabCountersRepositoryPostgres()).get_colab_counters(industry_id, date_start,
+                                                                                        date_end)
+
+
+    if len(smarket_data) == 0 or len(colab_data) == 0:
+        print("Erro na execução:")
+        print(f"Data de consulta: {date_start} - {date_end}")
+        print(f"len(smarket_data) = {len(smarket_data)}")
+        print(f"len(colab_data) = {len(colab_data)}")
+        print("Classificando dias como não aptos a atualização")
+
+        DB_CONTROLE.insert(break_no_data_found(industry, date_start, date_end))
+        print("Finalizando processo")
+        return 0
 
     #esta merda aqui vai ficar troncha, loop dentro de loop, mas é o que tem pra hoje
     print('Iniciando processamento')
     count_produtos_certos = {}
     count_produtos_errados = {}
     validation_intel = []
 
@@ -246,13 +269,13 @@
     """
     for validation in validation_intel:
         sql_insert += f"""({int(validation.industry_id)}, {int(validation.client_id)}, '{validation.sale_date}', {bool(validation.validation_status)}),"""
 
     sql_insert = sql_insert[:-1]
     print(sql_insert)
 
-    db.insert(sql_insert)
+    DB_CONTROLE.insert(sql_insert)
 
 
 
 if __name__ == "__main__":
-    asyncio.run(first_block(11, '2023-06-05', '2023-06-05', True))
+    asyncio.run(first_block(11, '2023-06-22', '2023-06-22', False))
```

### Comparing `validador_colab-0.0.4/.gitignore` & `validador_colab-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.4/pyproject.toml` & `validador_colab-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "validador-colab"
 description = 'Validador colab é uma ferramenta para validar os dados diarios incrementáis nas tabelas de fato do colab e no Analytics'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
-version = "0.0.4"
+version = "1.0.0"
 keywords = []
 authors = [
   { name = "Davi Amaral de Araujo", email = "davi@smarketsolutions.com.br" },
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `validador_colab-0.0.4/PKG-INFO` & `validador_colab-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validador-colab
-Version: 0.0.4
+Version: 1.0.0
 Summary: Validador colab é uma ferramenta para validar os dados diarios incrementáis nas tabelas de fato do colab e no Analytics
 Project-URL: Documentation, https://github.com/unknown/validador-colab#readme
 Project-URL: Issues, https://github.com/unknown/validador-colab/issues
 Project-URL: Source, https://github.com/unknown/validador-colab
 Author-email: Davi Amaral de Araujo <davi@smarketsolutions.com.br>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

