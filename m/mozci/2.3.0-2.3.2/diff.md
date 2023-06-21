# Comparing `tmp/mozci-2.3.0.tar.gz` & `tmp/mozci-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozci-2.3.0.tar", max compression
+gzip compressed data, was "mozci-2.3.2.tar", max compression
```

## Comparing `mozci-2.3.0.tar` & `mozci-2.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    16725 2019-12-03 23:09:31.000000 mozci-2.3.0/LICENSE
--rw-r--r--   0        0        0      133 2020-09-01 14:24:53.000000 mozci-2.3.0/mozci/__init__.py
--rw-r--r--   0        0        0     6851 2023-04-11 15:35:25.841411 mozci-2.3.0/mozci/configuration.py
--rw-r--r--   0        0        0      621 2023-05-05 21:03:08.495205 mozci-2.3.0/mozci/console/application.py
--rw-r--r--   0        0        0    12771 2023-05-05 21:03:08.495205 mozci-2.3.0/mozci/console/commands/batch_execution.py
--rw-r--r--   0        0        0     9702 2023-05-05 21:03:08.495205 mozci-2.3.0/mozci/console/commands/check_backfills.py
--rw-r--r--   0        0        0     5040 2023-05-05 21:03:08.495205 mozci-2.3.0/mozci/console/commands/decision.py
--rw-r--r--   0        0        0    53038 2023-05-17 18:14:56.605802 mozci-2.3.0/mozci/console/commands/push.py
--rw-r--r--   0        0        0      172 2020-09-01 14:24:53.000000 mozci-2.3.0/mozci/data/__init__.py
--rw-r--r--   0        0        0     3470 2022-03-25 23:42:30.000000 mozci-2.3.0/mozci/data/base.py
--rw-r--r--   0        0        0     7104 2023-05-17 18:14:56.605802 mozci-2.3.0/mozci/data/contract.py
--rw-r--r--   0        0        0        0 2020-09-01 14:24:53.000000 mozci-2.3.0/mozci/data/sources/__init__.py
--rw-r--r--   0        0        0     4065 2023-04-11 15:35:25.751411 mozci-2.3.0/mozci/data/sources/artifact/__init__.py
--rw-r--r--   0        0        0     1884 2022-01-13 21:51:04.000000 mozci-2.3.0/mozci/data/sources/bugbug/__init__.py
--rw-r--r--   0        0        0      652 2022-01-13 21:50:58.000000 mozci-2.3.0/mozci/data/sources/hgmo/__init__.py
--rw-r--r--   0        0        0     6213 2022-04-28 11:16:06.000000 mozci-2.3.0/mozci/data/sources/taskcluster/__init__.py
--rw-r--r--   0        0        0     7624 2022-03-25 23:54:19.000000 mozci-2.3.0/mozci/data/sources/treeherder/__init__.py
--rw-r--r--   0        0        0     3135 2022-01-13 21:50:58.000000 mozci-2.3.0/mozci/errors.py
--rw-r--r--   0        0        0    60180 2023-04-12 14:41:42.404758 mozci-2.3.0/mozci/push.py
--rw-r--r--   0        0        0    21263 2023-05-17 18:14:56.605802 mozci-2.3.0/mozci/task.py
--rw-r--r--   0        0        0        0 2019-12-13 09:52:36.000000 mozci-2.3.0/mozci/util/__init__.py
--rw-r--r--   0        0        0     7787 2022-01-13 21:51:14.000000 mozci-2.3.0/mozci/util/cache_stores.py
--rw-r--r--   0        0        0      239 2023-05-17 18:14:56.605802 mozci-2.3.0/mozci/util/defs.py
--rw-r--r--   0        0        0     7168 2022-06-24 14:12:09.000000 mozci-2.3.0/mozci/util/hgmo.py
--rw-r--r--   0        0        0     1093 2020-09-01 14:24:53.000000 mozci-2.3.0/mozci/util/logging.py
--rw-r--r--   0        0        0     1585 2022-01-13 21:50:44.000000 mozci-2.3.0/mozci/util/memoize.py
--rw-r--r--   0        0        0     1025 2022-01-13 21:50:44.000000 mozci-2.3.0/mozci/util/req.py
--rw-r--r--   0        0        0     7139 2022-05-10 10:03:58.000000 mozci-2.3.0/mozci/util/taskcluster.py
--rw-r--r--   0        0        0     1087 2020-02-26 16:06:17.000000 mozci-2.3.0/mozci/util/yaml.py
--rw-r--r--   0        0        0     1168 2023-05-17 18:20:46.945702 mozci-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 mozci-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2019-12-03 23:09:31.000000 mozci-2.3.2/LICENSE
+-rw-r--r--   0        0        0      133 2020-09-01 14:24:53.000000 mozci-2.3.2/mozci/__init__.py
+-rw-r--r--   0        0        0     6851 2023-05-19 09:55:23.916343 mozci-2.3.2/mozci/configuration.py
+-rw-r--r--   0        0        0      925 2023-05-19 18:27:35.108952 mozci-2.3.2/mozci/console/application.py
+-rw-r--r--   0        0        0    12528 2023-06-21 16:35:15.738478 mozci-2.3.2/mozci/console/commands/batch_execution.py
+-rw-r--r--   0        0        0    10092 2023-06-21 16:34:38.348480 mozci-2.3.2/mozci/console/commands/check_backfills.py
+-rw-r--r--   0        0        0     5472 2023-06-21 16:34:38.268480 mozci-2.3.2/mozci/console/commands/decision.py
+-rw-r--r--   0        0        0    55871 2023-06-21 16:34:39.528480 mozci-2.3.2/mozci/console/commands/push.py
+-rw-r--r--   0        0        0      172 2020-09-01 14:24:53.000000 mozci-2.3.2/mozci/data/__init__.py
+-rw-r--r--   0        0        0     3470 2022-03-25 23:42:30.000000 mozci-2.3.2/mozci/data/base.py
+-rw-r--r--   0        0        0     7104 2023-05-19 09:55:23.926343 mozci-2.3.2/mozci/data/contract.py
+-rw-r--r--   0        0        0        0 2020-09-01 14:24:53.000000 mozci-2.3.2/mozci/data/sources/__init__.py
+-rw-r--r--   0        0        0     4065 2023-05-19 09:55:23.926343 mozci-2.3.2/mozci/data/sources/artifact/__init__.py
+-rw-r--r--   0        0        0     1884 2022-01-13 21:51:04.000000 mozci-2.3.2/mozci/data/sources/bugbug/__init__.py
+-rw-r--r--   0        0        0      652 2022-01-13 21:50:58.000000 mozci-2.3.2/mozci/data/sources/hgmo/__init__.py
+-rw-r--r--   0        0        0     6213 2022-04-28 11:16:06.000000 mozci-2.3.2/mozci/data/sources/taskcluster/__init__.py
+-rw-r--r--   0        0        0     7624 2022-03-25 23:54:19.000000 mozci-2.3.2/mozci/data/sources/treeherder/__init__.py
+-rw-r--r--   0        0        0     3135 2022-01-13 21:50:58.000000 mozci-2.3.2/mozci/errors.py
+-rw-r--r--   0        0        0    60180 2023-04-12 14:41:42.404758 mozci-2.3.2/mozci/push.py
+-rw-r--r--   0        0        0    21263 2023-05-19 09:55:23.926343 mozci-2.3.2/mozci/task.py
+-rw-r--r--   0        0        0        0 2019-12-13 09:52:36.000000 mozci-2.3.2/mozci/util/__init__.py
+-rw-r--r--   0        0        0     7787 2022-01-13 21:51:14.000000 mozci-2.3.2/mozci/util/cache_stores.py
+-rw-r--r--   0        0        0      239 2023-05-19 09:55:23.926343 mozci-2.3.2/mozci/util/defs.py
+-rw-r--r--   0        0        0     7168 2022-06-24 14:12:09.000000 mozci-2.3.2/mozci/util/hgmo.py
+-rw-r--r--   0        0        0     1093 2020-09-01 14:24:53.000000 mozci-2.3.2/mozci/util/logging.py
+-rw-r--r--   0        0        0     1585 2022-01-13 21:50:44.000000 mozci-2.3.2/mozci/util/memoize.py
+-rw-r--r--   0        0        0     1025 2022-01-13 21:50:44.000000 mozci-2.3.2/mozci/util/req.py
+-rw-r--r--   0        0        0     7139 2022-05-10 10:03:58.000000 mozci-2.3.2/mozci/util/taskcluster.py
+-rw-r--r--   0        0        0     1087 2020-02-26 16:06:17.000000 mozci-2.3.2/mozci/util/yaml.py
+-rw-r--r--   0        0        0     1174 2023-06-21 16:52:16.168342 mozci-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 mozci-2.3.2/PKG-INFO
```

### Comparing `mozci-2.3.0/LICENSE` & `mozci-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/configuration.py` & `mozci-2.3.2/mozci/configuration.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/console/commands/batch_execution.py` & `mozci-2.3.2/mozci/console/commands/batch_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import os
 import time
 import uuid
 from multiprocessing import Pool
 
 from cleo.commands.command import Command
+from cleo.helpers import option
 from loguru import logger
 
 from mozci.console.commands.push import (
     parse_and_log_details,
     prepare_for_analysis,
     retrieve_sheriff_intermittents,
     retrieve_sheriff_reals,
@@ -114,22 +115,23 @@
             }
         )
 
     return csv_rows
 
 
 class BatchClassificationCommand(Command):
-    """
-    Run the classification algorithm with various parameters combinations for all submitted pushes within the last 30 days
-
-    classify
-        {--workers= : Number of workers to use in order to parallelize the executions.}
-    """
-
-    name = "batch-classification"
+    name = "batch-execution classify"
+    description = "Run the classification algorithm with various parameters combinations for all submitted pushes within the last 30 days"
+    options = [
+        option(
+            "workers",
+            description="Number of workers to use in order to parallelize the executions.",
+            flag=False,
+        )
+    ]
 
     csv_header = (
         ["run_uuid", "push_uuid"]
         + PARAMETERS_NAMES
         + ["classification", "time_spent", "now"]
     )
 
@@ -184,19 +186,16 @@
         pushes = make_push_objects(
             from_date=from_date, to_date=to_date, branch="autoland"
         )
         return [{"rev": push.rev, "branch": push.branch} for push in pushes]
 
 
 class BatchEvaluationCommand(Command):
-    """
-    Evaluate and aggregate the results produced by the classify_batch_execution script
-
-    evaluate
-    """
+    name = "batch-execution evaluate"
+    description = "Evaluate and aggregate the results produced by the classify_batch_execution script"
 
     csv_header = [
         "configuration",
         "total_pushes",
         "classify_errors",
         "evaluate_errors",
         "correct_good",
@@ -351,25 +350,7 @@
             except Exception as e:
                 configs[config]["evaluate_errors"] += 1
                 self.line(
                     f"<error>An error occurred during the evaluation of the classify execution with run_uuid {row['run_uuid']}: {e}</error>"
                 )
 
         return configs
-
-
-class BatchExecutionCommands(Command):
-    """
-    Contains commands that operate on lots of pushes using lots of classification algorithm configurations.
-
-    batch-execution
-    """
-
-    name = "batch-execution"
-
-    commands = [
-        BatchClassificationCommand(),
-        BatchEvaluationCommand(),
-    ]
-
-    def handle(self):
-        return self.call("help", self._config.name)
```

### Comparing `mozci-2.3.0/mozci/console/commands/check_backfills.py` & `mozci-2.3.2/mozci/console/commands/check_backfills.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 from collections import namedtuple
 from itertools import groupby
 from typing import Any, Dict
 
 import requests
 from cleo.commands.command import Command
+from cleo.helpers import argument, option
 from loguru import logger
 
 from mozci import config
 from mozci.push import make_push_objects
 from mozci.util.defs import TASK_FINAL_STATES
 from mozci.util.taskcluster import (
     COMMUNITY_TASKCLUSTER_ROOT_URL,
@@ -24,34 +25,50 @@
 BackfillTask = namedtuple("BackfillTask", ["task_id", "label", "th_symbol", "state"])
 
 NOTIFICATION_BACKFILL_GROUP_COMPLETED = "Backfill tasks associated to the Treeherder symbol {th_symbol} for push [{push.branch}/{push.rev}](https://treeherder.mozilla.org/jobs?group_state=expanded&repo={push.branch}{tochange}{fromchange}{searchstr}) are all in a final state."
 
 
 class CheckBackfillsCommand(Command):
     """
-    Check if backfills on last pushes are finished and notify Sheriffs when they are.
-
-    check-backfills
-        {--branch=autoland : Branch the pushes belongs to (e.g autoland, try, etc).}
-        {--nb-pushes=40 : Number of recent pushes to retrieve for the check.}
-        {--environment=testing : Environment in which the analysis is running (testing, production, ...)}
-
     The command will execute the following workflow:
       1. Retrieve the last <--nb-pushes> Pushes on branch <--branch>
       => Then for each Push:
       2. Check if it has any associated actions triggered by Treeherder, using Taskcluster indexation
       3. Find potential backfill tasks
       4. Group them by backfill groups
       => For each backfill group on the Push:
       5. Check if all backfill tasks in this group are completed
       6. If so (and if the notification wasn't already sent), send a notification on Matrix alerting that this backfill group is completed
       7. Add the current task in a dedicated index to avoid sending multiple times the same notification
     """
 
     name = "check-backfills"
+    description = "Check if backfills on last pushes are finished and notify Sheriffs when they are"
+    arguments = [
+        argument(
+            "branch",
+            description="Branch the pushes belongs to (e.g autoland, try, etc).",
+            optional=True,
+            default="autoland",
+        )
+    ]
+    options = [
+        option(
+            "nb-pushes",
+            description="Number of recent pushes to retrieve for the check.",
+            flag=False,
+            default=40,
+        ),
+        option(
+            "environment",
+            description="Environment in which the analysis is running (testing, production, ...).",
+            flag=False,
+            default="testing",
+        ),
+    ]
 
     def handle(self) -> None:
         branch = self.option("branch")
         environment = self.option("environment")
         matrix_room = config.get("matrix-room-id")
         current_task_id = os.environ.get("TASK_ID")
```

### Comparing `mozci-2.3.0/mozci/console/commands/decision.py` & `mozci-2.3.2/mozci/console/commands/decision.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,51 @@
 # -*- coding: utf-8 -*-
 
 import os
 from datetime import datetime
 
 import taskcluster
 from cleo.commands.command import Command
+from cleo.helpers import argument, option
 
 from mozci.push import Push, make_push_objects
 from mozci.util.memoize import memoized_property
 from mozci.util.taskcluster import get_taskcluster_options
 
 
 class DecisionCommand(Command):
-    """
-    Taskcluster decision task to generate classification tasks
-
-    decision
-        {branch=autoland : Branch the push belongs to (e.g autoland, try, etc).}
-        {--nb-pushes=15 : Do not create tasks on taskcluster, simply output actions.}
-        {--dry-run : Do not create tasks on taskcluster, simply output actions.}
-        {--environment=testing : Environment in which the analysis is running (testing, production, ...)}
-    """
-
     name = "decision"
+    description = "Taskcluster decision task to generate classification tasks"
+    arguments = [
+        argument(
+            "branch",
+            description="Branch the push belongs to (e.g autoland, try, etc).",
+            optional=True,
+            default="autoland",
+        )
+    ]
+    options = [
+        option(
+            "nb-pushes",
+            description="Number of pushes to analyze.",
+            flag=False,
+            default=15,
+        ),
+        option(
+            "dry-run",
+            description="Do not create tasks on taskcluster, simply output actions.",
+            flag=True,
+        ),
+        option(
+            "environment",
+            description="Environment in which the analysis is running (testing, production, ...).",
+            flag=False,
+            default="testing",
+        ),
+    ]
 
     def handle(self):
         branch = self.argument("branch")
         dry_run = self.option("dry-run")
         nb_pushes = int(self.option("nb-pushes"))
 
         self.queue = (
```

### Comparing `mozci-2.3.0/mozci/console/commands/push.py` & `mozci-2.3.2/mozci/console/commands/push.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import Any, Dict, List, Optional, Tuple
 from urllib.parse import urlencode
 
 import arrow
 import taskcluster
 from cleo.commands.command import Command
 from cleo.exceptions import CleoNoSuchOptionError
+from cleo.helpers import argument, option
 from loguru import logger
 from tabulate import tabulate
 from taskcluster.exceptions import TaskclusterRestFailure
 
 from mozci import config
 from mozci.errors import PushNotFound, SourcesNotFound, TaskNotFound
 from mozci.push import (
@@ -65,21 +66,22 @@
 
 """
 
 TWO_INTS_TUPLE_REGEXP = r"^\((\d+), ?(\d+)\)$"
 
 
 class PushTasksCommand(Command):
-    """
-    List the tasks that ran on a push.
-
-    tasks
-        {rev : Head revision of the push.}
-        {branch : Branch the push belongs to (e.g autoland, try, etc).}
-    """
+    name = "push tasks"
+    description = "List the tasks that ran on a push"
+    arguments = [
+        argument("rev", description="Head revision of the push."),
+        argument(
+            "branch", description="Branch the push belongs to (e.g autoland, try, etc)."
+        ),
+    ]
 
     def handle(self):
         push = Push(self.argument("rev"), self.argument("branch"))
 
         table = []
         for task in sorted(push.tasks, key=lambda t: t.label):
             table.append([task.label, task.result or "running"])
@@ -186,35 +188,100 @@
                 parameter_type, f"--{option_name}", option
             )
 
     return classify_parameters
 
 
 class ClassifyCommand(Command):
-    """
-    Display the classification for a given push (or a range of pushes) as GOOD, BAD or UNKNOWN.
-
-    classify
-        {branch=autoland : Branch the push belongs to (e.g autoland, try, etc).}
-        {--rev= : Head revision of the push.}
-        {--from-date= : Lower bound of the push range (as a date in yyyy-mm-dd format or a human expression like "1 days ago").}
-        {--to-date= : Upper bound of the push range (as a date in yyyy-mm-dd format or a human expression like "1 days ago"), defaults to now.}
-        {--intermittent-confidence-threshold= : Medium confidence threshold used to classify the regressions.}
-        {--real-confidence-threshold= : High confidence threshold used to classify the regressions.}
-        {--use-possible-regressions= : Use possible regressions while classifying the regressions.}
-        {--unknown-from-regressions= : Unknown from regressions while classifying the regressions.}
-        {--consider-children-pushes-configs= : Consider children pushes configs while classifying the regressions.}
-        {--cross-config-counts= : Cross-config counts used to classify the regressions.}
-        {--consistent-failures-counts= : Consistent failures counts used to classify the regressions.}
-        {--output= : Path towards a directory to save a JSON file containing classification and regressions details in.}
-        {--show-intermittents : If set, print tasks that should be marked as intermittent.}
-        {--environment=testing : Environment in which the analysis is running (testing, production, ...)}
-        {--retrigger-limit=3 : Number of failing groups (missing information) to be retriggered, defaults to 3.}
-        {--backfill-limit=3 : Number of failing groups (missing information) to be backfilled, defaults to 3.}
-    """
+    name = "push classify"
+    description = "Display the classification for a given push (or a range of pushes) as GOOD, BAD or UNKNOWN"
+    arguments = [
+        argument(
+            "branch",
+            description="Branch the push belongs to (e.g autoland, try, etc).",
+            optional=True,
+            default="autoland",
+        )
+    ]
+    options = [
+        option("rev", description="Head revision of the push.", flag=False),
+        option(
+            "from-date",
+            description='Lower bound of the push range (as a date in yyyy-mm-dd format or a human expression like "1 days ago").',
+            flag=False,
+        ),
+        option(
+            "to-date",
+            description='Upper bound of the push range (as a date in yyyy-mm-dd format or a human expression like "1 days ago"), defaults to now.',
+            flag=False,
+        ),
+        option(
+            "intermittent-confidence-threshold",
+            description="Medium confidence threshold used to classify the regressions.",
+            flag=False,
+        ),
+        option(
+            "real-confidence-threshold",
+            description="High confidence threshold used to classify the regressions.",
+            flag=False,
+        ),
+        option(
+            "use-possible-regressions",
+            description="Use possible regressions while classifying the regressions.",
+            flag=True,
+        ),
+        option(
+            "unknown-from-regressions",
+            description="Unknown from regressions while classifying the regressions.",
+            flag=True,
+        ),
+        option(
+            "consider-children-pushes-configs",
+            description="Consider children pushes configs while classifying the regressions.",
+            flag=True,
+        ),
+        option(
+            "cross-config-counts",
+            description="Cross-config counts used to classify the regressions.",
+            flag=False,
+        ),
+        option(
+            "consistent-failures-counts",
+            description="Consistent failures counts used to classify the regressions.",
+            flag=False,
+        ),
+        option(
+            "output",
+            description="Path towards a directory to save a JSON file containing classification and regressions details in.",
+            flag=False,
+        ),
+        option(
+            "show-intermittents",
+            description="If set, print tasks that should be marked as intermittent.",
+            flag=True,
+        ),
+        option(
+            "environment",
+            description="Environment in which the analysis is running (testing, production, ...).",
+            flag=False,
+            default="testing",
+        ),
+        option(
+            "retrigger-limit",
+            description="Number of failing groups (missing information) to be retriggered.",
+            flag=False,
+            default=3,
+        ),
+        option(
+            "backfill-limit",
+            description="Number of failing groups (missing information) to be backfilled.",
+            flag=False,
+            default=3,
+        ),
+    ]
 
     def handle(self) -> None:
         self.branch = self.argument("branch")
 
         pushes = classify_commands_pushes(
             self.branch,
             self.option("from-date"),
@@ -682,35 +749,97 @@
             for result in classified_as_cause[name]
         )
         if ever_classified_as_cause:
             return ever_classified_as_cause
 
 
 class ClassifyEvalCommand(Command):
-    """
-    Evaluate the classification results for a given push (or a range of pushes) by comparing them with reality.
-
-    classify-eval
-        {branch=autoland : Branch the push belongs to (e.g autoland, try, etc).}
-        {--rev= : Head revision of the push.}
-        {--from-date= : Lower bound of the push range (as a date in yyyy-mm-dd format or a human expression like "1 days ago").}
-        {--to-date= : Upper bound of the push range (as a date in yyyy-mm-dd format or a human expression like "1 days ago"), defaults to now.}
-        {--intermittent-confidence-threshold= : Medium confidence threshold used to classify the regressions.}
-        {--real-confidence-threshold= : High confidence threshold used to classify the regressions.}
-        {--use-possible-regressions= : Use possible regressions while classifying the regressions.}
-        {--unknown-from-regressions= : Unknown from regressions while classifying the regressions.}
-        {--consider-children-pushes-configs= : Consider children pushes configs while classifying the regressions.}
-        {--cross-config-counts= : Cross-config counts used to classify the regressions.}
-        {--consistent-failures-counts= : Consistent failures counts used to classify the regressions.}
-        {--recalculate : If set, recalculate the classification instead of fetching an artifact.}
-        {--output= : Path towards a path to save a CSV file with classification states for various pushes.}
-        {--send-email : If set, also send the evaluation report by email instead of just logging it.}
-        {--detailed-classifications : If set, compare real/intermittent group classifications with Sheriff's ones.}
-        {--environment=testing : Environment in which the analysis is running (testing, production, ...)}
-    """
+    name = "push classify-eval"
+    description = "Evaluate the classification results for a given push (or a range of pushes) by comparing them with reality"
+    arguments = [
+        argument(
+            "branch",
+            description="Branch the push belongs to (e.g autoland, try, etc).",
+            optional=True,
+            default="autoland",
+        )
+    ]
+    options = [
+        option(
+            "from-date",
+            description='Lower bound of the push range (as a date in yyyy-mm-dd format or a human expression like "1 days ago").',
+            flag=False,
+        ),
+        option(
+            "to-date",
+            description='Upper bound of the push range (as a date in yyyy-mm-dd format or a human expression like "1 days ago"), defaults to now.',
+            flag=False,
+        ),
+        option(
+            "intermittent-confidence-threshold",
+            description="Medium confidence threshold used to classify the regressions.",
+            flag=False,
+        ),
+        option(
+            "real-confidence-threshold",
+            description="High confidence threshold used to classify the regressions.",
+            flag=False,
+        ),
+        option(
+            "use-possible-regressions",
+            description="Use possible regressions while classifying the regressions.",
+            flag=True,
+        ),
+        option(
+            "unknown-from-regressions",
+            description="Unknown from regressions while classifying the regressions.",
+            flag=True,
+        ),
+        option(
+            "consider-children-pushes-configs",
+            description="Consider children pushes configs while classifying the regressions.",
+            flag=True,
+        ),
+        option(
+            "cross-config-counts",
+            description="Cross-config counts used to classify the regressions.",
+            flag=False,
+        ),
+        option(
+            "consistent-failures-counts",
+            description="Consistent failures counts used to classify the regressions.",
+            flag=False,
+        ),
+        option(
+            "recalculate",
+            description="If set, recalculate the classification instead of fetching an artifact.",
+            flag=True,
+        ),
+        option(
+            "output",
+            description="Path towards a path to save a CSV file with classification states for various pushes.",
+            flag=False,
+        ),
+        option(
+            "send-email",
+            description="If set, also send the evaluation report by email instead of just logging it.",
+            flag=True,
+        ),
+        option(
+            "detailed-classifications",
+            description="If set, compare real/intermittent group classifications with Sheriff's ones.",
+            flag=True,
+        ),
+        option(
+            "environment",
+            description="Environment in which the analysis is running (testing, production, ...).",
+            flag=False,
+            default="testing",
+        ),
+    ]
 
     def handle(self) -> None:
         branch = self.argument("branch")
 
         self.line("<comment>Loading pushes...</comment>")
         self.pushes = classify_commands_pushes(
             branch,
@@ -1164,21 +1293,40 @@
                 error_line=f"**{error_line}**" if error_line else "",
                 stats=stats,
             ),
         )
 
 
 class ClassifyPerfCommand(Command):
-    """
-    Generate a CSV file with performance stats for all classification tasks
-
-    perf
-        {--environment=testing : Environment in which the analysis is running (testing, production, ...)}
-        {--output=perfs.csv: Output CSV file path}
-    """
+    name = "push perf"
+    description = (
+        "Generate a CSV file with performance stats for all classification tasks"
+    )
+    arguments = [
+        argument(
+            "branch",
+            description="Branch the push belongs to (e.g autoland, try, etc).",
+            optional=True,
+            default="autoland",
+        )
+    ]
+    options = [
+        option(
+            "environment",
+            description="Environment in which the analysis is running (testing, production, ...).",
+            flag=False,
+            default="testing",
+        ),
+        option(
+            "output",
+            description="Output CSV file path.",
+            flag=False,
+            default="perfs.csv",
+        ),
+    ]
 
     REGEX_ROUTE = re.compile(
         r"^index.project.mozci.classification.([\w\-]+).(revision|push).(\w+)$"
     )
 
     def handle(self) -> None:
         environment = self.option("environment")
@@ -1308,27 +1456,7 @@
                 continue
 
             yield task_status
 
         # Cache all tasks if all completed
         if all(t["status"]["state"] == "completed" for t in tasks):
             config.cache.add(cache_key, tasks, int(config["cache"]["retention"]))
-
-
-class PushCommands(Command):
-    """
-    Contains commands that operate on a single push.
-
-    push
-    """
-
-    name = "push"
-
-    commands = [
-        PushTasksCommand(),
-        ClassifyCommand(),
-        ClassifyEvalCommand(),
-        ClassifyPerfCommand(),
-    ]
-
-    def handle(self):
-        return self.call("help", self._config.name)
```

### Comparing `mozci-2.3.0/mozci/data/base.py` & `mozci-2.3.2/mozci/data/base.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/data/contract.py` & `mozci-2.3.2/mozci/data/contract.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/data/sources/artifact/__init__.py` & `mozci-2.3.2/mozci/data/sources/artifact/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/data/sources/bugbug/__init__.py` & `mozci-2.3.2/mozci/data/sources/bugbug/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/data/sources/hgmo/__init__.py` & `mozci-2.3.2/mozci/data/sources/hgmo/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/data/sources/taskcluster/__init__.py` & `mozci-2.3.2/mozci/data/sources/taskcluster/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/data/sources/treeherder/__init__.py` & `mozci-2.3.2/mozci/data/sources/treeherder/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/errors.py` & `mozci-2.3.2/mozci/errors.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/push.py` & `mozci-2.3.2/mozci/push.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/task.py` & `mozci-2.3.2/mozci/task.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/util/cache_stores.py` & `mozci-2.3.2/mozci/util/cache_stores.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/util/hgmo.py` & `mozci-2.3.2/mozci/util/hgmo.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/util/logging.py` & `mozci-2.3.2/mozci/util/logging.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/util/memoize.py` & `mozci-2.3.2/mozci/util/memoize.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/util/req.py` & `mozci-2.3.2/mozci/util/req.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/util/taskcluster.py` & `mozci-2.3.2/mozci/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/mozci/util/yaml.py` & `mozci-2.3.2/mozci/util/yaml.py`

 * *Files identical despite different names*

### Comparing `mozci-2.3.0/pyproject.toml` & `mozci-2.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mozci"
-version = "2.3.0"
+version = "2.3.2"
 description = ""
 authors = [
   "Andrew Halberstadt <ahal@mozilla.com>",
   "Marco Castelluccio <marco@mozilla.com>",
 ]
 
 [tool.poetry.scripts]
@@ -24,15 +24,15 @@
 requests = "~2"
 flake8 = ">=3,<5"
 pyyaml = ">=5,<7"
 taskcluster = ">=38"
 lru-dict = "^1.1.7"
 
 # Optional dependencies
-ValidX = "^0.7"
+ValidX = ">=0.7,<0.9"
 cleo = "^2.0.1"
 tabulate = ">=0.8.9,<0.10.0"
 arrow = "^1.2.2"
 markdown2 = "^2.4.2"
 json-e = "^4.4.3"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `mozci-2.3.0/PKG-INFO` & `mozci-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozci
-Version: 2.3.0
+Version: 2.3.2
 Summary: 
 Author: Andrew Halberstadt
 Author-email: ahal@mozilla.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cache
 Provides-Extra: cache-memcached
 Provides-Extra: cache-redis
 Provides-Extra: cache-s3
 Provides-Extra: cache-seeded-file
-Requires-Dist: ValidX (>=0.7,<0.8)
+Requires-Dist: ValidX (>=0.7,<0.9)
 Requires-Dist: appdirs (>=1,<2)
 Requires-Dist: arrow (>=1.2.2,<2.0.0)
 Requires-Dist: boto3 (>=1,<2) ; extra == "cache" or extra == "cache-s3"
 Requires-Dist: cachy (>=0,<1)
 Requires-Dist: cleo (>=2.0.1,<3.0.0)
 Requires-Dist: flake8 (>=3,<5)
 Requires-Dist: json-e (>=4.4.3,<5.0.0)
```

