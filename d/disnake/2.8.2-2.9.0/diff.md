# Comparing `tmp/disnake-2.8.2.tar.gz` & `tmp/disnake-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disnake-2.8.2.tar", last modified: Wed Jun 21 16:24:57 2023, max compression
+gzip compressed data, was "disnake-2.9.0.tar", last modified: Wed Jun 21 16:26:12 2023, max compression
```

## Comparing `disnake-2.8.2.tar` & `disnake-2.9.0.tar`

### file list

```diff
@@ -1,183 +1,180 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.854082 disnake-2.8.2/
--rw-r--r--   0 root         (0) root         (0)     1125 2022-07-27 17:57:08.000000 disnake-2.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      217 2023-02-05 21:19:05.000000 disnake-2.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4899 2023-06-21 16:24:57.854082 disnake-2.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3705 2023-02-05 21:19:05.000000 disnake-2.8.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.806082 disnake-2.8.2/disnake/
--rw-r--r--   0 root         (0) root         (0)     2115 2023-06-21 16:23:17.000000 disnake-2.8.2/disnake/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10059 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/__main__.py
--rw-r--r--   0 root         (0) root         (0)    67140 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/abc.py
--rw-r--r--   0 root         (0) root         (0)    25770 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/activity.py
--rw-r--r--   0 root         (0) root         (0)    36947 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/app_commands.py
--rw-r--r--   0 root         (0) root         (0)    11361 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/appinfo.py
--rw-r--r--   0 root         (0) root         (0)     3819 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/application_role_connection.py
--rw-r--r--   0 root         (0) root         (0)    14845 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/asset.py
--rw-r--r--   0 root         (0) root         (0)    31284 2023-06-21 16:23:17.000000 disnake-2.8.2/disnake/audit_logs.py
--rw-r--r--   0 root         (0) root         (0)    26287 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/automod.py
--rw-r--r--   0 root         (0) root         (0)     2697 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/backoff.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/bans.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.814082 disnake-2.8.2/disnake/bin/
--rw-r--r--   0 root         (0) root         (0)     1487 2022-07-27 17:57:08.000000 disnake-2.8.2/disnake/bin/COPYING
--rw-r--r--   0 root         (0) root         (0)   441856 2022-07-27 17:57:08.000000 disnake-2.8.2/disnake/bin/libopus-0.x64.dll
--rw-r--r--   0 root         (0) root         (0)   366080 2022-07-27 17:57:08.000000 disnake-2.8.2/disnake/bin/libopus-0.x86.dll
--rw-r--r--   0 root         (0) root         (0)   126910 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/channel.py
--rw-r--r--   0 root         (0) root         (0)    93802 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/client.py
--rw-r--r--   0 root         (0) root         (0)     8925 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/colour.py
--rw-r--r--   0 root         (0) root         (0)    22674 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/components.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/context_managers.py
--rw-r--r--   0 root         (0) root         (0)      733 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/custom_warnings.py
--rw-r--r--   0 root         (0) root         (0)    28043 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/embeds.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/emoji.py
--rw-r--r--   0 root         (0) root         (0)    43776 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/enums.py
--rw-r--r--   0 root         (0) root         (0)    13422 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.778082 disnake-2.8.2/disnake/ext/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.826082 disnake-2.8.2/disnake/ext/commands/
--rw-r--r--   0 root         (0) root         (0)      616 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ext/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ext/commands/_types.py
--rw-r--r--   0 root         (0) root         (0)    27455 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/base_core.py
--rw-r--r--   0 root         (0) root         (0)    21192 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/bot.py
--rw-r--r--   0 root         (0) root         (0)    20651 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/bot_base.py
--rw-r--r--   0 root         (0) root         (0)    33920 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/cog.py
--rw-r--r--   0 root         (0) root         (0)    22428 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/common_bot_base.py
--rw-r--r--   0 root         (0) root         (0)    13932 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/context.py
--rw-r--r--   0 root         (0) root         (0)    42815 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/converter.py
--rw-r--r--   0 root         (0) root         (0)    11878 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ext/commands/cooldowns.py
--rw-r--r--   0 root         (0) root         (0)    88259 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/core.py
--rw-r--r--   0 root         (0) root         (0)    15025 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/ctx_menus_core.py
--rw-r--r--   0 root         (0) root         (0)      248 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ext/commands/custom_warnings.py
--rw-r--r--   0 root         (0) root         (0)    31523 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ext/commands/errors.py
--rw-r--r--   0 root         (0) root         (0)    20566 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/flag_converter.py
--rw-r--r--   0 root         (0) root         (0)     6136 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/flags.py
--rw-r--r--   0 root         (0) root         (0)    47166 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ext/commands/help.py
--rw-r--r--   0 root         (0) root         (0)    54110 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/interaction_bot_base.py
--rw-r--r--   0 root         (0) root         (0)    46620 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/params.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ext/commands/py.typed
--rw-r--r--   0 root         (0) root         (0)    31127 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/slash_core.py
--rw-r--r--   0 root         (0) root         (0)     4998 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ext/commands/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.826082 disnake-2.8.2/disnake/ext/mypy_plugin/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ext/mypy_plugin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.826082 disnake-2.8.2/disnake/ext/tasks/
--rw-r--r--   0 root         (0) root         (0)    26863 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ext/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ext/tasks/py.typed
--rw-r--r--   0 root         (0) root         (0)     4289 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/file.py
--rw-r--r--   0 root         (0) root         (0)    73724 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/flags.py
--rw-r--r--   0 root         (0) root         (0)    37896 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/gateway.py
--rw-r--r--   0 root         (0) root         (0)   177691 2023-06-21 16:23:17.000000 disnake-2.8.2/disnake/guild.py
--rw-r--r--   0 root         (0) root         (0)     3973 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/guild_preview.py
--rw-r--r--   0 root         (0) root         (0)    25620 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/guild_scheduled_event.py
--rw-r--r--   0 root         (0) root         (0)    90000 2023-06-21 16:23:17.000000 disnake-2.8.2/disnake/http.py
--rw-r--r--   0 root         (0) root         (0)    12966 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/i18n.py
--rw-r--r--   0 root         (0) root         (0)    12858 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/integrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.830082 disnake-2.8.2/disnake/interactions/
--rw-r--r--   0 root         (0) root         (0)      336 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/interactions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12145 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/interactions/application_command.py
--rw-r--r--   0 root         (0) root         (0)    68858 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/interactions/base.py
--rw-r--r--   0 root         (0) root         (0)     6736 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/interactions/message.py
--rw-r--r--   0 root         (0) root         (0)     5135 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/interactions/modal.py
--rw-r--r--   0 root         (0) root         (0)    21671 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/invite.py
--rw-r--r--   0 root         (0) root         (0)    34946 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/iterators.py
--rw-r--r--   0 root         (0) root         (0)    40246 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/member.py
--rw-r--r--   0 root         (0) root         (0)     5671 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/mentions.py
--rw-r--r--   0 root         (0) root         (0)    86781 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/message.py
--rw-r--r--   0 root         (0) root         (0)      536 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/mixins.py
--rw-r--r--   0 root         (0) root         (0)     1879 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/object.py
--rw-r--r--   0 root         (0) root         (0)     2700 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/oggparse.py
--rw-r--r--   0 root         (0) root         (0)    14584 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/opus.py
--rw-r--r--   0 root         (0) root         (0)     8265 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/partial_emoji.py
--rw-r--r--   0 root         (0) root         (0)    42227 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/permissions.py
--rw-r--r--   0 root         (0) root         (0)    26437 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/player.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-27 17:57:08.000000 disnake-2.8.2/disnake/py.typed
--rw-r--r--   0 root         (0) root         (0)    14090 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/raw_models.py
--rw-r--r--   0 root         (0) root         (0)     6159 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/reaction.py
--rw-r--r--   0 root         (0) root         (0)    16293 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/role.py
--rw-r--r--   0 root         (0) root         (0)    21116 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/shard.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/stage_instance.py
--rw-r--r--   0 root         (0) root         (0)    88546 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/state.py
--rw-r--r--   0 root         (0) root         (0)    15216 2023-06-21 16:23:17.000000 disnake-2.8.2/disnake/sticker.py
--rw-r--r--   0 root         (0) root         (0)     3658 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/team.py
--rw-r--r--   0 root         (0) root         (0)     8722 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/template.py
--rw-r--r--   0 root         (0) root         (0)    39657 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/threads.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.842082 disnake-2.8.2/disnake/types/
--rw-r--r--   0 root         (0) root         (0)      212 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/activity.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/types/appinfo.py
--rw-r--r--   0 root         (0) root         (0)      487 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/types/application_role_connection.py
--rw-r--r--   0 root         (0) root         (0)     7371 2023-06-21 16:23:17.000000 disnake-2.8.2/disnake/types/audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/types/automod.py
--rw-r--r--   0 root         (0) root         (0)     4801 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/types/channel.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/components.py
--rw-r--r--   0 root         (0) root         (0)     1310 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/embed.py
--rw-r--r--   0 root         (0) root         (0)      471 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/emoji.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/types/gateway.py
--rw-r--r--   0 root         (0) root         (0)     5486 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/types/guild.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/guild_scheduled_event.py
--rw-r--r--   0 root         (0) root         (0)       91 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/types/i18n.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/integration.py
--rw-r--r--   0 root         (0) root         (0)     9538 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/types/interactions.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/invite.py
--rw-r--r--   0 root         (0) root         (0)      716 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/types/member.py
--rw-r--r--   0 root         (0) root         (0)     3056 2023-06-21 16:23:17.000000 disnake-2.8.2/disnake/types/message.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/types/role.py
--rw-r--r--   0 root         (0) root         (0)      166 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/snowflake.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-06-21 16:23:17.000000 disnake-2.8.2/disnake/types/sticker.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-06-21 16:23:17.000000 disnake-2.8.2/disnake/types/team.py
--rw-r--r--   0 root         (0) root         (0)      557 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/template.py
--rw-r--r--   0 root         (0) root         (0)     1862 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/threads.py
--rw-r--r--   0 root         (0) root         (0)      483 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/user.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/voice.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/webhook.py
--rw-r--r--   0 root         (0) root         (0)      413 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/welcome_screen.py
--rw-r--r--   0 root         (0) root         (0)      958 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/types/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.846082 disnake-2.8.2/disnake/ui/
--rw-r--r--   0 root         (0) root         (0)      373 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29552 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ui/action_row.py
--rw-r--r--   0 root         (0) root         (0)    11042 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ui/button.py
--rw-r--r--   0 root         (0) root         (0)     5411 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ui/item.py
--rw-r--r--   0 root         (0) root         (0)     8617 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ui/modal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.850082 disnake-2.8.2/disnake/ui/select/
--rw-r--r--   0 root         (0) root         (0)      592 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ui/select/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5968 2023-03-02 19:46:40.000000 disnake-2.8.2/disnake/ui/select/base.py
--rw-r--r--   0 root         (0) root         (0)     7940 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/ui/select/channel.py
--rw-r--r--   0 root         (0) root         (0)     6611 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/ui/select/mentionable.py
--rw-r--r--   0 root         (0) root         (0)     6251 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/ui/select/role.py
--rw-r--r--   0 root         (0) root         (0)    11403 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/ui/select/string.py
--rw-r--r--   0 root         (0) root         (0)     6340 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/ui/select/user.py
--rw-r--r--   0 root         (0) root         (0)     4599 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/ui/text_input.py
--rw-r--r--   0 root         (0) root         (0)    19536 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/ui/view.py
--rw-r--r--   0 root         (0) root         (0)    14200 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/user.py
--rw-r--r--   0 root         (0) root         (0)    39348 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/utils.py
--rw-r--r--   0 root         (0) root         (0)    23354 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/voice_client.py
--rw-r--r--   0 root         (0) root         (0)     1342 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/voice_region.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.850082 disnake-2.8.2/disnake/webhook/
--rw-r--r--   0 root         (0) root         (0)      345 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/webhook/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66012 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/webhook/async_.py
--rw-r--r--   0 root         (0) root         (0)    42672 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/webhook/sync.py
--rw-r--r--   0 root         (0) root         (0)     6225 2023-03-02 19:46:41.000000 disnake-2.8.2/disnake/welcome_screen.py
--rw-r--r--   0 root         (0) root         (0)    13848 2023-02-05 21:19:05.000000 disnake-2.8.2/disnake/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.810082 disnake-2.8.2/disnake.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4899 2023-06-21 16:24:57.000000 disnake-2.8.2/disnake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4134 2023-06-21 16:24:57.000000 disnake-2.8.2/disnake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:24:57.000000 disnake-2.8.2/disnake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      425 2023-06-21 16:24:57.000000 disnake-2.8.2/disnake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-21 16:24:57.000000 disnake-2.8.2/disnake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4964 2023-03-02 19:46:41.000000 disnake-2.8.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.782082 disnake-2.8.2/requirements/
--rw-r--r--   0 root         (0) root         (0)      501 2023-03-02 19:43:54.000000 disnake-2.8.2/requirements/requirements_dev.txt
--rw-r--r--   0 root         (0) root         (0)      183 2023-02-05 21:19:05.000000 disnake-2.8.2/requirements/requirements_docs.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-02-05 21:19:05.000000 disnake-2.8.2/requirements/requirements_speed.txt
--rw-r--r--   0 root         (0) root         (0)      223 2023-02-05 21:19:05.000000 disnake-2.8.2/requirements/requirements_tools.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-09-29 19:24:42.000000 disnake-2.8.2/requirements/requirements_voice.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-02-05 21:19:05.000000 disnake-2.8.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 16:24:57.854082 disnake-2.8.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1965 2023-03-02 19:46:41.000000 disnake-2.8.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:24:57.854082 disnake-2.8.2/tests/
--rw-r--r--   0 root         (0) root         (0)     5854 2023-03-02 19:46:41.000000 disnake-2.8.2/tests/test_abc.py
--rw-r--r--   0 root         (0) root         (0)     1539 2023-02-05 21:19:05.000000 disnake-2.8.2/tests/test_colour.py
--rw-r--r--   0 root         (0) root         (0)    13955 2023-02-05 21:19:05.000000 disnake-2.8.2/tests/test_embeds.py
--rw-r--r--   0 root         (0) root         (0)    14422 2023-02-05 21:19:05.000000 disnake-2.8.2/tests/test_flags.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-02-05 21:19:05.000000 disnake-2.8.2/tests/test_http.py
--rw-r--r--   0 root         (0) root         (0)     4004 2023-02-05 21:19:05.000000 disnake-2.8.2/tests/test_mentions.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-03-02 19:46:41.000000 disnake-2.8.2/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-02-05 21:19:05.000000 disnake-2.8.2/tests/test_object.py
--rw-r--r--   0 root         (0) root         (0)    10977 2023-02-05 21:19:05.000000 disnake-2.8.2/tests/test_permissions.py
--rw-r--r--   0 root         (0) root         (0)    25451 2023-02-05 21:19:05.000000 disnake-2.8.2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.958299 disnake-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1125 2022-07-27 17:57:08.000000 disnake-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-21 16:25:59.000000 disnake-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5039 2023-06-21 16:26:12.958299 disnake-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-06-21 16:25:59.000000 disnake-2.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.930299 disnake-2.9.0/disnake/
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10110 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    71323 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/abc.py
+-rw-r--r--   0 root         (0) root         (0)    25789 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/activity.py
+-rw-r--r--   0 root         (0) root         (0)    36921 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/app_commands.py
+-rw-r--r--   0 root         (0) root         (0)    11361 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/appinfo.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/application_role_connection.py
+-rw-r--r--   0 root         (0) root         (0)    14844 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/asset.py
+-rw-r--r--   0 root         (0) root         (0)    31731 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/audit_logs.py
+-rw-r--r--   0 root         (0) root         (0)    28631 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/automod.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/backoff.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/bans.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.930299 disnake-2.9.0/disnake/bin/
+-rw-r--r--   0 root         (0) root         (0)     1487 2022-07-27 17:57:08.000000 disnake-2.9.0/disnake/bin/COPYING
+-rw-r--r--   0 root         (0) root         (0)   441856 2022-07-27 17:57:08.000000 disnake-2.9.0/disnake/bin/libopus-0.x64.dll
+-rw-r--r--   0 root         (0) root         (0)   366080 2022-07-27 17:57:08.000000 disnake-2.9.0/disnake/bin/libopus-0.x86.dll
+-rw-r--r--   0 root         (0) root         (0)   159210 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/channel.py
+-rw-r--r--   0 root         (0) root         (0)    94112 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/client.py
+-rw-r--r--   0 root         (0) root         (0)     8925 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/colour.py
+-rw-r--r--   0 root         (0) root         (0)    22659 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/components.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/context_managers.py
+-rw-r--r--   0 root         (0) root         (0)      713 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/custom_warnings.py
+-rw-r--r--   0 root         (0) root         (0)    28024 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/embeds.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/emoji.py
+-rw-r--r--   0 root         (0) root         (0)    44336 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/enums.py
+-rw-r--r--   0 root         (0) root         (0)    13422 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.902299 disnake-2.9.0/disnake/ext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.938299 disnake-2.9.0/disnake/ext/commands/
+-rw-r--r--   0 root         (0) root         (0)      615 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/ext/commands/_types.py
+-rw-r--r--   0 root         (0) root         (0)    27590 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/base_core.py
+-rw-r--r--   0 root         (0) root         (0)    21156 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/bot.py
+-rw-r--r--   0 root         (0) root         (0)    20650 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/bot_base.py
+-rw-r--r--   0 root         (0) root         (0)    34441 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/cog.py
+-rw-r--r--   0 root         (0) root         (0)    23084 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/common_bot_base.py
+-rw-r--r--   0 root         (0) root         (0)    13890 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/context.py
+-rw-r--r--   0 root         (0) root         (0)    43768 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/converter.py
+-rw-r--r--   0 root         (0) root         (0)    11885 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/cooldowns.py
+-rw-r--r--   0 root         (0) root         (0)    89205 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/core.py
+-rw-r--r--   0 root         (0) root         (0)    15025 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/ext/commands/ctx_menus_core.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/custom_warnings.py
+-rw-r--r--   0 root         (0) root         (0)    31414 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/errors.py
+-rw-r--r--   0 root         (0) root         (0)    20527 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/flag_converter.py
+-rw-r--r--   0 root         (0) root         (0)     6136 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/ext/commands/flags.py
+-rw-r--r--   0 root         (0) root         (0)    47682 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/help.py
+-rw-r--r--   0 root         (0) root         (0)    54256 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/interaction_bot_base.py
+-rw-r--r--   0 root         (0) root         (0)    50306 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/params.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/ext/commands/py.typed
+-rw-r--r--   0 root         (0) root         (0)    31091 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/slash_core.py
+-rw-r--r--   0 root         (0) root         (0)     5067 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/commands/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.938299 disnake-2.9.0/disnake/ext/mypy_plugin/
+-rw-r--r--   0 root         (0) root         (0)      287 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/mypy_plugin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.942299 disnake-2.9.0/disnake/ext/tasks/
+-rw-r--r--   0 root         (0) root         (0)    26807 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ext/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/ext/tasks/py.typed
+-rw-r--r--   0 root         (0) root         (0)     4284 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/file.py
+-rw-r--r--   0 root         (0) root         (0)    75334 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/flags.py
+-rw-r--r--   0 root         (0) root         (0)    37894 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/gateway.py
+-rw-r--r--   0 root         (0) root         (0)   183827 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/guild.py
+-rw-r--r--   0 root         (0) root         (0)     3973 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/guild_preview.py
+-rw-r--r--   0 root         (0) root         (0)    25609 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/guild_scheduled_event.py
+-rw-r--r--   0 root         (0) root         (0)    90490 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/http.py
+-rw-r--r--   0 root         (0) root         (0)    13069 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/i18n.py
+-rw-r--r--   0 root         (0) root         (0)    12872 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/integrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.942299 disnake-2.9.0/disnake/interactions/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/interactions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12116 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/interactions/application_command.py
+-rw-r--r--   0 root         (0) root         (0)    71563 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/interactions/base.py
+-rw-r--r--   0 root         (0) root         (0)     6752 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/interactions/message.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/interactions/modal.py
+-rw-r--r--   0 root         (0) root         (0)    21666 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/invite.py
+-rw-r--r--   0 root         (0) root         (0)    36098 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/iterators.py
+-rw-r--r--   0 root         (0) root         (0)    40608 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/member.py
+-rw-r--r--   0 root         (0) root         (0)     5671 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/mentions.py
+-rw-r--r--   0 root         (0) root         (0)    92487 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/message.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/mixins.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/object.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/oggparse.py
+-rw-r--r--   0 root         (0) root         (0)     6638 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/onboarding.py
+-rw-r--r--   0 root         (0) root         (0)    14632 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/opus.py
+-rw-r--r--   0 root         (0) root         (0)     7331 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/partial_emoji.py
+-rw-r--r--   0 root         (0) root         (0)    45359 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    26457 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/player.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-27 17:57:08.000000 disnake-2.9.0/disnake/py.typed
+-rw-r--r--   0 root         (0) root         (0)    14483 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/raw_models.py
+-rw-r--r--   0 root         (0) root         (0)     6224 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/reaction.py
+-rw-r--r--   0 root         (0) root         (0)    17974 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/role.py
+-rw-r--r--   0 root         (0) root         (0)    21116 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/shard.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/stage_instance.py
+-rw-r--r--   0 root         (0) root         (0)    90451 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/state.py
+-rw-r--r--   0 root         (0) root         (0)    15314 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/sticker.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/team.py
+-rw-r--r--   0 root         (0) root         (0)     8721 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/template.py
+-rw-r--r--   0 root         (0) root         (0)    40796 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/threads.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.950299 disnake-2.9.0/disnake/types/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/activity.py
+-rw-r--r--   0 root         (0) root         (0)     1326 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/types/appinfo.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/types/application_role_connection.py
+-rw-r--r--   0 root         (0) root         (0)     7371 2023-06-21 16:23:17.000000 disnake-2.9.0/disnake/types/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/types/automod.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/types/channel.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/components.py
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/embed.py
+-rw-r--r--   0 root         (0) root         (0)      471 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/emoji.py
+-rw-r--r--   0 root         (0) root         (0)    15913 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/types/gateway.py
+-rw-r--r--   0 root         (0) root         (0)     5589 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/types/guild.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/guild_scheduled_event.py
+-rw-r--r--   0 root         (0) root         (0)       91 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/types/i18n.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/types/integration.py
+-rw-r--r--   0 root         (0) root         (0)     9536 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/types/interactions.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/invite.py
+-rw-r--r--   0 root         (0) root         (0)      716 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/types/member.py
+-rw-r--r--   0 root         (0) root         (0)     3349 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/types/message.py
+-rw-r--r--   0 root         (0) root         (0)      739 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/types/onboarding.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/types/role.py
+-rw-r--r--   0 root         (0) root         (0)      166 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-21 16:23:17.000000 disnake-2.9.0/disnake/types/sticker.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-06-21 16:23:17.000000 disnake-2.9.0/disnake/types/team.py
+-rw-r--r--   0 root         (0) root         (0)      557 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/template.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/threads.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/types/user.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/voice.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/webhook.py
+-rw-r--r--   0 root         (0) root         (0)      413 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/welcome_screen.py
+-rw-r--r--   0 root         (0) root         (0)      958 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/types/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.950299 disnake-2.9.0/disnake/ui/
+-rw-r--r--   0 root         (0) root         (0)      372 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29552 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/ui/action_row.py
+-rw-r--r--   0 root         (0) root         (0)    11041 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ui/button.py
+-rw-r--r--   0 root         (0) root         (0)     5411 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/ui/item.py
+-rw-r--r--   0 root         (0) root         (0)     8617 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/ui/modal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.954299 disnake-2.9.0/disnake/ui/select/
+-rw-r--r--   0 root         (0) root         (0)      591 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ui/select/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5968 2023-03-02 19:46:40.000000 disnake-2.9.0/disnake/ui/select/base.py
+-rw-r--r--   0 root         (0) root         (0)     7940 2023-03-02 19:46:41.000000 disnake-2.9.0/disnake/ui/select/channel.py
+-rw-r--r--   0 root         (0) root         (0)     6611 2023-03-02 19:46:41.000000 disnake-2.9.0/disnake/ui/select/mentionable.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2023-03-02 19:46:41.000000 disnake-2.9.0/disnake/ui/select/role.py
+-rw-r--r--   0 root         (0) root         (0)    11403 2023-03-02 19:46:41.000000 disnake-2.9.0/disnake/ui/select/string.py
+-rw-r--r--   0 root         (0) root         (0)     6340 2023-03-02 19:46:41.000000 disnake-2.9.0/disnake/ui/select/user.py
+-rw-r--r--   0 root         (0) root         (0)     4599 2023-02-05 21:19:05.000000 disnake-2.9.0/disnake/ui/text_input.py
+-rw-r--r--   0 root         (0) root         (0)    19534 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/ui/view.py
+-rw-r--r--   0 root         (0) root         (0)    15669 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/user.py
+-rw-r--r--   0 root         (0) root         (0)    38599 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/utils.py
+-rw-r--r--   0 root         (0) root         (0)    23601 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/voice_client.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/voice_region.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.954299 disnake-2.9.0/disnake/webhook/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/webhook/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67023 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/webhook/async_.py
+-rw-r--r--   0 root         (0) root         (0)    43233 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/webhook/sync.py
+-rw-r--r--   0 root         (0) root         (0)     5870 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/welcome_screen.py
+-rw-r--r--   0 root         (0) root         (0)    13998 2023-06-21 16:25:59.000000 disnake-2.9.0/disnake/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.930299 disnake-2.9.0/disnake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5039 2023-06-21 16:26:12.000000 disnake-2.9.0/disnake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-06-21 16:26:12.000000 disnake-2.9.0/disnake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:26:12.000000 disnake-2.9.0/disnake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-21 16:26:12.000000 disnake-2.9.0/disnake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-21 16:26:12.000000 disnake-2.9.0/disnake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    10392 2023-06-21 16:25:59.000000 disnake-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 16:26:12.958299 disnake-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1326 2023-06-21 16:25:59.000000 disnake-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 16:26:12.958299 disnake-2.9.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     6429 2023-06-21 16:25:59.000000 disnake-2.9.0/tests/test_abc.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-21 16:25:59.000000 disnake-2.9.0/tests/test_colour.py
+-rw-r--r--   0 root         (0) root         (0)    14013 2023-06-21 16:25:59.000000 disnake-2.9.0/tests/test_embeds.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2023-06-21 16:25:59.000000 disnake-2.9.0/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)    14421 2023-06-21 16:25:59.000000 disnake-2.9.0/tests/test_flags.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-06-21 16:25:59.000000 disnake-2.9.0/tests/test_http.py
+-rw-r--r--   0 root         (0) root         (0)     4004 2023-02-05 21:19:05.000000 disnake-2.9.0/tests/test_mentions.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-06-21 16:25:59.000000 disnake-2.9.0/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-06-21 16:25:59.000000 disnake-2.9.0/tests/test_object.py
+-rw-r--r--   0 root         (0) root         (0)     3061 2023-06-21 16:25:59.000000 disnake-2.9.0/tests/test_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)    10993 2023-06-21 16:25:59.000000 disnake-2.9.0/tests/test_permissions.py
+-rw-r--r--   0 root         (0) root         (0)    25424 2023-06-21 16:25:59.000000 disnake-2.9.0/tests/test_utils.py
```

### Comparing `disnake-2.8.2/LICENSE` & `disnake-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/PKG-INFO` & `disnake-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disnake
-Version: 2.8.2
+Version: 2.9.0
 Summary: A Python wrapper for the Discord API
 Author: Disnake Development
 License: MIT
 Project-URL: Changelog, https://docs.disnake.dev/page/whats_new.html
 Project-URL: Documentation, https://docs.disnake.dev/
 Project-URL: Repository, https://github.com/DisnakeDev/disnake
 Keywords: disnake,discord,discord api
@@ -20,28 +20,28 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: speed
 Provides-Extra: voice
 Provides-Extra: docs
-Provides-Extra: speed
 Provides-Extra: discord
 License-File: LICENSE
 
 <!-- SPDX-License-Identifier: MIT -->
 
 [![Disnake Banner](https://raw.githubusercontent.com/DisnakeDev/disnake/master/assets/banner.png)](https://disnake.dev/)
 
 disnake
 =======
-
 <p align="center">
+    <img src="https://img.shields.io/github/actions/workflow/status/DisnakeDev/disnake/lint-test.yml?branch=master&style=flat-square"></img>
     <a href="https://discord.gg/disnake"><img src="https://img.shields.io/discord/808030843078836254?style=flat-square&color=5865f2&logo=discord&logoColor=ffffff&label=discord" alt="Discord server invite" /></a>
     <a href="https://pypi.org/project/disnake/"><img src="https://img.shields.io/pypi/v/disnake.svg?style=flat-square" alt="PyPI version info" /></a>
     <a href="https://pypi.org/project/disnake/"><img src="https://img.shields.io/pypi/pyversions/disnake.svg?style=flat-square" alt="PyPI supported Python versions" /></a>
     <a href="https://github.com/DisnakeDev/disnake/commits"><img src="https://img.shields.io/github/commit-activity/w/DisnakeDev/disnake.svg?style=flat-square" alt="Commit activity" /></a>
 </p>
 
 A modern, easy to use, feature-rich, and async-ready API wrapper for Discord written in Python.
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: disnake Version: 2.8.2 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: disnake Version: 2.9.0 Summary: A Python wrapper
 for the Discord API Author: Disnake Development License: MIT Project-URL:
 Changelog, https://docs.disnake.dev/page/whats_new.html Project-URL:
 Documentation, https://docs.disnake.dev/ Project-URL: Repository, https://
 github.com/DisnakeDev/disnake Keywords: disnake,discord,discord api Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Topic ::
 Utilities Classifier: Typing :: Typed Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: voice Provides-Extra: docs
-Provides-Extra: speed Provides-Extra: discord License-File: LICENSE  [![Disnake
+Content-Type: text/markdown Provides-Extra: speed Provides-Extra: voice
+Provides-Extra: docs Provides-Extra: discord License-File: LICENSE  [![Disnake
 Banner](https://raw.githubusercontent.com/DisnakeDev/disnake/master/assets/
 banner.png)](https://disnake.dev/) disnake =======
- [Discord_server_invite] [PyPI_version_info] [PyPI_supported_Python_versions]
-                               [Commit_activity]
+[https://img.shields.io/github/actions/workflow/status/DisnakeDev/disnake/lint-
+test.yml?branch=master&style=flat-square] [Discord_server_invite] [PyPI_version
+           info] [PyPI_supported_Python_versions] [Commit_activity]
 A modern, easy to use, feature-rich, and async-ready API wrapper for Discord
 written in Python. Key Features ------------ - Proper rate limit handling. -
 Type-safety measures. - [FastAPI](https://fastapi.tiangolo.com/)-like slash
 command syntax. The syntax and structure of `discord.py 2.0` is preserved.
 Installing ---------- **Python 3.8 or higher is required.** To install the
 library without full voice support, you can just run the following command: ```
 sh # Linux/macOS python3 -m pip install -U disnake # Windows py -3 -m pip
```

### Comparing `disnake-2.8.2/README.md` & `disnake-2.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!-- SPDX-License-Identifier: MIT -->
 
 [![Disnake Banner](https://raw.githubusercontent.com/DisnakeDev/disnake/master/assets/banner.png)](https://disnake.dev/)
 
 disnake
 =======
-
 <p align="center">
+    <img src="https://img.shields.io/github/actions/workflow/status/DisnakeDev/disnake/lint-test.yml?branch=master&style=flat-square"></img>
     <a href="https://discord.gg/disnake"><img src="https://img.shields.io/discord/808030843078836254?style=flat-square&color=5865f2&logo=discord&logoColor=ffffff&label=discord" alt="Discord server invite" /></a>
     <a href="https://pypi.org/project/disnake/"><img src="https://img.shields.io/pypi/v/disnake.svg?style=flat-square" alt="PyPI version info" /></a>
     <a href="https://pypi.org/project/disnake/"><img src="https://img.shields.io/pypi/pyversions/disnake.svg?style=flat-square" alt="PyPI supported Python versions" /></a>
     <a href="https://github.com/DisnakeDev/disnake/commits"><img src="https://img.shields.io/github/commit-activity/w/DisnakeDev/disnake.svg?style=flat-square" alt="Commit activity" /></a>
 </p>
 
 A modern, easy to use, feature-rich, and async-ready API wrapper for Discord written in Python.
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
  [![Disnake Banner](https://raw.githubusercontent.com/DisnakeDev/disnake/
 master/assets/banner.png)](https://disnake.dev/) disnake =======
- [Discord_server_invite] [PyPI_version_info] [PyPI_supported_Python_versions]
-                               [Commit_activity]
+[https://img.shields.io/github/actions/workflow/status/DisnakeDev/disnake/lint-
+test.yml?branch=master&style=flat-square] [Discord_server_invite] [PyPI_version
+           info] [PyPI_supported_Python_versions] [Commit_activity]
 A modern, easy to use, feature-rich, and async-ready API wrapper for Discord
 written in Python. Key Features ------------ - Proper rate limit handling. -
 Type-safety measures. - [FastAPI](https://fastapi.tiangolo.com/)-like slash
 command syntax. The syntax and structure of `discord.py 2.0` is preserved.
 Installing ---------- **Python 3.8 or higher is required.** To install the
 library without full voice support, you can just run the following command: ```
 sh # Linux/macOS python3 -m pip install -U disnake # Windows py -3 -m pip
```

### Comparing `disnake-2.8.2/disnake/__init__.py` & `disnake-2.9.0/disnake/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # SPDX-License-Identifier: MIT
 
-"""
-Discord API Wrapper
+"""Discord API Wrapper
 ~~~~~~~~~~~~~~~~~~~
 
 A basic wrapper for the Discord API.
 
 :copyright: (c) 2015-2021 Rapptz, 2021-present Disnake Development
 :license: MIT, see LICENSE for more details.
 
 """
 
 __title__ = "disnake"
 __author__ = "Rapptz, EQUENOS"
 __license__ = "MIT"
 __copyright__ = "Copyright 2015-present Rapptz, 2021-present EQUENOS"
-__version__ = "2.8.2"
+__version__ = "2.9.0"
 
 __path__ = __import__("pkgutil").extend_path(__path__, __name__)
 
 import logging
 from typing import Literal, NamedTuple
 
 from . import abc as abc, opus as opus, ui as ui, utils as utils  # explicitly re-export modules
@@ -49,14 +48,15 @@
 from .integrations import *
 from .interactions import *
 from .invite import *
 from .member import *
 from .mentions import *
 from .message import *
 from .object import *
+from .onboarding import *
 from .partial_emoji import *
 from .permissions import *
 from .player import *
 from .raw_models import *
 from .reaction import *
 from .role import *
 from .shard import *
@@ -77,10 +77,10 @@
     major: int
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=2, minor=8, micro=2, releaselevel="final", serial=0)
+version_info: VersionInfo = VersionInfo(major=2, minor=9, micro=0, releaselevel="final", serial=0)
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `disnake-2.8.2/disnake/__main__.py` & `disnake-2.9.0/disnake/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-License-Identifier: MIT
 
 import argparse
 import importlib.metadata
 import platform
 import sys
 from pathlib import Path
+from typing import Union
 
 import aiohttp
 
 import disnake
 
 
 def show_version() -> None:
@@ -159,15 +160,15 @@
 # NUL (0) and 1-31 are disallowed
 _byte_table = dict.fromkeys(map(chr, range(32)))
 _base_table = {**_ascii_table, **_byte_table}
 
 _translation_table = str.maketrans(_base_table)
 
 
-def to_path(parser, name, *, replace_spaces=False):
+def to_path(parser, name: Union[str, Path], *, replace_spaces: bool = False):
     if isinstance(name, Path):
         return name
 
     if sys.platform == "win32":
         forbidden = (
             "CON",
             "PRN",
```

### Comparing `disnake-2.8.2/disnake/abc.py` & `disnake-2.9.0/disnake/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     try_enum_to_int,
 )
 from .errors import ClientException
 from .file import File
 from .flags import ChannelFlags, MessageFlags
 from .invite import Invite
 from .mentions import AllowedMentions
+from .object import Object
 from .partial_emoji import PartialEmoji
 from .permissions import PermissionOverwrite, Permissions
 from .role import Role
 from .sticker import GuildSticker, StickerItem
 from .ui.action_row import components_to_dict
 from .utils import _overload_with_permissions
 from .voice_client import VoiceClient, VoiceProtocol
@@ -94,15 +95,15 @@
 MISSING = utils.MISSING
 
 
 @runtime_checkable
 class Snowflake(Protocol):
     """An ABC that details the common operations on a Discord model.
 
-    Almost all :ref:`Discord models <discord_api_models>` meet this
+    Almost all :ref:`Discord models <discord_model>` meet this
     abstract base class.
 
     If you want to create a snowflake on your own, consider using
     :class:`.Object`.
 
     Attributes
     ----------
@@ -128,37 +129,55 @@
 
     Attributes
     ----------
     name: :class:`str`
         The user's username.
     discriminator: :class:`str`
         The user's discriminator.
-    avatar: :class:`~disnake.Asset`
-        The avatar asset the user has.
+
+        .. note::
+            This is being phased out by Discord; the username system is moving away from ``username#discriminator``
+            to users having a globally unique username.
+            The value of a single zero (``"0"``) indicates that the user has been migrated to the new system.
+            See the `help article <https://dis.gd/app-usernames>`__ for details.
+
+    global_name: Optional[:class:`str`]
+        The user's global display name, if set.
+        This takes precedence over :attr:`.name` when shown.
+
+        .. versionadded:: 2.9
+
     bot: :class:`bool`
         Whether the user is a bot account.
     """
 
     __slots__ = ()
 
     name: str
     discriminator: str
-    avatar: Asset
+    global_name: Optional[str]
     bot: bool
 
     @property
     def display_name(self) -> str:
         """:class:`str`: Returns the user's display name."""
         raise NotImplementedError
 
     @property
     def mention(self) -> str:
         """:class:`str`: Returns a string that allows you to mention the given user."""
         raise NotImplementedError
 
+    @property
+    def avatar(self) -> Optional[Asset]:
+        """Optional[:class:`~disnake.Asset`]: Returns an :class:`~disnake.Asset` for
+        the avatar the user has.
+        """
+        raise NotImplementedError
+
 
 @runtime_checkable
 class PrivateChannel(Snowflake, Protocol):
     """An ABC that details the common operations on a private Discord channel.
 
     The following classes implement this ABC:
 
@@ -479,15 +498,16 @@
         tmp = self._overwrites
         if tmp:
             tmp[everyone_index], tmp[0] = tmp[0], tmp[everyone_index]
 
     @property
     def changed_roles(self) -> List[Role]:
         """List[:class:`.Role`]: Returns a list of roles that have been overridden from
-        their default values in the :attr:`.Guild.roles` attribute."""
+        their default values in the :attr:`.Guild.roles` attribute.
+        """
         ret = []
         g = self.guild
         for overwrite in filter(lambda o: o.is_role(), self._overwrites):
             role = g.get_role(overwrite.id)
             if role is None:
                 continue
 
@@ -599,25 +619,39 @@
 
         .. versionadded:: 2.6
         """
         return ChannelFlags._from_value(self._flags)
 
     @property
     def jump_url(self) -> str:
-        """
-        A URL that can be used to jump to this channel.
+        """A URL that can be used to jump to this channel.
 
         .. versionadded:: 2.4
 
         .. note::
 
             This exists for all guild channels but may not be usable by the client for all guild channel types.
         """
         return f"https://discord.com/channels/{self.guild.id}/{self.id}"
 
+    def _apply_implict_permissions(self, base: Permissions) -> None:
+        # if you can't send a message in a channel then you can't have certain
+        # permissions as well
+        if not base.send_messages:
+            base.send_tts_messages = False
+            base.send_voice_messages = False
+            base.mention_everyone = False
+            base.embed_links = False
+            base.attach_files = False
+
+        # if you can't view a channel then you have no permissions there
+        if not base.view_channel:
+            denied = Permissions.all_channel()
+            base.value &= ~denied.value
+
     def permissions_for(
         self,
         obj: Union[Member, Role],
         /,
         *,
         ignore_timeout: bool = MISSING,
     ) -> Permissions:
@@ -761,32 +795,19 @@
 
         # Apply member specific permission overwrites
         for overwrite in remaining_overwrites:
             if overwrite.is_member() and overwrite.id == obj.id:
                 base.handle_overwrite(allow=overwrite.allow, deny=overwrite.deny)
                 break
 
-        # if you can't send a message in a channel then you can't have certain
-        # permissions as well
-        if not base.send_messages:
-            base.send_tts_messages = False
-            base.mention_everyone = False
-            base.embed_links = False
-            base.attach_files = False
-
-        # if you can't view a channel then you have no permissions there
-        if not base.view_channel:
-            denied = Permissions.all_channel()
-            base.value &= ~denied.value
-
         # if you have a timeout then you can't have any permissions
         # except read messages and read message history
         if not ignore_timeout and obj.current_timeout:
-            denied = Permissions(view_channel=True, read_message_history=True)
-            base.value &= denied.value
+            allowed = Permissions(view_channel=True, read_message_history=True)
+            base.value &= allowed.value
 
         return base
 
     async def delete(self, *, reason: Optional[str] = None) -> None:
         """|coro|
 
         Deletes the channel.
@@ -842,14 +863,15 @@
         external_stickers: Optional[bool] = ...,
         kick_members: Optional[bool] = ...,
         manage_channels: Optional[bool] = ...,
         manage_emojis: Optional[bool] = ...,
         manage_emojis_and_stickers: Optional[bool] = ...,
         manage_events: Optional[bool] = ...,
         manage_guild: Optional[bool] = ...,
+        manage_guild_expressions: Optional[bool] = ...,
         manage_messages: Optional[bool] = ...,
         manage_nicknames: Optional[bool] = ...,
         manage_permissions: Optional[bool] = ...,
         manage_roles: Optional[bool] = ...,
         manage_threads: Optional[bool] = ...,
         manage_webhooks: Optional[bool] = ...,
         mention_everyone: Optional[bool] = ...,
@@ -859,34 +881,42 @@
         priority_speaker: Optional[bool] = ...,
         read_message_history: Optional[bool] = ...,
         read_messages: Optional[bool] = ...,
         request_to_speak: Optional[bool] = ...,
         send_messages: Optional[bool] = ...,
         send_messages_in_threads: Optional[bool] = ...,
         send_tts_messages: Optional[bool] = ...,
+        send_voice_messages: Optional[bool] = ...,
         speak: Optional[bool] = ...,
         start_embedded_activities: Optional[bool] = ...,
         stream: Optional[bool] = ...,
         use_application_commands: Optional[bool] = ...,
         use_embedded_activities: Optional[bool] = ...,
         use_external_emojis: Optional[bool] = ...,
+        use_external_sounds: Optional[bool] = ...,
         use_external_stickers: Optional[bool] = ...,
         use_slash_commands: Optional[bool] = ...,
+        use_soundboard: Optional[bool] = ...,
         use_voice_activation: Optional[bool] = ...,
         view_audit_log: Optional[bool] = ...,
         view_channel: Optional[bool] = ...,
+        view_creator_monetization_analytics: Optional[bool] = ...,
         view_guild_insights: Optional[bool] = ...,
     ) -> None:
         ...
 
     async def set_permissions(
-        self, target, *, overwrite=MISSING, reason=None, **permissions
+        self,
+        target,
+        *,
+        overwrite: Optional[PermissionOverwrite] = MISSING,
+        reason: Optional[str] = None,
+        **permissions,
     ) -> None:
-        """
-        |coro|
+        """|coro|
 
         Sets the channel specific permission overwrites for a target in the
         channel.
 
         The ``target`` parameter should either be a :class:`.Member` or a
         :class:`.Role` that belongs to guild.
 
@@ -906,15 +936,14 @@
             This method *replaces* the old overwrites with the ones given.
 
         .. versionchanged:: 2.6
             Raises :exc:`TypeError` instead of ``InvalidArgument``.
 
         Examples
         --------
-
         Setting allow and deny: ::
 
             await message.channel.set_permissions(message.author, view_channel=True,
                                                                   send_messages=False)
 
         Deleting overwrites ::
 
@@ -964,16 +993,16 @@
             raise TypeError("target parameter must be either Member or Role")
 
         if overwrite is MISSING:
             if len(permissions) == 0:
                 raise TypeError("No overwrite provided.")
             try:
                 overwrite = PermissionOverwrite(**permissions)
-            except (ValueError, TypeError):
-                raise TypeError("Invalid permissions given to keyword arguments.")
+            except (ValueError, TypeError) as e:
+                raise TypeError("Invalid permissions given to keyword arguments.") from e
         else:
             if len(permissions) > 0:
                 raise TypeError("Cannot mix overwrite and keyword arguments.")
 
         # TODO: wait for event
 
         if overwrite is None:
@@ -987,23 +1016,54 @@
             raise TypeError("Invalid overwrite type provided.")
 
     async def _clone_impl(
         self,
         base_attrs: Dict[str, Any],
         *,
         name: Optional[str] = None,
+        category: Optional[Snowflake] = MISSING,
+        overwrites: Mapping[Union[Role, Member], PermissionOverwrite] = MISSING,
         reason: Optional[str] = None,
     ) -> Self:
-        base_attrs["permission_overwrites"] = [x._asdict() for x in self._overwrites]
-        base_attrs["parent_id"] = self.category_id
+        # if the overwrites are MISSING, defaults to the
+        # original permissions of the channel
+        overwrites_payload: List[PermissionOverwritePayload]
+        if overwrites is not MISSING:
+            if not isinstance(overwrites, dict):
+                raise TypeError("overwrites parameter expects a dict.")
+
+            overwrites_payload = []
+            for target, perm in overwrites.items():
+                if not isinstance(perm, PermissionOverwrite):
+                    raise TypeError(
+                        f"Expected PermissionOverwrite, received {perm.__class__.__name__}"
+                    )
+
+                allow, deny = perm.pair()
+                payload: PermissionOverwritePayload = {
+                    "allow": str(allow.value),
+                    "deny": str(deny.value),
+                    "id": target.id,
+                    "type": (_Overwrites.ROLE if isinstance(target, Role) else _Overwrites.MEMBER),
+                }
+                overwrites_payload.append(payload)
+        else:
+            overwrites_payload = [x._asdict() for x in self._overwrites]
+        base_attrs["permission_overwrites"] = overwrites_payload
+        if category is not MISSING:
+            base_attrs["parent_id"] = category.id if category else None
+        else:
+            # if no category was given don't change the category
+            base_attrs["parent_id"] = self.category_id
         base_attrs["name"] = name or self.name
+        channel_type = base_attrs.get("type") or self.type.value
         guild_id = self.guild.id
         cls = self.__class__
         data = await self._state.http.create_channel(
-            guild_id, self.type.value, reason=reason, **base_attrs
+            guild_id, channel_type, reason=reason, **base_attrs
         )
         obj = cls(state=self._state, guild=self.guild, data=data)
 
         # temporarily add it to the cache
         self.guild._channels[obj.id] = obj  # type: ignore
         return obj
 
@@ -1216,29 +1276,35 @@
         reason: Optional[str] = None,
         max_age: int = 0,
         max_uses: int = 0,
         temporary: bool = False,
         unique: bool = True,
         target_type: Optional[InviteTarget] = None,
         target_user: Optional[User] = None,
-        target_application: Optional[PartyType] = None,
+        target_application: Optional[Union[Snowflake, PartyType]] = None,
         guild_scheduled_event: Optional[GuildScheduledEvent] = None,
     ) -> Invite:
         """|coro|
 
         Creates an instant invite from a text or voice channel.
 
         You must have :attr:`.Permissions.create_instant_invite` permission to
         do this.
 
         Parameters
         ----------
         max_age: :class:`int`
-            How long the invite should last in seconds. If it's 0 then the invite
+            How long the invite should last in seconds. If set to ``0``, then the invite
             doesn't expire. Defaults to ``0``.
+
+            .. warning::
+
+                If the guild is not a Community guild (has ``COMMUNITY`` in :attr:`.Guild.features`),
+                this must be set to a number between ``1`` and ``2592000`` seconds.
+
         max_uses: :class:`int`
             How many uses the invite could be used for. If it's 0 then there
             are unlimited uses. Defaults to ``0``.
         temporary: :class:`bool`
             Whether the invite grants temporary membership
             (i.e. they get kicked after they disconnect). Defaults to ``False``.
         unique: :class:`bool`
@@ -1247,24 +1313,27 @@
             invite.
         target_type: Optional[:class:`.InviteTarget`]
             The type of target for the voice channel invite, if any.
 
             .. versionadded:: 2.0
 
         target_user: Optional[:class:`User`]
-            The user whose stream to display for this invite, required if `target_type` is `TargetType.stream`.
+            The user whose stream to display for this invite, required if ``target_type`` is :attr:`.InviteTarget.stream`.
             The user must be streaming in the channel.
 
             .. versionadded:: 2.0
 
-        target_application: Optional[:class:`.PartyType`]
-            The ID of the embedded application for the invite, required if `target_type` is `TargetType.embedded_application`.
+        target_application: Optional[:class:`.Snowflake`]
+            The ID of the embedded application for the invite, required if ``target_type`` is :attr:`.InviteTarget.embedded_application`.
 
             .. versionadded:: 2.0
 
+            .. versionchanged:: 2.9
+                ``PartyType`` is deprecated, and :class:`.Snowflake` should be used instead.
+
         guild_scheduled_event: Optional[:class:`.GuildScheduledEvent`]
             The guild scheduled event to include with the invite.
 
             .. versionadded:: 2.3
 
         reason: Optional[:class:`str`]
             The reason for creating this invite. Shows up on the audit log.
@@ -1277,24 +1346,30 @@
             The channel that was passed is a category or an invalid channel.
 
         Returns
         -------
         :class:`.Invite`
             The newly created invite.
         """
+        if isinstance(target_application, PartyType):
+            utils.warn_deprecated(
+                "PartyType is deprecated and will be removed in future version",
+                stacklevel=2,
+            )
+            target_application = Object(target_application.value)
         data = await self._state.http.create_invite(
             self.id,
             reason=reason,
             max_age=max_age,
             max_uses=max_uses,
             temporary=temporary,
             unique=unique,
             target_type=try_enum_to_int(target_type),
             target_user_id=target_user.id if target_user else None,
-            target_application_id=try_enum_to_int(target_application),
+            target_application_id=target_application.id if target_application else None,
         )
         invite = Invite.from_incomplete(data=data, state=self._state)
         invite.guild_scheduled_event = guild_scheduled_event
         return invite
 
     async def invites(self) -> List[Invite]:
         """|coro|
@@ -1327,17 +1402,18 @@
     The following classes implement this ABC:
 
     - :class:`~disnake.TextChannel`
     - :class:`~disnake.DMChannel`
     - :class:`~disnake.GroupChannel`
     - :class:`~disnake.User`
     - :class:`~disnake.Member`
-    - :class:`~disnake.ext.commands.Context`
     - :class:`~disnake.Thread`
     - :class:`~disnake.VoiceChannel`
+    - :class:`~disnake.StageChannel`
+    - :class:`~disnake.ext.commands.Context`
     - :class:`~disnake.PartialMessageable`
     """
 
     __slots__ = ()
     _state: ConnectionState
 
     async def _get_channel(self) -> MessageableChannel:
@@ -1351,14 +1427,15 @@
         tts: bool = ...,
         embed: Embed = ...,
         file: File = ...,
         stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
         delete_after: float = ...,
         nonce: Union[str, int] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: AllowedMentions = ...,
         reference: Union[Message, MessageReference, PartialMessage] = ...,
         mention_author: bool = ...,
         view: View = ...,
         components: Components[MessageUIComponent] = ...,
     ) -> Message:
         ...
@@ -1371,14 +1448,15 @@
         tts: bool = ...,
         embed: Embed = ...,
         files: List[File] = ...,
         stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
         delete_after: float = ...,
         nonce: Union[str, int] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: AllowedMentions = ...,
         reference: Union[Message, MessageReference, PartialMessage] = ...,
         mention_author: bool = ...,
         view: View = ...,
         components: Components[MessageUIComponent] = ...,
     ) -> Message:
         ...
@@ -1391,14 +1469,15 @@
         tts: bool = ...,
         embeds: List[Embed] = ...,
         file: File = ...,
         stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
         delete_after: float = ...,
         nonce: Union[str, int] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: AllowedMentions = ...,
         reference: Union[Message, MessageReference, PartialMessage] = ...,
         mention_author: bool = ...,
         view: View = ...,
         components: Components[MessageUIComponent] = ...,
     ) -> Message:
         ...
@@ -1411,14 +1490,15 @@
         tts: bool = ...,
         embeds: List[Embed] = ...,
         files: List[File] = ...,
         stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
         delete_after: float = ...,
         nonce: Union[str, int] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: AllowedMentions = ...,
         reference: Union[Message, MessageReference, PartialMessage] = ...,
         mention_author: bool = ...,
         view: View = ...,
         components: Components[MessageUIComponent] = ...,
     ) -> Message:
         ...
@@ -1431,15 +1511,16 @@
         embed: Optional[Embed] = None,
         embeds: Optional[List[Embed]] = None,
         file: Optional[File] = None,
         files: Optional[List[File]] = None,
         stickers: Optional[Sequence[Union[GuildSticker, StickerItem]]] = None,
         delete_after: Optional[float] = None,
         nonce: Optional[Union[str, int]] = None,
-        suppress_embeds: bool = False,
+        suppress_embeds: Optional[bool] = None,
+        flags: Optional[MessageFlags] = None,
         allowed_mentions: Optional[AllowedMentions] = None,
         reference: Optional[Union[Message, MessageReference, PartialMessage]] = None,
         mention_author: Optional[bool] = None,
         view: Optional[View] = None,
         components: Optional[Components[MessageUIComponent]] = None,
     ):
         """|coro|
@@ -1531,14 +1612,24 @@
 
         suppress_embeds: :class:`bool`
             Whether to suppress embeds for the message. This hides
             all the embeds from the UI if set to ``True``.
 
             .. versionadded:: 2.5
 
+        flags: :class:`.MessageFlags`
+            The flags to set for this message.
+            Only :attr:`~.MessageFlags.suppress_embeds` and :attr:`~.MessageFlags.suppress_notifications`
+            are supported.
+
+            If parameter ``suppress_embeds`` is provided,
+            that will override the setting of :attr:`.MessageFlags.suppress_embeds`.
+
+            .. versionadded:: 2.9
+
         Raises
         ------
         HTTPException
             Sending the message failed.
         Forbidden
             You do not have the proper permissions to send the message.
         TypeError
@@ -1619,18 +1710,20 @@
 
         elif components:
             components_payload = components_to_dict(components)
 
         else:
             components_payload = None
 
-        if suppress_embeds:
-            flags = MessageFlags.suppress_embeds.flag
-        else:
-            flags = 0
+        flags_payload = None
+        if suppress_embeds is not None:
+            flags = MessageFlags._from_value(0 if flags is None else flags.value)
+            flags.suppress_embeds = suppress_embeds
+        if flags is not None:
+            flags_payload = flags.value
 
         if files is not None:
             if len(files) > 10:
                 raise ValueError("files parameter must be a list of up to 10 elements")
             elif not all(isinstance(file, File) for file in files):
                 raise TypeError("files parameter must be a list of File")
 
@@ -1642,15 +1735,15 @@
                     tts=tts,
                     embeds=embeds_payload,
                     nonce=nonce,
                     allowed_mentions=allowed_mentions_payload,
                     message_reference=reference_payload,
                     stickers=stickers_payload,
                     components=components_payload,
-                    flags=flags,
+                    flags=flags_payload,
                 )
             finally:
                 for f in files:
                     f.close()
         else:
             data = await state.http.send_message(
                 channel.id,
@@ -1658,15 +1751,15 @@
                 tts=tts,
                 embeds=embeds_payload,
                 nonce=nonce,
                 allowed_mentions=allowed_mentions_payload,
                 message_reference=reference_payload,
                 stickers=stickers_payload,
                 components=components_payload,
-                flags=flags,
+                flags=flags_payload,
             )
 
         ret = state.create_message(channel=channel, data=data)
         if view:
             state.store_view(view, ret.id)
 
         if delete_after is not None:
@@ -1769,15 +1862,14 @@
     ) -> HistoryIterator:
         """Returns an :class:`.AsyncIterator` that enables receiving the destination's message history.
 
         You must have :attr:`.Permissions.read_message_history` permission to use this.
 
         Examples
         --------
-
         Usage ::
 
             counter = 0
             async for message in channel.history(limit=200):
                 if message.author == client.user:
                     counter += 1
 
@@ -1816,15 +1908,15 @@
         ------
         Forbidden
             You do not have permissions to get channel message history.
         HTTPException
             The request to get message history failed.
 
         Yields
-        -------
+        ------
         :class:`.Message`
             The message with the message data parsed.
         """
         from .iterators import HistoryIterator  # cyclic import
 
         return HistoryIterator(
             self, limit=limit, before=before, after=after, around=around, oldest_first=oldest_first
```

### Comparing `disnake-2.8.2/disnake/activity.py` & `disnake-2.9.0/disnake/activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,14 +135,15 @@
     def to_dict(self) -> ActivityPayload:
         raise NotImplementedError
 
 
 # tag type for user-settable activities
 class BaseActivity(_BaseActivity):
     """The base activity that all user-settable activities inherit from.
+
     A user-settable activity is one that can be used in :meth:`Client.change_presence`.
 
     The following types currently count as user-settable:
 
     - :class:`Activity`
     - :class:`Game`
     - :class:`Streaming`
@@ -606,22 +607,24 @@
         """
         return ActivityType.listening
 
     @property
     def colour(self) -> Colour:
         """:class:`Colour`: Returns the Spotify integration colour, as a :class:`Colour`.
 
-        There is an alias for this named :attr:`color`"""
+        There is an alias for this named :attr:`color`
+        """
         return Colour(0x1DB954)
 
     @property
     def color(self) -> Colour:
         """:class:`Colour`: Returns the Spotify integration colour, as a :class:`Colour`.
 
-        There is an alias for this named :attr:`colour`"""
+        There is an alias for this named :attr:`colour`
+        """
         return self.colour
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "flags": 48,  # SYNC | PLAY
             "name": "Spotify",
             "assets": self.assets,
```

### Comparing `disnake-2.8.2/disnake/app_commands.py` & `disnake-2.9.0/disnake/app_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,15 +360,16 @@
         autocomplete: bool = False,
         min_value: Optional[float] = None,
         max_value: Optional[float] = None,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
     ) -> None:
         """Adds an option to the current list of options,
-        parameters are the same as for :class:`Option`."""
+        parameters are the same as for :class:`Option`.
+        """
         type = type or OptionType.string
         self.options.append(
             Option(
                 name=name,
                 description=description,
                 type=type,
                 required=required,
@@ -424,16 +425,15 @@
         for c in self.choices:
             c.localize(store)
         for o in self.options:
             o.localize(store)
 
 
 class ApplicationCommand(ABC):
-    """
-    The base class for application commands.
+    """The base class for application commands.
 
     The following classes implement this ABC:
 
     - :class:`~.SlashCommand`
     - :class:`~.MessageCommand`
     - :class:`~.UserCommand`
 
@@ -576,16 +576,15 @@
         self.guild_id: Optional[int] = _get_as_snowflake(data, "guild_id")
         self.version: int = int(data["version"])
         # deprecated, but kept until API stops returning this field
         self._default_permission = data.get("default_permission") is not False
 
 
 class UserCommand(ApplicationCommand):
-    """
-    A user context menu command.
+    """A user context menu command.
 
     Attributes
     ----------
     name: :class:`str`
         The user command's name.
     name_localizations: :class:`.LocalizationValue`
         Localizations for ``name``.
@@ -620,16 +619,15 @@
             dm_permission=dm_permission,
             default_member_permissions=default_member_permissions,
             nsfw=nsfw,
         )
 
 
 class APIUserCommand(UserCommand, _APIApplicationCommandMixin):
-    """
-    A user context menu command returned by the API.
+    """A user context menu command returned by the API.
 
     .. versionadded:: 2.4
 
     Attributes
     ----------
     name: :class:`str`
         The user command's name.
@@ -673,16 +671,15 @@
             nsfw=data.get("nsfw"),
         )
         self._update_common(data)
         return self
 
 
 class MessageCommand(ApplicationCommand):
-    """
-    A message context menu command
+    """A message context menu command
 
     Attributes
     ----------
     name: :class:`str`
         The message command's name.
     name_localizations: :class:`.LocalizationValue`
         Localizations for ``name``.
@@ -717,16 +714,15 @@
             dm_permission=dm_permission,
             default_member_permissions=default_member_permissions,
             nsfw=nsfw,
         )
 
 
 class APIMessageCommand(MessageCommand, _APIApplicationCommandMixin):
-    """
-    A message context menu command returned by the API.
+    """A message context menu command returned by the API.
 
     .. versionadded:: 2.4
 
     Attributes
     ----------
     name: :class:`str`
         The message command's name.
@@ -770,16 +766,15 @@
             nsfw=data.get("nsfw"),
         )
         self._update_common(data)
         return self
 
 
 class SlashCommand(ApplicationCommand):
-    """
-    The base class for building slash commands.
+    """The base class for building slash commands.
 
     Attributes
     ----------
     name: :class:`str`
         The slash command's name.
     name_localizations: :class:`.LocalizationValue`
         Localizations for ``name``.
@@ -901,16 +896,15 @@
         self.description_localizations._link(store)
 
         for o in self.options:
             o.localize(store)
 
 
 class APISlashCommand(SlashCommand, _APIApplicationCommandMixin):
-    """
-    A slash command returned by the API.
+    """A slash command returned by the API.
 
     .. versionadded:: 2.4
 
     Attributes
     ----------
     name: :class:`str`
         The slash command's name.
```

### Comparing `disnake-2.8.2/disnake/appinfo.py` & `disnake-2.9.0/disnake/appinfo.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/application_role_connection.py` & `disnake-2.9.0/disnake/application_role_connection.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/asset.py` & `disnake-2.9.0/disnake/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
         .. versionadded:: 2.5
 
         .. versionchanged:: 2.6
             Raises :exc:`TypeError` instead of ``InvalidArgument``.
 
         Parameters
-        -----------
+        ----------
         spoiler: :class:`bool`
             Whether the file is a spoiler.
         filename: Optional[:class:`str`]
             The filename to display when uploading to Discord. If this is not given, it defaults to
             the name of the asset's URL.
         description: Optional[:class:`str`]
             The file's description.
```

### Comparing `disnake-2.8.2/disnake/audit_logs.py` & `disnake-2.9.0/disnake/audit_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,16 +279,17 @@
 
 
 def _transform_default_reaction(
     entry: AuditLogEntry, data: Optional[DefaultReactionPayload]
 ) -> Optional[Union[Emoji, PartialEmoji]]:
     if data is None:
         return None
-    return PartialEmoji._emoji_from_name_id(
-        data.get("emoji_name"), utils._get_as_snowflake(data, "emoji_id"), state=entry._state
+    return entry._state._get_emoji_from_fields(
+        name=data.get("emoji_name"),
+        id=utils._get_as_snowflake(data, "emoji_id"),
     )
 
 
 class AuditLogDiff:
     def __len__(self) -> int:
         return len(self.__dict__)
 
@@ -479,40 +480,39 @@
 
 class _AuditLogProxyMemberPrune:
     delete_member_days: int
     members_removed: int
 
 
 class _AuditLogProxyMemberMoveOrMessageDelete:
-    channel: abc.GuildChannel
+    channel: Union[abc.GuildChannel, Thread]
     count: int
 
 
 class _AuditLogProxyMemberDisconnect:
     count: int
 
 
 class _AuditLogProxyPinAction:
-    channel: abc.GuildChannel
+    channel: Union[abc.GuildChannel, Thread]
     message_id: int
 
 
 class _AuditLogProxyStageInstanceAction:
     channel: abc.GuildChannel
 
 
-class _AuditLogProxyAutoModBlockMessage:
-    channel: abc.GuildChannel
+class _AuditLogProxyAutoModAction:
+    channel: Optional[Union[abc.GuildChannel, Thread]]
     rule_name: str
     rule_trigger_type: enums.AutoModTriggerType
 
 
 class AuditLogEntry(Hashable):
-    """
-    Represents an Audit Log entry.
+    """Represents an Audit Log entry.
 
     You retrieve these via :meth:`Guild.audit_logs`.
 
     .. container:: operations
 
         .. describe:: x == y
 
@@ -586,36 +586,42 @@
         # this key is technically not usually present
         self.reason = data.get("reason")
         self.extra = extra = data.get("options")
 
         if isinstance(self.action, enums.AuditLogAction) and extra:
             if self.action is enums.AuditLogAction.member_prune:
                 # member prune has two keys with useful information
-                self.extra = type(
-                    "_AuditLogProxy", (), {k: int(v) for k, v in extra.items()}  # type: ignore
-                )()
+                elems = {
+                    "delete_member_days": utils._get_as_snowflake(extra, "delete_member_days"),
+                    "members_removed": utils._get_as_snowflake(extra, "members_removed"),
+                }
+                self.extra = type("_AuditLogProxy", (), elems)()
             elif (
                 self.action is enums.AuditLogAction.member_move
                 or self.action is enums.AuditLogAction.message_delete
             ):
                 elems = {
                     "count": int(extra["count"]),
-                    "channel": self._get_channel(utils._get_as_snowflake(extra, "channel_id")),
+                    "channel": self._get_channel_or_thread(
+                        utils._get_as_snowflake(extra, "channel_id")
+                    ),
                 }
                 self.extra = type("_AuditLogProxy", (), elems)()
             elif self.action is enums.AuditLogAction.member_disconnect:
                 # The member disconnect action has a dict with some information
                 elems = {
                     "count": int(extra["count"]),
                 }
                 self.extra = type("_AuditLogProxy", (), elems)()
             elif self.action.name.endswith("pin"):
                 # the pin actions have a dict with some information
                 elems = {
-                    "channel": self._get_channel(utils._get_as_snowflake(extra, "channel_id")),
+                    "channel": self._get_channel_or_thread(
+                        utils._get_as_snowflake(extra, "channel_id")
+                    ),
                     "message_id": int(extra["message_id"]),
                 }
                 self.extra = type("_AuditLogProxy", (), elems)()
             elif self.action.name.startswith("overwrite_"):
                 # the overwrite_ actions have a dict with some information
                 instance_id = int(extra["id"])
                 the_type = extra.get("type")
@@ -625,30 +631,34 @@
                     role = self.guild.get_role(instance_id)
                     if role is None:
                         role = Object(id=instance_id)
                         role.name = extra.get("role_name")  # type: ignore
                     self.extra = role
             elif self.action.name.startswith("stage_instance"):
                 elems = {
-                    "channel": self._get_channel(utils._get_as_snowflake(extra, "channel_id")),
+                    "channel": self._get_channel_or_thread(
+                        utils._get_as_snowflake(extra, "channel_id")
+                    )
                 }
                 self.extra = type("_AuditLogProxy", (), elems)()
             elif self.action is enums.AuditLogAction.application_command_permission_update:
                 app_id = int(extra["application_id"])
                 elems = {
                     "integration": self._get_integration_by_application_id(app_id) or Object(app_id)
                 }
                 self.extra = type("_AuditLogProxy", (), elems)()
             elif self.action in (
                 enums.AuditLogAction.automod_block_message,
                 enums.AuditLogAction.automod_send_alert_message,
                 enums.AuditLogAction.automod_timeout,
             ):
                 elems = {
-                    "channel": (self._get_channel(utils._get_as_snowflake(extra, "channel_id"))),
+                    "channel": (
+                        self._get_channel_or_thread(utils._get_as_snowflake(extra, "channel_id"))
+                    ),
                     "rule_name": extra["auto_moderation_rule_name"],
                     "rule_trigger_type": enums.try_enum(
                         enums.AutoModTriggerType,
                         int(extra["auto_moderation_rule_trigger_type"]),
                     ),
                 }
                 self.extra = type("_AuditLogProxy", (), elems)()
@@ -657,15 +667,15 @@
         # actually this but there's no reason to annoy users with this:
         # Union[
         #     _AuditLogProxyMemberPrune,
         #     _AuditLogProxyMemberMoveOrMessageDelete,
         #     _AuditLogProxyMemberDisconnect,
         #     _AuditLogProxyPinAction,
         #     _AuditLogProxyStageInstanceAction,
-        #     _AuditLogProxyAutoModBlockMessage,
+        #     _AuditLogProxyAutoModAction,
         #     Member, User, None,
         #     Role,
         # ]
 
         # this key is not present when the above is present, typically.
         # It's a list of { new_value: a, old_value: b, key: c }
         # where new_value and old_value are not guaranteed to be there depending
@@ -677,18 +687,20 @@
         self._target_id = utils._get_as_snowflake(data, "target_id")
 
     def _get_member(self, user_id: Optional[int]) -> Union[Member, User, Object, None]:
         if not user_id:
             return None
         return self.guild.get_member(user_id) or self._users.get(user_id) or Object(id=user_id)
 
-    def _get_channel(self, channel_id: Optional[int]) -> Union[abc.GuildChannel, Object, None]:
+    def _get_channel_or_thread(
+        self, channel_id: Optional[int]
+    ) -> Union[abc.GuildChannel, Thread, Object, None]:
         if not channel_id:
             return None
-        return self.guild.get_channel(channel_id) or Object(channel_id)
+        return self.guild.get_channel_or_thread(channel_id) or Object(channel_id)
 
     def _get_integration_by_application_id(
         self, application_id: int
     ) -> Optional[PartialIntegration]:
         if not application_id:
             return None
```

### Comparing `disnake-2.8.2/disnake/automod.py` & `disnake-2.9.0/disnake/automod.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,16 +56,15 @@
     "AutoModTriggerMetadata",
     "AutoModRule",
     "AutoModActionExecution",
 )
 
 
 class AutoModAction:
-    """
-    A base class for auto moderation actions.
+    """A base class for auto moderation actions.
 
     This class is not meant to be instantiated by the user.
     The user-constructible subclasses are:
 
     - :class:`AutoModBlockMessageAction`
     - :class:`AutoModSendAlertAction`
     - :class:`AutoModTimeoutAction`
@@ -107,40 +106,57 @@
         return {
             "type": self.type.value,
             "metadata": self._metadata,
         }
 
 
 class AutoModBlockMessageAction(AutoModAction):
-    """
-    Represents an auto moderation action that blocks content from being sent.
+    """Represents an auto moderation action that blocks content from being sent.
 
     .. versionadded:: 2.6
 
+    Parameters
+    ----------
+    custom_message: Optional[:class:`str`]
+        The custom message to show to the user when the rule is triggered.
+        Maximum length is 150 characters.
+
+        .. versionadded:: 2.9
+
     Attributes
     ----------
     type: :class:`AutoModActionType`
         The action type.
         Always set to :attr:`~AutoModActionType.block_message`.
     """
 
     __slots__ = ()
 
     _metadata: AutoModBlockMessageActionMetadata
 
-    def __init__(self) -> None:
+    def __init__(self, custom_message: Optional[str] = None) -> None:
         super().__init__(type=AutoModActionType.block_message)
 
+        if custom_message is not None:
+            self._metadata["custom_message"] = custom_message
+
+    @property
+    def custom_message(self) -> Optional[str]:
+        """Optional[:class:`str`]: The custom message to show to the user when the rule is triggered.
+
+        .. versionadded:: 2.9
+        """
+        return self._metadata.get("custom_message")
+
     def __repr__(self) -> str:
-        return f"<{type(self).__name__}>"
+        return f"<{type(self).__name__} custom_message={self.custom_message!r}>"
 
 
 class AutoModSendAlertAction(AutoModAction):
-    """
-    Represents an auto moderation action that sends an alert to a channel.
+    """Represents an auto moderation action that sends an alert to a channel.
 
     .. versionadded:: 2.6
 
     Parameters
     ----------
     channel: :class:`abc.Snowflake`
         The channel to send an alert in when the rule is triggered.
@@ -167,16 +183,15 @@
         return int(self._metadata["channel_id"])
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__} channel_id={self.channel_id!r}>"
 
 
 class AutoModTimeoutAction(AutoModAction):
-    """
-    Represents an auto moderation action that times out the user.
+    """Represents an auto moderation action that times out the user.
 
     .. versionadded:: 2.6
 
     Parameters
     ----------
     duration: Union[:class:`int`, :class:`datetime.timedelta`]
         The duration (seconds or timedelta) for which to timeout the user when the rule is triggered.
@@ -198,34 +213,34 @@
         if isinstance(duration, timedelta):
             duration = int(duration.total_seconds())
         self._metadata["duration_seconds"] = duration
 
     @property
     def duration(self) -> int:
         """:class:`int`: The duration (in seconds) for which to timeout
-        the user when the rule is triggered."""
+        the user when the rule is triggered.
+        """
         return self._metadata["duration_seconds"]
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__} duration={self.duration!r}>"
 
 
 class AutoModTriggerMetadata:
-    """
-    Metadata for an auto moderation trigger.
+    """Metadata for an auto moderation trigger.
 
     Based on the trigger type, different fields can be used with various limits:
 
     .. csv-table::
-        :header: "Trigger Type", ``keyword_filter``, ``regex_patterns``, ``presets``, ``allow_list``, ``mention_total_limit``
+        :header: "Trigger Type", ``keyword_filter``, ``regex_patterns``, ``presets``, ``allow_list``, ``mention_total_limit``, ``mention_raid_protection_enabled``
 
-        :attr:`~AutoModTriggerType.keyword`,        ✅ (x1000), ✅ (x10), ❌, ✅ (x100),  ❌
-        :attr:`~AutoModTriggerType.spam`,           ❌,         ❌,       ❌, ❌,         ❌
-        :attr:`~AutoModTriggerType.keyword_preset`, ❌,         ❌,       ✅, ✅ (x1000), ❌
-        :attr:`~AutoModTriggerType.mention_spam`,   ❌,         ❌,       ❌, ❌,         ✅
+        :attr:`~AutoModTriggerType.keyword`,        ✅ (x1000), ✅ (x10), ❌, ✅ (x100),  ❌, ❌
+        :attr:`~AutoModTriggerType.spam`,           ❌,         ❌,       ❌, ❌,         ❌, ❌
+        :attr:`~AutoModTriggerType.keyword_preset`, ❌,         ❌,       ✅, ✅ (x1000), ❌, ❌
+        :attr:`~AutoModTriggerType.mention_spam`,   ❌,         ❌,       ❌, ❌,         ✅, ✅
 
     .. versionadded:: 2.6
 
     Attributes
     ----------
     keyword_filter: Optional[Sequence[:class:`str`]]
         The list of keywords to check for, up to 1000 keywords. Used with :attr:`AutoModTriggerType.keyword`.
@@ -252,22 +267,30 @@
         The keywords that should be exempt from a preset.
         Used with :attr:`AutoModTriggerType.keyword` (up to 100 exemptions) and :attr:`AutoModTriggerType.keyword_preset` (up to 1000 exemptions).
 
         Each keyword must be 60 characters or less.
 
     mention_total_limit: Optional[:class:`int`]
         The maximum number of mentions (members + roles) allowed, between 1 and 50. Used with :attr:`AutoModTriggerType.mention_spam`.
+
+    mention_raid_protection_enabled: Optional[:class:`bool`]
+        Whether to automatically detect mention raids. Used with :attr:`AutoModTriggerType.mention_spam`.
+
+        Defaults to ``False``.
+
+        .. versionadded:: 2.9
     """
 
     __slots__ = (
         "keyword_filter",
         "regex_patterns",
         "presets",
         "allow_list",
         "mention_total_limit",
+        "mention_raid_protection_enabled",
     )
 
     @overload
     def __init__(
         self,
         *,
         keyword_filter: Optional[Sequence[str]],
@@ -292,43 +315,47 @@
         *,
         presets: AutoModKeywordPresets,
         allow_list: Optional[Sequence[str]] = None,
     ) -> None:
         ...
 
     @overload
-    def __init__(self, *, mention_total_limit: int) -> None:
+    def __init__(
+        self, *, mention_total_limit: int, mention_raid_protection_enabled: bool = False
+    ) -> None:
         ...
 
     def __init__(
         self,
         *,
         keyword_filter: Optional[Sequence[str]] = None,
         regex_patterns: Optional[Sequence[str]] = None,
         presets: Optional[AutoModKeywordPresets] = None,
         allow_list: Optional[Sequence[str]] = None,
         mention_total_limit: Optional[int] = None,
+        mention_raid_protection_enabled: Optional[bool] = None,
     ) -> None:
         self.keyword_filter: Optional[Sequence[str]] = keyword_filter
         self.regex_patterns: Optional[Sequence[str]] = regex_patterns
         self.presets: Optional[AutoModKeywordPresets] = presets
         self.allow_list: Optional[Sequence[str]] = allow_list
         self.mention_total_limit: Optional[int] = mention_total_limit
+        self.mention_raid_protection_enabled: Optional[bool] = mention_raid_protection_enabled
 
     def with_changes(
         self,
         *,
         keyword_filter: Optional[Sequence[str]] = MISSING,
         regex_patterns: Optional[Sequence[str]] = MISSING,
         presets: Optional[AutoModKeywordPresets] = MISSING,
         allow_list: Optional[Sequence[str]] = MISSING,
         mention_total_limit: Optional[int] = MISSING,
+        mention_raid_protection_enabled: Optional[bool] = MISSING,
     ) -> Self:
-        """
-        Returns a new instance with the given changes applied.
+        """Returns a new instance with the given changes applied.
         All other fields will be kept intact.
 
         Returns
         -------
         :class:`AutoModTriggerMetadata`
             The new metadata instance.
         """
@@ -336,14 +363,19 @@
             keyword_filter=self.keyword_filter if keyword_filter is MISSING else keyword_filter,
             regex_patterns=self.regex_patterns if regex_patterns is MISSING else regex_patterns,
             presets=self.presets if presets is MISSING else presets,
             allow_list=self.allow_list if allow_list is MISSING else allow_list,
             mention_total_limit=(
                 self.mention_total_limit if mention_total_limit is MISSING else mention_total_limit
             ),
+            mention_raid_protection_enabled=(
+                self.mention_raid_protection_enabled
+                if mention_raid_protection_enabled is MISSING
+                else mention_raid_protection_enabled
+            ),
         )
 
     @classmethod
     def _from_dict(cls, data: AutoModTriggerMetadataPayload) -> Self:
         if (presets_data := data.get("presets")) is not None:
             presets = AutoModKeywordPresets._from_values(presets_data)
         else:
@@ -351,48 +383,52 @@
 
         return cls(  # type: ignore  # call doesn't match any overloads
             keyword_filter=data.get("keyword_filter"),
             regex_patterns=data.get("regex_patterns"),
             presets=presets,
             allow_list=data.get("allow_list"),
             mention_total_limit=data.get("mention_total_limit"),
+            mention_raid_protection_enabled=data.get("mention_raid_protection_enabled"),
         )
 
     def to_dict(self) -> AutoModTriggerMetadataPayload:
         data: AutoModTriggerMetadataPayload = {}
         if self.keyword_filter is not None:
             data["keyword_filter"] = list(self.keyword_filter)
         if self.regex_patterns is not None:
             data["regex_patterns"] = list(self.regex_patterns)
         if self.presets is not None:
             data["presets"] = self.presets.values  # type: ignore  # `values` contains ints instead of preset literal values
         if self.allow_list is not None:
             data["allow_list"] = list(self.allow_list)
         if self.mention_total_limit is not None:
             data["mention_total_limit"] = self.mention_total_limit
+        if self.mention_raid_protection_enabled is not None:
+            data["mention_raid_protection_enabled"] = self.mention_raid_protection_enabled
         return data
 
     def __repr__(self) -> str:
         s = f"<{type(self).__name__}"
         if self.keyword_filter is not None:
             s += f" keyword_filter={self.keyword_filter!r}"
         if self.regex_patterns is not None:
             s += f" regex_patterns={self.regex_patterns!r}"
         if self.presets is not None:
             s += f" presets={self.presets!r}"
         if self.allow_list is not None:
             s += f" allow_list={self.allow_list!r}"
         if self.mention_total_limit is not None:
             s += f" mention_total_limit={self.mention_total_limit!r}"
+        if self.mention_raid_protection_enabled is not None:
+            s += f" mention_raid_protection_enabled={self.mention_raid_protection_enabled!r}"
         return f"{s}>"
 
 
 class AutoModRule:
-    """
-    Represents an auto moderation rule.
+    """Represents an auto moderation rule.
 
     .. versionadded:: 2.6
 
     Attributes
     ----------
     id: :class:`int`
         The rule ID.
@@ -455,15 +491,16 @@
             if (exempt_channels := data.get("exempt_channels"))
             else frozenset()
         )
 
     @property
     def actions(self) -> List[AutoModAction]:
         """List[Union[:class:`AutoModBlockMessageAction`, :class:`AutoModSendAlertAction`, :class:`AutoModTimeoutAction`, :class:`AutoModAction`]]:
-        The list of actions that will execute if a matching event triggered this rule."""
+        The list of actions that will execute if a matching event triggered this rule.
+        """
         return list(self._actions)  # return a copy
 
     @property
     def creator(self) -> Optional[Member]:
         """Optional[:class:`Member`]: The guild member that created this rule.
         May be ``None`` if the member cannot be found. See also :attr:`.creator_id`.
         """
@@ -503,17 +540,19 @@
 
         Edits the auto moderation rule.
 
         You must have :attr:`.Permissions.manage_guild` permission to do this.
 
         All fields are optional.
 
+        .. versionchanged:: 2.9
+            Now raises a :exc:`TypeError` if given ``actions`` have an invalid type.
+
         Examples
         --------
-
         Edit name and enable rule:
 
         .. code-block:: python3
 
             await rule.edit(name="cool new rule", enabled=True)
 
         Add an action:
@@ -558,38 +597,44 @@
         reason: Optional[:class:`str`]
             The reason for editing the rule. Shows up on the audit log.
 
         Raises
         ------
         ValueError
             When editing the list of actions, at least one action must be provided.
+        TypeError
+            The specified ``actions`` are of an invalid type.
         Forbidden
             You do not have proper permissions to edit the rule.
         NotFound
             The rule does not exist.
         HTTPException
             Editing the rule failed.
 
         Returns
         -------
         :class:`AutoModRule`
             The newly updated auto moderation rule.
         """
-
         payload: EditAutoModRulePayload = {}
 
         if name is not MISSING:
             payload["name"] = name
         if event_type is not MISSING:
             payload["event_type"] = try_enum_to_int(event_type)
         if trigger_metadata is not MISSING:
             payload["trigger_metadata"] = trigger_metadata.to_dict()
         if actions is not MISSING:
-            if len(actions) == 0:
+            if not actions:
                 raise ValueError("At least one action must be provided.")
+            for action in actions:
+                if not isinstance(action, AutoModAction):
+                    raise TypeError(
+                        f"actions must be of type `AutoModAction` (or subtype), not {type(action)!r}"
+                    )
             payload["actions"] = [a.to_dict() for a in actions]
         if enabled is not MISSING:
             payload["enabled"] = enabled
         if exempt_roles is not MISSING:
             payload["exempt_roles"] = (
                 [e.id for e in exempt_roles] if exempt_roles is not None else []
             )
@@ -725,22 +770,24 @@
         """
         return self.guild._resolve_channel(self.channel_id)
 
     @property
     def message(self) -> Optional[Message]:
         """Optional[:class:`Message`]: The message that matched, if any.
         Not available if the message was blocked, if the content was not part of a message,
-        or if the message was not found in the message cache."""
+        or if the message was not found in the message cache.
+        """
         return self.guild._state._get_message(self.message_id)
 
     @property
     def alert_message(self) -> Optional[Message]:
         """Optional[:class:`Message`]: The alert message sent as a result of this action, if any.
         Only available if :attr:`action.type <AutoModAction.type>` is :attr:`~AutoModActionType.send_alert_message`
-        and the message was found in the message cache."""
+        and the message was found in the message cache.
+        """
         return self.guild._state._get_message(self.alert_message_id)
 
 
 _action_map: Dict[int, Type[AutoModAction]] = {
     AutoModActionType.block_message.value: AutoModBlockMessageAction,
     AutoModActionType.send_alert_message.value: AutoModSendAlertAction,
     AutoModActionType.timeout.value: AutoModTimeoutAction,
```

### Comparing `disnake-2.8.2/disnake/backoff.py` & `disnake-2.9.0/disnake/backoff.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/bin/COPYING` & `disnake-2.9.0/disnake/bin/COPYING`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/bin/libopus-0.x64.dll` & `disnake-2.9.0/disnake/bin/libopus-0.x64.dll`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/bin/libopus-0.x86.dll` & `disnake-2.9.0/disnake/bin/libopus-0.x86.dll`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/channel.py` & `disnake-2.9.0/disnake/channel.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     ThreadSortOrder,
     VideoQualityMode,
     try_enum,
     try_enum_to_int,
 )
 from .errors import ClientException
 from .file import File
-from .flags import ChannelFlags
+from .flags import ChannelFlags, MessageFlags
 from .iterators import ArchivedThreadIterator
 from .mixins import Hashable
 from .partial_emoji import PartialEmoji
 from .permissions import PermissionOverwrite, Permissions
 from .stage_instance import StageInstance
 from .threads import ForumTag, Thread
 from .utils import MISSING
@@ -74,14 +74,15 @@
     from .message import AllowedMentions, Message, PartialMessage
     from .role import Role
     from .state import ConnectionState
     from .sticker import GuildSticker, StickerItem
     from .threads import AnyThreadArchiveDuration, ThreadType
     from .types.channel import (
         CategoryChannel as CategoryChannelPayload,
+        DefaultReaction as DefaultReactionPayload,
         DMChannel as DMChannelPayload,
         ForumChannel as ForumChannelPayload,
         GroupDMChannel as GroupChannelPayload,
         StageChannel as StageChannelPayload,
         TextChannel as TextChannelPayload,
         VoiceChannel as VoiceChannelPayload,
     )
@@ -258,14 +259,15 @@
         self,
         obj: Union[Member, Role],
         /,
         *,
         ignore_timeout: bool = MISSING,
     ) -> Permissions:
         base = super().permissions_for(obj, ignore_timeout=ignore_timeout)
+        self._apply_implict_permissions(base)
 
         # text channels do not have voice related permissions
         denied = Permissions.voice()
         base.value &= ~denied.value
         return base
 
     @property
@@ -473,22 +475,120 @@
             reason=reason,
             **kwargs,
         )
         if payload is not None:
             # the payload will always be the proper channel payload
             return self.__class__(state=self._state, guild=self.guild, data=payload)  # type: ignore
 
-    @utils.copy_doc(disnake.abc.GuildChannel.clone)
     async def clone(
-        self, *, name: Optional[str] = None, reason: Optional[str] = None
+        self,
+        *,
+        name: Optional[str] = None,
+        topic: Optional[str] = MISSING,
+        position: int = MISSING,
+        nsfw: bool = MISSING,
+        category: Optional[Snowflake] = MISSING,
+        slowmode_delay: int = MISSING,
+        default_thread_slowmode_delay: Optional[int] = MISSING,
+        default_auto_archive_duration: AnyThreadArchiveDuration = MISSING,
+        overwrites: Mapping[Union[Role, Member], PermissionOverwrite] = MISSING,
+        news: bool = MISSING,
+        reason: Optional[str] = None,
     ) -> TextChannel:
+        """|coro|
+
+        Clones this channel. This creates a channel with the same properties
+        as this channel.
+
+        You must have :attr:`.Permissions.manage_channels` permission to
+        do this.
+
+        .. versionchanged:: 2.9
+            Added ``topic``, ``position``, ``nsfw``, ``category``, ``slowmode_delay``,
+            ``default_thread_slowmode_delay``, ``default_auto_archive_duration``, ``news``
+            and ``overwrites`` keyword-only parameters.
+
+        .. note::
+            The current :attr:`TextChannel.flags` value won't be cloned.
+            This is a Discord limitation.
+
+        Parameters
+        ----------
+        name: Optional[:class:`str`]
+            The name of the new channel. If not provided, defaults to this channel's name.
+        topic: Optional[:class:`str`]
+            The topic of the new channel. If not provided, defaults to this channel's topic.
+        position: :class:`int`
+            The position of the new channel. If not provided, defaults to this channel's position.
+        nsfw: :class:`bool`
+            Whether the new channel should be marked as NSFW. If not provided, defaults to this channel's NSFW value.
+        category: Optional[:class:`abc.Snowflake`]
+            The category where the new channel should be grouped. If not provided, defaults to this channel's category.
+        slowmode_delay: :class:`int`
+            The slowmode of the new channel. If not provided, defaults to this channel's slowmode.
+        default_thread_slowmode_delay: Optional[:class:`int`]
+            Specifies the slowmode rate limit at which users can send messages
+            in newly created threads in this channel, in seconds.
+            This does not apply retroactively to existing threads.
+            A value of ``0`` or ``None`` disables slowmode. The maximum value possible is ``21600``. If not provided, defaults
+            to this channel's default thread slowmode delay.
+        default_auto_archive_duration: Union[:class:`int`, :class:`ThreadArchiveDuration`]
+            The default auto archive duration of the new channel. If not provided, defaults to this channel's default auto archive duration.
+        overwrites: :class:`Mapping`
+            A :class:`Mapping` of target (either a role or a member) to :class:`PermissionOverwrite`
+            to apply to the channel. If not provided, defaults to this channel's overwrites.
+        news: :class:`bool`
+            Whether the new channel should be a news channel. News channels are text channels that can be followed.
+            This is only available to guilds that contain ``NEWS`` in :attr:`Guild.features`. If not provided, defaults to the current type of this channel.
+        reason: Optional[:class:`str`]
+            The reason for cloning this channel. Shows up on the audit log.
+
+        Raises
+        ------
+        Forbidden
+            You do not have the proper permissions to create this channel.
+        HTTPException
+            Creating the channel failed.
+
+        Returns
+        -------
+        :class:`TextChannel`
+            The newly created text channel.
+        """
+        if news is not MISSING:
+            # if news is True set the channel_type to News, otherwise if it's False set it to Text
+            channel_type = ChannelType.news if news else ChannelType.text
+        else:
+            # if news is not given falls back to the original TextChannel type
+            channel_type = self.type
+
         return await self._clone_impl(
-            {"topic": self.topic, "nsfw": self.nsfw, "rate_limit_per_user": self.slowmode_delay},
+            {
+                "topic": topic if topic is not MISSING else self.topic,
+                "position": position if position is not MISSING else self.position,
+                "nsfw": nsfw if nsfw is not MISSING else self.nsfw,
+                "type": channel_type.value,
+                "rate_limit_per_user": (
+                    slowmode_delay if slowmode_delay is not MISSING else self.slowmode_delay
+                ),
+                "default_thread_rate_limit_per_user": (
+                    default_thread_slowmode_delay
+                    if default_thread_slowmode_delay is not MISSING
+                    else self.default_thread_slowmode_delay
+                ),
+                "default_auto_archive_duration": (
+                    try_enum_to_int(default_auto_archive_duration)
+                    if default_auto_archive_duration is not MISSING
+                    else self.default_auto_archive_duration
+                ),
+            },
             name=name,
+            category=category,
             reason=reason,
+            overwrites=overwrites,
         )
 
     async def delete_messages(self, messages: Iterable[Snowflake]) -> None:
         """|coro|
 
         Deletes a list of messages. This is similar to :meth:`Message.delete`
         except it bulk deletes multiple messages.
@@ -556,15 +656,14 @@
         You must have :attr:`~Permissions.manage_messages` permission to
         delete messages even if they are your own.
         :attr:`~Permissions.read_message_history` permission is
         also needed to retrieve message history.
 
         Examples
         --------
-
         Deleting bot's messages ::
 
             def is_me(m):
                 return m.author == client.user
 
             deleted = await channel.purge(limit=100, check=is_me)
             await channel.send(f'Deleted {len(deleted)} message(s)')
@@ -985,15 +1084,15 @@
         ------
         Forbidden
             You do not have permissions to get archived threads.
         HTTPException
             The request to get the archived threads failed.
 
         Yields
-        -------
+        ------
         :class:`Thread`
             The archived threads.
         """
         return ArchivedThreadIterator(
             self.id, self.guild, limit=limit, joined=joined, private=private, before=before
         )
 
@@ -1081,14 +1180,43 @@
         """
         return {
             key: value
             for key, value in self.guild._voice_states.items()
             if value.channel and value.channel.id == self.id
         }
 
+    @utils.copy_doc(disnake.abc.GuildChannel.permissions_for)
+    def permissions_for(
+        self,
+        obj: Union[Member, Role],
+        /,
+        *,
+        ignore_timeout: bool = MISSING,
+    ) -> Permissions:
+        base = super().permissions_for(obj, ignore_timeout=ignore_timeout)
+        self._apply_implict_permissions(base)
+
+        # voice channels cannot be edited by people who can't connect to them
+        # It also implicitly denies all other voice perms
+        if not base.connect:
+            denied = Permissions.voice()
+            # voice channels also deny all text related permissions
+            denied.value |= Permissions.text().value
+            # stage channels remove the stage permissions
+            denied.value |= Permissions.stage().value
+
+            denied.update(
+                manage_channels=True,
+                manage_roles=True,
+                manage_events=True,
+                manage_webhooks=True,
+            )
+            base.value &= ~denied.value
+        return base
+
 
 class VoiceChannel(disnake.abc.Messageable, VocalGuildChannel):
     """Represents a Discord guild voice channel.
 
     .. container:: operations
 
         .. describe:: x == y
@@ -1194,20 +1322,104 @@
     def type(self) -> Literal[ChannelType.voice]:
         """:class:`ChannelType`: The channel's Discord type.
 
         This always returns :attr:`ChannelType.voice`.
         """
         return ChannelType.voice
 
-    @utils.copy_doc(disnake.abc.GuildChannel.clone)
     async def clone(
-        self, *, name: Optional[str] = None, reason: Optional[str] = None
+        self,
+        *,
+        name: Optional[str] = None,
+        bitrate: int = MISSING,
+        user_limit: int = MISSING,
+        position: int = MISSING,
+        category: Optional[Snowflake] = MISSING,
+        rtc_region: Optional[Union[str, VoiceRegion]] = MISSING,
+        video_quality_mode: VideoQualityMode = MISSING,
+        nsfw: bool = MISSING,
+        overwrites: Mapping[Union[Role, Member], PermissionOverwrite] = MISSING,
+        slowmode_delay: Optional[int] = MISSING,
+        reason: Optional[str] = None,
     ) -> VoiceChannel:
+        """|coro|
+
+        Clones this channel. This creates a channel with the same properties
+        as this channel.
+
+        You must have :attr:`.Permissions.manage_channels` permission to
+        do this.
+
+        .. versionchanged:: 2.9
+            Added ``bitrate``, ``user_limit``, ``position``, ``category``,
+            ``rtc_region``, ``video_quality_mode``, ``nsfw``, ``slowmode_delay``
+            and ``overwrites`` keyword-only parameters.
+
+        .. note::
+            The current :attr:`VoiceChannel.flags` value won't be cloned.
+            This is a Discord limitation.
+
+        Parameters
+        ----------
+        name: Optional[:class:`str`]
+            The name of the new channel. If not provided, defaults to this channel's name.
+        bitrate: :class:`int`
+            The bitrate of the new channel. If not provided, defaults to this channel's bitrate.
+        user_limit: :class:`int`
+            The user limit of the new channel. If not provided, defaults to this channel's user limit.
+        position: :class:`int`
+            The position of the new channel. If not provided, defaults to this channel's position.
+        category: Optional[:class:`abc.Snowflake`]
+            The category where the new channel should be grouped. If not provided, defaults to this channel's category.
+        rtc_region: Optional[Union[:class:`str`, :class:`VoiceRegion`]]
+            The rtc region of the new channel. If not provided, defaults to this channel's rtc region.
+        video_quality_mode: :class:`VideoQualityMode`
+            The video quality mode of the new channel. If not provided, defaults to this channel's video quality mode.
+        nsfw: :class:`bool`
+            Whether the new channel should be nsfw or not. If not provided, defaults to this channel's NSFW value.
+        overwrites: :class:`Mapping`
+            A :class:`Mapping` of target (either a role or a member) to :class:`PermissionOverwrite` to apply
+            to the channel. If not provided, defaults to this channel's overwrites.
+        slowmode_delay: Optional[:class:`int`]
+            The slowmode of the new channel. If not provided, defaults to this channel's slowmode.
+        reason: Optional[:class:`str`]
+            The reason for cloning this channel. Shows up on the audit log.
+
+        Raises
+        ------
+        Forbidden
+            You do not have the proper permissions to create this channel.
+        HTTPException
+            Creating the channel failed.
+
+        Returns
+        -------
+        :class:`VoiceChannel`
+            The channel that was created.
+        """
         return await self._clone_impl(
-            {"bitrate": self.bitrate, "user_limit": self.user_limit}, name=name, reason=reason
+            {
+                "bitrate": bitrate if bitrate is not MISSING else self.bitrate,
+                "user_limit": user_limit if user_limit is not MISSING else self.user_limit,
+                "position": position if position is not MISSING else self.position,
+                "rtc_region": (str(rtc_region) if rtc_region is not MISSING else self.rtc_region),
+                "video_quality_mode": (
+                    int(video_quality_mode)
+                    if video_quality_mode is not MISSING
+                    else int(self.video_quality_mode)
+                ),
+                "nsfw": nsfw if nsfw is not MISSING else self.nsfw,
+                "rate_limit_per_user": (
+                    slowmode_delay if slowmode_delay is not MISSING else self.slowmode_delay
+                ),
+            },
+            name=name,
+            category=category,
+            reason=reason,
+            overwrites=overwrites,
         )
 
     def is_nsfw(self) -> bool:
         """Whether the channel is marked as NSFW.
 
         .. versionadded:: 2.3
 
@@ -1256,34 +1468,14 @@
         :class:`PartialMessage`
             The partial message object.
         """
         from .message import PartialMessage
 
         return PartialMessage(channel=self, id=message_id)
 
-    @utils.copy_doc(disnake.abc.GuildChannel.permissions_for)
-    def permissions_for(
-        self,
-        obj: Union[Member, Role],
-        /,
-        *,
-        ignore_timeout: bool = MISSING,
-    ) -> Permissions:
-        base = super().permissions_for(obj, ignore_timeout=ignore_timeout)
-
-        # voice channels cannot be edited by people who can't connect to them
-        # It also implicitly denies all other voice perms
-        if not base.connect:
-            denied = Permissions.voice()
-            # voice channels also deny all text related permissions
-            denied.value |= Permissions.text().value
-            denied.update(manage_channels=True, manage_roles=True)
-            base.value &= ~denied.value
-        return base
-
     # if only these parameters are passed, `_move` is called and no channel will be returned
     @overload
     async def edit(
         self,
         *,
         position: int,
         category: Optional[Snowflake] = ...,
@@ -1356,21 +1548,21 @@
 
         .. versionchanged:: 2.6
             Raises :exc:`TypeError` or :exc:`ValueError` instead of ``InvalidArgument``.
 
         Parameters
         ----------
         name: :class:`str`
-            The new channel's name.
+            The channel's new name.
         bitrate: :class:`int`
-            The new channel's bitrate.
+            The channel's new bitrate.
         user_limit: :class:`int`
-            The new channel's user limit.
+            The channel's new user limit.
         position: :class:`int`
-            The new channel's position.
+            The channel's new position.
         sync_permissions: :class:`bool`
             Whether to sync permissions with the channel's new or pre-existing
             category. Defaults to ``False``.
         category: Optional[:class:`abc.Snowflake`]
             The new category for this channel. Can be ``None`` to remove the
             category.
         reason: Optional[:class:`str`]
@@ -1670,15 +1862,15 @@
 
         data = await self._state.http.create_webhook(
             self.id, name=str(name), avatar=avatar_data, reason=reason
         )
         return Webhook.from_state(data, state=self._state)
 
 
-class StageChannel(VocalGuildChannel):
+class StageChannel(disnake.abc.Messageable, VocalGuildChannel):
     """Represents a Discord guild stage channel.
 
     .. versionadded:: 1.7
 
     .. container:: operations
 
         .. describe:: x == y
@@ -1723,37 +1915,71 @@
         .. versionchanged:: 2.5
             No longer a ``VoiceRegion`` instance.
 
     video_quality_mode: :class:`VideoQualityMode`
         The camera video quality for the stage channel's participants.
 
         .. versionadded:: 2.0
+    nsfw: :class:`bool`
+        Whether the channel is marked as "not safe for work".
+
+        .. note::
+
+            To check if the channel or the guild of that channel are marked as NSFW, consider :meth:`is_nsfw` instead.
+
+        .. versionadded:: 2.9
+
+    slowmode_delay: :class:`int`
+        The number of seconds a member must wait between sending messages
+        in this channel. A value of `0` denotes that it is disabled.
+        Bots, and users with :attr:`~Permissions.manage_channels` or
+        :attr:`~Permissions.manage_messages`, bypass slowmode.
+
+        .. versionadded:: 2.9
+
+    last_message_id: Optional[:class:`int`]
+        The last message ID of the message sent to this channel. It may
+        *not* point to an existing or valid message.
+
+        .. versionadded:: 2.9
     """
 
-    __slots__ = ("topic",)
+    __slots__ = (
+        "topic",
+        "nsfw",
+        "slowmode_delay",
+        "last_message_id",
+    )
 
     def __repr__(self) -> str:
         attrs = (
             ("id", self.id),
             ("name", self.name),
             ("topic", self.topic),
             ("rtc_region", self.rtc_region),
             ("position", self.position),
             ("bitrate", self.bitrate),
             ("video_quality_mode", self.video_quality_mode),
             ("user_limit", self.user_limit),
             ("category_id", self.category_id),
+            ("nsfw", self.nsfw),
             ("flags", self.flags),
         )
         joined = " ".join(f"{k!s}={v!r}" for k, v in attrs)
         return f"<{self.__class__.__name__} {joined}>"
 
     def _update(self, guild: Guild, data: StageChannelPayload) -> None:
         super()._update(guild, data)
         self.topic: Optional[str] = data.get("topic")
+        self.nsfw: bool = data.get("nsfw", False)
+        self.slowmode_delay: int = data.get("rate_limit_per_user", 0)
+        self.last_message_id: Optional[int] = utils._get_as_snowflake(data, "last_message_id")
+
+    async def _get_channel(self):
+        return self
 
     @property
     def requesting_to_speak(self) -> List[Member]:
         """List[:class:`Member`]: A list of members who are requesting to speak in the stage channel."""
         return [
             member
             for member in self.members
@@ -1799,46 +2025,172 @@
     def type(self) -> Literal[ChannelType.stage_voice]:
         """:class:`ChannelType`: The channel's Discord type.
 
         This always returns :attr:`ChannelType.stage_voice`.
         """
         return ChannelType.stage_voice
 
-    @utils.copy_doc(disnake.abc.GuildChannel.clone)
     async def clone(
-        self, *, name: Optional[str] = None, reason: Optional[str] = None
+        self,
+        *,
+        name: Optional[str] = None,
+        bitrate: int = MISSING,
+        # user_limit: int = MISSING,
+        position: int = MISSING,
+        category: Optional[Snowflake] = MISSING,
+        slowmode_delay: int = MISSING,
+        rtc_region: Optional[Union[str, VoiceRegion]] = MISSING,
+        video_quality_mode: VideoQualityMode = MISSING,
+        nsfw: bool = MISSING,
+        overwrites: Mapping[Union[Role, Member], PermissionOverwrite] = MISSING,
+        reason: Optional[str] = None,
     ) -> StageChannel:
-        return await self._clone_impl({}, name=name, reason=reason)
+        """|coro|
+
+        Clones this channel. This creates a channel with the same properties
+        as this channel.
+
+        You must have :attr:`.Permissions.manage_channels` permission to
+        do this.
+
+        .. versionchanged:: 2.9
+            Added ``position``, ``category``, ``rtc_region``,
+            ``video_quality_mode``, ``bitrate``, ``nsfw``, ``slowmode_delay`` and ``overwrites`` keyword-only parameters.
+
+        .. note::
+            The current :attr:`StageChannel.flags` value won't be cloned.
+            This is a Discord limitation.
+
+        .. warning::
+            Currently the ``user_limit`` attribute is not cloned due to a Discord limitation.
+            You can directly edit the channel after its creation to set
+            a `user_limit`.
+
+        Parameters
+        ----------
+        name: Optional[:class:`str`]
+            The name of the new channel. If not provided, defaults to this channel's name.
+        bitrate: :class:`int`
+            The bitrate of the new channel. If not provided, defaults to this channel's bitrate.
+        position: :class:`int`
+            The position of the new channel. If not provided, defaults to this channel's position.
+        category: Optional[:class:`abc.Snowflake`]
+            The category where the new channel should be grouped. If not provided, defaults to this channel's category.
+        slowmode_delay: :class:`int`
+            The slowmode of the new channel. If not provided, defaults to this channel's slowmode.
+        rtc_region: Optional[Union[:class:`str`, :class:`VoiceRegion`]]
+            The rtc region of the new channel. If not provided, defaults to this channel's rtc region.
+        video_quality_mode: :class:`VideoQualityMode`
+            The video quality mode of the new channel. If not provided, defaults to this channel's video quality mode.
+        nsfw: :class:`bool`
+            Whether the new channel should be nsfw or not. If not provided, defaults to this channel's NSFW value.
+        overwrites: :class:`Mapping`
+            A :class:`Mapping` of target (either a role or a member) to :class:`PermissionOverwrite`
+            to apply to the channel. If not provided, defaults to this channel's overwrites.
+        reason: Optional[:class:`str`]
+            The reason for cloning this channel. Shows up on the audit log.
+
+        Raises
+        ------
+        Forbidden
+            You do not have the proper permissions to create this channel.
+        HTTPException
+            Creating the channel failed.
+
+        Returns
+        -------
+        :class:`StageChannel`
+            The channel that was created.
+        """
+        # TODO
+        # - check if discord-api-docs#5962 is solved and clone the user_limit attribute
+        return await self._clone_impl(
+            {
+                "rate_limit_per_user": (
+                    slowmode_delay if slowmode_delay is not MISSING else self.slowmode_delay
+                ),
+                "bitrate": bitrate if bitrate is not MISSING else self.bitrate,
+                # "user_limit": user_limit if user_limit is not MISSING else self.user_limit,
+                "position": position if position is not MISSING else self.position,
+                "rtc_region": (str(rtc_region) if rtc_region is not MISSING else self.rtc_region),
+                "video_quality_mode": (
+                    int(video_quality_mode)
+                    if video_quality_mode is not MISSING
+                    else int(self.video_quality_mode)
+                ),
+                "nsfw": nsfw if nsfw is not MISSING else self.nsfw,
+            },
+            name=name,
+            category=category,
+            reason=reason,
+            overwrites=overwrites,
+        )
+
+    def is_nsfw(self) -> bool:
+        """Whether the channel is marked as NSFW.
+
+        .. versionadded:: 2.9
+
+        :return type: :class:`bool`
+        """
+        return self.nsfw
+
+    @property
+    def last_message(self) -> Optional[Message]:
+        """Gets the last message in this channel from the cache.
+
+        The message might not be valid or point to an existing message.
+
+        .. admonition:: Reliable Fetching
+            :class: helpful
+
+            For a slightly more reliable method of fetching the
+            last message, consider using either :meth:`history`
+            or :meth:`fetch_message` with the :attr:`last_message_id`
+            attribute.
+
+        .. versionadded:: 2.9
+
+        Returns
+        -------
+        Optional[:class:`Message`]
+            The last message in this channel or ``None`` if not found.
+        """
+        return self._state._get_message(self.last_message_id) if self.last_message_id else None
+
+    def get_partial_message(self, message_id: int, /) -> PartialMessage:
+        """Creates a :class:`PartialMessage` from the given message ID.
+
+        This is useful if you want to work with a message and only have its ID without
+        doing an unnecessary API call.
+
+        .. versionadded:: 2.9
+
+        Parameters
+        ----------
+        message_id: :class:`int`
+            The message ID to create a partial message for.
+
+        Returns
+        -------
+        :class:`PartialMessage`
+            The partial message object.
+        """
+        from .message import PartialMessage
+
+        return PartialMessage(channel=self, id=message_id)
 
     @property
     def instance(self) -> Optional[StageInstance]:
         """Optional[:class:`StageInstance`]: The running stage instance of the stage channel.
 
         .. versionadded:: 2.0
         """
         return utils.get(self.guild.stage_instances, channel_id=self.id)
 
-    @utils.copy_doc(disnake.abc.GuildChannel.permissions_for)
-    def permissions_for(
-        self,
-        obj: Union[Member, Role],
-        /,
-        *,
-        ignore_timeout: bool = MISSING,
-    ) -> Permissions:
-        base = super().permissions_for(obj, ignore_timeout=ignore_timeout)
-
-        # voice channels cannot be edited by people who can't connect to them
-        # It also implicitly denies all other voice perms
-        if not base.connect:
-            denied = Permissions.voice()
-            denied.update(manage_channels=True, manage_roles=True)
-            base.value &= ~denied.value
-        return base
-
     async def create_instance(
         self,
         *,
         topic: str,
         privacy_level: StagePrivacyLevel = MISSING,
         notify_everyone: bool = False,
         reason: Optional[str] = None,
@@ -1950,37 +2302,43 @@
         ...
 
     @overload
     async def edit(
         self,
         *,
         name: str = ...,
+        bitrate: int = ...,
+        user_limit: int = ...,
         position: int = ...,
         sync_permissions: bool = ...,
         category: Optional[Snowflake] = ...,
         overwrites: Mapping[Union[Role, Member], PermissionOverwrite] = ...,
         rtc_region: Optional[Union[str, VoiceRegion]] = ...,
         video_quality_mode: VideoQualityMode = ...,
-        bitrate: int = ...,
+        nsfw: bool = ...,
+        slowmode_delay: Optional[int] = ...,
         flags: ChannelFlags = ...,
         reason: Optional[str] = ...,
     ) -> StageChannel:
         ...
 
     async def edit(
         self,
         *,
         name: str = MISSING,
+        bitrate: int = MISSING,
+        user_limit: int = MISSING,
         position: int = MISSING,
         sync_permissions: bool = MISSING,
         category: Optional[Snowflake] = MISSING,
         overwrites: Mapping[Union[Role, Member], PermissionOverwrite] = MISSING,
         rtc_region: Optional[Union[str, VoiceRegion]] = MISSING,
         video_quality_mode: VideoQualityMode = MISSING,
-        bitrate: int = MISSING,
+        nsfw: bool = MISSING,
+        slowmode_delay: Optional[int] = MISSING,
         flags: ChannelFlags = MISSING,
         reason: Optional[str] = None,
         **kwargs: Never,
     ) -> Optional[StageChannel]:
         """|coro|
 
         Edits the channel.
@@ -1993,20 +2351,34 @@
 
         .. versionchanged:: 2.0
             Edits are no longer in-place, the newly edited channel is returned instead.
 
         .. versionchanged:: 2.6
             Raises :exc:`TypeError` or :exc:`ValueError` instead of ``InvalidArgument``.
 
+        .. versionchanged:: 2.9
+            The ``user_limit``, ``nsfw``, and ``slowmode_delay``
+            keyword-only parameters were added.
+
         Parameters
         ----------
         name: :class:`str`
-            The new channel's name.
+            The channel's new name.
+        bitrate: :class:`int`
+            The channel's new bitrate.
+
+            .. versionadded:: 2.6
+
+        user_limit: :class:`int`
+            The channel's new user limit.
+
+            .. versionadded:: 2.9
+
         position: :class:`int`
-            The new channel's position.
+            The channel's new position.
         sync_permissions: :class:`bool`
             Whether to sync permissions with the channel's new or pre-existing
             category. Defaults to ``False``.
         category: Optional[:class:`abc.Snowflake`]
             The new category for this channel. Can be ``None`` to remove the
             category.
         overwrites: :class:`Mapping`
@@ -2014,20 +2386,26 @@
             :class:`PermissionOverwrite` to apply to the channel.
         rtc_region: Optional[Union[:class:`str`, :class:`VoiceRegion`]]
             The new region for the stage channel's voice communication.
             A value of ``None`` indicates automatic voice region detection.
         video_quality_mode: :class:`VideoQualityMode`
             The camera video quality for the stage channel's participants.
 
-            .. versionadded:: 2.0
+            .. versionadded:: 2.9
 
-        bitrate: :class:`int`
-            The new channel's bitrate.
+        nsfw: :class:`bool`
+            Whether to mark the channel as NSFW.
 
-            .. versionadded:: 2.6
+            .. versionadded:: 2.9
+
+        slowmode_delay: Optional[:class:`int`]
+            Specifies the slowmode rate limit for users in this channel, in seconds.
+            A value of ``0`` disables slowmode. The maximum value possible is ``21600``.
+
+            .. versionadded:: 2.9
 
         flags: :class:`ChannelFlags`
             The new flags to set for this channel. This will overwrite any existing flags set on this channel.
 
             .. versionadded:: 2.6
 
         reason: Optional[:class:`str`]
@@ -2048,29 +2426,263 @@
         -------
         Optional[:class:`.StageChannel`]
             The newly edited stage channel. If the edit was only positional
             then ``None`` is returned instead.
         """
         payload = await self._edit(
             name=name,
+            bitrate=bitrate,
             position=position,
+            user_limit=user_limit,
             sync_permissions=sync_permissions,
             category=category,
             overwrites=overwrites,
             rtc_region=rtc_region,
             video_quality_mode=video_quality_mode,
-            bitrate=bitrate,
+            nsfw=nsfw,
             flags=flags,
+            slowmode_delay=slowmode_delay,
             reason=reason,
             **kwargs,
         )
         if payload is not None:
             # the payload will always be the proper channel payload
             return self.__class__(state=self._state, guild=self.guild, data=payload)  # type: ignore
 
+    async def delete_messages(self, messages: Iterable[Snowflake]) -> None:
+        """|coro|
+
+        Deletes a list of messages. This is similar to :meth:`Message.delete`
+        except it bulk deletes multiple messages.
+
+        As a special case, if the number of messages is 0, then nothing
+        is done. If the number of messages is 1 then single message
+        delete is done. If it's more than two, then bulk delete is used.
+
+        You cannot bulk delete more than 100 messages or messages that
+        are older than 14 days.
+
+        You must have :attr:`~Permissions.manage_messages` permission to
+        do this.
+
+        .. versionadded:: 2.9
+
+        Parameters
+        ----------
+        messages: Iterable[:class:`abc.Snowflake`]
+            An iterable of messages denoting which ones to bulk delete.
+
+        Raises
+        ------
+        ClientException
+            The number of messages to delete was more than 100.
+        Forbidden
+            You do not have proper permissions to delete the messages.
+        NotFound
+            If single delete, then the message was already deleted.
+        HTTPException
+            Deleting the messages failed.
+        """
+        if not isinstance(messages, (list, tuple)):
+            messages = list(messages)
+
+        if len(messages) == 0:
+            return  # do nothing
+
+        if len(messages) == 1:
+            message_id: int = messages[0].id
+            await self._state.http.delete_message(self.id, message_id)
+            return
+
+        if len(messages) > 100:
+            raise ClientException("Can only bulk delete messages up to 100 messages")
+
+        message_ids: SnowflakeList = [m.id for m in messages]
+        await self._state.http.delete_messages(self.id, message_ids)
+
+    async def purge(
+        self,
+        *,
+        limit: Optional[int] = 100,
+        check: Callable[[Message], bool] = MISSING,
+        before: Optional[SnowflakeTime] = None,
+        after: Optional[SnowflakeTime] = None,
+        around: Optional[SnowflakeTime] = None,
+        oldest_first: Optional[bool] = False,
+        bulk: bool = True,
+    ) -> List[Message]:
+        """|coro|
+
+        Purges a list of messages that meet the criteria given by the predicate
+        ``check``. If a ``check`` is not provided then all messages are deleted
+        without discrimination.
+
+        You must have :attr:`~Permissions.manage_messages` permission to
+        delete messages even if they are your own.
+        :attr:`~Permissions.read_message_history` permission is
+        also needed to retrieve message history.
+
+        .. versionadded:: 2.9
+
+        .. note::
+
+            See :meth:`TextChannel.purge` for examples.
+
+        Parameters
+        ----------
+        limit: Optional[:class:`int`]
+            The number of messages to search through. This is not the number
+            of messages that will be deleted, though it can be.
+        check: Callable[[:class:`Message`], :class:`bool`]
+            The function used to check if a message should be deleted.
+            It must take a :class:`Message` as its sole parameter.
+        before: Optional[Union[:class:`abc.Snowflake`, :class:`datetime.datetime`]]
+            Same as ``before`` in :meth:`history`.
+        after: Optional[Union[:class:`abc.Snowflake`, :class:`datetime.datetime`]]
+            Same as ``after`` in :meth:`history`.
+        around: Optional[Union[:class:`abc.Snowflake`, :class:`datetime.datetime`]]
+            Same as ``around`` in :meth:`history`.
+        oldest_first: Optional[:class:`bool`]
+            Same as ``oldest_first`` in :meth:`history`.
+        bulk: :class:`bool`
+            If ``True``, use bulk delete. Setting this to ``False`` is useful for mass-deleting
+            a bot's own messages without :attr:`Permissions.manage_messages`. When ``True``, will
+            fall back to single delete if messages are older than two weeks.
+
+        Raises
+        ------
+        Forbidden
+            You do not have proper permissions to do the actions required.
+        HTTPException
+            Purging the messages failed.
+
+        Returns
+        -------
+        List[:class:`.Message`]
+            A list of messages that were deleted.
+        """
+        if check is MISSING:
+            check = lambda m: True
+
+        iterator = self.history(
+            limit=limit, before=before, after=after, oldest_first=oldest_first, around=around
+        )
+        ret: List[Message] = []
+        count = 0
+
+        minimum_time = int((time.time() - 14 * 24 * 60 * 60) * 1000.0 - 1420070400000) << 22
+        strategy = self.delete_messages if bulk else _single_delete_strategy
+
+        async for message in iterator:
+            if count == 100:
+                to_delete = ret[-100:]
+                await strategy(to_delete)
+                count = 0
+                await asyncio.sleep(1)
+
+            if not check(message):
+                continue
+
+            if message.id < minimum_time:
+                # older than 14 days old
+                if count == 1:
+                    await ret[-1].delete()
+                elif count >= 2:
+                    to_delete = ret[-count:]
+                    await strategy(to_delete)
+
+                count = 0
+                strategy = _single_delete_strategy
+
+            count += 1
+            ret.append(message)
+
+        # SOme messages remaining to poll
+        if count >= 2:
+            # more than 2 messages -> bulk delete
+            to_delete = ret[-count:]
+            await strategy(to_delete)
+        elif count == 1:
+            # delete a single message
+            await ret[-1].delete()
+
+        return ret
+
+    async def webhooks(self) -> List[Webhook]:
+        """|coro|
+
+        Retrieves the list of webhooks this channel has.
+
+        You must have :attr:`~.Permissions.manage_webhooks` permission to
+        use this.
+
+        .. versionadded:: 2.9
+
+        Raises
+        ------
+        Forbidden
+            You don't have permissions to get the webhooks.
+
+        Returns
+        -------
+        List[:class:`Webhook`]
+            The list of webhooks this channel has.
+        """
+        from .webhook import Webhook
+
+        data = await self._state.http.channel_webhooks(self.id)
+        return [Webhook.from_state(d, state=self._state) for d in data]
+
+    async def create_webhook(
+        self, *, name: str, avatar: Optional[bytes] = None, reason: Optional[str] = None
+    ) -> Webhook:
+        """|coro|
+
+        Creates a webhook for this channel.
+
+        You must have :attr:`~.Permissions.manage_webhooks` permission to
+        do this.
+
+        .. versionadded:: 2.9
+
+        Parameters
+        ----------
+        name: :class:`str`
+            The webhook's name.
+        avatar: Optional[:class:`bytes`]
+            The webhook's default avatar.
+            This operates similarly to :meth:`~ClientUser.edit`.
+        reason: Optional[:class:`str`]
+            The reason for creating this webhook. Shows up in the audit logs.
+
+        Raises
+        ------
+        NotFound
+            The ``avatar`` asset couldn't be found.
+        Forbidden
+            You do not have permissions to create a webhook.
+        HTTPException
+            Creating the webhook failed.
+        TypeError
+            The ``avatar`` asset is a lottie sticker (see :func:`Sticker.read`).
+
+        Returns
+        -------
+        :class:`Webhook`
+            The newly created webhook.
+        """
+        from .webhook import Webhook
+
+        avatar_data = await utils._assetbytes_to_base64_data(avatar)
+
+        data = await self._state.http.create_webhook(
+            self.id, name=str(name), avatar=avatar_data, reason=reason
+        )
+        return Webhook.from_state(data, state=self._state)
+
 
 class CategoryChannel(disnake.abc.GuildChannel, Hashable):
     """Represents a Discord channel category.
 
     These are useful to group channels to logical compartments.
 
     .. container:: operations
@@ -2150,26 +2762,89 @@
     def type(self) -> Literal[ChannelType.category]:
         """:class:`ChannelType`: The channel's Discord type.
 
         This always returns :attr:`ChannelType.category`.
         """
         return ChannelType.category
 
+    @utils.copy_doc(disnake.abc.GuildChannel.permissions_for)
+    def permissions_for(
+        self,
+        obj: Union[Member, Role],
+        /,
+        *,
+        ignore_timeout: bool = MISSING,
+    ) -> Permissions:
+        base = super().permissions_for(obj, ignore_timeout=ignore_timeout)
+        self._apply_implict_permissions(base)
+
+        return base
+
     def is_nsfw(self) -> bool:
         """Whether the category is marked as NSFW.
 
         :return type: :class:`bool`
         """
         return self.nsfw
 
-    @utils.copy_doc(disnake.abc.GuildChannel.clone)
     async def clone(
-        self, *, name: Optional[str] = None, reason: Optional[str] = None
+        self,
+        *,
+        name: Optional[str] = None,
+        position: int = MISSING,
+        overwrites: Mapping[Union[Role, Member], PermissionOverwrite] = MISSING,
+        reason: Optional[str] = None,
     ) -> CategoryChannel:
-        return await self._clone_impl({"nsfw": self.nsfw}, name=name, reason=reason)
+        """|coro|
+
+        Clones this channel. This creates a channel with the same properties
+        as this channel.
+
+        You must have :attr:`.Permissions.manage_channels` permission to
+        do this.
+
+        .. versionchanged:: 2.9
+            Added ``position``, ``nsfw`` and ``overwrites`` keyword-only parameters.
+
+        .. note::
+            The current :attr:`CategoryChannel.flags` value won't be cloned.
+            This is a Discord limitation.
+
+        Parameters
+        ----------
+        name: Optional[:class:`str`]
+            The name of the new channel. If not provided, defaults to this channel's name.
+        position: :class:`int`
+            The position of the new channel. If not provided, defaults to this channel's position.
+        overwrites: :class:`Mapping`
+            A :class:`Mapping` of target (either a role or a member) to :class:`PermissionOverwrite`
+            to apply to the channel. If not provided, defaults to this channel's overwrites.
+        reason: Optional[:class:`str`]
+            The reason for cloning this channel. Shows up on the audit log.
+
+        Raises
+        ------
+        Forbidden
+            You do not have the proper permissions to create this channel.
+        HTTPException
+            Creating the channel failed.
+
+        Returns
+        -------
+        :class:`CategoryChannel`
+            The channel that was created.
+        """
+        return await self._clone_impl(
+            {
+                "position": position if position is not MISSING else self.position,
+            },
+            name=name,
+            reason=reason,
+            overwrites=overwrites,
+        )
 
     # if only these parameters are passed, `_move` is called and no channel will be returned
     @overload
     async def edit(
         self,
         *,
         position: int,
@@ -2642,14 +3317,15 @@
         self,
         obj: Union[Member, Role],
         /,
         *,
         ignore_timeout: bool = MISSING,
     ) -> Permissions:
         base = super().permissions_for(obj, ignore_timeout=ignore_timeout)
+        self._apply_implict_permissions(base)
 
         # forum channels do not have voice related permissions
         denied = Permissions.voice()
         base.value &= ~denied.value
         return base
 
     @property
@@ -2686,16 +3362,17 @@
         The default emoji shown for reacting to threads.
 
         Due to a Discord limitation, this will have an empty
         :attr:`~PartialEmoji.name` if it is a custom :class:`PartialEmoji`.
 
         .. versionadded:: 2.6
         """
-        return PartialEmoji._emoji_from_name_id(
-            self._default_reaction_emoji_name, self._default_reaction_emoji_id, state=self._state
+        return self._state._get_emoji_from_fields(
+            name=self._default_reaction_emoji_name,
+            id=self._default_reaction_emoji_id,
         )
 
     @property
     def last_thread(self) -> Optional[Thread]:
         """Gets the last created thread in this channel from the cache.
 
         The thread might not be valid or point to an existing thread.
@@ -2933,27 +3610,139 @@
             reason=reason,
             **kwargs,
         )
         if payload is not None:
             # the payload will always be the proper channel payload
             return self.__class__(state=self._state, guild=self.guild, data=payload)  # type: ignore
 
-    @utils.copy_doc(disnake.abc.GuildChannel.clone)
     async def clone(
-        self, *, name: Optional[str] = None, reason: Optional[str] = None
+        self,
+        *,
+        name: Optional[str] = None,
+        topic: Optional[str] = MISSING,
+        position: int = MISSING,
+        nsfw: bool = MISSING,
+        category: Optional[Snowflake] = MISSING,
+        slowmode_delay: Optional[int] = MISSING,
+        default_thread_slowmode_delay: Optional[int] = MISSING,
+        default_auto_archive_duration: Optional[AnyThreadArchiveDuration] = MISSING,
+        available_tags: Sequence[ForumTag] = MISSING,
+        default_reaction: Optional[Union[str, Emoji, PartialEmoji]] = MISSING,
+        default_sort_order: Optional[ThreadSortOrder] = MISSING,
+        overwrites: Mapping[Union[Role, Member], PermissionOverwrite] = MISSING,
+        reason: Optional[str] = None,
     ) -> ForumChannel:
+        """|coro|
+
+        Clones this channel. This creates a channel with the same properties
+        as this channel.
+
+        You must have :attr:`.Permissions.manage_channels` permission to
+        do this.
+
+        .. versionchanged:: 2.9
+            Added new ``topic``, ``position``, ``nsfw``, ``category``, ``slowmode_delay``,
+            ``default_thread_slowmode_delay``, ``default_auto_archive_duration``,
+            ``available_tags``, ``default_reaction``, ``default_sort_order``
+            and ``overwrites`` keyword-only paremters.
+
+        .. note::
+            The current :attr:`ForumChannel.flags` value won't be cloned.
+            This is a Discord limitation.
+
+        Parameters
+        ----------
+        name: Optional[:class:`str`]
+            The name of the new channel. If not provided, defaults to this channel's name.
+        topic: Optional[:class:`str`]
+            The topic of the new channel. If not provided, defaults to this channel's topic.
+        position: :class:`int`
+            The position of the new channel. If not provided, defaults to this channel's position.
+        nsfw: :class:`bool`
+            Whether the new channel should be nsfw or not. If not provided, defaults to this channel's NSFW value.
+        category: Optional[:class:`abc.Snowflake`]
+            The category where the new channel should be grouped. If not provided, defaults to this channel's category.
+        slowmode_delay: Optional[:class:`int`]
+            The slowmode delay of the new channel. If not provided, defaults to this channel's slowmode delay.
+        default_thread_slowmode_delay: Optional[:class:`int`]
+            The default thread slowmode delay of the new channel. If not provided, defaults to this channel's default thread slowmode delay.
+        default_auto_archive_duration: Optional[Union[:class:`int`, :class:`ThreadArchiveDuration`]]
+            The default auto archive duration of the new channel. If not provided, defaults to this channel's default auto archive duration.
+        available_tags: Sequence[:class:`ForumTag`]
+            The applicable tags of the new channel. If not provided, defaults to this channel's available tags.
+        default_reaction: Optional[Union[:class:`str`, :class:`Emoji`, :class:`PartialEmoji`]]
+            The default reaction of the new channel. If not provided, defaults to this channel's default reaction.
+        default_sort_order: Optional[:class:`ThreadSortOrder`]
+            The default sort order of the new channel. If not provided, defaults to this channel's default sort order.
+        overwrites: :class:`Mapping`
+            A :class:`Mapping` of target (either a role or a member) to :class:`PermissionOverwrite`
+            to apply to the channel. If not provided, defaults to this channel's overwrites.
+        reason: Optional[:class:`str`]
+            The reason for cloning this channel. Shows up on the audit log.
+
+        Raises
+        ------
+        Forbidden
+            You do not have the proper permissions to create this channel.
+        HTTPException
+            Creating the channel failed.
+
+        Returns
+        -------
+        :class:`ForumChannel`
+            The channel that was created.
+        """
+        default_reaction_emoji_payload: Optional[DefaultReactionPayload] = MISSING
+        if default_reaction is MISSING:
+            default_reaction = self.default_reaction
+
+        if default_reaction is not None:
+            emoji_name, emoji_id = PartialEmoji._emoji_to_name_id(default_reaction)
+            default_reaction_emoji_payload = {
+                "emoji_name": emoji_name,
+                "emoji_id": emoji_id,
+            }
+        else:
+            default_reaction_emoji_payload = None
+
+        if default_sort_order is MISSING:
+            default_sort_order = self.default_sort_order
+
         return await self._clone_impl(
             {
-                "topic": self.topic,
-                "nsfw": self.nsfw,
-                "rate_limit_per_user": self.slowmode_delay,
-                "default_auto_archive_duration": self.default_auto_archive_duration,
+                "topic": topic if topic is not MISSING else self.topic,
+                "position": position if position is not MISSING else self.position,
+                "nsfw": nsfw if nsfw is not MISSING else self.nsfw,
+                "rate_limit_per_user": (
+                    slowmode_delay if slowmode_delay is not MISSING else self.slowmode_delay
+                ),
+                "default_thread_rate_limit_per_user": (
+                    default_thread_slowmode_delay
+                    if default_thread_slowmode_delay is not MISSING
+                    else self.default_thread_slowmode_delay
+                ),
+                "default_auto_archive_duration": (
+                    try_enum_to_int(default_auto_archive_duration)
+                    if default_auto_archive_duration is not MISSING
+                    else self.default_auto_archive_duration
+                ),
+                "available_tags": (
+                    [tag.to_dict() for tag in available_tags]
+                    if available_tags is not MISSING
+                    else [tag.to_dict() for tag in self.available_tags]
+                ),
+                "default_reaction_emoji": default_reaction_emoji_payload,
+                "default_sort_order": (
+                    try_enum_to_int(default_sort_order) if default_sort_order is not None else None
+                ),
             },
             name=name,
+            category=category,
             reason=reason,
+            overwrites=overwrites,
         )
 
     def get_thread(self, thread_id: int, /) -> Optional[Thread]:
         """Returns a thread with the given ID.
 
         Parameters
         ----------
@@ -2975,14 +3764,15 @@
         auto_archive_duration: AnyThreadArchiveDuration = ...,
         slowmode_delay: Optional[int] = ...,
         applied_tags: Sequence[Snowflake] = ...,
         content: str = ...,
         embed: Embed = ...,
         file: File = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
         allowed_mentions: AllowedMentions = ...,
         view: View = ...,
         components: Components = ...,
         reason: Optional[str] = None,
     ) -> ThreadWithMessage:
         ...
@@ -2995,14 +3785,15 @@
         auto_archive_duration: AnyThreadArchiveDuration = ...,
         slowmode_delay: Optional[int] = ...,
         applied_tags: Sequence[Snowflake] = ...,
         content: str = ...,
         embed: Embed = ...,
         files: List[File] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
         allowed_mentions: AllowedMentions = ...,
         view: View = ...,
         components: Components = ...,
         reason: Optional[str] = None,
     ) -> ThreadWithMessage:
         ...
@@ -3015,14 +3806,15 @@
         auto_archive_duration: AnyThreadArchiveDuration = ...,
         slowmode_delay: Optional[int] = ...,
         applied_tags: Sequence[Snowflake] = ...,
         content: str = ...,
         embeds: List[Embed] = ...,
         file: File = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
         allowed_mentions: AllowedMentions = ...,
         view: View = ...,
         components: Components = ...,
         reason: Optional[str] = None,
     ) -> ThreadWithMessage:
         ...
@@ -3035,14 +3827,15 @@
         auto_archive_duration: AnyThreadArchiveDuration = ...,
         slowmode_delay: Optional[int] = ...,
         applied_tags: Sequence[Snowflake] = ...,
         content: str = ...,
         embeds: List[Embed] = ...,
         files: List[File] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
         allowed_mentions: AllowedMentions = ...,
         view: View = ...,
         components: Components = ...,
         reason: Optional[str] = None,
     ) -> ThreadWithMessage:
         ...
@@ -3056,14 +3849,15 @@
         applied_tags: Sequence[Snowflake] = MISSING,
         content: str = MISSING,
         embed: Embed = MISSING,
         embeds: List[Embed] = MISSING,
         file: File = MISSING,
         files: List[File] = MISSING,
         suppress_embeds: bool = MISSING,
+        flags: MessageFlags = MISSING,
         stickers: Sequence[Union[GuildSticker, StickerItem]] = MISSING,
         allowed_mentions: AllowedMentions = MISSING,
         view: View = MISSING,
         components: Components[MessageUIComponent] = MISSING,
         reason: Optional[str] = None,
     ) -> ThreadWithMessage:
         """|coro|
@@ -3106,14 +3900,23 @@
             ``embeds`` parameter.
         embeds: List[:class:`.Embed`]
             A list of embeds to send with the content. Must be a maximum of 10.
             This cannot be mixed with the ``embed`` parameter.
         suppress_embeds: :class:`bool`
             Whether to suppress embeds for the message. This hides
             all the embeds from the UI if set to ``True``.
+        flags: :class:`MessageFlags`
+            The flags to set for this message.
+            Only :attr:`~MessageFlags.suppress_embeds` is supported.
+
+            If parameter ``suppress_embeds`` is provided,
+            that will override the setting of :attr:`MessageFlags.suppress_embeds`.
+
+            .. versionadded:: 2.9
+
         file: :class:`.File`
             The file to upload. This cannot be mixed with the ``files`` parameter.
         files: List[:class:`.File`]
             A list of files to upload. Must be a maximum of 10.
             This cannot be mixed with the ``file`` parameter.
         stickers: Sequence[Union[:class:`.GuildSticker`, :class:`.StickerItem`]]
             A list of stickers to upload. Must be a maximum of 3.
@@ -3159,14 +3962,15 @@
         params = handle_message_parameters_dict(
             content,
             embed=embed,
             embeds=embeds,
             file=file,
             files=files,
             suppress_embeds=suppress_embeds,
+            flags=flags,
             view=view,
             components=components,
             allowed_mentions=allowed_mentions,
             stickers=stickers,
         )
 
         if auto_archive_duration is not None:
@@ -3234,15 +4038,15 @@
         ------
         Forbidden
             You do not have permissions to get archived threads.
         HTTPException
             The request to get the archived threads failed.
 
         Yields
-        -------
+        ------
         :class:`Thread`
             The archived threads.
         """
         return ArchivedThreadIterator(
             self.id, self.guild, limit=limit, joined=False, private=False, before=before
         )
 
@@ -3446,16 +4250,15 @@
     @property
     def created_at(self) -> datetime.datetime:
         """:class:`datetime.datetime`: Returns the direct message channel's creation time in UTC."""
         return utils.snowflake_time(self.id)
 
     @property
     def jump_url(self) -> str:
-        """
-        A URL that can be used to jump to this channel.
+        """A URL that can be used to jump to this channel.
 
         .. versionadded:: 2.4
         """
         return f"https://discord.com/channels/@me/{self.id}"
 
     @property
     def flags(self) -> ChannelFlags:
```

### Comparing `disnake-2.8.2/disnake/client.py` & `disnake-2.9.0/disnake/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,16 +179,15 @@
         return (
             f"<SessionStartLimit total={self.total!r} remaining={self.remaining!r} "
             f"reset_after={self.reset_after!r} max_concurrency={self.max_concurrency!r} reset_time={self.reset_time!s}>"
         )
 
 
 class GatewayParams(NamedTuple):
-    """
-    Container type for configuring gateway connections.
+    """Container type for configuring gateway connections.
 
     .. versionadded:: 2.6
 
     Parameters
     ----------
     encoding: :class:`str`
         The payload encoding (``json`` is currently the only supported encoding).
@@ -199,16 +198,15 @@
     """
 
     encoding: Literal["json"] = "json"
     zlib: bool = True
 
 
 class Client:
-    """
-    Represents a client connection that connects to Discord.
+    """Represents a client connection that connects to Discord.
     This class is used to interact with the Discord WebSocket and API.
 
     A number of options can be passed to the :class:`Client`.
 
     Parameters
     ----------
     max_messages: Optional[:class:`int`]
@@ -1379,16 +1377,15 @@
         List[Union[:class:`.APIUserCommand`, :class:`.APIMessageCommand`, :class:`.APISlashCommand`]]
             The list of application commands.
         """
         data = self._connection._guild_application_commands.get(guild_id, {})
         return list(data.values())
 
     def get_guild_slash_commands(self, guild_id: int) -> List[APISlashCommand]:
-        """
-        Returns a list of all slash commands in the guild with the given ID.
+        """Returns a list of all slash commands in the guild with the given ID.
 
         Parameters
         ----------
         guild_id: :class:`int`
             The ID to search for.
 
         Returns
@@ -1396,16 +1393,15 @@
         List[:class:`.APISlashCommand`]
             The list of slash commands.
         """
         data = self._connection._guild_application_commands.get(guild_id, {})
         return [cmd for cmd in data.values() if isinstance(cmd, APISlashCommand)]
 
     def get_guild_user_commands(self, guild_id: int) -> List[APIUserCommand]:
-        """
-        Returns a list of all user commands in the guild with the given ID.
+        """Returns a list of all user commands in the guild with the given ID.
 
         Parameters
         ----------
         guild_id: :class:`int`
             The ID to search for.
 
         Returns
@@ -1413,16 +1409,15 @@
         List[:class:`.APIUserCommand`]
             The list of user commands.
         """
         data = self._connection._guild_application_commands.get(guild_id, {})
         return [cmd for cmd in data.values() if isinstance(cmd, APIUserCommand)]
 
     def get_guild_message_commands(self, guild_id: int) -> List[APIMessageCommand]:
-        """
-        Returns a list of all message commands in the guild with the given ID.
+        """Returns a list of all message commands in the guild with the given ID.
 
         Parameters
         ----------
         guild_id: :class:`int`
             The ID to search for.
 
         Returns
@@ -1430,32 +1425,30 @@
         List[:class:`.APIMessageCommand`]
             The list of message commands.
         """
         data = self._connection._guild_application_commands.get(guild_id, {})
         return [cmd for cmd in data.values() if isinstance(cmd, APIMessageCommand)]
 
     def get_global_command(self, id: int) -> Optional[APIApplicationCommand]:
-        """
-        Returns a global application command with the given ID.
+        """Returns a global application command with the given ID.
 
         Parameters
         ----------
         id: :class:`int`
             The ID to search for.
 
         Returns
         -------
         Optional[Union[:class:`.APIUserCommand`, :class:`.APIMessageCommand`, :class:`.APISlashCommand`]]
             The application command.
         """
         return self._connection._get_global_application_command(id)
 
     def get_guild_command(self, guild_id: int, id: int) -> Optional[APIApplicationCommand]:
-        """
-        Returns a guild application command with the given guild ID and application command ID.
+        """Returns a guild application command with the given guild ID and application command ID.
 
         Parameters
         ----------
         guild_id: :class:`int`
             The guild ID to search for.
         id: :class:`int`
             The command ID to search for.
@@ -1466,16 +1459,15 @@
             The application command.
         """
         return self._connection._get_guild_application_command(guild_id, id)
 
     def get_global_command_named(
         self, name: str, cmd_type: Optional[ApplicationCommandType] = None
     ) -> Optional[APIApplicationCommand]:
-        """
-        Returns a global application command matching the given name.
+        """Returns a global application command matching the given name.
 
         Parameters
         ----------
         name: :class:`str`
             The name to look for.
         cmd_type: :class:`.ApplicationCommandType`
             The type to look for. By default, no types are checked.
@@ -1486,16 +1478,15 @@
             The application command.
         """
         return self._connection._get_global_command_named(name, cmd_type)
 
     def get_guild_command_named(
         self, guild_id: int, name: str, cmd_type: Optional[ApplicationCommandType] = None
     ) -> Optional[APIApplicationCommand]:
-        """
-        Returns a guild application command matching the given name.
+        """Returns a guild application command matching the given name.
 
         Parameters
         ----------
         guild_id: :class:`int`
             The guild ID to search for.
         name: :class:`str`
             The command name to search for.
@@ -1543,22 +1534,21 @@
         The ``timeout`` parameter is passed onto :func:`asyncio.wait_for`. By default,
         it does not timeout. Note that this does propagate the
         :exc:`asyncio.TimeoutError` for you in case of timeout and is provided for
         ease of use.
 
         In case the event returns multiple arguments, a :class:`tuple` containing those
         arguments is returned instead. Please check the
-        :ref:`documentation <discord-api-events>` for a list of events and their
+        :ref:`documentation <disnake_api_events>` for a list of events and their
         parameters.
 
         This function returns the **first event that meets the requirements**.
 
         Examples
         --------
-
         Waiting for a user reply: ::
 
             @client.event
             async def on_message(message):
                 if message.content.startswith('$greet'):
                     channel = message.channel
                     await channel.send('Say hello!')
@@ -1600,15 +1590,15 @@
                     else:
                         await channel.send('\N{THUMBS UP SIGN}')
 
 
         Parameters
         ----------
         event: Union[:class:`str`, :class:`.Event`]
-            The event name, similar to the :ref:`event reference <discord-api-events>`,
+            The event name, similar to the :ref:`event reference <disnake_api_events>`,
             but without the ``on_`` prefix, to wait for. It's recommended
             to use :class:`.Event`.
         check: Optional[Callable[..., :class:`bool`]]
             A predicate to check what to wait for. The arguments must meet the
             parameters of the event being waited for.
         timeout: Optional[:class:`float`]
             The number of seconds to wait before timing out and raising
@@ -1620,15 +1610,15 @@
             If a timeout is provided and it was reached.
 
         Returns
         -------
         Any
             Returns no arguments, a single argument, or a :class:`tuple` of multiple
             arguments that mirrors the parameters passed in the
-            :ref:`event reference <discord-api-events>`.
+            :ref:`event <disnake_api_events>`.
         """
         future = self.loop.create_future()
         if check is None:
 
             def _check(*args) -> bool:
                 return True
 
@@ -1645,21 +1635,20 @@
         return asyncio.wait_for(future, timeout)
 
     # event registration
 
     def event(self, coro: CoroT) -> CoroT:
         """A decorator that registers an event to listen to.
 
-        You can find more info about the events on the :ref:`documentation below <discord-api-events>`.
+        You can find more info about the events in the :ref:`documentation <disnake_api_events>`.
 
         The events must be a :ref:`coroutine <coroutine>`, if not, :exc:`TypeError` is raised.
 
         Example
-        ---------
-
+        -------
         .. code-block:: python3
 
             @client.event
             async def on_ready():
                 print('Ready!')
 
         Raises
@@ -1680,28 +1669,28 @@
         activity: Optional[BaseActivity] = None,
         status: Optional[Status] = None,
     ) -> None:
         """|coro|
 
         Changes the client's presence.
 
+        .. versionchanged:: 2.0
+            Removed the ``afk`` keyword-only parameter.
+
         .. versionchanged:: 2.6
             Raises :exc:`TypeError` instead of ``InvalidArgument``.
 
         Example
         ---------
 
         .. code-block:: python3
 
             game = disnake.Game("with the API")
             await client.change_presence(status=disnake.Status.idle, activity=game)
 
-        .. versionchanged:: 2.0
-            Removed the ``afk`` keyword-only parameter.
-
         Parameters
         ----------
         activity: Optional[:class:`.BaseActivity`]
             The activity being done. ``None`` if no currently active activity is done.
         status: Optional[:class:`.Status`]
             Indicates what status to change to. If ``None``, then
             :attr:`.Status.online` is used.
@@ -1752,15 +1741,14 @@
 
         .. note::
 
             This method is an API call. For general usage, consider :attr:`guilds` instead.
 
         Examples
         --------
-
         Usage ::
 
             async for guild in client.fetch_guilds(limit=150):
                 print(guild.name)
 
         Flattening into a list ::
 
@@ -1787,15 +1775,15 @@
 
         Raises
         ------
         HTTPException
             Retrieving the guilds failed.
 
         Yields
-        --------
+        ------
         :class:`.Guild`
             The guild with the guild data parsed.
         """
         return GuildIterator(self, limit=limit, before=before, after=after)
 
     async def fetch_template(self, code: Union[Template, str]) -> Template:
         """|coro|
@@ -1902,14 +1890,19 @@
 
         Creates a :class:`.Guild`.
 
         See :func:`guild_builder` for a more comprehensive alternative.
 
         Bot accounts in 10 or more guilds are not allowed to create guilds.
 
+        .. note::
+
+            Using this, you will **not** receive :attr:`.Guild.channels`, :attr:`.Guild.members`,
+            :attr:`.Member.activity` and :attr:`.Member.voice` per :class:`.Member`.
+
         .. versionchanged:: 2.5
             Removed the ``region`` parameter.
 
         .. versionchanged:: 2.6
             Raises :exc:`ValueError` instead of ``InvalidArgument``.
 
         Parameters
@@ -1959,14 +1952,19 @@
         """Creates a builder object that can be used to create more complex guilds.
 
         This is a more comprehensive alternative to :func:`create_guild`.
         See :class:`.GuildBuilder` for details and examples.
 
         Bot accounts in 10 or more guilds are not allowed to create guilds.
 
+        .. note::
+
+            Using this, you will **not** receive :attr:`.Guild.channels`, :attr:`.Guild.members`,
+            :attr:`.Member.activity` and :attr:`.Member.voice` per :class:`.Member`.
+
         .. versionadded:: 2.8
 
         Parameters
         ----------
         name: :class:`str`
             The name of the guild.
```

### Comparing `disnake-2.8.2/disnake/colour.py` & `disnake-2.9.0/disnake/colour.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/components.py` & `disnake-2.9.0/disnake/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,17 +145,17 @@
         self.type: ComponentType = try_enum(ComponentType, data["type"])
         self.children: List[ComponentT] = [
             _component_factory(d) for d in data.get("components", [])
         ]
 
     def to_dict(self) -> ActionRowPayload:
         return {
-            "type": int(self.type),
+            "type": self.type.value,
             "components": [child.to_dict() for child in self.children],
-        }  # type: ignore
+        }
 
 
 class Button(Component):
     """Represents a button from the Discord Bot UI Kit.
 
     This inherits from :class:`Component`.
```

### Comparing `disnake-2.8.2/disnake/context_managers.py` & `disnake-2.9.0/disnake/context_managers.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/embeds.py` & `disnake-2.9.0/disnake/embeds.py`

 * *Files 0% similar despite different names*

```diff
@@ -727,27 +727,26 @@
             An invalid index was provided.
         """
         if not self._fields:
             raise IndexError("field index out of range")
         try:
             self._fields[index]
         except IndexError:
-            raise IndexError("field index out of range")
+            raise IndexError("field index out of range") from None
 
         field: EmbedFieldPayload = {
             "inline": inline,
             "name": str(name),
             "value": str(value),
         }
         self._fields[index] = field
         return self
 
     def to_dict(self) -> EmbedData:
         """Converts this embed object into a dict."""
-
         # add in the raw data into the dict
         result: EmbedData = {}
         if self._footer is not None:
             result["footer"] = self._footer
         if self._image is not None:
             result["image"] = self._image
         if self._thumbnail is not None:
@@ -781,16 +780,15 @@
         if self.title:
             result["title"] = self.title
 
         return result
 
     @classmethod
     def set_default_colour(cls, value: Optional[Union[int, Colour]]):
-        """
-        Set the default colour of all new embeds.
+        """Set the default colour of all new embeds.
 
         .. versionadded:: 2.4
 
         Returns
         -------
         Optional[:class:`Colour`]
             The colour that was set.
@@ -805,16 +803,15 @@
             )
         return cls._default_colour
 
     set_default_color = set_default_colour
 
     @classmethod
     def get_default_colour(cls) -> Optional[Colour]:
-        """
-        Get the default colour of all new embeds.
+        """Get the default colour of all new embeds.
 
         .. versionadded:: 2.4
 
         Returns
         -------
         Optional[:class:`Colour`]
             The default colour.
@@ -834,16 +831,15 @@
             self._files[key] = file
             return f"attachment://{file.filename}"
         else:
             self._files.pop(key, None)
             return str(url) if url is not None else None
 
     def check_limits(self) -> None:
-        """
-        Checks if this embed fits within the limits dictated by Discord.
+        """Checks if this embed fits within the limits dictated by Discord.
         There is also a 6000 character limit across all embeds in a message.
 
         Returns nothing on success, raises :exc:`ValueError` if an attribute exceeds the limits.
 
         +--------------------------+------------------------------------+
         |   Field                  |              Limit                 |
         +--------------------------+------------------------------------+
@@ -865,15 +861,14 @@
         .. versionadded:: 2.6
 
         Raises
         ------
         ValueError
             One or more of the embed attributes are too long.
         """
-
         if self.title and len(self.title.strip()) > 256:
             raise ValueError("Embed title cannot be longer than 256 characters")
 
         if self.description and len(self.description.strip()) > 4096:
             raise ValueError("Embed description cannot be longer than 4096 characters")
 
         if self._footer and len(self._footer.get("text", "").strip()) > 2048:
```

### Comparing `disnake-2.8.2/disnake/emoji.py` & `disnake-2.9.0/disnake/emoji.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,16 +64,17 @@
     managed: :class:`bool`
         Whether the emoji is managed by a Twitch integration.
     guild_id: :class:`int`
         The guild ID the emoji belongs to.
     available: :class:`bool`
         Whether the emoji is available for use.
     user: Optional[:class:`User`]
-        The user that created the emoji. This can only be retrieved using :meth:`Guild.fetch_emoji` and
-        having :attr:`~Permissions.manage_emojis` permission.
+        The user that created this emoji. This can only be retrieved using
+        :meth:`Guild.fetch_emoji`/:meth:`Guild.fetch_emojis` while
+        having the :attr:`~Permissions.manage_guild_expressions` permission.
     """
 
     __slots__: Tuple[str, ...] = (
         "require_colons",
         "animated",
         "managed",
         "id",
@@ -141,14 +142,17 @@
         return f"{Asset.BASE}/emojis/{self.id}.{fmt}"
 
     @property
     def roles(self) -> List[Role]:
         """List[:class:`Role`]: A :class:`list` of roles that are allowed to use this emoji.
 
         If roles is empty, the emoji is unrestricted.
+
+        Emojis with :attr:`subscription roles <RoleTags.integration_id>` are considered premium emojis,
+        and count towards a separate limit of 25 emojis.
         """
         guild = self.guild
         if guild is None:
             return []
 
         return [role for role in guild.roles if self._roles.has(role.id)]
 
@@ -173,15 +177,15 @@
         return any(my_roles.has(role_id) for role_id in emoji_roles)
 
     async def delete(self, *, reason: Optional[str] = None) -> None:
         """|coro|
 
         Deletes the custom emoji.
 
-        You must have :attr:`~Permissions.manage_emojis` permission to
+        You must have :attr:`~Permissions.manage_guild_expressions` permission to
         do this.
 
         Parameters
         ----------
         reason: Optional[:class:`str`]
             The reason for deleting this emoji. Shows up on the audit log.
 
@@ -193,31 +197,34 @@
             An error occurred deleting the emoji.
         """
         await self._state.http.delete_custom_emoji(self.guild.id, self.id, reason=reason)
 
     async def edit(
         self, *, name: str = MISSING, roles: List[Snowflake] = MISSING, reason: Optional[str] = None
     ) -> Emoji:
-        """
-        |coro|
+        """|coro|
 
         Edits the custom emoji.
 
-        You must have :attr:`~Permissions.manage_emojis` permission to
+        You must have :attr:`~Permissions.manage_guild_expressions` permission to
         do this.
 
         .. versionchanged:: 2.0
             The newly updated emoji is returned.
 
         Parameters
         ----------
         name: :class:`str`
             The new emoji name.
         roles: Optional[List[:class:`~disnake.abc.Snowflake`]]
             A list of roles that can use this emoji. An empty list can be passed to make it available to everyone.
+
+            An emoji cannot have both subscription roles (see :attr:`RoleTags.integration_id`) and
+            non-subscription roles, and emojis can't be converted between premium and non-premium
+            after creation.
         reason: Optional[:class:`str`]
             The reason for editing this emoji. Shows up on the audit log.
 
         Raises
         ------
         Forbidden
             You are not allowed to edit emojis.
```

### Comparing `disnake-2.8.2/disnake/enums.py` & `disnake-2.9.0/disnake/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # SPDX-License-Identifier: MIT
+from __future__ import annotations
 
 import types
 from functools import total_ordering
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Dict,
+    Iterator,
     List,
     NamedTuple,
     NoReturn,
     Optional,
     Type,
     TypeVar,
 )
 
+if TYPE_CHECKING:
+    from typing_extensions import Self
+
 __all__ = (
     "Enum",
     "ChannelType",
     "MessageType",
     "SpeakingState",
     "VerificationLevel",
     "ContentFilter",
@@ -57,14 +62,15 @@
     "AutoModTriggerType",
     "AutoModEventType",
     "AutoModActionType",
     "ThreadSortOrder",
     "ThreadLayout",
     "Event",
     "ApplicationRoleConnectionMetadataType",
+    "OnboardingPromptType",
 )
 
 
 class _EnumValueBase(NamedTuple):
     if TYPE_CHECKING:
         _cls_name: ClassVar[str]
 
@@ -99,15 +105,15 @@
 class EnumMeta(type):
     if TYPE_CHECKING:
         __name__: ClassVar[str]
         _enum_member_names_: ClassVar[List[str]]
         _enum_member_map_: ClassVar[Dict[str, Any]]
         _enum_value_map_: ClassVar[Dict[Any, Any]]
 
-    def __new__(cls, name, bases, attrs, *, comparable: bool = False):
+    def __new__(cls, name: str, bases, attrs, *, comparable: bool = False):
         value_mapping = {}
         member_mapping = {}
         member_names = []
 
         value_cls = _create_value_cls(name, comparable)
         for key, value in list(attrs.items()):
             is_descriptor = _is_descriptor(value)
@@ -137,18 +143,18 @@
         attrs["_enum_member_map_"] = member_mapping
         attrs["_enum_member_names_"] = member_names
         attrs["_enum_value_cls_"] = value_cls
         actual_cls = super().__new__(cls, name, bases, attrs)
         value_cls._actual_enum_cls_ = actual_cls  # type: ignore
         return actual_cls
 
-    def __iter__(cls):
+    def __iter__(cls) -> Iterator[Self]:
         return (cls._enum_member_map_[name] for name in cls._enum_member_names_)
 
-    def __reversed__(cls):
+    def __reversed__(cls) -> Iterator[Self]:
         return (cls._enum_member_map_[name] for name in reversed(cls._enum_member_names_))
 
     def __len__(cls) -> int:
         return len(cls._enum_member_names_)
 
     def __repr__(cls) -> str:
         return f"<enum {cls.__name__}>"
@@ -157,20 +163,20 @@
     def __members__(cls):
         return types.MappingProxyType(cls._enum_member_map_)
 
     def __call__(cls, value):
         try:
             return cls._enum_value_map_[value]
         except (KeyError, TypeError):
-            raise ValueError(f"{value!r} is not a valid {cls.__name__}")
+            raise ValueError(f"{value!r} is not a valid {cls.__name__}") from None
 
     def __getitem__(cls, key):
         return cls._enum_member_map_[key]
 
-    def __setattr__(cls, name, value) -> NoReturn:
+    def __setattr__(cls, name: str, value) -> NoReturn:
         raise TypeError("Enums are immutable.")
 
     def __delattr__(cls, attr) -> NoReturn:
         raise TypeError("Enums are immutable")
 
     def __instancecheck__(self, instance) -> bool:
         # isinstance(x, Y)
@@ -234,15 +240,20 @@
     thread_created = 18
     reply = 19
     application_command = 20
     thread_starter_message = 21
     guild_invite_reminder = 22
     context_menu_command = 23
     auto_moderation_action = 24
+    role_subscription_purchase = 25
     interaction_premium_upsell = 26
+    stage_start = 27
+    stage_end = 28
+    stage_speaker = 29
+    stage_topic = 31
     guild_application_premium_subscription = 32
 
 
 class PartyType(Enum):
     poker = 755827207812677713
     betrayal = 773336526917861400
     fishing = 814288819477020702
@@ -251,14 +262,15 @@
     word_snack = 879863976006127627
     doodle_crew = 878067389634314250
     checkers = 832013003968348200
     spellcast = 852509694341283871
     watch_together = 880218394199220334
     sketch_heads = 902271654783242291
     ocho = 832025144389533716
+    gartic_phone = 1007373802981822582
 
 
 class SpeakingState(Enum):
     none = 0
     voice = 1 << 0
     soundshare = 1 << 1
     priority = 1 << 2
@@ -306,14 +318,15 @@
 class DefaultAvatar(Enum):
     blurple = 0
     grey = 1
     gray = 1
     green = 2
     orange = 3
     red = 4
+    fuchsia = 5
 
     def __str__(self) -> str:
         return self.name
 
 
 class NotificationLevel(Enum, comparable=True):
     all_messages = 0
@@ -730,23 +743,23 @@
     def __str__(self) -> str:
         return self.value
 
 
 # reference: https://discord.com/developers/docs/reference#locales
 class Locale(Enum):
     bg = "bg"
-    "Bulgarian | български"
+    "Bulgarian | български"  # noqa: RUF001
     cs = "cs"
     "Czech | Čeština"
     da = "da"
     "Danish | Dansk"
     de = "de"
     "German | Deutsch"
     el = "el"
-    "Greek | Ελληνικά"
+    "Greek | Ελληνικά"  # noqa: RUF001
     en_GB = "en-GB"
     "English, UK | English, UK"
     en_US = "en-US"
     "English, US | English, US"
     es_ES = "es-ES"
     "Spanish | Español"
     fi = "fi"
@@ -776,23 +789,23 @@
     pl = "pl"
     "Polish | Polski"
     pt_BR = "pt-BR"
     "Portuguese, Brazilian | Português do Brasil"
     ro = "ro"
     "Romanian, Romania | Română"
     ru = "ru"
-    "Russian | Pусский"
+    "Russian | Pусский"  # noqa: RUF001
     sv_SE = "sv-SE"
     "Swedish | Svenska"
     th = "th"
     "Thai | ไทย"
     tr = "tr"
     "Turkish | Türkçe"
     uk = "uk"
-    "Ukrainian | Українська"
+    "Ukrainian | Українська"  # noqa: RUF001
     vi = "vi"
     "Vietnamese | Tiếng Việt"
     zh_CN = "zh-CN"
     "Chinese, China | 中文"
     zh_TW = "zh-TW"
     "Chinese, Taiwan | 繁體中文"
 
@@ -808,15 +821,16 @@
 
 class AutoModEventType(Enum):
     message_send = 1
 
 
 class AutoModTriggerType(Enum):
     keyword = 1
-    harmful_link = 2
+    if not TYPE_CHECKING:
+        harmful_link = 2  # obsolete/deprecated
     spam = 3
     keyword_preset = 4
     mention_spam = 5
 
 
 class ThreadSortOrder(Enum):
     latest_activity = 0
@@ -826,16 +840,15 @@
 class ThreadLayout(Enum):
     not_set = 0
     list_view = 1
     gallery_view = 2
 
 
 class Event(Enum):
-    """
-    Represents all the events of the library.
+    """Represents all the events of the library.
 
     These offer to register listeners/events in a more pythonic way; additionally autocompletion and documentation are both supported.
 
     .. versionadded:: 2.8
 
     """
 
@@ -987,22 +1000,22 @@
     """Called when a guild becomes unavailable.
     Represents the :func:`on_guild_unavailable` event.
     """
     guild_role_create = "guild_role_create"
     """Called when a `Guild` creates a new `Role`.
     Represents the :func:`on_guild_role_create` event.
     """
-    guild_role_update = "guild_role_update"
-    """Called when a `Guild` updates a `Role`.
-    Represents the :func:`on_guild_role_update` event.
-    """
     guild_role_delete = "guild_role_delete"
     """Called when a `Guild` deletes a `Role`.
     Represents the :func:`on_guild_role_delete` event.
     """
+    guild_role_update = "guild_role_update"
+    """Called when a `Guild` updates a `Role`.
+    Represents the :func:`on_guild_role_update` event.
+    """
     guild_emojis_update = "guild_emojis_update"
     """Called when a `Guild` adds or removes `Emoji`.
     Represents the :func:`on_guild_emojis_update` event.
     """
     guild_stickers_update = "guild_stickers_update"
     """Called when a `Guild` updates its stickers.
     Represents the :func:`on_guild_stickers_update` event.
@@ -1055,14 +1068,18 @@
     """Called when an `AutoModRule` is updated.
     Represents the :func:`on_automod_rule_update` event.
     """
     automod_rule_delete = "automod_rule_delete"
     """Called when an `AutoModRule` is deleted.
     Represents the :func:`on_automod_rule_delete` event.
     """
+    audit_log_entry_create = "audit_log_entry_create"
+    """Called when an audit log entry is created.
+    Represents the :func:`on_audit_log_entry_create` event.
+    """
     integration_create = "integration_create"
     """Called when an integration is created.
     Represents the :func:`on_integration_create` event.
     """
     integration_update = "integration_update"
     """Called when an integration is updated.
     Represents the :func:`on_integration_update` event.
@@ -1071,34 +1088,30 @@
     """Called when an integration is deleted.
     Represents the :func:`on_raw_integration_delete` event.
     """
     member_join = "member_join"
     """Called when a `Member` joins a `Guild`.
     Represents the :func:`on_member_join` event.
     """
-    member_update = "member_update"
-    """Called when a `Member` updates their profile.
-    Represents the :func:`on_member_update` event.
-    """
     member_remove = "member_remove"
     """Called when a `Member` leaves a `Guild`.
     Represents the :func:`on_member_remove` event.
     """
+    member_update = "member_update"
+    """Called when a `Member` is updated in a `Guild`.
+    Represents the :func:`on_member_update` event.
+    """
     raw_member_remove = "raw_member_remove"
     """Called when a member leaves a `Guild` regardless of the member cache.
     Represents the :func:`on_raw_member_remove` event.
     """
     raw_member_update = "raw_member_update"
-    """Called when a member updates their profile regardless of the member cache.
+    """Called when a `Member` is updated in a `Guild` regardless of the member cache.
     Represents the :func:`on_raw_member_update` event.
     """
-    audit_log_entry_create = "audit_log_entry_create"
-    """Called when an audit log entry is created.
-    Represents the :func:`on_audit_log_entry_create` event.
-    """
     member_ban = "member_ban"
     """Called when user gets banned from a `Guild`.
     Represents the :func:`on_member_ban` event.
     """
     member_unban = "member_unban"
     """Called when a `User` gets unbanned from a `Guild`.
     Represents the :func:`on_member_unban` event.
@@ -1115,22 +1128,22 @@
     """Called when a `Member` changes their `VoiceState`.
     Represents the :func:`on_voice_state_update` event.
     """
     stage_instance_create = "stage_instance_create"
     """Called when a `StageInstance` is created for a `StageChannel`.
     Represents the :func:`on_stage_instance_create` event.
     """
-    stage_instance_update = "stage_instance_update"
-    """Called when a `StageInstance` is updated.
-    Represents the :func:`on_stage_instance_update` event.
-    """
     stage_instance_delete = "stage_instance_delete"
     """Called when a `StageInstance` is deleted for a `StageChannel`.
     Represents the :func:`on_stage_instance_delete` event.
     """
+    stage_instance_update = "stage_instance_update"
+    """Called when a `StageInstance` is updated.
+    Represents the :func:`on_stage_instance_update` event.
+    """
     application_command = "application_command"
     """Called when an application command is invoked.
     Represents the :func:`on_application_command` event.
     """
     application_command_autocomplete = "application_command_autocomplete"
     """Called when an application command autocomplete is called.
     Represents the :func:`on_application_command_autocomplete` event.
@@ -1167,22 +1180,22 @@
     """Called when a message is deleted.
     Represents the :func:`on_message_delete` event.
     """
     bulk_message_delete = "bulk_message_delete"
     """Called when messages are bulk deleted.
     Represents the :func:`on_bulk_message_delete` event.
     """
-    raw_message_delete = "raw_message_delete"
-    """Called when a message is deleted regardless of the message being in the internal message cache or not.
-    Represents the :func:`on_raw_message_delete` event.
-    """
     raw_message_edit = "raw_message_edit"
     """Called when a message is edited regardless of the state of the internal message cache.
     Represents the :func:`on_raw_message_edit` event.
     """
+    raw_message_delete = "raw_message_delete"
+    """Called when a message is deleted regardless of the message being in the internal message cache or not.
+    Represents the :func:`on_raw_message_delete` event.
+    """
     raw_bulk_message_delete = "raw_bulk_message_delete"
     """Called when a bulk delete is triggered regardless of the messages being in the internal message cache or not.
     Represents the :func:`on_raw_bulk_message_delete` event.
     """
     reaction_add = "reaction_add"
     """Called when a message has a reaction added to it.
     Represents the :func:`on_reaction_add` event.
@@ -1281,29 +1294,33 @@
     integer_not_equal = 4
     datetime_less_than_or_equal = 5
     datetime_greater_than_or_equal = 6
     boolean_equal = 7
     boolean_not_equal = 8
 
 
+class OnboardingPromptType(Enum):
+    multiple_choice = 0
+    dropdown = 1
+
+
 T = TypeVar("T")
 
 
 def create_unknown_value(cls: Type[T], val: Any) -> T:
     value_cls = cls._enum_value_cls_  # type: ignore
     name = f"unknown_{val}"
     return value_cls(name=name, value=val)
 
 
 def try_enum(cls: Type[T], val: Any) -> T:
     """A function that tries to turn the value into enum ``cls``.
 
     If it fails it returns a proxy invalid value instead.
     """
-
     try:
         return cls._enum_value_map_[val]  # type: ignore
     except (KeyError, TypeError, AttributeError):
         return create_unknown_value(cls, val)
 
 
 def enum_if_int(cls: Type[T], val: Any) -> T:
```

### Comparing `disnake-2.8.2/disnake/errors.py` & `disnake-2.9.0/disnake/errors.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ext/commands/__init__.py` & `disnake-2.9.0/disnake/ext/commands/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # SPDX-License-Identifier: MIT
 
-"""
-disnake.ext.commands
+"""disnake.ext.commands
 ~~~~~~~~~~~~~~~~~~~~~
 
 An extension module to facilitate creation of bot commands.
 
 :copyright: (c) 2015-2021 Rapptz, 2021-present Disnake Development
 :license: MIT, see LICENSE for more details.
 """
```

### Comparing `disnake-2.8.2/disnake/ext/commands/_types.py` & `disnake-2.9.0/disnake/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ext/commands/base_core.py` & `disnake-2.9.0/disnake/ext/commands/base_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,29 +259,27 @@
         This is the non-decorator interface to :func:`.check`.
 
         Parameters
         ----------
         func
             The function that will be used as a check.
         """
-
         self.checks.append(func)
 
     def remove_check(self, func: Check) -> None:
         """Removes a check from the application command.
 
         This function is idempotent and will not raise an exception
         if the function is not in the command's checks.
 
         Parameters
         ----------
         func
             The function to remove from the checks.
         """
-
         try:
             self.checks.remove(func)
         except ValueError:
             pass
 
     async def __call__(self, interaction: ApplicationCommandInteraction, *args, **kwargs) -> Any:
         """|coro|
@@ -378,18 +376,16 @@
             bucket = self._buckets.get_bucket(inter)  # type: ignore
             dt = inter.created_at
             current = dt.replace(tzinfo=datetime.timezone.utc).timestamp()
             return bucket.get_retry_after(current)
 
         return 0.0
 
+    # This method isn't really usable in this class, but it's usable in subclasses.
     async def invoke(self, inter: ApplicationCommandInteraction, *args, **kwargs) -> None:
-        """
-        This method isn't really usable in this class, but it's usable in subclasses.
-        """
         await self.prepare(inter)
 
         try:
             await self(inter, *args, **kwargs)
         except CommandError:
             inter.command_failed = True
             raise
@@ -416,25 +412,22 @@
             The coroutine to register as the local error handler.
 
         Raises
         ------
         TypeError
             The coroutine passed is not actually a coroutine.
         """
-
         if not asyncio.iscoroutinefunction(coro):
             raise TypeError("The error handler must be a coroutine.")
 
         self.on_error: Error = coro
         return coro
 
     def has_error_handler(self) -> bool:
-        """
-        Checks whether the application command has an error handler registered.
-        """
+        """Checks whether the application command has an error handler registered."""
         return hasattr(self, "on_error")
 
     async def _call_local_error_handler(
         self, inter: ApplicationCommandInteraction, error: CommandError
     ) -> Any:
         if not self.has_error_handler():
             return
@@ -591,15 +584,14 @@
             by this function.
 
         Returns
         -------
         :class:`bool`
             A boolean indicating if the application command can be invoked.
         """
-
         original = inter.application_command
         inter.application_command = self
 
         if inter.data.type is ApplicationCommandType.chat_input:
             partial_attr_name = "slash_command"
         elif inter.data.type is ApplicationCommandType.user:
             partial_attr_name = "user_command"
@@ -654,14 +646,15 @@
     external_stickers: bool = ...,
     kick_members: bool = ...,
     manage_channels: bool = ...,
     manage_emojis: bool = ...,
     manage_emojis_and_stickers: bool = ...,
     manage_events: bool = ...,
     manage_guild: bool = ...,
+    manage_guild_expressions: bool = ...,
     manage_messages: bool = ...,
     manage_nicknames: bool = ...,
     manage_permissions: bool = ...,
     manage_roles: bool = ...,
     manage_threads: bool = ...,
     manage_webhooks: bool = ...,
     mention_everyone: bool = ...,
@@ -671,25 +664,29 @@
     priority_speaker: bool = ...,
     read_message_history: bool = ...,
     read_messages: bool = ...,
     request_to_speak: bool = ...,
     send_messages: bool = ...,
     send_messages_in_threads: bool = ...,
     send_tts_messages: bool = ...,
+    send_voice_messages: bool = ...,
     speak: bool = ...,
     start_embedded_activities: bool = ...,
     stream: bool = ...,
     use_application_commands: bool = ...,
     use_embedded_activities: bool = ...,
     use_external_emojis: bool = ...,
+    use_external_sounds: bool = ...,
     use_external_stickers: bool = ...,
     use_slash_commands: bool = ...,
+    use_soundboard: bool = ...,
     use_voice_activation: bool = ...,
     view_audit_log: bool = ...,
     view_channel: bool = ...,
+    view_creator_monetization_analytics: bool = ...,
     view_guild_insights: bool = ...,
 ) -> Callable[[T], T]:
     ...
 
 
 @overload
 @_generated
@@ -697,17 +694,16 @@
     value: int = 0,
 ) -> Callable[[T], T]:
     ...
 
 
 @_overload_with_permissions
 def default_member_permissions(value: int = 0, **permissions: bool) -> Callable[[T], T]:
-    """
-    A decorator that sets default required member permissions for the command.
-    Unlike :func:`~.ext.commands.has_permissions`, this decorator does not add any checks.
+    """A decorator that sets default required member permissions for the command.
+    Unlike :func:`~.has_permissions`, this decorator does not add any checks.
     Instead, it prevents the command from being run by members without *all* required permissions,
     if not overridden by moderators on a guild-specific basis.
 
     See also the ``default_member_permissions`` parameter for application command decorators.
 
     .. note::
         This does not work with slash subcommands/groups.
```

### Comparing `disnake-2.8.2/disnake/ext/commands/bot.py` & `disnake-2.9.0/disnake/ext/commands/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import disnake
 
 from .bot_base import BotBase, when_mentioned, when_mentioned_or
 from .interaction_bot_base import InteractionBotBase
 
 if TYPE_CHECKING:
-
     import asyncio
 
     import aiohttp
     from typing_extensions import Self
 
     from disnake.activity import BaseActivity
     from disnake.client import GatewayParams
@@ -58,15 +57,15 @@
     test_guilds: List[:class:`int`]
         The list of IDs of the guilds where you're going to test your application commands.
         Defaults to ``None``, which means global registration of commands across
         all guilds.
 
         .. versionadded:: 2.1
 
-    command_sync_flags: :class:`.ext.commands.CommandSyncFlags`
+    command_sync_flags: :class:`.CommandSyncFlags`
         The command sync flags for the session. This is a way of
         controlling when and how application commands will be synced with the Discord API.
         If not given, defaults to :func:`CommandSyncFlags.default`.
 
         .. versionadded:: 2.7
 
     sync_commands: :class:`bool`
@@ -167,15 +166,15 @@
         The content prefixed into the default help message.
 
         This can be provided as a parameter at creation.
 
     help_command: Optional[:class:`.HelpCommand`]
         The help command implementation to use. This can be dynamically
         set at runtime. To remove the help command pass ``None``. For more
-        information on implementing a help command, see :ref:`ext_commands_help_command`.
+        information on implementing a help command, see :ref:`ext_commands_api_help_commands`.
 
         This can be provided as a parameter at creation.
 
     owner_id: Optional[:class:`int`]
         The user ID that owns the bot. If this is not set and is then queried via
         :meth:`.is_owner` then it is fetched automatically using
         :meth:`~.Bot.application_info`.
@@ -262,15 +261,15 @@
             localization_provider: Optional[LocalizationProtocol] = None,
             strict_localization: bool = False,
         ) -> None:
             ...
 
 
 class AutoShardedBot(BotBase, InteractionBotBase, disnake.AutoShardedClient):
-    """This is similar to :class:`.Bot` except that it is inherited from
+    """Similar to :class:`.Bot`, except that it is inherited from
     :class:`disnake.AutoShardedClient` instead.
     """
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
@@ -332,15 +331,15 @@
     test_guilds: List[:class:`int`]
         The list of IDs of the guilds where you're going to test your application commands.
         Defaults to ``None``, which means global registration of commands across
         all guilds.
 
         .. versionadded:: 2.1
 
-    command_sync_flags: :class:`.ext.commands.CommandSyncFlags`
+    command_sync_flags: :class:`.CommandSyncFlags`
         The command sync flags for the session. This is a way of
         controlling when and how application commands will be synced with the Discord API.
         If not given, defaults to :func:`CommandSyncFlags.default`.
 
         .. versionadded:: 2.7
 
     sync_commands: :class:`bool`
@@ -463,15 +462,15 @@
             localization_provider: Optional[LocalizationProtocol] = None,
             strict_localization: bool = False,
         ) -> None:
             ...
 
 
 class AutoShardedInteractionBot(InteractionBotBase, disnake.AutoShardedClient):
-    """This is similar to :class:`.InteractionBot` except that it is inherited from
+    """Similar to :class:`.InteractionBot`, except that it is inherited from
     :class:`disnake.AutoShardedClient` instead.
     """
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
```

### Comparing `disnake-2.8.2/disnake/ext/commands/bot_base.py` & `disnake-2.9.0/disnake/ext/commands/bot_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,16 +68,15 @@
 
 def when_mentioned_or(*prefixes: str) -> Callable[[BotBase, Message], List[str]]:
     """A callable that implements when mentioned or other prefixes provided.
 
     These are meant to be passed into the :attr:`.Bot.command_prefix` attribute.
 
     Example
-    --------
-
+    -------
     .. code-block:: python3
 
         bot = commands.Bot(command_prefix=commands.when_mentioned_or('!'))
 
 
     .. note::
 
@@ -88,15 +87,15 @@
 
             async def get_prefix(bot, message):
                 extras = await prefixes_for(message.guild) # returns a list
                 return commands.when_mentioned_or(*extras)(bot, message)
 
 
     See Also
-    ----------
+    --------
     :func:`.when_mentioned`
     """
 
     def inner(bot, msg):
         r = list(prefixes)
         r = when_mentioned(bot, msg) + r
         return r
@@ -127,15 +126,15 @@
         *,
         strip_after_prefix: bool = False,
         **options: Any,
     ) -> None:
         super().__init__(**options)
 
         if not isinstance(self, disnake.Client):
-            raise RuntimeError("BotBase mixin must be used with disnake.Client")
+            raise RuntimeError("BotBase mixin must be used with disnake.Client")  # noqa: TRY004
 
         alternative = (
             "AutoShardedInteractionBot"
             if isinstance(self, disnake.AutoShardedClient)
             else "InteractionBot"
         )
         if command_prefix is None:
@@ -259,16 +258,15 @@
         check_list = self._check_once if call_once else self._checks
         try:
             check_list.remove(func)
         except ValueError:
             pass
 
     def check(self, func: T) -> T:
-        """
-        A decorator that adds a global check to the bot.
+        """A decorator that adds a global check to the bot.
 
         This is for text commands only, and doesn't apply to application commands.
 
         A global check is similar to a :func:`.check` that is applied
         on a per command basis except it is run before any command checks
         have been verified and applies to every command the bot has.
 
@@ -277,30 +275,28 @@
             This function can either be a regular function or a coroutine.
 
         Similar to a command :func:`.check`\\, this takes a single parameter
         of type :class:`.Context` and can only raise exceptions inherited from
         :exc:`.CommandError`.
 
         Example
-        ---------
-
+        -------
         .. code-block:: python3
 
             @bot.check
             def check_commands(ctx):
                 return ctx.command.qualified_name in allowed_commands
 
         """
         # T was used instead of Check to ensure the type matches on return
         self.add_check(func)  # type: ignore
         return func
 
     def check_once(self, func: CFT) -> CFT:
-        """
-        A decorator that adds a "call once" global check to the bot.
+        """A decorator that adds a "call once" global check to the bot.
 
         This is for text commands only, and doesn't apply to application commands.
 
         Unlike regular global checks, this one is called only once
         per :meth:`.invoke` call.
 
         Regular global checks are called whenever a command is called
@@ -319,16 +315,15 @@
             This function can either be a regular function or a coroutine.
 
         Similar to a command :func:`.check`\\, this takes a single parameter
         of type :class:`.Context` and can only raise exceptions inherited from
         :exc:`.CommandError`.
 
         Example
-        ---------
-
+        -------
         .. code-block:: python3
 
             @bot.check_once
             def whitelist(ctx):
                 return ctx.message.author.id in my_whitelist
 
         """
@@ -375,16 +370,15 @@
         if not asyncio.iscoroutinefunction(coro):
             raise TypeError("The pre-invoke hook must be a coroutine.")
 
         self._before_invoke = coro
         return coro
 
     def after_invoke(self, coro: CFT) -> CFT:
-        """
-        A decorator that registers a coroutine as a post-invoke hook.
+        """A decorator that registers a coroutine as a post-invoke hook.
 
         This is for text commands only, and doesn't apply to application commands.
 
         A post-invoke hook is called directly after the command is
         called. This makes it a useful function to clean-up database
         connections or any type of clean up required.
 
@@ -478,24 +472,23 @@
                 # replace it with our own error if that's the case.
                 if isinstance(ret, collections.abc.Iterable):
                     raise
 
                 raise TypeError(
                     "command_prefix must be plain string, iterable of strings, or callable "
                     f"returning either of these, not {ret.__class__.__name__}"
-                )
+                ) from None
 
             if not ret:
                 raise ValueError("Iterable command_prefix must contain at least one prefix")
 
         return ret
 
     async def get_context(self, message: Message, *, cls: Type[CXT] = Context) -> CXT:
-        """
-        |coro|
+        """|coro|
 
         Returns the invocation context from the message.
 
         This is a more low-level counter-part for :meth:`.process_commands`
         to allow users more fine grained control over the processing.
 
         The returned context is not guaranteed to be a valid invocation
@@ -515,15 +508,14 @@
 
         Returns
         -------
         :class:`.Context`
             The invocation context. The type of this can change via the
             ``cls`` parameter.
         """
-
         view = StringView(message.content)
         ctx = cast("CXT", cls(prefix=None, view=view, bot=self, message=message))
 
         if message.author.id == self.user.id:  # type: ignore
             return ctx
 
         prefix = await self.get_prefix(message)
@@ -544,23 +536,23 @@
                     return ctx
 
             except TypeError:
                 if not isinstance(prefix, list):
                     raise TypeError(
                         "get_prefix must return either a string or a list of string, "
                         f"not {prefix.__class__.__name__}"
-                    )
+                    ) from None
 
                 # It's possible a bad command_prefix got us here.
                 for value in prefix:
                     if not isinstance(value, str):
                         raise TypeError(
                             "Iterable command_prefix or list returned from get_prefix must "
                             f"contain only strings, not {value.__class__.__name__}"
-                        )
+                        ) from None
 
                 # Getting here shouldn't happen
                 raise
 
         if self.strip_after_prefix:
             view.skip_ws()
```

### Comparing `disnake-2.8.2/disnake/ext/commands/cog.py` & `disnake-2.9.0/disnake/ext/commands/cog.py`

 * *Files 4% similar despite different names*

```diff
@@ -280,76 +280,71 @@
                 # Update our parent's reference to our self
                 parent.remove_command(command.name)  # type: ignore
                 parent.add_command(command)  # type: ignore
 
         return self
 
     def get_commands(self) -> List[Command]:
-        """
-        Returns a list of commands the cog has.
+        """Returns a list of commands the cog has.
 
         Returns
         -------
         List[:class:`.Command`]
             A :class:`list` of :class:`.Command`\\s that are
             defined inside this cog.
 
             .. note::
 
                 This does not include subcommands.
         """
         return [c for c in self.__cog_commands__ if c.parent is None]
 
     def get_application_commands(self) -> List[InvokableApplicationCommand]:
-        """
-        Returns a list of application commands the cog has.
+        """Returns a list of application commands the cog has.
 
         Returns
         -------
         List[:class:`.InvokableApplicationCommand`]
             A :class:`list` of :class:`.InvokableApplicationCommand`\\s that are
             defined inside this cog.
 
             .. note::
 
                 This does not include subcommands.
         """
         return list(self.__cog_app_commands__)
 
     def get_slash_commands(self) -> List[InvokableSlashCommand]:
-        """
-        Returns a list of slash commands the cog has.
+        """Returns a list of slash commands the cog has.
 
         Returns
         -------
         List[:class:`.InvokableSlashCommand`]
             A :class:`list` of :class:`.InvokableSlashCommand`\\s that are
             defined inside this cog.
 
             .. note::
 
                 This does not include subcommands.
         """
         return [c for c in self.__cog_app_commands__ if isinstance(c, InvokableSlashCommand)]
 
     def get_user_commands(self) -> List[InvokableUserCommand]:
-        """
-        Returns a list of user commands the cog has.
+        """Returns a list of user commands the cog has.
 
         Returns
         -------
         List[:class:`.InvokableUserCommand`]
             A :class:`list` of :class:`.InvokableUserCommand`\\s that are
             defined inside this cog.
         """
         return [c for c in self.__cog_app_commands__ if isinstance(c, InvokableUserCommand)]
 
     def get_message_commands(self) -> List[InvokableMessageCommand]:
-        """
-        Returns a list of message commands the cog has.
+        """Returns a list of message commands the cog has.
 
         Returns
         -------
         List[:class:`.InvokableMessageCommand`]
             A :class:`list` of :class:`.InvokableMessageCommand`\\s that are
             defined inside this cog.
         """
@@ -555,27 +550,27 @@
     @_cog_special_method
     def bot_message_command_check(self, inter: ApplicationCommandInteraction) -> bool:
         """Similar to :meth:`.Bot.slash_command_check` but for message commands."""
         return True
 
     @_cog_special_method
     def cog_check(self, ctx: Context) -> bool:
-        """A special method that registers as a :func:`~.ext.commands.check`
+        """A special method that registers as a :func:`~.check`
         for every text command and subcommand in this cog.
 
         This is for text commands only, and doesn't apply to application commands.
 
         This function **can** be a coroutine and must take a sole parameter,
         ``ctx``, to represent the :class:`.Context`.
         """
         return True
 
     @_cog_special_method
     def cog_slash_command_check(self, inter: ApplicationCommandInteraction) -> bool:
-        """A special method that registers as a :func:`~.ext.commands.check`
+        """A special method that registers as a :func:`~.check`
         for every slash command and subcommand in this cog.
 
         This function **can** be a coroutine and must take a sole parameter,
         ``inter``, to represent the :class:`.ApplicationCommandInteraction`.
         """
         return True
 
@@ -724,61 +719,75 @@
 
     @_cog_special_method
     async def cog_after_message_command_invoke(self, inter: ApplicationCommandInteraction) -> None:
         """Similar to :meth:`cog_after_slash_command_invoke` but for message commands."""
         pass
 
     def _inject(self, bot: AnyBot) -> Self:
+        from .bot import AutoShardedInteractionBot, InteractionBot
+
         cls = self.__class__
 
+        if (
+            isinstance(bot, (InteractionBot, AutoShardedInteractionBot))
+            and len(self.__cog_commands__) > 0
+        ):
+            raise TypeError("@commands.command is not supported for interaction bots.")
+
         # realistically, the only thing that can cause loading errors
         # is essentially just the command loading, which raises if there are
         # duplicates. When this condition is met, we want to undo all what
         # we've added so far for some form of atomic loading.
         for index, command in enumerate(self.__cog_commands__):
             command.cog = self
             if command.parent is None:
                 try:
                     bot.add_command(command)  # type: ignore
-                except Exception as e:
+                except Exception:
                     # undo our additions
                     for to_undo in self.__cog_commands__[:index]:
                         if to_undo.parent is None:
                             bot.remove_command(to_undo.name)  # type: ignore
-                    raise e
+                    raise
 
         for index, command in enumerate(self.__cog_app_commands__):
             command.cog = self
             try:
                 if isinstance(command, InvokableSlashCommand):
                     bot.add_slash_command(command)
                 elif isinstance(command, InvokableUserCommand):
                     bot.add_user_command(command)
                 elif isinstance(command, InvokableMessageCommand):
                     bot.add_message_command(command)
-            except Exception as e:
+            except Exception:
                 # undo our additions
                 for to_undo in self.__cog_app_commands__[:index]:
                     if isinstance(to_undo, InvokableSlashCommand):
                         bot.remove_slash_command(to_undo.name)
                     elif isinstance(to_undo, InvokableUserCommand):
                         bot.remove_user_command(to_undo.name)
                     elif isinstance(to_undo, InvokableMessageCommand):
                         bot.remove_message_command(to_undo.name)
-                raise e
+                raise
 
         if not hasattr(self.cog_load.__func__, "__cog_special_method__"):
             bot.loop.create_task(disnake.utils.maybe_coroutine(self.cog_load))
 
         # check if we're overriding the default
         if cls.bot_check is not Cog.bot_check:
-            bot.add_check(self.bot_check)  # type: ignore
+            if isinstance(bot, (InteractionBot, AutoShardedInteractionBot)):
+                raise TypeError("Cog.bot_check is not supported for interaction bots.")
+
+            bot.add_check(self.bot_check)
 
         if cls.bot_check_once is not Cog.bot_check_once:
-            bot.add_check(self.bot_check_once, call_once=True)  # type: ignore
+            if isinstance(bot, (InteractionBot, AutoShardedInteractionBot)):
+                raise TypeError("Cog.bot_check_once is not supported for interaction bots.")
+
+            bot.add_check(self.bot_check_once, call_once=True)
 
         # Add application command checks
         if cls.bot_slash_command_check is not Cog.bot_slash_command_check:
             bot.add_app_command_check(self.bot_slash_command_check, slash_commands=True)  # type: ignore
 
         if cls.bot_user_command_check is not Cog.bot_user_command_check:
             bot.add_app_command_check(self.bot_user_command_check, user_commands=True)  # type: ignore
```

### Comparing `disnake-2.8.2/disnake/ext/commands/common_bot_base.py` & `disnake-2.9.0/disnake/ext/commands/common_bot_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     from ._types import CoroFunc
     from .bot import AutoShardedBot, AutoShardedInteractionBot, Bot, InteractionBot
     from .help import HelpCommand
 
     AnyBot = Union[Bot, AutoShardedBot, InteractionBot, AutoShardedInteractionBot]
 
 __all__ = ("CommonBotBase",)
+_log = logging.getLogger(__name__)
 
 CogT = TypeVar("CogT", bound="Cog")
 CFT = TypeVar("CFT", bound="CoroFunc")
 
 MISSING: Any = disnake.utils.MISSING
 
 
@@ -104,24 +105,24 @@
 
     async def close(self) -> None:
         self._is_closed = True
 
         for extension in tuple(self.__extensions):
             try:
                 self.unload_extension(extension)
-            except Exception:
-                # TODO: consider logging exception
-                pass
+            except Exception as error:
+                error.__suppress_context__ = True
+                _log.error("Failed to unload extension %r", extension, exc_info=error)
 
         for cog in tuple(self.__cogs):
             try:
                 self.remove_cog(cog)
-            except Exception:
-                # TODO: consider logging exception
-                pass
+            except Exception as error:
+                error.__suppress_context__ = True
+                _log.exception("Failed to remove cog %r", cog, exc_info=error)
 
         await super().close()  # type: ignore
 
     @disnake.utils.copy_doc(disnake.Client.login)
     async def login(self, token: str) -> None:
         self.loop.create_task(self._fill_owners())  # type: ignore
 
@@ -253,16 +254,15 @@
         """A decorator that registers another function as an external
         event listener. Basically this allows you to listen to multiple
         events from different places e.g. such as :func:`.on_ready`
 
         The functions being listened to must be a :ref:`coroutine <coroutine>`.
 
         Example
-        --------
-
+        -------
         .. code-block:: python3
 
             @bot.listen()
             async def on_message(message):
                 print('one')
 
             # in some other file...
@@ -391,44 +391,55 @@
         return cog
 
     @property
     def cogs(self) -> Mapping[str, Cog]:
         """Mapping[:class:`str`, :class:`Cog`]: A read-only mapping of cog name to cog."""
         return types.MappingProxyType(self.__cogs)
 
+    def get_listeners(self) -> Mapping[str, List[CoroFunc]]:
+        """Mapping[:class:`str`, List[Callable]]: A read-only mapping of event names to listeners.
+
+        .. note::
+            To add or remove a listener you should use :meth:`.add_listener` and
+            :meth:`.remove_listener`.
+
+        .. versionadded:: 2.9
+        """
+        return types.MappingProxyType(self.extra_events)
+
     # extensions
 
     def _remove_module_references(self, name: str) -> None:
         # find all references to the module
         # remove the cogs registered from the module
         for cogname, cog in self.__cogs.copy().items():
             if _is_submodule(name, cog.__module__):
                 self.remove_cog(cogname)
         # remove all the listeners from the module
         for event_list in self.extra_events.copy().values():
             remove = [
                 index
                 for index, event in enumerate(event_list)
-                if event.__module__ is not None and _is_submodule(name, event.__module__)
+                if event.__module__ and _is_submodule(name, event.__module__)
             ]
 
             for index in reversed(remove):
                 del event_list[index]
 
     def _call_module_finalizers(self, lib: types.ModuleType, key: str) -> None:
         try:
             func = lib.teardown
         except AttributeError:
             pass
         else:
             try:
                 func(self)
-            except Exception:
-                # TODO: consider logging exception
-                pass
+            except Exception as error:
+                error.__suppress_context__ = True
+                _log.error("Exception in extension finalizer %r", key, exc_info=error)
         finally:
             self.__extensions.pop(key, None)
             sys.modules.pop(key, None)
             name = lib.__name__
             for module in list(sys.modules.keys()):
                 if _is_submodule(name, module):
                     del sys.modules[module]
@@ -443,31 +454,31 @@
             del sys.modules[key]
             raise errors.ExtensionFailed(key, e) from e
 
         try:
             setup = lib.setup
         except AttributeError:
             del sys.modules[key]
-            raise errors.NoEntryPointError(key)
+            raise errors.NoEntryPointError(key) from None
 
         try:
             setup(self)
         except Exception as e:
             del sys.modules[key]
             self._remove_module_references(lib.__name__)
             self._call_module_finalizers(lib, key)
             raise errors.ExtensionFailed(key, e) from e
         else:
             self.__extensions[key] = lib
 
     def _resolve_name(self, name: str, package: Optional[str]) -> str:
         try:
             return importlib.util.resolve_name(name, package)
-        except ImportError:
-            raise errors.ExtensionNotFound(name)
+        except ImportError as e:
+            raise errors.ExtensionNotFound(name) from e
 
     def load_extension(self, name: str, *, package: Optional[str] = None) -> None:
         """Loads an extension.
 
         An extension is a python module that contains commands, cogs, or
         listeners.
```

### Comparing `disnake-2.8.2/disnake/ext/commands/context.py` & `disnake-2.9.0/disnake/ext/commands/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,15 @@
 if TYPE_CHECKING:
     P = ParamSpec("P")
 else:
     P = TypeVar("P")
 
 
 class Context(disnake.abc.Messageable, Generic[BotT]):
-    """
-    Represents the context in which a command is being invoked under.
+    """Represents the context in which a command is being invoked under.
 
     This class contains a lot of meta data to help you understand more about
     the invocation context. This class is not created manually and is instead
     passed around to commands as the first parameter.
 
     This class implements the :class:`.abc.Messageable` ABC.
 
@@ -127,16 +126,15 @@
         self.invoked_subcommand: Optional[Command] = invoked_subcommand
         self.subcommand_passed: Optional[str] = subcommand_passed
         self.command_failed: bool = command_failed
         self.current_parameter: Optional[inspect.Parameter] = current_parameter
         self._state: ConnectionState = self.message._state
 
     async def invoke(self, command: Command[CogT, P, T], /, *args: P.args, **kwargs: P.kwargs) -> T:
-        """
-        |coro|
+        """|coro|
 
         Calls a command with the arguments given.
 
         This is useful if you want to just call the callback that a
         :class:`.Command` holds internally.
 
         .. note::
@@ -345,17 +343,15 @@
         entity = args[0]
         if isinstance(entity, str):
             entity = bot.get_cog(entity) or bot.get_command(entity)
 
         if entity is None:
             return None
 
-        try:
-            entity.qualified_name
-        except AttributeError:
+        if not hasattr(entity, "qualified_name"):
             # if we're here then it's not a cog, group, or command.
             return None
 
         await cmd.prepare_help_command(self, entity.qualified_name)
 
         try:
             if hasattr(entity, "__cog_commands__"):
```

### Comparing `disnake-2.8.2/disnake/ext/commands/converter.py` & `disnake-2.9.0/disnake/ext/commands/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         The method to override to do conversion logic.
 
         If an error is found while converting, it is recommended to
         raise a :exc:`.CommandError` derived exception as it will
         properly propagate to the error handlers.
 
         Parameters
-        -----------
+        ----------
         ctx: Union[:class:`.Context`, :class:`.ApplicationCommandInteraction`]
             The invocation context that the argument is being used in.
         argument: :class:`str`
             The argument that is being converted.
 
         Raises
         ------
@@ -182,39 +182,54 @@
     """Converts to a :class:`~disnake.Member`.
 
     All lookups are via the local guild. If in a DM context, then the lookup
     is done by the global cache.
 
     The lookup strategy is as follows (in order):
 
-    1. Lookup by ID.
-    2. Lookup by mention.
-    3. Lookup by name#discrim
-    4. Lookup by name
+    1. Lookup by ID
+    2. Lookup by mention
+    3. Lookup by username#discrim
+    4. Lookup by username#0
     5. Lookup by nickname
+    6. Lookup by global name
+    7. Lookup by username
+
+    The name resolution order matches the one used by :meth:`.Guild.get_member_named`.
 
     .. versionchanged:: 1.5
         Raise :exc:`.MemberNotFound` instead of generic :exc:`.BadArgument`
 
     .. versionchanged:: 1.5.1
         This converter now lazily fetches members from the gateway and HTTP APIs,
         optionally caching the result if :attr:`.MemberCacheFlags.joined` is enabled.
+
+    .. versionchanged:: 2.9
+        Name resolution order changed from ``username > nick`` to
+        ``nick > global_name > username`` to account for the username migration.
     """
 
     async def query_member_named(
         self, guild: disnake.Guild, argument: str
     ) -> Optional[disnake.Member]:
         cache = guild._state.member_cache_flags.joined
-        if len(argument) > 5 and argument[-5] == "#":
-            username, _, discriminator = argument.rpartition("#")
+
+        username, _, discriminator = argument.rpartition("#")
+        if username and (
+            discriminator == "0" or (len(discriminator) == 4 and discriminator.isdecimal())
+        ):
+            # legacy behavior
             members = await guild.query_members(username, limit=100, cache=cache)
             return _utils_get(members, name=username, discriminator=discriminator)
         else:
             members = await guild.query_members(argument, limit=100, cache=cache)
-            return disnake.utils.find(lambda m: m.name == argument or m.nick == argument, members)
+            return disnake.utils.find(
+                lambda m: m.nick == argument or m.global_name == argument or m.name == argument,
+                members,
+            )
 
     async def query_member_by_id(
         self, bot: disnake.Client, guild: disnake.Guild, user_id: int
     ) -> Optional[disnake.Member]:
         ws = bot._get_websocket(shard_id=guild.shard_id)
         cache = guild._state.member_cache_flags.joined
         if ws.is_ratelimited():
@@ -280,25 +295,31 @@
 class UserConverter(IDConverter[disnake.User]):
     """Converts to a :class:`~disnake.User`.
 
     All lookups are via the global user cache.
 
     The lookup strategy is as follows (in order):
 
-    1. Lookup by ID.
-    2. Lookup by mention.
-    3. Lookup by name#discrim
-    4. Lookup by name
+    1. Lookup by ID
+    2. Lookup by mention
+    3. Lookup by username#discrim
+    4. Lookup by username#0
+    5. Lookup by global name
+    6. Lookup by username
 
     .. versionchanged:: 1.5
         Raise :exc:`.UserNotFound` instead of generic :exc:`.BadArgument`
 
     .. versionchanged:: 1.6
         This converter now lazily fetches users from the HTTP APIs if an ID is passed
         and it's not available in cache.
+
+    .. versionchanged:: 2.9
+        Now takes :attr:`~disnake.User.global_name` into account.
+        No longer automatically removes ``"@"`` prefix from arguments.
     """
 
     async def convert(self, ctx: AnyContext, argument: str) -> disnake.User:
         match = self._get_id_match(argument) or re.match(r"<@!?([0-9]{17,19})>$", argument)
         state = ctx._state
         bot: disnake.Client = ctx.bot
         result: Optional[Union[disnake.User, disnake.Member]] = None
@@ -319,32 +340,29 @@
                 except disnake.HTTPException:
                     raise UserNotFound(argument) from None
 
             if isinstance(result, disnake.Member):
                 return result._user
             return result
 
-        arg = argument
-
-        # Remove the '@' character if this is the first character from the argument
-        if arg[0] == "@":
-            # Remove first character
-            arg = arg[1:]
-
-        # check for discriminator if it exists,
-        if len(arg) > 5 and arg[-5] == "#":
-            discrim = arg[-4:]
-            name = arg[:-5]
-            result = disnake.utils.find(
-                lambda u: u.name == name and u.discriminator == discrim, state._users.values()
-            )
+        username, _, discriminator = argument.rpartition("#")
+        # n.b. there's no builtin method that only matches arabic digits, `isdecimal` is the closest one.
+        # it really doesn't matter much, worst case is unnecessary computations
+        if username and (
+            discriminator == "0" or (len(discriminator) == 4 and discriminator.isdecimal())
+        ):
+            # legacy behavior
+            result = _utils_get(state._users.values(), name=username, discriminator=discriminator)
             if result is not None:
                 return result
 
-        result = disnake.utils.find(lambda u: u.name == arg, state._users.values())
+        result = disnake.utils.find(
+            lambda u: u.global_name == argument or u.name == argument,
+            state._users.values(),
+        )
 
         if result is None:
             raise UserNotFound(argument)
 
         return result
 
 
@@ -427,17 +445,17 @@
             return message
         channel = PartialMessageConverter._resolve_channel(ctx, guild_id, channel_id)
         if not channel:
             raise ChannelNotFound(str(channel_id))
         try:
             return await channel.fetch_message(message_id)
         except disnake.NotFound:
-            raise MessageNotFound(argument)
+            raise MessageNotFound(argument) from None
         except disnake.Forbidden:
-            raise ChannelNotReadable(channel)  # type: ignore
+            raise ChannelNotReadable(channel) from None  # type: ignore
 
 
 class GuildChannelConverter(IDConverter[disnake.abc.GuildChannel]):
     """Converts to a :class:`.abc.GuildChannel`.
 
     All lookups are via the local guild. If in a DM context, then the lookup
     is done by the global cache.
@@ -664,15 +682,15 @@
     def parse_hex_number(self, argument: str) -> disnake.Color:
         arg = "".join(i * 2 for i in argument) if len(argument) == 3 else argument
         try:
             value = int(arg, base=16)
             if not (0 <= value <= 0xFFFFFF):
                 raise BadColourArgument(argument)
         except ValueError:
-            raise BadColourArgument(argument)
+            raise BadColourArgument(argument) from None
         else:
             return disnake.Color(value=value)
 
     def parse_rgb_number(self, argument: str, number: str) -> int:
         if number[-1] == "%":
             value = int(number[:-1])
             if not (0 <= value <= 100):
@@ -734,15 +752,15 @@
     .. versionchanged:: 1.5
         Raise :exc:`.RoleNotFound` instead of generic :exc:`.BadArgument`
     """
 
     async def convert(self, ctx: AnyContext, argument: str) -> disnake.Role:
         guild = ctx.guild
         if not guild:
-            raise NoPrivateMessage()
+            raise NoPrivateMessage
 
         match = self._get_id_match(argument) or re.match(r"<@&([0-9]{17,19})>$", argument)
         if match:
             result = guild.get_role(int(match.group(1)))
         else:
             result = _utils_get(guild._roles.values(), name=argument)
 
@@ -996,15 +1014,16 @@
     This behaves similarly to :attr:`~disnake.Message.clean_content`.
 
     Attributes
     ----------
     fix_channel_mentions: :class:`bool`
         Whether to clean channel mentions.
     use_nicknames: :class:`bool`
-        Whether to use nicknames when transforming mentions.
+        Whether to use :attr:`nicknames <.Member.nick>` and
+        :attr:`global names <.Member.global_name>` when transforming mentions.
     escape_markdown: :class:`bool`
         Whether to also escape special markdown characters.
     remove_markdown: :class:`bool`
         Whether to also remove special markdown characters. This option is not supported with ``escape_markdown``
 
         .. versionadded:: 1.7
     """
@@ -1023,17 +1042,19 @@
         self.remove_markdown = remove_markdown
 
     async def convert(self, ctx: AnyContext, argument: str) -> str:
         msg = ctx.message if isinstance(ctx, Context) else None
         bot: disnake.Client = ctx.bot
 
         def resolve_user(id: int) -> str:
-            m = (msg and _utils_get(msg.mentions, id=id)) or bot.get_user(id)
-            if m is None and ctx.guild:
-                m = ctx.guild.get_member(id)
+            m = (
+                (msg and _utils_get(msg.mentions, id=id))
+                or (ctx.guild and ctx.guild.get_member(id))
+                or bot.get_user(id)
+            )
             return f"@{m.display_name if self.use_nicknames else m.name}" if m else "@deleted-user"
 
         def resolve_role(id: int) -> str:
             if ctx.guild is None:
                 return "@deleted-role"
             r = (msg and _utils_get(msg.role_mentions, id=id)) or ctx.guild.get_role(id)
             return f"@{r.name}" if r else "@deleted-role"
@@ -1064,16 +1085,15 @@
             result = disnake.utils.remove_markdown(result)
 
         # Completely ensure no mentions escape:
         return disnake.utils.escape_mentions(result)
 
 
 class Greedy(List[T]):
-    """
-    A special converter that greedily consumes arguments until it can't.
+    """A special converter that greedily consumes arguments until it can't.
     As a consequence of this behaviour, most input errors are silently discarded,
     since it is used as an indicator of when to stop parsing.
 
     When a parser error is met the greedy converter stops converting, undoes the
     internal string parsing routine, and continues parsing regularly.
 
     For example, in the following code:
@@ -1172,15 +1192,15 @@
     disnake.Permissions: PermissionsConverter,
     disnake.GuildScheduledEvent: GuildScheduledEventConverter,
 }
 
 
 async def _actual_conversion(
     ctx: Context,
-    converter: Union[Type[T], Converter[T], Callable[[str], T]],
+    converter: Union[Type[T], Type[Converter[T]], Converter[T], Callable[[str], T]],
     argument: str,
     param: inspect.Parameter,
 ) -> T:
     if converter is bool:
         return _convert_to_bool(argument)  # type: ignore
 
     if isinstance(converter, type):
```

### Comparing `disnake-2.8.2/disnake/ext/commands/cooldowns.py` & `disnake-2.9.0/disnake/ext/commands/cooldowns.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         return self._cooldown is not None
 
     @property
     def type(self) -> Callable[[Message], Any]:
         return self._type
 
     @classmethod
-    def from_cooldown(cls, rate, per, type) -> Self:
+    def from_cooldown(cls, rate: float, per: float, type) -> Self:
         return cls(Cooldown(rate, per), type)
 
     def _bucket_key(self, msg: Message) -> Any:
         return self._type(msg)
 
     def _verify_cache_integrity(self, current: Optional[float] = None) -> None:
         # we want to delete all cache objects that haven't been used
@@ -263,15 +263,15 @@
         return False
 
     def create_bucket(self, message: Message) -> Cooldown:
         return self._factory(message)
 
 
 class _Semaphore:
-    """This class is a version of a semaphore.
+    """A custom version of a semaphore.
 
     If you're wondering why asyncio.Semaphore isn't being used,
     it's because it doesn't expose the internal value. This internal
     value is necessary because I need to support both `wait=True` and
     `wait=False`.
 
     An asyncio.Queue could have been used to do this as well -- but it is
```

### Comparing `disnake-2.8.2/disnake/ext/commands/core.py` & `disnake-2.9.0/disnake/ext/commands/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,16 +208,15 @@
 
     def __setitem__(self, k, v) -> None:
         super().__setitem__(k.casefold(), v)
 
 
 # TODO: ideally, `ContextT` should be bound on the class here as well
 class Command(_BaseCommand, Generic[CogT, P, T]):
-    """
-    A class that implements the protocol for a bot text command.
+    """A class that implements the protocol for a bot text command.
 
     These are not created manually, instead they are created via the
     decorator or functional interface.
 
     Attributes
     ----------
     name: :class:`str`
@@ -556,38 +555,38 @@
                 # if we're here, then it's a KEYWORD_ONLY param type
                 # since this is mostly useless, we'll helpfully transform Greedy[X]
                 # into just X and do the parsing that way.
                 converter = converter.converter
 
         if view.eof:
             if param.kind == param.VAR_POSITIONAL:
-                raise RuntimeError()  # break the loop
+                raise RuntimeError  # break the loop
             if required:
                 if self._is_typing_optional(param.annotation):
                     return None
                 if hasattr(converter, "__commands_is_flag__") and converter._can_be_constructible():
                     return await converter._construct_default(ctx)
                 raise MissingRequiredArgument(param)
             return param.default
 
         previous = view.index
         if consume_rest_is_special:
             argument = view.read_rest().strip()
         else:
             try:
                 argument = view.get_quoted_word()
-            except ArgumentParsingError as exc:
+            except ArgumentParsingError:
                 if (
                     self._is_typing_optional(param.annotation)
                     and not param.kind == param.VAR_POSITIONAL
                 ):
                     view.index = previous
                     return None
                 else:
-                    raise exc
+                    raise
         view.previous = previous
 
         # type-checker fails to narrow argument
         return await run_converters(ctx, converter, argument, param)  # type: ignore
 
     async def _transform_greedy_pos(
         self, ctx: Context, param: inspect.Parameter, required: bool, converter: Any
@@ -618,15 +617,15 @@
         view = ctx.view
         previous = view.index
         try:
             argument = view.get_quoted_word()
             value = await run_converters(ctx, converter, argument, param)  # type: ignore
         except (CommandError, ArgumentParsingError):
             view.index = previous
-            raise RuntimeError() from None  # break loop
+            raise RuntimeError from None  # break loop
         else:
             return value
 
     @property
     def clean_params(self) -> Dict[str, inspect.Parameter]:
         """Dict[:class:`str`, :class:`inspect.Parameter`]:
         Retrieves the parameter dictionary without the context or self parameters.
@@ -653,35 +652,35 @@
     def full_parent_name(self) -> str:
         """:class:`str`: Retrieves the fully qualified parent command name.
 
         This the base command name required to execute it. For example,
         in ``?one two three`` the parent name would be ``one two``.
         """
         entries = []
-        command = self
+        command: Command[Any, ..., Any] = self
         # command.parent is type-hinted as GroupMixin some attributes are resolved via MRO
-        while command.parent is not None:  # type: ignore
+        while command.parent is not None:
             command = command.parent  # type: ignore
-            entries.append(command.name)  # type: ignore
+            entries.append(command.name)
 
         return " ".join(reversed(entries))
 
     @property
     def parents(self) -> List[Group]:
         """List[:class:`Group`]: Retrieves the parents of this command.
 
         If the command has no parents then it returns an empty :class:`list`.
 
         For example in commands ``?a b c test``, the parents are ``[c, b, a]``.
 
         .. versionadded:: 1.1
         """
         entries = []
-        command = self
-        while command.parent is not None:  # type: ignore
+        command: Command[Any, ..., Any] = self
+        while command.parent is not None:
             command = command.parent  # type: ignore
             entries.append(command)
 
         return entries
 
     @property
     def root_parent(self) -> Optional[Group]:
@@ -699,15 +698,14 @@
     def qualified_name(self) -> str:
         """:class:`str`: Retrieves the fully qualified command name.
 
         This is the full parent name with the command name as well.
         For example, in ``?one two three`` the qualified name would be
         ``one two three``.
         """
-
         parent = self.full_parent_name
         if parent:
             return f"{parent} {self.name}"
         else:
             return self.name
 
     def __str__(self) -> str:
@@ -726,23 +724,23 @@
             # we have 'self' as the first parameter so just advance
             # the iterator and resume parsing
             try:
                 next(iterator)
             except StopIteration:
                 raise disnake.ClientException(
                     f'Callback for {self.name} command is missing "self" parameter.'
-                )
+                ) from None
 
         # next we have the 'ctx' as the next parameter
         try:
             next(iterator)
         except StopIteration:
             raise disnake.ClientException(
                 f'Callback for {self.name} command is missing "ctx" parameter.'
-            )
+            ) from None
 
         for name, param in iterator:
             ctx.current_parameter = param
             if param.kind in (param.POSITIONAL_OR_KEYWORD, param.POSITIONAL_ONLY):
                 transformed = await self.transform(ctx, param)
                 args.append(transformed)
             elif param.kind == param.KEYWORD_ONLY:
@@ -902,15 +900,15 @@
 
         return 0.0
 
     async def invoke(self, ctx: Context) -> None:
         await self.prepare(ctx)
 
         # terminate the invoked_subcommand chain.
-        # since we're in a regular command (and not a group) then
+        # since we're in a regular prefix command (and not a group) then
         # the invoked subcommand is None.
         ctx.invoked_subcommand = None
         ctx.subcommand_passed = None
         injected = hooked_wrapped_callback(self, ctx, self.callback)
         await injected(*ctx.args, **ctx.kwargs)
 
     async def reinvoke(self, ctx: Context, *, call_hooks: bool = False) -> None:
@@ -1688,16 +1686,15 @@
     """
     if cls is MISSING:
         cls = Group
     return command(name=name, cls=cls, **attrs)
 
 
 def check(predicate: Check) -> Callable[[T], T]:
-    """
-    A decorator that adds a check to the :class:`.Command` or its
+    """A decorator that adds a check to the :class:`.Command` or its
     subclasses. These checks could be accessed via :attr:`.Command.checks`.
 
     These checks should be predicates that take in a single parameter taking
     a :class:`.Context`. If the check returns a ``False``-like value then
     during invocation a :exc:`.CheckFailure` exception is raised and sent to
     the :func:`.on_command_error` event.
 
@@ -1726,15 +1723,14 @@
         even if the original function was not a coroutine.
 
     .. versionchanged:: 1.3
         The ``predicate`` attribute was added.
 
     Examples
     --------
-
     Creating a basic check to see if the command invoker is you.
 
     .. code-block:: python3
 
         def check_if_it_is_me(ctx):
             return ctx.message.author.id == 85309593344815104
 
@@ -1784,16 +1780,15 @@
 
         decorator.predicate = wrapper
 
     return decorator  # type: ignore
 
 
 def check_any(*checks: Check) -> Callable[[T], T]:
-    """
-    A :func:`check` that is added that checks if any of the checks passed
+    """A :func:`check` that is added that checks if any of the checks passed
     will pass, i.e. using logical OR.
 
     If all checks fail then :exc:`.CheckAnyFailure` is raised to signal the failure.
     It inherits from :exc:`.CheckFailure`.
 
     .. note::
 
@@ -1811,15 +1806,14 @@
     ------
     TypeError
         A check passed has not been decorated with the :func:`check`
         decorator.
 
     Examples
     --------
-
     Creating a basic check to see if it's the bot owner or
     the server owner:
 
     .. code-block:: python3
 
         def is_guild_owner():
             def predicate(ctx):
@@ -1881,31 +1875,30 @@
     ----------
     item: Union[:class:`int`, :class:`str`]
         The name or ID of the role to check.
     """
 
     def predicate(ctx: AnyContext) -> bool:
         if ctx.guild is None:
-            raise NoPrivateMessage()
+            raise NoPrivateMessage
 
         # ctx.guild is None doesn't narrow ctx.author to Member
         if isinstance(item, int):
             role = disnake.utils.get(ctx.author.roles, id=item)  # type: ignore
         else:
             role = disnake.utils.get(ctx.author.roles, name=item)  # type: ignore
         if role is None:
             raise MissingRole(item)
         return True
 
     return check(predicate)
 
 
 def has_any_role(*items: Union[int, str]) -> Callable[[T], T]:
-    """
-    A :func:`.check` that is added that checks if the member invoking the
+    """A :func:`.check` that is added that checks if the member invoking the
     command has **any** of the roles specified. This means that if they have
     one out of the three roles specified, then this check will return `True`.
 
     Similar to :func:`.has_role`\\, the names or IDs passed in must be exact.
 
     This check raises one of two special exceptions, :exc:`.MissingAnyRole` if the user
     is missing all roles, or :exc:`.NoPrivateMessage` if it is used in a private message.
@@ -1930,15 +1923,15 @@
         @commands.has_any_role('Library Devs', 'Moderators', 492212595072434186)
         async def cool(ctx):
             await ctx.send('You are cool indeed')
     """
 
     def predicate(ctx: AnyContext) -> bool:
         if ctx.guild is None:
-            raise NoPrivateMessage()
+            raise NoPrivateMessage
 
         # ctx.guild is None doesn't narrow ctx.author to Member
         getter = functools.partial(disnake.utils.get, ctx.author.roles)  # type: ignore
         if any(
             getter(id=item) is not None if isinstance(item, int) else getter(name=item) is not None
             for item in items
         ):
@@ -1961,15 +1954,15 @@
 
         Raise :exc:`.BotMissingRole` or :exc:`.NoPrivateMessage`
         instead of generic :exc:`.CheckFailure`
     """
 
     def predicate(ctx: AnyContext) -> bool:
         if ctx.guild is None:
-            raise NoPrivateMessage()
+            raise NoPrivateMessage
 
         me = cast(disnake.Member, ctx.me)
         if isinstance(item, int):
             role = disnake.utils.get(me.roles, id=item)
         else:
             role = disnake.utils.get(me.roles, name=item)
         if role is None:
@@ -1991,15 +1984,15 @@
 
         Raise :exc:`.BotMissingAnyRole` or :exc:`.NoPrivateMessage`
         instead of generic checkfailure
     """
 
     def predicate(ctx: AnyContext) -> bool:
         if ctx.guild is None:
-            raise NoPrivateMessage()
+            raise NoPrivateMessage
 
         me = cast(disnake.Member, ctx.me)
         getter = functools.partial(disnake.utils.get, me.roles)
         if any(
             getter(id=item) is not None if isinstance(item, int) else getter(name=item) is not None
             for item in items
         ):
@@ -2029,14 +2022,15 @@
     external_stickers: bool = ...,
     kick_members: bool = ...,
     manage_channels: bool = ...,
     manage_emojis: bool = ...,
     manage_emojis_and_stickers: bool = ...,
     manage_events: bool = ...,
     manage_guild: bool = ...,
+    manage_guild_expressions: bool = ...,
     manage_messages: bool = ...,
     manage_nicknames: bool = ...,
     manage_permissions: bool = ...,
     manage_roles: bool = ...,
     manage_threads: bool = ...,
     manage_webhooks: bool = ...,
     mention_everyone: bool = ...,
@@ -2046,25 +2040,29 @@
     priority_speaker: bool = ...,
     read_message_history: bool = ...,
     read_messages: bool = ...,
     request_to_speak: bool = ...,
     send_messages: bool = ...,
     send_messages_in_threads: bool = ...,
     send_tts_messages: bool = ...,
+    send_voice_messages: bool = ...,
     speak: bool = ...,
     start_embedded_activities: bool = ...,
     stream: bool = ...,
     use_application_commands: bool = ...,
     use_embedded_activities: bool = ...,
     use_external_emojis: bool = ...,
+    use_external_sounds: bool = ...,
     use_external_stickers: bool = ...,
     use_slash_commands: bool = ...,
+    use_soundboard: bool = ...,
     use_voice_activation: bool = ...,
     view_audit_log: bool = ...,
     view_channel: bool = ...,
+    view_creator_monetization_analytics: bool = ...,
     view_guild_insights: bool = ...,
 ) -> Callable[[T], T]:
     ...
 
 
 @overload
 @_generated
@@ -2146,14 +2144,15 @@
     external_stickers: bool = ...,
     kick_members: bool = ...,
     manage_channels: bool = ...,
     manage_emojis: bool = ...,
     manage_emojis_and_stickers: bool = ...,
     manage_events: bool = ...,
     manage_guild: bool = ...,
+    manage_guild_expressions: bool = ...,
     manage_messages: bool = ...,
     manage_nicknames: bool = ...,
     manage_permissions: bool = ...,
     manage_roles: bool = ...,
     manage_threads: bool = ...,
     manage_webhooks: bool = ...,
     mention_everyone: bool = ...,
@@ -2163,25 +2162,29 @@
     priority_speaker: bool = ...,
     read_message_history: bool = ...,
     read_messages: bool = ...,
     request_to_speak: bool = ...,
     send_messages: bool = ...,
     send_messages_in_threads: bool = ...,
     send_tts_messages: bool = ...,
+    send_voice_messages: bool = ...,
     speak: bool = ...,
     start_embedded_activities: bool = ...,
     stream: bool = ...,
     use_application_commands: bool = ...,
     use_embedded_activities: bool = ...,
     use_external_emojis: bool = ...,
+    use_external_sounds: bool = ...,
     use_external_stickers: bool = ...,
     use_slash_commands: bool = ...,
+    use_soundboard: bool = ...,
     use_voice_activation: bool = ...,
     view_audit_log: bool = ...,
     view_channel: bool = ...,
+    view_creator_monetization_analytics: bool = ...,
     view_guild_insights: bool = ...,
 ) -> Callable[[T], T]:
     ...
 
 
 @overload
 @_generated
@@ -2241,14 +2244,15 @@
     external_stickers: bool = ...,
     kick_members: bool = ...,
     manage_channels: bool = ...,
     manage_emojis: bool = ...,
     manage_emojis_and_stickers: bool = ...,
     manage_events: bool = ...,
     manage_guild: bool = ...,
+    manage_guild_expressions: bool = ...,
     manage_messages: bool = ...,
     manage_nicknames: bool = ...,
     manage_permissions: bool = ...,
     manage_roles: bool = ...,
     manage_threads: bool = ...,
     manage_webhooks: bool = ...,
     mention_everyone: bool = ...,
@@ -2258,25 +2262,29 @@
     priority_speaker: bool = ...,
     read_message_history: bool = ...,
     read_messages: bool = ...,
     request_to_speak: bool = ...,
     send_messages: bool = ...,
     send_messages_in_threads: bool = ...,
     send_tts_messages: bool = ...,
+    send_voice_messages: bool = ...,
     speak: bool = ...,
     start_embedded_activities: bool = ...,
     stream: bool = ...,
     use_application_commands: bool = ...,
     use_embedded_activities: bool = ...,
     use_external_emojis: bool = ...,
+    use_external_sounds: bool = ...,
     use_external_stickers: bool = ...,
     use_slash_commands: bool = ...,
+    use_soundboard: bool = ...,
     use_voice_activation: bool = ...,
     view_audit_log: bool = ...,
     view_channel: bool = ...,
+    view_creator_monetization_analytics: bool = ...,
     view_guild_insights: bool = ...,
 ) -> Callable[[T], T]:
     ...
 
 
 @overload
 @_generated
@@ -2333,14 +2341,15 @@
     external_stickers: bool = ...,
     kick_members: bool = ...,
     manage_channels: bool = ...,
     manage_emojis: bool = ...,
     manage_emojis_and_stickers: bool = ...,
     manage_events: bool = ...,
     manage_guild: bool = ...,
+    manage_guild_expressions: bool = ...,
     manage_messages: bool = ...,
     manage_nicknames: bool = ...,
     manage_permissions: bool = ...,
     manage_roles: bool = ...,
     manage_threads: bool = ...,
     manage_webhooks: bool = ...,
     mention_everyone: bool = ...,
@@ -2350,25 +2359,29 @@
     priority_speaker: bool = ...,
     read_message_history: bool = ...,
     read_messages: bool = ...,
     request_to_speak: bool = ...,
     send_messages: bool = ...,
     send_messages_in_threads: bool = ...,
     send_tts_messages: bool = ...,
+    send_voice_messages: bool = ...,
     speak: bool = ...,
     start_embedded_activities: bool = ...,
     stream: bool = ...,
     use_application_commands: bool = ...,
     use_embedded_activities: bool = ...,
     use_external_emojis: bool = ...,
+    use_external_sounds: bool = ...,
     use_external_stickers: bool = ...,
     use_slash_commands: bool = ...,
+    use_soundboard: bool = ...,
     use_voice_activation: bool = ...,
     view_audit_log: bool = ...,
     view_channel: bool = ...,
+    view_creator_monetization_analytics: bool = ...,
     view_guild_insights: bool = ...,
 ) -> Callable[[T], T]:
     ...
 
 
 @overload
 @_generated
@@ -2411,15 +2424,15 @@
     that is inherited from :exc:`.CheckFailure`.
 
     .. versionadded:: 1.1
     """
 
     def predicate(ctx: AnyContext) -> bool:
         if ctx.guild is not None:
-            raise PrivateMessageOnly()
+            raise PrivateMessageOnly
         return True
 
     return check(predicate)
 
 
 def guild_only() -> Callable[[T], T]:
     """A :func:`.check` that indicates this command must only be used in a
@@ -2428,15 +2441,15 @@
 
     This check raises a special exception, :exc:`.NoPrivateMessage`
     that is inherited from :exc:`.CheckFailure`.
     """
 
     def predicate(ctx: AnyContext) -> bool:
         if ctx.guild is None:
-            raise NoPrivateMessage()
+            raise NoPrivateMessage
         return True
 
     return check(predicate)
 
 
 def is_owner() -> Callable[[T], T]:
     """A :func:`.check` that checks if the person invoking this command is the
@@ -2467,15 +2480,23 @@
         Raise :exc:`.NSFWChannelRequired` instead of generic :exc:`.CheckFailure`.
         DM channels will also now pass this check.
     """
 
     def pred(ctx: AnyContext) -> bool:
         ch = ctx.channel
         if ctx.guild is None or (
-            isinstance(ch, (disnake.TextChannel, disnake.VoiceChannel, disnake.Thread))
+            isinstance(
+                ch,
+                (
+                    disnake.TextChannel,
+                    disnake.VoiceChannel,
+                    disnake.Thread,
+                    disnake.StageChannel,
+                ),
+            )
             and ch.is_nsfw()
         ):
             return True
         raise NSFWChannelRequired(ch)  # type: ignore
 
     return check(pred)
 
@@ -2605,16 +2626,15 @@
 
     This allows you to refer to one before invoke hook for several commands that
     do not have to be within the same cog.
 
     .. versionadded:: 1.4
 
     Example
-    ---------
-
+    -------
     .. code-block:: python3
 
         async def record_usage(ctx):
             print(ctx.author, 'used', ctx.command, 'at', ctx.message.created_at)
 
         @bot.command()
         @commands.before_invoke(record_usage)
```

### Comparing `disnake-2.8.2/disnake/ext/commands/ctx_menus_core.py` & `disnake-2.9.0/disnake/ext/commands/ctx_menus_core.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ext/commands/errors.py` & `disnake-2.9.0/disnake/ext/commands/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,15 @@
     "MissingFlagArgument",
     "TooManyFlags",
     "MissingRequiredFlag",
 )
 
 
 class CommandError(DiscordException):
-    """
-    The base exception type for all command related errors.
+    """The base exception type for all command related errors.
 
     This inherits from :exc:`disnake.DiscordException`.
 
     This exception and exceptions inherited from it are handled
     in a special way as they are caught and passed into a special event
     from :class:`.Bot`\\, :func:`.on_command_error`.
     """
@@ -105,15 +104,15 @@
 class ConversionError(CommandError):
     """Exception raised when a Converter class raises non-CommandError.
 
     This inherits from :exc:`CommandError`.
 
     Attributes
     ----------
-    converter: :class:`disnake.ext.commands.Converter`
+    converter: :class:`.Converter`
         The converter that failed.
     original: :exc:`Exception`
         The original exception that was raised. You can also get this via
         the ``__cause__`` attribute.
     """
 
     def __init__(self, converter: Any, original: Exception) -> None:
@@ -1039,15 +1038,15 @@
 
     This inherits from :exc:`FlagError`.
 
     .. versionadded:: 2.0
 
     Attributes
     ----------
-    flag: :class:`~disnake.ext.commands.Flag`
+    flag: :class:`.Flag`
         The flag that received too many values.
     values: List[:class:`str`]
         The values that were passed.
     """
 
     def __init__(self, flag: Flag, values: List[str]) -> None:
         self.flag: Flag = flag
@@ -1062,15 +1061,15 @@
 
     This inherits from :exc:`FlagError`
 
     .. versionadded:: 2.0
 
     Attributes
     ----------
-    flag: :class:`~disnake.ext.commands.Flag`
+    flag: :class:`.Flag`
         The flag that failed to convert.
     """
 
     def __init__(self, flag: Flag) -> None:
         self.flag: Flag = flag
         try:
             name = flag.annotation.__name__
@@ -1085,15 +1084,15 @@
 
     This inherits from :exc:`FlagError`
 
     .. versionadded:: 2.0
 
     Attributes
     ----------
-    flag: :class:`~disnake.ext.commands.Flag`
+    flag: :class:`.Flag`
         The required flag that was not found.
     """
 
     def __init__(self, flag: Flag) -> None:
         self.flag: Flag = flag
         super().__init__(f"Flag {flag.name!r} is required and missing")
 
@@ -1103,14 +1102,14 @@
 
     This inherits from :exc:`FlagError`
 
     .. versionadded:: 2.0
 
     Attributes
     ----------
-    flag: :class:`~disnake.ext.commands.Flag`
+    flag: :class:`.Flag`
         The flag that did not get a value.
     """
 
     def __init__(self, flag: Flag) -> None:
         self.flag: Flag = flag
         super().__init__(f"Flag {flag.name!r} does not have an argument")
```

### Comparing `disnake-2.8.2/disnake/ext/commands/flag_converter.py` & `disnake-2.9.0/disnake/ext/commands/flag_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     from .context import Context
 
 
 @dataclass
 class Flag:
     """Represents a flag parameter for :class:`FlagConverter`.
 
-    The :func:`~disnake.ext.commands.flag` function helps
+    The :func:`.flag` function helps
     create these flag objects, but it is not necessary to
     do so. These cannot be constructed manually.
 
     Attributes
     ----------
     name: :class:`str`
         The name of the flag.
@@ -183,15 +183,15 @@
             if flag.max_args is MISSING:
                 flag.max_args = 1
         else:
             if origin is Union:
                 # typing.Union
                 if flag.max_args is MISSING:
                     flag.max_args = 1
-                if annotation.__args__[-1] is type(None) and flag.default is MISSING:  # noqa: E721
+                if annotation.__args__[-1] is type(None) and flag.default is MISSING:
                     # typing.Optional
                     flag.default = None
             elif origin is tuple:
                 # typing.Tuple
                 # tuple parsing is e.g. `flag: peter 20`
                 # for Tuple[str, int] would give you flag: ('peter', 20)
                 if flag.max_args is MISSING:
@@ -407,15 +407,15 @@
                 return await tuple_convert_all(ctx, argument, flag, args[0])
             else:
                 return await tuple_convert_flag(ctx, argument, flag, args)
         elif origin is list:
             # typing.List[x]
             annotation = args[0]
             return await convert_flag(ctx, argument, flag, annotation)
-        elif origin is Union and args[-1] is type(None):  # noqa: E721
+        elif origin is Union and args[-1] is type(None):
             # typing.Optional[x]
             annotation = Union[args[:-1]]  # type: ignore
             return await run_converters(ctx, annotation, argument, param)
         elif origin is dict:
             # typing.Dict[K, V] -> typing.Tuple[K, V]
             return await tuple_convert_flag(ctx, argument, flag, args)
 
@@ -575,15 +575,15 @@
 
         self = cls.__new__(cls)
         for name, flag in flags.items():
             try:
                 values = arguments[name]
             except KeyError:
                 if flag.required:
-                    raise MissingRequiredFlag(flag)
+                    raise MissingRequiredFlag(flag) from None
                 else:
                     if callable(flag.default):
                         default = await maybe_coroutine(flag.default, ctx)
                         setattr(self, flag.attribute, default)
                     else:
                         setattr(self, flag.attribute, flag.default)
                     continue
```

### Comparing `disnake-2.8.2/disnake/ext/commands/flags.py` & `disnake-2.9.0/disnake/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ext/commands/help.py` & `disnake-2.9.0/disnake/ext/commands/help.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # SPDX-License-Identifier: MIT
+from __future__ import annotations
 
 import copy
 import functools
 import itertools
 import re
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional
 
 import disnake.utils
 
 from .core import Command, Group
 from .errors import CommandError
 
 if TYPE_CHECKING:
+    from ._types import MaybeCoro
     from .context import Context
 
 __all__ = (
     "Paginator",
     "HelpCommand",
     "DefaultHelpCommand",
     "MinimalHelpCommand",
@@ -67,22 +69,22 @@
 
     def __init__(
         self,
         prefix: Optional[str] = "```",
         suffix: Optional[str] = "```",
         max_size: int = 2000,
         linesep: str = "\n",
-    ):
+    ) -> None:
         self.prefix = prefix
         self.suffix = suffix
         self.max_size = max_size
         self.linesep = linesep
         self.clear()
 
-    def clear(self):
+    def clear(self) -> None:
         """Clears the paginator to have no pages."""
         if self.prefix is not None:
             self._current_page = [self.prefix]
             self._count = len(self.prefix) + self._linesep_len  # prefix + newline
         else:
             self._current_page = []
             self._count = 0
@@ -96,15 +98,15 @@
     def _suffix_len(self):
         return len(self.suffix) if self.suffix else 0
 
     @property
     def _linesep_len(self):
         return len(self.linesep)
 
-    def add_line(self, line="", *, empty=False):
+    def add_line(self, line: str = "", *, empty: bool = False):
         """Adds a line to the current page.
 
         If the line exceeds the :attr:`max_size` then an exception
         is raised.
 
         Parameters
         ----------
@@ -128,93 +130,93 @@
         self._count += len(line) + self._linesep_len
         self._current_page.append(line)
 
         if empty:
             self._current_page.append("")
             self._count += self._linesep_len
 
-    def close_page(self):
+    def close_page(self) -> None:
         """Prematurely terminate a page."""
         if self.suffix is not None:
             self._current_page.append(self.suffix)
         self._pages.append(self.linesep.join(self._current_page))
 
         if self.prefix is not None:
             self._current_page = [self.prefix]
             self._count = len(self.prefix) + self._linesep_len  # prefix + linesep
         else:
             self._current_page = []
             self._count = 0
 
-    def __len__(self):
+    def __len__(self) -> int:
         total = sum(len(p) for p in self._pages)
         return total + self._count
 
     @property
     def pages(self):
         """List[:class:`str`]: Returns the rendered list of pages."""
         # we have more than just the prefix in our current page
         if len(self._current_page) > (0 if self.prefix is None else 1):
             self.close_page()
         return self._pages
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         fmt = "<Paginator prefix: {0.prefix!r} suffix: {0.suffix!r} linesep: {0.linesep!r} max_size: {0.max_size} count: {0._count}>"
         return fmt.format(self)
 
 
 def _not_overriden(f):
     f.__help_command_not_overriden__ = True
     return f
 
 
 class _HelpCommandImpl(Command):
-    def __init__(self, inject, *args, **kwargs):
+    def __init__(self, inject, *args, **kwargs) -> None:
         super().__init__(inject.command_callback, *args, **kwargs)
         self._original = inject
         self._injected = inject
 
-    async def prepare(self, ctx):
+    async def prepare(self, ctx) -> None:
         self._injected = injected = self._original.copy()
         injected.context = ctx
         self.callback = injected.command_callback
 
         on_error = injected.on_help_command_error
         if not hasattr(on_error, "__help_command_not_overriden__"):
             if self.cog is not None:
                 self.on_error = self._on_error_cog_implementation
             else:
                 self.on_error = on_error
 
         await super().prepare(ctx)
 
-    async def _parse_arguments(self, ctx):
+    async def _parse_arguments(self, ctx) -> None:
         # Make the parser think we don't have a cog so it doesn't
         # inject the parameter into `ctx.args`.
         original_cog = self.cog
         self.cog = None
         try:
             await super()._parse_arguments(ctx)
         finally:
             self.cog = original_cog
 
-    async def _on_error_cog_implementation(self, dummy, ctx, error):
+    async def _on_error_cog_implementation(self, dummy, ctx, error) -> None:
         await self._injected.on_help_command_error(ctx, error)
 
     @property
     def clean_params(self):
         result = self.params.copy()
         try:
             del result[next(iter(result))]
         except StopIteration:
             raise ValueError("Missing context parameter") from None
         else:
             return result
 
-    def _inject_into_cog(self, cog):
+    def _inject_into_cog(self, cog) -> None:
         # Warning: hacky
 
         # Make the cog think that get_commands returns this command
         # as well if we inject it without modifying __cog_commands__
         # since that's used for the injection and ejection of cogs.
         def wrapped_get_commands(*, _original=cog.get_commands):
             ret = _original()
@@ -228,28 +230,27 @@
 
         functools.update_wrapper(wrapped_get_commands, cog.get_commands)
         functools.update_wrapper(wrapped_walk_commands, cog.walk_commands)
         cog.get_commands = wrapped_get_commands
         cog.walk_commands = wrapped_walk_commands
         self.cog = cog
 
-    def _eject_cog(self):
+    def _eject_cog(self) -> None:
         if self.cog is None:
             return
 
         # revert back into their original methods
         cog = self.cog
         cog.get_commands = cog.get_commands.__wrapped__
         cog.walk_commands = cog.walk_commands.__wrapped__
         self.cog = None
 
 
 class HelpCommand:
-    """
-    The base implementation for help command formatting.
+    """The base implementation for help command formatting.
 
     .. note::
 
         Internally instances of this class are deep copied every time
         the command itself is invoked to prevent a race condition
         mentioned in :issue-dpy:`2123`.
 
@@ -299,53 +300,51 @@
         # The keys can be safely copied as-is since they're 99.99% certain of being
         # string keys
         deepcopy = copy.deepcopy
         self.__original_kwargs__ = {k: deepcopy(v) for k, v in kwargs.items()}  # type: ignore
         self.__original_args__ = deepcopy(args)  # type: ignore
         return self
 
-    def __init__(self, **options):
+    def __init__(self, **options) -> None:
         self.show_hidden = options.pop("show_hidden", False)
         self.verify_checks = options.pop("verify_checks", True)
         self.command_attrs = attrs = options.pop("command_attrs", {})
         attrs.setdefault("name", "help")
         attrs.setdefault("help", "Shows this message")
         self.context: Context = disnake.utils.MISSING
         self._command_impl = _HelpCommandImpl(self, **self.command_attrs)
 
     def copy(self):
         obj = self.__class__(*self.__original_args__, **self.__original_kwargs__)  # type: ignore
         obj._command_impl = self._command_impl
         return obj
 
-    def _add_to_bot(self, bot):
+    def _add_to_bot(self, bot) -> None:
         command = _HelpCommandImpl(self, **self.command_attrs)
         bot.add_command(command)
         self._command_impl = command
 
-    def _remove_from_bot(self, bot):
+    def _remove_from_bot(self, bot) -> None:
         bot.remove_command(self._command_impl.name)
         self._command_impl._eject_cog()
 
-    def add_check(self, func):
-        """
-        Adds a check to the help command.
+    def add_check(self, func) -> None:
+        """Adds a check to the help command.
 
         .. versionadded:: 1.4
 
         Parameters
         ----------
         func
             The function that will be used as a check.
         """
         self._command_impl.add_check(func)
 
-    def remove_check(self, func):
-        """
-        Removes a check from the help command.
+    def remove_check(self, func) -> None:
+        """Removes a check from the help command.
 
         This function is idempotent and will not raise an exception if
         the function is not in the command's checks.
 
         .. versionadded:: 1.4
 
         Parameters
@@ -379,15 +378,15 @@
         """
         command_name = self._command_impl.name
         ctx = self.context
         if ctx is None or ctx.command is None or ctx.command.qualified_name != command_name:
             return command_name
         return ctx.invoked_with
 
-    def get_command_signature(self, command):
+    def get_command_signature(self, command) -> str:
         """Retrieves the signature portion of the help page.
 
         Parameters
         ----------
         command: :class:`Command`
             The command to get the signature of.
 
@@ -413,15 +412,15 @@
                 fmt = f"{parent_sig} {fmt}"
             alias = fmt
         else:
             alias = command.name if not parent_sig else f"{parent_sig} {command.name}"
 
         return f"{self.context.clean_prefix}{alias} {command.signature}"
 
-    def remove_mentions(self, string):
+    def remove_mentions(self, string: str):
         """Removes mentions from the string to prevent abuse.
 
         This includes ``@everyone``, ``@here``, member mentions and role mentions.
 
         Returns
         -------
         :class:`str`
@@ -447,23 +446,23 @@
         -------
         Optional[:class:`Cog`]
             The cog that is currently set for the help command.
         """
         return self._command_impl.cog
 
     @cog.setter
-    def cog(self, cog):
+    def cog(self, cog) -> None:
         # Remove whatever cog is currently valid, if any
         self._command_impl._eject_cog()
 
         # If a new cog is set then inject it.
         if cog is not None:
             self._command_impl._inject_into_cog(cog)
 
-    def command_not_found(self, string):
+    def command_not_found(self, string: str) -> MaybeCoro[str]:
         """|maybecoro|
 
         A method called when a command is not found in the help command.
         This is useful to override for i18n.
 
         Defaults to ``No command called {0} found.``
 
@@ -476,15 +475,15 @@
         Returns
         -------
         :class:`str`
             The string to use when a command has not been found.
         """
         return f'No command called "{string}" found.'
 
-    def subcommand_not_found(self, command, string):
+    def subcommand_not_found(self, command, string: str) -> MaybeCoro[str]:
         """|maybecoro|
 
         A method called when a command did not have a subcommand requested in the help command.
         This is useful to override for i18n.
 
         Defaults to either:
 
@@ -536,15 +535,14 @@
             passed as ``True`` then this will default as the command name.
 
         Returns
         -------
         List[:class:`Command`]
             A list of commands that passed the filter.
         """
-
         # set `key` iff `sort` is true
         if not sort:
             key = None
         elif key is None:
             key = lambda c: c.name
 
         iterator = commands if self.show_hidden else filter(lambda c: not c.hidden, commands)
@@ -601,15 +599,15 @@
         Returns
         -------
         :class:`.abc.Messageable`
             The destination where the help command will be output.
         """
         return self.context.channel
 
-    async def send_error_message(self, error):
+    async def send_error_message(self, error) -> None:
         """|coro|
 
         Handles the implementation when an error happens in the help command.
         For example, the result of :meth:`command_not_found` will be passed here.
 
         You can override this method to customise the behaviour.
 
@@ -626,15 +624,15 @@
             The error message to display to the user. Note that this has
             had mentions removed to prevent abuse.
         """
         destination = self.get_destination()
         await destination.send(error)
 
     @_not_overriden
-    async def on_help_command_error(self, ctx, error):
+    async def on_help_command_error(self, ctx, error) -> None:
         """|coro|
 
         The help command's error handler, as specified by :ref:`ext_commands_error_handler`.
 
         Useful to override if you need some specific behaviour when the error handler
         is called.
 
@@ -769,15 +767,15 @@
         Parameters
         ----------
         command: :class:`Command`
             The command that was requested for help.
         """
         return None
 
-    async def prepare_help_command(self, ctx, command=None):
+    async def prepare_help_command(self, ctx, command=None) -> None:
         """|coro|
 
         A low level method that can be used to prepare the help command
         before it does anything. For example, if you need to prepare
         some state in your subclass before the command does its processing
         then this would be the place to do it.
 
@@ -892,47 +890,47 @@
     no_category: :class:`str`
         The string used when there is a command which does not belong to any category(cog).
         Useful for i18n. Defaults to ``"No Category"``
     paginator: :class:`Paginator`
         The paginator used to paginate the help command output.
     """
 
-    def __init__(self, **options):
+    def __init__(self, **options) -> None:
         self.width = options.pop("width", 80)
         self.indent = options.pop("indent", 2)
         self.sort_commands = options.pop("sort_commands", True)
         self.dm_help = options.pop("dm_help", False)
         self.dm_help_threshold = options.pop("dm_help_threshold", 1000)
         self.commands_heading = options.pop("commands_heading", "Commands:")
         self.no_category = options.pop("no_category", "No Category")
         self.paginator = options.pop("paginator", Paginator())
 
         super().__init__(**options)
 
-    def shorten_text(self, text):
+    def shorten_text(self, text: str):
         """Shortens text to fit into the :attr:`width`.
 
         :return type: :class:`str`
         """
         if len(text) > self.width:
             return text[: self.width - 3].rstrip() + "..."
         return text
 
-    def get_ending_note(self):
+    def get_ending_note(self) -> Optional[str]:
         """Returns help command's ending note. This is mainly useful to override for i18n purposes.
 
         :return type: :class:`str`
         """
         command_name = self.invoked_with
         return (
             f"Type {self.context.clean_prefix}{command_name} command for more info on a command.\n"
             f"You can also type {self.context.clean_prefix}{command_name} category for more info on a category."
         )
 
-    def add_indented_commands(self, commands, *, heading, max_size=None):
+    def add_indented_commands(self, commands, *, heading, max_size: Optional[int] = None) -> None:
         """Indents a list of commands after the specified heading.
 
         The formatting is added to the :attr:`paginator`.
 
         The default implementation is the command name indented by
         :attr:`indent` spaces, padded to ``max_size`` followed by
         the command's :attr:`Command.short_doc` and then shortened
@@ -959,21 +957,21 @@
         get_width = disnake.utils._string_width
         for command in commands:
             name = command.name
             width = max_size - (get_width(name) - len(name))
             entry = f'{self.indent * " "}{name:<{width}} {command.short_doc}'
             self.paginator.add_line(self.shorten_text(entry))
 
-    async def send_pages(self):
+    async def send_pages(self) -> None:
         """A helper utility to send the page output from :attr:`paginator` to the destination."""
         destination = self.get_destination()
         for page in self.paginator.pages:
             await destination.send(page)
 
-    def add_command_formatting(self, command):
+    def add_command_formatting(self, command) -> None:
         """A utility function to format the non-indented block of commands and groups.
 
         Parameters
         ----------
         command: :class:`Command`
             The command to format.
         """
@@ -996,19 +994,19 @@
         if self.dm_help is True:
             return ctx.author
         elif self.dm_help is None and len(self.paginator) > self.dm_help_threshold:
             return ctx.author
         else:
             return ctx.channel
 
-    async def prepare_help_command(self, ctx, command):
+    async def prepare_help_command(self, ctx, command) -> None:
         self.paginator.clear()
         await super().prepare_help_command(ctx, command)
 
-    async def send_bot_help(self, mapping):
+    async def send_bot_help(self, mapping) -> None:
         ctx = self.context
         bot = ctx.bot
 
         if bot.description:
             # <description> portion
             self.paginator.add_line(bot.description, empty=True)
 
@@ -1032,34 +1030,34 @@
         note = self.get_ending_note()
         if note:
             self.paginator.add_line()
             self.paginator.add_line(note)
 
         await self.send_pages()
 
-    async def send_command_help(self, command):
+    async def send_command_help(self, command) -> None:
         self.add_command_formatting(command)
         self.paginator.close_page()
         await self.send_pages()
 
-    async def send_group_help(self, group):
+    async def send_group_help(self, group) -> None:
         self.add_command_formatting(group)
 
         filtered = await self.filter_commands(group.commands, sort=self.sort_commands)
         self.add_indented_commands(filtered, heading=self.commands_heading)
 
         if filtered:
             note = self.get_ending_note()
             if note:
                 self.paginator.add_line()
                 self.paginator.add_line(note)
 
         await self.send_pages()
 
-    async def send_cog_help(self, cog):
+    async def send_cog_help(self, cog) -> None:
         if cog.description:
             self.paginator.add_line(cog.description, empty=True)
 
         filtered = await self.filter_commands(cog.get_commands(), sort=self.sort_commands)
         self.add_indented_commands(filtered, heading=self.commands_heading)
 
         note = self.get_ending_note()
@@ -1098,32 +1096,32 @@
     no_category: :class:`str`
         The string used when there is a command which does not belong to any category(cog).
         Useful for i18n. Defaults to ``"No Category"``
     paginator: :class:`Paginator`
         The paginator used to paginate the help command output.
     """
 
-    def __init__(self, **options):
+    def __init__(self, **options) -> None:
         self.sort_commands = options.pop("sort_commands", True)
         self.commands_heading = options.pop("commands_heading", "Commands")
         self.dm_help = options.pop("dm_help", False)
         self.dm_help_threshold = options.pop("dm_help_threshold", 1000)
         self.aliases_heading = options.pop("aliases_heading", "Aliases:")
         self.no_category = options.pop("no_category", "No Category")
         self.paginator = options.pop("paginator", Paginator(suffix=None, prefix=None))
 
         super().__init__(**options)
 
-    async def send_pages(self):
+    async def send_pages(self) -> None:
         """A helper utility to send the page output from :attr:`paginator` to the destination."""
         destination = self.get_destination()
         for page in self.paginator.pages:
             await destination.send(page)
 
-    def get_opening_note(self):
+    def get_opening_note(self) -> Optional[str]:
         """Returns help command's opening note. This is mainly useful to override for i18n purposes.
 
         The default implementation returns ::
 
             Use `{prefix}{command_name} [command]` for more info on a command.
             You can also use `{prefix}{command_name} [category]` for more info on a category.
 
@@ -1134,30 +1132,30 @@
         """
         command_name = self.invoked_with
         return (
             f"Use `{self.context.clean_prefix}{command_name} [command]` for more info on a command.\n"
             f"You can also use `{self.context.clean_prefix}{command_name} [category]` for more info on a category."
         )
 
-    def get_command_signature(self, command):
+    def get_command_signature(self, command) -> str:
         return f"{self.context.clean_prefix}{command.qualified_name} {command.signature}"
 
-    def get_ending_note(self):
+    def get_ending_note(self) -> Optional[str]:
         """Return the help command's ending note. This is mainly useful to override for i18n purposes.
 
         The default implementation does nothing.
 
         Returns
         -------
         :class:`str`
             The help command ending note.
         """
         return None
 
-    def add_bot_commands_formatting(self, commands, heading):
+    def add_bot_commands_formatting(self, commands, heading) -> None:
         """Adds the minified bot heading with commands to the output.
 
         The formatting should be added to the :attr:`paginator`.
 
         The default implementation is a bold underline heading followed
         by commands separated by an EN SPACE (U+2002) in the next line.
 
@@ -1170,15 +1168,15 @@
         """
         if commands:
             # U+2002 Middle Dot
             joined = "\u2002".join(c.name for c in commands)
             self.paginator.add_line(f"__**{heading}**__")
             self.paginator.add_line(joined)
 
-    def add_subcommand_formatting(self, command):
+    def add_subcommand_formatting(self, command) -> None:
         """Adds formatting information on a subcommand.
 
         The formatting should be added to the :attr:`paginator`.
 
         The default implementation is the prefix and the :attr:`Command.qualified_name`
         optionally followed by an En dash and the command's :attr:`Command.short_doc`.
 
@@ -1188,15 +1186,15 @@
             The command to show information of.
         """
         fmt = "{0}{1} \N{EN DASH} {2}" if command.short_doc else "{0}{1}"
         self.paginator.add_line(
             fmt.format(self.context.clean_prefix, command.qualified_name, command.short_doc)
         )
 
-    def add_aliases_formatting(self, aliases):
+    def add_aliases_formatting(self, aliases) -> None:
         """Adds the formatting information on a command's aliases.
 
         The formatting should be added to the :attr:`paginator`.
 
         The default implementation is the :attr:`aliases_heading` bolded
         followed by a comma separated list of aliases.
 
@@ -1205,15 +1203,15 @@
         Parameters
         ----------
         aliases: Sequence[:class:`str`]
             A list of aliases to format.
         """
         self.paginator.add_line(f'**{self.aliases_heading}** {", ".join(aliases)}', empty=True)
 
-    def add_command_formatting(self, command):
+    def add_command_formatting(self, command) -> None:
         """A utility function to format commands and groups.
 
         Parameters
         ----------
         command: :class:`Command`
             The command to format.
         """
@@ -1240,19 +1238,19 @@
         if self.dm_help is True:
             return ctx.author
         elif self.dm_help is None and len(self.paginator) > self.dm_help_threshold:
             return ctx.author
         else:
             return ctx.channel
 
-    async def prepare_help_command(self, ctx, command):
+    async def prepare_help_command(self, ctx, command) -> None:
         self.paginator.clear()
         await super().prepare_help_command(ctx, command)
 
-    async def send_bot_help(self, mapping):
+    async def send_bot_help(self, mapping) -> None:
         ctx = self.context
         bot = ctx.bot
 
         if bot.description:
             self.paginator.add_line(bot.description, empty=True)
 
         note = self.get_opening_note()
@@ -1277,15 +1275,15 @@
         note = self.get_ending_note()
         if note:
             self.paginator.add_line()
             self.paginator.add_line(note)
 
         await self.send_pages()
 
-    async def send_cog_help(self, cog):
+    async def send_cog_help(self, cog) -> None:
         bot = self.context.bot
         if bot.description:
             self.paginator.add_line(bot.description, empty=True)
 
         note = self.get_opening_note()
         if note:
             self.paginator.add_line(note, empty=True)
@@ -1302,15 +1300,15 @@
             note = self.get_ending_note()
             if note:
                 self.paginator.add_line()
                 self.paginator.add_line(note)
 
         await self.send_pages()
 
-    async def send_group_help(self, group):
+    async def send_group_help(self, group) -> None:
         self.add_command_formatting(group)
 
         filtered = await self.filter_commands(group.commands, sort=self.sort_commands)
         if filtered:
             note = self.get_opening_note()
             if note:
                 self.paginator.add_line(note, empty=True)
@@ -1322,11 +1320,11 @@
             note = self.get_ending_note()
             if note:
                 self.paginator.add_line()
                 self.paginator.add_line(note)
 
         await self.send_pages()
 
-    async def send_command_help(self, command):
+    async def send_command_help(self, command) -> None:
         self.add_command_formatting(command)
         self.paginator.close_page()
         await self.send_pages()
```

### Comparing `disnake-2.8.2/disnake/ext/commands/interaction_bot_base.py` & `disnake-2.9.0/disnake/ext/commands/interaction_bot_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,19 +221,18 @@
     async def login(self, token: str) -> None:
         self._schedule_app_command_preparation()
 
         await super().login(token)
 
     @property
     def command_sync_flags(self) -> CommandSyncFlags:
-        """:class:`~.ext.commands.CommandSyncFlags`: The command sync flags configured for this bot.
+        """:class:`~.CommandSyncFlags`: The command sync flags configured for this bot.
 
         .. versionadded:: 2.7
         """
-
         return CommandSyncFlags._from_value(self._command_sync_flags.value)
 
     def application_commands_iterator(self) -> Iterable[InvokableApplicationCommand]:
         return chain(
             self.all_slash_commands.values(),
             self.all_user_commands.values(),
             self.all_message_commands.values(),
@@ -493,15 +492,15 @@
         options: Optional[List[Option]] = None,
         guild_ids: Optional[Sequence[int]] = None,
         connectors: Optional[Dict[str, str]] = None,
         auto_sync: Optional[bool] = None,
         extras: Optional[Dict[str, Any]] = None,
         **kwargs,
     ) -> Callable[[CommandCallback], InvokableSlashCommand]:
-        """A shortcut decorator that invokes :func:`.slash_command` and adds it to
+        """A shortcut decorator that invokes :func:`~disnake.ext.commands.slash_command` and adds it to
         the internal command list.
 
         Parameters
         ----------
         name: Optional[Union[:class:`str`, :class:`.Localized`]]
             The name of the slash command (defaults to function name).
 
@@ -586,15 +585,15 @@
         guild_ids: Optional[Sequence[int]] = None,
         auto_sync: Optional[bool] = None,
         extras: Optional[Dict[str, Any]] = None,
         **kwargs,
     ) -> Callable[
         [InteractionCommandCallback[CogT, UserCommandInteraction, P]], InvokableUserCommand
     ]:
-        """A shortcut decorator that invokes :func:`.user_command` and adds it to
+        """A shortcut decorator that invokes :func:`~disnake.ext.commands.user_command` and adds it to
         the internal command list.
 
         Parameters
         ----------
         name: Optional[Union[:class:`str`, :class:`.Localized`]]
             The name of the user command (defaults to function name).
 
@@ -663,15 +662,15 @@
         guild_ids: Optional[Sequence[int]] = None,
         auto_sync: Optional[bool] = None,
         extras: Optional[Dict[str, Any]] = None,
         **kwargs,
     ) -> Callable[
         [InteractionCommandCallback[CogT, MessageCommandInteraction, P]], InvokableMessageCommand
     ]:
-        """A shortcut decorator that invokes :func:`.message_command` and adds it to
+        """A shortcut decorator that invokes :func:`~disnake.ext.commands.message_command` and adds it to
         the internal command list.
 
         Parameters
         ----------
         name: Optional[Union[:class:`str`, :class:`.Localized`]]
             The name of the message command (defaults to function name).
 
@@ -820,15 +819,17 @@
 
             if update_required:
                 # Notice that we don't do any API requests if there're no changes.
                 to_send = _get_to_send_from_diff(diff)
                 try:
                     await self.bulk_overwrite_global_commands(to_send)
                 except Exception as e:
-                    warnings.warn(f"Failed to overwrite global commands due to {e}", SyncWarning)
+                    warnings.warn(
+                        f"Failed to overwrite global commands due to {e}", SyncWarning, stacklevel=1
+                    )
 
         # Same process but for each specified guild individually.
         # Notice that we're not doing this for every single guild for optimisation purposes.
         # See the note in :meth:`_cache_application_commands` about guild app commands.
         if self._command_sync_flags.sync_guild_commands:
             for guild_id, cmds in guild_cmds.items():
                 current_guild_cmds = self._connection._guild_application_commands.get(guild_id, {})
@@ -853,14 +854,15 @@
                     to_send = _get_to_send_from_diff(diff)
                     try:
                         await self.bulk_overwrite_guild_commands(guild_id, to_send)
                     except Exception as e:
                         warnings.warn(
                             f"Failed to overwrite commands in <Guild id={guild_id}> due to {e}",
                             SyncWarning,
+                            stacklevel=1,
                         )
         # Last debug message
         self._log_sync_debug("Command synchronization task has finished")
 
     def _log_sync_debug(self, text: str) -> None:
         if self._command_sync_flags.sync_commands_debug:
             # if sync debugging is enabled, *always* output logs
@@ -946,15 +948,15 @@
         )
 
     async def on_user_command_error(
         self, interaction: ApplicationCommandInteraction, exception: errors.CommandError
     ) -> None:
         """|coro|
 
-        Similar to :meth:`on_slash_command_error` but for user commands.
+        Similar to :meth:`on_slash_command_error() <Bot.on_slash_command_error>` but for user commands.
         """
         if self.extra_events.get("on_user_command_error", None):
             return
         command = interaction.application_command
         if command and command.has_error_handler():
             return
         cog = command.cog
@@ -966,15 +968,15 @@
         )
 
     async def on_message_command_error(
         self, interaction: ApplicationCommandInteraction, exception: errors.CommandError
     ) -> None:
         """|coro|
 
-        Similar to :meth:`on_slash_command_error` but for message commands.
+        Similar to :meth:`on_slash_command_error() <Bot.on_slash_command_error>` but for message commands.
         """
         if self.extra_events.get("on_message_command_error", None):
             return
         command = interaction.application_command
         if command and command.has_error_handler():
             return
         cog = command.cog
@@ -1005,15 +1007,15 @@
         the check won't be added.
 
         Parameters
         ----------
         func
             The function that will be used as a global check.
         call_once: :class:`bool`
-            Whether the function should only be called once per :meth:`.InvokableApplicationCommand.invoke` call.
+            Whether the function should only be called once per invoke call.
         slash_commands: :class:`bool`
             Whether this check is for slash commands.
         user_commands: :class:`bool`
             Whether this check is for user commands.
         message_commands: :class:`bool`
             Whether this check is for message commands.
         """
@@ -1129,16 +1131,15 @@
         slash_commands: bool = False,
         user_commands: bool = False,
         message_commands: bool = False,
     ) -> Callable[
         [Callable[[ApplicationCommandInteraction], Any]],
         Callable[[ApplicationCommandInteraction], Any],
     ]:
-        """
-        A decorator that adds a global application command check to the bot.
+        """A decorator that adds a global application command check to the bot.
 
         A global check is similar to a :func:`check` that is applied
         on a per command basis except it is run before any application command checks
         have been verified and applies to every application command the bot has.
 
         .. note::
 
@@ -1156,15 +1157,15 @@
             @bot.application_command_check()
             def check_app_commands(inter):
                 return inter.channel_id in whitelisted_channels
 
         Parameters
         ----------
         call_once: :class:`bool`
-            Whether the function should only be called once per :meth:`.InvokableApplicationCommand.invoke` call.
+            Whether the function should only be called once per invoke call.
         slash_commands: :class:`bool`
             Whether this check is for slash commands.
         user_commands: :class:`bool`
             Whether this check is for user commands.
         message_commands: :class:`bool`
             Whether this check is for message commands.
         """
@@ -1187,15 +1188,14 @@
             return func
 
         return decorator
 
     async def application_command_can_run(
         self, inter: ApplicationCommandInteraction, *, call_once: bool = False
     ) -> bool:
-
         if inter.data.type is ApplicationCommandType.chat_input:
             checks = self._slash_command_check_once if call_once else self._slash_command_checks
 
         elif inter.data.type is ApplicationCommandType.user:
             checks = self._user_command_check_once if call_once else self._user_command_checks
 
         elif inter.data.type is ApplicationCommandType.message:
@@ -1207,24 +1207,26 @@
         if len(checks) == 0:
             return True
 
         return await disnake.utils.async_all(f(inter) for f in checks)
 
     def before_slash_command_invoke(self, coro: CFT) -> CFT:
         """Similar to :meth:`Bot.before_invoke` but for slash commands,
-        and it takes an :class:`.ApplicationCommandInteraction` as its only parameter."""
+        and it takes an :class:`.ApplicationCommandInteraction` as its only parameter.
+        """
         if not asyncio.iscoroutinefunction(coro):
             raise TypeError("The pre-invoke hook must be a coroutine.")
 
         self._before_slash_command_invoke = coro
         return coro
 
     def after_slash_command_invoke(self, coro: CFT) -> CFT:
         """Similar to :meth:`Bot.after_invoke` but for slash commands,
-        and it takes an :class:`.ApplicationCommandInteraction` as its only parameter."""
+        and it takes an :class:`.ApplicationCommandInteraction` as its only parameter.
+        """
         if not asyncio.iscoroutinefunction(coro):
             raise TypeError("The post-invoke hook must be a coroutine.")
 
         self._after_slash_command_invoke = coro
         return coro
 
     def before_user_command_invoke(self, coro: CFT) -> CFT:
@@ -1301,15 +1303,14 @@
         you should invoke this coroutine as well.
 
         Parameters
         ----------
         interaction: :class:`disnake.ApplicationCommandInteraction`
             The interaction to process commands for.
         """
-
         # This usually comes from the blind spots of the sync algorithm.
         # Since not all guild commands are cached, it is possible to experience such issues.
         # In this case, the blind spot is the interaction guild, let's fix it:
         if (
             # if we're not currently syncing,
             not self._sync_queued.locked()
             # and we're instructed to sync guild commands
```

### Comparing `disnake-2.8.2/disnake/ext/commands/params.py` & `disnake-2.9.0/disnake/ext/commands/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,36 +6,38 @@
 
 import asyncio
 import collections.abc
 import inspect
 import itertools
 import math
 import sys
+from abc import ABC, abstractmethod
+from dataclasses import dataclass
 from enum import Enum, EnumMeta
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     Dict,
     Final,
     FrozenSet,
     Generic,
     List,
     Literal,
+    NoReturn,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
     get_type_hints,
-    overload,
 )
 
 import disnake
 from disnake.app_commands import Option, OptionChoice
 from disnake.channel import _channel_type_factory
 from disnake.enums import ChannelType, OptionType, try_enum_to_int
 from disnake.ext import commands
@@ -117,15 +119,15 @@
         else:
             # Other type hint specializations are not supported
             return False
     return issubclass(obj, tp)
 
 
 def remove_optionals(annotation: Any) -> Any:
-    """remove unwanted optionals from an annotation"""
+    """Remove unwanted optionals from an annotation"""
     if get_origin(annotation) in (Union, UnionType):
         args = tuple(i for i in annotation.__args__ if i not in (None, type(None)))
         if len(args) == 1:
             annotation = args[0]
         else:
             annotation = Union[args]  # type: ignore
 
@@ -147,21 +149,21 @@
 
     signature = inspect.signature(func)
     parameters = []
 
     for name, param in signature.parameters.items():
         if isinstance(param.annotation, str):
             param = param.replace(annotation=typehints.get(name, inspect.Parameter.empty))
-        if param.annotation is type(None):  # noqa: E721
+        if param.annotation is type(None):
             param = param.replace(annotation=None)
 
         parameters.append(param)
 
     return_annotation = typehints.get("return", inspect.Parameter.empty)
-    if return_annotation is type(None):  # noqa: E721
+    if return_annotation is type(None):
         return_annotation = None
 
     return signature.replace(parameters=parameters, return_annotation=return_annotation)
 
 
 def _xt_to_xe(xe: Optional[float], xt: Optional[float], direction: float = 1) -> Optional[float]:
     """Function for combining xt and xe
@@ -275,143 +277,171 @@
             classify_autocompleter(func)
             self.autocompleters[option_name] = func
             return func
 
         return decorator
 
 
-class RangeMeta(type):
-    """Custom Generic implementation for Range"""
-
-    @overload
-    def __getitem__(
-        self, args: Tuple[Union[int, EllipsisType], Union[int, EllipsisType]]
-    ) -> Type[int]:
-        ...
-
-    @overload
-    def __getitem__(
-        self, args: Tuple[Union[float, EllipsisType], Union[float, EllipsisType]]
-    ) -> Type[float]:
-        ...
+@dataclass(frozen=True)
+class _BaseRange(ABC):
+    """Internal base type for supporting ``Range[...]`` and ``String[...]``."""
+
+    _allowed_types: ClassVar[Tuple[Type[Any], ...]]
+
+    underlying_type: Type[Any]
+    min_value: Optional[Union[int, float]]
+    max_value: Optional[Union[int, float]]
+
+    def __class_getitem__(cls, params: Tuple[Any, ...]) -> Self:
+        # deconstruct type arguments
+        if not isinstance(params, tuple):
+            params = (params,)
+
+        name = cls.__name__
+
+        if len(params) == 2:
+            # backwards compatibility for `Range[1, 2]`
+
+            # FIXME: the warning context is incorrect when used with stringified annotations,
+            # and points to the eval frame instead of user code
+            disnake.utils.warn_deprecated(
+                f"Using `{name}` without an explicit type argument is deprecated, "
+                "as this form does not work well with modern type-checkers. "
+                f"Use `{name}[<type>, <min>, <max>]` instead.",
+                stacklevel=2,
+            )
 
-    def __getitem__(self, args: Tuple[Any, ...]) -> Any:
-        a, b = [None if isinstance(x, type(Ellipsis)) else x for x in args]
-        return Range.create(min_value=a, max_value=b)
+            # infer type from min/max values
+            params = (cls._infer_type(params),) + params
 
+        if len(params) != 3:
+            raise TypeError(
+                f"`{name}` expects 3 type arguments ({name}[<type>, <min>, <max>]), got {len(params)}"
+            )
 
-class Range(type, metaclass=RangeMeta):
-    """Type depicting a limited range of allowed values.
+        underlying_type, min_value, max_value = params
 
-    See :ref:`param_ranges` for more information.
+        # validate type (argument 1)
+        if not isinstance(underlying_type, type):
+            raise TypeError(f"First `{name}` argument must be a type, not `{underlying_type!r}`")
+
+        if not issubclass(underlying_type, cls._allowed_types):
+            allowed = "/".join(t.__name__ for t in cls._allowed_types)
+            raise TypeError(f"First `{name}` argument must be {allowed}, not `{underlying_type!r}`")
+
+        # validate min/max (arguments 2/3)
+        min_value = cls._coerce_bound(min_value, "min")
+        max_value = cls._coerce_bound(max_value, "max")
+
+        if min_value is None and max_value is None:
+            raise ValueError(f"`{name}` bounds cannot both be empty")
+
+        # n.b. this allows bounds to be equal, which doesn't really serve a purpose with numbers,
+        # but is still accepted by the api
+        if min_value is not None and max_value is not None and min_value > max_value:
+            raise ValueError(
+                f"`{name}` minimum ({min_value}) must be less than or equal to maximum ({max_value})"
+            )
 
-    .. versionadded:: 2.4
+        return cls(underlying_type=underlying_type, min_value=min_value, max_value=max_value)
 
-    """
+    @staticmethod
+    def _coerce_bound(value: Any, name: str) -> Optional[Union[int, float]]:
+        if value is None or isinstance(value, EllipsisType):
+            return None
+        elif isinstance(value, (int, float)):
+            if not math.isfinite(value):
+                raise ValueError(f"{name} value may not be NaN, inf, or -inf")
+            return value
+        else:
+            raise TypeError(f"{name} value must be int, float, None, or `...`, not `{type(value)}`")
 
-    min_value: Optional[float]
-    max_value: Optional[float]
+    def __repr__(self) -> str:
+        a = "..." if self.min_value is None else self.min_value
+        b = "..." if self.max_value is None else self.max_value
+        return f"{type(self).__name__}[{self.underlying_type.__name__}, {a}, {b}]"
 
-    @overload
     @classmethod
-    def create(
-        cls,
-        min_value: Optional[int] = None,
-        max_value: Optional[int] = None,
-        *,
-        le: Optional[int] = None,
-        lt: Optional[int] = None,
-        ge: Optional[int] = None,
-        gt: Optional[int] = None,
-    ) -> Type[int]:
-        ...
+    @abstractmethod
+    def _infer_type(cls, params: Tuple[Any, ...]) -> Type[Any]:
+        raise NotImplementedError
+
+    # hack to get `typing._type_check` to pass, e.g. when using `Range` as a generic parameter
+    def __call__(self) -> NoReturn:
+        raise NotImplementedError
 
-    @overload
-    @classmethod
-    def create(
-        cls,
-        min_value: Optional[float] = None,
-        max_value: Optional[float] = None,
-        *,
-        le: Optional[float] = None,
-        lt: Optional[float] = None,
-        ge: Optional[float] = None,
-        gt: Optional[float] = None,
-    ) -> Type[float]:
-        ...
+    # support new union syntax for `Range[int, 1, 2] | None`
+    if sys.version_info >= (3, 10):
 
-    @classmethod
-    def create(
-        cls,
-        min_value: Optional[float] = None,
-        max_value: Optional[float] = None,
-        *,
-        le: Optional[float] = None,
-        lt: Optional[float] = None,
-        ge: Optional[float] = None,
-        gt: Optional[float] = None,
-    ) -> Any:
-        """Construct a new range with any possible constraints"""
-        self = cls(cls.__name__, (), {})
-        self.min_value = min_value if min_value is not None else _xt_to_xe(le, lt, -1)
-        self.max_value = max_value if max_value is not None else _xt_to_xe(ge, gt, 1)
-        return self
+        def __or__(self, other):
+            return Union[self, other]  # type: ignore
 
-    @property
-    def underlying_type(self) -> Union[Type[int], Type[float]]:
-        if isinstance(self.min_value, float) or isinstance(self.max_value, float):
-            return float
 
-        return int
-
-    def __repr__(self) -> str:
-        a = "..." if self.min_value is None else self.min_value
-        b = "..." if self.max_value is None else self.max_value
-        return f"{type(self).__name__}[{a}, {b}]"
+if TYPE_CHECKING:
+    # aliased import since mypy doesn't understand `Range = Annotated`
+    from typing_extensions import Annotated as Range, Annotated as String
+else:
 
+    @dataclass(frozen=True, repr=False)
+    class Range(_BaseRange):
+        """Type representing a number with a limited range of allowed values.
 
-class StringMeta(type):
-    """Custom Generic implementation for String."""
+        See :ref:`param_ranges` for more information.
 
-    def __getitem__(
-        self, args: Tuple[Union[int, EllipsisType], Union[int, EllipsisType]]
-    ) -> Type[str]:
-        a, b = [None if isinstance(x, EllipsisType) else x for x in args]
-        return String.create(min_length=a, max_length=b)
+        .. versionadded:: 2.4
 
+        .. versionchanged:: 2.9
+            Syntax changed from ``Range[5, 10]`` to ``Range[int, 5, 10]``;
+            the type (:class:`int` or :class:`float`) must now be specified explicitly.
+        """
 
-class String(type, metaclass=StringMeta):
-    """Type depicting a string option with limited length.
+        _allowed_types = (int, float)
 
-    See :ref:`string_lengths` for more information.
+        def __post_init__(self):
+            for value in (self.min_value, self.max_value):
+                if value is None:
+                    continue
+
+                if self.underlying_type is int and not isinstance(value, int):
+                    raise TypeError("Range[int, ...] bounds must be int, not float")
+
+        @classmethod
+        def _infer_type(cls, params: Tuple[Any, ...]) -> Type[Any]:
+            if any(isinstance(p, float) for p in params):
+                return float
+            return int
+
+    @dataclass(frozen=True, repr=False)
+    class String(_BaseRange):
+        """Type representing a string option with a limited length.
 
-    .. versionadded:: 2.6
+        See :ref:`string_lengths` for more information.
 
-    """
+        .. versionadded:: 2.6
 
-    min_length: Optional[int]
-    max_length: Optional[int]
-    underlying_type: Final[Type[str]] = str
+        .. versionchanged:: 2.9
+            Syntax changed from ``String[5, 10]`` to ``String[str, 5, 10]``;
+            the type (:class:`str`) must now be specified explicitly.
+        """
 
-    @classmethod
-    def create(
-        cls,
-        min_length: Optional[int] = None,
-        max_length: Optional[int] = None,
-    ) -> Any:
-        """Construct a new String with constraints."""
-        self = cls(cls.__name__, (), {})
-        self.min_length = min_length
-        self.max_length = max_length
-        return self
+        _allowed_types = (str,)
 
-    def __repr__(self) -> str:
-        a = "..." if self.min_length is None else self.min_length
-        b = "..." if self.max_length is None else self.max_length
-        return f"{type(self).__name__}[{a}, {b}]"
+        def __post_init__(self):
+            for value in (self.min_value, self.max_value):
+                if value is None:
+                    continue
+
+                if not isinstance(value, int):
+                    raise TypeError("String bounds must be int, not float")
+                if value < 0:
+                    raise ValueError("String bounds may not be negative")
+
+        @classmethod
+        def _infer_type(cls, params: Tuple[Any, ...]) -> Type[Any]:
+            return str
 
 
 class LargeInt(int):
     """Type for large integers in slash commands."""
 
 
 # option types that require additional handling in verify_type
@@ -526,14 +556,39 @@
         self.channel_types = channel_types or []
         self.max_value = _xt_to_xe(le, lt, -1)
         self.min_value = _xt_to_xe(ge, gt, 1)
         self.min_length = min_length
         self.max_length = max_length
         self.large = large
 
+    def copy(self) -> ParamInfo:
+        # n. b. this method needs to be manually updated when a new attribute is added.
+        cls = self.__class__
+        ins = cls.__new__(cls)
+
+        ins.name = self.name
+        ins.name_localizations = self.name_localizations._copy()
+        ins.description = self.description
+        ins.description_localizations = self.description_localizations._copy()
+        ins.default = self.default
+        ins.param_name = self.param_name
+        ins.converter = self.converter
+        ins.convert_default = self.convert_default
+        ins.autocomplete = self.autocomplete
+        ins.choices = self.choices.copy()
+        ins.type = self.type
+        ins.channel_types = self.channel_types.copy()
+        ins.max_value = self.max_value
+        ins.min_value = self.min_value
+        ins.min_length = self.min_length
+        ins.max_length = self.max_length
+        ins.large = self.large
+
+        return ins
+
     @property
     def required(self) -> bool:
         return self.default is Ellipsis
 
     @property
     def discord_type(self) -> OptionType:
         return OptionType(self.TYPES.get(self.type, OptionType.string.value))
@@ -555,15 +610,16 @@
         type_hints: Dict[str, Any],
         parsed_docstring: Optional[Dict[str, disnake.utils._DocstringParam]] = None,
     ) -> Self:
         # hopefully repeated parsing won't cause any problems
         parsed_docstring = parsed_docstring or {}
 
         if isinstance(param.default, cls):
-            self = param.default
+            # we copy this ParamInfo instance because it can be used in multiple signatures
+            self = param.default.copy()
         else:
             default = param.default if param.default is not inspect.Parameter.empty else ...
             self = cls(default)
 
         self.parse_parameter(param)
         doc = parsed_docstring.get(param.name)
         if doc:
@@ -671,22 +727,22 @@
                 self.parse_converter_annotation(self.converter, annotation)
                 return True
 
         # short circuit if user forgot to provide annotations
         if annotation is inspect.Parameter.empty or annotation is Any:
             return False
 
-        # resolve type aliases
+        # resolve type aliases and special types
         if isinstance(annotation, Range):
             self.min_value = annotation.min_value
             self.max_value = annotation.max_value
             annotation = annotation.underlying_type
         if isinstance(annotation, String):
-            self.min_length = annotation.min_length
-            self.max_length = annotation.max_length
+            self.min_length = annotation.min_value
+            self.max_length = annotation.max_value
             annotation = annotation.underlying_type
         if issubclass_(annotation, LargeInt):
             self.large = True
             annotation = int
 
         if self.large:
             self.type = str
@@ -726,15 +782,15 @@
             raise TypeError(f"{annotation!r} is not a valid converter annotation")
         else:
             raise TypeError(f"{annotation!r} is not a valid parameter annotation")
 
         return True
 
     def parse_converter_annotation(self, converter: Callable, fallback_annotation: Any) -> None:
-        _, parameters = isolate_self(converter)
+        _, parameters = isolate_self(signature(converter))
 
         if len(parameters) != 1:
             raise TypeError(
                 "Converters must take precisely two arguments: the interaction and the argument"
             )
 
         _, parameter = parameters.popitem()
@@ -834,19 +890,17 @@
         elif parameter.name in possible_kwargs:
             kwargs[parameter.name] = possible_kwargs[parameter.name]
 
     return function(*args, **kwargs)
 
 
 def isolate_self(
-    function: Callable,
+    sig: inspect.Signature,
 ) -> Tuple[Tuple[Optional[inspect.Parameter], ...], Dict[str, inspect.Parameter]]:
     """Create parameters without self and the first interaction"""
-    sig = signature(function)
-
     parameters = dict(sig.parameters)
     parametersl = list(sig.parameters.values())
 
     if not parameters:
         return (None, None), {}
 
     cog_param: Optional[inspect.Parameter] = None
@@ -894,20 +948,28 @@
         )
 
     autocompleter.__has_cog_param__ = positional_param_count == 3
 
 
 def collect_params(
     function: Callable,
+    sig: Optional[inspect.Signature] = None,
 ) -> Tuple[Optional[str], Optional[str], List[ParamInfo], Dict[str, Injection]]:
-    """Collect all parameters in a function
+    """Collect all parameters in a function.
+
+    Optionally accepts an `inspect.Signature` object (as an optimization),
+    calls `signature(function)` if not provided.
 
     Returns: (`cog parameter`, `interaction parameter`, `param infos`, `injections`)
     """
-    (cog_param, inter_param), parameters = isolate_self(function)
+    if sig is None:
+        sig = signature(function)
+
+    (cog_param, inter_param), parameters = isolate_self(sig)
+
     doc = disnake.utils.parse_docstring(function)["params"]
 
     paraminfos: List[ParamInfo] = []
     injections: Dict[str, Injection] = {}
 
     for parameter in parameters.values():
         if parameter.kind in [parameter.VAR_POSITIONAL, parameter.VAR_KEYWORD]:
@@ -945,15 +1007,14 @@
         injections,
     )
 
 
 def collect_nested_params(function: Callable) -> List[ParamInfo]:
     """Collect all options from a function"""
     # TODO: Have these be actually sorted properly and not have injections always at the end
-
     _, _, paraminfos, injections = collect_params(function)
 
     for injection in injections.values():
         paraminfos += collect_nested_params(injection.function)
 
     return sorted(paraminfos, key=lambda param: not param.required)
 
@@ -1024,15 +1085,17 @@
 
 def expand_params(command: AnySlashCommand) -> List[Option]:
     """Update an option with its params *in-place*
 
     Returns the created options
     """
     sig = signature(command.callback)
-    _, inter_param, params, injections = collect_params(command.callback)
+    # pass `sig` down to avoid having to call `signature(func)` another time,
+    # which may cause side effects with deferred annotations and warnings
+    _, inter_param, params, injections = collect_params(command.callback, sig)
 
     if inter_param is None:
         raise TypeError(f"Couldn't find an interaction parameter in {command.callback}")
 
     for injection in injections.values():
         collected = collect_nested_params(injection.function)
         if injection.autocompleters:
@@ -1221,15 +1284,14 @@
 
         .. note::
 
             The return type is annotated with ``Any`` to avoid typing issues caused by how this
             extension works, but at runtime this is always an :class:`Injection` instance.
             You can find more in-depth explanation :ref:`here <why_params_and_injections_return_any>`.
     """
-
     return Injection(function, autocompleters=autocompleters)
 
 
 def injection(
     *,
     autocompleters: Optional[Dict[str, Callable]] = None,
 ) -> Callable[[Callable[..., Any]], Any]:
@@ -1262,16 +1324,15 @@
 
     return decorator
 
 
 def option_enum(
     choices: Union[Dict[str, TChoice], List[TChoice]], **kwargs: TChoice
 ) -> Type[TChoice]:
-    """
-    A utility function to create an enum type.
+    """A utility function to create an enum type.
     Returns a new :class:`~enum.Enum` based on the provided parameters.
 
     .. versionadded:: 2.1
 
     Parameters
     ----------
     choices: Union[Dict[:class:`str`, :class:`Any`], List[:class:`Any`]]
@@ -1317,15 +1378,15 @@
     autocompleters: Optional[Dict[str, Callable]] = None,
 ) -> Injection[P, T_]:
     """A decorator to register a global injection.
 
     .. versionadded:: 2.3
 
     .. versionchanged:: 2.6
-        Now returns :class:`disnake.ext.commands.Injection`.
+        Now returns :class:`.Injection`.
 
     .. versionchanged:: 2.6
         Added ``autocompleters`` keyword-only argument.
 
     Raises
     ------
     TypeError
```

### Comparing `disnake-2.8.2/disnake/ext/commands/slash_core.py` & `disnake-2.9.0/disnake/ext/commands/slash_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,16 +191,15 @@
         name: LocalizedOptional = None,
         description: LocalizedOptional = None,
         options: Optional[list] = None,
         connectors: Optional[dict] = None,
         extras: Optional[Dict[str, Any]] = None,
         **kwargs,
     ) -> Callable[[CommandCallback], SubCommand]:
-        """
-        A decorator that creates a subcommand in the subcommand group.
+        """A decorator that creates a subcommand in the subcommand group.
         Parameters are the same as in :class:`InvokableSlashCommand.sub_command`
 
         Returns
         -------
         Callable[..., :class:`SubCommand`]
             A decorator that converts the provided method into a SubCommand, adds it to the bot, then returns it.
         """
@@ -520,16 +519,15 @@
         name: LocalizedOptional = None,
         description: LocalizedOptional = None,
         options: Optional[list] = None,
         connectors: Optional[dict] = None,
         extras: Optional[Dict[str, Any]] = None,
         **kwargs,
     ) -> Callable[[CommandCallback], SubCommand]:
-        """
-        A decorator that creates a subcommand under the base command.
+        """A decorator that creates a subcommand under the base command.
 
         Parameters
         ----------
         name: Optional[Union[:class:`str`, :class:`.Localized`]]
             The name of the subcommand (defaults to function name).
 
             .. versionchanged:: 2.5
@@ -583,16 +581,15 @@
 
     def sub_command_group(
         self,
         name: LocalizedOptional = None,
         extras: Optional[Dict[str, Any]] = None,
         **kwargs,
     ) -> Callable[[CommandCallback], SubCommandGroup]:
-        """
-        A decorator that creates a subcommand group under the base command.
+        """A decorator that creates a subcommand group under the base command.
 
         Parameters
         ----------
         name: Optional[Union[:class:`str`, :class:`.Localized`]]
             The name of the subcommand group (defaults to function name).
 
             .. versionchanged:: 2.5
@@ -624,16 +621,15 @@
             self.children[new_func.name] = new_func
             self.body.options.append(new_func.option)
             return new_func
 
         return decorator
 
     def autocomplete(self, option_name: str) -> Callable[[Callable], Callable]:
-        """
-        A decorator that registers an autocomplete function for the specified option.
+        """A decorator that registers an autocomplete function for the specified option.
 
         Parameters
         ----------
         option_name: :class:`str`
             The name of the slash command option.
         """
         return _autocomplete(self, option_name)
```

### Comparing `disnake-2.8.2/disnake/ext/commands/view.py` & `disnake-2.9.0/disnake/ext/commands/view.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-License-Identifier: MIT
 
 from .errors import ExpectedClosingQuoteError, InvalidEndOfQuotedStringError, UnexpectedQuoteError
 
 # map from opening quotes to closing quotes
 _quotes = {
     '"': '"',
-    "‘": "’",
-    "‚": "‛",
+    "‘": "’",  # noqa: RUF001
+    "‚": "‛",  # noqa: RUF001
     "“": "”",
     "„": "‟",
     "⹂": "⹂",
     "「": "」",
     "『": "』",
     "〝": "〞",
     "﹁": "﹂",
     "﹃": "﹄",
-    "＂": "＂",
+    "＂": "＂",  # noqa: RUF001
     "｢": "｣",
     "«": "»",
-    "‹": "›",
+    "‹": "›",  # noqa: RUF001
     "《": "》",
     "〈": "〉",
 }
 _all_quotes = set(_quotes.keys()) | set(_quotes.values())
 
 
 class StringView:
@@ -54,15 +54,15 @@
             except IndexError:
                 break
 
         self.previous = self.index
         self.index += pos
         return self.previous != self.index
 
-    def skip_string(self, string) -> bool:
+    def skip_string(self, string: str) -> bool:
         strlen = len(string)
         if self.buffer[self.index : self.index + strlen] == string:
             self.previous = self.index
             self.index += strlen
             return True
         return False
```

### Comparing `disnake-2.8.2/disnake/ext/tasks/__init__.py` & `disnake-2.9.0/disnake/ext/tasks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,16 @@
         minutes: float = 0,
         hours: float = 0,
         time: Union[datetime.time, Sequence[datetime.time]] = MISSING,
         count: Optional[int] = None,
         reconnect: bool = True,
         loop: asyncio.AbstractEventLoop = MISSING,
     ) -> None:
-        """
-        .. note:
-            If you overwrite ``__init__`` arguments, make sure to redefine .clone too.
+        """.. note:
+        If you overwrite ``__init__`` arguments, make sure to redefine .clone too.
         """
         self.coro: LF = coro
         self.reconnect: bool = reconnect
         self.loop: asyncio.AbstractEventLoop = loop
         self.count: Optional[int] = count
         self._current_loop = 0
         self._handle: SleepHandle = MISSING
@@ -185,15 +184,15 @@
 
         except asyncio.CancelledError:
             self._is_being_cancelled = True
             raise
         except Exception as exc:
             self._has_failed = True
             await self._call_loop_function("error", exc)
-            raise exc
+            raise
         finally:
             await self._call_loop_function("after_loop")
             self._handle.cancel()
             self._is_being_cancelled = False
             self._current_loop = 0
             self._stop_next_iteration = False
             self._has_failed = False
@@ -277,16 +276,15 @@
         if self._task is MISSING:
             return None
         elif self._task and self._task.done() or self._stop_next_iteration:
             return None
         return self._next_iteration
 
     async def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        """
-        |coro|
+        """|coro|
 
         Calls the internal callback that the task holds.
 
         .. versionadded:: 1.6
 
         Parameters
         ----------
@@ -297,16 +295,15 @@
         """
         if self._injected is not None:
             args = (self._injected, *args)
 
         return await self.coro(*args, **kwargs)
 
     def start(self, *args: Any, **kwargs: Any) -> asyncio.Task[None]:
-        """
-        Starts the internal task in the event loop.
+        """Starts the internal task in the event loop.
 
         Parameters
         ----------
         *args
             The arguments to use.
         **kwargs
             The keyword arguments to use.
@@ -332,16 +329,15 @@
                 warnings.simplefilter("ignore", DeprecationWarning)
                 self.loop = asyncio.get_event_loop()
 
         self._task = self.loop.create_task(self._loop(*args, **kwargs))
         return self._task
 
     def stop(self) -> None:
-        """
-        Gracefully stops the task from running.
+        """Gracefully stops the task from running.
 
         Unlike :meth:`cancel`\\, this allows the task to finish its
         current iteration before gracefully exiting.
 
         .. note::
 
             If the internal function raises an error that can be
@@ -362,16 +358,15 @@
 
     def cancel(self) -> None:
         """Cancels the internal task, if it is running."""
         if self._can_be_cancelled():
             self._task.cancel()
 
     def restart(self, *args: Any, **kwargs: Any) -> None:
-        """
-        A convenience method to restart the internal task.
+        """A convenience method to restart the internal task.
 
         .. note::
 
             Due to the way this function works, the task is not
             returned like :meth:`start`.
 
         Parameters
@@ -387,16 +382,15 @@
             self.start(*args, **kwargs)
 
         if self._can_be_cancelled():
             self._task.add_done_callback(restart_when_over)
             self._task.cancel()
 
     def add_exception_type(self, *exceptions: Type[BaseException]) -> None:
-        """
-        Adds exception types to be handled during the reconnect logic.
+        """Adds exception types to be handled during the reconnect logic.
 
         By default the exception types handled are those handled by
         :meth:`disnake.Client.connect`\\, which includes a lot of internet disconnection
         errors.
 
         This function is useful if you're interacting with a 3rd party library that
         raises its own set of exceptions.
@@ -425,16 +419,15 @@
         .. note::
 
             This operation obviously cannot be undone!
         """
         self._valid_exception = ()
 
     def remove_exception_type(self, *exceptions: Type[BaseException]) -> bool:
-        """
-        Removes exception types from being handled during the reconnect logic.
+        """Removes exception types from being handled during the reconnect logic.
 
         Parameters
         ----------
         *exceptions: Type[:class:`BaseException`]
             An argument list of exception classes to handle.
 
         Returns
@@ -558,15 +551,15 @@
         ------
         TypeError
             The function was not a coroutine.
         """
         if not asyncio.iscoroutinefunction(coro):
             raise TypeError(f"Expected coroutine function, received {coro.__class__.__name__!r}.")
 
-        self._error = coro
+        self._error = coro  # type: ignore
         return coro
 
     def _get_next_sleep_time(self) -> datetime.datetime:
         if self._sleep is not MISSING:
             return self._last_iteration + datetime.timedelta(seconds=self._sleep)
 
         if self._time_index >= len(self._time):
@@ -791,15 +784,14 @@
     ValueError
         An invalid value was given.
     TypeError
         The function was not a coroutine, the ``cls`` parameter was not a subclass of ``Loop``,
         an invalid value for the ``time`` parameter was passed,
         or ``time`` parameter was passed in conjunction with relative time parameters.
     """
-
     if (origin := get_origin(cls)) is not None:
         cls = origin
 
     if not isinstance(cls, type) or not issubclass(cls, Loop):
         raise TypeError(f"cls argument must be a subclass of Loop, got {cls!r}")
 
     def decorator(func: LF) -> L_co:
```

### Comparing `disnake-2.8.2/disnake/file.py` & `disnake-2.9.0/disnake/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 import os
 from typing import TYPE_CHECKING, Optional, Union
 
 __all__ = ("File",)
 
 
 class File:
-    """
-    A parameter object used for sending file objects.
+    """A parameter object used for sending file objects.
 
     .. note::
 
         File objects are single use and are not meant to be reused in
         multiple :meth:`abc.Messageable.send`, :meth:`Message.edit`, :meth:`Interaction.send`,
         or :meth:`Interaction.edit_original_response` calls or similar methods.
```

### Comparing `disnake-2.8.2/disnake/flags.py` & `disnake-2.9.0/disnake/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,16 +279,15 @@
         elif toggle is False:
             self.value &= ~o
         else:
             raise TypeError(f"Value to set for {self.__class__.__name__} must be a bool.")
 
 
 class ListBaseFlags(BaseFlags, no_fill_flags=True):
-    """
-    A base class for flags that aren't powers of 2.
+    """A base class for flags that aren't powers of 2.
     Instead, values are used as exponents to map to powers of 2 to avoid collisions,
     and only the combined value is stored, which allows all bitwise operations to work as expected.
     """
 
     __slots__ = ()
 
     @classmethod
@@ -314,16 +313,15 @@
         return [i for i, c in enumerate(bin(self.value)[:1:-1]) if c == "1"]
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} values={self.values}>"
 
 
 class SystemChannelFlags(BaseFlags, inverted=True):
-    """
-    Wraps up a Discord system channel flag value.
+    """Wraps up a Discord system channel flag value.
 
     Similar to :class:`Permissions`\\, the properties provided are two way.
     You can set and retrieve individual bits using the properties as if they
     were regular bools. This allows you to edit the system flags easily.
 
     To construct an object you can pass keyword arguments denoting the flags
     to enable or disable.
@@ -415,14 +413,16 @@
         def __init__(
             self,
             *,
             guild_reminder_notifications: bool = ...,
             join_notification_replies: bool = ...,
             join_notifications: bool = ...,
             premium_subscriptions: bool = ...,
+            role_subscription_purchase_notification_replies: bool = ...,
+            role_subscription_purchase_notifications: bool = ...,
         ) -> None:
             ...
 
     # For some reason the flags for system channels are "inverted"
     # ergo, if they're set then it means "suppress" (off in the GUI toggle)
     # Since this is counter-intuitive from an API perspective and annoying
     # these will be inverted automatically
@@ -435,44 +435,61 @@
             self.value &= ~o
         elif toggle is False:
             self.value |= o
         else:
             raise TypeError("Value to set for SystemChannelFlags must be a bool.")
 
     @flag_value
-    def join_notifications(self):
+    def join_notifications(self) -> int:
         """:class:`bool`: Returns ``True`` if the system channel is used for member join notifications."""
-        return 1
+        return 1 << 0
 
     @flag_value
-    def premium_subscriptions(self):
+    def premium_subscriptions(self) -> int:
         """:class:`bool`: Returns ``True`` if the system channel is used for "Nitro boosting" notifications."""
-        return 2
+        return 1 << 1
 
     @flag_value
-    def guild_reminder_notifications(self):
+    def guild_reminder_notifications(self) -> int:
         """:class:`bool`: Returns ``True`` if the system channel is used for server setup helpful tips notifications.
 
         .. versionadded:: 2.0
         """
-        return 4
+        return 1 << 2
 
     @flag_value
-    def join_notification_replies(self):
+    def join_notification_replies(self) -> int:
         """:class:`bool`: Returns ``True`` if the system channel shows sticker reply
         buttons for member join notifications.
 
         .. versionadded:: 2.3
         """
-        return 8
+        return 1 << 3
+
+    @flag_value
+    def role_subscription_purchase_notifications(self):
+        """:class:`bool`: Returns ``True`` if the system channel shows role
+        subscription purchase/renewal notifications.
+
+        .. versionadded:: 2.9
+        """
+        return 1 << 4
+
+    @flag_value
+    def role_subscription_purchase_notification_replies(self):
+        """:class:`bool`: Returns ``True`` if the system channel shows sticker reply
+        buttons for role subscription purchase/renewal notifications.
+
+        .. versionadded:: 2.9
+        """
+        return 1 << 5
 
 
 class MessageFlags(BaseFlags):
-    """
-    Wraps up a Discord Message flag value.
+    """Wraps up a Discord Message flag value.
 
     See :class:`SystemChannelFlags`.
 
     .. container:: operations
 
         .. describe:: x == y
 
@@ -564,17 +581,19 @@
             self,
             *,
             crossposted: bool = ...,
             ephemeral: bool = ...,
             failed_to_mention_roles_in_thread: bool = ...,
             has_thread: bool = ...,
             is_crossposted: bool = ...,
+            is_voice_message: bool = ...,
             loading: bool = ...,
             source_message_deleted: bool = ...,
             suppress_embeds: bool = ...,
+            suppress_notifications: bool = ...,
             urgent: bool = ...,
         ) -> None:
             ...
 
     @flag_value
     def crossposted(self):
         """:class:`bool`: Returns ``True`` if the message is the original crossposted message."""
@@ -593,58 +612,76 @@
     @flag_value
     def source_message_deleted(self):
         """:class:`bool`: Returns ``True`` if the source message for this crosspost has been deleted."""
         return 1 << 3
 
     @flag_value
     def urgent(self):
-        """:class:`bool`: Returns ``True`` if the source message is an urgent message.
+        """:class:`bool`: Returns ``True`` if the message is an urgent message.
 
         An urgent message is one sent by Discord Trust and Safety.
         """
         return 1 << 4
 
     @flag_value
     def has_thread(self):
-        """:class:`bool`: Returns ``True`` if the source message is associated with a thread.
+        """:class:`bool`: Returns ``True`` if the message is associated with a thread.
 
         .. versionadded:: 2.0
         """
         return 1 << 5
 
     @flag_value
     def ephemeral(self):
-        """:class:`bool`: Returns ``True`` if the source message is ephemeral.
+        """:class:`bool`: Returns ``True`` if the message is ephemeral.
 
         .. versionadded:: 2.0
         """
         return 1 << 6
 
     @flag_value
     def loading(self):
-        """:class:`bool`: Returns ``True`` if the source message is a deferred
+        """:class:`bool`: Returns ``True`` if the message is a deferred
         interaction response and shows a "thinking" state.
 
         .. versionadded:: 2.3
         """
         return 1 << 7
 
     @flag_value
     def failed_to_mention_roles_in_thread(self):
-        """:class:`bool`: Returns ``True`` if the source message failed to
+        """:class:`bool`: Returns ``True`` if the message failed to
         mention some roles and add their members to the thread.
 
         .. versionadded:: 2.4
         """
         return 1 << 8
 
+    @flag_value
+    def suppress_notifications(self):
+        """:class:`bool`: Returns ``True`` if the message does not
+        trigger push and desktop notifications.
+
+        .. versionadded:: 2.9
+        """
+        return 1 << 12
+
+    @flag_value
+    def is_voice_message(self):
+        """:class:`bool`: Returns ``True`` if the message is a voice message.
+
+        Messages with this flag will have a single audio attachment, and no other content.
+
+        .. versionadded:: 2.9
+        """
+        return 1 << 13
+
 
 class PublicUserFlags(BaseFlags):
-    """
-    Wraps up the Discord User Public flags.
+    """Wraps up the Discord User Public flags.
 
     .. container:: operations
 
         .. describe:: x == y
 
             Checks if two PublicUserFlags instances are equal.
         .. describe:: x != y
@@ -871,16 +908,15 @@
 
     def all(self) -> List[UserFlags]:
         """List[:class:`UserFlags`]: Returns all public flags the user has."""
         return [public_flag for public_flag in UserFlags if self._has_flag(public_flag.value)]
 
 
 class Intents(BaseFlags):
-    """
-    Wraps up a Discord gateway intent flag.
+    """Wraps up a Discord gateway intent flag.
 
     Similar to :class:`Permissions`\\, the properties provided are two way.
     You can set and retrieve individual bits using the properties as if they
     were regular bools.
 
     To construct an object you can pass keyword arguments denoting the flags
     to enable or disable.
@@ -1107,14 +1143,15 @@
         - :attr:`Guild.members`
         - :attr:`Member.roles`
         - :attr:`Member.nick`
         - :attr:`Member.premium_since`
         - :attr:`User.name`
         - :attr:`User.avatar`
         - :attr:`User.discriminator`
+        - :attr:`User.global_name`
 
         For more information go to the :ref:`member intent documentation <need_members_intent>`.
 
         .. note::
 
             Currently, this requires opting in explicitly via the developer portal as well.
             Bots in over 100 guilds will need to apply to Discord for verification.
@@ -1692,25 +1729,25 @@
         return self
 
     @property
     def _empty(self):
         return self.value == self.DEFAULT_VALUE
 
     @flag_value
-    def voice(self):
+    def voice(self) -> int:
         """:class:`bool`: Whether to cache members that are in voice.
 
         This requires :attr:`Intents.voice_states`.
 
         Members that leave voice are no longer cached.
         """
         return 1
 
     @flag_value
-    def joined(self):
+    def joined(self) -> int:
         """:class:`bool`: Whether to cache members that joined the guild
         or are chunked as part of the initial log in flow.
 
         This requires :attr:`Intents.members`.
 
         Members that leave the guild are no longer cached.
         """
@@ -1748,16 +1785,15 @@
 
     @property
     def _voice_only(self):
         return self.value == 1
 
 
 class ApplicationFlags(BaseFlags):
-    """
-    Wraps up the Discord Application flags.
+    """Wraps up the Discord Application flags.
 
     .. container:: operations
 
         .. describe:: x == y
 
             Checks if two ApplicationFlags instances are equal.
         .. describe:: x != y
@@ -1842,27 +1878,33 @@
 
     if TYPE_CHECKING:
 
         @_generated
         def __init__(
             self,
             *,
+            application_auto_moderation_rule_create_badge: bool = ...,
             application_command_badge: bool = ...,
             embedded: bool = ...,
             gateway_guild_members: bool = ...,
             gateway_guild_members_limited: bool = ...,
             gateway_message_content: bool = ...,
             gateway_message_content_limited: bool = ...,
             gateway_presence: bool = ...,
             gateway_presence_limited: bool = ...,
             verification_pending_guild_limit: bool = ...,
         ) -> None:
             ...
 
     @flag_value
+    def application_auto_moderation_rule_create_badge(self):
+        """:class:`bool`: Returns ``True`` if the application uses the Auto Moderation API."""
+        return 1 << 6
+
+    @flag_value
     def gateway_presence(self):
         """:class:`bool`: Returns ``True`` if the application is verified and is allowed to
         receive presence information over the gateway.
         """
         return 1 << 12
 
     @flag_value
@@ -2031,16 +2073,15 @@
 
         .. versionadded:: 2.6
         """
         return 1 << 4
 
 
 class AutoModKeywordPresets(ListBaseFlags):
-    """
-    Wraps up the pre-defined auto moderation keyword lists, provided by Discord.
+    """Wraps up the pre-defined auto moderation keyword lists, provided by Discord.
 
     .. container:: operations
 
         .. describe:: x == y
 
             Checks if two AutoModKeywordPresets instances are equal.
         .. describe:: x != y
```

### Comparing `disnake-2.8.2/disnake/gateway.py` & `disnake-2.9.0/disnake/gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,23 +479,21 @@
             the result to the future. If ``None``, returns the data.
 
         Returns
         -------
         asyncio.Future
             A future to wait for.
         """
-
         future = self.loop.create_future()
         entry = EventListener(event=event, predicate=predicate, result=result, future=future)
         self._dispatch_listeners.append(entry)
         return future
 
     async def identify(self) -> None:
         """Sends the IDENTIFY packet."""
-
         state = self._connection
 
         payload: IdentifyCommand = {
             "op": self.IDENTIFY,
             "d": {
                 "token": self.token,
                 "properties": {
```

### Comparing `disnake-2.8.2/disnake/guild.py` & `disnake-2.9.0/disnake/guild.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     cast,
     overload,
 )
 
 from . import abc, utils
 from .app_commands import GuildApplicationCommandPermissions
 from .asset import Asset
-from .automod import AutoModRule
+from .automod import AutoModAction, AutoModRule
 from .bans import BanEntry
 from .channel import (
     CategoryChannel,
     ForumChannel,
     StageChannel,
     TextChannel,
     VoiceChannel,
@@ -62,14 +62,15 @@
 from .flags import SystemChannelFlags
 from .guild_scheduled_event import GuildScheduledEvent, GuildScheduledEventMetadata
 from .integrations import Integration, _integration_factory
 from .invite import Invite
 from .iterators import AuditLogIterator, BanIterator, MemberIterator
 from .member import Member, VoiceState
 from .mixins import Hashable
+from .onboarding import Onboarding
 from .partial_emoji import PartialEmoji
 from .permissions import PermissionOverwrite
 from .role import Role
 from .stage_instance import StageInstance
 from .sticker import GuildSticker
 from .threads import Thread, ThreadMember
 from .user import User
@@ -85,15 +86,15 @@
 VocalGuildChannel = Union[VoiceChannel, StageChannel]
 MISSING = utils.MISSING
 
 if TYPE_CHECKING:
     from .abc import Snowflake, SnowflakeTime
     from .app_commands import APIApplicationCommand
     from .asset import AssetBytes
-    from .automod import AutoModAction, AutoModTriggerMetadata
+    from .automod import AutoModTriggerMetadata
     from .permissions import Permissions
     from .state import ConnectionState
     from .template import Template
     from .threads import AnyThreadArchiveDuration, ForumTag
     from .types.channel import PermissionOverwrite as PermissionOverwritePayload
     from .types.guild import (
         Ban as BanPayload,
@@ -107,15 +108,15 @@
     from .types.role import CreateRole as CreateRolePayload
     from .types.sticker import CreateGuildSticker as CreateStickerPayload
     from .types.threads import Thread as ThreadPayload, ThreadArchiveDurationLiteral
     from .types.voice import GuildVoiceState
     from .voice_client import VoiceProtocol
     from .webhook import Webhook
 
-    GuildMessageable = Union[TextChannel, Thread, VoiceChannel]
+    GuildMessageable = Union[TextChannel, Thread, VoiceChannel, StageChannel]
     GuildChannel = Union[VoiceChannel, StageChannel, TextChannel, CategoryChannel, ForumChannel]
     ByCategoryItem = Tuple[Optional[CategoryChannel], List[GuildChannel]]
 
 
 class _GuildLimit(NamedTuple):
     emoji: int
     stickers: int
@@ -180,14 +181,19 @@
 
             This attribute is only available via :meth:`.Client.fetch_guild`.
     max_video_channel_users: Optional[:class:`int`]
         The maximum amount of users in a video channel.
 
         .. versionadded:: 1.4
 
+    max_stage_video_channel_users: Optional[:class:`int`]
+        The maximum amount of users in a stage video channel.
+
+        .. versionadded: 2.9
+
     description: Optional[:class:`str`]
         The guild's description.
     mfa_level: :class:`int`
         Indicates the guild's two-factor authentication level. If this value is 0 then
         the guild does not require 2FA for their administrative members
         to take moderation actions. If the value is 1, then 2FA is required.
     verification_level: :class:`VerificationLevel`
@@ -203,33 +209,37 @@
         A partial list of features is below:
 
         - ``ANIMATED_BANNER``: Guild can upload an animated banner.
         - ``ANIMATED_ICON``: Guild can upload an animated icon.
         - ``AUTO_MODERATION``: Guild has set up auto moderation rules.
         - ``BANNER``: Guild can upload and use a banner. (i.e. :attr:`.banner`)
         - ``COMMUNITY``: Guild is a community server.
+        - ``CREATOR_MONETIZABLE_PROVISIONAL``: Guild has enabled monetization.
+        - ``CREATOR_STORE_PAGE``: Guild has enabled the role subscription promo page.
         - ``DEVELOPER_SUPPORT_SERVER``: Guild is set as a support server in the app directory.
         - ``DISCOVERABLE``: Guild shows up in Server Discovery.
         - ``ENABLED_DISCOVERABLE_BEFORE``: Guild had Server Discovery enabled at least once.
         - ``FEATURABLE``: Guild is able to be featured in Server Discovery.
         - ``HAS_DIRECTORY_ENTRY``: Guild is listed in a student hub.
         - ``HUB``: Guild is a student hub.
         - ``INVITE_SPLASH``: Guild's invite page can have a special splash.
         - ``INVITES_DISABLED``: Guild has paused invites, preventing new users from joining.
         - ``LINKED_TO_HUB``: Guild is linked to a student hub.
         - ``MEMBER_VERIFICATION_GATE_ENABLED``: Guild has Membership Screening enabled.
-        - ``MONETIZATION_ENABLED``: Guild has enabled monetization.
         - ``MORE_EMOJI``: Guild has increased custom emoji slots.
         - ``MORE_STICKERS``: Guild has increased custom sticker slots.
         - ``NEWS``: Guild can create news channels.
         - ``NEW_THREAD_PERMISSIONS``: Guild is using the new thread permission system.
         - ``PARTNERED``: Guild is a partnered server.
         - ``PREVIEW_ENABLED``: Guild can be viewed before being accepted via Membership Screening.
         - ``PRIVATE_THREADS``: Guild has access to create private threads (no longer has any effect).
+        - ``RAID_ALERTS_DISABLED``: Guild has disabled alerts for join raids in the configured safety alerts channel.
         - ``ROLE_ICONS``: Guild has access to role icons.
+        - ``ROLE_SUBSCRIPTIONS_AVAILABLE_FOR_PURCHASE``: Guild has role subscriptions that can be purchased.
+        - ``ROLE_SUBSCRIPTIONS_ENABLED``: Guild has enabled role subscriptions.
         - ``SEVEN_DAY_THREAD_ARCHIVE``: Guild has access to the seven day archive time for threads (no longer has any effect).
         - ``TEXT_IN_VOICE_ENABLED``: Guild has text in voice channels enabled (no longer has any effect).
         - ``THREE_DAY_THREAD_ARCHIVE``: Guild has access to the three day archive time for threads (no longer has any effect).
         - ``THREADS_ENABLED``: Guild has access to threads (no longer has any effect).
         - ``TICKETED_EVENTS_ENABLED``: Guild has enabled ticketed events (no longer has any effect).
         - ``VANITY_URL``: Guild can have a vanity invite URL (e.g. discord.gg/disnake).
         - ``VERIFIED``: Guild is a verified server.
@@ -309,14 +319,15 @@
         "verification_level",
         "explicit_content_filter",
         "default_notifications",
         "description",
         "max_presences",
         "max_members",
         "max_video_channel_users",
+        "max_stage_video_channel_users",
         "premium_progress_bar_enabled",
         "premium_tier",
         "premium_subscription_count",
         "preferred_locale",
         "nsfw_level",
         "approximate_member_count",
         "approximate_presence_count",
@@ -338,14 +349,15 @@
         "_discovery_splash",
         "_rules_channel_id",
         "_public_updates_channel_id",
         "_stage_instances",
         "_scheduled_events",
         "_threads",
         "_region",
+        "_safety_alerts_channel_id",
     )
 
     _PREMIUM_GUILD_LIMITS: ClassVar[Dict[Optional[int], _GuildLimit]] = {
         None: _GuildLimit(emoji=50, stickers=5, bitrate=96e3, filesize=26214400),
         0: _GuildLimit(emoji=50, stickers=5, bitrate=96e3, filesize=26214400),
         1: _GuildLimit(emoji=100, stickers=15, bitrate=128e3, filesize=26214400),
         2: _GuildLimit(emoji=150, stickers=30, bitrate=256e3, filesize=52428800),
@@ -539,14 +551,17 @@
         self.features: List[GuildFeature] = guild.get("features", [])
         self._splash: Optional[str] = guild.get("splash")
         self._system_channel_id: Optional[int] = utils._get_as_snowflake(guild, "system_channel_id")
         self.description: Optional[str] = guild.get("description")
         self.max_presences: Optional[int] = guild.get("max_presences")
         self.max_members: Optional[int] = guild.get("max_members")
         self.max_video_channel_users: Optional[int] = guild.get("max_video_channel_users")
+        self.max_stage_video_channel_users: Optional[int] = guild.get(
+            "max_stage_video_channel_users"
+        )
         self.premium_tier: int = guild.get("premium_tier", 0)
         self.premium_subscription_count: int = guild.get("premium_subscription_count") or 0
         self._system_channel_flags: int = guild.get("system_channel_flags", 0)
         self.preferred_locale: Locale = try_enum(Locale, guild.get("preferred_locale"))
         self._discovery_splash: Optional[str] = guild.get("discovery_splash")
         self._rules_channel_id: Optional[int] = utils._get_as_snowflake(guild, "rules_channel_id")
         self._public_updates_channel_id: Optional[int] = utils._get_as_snowflake(
@@ -555,14 +570,17 @@
         self.nsfw_level: NSFWLevel = try_enum(NSFWLevel, guild.get("nsfw_level", 0))
         self.premium_progress_bar_enabled: bool = guild.get("premium_progress_bar_enabled", False)
         self.approximate_presence_count: Optional[int] = guild.get("approximate_presence_count")
         self.approximate_member_count: Optional[int] = guild.get("approximate_member_count")
         self.widget_enabled: Optional[bool] = guild.get("widget_enabled")
         self.widget_channel_id: Optional[int] = utils._get_as_snowflake(guild, "widget_channel_id")
         self.vanity_url_code: Optional[str] = guild.get("vanity_url_code")
+        self._safety_alerts_channel_id: Optional[int] = utils._get_as_snowflake(
+            guild, "safety_alerts_channel_id"
+        )
 
         stage_instances = guild.get("stage_instances")
         if stage_instances is not None:
             self._stage_instances = {}
             for s in stage_instances:
                 stage_instance = StageInstance(guild=self, data=s, state=state)
                 self._stage_instances[stage_instance.id] = stage_instance
@@ -818,40 +836,57 @@
     @property
     def system_channel_flags(self) -> SystemChannelFlags:
         """:class:`SystemChannelFlags`: Returns the guild's system channel settings."""
         return SystemChannelFlags._from_value(self._system_channel_flags)
 
     @property
     def rules_channel(self) -> Optional[TextChannel]:
-        """Optional[:class:`TextChannel`]: Return's the guild's channel used for the rules.
+        """Optional[:class:`TextChannel`]: Returns the guild's channel used for the rules.
         The guild must be a Community guild.
 
         If no channel is set, then this returns ``None``.
 
         .. versionadded:: 1.3
         """
         channel_id = self._rules_channel_id
         return channel_id and self._channels.get(channel_id)  # type: ignore
 
     @property
     def public_updates_channel(self) -> Optional[TextChannel]:
-        """Optional[:class:`TextChannel`]: Return's the guild's channel where admins and
+        """Optional[:class:`TextChannel`]: Returns the guild's channel where admins and
         moderators of the guild receive notices from Discord. The guild must be a
         Community guild.
 
         If no channel is set, then this returns ``None``.
 
         .. versionadded:: 1.4
         """
         channel_id = self._public_updates_channel_id
         return channel_id and self._channels.get(channel_id)  # type: ignore
 
     @property
+    def safety_alerts_channel(self) -> Optional[TextChannel]:
+        """Optional[:class:`TextChannel`]: Returns the guild's channel where admins and
+        moderators of the guild receive safety alerts from Discord. The guild must be a
+        Community guild.
+
+        If no channel is set, then this returns ``None``.
+
+        .. versionadded:: 2.9
+        """
+        channel_id = self._safety_alerts_channel_id
+        return channel_id and self._channels.get(channel_id)  # type: ignore
+
+    @property
     def emoji_limit(self) -> int:
-        """:class:`int`: The maximum number of emoji slots this guild has."""
+        """:class:`int`: The maximum number of emoji slots this guild has.
+
+        Premium emojis (i.e. those associated with subscription roles) count towards a
+        separate limit of 25.
+        """
         more_emoji = 200 if "MORE_EMOJI" in self.features else 50
         return max(more_emoji, self._PREMIUM_GUILD_LIMITS[self.premium_tier].emoji)
 
     @property
     def sticker_limit(self) -> int:
         """:class:`int`: The maximum number of sticker slots this guild has.
 
@@ -859,15 +894,16 @@
         """
         more_stickers = 60 if "MORE_STICKERS" in self.features else 0
         return max(more_stickers, self._PREMIUM_GUILD_LIMITS[self.premium_tier].stickers)
 
     @property
     def bitrate_limit(self) -> float:
         """:class:`float`: The maximum bitrate for voice channels this guild can have.
-        For stage channels, the maximum bitrate is 64000."""
+        For stage channels, the maximum bitrate is 64000.
+        """
         vip_guild = self._PREMIUM_GUILD_LIMITS[3].bitrate if "VIP_REGIONS" in self.features else 0
         return max(vip_guild, self._PREMIUM_GUILD_LIMITS[self.premium_tier].bitrate)
 
     @property
     def filesize_limit(self) -> int:
         """:class:`int`: The maximum number of bytes files can have when uploaded to this guild."""
         return self._PREMIUM_GUILD_LIMITS[self.premium_tier].filesize
@@ -1095,55 +1131,53 @@
     def created_at(self) -> datetime.datetime:
         """:class:`datetime.datetime`: Returns the guild's creation time in UTC."""
         return utils.snowflake_time(self.id)
 
     def get_member_named(self, name: str, /) -> Optional[Member]:
         """Returns the first member found that matches the name provided.
 
-        The name can have an optional discriminator argument, e.g. "Jake#0001"
-        or "Jake" will both do the lookup. However the former will give a more
-        precise result. Note that the discriminator must have all 4 digits
-        for this to work.
-
-        If a nickname is passed, then it is looked up via the nickname. Note
-        however, that a nickname + discriminator combo will not lookup the nickname
-        but rather the username + discriminator combo due to nickname + discriminator
-        not being unique.
+        The lookup strategy is as follows (in order):
+
+        1. Lookup by nickname.
+        2. Lookup by global name.
+        3. Lookup by username.
+
+        The name can have an optional discriminator argument, e.g. "Jake#0001",
+        in which case it will be treated as a username + discriminator combo
+        (note: this only works with usernames, not nicknames).
 
         If no member is found, ``None`` is returned.
 
+        .. versionchanged:: 2.9
+            Now takes :attr:`User.global_name` into account.
+
         Parameters
         ----------
         name: :class:`str`
-            The name of the member to lookup with an optional discriminator.
+            The name of the member to lookup (with an optional discriminator).
 
         Returns
         -------
         Optional[:class:`Member`]
             The member in this guild with the associated name. If not found
             then ``None`` is returned.
         """
-        result = None
-        members = self.members
-        if len(name) > 5 and name[-5] == "#":
-            # The 5 length is checking to see if #0000 is in the string,
-            # as a#0000 has a length of 6, the minimum for a potential
-            # discriminator lookup.
-            potential_discriminator = name[-4:]
-
-            # do the actual lookup and return if found
-            # if it isn't found then we'll do a full name lookup below.
-            result = utils.get(members, name=name[:-5], discriminator=potential_discriminator)
+        username, _, discriminator = name.rpartition("#")
+        if username and (
+            discriminator == "0" or (len(discriminator) == 4 and discriminator.isdecimal())
+        ):
+            # legacy behavior
+            result = utils.get(self._members.values(), name=username, discriminator=discriminator)
             if result is not None:
                 return result
 
         def pred(m: Member) -> bool:
-            return m.nick == name or m.name == name
+            return m.nick == name or m.global_name == name or m.name == name
 
-        return utils.find(pred, members)
+        return utils.find(pred, self._members.values())
 
     def _create_channel(
         self,
         name: str,
         channel_type: ChannelType,
         overwrites: Dict[Union[Role, Member], PermissionOverwrite] = MISSING,
         category: Optional[Snowflake] = None,
@@ -1213,15 +1247,14 @@
             will be required to update the position of the channel in the channel list.
 
         .. versionchanged:: 2.6
             Raises :exc:`TypeError` instead of ``InvalidArgument``.
 
         Examples
         --------
-
         Creating a basic channel:
 
         .. code-block:: python3
 
             channel = await guild.create_text_channel('cool-channel')
 
         Creating a "secret" channel:
@@ -1335,24 +1368,24 @@
         self._channels[channel.id] = channel
         return channel
 
     async def create_voice_channel(
         self,
         name: str,
         *,
-        reason: Optional[str] = None,
         category: Optional[CategoryChannel] = None,
         position: int = MISSING,
         bitrate: int = MISSING,
         user_limit: int = MISSING,
         rtc_region: Optional[Union[str, VoiceRegion]] = MISSING,
         video_quality_mode: VideoQualityMode = MISSING,
         nsfw: bool = MISSING,
         slowmode_delay: int = MISSING,
         overwrites: Dict[Union[Role, Member], PermissionOverwrite] = MISSING,
+        reason: Optional[str] = None,
     ) -> VoiceChannel:
         """|coro|
 
         This is similar to :meth:`create_text_channel` except makes a :class:`VoiceChannel` instead.
 
         .. versionchanged:: 2.6
             Raises :exc:`TypeError` instead of ``InvalidArgument``.
@@ -1455,17 +1488,21 @@
     async def create_stage_channel(
         self,
         name: str,
         *,
         topic: Optional[str] = MISSING,
         position: int = MISSING,
         bitrate: int = MISSING,
+        user_limit: int = MISSING,
+        rtc_region: Optional[Union[str, VoiceRegion]] = MISSING,
+        video_quality_mode: VideoQualityMode = MISSING,
         overwrites: Dict[Union[Role, Member], PermissionOverwrite] = MISSING,
         category: Optional[CategoryChannel] = None,
-        rtc_region: Optional[Union[str, VoiceRegion]] = MISSING,
+        nsfw: bool = MISSING,
+        slowmode_delay: int = MISSING,
         reason: Optional[str] = None,
     ) -> StageChannel:
         """|coro|
 
         This is similar to :meth:`create_text_channel` except makes a :class:`StageChannel` instead.
 
         .. versionadded:: 1.7
@@ -1501,14 +1538,27 @@
 
         rtc_region: Optional[Union[:class:`str`, :class:`VoiceRegion`]]
             The region for the stage channel's voice communication.
             A value of ``None`` indicates automatic voice region detection.
 
             .. versionadded:: 2.5
 
+        nsfw: :class:`bool`
+            Whether to mark the channel as NSFW.
+
+            .. versionadded:: 2.9
+
+        slowmode_delay: :class:`int`
+            Specifies the slowmode rate limit for users in this channel, in seconds.
+            A value of ``0`` disables slowmode. The maximum value possible is ``21600``.
+            If not provided, slowmode is disabled.
+
+            .. versionadded:: 2.9
+
+
         reason: Optional[:class:`str`]
             The reason for creating this channel. Shows up on the audit log.
 
         Raises
         ------
         Forbidden
             You do not have the proper permissions to create this channel.
@@ -1526,20 +1576,32 @@
 
         if topic is not MISSING:
             options["topic"] = topic
 
         if bitrate is not MISSING:
             options["bitrate"] = bitrate
 
+        if user_limit is not MISSING:
+            options["user_limit"] = user_limit
+
         if position is not MISSING:
             options["position"] = position
 
         if rtc_region is not MISSING:
             options["rtc_region"] = None if rtc_region is None else str(rtc_region)
 
+        if video_quality_mode is not MISSING:
+            options["video_quality_mode"] = video_quality_mode.value
+
+        if nsfw is not MISSING:
+            options["nsfw"] = nsfw
+
+        if slowmode_delay is not MISSING:
+            options["rate_limit_per_user"] = slowmode_delay
+
         data = await self._create_channel(
             name,
             overwrites=overwrites,
             channel_type=ChannelType.stage_voice,
             category=category,
             reason=reason,
             **options,
@@ -1793,30 +1855,31 @@
         description: Optional[str] = MISSING,
         icon: Optional[AssetBytes] = MISSING,
         banner: Optional[AssetBytes] = MISSING,
         splash: Optional[AssetBytes] = MISSING,
         discovery_splash: Optional[AssetBytes] = MISSING,
         community: bool = MISSING,
         invites_disabled: bool = MISSING,
+        raid_alerts_disabled: bool = MISSING,
         afk_channel: Optional[VoiceChannel] = MISSING,
         owner: Snowflake = MISSING,
         afk_timeout: int = MISSING,
         default_notifications: NotificationLevel = MISSING,
         verification_level: VerificationLevel = MISSING,
         explicit_content_filter: ContentFilter = MISSING,
         vanity_code: str = MISSING,
         system_channel: Optional[TextChannel] = MISSING,
         system_channel_flags: SystemChannelFlags = MISSING,
         preferred_locale: Locale = MISSING,
         rules_channel: Optional[TextChannel] = MISSING,
         public_updates_channel: Optional[TextChannel] = MISSING,
+        safety_alerts_channel: Optional[TextChannel] = MISSING,
         premium_progress_bar_enabled: bool = MISSING,
     ) -> Guild:
-        """
-        |coro|
+        """|coro|
 
         Edits the guild.
 
         You must have :attr:`~Permissions.manage_guild` permission
         to use this.
 
         .. versionchanged:: 1.4
@@ -1886,14 +1949,24 @@
             This is only available to guilds that contain ``COMMUNITY``
             in :attr:`Guild.features`.
 
             This cannot be changed at the same time as the ``community`` feature due a Discord API limitation.
 
             .. versionadded:: 2.6
 
+        raid_alerts_disabled: :class:`bool`
+            Whether the guild has disabled join raid alerts.
+
+            This is only available to guilds that contain ``COMMUNITY``
+            in :attr:`Guild.features`.
+
+            This cannot be changed at the same time as the ``community`` feature due a Discord API limitation.
+
+            .. versionadded:: 2.9
+
         afk_channel: Optional[:class:`VoiceChannel`]
             The new channel that is the AFK channel. Could be ``None`` for no AFK channel.
         afk_timeout: :class:`int`
             The number of seconds until someone is moved to the AFK channel.
             This can be set to ``60``, ``300``, ``900``, ``1800``, and ``3600``.
         owner: :class:`Member`
             The new owner of the guild to transfer ownership to. Note that you must
@@ -1920,14 +1993,21 @@
             The new channel that is used for rules. This is only available to
             guilds that contain ``COMMUNITY`` in :attr:`Guild.features`. Could be ``None`` for no rules
             channel.
         public_updates_channel: Optional[:class:`TextChannel`]
             The new channel that is used for public updates from Discord. This is only available to
             guilds that contain ``COMMUNITY`` in :attr:`Guild.features`. Could be ``None`` for no
             public updates channel.
+        safety_alerts_channel: Optional[:class:`TextChannel`]
+            The new channel that is used for safety alerts. This is only available to
+            guilds that contain ``COMMUNITY`` in :attr:`Guild.features`. Could be ``None`` for no
+            safety alerts channel.
+
+            .. versionadded:: 2.9
+
         premium_progress_bar_enabled: :class:`bool`
             Whether the server boost progress bar is enabled.
         reason: Optional[:class:`str`]
             The reason for editing this guild. Shows up on the audit log.
 
         Raises
         ------
@@ -1942,15 +2022,15 @@
             is a lottie sticker (see :func:`Sticker.read`),
             or one of the parameters ``default_notifications``, ``verification_level``,
             ``explicit_content_filter``, or ``system_channel_flags`` was of the incorrect type.
         ValueError
             ``community`` was set without setting both ``rules_channel`` and ``public_updates_channel`` parameters,
             or if you are not the owner of the guild and request an ownership transfer,
             or the image format passed in to ``icon`` is invalid,
-            or both ``community`` and ``invites_disabled`` were provided.
+            or both ``community`` and ``invites_disabled` or ``raid_alerts_disabled`` were provided.
 
         Returns
         -------
         :class:`Guild`
             The newly updated guild. Note that this has the same limitations as
             mentioned in :meth:`Client.fetch_guild` and may not have full data.
         """
@@ -2009,14 +2089,20 @@
 
         if public_updates_channel is not MISSING:
             if public_updates_channel is None:
                 fields["public_updates_channel_id"] = public_updates_channel
             else:
                 fields["public_updates_channel_id"] = public_updates_channel.id
 
+        if safety_alerts_channel is not MISSING:
+            if safety_alerts_channel is None:
+                fields["safety_alerts_channel_id"] = safety_alerts_channel
+            else:
+                fields["safety_alerts_channel_id"] = safety_alerts_channel.id
+
         if owner is not MISSING:
             if self.owner_id != self._state.self_id:
                 raise ValueError("To transfer ownership you must be the owner of the guild.")
 
             fields["owner_id"] = owner.id
 
         if verification_level is not MISSING:
@@ -2033,15 +2119,19 @@
 
         if system_channel_flags is not MISSING:
             if not isinstance(system_channel_flags, SystemChannelFlags):
                 raise TypeError("system_channel_flags field must be of type SystemChannelFlags")
 
             fields["system_channel_flags"] = system_channel_flags.value
 
-        if community is not MISSING or invites_disabled is not MISSING:
+        if (
+            community is not MISSING
+            or invites_disabled is not MISSING
+            or raid_alerts_disabled is not MISSING
+        ):
             # If we don't have complete feature information for the guild,
             # it is possible to disable or enable other features that we didn't intend to touch.
             # To enable or disable a feature, we will need to provide all of the existing features in advance.
             if self.unavailable:
                 raise RuntimeError(
                     "cannot modify features of an unavailable guild due to potentially destructive results."
                 )
@@ -2068,14 +2158,27 @@
                 if not isinstance(invites_disabled, bool):
                     raise TypeError("invites_disabled must be a bool")
                 if invites_disabled:
                     features.add("INVITES_DISABLED")
                 else:
                     features.discard("INVITES_DISABLED")
 
+            if raid_alerts_disabled is not MISSING:
+                if community is not MISSING:
+                    raise ValueError(
+                        "cannot modify both the COMMUNITY feature and RAID_ALERTS_DISABLED feature at the "
+                        "same time due to a discord limitation."
+                    )
+                if not isinstance(raid_alerts_disabled, bool):
+                    raise TypeError("raid_alerts_disabled must be a bool")
+                if raid_alerts_disabled:
+                    features.add("RAID_ALERTS_DISABLED")
+                else:
+                    features.discard("RAID_ALERTS_DISABLED")
+
             fields["features"] = list(features)
 
         if premium_progress_bar_enabled is not MISSING:
             fields["premium_progress_bar_enabled"] = premium_progress_bar_enabled
 
         data = await http.edit_guild(self.id, reason=reason, **fields)
         return Guild(data=data, state=self._state)
@@ -2353,15 +2456,14 @@
             could not be assumed from the ``channel``.
 
         Returns
         -------
         :class:`GuildScheduledEvent`
             The newly created guild scheduled event.
         """
-
         if entity_type is MISSING:
             if channel is None:
                 entity_type = GuildScheduledEventEntityType.external
             elif isinstance(channel_type := getattr(channel, "type", None), ChannelType):
                 if channel_type is ChannelType.voice:
                     entity_type = GuildScheduledEventEntityType.voice
                 elif channel_type is ChannelType.stage_voice:
@@ -2505,25 +2607,30 @@
                 payload["welcome_channels"] = welcome_channel_payload
 
         data = await self._state.http.edit_guild_welcome_screen(self.id, reason=reason, **payload)
         return WelcomeScreen(state=self._state, data=data, guild=self)
 
     # TODO: Remove Optional typing here when async iterators are refactored
     def fetch_members(
-        self, *, limit: int = 1000, after: Optional[SnowflakeTime] = None
+        self, *, limit: Optional[int] = 1000, after: Optional[SnowflakeTime] = None
     ) -> MemberIterator:
-        """Retrieves an :class:`.AsyncIterator` that enables receiving the guild's members. In order to use this,
-        :meth:`Intents.members` must be enabled.
+        """Retrieves an :class:`.AsyncIterator` that enables receiving the guild's members.
+
+        In order to use this, the :attr:`~Intents.members` intent must be
+        enabled in the developer portal.
 
         .. note::
 
             This method is an API call. For general usage, consider :attr:`members` instead.
 
         .. versionadded:: 1.3
 
+        .. versionchanged:: 2.9
+            No longer requires the intent to be enabled on the websocket connection.
+
         All parameters are optional.
 
         Parameters
         ----------
         limit: Optional[:class:`int`]
             The number of members to retrieve. Defaults to 1000.
             Pass ``None`` to fetch all members. Note that this is potentially slow.
@@ -2531,38 +2638,42 @@
             Retrieve members after this date or object.
             If a datetime is provided, it is recommended to use a UTC aware datetime.
             If the datetime is naive, it is assumed to be local time.
 
         Raises
         ------
         ClientException
-            The members intent is not enabled.
+            The members intent is not enabled in the developer portal.
         HTTPException
             Retrieving the members failed.
 
         Yields
         ------
         :class:`.Member`
             The member with the member data parsed.
 
         Examples
         --------
-
         Usage ::
 
             async for member in guild.fetch_members(limit=150):
                 print(member.name)
 
         Flattening into a list ::
 
             members = await guild.fetch_members(limit=150).flatten()
             # members is now a list of Member...
         """
-        if not self._state._intents.members:
-            raise ClientException("Intents.members must be enabled to use this.")
+        # `hasattr` check to avoid issues with uninitialized state
+        if hasattr(self._state, "application_flags"):
+            flags = self._state.application_flags
+            if not (flags.gateway_guild_members_limited or flags.gateway_guild_members):
+                raise ClientException(
+                    "The `members` intent must be enabled in the Developer Portal to be able to use this method."
+                )
 
         return MemberIterator(self, limit=limit, after=after)
 
     async def fetch_member(self, member_id: int, /) -> Member:
         """|coro|
 
         Retrieves a :class:`Member` with the given ID.
@@ -2677,16 +2788,15 @@
 
         You must have the :attr:`~Permissions.ban_members` permission to get this information.
 
         .. versionchanged:: 2.5
             Due to a breaking change in Discord's API, this now returns an :class:`~disnake.AsyncIterator` instead of a :class:`list`.
 
         Examples
-        ---------
-
+        --------
         Usage ::
 
             counter = 0
             async for ban in guild.bans(limit=200):
                 if not ban.user.bot:
                     counter += 1
 
@@ -2713,31 +2823,29 @@
         ------
         ~disnake.Forbidden
             You do not have permissions to get the bans.
         ~disnake.HTTPException
             An error occurred while fetching the bans.
 
         Yields
-        -------
+        ------
         :class:`~disnake.BanEntry`
             The ban with the ban data parsed.
         """
-
         return BanIterator(self, limit=limit, before=before, after=after)
 
     async def prune_members(
         self,
         *,
         days: int,
         compute_prune_count: bool = True,
         roles: List[Snowflake] = MISSING,
         reason: Optional[str] = None,
     ) -> Optional[int]:
-        """
-        |coro|
+        """|coro|
 
         Prunes the guild from its inactive members.
 
         The inactive members are denoted if they have not logged on in
         ``days`` number of days and they have no roles.
 
         You must have :attr:`~Permissions.kick_members` permission
@@ -3089,15 +3197,15 @@
         file: File,
         reason: Optional[str] = None,
     ) -> GuildSticker:
         """|coro|
 
         Creates a :class:`Sticker` for the guild.
 
-        You must have :attr:`~Permissions.manage_emojis_and_stickers` permission to
+        You must have :attr:`~Permissions.manage_guild_expressions` permission to
         do this.
 
         .. versionadded:: 2.0
 
         Parameters
         ----------
         name: :class:`str`
@@ -3139,15 +3247,15 @@
         return self._state.store_sticker(self, data)
 
     async def delete_sticker(self, sticker: Snowflake, *, reason: Optional[str] = None) -> None:
         """|coro|
 
         Deletes the custom :class:`Sticker` from the guild.
 
-        You must have :attr:`~Permissions.manage_emojis_and_stickers` permission to
+        You must have :attr:`~Permissions.manage_guild_expressions` permission to
         do this.
 
         .. versionadded:: 2.0
 
         Parameters
         ----------
         sticker: :class:`abc.Snowflake`
@@ -3220,46 +3328,53 @@
         self,
         *,
         name: str,
         image: AssetBytes,
         roles: Sequence[Role] = MISSING,
         reason: Optional[str] = None,
     ) -> Emoji:
-        """
-        |coro|
+        """|coro|
 
         Creates a custom :class:`Emoji` for the guild.
 
         Depending on the boost level of your guild (which can be obtained via :attr:`premium_tier`),
         the amount of custom emojis that can be created changes:
 
         .. csv-table::
             :header: "Boost level", "Max custom emoji limit"
 
             "0", "50"
             "1", "100"
             "2", "150"
             "3", "250"
 
-        You must have :attr:`~Permissions.manage_emojis` permission to
+        Emojis with subscription roles (see ``roles`` below) are considered premium emoji,
+        and count towards a separate limit of 25 emojis.
+
+        You must have :attr:`~Permissions.manage_guild_expressions` permission to
         do this.
 
         Parameters
         ----------
         name: :class:`str`
             The emoji name. Must be at least 2 characters.
         image: |resource_type|
             The image data of the emoji.
             Only JPG, PNG and GIF images are supported.
 
             .. versionchanged:: 2.5
                 Now accepts various resource types in addition to :class:`bytes`.
 
         roles: List[:class:`Role`]
-            A :class:`list` of :class:`Role`\\s that can use this emoji. Leave empty to make it available to everyone.
+            A list of roles that can use this emoji. Leave empty to make it available to everyone.
+
+            An emoji cannot have both subscription roles (see :attr:`RoleTags.integration_id`) and
+            non-subscription roles, and emojis can't be converted between premium and non-premium
+            after creation.
+
         reason: Optional[:class:`str`]
             The reason for creating this emoji. Shows up on the audit log.
 
         Raises
         ------
         NotFound
             The ``image`` asset couldn't be found.
@@ -3289,15 +3404,15 @@
         return self._state.store_emoji(self, data)
 
     async def delete_emoji(self, emoji: Snowflake, *, reason: Optional[str] = None) -> None:
         """|coro|
 
         Deletes the custom :class:`Emoji` from the guild.
 
-        You must have :attr:`~Permissions.manage_emojis` permission to
+        You must have :attr:`~Permissions.manage_guild_expressions` permission to
         do this.
 
         Parameters
         ----------
         emoji: :class:`abc.Snowflake`
             The emoji you are deleting.
         reason: Optional[:class:`str`]
@@ -3569,15 +3684,14 @@
             A list of all the roles in the guild.
         """
         if not isinstance(positions, dict):
             raise TypeError("positions parameter expects a dict.")
 
         role_positions: List[Any] = []
         for role, position in positions.items():
-
             payload = {"id": role.id, "position": position}
 
             role_positions.append(payload)
 
         data = await self._state.http.move_role_position(self.id, role_positions, reason=reason)
         roles: List[Role] = []
         for d in data:
@@ -3804,25 +3918,25 @@
         self,
         *,
         limit: Optional[int] = 100,
         before: Optional[SnowflakeTime] = None,
         after: Optional[SnowflakeTime] = None,
         user: Optional[Snowflake] = None,
         action: Optional[AuditLogAction] = None,
+        oldest_first: bool = False,
     ) -> AuditLogIterator:
         """Returns an :class:`AsyncIterator` that enables receiving the guild's audit logs.
 
         You must have :attr:`~Permissions.view_audit_log` permission to use this.
 
-        Entries are always returned in order from newest to oldest, regardless of the
-        ``before`` and ``after`` parameters.
+        Entries are returned in order from newest to oldest by default;
+        pass ``oldest_first=True`` to reverse the iteration order.
 
         Examples
         --------
-
         Getting the first 100 entries: ::
 
             async for entry in guild.audit_logs(limit=100):
                 print(f'{entry.user} did {entry.action} to {entry.target}')
 
         Getting entries for a specific action: ::
 
@@ -3834,36 +3948,40 @@
             entries = await guild.audit_logs(limit=None, user=guild.me).flatten()
             await channel.send(f'I made {len(entries)} moderation actions.')
 
         Parameters
         ----------
         limit: Optional[:class:`int`]
             The number of entries to retrieve. If ``None`` retrieve all entries.
-        before: Union[:class:`abc.Snowflake`, :class:`datetime.datetime`]
+        before: Optional[Union[:class:`abc.Snowflake`, :class:`datetime.datetime`]]
             Retrieve entries before this date or entry.
             If a datetime is provided, it is recommended to use a UTC aware datetime.
             If the datetime is naive, it is assumed to be local time.
-        after: Union[:class:`abc.Snowflake`, :class:`datetime.datetime`]
+        after: Optional[Union[:class:`abc.Snowflake`, :class:`datetime.datetime`]]
             Retrieve entries after this date or entry.
             If a datetime is provided, it is recommended to use a UTC aware datetime.
             If the datetime is naive, it is assumed to be local time.
-        user: :class:`abc.Snowflake`
+        user: Optional[:class:`abc.Snowflake`]
             The moderator to filter entries from.
-        action: :class:`AuditLogAction`
+        action: Optional[:class:`AuditLogAction`]
             The action to filter with.
+        oldest_first: :class:`bool`
+            If set to ``True``, return entries in oldest->newest order. Defaults to ``False``.
+
+            .. versionadded:: 2.9
 
         Raises
         ------
         Forbidden
             You are not allowed to fetch audit logs
         HTTPException
             An error occurred while fetching the audit logs.
 
         Yields
-        --------
+        ------
         :class:`AuditLogEntry`
             The audit log entry.
         """
         if user is not None:
             user_id = user.id
         else:
             user_id = None
@@ -3871,14 +3989,15 @@
         return AuditLogIterator(
             self,
             before=before,
             after=after,
             limit=limit,
             user_id=user_id,
             action_type=action.value if action is not None else None,
+            oldest_first=oldest_first,
         )
 
     async def widget(self) -> Widget:
         """|coro|
 
         Retrieves the widget of the guild.
 
@@ -4048,15 +4167,15 @@
 
         Raises
         ------
         ClientException
             The members intent is not enabled.
 
         Returns
-        --------
+        -------
         Optional[List[:class:`Member`]]
              Returns a list of all the members within the guild.
         """
         if not self._state._intents.members:
             raise ClientException("Intents.members must be enabled to use this.")
 
         if not self._state.is_guild_evicted(self):
@@ -4069,27 +4188,27 @@
         limit: int = 5,
         user_ids: Optional[List[int]] = None,
         presences: bool = False,
         cache: bool = True,
     ) -> List[Member]:
         """|coro|
 
-        Request members that belong to this guild whose username starts with
+        Request members that belong to this guild whose name starts with
         the query given.
 
         This is a websocket operation and can be slow.
 
         See also :func:`search_members`.
 
         .. versionadded:: 1.3
 
         Parameters
         ----------
         query: Optional[:class:`str`]
-            The string that the username's start with.
+            The string that the names start with.
         limit: :class:`int`
             The maximum number of members to send back. This must be
             a number between 5 and 100.
         presences: :class:`bool`
             Whether to request for presences to be provided. This defaults
             to ``False``.
 
@@ -4121,15 +4240,15 @@
         if presences and not self._state._intents.presences:
             raise ClientException("Intents.presences must be enabled to use this.")
 
         if query is None:
             if user_ids is None:
                 raise ValueError("Must pass either query or user_ids")
 
-        elif query == "":
+        elif not query:
             raise ValueError("Cannot pass empty query string.")
 
         elif user_ids is not None:
             raise ValueError("Cannot pass both query and user_ids")
 
         if user_ids is not None and not user_ids:
             raise ValueError("user_ids must contain at least 1 value")
@@ -4144,45 +4263,45 @@
         query: str,
         *,
         limit: int = 1,
         cache: bool = True,
     ):
         """|coro|
 
-        Retrieves members that belong to this guild whose username or nickname starts with
+        Retrieves members that belong to this guild whose name starts with
         the query given.
 
         Note that unlike :func:`query_members`, this is not a websocket operation, but an HTTP operation.
 
         See also :func:`query_members`.
 
         .. versionadded:: 2.5
 
         Parameters
-        -----------
+        ----------
         query: :class:`str`
-            The string that the usernames or nicknames start with.
+            The string that the names start with.
         limit: :class:`int`
             The maximum number of members to send back. This must be
             a number between 1 and 1000.
         cache: :class:`bool`
             Whether to cache the members internally. This makes operations
             such as :meth:`get_member` work for those that matched.
 
         Raises
-        -------
+        ------
         ValueError
             Invalid parameters were passed to the function
 
         Returns
-        --------
+        -------
         List[:class:`Member`]
             The list of members that have matched the query.
         """
-        if query == "":
+        if not query:
             raise ValueError("Cannot pass empty query string.")
         if limit < 1:
             raise ValueError("limit must be at least 1")
         limit = min(1000, limit)
         members = await self._state.http.search_guild_members(self.id, query=query, limit=limit)
         resp = []
         for member in members:
@@ -4208,33 +4327,33 @@
         If more than 100 members are missing, several websocket operations are made.
 
         Websocket operations can be slow, however, this method is cheaper than multiple :meth:`get_or_fetch_member` calls.
 
         .. versionadded:: 2.4
 
         Parameters
-        -----------
+        ----------
         user_ids: List[:class:`int`]
             List of user IDs to search for. If the user ID is not in the guild then it won't be returned.
         presences: :class:`bool`
             Whether to request for presences to be provided. Defaults to ``False``.
         cache: :class:`bool`
             Whether to cache the missing members internally. This makes operations
             such as :meth:`get_member` work for those that matched.
             It also speeds up this method on repeated calls. Defaults to ``True``.
 
         Raises
-        -------
+        ------
         asyncio.TimeoutError
             The query timed out waiting for the members.
         ClientException
             The presences intent is not enabled.
 
         Returns
-        --------
+        -------
         List[:class:`Member`]
             The list of members with the given IDs, if they exist.
         """
         if presences and not self._state._intents.presences:
             raise ClientException("Intents.presences must be enabled to use this.")
 
         members: List[Member] = []
@@ -4249,15 +4368,18 @@
 
         if not unresolved_ids:
             return members
 
         if len(unresolved_ids) == 1:
             # fetch_member is cheaper than query_members
             try:
-                members.append(await self.fetch_member(unresolved_ids[0]))
+                member = await self.fetch_member(unresolved_ids[0])
+                members.append(member)
+                if cache:
+                    self._add_member(member)
             except HTTPException:
                 pass
         else:
             # We have to split the request into several smaller requests
             # because the limit is 100 members per request.
             for i in range(0, len(unresolved_ids), 100):
                 limit = min(100, len(unresolved_ids) - i)
@@ -4409,15 +4531,14 @@
             Timing out the member failed.
 
         Returns
         -------
         :class:`Member`
             The newly updated member.
         """
-
         if not (duration is MISSING) ^ (until is MISSING):
             raise ValueError("Exactly one of `duration` and `until` must be provided")
 
         payload: Dict[str, Any] = {}
 
         if duration is not MISSING:
             if duration is None:
@@ -4508,14 +4629,17 @@
 
         The maximum number of rules for each trigger type is limited, see the
         :ddocs:`api docs <resources/auto-moderation#auto-moderation-rule-object-trigger-types>`
         for more details.
 
         .. versionadded:: 2.6
 
+        .. versionchanged:: 2.9
+            Now raises a :exc:`TypeError` if given ``actions`` have an invalid type.
+
         Parameters
         ----------
         name: :class:`str`
             The rule name.
         event_type: :class:`AutoModEventType`
             The type of events that this rule will be applied to.
         trigger_type: :class:`AutoModTriggerType`
@@ -4537,37 +4661,43 @@
             Can also include categories, in which case all channels inside that category will be exempt.
         reason: Optional[:class:`str`]
             The reason for creating the rule. Shows up on the audit log.
 
         Raises
         ------
         ValueError
-            The specified trigger type requires `trigger_metadata` to be set,
+            The specified trigger type requires ``trigger_metadata`` to be set,
             or no actions have been provided.
+        TypeError
+            The specified ``actions`` are of an invalid type.
         Forbidden
             You do not have proper permissions to create auto moderation rules.
         HTTPException
             Creating the rule failed.
 
         Returns
         -------
         :class:`AutoModRule`
             The newly created auto moderation rule.
         """
-
         trigger_type_int = try_enum_to_int(trigger_type)
         if not trigger_metadata and trigger_type_int in (
             AutoModTriggerType.keyword.value,
             AutoModTriggerType.keyword_preset.value,
             AutoModTriggerType.mention_spam.value,
         ):
             raise ValueError("Specified trigger type requires `trigger_metadata` to not be empty")
 
-        if len(actions) == 0:
+        if not actions:
             raise ValueError("At least one action must be provided.")
+        for action in actions:
+            if not isinstance(action, AutoModAction):
+                raise TypeError(
+                    f"actions must be of type `AutoModAction` (or subtype), not {type(action)!r}"
+                )
 
         data = await self._state.http.create_auto_moderation_rule(
             self.id,
             name=name,
             event_type=try_enum_to_int(event_type),
             trigger_type=trigger_type_int,
             actions=[a.to_dict() for a in actions],
@@ -4577,36 +4707,54 @@
             exempt_channels=(
                 [e.id for e in exempt_channels] if exempt_channels is not None else None
             ),
             reason=reason,
         )
         return AutoModRule(data=data, guild=self)
 
+    async def onboarding(self) -> Onboarding:
+        """|coro|
+
+        Retrieves the guild onboarding data.
+
+        .. versionadded:: 2.9
+
+        Raises
+        ------
+        HTTPException
+            Retrieving the guild onboarding data failed.
+
+        Returns
+        -------
+        :class:`Onboarding`
+            The guild onboarding data.
+        """
+        data = await self._state.http.get_guild_onboarding(self.id)
+        return Onboarding(data=data, guild=self)
+
 
 PlaceholderID = NewType("PlaceholderID", int)
 
 
 class GuildBuilder:
-    """
-    A guild builder object, created by :func:`Client.guild_builder`.
+    """A guild builder object, created by :func:`Client.guild_builder`.
 
     This allows for easier configuration of more complex guild setups,
     abstracting away some of the quirks of the guild creation endpoint.
 
     .. versionadded:: 2.8
 
     .. note::
         Many methods of this class return unspecified placeholder IDs
         (called ``PlaceholderID`` below) that can be used to reference the
         created object in other objects, for example referencing a category when
         creating a new text channel, or a role when setting permission overwrites.
 
     Examples
     --------
-
     Basic usage:
 
     .. code-block:: python3
 
         builder = client.guild_builder("Cat Pics")
         builder.add_text_channel("meow", topic="cat.")
         guild = await builder.create()
@@ -4666,15 +4814,15 @@
         The number of seconds until someone is moved to the AFK channel.
     system_channel: Optional[``PlaceholderID``]
         The channel that is used as the system channel.
     system_channel_flags: Optional[:class:`SystemChannelFlags`]
         The settings to use with the system channel.
     """
 
-    def __init__(self, *, state: ConnectionState, name: str):
+    def __init__(self, *, state: ConnectionState, name: str) -> None:
         self._state = state
         self.name: str = name
 
         # note: the first role corresponds to @everyone
         self._roles: List[CreateGuildPlaceholderRole] = []
         self._channels: List[CreateGuildPlaceholderChannel] = []
 
@@ -4790,16 +4938,15 @@
             afk_timeout=self.afk_timeout,
             system_channel=self.system_channel,
             system_channel_flags=try_enum_to_int(self.system_channel_flags),
         )
         return Guild(data=data, state=self._state)
 
     def update_everyone_role(self, *, permissions: Permissions = MISSING) -> PlaceholderID:
-        """
-        Updates attributes of the ``@everyone`` role.
+        """Updates attributes of the ``@everyone`` role.
 
         Parameters
         ----------
         permissions: :class:`Permissions`
             The permissions the role should have.
 
         Returns
@@ -4823,16 +4970,15 @@
         *,
         permissions: Permissions = MISSING,
         color: Union[Colour, int] = MISSING,
         colour: Union[Colour, int] = MISSING,
         hoist: bool = MISSING,
         mentionable: bool = MISSING,
     ) -> PlaceholderID:
-        """
-        Adds a role to the guild builder.
+        """Adds a role to the guild builder.
 
         The default (``@everyone``) role can be referenced using :attr:`everyone`
         and configured through :func:`update_everyone_role`.
 
         Parameters
         ----------
         name: :class:`str`
@@ -4886,16 +5032,15 @@
 
     def add_category(
         self,
         name: str,
         *,
         overwrites: Dict[PlaceholderID, PermissionOverwrite] = MISSING,
     ) -> PlaceholderID:
-        """
-        Adds a category channel to the guild builder.
+        """Adds a category channel to the guild builder.
 
         There is an alias for this named ``add_category_channel``.
 
         Parameters
         ----------
         name: :class:`str`
             The category's name.
@@ -4919,16 +5064,15 @@
         overwrites: Dict[PlaceholderID, PermissionOverwrite] = MISSING,
         category: PlaceholderID = MISSING,
         topic: Optional[str] = MISSING,
         slowmode_delay: int = MISSING,
         nsfw: bool = MISSING,
         default_auto_archive_duration: AnyThreadArchiveDuration = MISSING,
     ) -> PlaceholderID:
-        """
-        Adds a text channel to the guild builder.
+        """Adds a text channel to the guild builder.
 
         Parameters
         ----------
         name: :class:`str`
             The channel's name.
         overwrites: Dict[``PlaceholderID``, :class:`PermissionOverwrite`]
             A :class:`dict` of roles to :class:`PermissionOverwrite`\\s to apply to the channel.
@@ -4982,16 +5126,15 @@
         slowmode_delay: int = MISSING,
         nsfw: bool = MISSING,
         bitrate: int = MISSING,
         user_limit: int = MISSING,
         rtc_region: Optional[Union[str, VoiceRegion]] = MISSING,
         video_quality_mode: VideoQualityMode = MISSING,
     ) -> PlaceholderID:
-        """
-        Adds a voice channel to the guild builder.
+        """Adds a voice channel to the guild builder.
 
         Parameters
         ----------
         name: :class:`str`
             The channel's name.
         overwrites: Dict[``PlaceholderID``, :class:`PermissionOverwrite`]
             A :class:`dict` of roles to :class:`PermissionOverwrite`\\s to apply to the channel.
```

### Comparing `disnake-2.8.2/disnake/guild_preview.py` & `disnake-2.9.0/disnake/guild_preview.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/guild_scheduled_event.py` & `disnake-2.9.0/disnake/guild_scheduled_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,15 @@
     from .user import User
 
 
 __all__ = ("GuildScheduledEventMetadata", "GuildScheduledEvent")
 
 
 class GuildScheduledEventMetadata:
-    """
-    Represents a guild scheduled event entity metadata.
+    """Represents a guild scheduled event entity metadata.
 
     .. versionadded:: 2.3
 
     Attributes
     ----------
     location: Optional[:class:`str`]
         The location of the guild scheduled event. If :attr:`GuildScheduledEvent.entity_type` is
@@ -70,16 +69,15 @@
     def from_dict(
         cls, data: GuildScheduledEventEntityMetadataPayload
     ) -> GuildScheduledEventMetadata:
         return GuildScheduledEventMetadata(location=data.get("location"))
 
 
 class GuildScheduledEvent(Hashable):
-    """
-    Represents a guild scheduled event.
+    """Represents a guild scheduled event.
 
     .. versionadded:: 2.3
 
     .. container:: operations
 
         .. describe:: x == y
 
@@ -686,15 +684,14 @@
         Yields
         ------
         Union[:class:`User`, :class:`Member`]
             The member (if retrievable) or user subscribed to the guild scheduled event.
 
         Examples
         --------
-
         Usage ::
 
             async for user in event.fetch_users(limit=500):
                 print(user.name)
 
         Flattening into a list ::
```

### Comparing `disnake-2.8.2/disnake/http.py` & `disnake-2.9.0/disnake/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         guild,
         guild_scheduled_event,
         integration,
         interactions,
         invite,
         member,
         message,
+        onboarding,
         role,
         sticker,
         template,
         threads,
         user,
         voice,
         webhook,
@@ -85,22 +86,21 @@
 
 _API_VERSION = 10
 
 
 def _workaround_set_api_version(version: Literal[9, 10]) -> None:
     """Stopgap measure for verified bots without message content intent while intent is not enforced on api v9.
 
-
     .. note::
         This must be ran **before** connecting to the gateway.
     """
     if version not in (9, 10):
         raise TypeError("version must be either 9 or 10")
 
-    global _API_VERSION
+    global _API_VERSION  # noqa: PLW0603
     _API_VERSION = version
     Route.BASE = f"https://discord.com/api/v{_API_VERSION}"
 
 
 async def json_or_text(response: aiohttp.ClientResponse) -> Union[Dict[str, Any], str]:
     text = await response.text(encoding="utf-8")
     try:
@@ -110,20 +110,18 @@
         # Thanks Cloudflare
         pass
 
     return text
 
 
 def set_attachments(payload: Dict[str, Any], files: Sequence[File]) -> None:
-    """
-    Updates the payload's attachments list based on the provided files
+    """Updates the payload's attachments list based on the provided files
 
     note: this method modifies the provided ``payload`` and ``payload["attachments"]`` collections
     """
-
     attachments = payload.get("attachments", [])
     for index, file in enumerate(files):
         attachments.append(
             {
                 "id": index,
                 "description": file.description,
             }
@@ -132,19 +130,17 @@
     # if existing attachments weren't in the payload before and we
     # didn't add any new ones, don't add the list to the payload.
     if attachments:
         payload["attachments"] = attachments
 
 
 def to_multipart(payload: Dict[str, Any], files: Sequence[File]) -> List[Dict[str, Any]]:
-    """
-    Converts the payload and list of files to a multipart payload,
+    """Converts the payload and list of files to a multipart payload,
     as specified by https://discord.com/developers/docs/reference#uploading-files
     """
-
     multipart: List[Dict[str, Any]] = []
     for index, file in enumerate(files):
         multipart.append(
             {
                 "name": f"files[{index}]",
                 "value": file.fp,
                 "filename": file.filename,
@@ -155,20 +151,18 @@
     multipart.append({"name": "payload_json", "value": utils._to_json(payload)})
     return multipart
 
 
 def to_multipart_with_attachments(
     payload: Dict[str, Any], files: Sequence[File]
 ) -> List[Dict[str, Any]]:
-    """
-    Updates the payload's attachments and converts it to a multipart payload
+    """Updates the payload's attachments and converts it to a multipart payload
 
     Shorthand for ``set_attachments`` + ``to_multipart``
     """
-
     set_attachments(payload, files)
     return to_multipart(payload, files)
 
 
 class Route:
     BASE: ClassVar[str] = "https://discord.com/api/v10"
 
@@ -1372,14 +1366,15 @@
             "explicit_content_filter",
             "banner",
             "system_channel_flags",
             "rules_channel_id",
             "public_updates_channel_id",
             "preferred_locale",
             "premium_progress_bar_enabled",
+            "safety_alerts_channel_id",
         )
 
         payload = {k: v for k, v in fields.items() if k in valid_keys}
 
         return self.request(
             Route("PATCH", "/guilds/{guild_id}", guild_id=guild_id), json=payload, reason=reason
         )
@@ -1746,21 +1741,25 @@
 
         return self.request(r, reason=reason)
 
     def get_audit_logs(
         self,
         guild_id: Snowflake,
         limit: int = 100,
+        # only one of these two may be specified, otherwise `after` gets ignored
         before: Optional[Snowflake] = None,
+        after: Optional[Snowflake] = None,
         user_id: Optional[Snowflake] = None,
         action_type: Optional[audit_log.AuditLogEvent] = None,
     ) -> Response[audit_log.AuditLog]:
         params: Dict[str, Any] = {"limit": limit}
-        if before:
+        if before is not None:
             params["before"] = before
+        if after is not None:
+            params["after"] = after
         if user_id:
             params["user_id"] = user_id
         if action_type:
             params["action_type"] = action_type
 
         r = Route("GET", "/guilds/{guild_id}/audit-logs", guild_id=guild_id)
         return self.request(r, params=params)
@@ -2170,14 +2169,16 @@
             "description",
         )
         payload = {k: v for k, v in kwargs.items() if k in valid_keys}
 
         r = Route("PATCH", "/guilds/{guild_id}/welcome-screen", guild_id=guild_id)
         return self.request(r, json=payload, reason=reason)
 
+    # Auto moderation
+
     def get_auto_moderation_rules(self, guild_id: Snowflake) -> Response[List[automod.AutoModRule]]:
         return self.request(
             Route("GET", "/guilds/{guild_id}/auto-moderation/rules", guild_id=guild_id)
         )
 
     def get_auto_moderation_rule(
         self, guild_id: Snowflake, rule_id: Snowflake
@@ -2259,14 +2260,19 @@
                 "/guilds/{guild_id}/auto-moderation/rules/{rule_id}",
                 guild_id=guild_id,
                 rule_id=rule_id,
             ),
             reason=reason,
         )
 
+    # Guild Onboarding
+
+    def get_guild_onboarding(self, guild_id: Snowflake) -> Response[onboarding.Onboarding]:
+        return self.request(Route("GET", "/guilds/{guild_id}/onboarding", guild_id=guild_id))
+
     # Application commands (global)
 
     def get_global_commands(
         self,
         application_id: Snowflake,
         *,
         with_localizations: bool = True,
@@ -2653,25 +2659,25 @@
             json=records,
         )
 
     async def get_gateway(self, *, encoding: str = "json", zlib: bool = True) -> str:
         try:
             data: gateway.Gateway = await self.request(Route("GET", "/gateway"))
         except HTTPException as exc:
-            raise GatewayNotFound() from exc
+            raise GatewayNotFound from exc
 
         return self._format_gateway_url(data["url"], encoding=encoding, zlib=zlib)
 
     async def get_bot_gateway(
         self, *, encoding: str = "json", zlib: bool = True
     ) -> Tuple[int, str, gateway.SessionStartLimit]:
         try:
             data: gateway.GatewayBot = await self.request(Route("GET", "/gateway/bot"))
         except HTTPException as exc:
-            raise GatewayNotFound() from exc
+            raise GatewayNotFound from exc
 
         return (
             data["shards"],
             self._format_gateway_url(data["url"], encoding=encoding, zlib=zlib),
             data["session_start_limit"],
         )
```

### Comparing `disnake-2.8.2/disnake/i18n.py` & `disnake-2.9.0/disnake/i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,15 @@
 #     xyz: LocalizedOptional = None
 #
 # With that, one may use `abc="somename"` and `abc=Localized("somename", ...)`,
 # but not `abc=Localized(None, ...)`. All three work fine for `xyz` though.
 
 
 class Localized(Generic[StringT]):
-    """
-    A container type used for localized parameters.
+    """A container type used for localized parameters.
 
     Exactly one of ``key`` or ``data`` must be provided.
 
     There is an alias for this called ``Localised``.
 
     .. versionadded:: 2.5
 
@@ -173,16 +172,15 @@
         return self
 
 
 Localised = Localized
 
 
 class LocalizationValue:
-    """
-    Container type for (pending) localization data.
+    """Container type for (pending) localization data.
 
     .. versionadded:: 2.5
     """
 
     __slots__ = ("_key", "_data")
 
     def __init__(self, localizations: Optional[Localizations]) -> None:
@@ -223,14 +221,21 @@
         raise ValueError("Can't specify multiple localization keys or dicts")
 
     def _link(self, store: LocalizationProtocol) -> None:
         """Loads localizations from the specified store if this object has a key."""
         if self._key is not None:
             self._data = store.get(self._key)
 
+    def _copy(self) -> LocalizationValue:
+        cls = self.__class__
+        ins = cls.__new__(cls)
+        ins._key = self._key
+        ins._data = self._data
+        return ins
+
     @property
     def data(self) -> Optional[Dict[str, str]]:
         """Optional[Dict[:class:`str`, :class:`str`]]: A dict with a locale -> localization mapping, if available."""
         if self._data is MISSING:
             warnings.warn(
                 "value was never localized, this is likely a library bug",
                 LocalizationWarning,
@@ -244,26 +249,24 @@
         d2 = other.data
         # consider values equal if they're both falsy, or actually equal
         # (it doesn't matter if localizations are `None` or `{}`)
         return (not d1 and not d2) or d1 == d2
 
 
 class LocalizationProtocol(ABC):
-    """
-    Manages a key-value mapping of localizations.
+    """Manages a key-value mapping of localizations.
 
     This is an abstract class, a concrete implementation is provided as :class:`LocalizationStore`.
 
     .. versionadded:: 2.5
     """
 
     @abstractmethod
     def get(self, key: str) -> Optional[Dict[str, str]]:
-        """
-        Returns localizations for the specified key.
+        """Returns localizations for the specified key.
 
         Parameters
         ----------
         key: :class:`str`
             The lookup key.
 
         Raises
@@ -278,16 +281,15 @@
             The localizations for the provided key.
             May return ``None`` if no localizations could be found.
         """
         raise NotImplementedError
 
     # subtypes don't have to implement this
     def load(self, path: Union[str, os.PathLike]) -> None:
-        """
-        Adds localizations from the provided path.
+        """Adds localizations from the provided path.
 
         Parameters
         ----------
         path: Union[:class:`str`, :class:`os.PathLike`]
             The path to the file/directory to load.
 
         Raises
@@ -295,42 +297,39 @@
         RuntimeError
             The provided path is invalid or couldn't be loaded
         """
         raise NotImplementedError
 
     # subtypes don't have to implement this
     def reload(self) -> None:
-        """
-        Clears localizations and reloads all previously loaded sources again.
+        """Clears localizations and reloads all previously loaded sources again.
         If an exception occurs, the previous data gets restored and the exception is re-raised.
         """
         pass
 
 
 class LocalizationStore(LocalizationProtocol):
-    """
-    Manages a key-value mapping of localizations using ``.json`` files.
+    """Manages a key-value mapping of localizations using ``.json`` files.
 
     .. versionadded:: 2.5
 
     Attributes
-    ------------
+    ----------
     strict: :class:`bool`
         Specifies whether :meth:`.get` raises an exception if localizations for a provided key couldn't be found.
     """
 
     def __init__(self, *, strict: bool) -> None:
         self.strict = strict
 
         self._loc: DefaultDict[str, Dict[str, str]] = defaultdict(dict)
         self._paths: Set[Path] = set()
 
     def get(self, key: str) -> Optional[Dict[str, str]]:
-        """
-        Returns localizations for the specified key.
+        """Returns localizations for the specified key.
 
         Parameters
         ----------
         key: :class:`str`
             The lookup key.
 
         Raises
@@ -341,37 +340,34 @@
 
         Returns
         -------
         Optional[Dict[:class:`str`, :class:`str`]]
             The localizations for the provided key.
             Returns ``None`` if no localizations could be found and :attr:`strict` is disabled.
         """
-
         data = self._loc.get(key)
         if data is None and self.strict:
             raise LocalizationKeyError(key)
         return data
 
     def load(self, path: Union[str, os.PathLike]) -> None:
-        """
-        Adds localizations from the provided path to the store.
+        """Adds localizations from the provided path to the store.
         If the path points to a file, the file gets loaded.
         If it's a directory, all ``.json`` files in that directory get loaded (non-recursive).
 
         Parameters
         ----------
         path: Union[:class:`str`, :class:`os.PathLike`]
             The path to the file/directory to load.
 
         Raises
         ------
         RuntimeError
             The provided path is invalid or couldn't be loaded
         """
-
         path = Path(path)
 
         if path.is_file():
             self._load_file(path)
         elif path.is_dir():
             for file in path.glob("*.json"):
                 if not file.is_file():
@@ -379,20 +375,18 @@
                 self._load_file(file)
         else:
             raise RuntimeError(f"Path '{path}' does not exist or is not a directory/file")
 
         self._paths.add(path)
 
     def reload(self) -> None:
-        """
-        Clears localizations and reloads all previously loaded files/directories again.
+        """Clears localizations and reloads all previously loaded files/directories again.
         If an exception occurs, the previous data gets restored and the exception is re-raised.
         See :func:`~LocalizationStore.load` for possible raised exceptions.
         """
-
         old = self._loc
         try:
             self._loc = defaultdict(dict)
             for path in self._paths:
                 self.load(path)
         except Exception:
             # restore in case of error
```

### Comparing `disnake-2.8.2/disnake/integrations.py` & `disnake-2.9.0/disnake/integrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     id: :class:`int`
         The integration ID.
     name: :class:`str`
         The integration name.
     guild: :class:`Guild`
         The guild of the integration.
     type: :class:`str`
-        The integration type (i.e. Twitch).
+        The integration type (i.e. ``twitch``).
     account: :class:`IntegrationAccount`
         The account linked to this integration.
     application_id: Optional[:class:`int`]
         The ID of the application tied to this integration.
     """
 
     __slots__ = (
@@ -115,15 +115,15 @@
         The guild of the integration.
     type: :class:`str`
         The integration type (i.e. Twitch).
     enabled: :class:`bool`
         Whether the integration is currently enabled.
     account: :class:`IntegrationAccount`
         The account linked to this integration.
-    user: :class:`User`
+    user: Optional[:class:`User`]
         The user that added this integration.
     """
 
     __slots__ = (
         "_state",
         "user",
         "enabled",
```

### Comparing `disnake-2.8.2/disnake/interactions/application_command.py` & `disnake-2.9.0/disnake/interactions/application_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,17 +219,15 @@
             f"<ApplicationCommandInteractionData id={self.id!r} name={self.name!r} type={self.type!r} "
             f"target_id={self.target_id!r} target={self.target!r} resolved={self.resolved!r} options={self.options!r}>"
         )
 
     def _get_chain_and_kwargs(
         self, chain: Optional[Tuple[str, ...]] = None
     ) -> Tuple[Tuple[str, ...], Dict[str, Any]]:
-        """
-        Returns a chain of sub-command names and a dict of filled options.
-        """
+        """Returns a chain of sub-command names and a dict of filled options."""
         if chain is None:
             chain = ()
         for option in self.options:
             if option.value is None:
                 # Extend the chain and collect kwargs in the nesting
                 return option._get_chain_and_kwargs(chain + (option.name,))
             return chain, {o.name: o.value for o in self.options}
@@ -251,15 +249,15 @@
     def focused_option(self) -> ApplicationCommandInteractionDataOption:
         """The focused option"""
         # don't annotate as None for user experience
         return self._get_focused_option()  # type: ignore
 
 
 class ApplicationCommandInteractionDataOption(Dict[str, Any]):
-    """This class represents the structure of an interaction data option from the API.
+    """Represents the structure of an interaction data option from the API.
 
     Attributes
     ----------
     name: :class:`str`
         The option's name.
     type: :class:`OptionType`
         The option's type.
```

### Comparing `disnake-2.8.2/disnake/interactions/base.py` & `disnake-2.9.0/disnake/interactions/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -220,15 +220,16 @@
     def created_at(self) -> datetime:
         """:class:`datetime.datetime`: Returns the interaction's creation time in UTC."""
         return utils.snowflake_time(self.id)
 
     @property
     def user(self) -> Union[User, Member]:
         """Union[:class:`.User`, :class:`.Member`]: The user or member that sent the interaction.
-        There is an alias for this named :attr:`author`."""
+        There is an alias for this named :attr:`author`.
+        """
         return self.author
 
     @property
     def guild(self) -> Optional[Guild]:
         """Optional[:class:`Guild`]: The guild the interaction was sent from."""
         return self._state._get_guild(self.guild_id)
 
@@ -379,14 +380,15 @@
         embeds: List[Embed] = MISSING,
         file: File = MISSING,
         files: List[File] = MISSING,
         attachments: Optional[List[Attachment]] = MISSING,
         view: Optional[View] = MISSING,
         components: Optional[Components[MessageUIComponent]] = MISSING,
         suppress_embeds: bool = MISSING,
+        flags: MessageFlags = MISSING,
         allowed_mentions: Optional[AllowedMentions] = None,
     ) -> InteractionMessage:
         """|coro|
 
         Edits the original, previously sent interaction response message.
 
         This is a lower level interface to :meth:`InteractionMessage.edit` in case
@@ -452,14 +454,23 @@
             Whether to suppress embeds for the message. This hides
             all the embeds from the UI if set to ``True``. If set
             to ``False``, this brings the embeds back if they were
             suppressed.
 
             .. versionadded:: 2.7
 
+        flags: :class:`MessageFlags`
+            The new flags to set for this message. Overrides existing flags.
+            Only :attr:`~MessageFlags.suppress_embeds` is supported.
+
+            If parameter ``suppress_embeds`` is provided,
+            that will override the setting of :attr:`.MessageFlags.suppress_embeds`.
+
+            .. versionadded:: 2.9
+
         Raises
         ------
         HTTPException
             Editing the message failed.
         Forbidden
             Edited a message that is not yours.
         TypeError
@@ -484,14 +495,15 @@
             files=files,
             attachments=attachments,
             embed=embed,
             embeds=embeds,
             view=view,
             components=components,
             suppress_embeds=suppress_embeds,
+            flags=flags,
             allowed_mentions=allowed_mentions,
             previous_allowed_mentions=previous_mentions,
         )
         adapter = async_context.get()
         try:
             data = await adapter.edit_original_interaction_response(
                 self.application_id,
@@ -583,16 +595,17 @@
         embeds: List[Embed] = MISSING,
         file: File = MISSING,
         files: List[File] = MISSING,
         allowed_mentions: AllowedMentions = MISSING,
         view: View = MISSING,
         components: Components[MessageUIComponent] = MISSING,
         tts: bool = False,
-        ephemeral: bool = False,
-        suppress_embeds: bool = False,
+        ephemeral: bool = MISSING,
+        suppress_embeds: bool = MISSING,
+        flags: MessageFlags = MISSING,
         delete_after: float = MISSING,
     ) -> None:
         """|coro|
 
         Sends a message using either :meth:`response.send_message <InteractionResponse.send_message>`
         or :meth:`followup.send <Webhook.send>`.
 
@@ -641,14 +654,24 @@
             is set to 15 minutes.
         suppress_embeds: :class:`bool`
             Whether to suppress embeds for the message. This hides
             all the embeds from the UI if set to ``True``.
 
             .. versionadded:: 2.5
 
+        flags: :class:`MessageFlags`
+            The flags to set for this message.
+            Only :attr:`~MessageFlags.suppress_embeds`, :attr:`~MessageFlags.ephemeral`
+            and :attr:`~MessageFlags.suppress_notifications` are supported.
+
+            If parameters ``suppress_embeds`` or ``ephemeral`` are provided,
+            they will override the corresponding setting of this ``flags`` parameter.
+
+            .. versionadded:: 2.9
+
         delete_after: :class:`float`
             If provided, the number of seconds to wait in the background
             before deleting the message we just sent. If the deletion fails,
             then it is silently ignored.
 
             Can be up to 15 minutes after the interaction was created
             (see also :attr:`expires_at`/:attr:`is_expired`).
@@ -677,14 +700,15 @@
             files=files,
             allowed_mentions=allowed_mentions,
             view=view,
             components=components,
             tts=tts,
             ephemeral=ephemeral,
             suppress_embeds=suppress_embeds,
+            flags=flags,
             delete_after=delete_after,
         )
 
 
 class InteractionResponse:
     """Represents a Discord interaction response.
 
@@ -848,16 +872,17 @@
         embeds: List[Embed] = MISSING,
         file: File = MISSING,
         files: List[File] = MISSING,
         allowed_mentions: AllowedMentions = MISSING,
         view: View = MISSING,
         components: Components[MessageUIComponent] = MISSING,
         tts: bool = False,
-        ephemeral: bool = False,
-        suppress_embeds: bool = False,
+        ephemeral: bool = MISSING,
+        suppress_embeds: bool = MISSING,
+        flags: MessageFlags = MISSING,
         delete_after: float = MISSING,
     ) -> None:
         """|coro|
 
         Responds to this interaction by sending a message.
 
         Parameters
@@ -903,14 +928,24 @@
 
         suppress_embeds: :class:`bool`
             Whether to suppress embeds for the message. This hides
             all the embeds from the UI if set to ``True``.
 
             .. versionadded:: 2.5
 
+        flags: :class:`MessageFlags`
+            The flags to set for this message.
+            Only :attr:`~MessageFlags.suppress_embeds`, :attr:`~MessageFlags.ephemeral`
+            and :attr:`~MessageFlags.suppress_notifications` are supported.
+
+            If parameters ``suppress_embeds`` or ``ephemeral`` are provided,
+            they will override the corresponding setting of this ``flags`` parameter.
+
+            .. versionadded:: 2.9
+
         Raises
         ------
         HTTPException
             Sending the message failed.
         TypeError
             You specified both ``embed`` and ``embeds``.
         ValueError
@@ -962,19 +997,22 @@
                 payload["allowed_mentions"] = allowed_mentions.to_dict()
         elif previous_mentions is not None:
             payload["allowed_mentions"] = previous_mentions.to_dict()
 
         if content is not None:
             payload["content"] = str(content)
 
-        payload["flags"] = 0
-        if suppress_embeds:
-            payload["flags"] |= MessageFlags.suppress_embeds.flag
-        if ephemeral:
-            payload["flags"] |= MessageFlags.ephemeral.flag
+        if suppress_embeds is not MISSING or ephemeral is not MISSING:
+            flags = MessageFlags._from_value(0 if flags is MISSING else flags.value)
+            if suppress_embeds is not MISSING:
+                flags.suppress_embeds = suppress_embeds
+            if ephemeral is not MISSING:
+                flags.ephemeral = ephemeral
+        if flags is not MISSING:
+            payload["flags"] = flags.value
 
         if view is not MISSING:
             payload["components"] = view.to_components()
 
         if components is not MISSING:
             payload["components"] = components_to_dict(components)
 
@@ -1306,15 +1344,14 @@
             raise InteractionResponded(parent)
 
         modal_data: ModalPayload
 
         if modal is not None:
             modal_data = modal.to_components()
         elif title and components and custom_id:
-
             rows = components_to_dict(components)
             if len(rows) > 5:
                 raise ValueError("Maximum number of components exceeded.")
 
             modal_data = {
                 "title": title,
                 "custom_id": custom_id,
@@ -1380,15 +1417,15 @@
     author: Union[:class:`Member`, :class:`abc.User`]
         A :class:`Member` that sent the message. If :attr:`channel` is a
         private channel, then it is a :class:`User` instead.
     content: :class:`str`
         The actual contents of the message.
     embeds: List[:class:`Embed`]
         A list of embeds the message has.
-    channel: Union[:class:`TextChannel`, :class:`VoiceChannel`, :class:`Thread`, :class:`DMChannel`, :class:`GroupChannel`, :class:`PartialMessageable`]
+    channel: Union[:class:`TextChannel`, :class:`VoiceChannel`, :class:`StageChannel`, :class:`Thread`, :class:`DMChannel`, :class:`GroupChannel`, :class:`PartialMessageable`]
         The channel that the message was sent from.
         Could be a :class:`DMChannel` or :class:`GroupChannel` if it's a private message.
     reference: Optional[:class:`~disnake.MessageReference`]
         The message that this message references. This is only applicable to message replies.
     interaction: Optional[:class:`~disnake.InteractionReference`]
         The interaction that this message references.
         This exists only when the message is a response to an interaction without an existing message.
@@ -1442,14 +1479,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embed: Optional[Embed] = ...,
         file: File = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
     ) -> InteractionMessage:
         ...
 
     @overload
@@ -1457,14 +1495,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embed: Optional[Embed] = ...,
         files: List[File] = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
     ) -> InteractionMessage:
         ...
 
     @overload
@@ -1472,14 +1511,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embeds: List[Embed] = ...,
         file: File = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
     ) -> InteractionMessage:
         ...
 
     @overload
@@ -1487,14 +1527,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embeds: List[Embed] = ...,
         files: List[File] = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
     ) -> InteractionMessage:
         ...
 
     async def edit(
@@ -1503,14 +1544,15 @@
         *,
         embed: Optional[Embed] = MISSING,
         embeds: List[Embed] = MISSING,
         file: File = MISSING,
         files: List[File] = MISSING,
         attachments: Optional[List[Attachment]] = MISSING,
         suppress_embeds: bool = MISSING,
+        flags: MessageFlags = MISSING,
         allowed_mentions: Optional[AllowedMentions] = MISSING,
         view: Optional[View] = MISSING,
         components: Optional[Components[MessageUIComponent]] = MISSING,
     ) -> Message:
         """|coro|
 
         Edits the message.
@@ -1564,14 +1606,23 @@
             Whether to suppress embeds for the message. This hides
             all the embeds from the UI if set to ``True``. If set
             to ``False``, this brings the embeds back if they were
             suppressed.
 
             .. versionadded:: 2.7
 
+        flags: :class:`MessageFlags`
+            The new flags to set for this message. Overrides existing flags.
+            Only :attr:`~MessageFlags.suppress_embeds` is supported.
+
+            If parameter ``suppress_embeds`` is provided,
+            that will override the setting of :attr:`.MessageFlags.suppress_embeds`.
+
+            .. versionadded:: 2.9
+
         allowed_mentions: :class:`AllowedMentions`
             Controls the mentions being processed in this message.
             See :meth:`.abc.Messageable.send` for more information.
 
         Raises
         ------
         HTTPException
@@ -1596,14 +1647,15 @@
             params = {"file": file, "embed": embed}
             return await super().edit(
                 content=content,
                 embeds=embeds,
                 files=files,
                 attachments=attachments,
                 suppress_embeds=suppress_embeds,
+                flags=flags,
                 allowed_mentions=allowed_mentions,
                 view=view,
                 components=components,
                 **params,
             )
 
         # if no attachment list was provided but we're uploading new files,
@@ -1616,14 +1668,15 @@
             content=content,
             embed=embed,
             embeds=embeds,
             file=file,
             files=files,
             attachments=attachments,
             suppress_embeds=suppress_embeds,
+            flags=flags,
             allowed_mentions=allowed_mentions,
             view=view,
             components=components,
         )
 
     async def delete(self, *, delay: Optional[float] = None) -> None:
         """|coro|
@@ -1783,17 +1836,29 @@
 
     def __repr__(self) -> str:
         return (
             f"<InteractionDataResolved members={self.members!r} users={self.users!r} "
             f"roles={self.roles!r} channels={self.channels!r} messages={self.messages!r} attachments={self.attachments!r}>"
         )
 
+    @overload
     def get_with_type(
-        self, key: Snowflake, data_type: Union[OptionType, ComponentType], default: T = None
+        self, key: Snowflake, data_type: Union[OptionType, ComponentType]
+    ) -> Union[Member, User, Role, InteractionChannel, Message, Attachment, None]:
+        ...
+
+    @overload
+    def get_with_type(
+        self, key: Snowflake, data_type: Union[OptionType, ComponentType], default: T
     ) -> Union[Member, User, Role, InteractionChannel, Message, Attachment, T]:
+        ...
+
+    def get_with_type(
+        self, key: Snowflake, data_type: Union[OptionType, ComponentType], default: T = None
+    ) -> Union[Member, User, Role, InteractionChannel, Message, Attachment, T, None]:
         if data_type is OptionType.mentionable or data_type is ComponentType.mentionable_select:
             key = int(key)
             if (result := self.members.get(key)) is not None:
                 return result
             if (result := self.users.get(key)) is not None:
                 return result
             return self.roles.get(key, default)
```

### Comparing `disnake-2.8.2/disnake/interactions/message.py` & `disnake-2.9.0/disnake/interactions/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     def component(self) -> MessageComponent:
         """Union[:class:`Button`, :class:`BaseSelectMenu`]: The component the user interacted with"""
         for action_row in self.message.components:
             for component in action_row.children:
                 if component.custom_id == self.data.custom_id:
                     return component
 
-        raise Exception("MessageInteraction is malformed - no component found")
+        raise Exception("MessageInteraction is malformed - no component found")  # noqa: TRY002
 
 
 class MessageInteractionData(Dict[str, Any]):
     """Represents the data of an interaction with a message component.
 
     .. versionadded:: 2.1
```

### Comparing `disnake-2.8.2/disnake/interactions/modal.py` & `disnake-2.9.0/disnake/interactions/modal.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,31 +78,31 @@
         if message_data := data.get("message"):
             message = Message(state=self._state, channel=self.channel, data=message_data)
         else:
             message = None
         self.message: Optional[Message] = message
 
     def walk_raw_components(self) -> Generator[ModalInteractionComponentDataPayload, None, None]:
-        """
-        Returns a generator that yields raw component data from action rows one by one, as provided by Discord.
+        """Returns a generator that yields raw component data from action rows one by one, as provided by Discord.
         This does not contain all fields of the components due to API limitations.
 
         .. versionadded:: 2.6
 
         Returns
         -------
         Generator[:class:`dict`, None, None]
         """
         for action_row in self.data.components:
             yield from action_row["components"]
 
     @cached_slot_property("_cs_text_values")
     def text_values(self) -> Dict[str, str]:
         """Dict[:class:`str`, :class:`str`]: Returns the text values the user has entered in the modal.
-        This is a dict of the form ``{custom_id: value}``."""
+        This is a dict of the form ``{custom_id: value}``.
+        """
         text_input_type = ComponentType.text_input.value
         return {
             component["custom_id"]: component.get("value") or ""
             for component in self.walk_raw_components()
             if component.get("type") == text_input_type
         }
```

### Comparing `disnake-2.8.2/disnake/invite.py` & `disnake-2.9.0/disnake/invite.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,16 +247,15 @@
         """Optional[:class:`Asset`]: Returns the guild's invite splash asset, if available."""
         if self._splash is None:
             return None
         return Asset._from_guild_image(self._state, self.id, self._splash, path="splashes")
 
 
 class Invite(Hashable):
-    """
-    Represents a Discord :class:`Guild` or :class:`abc.GuildChannel` invite.
+    """Represents a Discord :class:`Guild` or :class:`abc.GuildChannel` invite.
 
     Depending on the way this object was created, some of the attributes can
     have a value of ``None`` (see table below).
 
     .. container:: operations
 
         .. describe:: x == y
```

### Comparing `disnake-2.8.2/disnake/iterators.py` & `disnake-2.9.0/disnake/iterators.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,19 +112,19 @@
     async def flatten(self) -> List[T]:
         return [element async for element in self]
 
     async def __anext__(self) -> T:
         try:
             return await self.next()
         except NoMoreItems:
-            raise StopAsyncIteration()
+            raise StopAsyncIteration from None
 
 
 class _ChunkedAsyncIterator(_AsyncIterator[List[T]]):
-    def __init__(self, iterator, max_size) -> None:
+    def __init__(self, iterator: _AsyncIterator[T], max_size: int) -> None:
         self.iterator = iterator
         self.max_size = max_size
 
     async def next(self) -> List[T]:
         ret: List[T] = []
         n = 0
         while n < self.max_size:
@@ -168,15 +168,15 @@
             item = await getter()
             ret = await maybe_coroutine(pred, item)
             if ret:
                 return item
 
 
 class ReactionIterator(_AsyncIterator[Union["User", "Member"]]):
-    def __init__(self, message, emoji, limit=100, after=None) -> None:
+    def __init__(self, message, emoji, limit: int = 100, after=None) -> None:
         self.message = message
         self.limit = limit
         self.after = after
         state = message._state
         self.getter = state.http.get_reaction_users
         self.state = state
         self.emoji = emoji
@@ -187,15 +187,15 @@
     async def next(self) -> Union[User, Member]:
         if self.users.empty():
             await self.fill_users()
 
         try:
             return self.users.get_nowait()
         except asyncio.QueueEmpty:
-            raise NoMoreItems()
+            raise NoMoreItems from None
 
     async def fill_users(self) -> None:
         if self.limit > 0:
             retrieve = min(self.limit, 100)
 
             after = self.after.id if self.after else None
             data: List[PartialUserPayload] = await self.getter(
@@ -257,15 +257,14 @@
         messageable: Messageable,
         limit: Optional[int] = 100,
         before: Optional[Union[Snowflake, datetime.datetime]] = None,
         after: Optional[Union[Snowflake, datetime.datetime]] = None,
         around: Optional[Union[Snowflake, datetime.datetime]] = None,
         oldest_first: Optional[bool] = None,
     ) -> None:
-
         if isinstance(before, datetime.datetime):
             before = Object(id=time_snowflake(before, high=False))
         if isinstance(after, datetime.datetime):
             after = Object(id=time_snowflake(after, high=True))
         if isinstance(around, datetime.datetime):
             around = Object(id=time_snowflake(around))
 
@@ -314,15 +313,15 @@
     async def next(self) -> Message:
         if self.messages.empty():
             await self.fill_messages()
 
         try:
             return self.messages.get_nowait()
         except asyncio.QueueEmpty:
-            raise NoMoreItems()
+            raise NoMoreItems from None
 
     def _get_retrieve(self):
         limit = self.limit
         if limit is None or limit > 100:
             retrieve = 100
         else:
             retrieve = limit
@@ -396,15 +395,15 @@
     ``after``, sorted with the oldest first. For filling over 1000 bans, update the
     ``after`` parameter to the oldest user received.
 
     A note that if both ``before`` and ``after`` are specified, ``after`` is ignored by the
     bans endpoint.
 
     Parameters
-    -----------
+    ----------
     guild: :class:`~disnake.Guild`
         The guild to get bans from.
     limit: Optional[:class:`int`]
         Maximum number of bans to retrieve.
     before: Optional[:class:`abc.Snowflake`]
         Object before which all bans must be.
     after: Optional[:class:`abc.Snowflake`]
@@ -439,15 +438,15 @@
     async def next(self) -> BanEntry:
         if self.bans.empty():
             await self.fill_bans()
 
         try:
             return self.bans.get_nowait()
         except asyncio.QueueEmpty:
-            raise NoMoreItems()
+            raise NoMoreItems from None
 
     def _get_retrieve(self) -> bool:
         self.retrieve = min(self.limit, 1000) if self.limit is not None else 1000
         return self.retrieve > 0
 
     async def fill_bans(self) -> None:
         if self._get_retrieve():
@@ -492,14 +491,15 @@
         self,
         guild: Guild,
         limit: Optional[int] = None,
         before: Optional[Union[Snowflake, datetime.datetime]] = None,
         after: Optional[Union[Snowflake, datetime.datetime]] = None,
         user_id: Optional[int] = None,
         action_type: Optional[AuditLogEvent] = None,
+        oldest_first: bool = False,
     ) -> None:
         if isinstance(before, datetime.datetime):
             before = Object(id=time_snowflake(before, high=False))
         if isinstance(after, datetime.datetime):
             after = Object(id=time_snowflake(after, high=True))
 
         self.limit: Optional[int] = limit
@@ -511,18 +511,24 @@
         self.guild = guild
         self._state = guild._state
         self.request = guild._state.http.get_audit_logs
 
         self.entries: asyncio.Queue[AuditLogEntry] = asyncio.Queue()
 
         self._filter: Optional[Callable[[AuditLogEntryPayload], bool]] = None
-        if self.after and self.after != OLDEST_OBJECT:
-            self._filter = lambda e: int(e["id"]) > self.after.id
+        if oldest_first:
+            self._strategy = self._after_strategy
+            if self.before:
+                self._filter = lambda m: int(m["id"]) < self.before.id  # type: ignore
+        else:
+            self._strategy = self._before_strategy
+            if self.after and self.after != OLDEST_OBJECT:
+                self._filter = lambda m: int(m["id"]) > self.after.id
 
-    async def _retrieve_data(self, retrieve: int) -> AuditLogPayload:
+    async def _before_strategy(self, retrieve: int) -> AuditLogPayload:
         before = self.before.id if self.before else None
         data: AuditLogPayload = await self.request(
             self.guild.id,
             limit=retrieve,
             user_id=self.user_id,
             action_type=self.action_type,
             before=before,
@@ -531,35 +537,54 @@
         entries = data.get("audit_log_entries", [])
         if entries:
             if self.limit is not None:
                 self.limit -= retrieve
             self.before = Object(id=int(entries[-1]["id"]))
         return data
 
+    async def _after_strategy(self, retrieve: int) -> AuditLogPayload:
+        after = self.after.id
+        data: AuditLogPayload = await self.request(
+            self.guild.id,
+            limit=retrieve,
+            user_id=self.user_id,
+            action_type=self.action_type,
+            after=after,
+        )
+
+        entries = data.get("audit_log_entries", [])
+        if entries:
+            if self.limit is not None:
+                self.limit -= retrieve
+            # note: unlike other paginated endpoints, this one returns entries in ascending
+            # order when using `after`; hence `-1` (instead of `0`) is correct here.
+            self.after = Object(id=int(entries[-1]["id"]))
+        return data
+
     async def next(self) -> AuditLogEntry:
         if self.entries.empty():
             await self._fill()
 
         try:
             return self.entries.get_nowait()
         except asyncio.QueueEmpty:
-            raise NoMoreItems()
+            raise NoMoreItems from None
 
     def _get_retrieve(self):
         limit = self.limit
         if limit is None or limit > 100:
             retrieve = 100
         else:
             retrieve = limit
         self.retrieve = retrieve
         return retrieve > 0
 
     async def _fill(self) -> None:
         if self._get_retrieve():
-            log_data = await self._retrieve_data(self.retrieve)
+            log_data = await self._strategy(self.retrieve)
             entries = log_data.get("audit_log_entries")
             if len(entries) < 100:
                 self.limit = 0  # terminate the infinite loop
 
             if self._filter:
                 entries = filter(self._filter, entries)
 
@@ -645,16 +670,15 @@
         Maximum number of guilds to retrieve.
     before: Optional[Union[:class:`abc.Snowflake`, :class:`datetime.datetime`]]
         Object before which all guilds must be.
     after: Optional[Union[:class:`abc.Snowflake`, :class:`datetime.datetime`]]
         Object after which all guilds must be.
     """
 
-    def __init__(self, bot, limit, before=None, after=None) -> None:
-
+    def __init__(self, bot, limit: Optional[int], before=None, after=None) -> None:
         if isinstance(before, datetime.datetime):
             before = Object(id=time_snowflake(before, high=False))
         if isinstance(after, datetime.datetime):
             after = Object(id=time_snowflake(after, high=True))
 
         self.bot = bot
         self.limit = limit
@@ -679,15 +703,15 @@
     async def next(self) -> Guild:
         if self.guilds.empty():
             await self.fill_guilds()
 
         try:
             return self.guilds.get_nowait()
         except asyncio.QueueEmpty:
-            raise NoMoreItems()
+            raise NoMoreItems from None
 
     def _get_retrieve(self):
         limit = self.limit
         if limit is None or limit > 200:
             retrieve = 200
         else:
             retrieve = limit
@@ -735,16 +759,15 @@
             if self.limit is not None:
                 self.limit -= retrieve
             self.after = Object(id=int(data[-1]["id"]))
         return data
 
 
 class MemberIterator(_AsyncIterator["Member"]):
-    def __init__(self, guild, limit=1000, after=None) -> None:
-
+    def __init__(self, guild, limit: Optional[int] = 1000, after=None) -> None:
         if isinstance(after, datetime.datetime):
             after = Object(id=time_snowflake(after, high=True))
 
         self.guild = guild
         self.limit = limit
         self.after = after or OLDEST_OBJECT
 
@@ -755,15 +778,15 @@
     async def next(self) -> Member:
         if self.members.empty():
             await self.fill_members()
 
         try:
             return self.members.get_nowait()
         except asyncio.QueueEmpty:
-            raise NoMoreItems()
+            raise NoMoreItems from None
 
     def _get_retrieve(self):
         limit = self.limit
         if limit is None or limit > 1000:
             retrieve = 1000
         else:
             retrieve = limit
@@ -842,27 +865,27 @@
     async def next(self) -> Thread:
         if self.queue.empty():
             await self.fill_queue()
 
         try:
             return self.queue.get_nowait()
         except asyncio.QueueEmpty:
-            raise NoMoreItems()
+            raise NoMoreItems from None
 
     @staticmethod
     def get_archive_timestamp(data: ThreadPayload) -> str:
         return data["thread_metadata"]["archive_timestamp"]
 
     @staticmethod
     def get_thread_id(data: ThreadPayload) -> str:
         return data["id"]  # type: ignore
 
     async def fill_queue(self) -> None:
         if not self.has_more:
-            raise NoMoreItems()
+            raise NoMoreItems
 
         limit = 50 if self.limit is None else max(self.limit, 50)
         data = await self.endpoint(self.channel_id, before=self.before, limit=limit)
 
         # This stuff is obviously WIP because 'members' is always empty
         threads: List[ThreadPayload] = data.get("threads", [])
         for d in reversed(threads):
@@ -917,15 +940,15 @@
     async def next(self) -> Message:
         if self.users.empty():
             await self.fill_users()
 
         try:
             return self.users.get_nowait()
         except asyncio.QueueEmpty:
-            raise NoMoreItems()
+            raise NoMoreItems from None
 
     def _get_retrieve(self) -> bool:
         limit = self.limit
         if limit is None or limit > 100:
             retrieve = 100
         else:
             retrieve = limit
```

### Comparing `disnake-2.8.2/disnake/member.py` & `disnake-2.9.0/disnake/member.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 
         .. describe:: hash(x)
 
             Returns the member's hash.
 
         .. describe:: str(x)
 
-            Returns the member's name with the discriminator.
+            Returns the member's username (with discriminator, if not migrated to new system yet).
 
     Attributes
     ----------
     joined_at: Optional[:class:`datetime.datetime`]
         An aware datetime object that specifies the date and time in UTC that the member joined the guild.
         If the member left and rejoined the guild, this will be the latest date. In certain cases, this can be ``None``.
     activities: Tuple[Union[:class:`BaseActivity`, :class:`Spotify`]]
@@ -245,14 +245,15 @@
             Due to a Discord API limitation, a user's Spotify activity may not appear
             if they are listening to a song with a title longer
             than 128 characters. See :issue-dpy:`1738` for more information.
     guild: :class:`Guild`
         The guild that the member belongs to.
     nick: Optional[:class:`str`]
         The guild specific nickname of the user.
+        This takes precedence over :attr:`.global_name` and :attr:`.name` when shown.
     pending: :class:`bool`
         Whether the member is pending member verification.
 
         .. versionadded:: 1.6
 
     premium_since: Optional[:class:`datetime.datetime`]
         An aware datetime object that specifies the date and time in UTC when the member used their
@@ -274,14 +275,16 @@
         "_communication_disabled_until",
         "_flags",
     )
 
     if TYPE_CHECKING:
         name: str
         id: int
+        discriminator: str
+        global_name: Optional[str]
         bot: bool
         system: bool
         created_at: datetime.datetime
         default_avatar: Asset
         avatar: Optional[Asset]
         dm_channel: Optional[DMChannel]
         create_dm = User.create_dm
@@ -341,15 +344,15 @@
         self._flags: int = data.get("flags", 0)
 
     def __str__(self) -> str:
         return str(self._user)
 
     def __repr__(self) -> str:
         return (
-            f"<Member id={self._user.id} name={self._user.name!r} discriminator={self._user.discriminator!r}"
+            f"<Member id={self._user.id} name={self._user.name!r} global_name={self._user.global_name!r} discriminator={self._user.discriminator!r}"
             f" bot={self._user.bot} nick={self.nick!r} guild={self.guild!r}>"
         )
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, _UserTag) and other.id == self.id
 
     def __ne__(self, other: Any) -> bool:
@@ -445,25 +448,26 @@
 
         if len(user) > 1:
             return self._update_inner_user(user)
         return None
 
     def _update_inner_user(self, user: UserPayload) -> Optional[Tuple[User, User]]:
         u = self._user
-        original = (u.name, u._avatar, u.discriminator, u._public_flags)
+        original = (u.name, u._avatar, u.discriminator, u.global_name, u._public_flags)
         # These keys seem to always be available
         modified = (
             user["username"],
             user["avatar"],
             user["discriminator"],
+            user.get("global_name"),
             user.get("public_flags", 0),
         )
         if original != modified:
             to_return = User._copy(self._user)
-            u.name, u._avatar, u.discriminator, u._public_flags = modified
+            u.name, u._avatar, u.discriminator, u.global_name, u._public_flags = modified
             # Signal to dispatch on_user_update
             return to_return, u
 
     @property
     def status(self) -> Status:
         """:class:`Status`: The member's overall status. If the value is unknown, then it will be a :class:`str` instead."""
         return try_enum(Status, self._client_status[None])
@@ -479,19 +483,16 @@
     @status.setter
     def status(self, value: Status) -> None:
         # internal use only
         self._client_status[None] = str(value)
 
     @property
     def tag(self) -> str:
-        return self._user.discriminator
-
-    @property
-    def discriminator(self) -> str:
-        return self._user.discriminator
+        """:class:`str`: An alias of :attr:`.discriminator`."""
+        return self.discriminator
 
     @property
     def mobile_status(self) -> Status:
         """:class:`Status`: The member's status on a mobile device, if applicable."""
         return try_enum(Status, self._client_status.get("mobile", "offline"))
 
     @property
@@ -562,19 +563,22 @@
         """:class:`str`: Returns a string that allows you to mention the member."""
         return f"<@{self._user.id}>"
 
     @property
     def display_name(self) -> str:
         """:class:`str`: Returns the user's display name.
 
-        For regular users this is just their username, but
-        if they have a guild specific nickname then that
-        is returned instead.
+        If they have a guild-specific :attr:`nickname <.nick>`, then
+        that is returned. If not, this is their :attr:`global name <.global_name>`
+        if set, or their :attr:`username <.name>` otherwise.
+
+        .. versionchanged:: 2.9
+            Added :attr:`.global_name`.
         """
-        return self.nick or self.name
+        return self.nick or self.global_name or self.name
 
     @property
     def display_avatar(self) -> Asset:
         """:class:`Asset`: Returns the member's display avatar.
 
         For regular members this is just their avatar, but
         if they have a guild specific avatar then that
@@ -691,15 +695,14 @@
 
     @property
     def current_timeout(self) -> Optional[datetime.datetime]:
         """Optional[:class:`datetime.datetime`]: Returns the datetime when the timeout expires, if any.
 
         .. versionadded:: 2.3
         """
-
         if self._communication_disabled_until is None:
             return None
 
         if self._communication_disabled_until < utils.utcnow():
             self._communication_disabled_until = None
             return None
 
@@ -881,31 +884,29 @@
             payload["deaf"] = deafen
 
         if mute is not MISSING:
             payload["mute"] = mute
 
         if suppress is not MISSING:
             if self.voice is None or self.voice.channel is None:
-                raise Exception("Cannot suppress a member which isn't in a vc")
+                raise Exception("Cannot suppress a member which isn't in a vc")  # noqa: TRY002
 
             voice_state_payload: Dict[str, Any] = {
                 "channel_id": self.voice.channel.id,
                 "suppress": suppress,
             }
 
             if suppress or self.bot:
                 voice_state_payload["request_to_speak_timestamp"] = None
 
             if me:
                 await http.edit_my_voice_state(guild_id, voice_state_payload)
             else:
                 if not suppress:
-                    voice_state_payload[
-                        "request_to_speak_timestamp"
-                    ] = datetime.datetime.utcnow().isoformat()
+                    voice_state_payload["request_to_speak_timestamp"] = utils.utcnow().isoformat()
                 await http.edit_voice_state(guild_id, self.id, voice_state_payload)
 
         if voice_channel is not MISSING:
             payload["channel_id"] = voice_channel and voice_channel.id
 
         if roles is not MISSING:
             payload["roles"] = tuple(r.id for r in roles)
@@ -952,19 +953,19 @@
         ------
         Forbidden
             You do not have the proper permissions to the action requested.
         HTTPException
             The operation failed.
         """
         if self.voice is None or self.voice.channel is None:
-            raise Exception("Cannot request to speak when not in a vc")
+            raise Exception("Cannot request to speak when not in a vc")  # noqa: TRY002
 
         payload = {
             "channel_id": self.voice.channel.id,
-            "request_to_speak_timestamp": datetime.datetime.utcnow().isoformat(),
+            "request_to_speak_timestamp": utils.utcnow().isoformat(),
         }
 
         if self._state.self_id != self.id:
             payload["suppress"] = False
             await self._state.http.edit_voice_state(self.guild.id, self.id, payload)
         else:
             await self._state.http.edit_my_voice_state(self.guild.id, payload)
@@ -991,16 +992,15 @@
             The reason for doing this action. Shows up on the audit log.
         """
         await self.edit(voice_channel=channel, reason=reason)
 
     async def add_roles(
         self, *roles: Snowflake, reason: Optional[str] = None, atomic: bool = True
     ) -> None:
-        """
-        |coro|
+        """|coro|
 
         Gives the member a number of :class:`Role`\\s.
 
         You must have :attr:`~Permissions.manage_roles` permission to
         use this, and the added :class:`Role`\\s must appear lower in the list
         of roles than the highest role of the member.
 
@@ -1032,16 +1032,15 @@
             user_id = self.id
             for role in roles:
                 await req(guild_id, user_id, role.id, reason=reason)
 
     async def remove_roles(
         self, *roles: Snowflake, reason: Optional[str] = None, atomic: bool = True
     ) -> None:
-        """
-        |coro|
+        """|coro|
 
         Removes :class:`Role`\\s from this member.
 
         You must have :attr:`~Permissions.manage_roles` permission to
         use this, and the removed :class:`Role`\\s must appear lower in the list
         of roles than the highest role of the member.
```

### Comparing `disnake-2.8.2/disnake/mentions.py` & `disnake-2.9.0/disnake/mentions.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/message.py` & `disnake-2.9.0/disnake/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 import asyncio
 import datetime
 import io
 import re
+from base64 import b64decode, b64encode
 from os import PathLike
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     Dict,
@@ -64,14 +65,15 @@
     from .types.message import (
         Attachment as AttachmentPayload,
         Message as MessagePayload,
         MessageActivity as MessageActivityPayload,
         MessageApplication as MessageApplicationPayload,
         MessageReference as MessageReferencePayload,
         Reaction as ReactionPayload,
+        RoleSubscriptionData as RoleSubscriptionDataPayload,
     )
     from .types.threads import ThreadArchiveDurationLiteral
     from .types.user import User as UserPayload
     from .ui.action_row import Components, MessageUIComponent
     from .ui.view import View
 
     EmojiInputType = Union[Emoji, PartialEmoji, str]
@@ -79,14 +81,15 @@
 __all__ = (
     "Attachment",
     "Message",
     "PartialMessage",
     "MessageReference",
     "InteractionReference",
     "DeletedReferencedMessage",
+    "RoleSubscriptionData",
 )
 
 
 def convert_emoji_reaction(emoji: Union[EmojiInputType, Reaction]) -> str:
     if isinstance(emoji, Reaction):
         emoji = emoji.emoji
 
@@ -122,14 +125,15 @@
     embed: Optional[Embed],
     embeds: List[Embed],
     file: File,
     files: List[File],
     attachments: Optional[List[Attachment]],
     suppress: bool,  # deprecated
     suppress_embeds: bool,
+    flags: MessageFlags,
     allowed_mentions: Optional[AllowedMentions],
     view: Optional[View],
     components: Optional[Components[MessageUIComponent]],
 ) -> Message:
     if embed is not MISSING and embeds is not MISSING:
         raise TypeError("Cannot mix embed and embeds keyword arguments.")
     if file is not MISSING and files is not MISSING:
@@ -162,16 +166,17 @@
         payload["embeds"] = [e.to_dict() for e in embeds]
         for embed in embeds:
             if embed._files:
                 files = files or []
                 files.extend(embed._files.values())
 
     if suppress_embeds is not MISSING:
-        flags = MessageFlags._from_value(default_flags)
+        flags = MessageFlags._from_value(default_flags if flags is MISSING else flags.value)
         flags.suppress_embeds = suppress_embeds
+    if flags is not MISSING:
         payload["flags"] = flags.value
 
     if allowed_mentions is MISSING:
         if previous_allowed_mentions:
             payload["allowed_mentions"] = previous_allowed_mentions.to_dict()
     else:
         if allowed_mentions:
@@ -252,55 +257,73 @@
         The attachment URL. If the message this attachment was attached
         to is deleted, then this will 404.
     proxy_url: :class:`str`
         The proxy URL. This is a cached version of the :attr:`~Attachment.url` in the
         case of images. When the message is deleted, this URL might be valid for a few
         minutes or not valid at all.
     content_type: Optional[:class:`str`]
-        The attachment's `media type <https://en.wikipedia.org/wiki/Media_type>`_
+        The attachment's `media type <https://en.wikipedia.org/wiki/Media_type>`_.
 
         .. versionadded:: 1.7
 
     ephemeral: :class:`bool`
         Whether the attachment is ephemeral.
 
         .. versionadded:: 2.1
 
     description: :class:`str`
-        The attachment's description
+        The attachment's description.
 
         .. versionadded:: 2.3
+
+    duration: Optional[:class:`float`]
+        The duration of the audio attachment in seconds, if this is attached to a voice message
+        (see :attr:`MessageFlags.is_voice_message`).
+
+        .. versionadded:: 2.9
+
+    waveform: Optional[:class:`bytes`]
+        The byte array representing a sampled waveform, if this is attached to a voice message
+        (see :attr:`MessageFlags.is_voice_message`).
+
+        .. versionadded:: 2.9
     """
 
     __slots__ = (
         "id",
         "size",
         "height",
         "width",
         "filename",
         "url",
         "proxy_url",
         "_http",
         "content_type",
         "ephemeral",
         "description",
+        "duration",
+        "waveform",
     )
 
     def __init__(self, *, data: AttachmentPayload, state: ConnectionState) -> None:
         self.id: int = int(data["id"])
         self.size: int = data["size"]
         self.height: Optional[int] = data.get("height")
         self.width: Optional[int] = data.get("width")
         self.filename: str = data["filename"]
         self.url: str = data["url"]
         self.proxy_url: str = data["proxy_url"]
         self._http = state.http
         self.content_type: Optional[str] = data.get("content_type")
         self.ephemeral: bool = data.get("ephemeral", False)
         self.description: Optional[str] = data.get("description")
+        self.duration: Optional[float] = data.get("duration_secs")
+        self.waveform: Optional[bytes] = (
+            b64decode(waveform_data) if (waveform_data := data.get("waveform")) else None
+        )
 
     def is_spoiler(self) -> bool:
         """Whether this attachment contains a spoiler.
 
         :return type: :class:`bool`
         """
         return self.filename.startswith("SPOILER_")
@@ -467,14 +490,18 @@
             result["height"] = self.height
         if self.width:
             result["width"] = self.width
         if self.content_type:
             result["content_type"] = self.content_type
         if self.description:
             result["description"] = self.description
+        if self.duration is not None:
+            result["duration_secs"] = self.duration
+        if self.waveform is not None:
+            result["waveform"] = b64encode(self.waveform).decode("ascii")
         return result
 
 
 class DeletedReferencedMessage:
     """A special sentinel type that denotes whether the
     resolved message referenced message had since been deleted.
 
@@ -629,16 +656,15 @@
             result["fail_if_not_exists"] = self.fail_if_not_exists
         return result
 
     to_message_reference_dict = to_dict
 
 
 class InteractionReference:
-    """
-    Represents an interaction being referenced in a message.
+    """Represents an interaction being referenced in a message.
 
     This means responses to message components do not include this property,
     instead including a message reference object as components always exist on preexisting messages.
 
     .. versionadded:: 2.1
 
     Attributes
@@ -672,14 +698,48 @@
         return f"<InteractionReference id={self.id!r} type={self.type!r} name={self.name!r} user={self.user!r}>"
 
     @property
     def author(self) -> User:
         return self.user
 
 
+class RoleSubscriptionData:
+    """Represents metadata of the role subscription purchase/renewal in a message
+    of type :attr:`MessageType.role_subscription_purchase`.
+
+    .. versionadded:: 2.9
+
+    Attributes
+    ----------
+    role_subscription_listing_id: :class:`int`
+        The ID of the subscription listing the user subscribed to.
+
+        See also :attr:`RoleTags.subscription_listing_id`.
+    tier_name: :class:`str`
+        The name of the tier the user subscribed to.
+    total_months_subscribed: :class:`int`
+        The cumulative number of months the user has been subscribed for.
+    is_renewal: :class:`bool`
+        Whether this message is for a subscription renewal instead of a new subscription.
+    """
+
+    __slots__ = (
+        "role_subscription_listing_id",
+        "tier_name",
+        "total_months_subscribed",
+        "is_renewal",
+    )
+
+    def __init__(self, data: RoleSubscriptionDataPayload) -> None:
+        self.role_subscription_listing_id: int = int(data["role_subscription_listing_id"])
+        self.tier_name: str = data["tier_name"]
+        self.total_months_subscribed: int = data["total_months_subscribed"]
+        self.is_renewal: bool = data["is_renewal"]
+
+
 def flatten_handlers(cls):
     prefix = len("_handle_")
     handlers = [
         (key[prefix:], value)
         for key, value in cls.__dict__.items()
         if key.startswith("_handle_") and key != "_handle_member"
     ]
@@ -689,16 +749,15 @@
     cls._HANDLERS = handlers
     cls._CACHED_SLOTS = [attr for attr in cls.__slots__ if attr.startswith("_cs_")]
     return cls
 
 
 @flatten_handlers
 class Message(Hashable):
-    """
-    Represents a message from Discord.
+    """Represents a message from Discord.
 
     .. container:: operations
 
         .. describe:: x == y
 
             Checks if two messages are equal.
 
@@ -725,15 +784,15 @@
     content: :class:`str`
         The actual contents of the message.
     nonce: Optional[Union[:class:`str`, :class:`int`]]
         The value used by the Discord guild and the client to verify that the message is successfully sent.
         This is not stored long term within Discord's servers and is only used ephemerally.
     embeds: List[:class:`Embed`]
         A list of embeds the message has.
-    channel: Union[:class:`TextChannel`, :class:`VoiceChannel`, :class:`Thread`, :class:`DMChannel`, :class:`GroupChannel`, :class:`PartialMessageable`]
+    channel: Union[:class:`TextChannel`, :class:`VoiceChannel`, :class:`StageChannel`, :class:`Thread`, :class:`DMChannel`, :class:`GroupChannel`, :class:`PartialMessageable`]
         The channel that the message was sent from.
         Could be a :class:`DMChannel` or :class:`GroupChannel` if it's a private message.
     position: Optional[:class:`int`]
         A number that indicates the approximate position of a message in a :class:`Thread`.
         This is a number that starts at 0. e.g. the first message is position 0.
         This is `None` if the message was not sent in a :class:`Thread`, or if it was sent before July 1, 2022.
 
@@ -825,15 +884,14 @@
 
     guild: Optional[:class:`Guild`]
         The guild that the message belongs to, if applicable.
     """
 
     __slots__ = (
         "_state",
-        "_edited_timestamp",
         "_cs_channel_mentions",
         "_cs_raw_mentions",
         "_cs_clean_content",
         "_cs_raw_channel_mentions",
         "_cs_raw_role_mentions",
         "_cs_system_content",
         "tts",
@@ -857,14 +915,16 @@
         "reference",
         "interaction",
         "application",
         "activity",
         "stickers",
         "components",
         "guild",
+        "_edited_timestamp",
+        "_role_subscription_data",
     )
 
     if TYPE_CHECKING:
         _HANDLERS: ClassVar[List[Tuple[str, Callable[..., None]]]]
         _CACHED_SLOTS: ClassVar[List[str]]
         guild: Optional[Guild]
         reference: Optional[MessageReference]
@@ -926,14 +986,18 @@
         except AttributeError:
             self.guild = state._get_guild(utils._get_as_snowflake(data, "guild_id"))
 
         if thread_data := data.get("thread"):
             if not self.thread and isinstance(self.guild, Guild):
                 self.guild._store_thread(thread_data)
 
+        self._role_subscription_data: Optional[RoleSubscriptionDataPayload] = data.get(
+            "role_subscription_data"
+        )
+
         try:
             ref = data["message_reference"]
         except KeyError:
             self.reference = None
         else:
             self.reference = ref = MessageReference.with_state(state, ref)
             try:
@@ -1165,15 +1229,16 @@
         the syntax of ``<@&role_id>`` in the message content.
         """
         return [int(x) for x in re.findall(r"<@&([0-9]{17,19})>", self.content)]
 
     @utils.cached_slot_property("_cs_channel_mentions")
     def channel_mentions(self) -> List[GuildChannel]:
         """List[:class:`abc.GuildChannel`]: A list of :class:`abc.GuildChannel` that were mentioned. If the message is in a private message
-        then the list is always empty."""
+        then the list is always empty.
+        """
         if self.guild is None:
             return []
         it = filter(None, map(self.guild.get_channel, self.raw_channel_mentions))
         return utils._unique(it)
 
     @utils.cached_slot_property("_cs_clean_content")
     def clean_content(self) -> str:
@@ -1234,24 +1299,34 @@
     def jump_url(self) -> str:
         """:class:`str`: Returns a URL that allows the client to jump to this message."""
         guild_id = getattr(self.guild, "id", "@me")
         return f"https://discord.com/channels/{guild_id}/{self.channel.id}/{self.id}"
 
     @property
     def thread(self) -> Optional[Thread]:
-        """
-        Optional[:class:`Thread`]: The thread started from this message. ``None`` if no thread has been started.
+        """Optional[:class:`Thread`]: The thread started from this message. ``None`` if no thread has been started.
 
         .. versionadded:: 2.4
         """
         if not isinstance(self.guild, Guild):
             return None
 
         return self.guild.get_thread(self.id)
 
+    @property
+    def role_subscription_data(self) -> Optional[RoleSubscriptionData]:
+        """Optional[:class:`RoleSubscriptionData`]: The metadata of the role
+        subscription purchase/renewal, if this message is a :attr:`MessageType.role_subscription_purchase`.
+
+        .. versionadded:: 2.9
+        """
+        if not self._role_subscription_data:
+            return None
+        return RoleSubscriptionData(self._role_subscription_data)
+
     def is_system(self) -> bool:
         """Whether the message is a system message.
 
         A system message is a message that is constructed entirely by the Discord API
         in response to something.
 
         .. versionadded:: 1.3
@@ -1264,16 +1339,15 @@
             MessageType.application_command,
             MessageType.thread_starter_message,
             MessageType.context_menu_command,
         )
 
     @utils.cached_slot_property("_cs_system_content")
     def system_content(self) -> Optional[str]:
-        """
-        Optional[:class:`str`]: A property that returns the content that is rendered
+        """Optional[:class:`str`]: A property that returns the content that is rendered
         regardless of the :attr:`Message.type`.
 
         In the case of :attr:`MessageType.default` and :attr:`MessageType.reply`\\,
         this just returns the regular :attr:`Message.content`. Otherwise this
         returns an English message denoting the contents of the system message.
 
         If the message type is unrecognised this method will return ``None``.
@@ -1394,17 +1468,46 @@
 
         if self.type is MessageType.context_menu_command:
             return self.content
 
         if self.type is MessageType.auto_moderation_action:
             return self.content
 
+        if self.type is MessageType.role_subscription_purchase:
+            if not (data := self.role_subscription_data):
+                return
+
+            guild_name = f"**{self.guild.name}**" if self.guild else None
+            if data.total_months_subscribed > 0:
+                action = "renewed" if data.is_renewal else "joined"
+                return (
+                    f"{self.author.name} {action} **{data.tier_name}** and has been a subscriber "
+                    f"of {guild_name} for {data.total_months_subscribed} "
+                    f"{'month' if data.total_months_subscribed == 1 else 'months'}!"
+                )
+            elif data.is_renewal:
+                return f"{self.author.name} renewed **{data.tier_name}** in their {guild_name} membership!"
+            else:
+                return f"{self.author.name} joined **{data.tier_name}** as a subscriber of {guild_name}!"
+
         if self.type is MessageType.interaction_premium_upsell:
             return self.content
 
+        if self.type is MessageType.stage_start:
+            return f"{self.author.name} started {self.content}"
+
+        if self.type is MessageType.stage_end:
+            return f"{self.author.name} ended {self.content}"
+
+        if self.type is MessageType.stage_speaker:
+            return f"{self.author.name} is now a speaker."
+
+        if self.type is MessageType.stage_topic:
+            return f"{self.author.name} changed the Stage topic: {self.content}"
+
         if self.type is MessageType.guild_application_premium_subscription:
             application_name = (
                 self.application["name"]
                 if self.application and "name" in self.application
                 else "a deleted application"
             )
             return f"{self.author.name} upgraded {application_name} to premium for this server! 🎉"
@@ -1457,14 +1560,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embed: Optional[Embed] = ...,
         file: File = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
         delete_after: Optional[float] = ...,
     ) -> Message:
         ...
 
@@ -1473,14 +1577,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embed: Optional[Embed] = ...,
         files: List[File] = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
         delete_after: Optional[float] = ...,
     ) -> Message:
         ...
 
@@ -1489,14 +1594,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embeds: List[Embed] = ...,
         file: File = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
         delete_after: Optional[float] = ...,
     ) -> Message:
         ...
 
@@ -1505,14 +1611,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embeds: List[Embed] = ...,
         files: List[File] = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
         delete_after: Optional[float] = ...,
     ) -> Message:
         ...
 
@@ -1523,14 +1630,15 @@
         embed: Optional[Embed] = MISSING,
         embeds: List[Embed] = MISSING,
         file: File = MISSING,
         files: List[File] = MISSING,
         attachments: Optional[List[Attachment]] = MISSING,
         suppress: bool = MISSING,  # deprecated
         suppress_embeds: bool = MISSING,
+        flags: MessageFlags = MISSING,
         allowed_mentions: Optional[AllowedMentions] = MISSING,
         view: Optional[View] = MISSING,
         components: Optional[Components[MessageUIComponent]] = MISSING,
         delete_after: Optional[float] = None,
     ) -> Message:
         """|coro|
 
@@ -1599,14 +1707,23 @@
                 Supports passing ``None`` to clear attachments.
 
         suppress_embeds: :class:`bool`
             Whether to suppress embeds for the message. This hides
             all the embeds from the UI if set to ``True``. If set
             to ``False``, this brings the embeds back if they were
             suppressed.
+        flags: :class:`MessageFlags`
+            The new flags to set for this message. Overrides existing flags.
+            Only :attr:`~MessageFlags.suppress_embeds` is supported.
+
+            If parameter ``suppress_embeds`` is provided,
+            that will override the setting of :attr:`.MessageFlags.suppress_embeds`.
+
+            .. versionadded:: 2.9
+
         delete_after: Optional[:class:`float`]
             If provided, the number of seconds to wait in the background
             before deleting the message we just edited. If the deletion fails,
             then it is silently ignored.
         allowed_mentions: Optional[:class:`~disnake.AllowedMentions`]
             Controls the mentions being processed in this message. If this is
             passed, then the object is merged with :attr:`Client.allowed_mentions`.
@@ -1663,14 +1780,15 @@
             embed=embed,
             embeds=embeds,
             file=file,
             files=files,
             attachments=attachments,
             suppress=suppress,
             suppress_embeds=suppress_embeds,
+            flags=flags,
             allowed_mentions=allowed_mentions,
             view=view,
             components=components,
             delete_after=delete_after,
         )
 
     async def publish(self) -> None:
@@ -1696,14 +1814,16 @@
         """|coro|
 
         Pins the message.
 
         You must have the :attr:`~Permissions.manage_messages` permission to do
         this in a non-private channel context.
 
+        This does not work with messages sent in a :class:`VoiceChannel` or :class:`StageChannel`.
+
         Parameters
         ----------
         reason: Optional[:class:`str`]
             The reason for pinning the message. Shows up on the audit log.
 
             .. versionadded:: 1.4
 
@@ -1711,15 +1831,15 @@
         ------
         Forbidden
             You do not have permissions to pin the message.
         NotFound
             The message or channel was not found or deleted.
         HTTPException
             Pinning the message failed, probably due to the channel
-            having more than 50 pinned messages.
+            having more than 50 pinned messages or the channel not supporting pins.
         """
         await self._state.http.pin_message(self.channel.id, self.id, reason=reason)
         self.pinned = True
 
     async def unpin(self, *, reason: Optional[str] = None) -> None:
         """|coro|
 
@@ -2033,14 +2153,15 @@
     a message and channel ID are present.
 
     There are two ways to construct this class. The first one is through
     the constructor itself, and the second is via the following:
 
     - :meth:`TextChannel.get_partial_message`
     - :meth:`VoiceChannel.get_partial_message`
+    - :meth:`StageChannel.get_partial_message`
     - :meth:`Thread.get_partial_message`
     - :meth:`DMChannel.get_partial_message`
     - :meth:`PartialMessageable.get_partial_message`
 
     Note that this class is trimmed down and has no rich attributes.
 
     .. versionadded:: 1.6
@@ -2057,15 +2178,15 @@
 
         .. describe:: hash(x)
 
             Returns the partial message's hash.
 
     Attributes
     ----------
-    channel: Union[:class:`TextChannel`, :class:`Thread`, :class:`DMChannel`, :class:`VoiceChannel`, :class:`PartialMessageable`]
+    channel: Union[:class:`TextChannel`, :class:`Thread`, :class:`DMChannel`, :class:`VoiceChannel`, :class:`StageChannel`, :class:`PartialMessageable`]
         The channel associated with this partial message.
     id: :class:`int`
         The message ID.
     """
 
     __slots__ = ("channel", "id", "_cs_guild", "_state")
 
@@ -2087,17 +2208,18 @@
             ChannelType.text,
             ChannelType.news,
             ChannelType.private,
             ChannelType.news_thread,
             ChannelType.public_thread,
             ChannelType.private_thread,
             ChannelType.voice,
+            ChannelType.stage_voice,
         ):
             raise TypeError(
-                f"Expected TextChannel, DMChannel, VoiceChannel, Thread, or PartialMessageable "
+                f"Expected TextChannel, VoiceChannel, DMChannel, StageChannel, Thread, or PartialMessageable "
                 f"with a valid type, not {type(channel)!r} (type: {channel.type!r})"
             )
 
         self.channel: MessageableChannel = channel
         self._state: ConnectionState = channel._state
         self.id: int = id
 
@@ -2150,14 +2272,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embed: Optional[Embed] = ...,
         file: File = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
         delete_after: Optional[float] = ...,
     ) -> Message:
         ...
 
@@ -2166,14 +2289,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embed: Optional[Embed] = ...,
         files: List[File] = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
         delete_after: Optional[float] = ...,
     ) -> Message:
         ...
 
@@ -2182,14 +2306,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embeds: List[Embed] = ...,
         file: File = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
         delete_after: Optional[float] = ...,
     ) -> Message:
         ...
 
@@ -2198,14 +2323,15 @@
         self,
         content: Optional[str] = ...,
         *,
         embeds: List[Embed] = ...,
         files: List[File] = ...,
         attachments: Optional[List[Attachment]] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: Optional[AllowedMentions] = ...,
         view: Optional[View] = ...,
         components: Optional[Components[MessageUIComponent]] = ...,
         delete_after: Optional[float] = ...,
     ) -> Message:
         ...
 
@@ -2216,14 +2342,15 @@
         embed: Optional[Embed] = MISSING,
         embeds: List[Embed] = MISSING,
         file: File = MISSING,
         files: List[File] = MISSING,
         attachments: Optional[List[Attachment]] = MISSING,
         suppress: bool = MISSING,  # deprecated
         suppress_embeds: bool = MISSING,
+        flags: MessageFlags = MISSING,
         allowed_mentions: Optional[AllowedMentions] = MISSING,
         view: Optional[View] = MISSING,
         components: Optional[Components[MessageUIComponent]] = MISSING,
         delete_after: Optional[float] = None,
     ) -> Message:
         """|coro|
 
@@ -2294,14 +2421,23 @@
                 Supports passing ``None`` to clear attachments.
 
         suppress_embeds: :class:`bool`
             Whether to suppress embeds for the message. This hides
             all the embeds from the UI if set to ``True``. If set
             to ``False``, this brings the embeds back if they were
             suppressed.
+        flags: :class:`MessageFlags`
+            The new flags to set for this message. Overrides existing flags.
+            Only :attr:`~MessageFlags.suppress_embeds` is supported.
+
+            If parameter ``suppress_embeds`` is provided,
+            that will override the setting of :attr:`.MessageFlags.suppress_embeds`.
+
+            .. versionadded:: 2.9
+
         delete_after: Optional[:class:`float`]
             If provided, the number of seconds to wait in the background
             before deleting the message we just edited. If the deletion fails,
             then it is silently ignored.
         allowed_mentions: Optional[:class:`~disnake.AllowedMentions`]
             Controls the mentions being processed in this message. If this is
             passed, then the object is merged with :attr:`Client.allowed_mentions`.
@@ -2353,12 +2489,13 @@
             embed=embed,
             embeds=embeds,
             file=file,
             files=files,
             attachments=attachments,
             suppress=suppress,
             suppress_embeds=suppress_embeds,
+            flags=flags,
             allowed_mentions=allowed_mentions,
             view=view,
             components=components,
             delete_after=delete_after,
         )
```

### Comparing `disnake-2.8.2/disnake/mixins.py` & `disnake-2.9.0/disnake/mixins.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/object.py` & `disnake-2.9.0/disnake/object.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/oggparse.py` & `disnake-2.9.0/disnake/oggparse.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/opus.py` & `disnake-2.9.0/disnake/opus.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,27 +223,27 @@
         except KeyError:
             _log.exception("Error assigning check function to %s", func)
 
     return lib
 
 
 def _load_default() -> bool:
-    global _lib
+    global _lib  # noqa: PLW0603
     try:
         if sys.platform == "win32":
             _basedir = os.path.dirname(os.path.abspath(__file__))
             _bitness = struct.calcsize("P") * 8
             _target = "x64" if _bitness > 32 else "x86"
             _filename = os.path.join(_basedir, "bin", f"libopus-0.{_target}.dll")
-            _lib = libopus_loader(_filename)
+            _lib = libopus_loader(_filename)  # noqa: PLW0603
         else:
             path = ctypes.util.find_library("opus")
             if not path:
                 raise AssertionError("could not find the opus library")
-            _lib = libopus_loader(path)
+            _lib = libopus_loader(path)  # noqa: PLW0603
     except Exception:
         _lib = MISSING
 
     return _lib is not MISSING
 
 
 def load_opus(name: str) -> None:
@@ -277,30 +277,29 @@
         without you having to call this.
 
     Parameters
     ----------
     name: :class:`str`
         The filename of the shared library.
     """
-    global _lib
+    global _lib  # noqa: PLW0603
     _lib = libopus_loader(name)
 
 
 def is_loaded() -> bool:
     """Function to check if opus lib is successfully loaded either
     via the :func:`ctypes.util.find_library` call of :func:`load_opus`.
 
     This must return ``True`` for voice to work.
 
     Returns
     -------
     :class:`bool`
         Indicates if the opus library has been loaded.
     """
-    global _lib
     return _lib is not MISSING
 
 
 class OpusError(DiscordException):
     """An exception that is thrown for libopus related errors.
 
     Attributes
@@ -330,15 +329,15 @@
     SAMPLES_PER_FRAME = int(SAMPLING_RATE / 1000 * FRAME_LENGTH)
 
     FRAME_SIZE = SAMPLES_PER_FRAME * SAMPLE_SIZE
 
     @staticmethod
     def get_opus_version() -> str:
         if not is_loaded() and not _load_default():
-            raise OpusNotLoaded()
+            raise OpusNotLoaded
 
         return _lib.opus_get_version_string().decode("utf-8")
 
 
 class Encoder(_OpusStruct):
     def __init__(self, application: int = APPLICATION_AUDIO) -> None:
         _OpusStruct.get_opus_version()
@@ -445,25 +444,23 @@
         gain = 10**x/(20.0*256)
         (from opus_defines.h)
         """
         return _lib.opus_decoder_ctl(self._state, CTL_SET_GAIN, adjustment)
 
     def set_gain(self, dB: float) -> int:
         """Sets the decoder gain in dB, from -128 to 128."""
-
         dB_Q8 = max(-32768, min(32767, round(dB * 256)))  # dB * 2^n where n is 8 (Q8)
         return self._set_gain(dB_Q8)
 
     def set_volume(self, mult: float) -> int:
         """Sets the output volume as a float percent, i.e. 0.5 for 50%, 1.75 for 175%, etc."""
         return self.set_gain(20 * math.log10(mult))  # amplitude ratio
 
     def _get_last_packet_duration(self) -> int:
         """Gets the duration (in samples) of the last packet successfully decoded or concealed."""
-
         ret = ctypes.c_int32()
         _lib.opus_decoder_ctl(self._state, CTL_LAST_PACKET_DURATION, ctypes.byref(ret))
         return ret.value
 
     @overload
     def decode(self, data: bytes, *, fec: bool) -> bytes:
         ...
```

### Comparing `disnake-2.8.2/disnake/partial_emoji.py` & `disnake-2.9.0/disnake/partial_emoji.py`

 * *Files 11% similar despite different names*

```diff
@@ -263,29 +263,7 @@
             emoji = PartialEmoji.from_str(emoji)
 
         # note: API only supports exactly one of `name` and `id` being set
         if emoji.id:
             return None, emoji.id
         else:
             return emoji.name, None
-
-    # utility method for unusual emoji model in forums
-    @staticmethod
-    def _emoji_from_name_id(
-        name: Optional[str], id: Optional[int], *, state: ConnectionState
-    ) -> Optional[Union[Emoji, PartialEmoji]]:
-        if not (name or id):
-            return None
-
-        emoji: Optional[Union[Emoji, PartialEmoji]] = None
-        if id:
-            emoji = state.get_emoji(id)
-        if not emoji:
-            emoji = PartialEmoji.with_state(
-                state=state,
-                # Note: this does not render correctly if it's a custom emoji, there's just no name information for those here.
-                # This may change in a future API version, but for now we'll just have to accept it.
-                name=name or "",
-                id=id,
-                # `animated` is unknown but presumably we already got the (animated) emoji from the guild cache at this point
-            )
-        return emoji
```

### Comparing `disnake-2.8.2/disnake/permissions.py` & `disnake-2.9.0/disnake/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,15 @@
         external_stickers: bool = ...,
         kick_members: bool = ...,
         manage_channels: bool = ...,
         manage_emojis: bool = ...,
         manage_emojis_and_stickers: bool = ...,
         manage_events: bool = ...,
         manage_guild: bool = ...,
+        manage_guild_expressions: bool = ...,
         manage_messages: bool = ...,
         manage_nicknames: bool = ...,
         manage_permissions: bool = ...,
         manage_roles: bool = ...,
         manage_threads: bool = ...,
         manage_webhooks: bool = ...,
         mention_everyone: bool = ...,
@@ -191,25 +192,29 @@
         priority_speaker: bool = ...,
         read_message_history: bool = ...,
         read_messages: bool = ...,
         request_to_speak: bool = ...,
         send_messages: bool = ...,
         send_messages_in_threads: bool = ...,
         send_tts_messages: bool = ...,
+        send_voice_messages: bool = ...,
         speak: bool = ...,
         start_embedded_activities: bool = ...,
         stream: bool = ...,
         use_application_commands: bool = ...,
         use_embedded_activities: bool = ...,
         use_external_emojis: bool = ...,
+        use_external_sounds: bool = ...,
         use_external_stickers: bool = ...,
         use_slash_commands: bool = ...,
+        use_soundboard: bool = ...,
         use_voice_activation: bool = ...,
         view_audit_log: bool = ...,
         view_channel: bool = ...,
+        view_creator_monetization_analytics: bool = ...,
         view_guild_insights: bool = ...,
     ) -> None:
         ...
 
     @overload
     @_generated
     def __init__(
@@ -263,15 +268,16 @@
     __lt__ = is_strict_subset  # type: ignore
     __gt__ = is_strict_superset  # type: ignore
 
     @classmethod
     @cached_creation
     def none(cls) -> Self:
         """A factory method that creates a :class:`Permissions` with all
-        permissions set to ``False``."""
+        permissions set to ``False``.
+        """
         return cls(0)
 
     @classmethod
     @cached_creation
     def all(cls) -> Self:
         """A factory method that creates a :class:`Permissions` with all
         permissions set to ``True``.
@@ -281,70 +287,79 @@
     @classmethod
     @cached_creation
     def all_channel(cls) -> Self:
         """A :class:`Permissions` with all channel-specific permissions set to
         ``True`` and the guild-specific ones set to ``False``. The guild-specific
         permissions are currently:
 
-        - :attr:`manage_emojis`
+        - :attr:`manage_guild_expressions`
         - :attr:`view_audit_log`
         - :attr:`view_guild_insights`
+        - :attr:`view_creator_monetization_analytics`
         - :attr:`manage_guild`
         - :attr:`change_nickname`
         - :attr:`manage_nicknames`
         - :attr:`kick_members`
         - :attr:`ban_members`
+        - :attr:`moderate_members`
         - :attr:`administrator`
 
         .. versionchanged:: 1.7
            Added :attr:`stream`, :attr:`priority_speaker` and :attr:`use_slash_commands` permissions.
 
         .. versionchanged:: 2.0
            Added :attr:`create_public_threads`, :attr:`create_private_threads`, :attr:`manage_threads`,
            :attr:`use_external_stickers`, :attr:`send_messages_in_threads` and
            :attr:`request_to_speak` permissions.
 
         .. versionchanged:: 2.3
             Added :attr:`use_embedded_activities` permission.
+
+        .. versionchanged:: 2.9
+            Added :attr:`use_soundboard` and :attr:`send_voice_messages` permissions.
         """
-        guild_specific_perms = {
-            "administrator",
-            "ban_members",
-            "change_nickname",
-            "kick_members",
-            "manage_emojis",
-            "manage_guild",
-            "manage_nicknames",
-            "moderate_members",
-            "view_audit_log",
-            "view_guild_insights",
-        }
         instance = cls.all()
-        instance.update(**dict.fromkeys(guild_specific_perms, False))
+        instance.update(
+            administrator=False,
+            ban_members=False,
+            change_nickname=False,
+            kick_members=False,
+            manage_guild=False,
+            manage_guild_expressions=False,
+            manage_nicknames=False,
+            moderate_members=False,
+            view_audit_log=False,
+            view_guild_insights=False,
+            view_creator_monetization_analytics=False,
+        )
         return instance
 
     @classmethod
     @cached_creation
     def general(cls) -> Self:
         """A factory method that creates a :class:`Permissions` with all
         "General" permissions from the official Discord UI set to ``True``.
 
         .. versionchanged:: 1.7
            Permission :attr:`read_messages` is now included in the general permissions, but
            permissions :attr:`administrator`, :attr:`create_instant_invite`, :attr:`kick_members`,
            :attr:`ban_members`, :attr:`change_nickname` and :attr:`manage_nicknames` are
            no longer part of the general permissions.
+
+        .. versionchanged:: 2.9
+            Added :attr:`view_creator_monetization_analytics` permission.
         """
         return cls(
             view_channel=True,
             manage_channels=True,
             manage_roles=True,
-            manage_emojis_and_stickers=True,
+            manage_guild_expressions=True,
             view_audit_log=True,
             view_guild_insights=True,
+            view_creator_monetization_analytics=True,
             manage_webhooks=True,
             manage_guild=True,
         )
 
     @classmethod
     @cached_creation
     def membership(cls) -> Self:
@@ -374,14 +389,17 @@
         .. versionchanged:: 1.7
            Permission :attr:`read_messages` is no longer part of the text permissions.
            Added :attr:`use_slash_commands` permission.
 
         .. versionchanged:: 2.0
            Added :attr:`create_public_threads`, :attr:`create_private_threads`, :attr:`manage_threads`,
            :attr:`send_messages_in_threads` and :attr:`use_external_stickers` permissions.
+
+        .. versionchanged:: 2.9
+            Added :attr:`send_voice_messages` permission.
         """
         return cls(
             send_messages=True,
             send_messages_in_threads=True,
             create_public_threads=True,
             create_private_threads=True,
             embed_links=True,
@@ -391,30 +409,36 @@
             use_external_stickers=True,
             mention_everyone=True,
             manage_messages=True,
             manage_threads=True,
             read_message_history=True,
             send_tts_messages=True,
             use_slash_commands=True,
+            send_voice_messages=True,
         )
 
     @classmethod
     @cached_creation
     def voice(cls) -> Self:
         """A factory method that creates a :class:`Permissions` with all
         "Voice" permissions from the official Discord UI set to ``True``.
 
         .. versionchanged:: 2.3
             Added :attr:`use_embedded_activities` permission.
+
+        .. versionchanged:: 2.9
+            Added :attr:`use_soundboard` and :attr:`use_external_sounds` permissions.
         """
         return cls(
             connect=True,
             speak=True,
             stream=True,
             use_embedded_activities=True,
+            use_soundboard=True,
+            use_external_sounds=True,
             use_voice_activation=True,
             priority_speaker=True,
             mute_members=True,
             deafen_members=True,
             move_members=True,
         )
 
@@ -518,14 +542,15 @@
         external_stickers: bool = ...,
         kick_members: bool = ...,
         manage_channels: bool = ...,
         manage_emojis: bool = ...,
         manage_emojis_and_stickers: bool = ...,
         manage_events: bool = ...,
         manage_guild: bool = ...,
+        manage_guild_expressions: bool = ...,
         manage_messages: bool = ...,
         manage_nicknames: bool = ...,
         manage_permissions: bool = ...,
         manage_roles: bool = ...,
         manage_threads: bool = ...,
         manage_webhooks: bool = ...,
         mention_everyone: bool = ...,
@@ -535,40 +560,43 @@
         priority_speaker: bool = ...,
         read_message_history: bool = ...,
         read_messages: bool = ...,
         request_to_speak: bool = ...,
         send_messages: bool = ...,
         send_messages_in_threads: bool = ...,
         send_tts_messages: bool = ...,
+        send_voice_messages: bool = ...,
         speak: bool = ...,
         start_embedded_activities: bool = ...,
         stream: bool = ...,
         use_application_commands: bool = ...,
         use_embedded_activities: bool = ...,
         use_external_emojis: bool = ...,
+        use_external_sounds: bool = ...,
         use_external_stickers: bool = ...,
         use_slash_commands: bool = ...,
+        use_soundboard: bool = ...,
         use_voice_activation: bool = ...,
         view_audit_log: bool = ...,
         view_channel: bool = ...,
+        view_creator_monetization_analytics: bool = ...,
         view_guild_insights: bool = ...,
     ) -> None:
         ...
 
     @overload
     @_generated
     def update(
         self,
     ) -> None:
         ...
 
     @_overload_with_permissions
     def update(self, **kwargs: bool) -> None:
-        """
-        Bulk updates this permission object.
+        """Bulk updates this permission object.
 
         Allows you to set multiple attributes by using keyword
         arguments. The names must be equivalent to the properties
         listed. Extraneous key/value pairs will be silently ignored.
 
         Arguments are applied in order, similar to the constructor.
 
@@ -619,15 +647,16 @@
         """
         return 1 << 3
 
     @flag_value
     def manage_channels(self) -> int:
         """:class:`bool`: Returns ``True`` if a user can edit, delete, or create channels in the guild.
 
-        This also corresponds to the "Manage Channel" channel-specific override."""
+        This also corresponds to the "Manage Channel" channel-specific override.
+        """
         return 1 << 4
 
     @flag_value
     def manage_guild(self) -> int:
         """:class:`bool`: Returns ``True`` if a user can edit guild properties."""
         return 1 << 5
 
@@ -666,15 +695,16 @@
     def read_messages(self) -> int:
         """:class:`bool`: An alias for :attr:`view_channel`."""
         return 1 << 10
 
     @flag_value
     def send_messages(self) -> int:
         """:class:`bool`: Returns ``True`` if a user can send messages from all or specific text channels
-        and create threads in forum channels."""
+        and create threads in forum channels.
+        """
         return 1 << 11
 
     @make_permission_alias("send_messages")
     def create_forum_threads(self) -> int:
         """:class:`bool`: An alias for :attr:`send_messages`.
 
         .. versionadded:: 2.5
@@ -795,21 +825,30 @@
 
     @flag_value
     def manage_webhooks(self) -> int:
         """:class:`bool`: Returns ``True`` if a user can create, edit, or delete webhooks."""
         return 1 << 29
 
     @flag_value
+    def manage_guild_expressions(self) -> int:
+        """:class:`bool`: Returns ``True`` if a user can create, edit, or delete
+        emojis, stickers, and soundboard sounds.
+
+        .. versionadded:: 2.9
+        """
+        return 1 << 30
+
+    @make_permission_alias("manage_guild_expressions")
     def manage_emojis(self) -> int:
-        """:class:`bool`: Returns ``True`` if a user can create, edit, or delete emojis."""
+        """:class:`bool`: An alias for :attr:`manage_guild_expressions`."""
         return 1 << 30
 
-    @make_permission_alias("manage_emojis")
+    @make_permission_alias("manage_guild_expressions")
     def manage_emojis_and_stickers(self) -> int:
-        """:class:`bool`: An alias for :attr:`manage_emojis`.
+        """:class:`bool`: An alias for :attr:`manage_guild_expressions`.
 
         .. versionadded:: 2.0
         """
         return 1 << 30
 
     @flag_value
     def use_application_commands(self) -> int:
@@ -919,14 +958,46 @@
         """:class:`bool`: Returns ``True`` if a user can perform limited moderation actions,
         such as timeouts or editing members' flags.
 
         .. versionadded:: 2.3
         """
         return 1 << 40
 
+    @flag_value
+    def view_creator_monetization_analytics(self) -> int:
+        """:class:`bool`: Returns ``True`` if a user can view role subscription insights.
+
+        .. versionadded:: 2.9
+        """
+        return 1 << 41
+
+    @flag_value
+    def use_soundboard(self) -> int:
+        """:class:`bool`: Returns ``True`` if a user can use the soundboard in voice channels.
+
+        .. versionadded:: 2.9
+        """
+        return 1 << 42
+
+    @flag_value
+    def use_external_sounds(self) -> int:
+        """:class:`bool`: Returns ``True`` if a user can use custom soundboard sounds from other guilds.
+
+        .. versionadded:: 2.9
+        """
+        return 1 << 45
+
+    @flag_value
+    def send_voice_messages(self) -> int:
+        """:class:`bool`: Returns ``True`` if a user can send voice messages.
+
+        .. versionadded:: 2.9
+        """
+        return 1 << 46
+
 
 def _augment_from_permissions(cls):
     cls.VALID_NAMES = set(Permissions.VALID_FLAGS)
     aliases = set()
 
     # make descriptors for all the valid names and aliases
     for name, value in Permissions.__dict__.items():
@@ -950,16 +1021,15 @@
 
     cls.PURE_FLAGS = cls.VALID_NAMES - aliases
     return cls
 
 
 @_augment_from_permissions
 class PermissionOverwrite:
-    """
-    A type that is used to represent a channel specific permission.
+    """A type that is used to represent a channel specific permission.
 
     Unlike a regular :class:`Permissions`\\, the default value of a
     permission is equivalent to ``None`` and not ``False``. Setting
     a value to ``False`` is **explicitly** denying that permission,
     while setting a value to ``True`` is **explicitly** allowing
     that permission.
 
@@ -1006,14 +1076,15 @@
         external_stickers: Optional[bool]
         kick_members: Optional[bool]
         manage_channels: Optional[bool]
         manage_emojis: Optional[bool]
         manage_emojis_and_stickers: Optional[bool]
         manage_events: Optional[bool]
         manage_guild: Optional[bool]
+        manage_guild_expressions: Optional[bool]
         manage_messages: Optional[bool]
         manage_nicknames: Optional[bool]
         manage_permissions: Optional[bool]
         manage_roles: Optional[bool]
         manage_threads: Optional[bool]
         manage_webhooks: Optional[bool]
         mention_everyone: Optional[bool]
@@ -1023,25 +1094,29 @@
         priority_speaker: Optional[bool]
         read_message_history: Optional[bool]
         read_messages: Optional[bool]
         request_to_speak: Optional[bool]
         send_messages: Optional[bool]
         send_messages_in_threads: Optional[bool]
         send_tts_messages: Optional[bool]
+        send_voice_messages: Optional[bool]
         speak: Optional[bool]
         start_embedded_activities: Optional[bool]
         stream: Optional[bool]
         use_application_commands: Optional[bool]
         use_embedded_activities: Optional[bool]
         use_external_emojis: Optional[bool]
+        use_external_sounds: Optional[bool]
         use_external_stickers: Optional[bool]
         use_slash_commands: Optional[bool]
+        use_soundboard: Optional[bool]
         use_voice_activation: Optional[bool]
         view_audit_log: Optional[bool]
         view_channel: Optional[bool]
+        view_creator_monetization_analytics: Optional[bool]
         view_guild_insights: Optional[bool]
 
     if TYPE_CHECKING:
         VALID_NAMES: ClassVar[Set[str]]
         PURE_FLAGS: ClassVar[Set[str]]
 
     @overload
@@ -1065,14 +1140,15 @@
         external_stickers: Optional[bool] = ...,
         kick_members: Optional[bool] = ...,
         manage_channels: Optional[bool] = ...,
         manage_emojis: Optional[bool] = ...,
         manage_emojis_and_stickers: Optional[bool] = ...,
         manage_events: Optional[bool] = ...,
         manage_guild: Optional[bool] = ...,
+        manage_guild_expressions: Optional[bool] = ...,
         manage_messages: Optional[bool] = ...,
         manage_nicknames: Optional[bool] = ...,
         manage_permissions: Optional[bool] = ...,
         manage_roles: Optional[bool] = ...,
         manage_threads: Optional[bool] = ...,
         manage_webhooks: Optional[bool] = ...,
         mention_everyone: Optional[bool] = ...,
@@ -1082,25 +1158,29 @@
         priority_speaker: Optional[bool] = ...,
         read_message_history: Optional[bool] = ...,
         read_messages: Optional[bool] = ...,
         request_to_speak: Optional[bool] = ...,
         send_messages: Optional[bool] = ...,
         send_messages_in_threads: Optional[bool] = ...,
         send_tts_messages: Optional[bool] = ...,
+        send_voice_messages: Optional[bool] = ...,
         speak: Optional[bool] = ...,
         start_embedded_activities: Optional[bool] = ...,
         stream: Optional[bool] = ...,
         use_application_commands: Optional[bool] = ...,
         use_embedded_activities: Optional[bool] = ...,
         use_external_emojis: Optional[bool] = ...,
+        use_external_sounds: Optional[bool] = ...,
         use_external_stickers: Optional[bool] = ...,
         use_slash_commands: Optional[bool] = ...,
+        use_soundboard: Optional[bool] = ...,
         use_voice_activation: Optional[bool] = ...,
         view_audit_log: Optional[bool] = ...,
         view_channel: Optional[bool] = ...,
+        view_creator_monetization_analytics: Optional[bool] = ...,
         view_guild_insights: Optional[bool] = ...,
     ) -> None:
         ...
 
     @overload
     @_generated
     def __init__(
@@ -1128,15 +1208,14 @@
         if value is None:
             self._values.pop(key, None)
         else:
             self._values[key] = value
 
     def pair(self) -> Tuple[Permissions, Permissions]:
         """Tuple[:class:`Permissions`, :class:`Permissions`]: Returns the (allow, deny) pair from this overwrite."""
-
         allow = Permissions.none()
         deny = Permissions.none()
 
         for key, value in self._values.items():
             if value is True:
                 setattr(allow, key, True)
             elif value is False:
@@ -1192,14 +1271,15 @@
         external_stickers: Optional[bool] = ...,
         kick_members: Optional[bool] = ...,
         manage_channels: Optional[bool] = ...,
         manage_emojis: Optional[bool] = ...,
         manage_emojis_and_stickers: Optional[bool] = ...,
         manage_events: Optional[bool] = ...,
         manage_guild: Optional[bool] = ...,
+        manage_guild_expressions: Optional[bool] = ...,
         manage_messages: Optional[bool] = ...,
         manage_nicknames: Optional[bool] = ...,
         manage_permissions: Optional[bool] = ...,
         manage_roles: Optional[bool] = ...,
         manage_threads: Optional[bool] = ...,
         manage_webhooks: Optional[bool] = ...,
         mention_everyone: Optional[bool] = ...,
@@ -1209,40 +1289,43 @@
         priority_speaker: Optional[bool] = ...,
         read_message_history: Optional[bool] = ...,
         read_messages: Optional[bool] = ...,
         request_to_speak: Optional[bool] = ...,
         send_messages: Optional[bool] = ...,
         send_messages_in_threads: Optional[bool] = ...,
         send_tts_messages: Optional[bool] = ...,
+        send_voice_messages: Optional[bool] = ...,
         speak: Optional[bool] = ...,
         start_embedded_activities: Optional[bool] = ...,
         stream: Optional[bool] = ...,
         use_application_commands: Optional[bool] = ...,
         use_embedded_activities: Optional[bool] = ...,
         use_external_emojis: Optional[bool] = ...,
+        use_external_sounds: Optional[bool] = ...,
         use_external_stickers: Optional[bool] = ...,
         use_slash_commands: Optional[bool] = ...,
+        use_soundboard: Optional[bool] = ...,
         use_voice_activation: Optional[bool] = ...,
         view_audit_log: Optional[bool] = ...,
         view_channel: Optional[bool] = ...,
+        view_creator_monetization_analytics: Optional[bool] = ...,
         view_guild_insights: Optional[bool] = ...,
     ) -> None:
         ...
 
     @overload
     @_generated
     def update(
         self,
     ) -> None:
         ...
 
     @_overload_with_permissions
     def update(self, **kwargs: Optional[bool]) -> None:
-        """
-        Bulk updates this permission overwrite object.
+        """Bulk updates this permission overwrite object.
 
         Allows you to set multiple attributes by using keyword
         arguments. The names must be equivalent to the properties
         listed. Extraneous key/value pairs will be silently ignored.
 
         Parameters
         ----------
```

### Comparing `disnake-2.8.2/disnake/player.py` & `disnake-2.9.0/disnake/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import asyncio
 import io
 import logging
 import re
 import shlex
-import subprocess
+import subprocess  # noqa: TID251
 import sys
 import threading
 import time
 import traceback
 import warnings
 from typing import IO, TYPE_CHECKING, Any, Callable, Generic, Optional, Tuple, TypeVar, Union
 
@@ -362,20 +362,19 @@
     def __init__(
         self,
         source: Union[str, io.BufferedIOBase],
         *,
         bitrate: int = 128,
         codec: Optional[str] = None,
         executable: str = "ffmpeg",
-        pipe=False,
+        pipe: bool = False,
         stderr=None,
         before_options=None,
         options=None,
     ) -> None:
-
         args = []
         subprocess_kwargs = {
             "stdin": subprocess.PIPE if pipe else subprocess.DEVNULL,
             "stderr": stderr,
         }
 
         if isinstance(before_options, str):
@@ -426,15 +425,14 @@
         """|coro|
 
         A factory method that creates a :class:`FFmpegOpusAudio` after probing
         the input source for audio codec and bitrate information.
 
         Examples
         --------
-
         Use this function to create an :class:`FFmpegOpusAudio` instance instead of the constructor: ::
 
             source = await disnake.FFmpegOpusAudio.from_probe("song.webm")
             voice_client.play(source)
 
         If you are on Windows and don't have ffprobe installed, use the ``fallback`` method
         to probe using ffmpeg instead: ::
@@ -473,15 +471,14 @@
             Invalid value for ``probe`` parameter, must be :class:`str` or a callable.
 
         Returns
         -------
         :class:`FFmpegOpusAudio`
             An instance of this class.
         """
-
         executable = kwargs.get("executable")
         codec, bitrate = await cls.probe(source, method=method, executable=executable)
         return cls(source, bitrate=bitrate, codec=codec, **kwargs)  # type: ignore
 
     @classmethod
     async def probe(
         cls,
@@ -513,15 +510,14 @@
             Invalid value for ``probe`` parameter, must be :class:`str` or a callable.
 
         Returns
         -------
         Optional[Tuple[Optional[:class:`str`], Optional[:class:`int`]]]
             A 2-tuple with the codec and bitrate of the input source.
         """
-
         method = method or "native"
         executable = executable or "ffmpeg"
         probefunc = fallback = None
 
         if isinstance(method, str):
             probefunc = getattr(cls, f"_probe_codec_{method}", None)
             if probefunc is None:
```

### Comparing `disnake-2.8.2/disnake/raw_models.py` & `disnake-2.9.0/disnake/raw_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,14 +160,18 @@
         The user ID who added the reaction or whose reaction was removed.
     channel_id: :class:`int`
         The channel ID where the reaction addition or removal took place.
     guild_id: Optional[:class:`int`]
         The guild ID where the reaction addition or removal took place, if applicable.
     emoji: :class:`PartialEmoji`
         The custom or unicode emoji being used.
+
+        .. versionchanged:: 2.9
+            This now also includes the correct :attr:`~PartialEmoji.animated` value when a reaction was removed.
+
     member: Optional[:class:`Member`]
         The member who added the reaction. Only available if `event_type` is `REACTION_ADD` and the reaction is inside a guild.
 
         .. versionadded:: 1.3
 
     event_type: :class:`str`
         The event type that triggered this action. Can be
@@ -232,14 +236,17 @@
         The message ID that got its reactions cleared.
     channel_id: :class:`int`
         The channel ID where the reaction clear took place.
     guild_id: Optional[:class:`int`]
         The guild ID where the reaction clear took place, if applicable.
     emoji: :class:`PartialEmoji`
         The custom or unicode emoji being removed.
+
+        .. versionchanged:: 2.9
+            This now also includes the correct :attr:`~PartialEmoji.animated` value.
     """
 
     __slots__ = ("message_id", "channel_id", "guild_id", "emoji")
 
     def __init__(self, data: MessageReactionRemoveEmojiEvent, emoji: PartialEmoji) -> None:
         self.emoji: PartialEmoji = emoji
         self.message_id: int = int(data["message_id"])
@@ -377,23 +384,28 @@
         The ID of the channel where the user started typing.
     guild_id: Optional[:class:`int`]
         The ID of the guild where the user started typing or ``None`` if it was in a DM.
     member: Optional[:class:`Member`]
         The member object of the user who started typing or ``None`` if it was in a DM.
     timestamp: :class:`datetime.datetime`
         The UTC datetime when the user started typing.
+
+        .. versionchanged:: 2.9
+            Changed from naive to aware datetime.
     """
 
     __slots__ = ("user_id", "channel_id", "guild_id", "member", "timestamp")
 
     def __init__(self, data: TypingStartEvent) -> None:
         self.user_id: int = int(data["user_id"])
         self.channel_id: int = int(data["channel_id"])
         self.member: Optional[Member] = None
-        self.timestamp: datetime.datetime = datetime.datetime.utcfromtimestamp(data["timestamp"])
+        self.timestamp: datetime.datetime = datetime.datetime.fromtimestamp(
+            data["timestamp"], tz=datetime.timezone.utc
+        )
         try:
             self.guild_id: Optional[int] = int(data["guild_id"])
         except KeyError:
             self.guild_id: Optional[int] = None
 
 
 class RawGuildMemberRemoveEvent(_RawReprMixin):
```

### Comparing `disnake-2.8.2/disnake/reaction.py` & `disnake-2.9.0/disnake/reaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
         self,
         *,
         message: Message,
         data: ReactionPayload,
         emoji: Optional[Union[PartialEmoji, Emoji, str]] = None,
     ) -> None:
         self.message: Message = message
-        self.emoji: Union[PartialEmoji, Emoji, str] = emoji or message._state.get_reaction_emoji(
+        # _get_emoji_from_data won't return None
+        self.emoji: Union[PartialEmoji, Emoji, str] = emoji or message._state._get_emoji_from_data(  # type: ignore
             data["emoji"]
         )
         self.count: int = data.get("count", 1)
         self.me: bool = data["me"]
 
     # TODO: typeguard
     def is_custom_emoji(self) -> bool:
@@ -181,15 +182,15 @@
 
         Raises
         ------
         HTTPException
             Getting the users for the reaction failed.
 
         Yields
-        --------
+        ------
         Union[:class:`User`, :class:`Member`]
             The member (if retrievable) or the user that has reacted
             to this message. The case where it can be a :class:`Member` is
             in a guild message context. Sometimes it can be a :class:`User`
             if the member has left the guild.
         """
         if not isinstance(self.emoji, str):
```

### Comparing `disnake-2.8.2/disnake/role.py` & `disnake-2.9.0/disnake/role.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,40 +42,60 @@
 
     Attributes
     ----------
     bot_id: Optional[:class:`int`]
         The bot's user ID that manages this role.
     integration_id: Optional[:class:`int`]
         The integration ID that manages the role.
+
+        Roles with this ID matching the guild's ``guild_subscription`` integration
+        are considered subscription roles.
+    subscription_listing_id: Optional[:class:`int`]
+        The ID of this role's subscription listing, if applicable.
+
+        .. versionadded:: 2.9
     """
 
     __slots__ = (
         "bot_id",
         "integration_id",
+        "subscription_listing_id",
         "_premium_subscriber",
         "_guild_connections",
+        "_available_for_purchase",
     )
 
     def __init__(self, data: RoleTagPayload) -> None:
         self.bot_id: Optional[int] = _get_as_snowflake(data, "bot_id")
         self.integration_id: Optional[int] = _get_as_snowflake(data, "integration_id")
-        # NOTE: The API returns "null" for this if it's valid, which corresponds to None.
+        self.subscription_listing_id: Optional[int] = _get_as_snowflake(
+            data, "subscription_listing_id"
+        )
+
+        # NOTE: A value of null/None for this corresponds to True.
+        # If a field is missing, it corresponds to False.
         # This is different from other fields where "null" means "not there".
-        # So in this case, a value of None is the same as True.
-        # Which means we would need a different sentinel.
         self._premium_subscriber: Optional[Any] = data.get("premium_subscriber", MISSING)
         self._guild_connections: Optional[Any] = data.get("guild_connections", MISSING)
+        self._available_for_purchase: Optional[Any] = data.get("available_for_purchase", MISSING)
 
     def is_bot_managed(self) -> bool:
         """Whether the role is associated with a bot.
 
         :return type: :class:`bool`
         """
         return self.bot_id is not None
 
+    def is_integration(self) -> bool:
+        """Whether the role is managed by an integration.
+
+        :return type: :class:`bool`
+        """
+        return self.integration_id is not None
+
     def is_premium_subscriber(self) -> bool:
         """Whether the role is the premium subscriber, AKA "boost", role for the guild.
 
         :return type: :class:`bool`
         """
         return self._premium_subscriber is None
 
@@ -84,25 +104,38 @@
 
         .. versionadded:: 2.8
 
         :return type: :class:`bool`
         """
         return self._guild_connections is None
 
-    def is_integration(self) -> bool:
-        """Whether the role is managed by an integration.
+    def is_available_for_purchase(self) -> bool:
+        """Whether the role is a subscription role and available for purchase.
+
+        .. versionadded:: 2.9
 
         :return type: :class:`bool`
         """
-        return self.integration_id is not None
+        return self._available_for_purchase is None
+
+    def is_subscription(self) -> bool:
+        """Whether the role is associated with a role subscription.
+
+        .. versionadded:: 2.9
+
+        :return type: :class:`bool`
+        """
+        return self.subscription_listing_id is not None
 
     def __repr__(self) -> str:
         return (
             f"<RoleTags bot_id={self.bot_id} integration_id={self.integration_id} "
+            f"subscription_listing_id={self.subscription_listing_id} "
             f"premium_subscriber={self.is_premium_subscriber()} "
+            f"available_for_purchase={self.is_available_for_purchase()} "
             f"linked_role={self.is_linked_role()}>"
         )
 
 
 class Role(Hashable):
     """Represents a Discord role in a :class:`Guild`.
 
@@ -290,14 +323,32 @@
 
         .. versionadded:: 1.6
 
         :return type: :class:`bool`
         """
         return self.tags is not None and self.tags.is_integration()
 
+    def is_available_for_purchase(self) -> bool:
+        """Whether the role is a subscription role and available for purchase.
+
+        .. versionadded:: 2.9
+
+        :return type: :class:`bool`
+        """
+        return self.tags is not None and self.tags.is_available_for_purchase()
+
+    def is_subscription(self) -> bool:
+        """Whether the role is associated with a role subscription.
+
+        .. versionadded:: 2.9
+
+        :return type: :class:`bool`
+        """
+        return self.tags is not None and self.tags.is_subscription()
+
     def is_assignable(self) -> bool:
         """Whether the role is able to be assigned or removed by the bot.
 
         .. versionadded:: 2.0
 
         :return type: :class:`bool`
         """
```

### Comparing `disnake-2.8.2/disnake/shard.py` & `disnake-2.9.0/disnake/shard.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/stage_instance.py` & `disnake-2.9.0/disnake/stage_instance.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/state.py` & `disnake-2.9.0/disnake/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from .audit_logs import AuditLogEntry
 from .automod import AutoModActionExecution, AutoModRule
 from .channel import (
     DMChannel,
     ForumChannel,
     GroupChannel,
     PartialMessageable,
+    StageChannel,
     TextChannel,
     VoiceChannel,
     _guild_channel_factory,
 )
 from .emoji import Emoji
 from .enums import ApplicationCommandType, ChannelType, ComponentType, MessageType, Status, try_enum
 from .flags import ApplicationFlags, Intents, MemberCacheFlags
@@ -91,15 +92,15 @@
     from .client import Client
     from .gateway import DiscordWebSocket
     from .guild import GuildChannel, VocalGuildChannel
     from .http import HTTPClient
     from .types import gateway
     from .types.activity import Activity as ActivityPayload
     from .types.channel import DMChannel as DMChannelPayload
-    from .types.emoji import Emoji as EmojiPayload
+    from .types.emoji import Emoji as EmojiPayload, PartialEmoji as PartialEmojiPayload
     from .types.guild import Guild as GuildPayload, UnavailableGuild as UnavailableGuildPayload
     from .types.message import Message as MessagePayload
     from .types.sticker import GuildSticker as GuildStickerPayload
     from .types.user import User as UserPayload
     from .types.webhook import Webhook as WebhookPayload
     from .voice_client import VoiceProtocol
 
@@ -720,23 +721,22 @@
 
         self._ready_state: asyncio.Queue[Guild] = asyncio.Queue()
         self.clear(views=False, application_commands=False, modals=False)
         self.user = ClientUser(state=self, data=data["user"])
         # self._users is a list of Users, we're setting a ClientUser
         self._users[self.user.id] = self.user  # type: ignore
 
-        if self.application_id is None:
-            try:
-                application = data["application"]
-            except KeyError:
-                pass
-            else:
+        try:
+            application = data["application"]
+        except KeyError:
+            pass
+        else:
+            if self.application_id is None:
                 self.application_id = utils._get_as_snowflake(application, "id")
-                # flags will always be present here
-                self.application_flags = ApplicationFlags._from_value(application["flags"])
+            self.application_flags = ApplicationFlags._from_value(application["flags"])
 
         for guild_data in data["guilds"]:
             self._add_guild_from_data(guild_data)
 
         self.dispatch("connect")
         self.call_handlers("connect_internal")
         self._ready_task = asyncio.create_task(self._delay_ready())
@@ -756,15 +756,15 @@
         message = Message(channel=channel, data=data, state=self)  # type: ignore
         self.dispatch("message", message)
         if self._messages is not None:
             self._messages.append(message)
 
         if channel:
             # we ensure that the channel is a type that implements last_message_id
-            if channel.__class__ in (TextChannel, Thread, VoiceChannel):
+            if channel.__class__ in (TextChannel, Thread, VoiceChannel, StageChannel):
                 channel.last_message_id = message.id  # type: ignore
             # Essentially, messages *don't* count towards message_count, if:
             # - they're the thread starter message
             # - or, they're the initial message of a forum channel thread (which uses MessageType.default)
             # This mirrors the current client and API behavior.
             if channel.__class__ is Thread and not (
                 message.type is MessageType.thread_starter_message
@@ -881,14 +881,15 @@
 
     def parse_message_reaction_remove(self, data: gateway.MessageReactionRemoveEvent) -> None:
         emoji = data["emoji"]
         emoji_id = utils._get_as_snowflake(emoji, "id")
         emoji = PartialEmoji.with_state(
             self,
             id=emoji_id,
+            animated=emoji.get("animated", False),
             # may be `None` in gateway events if custom emoji data isn't available anymore
             # https://discord.com/developers/docs/resources/emoji#emoji-object-custom-emoji-examples
             name=emoji["name"],  # type: ignore
         )
         raw = RawReactionActionEvent(data, emoji, "REACTION_REMOVE")
         self.dispatch("raw_reaction_remove", raw)
 
@@ -908,14 +909,15 @@
         self, data: gateway.MessageReactionRemoveEmojiEvent
     ) -> None:
         emoji = data["emoji"]
         emoji_id = utils._get_as_snowflake(emoji, "id")
         emoji = PartialEmoji.with_state(
             self,
             id=emoji_id,
+            animated=emoji.get("animated", False),
             # may be `None` in gateway events if custom emoji data isn't available anymore
             # https://discord.com/developers/docs/resources/emoji#emoji-object-custom-emoji-examples
             name=emoji["name"],  # type: ignore
         )
         raw = RawReactionClearEmojiEvent(data, emoji)
         self.dispatch("raw_reaction_clear_emoji", raw)
 
@@ -1902,30 +1904,78 @@
             webhooks={},
         )
         self.dispatch("audit_log_entry_create", entry)
 
     def _get_reaction_user(
         self, channel: MessageableChannel, user_id: int
     ) -> Optional[Union[User, Member]]:
-        if isinstance(channel, (TextChannel, VoiceChannel, Thread)):
+        if isinstance(channel, (TextChannel, VoiceChannel, Thread, StageChannel)):
             return channel.guild.get_member(user_id)
         return self.get_user(user_id)
 
-    def get_reaction_emoji(self, data) -> Union[Emoji, PartialEmoji]:
-        emoji_id = utils._get_as_snowflake(data, "id")
+    # methods to handle all sorts of different emoji formats
+
+    def _get_emoji_from_data(
+        self, data: PartialEmojiPayload
+    ) -> Optional[Union[str, Emoji, PartialEmoji]]:
+        """Convert partial emoji data to proper emoji.
+        Returns unicode emojis as strings.
 
+        Primarily used to handle reaction emojis.
+        """
+        emoji_id = utils._get_as_snowflake(data, "id")
         if not emoji_id:
             return data["name"]
 
-        try:
-            return self._emojis[emoji_id]
-        except KeyError:
-            return PartialEmoji.with_state(
-                self, animated=data.get("animated", False), id=emoji_id, name=data["name"]
-            )
+        if (emoji := self._emojis.get(emoji_id)) is not None:
+            return emoji
+
+        return PartialEmoji.with_state(
+            self,
+            # This may be `None` when custom emoji data in reactions isn't available.
+            # Should generally be fine, since we have an id at this point.
+            name=data["name"],  # type: ignore
+            id=emoji_id,
+            animated=data.get("animated", False),
+        )
+
+    # deprecated
+    get_reaction_emoji = _get_emoji_from_data
+
+    def _get_emoji_from_fields(
+        self,
+        *,
+        name: Optional[str],
+        id: Optional[int],
+        animated: Optional[bool] = False,
+    ) -> Optional[Union[Emoji, PartialEmoji]]:
+        """Convert partial emoji fields to proper emoji, if possible.
+        If both `id` and `name` are nullish, returns `None`.
+
+        Unlike _get_emoji_from_data, this returns `PartialEmoji`s instead of strings
+        for unicode emojis, and falls back to "" for the emoji name.
+
+        Primarily used for structures with nonstandard top-level `emoji_name` and `emoji_id` fields,
+        like forum channels/tags or welcome screens.
+        """
+        if not (name or id):
+            return None
+
+        if id and (emoji := self._emojis.get(id)) is not None:
+            return emoji
+
+        return PartialEmoji.with_state(
+            self,
+            # Note: this does not render correctly if it's a custom emoji, there's just no name information here sometimes.
+            # This may change in a future API version, but for now we'll just have to accept it.
+            name=name or "",
+            # Coerce `0` to `None`, occasional API inconsistency
+            id=id or None,
+            animated=animated or False,
+        )
 
     def _upgrade_partial_emoji(self, emoji: PartialEmoji) -> Union[Emoji, PartialEmoji, str]:
         emoji_id = emoji.id
         if not emoji_id:
             return emoji.name
         try:
             return self._emojis[emoji_id]
@@ -2089,15 +2139,15 @@
             if not msg.guild:
                 continue
 
             new_guild = self._get_guild(msg.guild.id)
             if new_guild is not None and new_guild is not msg.guild:
                 channel_id = msg.channel.id
                 channel = new_guild._resolve_channel(channel_id) or Object(id=channel_id)
-                # channel will either be a TextChannel, VoiceChannel, Thread or Object
+                # channel will either be a TextChannel, VoiceChannel, Thread, StageChannel, or Object
                 msg._rebind_cached_references(new_guild, channel)  # type: ignore
 
         # these generally get deallocated once the voice reconnect times out
         # (it never succeeds after gateway reconnects)
         # but we rebind the channel reference just in case
         for vc in self._voice_clients.values():
             if not getattr(vc.channel, "guild", None):
@@ -2233,22 +2283,22 @@
         if not hasattr(self, "_ready_state"):
             self._ready_state = asyncio.Queue()
 
         self.user = user = ClientUser(state=self, data=data["user"])
         # self._users is a list of Users, we're setting a ClientUser
         self._users[user.id] = user  # type: ignore
 
-        if self.application_id is None:
-            try:
-                application = data["application"]
-            except KeyError:
-                pass
-            else:
+        try:
+            application = data["application"]
+        except KeyError:
+            pass
+        else:
+            if self.application_id is None:
                 self.application_id = utils._get_as_snowflake(application, "id")
-                self.application_flags = ApplicationFlags._from_value(application["flags"])
+            self.application_flags = ApplicationFlags._from_value(application["flags"])
 
         for guild_data in data["guilds"]:
             self._add_guild_from_data(guild_data)
 
         self.dispatch("connect")
         self.dispatch("shard_connect", data["__shard_id__"])  # type: ignore  # set in websocket receive
         self.call_handlers("connect_internal")
```

### Comparing `disnake-2.8.2/disnake/sticker.py` & `disnake-2.9.0/disnake/sticker.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,16 +388,16 @@
         The format for the sticker's image.
     available: :class:`bool`
         Whether this sticker is available for use.
     guild_id: :class:`int`
         The ID of the guild that this sticker is from.
     user: Optional[:class:`User`]
         The user that created this sticker. This can only be retrieved using
-        :meth:`Guild.fetch_sticker`/:meth:`Guild.fetch_stickers` and
-        having the :attr:`~Permissions.manage_emojis_and_stickers` permission.
+        :meth:`Guild.fetch_sticker`/:meth:`Guild.fetch_stickers` while
+        having the :attr:`~Permissions.manage_guild_expressions` permission.
     emoji: :class:`str`
         The name of a unicode emoji that represents this sticker.
     """
 
     __slots__ = ("available", "guild_id", "user", "emoji", "type", "_cs_guild")
 
     def _from_data(self, data: GuildStickerPayload) -> None:
@@ -429,14 +429,17 @@
         emoji: str = MISSING,
         reason: Optional[str] = None,
     ) -> GuildSticker:
         """|coro|
 
         Edits a :class:`GuildSticker` for the guild.
 
+        You must have :attr:`~Permissions.manage_guild_expressions` permission to
+        do this.
+
         Parameters
         ----------
         name: :class:`str`
             The sticker's new name. Must be at least 2 characters.
         description: Optional[:class:`str`]
             The sticker's new description. Can be ``None``.
         emoji: :class:`str`
@@ -480,15 +483,15 @@
         return GuildSticker(state=self._state, data=data)
 
     async def delete(self, *, reason: Optional[str] = None) -> None:
         """|coro|
 
         Deletes the custom :class:`Sticker` from the guild.
 
-        You must have :attr:`~Permissions.manage_emojis_and_stickers` permission to
+        You must have :attr:`~Permissions.manage_guild_expressions` permission to
         do this.
 
         Parameters
         ----------
         reason: Optional[:class:`str`]
             The reason for deleting this sticker. Shows up on the audit log.
```

### Comparing `disnake-2.8.2/disnake/team.py` & `disnake-2.9.0/disnake/team.py`

 * *Files 13% similar despite different names*

```diff
@@ -80,26 +80,39 @@
 
         .. describe:: hash(x)
 
             Return the team member's hash.
 
         .. describe:: str(x)
 
-            Returns the team member's name with discriminator.
+            Returns the team member's username (with discriminator, if not migrated to new system yet).
 
     .. versionadded:: 1.3
 
     Attributes
     ----------
     name: :class:`str`
         The team member's username.
     id: :class:`int`
         The team member's unique ID.
     discriminator: :class:`str`
-        The team member's discriminator. This is given when the username has conflicts.
+        The team member's discriminator.
+
+        .. note::
+            This is being phased out by Discord; the username system is moving away from ``username#discriminator``
+            to users having a globally unique username.
+            The value of a single zero (``"0"``) indicates that the user has been migrated to the new system.
+            See the `help article <https://dis.gd/app-usernames>`__ for details.
+
+    global_name: Optional[:class:`str`]
+        The team members's global display name, if set.
+        This takes precedence over :attr:`.name` when shown.
+
+        .. versionadded:: 2.9
+
     avatar: Optional[:class:`str`]
         The avatar hash the team member has. Could be None.
     bot: :class:`bool`
         Specifies if the user is a bot account.
     team: :class:`Team`
         The team that the member is from.
     membership_state: :class:`TeamMembershipState`
@@ -114,10 +127,10 @@
             TeamMembershipState, data["membership_state"]
         )
         self.permissions: List[str] = data["permissions"]
         super().__init__(state=state, data=data["user"])
 
     def __repr__(self) -> str:
         return (
-            f"<{self.__class__.__name__} id={self.id} name={self.name!r} "
-            f"discriminator={self.discriminator!r} membership_state={self.membership_state!r}>"
+            f"<{self.__class__.__name__} id={self.id} name={self.name!r} global_name={self.global_name!r}"
+            f" discriminator={self.discriminator!r} membership_state={self.membership_state!r}>"
         )
```

### Comparing `disnake-2.8.2/disnake/template.py` & `disnake-2.9.0/disnake/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,14 @@
             This template does not exist.
 
         Returns
         -------
         :class:`Template`
             The newly edited template.
         """
-
         data = await self._state.http.sync_template(self.source_guild.id, self.code)
         return Template(state=self._state, data=data)
 
     async def edit(
         self,
         *,
         name: str = MISSING,
```

### Comparing `disnake-2.8.2/disnake/threads.py` & `disnake-2.9.0/disnake/threads.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import asyncio
 import time
 from typing import TYPE_CHECKING, Callable, Dict, Iterable, List, Literal, Optional, Sequence, Union
 
-from .abc import Messageable
+from .abc import GuildChannel, Messageable
 from .enums import ChannelType, ThreadArchiveDuration, try_enum, try_enum_to_int
 from .errors import ClientException
 from .flags import ChannelFlags
 from .mixins import Hashable
 from .partial_emoji import PartialEmoji, _EmojiTag
 from .utils import MISSING, _get_as_snowflake, _unique, parse_time, snowflake_time
 
@@ -161,15 +161,15 @@
         "_type",
         "_state",
         "_members",
     )
 
     def __init__(self, *, guild: Guild, state: ConnectionState, data: ThreadPayload) -> None:
         self._state: ConnectionState = state
-        self.guild = guild
+        self.guild: Guild = guild
         self._members: Dict[int, ThreadMember] = {}
         self._from_data(data)
 
     async def _get_channel(self):
         return self
 
     def __repr__(self) -> str:
@@ -179,47 +179,49 @@
             f"flags={self.flags!r} applied_tags={self.applied_tags!r}>"
         )
 
     def __str__(self) -> str:
         return self.name
 
     def _from_data(self, data: ThreadPayload) -> None:
-        self.id = int(data["id"])
-        self.parent_id = int(data["parent_id"])
-        self.owner_id = _get_as_snowflake(data, "owner_id")
-        self.name = data["name"]
+        self.id: int = int(data["id"])
+        self.parent_id: int = int(data["parent_id"])
+        self.owner_id: Optional[int] = _get_as_snowflake(data, "owner_id")
+        self.name: str = data["name"]
         self._type: ThreadType = try_enum(ChannelType, data["type"])  # type: ignore
-        self.last_message_id = _get_as_snowflake(data, "last_message_id")
-        self.slowmode_delay = data.get("rate_limit_per_user", 0)
-        self.message_count = data.get("message_count") or 0
-        self.total_message_sent = data.get("total_message_sent") or 0
-        self.member_count = data.get("member_count")
+        self.last_message_id: Optional[int] = _get_as_snowflake(data, "last_message_id")
+        self.slowmode_delay: int = data.get("rate_limit_per_user", 0)
+        self.message_count: int = data.get("message_count") or 0
+        self.total_message_sent: int = data.get("total_message_sent") or 0
+        self.member_count: Optional[int] = data.get("member_count")
         self.last_pin_timestamp: Optional[datetime.datetime] = parse_time(
             data.get("last_pin_timestamp")
         )
         self._flags: int = data.get("flags", 0)
-        self._applied_tags = list(map(int, data.get("applied_tags", [])))
+        self._applied_tags: List[int] = list(map(int, data.get("applied_tags", [])))
         self._unroll_metadata(data["thread_metadata"])
 
         try:
             member = data["member"]
         except KeyError:
             self.me = None
         else:
             self.me = ThreadMember(self, member)
 
     def _unroll_metadata(self, data: ThreadMetadata) -> None:
-        self.archived = data["archived"]
-        self.auto_archive_duration = data["auto_archive_duration"]
-        self.archive_timestamp = parse_time(data["archive_timestamp"])
-        self.locked = data.get("locked", False)
-        self.invitable = data.get("invitable", True)
-        self.create_timestamp = parse_time(data.get("create_timestamp"))
+        self.archived: bool = data["archived"]
+        self.auto_archive_duration: ThreadArchiveDurationLiteral = data["auto_archive_duration"]
+        self.archive_timestamp: datetime.datetime = parse_time(data["archive_timestamp"])
+        self.locked: bool = data.get("locked", False)
+        self.invitable: bool = data.get("invitable", True)
+        self.create_timestamp: Optional[datetime.datetime] = parse_time(
+            data.get("create_timestamp")
+        )
 
-    def _update(self, data) -> None:
+    def _update(self, data: ThreadPayload) -> None:
         try:
             self.name = data["name"]
         except KeyError:
             pass
 
         self.slowmode_delay = data.get("rate_limit_per_user", 0)
         self._flags = data.get("flags", 0)
@@ -316,24 +318,22 @@
             The parent channel was not cached and returned ``None``.
 
         Returns
         -------
         Optional[:class:`int`]
             The parent channel's category ID.
         """
-
         parent = self.parent
         if parent is None:
             raise ClientException("Parent channel not found")
         return parent.category_id
 
     @property
     def created_at(self) -> datetime.datetime:
-        """
-        :class:`datetime.datetime`: Returns the thread's creation time in UTC.
+        """:class:`datetime.datetime`: Returns the thread's creation time in UTC.
 
         .. versionchanged:: 2.4
             If create_timestamp is provided by discord, that will be used instead of the time in the ID.
         """
         return self.create_timestamp or snowflake_time(self.id)
 
     @property
@@ -342,16 +342,15 @@
 
         .. versionadded:: 2.5
         """
         return ChannelFlags._from_value(self._flags)
 
     @property
     def jump_url(self) -> str:
-        """
-        A URL that can be used to jump to this thread.
+        """A URL that can be used to jump to this thread.
 
         .. versionadded:: 2.4
         """
         return f"https://discord.com/channels/{self.guild.id}/{self.id}"
 
     def is_private(self) -> bool:
         """Whether the thread is a private thread.
@@ -420,17 +419,23 @@
         *,
         ignore_timeout: bool = MISSING,
     ) -> Permissions:
         """Handles permission resolution for the :class:`~disnake.Member`
         or :class:`~disnake.Role`.
 
         Since threads do not have their own permissions, they inherit them
-        from the parent channel. This is a convenience method for
-        calling :meth:`~disnake.TextChannel.permissions_for` on the
-        parent channel.
+        from the parent channel.
+        However, the permission context is different compared to a normal channel,
+        so this method has different behavior than calling the parent's
+        :attr:`GuildChannel.permissions_for <.abc.GuildChannel.permissions_for>`
+        method directly.
+
+        .. versionchanged:: 2.9
+            Properly takes :attr:`Permissions.send_messages_in_threads`
+            into consideration.
 
         Parameters
         ----------
         obj: Union[:class:`~disnake.Member`, :class:`~disnake.Role`]
             The object to resolve permissions for. This could be either
             a member or a role. If it's a role then member overwrites
             are not computed.
@@ -454,19 +459,35 @@
             The parent channel was not cached and returned ``None``
 
         Returns
         -------
         :class:`~disnake.Permissions`
             The resolved permissions for the member or role.
         """
-
         parent = self.parent
         if parent is None:
             raise ClientException("Parent channel not found")
-        return parent.permissions_for(obj, ignore_timeout=ignore_timeout)
+        # n.b. GuildChannel is used here so implicit overrides are not applied based on send_messages
+        base = GuildChannel.permissions_for(parent, obj, ignore_timeout=ignore_timeout)
+
+        # if you can't send a message in a channel then you can't have certain
+        # permissions as well
+        if not base.send_messages_in_threads:
+            base.send_tts_messages = False
+            base.send_voice_messages = False
+            base.mention_everyone = False
+            base.embed_links = False
+            base.attach_files = False
+
+        # if you can't view a channel then you have no permissions there
+        if not base.view_channel:
+            denied = Permissions.all_channel()
+            base.value &= ~denied.value
+
+        return base
 
     async def delete_messages(self, messages: Iterable[Snowflake]) -> None:
         """|coro|
 
         Deletes a list of messages. This is similar to :meth:`Message.delete`
         except it bulk deletes multiple messages.
 
@@ -536,15 +557,14 @@
         You must have the :attr:`~Permissions.manage_messages` permission to
         delete messages even if they are your own (unless you are a user
         account). The :attr:`~Permissions.read_message_history` permission is
         also needed to retrieve message history.
 
         Examples
         --------
-
         Deleting bot's messages ::
 
             def is_me(m):
                 return m.author == client.user
 
             deleted = await thread.purge(limit=100, check=is_me)
             await thread.send(f'Deleted {len(deleted)} message(s)')
@@ -578,15 +598,14 @@
             Purging the messages failed.
 
         Returns
         -------
         List[:class:`.Message`]
             The list of messages that were deleted.
         """
-
         if check is MISSING:
             check = lambda m: True
 
         iterator = self.history(
             limit=limit, before=before, after=after, oldest_first=oldest_first, around=around
         )
         ret: List[Message] = []
@@ -862,15 +881,14 @@
             Retrieving the members failed.
 
         Returns
         -------
         List[:class:`ThreadMember`]
             All thread members in the thread.
         """
-
         members = await self._state.http.get_thread_members(self.id)
         return [ThreadMember(parent=self, data=data) for data in members]
 
     async def delete(self, *, reason: Optional[str] = None) -> None:
         """|coro|
 
         Deletes this thread.
@@ -919,15 +937,14 @@
         Raises
         ------
         Forbidden
             You do not have permission to add these tags.
         HTTPException
             Editing the thread failed.
         """
-
         if not tags:
             return
 
         new_tags: List[int] = self._applied_tags.copy()
         new_tags.extend(t.id for t in tags)
         new_tags = _unique(new_tags)
 
@@ -957,15 +974,14 @@
         Raises
         ------
         Forbidden
             You do not have permission to remove these tags.
         HTTPException
             Editing the thread failed.
         """
-
         if not tags:
             return
 
         to_remove = {t.id for t in tags}
         new_tags: List[int] = [tag_id for tag_id in self._applied_tags if tag_id not in to_remove]
 
         await self._state.http.edit_channel(self.id, applied_tags=new_tags, reason=reason)
@@ -984,15 +1000,14 @@
             The message ID to create a partial message for.
 
         Returns
         -------
         :class:`PartialMessage`
             The partial message.
         """
-
         from .message import PartialMessage
 
         return PartialMessage(channel=self, id=message_id)
 
     def _add_member(self, member: ThreadMember) -> None:
         self._members[member.id] = member
 
@@ -1051,17 +1066,17 @@
         return (
             f"<ThreadMember id={self.id} thread_id={self.thread_id} joined_at={self.joined_at!r}>"
         )
 
     def _from_data(self, data: ThreadMemberPayload) -> None:
         try:
             self.id = int(data["user_id"])
-        except KeyError:
+        except KeyError as err:
             if (self_id := self._state.self_id) is None:
-                raise AssertionError("self_id is None when updating our own ThreadMember.")
+                raise AssertionError("self_id is None when updating our own ThreadMember.") from err
             self.id = self_id
 
         try:
             self.thread_id = int(data["id"])
         except KeyError:
             self.thread_id = self.parent.id
 
@@ -1071,16 +1086,15 @@
     @property
     def thread(self) -> Thread:
         """:class:`Thread`: The thread this member belongs to."""
         return self.parent
 
 
 class ForumTag(Hashable):
-    """
-    Represents a tag for threads in forum channels.
+    """Represents a tag for threads in forum channels.
 
     .. container:: operations
 
         .. describe:: x == y
 
             Checks if two tags are equal.
 
@@ -1097,15 +1111,14 @@
             Returns the tag's name.
 
     .. versionadded:: 2.6
 
 
     Examples
     --------
-
     Creating a new tag:
 
     .. code-block:: python3
 
         tags = forum.available_tags
         tags.append(ForumTag(name="cool new tag", moderated=True))
         await forum.edit(available_tags=tags)
@@ -1182,17 +1195,18 @@
         if self.id:
             data["id"] = self.id
 
         return data
 
     @classmethod
     def _from_data(cls, *, data: ForumTagPayload, state: ConnectionState) -> Self:
-        emoji_id = _get_as_snowflake(data, "emoji_id") or None
-        emoji_name = data.get("emoji_name")
-        emoji = PartialEmoji._emoji_from_name_id(emoji_name, emoji_id, state=state)
+        emoji = state._get_emoji_from_fields(
+            name=data.get("emoji_name"),
+            id=_get_as_snowflake(data, "emoji_id"),
+        )
 
         self = cls(
             name=data["name"],
             emoji=emoji,
             moderated=data["moderated"],
         )
         self.id = int(data["id"])
@@ -1202,16 +1216,15 @@
     def with_changes(
         self,
         *,
         name: str = MISSING,
         emoji: Optional[Union[str, Emoji, PartialEmoji]] = MISSING,
         moderated: bool = MISSING,
     ) -> Self:
-        """
-        Returns a new instance with the given changes applied,
+        """Returns a new instance with the given changes applied,
         for easy use with :func:`ForumChannel.edit`.
         All other fields will be kept intact.
 
         Returns
         -------
         :class:`ForumTag`
             The new tag instance.
```

### Comparing `disnake-2.8.2/disnake/types/activity.py` & `disnake-2.9.0/disnake/types/activity.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/appinfo.py` & `disnake-2.9.0/disnake/types/appinfo.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,10 +46,11 @@
 
 class PartialAppInfo(BaseAppInfo, total=False):
     rpc_origins: List[str]
     cover_image: str
     flags: int
 
 
+# see https://discord.com/developers/docs/topics/gateway-events#ready-ready-event-fields
 class PartialGatewayAppInfo(TypedDict):
     id: Snowflake
     flags: int
```

### Comparing `disnake-2.8.2/disnake/types/audit_log.py` & `disnake-2.9.0/disnake/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/automod.py` & `disnake-2.9.0/disnake/types/automod.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 AutoModTriggerType = Literal[1, 2, 3, 4, 5]
 AutoModEventType = Literal[1]
 AutoModActionType = Literal[1, 2]
 AutoModPresetType = Literal[1, 2, 3]
 
 
 class AutoModBlockMessageActionMetadata(TypedDict):
-    ...
+    custom_message: NotRequired[str]
 
 
 class AutoModSendAlertActionMetadata(TypedDict):
     channel_id: Snowflake
 
 
 class AutoModTimeoutActionMetadata(TypedDict):
@@ -40,14 +40,15 @@
 
 class AutoModTriggerMetadata(TypedDict, total=False):
     keyword_filter: List[str]
     regex_patterns: List[str]
     presets: List[AutoModPresetType]
     allow_list: List[str]
     mention_total_limit: int
+    mention_raid_protection_enabled: bool
 
 
 class AutoModRule(TypedDict):
     id: Snowflake
     guild_id: Snowflake
     name: str
     creator_id: Snowflake
```

### Comparing `disnake-2.8.2/disnake/types/channel.py` & `disnake-2.9.0/disnake/types/channel.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/components.py` & `disnake-2.9.0/disnake/types/components.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/embed.py` & `disnake-2.9.0/disnake/types/embed.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/gateway.py` & `disnake-2.9.0/disnake/types/gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,14 +240,15 @@
     d: VoiceResumeData
 
 
 #####
 # Gateway events
 #####
 
+
 # https://discord.com/developers/docs/topics/gateway-events#ready
 class ReadyEvent(TypedDict):
     v: int
     user: User
     guilds: List[UnavailableGuild]
     session_id: str
     resume_gateway_url: str
```

### Comparing `disnake-2.8.2/disnake/types/guild.py` & `disnake-2.9.0/disnake/types/guild.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,38 +37,40 @@
 GuildFeature = Literal[
     "ANIMATED_BANNER",
     "ANIMATED_ICON",
     "AUTO_MODERATION",
     "BANNER",
     "COMMUNITY",
     "CREATOR_MONETIZABLE",  # not yet documented/finalised
+    "CREATOR_MONETIZABLE_PROVISIONAL",
+    "CREATOR_STORE_PAGE",
     "DEVELOPER_SUPPORT_SERVER",
     "DISCOVERABLE",
     "ENABLED_DISCOVERABLE_BEFORE",
     "FEATURABLE",
     "GUILD_HOME_TEST",  # not yet documented/finalised
     "HAS_DIRECTORY_ENTRY",
     "HUB",
     "INVITE_SPLASH",
     "INVITES_DISABLED",
     "LINKED_TO_HUB",
     "MEMBER_PROFILES",  # not sure what this does, if anything
     "MEMBER_VERIFICATION_GATE_ENABLED",
-    "MONETIZATION_ENABLED",
     "MORE_EMOJI",
     "MORE_STICKERS",
     "NEWS",
     "NEW_THREAD_PERMISSIONS",  # deprecated
     "PARTNERED",
     "PREVIEW_ENABLED",
     "PRIVATE_THREADS",  # deprecated
+    "RAID_ALERTS_DISABLED",
     "RELAY_ENABLED",
     "ROLE_ICONS",
-    "ROLE_SUBSCRIPTIONS_AVAILABLE_FOR_PURCHASE",  # not yet documented/finalised
-    "ROLE_SUBSCRIPTIONS_ENABLED",  # not yet documented/finalised
+    "ROLE_SUBSCRIPTIONS_AVAILABLE_FOR_PURCHASE",
+    "ROLE_SUBSCRIPTIONS_ENABLED",
     "SEVEN_DAY_THREAD_ARCHIVE",  # deprecated
     "TEXT_IN_VOICE_ENABLED",  # deprecated
     "THREADS_ENABLED",  # deprecated
     "THREE_DAY_THREAD_ARCHIVE",  # deprecated
     "TICKETED_EVENTS_ENABLED",  # deprecated
     "VANITY_URL",
     "VERIFIED",
@@ -117,19 +119,21 @@
     vanity_url_code: Optional[str]
     banner: Optional[str]
     premium_tier: PremiumTier
     premium_subscription_count: NotRequired[int]
     preferred_locale: str
     public_updates_channel_id: Optional[Snowflake]
     max_video_channel_users: NotRequired[int]
+    max_stage_video_channel_users: NotRequired[int]
     approximate_member_count: NotRequired[int]
     approximate_presence_count: NotRequired[int]
     nsfw_level: NSFWLevel
     stickers: NotRequired[List[GuildSticker]]
     premium_progress_bar_enabled: bool
+    safety_alerts_channel_id: Optional[Snowflake]
 
     # specific to GUILD_CREATE event
     joined_at: NotRequired[Optional[str]]
     large: NotRequired[bool]
     member_count: NotRequired[int]
     voice_states: NotRequired[List[GuildVoiceState]]
     members: NotRequired[List[Member]]
```

### Comparing `disnake-2.8.2/disnake/types/guild_scheduled_event.py` & `disnake-2.9.0/disnake/types/guild_scheduled_event.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/integration.py` & `disnake-2.9.0/disnake/types/integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name: str
     type: IntegrationType
     account: IntegrationAccount
     # undocumented, only shown in example - used for audit logs
     application_id: NotRequired[Snowflake]
 
 
-IntegrationType = Literal["twitch", "youtube", "discord"]
+IntegrationType = Literal["twitch", "youtube", "discord", "guild_subscription"]
 
 
 class BaseIntegration(PartialIntegration):
     enabled: bool
     syncing: bool
     synced_at: str
     user: User
```

### Comparing `disnake-2.8.2/disnake/types/interactions.py` & `disnake-2.9.0/disnake/types/interactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,15 @@
     MessageComponentInteractionMentionableSelectData,
     MessageComponentInteractionChannelSelectData,
 ]
 
 
 ### Modal interaction components
 
+
 # TODO: add other select types
 class ModalInteractionStringSelectData(_BaseComponentInteractionData):
     type: Literal[3]
     values: List[str]
 
 
 class ModalInteractionTextInputData(_BaseComponentInteractionData):
@@ -301,15 +302,15 @@
 class InteractionApplicationCommandCallbackData(TypedDict, total=False):
     tts: bool
     content: str
     embeds: List[Embed]
     allowed_mentions: AllowedMentions
     flags: int
     components: List[Component]
-    # TODO: missing attachment field
+    attachments: List[Attachment]
 
 
 class InteractionAutocompleteCallbackData(TypedDict):
     choices: List[ApplicationCommandOptionChoice]
 
 
 InteractionResponseType = Literal[1, 4, 5, 6, 7]
```

### Comparing `disnake-2.8.2/disnake/types/invite.py` & `disnake-2.9.0/disnake/types/invite.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/member.py` & `disnake-2.9.0/disnake/types/member.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/message.py` & `disnake-2.9.0/disnake/types/message.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     content_type: NotRequired[str]
     size: int
     url: str
     proxy_url: str
     height: NotRequired[Optional[int]]
     width: NotRequired[Optional[int]]
     ephemeral: NotRequired[bool]
+    duration_secs: NotRequired[float]
+    waveform: NotRequired[str]
 
 
 MessageActivityType = Literal[1, 2, 3, 5]
 
 
 class MessageActivity(TypedDict):
     type: MessageActivityType
@@ -63,16 +65,23 @@
 class MessageReference(TypedDict, total=False):
     message_id: Snowflake
     channel_id: Snowflake
     guild_id: Snowflake
     fail_if_not_exists: bool
 
 
+class RoleSubscriptionData(TypedDict):
+    role_subscription_listing_id: Snowflake
+    tier_name: str
+    total_months_subscribed: int
+    is_renewal: bool
+
+
 # fmt: off
-MessageType = Literal[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 15, 18, 19, 20, 21, 22, 23, 24, 26, 27, 28, 29, 30, 31, 32]
+MessageType = Literal[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 15, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32]
 # fmt: on
 
 
 class Message(TypedDict):
     id: Snowflake
     channel_id: Snowflake
     author: User
@@ -99,14 +108,15 @@
     flags: NotRequired[int]
     referenced_message: NotRequired[Optional[Message]]
     interaction: NotRequired[InteractionMessageReference]
     thread: NotRequired[Thread]
     components: NotRequired[List[Component]]
     sticker_items: NotRequired[List[StickerItem]]
     position: NotRequired[int]
+    role_subscription_data: NotRequired[RoleSubscriptionData]
 
     # specific to MESSAGE_CREATE/MESSAGE_UPDATE events
     guild_id: NotRequired[Snowflake]
     member: NotRequired[Member]
 
 
 AllowedMentionType = Literal["roles", "users", "everyone"]
```

### Comparing `disnake-2.8.2/disnake/types/role.py` & `disnake-2.9.0/disnake/types/role.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 
 class RoleTags(TypedDict, total=False):
     bot_id: Snowflake
     integration_id: Snowflake
     premium_subscriber: None
     guild_connections: None
+    subscription_listing_id: Snowflake
+    available_for_purchase: None
 
 
 class CreateRole(TypedDict, total=False):
     name: str
     permissions: str
     color: int
     hoist: bool
```

### Comparing `disnake-2.8.2/disnake/types/sticker.py` & `disnake-2.9.0/disnake/types/sticker.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/template.py` & `disnake-2.9.0/disnake/types/template.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/threads.py` & `disnake-2.9.0/disnake/types/threads.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/voice.py` & `disnake-2.9.0/disnake/types/voice.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/webhook.py` & `disnake-2.9.0/disnake/types/webhook.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/types/widget.py` & `disnake-2.9.0/disnake/types/widget.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ui/action_row.py` & `disnake-2.9.0/disnake/ui/action_row.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ui/button.py` & `disnake-2.9.0/disnake/ui/button.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,14 @@
     row: Optional[:class:`int`]
         The relative row this button belongs to. A Discord component can only have 5
         rows. By default, items are arranged automatically into those 5 rows. If you'd
         like to control the relative positioning of the row then passing an index is advised.
         For example, row=1 will show up before row=2. Defaults to ``None``, which is automatic
         ordering. The row number must be between 0 and 4 (i.e. zero indexed).
     """
-
     if (origin := get_origin(cls)) is not None:
         cls = origin
 
     if not isinstance(cls, type) or not issubclass(cls, Button):
         raise TypeError(f"cls argument must be a subclass of Button, got {cls!r}")
 
     def decorator(func: ItemCallbackType[B_co]) -> DecoratedItem[B_co]:
```

### Comparing `disnake-2.8.2/disnake/ui/item.py` & `disnake-2.9.0/disnake/ui/item.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ui/modal.py` & `disnake-2.9.0/disnake/ui/modal.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ui/select/__init__.py` & `disnake-2.9.0/disnake/ui/select/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # SPDX-License-Identifier: MIT
 
-"""
-disnake.ui.select
+"""disnake.ui.select
 ~~~~~~~~~~~~~~~~~~
 
 Select Menu UI Kit Types
 
 :copyright: (c) 2021-present Disnake Development
 :license: MIT, see LICENSE for more details.
```

### Comparing `disnake-2.8.2/disnake/ui/select/base.py` & `disnake-2.9.0/disnake/ui/select/base.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ui/select/channel.py` & `disnake-2.9.0/disnake/ui/select/channel.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ui/select/mentionable.py` & `disnake-2.9.0/disnake/ui/select/mentionable.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ui/select/role.py` & `disnake-2.9.0/disnake/ui/select/role.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ui/select/string.py` & `disnake-2.9.0/disnake/ui/select/string.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ui/select/user.py` & `disnake-2.9.0/disnake/ui/select/user.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ui/text_input.py` & `disnake-2.9.0/disnake/ui/text_input.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/disnake/ui/view.py` & `disnake-2.9.0/disnake/ui/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,15 +510,15 @@
     @property
     def persistent_views(self) -> Sequence[View]:
         views = {view.id: view for view, _ in self._views.values() if view.is_persistent()}
         return list(views.values())
 
     def __verify_integrity(self) -> None:
         to_remove: List[Tuple[int, Optional[int], str]] = []
-        for (k, (view, _)) in self._views.items():
+        for k, (view, _) in self._views.items():
             if view.is_finished():
                 to_remove.append(k)
 
         for k in to_remove:
             del self._views[k]
 
     def add_view(self, view: View, message_id: Optional[int] = None) -> None:
```

### Comparing `disnake-2.8.2/disnake/user.py` & `disnake-2.9.0/disnake/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import disnake.abc
 
 from .asset import Asset
 from .colour import Colour
-from .enums import DefaultAvatar, Locale, try_enum
+from .enums import Locale, try_enum
 from .flags import PublicUserFlags
 from .utils import MISSING, _assetbytes_to_base64_data, snowflake_time
 
 if TYPE_CHECKING:
     from datetime import datetime
 
     from typing_extensions import Self
@@ -38,27 +38,29 @@
 
 
 class BaseUser(_UserTag):
     __slots__ = (
         "name",
         "id",
         "discriminator",
+        "global_name",
         "_avatar",
         "_banner",
         "_accent_colour",
         "bot",
         "system",
         "_public_flags",
         "_state",
     )
 
     if TYPE_CHECKING:
         name: str
         id: int
         discriminator: str
+        global_name: Optional[str]
         bot: bool
         system: bool
         _state: ConnectionState
         _avatar: Optional[str]
         _banner: Optional[str]
         _accent_colour: Optional[str]
         _public_flags: int
@@ -67,48 +69,54 @@
         self, *, state: ConnectionState, data: Union[UserPayload, PartialUserPayload]
     ) -> None:
         self._state = state
         self._update(data)
 
     def __repr__(self) -> str:
         return (
-            f"<BaseUser id={self.id} name={self.name!r} discriminator={self.discriminator!r}"
-            f" bot={self.bot} system={self.system}>"
+            f"<BaseUser id={self.id} name={self.name!r} global_name={self.global_name!r}"
+            f" discriminator={self.discriminator!r} bot={self.bot} system={self.system}>"
         )
 
     def __str__(self) -> str:
-        return f"{self.name}#{self.discriminator}"
+        discriminator = self.discriminator
+        if discriminator == "0":
+            return self.name
+        # legacy behavior
+        return f"{self.name}#{discriminator}"
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, _UserTag) and other.id == self.id
 
     def __ne__(self, other: Any) -> bool:
         return not self.__eq__(other)
 
     def __hash__(self) -> int:
         return self.id >> 22
 
     def _update(self, data: Union[UserPayload, PartialUserPayload]) -> None:
         self.name = data["username"]
         self.id = int(data["id"])
         self.discriminator = data["discriminator"]
+        self.global_name = data.get("global_name")
         self._avatar = data["avatar"]
         self._banner = data.get("banner", None)
         self._accent_colour = data.get("accent_color", None)
         self._public_flags = data.get("public_flags", 0)
         self.bot = data.get("bot", False)
         self.system = data.get("system", False)
 
     @classmethod
     def _copy(cls, user: BaseUser) -> Self:
         self = cls.__new__(cls)  # bypass __init__
 
         self.name = user.name
         self.id = user.id
         self.discriminator = user.discriminator
+        self.global_name = user.global_name
         self._avatar = user._avatar
         self._banner = user._banner
         self._accent_colour = user._accent_colour
         self.bot = user.bot
         self._state = user._state
         self._public_flags = user._public_flags
 
@@ -116,14 +124,15 @@
 
     def _to_minimal_user_json(self) -> UserPayload:
         return {
             "username": self.name,
             "id": self.id,
             "avatar": self._avatar,
             "discriminator": self.discriminator,
+            "global_name": self.global_name,
             "bot": self.bot,
             "public_flags": self._public_flags,
         }
 
     @property
     def public_flags(self) -> PublicUserFlags:
         """:class:`PublicUserFlags`: The publicly available flags the user has."""
@@ -138,16 +147,25 @@
         """
         if self._avatar is not None:
             return Asset._from_avatar(self._state, self.id, self._avatar)
         return None
 
     @property
     def default_avatar(self) -> Asset:
-        """:class:`Asset`: Returns the default avatar for a given user. This is calculated by the user's discriminator."""
-        return Asset._from_default_avatar(self._state, int(self.discriminator) % len(DefaultAvatar))
+        """:class:`Asset`: Returns the default avatar for a given user.
+
+        .. versionchanged:: 2.9
+            Added handling for users migrated to the new username system without discriminators.
+        """
+        if self.discriminator == "0":
+            index = (self.id >> 22) % 6
+        else:
+            # legacy behavior
+            index = int(self.discriminator) % 5
+        return Asset._from_default_avatar(self._state, index)
 
     @property
     def display_avatar(self) -> Asset:
         """:class:`Asset`: Returns the user's display avatar.
 
         For regular users this is just their default avatar or uploaded avatar.
 
@@ -229,34 +247,35 @@
         """
         return snowflake_time(self.id)
 
     @property
     def display_name(self) -> str:
         """:class:`str`: Returns the user's display name.
 
-        For regular users this is just their username, but
-        if they have a guild specific nickname then that
-        is returned instead.
+        This is their :attr:`global name <.global_name>` if set,
+        or their :attr:`username <.name>` otherwise.
+
+        .. versionchanged:: 2.9
+            Added :attr:`.global_name`.
         """
-        return self.name
+        return self.global_name or self.name
 
     def mentioned_in(self, message: Message) -> bool:
         """Checks if the user is mentioned in the specified message.
 
         Parameters
         ----------
         message: :class:`Message`
             The message to check.
 
         Returns
         -------
         :class:`bool`
             Indicates if the user is mentioned in the message.
         """
-
         if message.mention_everyone:
             return True
 
         return any(user.id == self.id for user in message.mentions)
 
 
 class ClientUser(BaseUser):
@@ -274,24 +293,31 @@
 
         .. describe:: hash(x)
 
             Return the user's hash.
 
         .. describe:: str(x)
 
-            Returns the user's name with discriminator.
+            Returns the user's username (with discriminator, if not migrated to new system yet).
 
     Attributes
     ----------
     name: :class:`str`
         The user's username.
     id: :class:`int`
         The user's unique ID.
     discriminator: :class:`str`
-        The user's discriminator. This is given when the username has conflicts.
+        The user's discriminator.
+
+    global_name: Optional[:class:`str`]
+        The user's global display name, if set.
+        This takes precedence over :attr:`.name` when shown.
+
+        .. versionadded:: 2.9
+
     bot: :class:`bool`
         Specifies if the user is a bot account.
     system: :class:`bool`
         Specifies if the user is a system user (i.e. represents Discord officially).
 
         .. versionadded:: 1.3
 
@@ -316,15 +342,15 @@
         _flags: int
 
     def __init__(self, *, state: ConnectionState, data: UserPayload) -> None:
         super().__init__(state=state, data=data)
 
     def __repr__(self) -> str:
         return (
-            f"<ClientUser id={self.id} name={self.name!r} discriminator={self.discriminator!r}"
+            f"<ClientUser id={self.id} name={self.name!r} global_name={self.global_name!r} discriminator={self.discriminator!r}"
             f" bot={self.bot} verified={self.verified} mfa_enabled={self.mfa_enabled}>"
         )
 
     def _update(self, data: UserPayload) -> None:
         super()._update(data)
         self.verified = data.get("verified", False)
         locale = data.get("locale")
@@ -405,34 +431,50 @@
 
         .. describe:: hash(x)
 
             Return the user's hash.
 
         .. describe:: str(x)
 
-            Returns the user's name with discriminator.
+            Returns the user's username (with discriminator, if not migrated to new system yet).
 
     Attributes
     ----------
     name: :class:`str`
         The user's username.
     id: :class:`int`
         The user's unique ID.
     discriminator: :class:`str`
-        The user's discriminator. This is given when the username has conflicts.
+        The user's discriminator.
+
+        .. note::
+            This is being phased out by Discord; the username system is moving away from ``username#discriminator``
+            to users having a globally unique username.
+            The value of a single zero (``"0"``) indicates that the user has been migrated to the new system.
+            See the `help article <https://dis.gd/app-usernames>`__ for details.
+
+    global_name: Optional[:class:`str`]
+        The user's global display name, if set.
+        This takes precedence over :attr:`.name` when shown.
+
+        .. versionadded:: 2.9
+
     bot: :class:`bool`
         Specifies if the user is a bot account.
     system: :class:`bool`
         Specifies if the user is a system user (i.e. represents Discord officially).
     """
 
     __slots__ = ("__weakref__",)
 
     def __repr__(self) -> str:
-        return f"<User id={self.id} name={self.name!r} discriminator={self.discriminator!r} bot={self.bot}>"
+        return (
+            f"<User id={self.id} name={self.name!r} global_name={self.global_name!r}"
+            f" discriminator={self.discriminator!r} bot={self.bot}>"
+        )
 
     async def _get_channel(self) -> DMChannel:
         ch = await self.create_dm()
         return ch
 
     @property
     def dm_channel(self) -> Optional[DMChannel]:
```

### Comparing `disnake-2.8.2/disnake/utils.py` & `disnake-2.9.0/disnake/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 import os
 import pkgutil
 import re
 import sys
 import unicodedata
 import warnings
-from base64 import b64encode, urlsafe_b64decode as b64decode
+from base64 import b64encode
 from bisect import bisect_left
 from inspect import getdoc as _getdoc, isawaitable as _isawaitable, signature as _signature
 from operator import attrgetter
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterator,
@@ -54,15 +54,14 @@
     HAS_ORJSON = False
 else:
     HAS_ORJSON = True
 
 
 __all__ = (
     "oauth_url",
-    "parse_token",
     "snowflake_time",
     "time_snowflake",
     "find",
     "get",
     "sleep_until",
     "utcnow",
     "remove_markdown",
@@ -326,44 +325,16 @@
     if redirect_uri is not MISSING:
         url += "&response_type=code&" + urlencode({"redirect_uri": redirect_uri})
     if disable_guild_select:
         url += "&disable_guild_select=true"
     return url
 
 
-def parse_token(token: str) -> Tuple[int, datetime.datetime, bytes]:
-    """Parse a token into its parts
-
-    Returns
-
-    Parameters
-    ----------
-    token: :class:`str`
-        The bot token
-
-    Returns
-    -------
-    Tuple[:class:`int`, :class:`datetime.datetime`, :class:`bytes`]
-        The bot's ID, the time when the token was generated and the hmac.
-    """
-    parts = token.split(".")
-
-    user_id = int(b64decode(parts[0]))
-
-    timestamp = int.from_bytes(b64decode(parts[1] + "=="), "big")
-    created_at = datetime.datetime.fromtimestamp(timestamp, datetime.timezone.utc)
-
-    hmac = b64decode(parts[2] + "==")
-
-    return user_id, created_at, hmac
-
-
 def snowflake_time(id: int) -> datetime.datetime:
-    """
-    Parameters
+    """Parameters
     ----------
     id: :class:`int`
         The snowflake ID.
 
     Returns
     -------
     :class:`datetime.datetime`
@@ -414,24 +385,22 @@
     Parameters
     ----------
     predicate
         A function that returns a boolean-like result.
     seq: :class:`collections.abc.Iterable`
         The iterable to search through.
     """
-
     for element in seq:
         if predicate(element):
             return element
     return None
 
 
 def get(iterable: Iterable[T], **attrs: Any) -> Optional[T]:
-    """
-    A helper that returns the first element in the iterable that meets
+    """A helper that returns the first element in the iterable that meets
     all the traits passed in ``attrs``. This is an alternative for
     :func:`~disnake.utils.find`.
 
     When multiple attributes are specified, they are checked using
     logical AND, not logical OR. Meaning they have to meet every
     attribute passed in and not one of them.
 
@@ -439,15 +408,14 @@
     pass in ``x__y`` as the keyword argument.
 
     If nothing is found that matches the attributes passed, then
     ``None`` is returned.
 
     Examples
     --------
-
     Basic usage:
 
     .. code-block:: python3
 
         member = disnake.utils.get(message.guild.members, name='Foo')
 
     Multiple attribute matching:
@@ -465,15 +433,14 @@
     Parameters
     ----------
     iterable
         An iterable to search through.
     **attrs
         Keyword arguments that denote attributes to search with.
     """
-
     # global -> local
     _all = all
     attrget = attrgetter
 
     # Special case the single element call
     if len(attrs) == 1:
         k, v = attrs.popitem()
@@ -612,15 +579,15 @@
 
 
 async def sane_wait_for(futures: Iterable[Awaitable[T]], *, timeout: float) -> Set[asyncio.Task[T]]:
     ensured = [asyncio.ensure_future(fut) for fut in futures]
     done, pending = await asyncio.wait(ensured, timeout=timeout, return_when=asyncio.ALL_COMPLETED)
 
     if len(pending) != 0:
-        raise asyncio.TimeoutError()
+        raise asyncio.TimeoutError
 
     return done
 
 
 def get_slots(cls: Type[Any]) -> Iterator[str]:
     for mro in reversed(cls.__mro__):
         slots = getattr(mro, "__slots__", [])
@@ -739,16 +706,15 @@
 ) -> Tuple[str, Dict[str, str]]:
     ...
 
 
 def resolve_invite(
     invite: Union[Invite, str], *, with_params: bool = False
 ) -> Union[str, Tuple[str, Dict[str, str]]]:
-    """
-    Resolves an invite from a :class:`~disnake.Invite`, URL or code.
+    """Resolves an invite from a :class:`~disnake.Invite`, URL or code.
 
     Parameters
     ----------
     invite: Union[:class:`~disnake.Invite`, :class:`str`]
         The invite to resolve.
     with_params: :class:`bool`
         Whether to also return the query parameters of the invite, if it's a url.
@@ -776,16 +742,15 @@
                 params = {k: v[0] for k, v in parse_qs(p or "").items()}
         else:
             code = invite
     return (code, params) if with_params else code
 
 
 def resolve_template(code: Union[Template, str]) -> str:
-    """
-    Resolves a template code from a :class:`~disnake.Template`, URL or code.
+    """Resolves a template code from a :class:`~disnake.Template`, URL or code.
 
     .. versionadded:: 1.4
 
     Parameters
     ----------
     code: Union[:class:`~disnake.Template`, :class:`str`]
         The code.
@@ -853,16 +818,15 @@
     regex = _MARKDOWN_STOCK_REGEX
     if ignore_links:
         regex = f"(?:{_URL_REGEX}|{regex})"
     return re.sub(regex, replacement, text, 0, re.MULTILINE)
 
 
 def escape_markdown(text: str, *, as_needed: bool = False, ignore_links: bool = True) -> str:
-    """
-    A helper function that escapes Discord's markdown.
+    """A helper function that escapes Discord's markdown.
 
     Parameters
     ----------
     text: :class:`str`
         The text to escape markdown from.
     as_needed: :class:`bool`
         Whether to escape the markdown characters as needed. This
@@ -877,15 +841,14 @@
         Defaults to ``True``.
 
     Returns
     -------
     :class:`str`
         The text with the markdown special characters escaped with a slash.
     """
-
     if not as_needed:
 
         def replacement(match):
             groupdict = match.groupdict()
             is_url = groupdict.get("url")
             if is_url:
                 return is_url
@@ -1167,15 +1130,15 @@
         tp = tp.__forward_arg__
         # ForwardRefs always evaluate their internals
         implicit_str = True
 
     if implicit_str and isinstance(tp, str):
         if tp in cache:
             return cache[tp]
-        evaluated = eval(  # noqa: S307  # this is how annotations are supposed to be evaled
+        evaluated = eval(  # noqa: PGH001 # this is how annotations are supposed to be unstringifed
             tp, globals, locals
         )
         cache[tp] = evaluated
         return evaluate_annotation(evaluated, globals, locals, cache)
 
     if hasattr(tp, "__args__"):
         implicit_str = True
@@ -1291,15 +1254,15 @@
 
     Parameters
     ----------
     path: :class:`str`
         The path to search for modules
 
     Yields
-    -------
+    ------
     :class:`str`
         The name of the found module. (usable in load_extension)
     """
     relpath = os.path.relpath(path)  # relative and normalized
     if ".." in relpath:
         raise ValueError("Modules outside the cwd require a package to be specified")
 
@@ -1319,16 +1282,15 @@
         if ispkg:
             yield from search_directory(os.path.join(path, name))
         else:
             yield prefix + name
 
 
 def as_valid_locale(locale: str) -> Optional[str]:
-    """
-    Converts the provided locale name to a name that is valid for use with the API,
+    """Converts the provided locale name to a name that is valid for use with the API,
     for example by returning ``en-US`` for ``en_US``.
     Returns ``None`` for invalid names.
 
     .. versionadded:: 2.5
 
     Parameters
     ----------
```

### Comparing `disnake-2.8.2/disnake/voice_client.py` & `disnake-2.9.0/disnake/voice_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # SPDX-License-Identifier: MIT
 
-"""
-Some documentation to refer to:
+"""Some documentation to refer to:
 
 - Our main web socket (mWS) sends opcode 4 with a guild ID and channel ID.
 - The mWS receives VOICE_STATE_UPDATE and VOICE_SERVER_UPDATE.
 - We pull the session_id from VOICE_STATE_UPDATE.
 - We pull the token, endpoint and server_id from VOICE_SERVER_UPDATE.
 - Then we initiate the voice web socket (vWS) pointing to the endpoint.
 - We send opcode 0 with the user_id, server_id, session_id and token using the vWS.
@@ -146,15 +145,17 @@
         ----------
         force: :class:`bool`
             Whether the disconnection was forced.
         """
         raise NotImplementedError
 
     def cleanup(self) -> None:
-        """This method *must* be called to ensure proper clean-up during a disconnect.
+        """Cleans up the internal state.
+
+        **This method *must* be called to ensure proper clean-up during a disconnect.**
 
         It is advisable to call this from within :meth:`disconnect` when you are
         completely done with the voice protocol instance.
 
         This method removes it from the internal state cache that keeps track of
         currently alive voice clients. Failure to clean-up will cause subsequent
         connections to report that it's still connected.
@@ -166,15 +167,15 @@
 class VoiceClient(VoiceProtocol):
     """Represents a Discord voice connection.
 
     You do not create these, you typically get them from
     e.g. :meth:`VoiceChannel.connect`.
 
     Warning
-    --------
+    -------
     In order to use PCM based AudioSources, you must have the opus library
     installed on your system and loaded through :func:`opus.load_opus`.
     Otherwise, your AudioSources must be opus encoded (e.g. using :class:`FFmpegOpusAudio`)
     or the library will not be able to transmit audio.
 
     Attributes
     ----------
@@ -239,15 +240,15 @@
         return self.channel.guild
 
     @property
     def user(self) -> ClientUser:
         """:class:`ClientUser`: The user connected to voice (i.e. ourselves)."""
         return self._state.user
 
-    def checked_add(self, attr, value, limit) -> None:
+    def checked_add(self, attr: str, value: int, limit: int) -> None:
         val = getattr(self, attr)
         if val + value > limit:
             setattr(self, attr, 0)
         else:
             setattr(self, attr, val + value)
 
     # connection related
@@ -422,14 +423,19 @@
 
     async def poll_voice_ws(self, reconnect: bool) -> None:
         backoff = ExponentialBackoff()
         while True:
             try:
                 await self.ws.poll_event()
             except (ConnectionClosed, asyncio.TimeoutError) as exc:
+                # Ensure the keep alive handler is closed
+                if self.ws._keep_alive:
+                    self.ws._keep_alive.stop()
+                    self.ws._keep_alive = None
+
                 if isinstance(exc, ConnectionClosed):
                     # The following close codes are undocumented so I will document them here.
                     # 1000 - normal closure (obviously)
                     # 4014 - voice channel has been deleted.
                     # 4015 - voice server has crashed
                     if exc.code in (1000, 4015):
                         _log.info("Disconnecting from voice normally, close code %d.", exc.code)
@@ -563,15 +569,14 @@
         ClientException
             Already playing audio or not connected.
         TypeError
             Source is not a :class:`AudioSource` or after is not a callable.
         OpusNotLoaded
             Source is not opus encoded and opus is not loaded.
         """
-
         if not self.is_connected():
             raise ClientException("Not connected to voice.")
 
         if self.is_playing():
             raise ClientException("Already playing audio.")
 
         if not isinstance(source, AudioSource):
@@ -640,15 +645,14 @@
         Raises
         ------
         ClientException
             You are not connected.
         opus.OpusError
             Encoding the data failed.
         """
-
         self.checked_add("sequence", 1, 65535)
         if encode:
             encoded_data = self.encoder.encode(data, self.encoder.SAMPLES_PER_FRAME)
         else:
             encoded_data = data
         packet = self._get_voice_packet(encoded_data)
         try:
```

### Comparing `disnake-2.8.2/disnake/voice_region.py` & `disnake-2.9.0/disnake/voice_region.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,55 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from .types.voice import VoiceRegion as VoiceRegionPayload
 
 
 __all__ = ("VoiceRegion",)
 
 
 class VoiceRegion:
     """Represents a Discord voice region.
 
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two :class:`VoiceRegion`\\s are equal.
+
+            .. versionadded:: 2.9
+
+        .. describe:: x != y
+
+            Checks if two :class:`VoiceRegion`\\s are not equal.
+
+            .. versionadded:: 2.9
+
+        .. describe:: str(x)
+
+            Returns the voice region's ID.
+
     .. versionadded:: 2.5
 
     Attributes
     ----------
     id: :class:`str`
         Unique ID for the region.
     name: :class:`str`
         The name of the region.
     optimal: :class:`bool`
         True for a single region that is closest to your client.
     deprecated: :class:`bool`
         Whether this is a deprecated voice region (avoid switching to these).
     custom: :class:`bool`
-        Whether this is a custom voice region (used for events/etc)
+        Whether this is a custom voice region (used for events/etc).
     """
 
     __slots__ = (
         "id",
         "name",
         "optimal",
         "deprecated",
@@ -46,7 +64,10 @@
         self.custom: bool = data.get("custom", False)
 
     def __str__(self) -> str:
         return self.id
 
     def __repr__(self) -> str:
         return f"<VoiceRegion id={self.id!r} name={self.name!r} optimal={self.optimal!r}>"
+
+    def __eq__(self, other: Any) -> bool:
+        return isinstance(other, VoiceRegion) and self.id == other.id
```

### Comparing `disnake-2.8.2/disnake/webhook/async_.py` & `disnake-2.9.0/disnake/webhook/async_.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 if TYPE_CHECKING:
     import datetime
     from types import TracebackType
 
     from ..abc import Snowflake
     from ..asset import AssetBytes
-    from ..channel import ForumChannel, TextChannel, VoiceChannel
+    from ..channel import ForumChannel, StageChannel, TextChannel, VoiceChannel
     from ..embeds import Embed
     from ..file import File
     from ..guild import Guild
     from ..http import Response
     from ..mentions import AllowedMentions
     from ..message import Attachment
     from ..state import ConnectionState
@@ -475,16 +475,17 @@
 
 def handle_message_parameters_dict(
     content: Optional[str] = MISSING,
     *,
     username: str = MISSING,
     avatar_url: Any = MISSING,
     tts: bool = False,
-    ephemeral: Optional[bool] = None,
-    suppress_embeds: Optional[bool] = None,
+    ephemeral: Optional[bool] = MISSING,
+    suppress_embeds: Optional[bool] = MISSING,
+    flags: MessageFlags = MISSING,
     file: File = MISSING,
     files: List[File] = MISSING,
     attachments: Optional[List[Attachment]] = MISSING,
     embed: Optional[Embed] = MISSING,
     embeds: List[Embed] = MISSING,
     view: Optional[View] = MISSING,
     components: Optional[Components[MessageUIComponent]] = MISSING,
@@ -527,20 +528,22 @@
 
     payload["tts"] = tts
     if avatar_url:
         payload["avatar_url"] = str(avatar_url)
     if username:
         payload["username"] = username
 
-    if ephemeral is not None or suppress_embeds is not None:
-        payload["flags"] = 0
-        if suppress_embeds:
-            payload["flags"] |= MessageFlags.suppress_embeds.flag
-        if ephemeral:
-            payload["flags"] |= MessageFlags.ephemeral.flag
+    if ephemeral not in (None, MISSING) or suppress_embeds not in (None, MISSING):
+        flags = MessageFlags._from_value(0 if flags is MISSING else flags.value)
+        if suppress_embeds not in (None, MISSING):
+            flags.suppress_embeds = suppress_embeds
+        if ephemeral not in (None, MISSING):
+            flags.ephemeral = ephemeral
+    if flags is not MISSING:
+        payload["flags"] = flags.value
 
     if allowed_mentions:
         if previous_allowed_mentions is not None:
             payload["allowed_mentions"] = previous_allowed_mentions.merge(
                 allowed_mentions
             ).to_dict()
         else:
@@ -559,16 +562,17 @@
 
 def handle_message_parameters(
     content: Optional[str] = MISSING,
     *,
     username: str = MISSING,
     avatar_url: Any = MISSING,
     tts: bool = False,
-    ephemeral: Optional[bool] = None,
-    suppress_embeds: Optional[bool] = None,
+    ephemeral: Optional[bool] = MISSING,
+    suppress_embeds: Optional[bool] = MISSING,
+    flags: MessageFlags = MISSING,
     file: File = MISSING,
     files: List[File] = MISSING,
     attachments: Optional[List[Attachment]] = MISSING,
     embed: Optional[Embed] = MISSING,
     embeds: List[Embed] = MISSING,
     view: Optional[View] = MISSING,
     components: Optional[Components[MessageUIComponent]] = MISSING,
@@ -580,14 +584,15 @@
     params = handle_message_parameters_dict(
         content=content,
         username=username,
         avatar_url=avatar_url,
         tts=tts,
         ephemeral=ephemeral,
         suppress_embeds=suppress_embeds,
+        flags=flags,
         file=file,
         files=files,
         attachments=attachments,
         embed=embed,
         embeds=embeds,
         view=view,
         components=components,
@@ -966,16 +971,16 @@
         """Optional[:class:`Guild`]: The guild this webhook belongs to.
 
         If this is a partial webhook, then this will always return ``None``.
         """
         return self._state and self._state._get_guild(self.guild_id)
 
     @property
-    def channel(self) -> Optional[Union[TextChannel, VoiceChannel, ForumChannel]]:
-        """Optional[Union[:class:`TextChannel`, :class:`VoiceChannel`, :class:`ForumChannel`]]: The channel this webhook belongs to.
+    def channel(self) -> Optional[Union[TextChannel, VoiceChannel, ForumChannel, StageChannel]]:
+        """Optional[Union[:class:`TextChannel`, :class:`VoiceChannel`, :class:`ForumChannel`, :class:`StageChannel`]]: The channel this webhook belongs to.
 
         If this is a partial webhook, then this will always return ``None``.
 
         Webhooks in :class:`ForumChannel`\\s can not send messages directly,
         they can only create new threads (see ``thread_name`` for :attr:`Webhook.send`)
         and interact with existing threads.
         """
@@ -1004,15 +1009,16 @@
     """Represents an asynchronous Discord webhook.
 
     Webhooks are a form to send messages to channels in Discord without a
     bot user or authentication.
 
     There are two main ways to use Webhooks. The first is through the ones
     received by the library such as :meth:`.Guild.webhooks`, :meth:`.TextChannel.webhooks`,
-    and :meth:`.VoiceChannel.webhooks`. The ones received by the library will
+    :meth:`.ForumChannel.webhooks`, :meth:`.VoiceChannel.webhooks`,
+    and :meth:`.StageChannel.webhooks`. The ones received by the library will
     automatically be bound using the library's internal HTTP session.
 
     The second form involves creating a webhook object manually using the
     :meth:`~.Webhook.from_url` or :meth:`~.Webhook.partial` classmethods.
 
     For example, creating a webhook from a URL and using :doc:`aiohttp <aio:index>`:
 
@@ -1200,14 +1206,15 @@
             "name": name,
             "channel_id": channel.id,
             "guild_id": channel.guild.id,
             "user": {
                 "username": user.name,
                 "discriminator": user.discriminator,
                 "id": user.id,
+                "global_name": user.global_name,
                 "avatar": user._avatar,
             },
         }
 
         state = channel._state
         session = channel._state.http._HTTPClient__session
         return cls(feed, session=session, state=state, token=state.http.token)
@@ -1430,14 +1437,15 @@
         content: Optional[str] = ...,
         *,
         username: str = ...,
         avatar_url: Any = ...,
         tts: bool = ...,
         ephemeral: bool = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         file: File = ...,
         files: List[File] = ...,
         embed: Embed = ...,
         embeds: List[Embed] = ...,
         allowed_mentions: AllowedMentions = ...,
         view: View = ...,
         components: Components[MessageUIComponent] = ...,
@@ -1454,14 +1462,15 @@
         content: Optional[str] = ...,
         *,
         username: str = ...,
         avatar_url: Any = ...,
         tts: bool = ...,
         ephemeral: bool = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         file: File = ...,
         files: List[File] = ...,
         embed: Embed = ...,
         embeds: List[Embed] = ...,
         allowed_mentions: AllowedMentions = ...,
         view: View = ...,
         components: Components[MessageUIComponent] = ...,
@@ -1475,16 +1484,17 @@
     async def send(
         self,
         content: Optional[str] = MISSING,
         *,
         username: str = MISSING,
         avatar_url: Any = MISSING,
         tts: bool = False,
-        ephemeral: bool = False,
-        suppress_embeds: bool = False,
+        ephemeral: bool = MISSING,
+        suppress_embeds: bool = MISSING,
+        flags: MessageFlags = MISSING,
         file: File = MISSING,
         files: List[File] = MISSING,
         embed: Embed = MISSING,
         embeds: List[Embed] = MISSING,
         allowed_mentions: AllowedMentions = MISSING,
         view: View = MISSING,
         components: Components[MessageUIComponent] = MISSING,
@@ -1595,14 +1605,24 @@
 
         suppress_embeds: :class:`bool`
             Whether to suppress embeds for the message. This hides
             all the embeds from the UI if set to ``True``.
 
             .. versionadded:: 2.5
 
+        flags: :class:`MessageFlags`
+            The flags to set for this message.
+            Only :attr:`~MessageFlags.suppress_embeds`, :attr:`~MessageFlags.ephemeral`
+            and :attr:`~MessageFlags.suppress_notifications` are supported.
+
+            If parameters ``suppress_embeds`` or ``ephemeral`` are provided,
+            they will override the corresponding setting of this ``flags`` parameter.
+
+            .. versionadded:: 2.9
+
         Raises
         ------
         HTTPException
             Sending the message failed.
         NotFound
             This webhook was not found.
         Forbidden
@@ -1658,14 +1678,15 @@
             tts=tts,
             file=file,
             files=files,
             embed=embed,
             embeds=embeds,
             ephemeral=ephemeral,
             suppress_embeds=suppress_embeds,
+            flags=flags,
             view=view,
             components=components,
             thread_name=thread_name,
             allowed_mentions=allowed_mentions,
             previous_allowed_mentions=previous_mentions,
         )
```

### Comparing `disnake-2.8.2/disnake/webhook/sync.py` & `disnake-2.9.0/disnake/webhook/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from errno import ECONNRESET
 from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional, Tuple, Type, Union, overload
 from urllib.parse import quote as urlquote
 
 from .. import utils
 from ..channel import PartialMessageable
 from ..errors import DiscordServerError, Forbidden, HTTPException, NotFound, WebhookTokenMissing
+from ..flags import MessageFlags
 from ..http import Route
 from ..message import Message
 from .async_ import BaseWebhook, _WebhookState, handle_message_parameters
 
 __all__ = (
     "SyncWebhook",
     "SyncWebhookMessage",
@@ -863,14 +864,15 @@
         avatar_url: Any = ...,
         tts: bool = ...,
         file: File = ...,
         files: List[File] = ...,
         embed: Embed = ...,
         embeds: List[Embed] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: AllowedMentions = ...,
         thread: Snowflake = ...,
         thread_name: str = ...,
         wait: Literal[True],
     ) -> SyncWebhookMessage:
         ...
 
@@ -883,14 +885,15 @@
         avatar_url: Any = ...,
         tts: bool = ...,
         file: File = ...,
         files: List[File] = ...,
         embed: Embed = ...,
         embeds: List[Embed] = ...,
         suppress_embeds: bool = ...,
+        flags: MessageFlags = ...,
         allowed_mentions: AllowedMentions = ...,
         thread: Snowflake = ...,
         thread_name: str = ...,
         wait: Literal[False] = ...,
     ) -> None:
         ...
 
@@ -902,14 +905,15 @@
         avatar_url: Any = MISSING,
         tts: bool = False,
         file: File = MISSING,
         files: List[File] = MISSING,
         embed: Embed = MISSING,
         embeds: List[Embed] = MISSING,
         suppress_embeds: bool = MISSING,
+        flags: MessageFlags = MISSING,
         allowed_mentions: AllowedMentions = MISSING,
         thread: Snowflake = MISSING,
         thread_name: Optional[str] = None,
         wait: bool = False,
     ) -> Optional[SyncWebhookMessage]:
         """Sends a message using the webhook.
 
@@ -966,14 +970,24 @@
 
         suppress_embeds: :class:`bool`
             Whether to suppress embeds for the message. This hides
             all the embeds from the UI if set to ``True``.
 
             .. versionadded:: 2.5
 
+        flags: :class:`MessageFlags`
+            The flags to set for this message.
+            Only :attr:`~MessageFlags.suppress_embeds` and :attr:`~MessageFlags.suppress_notifications`
+            are supported.
+
+            If parameter ``suppress_embeds`` is provided,
+            that will override the setting of :attr:`MessageFlags.suppress_embeds`.
+
+            .. versionadded:: 2.9
+
         wait: :class:`bool`
             Whether the server should wait before sending a response. This essentially
             means that the return type of this function changes from ``None`` to
             a :class:`WebhookMessage` if set to ``True``.
 
         Raises
         ------
@@ -1014,14 +1028,15 @@
 
         params = handle_message_parameters(
             content=content,
             username=username,
             avatar_url=avatar_url,
             tts=tts,
             suppress_embeds=suppress_embeds,
+            flags=flags,
             file=file,
             files=files,
             embed=embed,
             embeds=embeds,
             thread_name=thread_name,
             allowed_mentions=allowed_mentions,
             previous_allowed_mentions=previous_mentions,
```

### Comparing `disnake-2.8.2/disnake/welcome_screen.py` & `disnake-2.9.0/disnake/welcome_screen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, List, Optional, Union
 
 from . import utils
 from .partial_emoji import PartialEmoji, _EmojiTag
 
 if TYPE_CHECKING:
     from .emoji import Emoji
     from .guild import Guild
@@ -70,30 +70,23 @@
 
     @classmethod
     def _from_data(
         cls,
         *,
         data: WelcomeScreenChannelPayload,
         state: ConnectionState,
-        guild: Union[Guild, PartialInviteGuild],
     ) -> WelcomeScreenChannel:
-        emoji_id = utils._get_as_snowflake(data, "emoji_id")
-        emoji_name = data.get("emoji_name") or None
-        emoji = None
-        if emoji_name:
-            emojis: Optional[Tuple[Emoji]]
-            if emojis := getattr(guild, "emojis", None):
-                emoji = utils.get(emojis, id=emoji_id, name=emoji_name)
-            if not emoji:
-                emoji = PartialEmoji.with_state(state, name=emoji_name, id=emoji_id)
+        emoji = state._get_emoji_from_fields(
+            name=data.get("emoji_name"),
+            id=utils._get_as_snowflake(data, "emoji_id"),
+        )
 
         return cls(id=int(data["channel_id"]), description=data["description"], emoji=emoji)
 
     def to_dict(self) -> WelcomeScreenChannelPayload:
-
         result: WelcomeScreenChannelPayload = {}  # type: ignore
         result["channel_id"] = self.id
         result["description"] = self.description
 
         if self.emoji is not None:
             if self.emoji.id:
                 result["emoji_id"] = self.emoji.id
@@ -129,15 +122,15 @@
         state: ConnectionState,
         guild: Union[Guild, PartialInviteGuild],
     ) -> None:
         self._state = state
         self._guild = guild
         self.description: Optional[str] = data.get("description")
         self.channels: List[WelcomeScreenChannel] = [
-            WelcomeScreenChannel._from_data(data=channel, state=state, guild=guild)
+            WelcomeScreenChannel._from_data(data=channel, state=state)
             for channel in data["welcome_channels"]
         ]
 
     def __repr__(self) -> str:
         return f"<WelcomeScreen description={self.description!r} channels={self.channels!r} enabled={self.enabled!r}>"
 
     @property
```

### Comparing `disnake-2.8.2/disnake/widget.py` & `disnake-2.9.0/disnake/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,24 +101,29 @@
 
         .. describe:: hash(x)
 
             Return the widget member's hash.
 
         .. describe:: str(x)
 
-            Returns the widget member's `name#discriminator`.
+            Returns the widget member's name.
 
     Attributes
     ----------
     id: :class:`int`
         The member's anonymized ID.
     name: :class:`str`
-        The member's nickname (if set in the guild) or username.
+        The member's name.
     discriminator: :class:`str`
         The member's anonymized discriminator.
+
+        .. note::
+            This is being phased out by Discord; the username system is moving away from ``username#discriminator``
+            to users having a globally unique username.
+            See the `help article <https://dis.gd/app-usernames>`__ for details.
     status: :class:`Status`
         The member's status.
     activity: Optional[Union[:class:`BaseActivity`, :class:`Spotify`]]
         The member's activity. This generally only has the ``name`` set.
     deafened: Optional[:class:`bool`]
         Whether the member is currently deafened.
     muted: Optional[:class:`bool`]
@@ -162,16 +167,15 @@
     def __repr__(self) -> str:
         return f"<WidgetMember name={self.name!r} discriminator={self.discriminator!r}"
 
     # overwrite base type's @property since widget members always seem to have `avatar: null`,
     # and instead a separate `avatar_url` field with a full url
     @property
     def avatar(self) -> Optional[Asset]:
-        """
-        Optional[:class:`Asset`]: The user's avatar.
+        """Optional[:class:`Asset`]: The user's avatar.
         The size can be chosen using :func:`Asset.with_size`, however the format is always
         static and cannot be changed through :func:`Asset.with_format` or similar methods.
         """
         if (url := self._avatar_url) is not None:
             return Asset(self._state, url=url, key=url, animated=False)
         return None
 
@@ -248,15 +252,14 @@
             Editing the widget failed.
 
         Returns
         -------
         :class:`WidgetSettings`
             The new widget settings.
         """
-
         return await self.guild.edit_widget(enabled=enabled, channel=channel, reason=reason)
 
 
 class Widget:
     """Represents a :class:`Guild` widget.
 
     .. container:: operations
@@ -284,17 +287,16 @@
     members: List[:class:`WidgetMember`]
         The online members in the server. Offline members
         do not appear in the widget.
 
         .. note::
 
             Due to a Discord limitation, if this data is available
-            the users will be "anonymized" with linear IDs and discriminator
-            information being incorrect. Likewise, the number of members
-            retrieved is capped.
+            the users will be "anonymized" with linear IDs.
+            Likewise, the number of members retrieved is capped.
 
     presence_count: :class:`int`
         The number of online members in the server.
 
         .. versionadded:: 2.6
     """
```

### Comparing `disnake-2.8.2/disnake.egg-info/PKG-INFO` & `disnake-2.9.0/disnake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disnake
-Version: 2.8.2
+Version: 2.9.0
 Summary: A Python wrapper for the Discord API
 Author: Disnake Development
 License: MIT
 Project-URL: Changelog, https://docs.disnake.dev/page/whats_new.html
 Project-URL: Documentation, https://docs.disnake.dev/
 Project-URL: Repository, https://github.com/DisnakeDev/disnake
 Keywords: disnake,discord,discord api
@@ -20,28 +20,28 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: speed
 Provides-Extra: voice
 Provides-Extra: docs
-Provides-Extra: speed
 Provides-Extra: discord
 License-File: LICENSE
 
 <!-- SPDX-License-Identifier: MIT -->
 
 [![Disnake Banner](https://raw.githubusercontent.com/DisnakeDev/disnake/master/assets/banner.png)](https://disnake.dev/)
 
 disnake
 =======
-
 <p align="center">
+    <img src="https://img.shields.io/github/actions/workflow/status/DisnakeDev/disnake/lint-test.yml?branch=master&style=flat-square"></img>
     <a href="https://discord.gg/disnake"><img src="https://img.shields.io/discord/808030843078836254?style=flat-square&color=5865f2&logo=discord&logoColor=ffffff&label=discord" alt="Discord server invite" /></a>
     <a href="https://pypi.org/project/disnake/"><img src="https://img.shields.io/pypi/v/disnake.svg?style=flat-square" alt="PyPI version info" /></a>
     <a href="https://pypi.org/project/disnake/"><img src="https://img.shields.io/pypi/pyversions/disnake.svg?style=flat-square" alt="PyPI supported Python versions" /></a>
     <a href="https://github.com/DisnakeDev/disnake/commits"><img src="https://img.shields.io/github/commit-activity/w/DisnakeDev/disnake.svg?style=flat-square" alt="Commit activity" /></a>
 </p>
 
 A modern, easy to use, feature-rich, and async-ready API wrapper for Discord written in Python.
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: disnake Version: 2.8.2 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: disnake Version: 2.9.0 Summary: A Python wrapper
 for the Discord API Author: Disnake Development License: MIT Project-URL:
 Changelog, https://docs.disnake.dev/page/whats_new.html Project-URL:
 Documentation, https://docs.disnake.dev/ Project-URL: Repository, https://
 github.com/DisnakeDev/disnake Keywords: disnake,discord,discord api Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Topic ::
 Utilities Classifier: Typing :: Typed Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: voice Provides-Extra: docs
-Provides-Extra: speed Provides-Extra: discord License-File: LICENSE  [![Disnake
+Content-Type: text/markdown Provides-Extra: speed Provides-Extra: voice
+Provides-Extra: docs Provides-Extra: discord License-File: LICENSE  [![Disnake
 Banner](https://raw.githubusercontent.com/DisnakeDev/disnake/master/assets/
 banner.png)](https://disnake.dev/) disnake =======
- [Discord_server_invite] [PyPI_version_info] [PyPI_supported_Python_versions]
-                               [Commit_activity]
+[https://img.shields.io/github/actions/workflow/status/DisnakeDev/disnake/lint-
+test.yml?branch=master&style=flat-square] [Discord_server_invite] [PyPI_version
+           info] [PyPI_supported_Python_versions] [Commit_activity]
 A modern, easy to use, feature-rich, and async-ready API wrapper for Discord
 written in Python. Key Features ------------ - Proper rate limit handling. -
 Type-safety measures. - [FastAPI](https://fastapi.tiangolo.com/)-like slash
 command syntax. The syntax and structure of `discord.py 2.0` is preserved.
 Installing ---------- **Python 3.8 or higher is required.** To install the
 library without full voice support, you can just run the following command: ```
 sh # Linux/macOS python3 -m pip install -U disnake # Windows py -3 -m pip
```

### Comparing `disnake-2.8.2/disnake.egg-info/SOURCES.txt` & `disnake-2.9.0/disnake.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements.txt
 setup.py
-./requirements.txt
-./requirements/requirements_dev.txt
-./requirements/requirements_docs.txt
-./requirements/requirements_speed.txt
-./requirements/requirements_tools.txt
-./requirements/requirements_voice.txt
 disnake/__init__.py
 disnake/__main__.py
 disnake/abc.py
 disnake/activity.py
 disnake/app_commands.py
 disnake/appinfo.py
 disnake/application_role_connection.py
@@ -45,14 +38,15 @@
 disnake/iterators.py
 disnake/member.py
 disnake/mentions.py
 disnake/message.py
 disnake/mixins.py
 disnake/object.py
 disnake/oggparse.py
+disnake/onboarding.py
 disnake/opus.py
 disnake/partial_emoji.py
 disnake/permissions.py
 disnake/player.py
 disnake/py.typed
 disnake/raw_models.py
 disnake/reaction.py
@@ -123,14 +117,15 @@
 disnake/types/guild_scheduled_event.py
 disnake/types/i18n.py
 disnake/types/integration.py
 disnake/types/interactions.py
 disnake/types/invite.py
 disnake/types/member.py
 disnake/types/message.py
+disnake/types/onboarding.py
 disnake/types/role.py
 disnake/types/snowflake.py
 disnake/types/sticker.py
 disnake/types/team.py
 disnake/types/template.py
 disnake/types/threads.py
 disnake/types/user.py
@@ -154,14 +149,16 @@
 disnake/ui/select/user.py
 disnake/webhook/__init__.py
 disnake/webhook/async_.py
 disnake/webhook/sync.py
 tests/test_abc.py
 tests/test_colour.py
 tests/test_embeds.py
+tests/test_events.py
 tests/test_flags.py
 tests/test_http.py
 tests/test_mentions.py
 tests/test_message.py
 tests/test_object.py
+tests/test_onboarding.py
 tests/test_permissions.py
 tests/test_utils.py
```

### Comparing `disnake-2.8.2/tests/test_abc.py` & `disnake-2.9.0/tests/test_abc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # SPDX-License-Identifier: MIT
 
+from typing import cast
 from unittest import mock
 
 import pytest
 
 import disnake
 from disnake.abc import GuildChannel
 from disnake.utils import MISSING
 
 
 @pytest.mark.asyncio
 class TestGuildChannelEdit:
     # TODO: use proper mock models once we have state/guild mocks
-    @pytest.fixture()
+    @pytest.fixture
     def channel(self):
         ch = mock.Mock(GuildChannel, id=123, category_id=456)
         ch._state = mock.Mock(http=mock.AsyncMock())
         ch.guild = mock.Mock()
 
         parent = mock.Mock()
         parent._overwrites = [mock.Mock() for _ in range(3)]
@@ -147,7 +148,20 @@
         res = await GuildChannel._edit(channel, sync_permissions=sync_permissions, overwrites={})
         assert res is not None
 
         channel._move.assert_not_called()
         channel._state.http.edit_channel.assert_awaited_once_with(
             channel.id, permission_overwrites=[], reason=None
         )
+
+
+class TestUserProtocol:
+    def _test_typing_assignable(self) -> None:
+        def handle_abc_user(user: disnake.abc.User) -> None:
+            ...
+
+        # All of these should match the abc.User protocol and thus type-check correctly
+        # (they could just inherit from the protocol to ensure correct implementation,
+        # but we really only want structural (i.e. implicit) subtyping)
+        handle_abc_user(cast(disnake.User, ...))
+        handle_abc_user(cast(disnake.ClientUser, ...))
+        handle_abc_user(cast(disnake.Member, ...))
```

### Comparing `disnake-2.8.2/tests/test_colour.py` & `disnake-2.9.0/tests/test_colour.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,57 +4,57 @@
 from typing import Tuple
 
 import pytest
 
 from disnake import Color, Colour
 
 
-def test_init():
+def test_init() -> None:
     with pytest.raises(TypeError, match=r"Expected int parameter, received str instead."):
         Colour("0")  # type: ignore
 
 
 @pytest.mark.parametrize(
     ("value", "string"), [(0, "#000000"), (0x123, "#000123"), (0x12AB34, "#12ab34")]
 )
-def test_str(value: int, string: str):
+def test_str(value: int, string: str) -> None:
     assert str(Colour(value)) == string
 
 
-def test_compare():
+def test_compare() -> None:
     assert Colour(123) == Colour(123)
 
 
 @pytest.mark.parametrize(
     ("value", "parts"),
     [(0, (0, 0, 0)), (0xA00233, (0xA0, 0x02, 0x33)), (0x123456, (0x12, 0x34, 0x56))],
 )
-def test_to_rgb(value: int, parts: Tuple[int, int, int]):
+def test_to_rgb(value: int, parts: Tuple[int, int, int]) -> None:
     c = Colour(value)
     assert c.to_rgb() == parts
     assert (c.r, c.g, c.b) == parts
 
 
 @pytest.mark.parametrize(
     ("value", "parts"),
     [(0, (0, 0, 0)), (0xA00233, (0xA0, 0x02, 0x33)), (0x123456, (0x12, 0x34, 0x56))],
 )
-def test_from_rgb(value: int, parts: Tuple[int, int, int]):
+def test_from_rgb(value: int, parts: Tuple[int, int, int]) -> None:
     assert Colour.from_rgb(*parts).value == value
 
 
 @pytest.mark.parametrize(
     ("value", "parts"),
     [
         (0xFFFFFF, (123 / 360, 0, 1)),
         (0xF4A8B8, (348 / 360, 31 / 100, 96 / 100)),
         (0x5CCFF9, (196 / 360, 63 / 100, 98 / 100)),
     ],
 )
-def test_from_hsv(value: int, parts: Tuple[float, float, float]):
+def test_from_hsv(value: int, parts: Tuple[float, float, float]) -> None:
     expected = Colour(value)
     col = Colour.from_hsv(*parts)
     assert all(math.isclose(a, b, abs_tol=1) for a, b in zip(expected.to_rgb(), col.to_rgb()))
 
 
-def test_alias():
+def test_alias() -> None:
     assert Color is Colour
```

### Comparing `disnake-2.8.2/tests/test_embeds.py` & `disnake-2.9.0/tests/test_embeds.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 
 from disnake import Color, Embed, File, embeds
 from disnake.utils import MISSING, utcnow
 
 _BASE = {"type": "rich"}
 
 
-@pytest.fixture()
+@pytest.fixture
 def embed() -> Embed:
     time = utcnow() + timedelta(days=42)
     return Embed(
         type="link",
         title="wow",
         description="what a cool embed",
         url="http://endless.horse",
         timestamp=time,
         color=0xF8A8B8,
     )
 
 
-@pytest.fixture()
+@pytest.fixture
 def file() -> File:
     return File(io.BytesIO(b"abcd"), filename="data.txt")
 
 
 def test_init_empty() -> None:
     embed = Embed()
     assert embed.title is None
@@ -60,15 +60,15 @@
     assert Embed().type == "rich"
 
     # type shouldn't be set in from_dict if dict didn't contain a type
     assert Embed.from_dict({}).type is None
 
 
 def test_timestamp_naive(embed: Embed) -> None:
-    embed.timestamp = datetime.now()
+    embed.timestamp = datetime.now()  # noqa: DTZ005  # the point of this is to test naive dts
     assert embed.timestamp.tzinfo is not None
 
 
 def test_len(embed: Embed) -> None:
     assert len(embed) == 20
 
     embed.set_footer(text="hmm", icon_url="https://localhost")
@@ -475,8 +475,8 @@
     with pytest.warns(DeprecationWarning):
         assert Embed.Empty is None  # type: ignore
     with pytest.warns(DeprecationWarning):
         assert Embed().Empty is None  # type: ignore
 
     # make sure unknown module attrs continue to raise
     with pytest.raises(AttributeError):
-        embeds.this_does_not_exist  # type: ignore
+        _ = embeds.this_does_not_exist  # type: ignore
```

### Comparing `disnake-2.8.2/tests/test_flags.py` & `disnake-2.9.0/tests/test_flags.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,12 +490,11 @@
         assert b.values == [2]
         assert (~(a & b)).values == [0, 1]
 
 
 class TestIntents:
     def test_all_only_valid(self) -> None:
         """Test that Intents.all() doesn't include flags that aren't defined."""
-
         intents = flags.Intents.all()
 
         assert not (1 << 18 | 1 << 17) & intents.value
         assert 1 << 20 & intents.value
```

### Comparing `disnake-2.8.2/tests/test_http.py` & `disnake-2.9.0/tests/test_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,9 +39,9 @@
             "wss://gateway.discord.com/?v=10&compress=zlib-stream",
             "json",
             False,
             "wss://gateway.discord.com/?v=10&encoding=json",
         ),
     ],
 )
-def test_format_gateway_url(url: str, encoding: str, zlib: bool, expected: str):
+def test_format_gateway_url(url: str, encoding: str, zlib: bool, expected: str) -> None:
     assert HTTPClient._format_gateway_url(url, encoding=encoding, zlib=zlib) == expected
```

### Comparing `disnake-2.8.2/tests/test_mentions.py` & `disnake-2.9.0/tests/test_mentions.py`

 * *Files identical despite different names*

### Comparing `disnake-2.8.2/tests/test_message.py` & `disnake-2.9.0/tests/test_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,29 +13,29 @@
         # single char
         "💯",
         "🔥",
         # with combining characters
         "👩‍👩‍👧‍👦",
     ],
 )
-def test_convert_emoji_reaction__standard(emoji):
+def test_convert_emoji_reaction__standard(emoji) -> None:
     assert message.convert_emoji_reaction(emoji) == emoji
 
 
 @pytest.mark.parametrize(
     "emoji",
     [
         "test:1234",
         ":test:1234",
         "<:test:1234>",
         "a:test:1234",
         "<a:test:1234>",
     ],
 )
-def test_convert_emoji_reaction__custom(emoji):
+def test_convert_emoji_reaction__custom(emoji) -> None:
     assert message.convert_emoji_reaction(emoji) == "test:1234"
 
 
 def _create_emoji(animated: bool) -> disnake.Emoji:
     return disnake.Emoji(
         guild=disnake.Object(1),  # type: ignore
         state=MISSING,
@@ -49,9 +49,9 @@
         (disnake.PartialEmoji(name="🔥"), "🔥"),
         (_create_emoji(False), "test:1234"),
         (_create_emoji(True), "test:1234"),
         (_create_emoji(False)._to_partial(), "test:1234"),
         (_create_emoji(True)._to_partial(), "test:1234"),
     ],
 )
-def test_convert_emoji_reaction__object(emoji, expected):
+def test_convert_emoji_reaction__object(emoji, expected) -> None:
     assert message.convert_emoji_reaction(emoji) == expected
```

### Comparing `disnake-2.8.2/tests/test_object.py` & `disnake-2.9.0/tests/test_object.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import pytest
 
 from disnake import Object
 
 snowflake = 881536165478499999  # date/time of first commit
 
 
-def test_init():
+def test_init() -> None:
     with pytest.raises(
         TypeError, match=r"id parameter must be convertable to int not <class 'str'>"
     ):
         Object("hi")
 
 
-def test_compare():
+def test_compare() -> None:
     assert Object(42) == Object(42)
     assert Object(42) != Object(43)
 
 
-def test_hash():
+def test_hash() -> None:
     assert hash(Object(snowflake)) == 210174600000
 
 
-def test_created_at():
+def test_created_at() -> None:
     assert Object(snowflake).created_at == datetime(2021, 8, 29, 13, 50, 0, tzinfo=timezone.utc)
```

### Comparing `disnake-2.8.2/tests/test_permissions.py` & `disnake-2.9.0/tests/test_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     )
     def test_handle_overwrite(self, initial: int, allow: int, deny: int, expected: int) -> None:
         perms = Permissions(initial)
         assert perms.value == initial
         perms.handle_overwrite(allow, deny)
         assert perms.value == expected
 
-    def test_none_is_none(self):
+    def test_none_is_none(self) -> None:
         perms = Permissions.none()
         assert perms.value == 0
 
     @pytest.mark.parametrize(
         "method_name",
         [
             "all",
@@ -185,15 +185,15 @@
             "stage",
             "stage_moderator",
             "events",
             "advanced",
             "private_channel",
         ],
     )
-    def test_classmethods(self, method_name: str):
+    def test_classmethods(self, method_name: str) -> None:
         method = getattr(Permissions, method_name)
 
         perms: Permissions = method()
         assert isinstance(perms, Permissions)
 
         # check that caching does not return the same permissions instance
         perms_two: Permissions = method()
```

### Comparing `disnake-2.8.2/tests/test_utils.py` & `disnake-2.9.0/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,57 +16,57 @@
 
 import disnake
 from disnake import utils
 
 from . import helpers
 
 
-def test_missing():
+def test_missing() -> None:
     assert utils.MISSING != utils.MISSING
     assert not bool(utils.MISSING)
 
 
-def test_cached_property():
+def test_cached_property() -> None:
     class Test:
         @utils.cached_property
         def prop(self) -> object:
-            """stuff"""
+            """Does things"""
             return object()
 
     inst = Test()
     assert inst.prop is inst.prop
-    assert Test.prop.__doc__ == "stuff"
+    assert Test.prop.__doc__ == "Does things"
     assert isinstance(Test.prop, utils.cached_property)
 
 
-def test_cached_slot_property():
+def test_cached_slot_property() -> None:
     class Test:
         __slots__ = ("_cs_prop",)
 
         @utils.cached_slot_property("_cs_prop")
         def prop(self) -> object:
-            """stuff"""
+            """Does things"""
             return object()
 
     inst = Test()
     assert inst.prop is inst.prop
-    assert Test.prop.__doc__ == "stuff"
+    assert Test.prop.__doc__ == "Does things"
     assert isinstance(Test.prop, utils.CachedSlotProperty)
 
 
-def test_parse_time():
+def test_parse_time() -> None:
     assert utils.parse_time(None) is None
     assert utils.parse_time("2021-08-29T13:50:00+00:00") == datetime.datetime(
         2021, 8, 29, 13, 50, 0, tzinfo=timezone.utc
     )
 
 
-def test_copy_doc():
+def test_copy_doc() -> None:
     def func(num: int, *, arg: str) -> float:
-        """returns the best number"""
+        """Returns the best number"""
         ...
 
     @utils.copy_doc(func)
     def func2(*args: Any, **kwargs: Any) -> Any:
         ...
 
     assert func2.__doc__ == func.__doc__
@@ -74,15 +74,15 @@
 
 
 @mock.patch.object(warnings, "warn")
 @pytest.mark.parametrize(
     ("instead", "msg"),
     [(None, "stuff is deprecated."), ("other", "stuff is deprecated, use other instead.")],
 )
-def test_deprecated(mock_warn: mock.Mock, instead, msg):
+def test_deprecated(mock_warn: mock.Mock, instead, msg) -> None:
     @utils.deprecated(instead)
     def stuff(num: int) -> int:
         return num
 
     assert stuff(42) == 42
     mock_warn.assert_called_once_with(msg, stacklevel=3, category=DeprecationWarning)
 
@@ -111,77 +111,66 @@
             disnake.Object(9999),
             "http://endless.horse",
             ["bot", "applications.commands"],
             True,
         ),
     ],
 )
-def test_oauth_url(expected, perms, guild, redirect, scopes, disable_select):
+def test_oauth_url(expected, perms, guild, redirect, scopes, disable_select) -> None:
     url = utils.oauth_url(
         1234,
         permissions=perms,
         guild=guild,
         redirect_uri=redirect,
         scopes=scopes,
         disable_guild_select=disable_select,
     )
     assert dict(yarl.URL(url).query) == {"client_id": "1234", **expected}
 
 
-def test_parse_token():
-    # don't get your hopes up, this token isn't valid.
-    # taken from https://guide.disnake.dev/getting-started/initial-files
-    token = "OTA4MjgxMjk4NTU1MTA5Mzk2.YYzc4A.TB7Ng6DOnVDlpMS4idjGptsreFg"  # noqa: S105
-
-    parts = utils.parse_token(token)
-    assert parts[0] == 908281298555109396
-    assert parts[1] == datetime.datetime(2021, 11, 11, 9, 5, 36, tzinfo=timezone.utc)
-    assert parts[2] == bytes.fromhex("4c1ecd83a0ce9d50e5a4c4b889d8c6a6db2b7858")
-
-
 @pytest.mark.parametrize(
     ("num", "expected"),
     [
         (0, datetime.datetime(2015, 1, 1, tzinfo=timezone.utc)),
         (881536165478499999, datetime.datetime(2021, 8, 29, 13, 50, 0, tzinfo=timezone.utc)),
         (10000000000000000000, datetime.datetime(2090, 7, 20, 17, 49, 51, tzinfo=timezone.utc)),
     ],
 )
-def test_snowflake_time(num, expected):
+def test_snowflake_time(num: int, expected) -> None:
     assert utils.snowflake_time(num).replace(microsecond=0) == expected
 
 
 @pytest.mark.parametrize(
     ("dt", "expected"),
     [
         (datetime.datetime(2015, 1, 1, tzinfo=timezone.utc), 0),
         (datetime.datetime(2021, 8, 29, 13, 50, 0, tzinfo=timezone.utc), 881536165478400000),
     ],
 )
-def test_time_snowflake(dt, expected):
+def test_time_snowflake(dt, expected) -> None:
     low = utils.time_snowflake(dt)
     assert low == expected
 
     high = utils.time_snowflake(dt, high=True)
     assert low < high
     assert high + 1 == utils.time_snowflake(dt + timedelta(milliseconds=1))
 
 
-def test_find():
+def test_find() -> None:
     pred = lambda i: i == 42  # type: ignore
     assert utils.find(pred, []) is None
     assert utils.find(pred, [42]) == 42
     assert utils.find(pred, [1, 2, 42, 3, 4]) == 42
 
     pred = lambda i: i.id == 42  # type: ignore
     lst = list(map(disnake.Object, [1, 42, 42, 2]))
     assert utils.find(pred, lst) is lst[1]
 
 
-def test_get():
+def test_get() -> None:
     @dataclass
     class A:
         value: int
 
     @dataclass
     class B:
         value: int
@@ -210,33 +199,33 @@
     [
         ([1, 1, 1], [1]),
         ([3, 2, 1, 2], [3, 2, 1]),
         ([1, 2], [1, 2]),
         ([2, 1], [2, 1]),
     ],
 )
-def test_unique(it, expected):
+def test_unique(it, expected) -> None:
     assert utils._unique(it) == expected
 
 
 @pytest.mark.parametrize(
     ("data", "expected"),
     [
         ({}, None),
         ({"a": 42}, None),
         ({"key": None}, None),
         ({"key": 42}, 42),
         ({"key": "42"}, 42),
     ],
 )
-def test_get_as_snowflake(data, expected):
+def test_get_as_snowflake(data, expected) -> None:
     assert utils._get_as_snowflake(data, "key") == expected
 
 
-def test_maybe_cast():
+def test_maybe_cast() -> None:
     convert = lambda v: v + 1  # type: ignore
     default = object()
 
     assert utils._maybe_cast(utils.MISSING, convert) is None
     assert utils._maybe_cast(utils.MISSING, convert, default) is default
 
     assert utils._maybe_cast(42, convert) == 43
@@ -252,15 +241,15 @@
         (b"\xFF\xD8\xFFxxxxxxxxxxxx", "image/jpeg", ".jpg"),
         (b"xxxxxxJFIF", "image/jpeg", ".jpg"),
         (b"\x47\x49\x46\x38\x37\x61", "image/gif", ".gif"),
         (b"\x47\x49\x46\x38\x39\x61", "image/gif", ".gif"),
         (b"RIFFxxxxWEBP", "image/webp", ".webp"),
     ],
 )
-def test_mime_type_valid(data, expected_mime, expected_ext):
+def test_mime_type_valid(data, expected_mime, expected_ext) -> None:
     for d in (data, data + b"\xFF"):
         assert utils._get_mime_type_for_image(d) == expected_mime
         assert utils._get_extension_for_image(d) == expected_ext
 
     prefixed = b"\xFF" + data
     with pytest.raises(ValueError, match=r"Unsupported image type given"):
         utils._get_mime_type_for_image(prefixed)
@@ -273,22 +262,22 @@
         b"\x89\x50\x4E\x47\x0D\x0A\x1A\xFF",  # invalid png end
         b"\x47\x49\x46\x38\x38\x61",  # invalid gif version
         b"RIFFxxxxAAAA",
         b"AAAAxxxxWEBP",
         b"",
     ],
 )
-def test_mime_type_invalid(data):
+def test_mime_type_invalid(data) -> None:
     with pytest.raises(ValueError, match=r"Unsupported image type given"):
         utils._get_mime_type_for_image(data)
     assert utils._get_extension_for_image(data) is None
 
 
 @pytest.mark.asyncio
-async def test_assetbytes_base64():
+async def test_assetbytes_base64() -> None:
     assert await utils._assetbytes_to_base64_data(None) is None
 
     # test bytes
     data = b"RIFFabcdWEBPwxyz"
     expected = "data:image/webp;base64,UklGRmFiY2RXRUJQd3h5eg=="
     for conv in (bytes, bytearray, memoryview):
         assert await utils._assetbytes_to_base64_data(conv(data)) == expected
@@ -308,15 +297,15 @@
         # use timestamp
         (42, True, 7),
         (utils.MISSING, False, 7),
         (utils.MISSING, True, 7),
     ],
 )
 @helpers.freeze_time()
-def test_parse_ratelimit_header(after, use_clock, expected):
+def test_parse_ratelimit_header(after, use_clock, expected) -> None:
     reset_time = utils.utcnow() + timedelta(seconds=7)
 
     request = mock.Mock()
     request.headers = {"X-Ratelimit-Reset": reset_time.timestamp()}
     if after is not utils.MISSING:
         request.headers["X-Ratelimit-Reset-After"] = after
 
@@ -327,15 +316,15 @@
     "func",
     [
         mock.Mock(),
         mock.AsyncMock(),
     ],
 )
 @pytest.mark.asyncio
-async def test_maybe_coroutine(func: mock.Mock):
+async def test_maybe_coroutine(func: mock.Mock) -> None:
     assert await utils.maybe_coroutine(func, 42, arg="uwu") is func.return_value
     func.assert_called_once_with(42, arg="uwu")
 
 
 @pytest.mark.parametrize("mock_type", [mock.Mock, mock.AsyncMock])
 @pytest.mark.parametrize(
     ("gen", "expected"),
@@ -344,21 +333,21 @@
         ([True], True),
         ([False], False),
         ([False, True], False),
         ([True, False, True], False),
     ],
 )
 @pytest.mark.asyncio
-async def test_async_all(mock_type, gen, expected):
+async def test_async_all(mock_type, gen, expected) -> None:
     assert await utils.async_all(mock_type(return_value=x)() for x in gen) is expected
 
 
 @pytest.mark.looptime
 @pytest.mark.asyncio
-async def test_sane_wait_for(looptime):
+async def test_sane_wait_for(looptime) -> None:
     times = [10, 50, 25]
 
     def create():
         return [asyncio.sleep(n) for n in times]
 
     # no timeout
     await utils.sane_wait_for(create(), timeout=100)
@@ -373,15 +362,15 @@
     assert [t.done() for t in tasks] == [True, False, True]
 
     # tasks should continue running even if timeout occurred
     await asyncio.sleep(1000)
     assert all(t.done() for t in tasks)
 
 
-def test_get_slots():
+def test_get_slots() -> None:
     class A:
         __slots__ = ("a", "a2")
 
     class B:
         __slots__ = ()
 
     class C(A):
@@ -402,45 +391,45 @@
         None,
         timezone.utc,
         timezone(timedelta(hours=-9)),
     ],
 )
 @pytest.mark.parametrize(("delta", "expected"), [(7, 7), (-100, 0)])
 @helpers.freeze_time()
-def test_compute_timedelta(tz, delta, expected):
-    dt = datetime.datetime.now()
+def test_compute_timedelta(tz, delta, expected) -> None:
+    dt = datetime.datetime.now()  # noqa: DTZ005
     if tz is not utils.MISSING:
         dt = dt.astimezone(tz)
     assert utils.compute_timedelta(dt + timedelta(seconds=delta)) == expected
 
 
 @pytest.mark.parametrize(("delta", "expected"), [(0, 0), (42, 42), (-100, 0)])
 @pytest.mark.looptime
 @pytest.mark.asyncio
 @helpers.freeze_time()
-async def test_sleep_until(looptime, delta, expected):
+async def test_sleep_until(looptime, delta, expected) -> None:
     o = object()
     assert await utils.sleep_until(utils.utcnow() + timedelta(seconds=delta), o) is o
     assert looptime == expected
 
 
-def test_utcnow():
+def test_utcnow() -> None:
     assert utils.utcnow().tzinfo == timezone.utc
 
 
-def test_valid_icon_size():
+def test_valid_icon_size() -> None:
     for s in (2**x for x in range(4, 13)):
         assert utils.valid_icon_size(s)
 
     for s in [0, 1, 2, 8, 24, 100, 2**20]:
         assert not utils.valid_icon_size(s)
 
 
 @pytest.mark.parametrize(("s", "expected"), [("a一b", 4), ("abc", 3)])
-def test_string_width(s, expected):
+def test_string_width(s, expected) -> None:
     assert utils._string_width(s) == expected
 
 
 @pytest.mark.parametrize(
     ("url", "params", "expected"),
     [
         (mock.Mock(disnake.Invite, code="uwu"), {}, "uwu"),
@@ -448,15 +437,15 @@
         ("https://discord.com/disnake", {}, "https://discord.com/disnake"),
         ("https://discord.com/invite/disnake", {}, "disnake"),
         ("http://discord.gg/disnake?param=123%20456", {"param": "123 456"}, "disnake"),
         ("https://discordapp.com/invite/disnake?a=1&a=2", {"a": "1"}, "disnake"),
     ],
 )
 @pytest.mark.parametrize("with_params", [False, True])
-def test_resolve_invite(url, params, expected, with_params):
+def test_resolve_invite(url, params, expected, with_params) -> None:
     res = utils.resolve_invite(url, with_params=with_params)
     if with_params:
         assert res == (expected, params)
     else:
         assert res == expected
 
 
@@ -467,15 +456,15 @@
         ("uwu", "uwu"),
         ("http://discord.com/disnake", "http://discord.com/disnake"),
         ("http://discord.new/disnake", "disnake"),
         ("https://discord.com/template/disnake", "disnake"),
         ("https://discordapp.com/template/disnake", "disnake"),
     ],
 )
-def test_resolve_template(url, expected):
+def test_resolve_template(url, expected) -> None:
     assert utils.resolve_template(url) == expected
 
 
 @pytest.mark.parametrize(
     ("text", "exp_remove", "exp_escape"),
     [
         (
@@ -494,15 +483,15 @@
             "*h*\n> [li|nk](~~url~~) xyz **https://google.com/stuff?uwu=owo",
             "h\n xyz https://google.com/stuff?uwu=owo",
             # NOTE: currently doesn't escape inside `[x](y)`, should that be changed?
             r"\*h\*" "\n" r"\> \[li|nk](~~url~~) xyz \*\*https://google.com/stuff?uwu=owo",
         ),
     ],
 )
-def test_markdown(text, exp_remove, exp_escape):
+def test_markdown(text: str, exp_remove, exp_escape) -> None:
     assert utils.remove_markdown(text, ignore_links=False) == exp_remove
     assert utils.remove_markdown(text, ignore_links=True) == exp_remove
 
     assert utils.escape_markdown(text, ignore_links=False) == exp_escape
     assert utils.escape_markdown(text, ignore_links=True) == exp_escape
 
 
@@ -517,30 +506,30 @@
         (
             "abc [link](http://test~test.com)\n>>> <http://endless.horse/_*>",
             "abc \n<http://endless.horse/>",
             "abc \n<http://endless.horse/_*>",
         ),
     ],
 )
-def test_markdown_links(text, expected, expected_ignore):
+def test_markdown_links(text: str, expected, expected_ignore) -> None:
     assert utils.remove_markdown(text, ignore_links=False) == expected
     assert utils.remove_markdown(text, ignore_links=True) == expected_ignore
 
 
 @pytest.mark.parametrize(
     ("text", "expected"),
     [
         ("@everyone hey look at this cat", "@\u200beveryone hey look at this cat"),
         ("test @here", "test @\u200bhere"),
         ("<@12341234123412341> hi", "<@\u200b12341234123412341> hi"),
         ("<@!12341234123412341>", "<@\u200b!12341234123412341>"),
         ("<@&12341234123412341>", "<@\u200b&12341234123412341>"),
     ],
 )
-def test_escape_mentions(text, expected):
+def test_escape_mentions(text: str, expected) -> None:
     assert utils.escape_mentions(text) == expected
 
 
 @pytest.mark.parametrize(
     ("docstring", "expected"),
     [
         (None, ""),
@@ -586,16 +575,16 @@
             ----
             abc
             """,
             "stuff\n----\nabc",
         ),
     ],
 )
-def test_parse_docstring_desc(docstring, expected):
-    def f():
+def test_parse_docstring_desc(docstring: Optional[str], expected) -> None:
+    def f() -> None:
         ...
 
     f.__doc__ = docstring
     assert utils.parse_docstring(f) == {
         "description": expected,
         "params": {},
         "localization_key_name": None,
@@ -646,30 +635,29 @@
             Parameters
             ----------
             """,
             {},
         ),
     ],
 )
-def test_parse_docstring_param(docstring, expected):
-    def f():
+def test_parse_docstring_param(docstring: str, expected) -> None:
+    def f() -> None:
         ...
 
     f.__doc__ = docstring
     expected = {
         k: {**v, "type": None, "localization_key_name": None, "localization_key_desc": None}
         for k, v in expected.items()
     }
     assert utils.parse_docstring(f)["params"] == expected  # ignore description
 
 
-def test_parse_docstring_localizations():
-    def f():
-        """
-        Does stuff. {{cool_key}}
+def test_parse_docstring_localizations() -> None:
+    def f() -> None:
+        """Does stuff. {{cool_key}}
 
         Parameters
         ----------
         p1: {{ PARAM_1 }} Probably a number.
         p2: str
             Definitely a string {{   PARAM_X }}
         """
@@ -704,54 +692,54 @@
         ([0], 3, [[0]]),
         ([0, 1, 2], 2, [[0, 1], [2]]),
         ([0, 1, 2, 3, 4, 5], 3, [[0, 1, 2], [3, 4, 5]]),
     ],
 )
 @pytest.mark.parametrize("sync", [False, True])
 @pytest.mark.asyncio
-async def test_as_chunks(sync, it, max_size, expected):
+async def test_as_chunks(sync, it, max_size: int, expected) -> None:
     if sync:
         assert list(utils.as_chunks(it, max_size)) == expected
     else:
 
         async def _it():
             for x in it:
                 yield x
 
         assert [x async for x in utils.as_chunks(_it(), max_size)] == expected
 
 
 @pytest.mark.parametrize("max_size", [-1, 0])
-def test_as_chunks_size(max_size):
+def test_as_chunks_size(max_size: int) -> None:
     with pytest.raises(ValueError, match=r"Chunk sizes must be greater than 0."):
         utils.as_chunks(iter([]), max_size)
 
 
 @pytest.mark.parametrize(
     ("params", "expected"),
     [
         ([], ()),
         ([disnake.CommandInter, int, Optional[str]], (disnake.CommandInter, int, Optional[str])),
         # check flattening + deduplication (both of these are done automatically in 3.9.1+)
         ([float, Literal[1, 2, Literal[3, 4]], Literal["a", "bc"]], (float, 1, 2, 3, 4, "a", "bc")),
         ([Literal[1, 1, 2, 3, 3]], (1, 2, 3)),
     ],
 )
-def test_flatten_literal_params(params, expected):
+def test_flatten_literal_params(params, expected) -> None:
     assert utils.flatten_literal_params(params) == expected
 
 
 NoneType = type(None)
 
 
 @pytest.mark.parametrize(
     ("params", "expected"),
     [([NoneType], (NoneType,)), ([NoneType, int, NoneType, float], (int, float, NoneType))],
 )
-def test_normalise_optional_params(params, expected):
+def test_normalise_optional_params(params, expected) -> None:
     assert utils.normalise_optional_params(params) == expected
 
 
 @pytest.mark.parametrize(
     ("tp", "expected", "expected_cache"),
     [
         # simple types
@@ -773,42 +761,42 @@
             "int | Literal[False]",
             Union[int, Literal[False]],
             True,
             marks=pytest.mark.skipif(sys.version_info < (3, 10), reason="syntax requires py3.10"),
         ),
     ],
 )
-def test_resolve_annotation(tp, expected, expected_cache):
+def test_resolve_annotation(tp, expected, expected_cache) -> None:
     cache = {}
     result = utils.resolve_annotation(tp, globals(), locals(), cache)
     assert result == expected
 
     # check if state is what we expect
     assert bool(cache) == expected_cache
     # if it's a forward ref, resolve again and ensure cache is used
     if isinstance(tp, str):
         assert utils.resolve_annotation(tp, globals(), locals(), cache) is result
 
 
-def test_resolve_annotation_literal():
+def test_resolve_annotation_literal() -> None:
     with pytest.raises(
         TypeError, match=r"Literal arguments must be of type str, int, bool, or NoneType."
     ):
-        utils.resolve_annotation(Literal[datetime.datetime.now(), 3], globals(), locals(), {})  # type: ignore
+        utils.resolve_annotation(Literal[timezone.utc, 3], globals(), locals(), {})  # type: ignore
 
 
 @pytest.mark.parametrize(
     ("dt", "style", "expected"),
     [
         (0, "F", "<t:0:F>"),
         (1630245000.1234, "T", "<t:1630245000:T>"),
         (datetime.datetime(2021, 8, 29, 13, 50, 0, tzinfo=timezone.utc), "f", "<t:1630245000:f>"),
     ],
 )
-def test_format_dt(dt, style, expected):
+def test_format_dt(dt, style, expected) -> None:
     assert utils.format_dt(dt, style) == expected
 
 
 @pytest.fixture(scope="session")
 def tmp_module_root(tmp_path_factory):
     # this obviously isn't great code, but it'll do just fine for tests
     tmpdir = tmp_path_factory.mktemp("module_root")
@@ -830,15 +818,15 @@
     ("path", "expected"),
     [
         (".", ["test", "mod.ext"]),
         ("./", ["test", "mod.ext"]),
         ("empty/", []),
     ],
 )
-def test_search_directory(tmp_module_root, path, expected):
+def test_search_directory(tmp_module_root, path, expected) -> None:
     orig_cwd = os.getcwd()
     try:
         os.chdir(tmp_module_root)
 
         # test relative and absolute paths
         for p in [path, os.path.abspath(path)]:
             assert sorted(utils.search_directory(p)) == sorted(expected)
@@ -850,15 +838,15 @@
     ("path", "exc"),
     [
         ("../../", r"Modules outside the cwd require a package to be specified"),
         ("nonexistent", r"Provided path '.*?nonexistent' does not exist"),
         ("test.py", r"Provided path '.*?test.py' is not a directory"),
     ],
 )
-def test_search_directory_exc(tmp_module_root, path, exc):
+def test_search_directory_exc(tmp_module_root, path, exc) -> None:
     orig_cwd = os.getcwd()
     try:
         os.chdir(tmp_module_root)
 
         with pytest.raises(ValueError, match=exc):
             list(utils.search_directory(tmp_module_root / path))
     finally:
@@ -872,23 +860,23 @@
         ("en-US", "en-US"),
         ("en_US", "en-US"),
         ("de", "de"),
         ("de-DE", "de"),
         ("de_DE", "de"),
     ],
 )
-def test_as_valid_locale(locale, expected):
+def test_as_valid_locale(locale, expected) -> None:
     assert utils.as_valid_locale(locale) == expected
 
 
 @pytest.mark.parametrize(
     ("values", "expected"),
     [
         ([], "<none>"),
         (["one"], "one"),
         (["one", "two"], "one plus two"),
         (["one", "two", "three"], "one, two, plus three"),
         (["one", "two", "three", "four"], "one, two, three, plus four"),
     ],
 )
-def test_humanize_list(values, expected):
+def test_humanize_list(values, expected) -> None:
     assert utils.humanize_list(values, "plus") == expected
```

