# Comparing `tmp/hoyo_daily_logins_helper-2.6.2.tar.gz` & `tmp/hoyo_daily_logins_helper-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo_daily_logins_helper-2.6.2.tar", max compression
+gzip compressed data, was "hoyo_daily_logins_helper-2.7.0.tar", max compression
```

## Comparing `hoyo_daily_logins_helper-2.6.2.tar` & `hoyo_daily_logins_helper-2.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34227 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/LICENSE
--rw-r--r--   0        0        0     5277 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/README.md
--rw-r--r--   0        0        0        0 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/__init__.py
--rw-r--r--   0        0        0       55 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/__main__.py
--rw-r--r--   0        0        0       80 2023-06-14 03:01:46.477008 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/_version.py
--rw-r--r--   0        0        0       27 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/consts.py
--rw-r--r--   0        0        0     6916 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/games.py
--rw-r--r--   0        0        0     2050 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/http.py
--rw-r--r--   0        0        0     7180 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/main.py
--rw-r--r--   0        0        0     3410 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/notifications.py
--rw-r--r--   0        0        0     2631 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/scheduler.py
--rw-r--r--   0        0        0      100 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/utils.py
--rw-r--r--   0        0        0     1713 2023-06-14 03:01:46.477008 hoyo_daily_logins_helper-2.6.2/pyproject.toml
--rw-r--r--   0        0        0     6188 1970-01-01 00:00:00.000000 hoyo_daily_logins_helper-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0    34227 2023-06-21 02:58:24.705789 hoyo_daily_logins_helper-2.7.0/LICENSE
+-rw-r--r--   0        0        0     6229 2023-06-21 02:58:24.705789 hoyo_daily_logins_helper-2.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 02:58:24.705789 hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/__init__.py
+-rw-r--r--   0        0        0       55 2023-06-21 02:58:24.705789 hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/__main__.py
+-rw-r--r--   0        0        0       80 2023-06-21 02:58:49.262246 hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/_version.py
+-rw-r--r--   0        0        0       27 2023-06-21 02:58:24.705789 hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/consts.py
+-rw-r--r--   0        0        0     7278 2023-06-21 02:58:24.705789 hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/games.py
+-rw-r--r--   0        0        0     2050 2023-06-21 02:58:24.705789 hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/http.py
+-rw-r--r--   0        0        0     7227 2023-06-21 02:58:24.705789 hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/main.py
+-rw-r--r--   0        0        0     3828 2023-06-21 02:58:24.705789 hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/notifications.py
+-rw-r--r--   0        0        0     3870 2023-06-21 02:58:24.705789 hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/scheduler.py
+-rw-r--r--   0        0        0      100 2023-06-21 02:58:24.705789 hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/utils.py
+-rw-r--r--   0        0        0     1713 2023-06-21 02:58:49.258246 hoyo_daily_logins_helper-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7140 1970-01-01 00:00:00.000000 hoyo_daily_logins_helper-2.7.0/PKG-INFO
```

### Comparing `hoyo_daily_logins_helper-2.6.2/LICENSE` & `hoyo_daily_logins_helper-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo_daily_logins_helper-2.6.2/README.md` & `hoyo_daily_logins_helper-2.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -162,12 +162,56 @@
     {type = "discord", webhook_url = "https://...."}
 ]
 
 [[accounts]]
 # ....
 ```
 
+You can globally disable failure or success reports by adding the ```on``` property to the webhook
+
+```toml
+[config]
+# ...
+notifications = [
+    {type = "discord", webhook_url = "https://....", on = ["failure"]}
+]
+
+[[accounts]]
+# ....
+```
+
+You can also set accounts to only report on failure if you set the ```report_on``` property.
+
+```toml
+[conifg]
+# ...
+
+[[accounts]]
+game = "genshin"
+report_on = ["failure"]
+```
+
+### Adjusting schedule times
+
+The daily logins reset is globally the same at 00:00 Asia/Shanghai, but for various
+reasons you might want to delay this, so we added an option for this in the accounts section.
+
+```toml
+[config]
+# ...
+
+[[accounts]]
+game = "genshin"
+# example for configuring everything
+checkin_time = {hour = 17, minute = 0, timezone = "Europe/Berlin"}
+
+[[accounts]]
+game = "starrail"
+# example for only configurating this partially, in this case we want to have the script run at 00:42
+checkin_time = {minute = 42}
+```
+
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/games.py` & `hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/games.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,28 +39,33 @@
     },
 }
 _CAPTCHA_MESSAGE = """Captcha is required, please sign into the website: %s"""
 _COULD_NOT_CLAIM = (
     "Could not automatically claim rewards, please log in "
     "manually again here: %s"
 )
+_DEFAULT_REPORT_ON = ("success", "failure")
 
 
 def game_perform_checkin(
         account_ident: str,
         game: str,
         cookie_str: str,
         language: str,
         notification_manager: NotificationManager | None,
         skip_checkin: bool = False,
+        report_on: list[str] = _DEFAULT_REPORT_ON,
 ):
     if game not in GAMES:
         msg = f"unknown game identifier found: {game}"
         raise Exception(msg)
 
+    # some initial sleeping to off-set multiple runs a bit
+    sleep_random_time(15.0)
+
     game_name = GAMES[game]["name"]
     event_base_url = GAMES[game]["event_base_url"]
     act_id = GAMES[game]["act_id"]
     login_url = GAMES[game]["login_url"]
 
     referer_url = "https://act.hoyolab.com/"
     reward_url = (
@@ -102,17 +107,15 @@
     awards_data = http_get_json(reward_url)
 
     awards = awards_data.get("data", {}).get("awards")
 
     logging.info(f"Checking in account for {today}...")
 
     # a normal human can't instantly click, so we wait a bit
-    sleep_time = random.uniform(2.0, 10.0)
-    logging.debug(f"Sleep for {sleep_time}")
-    time.sleep(sleep_time)
+    sleep_random_time()
 
     request_data = json.dumps({
         "act_id": act_id,
     }, ensure_ascii=False)
 
     if not skip_checkin:
         response = http_post_json(sign_url, headers=headers, data=request_data)
@@ -132,15 +135,15 @@
 
     new_total_sign_in_day = info_list.get("data", {}).get("total_sign_day")
     already_signed_in = info_list.get("data", {}).get("is_sign")
 
     if not already_signed_in or new_total_sign_in_day == total_sign_in_day:
         msg = _COULD_NOT_CLAIM % login_url
         logging.error(msg)
-        if notification_manager:
+        if notification_manager and "failure" in report_on:
             notification_manager.send(Notification(
                 success=False,
                 account_identifier=account_ident,
                 game_name=game_name,
                 message=msg,
             ))
         return
@@ -155,26 +158,26 @@
     if code == RET_CODE_ALREADY_SIGNED_IN:
         logging.info("Already signed in for today...")
         return
 
     if is_captcha_required(response):
         msg = _CAPTCHA_MESSAGE % login_url
         logging.error(msg)
-        if notification_manager:
+        if notification_manager and "failure" in report_on:
             notification_manager.send(Notification(
                 success=False,
                 account_identifier=account_ident,
                 game_name=game_name,
                 message=msg,
             ))
         return
 
     if code != 0:
         logging.error(response["message"])
-        if notification_manager:
+        if notification_manager and "failure" in report_on:
             notification_manager.send(Notification(
                 success=False,
                 account_identifier=account_ident,
                 game_name=game_name,
                 message=response["message"],
             ))
         return
@@ -182,15 +185,15 @@
     reward = awards[total_sign_in_day - 1]
 
     logging.info("Check-in complete!")
     logging.info(f"\tTotal Sign-in Days: {total_sign_in_day}")
     logging.info(f"\tReward: {reward['cnt']}x {reward['name']}")
     logging.info(f"\tMessage: {response['message']}")
 
-    if notification_manager:
+    if notification_manager and "success" in report_on:
         notification_manager.send(Notification(
             success=True,
             account_identifier=account_ident,
             game_name=game_name,
             message=response["message"],
             custom_fields=[
                 {
@@ -212,7 +215,13 @@
     gt = response["gt_result"]["gt"]
     challenge = response["gt_result"]["challenge"]
 
     if not gt and not challenge:
         return False
 
     return True
+
+
+def sleep_random_time(until: float = 30.0):
+    sleep_time = random.uniform(2.0, until)
+    logging.debug(f"Sleep for {sleep_time}")
+    time.sleep(sleep_time)
```

### Comparing `hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/http.py` & `hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/http.py`

 * *Files identical despite different names*

### Comparing `hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/main.py` & `hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,19 @@
         )
         sys.exit(1)
 
     if args.user_agent:
         http_set_user_agent(args.user_agent)
 
     if enable_scheduler:
-        run_scheduler(config_data, args.language, notification_manager)
+        run_scheduler(
+            config_data,
+            args.language,
+            notification_manager,
+        )
         return
 
     for index, game in enumerate(args.game):
         identifier = f"Account #{index}"
         cookie = args.cookie[index]
 
         if account_identifiers[index]:
```

### Comparing `hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/notifications.py` & `hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/notifications.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,36 +14,50 @@
     account_identifier: str
     message: str
     custom_fields: list[dict] = ()
 
 
 @dataclass
 class _NotificationHandler:
-    pass
+    on: list[str]
 
     @staticmethod
     def create(data: dict):
         raise NotImplementedError
 
     def send(self, notification: Notification):
         raise NotImplementedError
 
+    def run_on_success(self) -> bool:
+        return "success" in self.on
+
+    def run_on_failure(self) -> bool:
+        return "failure" in self.on
+
 
 @dataclass
 class _DiscordNotificationHandler(_NotificationHandler):
     webhook_url: str
 
     @staticmethod
     def create(data: dict):
         if "webhook_url" not in data:
             msg = "No webhook_url defined in Discord notifications"
             raise Exception(msg)
-        return _DiscordNotificationHandler(data["webhook_url"])
+        if "on" not in data:
+            data["on"] = ["success", "failure"]
+        return _DiscordNotificationHandler(data["on"], data["webhook_url"])
 
     def send(self, notification: Notification):
+        if notification.success and not self.run_on_success():
+            return
+
+        if not notification.success and not self.run_on_failure():
+            return
+
         color_success = 4431943
         color_failure = 15022389
 
         fields = [
             {
                 "name": "Game",
                 "value": notification.game_name,
```

### Comparing `hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/scheduler.py` & `hoyo_daily_logins_helper-2.7.0/hoyo_daily_logins_helper/scheduler.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,62 +5,84 @@
 
 import pytz
 from scheduler import Scheduler
 
 from hoyo_daily_logins_helper.games import GAMES, game_perform_checkin
 from hoyo_daily_logins_helper.notifications import NotificationManager
 
-_RESET_TIME = time(tzinfo=pytz.timezone("Asia/Shanghai"), hour=0, minute=5)
+_RESET_HOUR = 0
+_RESET_MINUTE = 5
+_RESET_TIMEZONE = "Asia/Shanghai"
 
 
 def run_scheduler(
         config_data: dict,
         language: str,
         notifications_manager: NotificationManager | None,
 ):
     logging.info("Run in scheduler mode")
 
     tz = datetime.now(UTC).astimezone().tzinfo
 
     schedule = Scheduler(tzinfo=tz)
 
     accounts = config_data.get("accounts", [])
+    times = []
 
     for index, account in enumerate(accounts):
         identifier = account.get("identifier", None)
+        checkin_time = account.get("checkin_time", None)
+        report_on = account.get("report_on", ["success", "failure"])
 
         if not identifier:
             identifier = f"Account #{index}"
 
         game = account.get("game")
         game_name = GAMES[game]["name"]
 
+        if checkin_time is None:
+            checkin_time = {}
+
+        if "hour" not in checkin_time:
+            checkin_time["hour"] = _RESET_HOUR
+        if "minute" not in checkin_time:
+            checkin_time["minute"] = _RESET_MINUTE
+        if "timezone" not in checkin_time:
+            checkin_time["timezone"] = _RESET_TIMEZONE
+
         schedule.daily(
-            _RESET_TIME,
+            time(
+                tzinfo=pytz.timezone(checkin_time["timezone"]),
+                hour=checkin_time["hour"],
+                minute=checkin_time["minute"],
+            ),
             create_checkin_job(
                 identifier,
                 game,
                 account.get("cookie"),
                 language,
+                report_on,
                 notifications_manager,
             ),
         )
 
+        times.append((game_name, identifier, checkin_time))
+
         logging.info(
             f"Added {game_name} account '{identifier}' to scheduler",
         )
 
     if len(schedule.jobs) == 0:
         logging.error("No jobs scheduled")
         sys.exit(1)
 
-    print_time_till_next_reset()
+    print_time_till_next_reset(times)
     schedule.hourly(
         time(minute=0, second=0, tzinfo=tz),
-        print_time_till_next_reset,
+        lambda: print_time_till_next_reset(times),
     )
 
     logging.debug("Job schedule:")
     logging.debug(schedule)
 
     while True:
         schedule.exec_jobs()
@@ -68,40 +90,57 @@
 
 
 def create_checkin_job(
         account_ident: str,
         game: str,
         cookie_str: str,
         language: str,
+        report_on: list[str],
         notification_manager: NotificationManager | None,
 ):
     def _checkin_job():
         logging.info(f"Running scheduler for '{account_ident}'...")
         game_perform_checkin(
             account_ident,
             game,
             cookie_str,
             language,
             notification_manager,
+            report_on=report_on,
         )
 
     return _checkin_job
 
 
-def print_time_till_next_reset():
+def print_time_till_next_reset(times: list[tuple]):
     tz = datetime.now(UTC).astimezone().tzinfo
     now = datetime.now(tz=tz)
-    next_reset = datetime.now(tz=_RESET_TIME.tzinfo)
-    next_reset = next_reset.replace(
-        hour=_RESET_TIME.hour,
-        minute=_RESET_TIME.minute,
-        second=0,
-    )
 
-    if next_reset < now:
-        next_reset = next_reset + timedelta(days=1)
+    lines = []
+
+    for game_name, identifier, checkin_time in times:
+        reset_time = time(
+            tzinfo=pytz.timezone(checkin_time["timezone"]),
+            hour=checkin_time["hour"],
+            minute=checkin_time["minute"],
+        )
+
+        next_reset = datetime.now(tz=reset_time.tzinfo)
+        next_reset = next_reset.replace(
+            hour=reset_time.hour,
+            minute=reset_time.minute,
+            second=0,
+        )
 
-    diff = next_reset - now
+        if next_reset < now:
+            next_reset = next_reset + timedelta(days=1)
 
-    hours = round(diff.total_seconds() / 60 / 60, 1)
+        diff = next_reset - now
+
+        hours = round(diff.total_seconds() / 60 / 60, 1)
+
+        lines.append(
+            f"\t{game_name} - {identifier} in {hours} hours",
+        )
 
-    logging.info(f"Next reset time is in {hours} hours.")
+    lines_str = "\n".join(lines)
+    logging.info(f"Next reset times are:\n{lines_str}")
```

### Comparing `hoyo_daily_logins_helper-2.6.2/pyproject.toml` & `hoyo_daily_logins_helper-2.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 packages = [{include = "hoyo_daily_logins_helper"}]
 keywords = ["genshin", "genshin-impact", "starrail", "honkai-starrail", "game"]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
 
 # required, but set automatically by poetry-dynamic-versioning
-version = "2.6.2"
+version = "2.7.0"
 
 [tool.poetry.scripts]
 hoyo-daily-logins-helper = "hoyo_daily_logins_helper.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
```

### Comparing `hoyo_daily_logins_helper-2.6.2/PKG-INFO` & `hoyo_daily_logins_helper-2.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.6.2
+Version: 2.7.0
 Summary: Get hoyo daily login rewards automatically!
 Home-page: https://github.com/atomicptr/hoyo-daily-logins-helper
 License: GPL-3.0-or-later
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Author: Christopher Kaster
 Author-email: me@atomicptr.de
 Requires-Python: >=3.11,<4.0
@@ -183,12 +183,56 @@
     {type = "discord", webhook_url = "https://...."}
 ]
 
 [[accounts]]
 # ....
 ```
 
+You can globally disable failure or success reports by adding the ```on``` property to the webhook
+
+```toml
+[config]
+# ...
+notifications = [
+    {type = "discord", webhook_url = "https://....", on = ["failure"]}
+]
+
+[[accounts]]
+# ....
+```
+
+You can also set accounts to only report on failure if you set the ```report_on``` property.
+
+```toml
+[conifg]
+# ...
+
+[[accounts]]
+game = "genshin"
+report_on = ["failure"]
+```
+
+### Adjusting schedule times
+
+The daily logins reset is globally the same at 00:00 Asia/Shanghai, but for various
+reasons you might want to delay this, so we added an option for this in the accounts section.
+
+```toml
+[config]
+# ...
+
+[[accounts]]
+game = "genshin"
+# example for configuring everything
+checkin_time = {hour = 17, minute = 0, timezone = "Europe/Berlin"}
+
+[[accounts]]
+game = "starrail"
+# example for only configurating this partially, in this case we want to have the script run at 00:42
+checkin_time = {minute = 42}
+```
+
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

