# Comparing `tmp/plm-dgraham-0.3.4.tar.gz` & `tmp/plm-dgraham-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plm-dgraham-0.3.4.tar", last modified: Sat Mar 11 14:14:04 2023, max compression
+gzip compressed data, was "plm-dgraham-0.4.0.tar", last modified: Wed Jun 21 08:52:30 2023, max compression
```

## Comparing `plm-dgraham-0.3.4.tar` & `plm-dgraham-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-03-11 14:14:04.511849 plm-dgraham-0.3.4/
--rw-r--r--   0 dag        (501) staff       (20)    13502 2023-03-11 14:14:04.511635 plm-dgraham-0.3.4/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)    12593 2022-12-17 20:12:33.000000 plm-dgraham-0.3.4/README.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-03-11 14:14:04.510808 plm-dgraham-0.3.4/plm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2022-09-15 18:04:30.000000 plm-dgraham-0.3.4/plm/__init__.py
--rw-r--r--   0 dag        (501) staff       (20)     4634 2022-10-03 17:52:36.000000 plm-dgraham-0.3.4/plm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-03-11 14:13:53.000000 plm-dgraham-0.3.4/plm/__version__.py
--rw-r--r--   0 dag        (501) staff       (20)    47028 2023-03-11 14:13:53.000000 plm-dgraham-0.3.4/plm/plm.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-03-11 14:14:04.511418 plm-dgraham-0.3.4/plm_dgraham.egg-info/
--rw-r--r--   0 dag        (501) staff       (20)    13502 2023-03-11 14:14:04.000000 plm-dgraham-0.3.4/plm_dgraham.egg-info/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)      292 2023-03-11 14:14:04.000000 plm-dgraham-0.3.4/plm_dgraham.egg-info/SOURCES.txt
--rw-r--r--   0 dag        (501) staff       (20)        1 2023-03-11 14:14:04.000000 plm-dgraham-0.3.4/plm_dgraham.egg-info/dependency_links.txt
--rw-r--r--   0 dag        (501) staff       (20)       42 2023-03-11 14:14:04.000000 plm-dgraham-0.3.4/plm_dgraham.egg-info/entry_points.txt
--rw-r--r--   0 dag        (501) staff       (20)      134 2023-03-11 14:14:04.000000 plm-dgraham-0.3.4/plm_dgraham.egg-info/requires.txt
--rw-r--r--   0 dag        (501) staff       (20)        4 2023-03-11 14:14:04.000000 plm-dgraham-0.3.4/plm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-03-11 14:14:04.511892 plm-dgraham-0.3.4/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4570 2023-03-11 14:13:53.000000 plm-dgraham-0.3.4/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 08:52:30.957371 plm-dgraham-0.4.0/
+-rw-r--r--   0 dag        (501) staff       (20)    12679 2023-06-21 08:52:30.957186 plm-dgraham-0.4.0/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)    11770 2023-06-21 08:52:11.000000 plm-dgraham-0.4.0/README.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 08:52:30.956417 plm-dgraham-0.4.0/plm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2022-09-15 18:04:30.000000 plm-dgraham-0.4.0/plm/__init__.py
+-rw-r--r--   0 dag        (501) staff       (20)     4634 2022-10-03 17:52:36.000000 plm-dgraham-0.4.0/plm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-21 08:52:11.000000 plm-dgraham-0.4.0/plm/__version__.py
+-rw-r--r--   0 dag        (501) staff       (20)    47734 2023-06-21 08:52:11.000000 plm-dgraham-0.4.0/plm/plm.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 08:52:30.957020 plm-dgraham-0.4.0/plm_dgraham.egg-info/
+-rw-r--r--   0 dag        (501) staff       (20)    12679 2023-06-21 08:52:30.000000 plm-dgraham-0.4.0/plm_dgraham.egg-info/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)      292 2023-06-21 08:52:30.000000 plm-dgraham-0.4.0/plm_dgraham.egg-info/SOURCES.txt
+-rw-r--r--   0 dag        (501) staff       (20)        1 2023-06-21 08:52:30.000000 plm-dgraham-0.4.0/plm_dgraham.egg-info/dependency_links.txt
+-rw-r--r--   0 dag        (501) staff       (20)       42 2023-06-21 08:52:30.000000 plm-dgraham-0.4.0/plm_dgraham.egg-info/entry_points.txt
+-rw-r--r--   0 dag        (501) staff       (20)      134 2023-06-21 08:52:30.000000 plm-dgraham-0.4.0/plm_dgraham.egg-info/requires.txt
+-rw-r--r--   0 dag        (501) staff       (20)        4 2023-06-21 08:52:30.000000 plm-dgraham-0.4.0/plm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-21 08:52:30.957403 plm-dgraham-0.4.0/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4570 2023-03-11 14:13:53.000000 plm-dgraham-0.4.0/setup.py
```

### Comparing `plm-dgraham-0.3.4/PKG-INFO` & `plm-dgraham-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plm-dgraham
-Version: 0.3.4
+Version: 0.4.0
 Summary: player lineup manager
 Home-page: https://github.com/dagraham/plm-dgraham
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -72,85 +72,63 @@
 
 and then install *plm* itself
 
         ~ % python3 -m pip install -U plm-dgraham
 
 This will install *plm* and any needed supporting python modules. This same can also also be used to update *plm* when a new version becomes available.
 
-### For use in a virtual environment
+### For use in an isolated environment {#For-use-in-an-isolated-environment}
 
-Setting up a virtual environment for *plm* is only slightly more complicated. The steps for OS/X or linux are illustrated below. For details see [python-virtual-environments-a-primer](https://www.google.com/url?q=https%3A%2F%2Frealpython.com%2Fpython-virtual-environments-a-primer%2F&sa=D&sntz=1&usg=AFQjCNFh7QpJQ4rPCDjZ1eLrV1BRCCpSmw).
+Installing etm in an isolated or virtual environment (sandbox) is only slightly more complicated. Begin by using *pip* to install *pipx*:
 
-Open a terminal and begin by creating a new directory/folder for the virtual environment, say `plm-pypi`, in your home directory:
+    $ python3 -m pip install -U pipx
 
-        % mkdir ~/plm-pypi
-        % cd ~/plm-pypi
+Now run:
 
-Now continue by creating the virtual environment:
+    $ pipx ensurepath
 
-        % python3 -m venv env
+to ensure that directories necessary for *pipx* operation are in your PATH environment variable and finally to install *etm* itself:
 
-After a few seconds you will have a new `./env` directory. Now activate the virtual environment:
+    $ pipx install plm-dgraham
 
-        % source env/bin/activate
-
-The prompt will now change to something containing `(env)` to indicate that the virtual environment is active. Updating pip is now recommended:
-
-        (env) % pip install -U pip
-
-Note that this invokes `./env/bin/pip`. Once this is finished, use pip to install etm:
-
-        (env) % pip install -U plm-dgraham
-
-This will install *plm* and all its requirements in
-
-        ./env/lib/python3.x/sitepackages
-
-and will also install an executable called `plm` in `./env/bin`. This same command can be used to update *plm* when a new version becomes available.
-
-The virtual environment only affects the terminal window in which it was activated and can be deactivated, if you wish, by using:
-
-        (env) % deactivate
+To upgrade *etm* when a new version becomes available, simply replace "install" in this command with "upgrade".
 
 ## Starting *plm*
 
-If using a virtual environment, first change to that directory and activate the virtual environment, if necessary:
-
-        % cd ~/plm
-        % source env/bin/activate
-        (env) % plm
-
-Otherwise, just invoke *plm* directly
+Either way, you can then start *etm* with
 
-        % plm
+    $ plm <path to home>
 
-Either way, you will see something like this
+and you will see something like this
 
-        Player Lineup Manager (0.3.0)
+        Player Lineup Manager (0.3.4)
         home directory: ~/plm
+        project: The active project has not yet been chosen.
+        Use command 'c' to create one or 'p' to select one.
 
         commands:
             h:  show this help message
             H:  show on-line documentation
             e:  edit 'roster.yaml' using the default text editor
-            p:  create/update a project                           (1)
+            c:  create/update a project                           (1)
+            p:  select the active project from existing projects  (1)
             a:  ask players for their "can play" dates            (2)
             r:  record the "can play" responses                   (3)
-            s:  schedule play using the "can play" responses      (4)
-            d:  deliver the schedule to the players               (5)
+            n:  nag players to submit can play responses          (4)
+            s:  schedule play using the "can play" responses      (5)
+            d:  deliver the schedule to the players               (6)
             v:  view the current settings of a project
             u:  check for an update to a later plm version
-            l:  clear the screen
             q:  quit
 
         command:
 
 This begins a loop in which *plm* waits for you to enter a command at the prompt, processes the command and, unless the command *q* (quit) is given, waits for your next command.
 
-Note: the commands *p*, *a*, *r*, *s*, *d* and *v* begin with a request that you select the relevant project. Tab completion is available and, once a selection is made, this project becomes the *default project* for any further use of the commands in this group while the command loop continues.
+Note: the commands *a*, *r*, *s*, *d* and *v* begin with a request that you select the *active project* if you have not already done so with either *c* or *p*. Tab completion is available and, once a selection is made, this project becomes the *active project* for any further use of the commands in this group while the command loop continues.
 
 ### The Player Directory: roster.yaml
 
 This file is the directory for the players in all of your projects. It should be populated with all the relevant players for a project before you create the project itself.
 
 You can open `roster.yaml` in your favorite editor or use command *e*:
 
@@ -171,17 +149,17 @@
 It is worth devoting some thought to the *tag* scheme you will use before you start adding players. My schedules involve groups that play on a particular week day so I tend to use tags for the week day that the group plays, e.g., `mon` for the group that plays on *Monday*. Note that tags are case sensitive so `mon`, `Mon` and `MON` are all different tags.
 
 
 ### A New Project From Start to Finish
 
 #### 1. Create the project file
 
-Start *plm*, if necessary, and use the *project* command:
+Start *plm*, if necessary, and use the *create project* command:
 
-        command: p
+        command: c
 
 Then follow the on-line prompts to enter the project information. This information will be stored in a new file in the projects directory, `<project_name>.yaml`, where `<project_name>` is the name you provide for the project. A short name that sorts well and is suggestive is recommended, e.g., `2022-4Q-TU`.
 
 
 #### 2. Request players' availability dates
 
 With the project file created, the next step is to request the "can play" dates from the players. To do this start *plm*, if necessary, and use the *ask* command:
```

### Comparing `plm-dgraham-0.3.4/README.md` & `plm-dgraham-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -49,85 +49,63 @@
 
 and then install *plm* itself
 
         ~ % python3 -m pip install -U plm-dgraham
 
 This will install *plm* and any needed supporting python modules. This same can also also be used to update *plm* when a new version becomes available.
 
-### For use in a virtual environment
+### For use in an isolated environment {#For-use-in-an-isolated-environment}
 
-Setting up a virtual environment for *plm* is only slightly more complicated. The steps for OS/X or linux are illustrated below. For details see [python-virtual-environments-a-primer](https://www.google.com/url?q=https%3A%2F%2Frealpython.com%2Fpython-virtual-environments-a-primer%2F&sa=D&sntz=1&usg=AFQjCNFh7QpJQ4rPCDjZ1eLrV1BRCCpSmw).
+Installing etm in an isolated or virtual environment (sandbox) is only slightly more complicated. Begin by using *pip* to install *pipx*:
 
-Open a terminal and begin by creating a new directory/folder for the virtual environment, say `plm-pypi`, in your home directory:
+    $ python3 -m pip install -U pipx
 
-        % mkdir ~/plm-pypi
-        % cd ~/plm-pypi
+Now run:
 
-Now continue by creating the virtual environment:
+    $ pipx ensurepath
 
-        % python3 -m venv env
+to ensure that directories necessary for *pipx* operation are in your PATH environment variable and finally to install *etm* itself:
 
-After a few seconds you will have a new `./env` directory. Now activate the virtual environment:
+    $ pipx install plm-dgraham
 
-        % source env/bin/activate
-
-The prompt will now change to something containing `(env)` to indicate that the virtual environment is active. Updating pip is now recommended:
-
-        (env) % pip install -U pip
-
-Note that this invokes `./env/bin/pip`. Once this is finished, use pip to install etm:
-
-        (env) % pip install -U plm-dgraham
-
-This will install *plm* and all its requirements in
-
-        ./env/lib/python3.x/sitepackages
-
-and will also install an executable called `plm` in `./env/bin`. This same command can be used to update *plm* when a new version becomes available.
-
-The virtual environment only affects the terminal window in which it was activated and can be deactivated, if you wish, by using:
-
-        (env) % deactivate
+To upgrade *etm* when a new version becomes available, simply replace "install" in this command with "upgrade".
 
 ## Starting *plm*
 
-If using a virtual environment, first change to that directory and activate the virtual environment, if necessary:
-
-        % cd ~/plm
-        % source env/bin/activate
-        (env) % plm
-
-Otherwise, just invoke *plm* directly
+Either way, you can then start *etm* with
 
-        % plm
+    $ plm <path to home>
 
-Either way, you will see something like this
+and you will see something like this
 
-        Player Lineup Manager (0.3.0)
+        Player Lineup Manager (0.3.4)
         home directory: ~/plm
+        project: The active project has not yet been chosen.
+        Use command 'c' to create one or 'p' to select one.
 
         commands:
             h:  show this help message
             H:  show on-line documentation
             e:  edit 'roster.yaml' using the default text editor
-            p:  create/update a project                           (1)
+            c:  create/update a project                           (1)
+            p:  select the active project from existing projects  (1)
             a:  ask players for their "can play" dates            (2)
             r:  record the "can play" responses                   (3)
-            s:  schedule play using the "can play" responses      (4)
-            d:  deliver the schedule to the players               (5)
+            n:  nag players to submit can play responses          (4)
+            s:  schedule play using the "can play" responses      (5)
+            d:  deliver the schedule to the players               (6)
             v:  view the current settings of a project
             u:  check for an update to a later plm version
-            l:  clear the screen
             q:  quit
 
         command:
 
 This begins a loop in which *plm* waits for you to enter a command at the prompt, processes the command and, unless the command *q* (quit) is given, waits for your next command.
 
-Note: the commands *p*, *a*, *r*, *s*, *d* and *v* begin with a request that you select the relevant project. Tab completion is available and, once a selection is made, this project becomes the *default project* for any further use of the commands in this group while the command loop continues.
+Note: the commands *a*, *r*, *s*, *d* and *v* begin with a request that you select the *active project* if you have not already done so with either *c* or *p*. Tab completion is available and, once a selection is made, this project becomes the *active project* for any further use of the commands in this group while the command loop continues.
 
 ### The Player Directory: roster.yaml
 
 This file is the directory for the players in all of your projects. It should be populated with all the relevant players for a project before you create the project itself.
 
 You can open `roster.yaml` in your favorite editor or use command *e*:
 
@@ -148,17 +126,17 @@
 It is worth devoting some thought to the *tag* scheme you will use before you start adding players. My schedules involve groups that play on a particular week day so I tend to use tags for the week day that the group plays, e.g., `mon` for the group that plays on *Monday*. Note that tags are case sensitive so `mon`, `Mon` and `MON` are all different tags.
 
 
 ### A New Project From Start to Finish
 
 #### 1. Create the project file
 
-Start *plm*, if necessary, and use the *project* command:
+Start *plm*, if necessary, and use the *create project* command:
 
-        command: p
+        command: c
 
 Then follow the on-line prompts to enter the project information. This information will be stored in a new file in the projects directory, `<project_name>.yaml`, where `<project_name>` is the name you provide for the project. A short name that sorts well and is suggestive is recommended, e.g., `2022-4Q-TU`.
 
 
 #### 2. Request players' availability dates
 
 With the project file created, the next step is to request the "can play" dates from the players. To do this start *plm*, if necessary, and use the *ask* command:
```

### Comparing `plm-dgraham-0.3.4/plm/__main__.py` & `plm-dgraham-0.4.0/plm/__main__.py`

 * *Files identical despite different names*

### Comparing `plm-dgraham-0.3.4/plm/plm.py` & `plm-dgraham-0.4.0/plm/plm.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,21 +84,25 @@
     else:
         logger.debug(f"ok False; res: '{res}'")
         show_message('goto', f"failed to open '{path}'")
     return
 
 
 def get_project(default_project=""):
+    # clear_screen()
+    project = os.path.split(default_project)[1] if default_project else ""
+    print("Select the active project.")
     possible = [x for x in os.listdir(plm_projects) if os.path.splitext(x)[1] == '.yaml']
     possible.sort()
     completer = FuzzyWordCompleter(possible)
-    proj = prompt("project: ", completer=completer, default=default_project).strip()
+    proj = prompt("project: ", completer=completer, default=project).strip()
     proj = proj if proj.endswith('.yaml') else proj + '.yaml'
     project = os.path.join(plm_projects, proj)
     if os.path.isfile(project):
+        clear_screen()
         return project
     else:
         print(f"project '{project}' not found")
         return None
 
 
 def get_dates(label, year, month, default):
@@ -220,80 +224,96 @@
         openWithDefault(project)
 
 def open_readme():
     help_link = "https://dagraham.github.io/plm-dgraham/"
     openWithDefault(help_link)
 
 def main():
+    default_project = clear_screen(default_project="")
+    project = "{default_project}" if default_project else "not yet selected"
 
     commands = """
 commands:
     h:  show this help message
     H:  show on-line documentation
     e:  edit 'roster.yaml' using the default text editor
-    p:  create/update a project                           (1)
+    c:  create/update a project                           (1)
+    p:  select the active project from existing projects  (1)
     a:  ask players for their "can play" dates            (2)
     r:  record the "can play" responses                   (3)
     n:  nag players to submit can play responses          (4)
     s:  schedule play using the "can play" responses      (5)
     d:  deliver the schedule to the players               (6)
     v:  view the current settings of a project
     u:  check for an update to a later plm version
-    l:  clear the screen
     q:  quit
 """
 
-    help = f"""\
-Player Lineup Manager ({plm_version})
-home directory: {plm_home}
-{commands}"""
+    # help = f"""\
+# Player Lineup Manager ({plm_version})
+# home directory: {plm_home}
+# selected project: {project}
+# {commands}"""
 
-    print(help)
-    default_project = ""
     try:
         again = True
         while again:
+            if default_project:
+                project = os.path.split(default_project)[1]
+            else:
+                project = """\
+The active project has not yet been chosen.
+Use command 'c' to create one or 'p' to select one.
+"""
+            help = f"""\
+Player Lineup Manager ({plm_version})
+home directory: {plm_home}
+project: {project}
+{commands}"""
+            print(help)
             answer = input("command: ").strip()
-            if answer not in 'lhevpnarsdouq?H':
+            if answer not in 'clhevpnarsdouq?H':
                 print(f"invalid command: '{answer}'")
                 print(commands)
             elif answer in ['h', '?']:
-                print(help)
+                clear_screen()
             elif answer == 'H':
                 open_readme()
             elif answer == 'u':
                 res = check_update()
-                print(res)
+                print(f"\n{res}\n")
             elif answer == 'q':
                 again = False
                 print("quitting plm ...")
             else:
                 if answer == 'e':
                     edit_roster()
                 elif answer == 'o':
                     default_project = open_project(default_project)
                 elif answer == 'v':
                     default_project = view_project(default_project)
-                elif answer == 'p':
+                elif answer == 'c':
                     default_project = create_project(default_project)
+                elif answer == 'p':
+                    default_project = get_project(default_project)
                 elif answer == 'a':
                     default_project = ask_players(default_project)
                 elif answer == 'n':
                     default_project = nag_players(default_project)
                 elif answer == 'r':
                     default_project = record_responses(default_project)
                 elif answer == 's':
                     default_project = create_schedule(default_project)
                 elif answer == 'd':
                     default_project = deliver_schedule(default_project)
                 elif answer == 'l':
                     default_project = clear_screen(default_project)
-                    print(help)
-                if default_project:
-                    print(f"default project: {default_project}")
+                    # print(help)
+                # if default_project:
+                #     print(f"default project: {default_project}")
 
     except KeyboardInterrupt:
         play = False
         print("\nquitting plm ...")
 
 
 def check_update():
@@ -314,41 +334,43 @@
             res = f"An update is available from {plm_version} (installed) to {url_version}"
         else:
             res = f"The installed version of plm, {plm_version}, is the latest available."
 
     return res
 
 def view_project(default_project=""):
+    if not default_project:
+        print("The first step is to select the project.")
+        default_project = get_project(default_project)
+        if not default_project:
+            print("Cancelled")
+            return
 
-    print("Select the project to be viewed.")
-    project = get_project(default_project)
-    if not project:
-        print("Cancelled")
-        return default_project
-    with open(project) as fo:
+    with open(default_project) as fo:
         lines = fo.readlines()
-    project_name = os.path.split(project)[1]
+    project_name = os.path.split(default_project)[1]
     border_length = min(18, (COLUMNS - len(project_name) - 10)//2)
     markers = "="*border_length
     print(f"{markers} begin {project_name} {markers}")
     print("".join(lines))
     print(f"{markers}= end {project_name} ={markers}")
 
-    return os.path.split(project)[1]
+    return default_project
 
 
 def create_project(default_project=""):
-    # Create prompt object.
+    clear_screen()
     session = PromptSession()
     problems = []
     if not os.path.exists(plm_roster):
         problems.append(f"Could not find {plm_roster}")
     if not os.path.exists(plm_projects) or not os.path.isdir(plm_projects):
         problems.append(f"Either {plm_projects} does not exist or it is not a directory")
     if problems:
+        print(f"problems: {problems}")
         sys.exit(problems)
 
     with open(plm_roster, 'r') as fo:
         roster_data = yaml.load(fo)
 
     tags = set([])
     players = {}
@@ -376,26 +398,26 @@
     # creating a new project
     possible = [x for x in os.listdir(plm_projects) if os.path.splitext(x)[1] == '.yaml']
     possible.sort()
     completer = FuzzyWordCompleter(possible)
     proj = prompt("project: ", completer=completer, default=default_project).strip()
     if not proj:
         sys.exit("canceled")
-    default_project = proj
 
 
     project_name = os.path.join(plm_projects, proj)
 
     project_file = os.path.join(plm_projects, os.path.splitext(project_name)[0] + '.yaml')
+    default_project = project_file
 
     if os.path.exists(project_file):
         print(f"using defaults from the existing: {project_file}")
         ok = session.prompt(f"modify {project_file}: [Yn] ").strip()
         if ok.lower() == 'n':
-            sys.exit("canceled")
+            return default_project
         # get defaults from existing project file
         with open(project_file, 'r') as fo:
             yaml_data = yaml.load(fo)
 
         TITLE = yaml_data['TITLE']
         TAG = yaml_data['PLAYER_TAG']
         REPLY_BY = yaml_data['REPLY_BY']
@@ -529,15 +551,15 @@
     rep_date = rep_dt.format("hA on dddd, MMMM D")
     rep_DATE = rep_dt.format("hA on dddd, MMMM D, YYYY")
 
     eg_day = pendulum.instance(days[1])
     eg_yes = eg_day.format("M/D")
     eg_no = eg_day.format("MMMM D")
 
-    tmpl = f"""# created by plm -p
+    tmpl = f"""# created by plm -c
 TITLE: {title}
 PLAYER_TAG: {tag}
 REPLY_BY: {reply_formatted}
 REPEAT: {repeat}
 DAY: {day}
 BEGIN: {beginning_formatted}
 END: {ending_formatted}
@@ -674,14 +696,23 @@
             freq[new][name] += 1
         chosen.append(new)
         remaining.remove(new)
 
     return freq, chosen, remaining
 
 def create_schedule(default_project=""):
+    if not default_project:
+        print("The first step is to select the project.")
+        default_project = get_project(default_project)
+        if not default_project:
+            print("Cancelled")
+            return
+    with open(default_project) as fo:
+        yaml_data = yaml.load(fo)
+
     possible = {}
     available = {}
     availabledates = {}
     availablebydates = {}
     substitutebydates = {}
     unselected = {}
     opportunities = {}
@@ -699,27 +730,18 @@
     notresponded = []
     dates_scheduled = []
     dates_notscheduled= []
     unavailable = {}
     project_hsh = {}
     courts_scheduled = {}
     session = PromptSession()
-    proj_path = get_project(default_project)
+    proj_path = default_project
     now = pendulum.now()
     cur_year = now.year
     cur_month = now.month
-    if not proj_path:
-        print("Cancelled")
-        return
-    if not os.path.isfile(proj_path):
-        print(f"project '{proj_path}' not found")
-        return
-    default_project = os.path.split(proj_path)[1]
-    with open(proj_path, 'r') as fo:
-        yaml_data = yaml.load(fo)
 
     TITLE = yaml_data['TITLE']
     responses = yaml_data['RESPONSES']
     addresses = yaml_data['ADDRESSES']
     DATES = yaml_data['DATES']
     NUM_PLAYERS = yaml_data['NUM_PLAYERS']
     # TAG = yaml_data['PLAYER_TAG']
@@ -1054,35 +1076,36 @@
     output.append(wrap_format(schdatestr))
     output.append('')
 
     schedule = "\n".join(output)
 
     yaml_data['SCHEDULE'] = schedule
 
-    with open(proj_path, 'w') as fn:
+    with open(default_project, 'w') as fn:
         # yaml.default_flow_style = None
         # yaml.indent(mapping=2, sequence=4, offset=2)
         yaml.dump(yaml_data, fn)
         print(f"Schedule saved to {proj_path}")
 
     return default_project
 
 
 def ask_players(default_project=""):
+    if not default_project:
+        print("The first step is to select the project.")
+        default_project = get_project(default_project)
+        if not default_project:
+            print("Cancelled")
+            return
+    clear_screen()
     print("""
 This will help you prepare an email to request can play dates
 from the relevant players.""")
 
-    print("The first step is to select the project.")
-    project = get_project(default_project)
-    if not project:
-        print("Cancelled")
-        return
-    default_project = os.path.split(project)[1]
-    with open(project) as fo:
+    with open(default_project) as fo:
         yaml_data = yaml.load(fo)
 
     print("""The next step is to
 1) open your favorite email application,
 2) create a new email and
 3) be ready to paste
   (a) the addresses
@@ -1264,48 +1287,54 @@
     ok = prompt("Has the SCHEDULE been pasted? ", default='yes')
     if not ok == 'yes':
         print("Cancelled")
         return
 
 
 def record_responses(default_project=""):
-
-    project = get_project(default_project)
-    if not project:
-        print("Cancelled")
-        return default_project
-    default_project = os.path.split(project)[1]
-    with open(project) as fo:
+    if not default_project:
+        print("The first step is to select the project.")
+        default_project = get_project(default_project)
+        if not default_project:
+            print("Cancelled")
+            return
+    with open(default_project) as fo:
         yaml_data = yaml.load(fo)
 
 
     RESPONSES = yaml_data['RESPONSES']
     DATES = yaml_data['DATES']
     PLAYER_TAG = yaml_data['PLAYER_TAG']
 
     players = FuzzyWordCompleter([x for x in RESPONSES] + ['.', '?'])
 
     again = True
     player_default = ""
     print(f"""\
+Entering responses for project {os.path.split(default_project)[1]}
+
 The response for a player should be 'all', 'none', 'nr' (no reply)
 or a comma separated list of CAN PLAY DATES using the month/day
 format. Asterisks can be appended to dates in which the player
 wants to be listed as a sub, e.g., '{DATES[0]}, {DATES[2]}*, {DATES[3]}'.
 
 dates: {wrap_format(", ".join(DATES))}
 player tag: {PLAYER_TAG}
 """)
 
     changes = ""
     while again:
+
         if changes:
-            print("Enter player's name, '?' to review current responses\nor '.' to stop recording responses and (optionally) save changes.")
-        else:
-            print("Enter player's name, '?' to review current responses\nor '.' to stop recording responses.")
+            with open(default_project, 'w') as fn:
+                yaml.dump(yaml_data, fn)
+            print(f"saved changes: {changes}")
+            changes = ""
+
+        print("Enter player's name, '?' to review current responses\nor '.' to stop recording responses.")
         player = prompt("player: ", completer=players).strip()
         if player == '.':
             again = False
             continue
         if player == '?':
             # show responses recorded thus far
             count = 0
@@ -1359,25 +1388,14 @@
 
             new = RESPONSES[player]
             if isinstance(new, list):
                 new = ", ".join(new)
             if new != default:
                 changes += f"  {player}: {new}\n"
 
-    if changes:
-        print(f"Changes:\n{changes}")
-        ok = prompt("Save changes: [Yn] ").strip()
-        if ok.lower() == 'n':
-            sys.exit("changes discarded")
-        with open(project, 'w') as fn:
-            # yaml.default_flow_style = None
-            # yaml.indent(mapping=2, sequence=4, offset=2)
-            yaml.dump(yaml_data, fn)
-    else:
-        print("no changes to save")
     return default_project
 
 
 
 def print_head(s):
     print("{0}".format(s.upper()))
     print("="*len(s))
```

### Comparing `plm-dgraham-0.3.4/plm_dgraham.egg-info/PKG-INFO` & `plm-dgraham-0.4.0/plm_dgraham.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plm-dgraham
-Version: 0.3.4
+Version: 0.4.0
 Summary: player lineup manager
 Home-page: https://github.com/dagraham/plm-dgraham
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -72,85 +72,63 @@
 
 and then install *plm* itself
 
         ~ % python3 -m pip install -U plm-dgraham
 
 This will install *plm* and any needed supporting python modules. This same can also also be used to update *plm* when a new version becomes available.
 
-### For use in a virtual environment
+### For use in an isolated environment {#For-use-in-an-isolated-environment}
 
-Setting up a virtual environment for *plm* is only slightly more complicated. The steps for OS/X or linux are illustrated below. For details see [python-virtual-environments-a-primer](https://www.google.com/url?q=https%3A%2F%2Frealpython.com%2Fpython-virtual-environments-a-primer%2F&sa=D&sntz=1&usg=AFQjCNFh7QpJQ4rPCDjZ1eLrV1BRCCpSmw).
+Installing etm in an isolated or virtual environment (sandbox) is only slightly more complicated. Begin by using *pip* to install *pipx*:
 
-Open a terminal and begin by creating a new directory/folder for the virtual environment, say `plm-pypi`, in your home directory:
+    $ python3 -m pip install -U pipx
 
-        % mkdir ~/plm-pypi
-        % cd ~/plm-pypi
+Now run:
 
-Now continue by creating the virtual environment:
+    $ pipx ensurepath
 
-        % python3 -m venv env
+to ensure that directories necessary for *pipx* operation are in your PATH environment variable and finally to install *etm* itself:
 
-After a few seconds you will have a new `./env` directory. Now activate the virtual environment:
+    $ pipx install plm-dgraham
 
-        % source env/bin/activate
-
-The prompt will now change to something containing `(env)` to indicate that the virtual environment is active. Updating pip is now recommended:
-
-        (env) % pip install -U pip
-
-Note that this invokes `./env/bin/pip`. Once this is finished, use pip to install etm:
-
-        (env) % pip install -U plm-dgraham
-
-This will install *plm* and all its requirements in
-
-        ./env/lib/python3.x/sitepackages
-
-and will also install an executable called `plm` in `./env/bin`. This same command can be used to update *plm* when a new version becomes available.
-
-The virtual environment only affects the terminal window in which it was activated and can be deactivated, if you wish, by using:
-
-        (env) % deactivate
+To upgrade *etm* when a new version becomes available, simply replace "install" in this command with "upgrade".
 
 ## Starting *plm*
 
-If using a virtual environment, first change to that directory and activate the virtual environment, if necessary:
-
-        % cd ~/plm
-        % source env/bin/activate
-        (env) % plm
-
-Otherwise, just invoke *plm* directly
+Either way, you can then start *etm* with
 
-        % plm
+    $ plm <path to home>
 
-Either way, you will see something like this
+and you will see something like this
 
-        Player Lineup Manager (0.3.0)
+        Player Lineup Manager (0.3.4)
         home directory: ~/plm
+        project: The active project has not yet been chosen.
+        Use command 'c' to create one or 'p' to select one.
 
         commands:
             h:  show this help message
             H:  show on-line documentation
             e:  edit 'roster.yaml' using the default text editor
-            p:  create/update a project                           (1)
+            c:  create/update a project                           (1)
+            p:  select the active project from existing projects  (1)
             a:  ask players for their "can play" dates            (2)
             r:  record the "can play" responses                   (3)
-            s:  schedule play using the "can play" responses      (4)
-            d:  deliver the schedule to the players               (5)
+            n:  nag players to submit can play responses          (4)
+            s:  schedule play using the "can play" responses      (5)
+            d:  deliver the schedule to the players               (6)
             v:  view the current settings of a project
             u:  check for an update to a later plm version
-            l:  clear the screen
             q:  quit
 
         command:
 
 This begins a loop in which *plm* waits for you to enter a command at the prompt, processes the command and, unless the command *q* (quit) is given, waits for your next command.
 
-Note: the commands *p*, *a*, *r*, *s*, *d* and *v* begin with a request that you select the relevant project. Tab completion is available and, once a selection is made, this project becomes the *default project* for any further use of the commands in this group while the command loop continues.
+Note: the commands *a*, *r*, *s*, *d* and *v* begin with a request that you select the *active project* if you have not already done so with either *c* or *p*. Tab completion is available and, once a selection is made, this project becomes the *active project* for any further use of the commands in this group while the command loop continues.
 
 ### The Player Directory: roster.yaml
 
 This file is the directory for the players in all of your projects. It should be populated with all the relevant players for a project before you create the project itself.
 
 You can open `roster.yaml` in your favorite editor or use command *e*:
 
@@ -171,17 +149,17 @@
 It is worth devoting some thought to the *tag* scheme you will use before you start adding players. My schedules involve groups that play on a particular week day so I tend to use tags for the week day that the group plays, e.g., `mon` for the group that plays on *Monday*. Note that tags are case sensitive so `mon`, `Mon` and `MON` are all different tags.
 
 
 ### A New Project From Start to Finish
 
 #### 1. Create the project file
 
-Start *plm*, if necessary, and use the *project* command:
+Start *plm*, if necessary, and use the *create project* command:
 
-        command: p
+        command: c
 
 Then follow the on-line prompts to enter the project information. This information will be stored in a new file in the projects directory, `<project_name>.yaml`, where `<project_name>` is the name you provide for the project. A short name that sorts well and is suggestive is recommended, e.g., `2022-4Q-TU`.
 
 
 #### 2. Request players' availability dates
 
 With the project file created, the next step is to request the "can play" dates from the players. To do this start *plm*, if necessary, and use the *ask* command:
```

### Comparing `plm-dgraham-0.3.4/setup.py` & `plm-dgraham-0.4.0/setup.py`

 * *Files identical despite different names*

