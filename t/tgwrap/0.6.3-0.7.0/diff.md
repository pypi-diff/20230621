# Comparing `tmp/tgwrap-0.6.3.tar.gz` & `tmp/tgwrap-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.6.3.tar", max compression
+gzip compressed data, was "tgwrap-0.7.0.tar", max compression
```

## Comparing `tgwrap-0.6.3.tar` & `tgwrap-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.6.3/LICENSE
--rw-r--r--   0        0        0     7169 2023-05-26 12:45:31.451829 tgwrap-0.6.3/README.md
--rw-r--r--   0        0        0      902 2023-06-14 08:03:33.130998 tgwrap-0.6.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.6.3/tgwrap/__init__.py
--rw-r--r--   0        0        0     9164 2023-05-26 12:32:25.245403 tgwrap-0.6.3/tgwrap/analyze.py
--rwxr-xr-x   0        0        0    25922 2023-05-26 13:18:56.546086 tgwrap-0.6.3/tgwrap/cli.py
--rwxr-xr-x   0        0        0    56945 2023-06-14 08:01:07.947011 tgwrap-0.6.3/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.6.3/tgwrap/printer.py
--rw-r--r--   0        0        0     8321 1970-01-01 00:00:00.000000 tgwrap-0.6.3/setup.py
--rw-r--r--   0        0        0     8252 1970-01-01 00:00:00.000000 tgwrap-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.7.0/LICENSE
+-rw-r--r--   0        0        0     8381 2023-06-21 12:44:31.502352 tgwrap-0.7.0/README.md
+-rw-r--r--   0        0        0      902 2023-06-21 13:03:44.353606 tgwrap-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.7.0/tgwrap/__init__.py
+-rw-r--r--   0        0        0     9164 2023-05-26 12:32:25.245403 tgwrap-0.7.0/tgwrap/analyze.py
+-rwxr-xr-x   0        0        0    26165 2023-06-21 12:44:01.844554 tgwrap-0.7.0/tgwrap/cli.py
+-rwxr-xr-x   0        0        0    61348 2023-06-21 12:44:14.962219 tgwrap-0.7.0/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.7.0/tgwrap/printer.py
+-rw-r--r--   0        0        0     9561 1970-01-01 00:00:00.000000 tgwrap-0.7.0/setup.py
+-rw-r--r--   0        0        0     9464 1970-01-01 00:00:00.000000 tgwrap-0.7.0/PKG-INFO
```

### Comparing `tgwrap-0.6.3/LICENSE` & `tgwrap-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.6.3/README.md` & `tgwrap-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -79,14 +79,41 @@
     drift_impact:
       create: minor
       update: minor
   azurerm_application_insights.: {}
   # and so on, and so forth
 ```
 
+### Speeding up the performance of analyze
+
+This `analyze` function turned out to be pretty slow, where most of the time went into the `terragrunt show` function that is executed for each individual module. 
+
+This was a bit surprising as the plan file is already available on the file system, but it turns out that terragrunt is taking quite a bit of time for managing the depdencies. Even when you're excluding the external dependencies and are located in a particular module.
+
+So, if you add the following to your root `terragrunt.hcl`:
+
+```hcl
+terraform {
+  after_hook "link_to_current_module" {
+    commands = ["init", "plan", "apply", "validate", "destroy"]
+    execute  = ["bash", "-c", "ln -sf $(pwd) ${get_terragrunt_dir()}/.terragrunt-cache/current"]
+  }
+}
+```
+
+The directory where the plan file is stored (including the other resources that terraform needs) becomes predictable and it becomes possible to run a native `terraform show` (instead `terragrunt show`) which dramatically speed up things.
+
+Just set the proper value as an environment variable:
+
+```console
+export TGWRAP_PLANFILE_DIR=".terragrunt-cache/current"
+```
+
+Or pass it along with the `--planfile-dir|-P` option and it will use that.
+
 ## Usage
 
 ```console
 # general help
 tgwrap --help
 
 tgwrap run -h
```

### Comparing `tgwrap-0.6.3/pyproject.toml` & `tgwrap-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.6.3"
+version = "0.7.0"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
```

### Comparing `tgwrap-0.6.3/tgwrap/analyze.py` & `tgwrap-0.7.0/tgwrap/analyze.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.6.3/tgwrap/cli.py` & `tgwrap-0.7.0/tgwrap/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,33 +343,38 @@
     show_default=True
     )
 @click.option('--exclude-dir', '-E',
     multiple=True, default=[],
     help='A glob of a directory that needs to be excluded, this option can be used multiple times. For example: -E "integrations/\*/\*"',
     show_default=True,
     )
+@click.option('--planfile-dir', '-P', default=None,
+    help='Relative path to directory with plan file, see README for more details',
+    envvar='TGWRAP_PLANFILE_DIR', type=click.Path(),
+    )
 @click.argument('terragrunt-args', nargs=-1, type=click.UNPROCESSED)
 @click.version_option(version=__version__)
 def run_analyze(verbose, exclude_external_dependencies, working_dir, start_at_step,
             out, analyze_config, parallel_execution,
-            include_dir, exclude_dir, terragrunt_args):
+            include_dir, exclude_dir, planfile_dir, terragrunt_args):
     """ Analyzes the plan files """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
     tgwrap.analyze(
         exclude_external_dependencies=exclude_external_dependencies,
         working_dir=working_dir,
         start_at_step=start_at_step,
         out=out,
         analyze_config=analyze_config,
         parallel_execution=parallel_execution,
         include_dir=include_dir,
         exclude_dir=exclude_dir,
+        planfile_dir=planfile_dir,
         terragrunt_args=terragrunt_args,
     )
 
 @main.command(
     name="lock",
     context_settings=dict(
         ignore_unknown_options=True,
```

### Comparing `tgwrap-0.6.3/tgwrap/main.py` & `tgwrap-0.7.0/tgwrap/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import yaml
 import threading
 import queue
 import multiprocessing
 import click
 import networkx as nx
 import hcl2
+import fnmatch
 
 from datetime import datetime, timezone
 from .printer import Printer
 from .analyze import run_analyze
 
 class DateTimeEncoder(json.JSONEncoder):
     def default(self, obj):
@@ -69,15 +70,15 @@
         return shutil.which(program) is not None
 
     def load_yaml_file(self, filepath):
         try:
             with open(filepath, 'r') as file:
                 return yaml.safe_load(file)
         except yaml.parser.ParserError as e:
-            print(f'Cannot parse YAML file {filepath}, check syntax please!')
+            self.printer.error(f'Cannot parse YAML file {filepath}, check syntax please!')
             sys.exit(1)
 
     def _construct_command(self, command, debug, exclude_external_dependencies,
         non_interactive=True, no_auto_approve=True, no_lock=True, update=False,
         planfile=None, working_dir=None, limit_parallelism=None, 
         include_dir=[], exclude_dir=[], terragrunt_args=()):
         """ Constructs the command """
@@ -278,35 +279,44 @@
             error = True
 
         if 'skipping terragrunt module' in messages.lower():
             skip = True
 
         return error, skip
 
-    def _run_graph_step(self, command, working_dir, module, collect_output_file, dry_run, progress, 
-        output_queue=None, semaphore=None):
+    def _run_graph_step(self, command, working_dir, add_to_workdir, module, collect_output_file,
+        dry_run, progress, output_queue=None, semaphore=None):
         """ Runs a step in the graph """
 
         MODULE_IDENTIFIER=f'{module}{self.SEPARATOR}'
 
         stop_processing = False
         error = False
         skip = False
         output = None
         error_msg = None
+        messages = ""
 
         try:
             # if we are in multi-threading mode, acquire a semaphore
             if semaphore:
                 semaphore.acquire()
 
             # if we have a specific working dir, and the dir is relative, combine the two
             if working_dir and not os.path.isabs(module):
-                module = os.path.join(os.path.abspath(working_dir), module)
-                self.printer.verbose(f'Executing in directory: {working_dir}')
+                working_dir = os.path.join(os.path.abspath(working_dir), module)
+            else:
+                working_dir = module
+            
+            if add_to_workdir:
+                working_dir = os.path.join(working_dir, add_to_workdir)
+
+            self.printer.verbose(f'Execute command: {command} in working dir: {working_dir}')
+
+            self.printer.verbose(f'Executing in directory: {working_dir}')
 
             self.printer.header(
                 f'\n\nStart processing module: {module} ({progress})\n\n',
                 print_line_before=True,
                 )
 
             if dry_run:
@@ -325,70 +335,74 @@
 
                     # no output file, but data must be written to queue
                     # so we need to capture the output
                     collect_output_file = subprocess.PIPE
 
                 messages = ""
 
-                with tempfile.NamedTemporaryFile(mode='w+', prefix='tgwrap-', delete=False) as f:
-                    self.printer.verbose(f"Opened temp file for error collection: {f.name}")
-                    rc = {'returncode': 0}
-                    rc = subprocess.run(
-                        shlex.split(command),
-                        text=True,
-                        cwd=module,
-                        stdout=collect_output_file if collect_output_file else sys.stdout,
-                        stderr=f,
-                    )
+                if os.path.exists(working_dir):
+                    with tempfile.NamedTemporaryFile(mode='w+', prefix='tgwrap-', delete=False) as f:
+                        self.printer.verbose(f"Opened temp file for error collection: {f.name}")
+                        rc = {'returncode': 0}
+                        rc = subprocess.run(
+                            shlex.split(command),
+                            text=True,
+                            cwd=working_dir,
+                            stdout=collect_output_file if collect_output_file else sys.stdout,
+                            stderr=f,
+                        )
 
-                    self.printer.verbose(f'arguments: {rc.args}')
-                    self.printer.verbose(f'returncode: {rc.returncode}')
-                    try:
-                        self.printer.verbose(f'stdout: {rc.stdout[:200]}')
-                    except Exception:
-                        pass
-
-                with open(f.name, 'r') as f:
-                    messages = f.read()
-
-                error, skip = self._analyze_results(
-                    rc=rc,
-                    messages=messages,
-                    )
-                
-                # if we have a skipped module, and are collecting output, make sure we end up on a new line
+                        self.printer.verbose(f'arguments: {rc.args}')
+                        self.printer.verbose(f'returncode: {rc.returncode}')
+                        try:
+                            self.printer.verbose(f'stdout: {rc.stdout[:200]}')
+                        except Exception:
+                            pass
+
+                    with open(f.name, 'r') as f:
+                        messages = f.read()
+
+                    error, skip = self._analyze_results(
+                        rc=rc,
+                        messages=messages,
+                        )
+                    
+                    # if we have a skipped module, and are collecting output, make sure we end up on a new line
 
-                output = rc.stdout if rc.stdout else '\n'
+                    output = rc.stdout if rc.stdout else '\n'
+                else:
+                    skip = True
+                    output = '\n'
+                    self.printer.verbose(f"Directory '{working_dir}' does not exist")
 
                 if skip:
                     self.printer.verbose("Module is skipped")
 
                 if error:
                     raise Exception(
                         f'An error situation detected while processing the terragrunt dependencies graph in directory {module}'
                     )
                 else:
                     self.printer.success(
                         f'Directory {module} processed successfully',
                     )
 
         except FileNotFoundError:
-            error_msg = f'Directory {module} not found, continue'
+            error_msg = f'Directory {working_dir} not found, continue'
             self.printer.warning(error_msg)
         except Exception as e:
             error_msg = f"Error occurred:\n{str(e)}"
             self.printer.error(error_msg)
             self.printer.error("Full stack:", print_line_before=True)
             self.printer.normal(messages, print_line_after=True)
             self.printer.normal(f"Directory {module} failed!")
 
             stop_processing = True
         finally:
             if error_msg:
-                # output = f'{{"exception": "{error_msg}"}}'
                 output = json.dumps({"exception": error_msg})
 
             try:
                 # communicate the results if desired
                 if output_queue:
                     output_queue.put(f'{MODULE_IDENTIFIER}{output}')
                 elif collect_output_file and (skip or error):
@@ -402,31 +416,88 @@
             try:
                 os.remove(f.name)
             except Exception:
                 pass
 
         return stop_processing
 
+    def _get_subdirectories_with_file(self, root_dir, file_name, exclude_dir=[], include_dir=[], exclude_hidden_dir=True):
+
+        # ensure consistency, remove possible trailing slashes from the dirs
+        exclude_dir = [dir.rstrip(os.path.sep) for dir in exclude_dir]
+        include_dir = [dir.rstrip(os.path.sep) for dir in include_dir]
+
+        subdirectories = []
+        for directory, dirnames, filenames in os.walk(root_dir):
+            dir_excluded = False
+            dir_included = True if len(include_dir) == 0 else False
+            dir_excluded_reason = ""
+
+            # Exclude hidden directories that start with a dot
+            dirnames[:] = [d for d in dirnames if not (d.startswith('.') and exclude_hidden_dir)]
+
+            # Check if the current directory contains the specified file
+            if file_name in filenames:
+                self.printer.verbose(f"Directory found: {directory}")
+
+                for i in exclude_dir:
+                    exclude_paths = glob.glob(i)
+                    if directory in exclude_paths:
+                        dir_excluded = True
+                        dir_excluded_reason = "directory explicitly excluded"
+
+                # if we have a specific set of include_dirs, then everything else should be excluded
+                for i in include_dir:
+                    include_paths = glob.glob(i)
+                    if directory in include_paths:
+                        dir_included = True
+
+                if dir_excluded:
+                    self.printer.verbose(
+                        f"- Remove directory '{directory}': {dir_excluded_reason}"
+                        )
+                elif not dir_included:
+                    self.printer.verbose(
+                        f"- Remove directory '{directory}': specific list of include dirs given"
+                        )
+                else:
+                    self.printer.verbose(f"+ Include directory: {directory}")
+                    subdirectories.append(directory)
+
+        return subdirectories
+
     def _run_di_graph(
         self, command, exclude_external_dependencies, start_at_step, dry_run,
         parallel_execution=False, ask_for_confirmation=False, collect_output_file=None,
-        backwards=False, working_dir=None, include_dir=[], exclude_dir=[], 
+        backwards=False, working_dir=None, include_dir=[], exclude_dir=[],
+        use_native_terraform=False, add_to_workdir=None,
         ):
         "Runs the desired command in the directories as defined in the directed graph"
 
-        graph = self._get_di_graph(backwards=backwards, working_dir=working_dir)
-
-        # first go through the groups and clean up where needed
-        groups = self._prepare_groups(
-            graph=graph,
-            exclude_external_dependencies=exclude_external_dependencies,
-            working_dir=working_dir,
-            include_dir=include_dir,
-            exclude_dir=exclude_dir,
+        if use_native_terraform:
+            module_dirs = self._get_subdirectories_with_file(
+                root_dir = working_dir if working_dir else ".",
+                file_name="terragrunt.hcl",
+                exclude_hidden_dir=True,
+                include_dir=include_dir,
+                exclude_dir=exclude_dir,
             )
+            # for native terraform, we just have one group with no inter-dependencies
+            groups = [module_dirs]
+        else:
+            graph = self._get_di_graph(backwards=backwards, working_dir=working_dir)
+
+            # first go through the groups and clean up where needed
+            groups = self._prepare_groups(
+                graph=graph,
+                exclude_external_dependencies=exclude_external_dependencies,
+                working_dir=working_dir,
+                include_dir=include_dir,
+                exclude_dir=exclude_dir,
+                )
 
         if not groups:
             self.printer.error('No groups to process, this smells fishy!')
         elif ask_for_confirmation or self.printer.verbose:
             self.printer.header("The following groups will be processed:")
             for idx, group in enumerate(groups):
                 self.printer.normal(f"\nGroup {idx+1}:")
@@ -468,28 +539,30 @@
                 if parallel_execution:
                     self.printer.verbose(f'Start thread #{counter} for step {step_nbr}')
                     t = threading.Thread(
                         target=self._run_graph_step,
                         kwargs={
                             "command": command,
                             "working_dir": working_dir,
+                            "add_to_workdir": add_to_workdir,
                             "module": module,
                             "collect_output_file": None, # in parallel mode we can't write directly to the output file
                             "dry_run": dry_run,
                             "progress": progress,
                             "output_queue": q,
                             "semaphore": semaphore,
                             }
                         )
                     t.start()
                     threads.append(t)
                 else:
                     stop_processing = self._run_graph_step(
                         command=command,
                         working_dir=working_dir,
+                        add_to_workdir=add_to_workdir,
                         module=module,
                         collect_output_file=collect_output_file,
                         dry_run=dry_run,
                         progress=progress,
                     )
 
                     if stop_processing:
@@ -505,16 +578,18 @@
             total_counter = counter
             counter = 0
             for t in threads:
                 counter += 1
                 self.printer.verbose(f'Wait for thread #{counter} (of {total_counter}) to finish')
                 t.join()
                 collect_output_file.write(q.get())
-        
-        self.printer.verbose(f'Executed {group_nbr} groups and {step_nbr} steps')
+
+        if self.printer.print_verbose:
+            total_items = sum(len(group) for group in groups)
+            self.printer.verbose(f'Executed {group_nbr} groups and {total_items} steps')
 
     def _run_sync(
         self, source_path, target_path, auto_approve, include_lock_file, dry_run, clean,
         chmod_to_readonly=False, excludes=[], source_stage=None, target_stage=None, source_domain=None,
         ):
         """ Run a sync copying files from a source to a target path """
 
@@ -627,14 +702,16 @@
 
             # the `posix=False` is to prevent the split command to remove quotes from strings,
             # e.g. when executing commands like this:
             # tgwrap state mv 'azuread_group.this["viewers"]' 'azuread_group.this["readers"]'
             rc = subprocess.run(shlex.split(cmd, posix=False))
             self.printer.verbose(rc)
 
+            sys.exit(rc.returncode)
+
     def run_all(self, command, debug, dry_run, no_lock, update,
         exclude_external_dependencies, step_by_step, planfile, auto_approve, clean,
         working_dir, start_at_step, limit_parallelism, include_dir, exclude_dir, terragrunt_args):
         """ Executes a terragrunt command across multiple modules """
 
         self.printer.verbose(f"Attempting to execute 'run-all {command}'")
         if terragrunt_args:
@@ -682,14 +759,16 @@
         else:
             if dry_run:
                 self.printer.warning('In dry run mode, no real actions are executed!!')
             else:
                 rc = subprocess.run(shlex.split(cmd))
                 self.printer.verbose(rc)
 
+                sys.exit(rc.returncode)
+
     def run_import(self, address, id, dry_run, working_dir, no_lock, terragrunt_args):
         """ Executes the terragrunt/terraform import command """
 
         self.printer.verbose(f"Attempting to execute 'run import'")
         if terragrunt_args:
             self.printer.verbose(f"- with additional parameters: {' '.join(terragrunt_args)}")
 
@@ -730,28 +809,38 @@
                 shlex.split(cmd, posix=False),
                 env=env,
             )
             self.printer.verbose(rc)
 
     def analyze(self, exclude_external_dependencies, working_dir, start_at_step,
         out, analyze_config, parallel_execution,
-        include_dir, exclude_dir, terragrunt_args):
+        include_dir, exclude_dir, planfile_dir, terragrunt_args):
         """ Analyzes the plan files """
 
         self.printer.verbose("Attempting to 'analyze'")
         if terragrunt_args:
             self.printer.verbose(f"- with additional parameters: {' '.join(terragrunt_args)}")
 
-        # first run a 'show' and write output to file
-        cmd = self._construct_command(
-            command='show',
-            exclude_external_dependencies=True,
-            debug=False,
-            terragrunt_args=terragrunt_args,
+        # determine whether we are going to use a native 'terraform show' (faster!) or need 
+        # to use a terragrunt show
+        if start_at_step > 1 or not exclude_external_dependencies or not planfile_dir:
+            self.printer.verbose('Use terragrunt for module selection')
+
+            use_native_terraform = False
+            # first run a 'show' and write output to file
+            cmd = self._construct_command(
+                command='show',
+                exclude_external_dependencies=True,
+                debug=False,
+                terragrunt_args=terragrunt_args,
             )
+        else:
+            self.printer.verbose('Use native terraform for module selection')
+            use_native_terraform = True
+            cmd = "terraform show -json planfile"
 
         config = None
         if not analyze_config:
             self.printer.warning(
                 f"Analyze  config file is not set, this is required for checking for unauthorized deletions and drift detection scores!"
                 )
         else:
@@ -775,25 +864,29 @@
                     collect_output_file=f,
                     working_dir=working_dir,
                     start_at_step=start_at_step,
                     ask_for_confirmation=False,
                     include_dir=include_dir,
                     exclude_dir=exclude_dir,
                     parallel_execution=parallel_execution,
+                    use_native_terraform=use_native_terraform,
+                    add_to_workdir=planfile_dir if use_native_terraform else None,
                 )
 
             with open(f.name, 'r') as f:
                 for line in f:
                     split_line = line.split(self.SEPARATOR)
                     module = split_line[0]
+
                     try:
                         plan_file = split_line[1]
                     except IndexError:
                         self.printer.warning(f'Could not determine planfile: {line[:100]}')
 
+
                     try:
                         # plan file could be empty (except for new line) if module is skipped
                         if len(plan_file) > 1:
                             data = json.loads(plan_file)
 
                             # do we have an exception logged?
                             if 'exception' in data:
@@ -839,23 +932,24 @@
 
         # calulate the total drifts and scoe
         total_drifts = {
             "minor": 0,
             "medium": 0,
             "major": 0,
             "unknown": 0,
-            "total": 0
+            "total": 0,
         }
 
         for key, value in changes.items():
             for type in ["minor", "medium", "major", "unknown", "total"]:
                 total_drifts[type] += value["drifts"][type]
 
-        total_drift_score = f"{total_drifts['major']}.{total_drifts['medium']}.{total_drifts['minor']}"
-        self.printer.header(f"Drift score: {total_drift_score}")
+        # the formula below is just a way to achieve a numeric results that is coming from the various drift categories
+        total_drift_score = total_drifts['major'] * 10 + total_drifts['medium'] + total_drifts['minor'] / 10
+        self.printer.header(f"Drift score: {total_drift_score} ({total_drifts['major']}.{total_drifts['medium']}.{total_drifts['minor']})")
         if total_drifts["unknown"] > 0:
             self.printer.warning(f"For {total_drifts['unknown']} resources, drift score is not configured, please update configuration!")
             self.printer.warning('- Unknowns:')
             for key, value in changes.items():
                 for m in value["unknowns"]:
                     self.printer.warning(f' -> {m}')
```

### Comparing `tgwrap-0.6.3/tgwrap/printer.py` & `tgwrap-0.7.0/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.6.3/setup.py` & `tgwrap-0.7.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,17 +18,17 @@
  'terrasafe>=0.5.1,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['tgwrap = tgwrap.cli:main']}
 
 setup_kwargs = {
     'name': 'tgwrap',
-    'version': '0.6.3',
+    'version': '0.7.0',
     'description': 'A (terragrunt) wrapper around a (terraform) wrapper around ....',
-    'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if a config file is availabe) calculates a drift score and runs a [terrasafe](https://pypi.org/project/terrasafe/) style validation check.\n\nIt needs a config file as follows:\n\n```yaml\n---\n#\n# Critically of resources as interpreted by \'tgwrap analyze\'.\n# It uses it for a \'terrasafe\' like validation if resources can safely be deleted.\n# On top of that it tries to analyze and quantify the drift impact of the changes,\n# so that this can be monitored.\n#\nlow:\n  # defaults:\n  #   terrasafe_level: ignore_deletions\n  #   drift_impact:\n  #     default: minor\n  #     delete: medium\n  azuread_application.: {} # if we you want to use the defaults\n  azuread_app_role_assignment: # or if you want to override these\n    drift_impact:\n      delete: minor\n  # and so on, and so forth\nmedium:\n  # defaults:\n  #   terrasafe_level: ignore_deletion_if_recreation\n  #   drift_impact:\n  #     default: medium\n  #     delete: major\n  azurerm_data_factory_linked_service_key_vault.: {}\n  # and so on, and so forth\nhigh:\n  # defaults:\n  #   terrasafe_level: unauthorized_deletion\n  #   drift_impact:\n  #     default: major\n  #     update: medium\n  azuread_group.:\n    drift_impact:\n      create: minor\n      update: minor\n  azurerm_application_insights.: {}\n  # and so on, and so forth\n```\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n## A word about escaping inputs\n\nYour shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.\n\nFor example:\n\n```console\n# to exclude certain modules from an action (such as analyze):\ntgwrap analyze -E \'integrations/\\*/\\*\'\n\n# to import a resource that has a " in its address:\ntgwrap import -a \'azuread_group.this[\\"my_group\\"]\' -i ${GROUP_ID}\n```\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    base_dir: platform # optional, if you want to deploy the base modules in its own dir, side by side with substacks\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n\n# global configuration files that are deployed as well\n# note that these files are typically applicable to all landing zones and stages!\n# this might lead to unexpected behaviour\n# note that you can exclude syncing these files with a command line switch\nglobal_config_files:\n  root-terragrunt:\n    source: ../../terragrunt.hcl # relative to base_path\n    target: ../../terragrunt.hcl # can be omitted, then it is same as source path\n  terrasafe-config:\n    source: ../../terrasafe-config.json\n```\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
+    'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if a config file is availabe) calculates a drift score and runs a [terrasafe](https://pypi.org/project/terrasafe/) style validation check.\n\nIt needs a config file as follows:\n\n```yaml\n---\n#\n# Critically of resources as interpreted by \'tgwrap analyze\'.\n# It uses it for a \'terrasafe\' like validation if resources can safely be deleted.\n# On top of that it tries to analyze and quantify the drift impact of the changes,\n# so that this can be monitored.\n#\nlow:\n  # defaults:\n  #   terrasafe_level: ignore_deletions\n  #   drift_impact:\n  #     default: minor\n  #     delete: medium\n  azuread_application.: {} # if we you want to use the defaults\n  azuread_app_role_assignment: # or if you want to override these\n    drift_impact:\n      delete: minor\n  # and so on, and so forth\nmedium:\n  # defaults:\n  #   terrasafe_level: ignore_deletion_if_recreation\n  #   drift_impact:\n  #     default: medium\n  #     delete: major\n  azurerm_data_factory_linked_service_key_vault.: {}\n  # and so on, and so forth\nhigh:\n  # defaults:\n  #   terrasafe_level: unauthorized_deletion\n  #   drift_impact:\n  #     default: major\n  #     update: medium\n  azuread_group.:\n    drift_impact:\n      create: minor\n      update: minor\n  azurerm_application_insights.: {}\n  # and so on, and so forth\n```\n\n### Speeding up the performance of analyze\n\nThis `analyze` function turned out to be pretty slow, where most of the time went into the `terragrunt show` function that is executed for each individual module. \n\nThis was a bit surprising as the plan file is already available on the file system, but it turns out that terragrunt is taking quite a bit of time for managing the depdencies. Even when you\'re excluding the external dependencies and are located in a particular module.\n\nSo, if you add the following to your root `terragrunt.hcl`:\n\n```hcl\nterraform {\n  after_hook "link_to_current_module" {\n    commands = ["init", "plan", "apply", "validate", "destroy"]\n    execute  = ["bash", "-c", "ln -sf $(pwd) ${get_terragrunt_dir()}/.terragrunt-cache/current"]\n  }\n}\n```\n\nThe directory where the plan file is stored (including the other resources that terraform needs) becomes predictable and it becomes possible to run a native `terraform show` (instead `terragrunt show`) which dramatically speed up things.\n\nJust set the proper value as an environment variable:\n\n```console\nexport TGWRAP_PLANFILE_DIR=".terragrunt-cache/current"\n```\n\nOr pass it along with the `--planfile-dir|-P` option and it will use that.\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n## A word about escaping inputs\n\nYour shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.\n\nFor example:\n\n```console\n# to exclude certain modules from an action (such as analyze):\ntgwrap analyze -E \'integrations/\\*/\\*\'\n\n# to import a resource that has a " in its address:\ntgwrap import -a \'azuread_group.this[\\"my_group\\"]\' -i ${GROUP_ID}\n```\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    base_dir: platform # optional, if you want to deploy the base modules in its own dir, side by side with substacks\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n\n# global configuration files that are deployed as well\n# note that these files are typically applicable to all landing zones and stages!\n# this might lead to unexpected behaviour\n# note that you can exclude syncing these files with a command line switch\nglobal_config_files:\n  root-terragrunt:\n    source: ../../terragrunt.hcl # relative to base_path\n    target: ../../terragrunt.hcl # can be omitted, then it is same as source path\n  terrasafe-config:\n    source: ../../terrasafe-config.json\n```\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
     'author': 'Gerco Grandia',
     'author_email': 'gerco.grandia@4synergy.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/lunadata/tgwrap',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `tgwrap-0.6.3/PKG-INFO` & `tgwrap-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgwrap
-Version: 0.6.3
+Version: 0.7.0
 Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
 Home-page: https://gitlab.com/lunadata/tgwrap
 License: MIT
 Keywords: terraform,terragrunt,terrasafe,python
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.8,<4.0
@@ -107,14 +107,41 @@
     drift_impact:
       create: minor
       update: minor
   azurerm_application_insights.: {}
   # and so on, and so forth
 ```
 
+### Speeding up the performance of analyze
+
+This `analyze` function turned out to be pretty slow, where most of the time went into the `terragrunt show` function that is executed for each individual module. 
+
+This was a bit surprising as the plan file is already available on the file system, but it turns out that terragrunt is taking quite a bit of time for managing the depdencies. Even when you're excluding the external dependencies and are located in a particular module.
+
+So, if you add the following to your root `terragrunt.hcl`:
+
+```hcl
+terraform {
+  after_hook "link_to_current_module" {
+    commands = ["init", "plan", "apply", "validate", "destroy"]
+    execute  = ["bash", "-c", "ln -sf $(pwd) ${get_terragrunt_dir()}/.terragrunt-cache/current"]
+  }
+}
+```
+
+The directory where the plan file is stored (including the other resources that terraform needs) becomes predictable and it becomes possible to run a native `terraform show` (instead `terragrunt show`) which dramatically speed up things.
+
+Just set the proper value as an environment variable:
+
+```console
+export TGWRAP_PLANFILE_DIR=".terragrunt-cache/current"
+```
+
+Or pass it along with the `--planfile-dir|-P` option and it will use that.
+
 ## Usage
 
 ```console
 # general help
 tgwrap --help
 
 tgwrap run -h
```

