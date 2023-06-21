# Comparing `tmp/nonebot_plugin_bam-0.2.0a1.tar.gz` & `tmp/nonebot_plugin_bam-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bam-0.2.0a1.tar", max compression
+gzip compressed data, was "nonebot_plugin_bam-0.2.0a2.tar", max compression
```

## Comparing `nonebot_plugin_bam-0.2.0a1.tar` & `nonebot_plugin_bam-0.2.0a2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1059 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/LICENSE
--rw-r--r--   0        0        0      663 2023-06-15 14:22:23.241393 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/__init__.py
--rw-r--r--   0        0        0     1574 2023-06-15 13:02:15.074738 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/activity.py
--rw-r--r--   0        0        0        0 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/__init__.py
--rw-r--r--   0        0        0    11587 2023-06-15 13:28:21.379404 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/activity.py
--rw-r--r--   0        0        0     2623 2023-06-15 13:30:12.670071 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/api.py
--rw-r--r--   0        0        0      766 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/live1.py
--rw-r--r--   0        0        0      832 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/live2.py
--rw-r--r--   0        0        0      624 2023-06-15 13:30:55.101501 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/user.py
--rw-r--r--   0        0        0     1836 2023-06-15 13:31:00.559739 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/wbi.py
--rw-r--r--   0        0        0      947 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/common.py
--rw-r--r--   0        0        0      371 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/config.py
--rw-r--r--   0        0        0       91 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/__init__.py
--rw-r--r--   0        0        0     1404 2023-06-14 18:24:18.904298 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/db.py
--rw-r--r--   0        0        0     3454 2023-06-15 13:08:52.469278 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/helper.py
--rw-r--r--   0        0        0      154 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/tables/__init__.py
--rw-r--r--   0        0        0      336 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/tables/bilibili_user.py
--rw-r--r--   0        0        0      468 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/tables/bilibili_user_status.py
--rw-r--r--   0        0        0      481 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/tables/follow_link.py
--rw-r--r--   0        0        0      311 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/tables/group.py
--rw-r--r--   0        0        0     5533 2023-06-15 13:05:10.058734 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/follow.py
--rw-r--r--   0        0        0     3192 2023-06-15 12:58:16.897376 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/group.py
--rw-r--r--   0        0        0        0 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/tasks/__init__.py
--rw-r--r--   0        0        0     5208 2023-06-15 13:29:49.270283 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/tasks/activity_monitor.py
--rw-r--r--   0        0        0     4166 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/tasks/live_monitor.py
--rw-r--r--   0        0        0     1131 2023-06-15 13:00:44.289439 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/user.py
--rw-r--r--   0        0        0     1223 2023-06-15 14:22:29.663608 nonebot_plugin_bam-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     4854 2023-06-15 14:10:02.101887 nonebot_plugin_bam-0.2.0a1/README.md
--rw-r--r--   0        0        0     5994 1970-01-01 00:00:00.000000 nonebot_plugin_bam-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-06-14 06:44:18.264807 nonebot_plugin_bam-0.2.0a2/LICENSE
+-rw-r--r--   0        0        0     4854 2023-06-16 08:56:03.559872 nonebot_plugin_bam-0.2.0a2/README.md
+-rw-r--r--   0        0        0      663 2023-06-16 09:21:09.846465 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/__init__.py
+-rw-r--r--   0        0        0     1574 2023-06-16 08:56:03.560453 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/activity.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:44:18.265535 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/__init__.py
+-rw-r--r--   0        0        0    11587 2023-06-16 08:56:03.560845 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/activity.py
+-rw-r--r--   0        0        0     2623 2023-06-16 08:56:03.561388 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/api.py
+-rw-r--r--   0        0        0      766 2023-06-14 06:44:18.266043 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/live1.py
+-rw-r--r--   0        0        0      832 2023-06-14 07:53:56.620081 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/live2.py
+-rw-r--r--   0        0        0      624 2023-06-14 07:52:16.640215 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/user.py
+-rw-r--r--   0        0        0     1836 2023-06-16 08:56:03.561693 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/wbi.py
+-rw-r--r--   0        0        0     1229 2023-06-16 09:18:53.017876 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/common.py
+-rw-r--r--   0        0        0      371 2023-06-14 09:43:07.419841 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/config.py
+-rw-r--r--   0        0        0       91 2023-06-14 06:44:18.266730 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/__init__.py
+-rw-r--r--   0        0        0     1404 2023-06-15 09:41:09.332144 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/db.py
+-rw-r--r--   0        0        0     3454 2023-06-16 08:56:03.562014 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/helper.py
+-rw-r--r--   0        0        0      154 2023-06-14 06:44:18.267190 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/tables/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-14 06:44:18.267312 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/tables/bilibili_user.py
+-rw-r--r--   0        0        0      468 2023-06-14 06:44:18.267419 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/tables/bilibili_user_status.py
+-rw-r--r--   0        0        0      481 2023-06-14 06:44:18.267541 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/tables/follow_link.py
+-rw-r--r--   0        0        0      311 2023-06-14 06:44:18.267650 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/tables/group.py
+-rw-r--r--   0        0        0     5533 2023-06-16 08:56:03.562318 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/follow.py
+-rw-r--r--   0        0        0     3192 2023-06-16 08:56:03.562951 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/group.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:44:18.268036 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/tasks/__init__.py
+-rw-r--r--   0        0        0     4694 2023-06-16 09:19:56.392130 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/tasks/activity_monitor.py
+-rw-r--r--   0        0        0     4017 2023-06-16 09:20:24.425842 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/tasks/live_monitor.py
+-rw-r--r--   0        0        0     1131 2023-06-16 08:56:03.564006 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/user.py
+-rw-r--r--   0        0        0     1315 2023-06-16 09:21:15.341132 nonebot_plugin_bam-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     5994 1970-01-01 00:00:00.000000 nonebot_plugin_bam-0.2.0a2/PKG-INFO
```

### Comparing `nonebot_plugin_bam-0.2.0a1/LICENSE` & `nonebot_plugin_bam-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/__init__.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .config import Config
 from .follow import cmd_follower_add, cmd_follower_list, cmd_follower_remove
 from .group import cmd_group_add, cmd_group_list, cmd_group_remove
 from .tasks.activity_monitor import task_check_new_activity
 from .tasks.live_monitor import task_check_all_live_status
 from .user import cmd_user_fetch
 
-__version__ = "0.2.0a1"
+__version__ = "0.2.0a2"
 
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name = "BAM",
     description="Bilibili Activity Monitor",
     usage="Bilibili用户动态/开播监控器",
```

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/activity.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/activity.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/activity.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/activity.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/api.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/live1.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/live1.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/live2.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/live2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/user.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/wbi.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/wbi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/db.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/helper.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/helper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/follow.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/follow.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/group.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/tasks/activity_monitor.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/tasks/activity_monitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import asyncio
 import traceback
 from datetime import datetime, timedelta
 from typing import Optional
 
-from nonebot import get_bot, require
+from nonebot import require
 from nonebot.log import logger
 
 from ..bilibili.activity import ActivityList, H5Activity, activity_list
-from ..common import send_exception_to_su
+from ..common import send_exception_to_su, try_get_bot
 from ..config import CONF
 from ..database import helper
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 JOB_ID = "activity_monitor"
-LOGNAME = "TASK:ACTIVITY"
+LOGNAME = "BTASK:ACTIVITY"
 INTERVAL = CONF.bam_monitor_task_interval
 
 
 @scheduler.scheduled_job(
     "interval",
     seconds=0,
     id=JOB_ID,
@@ -51,53 +51,50 @@
         )
         if latest == 0:  # first fetch, only get latest id
             for _, act in zip(range(1), actlist):
                 if act is not None:
                     latest = act.id
                     has_new = True
         else:  # get new activities
-            bot = get_bot()
+            bot = try_get_bot()
             for _, act in reversed(list(zip(range(3), actlist))):  # max send 3
-                if act is None:
+                if act is None or act.id <= latest or bot is None:
                     continue
-
-                if act.id > latest:
-                    has_new = True
-                    latest = act.id
-                    if bot is not None:
-                        group_message = f"叮铃铃铃！{user.nickname} 有新动态！\n{act.display()}"
-                        h5_share_card = None
-                        if isinstance(act, H5Activity):
-                            h5_share_card = act.h5_share_card()
-                        for link in user.groups:
-                            group_id = link.group_id
-                            at_users = link.at_users
-                            the_group_message = group_message
-                            if at_users:
-                                the_group_message += "\n"
-                                for at_user in at_users.split(";"):
-                                    the_group_message += f"[CQ:at,qq={at_user}]"
-                            logger.info(f"Send activity message: {the_group_message}")
-                            try:
-                                await bot.send_group_msg(
-                                    group_id=group_id,
-                                    message=the_group_message,
-                                    auto_escape=False,
-                                )
-                            except Exception as e:
-                                send_exception_to_su(e, the_group_message)
-                            if h5_share_card is not None:
-                                try:
-                                    await bot.send_group_msg(
-                                        group_id=group_id,
-                                        message=h5_share_card,
-                                        auto_escape=False,
-                                    )
-                                except Exception as e:
-                                    pass
+                has_new = True
+                latest = act.id
+                group_message = f"叮铃铃铃！{user.nickname} 有新动态！\n{act.display()}"
+                h5_share_card = None
+                if isinstance(act, H5Activity):
+                    h5_share_card = act.h5_share_card()
+                for link in user.groups:
+                    group_id = link.group_id
+                    at_users = link.at_users
+                    the_group_message = group_message
+                    if at_users:
+                        the_group_message += "\n"
+                        for at_user in at_users.split(";"):
+                            the_group_message += f"[CQ:at,qq={at_user}]"
+                    logger.info(f"Send activity message: {the_group_message}")
+                    try:
+                        await bot.send_group_msg(
+                            group_id=group_id,
+                            message=the_group_message,
+                            auto_escape=False,
+                        )
+                    except Exception as e:
+                        send_exception_to_su(e, the_group_message)
+                    if h5_share_card is not None:
+                        try:
+                            await bot.send_group_msg(
+                                group_id=group_id,
+                                message=h5_share_card,
+                                auto_escape=False,
+                            )
+                        except Exception as e:
+                            pass
     elif hasattr(actlist, "code"):
         logger.info(
             f"[{LOGNAME}] check {user.nickname}({user.uid}) failed: {actlist.code} {actlist.message}"
         )
     return has_new, latest
 
 
@@ -109,18 +106,14 @@
     user_newest_activity_ids = {}
 
     for user in filter(lambda u: len(u.groups) > 0, users.values()):
         actlist = None
         try:
             logger.info(f"[{LOGNAME}] checking {user.nickname} activities...")
             actlist = await activity_list(uid=user.uid)
-            if not actlist.ok and hasattr(actlist, "code"):
-                logger.warning(
-                    f"[{LOGNAME}] check {user.nickname}({user.uid})'s activities failed: {actlist.code} {actlist.message}"
-                )
         except Exception as e:
             logger.warning(
                 f"[{LOGNAME}] check {user.uid} activity list task failed: {str(e)}"
             )
         has_new, latest = await process_user_actlist(user, actlist)
 
         if has_new:
```

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/tasks/live_monitor.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/tasks/live_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
-import json
 import traceback
+from typing import Optional, cast
 
-from nonebot import get_bot, require
+from nonebot import require
 from nonebot.log import logger
 
-from ..common import send_exception_to_su
+from ..common import send_exception_to_su, try_get_bot
 from ..config import CONF
 from ..database import helper
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 JOB_ID = "live_monitor"
 LOGNAME = "BTASK:LIVE"
@@ -38,15 +38,15 @@
     except Exception as e:
         logger.warning(f"[{LOGNAME}] {type(e).__name__}: {repr(e)}")
         logger.warning(f"[{LOGNAME}] {traceback.format_exc()}")
         send_exception_to_su(e)
     scheduler.resume_job(JOB_ID)
 
 
-async def process_user_room_info(user, room: RoomInfo):
+async def process_user_room_info(user, room: Optional[RoomInfo]):
     ret = 0
 
     if room is None:
         return ret
 
     if room.ok:
         message = []
@@ -64,15 +64,15 @@
             ret = 1
 
         if user.status.live_status == True and room.isLive == False:
             logger.info(f"[{LOGNAME}] {user.nickname} is offline")
             message.extend([f"{user.nickname} 下播啦！", "期待着TA的下一次直播吧~"])
             ret = -1
 
-        bot = get_bot()
+        bot = try_get_bot()
         if bot is not None and len(message) > 0:
             group_message = "\n".join(message)
             for link in user.groups:
                 group_id = link.group_id
                 at_users = link.at_users
                 the_group_message = group_message
                 if at_users:
@@ -103,24 +103,20 @@
     live_become_closed_users = []
 
     for user in filter(lambda u: len(u.groups) > 0, users.values()):
         room = None
         try:
             logger.info(f"[{LOGNAME}] checking {user.nickname} live status...")
             room = await room_info(uid=user.uid, rid=user.rid)
-            if not room.ok and hasattr(room, "code"):
-                logger.warning(
-                    f"[{LOGNAME}] check {user.nickname}({user.uid})'s room failed: {room.code} {room.message}"
-                )
         except Exception as e:
             logger.warning(
                 f"[{LOGNAME}] check {user.uid} live status task failed: {str(e)}"
             )
 
-        ret = await process_user_room_info(user, room)
+        ret = await process_user_room_info(user, cast(Optional[RoomInfo], room))
 
         if ret > 0:
             live_become_open_users.append(user)
         if ret < 0:
             live_become_closed_users.append(user)
 
         await asyncio.sleep(INTERVAL)
```

### Comparing `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/user.py` & `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/pyproject.toml` & `nonebot_plugin_bam-0.2.0a2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "nonebot_plugin_bam"
-version = "0.2.0a1"
+version = "0.2.0a2"
 description = "Bilibili activity monitor plugin for nonebot"
 authors = ["7sDream <i@7sdre.am>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/7sDream/nonebot-plugin-bam"
 repository = "https://github.com/7sDream/nonebot-plugin-bam"
 keywords = ["nonebot", "bilibili", "qqbot"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Plugins",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "LICENSE",
 ]
```

### Comparing `nonebot_plugin_bam-0.2.0a1/README.md` & `nonebot_plugin_bam-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a1/PKG-INFO` & `nonebot_plugin_bam-0.2.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bam
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: Bilibili activity monitor plugin for nonebot
 Home-page: https://github.com/7sDream/nonebot-plugin-bam
 License: MIT
 Keywords: nonebot,bilibili,qqbot
 Author: 7sDream
 Author-email: i@7sdre.am
 Requires-Python: >=3.9,<4.0
```

