# Comparing `tmp/astronomer_starship-1.0.2.tar.gz` & `tmp/astronomer_starship-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomer_starship-1.0.2.tar", max compression
+gzip compressed data, was "astronomer_starship-1.0.3.tar", max compression
```

## Comparing `astronomer_starship-1.0.2.tar` & `astronomer_starship-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      547 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/LICENSE
--rw-r--r--   0        0        0     9187 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/README.rst
--rw-r--r--   0        0        0        0 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/aeroscope/__init__.py
--rw-r--r--   0        0        0     2434 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/aeroscope/operators.py
--rw-r--r--   0        0        0     4126 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/aeroscope/plugins/__init__.py
--rw-r--r--   0        0        0      262 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/aeroscope/plugins/templates/aeroscope/formhelper.html
--rw-r--r--   0        0        0     2524 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/aeroscope/plugins/templates/aeroscope/main.html
--rw-r--r--   0        0        0     1561 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/aeroscope/util.py
--rw-r--r--   0        0        0        0 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/__init__.py
--rw-r--r--   0        0        0    13578 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/main.py
--rw-r--r--   0        0        0     7950 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/operators.py
--rw-r--r--   0        0        0        0 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/services/__init__.py
--rw-r--r--   0        0        0     7382 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/services/astro_client.py
--rw-r--r--   0        0        0     4318 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/services/local_airflow_client.py
--rw-r--r--   0        0        0     5230 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/services/remote_airflow_client.py
--rw-r--r--   0        0        0    39434 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/static/js/htmx.min.js
--rw-r--r--   0        0        0     7015 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/static/js/idiomorph.min.js
--rw-r--r--   0        0        0    20095 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/static/js/popper.js
--rw-r--r--   0        0        0    25717 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/static/js/tippy.js
--rw-r--r--   0        0        0     1309 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/static/tail-spin.svg
--rw-r--r--   0        0        0     2926 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/dag_row.html
--rw-r--r--   0        0        0      283 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/env_checkbox.html
--rw-r--r--   0        0        0      200 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/github_loop.html
--rw-r--r--   0        0        0      738 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/migrate_connection_button.html
--rw-r--r--   0        0        0      360 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/migrate_pool_button.html
--rw-r--r--   0        0        0      367 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/migrate_variable_button.html
--rw-r--r--   0        0        0     1194 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/tabs.html
--rw-r--r--   0        0        0     2088 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/tabs_loading.html
--rw-r--r--   0        0        0     1661 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/target_deployment_select.html
--rw-r--r--   0        0        0     1227 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/target_deployment_select_loading.html
--rw-r--r--   0        0        0      177 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/test_connection_label.html
--rw-r--r--   0        0        0     2644 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/token_modal.html
--rw-r--r--   0        0        0       15 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/user_label.html
--rw-r--r--   0        0        0     1759 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/connections.html
--rw-r--r--   0        0        0     1089 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/dags.html
--rw-r--r--   0        0        0     1847 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/env.html
--rw-r--r--   0        0        0      775 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/main.html
--rw-r--r--   0        0        0      980 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/migration.html
--rw-r--r--   0        0        0     1415 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/pools.html
--rw-r--r--   0        0        0     1376 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/variables.html
--rw-r--r--   0        0        0     1363 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/variables/operators.py
--rw-r--r--   0        0        0     2734 2023-06-12 21:22:15.226787 astronomer_starship-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     9984 1970-01-01 00:00:00.000000 astronomer_starship-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      547 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/LICENSE
+-rw-r--r--   0        0        0     9187 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/README.rst
+-rw-r--r--   0        0        0        0 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/__init__.py
+-rw-r--r--   0        0        0     2434 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/operators.py
+-rw-r--r--   0        0        0     4126 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/plugins/__init__.py
+-rw-r--r--   0        0        0      262 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/plugins/templates/aeroscope/formhelper.html
+-rw-r--r--   0        0        0     2524 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/plugins/templates/aeroscope/main.html
+-rw-r--r--   0        0        0     1561 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/util.py
+-rw-r--r--   0        0        0        0 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/__init__.py
+-rw-r--r--   0        0        0    14265 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/main.py
+-rw-r--r--   0        0        0     7950 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/operators.py
+-rw-r--r--   0        0        0        0 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/services/__init__.py
+-rw-r--r--   0        0        0     7382 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/services/astro_client.py
+-rw-r--r--   0        0        0     4416 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/services/local_airflow_client.py
+-rw-r--r--   0        0        0     6601 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/services/remote_airflow_client.py
+-rw-r--r--   0        0        0    39434 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/static/js/htmx.min.js
+-rw-r--r--   0        0        0     7015 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/static/js/idiomorph.min.js
+-rw-r--r--   0        0        0    20095 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/static/js/popper.js
+-rw-r--r--   0        0        0    25717 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/static/js/tippy.js
+-rw-r--r--   0        0        0     1309 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/static/tail-spin.svg
+-rw-r--r--   0        0        0     2926 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/dag_row.html
+-rw-r--r--   0        0        0      283 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/env_checkbox.html
+-rw-r--r--   0        0        0      200 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/github_loop.html
+-rw-r--r--   0        0        0      738 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/migrate_connection_button.html
+-rw-r--r--   0        0        0      360 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/migrate_pool_button.html
+-rw-r--r--   0        0        0      367 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/migrate_variable_button.html
+-rw-r--r--   0        0        0     1194 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/tabs.html
+-rw-r--r--   0        0        0     2088 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/tabs_loading.html
+-rw-r--r--   0        0        0     1661 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/target_deployment_select.html
+-rw-r--r--   0        0        0     1227 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/target_deployment_select_loading.html
+-rw-r--r--   0        0        0      177 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/test_connection_label.html
+-rw-r--r--   0        0        0     2644 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/token_modal.html
+-rw-r--r--   0        0        0       15 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/user_label.html
+-rw-r--r--   0        0        0     1759 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/connections.html
+-rw-r--r--   0        0        0     1089 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/dags.html
+-rw-r--r--   0        0        0     1847 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/env.html
+-rw-r--r--   0        0        0      775 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/main.html
+-rw-r--r--   0        0        0      980 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/migration.html
+-rw-r--r--   0        0        0     1415 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/pools.html
+-rw-r--r--   0        0        0     1376 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/variables.html
+-rw-r--r--   0        0        0     1363 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/variables/operators.py
+-rw-r--r--   0        0        0     3190 2023-06-21 14:45:14.855371 astronomer_starship-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10034 1970-01-01 00:00:00.000000 astronomer_starship-1.0.3/PKG-INFO
```

### Comparing `astronomer_starship-1.0.2/LICENSE` & `astronomer_starship-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/README.rst` & `astronomer_starship-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/aeroscope/operators.py` & `astronomer_starship-1.0.3/astronomer/aeroscope/operators.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/aeroscope/plugins/__init__.py` & `astronomer_starship-1.0.3/astronomer/aeroscope/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/aeroscope/plugins/templates/aeroscope/main.html` & `astronomer_starship-1.0.3/astronomer/aeroscope/plugins/templates/aeroscope/main.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/aeroscope/util.py` & `astronomer_starship-1.0.3/astronomer/aeroscope/util.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/main.py` & `astronomer_starship-1.0.3/astronomer/starship/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -311,52 +311,68 @@
             "POST",
         ),
     )
     @auth.has_access([(permissions.ACTION_CAN_EDIT, permissions.RESOURCE_DAG)])
     def dag_cutover_row(
         self, deployment: str, dag_id: str, dest: str = "local", action: str = "init"
     ):
+        valid_actions = ["pause", "unpause", "migrate", "init"]
         if dest not in ["local", "astro"]:
             raise RuntimeError("dest must be 'local' or 'astro'")
-        if action not in ["pause", "unpause", "migrate", "init"]:
-            raise Exception("action must be 'pause', 'unpause', or 'migrate'")
+        if action not in valid_actions:
+            raise RuntimeError(
+                f"action({action}) must be in valid_actions({valid_actions})"
+            )
 
         token = session.get("token")
         deployment_url = astro_client.get_deployment_url(deployment, token)
 
         if request.method == "POST":
             if action == "migrate":
                 remote_airflow_client.migrate_dag(
                     dag_id, deployment_url=deployment_url, token=token
                 )
+                # force an update, make sure the change went through
+                remote_airflow_client.get_dag(
+                    dag_id, deployment_url, token, skip_cache=True
+                )
             else:
                 is_paused = "pause" == action
                 if dest == "local":
                     local_airflow_client.set_dag_is_paused(dag_id, is_paused)
                 else:
                     remote_airflow_client.set_dag_is_paused(
                         dag_id, is_paused, deployment_url, token
                     )
+                    # force an update, make sure the change went through
+                    remote_airflow_client.get_dag(
+                        dag_id, deployment_url, token, skip_cache=True
+                    )
 
-        r = remote_airflow_client.get_dag(dag_id, deployment_url, token)
-        dag_runs = remote_airflow_client.get_dag_runs(
+        remote_dag_response = remote_airflow_client.get_dag(
             dag_id, deployment_url, token
-        ).json()
-        is_on_astro = not r.status_code == 404
-        remote_dag = r.json()
+        )
+        is_on_astro = remote_dag_response is not None
+        remote_dag = remote_dag_response or {}
+        remote_dag_runs = (
+            remote_airflow_client.get_dag_runs(dag_id, deployment_url, token).json()
+            if is_on_astro
+            else {}
+        )
+        has_history_on_astro = bool(remote_dag_runs.get("total_entries", 0))
         local_dag = local_airflow_client.get_dag(dag_id)
 
         return self.render_template(
             "starship/components/dag_row.html",
             dag_={
                 "id": local_dag.dag_id,
                 "is_on_astro": is_on_astro,
                 "is_paused_here": local_dag.is_paused,
                 "is_paused_on_astro": remote_dag["is_paused"] if is_on_astro else False,
-                "has_history_on_astro": bool(dag_runs["total_entries"]),
+                "has_history_on_astro": has_history_on_astro,
             },
         )
 
 
 v_appbuilder_view = AstroMigration()
 
 v_appbuilder_package = {
```

### Comparing `astronomer_starship-1.0.2/astronomer/starship/operators.py` & `astronomer_starship-1.0.3/astronomer/starship/operators.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/services/astro_client.py` & `astronomer_starship-1.0.3/astronomer/starship/services/astro_client.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/services/local_airflow_client.py` & `astronomer_starship-1.0.3/astronomer/starship/services/local_airflow_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 from typing import List
 
 import sqlalchemy
 from airflow import DAG, settings
 from airflow.models import DagModel
 from airflow.utils.session import provide_session
+from cachetools.func import ttl_cache
 from deprecated import deprecated
 from sqlalchemy import MetaData, Table
 from sqlalchemy.exc import NoSuchTableError
 from sqlalchemy.orm import Session
 from airflow.models import Connection
 from airflow.models import Pool
 
@@ -38,14 +39,15 @@
     return variables
 
 
 def get_variable(variable: str):
     return [v for v in get_variables() if v.key == variable][0]
 
 
+@ttl_cache(ttl=60)
 def get_dags():
     from airflow.models import DagBag
 
     dags = DagBag().dags
     return dags
 
 
@@ -100,15 +102,17 @@
                         ti_key
                     ] = f"{ti_value.strftime('%Y-%m-%d %H:%M:%S.%f+00')}"
             rtn.append(ti_result)
 
     return rtn
 
 
-def receive_dag(data: list = []):
+def receive_dag(data: list = None):
+    if data is None:
+        data = []
     dest_session = settings.Session()
     dest_engine = dest_session.get_bind()
     dest_metadata_obj = MetaData(bind=dest_engine)
     for datum in data:
         try:
             del datum["conf"]
             del datum["id"]
```

### Comparing `astronomer_starship-1.0.2/astronomer/starship/services/remote_airflow_client.py` & `astronomer_starship-1.0.3/astronomer/starship/services/remote_airflow_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import json
-from typing import Any, List
+from datetime import datetime, timedelta
+from typing import Any, List, Dict, Optional
 
 import requests
 from airflow.models import Connection, Pool, Variable
 from cachetools.func import ttl_cache
 from deprecated import deprecated
 from requests import Response
 
 from astronomer.starship.services import local_airflow_client
 
+remote_dags: Dict[str, Dict[str, Any]] = {}
+dag_fetch_time: datetime = datetime(1970, 1, 1)
+
 
 def conn_to_json(connection: Connection) -> dict:
     return {
         "connection_id": connection.conn_id,
         "conn_type": connection.conn_type,
         "host": connection.host,
         "login": connection.login,
@@ -147,26 +151,65 @@
         headers={"Authorization": f"Bearer {token}"},
         json={"is_paused": is_paused},
     )
     r.raise_for_status()
     return r
 
 
-def get_dag(dag_id, deployment_url, token) -> Response:
+def _get_remote_dags(deployment_url: str, token: str) -> Response:
+    r = requests.get(
+        f"{deployment_url}/api/v1/dags",
+        headers={"Authorization": f"Bearer {token}"},
+    )
+    return r
+
+
+def _get_remote_dag(dag_id: str, deployment_url: str, token: str) -> Response:
     r = requests.get(
         f"{deployment_url}/api/v1/dags/{dag_id}",
         headers={"Authorization": f"Bearer {token}"},
     )
-    r.raise_for_status()
     return r
 
 
+def get_dag(
+    dag_id: str,
+    deployment_url: str,
+    token: str,
+    ttl: timedelta = timedelta(seconds=60),
+    skip_cache: bool = False,
+) -> Optional[Dict[str, Any]]:
+    global remote_dags
+    global dag_fetch_time
+
+    if dag_fetch_time + ttl < datetime.now():
+        r = _get_remote_dags(deployment_url, token)
+        if not r.ok:
+            remote_dags = {}
+            dag_fetch_time = datetime.now()
+            r.raise_for_status()
+        else:
+            # reset the cache - reset the ttl timer
+            remote_dags = {dag["dag_id"]: dag for dag in r.json().get("dags", [])}
+            dag_fetch_time = datetime.now()
+        return remote_dags.get(dag_id)
+    elif skip_cache:
+        r = _get_remote_dag(dag_id, deployment_url, token)
+        r.raise_for_status()
+        dag = r.json()
+        remote_dags[dag_id] = dag
+        # we don't reset the cache time - because all other entries are still on the clock
+        return dag
+    else:
+        return remote_dags.get(dag_id)
+
+
 def get_dag_runs(dag_id, deployment_url, token) -> Response:
     r = requests.get(
-        f"{deployment_url}/api/v1/dags/{dag_id}/dagRuns",
+        f"{deployment_url}/api/v1/dags/{dag_id}/dagRuns?limit=1",
         headers={"Authorization": f"Bearer {token}"},
     )
     r.raise_for_status()
     return r
 
 
 def migrate_dag(dag: str, deployment_url: str, token: str):
```

### Comparing `astronomer_starship-1.0.2/astronomer/starship/static/js/htmx.min.js` & `astronomer_starship-1.0.3/astronomer/starship/static/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/static/js/idiomorph.min.js` & `astronomer_starship-1.0.3/astronomer/starship/static/js/idiomorph.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/static/js/popper.js` & `astronomer_starship-1.0.3/astronomer/starship/static/js/popper.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/static/js/tippy.js` & `astronomer_starship-1.0.3/astronomer/starship/static/js/tippy.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/static/tail-spin.svg` & `astronomer_starship-1.0.3/astronomer/starship/static/tail-spin.svg`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/dag_row.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/dag_row.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/migrate_connection_button.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/migrate_connection_button.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/tabs.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/tabs.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/tabs_loading.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/tabs_loading.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/target_deployment_select.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/target_deployment_select.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/target_deployment_select_loading.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/target_deployment_select_loading.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/token_modal.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/token_modal.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/connections.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/connections.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/dags.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/dags.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/env.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/env.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/main.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/main.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/migration.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/migration.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/pools.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/pools.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/templates/starship/variables.html` & `astronomer_starship-1.0.3/astronomer/starship/templates/starship/variables.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/astronomer/starship/variables/operators.py` & `astronomer_starship-1.0.3/astronomer/starship/variables/operators.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.2/pyproject.toml` & `astronomer_starship-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "astronomer-starship"
-version = "1.0.2"
+version = "1.0.3"
 description = "Migrations to Astro"
 authors = ["ADE Team <ade@astronomer.io>"]
 readme = "README.rst"
 repository = "https://github.com/astronomer/starship"
 homepage = "https://astronomer.io"
 license = "Proprietary"
 packages = [{include = "astronomer"}]  #, from = "." }]
@@ -17,44 +17,46 @@
 #[tool.setuptools]
 #package-dir = {"" = "astronomer"}
 #
 #[tool.setuptools.packages.find]
 #where = ["astronomer"]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.7.2,<4.0"
 pydash = "^7.0.0"
 python-graphql-client = "^0.4.3"
 requests = "^2.28.2"
 cachetools = "^5.3.0"
 pygithub = "^1.58.1"
 
 [tool.poetry.group.orion.dependencies]
 click = "^8.1.3"
 halo = "^0.0.31"
-sh = "^2.0.2"
 fs = "^2.4.16"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 black = "^23.1.0"
 pytest-cov = "^4.0.0"
 requests = "^2.28.2"
 twine = "^4.0.2"
-pre-commit = "^3.2.2"
 ruff = "^0.0.261"
-isort = "^5.12.0"
-pylint = "^2.17.2"
+pylint = {version = "^2.17.2", python = ">=3.8.1"}
 pyupgrade = "^3.3.1"
 pytest-integration = "^0.2.3"
 pyyaml = "^6.0"
-python-dotenv = "^1.0.0"
 pulumi = "^3.63.0"
 pulumi-aws = "^5.35.0"
-sh = "^2.0.3"
+pytest-mock = "^3.10.0"
+apache-airflow = "^2.6.1"
+isort = {version = "^5.12.0", python = ">=3.8.1"}
+python-dotenv = {version = "^1.0.0", python = ">=3.8.1"}
+sh = {version = "^2.0.4", python = ">=3.8.1"}
+pre-commit = {version = "^3.3.3", python = ">=3.8.1"}
+toml = {version = "^0.10.2", python = "<3.11"}
 
 
 [tool.poetry.group.aws.dependencies]
 boto3 = "^1.26.81"
 boto3-stubs = {extras = ["mwaa", "s3"], version = "^1.26.81"}
 fs-s3fs = "^1.1.1"
 
@@ -64,17 +66,21 @@
 
 # dynamically add plugin to Airflow Plugins
 [tool.poetry.plugins] # Optional super table
 [tool.poetry.plugins."airflow.plugins"]
 "starship" = "astronomer.starship.main:StarshipPlugin"
 "starship_aeroscope" = "astronomer.aeroscope.plugins:AeroscopePlugin"
 
+# for pip installing this pyproject.toml
+[project.entry-points."airflow.plugins"]
+"starship" = "astronomer.starship.main:StarshipPlugin"
+"starship_aeroscope" = "astronomer.aeroscope.plugins:AeroscopePlugin"
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 # https://github.com/psf/black
 color = true
 
 [tool.bandit]
@@ -91,15 +97,15 @@
 
 [tool.rstcheck]
 report_level = "WARNING"
 
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
 # Directories that are not visited by pytest collector:
-#norecursedirs =["tests/resources/", "hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__"]
+norecursedirs =["tests/resources/", "hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__"]
 doctest_optionflags = ["NUMBER", "NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
 
 # Extra options:
 addopts = [
 #  "--ignore=tests/resources/example-dag.py",
 #  "--ignore=resources/fix.py",
 #  "--numprocesses=auto",
```

### Comparing `astronomer_starship-1.0.2/PKG-INFO` & `astronomer_starship-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: astronomer-starship
-Version: 1.0.2
+Version: 1.0.3
 Summary: Migrations to Astro
 Home-page: https://astronomer.io
 License: Proprietary
 Author: ADE Team
 Author-email: ade@astronomer.io
-Requires-Python: >=3.8.1,<4.0
+Requires-Python: >=3.7.2,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cachetools (>=5.3.0,<6.0.0)
 Requires-Dist: pydash (>=7.0.0,<8.0.0)
 Requires-Dist: pygithub (>=1.58.1,<2.0.0)
 Requires-Dist: python-graphql-client (>=0.4.3,<0.5.0)
```

