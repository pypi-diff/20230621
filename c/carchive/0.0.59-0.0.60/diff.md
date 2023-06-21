# Comparing `tmp/carchive-0.0.59.tar.gz` & `tmp/carchive-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.59.tar", last modified: Mon May 22 11:57:32 2023, max compression
+gzip compressed data, was "carchive-0.0.60.tar", last modified: Wed Jun 21 16:52:40 2023, max compression
```

## Comparing `carchive-0.0.59.tar` & `carchive-0.0.60.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:57:32.196610 carchive-0.0.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-22 11:57:25.000000 carchive-0.0.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-22 11:57:32.196610 carchive-0.0.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 11:57:25.000000 carchive-0.0.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:57:32.196610 carchive-0.0.59/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10290 2023-05-22 11:57:25.000000 carchive-0.0.59/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:57:32.196610 carchive-0.0.59/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-22 11:57:32.000000 carchive-0.0.59/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 11:57:32.000000 carchive-0.0.59/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:57:32.000000 carchive-0.0.59/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 11:57:32.000000 carchive-0.0.59/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 11:57:32.000000 carchive-0.0.59/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:57:32.196610 carchive-0.0.59/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3358 2023-05-22 11:57:25.000000 carchive-0.0.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:52:40.182888 carchive-0.0.60/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-21 16:52:36.000000 carchive-0.0.60/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-21 16:52:40.178887 carchive-0.0.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 16:52:36.000000 carchive-0.0.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:52:40.178887 carchive-0.0.60/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11919 2023-06-21 16:52:36.000000 carchive-0.0.60/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:52:40.178887 carchive-0.0.60/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-21 16:52:40.000000 carchive-0.0.60/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-21 16:52:40.000000 carchive-0.0.60/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:52:40.000000 carchive-0.0.60/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-21 16:52:40.000000 carchive-0.0.60/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 16:52:40.000000 carchive-0.0.60/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:52:40.182888 carchive-0.0.60/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3358 2023-06-21 16:52:36.000000 carchive-0.0.60/setup.py
```

### Comparing `carchive-0.0.59/LICENSE` & `carchive-0.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.59/carchive/__init__.py` & `carchive-0.0.60/carchive/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os, requests, datetime, time, queue, threading, asyncio
 from copy import deepcopy as dc
 from threading import Lock
 from typing import Dict, List, Callable, Generic, TypeVar
 from abc import ABC, abstractmethod
-
+from fileinput import FileInput as finput
 import mystring,splittr
 import pause
 from github import Github, Repository
 import git2net
 import pygit2 as git2
+from contextlib import suppress
+
+GRepo_Saving_Progress_Lock = threading.Lock()
 
 class niceghapi(object):
 	def __init__(self):
 		self.cur_status = None
 		self.now = None
 		self.resetdate = None
 
@@ -215,16 +218,60 @@
 
 		def appr(string: mystring.string):
 			with open("mapping_file_{0}.csv".format(string.tobase64()), "a+") as writer:
 				writer.write(string)
 		self.appr = appr
 		self.api_watch = niceghapi()
 		self.delete_paths = delete_paths
-		asyncio.run(self.handle_git())
-	
+		self.query_string = None
+		self.tracking_repos = None
+		self.tracking_name = None
+		asyncio.run(self.handle_history())
+
+	@property
+	def localfilename(self):
+		if self.tracking_name is None:
+			self.tracking_name = mystring.string("query_progress_{0}.csv".format(
+				mystring.string("{query_string}".format(query_string=self.query_string)).tobase64())
+			)
+		return self.tracking_name
+
+
+	@property
+	def repos(self):
+		if self.tracking_repos is None:
+			self.tracking_repos = []
+			if os.path.exists(self.localfilename):
+				with open(self.localfilename, "r") as reader:
+					for line in reader:
+						ProjectItr, ProjectURL, ProjectScanned = line.split(",")
+						if ProjectScanned == "false":
+							self.tracking_repos.append(ProjectURL)
+			else:
+				self.tracking_repos = [x.clone_url for x in self.g.search_repositories(query=self.query_string)]
+		return self.tracking_repos
+
+	def save(self, current_project_url:str=None):
+		#Make Thread Safe
+		with GRepo_Saving_Progress_Lock:
+			if not os.path.exists(self.localfilename):
+				with open(self.localfilename, "w+") as writer:
+					writer.write("ProjectItr,ProjectURL,ProjectScanned\n")
+					for proj_itr, proj in enumerate(self.repos):
+						writer.write("{0},{1},false\n".format(proj_itr, proj))
+
+			if current_project_url is not None:
+				found = False
+				with finput(self.localfilename, inplace=True) as reader:
+					for line in reader:
+						if not found and current_project_url in line:
+							line = line.replace("false", "true")
+						print(line, end='')
+		return
+
 	@property
 	def timing(self):
 		self.api_watch.timing
 
 		extra_rate_limiting = self.g.get_rate_limit()
 		if hasattr(extra_rate_limiting, "search"):
 			search_limits = getattr(extra_rate_limiting, "search")
@@ -238,28 +285,29 @@
 		if create:
 			os.makedirs(path, exist_ok=True)
 
 	def __call__(self, search_string:str):
 		self.timing
 		search_string = mystring.string(search_string)
 
-		def process_prep(repo_itr:int, repo:Repository, search_string:str, appr:Callable, fin_queue:queue.Queue):
+		def process_prep(repo_itr:int, repo_clone_url:str, search_string:str, appr:Callable, fin_queue:queue.Queue):
+			self.query_string = search_string
 			def process():
 				name = mystring.string("ITR>{0}_URL>{1}_STR>{2}\n".format(
-					repo_itr, repo.url, search_string
+					repo_itr, repo_clone_url, search_string
 				))
 				repo_dir = "repo_" + str(name.tobase64())
 				results_dir = "results_" + str(name.tobase64())
 
 				self.repair(repo_dir, create=False)
 				self.repair(results_dir)
 
 				sqlite_db_file = os.path.join(results_dir, "git_to_net.sqlite")
 
-				git2.clone_repository(repo.clone_url, repo_dir)  # Clones a non-bare repository
+				git2.clone_repository(repo_clone_url, repo_dir)  # Clones a non-bare repository
 
 				if self.num_processes is None:
 					git2net.mine_git_repo(repo_dir, sqlite_db_file)
 				else:
 					git2net.mine_git_repo(repo_dir, sqlite_db_file, no_of_processes=self.num_processes)
 				
 				git2net.mining_state_summary(repo_dir, sqlite_db_file)
@@ -270,40 +318,36 @@
 					with mystring.foldentre(new_path=results_dir):
 						raw_db_file = sqlite_db_file.replace(results_dir, '')
 						splittr.hash(raw_db_file)
 						splittr.split(raw_db_file, 50_000_000)
 						splittr.template(raw_db_file+".py")
 
 				appr(mystring.string(name.replace(',',';').replace('_',',').strip()))
-				fin_queue.put(repo)
+				fin_queue.put(repo_clone_url)
 
 			return process
 
-		repos = self.g.search_repositories(query=search_string)
-		self.total_repo_len = repos.totalCount
-		if self.total_repo_len > 0:
-			for repo_itr, repo in enumerate(repos):
-				self.processor += process_prep(repo_itr, repo, search_string, self.appr, self.processed_paths)
+		if len(self.repos) > 0:
+			for repo_itr, repo_url in enumerate(self.repos):
+				self.processor += process_prep(repo_itr, repo_url, search_string, self.appr, self.processed_paths)
 				self.current_repo_itr = repo_itr
 		else:
 			print("No Repos Found")
 
 	def login(self):
 		os.environ['GH_TOKEN'] = self.token
-		try:
+		with suppress(Exception):
 			with open("~/.bashrc", "a+") as writer:
 				writer.write("GH_TOKEN={0}".format(self.token))
-		except:
-			pass
 
 	@property
 	def complete(self):
 		return self.total_repo_len == self.current_repo_itr and self.processor.complete
 
-	async def handle_git(self):
+	async def handle_history(self):
 		while not self.complete:
 			# Get up to 5 strings from the queue
 			paths,num_waiting = [], 5
 			while len(paths) < num_waiting:
 				try:
 					path = self.processed_paths.get()
 					paths.append(path)
@@ -313,8 +357,11 @@
 
 			# Process the strings
 			for path in paths:
 				mystring.string("git add {0}".format(path)).exec()
 			mystring.string("git commit -m \"Added multiple paths\"").exec()
 			mystring.string("git push").exec()
 			for path in paths:
-				mystring.string("yes|rm -r {0}".format(path)).exec()
+				mystring.string("yes|rm -r {0}".format(path)).exec()
+
+			for path in paths:
+				self.save(path)
```

### Comparing `carchive-0.0.59/setup.py` & `carchive-0.0.60/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.59"
+VERSION = "0.0.60"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

