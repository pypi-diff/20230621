# Comparing `tmp/surge_api-1.1.1-py3-none-any.whl.zip` & `tmp/surge_api-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 17525 bytes, number of entries: 16
+Zip file size: 17563 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      186 b- defN 23-Jun-19 05:11 surge/__init__.py
--rw-r--r--  2.0 unx     2905 b- defN 23-Jun-19 05:44 surge/api_resource.py
+-rw-r--r--  2.0 unx     2905 b- defN 23-Jun-21 06:40 surge/api_resource.py
 -rw-r--r--  2.0 unx      734 b- defN 23-Jun-19 05:11 surge/carousel.py
 -rw-r--r--  2.0 unx     1606 b- defN 23-Jun-19 05:11 surge/errors.py
--rw-r--r--  2.0 unx    12092 b- defN 23-Jun-19 05:47 surge/projects.py
+-rw-r--r--  2.0 unx    12142 b- defN 23-Jun-21 06:22 surge/projects.py
 -rw-r--r--  2.0 unx    26952 b- defN 23-Jun-19 05:11 surge/questions.py
 -rw-r--r--  2.0 unx     5173 b- defN 23-Jun-19 05:11 surge/reports.py
 -rw-r--r--  2.0 unx      939 b- defN 23-Jun-19 05:11 surge/responses.py
 -rw-r--r--  2.0 unx     5799 b- defN 23-Jun-19 05:11 surge/tasks.py
 -rw-r--r--  2.0 unx     4107 b- defN 23-Jun-19 05:11 surge/teams.py
 -rw-r--r--  2.0 unx      442 b- defN 23-Jun-19 05:11 surge/utils.py
--rw-r--r--  2.0 unx     1062 b- defN 23-Jun-20 05:35 surge_api-1.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3742 b- defN 23-Jun-20 05:35 surge_api-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 05:35 surge_api-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 05:35 surge_api-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1201 b- defN 23-Jun-20 05:35 surge_api-1.1.1.dist-info/RECORD
-16 files, 67038 bytes uncompressed, 15587 bytes compressed:  76.7%
+-rw-r--r--  2.0 unx     1062 b- defN 23-Jun-21 06:40 surge_api-1.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3742 b- defN 23-Jun-21 06:40 surge_api-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 06:40 surge_api-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-21 06:40 surge_api-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1201 b- defN 23-Jun-21 06:40 surge_api-1.1.2.dist-info/RECORD
+16 files, 67088 bytes uncompressed, 15625 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: surge/teams.py
 Comment: 
 
 Filename: surge/utils.py
 Comment: 
 
-Filename: surge_api-1.1.1.dist-info/LICENSE
+Filename: surge_api-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: surge_api-1.1.1.dist-info/METADATA
+Filename: surge_api-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: surge_api-1.1.1.dist-info/WHEEL
+Filename: surge_api-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: surge_api-1.1.1.dist-info/top_level.txt
+Filename: surge_api-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: surge_api-1.1.1.dist-info/RECORD
+Filename: surge_api-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## surge/projects.py

```diff
@@ -57,15 +57,15 @@
                qualifications_required: list = [],
                teams_required: list = [],
                callback_url: str = None,
                fields_template: str = None,
                num_workers_per_task: int = 1,
                tags=[],
                carousel=None,
-               copy_from_project_id=None):
+               template_id=None):
         '''
         Creates a new Project.
 
         Arguments:
             name (str): Name of the project.
             payment_per_response (float, optional):
                 How much a worker is paid (in US dollars) for an individual response.
@@ -77,16 +77,15 @@
             teams_required (list, optional): If you have created custom teams, you can pass a list of team ids Surgers must have to work on the project here.
             callback_url (str, optional): url that receives a POST request with the project's data.
             fields_template (str, optional): A template describing how fields are shown to workers working on the task.
                 For example, if fields_template is "{{company_name}}", then workers will be shown a link to the company.
             num_workers_per_task (int, optional): How many workers work on each task (i.e., how many responses per task).
             tags (list, optional): An array of strings to tag the project with. Worker won't see these tags.
             carousel (dict, optional): Advanced options for creating a carousel project.
-            copy_from_project_id (str, optional): ID of project to copy from.
-
+            template_id (str, optional): ID of project to copy from. If you are using a template, you can omit all other parameters besides the name of the copy.
         Returns:
             project: new Project object
         '''
 
         Project._validate_questions(questions)
 
         questions_json = [q.to_dict() for q in questions]
@@ -107,16 +106,16 @@
             "num_workers_per_task": num_workers_per_task,
             "tags": tags
         }
         if carousel is not None:
             params = {**params, **carousel.to_dict()}
         if payment_per_response is not None:
             params["payment_per_response"] = payment_per_response
-        if copy_from_project_id is not None:
-            params["copy_from_project"] = copy_from_project_id
+        if template_id is not None:
+            params["template_id"] = template_id
         response_json = cls.post(PROJECTS_ENDPOINT, params)
         return cls(**response_json)
 
     @classmethod
     def list(cls, page: int = 1):
         '''
         Lists all projects you have created.
```

## Comparing `surge_api-1.1.1.dist-info/LICENSE` & `surge_api-1.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `surge_api-1.1.1.dist-info/METADATA` & `surge_api-1.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surge-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: Surge Python SDK
 Home-page: https://github.com/surge-ai/surge-python
 Author: Surge
 Author-email: team@surgehq.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

## Comparing `surge_api-1.1.1.dist-info/RECORD` & `surge_api-1.1.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 surge/__init__.py,sha256=nwW3UeCwjeg4ecB1NvB_7GsEpr8RJQJPVFRt_N7Xhz4,186
 surge/api_resource.py,sha256=e3kEVqMzkBJ3jZjBEFKGhWlqWYtbPKdXxeCRBXZT7Eo,2905
 surge/carousel.py,sha256=CLWol7VCMVZR_boGJvV4z2G03x12GErHhYO3FhyYSrw,734
 surge/errors.py,sha256=N83WpLlqrRi_Y03-q8JUXlutgCUpUrMeL47TvbOv11c,1606
-surge/projects.py,sha256=YRJ2AczwbyUGGwLxqGRQe5fOH2coi8cxYk_O-oaU2Sc,12092
+surge/projects.py,sha256=w4gbkCdKib163VDVcncWOG9fhgqhmi6LpzpGx5XHJyM,12142
 surge/questions.py,sha256=WX_pmvrGopKvd6V_s-RPngq-zSTYHcJVpzB87_yBa-Y,26952
 surge/reports.py,sha256=e5MqfkqhKeC8_c67QDtPTn8G3tQqcciEwxA9m6Ugaa4,5173
 surge/responses.py,sha256=uQIQj55KS2H334OBXIe59FFEerOnDuqk0MhTTUye-D4,939
 surge/tasks.py,sha256=prAA86aWwiWuoXA8j7z4dObdA1QHZdSWezAJMqs68l4,5799
 surge/teams.py,sha256=PhBjTRjkZwnvkGcaplFicNKwYVx7w_ryqKF9lPbV9_0,4107
 surge/utils.py,sha256=4SO3vQVwOOgn-mrDFmUH0HipfRJwcU8v5eTXp4uoZag,442
-surge_api-1.1.1.dist-info/LICENSE,sha256=n298NNjFKoaxocxZ1_4E-TJURJV1-MLq78cFp6bo2I0,1062
-surge_api-1.1.1.dist-info/METADATA,sha256=3qJen_eG-Ne41CvRsDBk6_vvMoG4JgZutlX2pj5lnJQ,3742
-surge_api-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-surge_api-1.1.1.dist-info/top_level.txt,sha256=jnubIyC0boBGzxSTRKNAKSVrVru3VgSHWf_q_qFRm_A,6
-surge_api-1.1.1.dist-info/RECORD,,
+surge_api-1.1.2.dist-info/LICENSE,sha256=n298NNjFKoaxocxZ1_4E-TJURJV1-MLq78cFp6bo2I0,1062
+surge_api-1.1.2.dist-info/METADATA,sha256=PSd3yls-rGQP5cFExP_g_d_UTFds6qvEjuWUjX00SeM,3742
+surge_api-1.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+surge_api-1.1.2.dist-info/top_level.txt,sha256=jnubIyC0boBGzxSTRKNAKSVrVru3VgSHWf_q_qFRm_A,6
+surge_api-1.1.2.dist-info/RECORD,,
```

