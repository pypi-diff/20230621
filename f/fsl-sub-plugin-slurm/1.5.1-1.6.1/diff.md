# Comparing `tmp/fsl_sub_plugin_slurm-1.5.1.tar.gz` & `tmp/fsl_sub_plugin_slurm-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsl_sub_plugin_slurm-1.5.1.tar", last modified: Thu Mar 23 10:07:15 2023, max compression
+gzip compressed data, was "fsl_sub_plugin_slurm-1.6.1.tar", last modified: Wed Jun 21 08:14:49 2023, max compression
```

## Comparing `fsl_sub_plugin_slurm-1.5.1.tar` & `fsl_sub_plugin_slurm-1.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:07:15.518498 fsl_sub_plugin_slurm-1.5.1/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-03-23 10:07:06.000000 fsl_sub_plugin_slurm-1.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12896 2023-03-23 10:07:15.518498 fsl_sub_plugin_slurm-1.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11666 2023-03-23 10:07:06.000000 fsl_sub_plugin_slurm-1.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:07:15.518498 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm/
--rw-rw-rw-   0 root         (0) root         (0)    41781 2023-03-23 10:07:06.000000 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3307 2023-03-23 10:07:06.000000 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm/fsl_sub_slurm.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:07:15.518498 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-23 10:07:06.000000 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    56403 2023-03-23 10:07:06.000000 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm/tests/test_fsl_sub_plugin_slurm.py
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-23 10:07:06.000000 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:07:15.518498 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12896 2023-03-23 10:07:15.000000 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2023-03-23 10:07:15.000000 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 10:07:15.000000 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-03-23 10:07:15.000000 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-23 10:07:15.000000 fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-23 10:07:15.518498 fsl_sub_plugin_slurm-1.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1921 2023-03-23 10:07:06.000000 fsl_sub_plugin_slurm-1.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 08:14:49.646432 fsl_sub_plugin_slurm-1.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-21 08:14:40.000000 fsl_sub_plugin_slurm-1.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    14004 2023-06-21 08:14:49.646432 fsl_sub_plugin_slurm-1.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12774 2023-06-21 08:14:40.000000 fsl_sub_plugin_slurm-1.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 08:14:49.642432 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm/
+-rw-rw-rw-   0 root         (0) root         (0)    42504 2023-06-21 08:14:40.000000 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3495 2023-06-21 08:14:40.000000 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm/fsl_sub_slurm.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 08:14:49.646432 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:14:40.000000 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    64932 2023-06-21 08:14:40.000000 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm/tests/test_fsl_sub_plugin_slurm.py
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-21 08:14:40.000000 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 08:14:49.646432 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14004 2023-06-21 08:14:49.000000 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-21 08:14:49.000000 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 08:14:49.000000 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-21 08:14:49.000000 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-21 08:14:49.000000 fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 08:14:49.646432 fsl_sub_plugin_slurm-1.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2023-06-21 08:14:40.000000 fsl_sub_plugin_slurm-1.6.1/setup.py
```

### Comparing `fsl_sub_plugin_slurm-1.5.1/LICENSE` & `fsl_sub_plugin_slurm-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fsl_sub_plugin_slurm-1.5.1/PKG-INFO` & `fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fsl_sub_plugin_slurm
-Version: 1.5.1
+Name: fsl-sub-plugin-slurm
+Version: 1.6.1
 Summary: FSL Cluster Submission Plugin for Slurm
 Home-page: https://git.fmrib.ox.ac.uk/fsl/fsl_sub_plugin_slurm
 Author: Duncan Mortimer
 Author-email: duncan.mortimer@ndcn.ox.ac.uk
 License: Apache License Version 2.0
 Project-URL: Documentation, https://fsl.fmrib.ox.ac.uk/fsl/fslwiki
 Project-URL: Source, https://git.fmrib.ox.ac.uk/fsl/fsl_sub_plugin_slurm
@@ -25,15 +25,16 @@
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fsl_sub_plugin_slurm
 
 Job submission to SLURM variant cluster queues.
-_Copyright 2018-2021, University of Oxford (Duncan Mortimer)_
+
+_Copyright 2018-2023 University of Oxford, Oxford, UK._
 
 ## Introduction
 
 fsl\_sub provides a consistent interface to various cluster backends, with a fall back to running tasks locally where no cluster is available.
 This fsl\_sub plugin provides support for submitting tasks to SLURM clusters.
 
 For installation instructions please see INSTALL.md; for building packages see BUILD.md.
@@ -59,24 +60,25 @@
 | copy\_environment | **True**/False | Whether to replicate the environment variables in the shell that called fsl_sub into the job's shell
 | has\_parallel_envs | **False**/True | SLURM does not provide parallel environments so this should always be false
 | script\_conf | **True**/False | Whether _--usesscript_ option to fsl_sub is available via this method. This option allows you to define the grid options as comments in a shell script and then provide this to the cluster for running. Should be set to True.
 | mail\_support | True/**False** | Whether the grid installation is configured to send email on job events.
 | mail\_modes | Dictionary of option lists | If the grid has email notifications turned on, this option configures the submission options for different verbosity levels, 'b' = job start, 'e' = job end, 'a' = job abort, 'f' = all events, 'n' = no mail. Each event type should then have a list of submission mail arguments that will be applied to the submitted job. Typically, these should not be edited.
 | mail\_mode | b/e/a/f/**n** | Which of the above mail_modes to use by default
 | notify\_ram\_usage | **True**/False | Whether to notify SLURM of the RAM you have requested. SLURM is typically configured to give jobs a small RAM allocation so you will invariably need this set to true.
-| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected *maximum* run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True').
+| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected **maximum** run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True').
 | array\_holds | **True**/False | Enable support array holds, e.g. sub-task 1 waits for parent sub-task 1.
 | array\_limit | **True**/False | Enable limiting number of concurrent array tasks.
 | job\_resources | **True**/False | Enable additional job resource specification support.
 | projects | **True**/False | Enable support for projects typically used auditing/charging purposes.
 | preseve\_modules | True/**False** | Whether to re-load shell modules on the compute node. Required if you have multiple CPU generations and per-generation optimised libraries configured with modules.
 | add_module_paths | **[]**/ a list | List of file system paths to search for modules in addition to the system defined ones. Useful if you have your own shell modules directory but need to allow the compute node to auto-set it's MODULEPATH environment variable (e.g. to a architecture specific folder). Only used when preserve_modules is True.
 | export\_vars | **[]**/List | List of environment variables that should transfered with the job to the compute node
-| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `jobid_wrapper.sh`. This file contains sufficient information to resubmit this job in the future.
+| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `wrapper_<jobid>.sh`. This file contains sufficient information to resubmit this job in the future. If the job fails to submit, this will be preserved in the file `wrapper_failed_<DD>-<MMM>-<YYYY>_<HH><MM><SS>.sh`.
 | extra\_args | **[]**/List | List of additional SLURM arguments to pass through to the sheduler.
+| strict_dependencies | True/**False** | Whether to use 'afterok' (True) or 'afterany' (False) when specifying simple job dependencies. This can also be controlled by the environment variable `FSLSUB_STRICTDEPS` (True="1", False="0").
 
 ### Coprocessor Configuration
 
 This plugin is not capable of automatically determining all the necessary information to configure your co-processors but will advise of the information it can find and propose queue definitions for these GPU resources.
 
 SLURM typically selects GPU resources with a GRES (Generic RESource) that defines the type and quantity of the co-processor. Where multiple classes of co-processor are available this might be selectable via the GRES or you may need to provide a _constraint_. If you would like to be able to support running on a class and all superior devices you need to be able to use constraints as GRES requests do not support logical combinations. The automatically generated configuration should include useful information about your GRES and constraints, but should you wish to obtain this information yourself use the commands:
 
@@ -132,7 +134,14 @@
 | | exclusive | True/**False** | Whether this queue is only used for co-processor requiring tasks. |
 
 Where a partition has obvious GRES or features that define GPUs a proposed GPU configuration will be added as comments to the start of the queue definition. You should review this, create/update the coproc_opts>cuda record with the information in the comments and then this section can be uncommented to enable GPU support.
 
 #### Compound Queues
 
 Some clusters may be configured with multiple variants of the same partition, e.g. short.a, short.b, with each queue having different hardware, perhaps CPU generation or maximum memory or memory available per slot. To maximise scheduling options you can define compound queues which have the configuration of the least capable constituent. To define a compound queue, the queue name (key of the YAML dictionary) should be a comma separated list of queue names (no space).
+
+## SLURM specific usage
+
+### Job dependencies
+
+The default dependency handler (`-j`) takes a job id and uses `--dependency=afterany:\<jobid>` to control job hierarchies of non-array tasks. To switch to the old behaviour (pre-version 1.6.0) of using `afterok` (ancestor job must complete successfully), either modify the method configuration to set `strict_dependencies` to True or set the environment variable `FSLSUB_STRICTDEPS` to "1".
+Where you need to specify complex dependencies you may pass the raw SLURM dependency description (without the `--dependency=`) in the `-j` argument. For array tasks, the `array_hold` argument is used instead of the `-j` argument. This can take the same forms as the `-j` argument (job ids or complex hold descriptions).
```

### Comparing `fsl_sub_plugin_slurm-1.5.1/README.md` & `fsl_sub_plugin_slurm-1.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # fsl_sub_plugin_slurm
 
 Job submission to SLURM variant cluster queues.
-_Copyright 2018-2021, University of Oxford (Duncan Mortimer)_
+
+_Copyright 2018-2023 University of Oxford, Oxford, UK._
 
 ## Introduction
 
 fsl\_sub provides a consistent interface to various cluster backends, with a fall back to running tasks locally where no cluster is available.
 This fsl\_sub plugin provides support for submitting tasks to SLURM clusters.
 
 For installation instructions please see INSTALL.md; for building packages see BUILD.md.
@@ -31,24 +32,25 @@
 | copy\_environment | **True**/False | Whether to replicate the environment variables in the shell that called fsl_sub into the job's shell
 | has\_parallel_envs | **False**/True | SLURM does not provide parallel environments so this should always be false
 | script\_conf | **True**/False | Whether _--usesscript_ option to fsl_sub is available via this method. This option allows you to define the grid options as comments in a shell script and then provide this to the cluster for running. Should be set to True.
 | mail\_support | True/**False** | Whether the grid installation is configured to send email on job events.
 | mail\_modes | Dictionary of option lists | If the grid has email notifications turned on, this option configures the submission options for different verbosity levels, 'b' = job start, 'e' = job end, 'a' = job abort, 'f' = all events, 'n' = no mail. Each event type should then have a list of submission mail arguments that will be applied to the submitted job. Typically, these should not be edited.
 | mail\_mode | b/e/a/f/**n** | Which of the above mail_modes to use by default
 | notify\_ram\_usage | **True**/False | Whether to notify SLURM of the RAM you have requested. SLURM is typically configured to give jobs a small RAM allocation so you will invariably need this set to true.
-| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected *maximum* run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True').
+| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected **maximum** run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True').
 | array\_holds | **True**/False | Enable support array holds, e.g. sub-task 1 waits for parent sub-task 1.
 | array\_limit | **True**/False | Enable limiting number of concurrent array tasks.
 | job\_resources | **True**/False | Enable additional job resource specification support.
 | projects | **True**/False | Enable support for projects typically used auditing/charging purposes.
 | preseve\_modules | True/**False** | Whether to re-load shell modules on the compute node. Required if you have multiple CPU generations and per-generation optimised libraries configured with modules.
 | add_module_paths | **[]**/ a list | List of file system paths to search for modules in addition to the system defined ones. Useful if you have your own shell modules directory but need to allow the compute node to auto-set it's MODULEPATH environment variable (e.g. to a architecture specific folder). Only used when preserve_modules is True.
 | export\_vars | **[]**/List | List of environment variables that should transfered with the job to the compute node
-| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `jobid_wrapper.sh`. This file contains sufficient information to resubmit this job in the future.
+| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `wrapper_<jobid>.sh`. This file contains sufficient information to resubmit this job in the future. If the job fails to submit, this will be preserved in the file `wrapper_failed_<DD>-<MMM>-<YYYY>_<HH><MM><SS>.sh`.
 | extra\_args | **[]**/List | List of additional SLURM arguments to pass through to the sheduler.
+| strict_dependencies | True/**False** | Whether to use 'afterok' (True) or 'afterany' (False) when specifying simple job dependencies. This can also be controlled by the environment variable `FSLSUB_STRICTDEPS` (True="1", False="0").
 
 ### Coprocessor Configuration
 
 This plugin is not capable of automatically determining all the necessary information to configure your co-processors but will advise of the information it can find and propose queue definitions for these GPU resources.
 
 SLURM typically selects GPU resources with a GRES (Generic RESource) that defines the type and quantity of the co-processor. Where multiple classes of co-processor are available this might be selectable via the GRES or you may need to provide a _constraint_. If you would like to be able to support running on a class and all superior devices you need to be able to use constraints as GRES requests do not support logical combinations. The automatically generated configuration should include useful information about your GRES and constraints, but should you wish to obtain this information yourself use the commands:
 
@@ -104,7 +106,14 @@
 | | exclusive | True/**False** | Whether this queue is only used for co-processor requiring tasks. |
 
 Where a partition has obvious GRES or features that define GPUs a proposed GPU configuration will be added as comments to the start of the queue definition. You should review this, create/update the coproc_opts>cuda record with the information in the comments and then this section can be uncommented to enable GPU support.
 
 #### Compound Queues
 
 Some clusters may be configured with multiple variants of the same partition, e.g. short.a, short.b, with each queue having different hardware, perhaps CPU generation or maximum memory or memory available per slot. To maximise scheduling options you can define compound queues which have the configuration of the least capable constituent. To define a compound queue, the queue name (key of the YAML dictionary) should be a comma separated list of queue names (no space).
+
+## SLURM specific usage
+
+### Job dependencies
+
+The default dependency handler (`-j`) takes a job id and uses `--dependency=afterany:\<jobid>` to control job hierarchies of non-array tasks. To switch to the old behaviour (pre-version 1.6.0) of using `afterok` (ancestor job must complete successfully), either modify the method configuration to set `strict_dependencies` to True or set the environment variable `FSLSUB_STRICTDEPS` to "1".
+Where you need to specify complex dependencies you may pass the raw SLURM dependency description (without the `--dependency=`) in the `-j` argument. For array tasks, the `array_hold` argument is used instead of the `-j` argument. This can take the same forms as the `-j` argument (job ids or complex hold descriptions).
```

### Comparing `fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm/__init__.py` & `fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,51 @@
     return (result.stdout, result.returncode)
 
 
 def _slurm_option(opt):
     return "#SBATCH " + opt
 
 
+def _no_waiton(waiton):
+    return any((waiton is None, not waiton, waiton == [], waiton == ()))
+
+
+def _get_dependency(config, waiton=None, array_task=False, array_hold=None):
+    if array_task is True:
+        if array_hold is None and _no_waiton(waiton):
+            return None
+    elif _no_waiton(waiton):
+        return None
+
+    hold_state = 'afterany:'
+    if (
+            os.environ.get('FSLSUB_STRICTDEPS', "0") == "1"
+            or config.get('strict_dependancies', False)):
+        hold_state = 'afterok:'
+
+    if array_task and array_hold is not None:
+        if config['array_holds']:
+            # Requires Slurm 16.05
+            hold_state = 'aftercorr:'
+        waiton = array_hold
+
+    if isinstance(waiton, (list, tuple, )):
+        ancestors = ':'.join([str(a).replace('.', '_') for a in waiton])
+    elif isinstance(waiton, str):
+        ancestors = waiton
+        if ":" in waiton:
+            hold_state = ''
+    elif isinstance(waiton, int):
+        ancestors = str(waiton)
+    else:
+        raise BadSubmission(
+            "jobhold is of unsupported type " + str(type(waiton)))
+    return f'{hold_state}{ancestors}'
+
+
 def _get_logger():
     return logging.getLogger('fsl_sub.' + __name__)
 
 
 def submit(
         command,
         job_name=None,
@@ -397,40 +434,17 @@
                     logtemplate.format(
                         job_name.replace(' ', '_'),
                         lf)
                 )
             command_args.append(['-o', logs['o'], ])
             command_args.append(['-e', logs['e'], ])
 
-        hold_state = 'afterok'
-        if array_task and array_hold is not None:
-            if mconf['array_holds']:
-                # Requires Slurm 16.05
-                jobhold = array_hold
-                hold_state = 'aftercorr'
-            else:
-                jobhold = array_hold
-
-        if jobhold:
-            if isinstance(jobhold, (list, tuple, )):
-                parents = ':'.join([str(a).replace('.', '_') for a in jobhold])
-            elif isinstance(jobhold, str):
-                parents = jobhold
-            elif isinstance(jobhold, int):
-                parents = str(jobhold)
-            else:
-                raise BadSubmission(
-                    "jobhold is of unsupported type " + type(jobhold))
-            command_args.append(
-                "=".join(
-                    (
-                        '--dependency',
-                        hold_state + ':' + parents)
-                )
-            )
+        job_hold = _get_dependency(mconf, waiton=jobhold, array_task=array_task, array_hold=array_hold)
+        if job_hold is not None:
+            command_args.append("=".join(('--dependency', job_hold)))
 
         if array_task is not None:
             # ntasks%array_limit
             if mconf['array_limits'] and array_limit:
                 array_limit_modifier = "%{}".format(array_limit)
             else:
                 array_limit_modifier = ""
@@ -630,37 +644,50 @@
         result = sp.run(
             command_args,
             input='\n'.join(js_lines),
             universal_newlines=True,
             stdout=sp.PIPE, stderr=sp.PIPE
         )
     if result.returncode != 0:
+        if keep_jobscript:
+            rename_jobscript(
+                wrapper_name,
+                "".join((
+                    "failed_",
+                    datetime.datetime.now().strftime('%d-%b-%Y_%H%M%S'),
+                )))
         raise BadSubmission(result.stderr)
     job_words = result.stdout.split(';')
     try:
         job_id = int(job_words[0].split('.')[0])
     except ValueError:
         raise GridOutputError("Grid output was " + result.stdout)
 
     if keep_jobscript:
-        new_name = os.path.join(
-            os.getcwd(),
-            '_'.join(('wrapper', str(job_id))) + '.sh'
-        )
-        try:
-            logger.debug("Renaming wrapper to " + new_name)
-            shutil.move(
-                wrapper_name,
-                new_name
-            )
-        except OSError:
-            warnings.warn("Unable to preserve wrapper script")
+        rename_jobscript(wrapper_name, job_id)
+
     return job_id
 
 
+def rename_jobscript(src, jobid):
+    logger = logging.getLogger(__name__)
+    new_name = os.path.join(
+        os.getcwd(),
+        '_'.join(('wrapper', str(jobid))) + '.sh'
+    )
+    try:
+        logger.debug("Renaming wrapper to " + new_name)
+        shutil.move(
+            src,
+            new_name
+        )
+    except OSError:
+        warnings.warn("Unable to preserve wrapper script")
+
+
 def _default_config_file():
     return os.path.join(
         os.path.realpath(os.path.dirname(__file__)),
         'fsl_sub_slurm.yml')
 
 
 def default_conf():
```

### Comparing `fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm/fsl_sub_slurm.yml` & `fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm/fsl_sub_slurm.yml`

 * *Files 8% similar despite different names*

```diff
@@ -41,13 +41,15 @@
     # (where a system used modules). Users will not be able to overwrite this.
     preserve_modules: False # Do you want to load your currently loaded modules in the cluster job?
     # If your system uses shell modules to configure environment variables then enable
     # this.
     add_module_paths: [] # If preserve_modules is set and you need to add additional
     # folders to the MODULESPATH environment variable in the job's environment then
     # add these paths to this list
+    strict_dependencies: False # Do you want to allow subsequent jobs in a pipeline to run even
+    # if an earlier job fails - equivalent environment variable FSLSUB_STRICTDEPS (0=False)
 coproc_opts:
   cuda:
     class_constraint: False # Does the SURLM cluster use constraints to specify GPU types rather than
     # adding it to the GRES? If your cluster instructions say use --constraint (or -C) <class> then set this
     # to true.
     # If you are told to use --gres gpu:<class>:<qty> then set this to false.
```

### Comparing `fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm/tests/test_fsl_sub_plugin_slurm.py` & `fsl_sub_plugin_slurm-1.6.1/fsl_sub_plugin_slurm/tests/test_fsl_sub_plugin_slurm.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import subprocess
 import tempfile
 import unittest
 import fsl_sub_plugin_slurm
 
 from collections import defaultdict
 from ruamel.yaml import YAML
-from unittest.mock import (patch, )
+from unittest.mock import patch
 
 import fsl_sub.consts
 from fsl_sub.exceptions import (
     BadSubmission,
     UnknownJobId
 )
 from fsl_sub.utils import (
@@ -145,14 +145,65 @@
             newcomments, 'Another comment'
         )
         self.assertListEqual(
             ['A comment', 'Another comment', ],
             newcomments
         )
 
+    def test__no_waiton(self):
+        self.assertTrue(fsl_sub_plugin_slurm._no_waiton([]))
+        self.assertTrue(fsl_sub_plugin_slurm._no_waiton(()))
+        self.assertTrue(fsl_sub_plugin_slurm._no_waiton(None))
+        self.assertTrue(fsl_sub_plugin_slurm._no_waiton(False))
+        self.assertTrue(fsl_sub_plugin_slurm._no_waiton(''))
+
+    def test__get_dependency(self):
+        config = {'strict_dependancies': True, }
+        self.assertEqual('afterok:1234', fsl_sub_plugin_slurm._get_dependency(config, waiton=1234))
+        config = {'strict_dependancies': False, }
+        self.assertEqual('afterany:1234', fsl_sub_plugin_slurm._get_dependency(config, waiton=1234))
+        config = {'strict_dependancies': False, }
+        self.assertEqual('afterany:1234', fsl_sub_plugin_slurm._get_dependency(config, waiton="1234"))
+        config = {'strict_dependancies': False, }
+        self.assertEqual('afterany:1234', fsl_sub_plugin_slurm._get_dependency(config, waiton=[1234, ]))
+        config = {'strict_dependancies': False, }
+        self.assertEqual('afterany:1234', fsl_sub_plugin_slurm._get_dependency(config, waiton=["1234", ]))
+        config = {'strict_dependancies': False, }
+        self.assertEqual('afterany:1234', fsl_sub_plugin_slurm._get_dependency(config, waiton=(1234, )))
+        config = {}
+        self.assertEqual('afterany:1234', fsl_sub_plugin_slurm._get_dependency(config, waiton=1234))
+        self.assertEqual(
+            'afterany:1234?afternotok:1235',
+            fsl_sub_plugin_slurm._get_dependency(config, waiton="afterany:1234?afternotok:1235"))
+        with patch.dict(os.environ, {"FSLSUB_STRICTDEPS": "1"}, clear=True):
+            self.assertEqual('afterok:1234', fsl_sub_plugin_slurm._get_dependency(config, waiton=1234))
+        with patch.dict(os.environ, {"FSLSUB_STRICTDEPS": "0"}, clear=True):
+            self.assertEqual('afterany:1234', fsl_sub_plugin_slurm._get_dependency(config, waiton=1234))
+        with patch.dict(os.environ, {}, clear=True):
+            self.assertEqual('afterany:1234', fsl_sub_plugin_slurm._get_dependency(config, waiton=1234))
+        config = {'array_holds': True, }
+        self.assertEqual(
+            'aftercorr:1234',
+            fsl_sub_plugin_slurm._get_dependency(config, waiton=None, array_task=True, array_hold=1234))
+        self.assertIsNone(
+            fsl_sub_plugin_slurm._get_dependency(config, waiton=None, array_task=True))
+        self.assertIsNone(fsl_sub_plugin_slurm._get_dependency(config, waiton=(), array_task=True))
+        self.assertIsNone(fsl_sub_plugin_slurm._get_dependency(config, waiton=[], array_task=True))
+        self.assertIsNone(fsl_sub_plugin_slurm._get_dependency(config, waiton=()))
+        self.assertIsNone(fsl_sub_plugin_slurm._get_dependency(config, waiton=[]))
+        self.assertIsNone(fsl_sub_plugin_slurm._get_dependency(config, waiton=None))
+        self.assertEqual(
+            'afterany:1234',
+            fsl_sub_plugin_slurm._get_dependency(config, waiton=1234, array_task=True))
+        with self.assertRaises(BadSubmission) as exc:
+            fsl_sub_plugin_slurm._get_dependency(config, waiton={'key': 'value'})
+        self.assertEqual(
+            str(exc.exception), "jobhold is of unsupported type <class 'dict'>"
+        )
+
 
 class TestslurmFinders(unittest.TestCase):
     @patch('fsl_sub_plugin_slurm.which', autospec=True)
     def test_qstat(self, mock_which):
         bin_path = '/usr/bin/squeue'
         with self.subTest("Test 1"):
             mock_which.return_value = bin_path
@@ -306,23 +357,25 @@
         self.parsable_str = '#SBATCH --parsable'
         self.requeue_str = '#SBATCH --requeue'
         self.ntasks_str = '#SBATCH --ntasks=1'
         self.nthreads_str_gpu = '#SBATCH --gpus-per-task'
         self.nthreads_str = '#SBATCH --cpus-per-task'
         self.module_load_str = 'module load ' + self.module
         self.version_str = '# Built by fsl_sub v.1.0.0 and fsl_sub_plugin_slurm v.2.0.0'
-        self.sys_argv_str = '# Command line: fsl_sub -q {0} {1}'.format(self.queue, ' '.join(self.cmd))
+        self.sys_argv_str_base = '# Command line: '
+        self.sys_argv_str = f'{self.sys_argv_str_base}fsl_sub -q {self.queue} {" ".join(self.cmd)}'
         self.submission_time_str = '# Submission time (H:M:S DD/MM/YYYY): ' + self.now.strftime("%H:%M:%S %d/%m/%Y")
         self.cmd_str = '\n'.join(('', ' '.join(self.cmd)))
 
     def submit_str(
             self, cmd=None, threads=1, copy_env=False,
             exports=[],
             queue=None, modules=None, host_list=[],
-            project=None, module_path=None, gpu_lines=[]):
+            project=None, module_path=None, gpu_lines=[],
+            dependencies=None):
         if modules is None:
             modules = [self.module]
         if queue is None:
             queue = self.queue
         sub_str = [self.script_head, ]
         if copy_env:
             e_str = self.export_str.replace("--export=", '--export=ALL,')
@@ -330,14 +383,16 @@
             e_str = self.export_str.replace("--export=", '--export=' + ','.join(exports) + ',')
         else:
             e_str = self.export_str
         sub_str.append(e_str)
         for gl in gpu_lines:
             sub_str.append('#SBATCH ' + gl)
         sub_str.append(self.log_str)
+        if dependencies is not None:
+            sub_str.append(f'#SBATCH --dependency={dependencies}')
         sub_str.append(self.name_str)
         sub_str.append(self.chdir_str)
         sub_str.append('#SBATCH -p ' + queue)
         if host_list:
             sub_str.append('#SBATCH -w ' + ','.join(host_list))
         sub_str.append(self.parsable_str)
         sub_str.append(self.requeue_str)
@@ -354,15 +409,15 @@
             sub_str.append('MODULEPATH={0}:$MODULEPATH'.format(module_path))
         for module in modules:
             sub_str.append('module load ' + module)
         sub_str.append(self.version_str)
         if cmd is None:
             sub_str.append(self.sys_argv_str)
         else:
-            sub_str.append('# Command line: ' + cmd)
+            sub_str.append(f'{self.sys_argv_str_base}{cmd}')
         sub_str.append(self.submission_time_str)
         sub_str.append('\n'.join(('', ' '.join(self.cmd))))
         sub_str.append('')
         return '\n'.join(sub_str)
 
     def TearDown(self):
         self.ww.close()
@@ -411,14 +466,82 @@
                 expected_cmd,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 universal_newlines=True,
                 input=expected_script
             )
 
+    def test_submit_dependencies(
+            self, mock_sprun, mock_cpconf,
+            mock_srbs, mock_qsub,
+            mock_getcwd):
+        with self.subTest("Slurm"):
+            expected_cmd = ['/usr/bin/sbatch']
+
+            cmd_argv_base = ['fsl_sub', '-q', self.queue, ]
+            with self.subTest('Basic dependency'):
+                cmd_argv = copy.copy(cmd_argv_base)
+                jh = '1234'
+                cmd_argv.extend(['-j', '1234', ])
+                cmd_argv.extend(self.cmd)
+                expected_script = self.submit_str(
+                    cmd=f'{" ".join(cmd_argv)}',
+                    dependencies=f"afterany:{jh}")
+                mock_sprun.reset_mock()
+                mock_sprun.return_value = subprocess.CompletedProcess(
+                    expected_cmd, 0,
+                    stdout=self.qsub_out, stderr=None)
+
+                with patch('fsl_sub.utils.sys.argv', cmd_argv):
+                    self.assertEqual(
+                        self.jid,
+                        self.plugin.submit(
+                            command=self.cmd,
+                            job_name=self.job_name,
+                            queue=self.queue,
+                            jobhold=jh
+                        )
+                    )
+                mock_sprun.assert_called_once_with(
+                    expected_cmd,
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.PIPE,
+                    universal_newlines=True,
+                    input=expected_script
+                )
+            with self.subTest('Complex dependency'):
+                cmd_argv = copy.copy(cmd_argv_base)
+                jh = 'afterany:1234:afternotok:1345'
+                cmd_argv.extend(['-j', jh, ])
+                cmd_argv.extend(self.cmd)
+                expected_script = self.submit_str(
+                    cmd=f'{" ".join(cmd_argv)}',
+                    dependencies=jh)
+                mock_sprun.reset_mock()
+                mock_sprun.return_value = subprocess.CompletedProcess(
+                    expected_cmd, 0,
+                    stdout=self.qsub_out, stderr=None)
+                with patch('fsl_sub.utils.sys.argv', cmd_argv):
+                    self.assertEqual(
+                        self.jid,
+                        self.plugin.submit(
+                            command=self.cmd,
+                            job_name=self.job_name,
+                            queue=self.queue,
+                            jobhold=jh
+                        )
+                    )
+                mock_sprun.assert_called_once_with(
+                    expected_cmd,
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.PIPE,
+                    universal_newlines=True,
+                    input=expected_script
+                )
+
     def test_submit_basic_export_vars(
             self, mock_sprun, mock_cpconf,
             mock_srbs, mock_qsub,
             mock_getcwd):
         with self.subTest("Slurm"):
             self.mconfig['export_vars'] = ['FSLTEST']
             self.mconfig['copy_environment'] = False
@@ -897,14 +1020,70 @@
             self.ww.name,
             os.path.join(
                 os.getcwd(),
                 '_'.join(('wrapper', str(self.jid) + '.sh'))
             )
         )
 
+    def test_submit_wrapper_keep_with_error(
+            self, mock_sprun, mock_cpconf,
+            mock_srbs, mock_qsub,
+            mock_getcwd):
+        w_conf = self.config
+        w_conf['method_opts']['slurm']['keep_jobscript'] = True
+        w_conf['method_opts']['slurm']['copy_environment'] = False
+        self.mocks['fsl_sub_plugin_slurm.method_config'].return_value = w_conf['method_opts']['slurm']
+        mock_cpconf.return_value = w_conf['copro_opts']['cuda']
+        cmd_argv = ['fsl_sub', '-q', self.queue, ]
+        cmd_argv.extend(self.cmd)
+
+        expected_cmd = ['/usr/bin/sbatch', self.ww.name]
+        expected_script = self.submit_str()
+        mock_sprun.return_value = subprocess.CompletedProcess(
+            expected_cmd, 1,
+            stdout=self.qsub_out, stderr="An error")
+        mock_now = datetime.datetime.now()
+
+        with patch('fsl_sub_plugin_slurm.os.rename') as mock_rename:
+            with patch('fsl_sub.utils.sys.argv', cmd_argv):
+
+                with patch('fsl_sub_plugin_slurm.datetime', wraps=datetime) as mock_time:
+                    mock_time.datetime.now.return_value = mock_now
+                    with self.assertRaises(fsl_sub.exceptions.BadSubmission) as ex:
+                        self.plugin.submit(
+                            command=self.cmd,
+                            job_name=self.job_name,
+                            queue=self.queue,
+                            keep_jobscript=True
+                        )
+
+                message = str(ex.exception)
+                self.assertEqual(message, "An error")
+        mock_sprun.assert_called_once_with(
+            expected_cmd,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            universal_newlines=True,
+        )
+        mock_sprun.reset_mock()
+        self.ww.seek(0)
+        wrapper_lines = self.ww.read().splitlines()
+        self.maxDiff = None
+        self.assertListEqual(
+            wrapper_lines,
+            expected_script.split('\n')
+        )
+        mock_rename.assert_called_once_with(
+            self.ww.name,
+            os.path.join(
+                os.getcwd(),
+                '_'.join(('wrapper_failed', str(mock_now.strftime("%d-%b-%Y_%H%M%S")) + '.sh'))
+            )
+        )
+
     def test_submit_script(
             self, mock_sprun, mock_cpconf,
             mock_srbs, mock_qsub,
             mock_getcwd):
         w_conf = self.config
         w_conf['method_opts']['slurm']['keep_jobscript'] = True
         w_conf['method_opts']['slurm']['copy_environment'] = False
@@ -1029,15 +1208,14 @@
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             universal_newlines=True,
             input=expected_script
         )
 
 
-
 class TestQdel(unittest.TestCase):
     @patch('fsl_sub_plugin_slurm.which', autospec=True)
     @patch('fsl_sub_plugin_slurm.sp.run', autospec=True)
     def testqdel(self, mock_spr, mock_which):
         pid = 1234
         mock_which.return_value = '/usr/bin/scancel'
         mock_spr.return_value = subprocess.CompletedProcess(
@@ -1202,36 +1380,37 @@
             task_output_keys.sort()
             self.assertListEqual(task_output_keys, self.task_expected_keys)
             self.assertDictEqual(job_stat, self.sacct_failedbatch_job)
 
 
 class TestQueueCapture(unittest.TestCase):
     def setUp(self):
-        self.sinfo_f_one_host = '''os:centos7,
+        self.sinfo_f_one_h = '''os:centos7,
 '''
-        self.sinfo_f_two_host = (
+        self.sinfo_f_two_h = (
             '''gpu,'''
             '''gpu_sku:P100,
             gpu,'''
             '''gpu_sku:V100,
 ''')
         self.sinfo_s = '''htc*\n'''
-        self.sinfo_G_two_host = 'gpu:p100:4(S:0-1)\ngpu:v100:8(S:0-1)'
-        self.sinfo_G_one_host = '(null)'
+        self.sinfo_G_two_h = 'gpu:p100:4(S:0-1)\ngpu:v100:8(S:0-1)'
+        self.sinfo_G_one_h = '(null)'
         self.sinfo_G_no_parens = 'gpu:gtx:2'
         self.sinfo_G_no_type = 'gpu:2(S:0-1)'
         self.sinfo_G_multiplier = 'gpu:2K(S:0-2023)'
         self.sinfo_G_list = 'gpu:p100:2(S:0-1),gpu:v100:2(S:0-1)'
-        self.sinfo_O_one_host = '''8                  UNLIMITED           64000             1-00:00:00          htc-node1
+        self.sinfo_O_one_h = '''8                  UNLIMITED           64000             1-00:00:00          htc-node1
 '''
-        self.sinfo_O_one_host_inf = '''8                  UNLIMITED           64000             infinite          htc-node1
+        self.sinfo_O_one_h_inf = '''8                  UNLIMITED           64000             infinite          htc-node1
 '''
-        self.sinfo_O_two_host = '''8                   UNLIMITED           384000               1-00:00:00          htc-gpu1
+        self.sinfo_O_two_h = ('''8                   UNLIMITED           384000               1-00:00:00          '''
+                              '''htc-gpu1
 16                 UNLIMITED           512000               5-00:00:00          htc-gpu2
-'''
+''')
 
     @patch('fsl_sub_plugin_slurm._sinfo_cmd', return_value='/usr/bin/sinfo')
     def test__get_queue_gres(self, mock_sinfo):
         with patch('fsl_sub_plugin_slurm.sp.run') as mock_spr:
             with self.subTest('No Type'):
                 mock_spr.return_value = subprocess.CompletedProcess(
                     ['sinfo', '%G', ], 0, self.sinfo_G_no_type
@@ -1262,43 +1441,43 @@
                 )
                 gres = fsl_sub_plugin_slurm._get_queue_gres('htc')
                 self.assertDictEqual(
                     gres,
                     {'gpu': [('p100', 2), ('v100', 2), ]})
             with self.subTest("No GRES"):
                 mock_spr.return_value = subprocess.CompletedProcess(
-                    ['sinfo', '%G', ], 0, self.sinfo_G_one_host
+                    ['sinfo', '%G', ], 0, self.sinfo_G_one_h
                 )
                 gres = fsl_sub_plugin_slurm._get_queue_gres('htc')
                 self.assertDictEqual(gres, defaultdict(list))
             with self.subTest('Two hosts'):
                 mock_spr.return_value = subprocess.CompletedProcess(
-                    ['sinfo', '%G', ], 0, self.sinfo_G_two_host
+                    ['sinfo', '%G', ], 0, self.sinfo_G_two_h
                 )
                 gres = fsl_sub_plugin_slurm._get_queue_gres('htc')
                 self.assertDictEqual(gres, {'gpu': [('p100', 4, ), ('v100', 8, ), ], })
 
     @patch('fsl_sub_plugin_slurm._sinfo_cmd', return_value='/usr/bin/sinfo')
     def test__get_queue_info(self, mock_sinfo):
         with patch('fsl_sub_plugin_slurm.sp.run') as mock_spr:
             mock_spr.return_value = subprocess.CompletedProcess(
-                ['sinfo', '%f', ], 0, self.sinfo_O_one_host
+                ['sinfo', '%f', ], 0, self.sinfo_O_one_h
             )
             (qdef, comments) = fsl_sub_plugin_slurm._get_queue_info('htc')
             self.assertDictEqual(
                 qdef,
                 {
                     'cpus': 8,
                     'memory': 64,
                     'qname': 'htc',
                     'qtime': 1440,
                 })
         with patch('fsl_sub_plugin_slurm.sp.run') as mock_spr:
             mock_spr.return_value = subprocess.CompletedProcess(
-                ['sinfo', '%f', ], 0, self.sinfo_O_one_host_inf
+                ['sinfo', '%f', ], 0, self.sinfo_O_one_h_inf
             )
             (qdef, comments) = fsl_sub_plugin_slurm._get_queue_info('htc')
             self.assertDictEqual(
                 qdef,
                 {
                     'cpus': 8,
                     'memory': 64,
@@ -1306,41 +1485,41 @@
                     'qtime': 527039,
                 })
 
     @patch('fsl_sub_plugin_slurm._sinfo_cmd', return_value='/usr/bin/sinfo')
     def test__get_queue_features(self, mock_sinfo):
         with patch('fsl_sub_plugin_slurm.sp.run') as mock_spr:
             mock_spr.return_value = subprocess.CompletedProcess(
-                ['sinfo', '%f', ], 0, self.sinfo_f_one_host
+                ['sinfo', '%f', ], 0, self.sinfo_f_one_h
             )
             features = fsl_sub_plugin_slurm._get_queue_features('htc')
             self.assertDictEqual(features, {'os': ['centos7', ], })
         with patch('fsl_sub_plugin_slurm.sp.run') as mock_spr:
             mock_spr.return_value = subprocess.CompletedProcess(
-                ['sinfo', '%f', ], 0, self.sinfo_f_two_host
+                ['sinfo', '%f', ], 0, self.sinfo_f_two_h
             )
             features = fsl_sub_plugin_slurm._get_queue_features('htc')
             self.assertDictEqual(features, {'gpu': [], 'gpu_sku': ['P100', 'V100'], })
 
     @patch('fsl_sub_plugin_slurm._sinfo_cmd', return_value='/usr/bin/sinfo')
     @patch('fsl_sub_plugin_slurm.method_config', return_value=conf_dict['method_opts']['slurm'])
     def test_build_queue_defs(self, mock_mconf, mock_sinfo):
         with patch('fsl_sub_plugin_slurm.sp.run') as mock_spr:
             mock_spr.side_effect = (
                 subprocess.CompletedProcess(
                     ['sinfo', '-s', ], 0, self.sinfo_s
                 ),
                 subprocess.CompletedProcess(
-                    ['sinfo', '%O', ], 0, self.sinfo_O_one_host
+                    ['sinfo', '%O', ], 0, self.sinfo_O_one_h
                 ),
                 subprocess.CompletedProcess(
-                    ['sinfo', '%G', ], 0, self.sinfo_G_one_host
+                    ['sinfo', '%G', ], 0, self.sinfo_G_one_h
                 ),
                 subprocess.CompletedProcess(
-                    ['sinfo', '%f', ], 0, self.sinfo_f_one_host
+                    ['sinfo', '%f', ], 0, self.sinfo_f_one_h
                 )
             )
             qdefs = fsl_sub_plugin_slurm.build_queue_defs()
             yaml = YAML()
             yaml.width = 128
         expected_yaml = yaml.load('''queues:
   htc: # Queue name
@@ -1363,21 +1542,21 @@
         with self.subTest("Two hosts"):
             with patch('fsl_sub_plugin_slurm.sp.run') as mock_spr:
                 mock_spr.side_effect = (
                     subprocess.CompletedProcess(
                         ['sinfo', '-s', ], 0, self.sinfo_s
                     ),
                     subprocess.CompletedProcess(
-                        ['sinfo', '%O', ], 0, self.sinfo_O_two_host
+                        ['sinfo', '%O', ], 0, self.sinfo_O_two_h
                     ),
                     subprocess.CompletedProcess(
-                        ['sinfo', '%G', ], 0, self.sinfo_G_two_host
+                        ['sinfo', '%G', ], 0, self.sinfo_G_two_h
                     ),
                     subprocess.CompletedProcess(
-                        ['sinfo', '%f', ], 0, self.sinfo_f_two_host
+                        ['sinfo', '%f', ], 0, self.sinfo_f_two_h
                     )
                 )
                 qdefs = fsl_sub_plugin_slurm.build_queue_defs()
                 yaml = YAML()
                 yaml.width = 128
             expected_yaml = yaml.load(
                 '''queues:
```

### Comparing `fsl_sub_plugin_slurm-1.5.1/fsl_sub_plugin_slurm.egg-info/PKG-INFO` & `fsl_sub_plugin_slurm-1.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fsl-sub-plugin-slurm
-Version: 1.5.1
+Name: fsl_sub_plugin_slurm
+Version: 1.6.1
 Summary: FSL Cluster Submission Plugin for Slurm
 Home-page: https://git.fmrib.ox.ac.uk/fsl/fsl_sub_plugin_slurm
 Author: Duncan Mortimer
 Author-email: duncan.mortimer@ndcn.ox.ac.uk
 License: Apache License Version 2.0
 Project-URL: Documentation, https://fsl.fmrib.ox.ac.uk/fsl/fslwiki
 Project-URL: Source, https://git.fmrib.ox.ac.uk/fsl/fsl_sub_plugin_slurm
@@ -25,15 +25,16 @@
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fsl_sub_plugin_slurm
 
 Job submission to SLURM variant cluster queues.
-_Copyright 2018-2021, University of Oxford (Duncan Mortimer)_
+
+_Copyright 2018-2023 University of Oxford, Oxford, UK._
 
 ## Introduction
 
 fsl\_sub provides a consistent interface to various cluster backends, with a fall back to running tasks locally where no cluster is available.
 This fsl\_sub plugin provides support for submitting tasks to SLURM clusters.
 
 For installation instructions please see INSTALL.md; for building packages see BUILD.md.
@@ -59,24 +60,25 @@
 | copy\_environment | **True**/False | Whether to replicate the environment variables in the shell that called fsl_sub into the job's shell
 | has\_parallel_envs | **False**/True | SLURM does not provide parallel environments so this should always be false
 | script\_conf | **True**/False | Whether _--usesscript_ option to fsl_sub is available via this method. This option allows you to define the grid options as comments in a shell script and then provide this to the cluster for running. Should be set to True.
 | mail\_support | True/**False** | Whether the grid installation is configured to send email on job events.
 | mail\_modes | Dictionary of option lists | If the grid has email notifications turned on, this option configures the submission options for different verbosity levels, 'b' = job start, 'e' = job end, 'a' = job abort, 'f' = all events, 'n' = no mail. Each event type should then have a list of submission mail arguments that will be applied to the submitted job. Typically, these should not be edited.
 | mail\_mode | b/e/a/f/**n** | Which of the above mail_modes to use by default
 | notify\_ram\_usage | **True**/False | Whether to notify SLURM of the RAM you have requested. SLURM is typically configured to give jobs a small RAM allocation so you will invariably need this set to true.
-| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected *maximum* run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True').
+| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected **maximum** run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True').
 | array\_holds | **True**/False | Enable support array holds, e.g. sub-task 1 waits for parent sub-task 1.
 | array\_limit | **True**/False | Enable limiting number of concurrent array tasks.
 | job\_resources | **True**/False | Enable additional job resource specification support.
 | projects | **True**/False | Enable support for projects typically used auditing/charging purposes.
 | preseve\_modules | True/**False** | Whether to re-load shell modules on the compute node. Required if you have multiple CPU generations and per-generation optimised libraries configured with modules.
 | add_module_paths | **[]**/ a list | List of file system paths to search for modules in addition to the system defined ones. Useful if you have your own shell modules directory but need to allow the compute node to auto-set it's MODULEPATH environment variable (e.g. to a architecture specific folder). Only used when preserve_modules is True.
 | export\_vars | **[]**/List | List of environment variables that should transfered with the job to the compute node
-| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `jobid_wrapper.sh`. This file contains sufficient information to resubmit this job in the future.
+| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `wrapper_<jobid>.sh`. This file contains sufficient information to resubmit this job in the future. If the job fails to submit, this will be preserved in the file `wrapper_failed_<DD>-<MMM>-<YYYY>_<HH><MM><SS>.sh`.
 | extra\_args | **[]**/List | List of additional SLURM arguments to pass through to the sheduler.
+| strict_dependencies | True/**False** | Whether to use 'afterok' (True) or 'afterany' (False) when specifying simple job dependencies. This can also be controlled by the environment variable `FSLSUB_STRICTDEPS` (True="1", False="0").
 
 ### Coprocessor Configuration
 
 This plugin is not capable of automatically determining all the necessary information to configure your co-processors but will advise of the information it can find and propose queue definitions for these GPU resources.
 
 SLURM typically selects GPU resources with a GRES (Generic RESource) that defines the type and quantity of the co-processor. Where multiple classes of co-processor are available this might be selectable via the GRES or you may need to provide a _constraint_. If you would like to be able to support running on a class and all superior devices you need to be able to use constraints as GRES requests do not support logical combinations. The automatically generated configuration should include useful information about your GRES and constraints, but should you wish to obtain this information yourself use the commands:
 
@@ -132,7 +134,14 @@
 | | exclusive | True/**False** | Whether this queue is only used for co-processor requiring tasks. |
 
 Where a partition has obvious GRES or features that define GPUs a proposed GPU configuration will be added as comments to the start of the queue definition. You should review this, create/update the coproc_opts>cuda record with the information in the comments and then this section can be uncommented to enable GPU support.
 
 #### Compound Queues
 
 Some clusters may be configured with multiple variants of the same partition, e.g. short.a, short.b, with each queue having different hardware, perhaps CPU generation or maximum memory or memory available per slot. To maximise scheduling options you can define compound queues which have the configuration of the least capable constituent. To define a compound queue, the queue name (key of the YAML dictionary) should be a comma separated list of queue names (no space).
+
+## SLURM specific usage
+
+### Job dependencies
+
+The default dependency handler (`-j`) takes a job id and uses `--dependency=afterany:\<jobid>` to control job hierarchies of non-array tasks. To switch to the old behaviour (pre-version 1.6.0) of using `afterok` (ancestor job must complete successfully), either modify the method configuration to set `strict_dependencies` to True or set the environment variable `FSLSUB_STRICTDEPS` to "1".
+Where you need to specify complex dependencies you may pass the raw SLURM dependency description (without the `--dependency=`) in the `-j` argument. For array tasks, the `array_hold` argument is used instead of the `-j` argument. This can take the same forms as the `-j` argument (job ids or complex hold descriptions).
```

### Comparing `fsl_sub_plugin_slurm-1.5.1/setup.py` & `fsl_sub_plugin_slurm-1.6.1/setup.py`

 * *Files identical despite different names*

