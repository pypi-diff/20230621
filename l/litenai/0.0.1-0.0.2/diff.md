# Comparing `tmp/litenai-0.0.1-py3-none-any.whl.zip` & `tmp/litenai-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,22 @@
-Zip file size: 18202 bytes, number of entries: 17
+Zip file size: 87170 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      539 b- defN 23-Jun-18 23:21 liten/__init__.py
--rw-r--r--  2.0 unx     7204 b- defN 23-Jun-18 23:28 liten/agent.py
--rw-r--r--  2.0 unx     6418 b- defN 23-Jun-16 03:48 liten/chatbot.py
+-rw-r--r--  2.0 unx     7295 b- defN 23-Jun-21 02:01 liten/agent.py
+-rw-r--r--  2.0 unx     6751 b- defN 23-Jun-21 01:58 liten/chatbot.py
 -rw-r--r--  2.0 unx     1750 b- defN 23-Jun-11 17:47 liten/config.py
 -rw-r--r--  2.0 unx     1009 b- defN 23-Jun-14 18:36 liten/database.py
 -rw-r--r--  2.0 unx     8246 b- defN 23-Jun-17 20:57 liten/demofiles.py
 -rw-r--r--  2.0 unx     1211 b- defN 23-May-06 21:10 liten/message.py
 -rw-r--r--  2.0 unx     8118 b- defN 23-Jun-11 17:47 liten/openai.py
 -rw-r--r--  2.0 unx     2089 b- defN 23-Jun-14 18:36 liten/plotdf.py
--rw-r--r--  2.0 unx     7410 b- defN 23-Jun-18 23:20 liten/session.py
+-rw-r--r--  2.0 unx     7627 b- defN 23-Jun-21 01:58 liten/session.py
 -rw-r--r--  2.0 unx     5106 b- defN 23-Jun-11 17:47 liten/storage.py
 -rw-r--r--  2.0 unx      904 b- defN 23-May-20 07:14 liten/utils.py
 -rw-r--r--  2.0 unx     2720 b- defN 23-Jun-18 23:28 liten/workitem.py
--rw-r--r--  2.0 unx      594 b- defN 23-Jun-20 00:44 litenai-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 00:44 litenai-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 00:44 litenai-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1241 b- defN 23-Jun-20 00:44 litenai-0.0.1.dist-info/RECORD
-17 files, 54657 bytes uncompressed, 16220 bytes compressed:  70.3%
+-rw-r--r--  2.0 unx    64037 b- defN 23-Jun-21 00:44 resources/SyslogAnalyze.ipynb
+-rw-r--r--  2.0 unx   200549 b- defN 23-Jun-21 00:44 resources/WeblogAnalyze.ipynb
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 22:21 resources/__init__.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Jun-21 02:03 litenai-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 02:03 litenai-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-21 02:03 litenai-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1492 b- defN 23-Jun-21 02:03 litenai-0.0.2.dist-info/RECORD
+20 files, 320124 bytes uncompressed, 84802 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -33,20 +33,29 @@
 
 Filename: liten/utils.py
 Comment: 
 
 Filename: liten/workitem.py
 Comment: 
 
-Filename: litenai-0.0.1.dist-info/METADATA
+Filename: resources/SyslogAnalyze.ipynb
 Comment: 
 
-Filename: litenai-0.0.1.dist-info/WHEEL
+Filename: resources/WeblogAnalyze.ipynb
 Comment: 
 
-Filename: litenai-0.0.1.dist-info/top_level.txt
+Filename: resources/__init__.py
 Comment: 
 
-Filename: litenai-0.0.1.dist-info/RECORD
+Filename: litenai-0.0.2.dist-info/METADATA
+Comment: 
+
+Filename: litenai-0.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: litenai-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: litenai-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## liten/agent.py

```diff
@@ -93,17 +93,18 @@
         workitem = self.get_workitem(item)
         if workitem is None:
             return  
         workitem.summarize()
         print(f"Workitem {item}: {workitem.summary()}\n")
     
     def summarize(self):
-        for workitem in self._workitems:
+        for item in range(0, len(self._workitems)):
+            workitem = self._workitems[item]
             workitem.summarize()
-            print(f"Workitem {workitem.item()}: {workitem.summary()}\n")
+            print(f"Workitem {item}: {workitem.summary()}\n")
         
     def replay(self, item):
         """
         Replay the queries of a work
         """
         workitem = self.get_workitem(item)
         if workitem is None:
@@ -120,16 +121,17 @@
             return
         s = workitem.explain()
         print(f"Work {id}: {s.strip()}\n")
         return
     
     def find_similar(self, prompt):
         syscontent = "Find a list of works below. Each work starts with work keyword followed by a number. It is followed by a short summary.\n"
-        for workitem in self._workitems:
-            syscontent += f"Work {workitem.item()} = {workitem.summarize()}\n"
+        for item in range(0, len(self._workitems)):
+            workitem = self._workitems[item]
+            syscontent += f"Work {item} = {workitem.summarize()}\n"
         rsyscontent = self.reduce_prompt_size(syscontent)
         chatprompt = "List the work closest to the following work summary.\n"
         chatprompt += prompt
         rchatprompt = self.reduce_prompt_size(chatprompt)
         msg = [
             {"role": "system", "content" : rsyscontent},
             {"role": "user", "content" : rchatprompt}
@@ -147,15 +149,16 @@
     def complete_data_chat(self, df, prompt):
         completed_chat = False
         if 'syslog' == self._name:
             try:
                 self.complete_syslog_data_chat(df, prompt)
                 completed_chat = True
             except:
-                print("Agent was syslog but data does not have syslog schema. Will use general schema.")
+                pass
+                #print("Agent was syslog but data does not have syslog schema. Will use general schema.")
         if not completed_chat:
             usercontent = f"""Find a log data file below. This starts with a triple quote like ``` and ends with triple quote ``` again. Each line is a single row of data. All fields in that row are separated by comma. Read this data and respond to the following prompt.
 {prompt}
 ```
             """
             num_cols = len(df.columns)
             for d in df.collect():
@@ -175,16 +178,16 @@
         usercontent = f"""Find a log data generated by Linux system log file. This starts with a triple quote like ``` and ends with triple quote ``` again. Read this data and respond to the following prompt.
 {prompt}
 ```
         """
         #  Jun 14 15:16:01 combo sshd(pam_unix)[19939]: authentication failure; logname= uid=0 euid=0 tty=NODEVssh ruser= rhost=218.188.2.4                
         for r in df.collect():
             timestr = ""
-            if r['timestamp']:
-                timestr = to_date(r['timestamp'],'MMM DD HH:mm:ss')           
+            if r['time']:
+                timestr = to_date(r['time'],'MMM DD HH:mm:ss')
             usercontent += f"""{timestr} {r['hostname']} {r['process']}({r['pid']}); {r['message']}\n"""
 
         rusercontent = self.reduce_prompt_size(usercontent)
         rusercontent += """```"""
         msg = [
             {"role": "user", "content" : rusercontent}
         ]
```

## liten/chatbot.py

```diff
@@ -8,17 +8,18 @@
 from pyspark.sql import SparkSession
 
 from io import StringIO
 from contextlib import redirect_stdout
 from contextlib import redirect_stderr
 
 class ChatBot:
-    def __init__(self, sc) -> None:
+    def __init__(self, spark, agent) -> None:
         pn.extension()
-        self._spark = sc
+        self._agent = agent
+        self._spark = spark
         self._df = None
         self._openai = OpenAI()
         self._panels = [] # Collect all display
         self._width = 1000 # Default pixel width
         self._context = [ {'role':'system', 
                             'content':"""
 You are a Bot, an automated service to talk to users. Your job is to analyze data files and \
@@ -118,16 +119,24 @@
             pandas_df = self._df.na.drop().toPandas()
             pandas_df['time'] = pd.to_datetime(pandas_df['time'])
             explorer_plot = hvplot.explorer(pandas_df)
             self._panels.append(explorer_plot)
         pass
 
     def _analyze_collect_messages(self,_):
+        prompt = self._inp.value_input
+        self._inp.value = ''
+        fout = StringIO()
+        ferr = StringIO()
+        with redirect_stdout(fout), redirect_stderr(ferr):
+            exec('self._agent.analyze(df=self._df, prompt=prompt)')
+        response = fout.getvalue()
+        response += ferr.getvalue()
         self._panels.append(
-            pn.Row('Bot:', pn.pane.Markdown('Action Analyze not yet supported', width=self._width, styles={'background-color': '#F6F6F6'}))
+            pn.Row('Bot:', pn.pane.Markdown(response, width=self._width, styles={'background-color': '#F6F6F6'}))
         )
         pass
     
     def _work_collect_messages(self,_):
         self._panels.append(
             pn.Row('Bot:', pn.pane.Markdown('Action Work not yet supported', width=self._width, styles={'background-color': '#F6F6F6'}))
         )
```

## liten/session.py

```diff
@@ -10,14 +10,17 @@
 from datetime import datetime
 import panel as pn
 import pandas as pd
 import hvplot
 import param
 import hvplot.pandas
 
+import importlib.resources as pkg_resources
+import resources
+
 from .openai import OpenAI
 from .agent import Agent
 from .database import Database
 from .chatbot import ChatBot
 from .config import Config
 from .demofiles import DemoFiles
 from .plotdf import PlotDf
@@ -39,27 +42,29 @@
         self._agents = {
             'common' : Agent('common',self._spark),
             'weblog' : Agent('weblog',self._spark),
             'syslog' : Agent('syslog',self._spark),
             'emailaccesslog' : Agent('emailaccesslog',self._spark)
         }
         self._agent = self._agents['common']
-        self._agents['weblog'].load('work/WeblogAnalyze.ipynb')
-        self._agents['syslog'].load('work/SyslogAnalyze.ipynb')
+        weblog_pynb = (pkg_resources.files(resources) / 'WeblogAnalyze.ipynb')
+        self._agents['weblog'].load(weblog_pynb)
+        syslog_pynb = (pkg_resources.files(resources) / 'SyslogAnalyze.ipynb')
+        self._agents['syslog'].load(syslog_pynb)
         self._openai = OpenAI()
         pass
 
     def _init_spark(self):
         """
         Initialize spark session
         """
         # TBD move all spark configs to yml file
-        # gives error for now "spark.sql.execution.arrow.enabled", "true"
         spark_config = SparkConf().setMaster("local[2]") \
                                     .setAppName('litendata.com') \
+                                    .set("spark.sql.execution.arrow.enabled", "true") \
                                     .set("spark.sql.legacy.timeParserPolicy", "LEGACY") \
                                     .set("spark.sql.debug.maxToStringFields", "100") \
                                     .set("spark.hadoop.delta.enableFastS3AListFrom", "true") \
                                     .set("spark.hadoop.fs.s3a.fast.upload", "true") \
                                     .set("spark.hadoop.fs.s3a.impl", "org.apache.hadoop.fs.s3a.S3AFileSystem") \
                                     .set("spark.hadoop.fs.s3a.connection.maximum", "1000") \
                                     .set("spark.hadoop.fs.s3a.connection.establish.timeout", self._config.s3_connection_timeout) \
@@ -122,15 +127,15 @@
         prompt: prompt to complete
         """
         resp = self._openai.complete_prompt_chat(prompt)
         print(resp)
         return
     
     def chatbot(self):
-        cbot = ChatBot(self._spark)
+        cbot = ChatBot(self._spark, self._agent)
         col_panel = cbot.start()
         return col_panel
     
     def _codegen(self, prompt, lang='sql'):
         code_str = None
         if lang == 'sql':
             code_str = self._agent.generate_sql(prompt)
```

## Comparing `litenai-0.0.1.dist-info/METADATA` & `litenai-0.0.2.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: litenai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Liten AI Data Platform
 Author: HK Verma
 Author-email: hkverma@litendata.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: botocore
 Requires-Dist: boto3
 Requires-Dist: langchain
-Requires-Dist: minio
 Requires-Dist: openai
 Requires-Dist: pandas
 Requires-Dist: panel
 Requires-Dist: hvplot
 Requires-Dist: python-dotenv
 Requires-Dist: tiktoken
```

## Comparing `litenai-0.0.1.dist-info/RECORD` & `litenai-0.0.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 liten/__init__.py,sha256=7ro9fopZ-bKwm8gTlCcBgEagMpKU_d30mxaUm02aycw,539
-liten/agent.py,sha256=p1y2d9X6yvXysCkKPPGvsuIF_3FqBEK9B28qy_4fYw0,7204
-liten/chatbot.py,sha256=YR0JcyBNOJgWWEUYV9urJ_avC5OOy-Fr3mAMpldMsVs,6418
+liten/agent.py,sha256=nKh985nFnH3FbucUTbUdBmVnsGWUgXXgo0UuVQMnUQA,7295
+liten/chatbot.py,sha256=moa7bT3PfGUFFJB0hBNdnwTmLhmMoN7iUyGl4uo5GHE,6751
 liten/config.py,sha256=c-vBDc73op0rqBlNqgrJluY395idgX0KKijoemVX-jc,1750
 liten/database.py,sha256=OgbwKDvW_lXGnmkuT2-SoXhEfnwmUZJ12ADkO29X034,1009
 liten/demofiles.py,sha256=JOMzFNn6wHsOGA8ZLL9DEZ6UCZaea6FI_N7Ffu1Cr5g,8246
 liten/message.py,sha256=nWY5brow8w1a9hbQ443JNXSVhk3flOjd1Cxms_ufpRA,1211
 liten/openai.py,sha256=d7_cCYERXykTdPPYcLMWURRu5itZdMbllbg1pGgGoaU,8118
 liten/plotdf.py,sha256=pDI8xWR0eb-gqpvfuRbOTTPSFR9BhI67VLT2YoGI5m8,2089
-liten/session.py,sha256=4BRtWMwCetAEZsExa4b_gAVIylK6gRdAberZcsTALXg,7410
+liten/session.py,sha256=FlevTmuM-3ySfGiq7zVta4pDL0i3VERJmxUahNV8J_c,7627
 liten/storage.py,sha256=Aek3JLHy8Ihtoo3GKexpT5VreGoOm4mwqaiHQS3GXqs,5106
 liten/utils.py,sha256=OJkV16YHz1kxNNBNU_fOCcX9QG01XxO49b0P7AW5Gvg,904
 liten/workitem.py,sha256=LvJi_yV_Qft7ZxklmVrWC2KtqfwLLxOLvdyM3VwOdh0,2720
-litenai-0.0.1.dist-info/METADATA,sha256=p8nMMWaP9Iu-eJnRIvNWMsRhh20Z0-HMPOEpbUL0pTk,594
-litenai-0.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-litenai-0.0.1.dist-info/top_level.txt,sha256=1e434378pw_VpnYeyO3fsUhPYj4d_BAox9LsSy1AyN4,6
-litenai-0.0.1.dist-info/RECORD,,
+resources/SyslogAnalyze.ipynb,sha256=n46r9PaKc-6zbsDx1ZV5Y2UXB6hrGiMON1BdgAoU--0,64037
+resources/WeblogAnalyze.ipynb,sha256=fzetLj3F0Pbu4qBhK0kghDL4Q91E2laOHmyIkoAL2jQ,200549
+resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+litenai-0.0.2.dist-info/METADATA,sha256=GcNKvrw3eyhFi_KtUP3fx6j5LQI1vtFDAz--sS2qfeU,573
+litenai-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+litenai-0.0.2.dist-info/top_level.txt,sha256=d49BG1ppukREYLpoOTg6dQxJpObTS1X6hXI70BJmgO8,16
+litenai-0.0.2.dist-info/RECORD,,
```

