# Comparing `tmp/neon-skill-user_settings-0.5.2a2.tar.gz` & `tmp/neon-skill-user_settings-0.5.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-user_settings-0.5.2a2.tar", last modified: Thu Jun 15 22:00:53 2023, max compression
+gzip compressed data, was "neon-skill-user_settings-0.5.2a3.tar", last modified: Tue Jun 20 23:08:32 2023, max compression
```

## Comparing `neon-skill-user_settings-0.5.2a2.tar` & `neon-skill-user_settings-0.5.2a3.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:00:53.010556 neon-skill-user_settings-0.5.2a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-15 22:00:53.010556 neon-skill-user_settings-0.5.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    50468 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:00:52.998556 neon-skill-user_settings-0.5.2a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:00:52.998556 neon-skill-user_settings-0.5.2a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:00:53.006556 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/also_change_location_tz.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/birthday_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/birthday_is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/birthday_not_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/birthday_not_known.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/change_location_tz.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/dialog_mode_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/dialog_mode_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/email_already_set_same.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/email_confirmation.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/email_is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/email_not_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/email_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/email_not_known.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/email_overwrite.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/email_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/email_set_error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/error_change_username.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/happy_birthday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/hesitation_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/hesitation_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/language_change_confirmation.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/language_not_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/language_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/language_not_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/language_not_recognized.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/language_not_supported.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/language_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/language_setting.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/location_is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/location_not_found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/location_uknown_offline.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/location_unknown_online.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/name_is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/name_no_username.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/name_not_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/name_not_known.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/name_set_full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/name_set_part.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/only_one_language.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/speech_speed_faster.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/speech_speed_limit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/speech_speed_normal.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/speech_speed_slower.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/time_format_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/time_format_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/transcription_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/transcription_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/units_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/units_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_at.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_audio.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_email_title.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_faster.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_female.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_first_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_full_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_imperial.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_last_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_limited.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_male.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_metric.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_middle_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_preferred_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_primary.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_random.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_secondary.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_slower.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_speak.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_stt.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_text.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_timezone.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_understand.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/dialog/word_username.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:00:53.006556 neon-skill-user_settings-0.5.2a2/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/intent/language_settings.intent
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/intent/language_stt.intent
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/intent/language_tts.intent
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/intent/when_is_my_birthday.intent
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/intent/where_am_i.intent
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/intent/who_am_i.intent
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/languages.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:00:53.006556 neon-skill-user_settings-0.5.2a2/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/regex/language.rx
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/regex/name.rx
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/regex/place.rx
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/regex/primary_tts.rx
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/regex/secondary_tts.rx
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/regex/setting.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:00:53.010556 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/at.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/audio.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/birthday.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/deny.voc
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/dialog_mode.voc
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/dot.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/email.voc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/faster.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/female.voc
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/first_name.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/full.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/full_name.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/half.voc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/hesitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/imperial.voc
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/language.voc
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/language_settings.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/language_stt.voc
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/language_tts.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/last_name.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/limited.voc
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/location.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/male.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/metric.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/middle_name.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/my.voc
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/my_name_is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/name.voc
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/no_secondary_language.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/normally.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/permit.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/preferred.voc
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/preferred_name.voc
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/random.voc
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/retention.voc
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/second.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/slower.voc
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/speak_to_me.voc
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/tell_me_my.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/text.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/timezone.voc
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/units.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/locale/en-us/vocab/username.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:00:53.010556 neon-skill-user_settings-0.5.2a2/neon_skill_user_settings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-15 22:00:52.000000 neon-skill-user_settings-0.5.2a2/neon_skill_user_settings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-15 22:00:52.000000 neon-skill-user_settings-0.5.2a2/neon_skill_user_settings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:00:52.000000 neon-skill-user_settings-0.5.2a2/neon_skill_user_settings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-15 22:00:52.000000 neon-skill-user_settings-0.5.2a2/neon_skill_user_settings.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 22:00:52.000000 neon-skill-user_settings-0.5.2a2/neon_skill_user_settings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 22:00:52.000000 neon-skill-user_settings-0.5.2a2/neon_skill_user_settings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:00:53.010556 neon-skill-user_settings-0.5.2a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:00:53.010556 neon-skill-user_settings-0.5.2a2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    75751 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:00:53.010556 neon-skill-user_settings-0.5.2a2/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/ui/SYSTEM_InputBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:00:48.000000 neon-skill-user_settings-0.5.2a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:08:32.214647 neon-skill-user_settings-0.5.2a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-20 23:08:32.214647 neon-skill-user_settings-0.5.2a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    50521 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:08:32.202647 neon-skill-user_settings-0.5.2a3/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:08:32.202647 neon-skill-user_settings-0.5.2a3/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:08:32.210647 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/also_change_location_tz.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/birthday_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/birthday_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/birthday_not_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/birthday_not_known.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/change_location_tz.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/dialog_mode_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/dialog_mode_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/email_already_set_same.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/email_confirmation.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/email_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/email_not_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/email_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/email_not_known.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/email_overwrite.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/email_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/email_set_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/error_change_username.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/happy_birthday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/hesitation_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/hesitation_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/language_change_confirmation.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/language_not_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/language_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/language_not_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/language_not_recognized.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/language_not_supported.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/language_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/language_setting.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/location_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/location_not_found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/location_uknown_offline.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/location_unknown_online.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/name_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/name_no_username.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/name_not_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/name_not_known.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/name_set_full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/name_set_part.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/only_one_language.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/speech_speed_faster.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/speech_speed_limit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/speech_speed_normal.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/speech_speed_slower.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/time_format_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/time_format_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/transcription_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/transcription_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/units_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/units_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_at.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_audio.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_email_title.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_faster.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_female.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_first_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_full_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_imperial.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_last_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_limited.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_male.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_metric.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_middle_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_preferred_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_primary.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_random.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_secondary.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_slower.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_speak.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_stt.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_text.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_timezone.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_understand.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/dialog/word_username.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:08:32.210647 neon-skill-user_settings-0.5.2a3/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/intent/language_settings.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/intent/language_stt.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/intent/language_tts.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/intent/when_is_my_birthday.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/intent/where_am_i.intent
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/intent/who_am_i.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/languages.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:08:32.210647 neon-skill-user_settings-0.5.2a3/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/regex/language.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/regex/name.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/regex/place.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/regex/primary_tts.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/regex/secondary_tts.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/regex/setting.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:08:32.214647 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/at.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/audio.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/birthday.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/deny.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/dialog_mode.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/dot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/email.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/faster.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/female.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/first_name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/full.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/full_name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/half.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/hesitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/imperial.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/language.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/language_settings.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/language_stt.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/language_tts.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/last_name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/limited.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/location.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/male.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/metric.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/middle_name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/my.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/my_name_is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/no_secondary_language.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/normally.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/permit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/preferred.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/preferred_name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/random.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/retention.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/second.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/slower.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/speak_to_me.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/tell_me_my.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/text.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/timezone.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/units.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/locale/en-us/vocab/username.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:08:32.214647 neon-skill-user_settings-0.5.2a3/neon_skill_user_settings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-20 23:08:32.000000 neon-skill-user_settings-0.5.2a3/neon_skill_user_settings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-20 23:08:32.000000 neon-skill-user_settings-0.5.2a3/neon_skill_user_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:08:32.000000 neon-skill-user_settings-0.5.2a3/neon_skill_user_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 23:08:32.000000 neon-skill-user_settings-0.5.2a3/neon_skill_user_settings.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 23:08:32.000000 neon-skill-user_settings-0.5.2a3/neon_skill_user_settings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 23:08:32.000000 neon-skill-user_settings-0.5.2a3/neon_skill_user_settings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:08:32.214647 neon-skill-user_settings-0.5.2a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:08:32.214647 neon-skill-user_settings-0.5.2a3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    75751 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:08:32.214647 neon-skill-user_settings-0.5.2a3/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/ui/SYSTEM_InputBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-20 23:08:25.000000 neon-skill-user_settings-0.5.2a3/version.py
```

### Comparing `neon-skill-user_settings-0.5.2a2/LICENSE.md` & `neon-skill-user_settings-0.5.2a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-0.5.2a2/PKG-INFO` & `neon-skill-user_settings-0.5.2a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-user_settings
-Version: 0.5.2a2
+Version: 0.5.2a3
 Home-page: https://github.com/NeonGeckoCom/skill-user_settings
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-user_settings-0.5.2a2/README.md` & `neon-skill-user_settings-0.5.2a3/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-0.5.2a2/__init__.py` & `neon-skill-user_settings-0.5.2a3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,30 +52,31 @@
 
 
 class UserSettingsSkill(NeonSkill):
     MAX_SPEECH_SPEED = 1.5
     MIN_SPEECH_SPEED = 0.7
 
     def __init__(self, **kwargs):
-        NeonSkill.__init__(self, **kwargs)
         self._languages = None
         self._get_location = Event()
+        NeonSkill.__init__(self, **kwargs)
 
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(network_before_load=False,
                                    internet_before_load=False,
                                    gui_before_load=False,
                                    requires_internet=True,
                                    requires_network=True,
                                    requires_gui=False,
                                    no_internet_fallback=True,
                                    no_network_fallback=True,
                                    no_gui_fallback=True)
 
+    # TODO: move to __init__ after stable ovos-workshop release
     def initialize(self):
         if self.settings.get('use_geolocation'):
             LOG.debug(f"Geolocation update enabled")
             self.add_event("mycroft.ready", self._request_location_update,
                            once=True)
 
     def _request_location_update(self, _=None):
@@ -94,34 +95,34 @@
     def _handle_location_ipgeo_update(self, message):
         self._get_location.set()
         updated_location = message.data.get('location')
         if not updated_location:
             LOG.warning(f"No geolocation returned by plugin")
             return
         from neon_utils.user_utils import apply_local_user_profile_updates
-        from neon_utils.configuration_utils import get_neon_user_config
-        user_config = get_neon_user_config()
+        from neon_utils.configuration_utils import NGIConfig
+        user_config = NGIConfig("ngi_user_info")
         if not all((user_config['location']['lat'],
                     user_config['location']['lng'])):
             LOG.info(f'Updating default user config from ip geolocation')
             new_loc = {
                     'lat': str(updated_location['coordinate']['latitude']),
                     'lon': str(updated_location['coordinate']['longitude']),
                     'city': updated_location['city']['name'],
                     'state': updated_location['city']['state']['name'],
                     'country': updated_location['city']['state']['country']['name'],
                 }
             name, offset = self._get_timezone_from_location(new_loc)
             new_loc['lng'] = new_loc.pop('lon')
             new_loc['tz'] = name
             new_loc['utc'] = str(round(offset, 1))
-            apply_local_user_profile_updates({'location': new_loc},
-                                             get_neon_user_config())
+            apply_local_user_profile_updates({'location': new_loc}, user_config)
         else:
-            LOG.debug(f'Ignoring IP location for already defined user location')
+            LOG.debug(f'Ignoring IP location for already defined user location:'
+                      f'{user_config["location"]}')
         # Remove listener after a successful update
         self.remove_event('ovos.ipgeo.update.response')
 
     @property
     def stt_languages(self) -> Optional[set]:
         self._get_supported_languages()
         if not all((self._languages.skills, self._languages.stt)):
```

### Comparing `neon-skill-user_settings-0.5.2a2/neon_skill_user_settings.egg-info/PKG-INFO` & `neon-skill-user_settings-0.5.2a3/neon_skill_user_settings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-user-settings
-Version: 0.5.2a2
+Version: 0.5.2a3
 Home-page: https://github.com/NeonGeckoCom/skill-user_settings
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-user_settings-0.5.2a2/neon_skill_user_settings.egg-info/SOURCES.txt` & `neon-skill-user_settings-0.5.2a3/neon_skill_user_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-0.5.2a2/setup.py` & `neon-skill-user_settings-0.5.2a3/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-0.5.2a2/skill.json` & `neon-skill-user_settings-0.5.2a3/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-0.5.2a2/test/test_skill.py` & `neon-skill-user_settings-0.5.2a3/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-0.5.2a2/ui/SYSTEM_InputBox.qml` & `neon-skill-user_settings-0.5.2a3/ui/SYSTEM_InputBox.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-0.5.2a2/version.py` & `neon-skill-user_settings-0.5.2a3/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.5.2a2"
+__version__ = "0.5.2a3"
```

