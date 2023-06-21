# Comparing `tmp/acondbs-0.4.3.tar.gz` & `tmp/acondbs-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acondbs-0.4.3.tar", last modified: Tue Mar 15 14:05:16 2022, max compression
+gzip compressed data, was "acondbs-0.4.4.tar", last modified: Wed Jun 21 16:32:18 2023, max compression
```

## Comparing `acondbs-0.4.3.tar` & `acondbs-0.4.4.tar`

### file list

```diff
@@ -1,603 +1,557 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.184137 acondbs-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-03-15 14:05:05.000000 acondbs-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-03-15 14:05:05.000000 acondbs-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3570 2022-03-15 14:05:16.184137 acondbs-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2938 2022-03-15 14:05:05.000000 acondbs-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.184137 acondbs-0.4.3/acondbs/
--rw-r--r--   0 runner    (1001) docker     (121)     2444 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-03-15 14:05:16.184137 acondbs-0.4.3/acondbs/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.108137 acondbs-0.4.3/acondbs/auth/
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.108137 acondbs-0.4.3/acondbs/blueprint/
--rw-r--r--   0 runner    (1001) docker     (121)     4231 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/blueprint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.108137 acondbs-0.4.3/acondbs/blueprint/graphql_ide/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/blueprint/graphql_ide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3801 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/blueprint/graphql_ide/graphiql_newer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/blueprint/graphql_ide/graphql_playground.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.108137 acondbs-0.4.3/acondbs/db/
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3652 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/db/backup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/db/cmds.py
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/db/conn.py
--rw-r--r--   0 runner    (1001) docker     (121)     8520 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/db/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/db/sa.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.108137 acondbs-0.4.3/acondbs/github/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4481 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/github/call.py
--rw-r--r--   0 runner    (1001) docker     (121)     7528 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/github/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     5432 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/github/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.108137 acondbs-0.4.3/acondbs/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.116137 acondbs-0.4.3/acondbs/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/097c6676314c_change_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/0cce33011766_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/0f7fd06aa729_add_three_columns_to_product_relation_.py
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/0ff075f16b94_rename_column.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/12cc2bed191c_rename_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     5418 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/1583f2de9f39_add_attribute_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     2236 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/1f86dd56d829_copy_data_in_web_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5070 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/2910eaefa574_copy_to_attribute_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/2b15f740eed9_add_a_field_time_created_to_github_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/2ed9841987be_remove_columns_from_products.py
--rw-r--r--   0 runner    (1001) docker     (121)     7666 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/35e6ddccd22a_copy_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/3746a752f344_add_table_web_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/3f4e8bfd8a7f_add_column_reverse_type_id_to_product_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/3f6526e7e5ff_add_tables_github_.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/3f804a98ab06_add_table_log.py
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/41e5ff6f2878_add_attribute_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     5122 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/4398f463d243_delete_some_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/4c32365bb655_rename_a_column_name_in_account_admins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/4e8693037e72_add_fields_to_github_orgs_and_github_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/63033c01def0_add_fields_to_github_admin_app_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/63790f65e724_rename_table_web_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/6bd27755b1a8_remove_column_from_attribute_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/8585129ca524_make_login_unique_on_github_users.py
--rw-r--r--   0 runner    (1001) docker     (121)     5512 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/8e3f13ce98cb_make_nullable_false.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/919b1bc74839_add_a_field_git_hub_id_to_github_orgs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/936fc5b02f16_rename_the_table_github_accepted_orgs_.py
--rw-r--r--   0 runner    (1001) docker     (121)     3034 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/9495d7cb31ec_enter_data_to_field_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/9f22f713c4ea_add_a_field_git_hub_id_to_github_users.py
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/a4105346b478_change_column_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/aeec123e508c_make_fields_in_product_relations_non_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/babb78f6f6b3_add_fields_to_products.py
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/bad578ddbf3a_rename_the_table_github_admin_app_token_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/c090bba0e451_replace_date_with_data_time_in_products.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/c0d8d6a8f071_add_fields_to_github_users.py
--rw-r--r--   0 runner    (1001) docker     (121)     3382 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/cc64c8ef2115_re_initialize_migration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/ccd0df2c7da1_add_a_table_web_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     9090 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/cceebfa64b83_enter_data_in_attribute_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/ce157c2fa22e_constraint_on_product_relations.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/d5e539d43045_add_a_table_admin_app_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/d7cac99bbffa_add_columns_to_product_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/d8afc036053a_add_a_column_to_product_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/e077a31ad00b_add_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/e1d390d440d5_add_table_account_admins.py
--rw-r--r--   0 runner    (1001) docker     (121)     5035 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/e58cc402c887_add_column_to_attribute_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/e69be63fc3b8_remove_table_web_config_old.py
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/f84493df4297_update_type_field_association.py
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/f92f99aa6fdd_rename_the_table_admin_app_token_github_.py
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/migrations/versions/f97ed2cdfb29_add_column_on_type_field_association.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.116137 acondbs-0.4.3/acondbs/misc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5493 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/misc/cap.py
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/misc/gitb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/misc/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.116137 acondbs-0.4.3/acondbs/models/
--rw-r--r--   0 runner    (1001) docker     (121)     3416 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.116137 acondbs-0.4.3/acondbs/models/account/
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/account/account_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.116137 acondbs-0.4.3/acondbs/models/github/
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/github/github_org.py
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/github/github_org_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/github/github_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/github/github_user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.116137 acondbs-0.4.3/acondbs/models/misc/
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/misc/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.120137 acondbs-0.4.3/acondbs/models/product/
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/product/attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/product/field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/product/product.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/product/product_file_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     3628 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/product/product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/product/product_relation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/product/product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1820 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/product/type_field_association.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.120137 acondbs-0.4.3/acondbs/models/web/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/models/web/web_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.120137 acondbs-0.4.3/acondbs/ops/
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/ops/field.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/ops/log.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/ops/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7116 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/ops/product.py
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/ops/product_file_path.py
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/ops/product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/ops/product_relation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/ops/product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/ops/web_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.124137 acondbs-0.4.3/acondbs/schema/
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.124137 acondbs-0.4.3/acondbs/schema/auth/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/auth/query.py
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/filter_.py
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.124137 acondbs-0.4.3/acondbs/schema/github/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3025 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/github/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/github/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/github/type_.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.124137 acondbs-0.4.3/acondbs/schema/misc/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/misc/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/misc/query.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/misc/type_.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.124137 acondbs-0.4.3/acondbs/schema/product/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.124137 acondbs-0.4.3/acondbs/schema/product/mutation/
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/product/mutation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/product/mutation/field.py
--rw-r--r--   0 runner    (1001) docker     (121)     8122 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/product/mutation/product.py
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/product/mutation/product_file_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/product/mutation/product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3160 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/product/mutation/product_relation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     2799 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/product/mutation/product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     3423 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/product/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     6489 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/product/type_.py
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.128137 acondbs-0.4.3/acondbs/schema/web/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/web/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/web/query.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-03-15 14:05:05.000000 acondbs-0.4.3/acondbs/schema/web/type_.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.108137 acondbs-0.4.3/acondbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3570 2022-03-15 14:05:15.000000 acondbs-0.4.3/acondbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    23897 2022-03-15 14:05:15.000000 acondbs-0.4.3/acondbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 14:05:15.000000 acondbs-0.4.3/acondbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-03-15 14:05:15.000000 acondbs-0.4.3/acondbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-15 14:05:15.000000 acondbs-0.4.3/acondbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-03-15 14:05:16.184137 acondbs-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-03-15 14:05:05.000000 acondbs-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.100137 acondbs-0.4.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.128137 acondbs-0.4.3/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/auth/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/auth/test_get_token_from_http_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/auth/test_is_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/auth/test_is_signed_in.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.128137 acondbs-0.4.3/tests/blueprint/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/blueprint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.128137 acondbs-0.4.3/tests/blueprint/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/blueprint/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15315 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/blueprint/snapshots/snap_test_schema_based_on_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/blueprint/snapshots/snap_test_url_path_graphql.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/blueprint/test_graphiql.py
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/blueprint/test_schema_based_on_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/blueprint/test_url_path_graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.128137 acondbs-0.4.3/tests/db/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.132137 acondbs-0.4.3/tests/db/backup/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/backup/test_as_csv_to_github.py
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/backup/test_as_csv_to_github_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/backup/test_backup_db.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/backup/test_request_backup_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/backup/test_to_github.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.132137 acondbs-0.4.3/tests/db/ops/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.132137 acondbs-0.4.3/tests/db/ops/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20287 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/snapshots/snap_test_define_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)    16972 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/snapshots/snap_test_export_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)    17153 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/snapshots/snap_test_export_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)    16959 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/snapshots/snap_test_import_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/test_csv_specification.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/test_define_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/test_export_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/test_export_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     4725 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/test_import_convert_str.py
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/test_import_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/ops/test_import_csv_encrypted.py
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/test_cmds.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/test_db.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/db/test_sa.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.132137 acondbs-0.4.3/tests/github/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.132137 acondbs-0.4.3/tests/github/call/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/call/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.132137 acondbs-0.4.3/tests/github/call/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/call/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/call/snapshots/snap_test_call_graphql_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/call/snapshots/snap_test_exchange_code_for_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     3451 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/call/test_call_graphql_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/call/test_exchange_code_for_token.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.136137 acondbs-0.4.3/tests/github/ops/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/ops/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.136137 acondbs-0.4.3/tests/github/ops/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/ops/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/ops/snapshots/snap_test_exchange_code_for_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/ops/snapshots/snap_test_get_github_oauth_app_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/ops/test_exchange_code_for_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/ops/test_get_github_oauth_app_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/ops/test_get_user_for_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/ops/test_update_org_member_lists.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.136137 acondbs-0.4.3/tests/github/query/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/github/query/test_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.136137 acondbs-0.4.3/tests/misc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.136137 acondbs-0.4.3/tests/misc/gitb/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/misc/gitb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/misc/gitb/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/misc/gitb/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/misc/gitb/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (121)     1797 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/misc/gitb/test_push.py
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/misc/test_cap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/misc/test_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.136137 acondbs-0.4.3/tests/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.136137 acondbs-0.4.3/tests/models/account/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/account/test_account_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.140137 acondbs-0.4.3/tests/models/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/examples/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/examples/test_add.py
--rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/examples/test_date_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/examples/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     2285 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/examples/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.140137 acondbs-0.4.3/tests/models/funcs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/funcs/test_shorten.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.140137 acondbs-0.4.3/tests/models/github/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.140137 acondbs-0.4.3/tests/models/github/github_org/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/github/github_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/github/github_org/test_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.140137 acondbs-0.4.3/tests/models/github/github_org_membership/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/github/github_org_membership/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/github/github_org_membership/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/github/github_org_membership/test_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.140137 acondbs-0.4.3/tests/models/github/github_token/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/github/github_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/github/github_token/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2736 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/github/github_token/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.140137 acondbs-0.4.3/tests/models/github/github_user/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/github/github_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/github/github_user/test_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.140137 acondbs-0.4.3/tests/models/misc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.140137 acondbs-0.4.3/tests/models/misc/log/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/misc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/misc/log/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.140137 acondbs-0.4.3/tests/models/product/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.144137 acondbs-0.4.3/tests/models/product/attribute/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/attribute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3360 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/attribute/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    11628 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/attribute/test_attribute.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.144137 acondbs-0.4.3/tests/models/product/field/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/field/test_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/field/test_field_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.144137 acondbs-0.4.3/tests/models/product/product_relation_types/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relation_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relation_types/test_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relation_types/test_relations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.144137 acondbs-0.4.3/tests/models/product/product_relations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     8295 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relations/test_add_reverse_automatically.py
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relations/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (121)     7433 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relations/test_delete_cascade.py
--rw-r--r--   0 runner    (1001) docker     (121)     3509 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relations/test_delete_nullable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relations/test_example_how_to_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relations/test_relations.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_relations/test_repr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.144137 acondbs-0.4.3/tests/models/product/product_type/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/product_type/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.144137 acondbs-0.4.3/tests/models/product/products/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/products/test_products.py
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/test_product_file_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.144137 acondbs-0.4.3/tests/models/product/type_field_association/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/type_field_association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/type_field_association/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/product/type_field_association/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.144137 acondbs-0.4.3/tests/models/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/snapshots/snap_test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/test_add_owners.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.148137 acondbs-0.4.3/tests/models/web/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.148137 acondbs-0.4.3/tests/models/web/web_config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/web/web_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/models/web/web_config/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.148137 acondbs-0.4.3/tests/ops/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/ops/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/ops/test_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/ops/test_log.py
--rw-r--r--   0 runner    (1001) docker     (121)    14205 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/ops/test_product.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/ops/test_product_file_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/ops/test_product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3404 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/ops/test_product_relation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/ops/test_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/ops/test_web_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.148137 acondbs-0.4.3/tests/schema/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.148137 acondbs-0.4.3/tests/schema/auth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/auth/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.148137 acondbs-0.4.3/tests/schema/auth/query/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/auth/query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.152137 acondbs-0.4.3/tests/schema/auth/query/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/auth/query/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/auth/query/snapshots/snap_test_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/auth/query/snapshots/snap_test_is_signed_in.py
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/auth/query/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/auth/query/test_is_signed_in.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.152137 acondbs-0.4.3/tests/schema/github/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.152137 acondbs-0.4.3/tests/schema/github/mutation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/mutation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.152137 acondbs-0.4.3/tests/schema/github/mutation/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/mutation/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/mutation/snapshots/snap_test_add_git_hub_admin_app_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/mutation/snapshots/snap_test_delete_git_hub_admin_app_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/mutation/test_add_git_hub_admin_app_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/mutation/test_authenticate_with_git_hub.py
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/mutation/test_delete_git_hub_admin_app_token.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.152137 acondbs-0.4.3/tests/schema/github/query/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.152137 acondbs-0.4.3/tests/schema/github/query/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2183 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/snapshots/snap_test_all_git_hub_orgs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/snapshots/snap_test_all_git_hub_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     6344 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/snapshots/snap_test_all_git_hub_users.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/snapshots/snap_test_git_hub_o_auth_app_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/snapshots/snap_test_git_hub_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/test_all_git_hub_orgs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/test_all_git_hub_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/test_all_git_hub_users.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/test_git_hub_o_auth_app_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/github/query/test_git_hub_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.156137 acondbs-0.4.3/tests/schema/misc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.156137 acondbs-0.4.3/tests/schema/misc/gql/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.156137 acondbs-0.4.3/tests/schema/misc/gql/fragments/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/gql/fragments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/gql/fragments/fragment_log.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/gql/fragments/fragment_log_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.156137 acondbs-0.4.3/tests/schema/misc/gql/mutations/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/gql/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/gql/mutations/mutation_create_log.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/gql/mutations/mutation_delete_log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.156137 acondbs-0.4.3/tests/schema/misc/gql/queries/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/gql/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/gql/queries/query_all_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/gql/queries/query_log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.156137 acondbs-0.4.3/tests/schema/misc/mutation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/mutation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.156137 acondbs-0.4.3/tests/schema/misc/mutation/log/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/mutation/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/mutation/log/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.156137 acondbs-0.4.3/tests/schema/misc/mutation/log/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/mutation/log/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/mutation/log/snapshots/snap_test_create.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/mutation/log/snapshots/snap_test_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/mutation/log/test_create.py
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/mutation/log/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.156137 acondbs-0.4.3/tests/schema/misc/query/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.160137 acondbs-0.4.3/tests/schema/misc/query/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/query/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/query/snapshots/snap_test_all_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/query/snapshots/snap_test_log.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/query/test_all_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/misc/query/test_log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.160137 acondbs-0.4.3/tests/schema/product/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.160137 acondbs-0.4.3/tests/schema/product/gql/
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.160137 acondbs-0.4.3/tests/schema/product/gql/fragments/
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_field_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_product.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_product_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_product_connection_shallow.py
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_product_relation_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_product_relation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_product_relation_type_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_product_shallow.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_product_type_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.164137 acondbs-0.4.3/tests/schema/product/gql/mutations/
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_convert_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_create_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_create_product.py
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_create_product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_create_product_relation_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_create_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_delete_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_delete_product.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_delete_product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_delete_product_relation_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_delete_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_update_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_update_product.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_update_product_relation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/mutations/mutation_update_product_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.168137 acondbs-0.4.3/tests/schema/product/gql/queries/
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_all_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_all_product_file_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_all_product_relation_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_all_product_relation_types_total_count.py
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_all_product_relations.py
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_all_product_relations_total_count.py
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_all_product_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_all_products.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_all_products_shallow.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_all_products_total_count.py
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_product.py
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_product_relation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_product_shallow.py
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/gql/queries/query_product_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.168137 acondbs-0.4.3/tests/schema/product/mutation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.168137 acondbs-0.4.3/tests/schema/product/mutation/field/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/field/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.168137 acondbs-0.4.3/tests/schema/product/mutation/field/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/field/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3171 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/field/snapshots/snap_test_create_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/field/snapshots/snap_test_delete_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/field/snapshots/snap_test_update_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     2215 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/field/test_create_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/field/test_delete_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/field/test_update_field.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.168137 acondbs-0.4.3/tests/schema/product/mutation/product/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3427 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.168137 acondbs-0.4.3/tests/schema/product/mutation/product/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40255 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product/snapshots/snap_test_convert_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    40155 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product/snapshots/snap_test_create_product.py
--rw-r--r--   0 runner    (1001) docker     (121)     7328 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product/snapshots/snap_test_delete_product.py
--rw-r--r--   0 runner    (1001) docker     (121)    67687 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product/snapshots/snap_test_update_product.py
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product/test_convert_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     4302 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product/test_create_product.py
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product/test_delete_product.py
--rw-r--r--   0 runner    (1001) docker     (121)     4215 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product/test_update_product.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.172137 acondbs-0.4.3/tests/schema/product/mutation/product_file_path/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_file_path/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.172137 acondbs-0.4.3/tests/schema/product/mutation/product_file_path/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_file_path/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_file_path/snapshots/snap_test_create_product_file_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_file_path/snapshots/snap_test_delete_product_file_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_file_path/snapshots/snap_test_update_product_file_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     3103 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_file_path/test_create_product_file_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_file_path/test_delete_product_file_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_file_path/test_update_product_file_path.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.172137 acondbs-0.4.3/tests/schema/product/mutation/product_relation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.172137 acondbs-0.4.3/tests/schema/product/mutation/product_relation/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16918 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation/snapshots/snap_test_create_product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4777 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation/snapshots/snap_test_delete_product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2858 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation/test_create_product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation/test_delete_product_relation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.172137 acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.172137 acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27347 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/snapshots/snap_test_create_product_relation_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    17239 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/snapshots/snap_test_delete_product_relation_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    14309 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/snapshots/snap_test_update_product_relation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     3893 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/test_create_product_relation_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/test_delete_product_relation_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2239 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/test_update_product_relation_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.176137 acondbs-0.4.3/tests/schema/product/mutation/product_type/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_type/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.176137 acondbs-0.4.3/tests/schema/product/mutation/product_type/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_type/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    42894 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_type/snapshots/snap_test_create_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_type/snapshots/snap_test_delete_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    25853 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_type/snapshots/snap_test_update_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_type/test_create_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_type/test_delete_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     3463 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/mutation/product_type/test_update_product_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.176137 acondbs-0.4.3/tests/schema/product/query/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4342 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.180137 acondbs-0.4.3/tests/schema/product/query/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_all_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     2980 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_all_product_file_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     6341 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_all_product_relation_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4608 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_all_product_relations.py
--rw-r--r--   0 runner    (1001) docker     (121)     5852 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_all_product_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    37258 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_all_products.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     6755 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_product.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5601 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_product_relation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     7443 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_product_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/test_all_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/test_all_product_file_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/test_all_product_relation_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/test_all_product_relations.py
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/test_all_product_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/test_all_products.py
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/test_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/test_product.py
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/test_product_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/test_product_relation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/product/query/test_product_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.180137 acondbs-0.4.3/tests/schema/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/snapshots/snap_test_alembic_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/snapshots/snap_test_error.py
--rw-r--r--   0 runner    (1001) docker     (121)   158007 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/snapshots/snap_test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/test_alembic_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/test_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.180137 acondbs-0.4.3/tests/schema/web/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.180137 acondbs-0.4.3/tests/schema/web/gql/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.180137 acondbs-0.4.3/tests/schema/web/gql/mutations/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/gql/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/gql/mutations/mutation_save_web_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.180137 acondbs-0.4.3/tests/schema/web/gql/queries/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/gql/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/gql/queries/query_web_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.180137 acondbs-0.4.3/tests/schema/web/mutation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/mutation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.184137 acondbs-0.4.3/tests/schema/web/mutation/web_config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/mutation/web_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/mutation/web_config/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.184137 acondbs-0.4.3/tests/schema/web/mutation/web_config/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/mutation/web_config/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/mutation/web_config/snapshots/snap_test_save.py
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/mutation/web_config/test_save.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.184137 acondbs-0.4.3/tests/schema/web/query/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:16.184137 acondbs-0.4.3/tests/schema/web/query/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/query/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/query/snapshots/snap_test_web_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-03-15 14:05:05.000000 acondbs-0.4.3/tests/schema/web/query/test_web_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-03-15 14:05:05.000000 acondbs-0.4.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.385777 acondbs-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 16:32:08.000000 acondbs-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-21 16:32:08.000000 acondbs-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-21 16:32:18.385777 acondbs-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-21 16:32:08.000000 acondbs-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.385777 acondbs-0.4.4/acondbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 16:32:18.385777 acondbs-0.4.4/acondbs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.341775 acondbs-0.4.4/acondbs/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.341775 acondbs-0.4.4/acondbs/blueprint/
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/blueprint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.341775 acondbs-0.4.4/acondbs/blueprint/graphql_ide/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/blueprint/graphql_ide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/blueprint/graphql_ide/graphiql_newer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/blueprint/graphql_ide/graphql_playground.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.341775 acondbs-0.4.4/acondbs/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/db/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/db/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/db/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/db/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/db/sa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.345775 acondbs-0.4.4/acondbs/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/github/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/github/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/github/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.345775 acondbs-0.4.4/acondbs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/migrations/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.345775 acondbs-0.4.4/acondbs/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/migrations/versions/2023-06-14_14:41-2ed9841987be.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.345775 acondbs-0.4.4/acondbs/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/misc/cap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/misc/gitb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/misc/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.345775 acondbs-0.4.4/acondbs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.345775 acondbs-0.4.4/acondbs/models/account/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/account/account_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.345775 acondbs-0.4.4/acondbs/models/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/github/github_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/github/github_org_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/github/github_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/github/github_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.345775 acondbs-0.4.4/acondbs/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/misc/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.345775 acondbs-0.4.4/acondbs/models/product/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/product/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/product/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/product/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/product/product_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/product/product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/product/product_relation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/product/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/product/type_field_association.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.345775 acondbs-0.4.4/acondbs/models/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/models/web/web_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.349776 acondbs-0.4.4/acondbs/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/ops/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/ops/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/ops/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/ops/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/ops/product_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/ops/product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/ops/product_relation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/ops/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/ops/web_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.349776 acondbs-0.4.4/acondbs/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.349776 acondbs-0.4.4/acondbs/schema/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/auth/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/filter_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.349776 acondbs-0.4.4/acondbs/schema/github/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/github/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/github/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/github/type_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.349776 acondbs-0.4.4/acondbs/schema/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/misc/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/misc/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/misc/type_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.349776 acondbs-0.4.4/acondbs/schema/product/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.349776 acondbs-0.4.4/acondbs/schema/product/mutation/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/product/mutation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/product/mutation/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/product/mutation/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/product/mutation/product_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/product/mutation/product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/product/mutation/product_relation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/product/mutation/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/product/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/product/type_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.349776 acondbs-0.4.4/acondbs/schema/web/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/web/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/web/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-21 16:32:08.000000 acondbs-0.4.4/acondbs/schema/web/type_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.341775 acondbs-0.4.4/acondbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-21 16:32:18.000000 acondbs-0.4.4/acondbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-06-21 16:32:18.000000 acondbs-0.4.4/acondbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:32:18.000000 acondbs-0.4.4/acondbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-21 16:32:18.000000 acondbs-0.4.4/acondbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 16:32:18.000000 acondbs-0.4.4/acondbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-21 16:32:08.000000 acondbs-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-21 16:32:18.385777 acondbs-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-21 16:32:08.000000 acondbs-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.337775 acondbs-0.4.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.349776 acondbs-0.4.4/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/auth/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/auth/test_get_token_from_http_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/auth/test_is_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/auth/test_is_signed_in.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.349776 acondbs-0.4.4/tests/blueprint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/blueprint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.353776 acondbs-0.4.4/tests/blueprint/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/blueprint/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/blueprint/snapshots/snap_test_schema_based_on_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/blueprint/snapshots/snap_test_url_path_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/blueprint/test_graphiql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/blueprint/test_schema_based_on_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/blueprint/test_url_path_graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.353776 acondbs-0.4.4/tests/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.353776 acondbs-0.4.4/tests/db/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/backup/test_as_csv_to_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/backup/test_as_csv_to_github_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/backup/test_backup_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/backup/test_request_backup_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/backup/test_to_github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.353776 acondbs-0.4.4/tests/db/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.353776 acondbs-0.4.4/tests/db/ops/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20876 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/snapshots/snap_test_define_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/snapshots/snap_test_export_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/snapshots/snap_test_export_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16101 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/snapshots/snap_test_import_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/test_csv_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/test_define_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/test_export_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/test_export_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/test_import_convert_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/test_import_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/ops/test_import_csv_encrypted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/test_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/db/test_sa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.353776 acondbs-0.4.4/tests/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.353776 acondbs-0.4.4/tests/github/call/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/call/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.353776 acondbs-0.4.4/tests/github/call/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/call/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/call/snapshots/snap_test_call_graphql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/call/snapshots/snap_test_exchange_code_for_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/call/test_call_graphql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/call/test_exchange_code_for_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.353776 acondbs-0.4.4/tests/github/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/ops/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/github/ops/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/ops/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/ops/snapshots/snap_test_exchange_code_for_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/ops/snapshots/snap_test_get_github_oauth_app_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/ops/test_exchange_code_for_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/ops/test_get_github_oauth_app_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/ops/test_get_user_for_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/ops/test_update_org_member_lists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/github/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/github/query/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/misc/gitb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/misc/gitb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/misc/gitb/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/misc/gitb/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/misc/gitb/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/misc/gitb/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/misc/test_cap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/misc/test_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/account/test_account_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/examples/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/examples/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/examples/test_date_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/examples/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/examples/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/funcs/test_shorten.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/github/github_org/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/github/github_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/github/github_org/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/github/github_org_membership/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/github/github_org_membership/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/github/github_org_membership/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/github/github_org_membership/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/github/github_token/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/github/github_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/github/github_token/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/github/github_token/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/github/github_user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/github/github_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/github/github_user/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/misc/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/misc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/misc/log/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.357776 acondbs-0.4.4/tests/models/product/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.361776 acondbs-0.4.4/tests/models/product/attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/attribute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/attribute/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/attribute/test_attribute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.361776 acondbs-0.4.4/tests/models/product/field/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/field/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/field/test_field_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.361776 acondbs-0.4.4/tests/models/product/product_relation_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relation_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relation_types/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relation_types/test_relations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.361776 acondbs-0.4.4/tests/models/product/product_relations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relations/test_add_reverse_automatically.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relations/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relations/test_delete_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relations/test_delete_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relations/test_example_how_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relations/test_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_relations/test_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.361776 acondbs-0.4.4/tests/models/product/product_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/product_type/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.361776 acondbs-0.4.4/tests/models/product/products/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/products/test_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/test_product_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.361776 acondbs-0.4.4/tests/models/product/type_field_association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/type_field_association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/type_field_association/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/product/type_field_association/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.361776 acondbs-0.4.4/tests/models/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/snapshots/snap_test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/test_add_owners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.361776 acondbs-0.4.4/tests/models/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.361776 acondbs-0.4.4/tests/models/web/web_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/web/web_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/models/web/web_config/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.361776 acondbs-0.4.4/tests/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/ops/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/ops/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/ops/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/ops/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/ops/test_product_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/ops/test_product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/ops/test_product_relation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/ops/test_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/ops/test_web_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/auth/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/auth/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/auth/query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/auth/query/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/auth/query/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/auth/query/snapshots/snap_test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/auth/query/snapshots/snap_test_is_signed_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/auth/query/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/auth/query/test_is_signed_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/github/mutation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/mutation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/github/mutation/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/mutation/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/mutation/snapshots/snap_test_add_git_hub_admin_app_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/mutation/snapshots/snap_test_delete_git_hub_admin_app_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/mutation/test_add_git_hub_admin_app_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/mutation/test_authenticate_with_git_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/mutation/test_delete_git_hub_admin_app_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/github/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/github/query/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/snapshots/snap_test_all_git_hub_orgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/snapshots/snap_test_all_git_hub_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/snapshots/snap_test_all_git_hub_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/snapshots/snap_test_git_hub_o_auth_app_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/snapshots/snap_test_git_hub_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/test_all_git_hub_orgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/test_all_git_hub_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/test_all_git_hub_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/test_git_hub_o_auth_app_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/github/query/test_git_hub_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/misc/gql/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/misc/gql/fragments/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/gql/fragments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/gql/fragments/fragment_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/gql/fragments/fragment_log_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.365776 acondbs-0.4.4/tests/schema/misc/gql/mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/gql/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/gql/mutations/mutation_create_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/gql/mutations/mutation_delete_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.369776 acondbs-0.4.4/tests/schema/misc/gql/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/gql/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/gql/queries/query_all_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/gql/queries/query_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.369776 acondbs-0.4.4/tests/schema/misc/mutation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/mutation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.369776 acondbs-0.4.4/tests/schema/misc/mutation/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/mutation/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/mutation/log/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.369776 acondbs-0.4.4/tests/schema/misc/mutation/log/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/mutation/log/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/mutation/log/snapshots/snap_test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/mutation/log/snapshots/snap_test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/mutation/log/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/mutation/log/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.369776 acondbs-0.4.4/tests/schema/misc/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.369776 acondbs-0.4.4/tests/schema/misc/query/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/query/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/query/snapshots/snap_test_all_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/query/snapshots/snap_test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/query/test_all_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/misc/query/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.369776 acondbs-0.4.4/tests/schema/product/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.369776 acondbs-0.4.4/tests/schema/product/gql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.369776 acondbs-0.4.4/tests/schema/product/gql/fragments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_field_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_product_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_product_connection_shallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_product_relation_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_product_relation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_product_relation_type_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_product_shallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_product_type_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.373777 acondbs-0.4.4/tests/schema/product/gql/mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_convert_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_create_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_create_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_create_product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_create_product_relation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_create_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_delete_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_delete_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_delete_product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_delete_product_relation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_delete_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_update_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_update_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_update_product_relation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/mutations/mutation_update_product_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.373777 acondbs-0.4.4/tests/schema/product/gql/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_all_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_all_product_file_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_all_product_relation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_all_product_relation_types_total_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_all_product_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_all_product_relations_total_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_all_product_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_all_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_all_products_shallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_all_products_total_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_product_relation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_product_shallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/gql/queries/query_product_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.373777 acondbs-0.4.4/tests/schema/product/mutation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.373777 acondbs-0.4.4/tests/schema/product/mutation/field/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/field/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.373777 acondbs-0.4.4/tests/schema/product/mutation/field/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/field/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/field/snapshots/snap_test_create_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/field/snapshots/snap_test_delete_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/field/snapshots/snap_test_update_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/field/test_create_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/field/test_delete_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/field/test_update_field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.377777 acondbs-0.4.4/tests/schema/product/mutation/product/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.377777 acondbs-0.4.4/tests/schema/product/mutation/product/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33767 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product/snapshots/snap_test_convert_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25668 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product/snapshots/snap_test_create_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product/snapshots/snap_test_delete_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46273 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product/snapshots/snap_test_update_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product/test_convert_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product/test_create_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product/test_delete_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product/test_update_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.377777 acondbs-0.4.4/tests/schema/product/mutation/product_file_path/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_file_path/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.377777 acondbs-0.4.4/tests/schema/product/mutation/product_file_path/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_file_path/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_file_path/snapshots/snap_test_create_product_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_file_path/snapshots/snap_test_delete_product_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_file_path/snapshots/snap_test_update_product_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_file_path/test_create_product_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_file_path/test_delete_product_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_file_path/test_update_product_file_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.377777 acondbs-0.4.4/tests/schema/product/mutation/product_relation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.377777 acondbs-0.4.4/tests/schema/product/mutation/product_relation/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation/snapshots/snap_test_create_product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation/snapshots/snap_test_delete_product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation/test_create_product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation/test_delete_product_relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.377777 acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.377777 acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18460 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/snapshots/snap_test_create_product_relation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/snapshots/snap_test_delete_product_relation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/snapshots/snap_test_update_product_relation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/test_create_product_relation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/test_delete_product_relation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/test_update_product_relation_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.377777 acondbs-0.4.4/tests/schema/product/mutation/product_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_type/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.381777 acondbs-0.4.4/tests/schema/product/mutation/product_type/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_type/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34573 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_type/snapshots/snap_test_create_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_type/snapshots/snap_test_delete_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_type/snapshots/snap_test_update_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_type/test_create_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_type/test_delete_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/mutation/product_type/test_update_product_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.381777 acondbs-0.4.4/tests/schema/product/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.381777 acondbs-0.4.4/tests/schema/product/query/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_all_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_all_product_file_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_all_product_relation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_all_product_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_all_product_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30326 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_all_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_product_relation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/test_all_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/test_all_product_file_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/test_all_product_relation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/test_all_product_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/test_all_product_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/test_all_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/test_product_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/test_product_relation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/product/query/test_product_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.381777 acondbs-0.4.4/tests/schema/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/snapshots/snap_test_alembic_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/snapshots/snap_test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91443 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/snapshots/snap_test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/test_alembic_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.381777 acondbs-0.4.4/tests/schema/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.381777 acondbs-0.4.4/tests/schema/web/gql/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.381777 acondbs-0.4.4/tests/schema/web/gql/mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/gql/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/gql/mutations/mutation_save_web_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.381777 acondbs-0.4.4/tests/schema/web/gql/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/gql/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/gql/queries/query_web_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.381777 acondbs-0.4.4/tests/schema/web/mutation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/mutation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.385777 acondbs-0.4.4/tests/schema/web/mutation/web_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/mutation/web_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/mutation/web_config/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.385777 acondbs-0.4.4/tests/schema/web/mutation/web_config/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/mutation/web_config/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/mutation/web_config/snapshots/snap_test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/mutation/web_config/test_save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.385777 acondbs-0.4.4/tests/schema/web/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:18.385777 acondbs-0.4.4/tests/schema/web/query/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/query/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/query/snapshots/snap_test_web_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-21 16:32:08.000000 acondbs-0.4.4/tests/schema/web/query/test_web_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-21 16:32:08.000000 acondbs-0.4.4/versioneer.py
```

### Comparing `acondbs-0.4.3/LICENSE` & `acondbs-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.3/PKG-INFO` & `acondbs-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acondbs
-Version: 0.4.3
+Version: 0.4.4
 Summary: A GraphQL server for product DB
 Home-page: https://github.com/simonsobs/acondbs
 Author: Simons Observatory
 Author-email: so_software@simonsobservatory.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -67,15 +67,15 @@
 git clone git@github.com:TaiSakuma/acondbs-instance-example.git instance
 ```
 
 Set environmental variables
 
 ```bash
 export FLASK_APP="acondbs:create_app('$PWD/instance/config.py')"
-export FLASK_ENV=development
+export FLASK_DEBUG=1
 ```
 
 ### Initialize database
 
 ```bash
 flask init-db
 ```
```

### Comparing `acondbs-0.4.3/README.md` & `acondbs-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 git clone git@github.com:TaiSakuma/acondbs-instance-example.git instance
 ```
 
 Set environmental variables
 
 ```bash
 export FLASK_APP="acondbs:create_app('$PWD/instance/config.py')"
-export FLASK_ENV=development
+export FLASK_DEBUG=1
 ```
 
 ### Initialize database
 
 ```bash
 flask init-db
 ```
```

### Comparing `acondbs-0.4.3/acondbs/__init__.py` & `acondbs-0.4.4/acondbs/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 # 'attach_enctype_error_multidict' from partially initialized module
 # 'flask.debughelpers' (most likely due to a circular import)
 from flask import debughelpers  # noqa: F401
 
 from . import _warnings  # noqa: F401
 from . import _logging
 
-##__________________________________________________________________||
+
 DEFAULT_CONFIG_DICT = dict(
     SECRET_KEY="dev",
     SQLALCHEMY_DATABASE_URI="sqlite:///:memory:",
     SQLALCHEMY_TRACK_MODIFICATIONS=False,
 )
 
 
-##__________________________________________________________________||
 def create_app(config_path=None, **kwargs):
-
     _logging.configure_logging()
 
     app = Flask(__name__, instance_relative_config=False)
     app.config.from_mapping(**DEFAULT_CONFIG_DICT)
 
     if config_path is not None:
         config_path = Path(config_path)
@@ -61,24 +59,20 @@
 
     CORS(app, resources={r"/*": {"origins": "*"}})
 
     app.logger.info('"app" initialized')
     return app
 
 
-##__________________________________________________________________||
-
 from ._version import get_versions  # noqa: E402
 
 __version__ = get_versions()["version"]
 """str: version
 
 The version string, e.g., "0.1.2", "0.1.2+83.ga093a20.dirty".
 generated from git tags by versioneer.
 
 Versioneer: https://github.com/warner/python-versioneer
 
 """
 
 del get_versions
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/_logging.py` & `acondbs-0.4.4/acondbs/_logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Configure logging
 
 """
 import logging
 from logging.config import dictConfig
 from pathlib import Path
 
-##__________________________________________________________________||
 _module_path = Path(__file__).resolve().parent.parent
 # the path to the dir in which the module is installed,
 # i.e., the one dir above the module path.
 # e.g., /home/username/venv/lib/python3.8/site-packages
 
 # https://docs.python.org/3/library/logging.html#logrecord-objects
 _old_factory = logging.getLogRecordFactory()
@@ -24,26 +23,23 @@
     with
     "acondbs/schema/auth.py"
 
     """
 
     record = _old_factory(*args, **kwargs)
     try:
-        record.pathname = (
-            Path(record.pathname).resolve().relative_to(_module_path)
-        )
+        record.pathname = Path(record.pathname).resolve().relative_to(_module_path)
     except Exception:
         pass
     return record
 
 
 logging.setLogRecordFactory(record_factory)
 
 
-##__________________________________________________________________||
 def configure_logging():
     """configure logging
 
     This function needs to be called early in the program, i.e., in
     the beginning of create_app() before app.logger is accessed. (It
     seems fine to be called after "app" is created.)
 
@@ -68,15 +64,10 @@
             "handlers": {
                 "wsgi": {
                     "class": "logging.StreamHandler",
                     "stream": "ext://flask.logging.wsgi_errors_stream",
                     "formatter": "default",
                 }
             },
-            "loggers": {
-                logger_name: {"level": logger_level, "handlers": ["wsgi"]}
-            },
+            "loggers": {logger_name: {"level": logger_level, "handlers": ["wsgi"]}},
         }
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/_warnings.py` & `acondbs-0.4.4/acondbs/_warnings.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 https://docs.python.org/3/library/warnings.html
 
 """
 import warnings
 from pathlib import Path
 
-##__________________________________________________________________||
 _module_path = Path(__file__).resolve().parent.parent
 # the path to the dir in which the module is installed,
 # i.e., the one dir above the module path.
 
 
 def format(message, category, filename, lineno, file=None, line=None):
     try:
@@ -18,9 +17,7 @@
     except Exception:
         pass
     ret = "{}:{}: {}\n".format(filename, lineno, message)
     return ret
 
 
 warnings.formatwarning = format
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/auth/__init__.py` & `acondbs-0.4.4/acondbs/auth/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 from flask import request
 
-from ..models import (
-    GitHubToken,
-    GitHubUser,
-    AccountAdmin
-)
+from ..models import AccountAdmin, GitHubToken, GitHubUser
+
 
-##__________________________________________________________________||
 def is_signed_in():
-    """
-    """
+    """ """
     token = _get_token_from_http_headers()
     if not token:
         return False
 
     token_model = GitHubToken.query.filter_by(token=token).one_or_none()
     if not token_model:
         return False
 
     return True
 
-##__________________________________________________________________||
+
 def is_admin():
-    """
-    """
+    """ """
 
     if not is_signed_in():
         return False
 
     token = _get_token_from_http_headers()
     if not token:
         return False
 
-    user_model = GitHubUser.query.join(GitHubToken). \
-        filter(GitHubToken.token==token). \
-        one_or_none()
+    user_model = (
+        GitHubUser.query.join(GitHubToken)
+        .filter(GitHubToken.token == token)
+        .one_or_none()
+    )
 
     if not user_model:
         return False
 
-    admin_model = AccountAdmin.query. \
-        filter_by(git_hub_login=user_model.login). \
-        one_or_none()
+    admin_model = AccountAdmin.query.filter_by(
+        git_hub_login=user_model.login
+    ).one_or_none()
 
     if not admin_model:
         return False
 
     return True
 
-##__________________________________________________________________||
+
 def _get_token_from_http_headers():
     auth_header = request.headers.get('Authorization')
     # e.g., 'Bearer "xxxx"', "Bearer 'xxxx'",  or 'Bearer xxxx'
 
     if not auth_header:
         return None
 
     token = auth_header.split()[1].strip('"\'')
     # e.g., "xxxx"
 
     return token
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/blueprint/__init__.py` & `acondbs-0.4.4/acondbs/blueprint/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-import textwrap
 import json
+import textwrap
 import traceback
 
-from flask import Blueprint, current_app
+from flask import Blueprint, current_app, request
 from flask_graphql import GraphQLView
 
-from .. import auth, schema, ops
+from .. import auth, ops, schema
 from .graphql_ide import GRAPHIQL_NEWER, GRAPHQL_PLAYGROUND
 
-##__________________________________________________________________||
-from flask import request
-
 
 def format_to_str(data_dict):
-
     format_item = textwrap.dedent(
         """
         - {key}:
         {value}
         """
     ).lstrip()
 
@@ -124,24 +120,22 @@
                 "graphiql": current_app.config.get("ACONDBS_GRAPHIQL", False),
                 "graphiql_template": _select_graphiql_template(),
             }
         )
         super().__init__(**kwargs)
 
 
-##__________________________________________________________________||
 bp = Blueprint("graphql", __name__)
 bp.add_url_rule("/graphql", view_func=GraphQLViewW.as_view("graphql"))
 
 
 def init_app(app):
     app.register_blueprint(bp)
 
 
-##__________________________________________________________________||
 def _select_schema():
     if auth.is_admin():
         return schema.schema_admin
     elif auth.is_signed_in():
         return schema.schema_private
     else:
         return schema.schema_public
@@ -151,10 +145,7 @@
     template_no = current_app.config.get("ACONDBS_GRAPHIQL_TEMPLATE_NO", None)
     if template_no == 1:
         return GRAPHIQL_NEWER
     elif template_no == 2:
         return GRAPHQL_PLAYGROUND
     else:
         return None
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/blueprint/graphql_ide/graphiql_newer.py` & `acondbs-0.4.4/acondbs/blueprint/graphql_ide/graphiql_newer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-##__________________________________________________________________||
 # Based on https://github.com/graphql/graphiql/blob/codemirror-graphql@1.0.0/examples/graphiql-cdn/index.html
 # To obtain fetchURL, inserted the lines https://github.com/graphql-python/flask-graphql/blob/v2.0.1/flask_graphql/render_graphiql.py#L33-L64
 GRAPHIQL_NEWER = '''<!--
  *  Copyright (c) 2021 GraphQL Contributors
  *  All rights reserved.
  *
  *  This source code is licensed under the license found in the
@@ -116,9 +114,7 @@
           defaultVariableEditorOpen: true,
         }),
         document.getElementById('graphiql'),
       );
     </script>
   </body>
 </html>'''
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/blueprint/graphql_ide/graphql_playground.py` & `acondbs-0.4.4/acondbs/blueprint/graphql_ide/graphql_playground.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-##__________________________________________________________________||
 # From https://github.com/graphql/graphql-playground/blob/v1.8.10/packages/graphql-playground-html/minimal.html
 GRAPHQL_PLAYGROUND = '''<!DOCTYPE html>
 <html>
 
 <head>
   <meta charset=utf-8/>
   <meta name="viewport" content="user-scalable=no, initial-scale=1.0, minimum-scale=1.0, maximum-scale=1.0, minimal-ui">
@@ -54,9 +53,7 @@
       GraphQLPlayground.init(document.getElementById('root'), {
         // options as 'endpoint' belong here
       })
     })</script>
 </body>
 
 </html>'''
-
-##__________________________________________________________________||
```

#### html2text {}

```diff
@@ -1,8 +1,7 @@
-##__________________________________________________________________|| # From
-https://github.com/graphql/graphql-playground/blob/v1.8.10/packages/graphql-
-playground-html/minimal.html GRAPHQL_PLAYGROUND = '''
+# From https://github.com/graphql/graphql-playground/blob/v1.8.10/packages/
+graphql-playground-html/minimal.html GRAPHQL_PLAYGROUND = '''
 
 
 
 Loading GraphQL Playground
-''' ##__________________________________________________________________||
+'''
```

### Comparing `acondbs-0.4.3/acondbs/db/backup.py` & `acondbs-0.4.4/acondbs/db/backup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,101 +1,112 @@
 """Backup DB
 """
-from pathlib import Path
 import atexit
-import threading
 import subprocess
+import threading
 import warnings
+from pathlib import Path
 
 from flask import current_app
 
-from acondbs.misc.cap import cap_exec_rate
 from acondbs.db.ops import export_db_to_csv_files
-from acondbs.misc import gitb
-from acondbs.misc import lock
+from acondbs.misc import gitb, lock
+from acondbs.misc.cap import cap_exec_rate
+
 
-##__________________________________________________________________||
 def request_backup_db():
-    """reqeust to take a backup of the DB.
-    """
+    """reqeust to take a backup of the DB."""
     global _lock
     global _capped_backup_func
     with _lock:
         if not _capped_backup_func:
             pause = current_app.config['ACONDBS_DB_BACKUP_PAUSE']
             _capped_backup_func = cap_exec_rate(
-                func=run_flask_backup_db,
-                pause_time=pause, daemon=True)
-                # Need to set daemon=True. Otherwise
-                # threading waits for the thread to join
-                # before the function registered in atexist
-                # is executed.
+                func=run_flask_backup_db, pause_time=pause, daemon=True
+            )
+            # Need to set daemon=True. Otherwise
+            # threading waits for the thread to join
+            # before the function registered in atexist
+            # is executed.
     _capped_backup_func()
 
+
 _lock = threading.Lock()
 _capped_backup_func = None
 
-##__________________________________________________________________||
+
 def end_backup_thread():
     global _lock
     global _capped_backup_func
     with _lock:
         if _capped_backup_func:
             _capped_backup_func.end()
         _capped_backup_func = None
 
-import multiprocessing.queues # This import prevents the error described in
-                               # https://github.com/alphatwirl/atpbar/issues/4#issuecomment-473426630
+
+import multiprocessing.queues  # This import prevents the error described in
+
+# https://github.com/alphatwirl/atpbar/issues/4#issuecomment-473426630
 
 atexit.register(end_backup_thread)
 
-##__________________________________________________________________||
+
 def run_flask_backup_db():
     proc = subprocess.run(['flask', 'backup-db'])
 
-##__________________________________________________________________||
+
 def backup_db(exclude_csv=None):
     try:
         backup_db_to_github()
     except Exception as e:
         warnings.warn('An exception occurred in backup_db_to_github(): {}'.format(e))
 
     try:
         backup_db_as_csv_to_github(exclude=exclude_csv)
     except Exception as e:
-        warnings.warn('An exception occurred in backup_db_as_csv_to_github(): {}'.format(e))
+        warnings.warn(
+            'An exception occurred in backup_db_as_csv_to_github(): {}'.format(e)
+        )
+
 
-##__________________________________________________________________||
 def backup_db_to_github():
     repo_path = current_app.config['ACONDBS_DB_FOLDER']
     lock_path = current_app.config['ACONDBS_DB_BACKUP_LOCK']
     timeout = current_app.config['ACONDBS_DB_BACKUP_LOCK_TIMEOUT']
     try:
         with lock.lock(lock_path, timeout=timeout):
             backup_db_to_github_(repo_path)
     except lock.TimeOutAcquiringLock:
-        warnings.warn('Time out! unable to acquire the lock in {} seconds: {}'.format(timeout, lock_path))
+        warnings.warn(
+            'Time out! unable to acquire the lock in {} seconds: {}'.format(
+                timeout, lock_path
+            )
+        )
+
 
 def backup_db_to_github_(repo_path):
     gitb.commit(repo_path)
     gitb.push(repo_path)
 
-##__________________________________________________________________||
+
 def backup_db_as_csv_to_github(exclude=None):
     repo_path = current_app.config['ACONDBS_DB_BACKUP_CSV_GIT_FOLDER']
     lock_path = current_app.config['ACONDBS_DB_BACKUP_CSV_GIT_LOCK']
     timeout = current_app.config['ACONDBS_DB_BACKUP_CSV_GIT_LOCK_TIMEOUT']
     try:
         with lock.lock(lock_path, timeout=timeout):
             backup_db_as_csv_to_github_(repo_path, exclude)
     except lock.TimeOutAcquiringLock:
-        warnings.warn('Time out! unable to acquire the lock in {} seconds: {}'.format(timeout, lock_path))
+        warnings.warn(
+            'Time out! unable to acquire the lock in {} seconds: {}'.format(
+                timeout, lock_path
+            )
+        )
+
 
 def backup_db_as_csv_to_github_(repo_path, exclude=None):
     repo_path = Path(repo_path)
     for csv_file in repo_path.glob('*.csv'):
         csv_file.unlink()
     export_db_to_csv_files(repo_path, exclude)
     gitb.commit(repo_path)
     gitb.push(repo_path)
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/db/cmds.py` & `acondbs-0.4.4/acondbs/db/cmds.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 """Commands (click)
 
 """
-from flask.cli import with_appcontext
-import click
-
 import json
 
-from .ops import define_tables
-from .ops import export_db_to_dict_of_dict_list
-from .ops import import_tables_from_csv_files
-from .ops import export_db_to_csv_files
+import click
+from flask.cli import with_appcontext
+
 from .backup import backup_db
+from .ops import (
+    define_tables,
+    export_db_to_csv_files,
+    export_db_to_dict_of_dict_list,
+    import_tables_from_csv_files,
+)
 
 
-##__________________________________________________________________||
 @click.command("init-db")
 @with_appcontext
 def init_db_command():
     """Clear existing data and create new tables."""
     define_tables()
     click.echo("Initialized the database.")
 
 
-##__________________________________________________________________||
 @click.command("dump-db")
 @with_appcontext
 def dump_db_command():
     """Dump the DB contents"""
     db_content = export_db_to_dict_of_dict_list()
 
     click.echo(json.dumps(db_content, indent=2, default=str))
     # https://stackoverflow.com/questions/11875770/how-to-overcome-datetime-datetime-not-json-serializable
 
 
-##__________________________________________________________________||
 @click.command("import-csv")
 @click.argument("csvdir", type=click.Path(exists=True))
 @with_appcontext
 def import_csv_command(csvdir):
     """Import tables from CSV files in CSVDIR into the DB."""
     import_tables_from_csv_files(csvdir)
 
 
-##__________________________________________________________________||
 @click.command("export-csv")
 @click.argument("csvdir", type=click.Path())
 @with_appcontext
 def export_csv_command(csvdir):
     """Export the tables into the DB to CSV files in CSVDIR."""
     export_db_to_csv_files(csvdir)
 
 
-##__________________________________________________________________||
 DEFAULT_EXCLUDES = ("github_tokens", "account_admins", "log")
 
 
 @click.command("backup-db")
 @click.option(
     "--exclude-csv",
     "-e",
@@ -78,10 +75,7 @@
 def backup_db_command(exclude_csv, include_default_excludes):
     """Back up the DB and its content as CSV to GitHub"""
 
     exclude_csv = set(exclude_csv)
     if not include_default_excludes:
         exclude_csv |= set(DEFAULT_EXCLUDES)
     backup_db(exclude_csv)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/db/ops.py` & `acondbs-0.4.4/acondbs/db/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """DB operations
 
 The functions in this module need to be called within the application
 context of Flask unless stated otherwise.
 
 """
-import datetime
-import csv
 import ast
+import csv
+import datetime
 from pathlib import Path
 
 from sqlalchemy import MetaData
 from sqlalchemy.sql import sqltypes
 
-from .sa import sa
 from .conn import get_db_connection
+from .sa import sa
 
 
-##__________________________________________________________________||
 def define_tables():
     """Define DB tables from ORM models
 
     After dropping any existing tables, this function defines tables
     in the DB based on ORM models.
 
     """
@@ -55,15 +54,14 @@
     msg = f"Created tables: {tbl_names}"
 
     sa.Model.metadata.create_all(engine)
 
     print(msg)
 
 
-##__________________________________________________________________||
 def get_all_table_names():
     """returns the names of all tables in the DB.
 
     Returns
     -------
     list of str
         the names of all tables in the DB
@@ -139,15 +137,14 @@
     engine = sa.engine
     metadata = MetaData()
     metadata.reflect(bind=engine)
     tbl = metadata.tables[tbl_name]
     return engine.execute(tbl.select())
 
 
-##__________________________________________________________________||
 def import_tables_from_csv_files(csvdir):
     """imports tables from CSV files into the DB
 
     The tables need to be already defined in the DB.
 
     The folder `csvdir` should contain CSV files with the table
     contents to be imported: one CSV file for one table with the file
@@ -275,15 +272,14 @@
         try:
             return type_.python_type(ast.literal_eval(str_))
         except BaseException:
             return str_
     return None
 
 
-##__________________________________________________________________||
 def export_db_to_csv_files(outdir, exclude=None):
     """export all tables in the DB to CSV files
 
     The CSV files will be stored in the folder `csvdir`: one CSV file
     for one table with the file name <<table name>>.csv
 
     Parameters
@@ -323,10 +319,7 @@
     tbl_name : str
         the name of a table to be exported
     """
     result_proxy = get_resultproxy_of_select_all_rows(tbl_name)
     csv_writer = csv.writer(file_, lineterminator="\n")
     csv_writer.writerow(result_proxy.keys())
     csv_writer.writerows(result_proxy)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/db/sa.py` & `acondbs-0.4.4/acondbs/db/sa.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """the instance of SQLAlchemy from Flask-SQLAlchemy
 
 """
-from sqlalchemy import MetaData
 from flask_sqlalchemy import SQLAlchemy
+from sqlalchemy import MetaData
 
-##__________________________________________________________________||
 # https://flask-sqlalchemy.palletsprojects.com/en/2.x/config/#using-custom-metadata-and-naming-conventions
 # https://stackoverflow.com/a/56000475/7309855
 convention = {
     "ix": 'ix_%(column_0_label)s',
     "uq": "uq_%(table_name)s_%(column_0_name)s",
     # "ck": "ck_%(table_name)s_%(constraint_name)s",
     "ck": "ck_%(table_name)s_%(column_0_name)s",
     "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
-    "pk": "pk_%(table_name)s"
+    "pk": "pk_%(table_name)s",
 }
 metadata = MetaData(naming_convention=convention)
 
-##__________________________________________________________________||
+
 sa = SQLAlchemy(metadata=metadata)
 """the instance of SQLAlchemy from Flask-SQLAlchemy
 
 While the instance is named "sa" here, it is more commonly named "db"
 in example code found online.
 
 - API: https://flask-sqlalchemy.palletsprojects.com/en/2.x/api/#flask_sqlalchemy.SQLAlchemy
 - The difference from the plain SQLAlchemy:
   https://flask-sqlalchemy.palletsprojects.com/en/2.x/api/#flask_sqlalchemy.SQLAlchemy
 
 """
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/github/call.py` & `acondbs-0.4.4/acondbs/github/call.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """
 
 import requests
 
 API_URL = 'https://api.github.com/graphql'
 
-##__________________________________________________________________||
+
 def call_graphql_api(query, variables=None, token=None):
     """Call a GitHub GraphQL API
 
     Parameters
     ----------
     query : str
         A GraphQL query, e.g.,
@@ -35,31 +35,30 @@
     Exception
         If the query results include the field "errors" or don't include the
         field "data."
     """
 
     headers = {}
     if token:
-      headers['Authorization'] = 'token {}'.format(token)
+        headers['Authorization'] = 'token {}'.format(token)
 
-    json = {'query': query }
+    json = {'query': query}
     if variables:
         json['variables'] = variables
 
     # example:
     #   headers = {'Authorization': 'token XXXXXXXXXXXXXXXXXXXX'}
     #   json = {
     #       'query': (
     #           'query User($login: String!) '
     #           '{ user(login: $login) { name } }'
     #       ),
     #       'variables': {"login": "octocat"}
     #   }
 
-
     response = requests.post(API_URL, json=json, headers=headers)
     response = response.json()
     # examples:
     #   success:
     #     response = {"data": {"user": {"name": "The Octocat"} } }
     #
     #   error: (note: the 'data' field might not exist.)
@@ -78,22 +77,22 @@
     #   bad credentials:
     #     response = {
     #         'message': 'Bad credentials',
     #         'documentation_url': 'https://docs.github.com/graphql'
     #     }
 
     if 'errors' in response:
-      raise Exception(response['errors'])
+        raise Exception(response['errors'])
 
     if 'data' not in response:
-      raise Exception(response)
+        raise Exception(response)
 
     return response['data']
 
-##__________________________________________________________________||
+
 def exchange_code_for_token(code, token_url, client_id, client_secret, redirect_uri):
     """exchange a OAuth2 authorization code for an access token
 
     https://docs.github.com/en/free-pro-team@latest/developers/apps/authorizing-oauth-apps#2-users-are-redirected-back-to-your-site-by-github
 
     Parameters
     ----------
@@ -122,23 +121,23 @@
     """
 
     params = {
         'grant_type': 'authorization_code',
         'client_id': client_id,
         'client_secret': client_secret,
         'redirect_uri': redirect_uri,
-        'code': code
+        'code': code,
     }
 
     headers = {
         'Accept': "application/vnd.github.v3+json, application/json",
     }
 
     response = requests.post(token_url, json=params, headers=headers)
-    response = response.json() # dict
+    response = response.json()  # dict
     # examples:
     #   success:
     #     response = {'access_token': 'XXXXXXXXXXXXXXXXXXXX', 'token_type': 'bearer', 'scope': 'user'}
     #
     #   error:
     #     response = {
     #         'error': 'bad_verification_code',
@@ -146,9 +145,7 @@
     #         'error_uri': 'https://docs.github.com/apps/managing-oauth-apps/troubleshooting-oauth-app-access-token-request-errors/#bad-verification-code'
     #     }
 
     if 'access_token' not in response:
         raise Exception(response)
 
     return response
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/github/ops.py` & `acondbs-0.4.4/acondbs/github/ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Operations on DB
 """
 
 from flask import current_app
 
 from ..db.sa import sa
-
 from ..models import (
+    AccountAdmin,
     GitHubOrg,
-    GitHubUser,
-    GitHubToken,
     GitHubOrgMembership,
-    AccountAdmin
+    GitHubToken,
+    GitHubUser,
 )
-
 from . import call, query
 
-##__________________________________________________________________||
+
 def get_github_oauth_app_info():
     """Return GitHub OAuth App information
 
     Returns
     -------
     dict
         e.g.,
@@ -32,19 +30,19 @@
             }
     """
     ret = dict(
         authorize_url=current_app.config['GITHUB_AUTH_AUTHORIZE_URL'],
         token_url=current_app.config['GITHUB_AUTH_TOKEN_URL'],
         client_id=current_app.config['GITHUB_AUTH_CLIENT_ID'],
         client_secret=current_app.config['GITHUB_AUTH_CLIENT_SECRET'],
-        redirect_uri=current_app.config['GITHUB_AUTH_REDIRECT_URI']
+        redirect_uri=current_app.config['GITHUB_AUTH_REDIRECT_URI'],
     )
     return ret
 
-##__________________________________________________________________||
+
 def exchange_code_for_token(code):
     """Exchange an OAuth authentication code for a access token
 
     Parameters
     ----------
     code : str
         An OAuth authentication code, e.g, '7a31b6726dd2927b0af7'
@@ -62,18 +60,18 @@
     """
     oauth_app_info = get_github_oauth_app_info()
     return call.exchange_code_for_token(
         code,
         token_url=oauth_app_info['token_url'],
         client_id=oauth_app_info['client_id'],
         client_secret=current_app.config['GITHUB_AUTH_CLIENT_SECRET'],
-        redirect_uri=current_app.config['GITHUB_AUTH_REDIRECT_URI']
-        )
+        redirect_uri=current_app.config['GITHUB_AUTH_REDIRECT_URI'],
+    )
+
 
-##__________________________________________________________________||
 def add_org(login):
     if GitHubOrg.query.filter_by(login=login).one_or_none() is not None:
         raise Exception(f'already exists: {login}')
     if not (tokens := GitHubToken.query.all()):
         raise Exception('No tokens available.')
     r = None
     for token in tokens:
@@ -81,85 +79,98 @@
             r = query.org(login, token.token)
         except:
             continue
         break
     if r is None:
         raise Exception(f'Unable to find an org: {login}')
     model = GitHubOrg(
-        login=login,
-        git_hub_id=r['id'],
-        avatar_url=r['avatarUrl'],
-        url=r['url']
+        login=login, git_hub_id=r['id'], avatar_url=r['avatarUrl'], url=r['url']
     )
     sa.session.add(model)
     sa.session.commit()
     return model
 
+
 def delete_org(login):
     if (model := GitHubOrg.query.filter_by(login=login).one_or_none()) is None:
         raise Exception(f'does not exist: {login}')
     sa.session.delete(model)
     sa.session.commit()
 
-##__________________________________________________________________||
+
 def update_org_member_lists():
-    if not (tokens := GitHubToken.query.filter(GitHubToken.scope.like('%read:org%')).all()):
+    if not (
+        tokens := GitHubToken.query.filter(GitHubToken.scope.like('%read:org%')).all()
+    ):
         raise Exception('No tokens with relevant scopes available.')
     if not (orgs := GitHubOrg.query.all()):
         raise Exception('No orgs found.')
     with sa.session.no_autoflush:
         memberships = GitHubOrgMembership.query.all()
         for membership in memberships:
             sa.session.delete(membership)
         for org in orgs:
             edges = None
             for token in tokens:
                 try:
                     edges = query.org_members(org.login, token.token)
                 except Exception as exc:
                     import traceback
+
                     print(
                         "".join(
                             traceback.format_exception(
-                                type(exc), exc, exc.__traceback__)),)
+                                type(exc), exc, exc.__traceback__
+                            )
+                        ),
+                    )
                     continue
                 break
             if edges is None:
                 raise Exception(f'Unable to find an org: {org.login}')
             for edge in edges:
                 node = edge['node']
-                if (member := GitHubUser.query.filter_by(git_hub_id=node['id']).one_or_none()) is None:
-                    if (member := GitHubUser.query.filter_by(login=node['login']).one_or_none()) is None:
+                if (
+                    member := GitHubUser.query.filter_by(
+                        git_hub_id=node['id']
+                    ).one_or_none()
+                ) is None:
+                    if (
+                        member := GitHubUser.query.filter_by(
+                            login=node['login']
+                        ).one_or_none()
+                    ) is None:
                         member = GitHubUser(git_hub_id=node['id'])
                 member.login = node['login']
                 member.name = node['name']
                 member.avatar_url = node['avatarUrl']
                 member.url = node['url']
                 membership = GitHubOrgMembership(org=org, member=member)
                 sa.session.add(membership)
     sa.session.commit()
 
-##__________________________________________________________________||
+
 def store_token_for_code(code):
     token_dict = exchange_code_for_token(code)
     viewer = query.viewer(token_dict['access_token'])
-    if (user_model := GitHubUser.query.filter_by(git_hub_id=viewer['id']).one_or_none()) is None:
+    if (
+        user_model := GitHubUser.query.filter_by(git_hub_id=viewer['id']).one_or_none()
+    ) is None:
         user_model = GitHubUser(git_hub_id=viewer['id'])
     user_model.login = viewer['login']
     user_model.name = viewer['name']
     user_model.avatar_url = viewer['avatarUrl']
     user_model.url = viewer['url']
     token_model = GitHubToken(
-        token=token_dict['access_token'],
-        scope=token_dict['scope'],
-        user=user_model)
+        token=token_dict['access_token'], scope=token_dict['scope'], user=user_model
+    )
     sa.session.add(token_model)
     sa.session.commit()
 
-##__________________________________________________________________||
+
 def authenticate(code):
     """Authenticate a GitHub user with an OAuth authentication code
 
     This function authenticates a GitHub user with an OAuth
     authentication code. It also checks the membership of GitHub
     organizations and updates the DB.
 
@@ -183,39 +194,35 @@
     Exception
         If the authentication is unsuccessful.
 
     """
 
     token_dict = exchange_code_for_token(code)
     viewer = query.viewer(token_dict['access_token'])
-    account_admin_model = AccountAdmin.query.filter_by(git_hub_login=viewer['login']).one_or_none()
-    user_model= GitHubUser.query.filter_by(git_hub_id=viewer['id']).one_or_none()
+    account_admin_model = AccountAdmin.query.filter_by(
+        git_hub_login=viewer['login']
+    ).one_or_none()
+    user_model = GitHubUser.query.filter_by(git_hub_id=viewer['id']).one_or_none()
     if account_admin_model is None:
         if user_model is None:
             raise Exception(f'{viewer["login"]} is not a member.')
         if not user_model.memberships:
             raise Exception(f'{viewer["login"]} is not a member!')
     else:
         if user_model is None:
             user_model = GitHubUser(git_hub_id=viewer['id'])
     user_model.login = viewer['login']
     user_model.name = viewer['name']
     user_model.avatar_url = viewer['avatarUrl']
     user_model.url = viewer['url']
     token_model = GitHubToken(
-        token=token_dict['access_token'],
-        scope=token_dict['scope'],
-        user=user_model)
+        token=token_dict['access_token'], scope=token_dict['scope'], user=user_model
+    )
     sa.session.add(token_model)
     sa.session.commit()
     return token_dict
 
-##__________________________________________________________________||
+
 def get_user_for_token(token):
-    """
-    """
-    user = GitHubUser.query.join(GitHubToken). \
-        filter(GitHubToken.token==token). \
-        one()
+    """ """
+    user = GitHubUser.query.join(GitHubToken).filter(GitHubToken.token == token).one()
     return user
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/github/query.py` & `acondbs-0.4.4/acondbs/github/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Queries to GitHub API
 """
 
 import base64
 
 from .call import call_graphql_api
 
-##__________________________________________________________________||
+
 def org(login, token):
     query = """
       query Organization($login: String!) {
         organization(login: $login) {
           id
           login
           avatarUrl
           url
         }
       }
     """
-    variables = { "login": login }
+    variables = {"login": login}
     r = call_graphql_api(query=query, variables=variables, token=token)
     # e.g.,
     #   {
     #       "organization": {
     #           "id": "MDEyOk9yZ2FuaXphdGlvbjc1NjMxODQ0",
     #           "login": "urban-octo-disco",
     #           "avatarUrl": "https://avatars0.githubusercontent.com/u/75631844?v=4",
@@ -30,17 +30,16 @@
     #   }
 
     r['organization']['id'] = _decode_id(r['organization']['id'])
     # e.g., "012:Organization75631844"
 
     return r['organization']
 
-##__________________________________________________________________||
-def org_members(org_login, token):
 
+def org_members(org_login, token):
     first = 100
 
     query = """
       query OrganizationMembers($org_login: String!, $first: Int!, $after: String) {
         organization(login: $org_login) {
           login
           membersWithRole(first: $first, after: $after) {
@@ -111,15 +110,15 @@
         variables["after"] = pageInfo['endCursor']
 
     for e in edges:
         e['node']['id'] = _decode_id(e['node']['id'])
 
     return edges
 
-##__________________________________________________________________||
+
 def viewer(token):
     """Return info about the GitHub user for a token
 
     Parameters
     ----------
     token : str
         An access token, e.g, '4d5dc8b74eccdf65859d6ac64358a3a98300c351'
@@ -153,15 +152,15 @@
     viewer = r['viewer']
 
     viewer['id'] = _decode_id(viewer['id'])
     # e.g., '04:User583231'
 
     return viewer
 
-##__________________________________________________________________||
+
 def _decode_id(id_):
     """Decode a GitHub user or organization ID returned from GitHub GraphQL API
 
     Parameters
     ----------
     id_ : str
         An encoded GitHub user or GitHub organization ID returned from
@@ -173,10 +172,7 @@
         The decoded ID, e.g., "04:User583231", "012:Organization75631844"
 
     """
     try:
         return base64.b64decode(id_).decode()
     except BaseException:
         return f"raw:{id_}"
-
-##__________________________________________________________________||
-
```

### Comparing `acondbs-0.4.3/acondbs/migrations/README.md` & `acondbs-0.4.4/acondbs/migrations/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Example
 
 ```bash
 # cd to one dicrectory above this package, i.e., three directories above from here
 
 export FLASK_APP="acondbs:create_app('$PWD/acondbs/tests/sample/config.py')"
-export FLASK_ENV=development
+export FLASK_DEBUG=1
 
 cd acondbs/
 
 rm -f tests/sample/product.sqlite3
 
 flask db upgrade
```

### Comparing `acondbs-0.4.3/acondbs/migrations/alembic.ini` & `acondbs-0.4.4/acondbs/migrations/alembic.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # A generic, single database configuration.
 
 [alembic]
 # template used to generate migration files
 # file_template = %%(rev)s_%%(slug)s
+file_template = %%(year)d-%%(month).2d-%%(day).2d_%%(hour).2d:%%(minute).2d-%%(rev)s
 
 # set to 'true' to run the environment during
 # the 'revision' command, regardless of autogenerate
 # revision_environment = false
 
 
 # Logging configuration
```

### Comparing `acondbs-0.4.3/acondbs/migrations/env.py` & `acondbs-0.4.4/acondbs/migrations/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,19 @@
 logger = logging.getLogger('alembic.env')
 
 # add your model's MetaData object here
 # for 'autogenerate' support
 # from myapp import mymodel
 # target_metadata = mymodel.Base.metadata
 from flask import current_app
+
 config.set_main_option(
     'sqlalchemy.url',
-    str(current_app.extensions['migrate'].db.engine.url).replace('%', '%%'))
+    str(current_app.extensions['migrate'].db.engine.url).replace('%', '%%'),
+)
 target_metadata = current_app.extensions['migrate'].db.metadata
 
 # other values from the config, defined by the needs of env.py,
 # can be acquired:
 # my_important_option = config.get_main_option("my_important_option")
 # ... etc.
 
@@ -42,17 +44,15 @@
     we don't even need a DBAPI to be available.
 
     Calls to context.execute() here emit the given string to the
     script output.
 
     """
     url = config.get_main_option("sqlalchemy.url")
-    context.configure(
-        url=url, target_metadata=target_metadata, literal_binds=True
-    )
+    context.configure(url=url, target_metadata=target_metadata, literal_binds=True)
 
     with context.begin_transaction():
         context.run_migrations()
 
 
 def run_migrations_online():
     """Run migrations in 'online' mode.
@@ -78,17 +78,17 @@
         poolclass=pool.NullPool,
     )
 
     with connectable.connect() as connection:
         context.configure(
             connection=connection,
             target_metadata=target_metadata,
-            render_as_batch=True,
+            # render_as_batch=True,
             process_revision_directives=process_revision_directives,
-            **current_app.extensions['migrate'].configure_args
+            **current_app.extensions['migrate'].configure_args,
         )
 
         with context.begin_transaction():
             context.run_migrations()
 
 
 if context.is_offline_mode():
```

### Comparing `acondbs-0.4.3/acondbs/misc/cap.py` & `acondbs-0.4.4/acondbs/misc/cap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Throttle function executions
 """
-import threading
 import functools
 import queue
+import threading
 import time
 from enum import Enum
 
-##__________________________________________________________________||
+
 class cap_exec_rate:
     """cap the execution rate of a function
 
     This class prevents a function from being executed too often. This
     class executes a function in another thread. Once it executes a
     function, it starts a timer. If the function is called again
     through this class while the timer is still running, this class
@@ -37,23 +37,25 @@
         until the thread ends; the method `end()` needs to be called;
         the function will be executed one last time if it has been
         called but not executed. If `True`, the thread can be abruptly
         stopped at the end of Python program; the function that has
         been called but not executed will not be executed.
 
     """
+
     def __init__(self, func, pause_time=1.0, daemon=False):
         self.func = func
         self.pause_time = pause_time
         self.daemon = daemon
 
         self.queue = queue.Queue()
         config = Config(func, self.queue, pause_time)
         self.machine = threading.Thread(
-            target=state_machine, args=(config, ), daemon=daemon)
+            target=state_machine, args=(config,), daemon=daemon
+        )
         self.machine.start()
 
     def __call__(self):
         """call the function
 
         The number of executions of the function is capped
         """
@@ -66,111 +68,132 @@
         the timer. This method returns after the function is executed
         and the thread joins.
 
         """
         self.queue.put(Message.EXIT)
         self.machine.join()
 
+
 def state_machine(config):
-    """the entry function to be executed in a thread
-    """
+    """the entry function to be executed in a thread"""
     state = Active(config)
     while not state.end:
         state = state()
 
+
 class Message(Enum):
     FUNC_CALLED = 1
     TIMER_GOES_OFF = 2
     EXIT = 3
 
+
 class Config:
-    """Configuration of the state
-    """
+    """Configuration of the state"""
+
     def __init__(self, func, queue, pause_time):
         self.func = func
         self.queue = queue
         self.pause_time = pause_time
 
-##__________________________________________________________________||
+
 class State:
-    """The base class of the states
-    """
+    """The base class of the states"""
+
     def __init__(self, config):
         self.config = config
+
     def __call__(self):
         message = self.config.queue.get()
         if message == Message.FUNC_CALLED:
             return self.func_called()
         elif message == Message.TIMER_GOES_OFF:
             return self.timer_goes_off()
         elif message == Message.EXIT:
             return self.exit_()
         else:
             raise ValueError('unknown message: {!r}'.format(message))
 
+
 class Active(State):
     """Active state
 
     The timer is not running. The function can be executed immediately
     if it is called.
     """
+
     end = False
+
     def __init__(self, config):
         super().__init__(config)
+
     def func_called(self):
         self.config.func()
         return Pause(self.config)
+
     def exit_(self):
         return Exit(self.config)
 
+
 def timer_end(queue):
     queue.put(Message.TIMER_GOES_OFF)
 
+
 class Pause(State):
     """Pause state. The function has not been called
 
     The timer is running. The function has not been called. It won't
     be executed immediately when it is called.
     """
+
     end = False
+
     def __init__(self, config):
         super().__init__(config)
         self.timer = threading.Timer(
-            self.config.pause_time,
-            functools.partial(timer_end, self.config.queue))
+            self.config.pause_time, functools.partial(timer_end, self.config.queue)
+        )
         self.timer.start()
+
     def func_called(self):
         return PauseCalled(self.config, self.timer)
+
     def timer_goes_off(self):
         return Active(self.config)
+
     def exit_(self):
         self.timer.cancel()
         return Exit(self.config)
 
+
 class PauseCalled(State):
     """Pause state. The function has been called
 
     The timer is running. The function has been called. The function
     won't be executed until the timer goes off.
     """
+
     end = False
+
     def __init__(self, config, timer):
         super().__init__(config)
         self.timer = timer
+
     def func_called(self):
         return self
+
     def timer_goes_off(self):
         self.config.func()
         return Pause(self.config)
+
     def exit_(self):
         self.timer.cancel()
         self.config.func()
         return Exit(self.config)
 
+
 class Exit(State):
-    """Exit state
-    """
+    """Exit state"""
+
     end = True
+
     def __init__(self, config):
         super().__init__(config)
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/misc/gitb.py` & `acondbs-0.4.4/acondbs/misc/gitb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Git operations
 """
+import warnings
 from pathlib import Path
+
 import git
-import warnings
 
-##__________________________________________________________________||
+
 def commit(path, message=None):
     """commit all changes in a git repository to git
 
     If the path is not a git repository, unless it is empty, it will
     be initialized as a new repository.
 
     Parameters
@@ -47,15 +48,15 @@
 
     repo.git.add(A=True)
 
     if not message:
         message = 'commit all'
     repo.index.commit(message)
 
-##__________________________________________________________________||
+
 def pull(path):
     """pull from a tracking branch
 
     Equivalent to execute "git pull" in the path.
 
     Parameters
     ----------
@@ -88,15 +89,15 @@
 
     if not tracking_branch:
         raise ValueError("repo has no tracking branch: {}".format(path))
 
     remote = repo.remotes[tracking_branch.remote_name]
     remote.pull()
 
-##__________________________________________________________________||
+
 def push(path):
     """push to a upstream branch
 
     Equivalent to execute "git push" in the path.
 
     Parameters
     ----------
@@ -129,21 +130,19 @@
 
     if not tracking_branch:
         raise ValueError("repo has no tracking branch: {}".format(path))
 
     remote = repo.remotes[tracking_branch.remote_name]
     remote.push()
 
-##__________________________________________________________________||
+
 def is_git_repo(path):
     """test if a folder is a git repository
 
     copied from https://stackoverflow.com/a/39956572/7309855
 
     """
     try:
         _ = git.Repo(path).git_dir
         return True
     except git.exc.InvalidGitRepositoryError:
         return False
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/models/__init__.py` & `acondbs-0.4.4/acondbs/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 https://flask-sqlalchemy.palletsprojects.com/en/2.x/models/
 
 "Declare a Mapping" in SQLAlchemy doc:
 https://docs.sqlalchemy.org/en/14/orm/tutorial.html#declare-a-mapping
 
 """
 
-##__________________________________________________________________||
+
 from .product import (  # noqa: F401
     ProductType,
     Product,
     ProductFilePath,
     ProductRelationType,
     ProductRelation,
     AttributeUnicodeText,
@@ -42,15 +42,14 @@
 from .account import AccountAdmin  # noqa: F401
 
 from .web import WebConfig  # noqa: F401
 
 from .misc import Log  # noqa: F401
 
 
-##__________________________________________________________________||
 def init_app(app):
     """Initialize the Flask application object
 
     This function is called by `create_app()` of Flask
 
     Parameters
     ----------
@@ -58,64 +57,54 @@
         The Flask application object, an instance of `Flask`
     """
 
     _add_owners_to_db_as_admins(app)
     # remove_git_hub_tokens_with_invalid_decryption_key(app)
 
 
-##__________________________________________________________________||
 def _add_owners_to_db_as_admins(app):
     import sqlalchemy
     from ..db.sa import sa
 
     # Test if tables are defined. For example, tables are not defined
     # when a migration version is being created.
     with app.app_context():
         try:
             _ = AccountAdmin.query.all()
         except sqlalchemy.exc.OperationalError:
             return
 
     with app.app_context():
-
         owners = app.config.get("ACONDBS_OWNERS_GITHUB_LOGINS", "")
         # e.g., "octocat,dojocat"
 
         owners = {e.strip() for e in owners.split(",")}
         # e.g., {"octocat", "dojocat"}
 
         # remove empty strings
         owners = {e for e in owners if e}
 
         # sort so that "admin_id" is deterministic in tests
         owners = sorted(owners)
 
         for owner in owners:
             if (
-                admin := AccountAdmin.query.filter_by(
-                    git_hub_login=owner
-                ).one_or_none()
+                admin := AccountAdmin.query.filter_by(git_hub_login=owner).one_or_none()
             ) is None:
                 admin = AccountAdmin(git_hub_login=owner)
                 sa.session.add(admin)
         sa.session.commit()
 
 
-##__________________________________________________________________||
 def remove_git_hub_tokens_with_invalid_decryption_key(app):
     from ..db.sa import sa
 
     with app.app_context():
-        token_ids = [
-            e[0] for e in sa.session.query(GitHubToken.token_id).all()
-        ]
+        token_ids = [e[0] for e in sa.session.query(GitHubToken.token_id).all()]
         for token_id in token_ids:
             try:
                 token = GitHubToken.query.filter_by(  # noqa: F841
                     token_id=token_id
                 ).one()
             except ValueError:
                 sql = f"delete from {GitHubToken.__tablename__} where token_id={token_id};"
                 sa.engine.execute(sql)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/models/github/github_org_membership.py` & `acondbs-0.4.4/acondbs/models/github/github_org_membership.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from ...db.sa import sa
 
 
-##__________________________________________________________________||
 class GitHubOrgMembership(sa.Model):
     __tablename__ = "github_org_memberships"
     entry_id = sa.Column(sa.Integer(), primary_key=True)
     org_id = sa.Column(sa.ForeignKey("github_orgs.org_id"), nullable=False)
     org = sa.relationship(
         "GitHubOrg",
         backref=sa.backref("memberships", cascade="all"),
     )
-    member_id = sa.Column(
-        sa.ForeignKey("github_users.user_id"), nullable=False
-    )
+    member_id = sa.Column(sa.ForeignKey("github_users.user_id"), nullable=False)
     member = sa.relationship(
         "GitHubUser", backref=sa.backref("memberships", cascade="all")
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/models/github/github_token.py` & `acondbs-0.4.4/acondbs/models/github/github_token.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,18 @@
 from ...db.sa import sa
 
 
 def encription_key():
     return current_app.config["SECRET_KEY"]
 
 
-##__________________________________________________________________||
 class GitHubToken(sa.Model):
     __tablename__ = "github_tokens"
     token_id = sa.Column(sa.Integer(), primary_key=True)
     token = sa.Column(EncryptedType(sa.Text(), key=encription_key))
     scope = sa.Column(sa.Text())
     user_id = sa.Column(sa.ForeignKey("github_users.user_id"), nullable=False)
     user = sa.relationship(
         "GitHubUser",
         backref=sa.backref("tokens", cascade="all, delete-orphan"),
     )
-    time_created = sa.Column(
-        sa.DateTime(), default=lambda: datetime.datetime.now()
-    )
-
-
-##__________________________________________________________________||
+    time_created = sa.Column(sa.DateTime(), default=lambda: datetime.datetime.now())
```

### Comparing `acondbs-0.4.3/acondbs/models/product/__init__.py` & `acondbs-0.4.4/acondbs/models/product/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """declare ORM models for tables for products
 
 """
 
-##__________________________________________________________________||
+
 from .product_type import ProductType  # noqa: F401
 from .product import Product  # noqa: F401
 from .product_file_path import ProductFilePath  # noqa: F401
 from .product_relation_type import ProductRelationType  # noqa: F401
 from .product_relation import ProductRelation  # noqa: F401
 
 from .attribute import (  # noqa: F401
@@ -23,9 +23,7 @@
     FieldType,  # enum
     saEnumFieldType,  # SQLAlchemy Enum
     Field,
 )
 
 
 from .type_field_association import TypeFieldAssociation  # noqa: F401
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/models/product/attribute.py` & `acondbs-0.4.4/acondbs/models/product/attribute.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from sqlalchemy.orm import declared_attr
-from sqlalchemy.orm import declarative_mixin
+from sqlalchemy.orm import declarative_mixin, declared_attr
 
 from ...db.sa import sa
 
 
-##__________________________________________________________________||
 @declarative_mixin
 class AttributeBase:
     iid = sa.Column(sa.Integer(), primary_key=True)
 
     @declared_attr
     def product_id(self):
         return sa.Column(
@@ -62,27 +60,24 @@
                 self.backref_column,
                 cascade="all, delete-orphan",
             ),
         )
         # TODO: remove, replace with type_field_association
 
     def __repr__(self):
-        return (
-            f"<{self.__class__.__name__} {self.field_name!r}: {self.value!r}>"
-        )
+        return f"<{self.__class__.__name__} {self.field_name!r}: {self.value!r}>"
 
     @property
     def field_name(self):
         try:
             return self.field.name
         except BaseException:
             return self.field
 
 
-##__________________________________________________________________||
 class AttributeUnicodeText(AttributeBase, sa.Model):
     __tablename__ = "attribute_unicode_text"
     backref_column = "attributes_unicode_text"
     value = sa.Column(sa.UnicodeText())
 
 
 class AttributeBoolean(AttributeBase, sa.Model):
@@ -115,10 +110,7 @@
     value = sa.Column(sa.DateTime())
 
 
 class AttributeTime(AttributeBase, sa.Model):
     __tablename__ = "attribute_time"
     backref_column = "attributes_time"
     value = sa.Column(sa.Time())
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/models/product/field.py` & `acondbs-0.4.4/acondbs/models/product/field.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import enum
 
 from ...db.sa import sa
-
 from . import attribute
 
 
-##__________________________________________________________________||
 class FieldType(enum.Enum):
     # SQLAlchemy generic types: https://docs.sqlalchemy.org/en/14/core/type_basics.html#generic-types
     UnicodeText = 1
     Boolean = 2
     Integer = 3
     Float = 4
     Date = 5
@@ -47,10 +45,7 @@
     @property
     def type_name(self):
         # used in __repr__()
         try:
             return self.type_.name
         except BaseException:
             return self.type_
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/models/product/product.py` & `acondbs-0.4.4/acondbs/models/product/product.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 import datetime
 
 from ...db.sa import sa
 
 
-##__________________________________________________________________||
 class Product(sa.Model):
     # TODO: rename the class name to be more generic, e.g., "Entry"
     # TODO: use singular for the table name
     __tablename__ = "products"
     product_id = sa.Column(sa.Integer(), primary_key=True)
     type_id = sa.Column(sa.ForeignKey("product_types.type_id"), nullable=False)
     type_ = sa.relationship("ProductType", backref=sa.backref("products"))
     name = sa.Column(sa.Text(), nullable=False)
-    time_posted = sa.Column(
-        sa.DateTime(), default=lambda: datetime.datetime.now()
-    )
+    time_posted = sa.Column(sa.DateTime(), default=lambda: datetime.datetime.now())
     posting_git_hub_user_id = sa.Column(sa.ForeignKey("github_users.user_id"))
     posting_git_hub_user = sa.relationship(
         "GitHubUser",
         foreign_keys=[posting_git_hub_user_id],
         backref=sa.backref("posted_products", cascade="all"),
     )
     time_updated = sa.Column(sa.DateTime())
     updating_git_hub_user_id = sa.Column(sa.ForeignKey("github_users.user_id"))
     updating_git_hub_user = sa.relationship(
         "GitHubUser",
         foreign_keys=[updating_git_hub_user_id],
         backref=sa.backref("updated_products", cascade="all"),
     )
     note = sa.Column(sa.Text())
-    __table_args__ = (
-        sa.UniqueConstraint("type_id", "name", name="_type_id_name"),
-    )
+    __table_args__ = (sa.UniqueConstraint("type_id", "name", name="_type_id_name"),)
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {self.name!r}>"
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/models/product/product_relation.py` & `acondbs-0.4.4/acondbs/models/product/product_relation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-from ...db.sa import sa
-
 from sqlalchemy.event import listens_for
 
+from ...db.sa import sa
+
 
-##__________________________________________________________________||
 class ProductRelation(sa.Model):
     __tablename__ = "product_relations"
     relation_id = sa.Column(sa.Integer(), primary_key=True)
     type_id = sa.Column(
         sa.Integer(),
         sa.ForeignKey("product_relation_types.type_id"),
         nullable=False,
     )
-    type_ = sa.relationship(
-        "ProductRelationType", backref=sa.backref("relations")
-    )
+    type_ = sa.relationship("ProductRelationType", backref=sa.backref("relations"))
     self_product_id = sa.Column(
         sa.Integer(), sa.ForeignKey("products.product_id"), nullable=False
     )
     self_ = sa.relationship(
         "Product",
         foreign_keys=[self_product_id],
         backref=sa.backref("relations", cascade="all, delete-orphan"),
     )
     other_product_id = sa.Column(
         sa.Integer(), sa.ForeignKey("products.product_id"), nullable=False
     )
     other = sa.relationship("Product", foreign_keys=[other_product_id])
-    reverse_relation_id = sa.Column(
-        sa.ForeignKey("product_relations.relation_id")
-    )
+    reverse_relation_id = sa.Column(sa.ForeignKey("product_relations.relation_id"))
     reverse = sa.relationship(
         lambda: ProductRelation,
         uselist=False,
         foreign_keys=[reverse_relation_id],
         remote_side="ProductRelation.relation_id",
         cascade="all",
         post_update=True,
@@ -55,15 +50,14 @@
         # used in __repr__()
         try:
             return self.type_.name
         except BaseException:
             return self.type_
 
 
-##__________________________________________________________________||
 @listens_for(ProductRelation.type_, "set")
 def set_reverse_type(target, value, oldvalue, initiator):
     relation = target
 
     try:
         if relation.__avoid_recursive:
             return
@@ -121,10 +115,7 @@
     except Exception:
         pass
 
     if not relation.reverse.self_:
         relation.reverse.__avoid_recursive = True
         relation.reverse.self_ = value
         del relation.reverse.__avoid_recursive
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/models/product/product_relation_type.py` & `acondbs-0.4.4/acondbs/models/product/product_relation_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from ...db.sa import sa
-
 from sqlalchemy.event import listens_for
 
+from ...db.sa import sa
+
 
-##__________________________________________________________________||
 class ProductRelationType(sa.Model):
     __tablename__ = "product_relation_types"
     type_id = sa.Column(sa.Integer(), primary_key=True)
-    name = sa.Column(sa.Text(), nullable=False, unique=True, index=True)  # TODO: set unique False
-    reverse_type_id = sa.Column(
-        sa.ForeignKey("product_relation_types.type_id")
-    )
+    name = sa.Column(
+        sa.Text(), nullable=False, unique=True, index=True
+    )  # TODO: set unique False
+    reverse_type_id = sa.Column(sa.ForeignKey("product_relation_types.type_id"))
     reverse = sa.relationship(
         lambda: ProductRelationType,
         uselist=False,
         foreign_keys=[reverse_type_id],
         remote_side="ProductRelationType.type_id",
         cascade="all",
         post_update=True,
@@ -23,15 +22,14 @@
     singular = sa.Column(sa.Text())
     plural = sa.Column(sa.Text())
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {self.name!r}>"
 
 
-##__________________________________________________________________||
 @listens_for(ProductRelationType.reverse, "set")
 def set_reverse(target, value, oldvalue, initiator):
     """set the reciprocating reverse
 
     For example, if the reverse of the type1 is set type2,
        type1.reverse = type2
     this function sets the reverse of the type2 to type1,
@@ -51,10 +49,7 @@
     except Exception:
         pass
 
     if not type2.reverse:
         type2.__avoid_recursive = True
         type2.reverse = type1
         del type2.__avoid_recursive
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/models/product/type_field_association.py` & `acondbs-0.4.4/acondbs/models/product/type_field_association.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from ...db.sa import sa
 
 
-##__________________________________________________________________||
 class TypeFieldAssociation(sa.Model):
     """Many-to-many relation between ProductType and Field
 
 
     This class defines which fields each product type has.
 
     When a product type is deleted, all related instances of this
@@ -36,17 +35,15 @@
         backref=sa.backref("fields", cascade="all, delete-orphan"),
     )
     field = sa.relationship(
         "Field",
         backref=sa.backref("entry_types"),
     )
 
-    __table_args__ = (
-        sa.UniqueConstraint("type_id", "field_id", name="_type_field"),
-    )
+    __table_args__ = (sa.UniqueConstraint("type_id", "field_id", name="_type_field"),)
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {self.type_name!r} {self.field_name!r}>"
 
     @property
     def type_name(self):
         # used in __repr__()
@@ -58,10 +55,7 @@
     @property
     def field_name(self):
         # used in __repr__()
         try:
             return self.field.name
         except BaseException:
             return self.field
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/ops/field.py` & `acondbs-0.4.4/acondbs/ops/field.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from ..models import Field, FieldType
 from ..db.sa import sa
+from ..models import Field, FieldType
 
 
-##__________________________________________________________________||
 def create_field(name, type_, field_id=None):
     """Instantiate SQLAlchemy ORM model "Field"
 
     Parameters
     ----------
     name : str
         The name of the new field
@@ -61,10 +60,7 @@
     Returns
     -------
     None
 
     """
     model = Field.query.filter_by(field_id=field_id).one()
     sa.session.delete(model)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/ops/product.py` & `acondbs-0.4.4/acondbs/ops/product.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,50 @@
 import datetime
 
+from ..db.sa import sa
 from ..models import (
-    ProductType,
+    FieldType,
+    GitHubUser,
     Product,
     ProductFilePath,
     ProductRelation,
     ProductRelationType,
-    FieldType,
-    GitHubUser,
+    ProductType,
 )
 
-from ..db.sa import sa
 
-
-##__________________________________________________________________||
 def create_product(
     type_id,
     paths=None,
     relations=None,
     attributes=None,
     posting_git_hub_user_id=None,
-    **kwargs
+    **kwargs,
 ):
     """Create a product"""
 
     with sa.session.no_autoflush:
         return _create_product(
-            type_id,
-            paths,
-            relations,
-            attributes,
-            posting_git_hub_user_id,
-            **kwargs
+            type_id, paths, relations, attributes, posting_git_hub_user_id, **kwargs
         )
 
 
 def update_product(
     product_id,
     paths=None,
     relations=None,
     attributes=None,
     updating_git_hub_user_id=None,
-    **kwargs
+    **kwargs,
 ):
     """Update a product"""
 
     with sa.session.no_autoflush:
         return _update_product(
-            product_id,
-            paths,
-            relations,
-            attributes,
-            updating_git_hub_user_id,
-            **kwargs
+            product_id, paths, relations, attributes, updating_git_hub_user_id, **kwargs
         )
 
 
 def delete_product(product_id):
     """Delete a product"""
 
     model = Product.query.filter_by(product_id=product_id).one()
@@ -65,15 +53,14 @@
 
 
 def convert_product_type(product_id, type_id, updating_git_hub_user_id=None):
     with sa.session.no_autoflush:
         return _convert_product_type(product_id, type_id, updating_git_hub_user_id)
 
 
-##__________________________________________________________________||
 def uniq_preserving_order(list_):
     # https://stackoverflow.com/a/17016257/7309855
     return list(dict.fromkeys(list_))
 
 
 def _normalize_paths(paths):
     # e.g., paths = ["  /d/e ", " ", "/a/b/c", "/f/g", "/d/e"]
@@ -86,35 +73,30 @@
 
     ret = uniq_preserving_order(ret)
     # e.g., ["/d/e", "/a/b/c", "/f/g"]
 
     return ret
 
 
-##__________________________________________________________________||
 def _create_product(
     type_id, paths, relations, attributes, posting_git_hub_user_id, **kwargs
 ):
     product_type = ProductType.query.filter_by(type_id=type_id).one()
 
     model = Product(type_=product_type, **kwargs)
 
     if paths is not None:
         paths = _normalize_paths(paths)
         model.paths = [ProductFilePath(path=p) for p in paths]
 
     if relations is not None:
         model.relations = [
             ProductRelation(
-                type_=ProductRelationType.query.filter_by(
-                    type_id=r["type_id"]
-                ).one(),
-                other=Product.query.filter_by(
-                    product_id=r["product_id"]
-                ).one(),
+                type_=ProductRelationType.query.filter_by(type_id=r["type_id"]).one(),
+                other=Product.query.filter_by(product_id=r["product_id"]).one(),
             )
             for r in relations
         ]
 
     if attributes is None:
         attributes = {}
 
@@ -134,22 +116,16 @@
         ).one()
 
     sa.session.add(model)
     return model
 
 
 def _update_product(
-    product_id,
-    paths,
-    relations,
-    attributes,
-    updating_git_hub_user_id,
-    **kwargs
+    product_id, paths, relations, attributes, updating_git_hub_user_id, **kwargs
 ):
-
     model = Product.query.filter_by(product_id=product_id).one()
 
     if not attributes:
         attributes = {}
 
     # update paths
     if paths is not None:
@@ -190,22 +166,18 @@
 
     return model
 
 
 def _update_paths(old, input):
     input = _normalize_paths(input)
     path_dict = {p.path: p for p in old}
-    return [
-        path_dict[p] if p in path_dict else ProductFilePath(path=p)
-        for p in input
-    ]
+    return [path_dict[p] if p in path_dict else ProductFilePath(path=p) for p in input]
 
 
 def _update_relations(old, input):
-
     # sets of tuples (type_id, other_product_id) of ProductRelation
     new_ids = {(i["type_id"], i["product_id"]) for i in input}
     old_ids = {(r.type_id, r.other_product_id) for r in old}
 
     added_ids = new_ids - old_ids
 
     model_dict = {(r.type_id, r.other_product_id): r for r in old}
@@ -214,23 +186,21 @@
         type_ = ProductRelationType.query.filter_by(type_id=type_id).one()
         other = Product.query.filter_by(product_id=product_id).one()
         model_dict[id_] = ProductRelation(type_=type_, other=other)
 
     return [model_dict[i] for i in new_ids]
 
 
-##__________________________________________________________________||
 def _convert_product_type(product_id, type_id, updating_git_hub_user_id):
     model = Product.query.filter_by(product_id=product_id).one()
     product_type = ProductType.query.filter_by(type_id=type_id).one()
     model.type_ = product_type
 
     attr_names = [
-        a.attribute_class.backref_column
-        for a in FieldType.__members__.values()
+        a.attribute_class.backref_column for a in FieldType.__members__.values()
     ]
     # e.g., 'attributes_unicode_text', 'attributes_boolean'
 
     attrs = [e for attr in attr_names for e in getattr(model, attr)]
     # e.g., AttributeUnicodeText
 
     attr_dict = {a.field_id: a for a in attrs}
@@ -254,10 +224,7 @@
 
     model.time_updated = datetime.datetime.now()
     if updating_git_hub_user_id:
         GitHubUser.query.filter_by(user_id=updating_git_hub_user_id).one()
     model.updating_git_hub_user_id = updating_git_hub_user_id
 
     return model
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/ops/product_relation.py` & `acondbs-0.4.4/acondbs/ops/product_relation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-from ..models import (
-    Product,
-    ProductRelation,
-    ProductRelationType,
-)
-
 from ..db.sa import sa
+from ..models import Product, ProductRelation, ProductRelationType
 
 
 def create_product_relation(type_id, self_product_id, other_product_id, **kwargs):
     type_ = ProductRelationType.query.filter_by(type_id=type_id).one()
     self_ = Product.query.filter_by(product_id=self_product_id).one()
     other = Product.query.filter_by(product_id=other_product_id).one()
     model = ProductRelation(type_=type_, self_=self_, other=other, **kwargs)
```

### Comparing `acondbs-0.4.3/acondbs/ops/product_relation_type.py` & `acondbs-0.4.4/acondbs/ops/product_relation_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ..db.sa import sa
 from ..models import ProductRelationType
 
 
-##__________________________________________________________________||
 def create_product_relation_type(type_, reverse=None, self_reverse=False):
     """Create a product relation type"""
 
     if self_reverse and reverse:
         raise ValueError('"reverse" is given when "self_reverse" is True')
 
     if not (self_reverse or reverse):
@@ -30,10 +29,7 @@
     return model
 
 
 def delete_product_relation_type(type_id):
     """Delete a product relation type"""
     model = ProductRelationType.query.filter_by(type_id=type_id).one()
     sa.session.delete(model)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/ops/product_type.py` & `acondbs-0.4.4/acondbs/ops/product_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ..db.sa import sa
-from ..models import ProductType, Field, TypeFieldAssociation
+from ..models import Field, ProductType, TypeFieldAssociation
 
 
-##__________________________________________________________________||
 def create_product_type(field_ids=None, **kwargs):
     """Create a product type"""
     model = ProductType(**kwargs)
     if field_ids:
         with sa.session.no_autoflush:
             model.fields = _create_fields(field_ids)
     sa.session.add(model)
@@ -15,15 +14,14 @@
 
 def _create_fields(field_ids):
     ids = sorted(set(field_ids))
     fields_ = [Field.query.filter_by(field_id=i).one() for i in ids]
     return [TypeFieldAssociation(field=f) for f in fields_]
 
 
-##__________________________________________________________________||
 def update_product_type(type_id, field_ids=None, **kwargs):
     """Update a product type"""
 
     model = ProductType.query.filter_by(type_id=type_id).one()
 
     for k, v in kwargs.items():
         setattr(model, k, v)
@@ -32,15 +30,14 @@
         with sa.session.no_autoflush:
             model.fields = _update_fields(model.fields, field_ids)
 
     return model
 
 
 def _update_fields(old_fields: list, new_field_ids: list) -> list:
-
     new_ids = set(new_field_ids)
     old_ids = {f.field_id for f in old_fields}
 
     added_ids = new_ids - old_ids
 
     field_dict = {f.field_id: f for f in old_fields}
     #  {field_id: TypeFieldAssociation}
@@ -54,15 +51,11 @@
     # TypeFieldAssociation from the session by calling
     # sa.session.delete(). They will be automatically deleted because
     # of the cascade option of the relationship.
 
     return [field_dict[i] for i in sorted(new_ids)]
 
 
-##__________________________________________________________________||
 def delete_product_type(type_id):
     """Delete a product type"""
     model = ProductType.query.filter_by(type_id=type_id).one()
     sa.session.delete(model)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/__init__.py` & `acondbs-0.4.4/acondbs/schema/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,29 +7,26 @@
     auth,
     github,
     misc,
     product as p,
 )
 
 
-##__________________________________________________________________||
 class QueryPublic(graphene.ObjectType):
     web_config = web.query.web_config_field
     is_signed_in = auth.query.is_signed_in_field
     git_hub_o_auth_app_info = github.query.git_hub_o_auth_app_info_field
 
 
 class MutationPublic(graphene.ObjectType):
     authenticate_with_git_hub = github.mutation.AuthenticateWithGitHub.Field()
     create_log = misc.mutation.CreateLog.Field()
 
 
-##__________________________________________________________________||
 class QueryPrivate(QueryPublic):
-
     #
     version = version_.version_field
     alembic_version = version_.alembic_version_field
 
     node = relay.Node.Field()
 
     #
@@ -50,92 +47,74 @@
     product_relation = p.query.product_relation_field
     product_relation_type = p.query.product_relation_type_field
     product_type = p.query.product_type_field
     field = p.query.field_field
 
 
 class MutationPrivate(MutationPublic):
-
     #
     create_product = p.mutation.CreateProduct.Field()
     delete_product = p.mutation.DeleteProduct.Field()
     update_product = p.mutation.UpdateProduct.Field()
     convert_product_type = p.mutation.ConvertProductType.Field()
 
     create_product_file_path = p.mutation.CreateProductFilePath.Field()
     delete_product_file_path = p.mutation.DeleteProductFilePath.Field()
     update_product_file_path = p.mutation.UpdateProductFilePath.Field()
 
     create_product_relation = p.mutation.CreateProductRelation.Field()
     delete_product_relation = p.mutation.DeleteProductRelation.Field()
 
-    create_product_relation_types = (
-        p.mutation.CreateProductRelationTypes.Field()
-    )
-    delete_product_relation_types = (
-        p.mutation.DeleteProductRelationTypes.Field()
-    )
+    create_product_relation_types = p.mutation.CreateProductRelationTypes.Field()
+    delete_product_relation_types = p.mutation.DeleteProductRelationTypes.Field()
     update_product_relation_type = p.mutation.UpdateProductRelationType.Field()
 
     create_product_type = p.mutation.CreateProductType.Field()
     delete_product_type = p.mutation.DeleteProductType.Field()
     update_product_type = p.mutation.UpdateProductType.Field()
 
     create_field = p.mutation.CreateField.Field()
     delete_field = p.mutation.DeleteField.Field()
     update_field = p.mutation.UpdateField.Field()
 
 
-##__________________________________________________________________||
 class QueryAdmin(QueryPrivate):
-
     #
     all_git_hub_orgs = github.query.all_git_hub_orgs_field
     all_git_hub_tokens = github.query.all_git_hub_tokens_field
     all_git_hub_users = github.query.all_git_hub_users_field
 
     #
     all_logs = misc.query.all_logs_field
 
     #
     log = misc.query.log_field
 
 
 class MutationAdmin(MutationPrivate):
-
     #
     add_git_hub_org = github.mutation.AddGitHubOrg.Field()
     delete_git_hub_org = github.mutation.DeleteGitHubOrg.Field()
 
-    add_git_hub_admin_app_token = (
-        github.mutation.AddGitHubAdminAppToken.Field()
-    )
-    delete_git_hub_admin_app_token = (
-        github.mutation.DeleteGitHubAdminAppToken.Field()
-    )
-
-    update_git_hub_org_member_lists = (
-        github.mutation.UpdateGitHubOrgMemberLists.Field()
-    )
+    add_git_hub_admin_app_token = github.mutation.AddGitHubAdminAppToken.Field()
+    delete_git_hub_admin_app_token = github.mutation.DeleteGitHubAdminAppToken.Field()
+
+    update_git_hub_org_member_lists = github.mutation.UpdateGitHubOrgMemberLists.Field()
 
     delete_log = misc.mutation.DeleteLog.Field()
 
     save_web_config = web.mutation.SaveWebconfig.Field()
 
 
-##__________________________________________________________________||
 class Query(QueryAdmin):
     pass
 
 
 class Mutation(MutationAdmin):
     pass
 
 
-##__________________________________________________________________||
 schema_public = graphene.Schema(query=QueryPublic, mutation=MutationPublic)
 schema_private = graphene.Schema(query=QueryPrivate, mutation=MutationPrivate)
 schema_admin = graphene.Schema(query=QueryAdmin, mutation=MutationAdmin)
 
 schema = graphene.Schema(query=Query, mutation=Mutation)
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/connection.py` & `acondbs-0.4.4/acondbs/schema/connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from graphene import Int, NonNull
 from graphene.relay import Connection
 
 
-##__________________________________________________________________||
 class CountedConnection(Connection):
     """
 
     copied from https://github.com/graphql-python/graphene-sqlalchemy/issues/153#issuecomment-501949939
 
     """
 
@@ -20,10 +19,7 @@
         # `__init_subclass_with_meta__()`.
         abstract = True
 
     total_count = NonNull(Int)
 
     def resolve_total_count(self, info, **kwargs):
         return self.length
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/filter_.py` & `acondbs-0.4.4/acondbs/schema/filter_.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,28 +4,22 @@
 https://github.com/art1415926535/graphene-sqlalchemy-filter
 
 example:
 https://github.com/art1415926535/graphene-sqlalchemy-filter/blob/1.10.2/examples/clients_and_records/filters.py
 
 """
 import graphene
-from graphene_sqlalchemy_filter import (
-    FilterableConnectionField,
-    FilterSet,
-)
-
-from ..models import (
-    Product as ProductModel,
-    ProductType as ProductTypeModel,
-    GitHubToken as GitHubTokenModel,
-    GitHubUser as GitHubUserModel,
-)
+from graphene_sqlalchemy_filter import FilterableConnectionField, FilterSet
+
+from ..models import GitHubToken as GitHubTokenModel
+from ..models import GitHubUser as GitHubUserModel
+from ..models import Product as ProductModel
+from ..models import ProductType as ProductTypeModel
 
 
-##__________________________________________________________________||
 class ProductFilter(FilterSet):
     type_name = graphene.String()
 
     class Meta:
         model = ProductModel
         fields = {
             "type_id": [
@@ -44,43 +38,37 @@
 
 class ProductTypeFilter(FilterSet):
     class Meta:
         model = ProductTypeModel
         fields = {}
 
 
-##__________________________________________________________________||
 class GitHubTokenFilter(FilterSet):
     class Meta:
         model = GitHubTokenModel
         fields = {
             "scope": [
                 "ilike",
             ],
         }
 
 
-##__________________________________________________________________||
 class GitHubUserFilter(FilterSet):
     org_member = graphene.Boolean()
 
     class Meta:
         model = GitHubUserModel
         fields = {}
 
     @staticmethod
     def org_member_filter(info, query, value):
         filter_ = GitHubUserModel.memberships.any() if value else None
         return query, filter_
 
 
-##__________________________________________________________________||
 class PFilterableConnectionField(FilterableConnectionField):
     filters = {
         ProductModel: ProductFilter(),
         ProductTypeModel: ProductTypeFilter(),
         GitHubTokenModel: GitHubTokenFilter(),
         GitHubUserModel: GitHubUserFilter(),
     }
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/github/mutation.py` & `acondbs-0.4.4/acondbs/schema/github/mutation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 import graphene
 from graphql import GraphQLError
 
-from ...db.sa import sa
 from ...db.backup import request_backup_db
-
-from ...models import (
-    GitHubToken as GitHubTokenModel,
-)
+from ...db.sa import sa
 from ...github.ops import (
-    update_org_member_lists,
     add_org,
+    authenticate,
     delete_org,
     store_token_for_code,
-    authenticate,
+    update_org_member_lists,
 )
-
+from ...models import GitHubToken as GitHubTokenModel
 from . import type_
 
 
-##__________________________________________________________________||
 class AddGitHubOrg(graphene.Mutation):
     class Arguments:
         login = graphene.String(required=True)
 
     ok = graphene.Boolean()
     git_hub_org = graphene.Field(lambda: type_.GitHubOrg)
 
@@ -42,30 +37,28 @@
     def mutate(root, info, login):
         delete_org(login)
         ok = True
         # request_backup_db()
         return DeleteGitHubOrg(ok=ok)
 
 
-##__________________________________________________________________||
 class AuthenticateWithGitHub(graphene.Mutation):
     class Arguments:
         code = graphene.String(required=True)
 
     authPayload = graphene.Field(lambda: type_.AuthPayload)
 
     def mutate(root, info, code):
         token_dict = authenticate(code)
         if not token_dict:
             raise GraphQLError("Unsuccessful to obtain the token")
         authPayload = type_.AuthPayload(token=token_dict["access_token"])
         return AuthenticateWithGitHub(authPayload=authPayload)
 
 
-##__________________________________________________________________||
 class AddGitHubAdminAppToken(graphene.Mutation):
     """Add a token for a GitHub Admin App"""
 
     class Arguments:
         code = graphene.String(required=True)
 
     ok = graphene.Boolean()
@@ -73,15 +66,14 @@
     def mutate(root, info, code):
         store_token_for_code(code)
         ok = True
         request_backup_db()
         return AddGitHubAdminAppToken(ok=ok)
 
 
-##__________________________________________________________________||
 class DeleteGitHubAdminAppToken(graphene.Mutation):
     """Delete a token for a GitHub Admin App"""
 
     class Arguments:
         token_id = graphene.Int(required=True)
 
     ok = graphene.Boolean()
@@ -91,21 +83,17 @@
         sa.session.delete(model)
         sa.session.commit()
         ok = True
         request_backup_db()
         return DeleteGitHubAdminAppToken(ok=ok)
 
 
-##__________________________________________________________________||
 class UpdateGitHubOrgMemberLists(graphene.Mutation):
     """Update the member lists of GitHub organizations"""
 
     ok = graphene.Boolean()
 
     def mutate(root, info):
         update_org_member_lists()
         ok = True
         # request_backup_db()
         return UpdateGitHubOrgMemberLists(ok=ok)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/github/query.py` & `acondbs-0.4.4/acondbs/schema/github/query.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,32 @@
 import graphene
 
 from ...github.ops import get_github_oauth_app_info
-
-from ..funcs import get_git_hub_viewer_from_info
 from ..filter_ import PFilterableConnectionField
+from ..funcs import get_git_hub_viewer_from_info
 from . import type_
 
-##__________________________________________________________________||
 all_git_hub_orgs_field = PFilterableConnectionField(type_.GitHubOrg.connection)
-all_git_hub_users_field = PFilterableConnectionField(
-    type_.GitHubUser.connection
-)
-all_git_hub_tokens_field = PFilterableConnectionField(
-    type_.GitHubToken.connection
-)
+all_git_hub_users_field = PFilterableConnectionField(type_.GitHubUser.connection)
+all_git_hub_tokens_field = PFilterableConnectionField(type_.GitHubToken.connection)
 
 
-##__________________________________________________________________||
 def resolve_git_hub_o_auth_app_info(parent, info):
     info = get_github_oauth_app_info()
     return type_.GitHubOAuthAppInfo(
         client_id=info["client_id"],
         authorize_url=info["authorize_url"],
         redirect_uri=info["redirect_uri"],
     )
 
 
 git_hub_o_auth_app_info_field = graphene.Field(
     type_.GitHubOAuthAppInfo, resolver=resolve_git_hub_o_auth_app_info
 )
 
 
-##__________________________________________________________________||
 def resolve_git_hub_viewer(parent, info):
     user = get_git_hub_viewer_from_info(info)
     return user
 
 
-git_hub_viewer_field = graphene.Field(
-    type_.GitHubUser, resolver=resolve_git_hub_viewer
-)
-
-##__________________________________________________________________||
+git_hub_viewer_field = graphene.Field(type_.GitHubUser, resolver=resolve_git_hub_viewer)
```

### Comparing `acondbs-0.4.3/acondbs/schema/misc/mutation.py` & `acondbs-0.4.4/acondbs/schema/misc/mutation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import graphene
 
-from . import type_
-
 from ... import ops
+from . import type_
 
 
 class CreateLogInput(graphene.InputObjectType):
     """Input to createLog()"""
 
     id_ = graphene.Int()
     level = graphene.String(description="The log level")
```

### Comparing `acondbs-0.4.3/acondbs/schema/product/mutation/__init__.py` & `acondbs-0.4.4/acondbs/schema/product/mutation/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,23 @@
+from .field import CreateField, DeleteField, UpdateField  # noqa: F401
 from .product import (  # noqa: F401
+    ConvertProductType,
     CreateProduct,
-    UpdateProduct,
     DeleteProduct,
-    ConvertProductType,
+    UpdateProduct,
 )
 from .product_file_path import (  # noqa: F401
     CreateProductFilePath,
-    UpdateProductFilePath,
     DeleteProductFilePath,
+    UpdateProductFilePath,
 )
-from .product_type import (  # noqa: F401
-    CreateProductType,
-    UpdateProductType,
-    DeleteProductType,
-)
+from .product_relation import CreateProductRelation, DeleteProductRelation  # noqa: F401
 from .product_relation_type import (  # noqa: F401
     CreateProductRelationTypes,
-    UpdateProductRelationType,
     DeleteProductRelationTypes,
+    UpdateProductRelationType,
 )
-from .product_relation import (  # noqa: F401
-    CreateProductRelation,
-    DeleteProductRelation,
-)
-from .field import (  # noqa: F401
-    CreateField,
-    UpdateField,
-    DeleteField,
+from .product_type import (  # noqa: F401
+    CreateProductType,
+    DeleteProductType,
+    UpdateProductType,
 )
```

### Comparing `acondbs-0.4.3/acondbs/schema/product/mutation/field.py` & `acondbs-0.4.4/acondbs/schema/product/mutation/field.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import graphene
 
-from .. import type_
-
 from .... import ops
+from .. import type_
 
 
-##__________________________________________________________________||
 class CommonInputFields:
     name = graphene.String(
         required=True,
         description="The name of the field",
     )
 
 
 class CreateFieldInput(graphene.InputObjectType, CommonInputFields):
     """Input to createField()"""
+
     type_ = type_.FieldType()
 
 
 class UpdateFieldInput(graphene.InputObjectType, CommonInputFields):
     """Input to updateField()"""
 
 
-##__________________________________________________________________||
 class CreateField(graphene.Mutation):
     """Create a field"""
 
     class Arguments:
         input = CreateFieldInput(required=True)
 
     ok = graphene.Boolean()
@@ -66,10 +64,7 @@
     ok = graphene.Boolean()
 
     def mutate(root, info, field_id):
         ops.delete_field(field_id)
         ops.commit()
         ok = True
         return DeleteField(ok=ok)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/product/mutation/product.py` & `acondbs-0.4.4/acondbs/schema/product/mutation/product.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import graphene
 
+from .... import ops
 from ...funcs import get_git_hub_viewer_from_info
 from .. import type_
 
-from .... import ops
-
 
-##__________________________________________________________________||
 def _reshape_arg_attributes(attributes):
     ret = {e["field_id"]: e["value"] for t, v in attributes.items() for e in v}
     return ret
 
 
-##__________________________________________________________________||
 class RelationInputFields(graphene.InputObjectType):
     """A relation to another product"""
 
     product_id = graphene.Int(
         required=True,
         description="The product ID of the other product",
     )
@@ -164,39 +161,37 @@
     """Input to updateProduct()"""
 
     name = graphene.String(
         description="The name of the product",
     )
 
 
-##__________________________________________________________________||
 class CreateProduct(graphene.Mutation):
     """Create a product"""
 
     class Arguments:
         input = CreateProductInput(
             required=True,
             description="the input to createProduct()",
         )
 
     ok = graphene.Boolean()
     product = graphene.Field(lambda: type_.Product)
 
     def mutate(root, info, input):
-
         viewer = get_git_hub_viewer_from_info(info)
         posting_git_hub_user_id = viewer.user_id
 
         attributes = input.pop("attributes", {})
         attributes = _reshape_arg_attributes(attributes)
 
         model = ops.create_product(
             attributes=attributes,
             posting_git_hub_user_id=posting_git_hub_user_id,
-            **input
+            **input,
         )
 
         ops.commit()
         ok = True
         return CreateProduct(product=model, ok=ok)
 
 
@@ -218,26 +213,25 @@
             description="an input to updateProduct()",
         )
 
     ok = graphene.Boolean()
     product = graphene.Field(lambda: type_.Product)
 
     def mutate(root, info, product_id, input):
-
         viewer = get_git_hub_viewer_from_info(info)
         updating_git_hub_user_id = viewer.user_id
 
         attributes = input.pop("attributes", {})
         attributes = _reshape_arg_attributes(attributes)
 
         model = ops.update_product(
             product_id=product_id,
             attributes=attributes,
             updating_git_hub_user_id=updating_git_hub_user_id,
-            **input
+            **input,
         )
         ops.commit()
         ok = True
         return UpdateProduct(product=model, ok=ok)
 
 
 class DeleteProduct(graphene.Mutation):
@@ -254,15 +248,14 @@
     def mutate(root, info, product_id):
         ops.delete_product(product_id)
         ops.commit()
         ok = True
         return DeleteProduct(ok=ok)
 
 
-##__________________________________________________________________||
 class ConvertProductType(graphene.Mutation):
     """Convert the product type of a product"""
 
     class Arguments:
         product_id = graphene.Int(
             required=True,
             description="The productId of a product to be converted.",
@@ -282,10 +275,7 @@
             product_id,
             type_id,
             updating_git_hub_user_id=updating_git_hub_user_id,
         )
         ops.commit()
         ok = True
         return ConvertProductType(ok=ok, product=model)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/product/mutation/product_relation.py` & `acondbs-0.4.4/acondbs/schema/product/mutation/product_relation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import graphene
 
-from .. import type_
 from .... import ops
+from .. import type_
 
 
-##__________________________________________________________________||
 class CreateProductRelationInput(graphene.InputObjectType):
     """An input to createProductRelation()"""
 
     type_id = graphene.Int(
         required=True,
         description=(
             "The typeId of the product relation type of the relation "
@@ -19,15 +18,14 @@
         required=True, description=("The productId of the self product")
     )
     other_product_id = graphene.Int(
         required=True, description=("The productId of the other product")
     )
 
 
-##__________________________________________________________________||
 class CreateProductRelation(graphene.Mutation):
     """Add relations between two products. The arguments only specify the relation
     from one product to the other. The reverse relation will be also added.
 
     """
 
     class Arguments:
@@ -58,10 +56,7 @@
     ok = graphene.Boolean()
 
     def mutate(root, info, relation_id):
         ops.delete_product_relation(relation_id)
         ops.commit()
         ok = True
         return DeleteProductRelation(ok=ok)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/product/mutation/product_relation_type.py` & `acondbs-0.4.4/acondbs/schema/product/mutation/product_relation_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import graphene
 
-from .. import type_
-
 from .... import ops
+from .. import type_
 
 
-##__________________________________________________________________||
 class CommonInputFields:
     indef_article = graphene.String(
         description=(
             'The indefinite article placed before the singular noun "'
             'i.e., "a" or "an". '
         )
     )
@@ -17,31 +15,24 @@
         description=("The singular noun, the relation type name in singular.")
     )
     plural = graphene.String(
         description=("The plural noun, the relation type name in plural.")
     )
 
 
-class CreateProductRelationTypeInput(
-    graphene.InputObjectType, CommonInputFields
-):
+class CreateProductRelationTypeInput(graphene.InputObjectType, CommonInputFields):
     """An input to createProductRelationTypes()"""
 
-    name = graphene.String(
-        required=True, description=("The name of the relation type")
-    )
+    name = graphene.String(required=True, description=("The name of the relation type"))
 
 
-class UpdateProductRelationTypeInput(
-    graphene.InputObjectType, CommonInputFields
-):
+class UpdateProductRelationTypeInput(graphene.InputObjectType, CommonInputFields):
     """An input to updateProductRelationType()"""
 
 
-##__________________________________________________________________||
 class CreateProductRelationTypes(graphene.Mutation):
     """Create a pair of product relation types"""
 
     class Arguments:
         type = CreateProductRelationTypeInput(
             required=True, description=("A relation type")
         )
@@ -97,10 +88,7 @@
     ok = graphene.Boolean()
 
     def mutate(root, info, type_id):
         ops.delete_product_relation_type(type_id)
         ops.commit()
         ok = True
         return DeleteProductRelationTypes(ok=ok)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/product/mutation/product_type.py` & `acondbs-0.4.4/acondbs/schema/product/mutation/product_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import graphene
 
-from .. import type_
-
 from .... import ops
+from .. import type_
 
 
-##__________________________________________________________________||
 class CommonInputFields:
     order = graphene.Int(
         description=(
             "The order in which the type is displayed, for example, "
             "in navigation bars."
         )
     )
@@ -22,39 +20,31 @@
     singular = graphene.String(
         description=("The singular noun, the product type name in singular.")
     )
     plural = graphene.String(
         description=("The plural noun, the product type name in plural.")
     )
     icon = graphene.String(
-        description=(
-            "A name of the icon from https://materialdesignicons.com/"
-        )
-    )
-    field_ids = graphene.List(
-        graphene.Int,
-        description=("The field IDs")
+        description=("A name of the icon from https://materialdesignicons.com/")
     )
+    field_ids = graphene.List(graphene.Int, description=("The field IDs"))
 
 
 class CreateProductTypeInput(graphene.InputObjectType, CommonInputFields):
     """Input to createProductType()"""
 
-    name = graphene.String(
-        required=True, description="The name of the product type"
-    )
+    name = graphene.String(required=True, description="The name of the product type")
 
 
 class UpdateProductTypeInput(graphene.InputObjectType, CommonInputFields):
     """Input to updateProductType()"""
 
     name = graphene.String(description="The name of the product type")
 
 
-##__________________________________________________________________||
 class CreateProductType(graphene.Mutation):
     """Create a product type"""
 
     class Arguments:
         input = CreateProductTypeInput(required=True)
 
     ok = graphene.Boolean()
@@ -93,10 +83,7 @@
     ok = graphene.Boolean()
 
     def mutate(root, info, type_id):
         ops.delete_product_type(type_id)
         ops.commit()
         ok = True
         return DeleteProductType(ok=ok)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/product/query.py` & `acondbs-0.4.4/acondbs/schema/product/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 import graphene
 
-from ...models import (
-    Product as ProductModel,
-    ProductType as ProductTypeModel,
-    ProductRelation as ProductRelationModel,
-    ProductRelationType as ProductRelationTypeModel,
-    Field as FieldModel,
-)
-
+from ...models import Field as FieldModel
+from ...models import Product as ProductModel
+from ...models import ProductRelation as ProductRelationModel
+from ...models import ProductRelationType as ProductRelationTypeModel
+from ...models import ProductType as ProductTypeModel
 from ..filter_ import PFilterableConnectionField
 from . import type_
 
-##__________________________________________________________________||
 all_products_field = PFilterableConnectionField(type_.Product.connection)
 all_product_types_field = PFilterableConnectionField(type_.ProductType.connection)  # fmt: skip
 all_product_relations_field = PFilterableConnectionField(type_.ProductRelation.connection)  # fmt: skip
 all_product_relation_types_field = PFilterableConnectionField(type_.ProductRelationType.connection)  # fmt: skip
 all_product_file_paths_field = PFilterableConnectionField(type_.ProductFilePath.connection)  # fmt: skip
 all_fields_field = PFilterableConnectionField(type_.Field.connection)
 
 
-##__________________________________________________________________||
 def resolve_product(parent, info, **kwargs):
-
     filter = [getattr(ProductModel, k) == v for k, v in kwargs.items()]
     # e.g., [ProductModel.type_id == 1, ProductModel.name == 'map_001']
 
     return type_.Product.get_query(info).filter(*filter).one_or_none()
 
 
 product_field = graphene.Field(
@@ -34,15 +28,14 @@
     product_id=graphene.Int(),
     type_id=graphene.Int(),
     name=graphene.String(),
     resolver=resolve_product,
 )
 
 
-##__________________________________________________________________||
 def resolve_product_type(parent, info, **kwargs):
     filter = [getattr(ProductTypeModel, k) == v for k, v in kwargs.items()]
     # e.g., [ProductTypeModel.type_id == 1, ProductTypeModel.name == 'map']
 
     return type_.ProductType.get_query(info).filter(*filter).one_or_none()
 
 
@@ -50,56 +43,45 @@
     type_.ProductType,
     type_id=graphene.Int(),
     name=graphene.String(),
     resolver=resolve_product_type,
 )
 
 
-##__________________________________________________________________||
 def resolve_product_relation(parent, info, **kwargs):
     filter = [getattr(ProductRelationModel, k) == v for k, v in kwargs.items()]
     return type_.ProductRelation.get_query(info).filter(*filter).one_or_none()
 
 
 product_relation_field = graphene.Field(
     type_.ProductRelation,
     relation_id=graphene.Int(),
     resolver=resolve_product_relation,
 )
 
 
-##__________________________________________________________________||
 def resolve_product_relation_type(parent, info, **kwargs):
-    filter = [
-        getattr(ProductRelationTypeModel, k) == v for k, v in kwargs.items()
-    ]
-    return (
-        type_.ProductRelationType.get_query(info).filter(*filter).one_or_none()
-    )
+    filter = [getattr(ProductRelationTypeModel, k) == v for k, v in kwargs.items()]
+    return type_.ProductRelationType.get_query(info).filter(*filter).one_or_none()
 
 
 product_relation_type_field = graphene.Field(
     type_.ProductRelationType,
     type_id=graphene.Int(),
     name=graphene.String(),
     resolver=resolve_product_relation_type,
 )
 
 
-##__________________________________________________________________||
 def resolve_field(parent, info, **kwargs):
-
     filter = [getattr(FieldModel, k) == v for k, v in kwargs.items()]
     # e.g., [FieldModel.field_id == 1, FieldModel.name == 'contact']
 
     return type_.Field.get_query(info).filter(*filter).one_or_none()
 
 
 field_field = graphene.Field(
     type_.Field,
     field_id=graphene.Int(),
     name=graphene.String(),
     resolver=resolve_field,
 )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/product/type_.py` & `acondbs-0.4.4/acondbs/schema/product/type_.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 )
 from ..filter_ import PFilterableConnectionField
 
 
 from graphene_sqlalchemy.enums import _convert_sa_to_graphene_enum
 
 
-##__________________________________________________________________||
 # FieldType is an enum. It is manually converted to a graphene enum
 # here. An enum will be usually automatically converted. However, the
 # automatic conversion causes an error if the automatic conversion
 # of the same enum happens multiple times as described in
 # https://github.com/graphql-python/graphene-sqlalchemy/issues/211.
 
 # It is possible to use graphene.Enum.from_enum() as
@@ -39,66 +38,60 @@
 
 # However, instead, a private function _convert_sa_to_graphene_enum()
 # is used here because this function desirably converts field names to
 # the upper case, e.g., "UnicodeText" to "UNICODE_TEXT"
 FieldType = _convert_sa_to_graphene_enum(saEnumFieldType)
 
 
-##__________________________________________________________________||
 class Product(SQLAlchemyObjectType):
     class Meta:
         model = ProductModel
         interfaces = (relay.Node,)
         connection_class = CountedConnection
         connection_field_factory = PFilterableConnectionField.factory
 
 
-##__________________________________________________________________||
 class ProductType(SQLAlchemyObjectType):
     """A product type"""
 
     class Meta:
         model = ProductTypeModel
         interfaces = (graphene.relay.Node,)
         connection_class = CountedConnection
         connection_field_factory = PFilterableConnectionField.factory
 
 
-##__________________________________________________________________||
 class ProductRelation(SQLAlchemyObjectType):
     """A relation from one product to another"""
 
     class Meta:
         model = ProductRelationModel
         interfaces = (graphene.relay.Node,)
         connection_class = CountedConnection
         connection_field_factory = PFilterableConnectionField.factory
 
 
-##__________________________________________________________________||
 class ProductRelationType(SQLAlchemyObjectType):
     """A type of relations between products"""
 
     class Meta:
         model = ProductRelationTypeModel
         interfaces = (graphene.relay.Node,)
         connection_class = CountedConnection
         connection_field_factory = PFilterableConnectionField.factory
 
 
-##__________________________________________________________________||
 class ProductFilePath(SQLAlchemyObjectType):
     class Meta:
         model = ProductFilePathModel
         interfaces = (relay.Node,)
         connection_class = CountedConnection
         connection_field_factory = PFilterableConnectionField.factory
 
 
-##__________________________________________________________________||
 class Field(SQLAlchemyObjectType):
     class Meta:
         model = FieldModel
         interfaces = (relay.Node,)
         connection_class = CountedConnection
         connection_field_factory = PFilterableConnectionField.factory
         exclude_fields = ("type_",)
@@ -182,10 +175,7 @@
     """A time attribute of a product"""
 
     class Meta:
         model = AttributeTimeModel
         interfaces = (relay.Node,)
         connection_class = CountedConnection
         connection_field_factory = PFilterableConnectionField.factory
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs/schema/version.py` & `acondbs-0.4.4/acondbs/schema/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 import graphene
-
 from alembic.migration import MigrationContext
 
 from ..db.conn import get_db_connection
 
 
-##__________________________________________________________________||
 def resolve_version(parent, info):
     from .. import __version__
 
     return __version__
 
 
 version_field = graphene.Field(
     graphene.String,
     description="The version of Acondbs",
     resolver=resolve_version,
 )
 
 
-##__________________________________________________________________||
 def resolve_alembic_version(parent, info):
     conn = get_db_connection()
     context = MigrationContext.configure(conn)
     ret = context.get_current_revision()
     # e.g., "35e6ddccd22a"
     return ret
 
 
 alembic_version_field = graphene.Field(
     graphene.String,
     description="The version of Alembic migration",
     resolver=resolve_alembic_version,
 )
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/acondbs.egg-info/PKG-INFO` & `acondbs-0.4.4/acondbs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acondbs
-Version: 0.4.3
+Version: 0.4.4
 Summary: A GraphQL server for product DB
 Home-page: https://github.com/simonsobs/acondbs
 Author: Simons Observatory
 Author-email: so_software@simonsobservatory.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -67,15 +67,15 @@
 git clone git@github.com:TaiSakuma/acondbs-instance-example.git instance
 ```
 
 Set environmental variables
 
 ```bash
 export FLASK_APP="acondbs:create_app('$PWD/instance/config.py')"
-export FLASK_ENV=development
+export FLASK_DEBUG=1
 ```
 
 ### Initialize database
 
 ```bash
 flask init-db
 ```
```

### Comparing `acondbs-0.4.3/acondbs.egg-info/SOURCES.txt` & `acondbs-0.4.4/acondbs.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 acondbs/__init__.py
 acondbs/_logging.py
 acondbs/_version.py
 acondbs/_warnings.py
@@ -28,62 +29,15 @@
 acondbs/github/call.py
 acondbs/github/ops.py
 acondbs/github/query.py
 acondbs/migrations/README.md
 acondbs/migrations/alembic.ini
 acondbs/migrations/env.py
 acondbs/migrations/script.py.mako
-acondbs/migrations/versions/097c6676314c_change_enum.py
-acondbs/migrations/versions/0cce33011766_.py
-acondbs/migrations/versions/0f7fd06aa729_add_three_columns_to_product_relation_.py
-acondbs/migrations/versions/0ff075f16b94_rename_column.py
-acondbs/migrations/versions/12cc2bed191c_rename_table.py
-acondbs/migrations/versions/1583f2de9f39_add_attribute_tables.py
-acondbs/migrations/versions/1f86dd56d829_copy_data_in_web_config.py
-acondbs/migrations/versions/2910eaefa574_copy_to_attribute_tables.py
-acondbs/migrations/versions/2b15f740eed9_add_a_field_time_created_to_github_.py
-acondbs/migrations/versions/2ed9841987be_remove_columns_from_products.py
-acondbs/migrations/versions/35e6ddccd22a_copy_attributes.py
-acondbs/migrations/versions/3746a752f344_add_table_web_config.py
-acondbs/migrations/versions/3f4e8bfd8a7f_add_column_reverse_type_id_to_product_.py
-acondbs/migrations/versions/3f6526e7e5ff_add_tables_github_.py
-acondbs/migrations/versions/3f804a98ab06_add_table_log.py
-acondbs/migrations/versions/41e5ff6f2878_add_attribute_tables.py
-acondbs/migrations/versions/4398f463d243_delete_some_attributes.py
-acondbs/migrations/versions/4c32365bb655_rename_a_column_name_in_account_admins.py
-acondbs/migrations/versions/4e8693037e72_add_fields_to_github_orgs_and_github_.py
-acondbs/migrations/versions/63033c01def0_add_fields_to_github_admin_app_token.py
-acondbs/migrations/versions/63790f65e724_rename_table_web_config.py
-acondbs/migrations/versions/6bd27755b1a8_remove_column_from_attribute_tables.py
-acondbs/migrations/versions/8585129ca524_make_login_unique_on_github_users.py
-acondbs/migrations/versions/8e3f13ce98cb_make_nullable_false.py
-acondbs/migrations/versions/919b1bc74839_add_a_field_git_hub_id_to_github_orgs.py
-acondbs/migrations/versions/936fc5b02f16_rename_the_table_github_accepted_orgs_.py
-acondbs/migrations/versions/9495d7cb31ec_enter_data_to_field_table.py
-acondbs/migrations/versions/9f22f713c4ea_add_a_field_git_hub_id_to_github_users.py
-acondbs/migrations/versions/a4105346b478_change_column_type.py
-acondbs/migrations/versions/aeec123e508c_make_fields_in_product_relations_non_.py
-acondbs/migrations/versions/babb78f6f6b3_add_fields_to_products.py
-acondbs/migrations/versions/bad578ddbf3a_rename_the_table_github_admin_app_token_.py
-acondbs/migrations/versions/c090bba0e451_replace_date_with_data_time_in_products.py
-acondbs/migrations/versions/c0d8d6a8f071_add_fields_to_github_users.py
-acondbs/migrations/versions/cc64c8ef2115_re_initialize_migration.py
-acondbs/migrations/versions/ccd0df2c7da1_add_a_table_web_config.py
-acondbs/migrations/versions/cceebfa64b83_enter_data_in_attribute_tables.py
-acondbs/migrations/versions/ce157c2fa22e_constraint_on_product_relations.py
-acondbs/migrations/versions/d5e539d43045_add_a_table_admin_app_token.py
-acondbs/migrations/versions/d7cac99bbffa_add_columns_to_product_types.py
-acondbs/migrations/versions/d8afc036053a_add_a_column_to_product_types.py
-acondbs/migrations/versions/e077a31ad00b_add_tables.py
-acondbs/migrations/versions/e1d390d440d5_add_table_account_admins.py
-acondbs/migrations/versions/e58cc402c887_add_column_to_attribute_tables.py
-acondbs/migrations/versions/e69be63fc3b8_remove_table_web_config_old.py
-acondbs/migrations/versions/f84493df4297_update_type_field_association.py
-acondbs/migrations/versions/f92f99aa6fdd_rename_the_table_admin_app_token_github_.py
-acondbs/migrations/versions/f97ed2cdfb29_add_column_on_type_field_association.py
+acondbs/migrations/versions/2023-06-14_14:41-2ed9841987be.py
 acondbs/misc/__init__.py
 acondbs/misc/cap.py
 acondbs/misc/gitb.py
 acondbs/misc/lock.py
 acondbs/models/__init__.py
 acondbs/models/funcs.py
 acondbs/models/account/__init__.py
```

### Comparing `acondbs-0.4.3/setup.py` & `acondbs-0.4.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,21 +23,21 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     packages=find_packages(exclude=["docs", "tests"]),
     include_package_data=True,
     install_requires=[
-        "SQLAlchemy>=1.4",
-        "SQLAlchemy-Utils>=0.37",
-        "Flask>=2.0",
+        "SQLAlchemy>=1.4,<3",
+        "SQLAlchemy-Utils>=0.41",
+        "Flask>=2.3",
         "Flask-Cors>=3.0",
         "Flask-GraphQL>=2.0",
-        "Flask-Migrate>=3.1",
-        "Flask-SQLAlchemy>=2.5",
+        "Flask-Migrate>=3.1,<4",
+        "Flask-SQLAlchemy>=2.5,<3",
         "graphene-sqlalchemy>=2.3",
         "graphene-sqlalchemy-filter>=1.10",
         "cryptography>=3.2",
         "gitpython>=3.1",
         "requests>=2.24",
         "a2wsgi>=1.4"
     ],
```

### Comparing `acondbs-0.4.3/tests/auth/test_get_token_from_http_headers.py` & `acondbs-0.4.4/tests/auth/test_get_token_from_http_headers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import pytest
 
 from acondbs import auth
 
-##__________________________________________________________________||
 params = [
     pytest.param('Bearer {token}', id='no-quote'),
     pytest.param('Bearer "{token}"', id='double-quote'),
     pytest.param("Bearer '{token}'", id='single-quote'),
 ]
 
+
 @pytest.mark.parametrize('format_', params)
 def test_format(format_, app):
     token = '90b2ee5fed25506df04fd37343bb68d1803dd97f'
     environ_base = {'HTTP_AUTHORIZATION': format_.format(token=token)}
     with app.test_request_context(environ_base=environ_base):
         assert token == auth._get_token_from_http_headers()
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/auth/test_is_admin.py` & `acondbs-0.4.4/tests/auth/test_is_admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from acondbs import auth
 
-##__________________________________________________________________||
+
 def test_true(app):
-    token = '90b2ee5fed25506df04fd37343bb68d1803dd97f' # octcat
+    token = '90b2ee5fed25506df04fd37343bb68d1803dd97f'  # octcat
     environ_base = {'HTTP_AUTHORIZATION': f'Bearer {token}'}
     with app.test_request_context(environ_base=environ_base):
         assert auth.is_signed_in()
         assert auth.is_admin()
 
-##__________________________________________________________________||
+
 def test_false_not_admin(app):
-    token = '0fb8c9e16d6f7c4961c4c49212bf197d79f14080' # dojocat
+    token = '0fb8c9e16d6f7c4961c4c49212bf197d79f14080'  # dojocat
     environ_base = {'HTTP_AUTHORIZATION': f'Bearer {token}'}
     with app.test_request_context(environ_base=environ_base):
         assert auth.is_signed_in()
         assert not auth.is_admin()
 
-##__________________________________________________________________||
+
 def test_false_wrong_token(app):
     token = '0000000000000000000000000000000000000000'
     environ_base = {'HTTP_AUTHORIZATION': f'Bearer {token}'}
     with app.test_request_context(environ_base=environ_base):
         assert not auth.is_admin()
 
-##__________________________________________________________________||
+
 def test_false_no_token(app):
     environ_base = {}
     with app.test_request_context(environ_base=environ_base):
         assert not auth.is_admin()
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/auth/test_is_signed_in.py` & `acondbs-0.4.4/tests/auth/test_is_signed_in.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from acondbs import auth
 
-##__________________________________________________________________||
+
 def test_true(app):
     token = '90b2ee5fed25506df04fd37343bb68d1803dd97f'
     environ_base = {'HTTP_AUTHORIZATION': f'Bearer {token}'}
     with app.test_request_context(environ_base=environ_base):
         assert auth.is_signed_in()
 
-##__________________________________________________________________||
+
 def test_false_wrong_token(app):
     token = '0000000000000000000000000000000000000000'
     environ_base = {'HTTP_AUTHORIZATION': f'Bearer {token}'}
     with app.test_request_context(environ_base=environ_base):
         assert not auth.is_signed_in()
 
-##__________________________________________________________________||
+
 def test_false_no_token(app):
     environ_base = {}
     with app.test_request_context(environ_base=environ_base):
         assert not auth.is_signed_in()
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/blueprint/test_graphiql.py` & `acondbs-0.4.4/tests/blueprint/test_graphiql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import pytest
 
 from acondbs import create_app
 from acondbs.db.ops import define_tables
 
-
-##__________________________________________________________________||
 params = [
     [True, 200, "<!DOCTYPE html>"],
     [False, 400, "errors"],
 ]
 
 
 @pytest.mark.parametrize("graphiql, code, data", params)
@@ -24,15 +22,14 @@
     client = app.test_client()
 
     response = client.get("/graphql", headers={"Accept": "text/html"})
     assert code == response.status_code
     assert data in response.data.decode("utf-8")
 
 
-##__________________________________________________________________||
 params = [
     [None, "//cdn.jsdelivr.net/npm/graphiql@0.11.11/graphiql.min.js"],
     [1, "https://unpkg.com/graphiql/graphiql.min.js"],
     [2, "graphql-playground"],
 ]
 
 
@@ -47,10 +44,7 @@
         define_tables()
 
     client = app.test_client()
 
     response = client.get("/graphql", headers={"Accept": "text/html"})
     assert 200 == response.status_code
     assert data in response.data.decode("utf-8")
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/blueprint/test_schema_based_on_auth.py` & `acondbs-0.4.4/tests/blueprint/test_schema_based_on_auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from flask import json
+import unittest.mock as mock
 
 import pytest
-import unittest.mock as mock
+from flask import json
 
 from acondbs import create_app
 from acondbs.db.ops import define_tables
 
-
-##__________________________________________________________________||
 QUERY = '''
 {
   __schema {
     queryType {
       fields {
         name
       }
@@ -27,33 +25,30 @@
       }
     }
   }
 }
 '''
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app_empty():
     database_uri = "sqlite:///:memory:"
     y = create_app(SQLALCHEMY_DATABASE_URI=database_uri)
     with y.app_context():
         define_tables()
     yield y
 
 
-##__________________________________________________________________||
 @pytest.fixture()
 def mock_auth(monkeypatch):
     y = mock.Mock()
     monkeypatch.setattr("acondbs.blueprint.auth", y)
     yield y
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize('is_signed_in', [True, False])
 @pytest.mark.parametrize('is_admin', [True, False])
 def test_schema_selection(app_empty, is_signed_in, is_admin, mock_auth, snapshot):
     app = app_empty
 
     mock_auth.is_signed_in.return_value = is_signed_in
     mock_auth.is_admin.return_value = is_admin
@@ -65,9 +60,7 @@
     assert 200 == response.status_code
 
     result = json.loads(response.data)['data']
 
     un_jsonified = json.loads(response.data)
     snapshot.assert_match(un_jsonified)
     # print(json.dumps(un_jsonified, indent=2))
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/db/backup/test_as_csv_to_github.py` & `acondbs-0.4.4/tests/db/backup/test_as_csv_to_github.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-from pathlib import Path
+import unittest.mock as mock
 import warnings
+from pathlib import Path
 
 import pytest
-import unittest.mock as mock
 
 from acondbs.db.backup import backup_db_as_csv_to_github
 
-##__________________________________________________________________||
+
 @pytest.fixture()
 def mock_backup_db_as_csv_to_github_(monkeypatch):
     y = mock.Mock()
     monkeypatch.setattr("acondbs.db.backup.backup_db_as_csv_to_github_", y)
     yield y
 
+
 @pytest.fixture()
 def mock_lock_path(app, monkeypatch, tmpdir_factory):
     folder = Path(tmpdir_factory.mktemp('backup'))
     y = folder.joinpath('lock')
     monkeypatch.setitem(app.config, 'ACONDBS_DB_BACKUP_CSV_GIT_LOCK', str(y))
     monkeypatch.setitem(app.config, 'ACONDBS_DB_BACKUP_CSV_GIT_LOCK_TIMEOUT', 0.01)
     yield y
 
-##__________________________________________________________________||
-def test_backup_db_as_csv_to_github(app, mock_lock_path, mock_backup_db_as_csv_to_github_):
+
+def test_backup_db_as_csv_to_github(
+    app, mock_lock_path, mock_backup_db_as_csv_to_github_
+):
     with app.app_context():
         repo_path = app.config['ACONDBS_DB_BACKUP_CSV_GIT_FOLDER']
         backup_db_as_csv_to_github()
-    assert [mock.call(repo_path, None)] == mock_backup_db_as_csv_to_github_.call_args_list
+    assert [
+        mock.call(repo_path, None)
+    ] == mock_backup_db_as_csv_to_github_.call_args_list
+
 
-##__________________________________________________________________||
 def test_backup_db_locked(app, mock_lock_path, mock_backup_db_as_csv_to_github_):
     mock_lock_path.touch()
     with app.app_context():
         with warnings.catch_warnings(record=True) as w:
             backup_db_as_csv_to_github()
     assert [] == mock_backup_db_as_csv_to_github_.call_args_list
     assert len(w) == 1
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/db/backup/test_as_csv_to_github_.py` & `acondbs-0.4.4/tests/db/backup/test_as_csv_to_github_.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 from pathlib import Path
-import git
 
+import git
 import pytest
 from graphene.test import Client
 
-
+from acondbs.db.backup import backup_db_as_csv_to_github_
 from acondbs.db.ops import export_db_to_csv_files
 from acondbs.schema import schema_admin
 
-from acondbs.db.backup import backup_db_as_csv_to_github_
 
-##__________________________________________________________________||
 @pytest.fixture
 def local_repo(app, tmpdir_factory):
-    """
-    """
+    """ """
 
     # create a local repo with CSV files
     local_folder = Path(tmpdir_factory.mktemp('backup'))
     with app.app_context():
         export_db_to_csv_files(local_folder)
     local_repo = git.Repo.init(local_folder)
     local_repo.git.add(A=True)
     local_repo.index.commit('initial commit')
 
     yield local_repo
 
+
 @pytest.fixture
 def remote_repo(local_repo, tmpdir_factory):
-    """remote repo
-
-    """
+    """remote repo"""
 
     # create a remote repo (bare repo)
     folder = Path(tmpdir_factory.mktemp('backup'))
     remote_repo = git.Repo.init(folder, bare=True)
     remote_url = remote_repo.git_dir
 
     # push the current branch of the local repo to the remote repo
     remote = local_repo.create_remote('origin', url=remote_url)
     branch_name = local_repo.active_branch.name
     remote.push(refspec='{}:{}'.format(branch_name, branch_name))
     local_repo.heads[branch_name].set_tracking_branch(remote.refs[branch_name])
 
     yield remote_repo
 
-##__________________________________________________________________||
-def test_backup_db_as_csv_to_github_(app, local_repo, remote_repo):
 
+def test_backup_db_as_csv_to_github_(app, local_repo, remote_repo):
     repo_path = local_repo.working_tree_dir
     head_sha_old = local_repo.head.commit.hexsha
     assert head_sha_old == remote_repo.head.commit.hexsha
 
     # change the DB content
     mutation = '''
           mutation m {
@@ -70,9 +65,7 @@
         backup_db_as_csv_to_github_(repo_path)
 
     # assert
     assert not local_repo.is_dirty(untracked_files=True)
     head_sha_new = local_repo.head.commit.hexsha
     assert not head_sha_old == head_sha_new
     assert head_sha_new == remote_repo.head.commit.hexsha
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/db/backup/test_backup_db.py` & `acondbs-0.4.4/tests/db/backup/test_backup_db.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
+import unittest.mock as mock
 import warnings
 
 import pytest
-import unittest.mock as mock
 
 from acondbs.db.backup import backup_db
 
-##__________________________________________________________________||
+
 @pytest.fixture()
 def mock_backup_db_to_github(monkeypatch):
     y = mock.Mock()
     monkeypatch.setattr("acondbs.db.backup.backup_db_to_github", y)
     yield y
 
+
 @pytest.fixture()
 def mock_backup_db_as_csv_to_github(monkeypatch):
     y = mock.Mock()
     monkeypatch.setattr("acondbs.db.backup.backup_db_as_csv_to_github", y)
     yield y
 
-##__________________________________________________________________||
+
 def test_backup_db(mock_backup_db_to_github, mock_backup_db_as_csv_to_github):
     backup_db()
     mock_backup_db_to_github.assert_called_once()
     mock_backup_db_as_csv_to_github.assert_called_once()
 
+
 def test_exceptions(mock_backup_db_to_github, mock_backup_db_as_csv_to_github):
     mock_backup_db_to_github.side_effect = Exception()
     mock_backup_db_as_csv_to_github.side_effect = Exception()
     with warnings.catch_warnings(record=True) as w:
         backup_db()
     assert len(w) == 2
     mock_backup_db_to_github.assert_called_once()
     mock_backup_db_as_csv_to_github.assert_called_once()
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/db/ops/snapshots/snap_test_define_tables.py` & `acondbs-0.4.4/tests/db/ops/snapshots/snap_test_define_tables.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,139 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import GenericRepr, Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_define_tables_start_with_empty_db 1'] = {
-    'account_admins': GenericRepr("Table('account_admins', MetaData(), Column('admin_id', INTEGER(), table=<account_admins>, primary_key=True, nullable=False), Column('git_hub_login', TEXT(), table=<account_admins>, nullable=False), schema=None)"),
-    'attribute_boolean': GenericRepr("Table('attribute_boolean', MetaData(), Column('iid', INTEGER(), table=<attribute_boolean>, primary_key=True, nullable=False), Column('value', BOOLEAN(), table=<attribute_boolean>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_boolean>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_boolean>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_boolean>, nullable=False), schema=None)"),
-    'attribute_date': GenericRepr("Table('attribute_date', MetaData(), Column('iid', INTEGER(), table=<attribute_date>, primary_key=True, nullable=False), Column('value', DATE(), table=<attribute_date>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_date>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_date>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_date>, nullable=False), schema=None)"),
-    'attribute_date_time': GenericRepr("Table('attribute_date_time', MetaData(), Column('iid', INTEGER(), table=<attribute_date_time>, primary_key=True, nullable=False), Column('value', DATETIME(), table=<attribute_date_time>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_date_time>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_date_time>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_date_time>, nullable=False), schema=None)"),
-    'attribute_float': GenericRepr("Table('attribute_float', MetaData(), Column('iid', INTEGER(), table=<attribute_float>, primary_key=True, nullable=False), Column('value', FLOAT(), table=<attribute_float>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_float>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_float>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_float>, nullable=False), schema=None)"),
-    'attribute_integer': GenericRepr("Table('attribute_integer', MetaData(), Column('iid', INTEGER(), table=<attribute_integer>, primary_key=True, nullable=False), Column('value', INTEGER(), table=<attribute_integer>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_integer>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_integer>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_integer>, nullable=False), schema=None)"),
-    'attribute_time': GenericRepr("Table('attribute_time', MetaData(), Column('iid', INTEGER(), table=<attribute_time>, primary_key=True, nullable=False), Column('value', TIME(), table=<attribute_time>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_time>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_time>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_time>, nullable=False), schema=None)"),
-    'attribute_unicode_text': GenericRepr("Table('attribute_unicode_text', MetaData(), Column('iid', INTEGER(), table=<attribute_unicode_text>, primary_key=True, nullable=False), Column('value', TEXT(), table=<attribute_unicode_text>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_unicode_text>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_unicode_text>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_unicode_text>, nullable=False), schema=None)"),
-    'field': GenericRepr("Table('field', MetaData(), Column('field_id', INTEGER(), table=<field>, primary_key=True, nullable=False), Column('name', TEXT(), table=<field>, nullable=False), Column('type_', VARCHAR(length=11), table=<field>, nullable=False), schema=None)"),
-    'github_org_memberships': GenericRepr("Table('github_org_memberships', MetaData(), Column('entry_id', INTEGER(), table=<github_org_memberships>, primary_key=True, nullable=False), Column('org_id', INTEGER(), ForeignKey('github_orgs.org_id'), table=<github_org_memberships>, nullable=False), Column('member_id', INTEGER(), ForeignKey('github_users.user_id'), table=<github_org_memberships>, nullable=False), schema=None)"),
-    'github_orgs': GenericRepr("Table('github_orgs', MetaData(), Column('org_id', INTEGER(), table=<github_orgs>, primary_key=True, nullable=False), Column('git_hub_id', TEXT(), table=<github_orgs>, nullable=False), Column('login', TEXT(), table=<github_orgs>, nullable=False), Column('avatar_url', TEXT(), table=<github_orgs>), Column('url', TEXT(), table=<github_orgs>), schema=None)"),
-    'github_tokens': GenericRepr("Table('github_tokens', MetaData(), Column('token_id', INTEGER(), table=<github_tokens>, primary_key=True, nullable=False), Column('token', BLOB(), table=<github_tokens>), Column('scope', TEXT(), table=<github_tokens>), Column('user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<github_tokens>, nullable=False), Column('time_created', DATETIME(), table=<github_tokens>), schema=None)"),
-    'github_users': GenericRepr("Table('github_users', MetaData(), Column('user_id', INTEGER(), table=<github_users>, primary_key=True, nullable=False), Column('git_hub_id', TEXT(), table=<github_users>, nullable=False), Column('login', TEXT(), table=<github_users>, nullable=False), Column('name', TEXT(), table=<github_users>), Column('avatar_url', TEXT(), table=<github_users>), Column('url', TEXT(), table=<github_users>), schema=None)"),
-    'log': GenericRepr("Table('log', MetaData(), Column('id_', INTEGER(), table=<log>, primary_key=True, nullable=False), Column('level', TEXT(), table=<log>), Column('message', TEXT(), table=<log>), Column('time', DATETIME(), table=<log>), schema=None)"),
-    'product_file_paths': GenericRepr("Table('product_file_paths', MetaData(), Column('path_id', INTEGER(), table=<product_file_paths>, primary_key=True, nullable=False), Column('path', TEXT(), table=<product_file_paths>), Column('note', TEXT(), table=<product_file_paths>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_file_paths>), schema=None)"),
-    'product_relation_types': GenericRepr("Table('product_relation_types', MetaData(), Column('type_id', INTEGER(), table=<product_relation_types>, primary_key=True, nullable=False), Column('name', TEXT(), table=<product_relation_types>, nullable=False), Column('reverse_type_id', INTEGER(), ForeignKey('product_relation_types.type_id'), table=<product_relation_types>), Column('indef_article', TEXT(), table=<product_relation_types>), Column('singular', TEXT(), table=<product_relation_types>), Column('plural', TEXT(), table=<product_relation_types>), schema=None)"),
-    'product_relations': GenericRepr("Table('product_relations', MetaData(), Column('relation_id', INTEGER(), table=<product_relations>, primary_key=True, nullable=False), Column('type_id', INTEGER(), ForeignKey('product_relation_types.type_id'), table=<product_relations>, nullable=False), Column('self_product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_relations>, nullable=False), Column('other_product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_relations>, nullable=False), Column('reverse_relation_id', INTEGER(), ForeignKey('product_relations.relation_id'), table=<product_relations>), schema=None)"),
-    'product_types': GenericRepr("Table('product_types', MetaData(), Column('type_id', INTEGER(), table=<product_types>, primary_key=True, nullable=False), Column('name', TEXT(), table=<product_types>, nullable=False), Column('order', INTEGER(), table=<product_types>), Column('indef_article', TEXT(), table=<product_types>), Column('singular', TEXT(), table=<product_types>), Column('plural', TEXT(), table=<product_types>), Column('icon', TEXT(), table=<product_types>), schema=None)"),
-    'products': GenericRepr("Table('products', MetaData(), Column('product_id', INTEGER(), table=<products>, primary_key=True, nullable=False), Column('type_id', INTEGER(), ForeignKey('product_types.type_id'), table=<products>, nullable=False), Column('name', TEXT(), table=<products>, nullable=False), Column('time_posted', DATETIME(), table=<products>), Column('posting_git_hub_user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<products>), Column('time_updated', DATETIME(), table=<products>), Column('updating_git_hub_user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<products>), Column('note', TEXT(), table=<products>), schema=None)"),
-    'type_field_association': GenericRepr("Table('type_field_association', MetaData(), Column('iid', INTEGER(), table=<type_field_association>, primary_key=True, nullable=False), Column('order', INTEGER(), table=<type_field_association>), Column('type_id', INTEGER(), ForeignKey('product_types.type_id'), table=<type_field_association>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<type_field_association>, nullable=False), schema=None)"),
-    'web_config': GenericRepr("Table('web_config', MetaData(), Column('id_', INTEGER(), table=<web_config>, primary_key=True, nullable=False), Column('json', TEXT(), table=<web_config>), schema=None)")
+    'account_admins': GenericRepr(
+        "Table('account_admins', MetaData(), Column('admin_id', INTEGER(), table=<account_admins>, primary_key=True, nullable=False), Column('git_hub_login', TEXT(), table=<account_admins>, nullable=False), schema=None)"
+    ),
+    'attribute_boolean': GenericRepr(
+        "Table('attribute_boolean', MetaData(), Column('iid', INTEGER(), table=<attribute_boolean>, primary_key=True, nullable=False), Column('value', BOOLEAN(), table=<attribute_boolean>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_boolean>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_boolean>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_boolean>, nullable=False), schema=None)"
+    ),
+    'attribute_date': GenericRepr(
+        "Table('attribute_date', MetaData(), Column('iid', INTEGER(), table=<attribute_date>, primary_key=True, nullable=False), Column('value', DATE(), table=<attribute_date>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_date>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_date>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_date>, nullable=False), schema=None)"
+    ),
+    'attribute_date_time': GenericRepr(
+        "Table('attribute_date_time', MetaData(), Column('iid', INTEGER(), table=<attribute_date_time>, primary_key=True, nullable=False), Column('value', DATETIME(), table=<attribute_date_time>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_date_time>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_date_time>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_date_time>, nullable=False), schema=None)"
+    ),
+    'attribute_float': GenericRepr(
+        "Table('attribute_float', MetaData(), Column('iid', INTEGER(), table=<attribute_float>, primary_key=True, nullable=False), Column('value', FLOAT(), table=<attribute_float>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_float>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_float>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_float>, nullable=False), schema=None)"
+    ),
+    'attribute_integer': GenericRepr(
+        "Table('attribute_integer', MetaData(), Column('iid', INTEGER(), table=<attribute_integer>, primary_key=True, nullable=False), Column('value', INTEGER(), table=<attribute_integer>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_integer>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_integer>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_integer>, nullable=False), schema=None)"
+    ),
+    'attribute_time': GenericRepr(
+        "Table('attribute_time', MetaData(), Column('iid', INTEGER(), table=<attribute_time>, primary_key=True, nullable=False), Column('value', TIME(), table=<attribute_time>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_time>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_time>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_time>, nullable=False), schema=None)"
+    ),
+    'attribute_unicode_text': GenericRepr(
+        "Table('attribute_unicode_text', MetaData(), Column('iid', INTEGER(), table=<attribute_unicode_text>, primary_key=True, nullable=False), Column('value', TEXT(), table=<attribute_unicode_text>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_unicode_text>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_unicode_text>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_unicode_text>, nullable=False), schema=None)"
+    ),
+    'field': GenericRepr(
+        "Table('field', MetaData(), Column('field_id', INTEGER(), table=<field>, primary_key=True, nullable=False), Column('name', TEXT(), table=<field>, nullable=False), Column('type_', VARCHAR(length=11), table=<field>, nullable=False), schema=None)"
+    ),
+    'github_org_memberships': GenericRepr(
+        "Table('github_org_memberships', MetaData(), Column('entry_id', INTEGER(), table=<github_org_memberships>, primary_key=True, nullable=False), Column('org_id', INTEGER(), ForeignKey('github_orgs.org_id'), table=<github_org_memberships>, nullable=False), Column('member_id', INTEGER(), ForeignKey('github_users.user_id'), table=<github_org_memberships>, nullable=False), schema=None)"
+    ),
+    'github_orgs': GenericRepr(
+        "Table('github_orgs', MetaData(), Column('org_id', INTEGER(), table=<github_orgs>, primary_key=True, nullable=False), Column('git_hub_id', TEXT(), table=<github_orgs>, nullable=False), Column('login', TEXT(), table=<github_orgs>, nullable=False), Column('avatar_url', TEXT(), table=<github_orgs>), Column('url', TEXT(), table=<github_orgs>), schema=None)"
+    ),
+    'github_tokens': GenericRepr(
+        "Table('github_tokens', MetaData(), Column('token_id', INTEGER(), table=<github_tokens>, primary_key=True, nullable=False), Column('token', BLOB(), table=<github_tokens>), Column('scope', TEXT(), table=<github_tokens>), Column('user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<github_tokens>, nullable=False), Column('time_created', DATETIME(), table=<github_tokens>), schema=None)"
+    ),
+    'github_users': GenericRepr(
+        "Table('github_users', MetaData(), Column('user_id', INTEGER(), table=<github_users>, primary_key=True, nullable=False), Column('git_hub_id', TEXT(), table=<github_users>, nullable=False), Column('login', TEXT(), table=<github_users>, nullable=False), Column('name', TEXT(), table=<github_users>), Column('avatar_url', TEXT(), table=<github_users>), Column('url', TEXT(), table=<github_users>), schema=None)"
+    ),
+    'log': GenericRepr(
+        "Table('log', MetaData(), Column('id_', INTEGER(), table=<log>, primary_key=True, nullable=False), Column('level', TEXT(), table=<log>), Column('message', TEXT(), table=<log>), Column('time', DATETIME(), table=<log>), schema=None)"
+    ),
+    'product_file_paths': GenericRepr(
+        "Table('product_file_paths', MetaData(), Column('path_id', INTEGER(), table=<product_file_paths>, primary_key=True, nullable=False), Column('path', TEXT(), table=<product_file_paths>), Column('note', TEXT(), table=<product_file_paths>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_file_paths>), schema=None)"
+    ),
+    'product_relation_types': GenericRepr(
+        "Table('product_relation_types', MetaData(), Column('type_id', INTEGER(), table=<product_relation_types>, primary_key=True, nullable=False), Column('name', TEXT(), table=<product_relation_types>, nullable=False), Column('reverse_type_id', INTEGER(), ForeignKey('product_relation_types.type_id'), table=<product_relation_types>), Column('indef_article', TEXT(), table=<product_relation_types>), Column('singular', TEXT(), table=<product_relation_types>), Column('plural', TEXT(), table=<product_relation_types>), schema=None)"
+    ),
+    'product_relations': GenericRepr(
+        "Table('product_relations', MetaData(), Column('relation_id', INTEGER(), table=<product_relations>, primary_key=True, nullable=False), Column('type_id', INTEGER(), ForeignKey('product_relation_types.type_id'), table=<product_relations>, nullable=False), Column('self_product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_relations>, nullable=False), Column('other_product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_relations>, nullable=False), Column('reverse_relation_id', INTEGER(), ForeignKey('product_relations.relation_id'), table=<product_relations>), schema=None)"
+    ),
+    'product_types': GenericRepr(
+        "Table('product_types', MetaData(), Column('type_id', INTEGER(), table=<product_types>, primary_key=True, nullable=False), Column('name', TEXT(), table=<product_types>, nullable=False), Column('order', INTEGER(), table=<product_types>), Column('indef_article', TEXT(), table=<product_types>), Column('singular', TEXT(), table=<product_types>), Column('plural', TEXT(), table=<product_types>), Column('icon', TEXT(), table=<product_types>), schema=None)"
+    ),
+    'products': GenericRepr(
+        "Table('products', MetaData(), Column('product_id', INTEGER(), table=<products>, primary_key=True, nullable=False), Column('type_id', INTEGER(), ForeignKey('product_types.type_id'), table=<products>, nullable=False), Column('name', TEXT(), table=<products>, nullable=False), Column('time_posted', DATETIME(), table=<products>), Column('posting_git_hub_user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<products>), Column('time_updated', DATETIME(), table=<products>), Column('updating_git_hub_user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<products>), Column('note', TEXT(), table=<products>), schema=None)"
+    ),
+    'type_field_association': GenericRepr(
+        "Table('type_field_association', MetaData(), Column('iid', INTEGER(), table=<type_field_association>, primary_key=True, nullable=False), Column('order', INTEGER(), table=<type_field_association>), Column('type_id', INTEGER(), ForeignKey('product_types.type_id'), table=<type_field_association>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<type_field_association>, nullable=False), schema=None)"
+    ),
+    'web_config': GenericRepr(
+        "Table('web_config', MetaData(), Column('id_', INTEGER(), table=<web_config>, primary_key=True, nullable=False), Column('json', TEXT(), table=<web_config>), schema=None)"
+    ),
 }
 
 snapshots['test_define_tables_start_with_nonempty_db 1'] = {
-    'account_admins': GenericRepr("Table('account_admins', MetaData(), Column('admin_id', INTEGER(), table=<account_admins>, primary_key=True, nullable=False), Column('git_hub_login', TEXT(), table=<account_admins>, nullable=False), schema=None)"),
-    'attribute_boolean': GenericRepr("Table('attribute_boolean', MetaData(), Column('iid', INTEGER(), table=<attribute_boolean>, primary_key=True, nullable=False), Column('value', BOOLEAN(), table=<attribute_boolean>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_boolean>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_boolean>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_boolean>, nullable=False), schema=None)"),
-    'attribute_date': GenericRepr("Table('attribute_date', MetaData(), Column('iid', INTEGER(), table=<attribute_date>, primary_key=True, nullable=False), Column('value', DATE(), table=<attribute_date>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_date>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_date>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_date>, nullable=False), schema=None)"),
-    'attribute_date_time': GenericRepr("Table('attribute_date_time', MetaData(), Column('iid', INTEGER(), table=<attribute_date_time>, primary_key=True, nullable=False), Column('value', DATETIME(), table=<attribute_date_time>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_date_time>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_date_time>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_date_time>, nullable=False), schema=None)"),
-    'attribute_float': GenericRepr("Table('attribute_float', MetaData(), Column('iid', INTEGER(), table=<attribute_float>, primary_key=True, nullable=False), Column('value', FLOAT(), table=<attribute_float>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_float>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_float>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_float>, nullable=False), schema=None)"),
-    'attribute_integer': GenericRepr("Table('attribute_integer', MetaData(), Column('iid', INTEGER(), table=<attribute_integer>, primary_key=True, nullable=False), Column('value', INTEGER(), table=<attribute_integer>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_integer>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_integer>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_integer>, nullable=False), schema=None)"),
-    'attribute_time': GenericRepr("Table('attribute_time', MetaData(), Column('iid', INTEGER(), table=<attribute_time>, primary_key=True, nullable=False), Column('value', TIME(), table=<attribute_time>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_time>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_time>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_time>, nullable=False), schema=None)"),
-    'attribute_unicode_text': GenericRepr("Table('attribute_unicode_text', MetaData(), Column('iid', INTEGER(), table=<attribute_unicode_text>, primary_key=True, nullable=False), Column('value', TEXT(), table=<attribute_unicode_text>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_unicode_text>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_unicode_text>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_unicode_text>, nullable=False), schema=None)"),
-    'field': GenericRepr("Table('field', MetaData(), Column('field_id', INTEGER(), table=<field>, primary_key=True, nullable=False), Column('name', TEXT(), table=<field>, nullable=False), Column('type_', VARCHAR(length=11), table=<field>, nullable=False), schema=None)"),
-    'github_org_memberships': GenericRepr("Table('github_org_memberships', MetaData(), Column('entry_id', INTEGER(), table=<github_org_memberships>, primary_key=True, nullable=False), Column('org_id', INTEGER(), ForeignKey('github_orgs.org_id'), table=<github_org_memberships>, nullable=False), Column('member_id', INTEGER(), ForeignKey('github_users.user_id'), table=<github_org_memberships>, nullable=False), schema=None)"),
-    'github_orgs': GenericRepr("Table('github_orgs', MetaData(), Column('org_id', INTEGER(), table=<github_orgs>, primary_key=True, nullable=False), Column('git_hub_id', TEXT(), table=<github_orgs>, nullable=False), Column('login', TEXT(), table=<github_orgs>, nullable=False), Column('avatar_url', TEXT(), table=<github_orgs>), Column('url', TEXT(), table=<github_orgs>), schema=None)"),
-    'github_tokens': GenericRepr("Table('github_tokens', MetaData(), Column('token_id', INTEGER(), table=<github_tokens>, primary_key=True, nullable=False), Column('token', BLOB(), table=<github_tokens>), Column('scope', TEXT(), table=<github_tokens>), Column('user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<github_tokens>, nullable=False), Column('time_created', DATETIME(), table=<github_tokens>), schema=None)"),
-    'github_users': GenericRepr("Table('github_users', MetaData(), Column('user_id', INTEGER(), table=<github_users>, primary_key=True, nullable=False), Column('git_hub_id', TEXT(), table=<github_users>, nullable=False), Column('login', TEXT(), table=<github_users>, nullable=False), Column('name', TEXT(), table=<github_users>), Column('avatar_url', TEXT(), table=<github_users>), Column('url', TEXT(), table=<github_users>), schema=None)"),
-    'log': GenericRepr("Table('log', MetaData(), Column('id_', INTEGER(), table=<log>, primary_key=True, nullable=False), Column('level', TEXT(), table=<log>), Column('message', TEXT(), table=<log>), Column('time', DATETIME(), table=<log>), schema=None)"),
-    'product_file_paths': GenericRepr("Table('product_file_paths', MetaData(), Column('path_id', INTEGER(), table=<product_file_paths>, primary_key=True, nullable=False), Column('path', TEXT(), table=<product_file_paths>), Column('note', TEXT(), table=<product_file_paths>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_file_paths>), schema=None)"),
-    'product_relation_types': GenericRepr("Table('product_relation_types', MetaData(), Column('type_id', INTEGER(), table=<product_relation_types>, primary_key=True, nullable=False), Column('name', TEXT(), table=<product_relation_types>, nullable=False), Column('reverse_type_id', INTEGER(), ForeignKey('product_relation_types.type_id'), table=<product_relation_types>), Column('indef_article', TEXT(), table=<product_relation_types>), Column('singular', TEXT(), table=<product_relation_types>), Column('plural', TEXT(), table=<product_relation_types>), schema=None)"),
-    'product_relations': GenericRepr("Table('product_relations', MetaData(), Column('relation_id', INTEGER(), table=<product_relations>, primary_key=True, nullable=False), Column('type_id', INTEGER(), ForeignKey('product_relation_types.type_id'), table=<product_relations>, nullable=False), Column('self_product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_relations>, nullable=False), Column('other_product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_relations>, nullable=False), Column('reverse_relation_id', INTEGER(), ForeignKey('product_relations.relation_id'), table=<product_relations>), schema=None)"),
-    'product_types': GenericRepr("Table('product_types', MetaData(), Column('type_id', INTEGER(), table=<product_types>, primary_key=True, nullable=False), Column('name', TEXT(), table=<product_types>, nullable=False), Column('order', INTEGER(), table=<product_types>), Column('indef_article', TEXT(), table=<product_types>), Column('singular', TEXT(), table=<product_types>), Column('plural', TEXT(), table=<product_types>), Column('icon', TEXT(), table=<product_types>), schema=None)"),
-    'products': GenericRepr("Table('products', MetaData(), Column('product_id', INTEGER(), table=<products>, primary_key=True, nullable=False), Column('type_id', INTEGER(), ForeignKey('product_types.type_id'), table=<products>, nullable=False), Column('name', TEXT(), table=<products>, nullable=False), Column('time_posted', DATETIME(), table=<products>), Column('posting_git_hub_user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<products>), Column('time_updated', DATETIME(), table=<products>), Column('updating_git_hub_user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<products>), Column('note', TEXT(), table=<products>), schema=None)"),
-    'type_field_association': GenericRepr("Table('type_field_association', MetaData(), Column('iid', INTEGER(), table=<type_field_association>, primary_key=True, nullable=False), Column('order', INTEGER(), table=<type_field_association>), Column('type_id', INTEGER(), ForeignKey('product_types.type_id'), table=<type_field_association>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<type_field_association>, nullable=False), schema=None)"),
-    'web_config': GenericRepr("Table('web_config', MetaData(), Column('id_', INTEGER(), table=<web_config>, primary_key=True, nullable=False), Column('json', TEXT(), table=<web_config>), schema=None)")
+    'account_admins': GenericRepr(
+        "Table('account_admins', MetaData(), Column('admin_id', INTEGER(), table=<account_admins>, primary_key=True, nullable=False), Column('git_hub_login', TEXT(), table=<account_admins>, nullable=False), schema=None)"
+    ),
+    'attribute_boolean': GenericRepr(
+        "Table('attribute_boolean', MetaData(), Column('iid', INTEGER(), table=<attribute_boolean>, primary_key=True, nullable=False), Column('value', BOOLEAN(), table=<attribute_boolean>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_boolean>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_boolean>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_boolean>, nullable=False), schema=None)"
+    ),
+    'attribute_date': GenericRepr(
+        "Table('attribute_date', MetaData(), Column('iid', INTEGER(), table=<attribute_date>, primary_key=True, nullable=False), Column('value', DATE(), table=<attribute_date>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_date>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_date>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_date>, nullable=False), schema=None)"
+    ),
+    'attribute_date_time': GenericRepr(
+        "Table('attribute_date_time', MetaData(), Column('iid', INTEGER(), table=<attribute_date_time>, primary_key=True, nullable=False), Column('value', DATETIME(), table=<attribute_date_time>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_date_time>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_date_time>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_date_time>, nullable=False), schema=None)"
+    ),
+    'attribute_float': GenericRepr(
+        "Table('attribute_float', MetaData(), Column('iid', INTEGER(), table=<attribute_float>, primary_key=True, nullable=False), Column('value', FLOAT(), table=<attribute_float>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_float>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_float>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_float>, nullable=False), schema=None)"
+    ),
+    'attribute_integer': GenericRepr(
+        "Table('attribute_integer', MetaData(), Column('iid', INTEGER(), table=<attribute_integer>, primary_key=True, nullable=False), Column('value', INTEGER(), table=<attribute_integer>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_integer>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_integer>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_integer>, nullable=False), schema=None)"
+    ),
+    'attribute_time': GenericRepr(
+        "Table('attribute_time', MetaData(), Column('iid', INTEGER(), table=<attribute_time>, primary_key=True, nullable=False), Column('value', TIME(), table=<attribute_time>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_time>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_time>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_time>, nullable=False), schema=None)"
+    ),
+    'attribute_unicode_text': GenericRepr(
+        "Table('attribute_unicode_text', MetaData(), Column('iid', INTEGER(), table=<attribute_unicode_text>, primary_key=True, nullable=False), Column('value', TEXT(), table=<attribute_unicode_text>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<attribute_unicode_text>, nullable=False), Column('type_field_association_iid', INTEGER(), ForeignKey('type_field_association.iid'), table=<attribute_unicode_text>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<attribute_unicode_text>, nullable=False), schema=None)"
+    ),
+    'field': GenericRepr(
+        "Table('field', MetaData(), Column('field_id', INTEGER(), table=<field>, primary_key=True, nullable=False), Column('name', TEXT(), table=<field>, nullable=False), Column('type_', VARCHAR(length=11), table=<field>, nullable=False), schema=None)"
+    ),
+    'github_org_memberships': GenericRepr(
+        "Table('github_org_memberships', MetaData(), Column('entry_id', INTEGER(), table=<github_org_memberships>, primary_key=True, nullable=False), Column('org_id', INTEGER(), ForeignKey('github_orgs.org_id'), table=<github_org_memberships>, nullable=False), Column('member_id', INTEGER(), ForeignKey('github_users.user_id'), table=<github_org_memberships>, nullable=False), schema=None)"
+    ),
+    'github_orgs': GenericRepr(
+        "Table('github_orgs', MetaData(), Column('org_id', INTEGER(), table=<github_orgs>, primary_key=True, nullable=False), Column('git_hub_id', TEXT(), table=<github_orgs>, nullable=False), Column('login', TEXT(), table=<github_orgs>, nullable=False), Column('avatar_url', TEXT(), table=<github_orgs>), Column('url', TEXT(), table=<github_orgs>), schema=None)"
+    ),
+    'github_tokens': GenericRepr(
+        "Table('github_tokens', MetaData(), Column('token_id', INTEGER(), table=<github_tokens>, primary_key=True, nullable=False), Column('token', BLOB(), table=<github_tokens>), Column('scope', TEXT(), table=<github_tokens>), Column('user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<github_tokens>, nullable=False), Column('time_created', DATETIME(), table=<github_tokens>), schema=None)"
+    ),
+    'github_users': GenericRepr(
+        "Table('github_users', MetaData(), Column('user_id', INTEGER(), table=<github_users>, primary_key=True, nullable=False), Column('git_hub_id', TEXT(), table=<github_users>, nullable=False), Column('login', TEXT(), table=<github_users>, nullable=False), Column('name', TEXT(), table=<github_users>), Column('avatar_url', TEXT(), table=<github_users>), Column('url', TEXT(), table=<github_users>), schema=None)"
+    ),
+    'log': GenericRepr(
+        "Table('log', MetaData(), Column('id_', INTEGER(), table=<log>, primary_key=True, nullable=False), Column('level', TEXT(), table=<log>), Column('message', TEXT(), table=<log>), Column('time', DATETIME(), table=<log>), schema=None)"
+    ),
+    'product_file_paths': GenericRepr(
+        "Table('product_file_paths', MetaData(), Column('path_id', INTEGER(), table=<product_file_paths>, primary_key=True, nullable=False), Column('path', TEXT(), table=<product_file_paths>), Column('note', TEXT(), table=<product_file_paths>), Column('product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_file_paths>), schema=None)"
+    ),
+    'product_relation_types': GenericRepr(
+        "Table('product_relation_types', MetaData(), Column('type_id', INTEGER(), table=<product_relation_types>, primary_key=True, nullable=False), Column('name', TEXT(), table=<product_relation_types>, nullable=False), Column('reverse_type_id', INTEGER(), ForeignKey('product_relation_types.type_id'), table=<product_relation_types>), Column('indef_article', TEXT(), table=<product_relation_types>), Column('singular', TEXT(), table=<product_relation_types>), Column('plural', TEXT(), table=<product_relation_types>), schema=None)"
+    ),
+    'product_relations': GenericRepr(
+        "Table('product_relations', MetaData(), Column('relation_id', INTEGER(), table=<product_relations>, primary_key=True, nullable=False), Column('type_id', INTEGER(), ForeignKey('product_relation_types.type_id'), table=<product_relations>, nullable=False), Column('self_product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_relations>, nullable=False), Column('other_product_id', INTEGER(), ForeignKey('products.product_id'), table=<product_relations>, nullable=False), Column('reverse_relation_id', INTEGER(), ForeignKey('product_relations.relation_id'), table=<product_relations>), schema=None)"
+    ),
+    'product_types': GenericRepr(
+        "Table('product_types', MetaData(), Column('type_id', INTEGER(), table=<product_types>, primary_key=True, nullable=False), Column('name', TEXT(), table=<product_types>, nullable=False), Column('order', INTEGER(), table=<product_types>), Column('indef_article', TEXT(), table=<product_types>), Column('singular', TEXT(), table=<product_types>), Column('plural', TEXT(), table=<product_types>), Column('icon', TEXT(), table=<product_types>), schema=None)"
+    ),
+    'products': GenericRepr(
+        "Table('products', MetaData(), Column('product_id', INTEGER(), table=<products>, primary_key=True, nullable=False), Column('type_id', INTEGER(), ForeignKey('product_types.type_id'), table=<products>, nullable=False), Column('name', TEXT(), table=<products>, nullable=False), Column('time_posted', DATETIME(), table=<products>), Column('posting_git_hub_user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<products>), Column('time_updated', DATETIME(), table=<products>), Column('updating_git_hub_user_id', INTEGER(), ForeignKey('github_users.user_id'), table=<products>), Column('note', TEXT(), table=<products>), schema=None)"
+    ),
+    'type_field_association': GenericRepr(
+        "Table('type_field_association', MetaData(), Column('iid', INTEGER(), table=<type_field_association>, primary_key=True, nullable=False), Column('order', INTEGER(), table=<type_field_association>), Column('type_id', INTEGER(), ForeignKey('product_types.type_id'), table=<type_field_association>, nullable=False), Column('field_id', INTEGER(), ForeignKey('field.field_id'), table=<type_field_association>, nullable=False), schema=None)"
+    ),
+    'web_config': GenericRepr(
+        "Table('web_config', MetaData(), Column('id_', INTEGER(), table=<web_config>, primary_key=True, nullable=False), Column('json', TEXT(), table=<web_config>), schema=None)"
+    ),
 }
```

### Comparing `acondbs-0.4.3/tests/db/ops/snapshots/snap_test_export_csv.py` & `acondbs-0.4.4/tests/db/ops/snapshots/snap_test_export_csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,627 +1,541 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import GenericRepr, Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_export_db_to_csv_files 1'] = {
-    'account_admins': [
-    ],
-    'attribute_boolean': [
-    ],
+    'account_admins': [],
+    'attribute_boolean': [],
     'attribute_date': [
         {
             'field_id': 3,
             'iid': 1,
             'product_id': 1001,
             'type_field_association_iid': 3,
-            'value': GenericRepr('datetime.date(2019, 2, 13)')
+            'value': GenericRepr('datetime.date(2019, 2, 13)'),
         },
         {
             'field_id': 3,
             'iid': 2,
             'product_id': 1002,
             'type_field_association_iid': 9,
-            'value': GenericRepr('datetime.date(2019, 3, 15)')
+            'value': GenericRepr('datetime.date(2019, 3, 15)'),
         },
         {
             'field_id': 3,
             'iid': 3,
             'product_id': 1010,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2018, 1, 1)')
+            'value': GenericRepr('datetime.date(2018, 1, 1)'),
         },
         {
             'field_id': 3,
             'iid': 4,
             'product_id': 1012,
             'type_field_association_iid': 3,
-            'value': GenericRepr('datetime.date(2020, 1, 20)')
+            'value': GenericRepr('datetime.date(2020, 1, 20)'),
         },
         {
             'field_id': 3,
             'iid': 5,
             'product_id': 1013,
             'type_field_association_iid': 3,
-            'value': GenericRepr('datetime.date(2020, 2, 1)')
+            'value': GenericRepr('datetime.date(2020, 2, 1)'),
         },
         {
             'field_id': 3,
             'iid': 6,
             'product_id': 1070,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2019, 3, 4)')
+            'value': GenericRepr('datetime.date(2019, 3, 4)'),
         },
         {
             'field_id': 3,
             'iid': 7,
             'product_id': 1120,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2019, 6, 7)')
+            'value': GenericRepr('datetime.date(2019, 6, 7)'),
         },
         {
             'field_id': 3,
             'iid': 8,
             'product_id': 1130,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2020, 1, 23)')
+            'value': GenericRepr('datetime.date(2020, 1, 23)'),
         },
         {
             'field_id': 3,
             'iid': 9,
             'product_id': 1150,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2020, 2, 7)')
-        }
-    ],
-    'attribute_date_time': [
-    ],
-    'attribute_float': [
-    ],
-    'attribute_integer': [
-    ],
-    'attribute_time': [
+            'value': GenericRepr('datetime.date(2020, 2, 7)'),
+        },
     ],
+    'attribute_date_time': [],
+    'attribute_float': [],
+    'attribute_integer': [],
+    'attribute_time': [],
     'attribute_unicode_text': [
         {
             'field_id': 1,
             'iid': 2,
             'product_id': 1001,
             'type_field_association_iid': 1,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 3,
             'product_id': 1001,
             'type_field_association_iid': 2,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 8,
             'product_id': 1002,
             'type_field_association_iid': 7,
-            'value': 'abc-def'
+            'value': 'abc-def',
         },
         {
             'field_id': 2,
             'iid': 9,
             'product_id': 1002,
             'type_field_association_iid': 8,
-            'value': 'abc-def'
+            'value': 'abc-def',
         },
         {
             'field_id': 1,
             'iid': 14,
             'product_id': 1010,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 15,
             'product_id': 1010,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 20,
             'product_id': 1012,
             'type_field_association_iid': 1,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 21,
             'product_id': 1012,
             'type_field_association_iid': 2,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 26,
             'product_id': 1013,
             'type_field_association_iid': 1,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 27,
             'product_id': 1013,
             'type_field_association_iid': 2,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 32,
             'product_id': 1070,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 33,
             'product_id': 1070,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 38,
             'product_id': 1120,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 39,
             'product_id': 1120,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 44,
             'product_id': 1130,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 45,
             'product_id': 1130,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 50,
             'product_id': 1150,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 51,
             'product_id': 1150,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
-        }
-    ],
-    'field': [
-        {
-            'field_id': 1,
-            'name': 'contact',
-            'type_': 'UnicodeText'
-        },
-        {
-            'field_id': 2,
-            'name': 'produced_by',
-            'type_': 'UnicodeText'
+            'value': 'pwg-pmn',
         },
-        {
-            'field_id': 3,
-            'name': 'date_produced',
-            'type_': 'Date'
-        }
     ],
-    'github_org_memberships': [
+    'field': [
+        {'field_id': 1, 'name': 'contact', 'type_': 'UnicodeText'},
+        {'field_id': 2, 'name': 'produced_by', 'type_': 'UnicodeText'},
+        {'field_id': 3, 'name': 'date_produced', 'type_': 'Date'},
     ],
+    'github_org_memberships': [],
     'github_orgs': [
         {
             'avatar_url': 'https://avatars0.githubusercontent.com/u/75631844?v=4',
             'git_hub_id': '012:Organization75631844',
             'login': 'urban-octo-disco',
             'org_id': 1,
-            'url': 'https://github.com/urban-octo-disco'
+            'url': 'https://github.com/urban-octo-disco',
         }
     ],
     'github_tokens': [
         {
             'scope': 'read:org',
             'time_created': GenericRepr('datetime.datetime(2020, 1, 4, 14, 32, 15)'),
             'token': b'aKjGknYDHY39Z2xAaN7+sQ==',
             'token_id': 1,
-            'user_id': 1
+            'user_id': 1,
         }
     ],
     'github_users': [
         {
             'avatar_url': 'https://avatars3.githubusercontent.com/u/583231?v=4',
             'git_hub_id': '04:User583231',
             'login': 'octocat',
             'name': 'The Octocat',
             'url': 'https://github.com/octocat',
-            'user_id': 1
+            'user_id': 1,
         },
         {
             'avatar_url': 'https://avatars0.githubusercontent.com/u/9758946?v=4',
             'git_hub_id': '04:User9758946',
             'login': 'dojocat',
             'name': 'dojocat',
             'url': 'https://github.com/dojocat',
-            'user_id': 2
-        }
-    ],
-    'log': [
+            'user_id': 2,
+        },
     ],
+    'log': [],
     'product_file_paths': [
-        {
-            'note': '',
-            'path': 'nersc:/go/to/my/maps',
-            'path_id': 1,
-            'product_id': 1001
-        },
+        {'note': '', 'path': 'nersc:/go/to/my/maps', 'path_id': 1, 'product_id': 1001},
         {
             'note': 'lat only',
             'path': 'nersc:/go/to/my/maps_v2',
             'path_id': 2,
-            'product_id': 1012
+            'product_id': 1012,
         },
         {
             'note': 'lat only',
             'path': 'abcde:/path/to/the/maps_v2',
             'path_id': 3,
-            'product_id': 1012
+            'product_id': 1012,
         },
         {
             'note': 'lat only',
             'path': 'nersc:/go/to/my/maps_v3',
             'path_id': 4,
-            'product_id': 1013
+            'product_id': 1013,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20190304',
             'path_id': 5,
-            'product_id': 1070
+            'product_id': 1070,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20190607',
             'path_id': 6,
-            'product_id': 1120
+            'product_id': 1120,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20200123',
             'path_id': 7,
-            'product_id': 1130
+            'product_id': 1130,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20200207',
             'path_id': 8,
-            'product_id': 1150
+            'product_id': 1150,
         },
         {
             'note': '',
             'path': 'nersc:/go/to/my/simulations',
             'path_id': 9,
-            'product_id': 1002
+            'product_id': 1002,
         },
         {
             'note': '',
             'path': 'abcde:/path/to/the/simulations',
             'path_id': 10,
-            'product_id': 1002
-        }
+            'product_id': 1002,
+        },
     ],
     'product_relation_types': [
         {
             'indef_article': 'a',
             'name': 'parent',
             'plural': 'parents',
             'reverse_type_id': 2,
             'singular': 'parent',
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'indef_article': 'a',
             'name': 'child',
             'plural': 'children',
             'reverse_type_id': 1,
             'singular': 'child',
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'indef_article': 'a',
             'name': 'plaintiff',
             'plural': 'plaintiffs',
             'reverse_type_id': 4,
             'singular': 'plaintiff',
-            'type_id': 3
+            'type_id': 3,
         },
         {
             'indef_article': 'a',
             'name': 'defendant',
             'plural': 'defendants',
             'reverse_type_id': 3,
             'singular': 'defendant',
-            'type_id': 4
-        }
+            'type_id': 4,
+        },
     ],
     'product_relations': [
         {
             'other_product_id': 1012,
             'relation_id': 1,
             'reverse_relation_id': 2,
             'self_product_id': 1130,
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'other_product_id': 1130,
             'relation_id': 2,
             'reverse_relation_id': 1,
             'self_product_id': 1012,
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'other_product_id': 1013,
             'relation_id': 3,
             'reverse_relation_id': 4,
             'self_product_id': 1150,
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'other_product_id': 1150,
             'relation_id': 4,
             'reverse_relation_id': 3,
             'self_product_id': 1013,
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'other_product_id': 1130,
             'relation_id': 5,
             'reverse_relation_id': 6,
             'self_product_id': 1150,
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'other_product_id': 1150,
             'relation_id': 6,
             'reverse_relation_id': 5,
             'self_product_id': 1130,
-            'type_id': 2
-        }
+            'type_id': 2,
+        },
     ],
     'product_types': [
         {
             'icon': 'mdi-map',
             'indef_article': 'a',
             'name': 'map',
             'order': 2,
             'plural': 'maps',
             'singular': 'map',
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'icon': 'mdi-spotlight-beam',
             'indef_article': 'a',
             'name': 'beam',
             'order': 3,
             'plural': 'beams',
             'singular': 'beam',
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'icon': 'mdi-creation',
             'indef_article': 'a',
             'name': 'simulation',
             'order': 1,
             'plural': 'simulations',
             'singular': 'simulation',
-            'type_id': 3
+            'type_id': 3,
         },
         {
             'icon': '',
             'indef_article': '',
             'name': 'anchor',
             'order': 4,
             'plural': '',
             'singular': '',
-            'type_id': 4
-        }
+            'type_id': 4,
+        },
     ],
     'products': [
         {
             'name': 'lat20190213',
             'note': '''- This is a dummy test with a lat map
 - This should not depend on any beam''',
             'posting_git_hub_user_id': 1,
             'product_id': 1001,
             'time_posted': GenericRepr('datetime.datetime(2019, 2, 13, 10, 5, 23)'),
             'time_updated': None,
             'type_id': 1,
-            'updating_git_hub_user_id': 2
+            'updating_git_hub_user_id': 2,
         },
         {
             'name': 'xyz-s1234-20200101',
             'note': '''- note 1
 - note 2''',
             'posting_git_hub_user_id': 1,
             'product_id': 1002,
             'time_posted': GenericRepr('datetime.datetime(2019, 3, 15, 9, 11, 25)'),
             'time_updated': None,
             'type_id': 3,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20180101',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1010,
             'time_posted': GenericRepr('datetime.datetime(2018, 1, 1, 15, 32, 10)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': 'lat20200120',
             'note': '''- This is a dummy test with a lat map
 - A beam depends on this map''',
             'posting_git_hub_user_id': 1,
             'product_id': 1012,
             'time_posted': GenericRepr('datetime.datetime(2020, 1, 20, 18, 10, 5)'),
             'time_updated': None,
             'type_id': 1,
-            'updating_git_hub_user_id': 2
+            'updating_git_hub_user_id': 2,
         },
         {
             'name': 'lat20200201',
             'note': '''- This is a dummy test with a lat map
 - A beam depends on this map''',
             'posting_git_hub_user_id': 1,
             'product_id': 1013,
             'time_posted': GenericRepr('datetime.datetime(2020, 2, 1, 11, 5, 2)'),
             'time_updated': None,
             'type_id': 1,
-            'updating_git_hub_user_id': 2
+            'updating_git_hub_user_id': 2,
         },
         {
             'name': '20190304',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1070,
             'time_posted': GenericRepr('datetime.datetime(2019, 3, 4, 8, 12, 41)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20190607',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1120,
             'time_posted': GenericRepr('datetime.datetime(2019, 6, 7, 18, 21, 21)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20200123',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1130,
             'time_posted': GenericRepr('datetime.datetime(2020, 1, 23, 12, 11, 45)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20200207',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1150,
             'time_posted': GenericRepr('datetime.datetime(2020, 2, 7, 9, 42, 11)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
-        }
+            'updating_git_hub_user_id': None,
+        },
     ],
     'type_field_association': [
-        {
-            'field_id': 1,
-            'iid': 1,
-            'order': None,
-            'type_id': 1
-        },
-        {
-            'field_id': 2,
-            'iid': 2,
-            'order': None,
-            'type_id': 1
-        },
-        {
-            'field_id': 3,
-            'iid': 3,
-            'order': None,
-            'type_id': 1
-        },
-        {
-            'field_id': 1,
-            'iid': 4,
-            'order': None,
-            'type_id': 2
-        },
-        {
-            'field_id': 2,
-            'iid': 5,
-            'order': None,
-            'type_id': 2
-        },
-        {
-            'field_id': 3,
-            'iid': 6,
-            'order': None,
-            'type_id': 2
-        },
-        {
-            'field_id': 1,
-            'iid': 7,
-            'order': None,
-            'type_id': 3
-        },
-        {
-            'field_id': 2,
-            'iid': 8,
-            'order': None,
-            'type_id': 3
-        },
-        {
-            'field_id': 3,
-            'iid': 9,
-            'order': None,
-            'type_id': 3
-        },
-        {
-            'field_id': 1,
-            'iid': 10,
-            'order': None,
-            'type_id': 4
-        },
-        {
-            'field_id': 2,
-            'iid': 11,
-            'order': None,
-            'type_id': 4
-        },
-        {
-            'field_id': 3,
-            'iid': 12,
-            'order': None,
-            'type_id': 4
-        }
+        {'field_id': 1, 'iid': 1, 'order': None, 'type_id': 1},
+        {'field_id': 2, 'iid': 2, 'order': None, 'type_id': 1},
+        {'field_id': 3, 'iid': 3, 'order': None, 'type_id': 1},
+        {'field_id': 1, 'iid': 4, 'order': None, 'type_id': 2},
+        {'field_id': 2, 'iid': 5, 'order': None, 'type_id': 2},
+        {'field_id': 3, 'iid': 6, 'order': None, 'type_id': 2},
+        {'field_id': 1, 'iid': 7, 'order': None, 'type_id': 3},
+        {'field_id': 2, 'iid': 8, 'order': None, 'type_id': 3},
+        {'field_id': 3, 'iid': 9, 'order': None, 'type_id': 3},
+        {'field_id': 1, 'iid': 10, 'order': None, 'type_id': 4},
+        {'field_id': 2, 'iid': 11, 'order': None, 'type_id': 4},
+        {'field_id': 3, 'iid': 12, 'order': None, 'type_id': 4},
     ],
     'web_config': [
         {
             'id_': 1,
-            'json': '{"headTitle": "Product DB (test)", "toolbarTitle": "Product DB (test)", "devtoolLoadingstate": true, "productCreationDialog": false, "productUpdateDialog": true, "productDeletionDialog": false}'
+            'json': '{"headTitle": "Product DB (test)", "toolbarTitle": "Product DB (test)", "devtoolLoadingstate": true, "productCreationDialog": false, "productUpdateDialog": true, "productDeletionDialog": false}',
         }
-    ]
+    ],
 }
```

### Comparing `acondbs-0.4.3/tests/db/ops/snapshots/snap_test_export_dict.py` & `acondbs-0.4.4/tests/db/ops/snapshots/snap_test_import_csv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,635 +1,541 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import GenericRepr, Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_export_db_to_dict_of_dict_list 1'] = {
-    'account_admins': [
-        {
-            'admin_id': 1,
-            'git_hub_login': 'dojocat'
-        },
-        {
-            'admin_id': 2,
-            'git_hub_login': 'octocat'
-        }
-    ],
-    'attribute_boolean': [
-    ],
+snapshots['test_non_empty 1'] = {
+    'account_admins': [],
+    'attribute_boolean': [],
     'attribute_date': [
         {
             'field_id': 3,
             'iid': 1,
             'product_id': 1001,
             'type_field_association_iid': 3,
-            'value': GenericRepr('datetime.date(2019, 2, 13)')
+            'value': GenericRepr('datetime.date(2019, 2, 13)'),
         },
         {
             'field_id': 3,
             'iid': 2,
             'product_id': 1002,
             'type_field_association_iid': 9,
-            'value': GenericRepr('datetime.date(2019, 3, 15)')
+            'value': GenericRepr('datetime.date(2019, 3, 15)'),
         },
         {
             'field_id': 3,
             'iid': 3,
             'product_id': 1010,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2018, 1, 1)')
+            'value': GenericRepr('datetime.date(2018, 1, 1)'),
         },
         {
             'field_id': 3,
             'iid': 4,
             'product_id': 1012,
             'type_field_association_iid': 3,
-            'value': GenericRepr('datetime.date(2020, 1, 20)')
+            'value': GenericRepr('datetime.date(2020, 1, 20)'),
         },
         {
             'field_id': 3,
             'iid': 5,
             'product_id': 1013,
             'type_field_association_iid': 3,
-            'value': GenericRepr('datetime.date(2020, 2, 1)')
+            'value': GenericRepr('datetime.date(2020, 2, 1)'),
         },
         {
             'field_id': 3,
             'iid': 6,
             'product_id': 1070,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2019, 3, 4)')
+            'value': GenericRepr('datetime.date(2019, 3, 4)'),
         },
         {
             'field_id': 3,
             'iid': 7,
             'product_id': 1120,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2019, 6, 7)')
+            'value': GenericRepr('datetime.date(2019, 6, 7)'),
         },
         {
             'field_id': 3,
             'iid': 8,
             'product_id': 1130,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2020, 1, 23)')
+            'value': GenericRepr('datetime.date(2020, 1, 23)'),
         },
         {
             'field_id': 3,
             'iid': 9,
             'product_id': 1150,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2020, 2, 7)')
-        }
-    ],
-    'attribute_date_time': [
-    ],
-    'attribute_float': [
-    ],
-    'attribute_integer': [
-    ],
-    'attribute_time': [
+            'value': GenericRepr('datetime.date(2020, 2, 7)'),
+        },
     ],
+    'attribute_date_time': [],
+    'attribute_float': [],
+    'attribute_integer': [],
+    'attribute_time': [],
     'attribute_unicode_text': [
         {
             'field_id': 1,
             'iid': 2,
             'product_id': 1001,
             'type_field_association_iid': 1,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 3,
             'product_id': 1001,
             'type_field_association_iid': 2,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 8,
             'product_id': 1002,
             'type_field_association_iid': 7,
-            'value': 'abc-def'
+            'value': 'abc-def',
         },
         {
             'field_id': 2,
             'iid': 9,
             'product_id': 1002,
             'type_field_association_iid': 8,
-            'value': 'abc-def'
+            'value': 'abc-def',
         },
         {
             'field_id': 1,
             'iid': 14,
             'product_id': 1010,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 15,
             'product_id': 1010,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 20,
             'product_id': 1012,
             'type_field_association_iid': 1,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 21,
             'product_id': 1012,
             'type_field_association_iid': 2,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 26,
             'product_id': 1013,
             'type_field_association_iid': 1,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 27,
             'product_id': 1013,
             'type_field_association_iid': 2,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 32,
             'product_id': 1070,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 33,
             'product_id': 1070,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 38,
             'product_id': 1120,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 39,
             'product_id': 1120,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 44,
             'product_id': 1130,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 45,
             'product_id': 1130,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 50,
             'product_id': 1150,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 51,
             'product_id': 1150,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
-        }
-    ],
-    'field': [
-        {
-            'field_id': 1,
-            'name': 'contact',
-            'type_': 'UnicodeText'
-        },
-        {
-            'field_id': 2,
-            'name': 'produced_by',
-            'type_': 'UnicodeText'
+            'value': 'pwg-pmn',
         },
-        {
-            'field_id': 3,
-            'name': 'date_produced',
-            'type_': 'Date'
-        }
     ],
-    'github_org_memberships': [
+    'field': [
+        {'field_id': 1, 'name': 'contact', 'type_': 'UnicodeText'},
+        {'field_id': 2, 'name': 'produced_by', 'type_': 'UnicodeText'},
+        {'field_id': 3, 'name': 'date_produced', 'type_': 'Date'},
     ],
+    'github_org_memberships': [],
     'github_orgs': [
         {
             'avatar_url': 'https://avatars0.githubusercontent.com/u/75631844?v=4',
             'git_hub_id': '012:Organization75631844',
             'login': 'urban-octo-disco',
             'org_id': 1,
-            'url': 'https://github.com/urban-octo-disco'
+            'url': 'https://github.com/urban-octo-disco',
         }
     ],
     'github_tokens': [
         {
             'scope': 'read:org',
             'time_created': GenericRepr('datetime.datetime(2020, 1, 4, 14, 32, 15)'),
             'token': b'aKjGknYDHY39Z2xAaN7+sQ==',
             'token_id': 1,
-            'user_id': 1
+            'user_id': 1,
         }
     ],
     'github_users': [
         {
             'avatar_url': 'https://avatars3.githubusercontent.com/u/583231?v=4',
             'git_hub_id': '04:User583231',
             'login': 'octocat',
             'name': 'The Octocat',
             'url': 'https://github.com/octocat',
-            'user_id': 1
+            'user_id': 1,
         },
         {
             'avatar_url': 'https://avatars0.githubusercontent.com/u/9758946?v=4',
             'git_hub_id': '04:User9758946',
             'login': 'dojocat',
             'name': 'dojocat',
             'url': 'https://github.com/dojocat',
-            'user_id': 2
-        }
-    ],
-    'log': [
+            'user_id': 2,
+        },
     ],
+    'log': [],
     'product_file_paths': [
-        {
-            'note': '',
-            'path': 'nersc:/go/to/my/maps',
-            'path_id': 1,
-            'product_id': 1001
-        },
+        {'note': '', 'path': 'nersc:/go/to/my/maps', 'path_id': 1, 'product_id': 1001},
         {
             'note': 'lat only',
             'path': 'nersc:/go/to/my/maps_v2',
             'path_id': 2,
-            'product_id': 1012
+            'product_id': 1012,
         },
         {
             'note': 'lat only',
             'path': 'abcde:/path/to/the/maps_v2',
             'path_id': 3,
-            'product_id': 1012
+            'product_id': 1012,
         },
         {
             'note': 'lat only',
             'path': 'nersc:/go/to/my/maps_v3',
             'path_id': 4,
-            'product_id': 1013
+            'product_id': 1013,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20190304',
             'path_id': 5,
-            'product_id': 1070
+            'product_id': 1070,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20190607',
             'path_id': 6,
-            'product_id': 1120
+            'product_id': 1120,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20200123',
             'path_id': 7,
-            'product_id': 1130
+            'product_id': 1130,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20200207',
             'path_id': 8,
-            'product_id': 1150
+            'product_id': 1150,
         },
         {
             'note': '',
             'path': 'nersc:/go/to/my/simulations',
             'path_id': 9,
-            'product_id': 1002
+            'product_id': 1002,
         },
         {
             'note': '',
             'path': 'abcde:/path/to/the/simulations',
             'path_id': 10,
-            'product_id': 1002
-        }
+            'product_id': 1002,
+        },
     ],
     'product_relation_types': [
         {
             'indef_article': 'a',
             'name': 'parent',
             'plural': 'parents',
             'reverse_type_id': 2,
             'singular': 'parent',
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'indef_article': 'a',
             'name': 'child',
             'plural': 'children',
             'reverse_type_id': 1,
             'singular': 'child',
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'indef_article': 'a',
             'name': 'plaintiff',
             'plural': 'plaintiffs',
             'reverse_type_id': 4,
             'singular': 'plaintiff',
-            'type_id': 3
+            'type_id': 3,
         },
         {
             'indef_article': 'a',
             'name': 'defendant',
             'plural': 'defendants',
             'reverse_type_id': 3,
             'singular': 'defendant',
-            'type_id': 4
-        }
+            'type_id': 4,
+        },
     ],
     'product_relations': [
         {
             'other_product_id': 1012,
             'relation_id': 1,
             'reverse_relation_id': 2,
             'self_product_id': 1130,
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'other_product_id': 1130,
             'relation_id': 2,
             'reverse_relation_id': 1,
             'self_product_id': 1012,
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'other_product_id': 1013,
             'relation_id': 3,
             'reverse_relation_id': 4,
             'self_product_id': 1150,
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'other_product_id': 1150,
             'relation_id': 4,
             'reverse_relation_id': 3,
             'self_product_id': 1013,
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'other_product_id': 1130,
             'relation_id': 5,
             'reverse_relation_id': 6,
             'self_product_id': 1150,
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'other_product_id': 1150,
             'relation_id': 6,
             'reverse_relation_id': 5,
             'self_product_id': 1130,
-            'type_id': 2
-        }
+            'type_id': 2,
+        },
     ],
     'product_types': [
         {
             'icon': 'mdi-map',
             'indef_article': 'a',
             'name': 'map',
             'order': 2,
             'plural': 'maps',
             'singular': 'map',
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'icon': 'mdi-spotlight-beam',
             'indef_article': 'a',
             'name': 'beam',
             'order': 3,
             'plural': 'beams',
             'singular': 'beam',
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'icon': 'mdi-creation',
             'indef_article': 'a',
             'name': 'simulation',
             'order': 1,
             'plural': 'simulations',
             'singular': 'simulation',
-            'type_id': 3
+            'type_id': 3,
         },
         {
             'icon': '',
             'indef_article': '',
             'name': 'anchor',
             'order': 4,
             'plural': '',
             'singular': '',
-            'type_id': 4
-        }
+            'type_id': 4,
+        },
     ],
     'products': [
         {
             'name': 'lat20190213',
             'note': '''- This is a dummy test with a lat map
 - This should not depend on any beam''',
             'posting_git_hub_user_id': 1,
             'product_id': 1001,
             'time_posted': GenericRepr('datetime.datetime(2019, 2, 13, 10, 5, 23)'),
             'time_updated': None,
             'type_id': 1,
-            'updating_git_hub_user_id': 2
+            'updating_git_hub_user_id': 2,
         },
         {
             'name': 'xyz-s1234-20200101',
             'note': '''- note 1
 - note 2''',
             'posting_git_hub_user_id': 1,
             'product_id': 1002,
             'time_posted': GenericRepr('datetime.datetime(2019, 3, 15, 9, 11, 25)'),
             'time_updated': None,
             'type_id': 3,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20180101',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1010,
             'time_posted': GenericRepr('datetime.datetime(2018, 1, 1, 15, 32, 10)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': 'lat20200120',
             'note': '''- This is a dummy test with a lat map
 - A beam depends on this map''',
             'posting_git_hub_user_id': 1,
             'product_id': 1012,
             'time_posted': GenericRepr('datetime.datetime(2020, 1, 20, 18, 10, 5)'),
             'time_updated': None,
             'type_id': 1,
-            'updating_git_hub_user_id': 2
+            'updating_git_hub_user_id': 2,
         },
         {
             'name': 'lat20200201',
             'note': '''- This is a dummy test with a lat map
 - A beam depends on this map''',
             'posting_git_hub_user_id': 1,
             'product_id': 1013,
             'time_posted': GenericRepr('datetime.datetime(2020, 2, 1, 11, 5, 2)'),
             'time_updated': None,
             'type_id': 1,
-            'updating_git_hub_user_id': 2
+            'updating_git_hub_user_id': 2,
         },
         {
             'name': '20190304',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1070,
             'time_posted': GenericRepr('datetime.datetime(2019, 3, 4, 8, 12, 41)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20190607',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1120,
             'time_posted': GenericRepr('datetime.datetime(2019, 6, 7, 18, 21, 21)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20200123',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1130,
             'time_posted': GenericRepr('datetime.datetime(2020, 1, 23, 12, 11, 45)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20200207',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1150,
             'time_posted': GenericRepr('datetime.datetime(2020, 2, 7, 9, 42, 11)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
-        }
+            'updating_git_hub_user_id': None,
+        },
     ],
     'type_field_association': [
-        {
-            'field_id': 1,
-            'iid': 1,
-            'order': None,
-            'type_id': 1
-        },
-        {
-            'field_id': 2,
-            'iid': 2,
-            'order': None,
-            'type_id': 1
-        },
-        {
-            'field_id': 3,
-            'iid': 3,
-            'order': None,
-            'type_id': 1
-        },
-        {
-            'field_id': 1,
-            'iid': 4,
-            'order': None,
-            'type_id': 2
-        },
-        {
-            'field_id': 2,
-            'iid': 5,
-            'order': None,
-            'type_id': 2
-        },
-        {
-            'field_id': 3,
-            'iid': 6,
-            'order': None,
-            'type_id': 2
-        },
-        {
-            'field_id': 1,
-            'iid': 7,
-            'order': None,
-            'type_id': 3
-        },
-        {
-            'field_id': 2,
-            'iid': 8,
-            'order': None,
-            'type_id': 3
-        },
-        {
-            'field_id': 3,
-            'iid': 9,
-            'order': None,
-            'type_id': 3
-        },
-        {
-            'field_id': 1,
-            'iid': 10,
-            'order': None,
-            'type_id': 4
-        },
-        {
-            'field_id': 2,
-            'iid': 11,
-            'order': None,
-            'type_id': 4
-        },
-        {
-            'field_id': 3,
-            'iid': 12,
-            'order': None,
-            'type_id': 4
-        }
+        {'field_id': 1, 'iid': 1, 'order': None, 'type_id': 1},
+        {'field_id': 2, 'iid': 2, 'order': None, 'type_id': 1},
+        {'field_id': 3, 'iid': 3, 'order': None, 'type_id': 1},
+        {'field_id': 1, 'iid': 4, 'order': None, 'type_id': 2},
+        {'field_id': 2, 'iid': 5, 'order': None, 'type_id': 2},
+        {'field_id': 3, 'iid': 6, 'order': None, 'type_id': 2},
+        {'field_id': 1, 'iid': 7, 'order': None, 'type_id': 3},
+        {'field_id': 2, 'iid': 8, 'order': None, 'type_id': 3},
+        {'field_id': 3, 'iid': 9, 'order': None, 'type_id': 3},
+        {'field_id': 1, 'iid': 10, 'order': None, 'type_id': 4},
+        {'field_id': 2, 'iid': 11, 'order': None, 'type_id': 4},
+        {'field_id': 3, 'iid': 12, 'order': None, 'type_id': 4},
     ],
     'web_config': [
         {
             'id_': 1,
-            'json': '{"headTitle": "Product DB (test)", "toolbarTitle": "Product DB (test)", "devtoolLoadingstate": true, "productCreationDialog": false, "productUpdateDialog": true, "productDeletionDialog": false}'
+            'json': '{"headTitle": "Product DB (test)", "toolbarTitle": "Product DB (test)", "devtoolLoadingstate": true, "productCreationDialog": false, "productUpdateDialog": true, "productDeletionDialog": false}',
         }
-    ]
+    ],
 }
```

### Comparing `acondbs-0.4.3/tests/db/ops/snapshots/snap_test_import_csv.py` & `acondbs-0.4.4/tests/db/ops/snapshots/snap_test_export_dict.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,627 +1,544 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import GenericRepr, Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_non_empty 1'] = {
+snapshots['test_export_db_to_dict_of_dict_list 1'] = {
     'account_admins': [
+        {'admin_id': 1, 'git_hub_login': 'dojocat'},
+        {'admin_id': 2, 'git_hub_login': 'octocat'},
     ],
-    'attribute_boolean': [
-    ],
+    'attribute_boolean': [],
     'attribute_date': [
         {
             'field_id': 3,
             'iid': 1,
             'product_id': 1001,
             'type_field_association_iid': 3,
-            'value': GenericRepr('datetime.date(2019, 2, 13)')
+            'value': GenericRepr('datetime.date(2019, 2, 13)'),
         },
         {
             'field_id': 3,
             'iid': 2,
             'product_id': 1002,
             'type_field_association_iid': 9,
-            'value': GenericRepr('datetime.date(2019, 3, 15)')
+            'value': GenericRepr('datetime.date(2019, 3, 15)'),
         },
         {
             'field_id': 3,
             'iid': 3,
             'product_id': 1010,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2018, 1, 1)')
+            'value': GenericRepr('datetime.date(2018, 1, 1)'),
         },
         {
             'field_id': 3,
             'iid': 4,
             'product_id': 1012,
             'type_field_association_iid': 3,
-            'value': GenericRepr('datetime.date(2020, 1, 20)')
+            'value': GenericRepr('datetime.date(2020, 1, 20)'),
         },
         {
             'field_id': 3,
             'iid': 5,
             'product_id': 1013,
             'type_field_association_iid': 3,
-            'value': GenericRepr('datetime.date(2020, 2, 1)')
+            'value': GenericRepr('datetime.date(2020, 2, 1)'),
         },
         {
             'field_id': 3,
             'iid': 6,
             'product_id': 1070,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2019, 3, 4)')
+            'value': GenericRepr('datetime.date(2019, 3, 4)'),
         },
         {
             'field_id': 3,
             'iid': 7,
             'product_id': 1120,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2019, 6, 7)')
+            'value': GenericRepr('datetime.date(2019, 6, 7)'),
         },
         {
             'field_id': 3,
             'iid': 8,
             'product_id': 1130,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2020, 1, 23)')
+            'value': GenericRepr('datetime.date(2020, 1, 23)'),
         },
         {
             'field_id': 3,
             'iid': 9,
             'product_id': 1150,
             'type_field_association_iid': 6,
-            'value': GenericRepr('datetime.date(2020, 2, 7)')
-        }
-    ],
-    'attribute_date_time': [
-    ],
-    'attribute_float': [
-    ],
-    'attribute_integer': [
-    ],
-    'attribute_time': [
+            'value': GenericRepr('datetime.date(2020, 2, 7)'),
+        },
     ],
+    'attribute_date_time': [],
+    'attribute_float': [],
+    'attribute_integer': [],
+    'attribute_time': [],
     'attribute_unicode_text': [
         {
             'field_id': 1,
             'iid': 2,
             'product_id': 1001,
             'type_field_association_iid': 1,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 3,
             'product_id': 1001,
             'type_field_association_iid': 2,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 8,
             'product_id': 1002,
             'type_field_association_iid': 7,
-            'value': 'abc-def'
+            'value': 'abc-def',
         },
         {
             'field_id': 2,
             'iid': 9,
             'product_id': 1002,
             'type_field_association_iid': 8,
-            'value': 'abc-def'
+            'value': 'abc-def',
         },
         {
             'field_id': 1,
             'iid': 14,
             'product_id': 1010,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 15,
             'product_id': 1010,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 20,
             'product_id': 1012,
             'type_field_association_iid': 1,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 21,
             'product_id': 1012,
             'type_field_association_iid': 2,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 26,
             'product_id': 1013,
             'type_field_association_iid': 1,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 27,
             'product_id': 1013,
             'type_field_association_iid': 2,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 32,
             'product_id': 1070,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 33,
             'product_id': 1070,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 38,
             'product_id': 1120,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 39,
             'product_id': 1120,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 44,
             'product_id': 1130,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 45,
             'product_id': 1130,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 1,
             'iid': 50,
             'product_id': 1150,
             'type_field_association_iid': 4,
-            'value': 'pwg-pmn'
+            'value': 'pwg-pmn',
         },
         {
             'field_id': 2,
             'iid': 51,
             'product_id': 1150,
             'type_field_association_iid': 5,
-            'value': 'pwg-pmn'
-        }
-    ],
-    'field': [
-        {
-            'field_id': 1,
-            'name': 'contact',
-            'type_': 'UnicodeText'
+            'value': 'pwg-pmn',
         },
-        {
-            'field_id': 2,
-            'name': 'produced_by',
-            'type_': 'UnicodeText'
-        },
-        {
-            'field_id': 3,
-            'name': 'date_produced',
-            'type_': 'Date'
-        }
     ],
-    'github_org_memberships': [
+    'field': [
+        {'field_id': 1, 'name': 'contact', 'type_': 'UnicodeText'},
+        {'field_id': 2, 'name': 'produced_by', 'type_': 'UnicodeText'},
+        {'field_id': 3, 'name': 'date_produced', 'type_': 'Date'},
     ],
+    'github_org_memberships': [],
     'github_orgs': [
         {
             'avatar_url': 'https://avatars0.githubusercontent.com/u/75631844?v=4',
             'git_hub_id': '012:Organization75631844',
             'login': 'urban-octo-disco',
             'org_id': 1,
-            'url': 'https://github.com/urban-octo-disco'
+            'url': 'https://github.com/urban-octo-disco',
         }
     ],
     'github_tokens': [
         {
             'scope': 'read:org',
             'time_created': GenericRepr('datetime.datetime(2020, 1, 4, 14, 32, 15)'),
             'token': b'aKjGknYDHY39Z2xAaN7+sQ==',
             'token_id': 1,
-            'user_id': 1
+            'user_id': 1,
         }
     ],
     'github_users': [
         {
             'avatar_url': 'https://avatars3.githubusercontent.com/u/583231?v=4',
             'git_hub_id': '04:User583231',
             'login': 'octocat',
             'name': 'The Octocat',
             'url': 'https://github.com/octocat',
-            'user_id': 1
+            'user_id': 1,
         },
         {
             'avatar_url': 'https://avatars0.githubusercontent.com/u/9758946?v=4',
             'git_hub_id': '04:User9758946',
             'login': 'dojocat',
             'name': 'dojocat',
             'url': 'https://github.com/dojocat',
-            'user_id': 2
-        }
-    ],
-    'log': [
+            'user_id': 2,
+        },
     ],
+    'log': [],
     'product_file_paths': [
-        {
-            'note': '',
-            'path': 'nersc:/go/to/my/maps',
-            'path_id': 1,
-            'product_id': 1001
-        },
+        {'note': '', 'path': 'nersc:/go/to/my/maps', 'path_id': 1, 'product_id': 1001},
         {
             'note': 'lat only',
             'path': 'nersc:/go/to/my/maps_v2',
             'path_id': 2,
-            'product_id': 1012
+            'product_id': 1012,
         },
         {
             'note': 'lat only',
             'path': 'abcde:/path/to/the/maps_v2',
             'path_id': 3,
-            'product_id': 1012
+            'product_id': 1012,
         },
         {
             'note': 'lat only',
             'path': 'nersc:/go/to/my/maps_v3',
             'path_id': 4,
-            'product_id': 1013
+            'product_id': 1013,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20190304',
             'path_id': 5,
-            'product_id': 1070
+            'product_id': 1070,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20190607',
             'path_id': 6,
-            'product_id': 1120
+            'product_id': 1120,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20200123',
             'path_id': 7,
-            'product_id': 1130
+            'product_id': 1130,
         },
         {
             'note': '',
             'path': 'BEAM_DEPOT/Beams/20200207',
             'path_id': 8,
-            'product_id': 1150
+            'product_id': 1150,
         },
         {
             'note': '',
             'path': 'nersc:/go/to/my/simulations',
             'path_id': 9,
-            'product_id': 1002
+            'product_id': 1002,
         },
         {
             'note': '',
             'path': 'abcde:/path/to/the/simulations',
             'path_id': 10,
-            'product_id': 1002
-        }
+            'product_id': 1002,
+        },
     ],
     'product_relation_types': [
         {
             'indef_article': 'a',
             'name': 'parent',
             'plural': 'parents',
             'reverse_type_id': 2,
             'singular': 'parent',
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'indef_article': 'a',
             'name': 'child',
             'plural': 'children',
             'reverse_type_id': 1,
             'singular': 'child',
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'indef_article': 'a',
             'name': 'plaintiff',
             'plural': 'plaintiffs',
             'reverse_type_id': 4,
             'singular': 'plaintiff',
-            'type_id': 3
+            'type_id': 3,
         },
         {
             'indef_article': 'a',
             'name': 'defendant',
             'plural': 'defendants',
             'reverse_type_id': 3,
             'singular': 'defendant',
-            'type_id': 4
-        }
+            'type_id': 4,
+        },
     ],
     'product_relations': [
         {
             'other_product_id': 1012,
             'relation_id': 1,
             'reverse_relation_id': 2,
             'self_product_id': 1130,
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'other_product_id': 1130,
             'relation_id': 2,
             'reverse_relation_id': 1,
             'self_product_id': 1012,
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'other_product_id': 1013,
             'relation_id': 3,
             'reverse_relation_id': 4,
             'self_product_id': 1150,
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'other_product_id': 1150,
             'relation_id': 4,
             'reverse_relation_id': 3,
             'self_product_id': 1013,
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'other_product_id': 1130,
             'relation_id': 5,
             'reverse_relation_id': 6,
             'self_product_id': 1150,
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'other_product_id': 1150,
             'relation_id': 6,
             'reverse_relation_id': 5,
             'self_product_id': 1130,
-            'type_id': 2
-        }
+            'type_id': 2,
+        },
     ],
     'product_types': [
         {
             'icon': 'mdi-map',
             'indef_article': 'a',
             'name': 'map',
             'order': 2,
             'plural': 'maps',
             'singular': 'map',
-            'type_id': 1
+            'type_id': 1,
         },
         {
             'icon': 'mdi-spotlight-beam',
             'indef_article': 'a',
             'name': 'beam',
             'order': 3,
             'plural': 'beams',
             'singular': 'beam',
-            'type_id': 2
+            'type_id': 2,
         },
         {
             'icon': 'mdi-creation',
             'indef_article': 'a',
             'name': 'simulation',
             'order': 1,
             'plural': 'simulations',
             'singular': 'simulation',
-            'type_id': 3
+            'type_id': 3,
         },
         {
             'icon': '',
             'indef_article': '',
             'name': 'anchor',
             'order': 4,
             'plural': '',
             'singular': '',
-            'type_id': 4
-        }
+            'type_id': 4,
+        },
     ],
     'products': [
         {
             'name': 'lat20190213',
             'note': '''- This is a dummy test with a lat map
 - This should not depend on any beam''',
             'posting_git_hub_user_id': 1,
             'product_id': 1001,
             'time_posted': GenericRepr('datetime.datetime(2019, 2, 13, 10, 5, 23)'),
             'time_updated': None,
             'type_id': 1,
-            'updating_git_hub_user_id': 2
+            'updating_git_hub_user_id': 2,
         },
         {
             'name': 'xyz-s1234-20200101',
             'note': '''- note 1
 - note 2''',
             'posting_git_hub_user_id': 1,
             'product_id': 1002,
             'time_posted': GenericRepr('datetime.datetime(2019, 3, 15, 9, 11, 25)'),
             'time_updated': None,
             'type_id': 3,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20180101',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1010,
             'time_posted': GenericRepr('datetime.datetime(2018, 1, 1, 15, 32, 10)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': 'lat20200120',
             'note': '''- This is a dummy test with a lat map
 - A beam depends on this map''',
             'posting_git_hub_user_id': 1,
             'product_id': 1012,
             'time_posted': GenericRepr('datetime.datetime(2020, 1, 20, 18, 10, 5)'),
             'time_updated': None,
             'type_id': 1,
-            'updating_git_hub_user_id': 2
+            'updating_git_hub_user_id': 2,
         },
         {
             'name': 'lat20200201',
             'note': '''- This is a dummy test with a lat map
 - A beam depends on this map''',
             'posting_git_hub_user_id': 1,
             'product_id': 1013,
             'time_posted': GenericRepr('datetime.datetime(2020, 2, 1, 11, 5, 2)'),
             'time_updated': None,
             'type_id': 1,
-            'updating_git_hub_user_id': 2
+            'updating_git_hub_user_id': 2,
         },
         {
             'name': '20190304',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1070,
             'time_posted': GenericRepr('datetime.datetime(2019, 3, 4, 8, 12, 41)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20190607',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1120,
             'time_posted': GenericRepr('datetime.datetime(2019, 6, 7, 18, 21, 21)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20200123',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1130,
             'time_posted': GenericRepr('datetime.datetime(2020, 1, 23, 12, 11, 45)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
+            'updating_git_hub_user_id': None,
         },
         {
             'name': '20200207',
             'note': '- test entry',
             'posting_git_hub_user_id': 1,
             'product_id': 1150,
             'time_posted': GenericRepr('datetime.datetime(2020, 2, 7, 9, 42, 11)'),
             'time_updated': None,
             'type_id': 2,
-            'updating_git_hub_user_id': None
-        }
+            'updating_git_hub_user_id': None,
+        },
     ],
     'type_field_association': [
-        {
-            'field_id': 1,
-            'iid': 1,
-            'order': None,
-            'type_id': 1
-        },
-        {
-            'field_id': 2,
-            'iid': 2,
-            'order': None,
-            'type_id': 1
-        },
-        {
-            'field_id': 3,
-            'iid': 3,
-            'order': None,
-            'type_id': 1
-        },
-        {
-            'field_id': 1,
-            'iid': 4,
-            'order': None,
-            'type_id': 2
-        },
-        {
-            'field_id': 2,
-            'iid': 5,
-            'order': None,
-            'type_id': 2
-        },
-        {
-            'field_id': 3,
-            'iid': 6,
-            'order': None,
-            'type_id': 2
-        },
-        {
-            'field_id': 1,
-            'iid': 7,
-            'order': None,
-            'type_id': 3
-        },
-        {
-            'field_id': 2,
-            'iid': 8,
-            'order': None,
-            'type_id': 3
-        },
-        {
-            'field_id': 3,
-            'iid': 9,
-            'order': None,
-            'type_id': 3
-        },
-        {
-            'field_id': 1,
-            'iid': 10,
-            'order': None,
-            'type_id': 4
-        },
-        {
-            'field_id': 2,
-            'iid': 11,
-            'order': None,
-            'type_id': 4
-        },
-        {
-            'field_id': 3,
-            'iid': 12,
-            'order': None,
-            'type_id': 4
-        }
+        {'field_id': 1, 'iid': 1, 'order': None, 'type_id': 1},
+        {'field_id': 2, 'iid': 2, 'order': None, 'type_id': 1},
+        {'field_id': 3, 'iid': 3, 'order': None, 'type_id': 1},
+        {'field_id': 1, 'iid': 4, 'order': None, 'type_id': 2},
+        {'field_id': 2, 'iid': 5, 'order': None, 'type_id': 2},
+        {'field_id': 3, 'iid': 6, 'order': None, 'type_id': 2},
+        {'field_id': 1, 'iid': 7, 'order': None, 'type_id': 3},
+        {'field_id': 2, 'iid': 8, 'order': None, 'type_id': 3},
+        {'field_id': 3, 'iid': 9, 'order': None, 'type_id': 3},
+        {'field_id': 1, 'iid': 10, 'order': None, 'type_id': 4},
+        {'field_id': 2, 'iid': 11, 'order': None, 'type_id': 4},
+        {'field_id': 3, 'iid': 12, 'order': None, 'type_id': 4},
     ],
     'web_config': [
         {
             'id_': 1,
-            'json': '{"headTitle": "Product DB (test)", "toolbarTitle": "Product DB (test)", "devtoolLoadingstate": true, "productCreationDialog": false, "productUpdateDialog": true, "productDeletionDialog": false}'
+            'json': '{"headTitle": "Product DB (test)", "toolbarTitle": "Product DB (test)", "devtoolLoadingstate": true, "productCreationDialog": false, "productUpdateDialog": true, "productDeletionDialog": false}',
         }
-    ]
+    ],
 }
```

### Comparing `acondbs-0.4.3/tests/db/ops/test_csv_specification.py` & `acondbs-0.4.4/tests/db/ops/test_csv_specification.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import csv
 
 import pytest
 
-##__________________________________________________________________||
 multiline_entry = """\
 "abc
 xyz",def,ghi\
 """
 
 params = [
     pytest.param(
@@ -49,10 +48,7 @@
     This test is used to check the CSV specification as implemented in
     csv.reader(), in particular, to understand how quotes are treated
     and how to include double quotes, commas, and line breaks in data
 
     """
     rows = list(csv.reader(input))
     assert expected == rows
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/db/ops/test_define_tables.py` & `acondbs-0.4.4/tests/db/ops/test_define_tables.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-from sqlalchemy import MetaData
-
 import pytest
+from sqlalchemy import MetaData
 
 from acondbs import create_app
 from acondbs.db.ops import define_tables
 from acondbs.db.sa import sa
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app_with_empty_db():
     database_uri = "sqlite:///:memory:"
     app = create_app(SQLALCHEMY_DATABASE_URI=database_uri)
     yield app
 
 
-##__________________________________________________________________||
 def test_define_tables_start_with_empty_db(app_with_empty_db, snapshot):
     """test define_tables()
 
     This function tests if tables will be defined starting from new db without
     any tables.
 
     """
@@ -37,15 +34,14 @@
 
     with app.app_context():
         metadata = MetaData()
         metadata.reflect(bind=sa.engine)
         snapshot.assert_match(metadata.tables)
 
 
-##__________________________________________________________________||
 def test_define_tables_start_with_nonempty_db(app, snapshot):
     """test define_tables()
 
     This function tests if tables will be redefined starting from db
     with tables with entries.
 
     """
@@ -74,10 +70,7 @@
         total_nentries = sum(
             [
                 len([r for r in sa.engine.execute(tbl.select())])
                 for tbl in metadata.sorted_tables
             ]
         )
         assert total_nentries == 0
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/db/ops/test_export_csv.py` & `acondbs-0.4.4/tests/db/ops/test_export_csv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from pathlib import Path
+
 import pytest
 
 from acondbs import create_app
 from acondbs.db.ops import (
     define_tables,
-    import_tables_from_csv_files,
-    export_db_to_dict_of_dict_list,
     export_db_to_csv_files,
+    export_db_to_dict_of_dict_list,
+    import_tables_from_csv_files,
 )
 
 from ...constants import SAMPLE_DIR
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app():
     config_path = Path(SAMPLE_DIR, "config.py")
     database_uri = "sqlite:///:memory:"
-    app = create_app(
-        config_path=config_path, SQLALCHEMY_DATABASE_URI=database_uri
-    )
+    app = create_app(config_path=config_path, SQLALCHEMY_DATABASE_URI=database_uri)
     csvdir = Path(SAMPLE_DIR, "csv")
     with app.app_context():
         define_tables()
         import_tables_from_csv_files(csvdir)
     yield app
 
 
-##__________________________________________________________________||
 def test_export_db_to_csv_files(app, tmpdir_factory, snapshot):
     outdir = str(tmpdir_factory.mktemp("csv"))
 
     with app.app_context():
         export_db_to_csv_files(outdir)
 
     with app.app_context():
         define_tables()
         import_tables_from_csv_files(outdir)
         snapshot.assert_match(export_db_to_dict_of_dict_list())
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/db/ops/test_import_convert_str.py` & `acondbs-0.4.4/tests/db/ops/test_import_convert_str.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import csv
-from io import StringIO
-
 import datetime
+from io import StringIO
 
-from sqlalchemy import MetaData
+import pytest
 from flask_sqlalchemy import SQLAlchemy
+from sqlalchemy import MetaData
 from sqlalchemy_utils import EncryptedType
 
-import pytest
-
 from acondbs import create_app
 from acondbs.db.ops import convert_data_type_for_insert
 
-
-##__________________________________________________________________||
 sa = SQLAlchemy()
 
 
 class SampleTable(sa.Model):
     __tablename__ = "sample_table"
     id_ = sa.Column(sa.Integer(), primary_key=True)
 
@@ -29,15 +25,14 @@
     float = sa.Column(sa.Float())
     date = sa.Column(sa.Date())
     date_time = sa.Column(sa.DateTime())
     time = sa.Column(sa.Time())
     encrypted = sa.Column(EncryptedType(sa.Text(), "8b5d3d25b3e5"))
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app_with_empty_db():
     database_uri = "sqlite:///:memory:"
     app = create_app(SQLALCHEMY_DATABASE_URI=database_uri)
     yield app
 
 
@@ -51,15 +46,14 @@
         metadata = MetaData()
         metadata.reflect(bind=engine)
         metadata.drop_all(bind=engine)
         sa.Model.metadata.create_all(engine)
     yield app
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         dict(
             text="abcde",
             unicode_text="絵文字😀 😃 😄 😁 😆",
             boolean=False,
             integer=512,
@@ -128,15 +122,14 @@
 
         # empty the table
         SampleTable.query.delete()
         sa.session.commit()
 
     # import from the csv
     with app.app_context():
-
         # confirm the table is empty
         assert SampleTable.query.count() == 0
 
         _import_tbl_from_csv(tbl_name, csv_str)
 
     # assert
     with app.app_context():
@@ -153,15 +146,14 @@
     csv_writer.writerows(result_proxy)
     ret = b.getvalue()
     b.close()
     return ret
 
 
 def _import_tbl_from_csv(tbl_name, csv_str):
-
     engine = sa.engine
     metadata = MetaData()
     metadata.reflect(bind=engine)
     tbl = metadata.tables[tbl_name]
 
     rows = list(csv.reader(StringIO(csv_str)))
     fields = rows[0]
@@ -175,10 +167,7 @@
             for f, t, e in zip(fields, field_types, r)
         }
         for r in rows
     ]
 
     ins = tbl.insert()
     sa.session.execute(ins, data)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/db/ops/test_import_csv.py` & `acondbs-0.4.4/tests/db/ops/test_import_csv.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,41 @@
 from pathlib import Path
+
 import pytest
 
 from acondbs import create_app
 from acondbs.db.ops import (
     define_tables,
-    import_tables_from_csv_files,
-    export_db_to_dict_of_dict_list,
     export_db_to_csv_files,
+    export_db_to_dict_of_dict_list,
+    import_tables_from_csv_files,
 )
 
 from ...constants import SAMPLE_DIR
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app():
     config_path = Path(SAMPLE_DIR, "config.py")
     database_uri = "sqlite:///:memory:"
-    app = create_app(
-        config_path=config_path, SQLALCHEMY_DATABASE_URI=database_uri
-    )
+    app = create_app(config_path=config_path, SQLALCHEMY_DATABASE_URI=database_uri)
     with app.app_context():
         define_tables()
     yield app
 
 
-##__________________________________________________________________||
 def test_non_empty(app, snapshot):
     csvdir = Path(SAMPLE_DIR, "csv")
     with app.app_context():
         import_tables_from_csv_files(csvdir)
     with app.app_context():
         snapshot.assert_match(export_db_to_dict_of_dict_list())
 
 
-##__________________________________________________________________||
 def test_empty(app, tmpdir_factory):
     csvdir = str(tmpdir_factory.mktemp("csv"))
 
     with app.app_context():
         export_db_to_csv_files(csvdir)
 
     with app.app_context():
         import_tables_from_csv_files(csvdir)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/db/ops/test_import_csv_encrypted.py` & `acondbs-0.4.4/tests/db/ops/test_import_csv_encrypted.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 from pathlib import Path
+
 import pytest
 
 from acondbs import create_app
 from acondbs.db.ops import define_tables, import_tables_from_csv_files
-
-
 from acondbs.models import GitHubToken
 
 from ...constants import SAMPLE_DIR
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app():
     config_path = Path(SAMPLE_DIR, "config.py")
     database_uri = "sqlite:///:memory:"
-    app = create_app(
-        config_path=config_path, SQLALCHEMY_DATABASE_URI=database_uri
-    )
+    app = create_app(config_path=config_path, SQLALCHEMY_DATABASE_URI=database_uri)
     with app.app_context():
         define_tables()
     yield app
 
 
-##__________________________________________________________________||
 def test_encrypted_field(app):
     csvdir = Path(SAMPLE_DIR, "csv")
     with app.app_context():
         import_tables_from_csv_files(csvdir)
         assert "token123" == GitHubToken.query.one().token
 
 
@@ -42,10 +37,7 @@
 
     engine = AesEngine()
     engine._update_key(secret_key)
     engine._set_padding_mechanism(None)
 
     assert engine.encrypt(unencrypted) == encrypted
     assert engine.decrypt(encrypted) == unencrypted
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/db/test_cmds.py` & `acondbs-0.4.4/tests/db/test_cmds.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,36 @@
+import unittest.mock as mock
 from pathlib import Path
 
 import pytest
-import unittest.mock as mock
 
 from ..constants import SAMPLE_DIR
 
 
-##__________________________________________________________________||
 @pytest.fixture()
 def mock_define_tables(monkeypatch):
     ret = mock.Mock()
     monkeypatch.setattr("acondbs.db.cmds.define_tables", ret)
     return ret
 
 
 def test_init_db_command(runner, mock_define_tables):
     """test command init-db"""
     result = runner.invoke(args=["init-db"])
     assert [mock.call()] == mock_define_tables.call_args_list
     assert "Initialized" in result.output
 
 
-##__________________________________________________________________||
 def test_dump_db_command(runner):
     """test command dump-db"""
     result = runner.invoke(args=["dump-db"])
     assert 0 == result.exit_code
     assert 1800 < len(result.output)
 
 
-##__________________________________________________________________||
 @pytest.fixture()
 def mock_import_tables_from_csv_files(monkeypatch):
     ret = mock.Mock()
     monkeypatch.setattr("acondbs.db.cmds.import_tables_from_csv_files", ret)
     return ret
 
 
@@ -42,34 +39,26 @@
 
     csvdir = str(Path(SAMPLE_DIR, "csv"))
     # needs to give an existing path to `import-csv` as `click.Path()`
     # checks the check the existence.
 
     result = runner.invoke(args=["import-csv", csvdir])
     assert 0 == result.exit_code
-    assert [
-        mock.call(csvdir)
-    ] == mock_import_tables_from_csv_files.call_args_list
+    assert [mock.call(csvdir)] == mock_import_tables_from_csv_files.call_args_list
 
 
-##__________________________________________________________________||
 @pytest.fixture()
 def mock_export_db_to_csv_files(monkeypatch):
     ret = mock.Mock()
     monkeypatch.setattr("acondbs.db.cmds.export_db_to_csv_files", ret)
     return ret
 
 
-def test_export_csv_command(
-    runner, tmpdir_factory, mock_export_db_to_csv_files
-):
+def test_export_csv_command(runner, tmpdir_factory, mock_export_db_to_csv_files):
     """test command export-csv"""
 
     tmpdir = str(tmpdir_factory.mktemp("csv_out"))
     csvdir = str(Path(tmpdir, "csv"))
 
     result = runner.invoke(args=["export-csv", csvdir])
     assert 0 == result.exit_code
     assert [mock.call(csvdir)] == mock_export_db_to_csv_files.call_args_list
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/github/call/snapshots/snap_test_exchange_code_for_token.py` & `acondbs-0.4.4/tests/github/call/snapshots/snap_test_exchange_code_for_token.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,41 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_error 1'] = [
+    ((), {}),
     (
-        (
-        ),
-        {
-        }
-    ),
-    (
-        (
-            'https://github.com/login/oauth/access_token'
-        ,),
+        ('https://github.com/login/oauth/access_token',),
         {
-            'headers': {
-                'Accept': 'application/vnd.github.v3+json, application/json'
-            },
+            'headers': {'Accept': 'application/vnd.github.v3+json, application/json'},
             'json': {
                 'client_id': 'client_id_0123',
                 'client_secret': 'client_secret_0123',
                 'code': 'code-xyz',
                 'grant_type': 'authorization_code',
-                'redirect_uri': 'http://localhost/auth'
-            }
-        }
-    )
+                'redirect_uri': 'http://localhost/auth',
+            },
+        },
+    ),
 ]
 
 snapshots['test_success 1'] = [
+    ((), {}),
     (
-        (
-        ),
+        ('https://github.com/login/oauth/access_token',),
         {
-        }
-    ),
-    (
-        (
-            'https://github.com/login/oauth/access_token'
-        ,),
-        {
-            'headers': {
-                'Accept': 'application/vnd.github.v3+json, application/json'
-            },
+            'headers': {'Accept': 'application/vnd.github.v3+json, application/json'},
             'json': {
                 'client_id': 'client_id_0123',
                 'client_secret': 'client_secret_0123',
                 'code': 'code-xyz',
                 'grant_type': 'authorization_code',
-                'redirect_uri': 'http://localhost/auth'
-            }
-        }
-    )
+                'redirect_uri': 'http://localhost/auth',
+            },
+        },
+    ),
 ]
```

### Comparing `acondbs-0.4.3/tests/github/call/test_call_graphql_api.py` & `acondbs-0.4.4/tests/github/call/test_call_graphql_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,44 @@
+import unittest.mock as mock
 
 import pytest
-import unittest.mock as mock
 
 from acondbs.github.call import call_graphql_api
 
-##__________________________________________________________________||
+
 @pytest.fixture(autouse=True)
 def mock_requests(monkeypatch):
     y = mock.Mock()
     monkeypatch.setattr("acondbs.github.call.requests", y)
     yield y
 
 
-##__________________________________________________________________||
 def test_simple(mock_requests, snapshot):
-
     query = '{ viewer { login name avatarUrl } }'
     token = 'token-xxx'
 
     response = {
         "data": {
             "viewer": {
                 "login": "octocat",
                 "name": "The Octocat",
-                "avatarUrl": "https://avatars3.githubusercontent.com/u/583231?u=a59fef2a493e2b67dd13754231daf220c82ba84d&v=4"
+                "avatarUrl": "https://avatars3.githubusercontent.com/u/583231?u=a59fef2a493e2b67dd13754231daf220c82ba84d&v=4",
             }
         }
     }
     mock_requests.post().json.return_value = response
 
     r = call_graphql_api(query=query, token=token)
 
     assert response['data'] == r
 
     snapshot.assert_match(mock_requests.post.call_args_list)
 
-##__________________________________________________________________||
-def test_variables(mock_requests, snapshot):
 
+def test_variables(mock_requests, snapshot):
     query = '''
       query Organization($org_login: String!) {
         organization(login: $org_login) {
           login
           avatarUrl
         }
       }
@@ -50,31 +47,30 @@
     variables = {"org_login": "urban-octo-disco"}
 
     token = 'token-xxx'
 
     response = {
         "data": {
             "organization": {
-            "login": "urban-octo-disco",
-            "avatarUrl": "https://avatars0.githubusercontent.com/u/75631844?v=4"
+                "login": "urban-octo-disco",
+                "avatarUrl": "https://avatars0.githubusercontent.com/u/75631844?v=4",
             }
         }
     }
 
     mock_requests.post().json.return_value = response
 
     r = call_graphql_api(query=query, variables=variables, token=token)
 
     assert response['data'] == r
 
     snapshot.assert_match(mock_requests.post.call_args_list)
 
-##__________________________________________________________________||
-def test_error(mock_requests, snapshot):
 
+def test_error(mock_requests, snapshot):
     query = '''
       {
         viewer {
           login
           followers {
             edges {
               node {
@@ -88,46 +84,35 @@
 
     token = 'token-xxx'
 
     response = {
         "errors": [
             {
                 "type": "MISSING_PAGINATION_BOUNDARIES",
-                "path": [
-                    "viewer",
-                    "followers"
-                ],
-                "locations": [
-                    {
-                        "line": 9,
-                        "column": 5
-                    }
-                ],
-                "message": "You must provide a `first` or `last` value to properly paginate the `followers` connection."
+                "path": ["viewer", "followers"],
+                "locations": [{"line": 9, "column": 5}],
+                "message": "You must provide a `first` or `last` value to properly paginate the `followers` connection.",
             }
         ]
     }
     mock_requests.post().json.return_value = response
 
     with pytest.raises(Exception) as e:
         call_graphql_api(query=query, token=token)
 
     assert response['errors'] == e.value.args[0]
 
-##__________________________________________________________________||
-def test_bad_credentials(mock_requests):
 
+def test_bad_credentials(mock_requests):
     query = '{ viewer { login name avatarUrl } }'
     token = 'token-xxx'
 
     response = {
         'message': 'Bad credentials',
-        'documentation_url': 'https://docs.github.com/graphql'
+        'documentation_url': 'https://docs.github.com/graphql',
     }
     mock_requests.post().json.return_value = response
 
     with pytest.raises(Exception) as e:
         call_graphql_api(query=query, token=token)
 
     assert response == e.value.args[0]
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/github/call/test_exchange_code_for_token.py` & `acondbs-0.4.4/tests/github/call/test_exchange_code_for_token.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,58 @@
-import pytest
 import unittest.mock as mock
 
+import pytest
+
 from acondbs.github.call import exchange_code_for_token
 
-##__________________________________________________________________||
+
 @pytest.fixture(autouse=True)
 def mock_requests(monkeypatch):
     y = mock.Mock()
     monkeypatch.setattr("acondbs.github.call.requests", y)
     yield y
 
-##__________________________________________________________________||
-def test_success(mock_requests, snapshot):
 
+def test_success(mock_requests, snapshot):
     code = 'code-xyz'
 
     token_url = 'https://github.com/login/oauth/access_token'
     client_id = 'client_id_0123'
     client_secret = 'client_secret_0123'
     redirect_uri = 'http://localhost/auth'
 
-    return_value = {'access_token': 'token-xxx', 'token_type': 'bearer', 'scope': 'user'}
+    return_value = {
+        'access_token': 'token-xxx',
+        'token_type': 'bearer',
+        'scope': 'user',
+    }
     mock_requests.post().json.return_value = dict(return_value)
 
-    response = exchange_code_for_token(code, token_url, client_id, client_secret, redirect_uri)
+    response = exchange_code_for_token(
+        code, token_url, client_id, client_secret, redirect_uri
+    )
 
     assert return_value == response
     snapshot.assert_match(mock_requests.post.call_args_list)
 
-##__________________________________________________________________||
-def test_error(mock_requests, snapshot):
 
+def test_error(mock_requests, snapshot):
     code = 'code-xyz'
 
     token_url = 'https://github.com/login/oauth/access_token'
     client_id = 'client_id_0123'
     client_secret = 'client_secret_0123'
     redirect_uri = 'http://localhost/auth'
 
     response = {
         'error': 'bad_verification_code',
         'error_description': 'The code passed is incorrect or expired.',
-        'error_uri': 'https://docs.github.com/apps/managing-oauth-apps/troubleshooting-oauth-app-access-token-request-errors/#bad-verification-code'
+        'error_uri': 'https://docs.github.com/apps/managing-oauth-apps/troubleshooting-oauth-app-access-token-request-errors/#bad-verification-code',
     }
     mock_requests.post().json.return_value = response
 
     with pytest.raises(Exception) as e:
         exchange_code_for_token(code, token_url, client_id, client_secret, redirect_uri)
 
     assert response == e.value.args[0]
 
     snapshot.assert_match(mock_requests.post.call_args_list)
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/github/ops/test_exchange_code_for_token.py` & `acondbs-0.4.4/tests/github/ops/test_exchange_code_for_token.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-import pytest
 import unittest.mock as mock
 
+import pytest
+
 from acondbs.github.ops import exchange_code_for_token
 
-##__________________________________________________________________||
+
 @pytest.fixture(autouse=True)
 def mock_call(monkeypatch):
     y = mock.Mock()
     monkeypatch.setattr("acondbs.github.ops.call", y)
     yield y
 
-##__________________________________________________________________||
+
 def test_call(app, snapshot, mock_call):
     code = "kp5b8653"
     return_value = {'access_token': "wuk5phc8", 'token_type': 'bearer', 'scope': 'user'}
     mock_call.exchange_code_for_token.return_value = dict(return_value)
     with app.app_context():
         ret = exchange_code_for_token(code)
     assert ret == return_value
     snapshot.assert_match(mock_call.exchange_code_for_token.call_args_list)
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/github/query/test_viewer.py` & `acondbs-0.4.4/tests/github/query/test_viewer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,63 @@
+import unittest.mock as mock
 
 import pytest
-import unittest.mock as mock
 
 from acondbs.github import query
 
-##__________________________________________________________________||
+
 @pytest.fixture(autouse=True)
 def mock_requests(monkeypatch):
     y = mock.Mock()
     monkeypatch.setattr("acondbs.github.call.requests", y)
     yield y
 
 
-##__________________________________________________________________||
 def test_success(mock_requests):
-
     token = '4d5dc8b74eccdf65859d6ac64358a3a98300c351'
     # random string generated with
     # ''.join(random.choice('0123456789abcdef') for i in range(40))
 
     mock_requests.post().json.return_value = {
         'data': {
             'viewer': {
                 "id": "MDQ6VXNlcjU4MzIzMQ==",
                 "login": "octocat",
                 "name": "The Octocat",
                 "avatarUrl": "https://avatars3.githubusercontent.com/u/583231?u=a59fef2a493e2b67dd13754231daf220c82ba84d&v=4",
-                "url": "https://github.com/octocat"
+                "url": "https://github.com/octocat",
             }
         }
     }
 
     expected = {
         "id": "04:User583231",
         "login": "octocat",
         "name": "The Octocat",
         "avatarUrl": "https://avatars3.githubusercontent.com/u/583231?u=a59fef2a493e2b67dd13754231daf220c82ba84d&v=4",
-        "url": "https://github.com/octocat"
+        "url": "https://github.com/octocat",
     }
 
     actual = query.viewer(token)
 
     assert expected == actual
 
-##__________________________________________________________________||
-def test_bad_credentials(mock_requests):
 
+def test_bad_credentials(mock_requests):
     token = '4d5dc8b74eccdf65859d6ac64358a3a98300c351'
     # random string generated with
     # ''.join(random.choice('0123456789abcdef') for i in range(40))
 
     mock_requests.post().json.return_value = {
         'message': 'Bad credentials',
-        'documentation_url': 'https://docs.github.com/graphql'
+        'documentation_url': 'https://docs.github.com/graphql',
     }
 
     with pytest.raises(Exception) as e:
         query.viewer(token)
 
     expected = {
         'message': 'Bad credentials',
-        'documentation_url': 'https://docs.github.com/graphql'
+        'documentation_url': 'https://docs.github.com/graphql',
     }
 
     assert expected == e.value.args[0]
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/misc/gitb/test_commit.py` & `acondbs-0.4.4/tests/misc/gitb/test_commit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-import git
-
-from pathlib import Path
 import warnings
+from pathlib import Path
 
+import git
 import pytest
 
 from acondbs.misc import gitb
 
-##__________________________________________________________________||
+
 def test_empty_folder(tmpdir_factory):
-    """assert empty folder won't be initialized as a repo
-    """
+    """assert empty folder won't be initialized as a repo"""
     folder = Path(tmpdir_factory.mktemp('git'))
     with warnings.catch_warnings(record=True) as w:
         gitb.commit(folder)
     assert len(w) == 1
     assert not gitb.is_git_repo(folder)
 
-##__________________________________________________________________||
+
 @pytest.fixture()
 def nonexistent_path(tmpdir_factory):
-    """path to a nonexistent file
-    """
+    """path to a nonexistent file"""
     folder = Path(tmpdir_factory.mktemp('git'))
     path = folder.joinpath('nonexistent')
     yield path
 
+
 def test_nonexistent_path(nonexistent_path):
-    """assert exception is raised for nonexistent path
-    """
+    """assert exception is raised for nonexistent path"""
     with pytest.raises(ValueError):
         gitb.commit(nonexistent_path)
 
-##__________________________________________________________________||
+
 def test_non_empty_folder(folder):
-    """assert a repo initialized and files committed
-    """
+    """assert a repo initialized and files committed"""
     gitb.commit(folder)
     repo = git.Repo(folder)
     assert not repo.is_dirty(untracked_files=True)
     ncommits = len(list(repo.iter_commits()))
     assert 1 == ncommits
 
-##__________________________________________________________________||
+
 def test_clean_repo(repo):
-    """assert no empty commit is made
-    """
+    """assert no empty commit is made"""
     folder = repo.working_tree_dir
     with warnings.catch_warnings(record=True) as w:
         gitb.commit(folder)
     assert len(w) == 1
     assert not repo.is_dirty(untracked_files=True)
     ncommits = len(list(repo.iter_commits()))
     assert 1 == ncommits
 
+
 @pytest.fixture()
 def repo_dirty(repo):
     """a dirty repo
 
     The repo cotains a staged file, a modified file, a deleted file,
     and an untracked file.
 
@@ -69,30 +65,30 @@
     file1.write_text('xyz')
     repo.git.add(file1)
     file1.write_text('zzz')
     file2.unlink()
     file3.write_text('qwe')
     yield repo
 
+
 def test_dirty_repo(repo_dirty):
-    """assert all changes commit
-    """
+    """assert all changes commit"""
     repo = repo_dirty
     folder = repo.working_tree_dir
     gitb.commit(folder)
     assert not repo.is_dirty(untracked_files=True)
     ncommits = len(list(repo.iter_commits()))
     assert 2 == ncommits
 
+
 def test_default_message(repo_dirty):
     repo = repo_dirty
     folder = repo.working_tree_dir
     gitb.commit(folder)
     assert 'commit all' == repo.head.commit.message
 
+
 def test_custom_message(repo_dirty):
     repo = repo_dirty
     folder = repo.working_tree_dir
     gitb.commit(folder, 'custom message')
     assert 'custom message' == repo.head.commit.message
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/misc/gitb/test_pull.py` & `acondbs-0.4.4/tests/misc/gitb/test_pull.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import git
 from pathlib import Path
 
+import git
 import pytest
 
 from acondbs.misc import gitb
 
-##__________________________________________________________________||
-def test_pull(remote_url, tmpdir_factory):
-    """test pull()
 
-    """
+def test_pull(remote_url, tmpdir_factory):
+    """test pull()"""
 
     # create two clones
     folder1 = Path(tmpdir_factory.mktemp('git'))
     repo1 = git.Repo.clone_from(remote_url, folder1)
 
     folder2 = Path(tmpdir_factory.mktemp('git'))
     repo2 = git.Repo.clone_from(remote_url, folder2)
@@ -35,32 +33,29 @@
     gitb.pull(folder2)
 
     # assert
     head_sha_new = repo2.head.commit.hexsha
     assert not head_sha_old == head_sha_new
     assert head_sha_repo1 == head_sha_new
 
-##__________________________________________________________________||
+
 def test_nonexistent_path(tmpdir_factory):
-    """assert exception is raised for nonexistent path
-    """
+    """assert exception is raised for nonexistent path"""
     folder = Path(tmpdir_factory.mktemp('git'))
     path = folder.joinpath('nonexistent')
 
     with pytest.raises(ValueError):
         gitb.pull(path)
 
+
 def test_path_not_repo(folder):
-    """assert exception is raised if not a repo
-    """
+    """assert exception is raised if not a repo"""
 
     with pytest.raises(ValueError):
         gitb.pull(folder)
 
+
 def test_repo_no_remote(repo):
-    """assert exception is raised if a repo has no tracking branch
-    """
+    """assert exception is raised if a repo has no tracking branch"""
 
     with pytest.raises(ValueError):
         gitb.pull(repo.working_tree_dir)
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/misc/gitb/test_push.py` & `acondbs-0.4.4/tests/misc/gitb/test_push.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import git
 from pathlib import Path
 
+import git
 import pytest
 
 from acondbs.misc import gitb
 
-##__________________________________________________________________||
-def test_push(remote_url, tmpdir_factory):
-    """test push()
 
-    """
+def test_push(remote_url, tmpdir_factory):
+    """test push()"""
 
     # create two clones
     folder1 = Path(tmpdir_factory.mktemp('git'))
     repo1 = git.Repo.clone_from(remote_url, folder1)
 
     folder2 = Path(tmpdir_factory.mktemp('git'))
     repo2 = git.Repo.clone_from(remote_url, folder2)
@@ -38,32 +36,28 @@
 
     # assert
     remote2 = repo2.remotes[repo2.active_branch.tracking_branch().remote_name]
     remote2.pull()
     assert head_sha_new == repo2.head.commit.hexsha
 
 
-##__________________________________________________________________||
 def test_nonexistent_path(tmpdir_factory):
-    """assert exception is raised for nonexistent path
-    """
+    """assert exception is raised for nonexistent path"""
     folder = Path(tmpdir_factory.mktemp('git'))
     path = folder.joinpath('nonexistent')
 
     with pytest.raises(ValueError):
         gitb.push(path)
 
+
 def test_path_not_repo(folder):
-    """assert exception is raised if not a repo
-    """
+    """assert exception is raised if not a repo"""
 
     with pytest.raises(ValueError):
         gitb.push(folder)
 
+
 def test_repo_no_remote(repo):
-    """assert exception is raised if a repo has no tracking branch
-    """
+    """assert exception is raised if a repo has no tracking branch"""
 
     with pytest.raises(ValueError):
         gitb.push(repo.working_tree_dir)
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/misc/test_cap.py` & `acondbs-0.4.4/tests/misc/test_cap.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,89 @@
 import time
-from acondbs.misc.cap import cap_exec_rate
-from acondbs.misc.cap import State
+import unittest.mock as mock
 
 import pytest
-import unittest.mock as mock
 
-##__________________________________________________________________||
+from acondbs.misc.cap import State, cap_exec_rate
+
+
 class Task:
     def __init__(self):
         self.counter = 0
 
     def __call__(self):
         self.counter += 1
 
+
 def test_init():
     task = Task()
     cap = cap_exec_rate(func=task, pause_time=0.1)
     assert cap.func is task
     assert 0.1 == cap.pause_time
     assert not cap.daemon
     cap.end()
     assert 0 == task.counter
 
+
 def test_daemon():
     task = Task()
     cap = cap_exec_rate(func=task, pause_time=0.1, daemon=True)
     assert cap.daemon
     # end() doesn't need to be called
     assert 0 == task.counter
 
+
 def test_call():
     task = Task()
     cap = cap_exec_rate(func=task, pause_time=0.1)
     cap()
     time.sleep(0.05)
     assert 1 == task.counter
     cap.end()
 
+
 def test_call_2():
     task = Task()
     cap = cap_exec_rate(func=task, pause_time=0.05)
     cap()
     time.sleep(0.2)
     cap()
     time.sleep(0.05)
     assert 2 == task.counter
     cap.end()
 
+
 def test_call_3():
     task = Task()
     cap = cap_exec_rate(func=task, pause_time=0.1)
-    cap() # executed immediately
-    cap() # not executed
-    cap() # not executed
-    cap() # not executed
-    cap() # executed after the pause
+    cap()  # executed immediately
+    cap()  # not executed
+    cap()  # not executed
+    cap()  # not executed
+    cap()  # executed after the pause
     time.sleep(0.05)
     assert 1 == task.counter
     time.sleep(0.1)
     assert 2 == task.counter
     cap.end()
 
+
 def test_call_4():
     task = Task()
     cap = cap_exec_rate(func=task, pause_time=10)
-    cap() # executed immediately
-    cap() # not executed
-    cap() # not executed
-    cap() # not executed
-    cap() # executed at the end
+    cap()  # executed immediately
+    cap()  # not executed
+    cap()  # not executed
+    cap()  # not executed
+    cap()  # executed at the end
     time.sleep(0.05)
     assert 1 == task.counter
     cap.end()
     assert 2 == task.counter
 
-##__________________________________________________________________||
+
 def test_state_raise():
     config = mock.Mock()
     config.queue.get().return_value = 'unknown message'
     state = State(config)
     with pytest.raises(ValueError):
         state()
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/misc/test_lock.py` & `acondbs-0.4.4/tests/misc/test_lock.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,69 @@
+import unittest.mock as mock
 from pathlib import Path
 
-
 import pytest
-import unittest.mock as mock
 
-from acondbs.misc.lock import lock
-from acondbs.misc.lock import TimeOutAcquiringLock
+from acondbs.misc.lock import TimeOutAcquiringLock, lock
+
 
-##__________________________________________________________________||
 def test_acquire_release(tmpdir_factory):
     folder = Path(tmpdir_factory.mktemp('lock'))
     lock_file = folder.joinpath('.lock')
 
     l = lock(lock_file)
     assert not l.locked
     l.acquire()
     assert l.locked
     assert lock_file.exists()
     l.release()
     assert not l.locked
     assert not lock_file.exists()
 
-##__________________________________________________________________||
+
 def test_release_when_not_lockded(tmpdir_factory):
     folder = Path(tmpdir_factory.mktemp('lock'))
     lock_file = folder.joinpath('.lock')
 
     l = lock(lock_file)
     assert not l.locked
     l.release()
     assert not l.locked
     assert not lock_file.exists()
 
-##__________________________________________________________________||
+
 def test_release_not_delete_when_not_lockded(tmpdir_factory):
     folder = Path(tmpdir_factory.mktemp('lock'))
     lock_file = folder.joinpath('.lock')
 
     lock_file.touch()
 
     l = lock(lock_file)
     assert not l.locked
     l.release()
     assert not l.locked
     assert lock_file.exists()
 
-##__________________________________________________________________||
+
 def test_acquire_timeout(tmpdir_factory):
-    timeout = 0.1 # sec
+    timeout = 0.1  # sec
 
     folder = Path(tmpdir_factory.mktemp('lock'))
     lock_file = folder.joinpath('.lock')
 
     lock_file.touch()
 
     l = lock(lock_file, timeout=timeout)
 
     with pytest.raises(TimeOutAcquiringLock):
         l.acquire()
 
-##__________________________________________________________________||
+
 def test_with_success(tmpdir_factory):
     folder = Path(tmpdir_factory.mktemp('lock'))
     lock_file = folder.joinpath('.lock')
 
     with lock(lock_file) as l:
         assert l.locked
         assert lock_file.exists()
     assert not l.locked
     assert not lock_file.exists()
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/examples/test_add.py` & `acondbs-0.4.4/tests/models/examples/test_add.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 from acondbs.db.sa import sa
-from acondbs.models import ProductType, Product
+from acondbs.models import Product, ProductType
 
 # These tests are written primarily for the developer to understand
 # how models in flask_sqlalchemy work.
 
 
-##__________________________________________________________________||
 def test_simple(app):
     """A simple test of adding an object"""
 
     with app.app_context():
-
         # the number of the product types is zero initially
         assert 0 == len(ProductType.query.all())
 
     # this instantiation doesn't need be within a app context
     type1 = ProductType(name="type1")
 
     with app.app_context():
         sa.session.add(type1)
         sa.session.commit()
 
     with app.app_context():
-
         # the number of the product types is increased by one
         assert 1 == len(ProductType.query.all())
 
         # the new product type can be retrieved in a different app context
         type1_ = ProductType.query.filter_by(name="type1").one_or_none()
         assert isinstance(type1_, ProductType)
 
 
-##__________________________________________________________________||
 def test_python_object(app):
     """A simple test about Python object"""
 
     type1 = ProductType(name="type1")
 
     with app.app_context():
         sa.session.add(type1)
@@ -49,15 +45,14 @@
     with app.app_context():
         type1_ = ProductType.query.filter_by(name="type1").first()
 
         # In a different app context, no longer the same Python object
         assert type1 is not type1_
 
 
-##__________________________________________________________________||
 def test_primary_key(app):
     """A simple test about the primary key"""
 
     type1 = ProductType(name="type1")
 
     # The primary key (type_id) is None at this point
     assert type1.type_id is None
@@ -67,21 +62,19 @@
         sa.session.commit()
 
         # After the commit, type_id is automatically assigned
         type_id = type1.type_id
         assert type_id is not None
 
     with app.app_context():
-
         # The object can be retrived by the product_id in another context
         type1 = ProductType.query.filter_by(type_id=type_id).first()
         assert "type1" == type1.name
 
 
-##__________________________________________________________________||
 def test_relation(app):
     """A simple test of adding an object with relation"""
 
     type1 = ProductType(name="type1")
     product1 = Product(name="product1", type_=type1)
 
     # The relation has been already established
@@ -108,10 +101,7 @@
         product1 = Product.query.filter_by(name="product1").first()
 
         # The relation is preserved in a different app context
         type1 = product1.type_
         assert "type1" == type1.name
         assert product1 is type1.products[0]
         assert product1.type_id == type1.type_id
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/examples/test_date_time.py` & `acondbs-0.4.4/tests/models/examples/test_date_time.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
-import sqlalchemy
+
 import pytest
+import sqlalchemy
 
 from acondbs.db.sa import sa
-from acondbs.models import ProductType, Product
+from acondbs.models import Product, ProductType
 
 
-##__________________________________________________________________||
 def test_add(app):
     """A simple test of adding an object with a date field"""
 
     type1 = ProductType(name="type1")
 
     # time_posted needs to be initialized with a datetime.date
     time_posted = datetime.datetime(2019, 2, 23, 9, 10, 25)
@@ -22,35 +22,26 @@
 
     with app.app_context():
         product1 = Product.query.filter_by(name="product1").first()
 
         # The type of the field "time_posted" of Product is "datetime.date"
         assert isinstance(product1.time_posted, datetime.date)
 
-        assert (
-            datetime.datetime(2019, 2, 23, 9, 10, 25) == product1.time_posted
-        )
+        assert datetime.datetime(2019, 2, 23, 9, 10, 25) == product1.time_posted
 
 
-##__________________________________________________________________||
 def test_add_raise(app):
     """A simple test of adding an object with a wrong type"""
 
     type1 = ProductType(name="type1")
 
     # It is not impossible to instnaiate a date field with a wrong
     # type, e.g, str
-    product1 = Product(
-        name="product1", time_posted="2019-02-13 10:15:21", type_=type1
-    )
+    product1 = Product(name="product1", time_posted="2019-02-13 10:15:21", type_=type1)
 
     with app.app_context():
-
         # It is also possible to add
         sa.session.add(product1)
 
         # However, it is not possible to commit
         with pytest.raises(sqlalchemy.exc.StatementError):
             sa.session.commit()
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/examples/test_delete.py` & `acondbs-0.4.4/tests/models/examples/test_delete.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import pytest
 
 from acondbs.db.sa import sa
-from acondbs.models import ProductType, Product
+from acondbs.models import Product, ProductType
 
 # These tests are written primarily for the developer to understand
 # how models in flask_sqlalchemy work.
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app):
     y = app
 
     type_map = ProductType(name="map")
     map1 = Product(name="map1", type_=type_map)  # noqa: F841
     map2 = Product(name="map2", type_=type_map)  # noqa: F841
@@ -20,30 +19,24 @@
     with y.app_context():
         sa.session.add(type_map)
         sa.session.commit()
 
     yield y
 
 
-##__________________________________________________________________||
 def test_simple(app):
     """A simple test of deleting an object"""
 
     with app.app_context():
-
         assert 3 == len(Product.query.all())
 
     with app.app_context():
         product1 = Product.query.filter_by(name="map1").first()
         sa.session.delete(product1)
         sa.session.commit()
 
     with app.app_context():
-
         assert 2 == len(Product.query.all())
 
         # the product is no longer found
         product1 = Product.query.filter_by(name="map1").first()
         assert product1 is None
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/examples/test_query.py` & `acondbs-0.4.4/tests/models/examples/test_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import pytest
-
 from flask_sqlalchemy import BaseQuery
 
 from acondbs.db.sa import sa
-from acondbs.models import ProductType, Product
+from acondbs.models import Product, ProductType
 
 # These tests are written primarily for the developer to understand
 # how models in flask_sqlalchemy work.
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app):
     y = app
 
     type_map = ProductType(name="map")
     map1 = Product(name="map1", type_=type_map)  # noqa: F841
     map2 = Product(name="map2", type_=type_map)  # noqa: F841
@@ -22,44 +20,38 @@
     with y.app_context():
         sa.session.add(type_map)
         sa.session.commit()
 
     yield y
 
 
-##__________________________________________________________________||
 def test_context(app):
-
     # query cannot be accessed outside of the app context
     with pytest.raises(RuntimeError):
         Product.query
 
     with app.app_context():
         Product.query
 
 
 def test_query_all(app):
-
     with app.app_context():
-
         # query is an instance of BaseQuery
         query = Product.query
         assert isinstance(query, BaseQuery)
 
         # query.all() returns a list of products
         results = query.all()
         # e.g., [<Product 1>, <Product 2>, <Product 3>]
 
         assert isinstance(results[0], Product)
 
 
 def test_query_filter(app):
-
     with app.app_context():
-
         # filter_by() returns an instance of BaseQuery
         query = Product.query.filter_by(name="map1")
         assert isinstance(query, BaseQuery)
 
         # the results are a list with one element
         results = query.all()
         assert 1 == len(results)
@@ -68,23 +60,18 @@
         # first() returns a product
         product = query.first()
         assert isinstance(product, Product)
         assert "map1" == product.name
 
 
 def test_query_filter_nonexistent(app):
-
     with app.app_context():
-
         query = Product.query.filter_by(name="no-such-product")
         assert isinstance(query, BaseQuery)
 
         # the results are an empty list
         results = query.all()
         assert [] == results
 
         # first() returns None
         product = query.first()
         assert product is None
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/funcs/test_shorten.py` & `acondbs-0.4.4/tests/models/funcs/test_shorten.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 
 from acondbs.models.funcs import shorten
 
-
 params = [
     ("0123456789", dict(width=0), "..."),
     ("0123456789", dict(width=1), "..."),
     ("0123456789", dict(width=2), "..."),
     ("0123456789", dict(width=3), "..."),
     ("0123456789", dict(width=4), "0..."),
     ("0123456789", dict(width=5), "01..."),
```

### Comparing `acondbs-0.4.3/tests/models/github/github_org_membership/test_entry.py` & `acondbs-0.4.4/tests/models/github/github_org_membership/test_entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from acondbs.db.sa import sa
-from acondbs.models import GitHubOrg, GitHubUser, GitHubOrgMembership
+from acondbs.models import GitHubOrg, GitHubOrgMembership, GitHubUser
 
 
-##__________________________________________________________________||
 def test_relation(app):
-
     with app.app_context():
         membership = GitHubOrgMembership.query.one()
         org1 = GitHubOrg.query.one()
         user1 = GitHubUser.query.one()
         assert org1 == membership.org
         assert user1 == membership.member
         assert [membership] == org1.memberships
         assert [membership] == user1.memberships
 
 
-##__________________________________________________________________||
 def test_cascade_delete_org(app):
-
     with app.app_context():
         org1 = GitHubOrg.query.filter_by(login="org1").one()
         sa.session.delete(org1)
         sa.session.commit()
 
     with app.app_context():
         memberships = GitHubOrgMembership.query.all()
@@ -29,15 +25,14 @@
         users = GitHubUser.query.all()
         assert len(memberships) == 0
         assert len(orgs) == 0
         assert len(users) == 1
 
 
 def test_cascade_delete_user(app):
-
     with app.app_context():
         user1 = GitHubUser.query.filter_by(login="user1").one()
         sa.session.delete(user1)
         sa.session.commit()
 
     with app.app_context():
         memberships = GitHubOrgMembership.query.all()
@@ -45,23 +40,19 @@
         users = GitHubUser.query.all()
         assert len(memberships) == 0
         assert len(orgs) == 1
         assert len(users) == 0
 
 
 def test_cascade_delete_membership(app):
-
     with app.app_context():
         membership = GitHubOrgMembership.query.one()
         sa.session.delete(membership)
         sa.session.commit()
 
     with app.app_context():
         memberships = GitHubOrgMembership.query.all()
         orgs = GitHubOrg.query.all()
         users = GitHubUser.query.all()
         assert len(memberships) == 0
         assert len(orgs) == 1
         assert len(users) == 1
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/github/github_token/conftest.py` & `acondbs-0.4.4/tests/models/github/github_token/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 import pytest
 
 from acondbs.db.sa import sa
 from acondbs.models import GitHubToken, GitHubUser
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app_empty):
-
     y = app_empty
 
     #
     #  +-------+        +--------+
     #  | user1 | --+--> | token1 |
     #  +-------+   |    +--------+
     #              |
     #              |    +--------+
     #              +--> | token2 |
     #                   +--------+
     #
 
     user1 = GitHubUser(login="octocat", git_hub_id="04:User583231")
-    token1 = GitHubToken(  # noqa: F841
-        token="token_001", scope="read:org", user=user1
-    )
-    token2 = GitHubToken(  # noqa: F841
-        token="token_002", scope="read:org", user=user1
-    )
+    token1 = GitHubToken(token="token_001", scope="read:org", user=user1)  # noqa: F841
+    token2 = GitHubToken(token="token_002", scope="read:org", user=user1)  # noqa: F841
 
     with y.app_context():
         sa.session.add(user1)
         sa.session.commit()
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/github/github_token/test_model.py` & `acondbs-0.4.4/tests/models/github/github_token/test_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import datetime
 
 from acondbs.db.sa import sa
 from acondbs.models import GitHubToken, GitHubUser
 
 
-##__________________________________________________________________||
 def test_query(app):
-
     with app.app_context():
         user1 = GitHubUser.query.filter_by(login="octocat").one()
         token1, token2 = user1.tokens
 
         assert token1.token == "token_001"
         assert token1.scope == "read:org"
         assert token1.user == user1
 
         assert token2.token == "token_002"
         assert token2.scope == "read:org"
         assert token2.user == user1
 
 
-##__________________________________________________________________||
 def test_add(app):
-
     with app.app_context():
         user1 = GitHubUser.query.filter_by(login="octocat").one()
         ntokens = len(user1.tokens)  # = 2
         token3 = GitHubToken(token="token_003", scope="read:org", user=user1)
         sa.session.commit()
 
     with app.app_context():
@@ -42,17 +38,15 @@
             datetime.datetime(2021, 1, 4, 14, 32, 20) == token3.time_created
         )  # default value set in the fixture mock_datetime
         user1 = token3.user
         assert "octocat" == user1.login
         assert ntokens + 1 == len(user1.tokens)
 
 
-##__________________________________________________________________||
 def test_delete(app):
-
     with app.app_context():
         user1 = GitHubUser.query.filter_by(login="octocat").one()
         ntokens = len(user1.tokens)  # = 2
         token1 = user1.tokens[0]
         sa.session.delete(token1)
         sa.session.commit()
 
@@ -67,21 +61,16 @@
         sa.session.commit()
 
     with app.app_context():
         user1 = GitHubUser.query.filter_by(login="octocat").one()
         assert ntokens - 2 == len(user1.tokens)  # 0
 
 
-##__________________________________________________________________||
 def test_delete_cascade(app):
-
     with app.app_context():
         user1 = GitHubUser.query.filter_by(login="octocat").one()
         sa.session.delete(user1)
         sa.session.commit()
 
     with app.app_context():
         tokens = GitHubToken.query.all()
         assert 0 == len(tokens)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/github/github_user/test_entry.py` & `acondbs-0.4.4/tests/models/github/github_user/test_entry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from acondbs.db.sa import sa
 from acondbs.models import GitHubUser
 
 
-##__________________________________________________________________||
 def test_entry(app_empty):
     app = app_empty
 
     user1 = GitHubUser(
         login="octocat",
         git_hub_id="04:User583231",
         name="The Octocat",
@@ -16,10 +15,7 @@
     with app.app_context():
         sa.session.add(user1)
         sa.session.commit()
 
     with app.app_context():
         user1 = GitHubUser.query.filter_by(login="octocat").one()
         assert "octocat" == user1.login
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/misc/log/test_model.py` & `acondbs-0.4.4/tests/models/misc/log/test_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from acondbs.db.sa import sa
 from acondbs.models import Log
 
 
-##__________________________________________________________________||
 def test_column(app_empty):
     app = app_empty
 
     with app.app_context():
         model = Log(level="ERROR", message="an exception occurred")
         sa.session.add(model)
         sa.session.commit()
@@ -28,10 +27,7 @@
         sa.session.add(model)
         sa.session.commit()
         id_ = model.id_
 
     with app.app_context():
         model = Log.query.filter_by(id_=id_).one()
         repr(model)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/attribute/conftest.py` & `acondbs-0.4.4/tests/models/product/attribute/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,17 @@
-import pytest
-
 import datetime
 
+import pytest
+
 from acondbs.db.sa import sa
-from acondbs.models import (
-    ProductType,
-    FieldType,
-    Field,
-    TypeFieldAssociation,
-    Product,
-)
+from acondbs.models import Field, FieldType, Product, ProductType, TypeFieldAssociation
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app_empty):
-
     y = app_empty
 
     # create fields
     field1 = Field(name="attr1", type_=FieldType.UnicodeText)
     field2 = Field(name="date_produced", type_=FieldType.Date)
     field3 = Field(name="time_posted", type_=FieldType.DateTime)
     fields = [field1, field2, field3]
@@ -119,10 +111,7 @@
 
     with y.app_context():
         sa.session.add(Map)
         sa.session.add(Beam)
         sa.session.commit()
 
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/attribute/test_attribute.py` & `acondbs-0.4.4/tests/models/product/attribute/test_attribute.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,47 @@
 import datetime
-from sqlalchemy.orm import aliased
-
-import sqlparse
 
 import pytest
+import sqlparse
+from sqlalchemy.orm import aliased
 
 from acondbs.db.sa import sa
-
 from acondbs.models import (
-    Product,
-    ProductType,
-    FieldType,
-    Field,
-    TypeFieldAssociation,
-    AttributeUnicodeText,
     AttributeBoolean,
-    AttributeInteger,
-    AttributeFloat,
     AttributeDate,
     AttributeDateTime,
+    AttributeFloat,
+    AttributeInteger,
     AttributeTime,
+    AttributeUnicodeText,
+    Field,
+    FieldType,
+    Product,
+    ProductType,
+    TypeFieldAssociation,
 )
 
-
-##__________________________________________________________________||
 params = [
     pytest.param(
         FieldType.UnicodeText,
         AttributeUnicodeText,
         "value1 値１",
         id="UnicodeText",
     ),
     pytest.param(FieldType.Boolean, AttributeBoolean, True, id="Boolean"),
     pytest.param(FieldType.Integer, AttributeInteger, -512442, id="Integer"),
     pytest.param(FieldType.Float, AttributeFloat, 3.14592613, id="Float"),
-    pytest.param(
-        FieldType.Date, AttributeDate, datetime.date(2020, 2, 1), id="Date"
-    ),
+    pytest.param(FieldType.Date, AttributeDate, datetime.date(2020, 2, 1), id="Date"),
     pytest.param(
         FieldType.DateTime,
         AttributeDateTime,
         datetime.datetime(2020, 2, 1, 9, 10, 25),
         id="DateTime",
     ),
-    pytest.param(
-        FieldType.Time, AttributeTime, datetime.time(9, 10, 25), id="Time"
-    ),
+    pytest.param(FieldType.Time, AttributeTime, datetime.time(9, 10, 25), id="Time"),
 ]
 
 
 @pytest.mark.parametrize("field_type, AttributeClass, value", params)
 def test_repr(app_empty, field_type, AttributeClass, value):
     app = app_empty  # noqa: F841
 
@@ -106,27 +98,23 @@
         assert attr.field.name == "field1"
         assert attr.field.type_ is field_type
         assert attr.value == value
         assert getattr(attr.product, AttributeClass.backref_column) == [attr]
         assert getattr(attr.field, AttributeClass.backref_column) == [attr]
 
 
-##__________________________________________________________________||
 def test_filter(app):
-
     with app.app_context():
         expected = Product.query.filter_by(product_id=1).one()
         print(expected.attributes_unicode_text[0].type_field_association)
         query = (
             Product.query.join(AttributeUnicodeText)
             .join(TypeFieldAssociation)
             .join(Field)
-            .filter(
-                Field.name == "attr1", AttributeUnicodeText.value == "value1"
-            )
+            .filter(Field.name == "attr1", AttributeUnicodeText.value == "value1")
         )
         # print(sqlparse.format(str(query), reindent=True))
         actual = query.one()
         assert actual is expected
 
         # another way
         query = (
@@ -138,15 +126,14 @@
         )
         # print(sqlparse.format(str(query), reindent=True))
         actual = query.one()
         assert actual is expected
 
 
 def test_order(app):
-
     with app.app_context():
         map1 = Product.query.filter_by(product_id=1).one()
         map2 = Product.query.filter_by(product_id=2).one()
         map3 = Product.query.filter_by(product_id=3).one()
 
         expected = [map3, map2, map1]
 
@@ -163,15 +150,14 @@
         # print(sqlparse.format(str(query), reindent=True))
 
         actual = query.all()
 
         assert actual == expected
 
 
-##__________________________________________________________________||
 def test_order_nested(app_empty):
     app = app_empty
 
     field_attr1 = Field(name="attr1", type_=FieldType.UnicodeText)
     field_attr2 = Field(name="attr2", type_=FieldType.UnicodeText)
     Map = ProductType(type_id=1, name="map")
     assoc1 = TypeFieldAssociation(field=field_attr1)
@@ -247,15 +233,14 @@
     )
 
     with app.app_context():
         sa.session.add(Map)
         sa.session.commit()
 
     with app.app_context():
-
         map1 = Product.query.filter_by(product_id=1).one()
         map2 = Product.query.filter_by(product_id=2).one()
         map3 = Product.query.filter_by(product_id=3).one()
         map4 = Product.query.filter_by(product_id=4).one()
         map5 = Product.query.filter_by(product_id=5).one()
 
         expected = [map2, map4, map5, map1, map3]
@@ -276,31 +261,28 @@
             Product.query.join(ProductType)
             .filter_by(name="map")
             .join(AliasedAttributeUnicodeText1)
             .join(AliasedTypeFieldAssociation1)
             .join(AliasedField1)
             .filter_by(name="attr1")
             .order_by(AliasedAttributeUnicodeText1.value.desc())
-            .join(
-                AliasedAttributeUnicodeText2, Product.attributes_unicode_text
-            )
+            .join(AliasedAttributeUnicodeText2, Product.attributes_unicode_text)
             .join(AliasedTypeFieldAssociation2)
             .join(AliasedField2)
             .filter_by(name="attr2")
             .order_by(AliasedAttributeUnicodeText2.value)
         )
 
         # print(sqlparse.format(str(query), reindent=True))
 
         actual = query.all()
 
         assert actual == expected
 
 
-##__________________________________________________________________||
 def test_delte_orphan_product(app_empty):
     app = app_empty
 
     with app.app_context():
         field1 = Field(name="field1", type_=FieldType.UnicodeText)
         assoc1 = TypeFieldAssociation(field=field1)
         type1 = ProductType(type_id=1, name="type1", fields=[assoc1])
@@ -322,20 +304,16 @@
 
     with app.app_context():
         product1 = Product.query.filter_by(product_id=product1_id).one()
         sa.session.delete(product1)
         sa.session.commit()
 
     with app.app_context():
-        product1 = Product.query.filter_by(
-            product_id=product1_id
-        ).one_or_none()
-        attr1 = field1_attribute_class.query.filter_by(
-            iid=attr1_id
-        ).one_or_none()
+        product1 = Product.query.filter_by(product_id=product1_id).one_or_none()
+        attr1 = field1_attribute_class.query.filter_by(iid=attr1_id).one_or_none()
         assert product1 is None
         assert attr1 is None
 
 
 def test_delte_orphan_type_field_association_and_field(app_empty):
     app = app_empty
 
@@ -366,14 +344,9 @@
         field1 = Field.query.filter_by(field_id=field1_id).one()
         sa.session.delete(assoc1)
         sa.session.delete(field1)
         sa.session.commit()
 
     with app.app_context():
         product1 = Product.query.filter_by(product_id=product1_id).one()
-        attr1 = field1_attribute_class.query.filter_by(
-            iid=attr1_id
-        ).one_or_none()
+        attr1 = field1_attribute_class.query.filter_by(iid=attr1_id).one_or_none()
         assert attr1 is None
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/field/test_field.py` & `acondbs-0.4.4/tests/models/product/field/test_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from sqlalchemy import exc
-
 import pytest
+from sqlalchemy import exc
 
 from acondbs.db.sa import sa
-from acondbs.models import FieldType, Field
+from acondbs.models import Field, FieldType
 
 
-##__________________________________________________________________||
 def test_repr(app_empty):
     app = app_empty  # noqa: F841
 
     field1 = Field(name="field1")
     repr(field1)
 
     field1.type_ = FieldType.UnicodeText
     repr(field1)
 
 
-##__________________________________________________________________||
 def test_commit(app_empty):
     app = app_empty
 
     with app.app_context():
         field1 = Field(name="field1", type_=FieldType.Date)
         sa.session.add(field1)
         sa.session.commit()
@@ -29,30 +26,28 @@
     with app.app_context():
         field1 = Field.query.filter_by(name="field1").one()
         assert field1.field_id
         assert field1.name == "field1"
         assert field1.type_ is FieldType.Date
 
 
-##__________________________________________________________________||
 def test_commit_with_field_id(app_empty):
     app = app_empty
 
     with app.app_context():
         field1 = Field(field_id=259, name="field1", type_=FieldType.Date)
         sa.session.add(field1)
         sa.session.commit()
 
     with app.app_context():
         field1 = Field.query.filter_by(field_id=259).one()
         assert field1.name == "field1"
         assert field1.type_ is FieldType.Date
 
 
-##__________________________________________________________________||
 def test_nullable(app_empty):
     app = app_empty  # noqa: F841
 
     # without type_
     with app.app_context():
         field = Field(name="field")
         sa.session.add(field)
@@ -63,25 +58,21 @@
     with app.app_context():
         field = Field(type_=FieldType.UnicodeText)
         sa.session.add(field)
         with pytest.raises(exc.IntegrityError):
             sa.session.commit()
 
 
-##__________________________________________________________________||
 def test_enum_by_int(app_empty):
     """Test if an enum can be given by a number
 
     No. It raises an exception at a commit
 
     TODO: move this test to tests.models.example
     """
     app = app_empty
 
     with app.app_context():
         field1 = Field(name="field1", type_=1)
         sa.session.add(field1)
         with pytest.raises(exc.StatementError):
             sa.session.commit()
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/field/test_field_type.py` & `acondbs-0.4.4/tests/models/product/field/test_field_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 from acondbs.models import FieldType, saEnumFieldType
 
 
-##__________________________________________________________________||
 def test_attribute_class():
     for name, type_ in FieldType.__members__.items():
         # e.g., name = "UnicodeText", type_ = FieldType.UnicodeText
         assert type_.attribute_class.__name__ == f"Attribute{name}"
 
 
 def test_import_sa_enum():
     assert saEnumFieldType
 
 
-##__________________________________________________________________||
 def test_example():
-
     # can be instantiated with an int
     type_ = FieldType(1)
 
     # the same object
     assert type_ is FieldType(1)
     assert type_ is FieldType.UnicodeText
 
     # access to name and value
     assert type_.name == "UnicodeText"
     assert type_.value == 1
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/product_relation_types/test_relations.py` & `acondbs-0.4.4/tests/models/product/product_relation_types/test_relations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import pytest
 
 from acondbs.db.sa import sa
 from acondbs.models import ProductRelationType
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app_empty):
-
     y = app_empty
 
     #
     #  +--------+                +-------+
     #  |        | --(reverse)->  |       |
     #  | parent |                | child |
     #  |        | <-(reverse)--  |       |
@@ -38,45 +36,36 @@
     with y.app_context():
         sa.session.add(parent)
         sa.session.add(sibling)
         sa.session.commit()
     yield y
 
 
-##__________________________________________________________________||
 def test_reverse(app):
-
     with app.app_context():
         parent = ProductRelationType.query.filter_by(name="parent").one()
         child = ProductRelationType.query.filter_by(name="child").one()
 
         assert child is parent.reverse
         assert parent is child.reverse
 
 
 def test_self_reverse(app):
-
     with app.app_context():
         sibling = ProductRelationType.query.filter_by(name="sibling").one()
         assert sibling is sibling.reverse
 
 
 def test_cascade(app):
-
     # delete parent
     with app.app_context():
         parent = ProductRelationType.query.filter_by(name="parent").one()
         sa.session.delete(parent)
         sa.session.commit()
 
     # assert
     with app.app_context():
-        parent = ProductRelationType.query.filter_by(
-            name="parent"
-        ).one_or_none()
+        parent = ProductRelationType.query.filter_by(name="parent").one_or_none()
         child = ProductRelationType.query.filter_by(name="child").one_or_none()
 
         assert parent is None
         assert child is None
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/product_relations/conftest.py` & `acondbs-0.4.4/tests/models/product/product_relations/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 import pytest
 
 from acondbs.db.sa import sa
-from acondbs.models import (
-    ProductType,
-    Product,
-    ProductRelation,
-    ProductRelationType,
-)
+from acondbs.models import Product, ProductRelation, ProductRelationType, ProductType
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app_empty):
-
     y = app_empty
 
     #                              +--------+
     #               --(child)-->   |        |
     #                    |         | child1 |
     #  +---------+  <-(parent)--   |        |
     #  |         |                 +--------+
@@ -55,10 +48,7 @@
     ## automatically set
 
     # commit
     with y.app_context():
         sa.session.add(parent1)
         sa.session.commit()
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/product_relations/test_add_reverse_automatically.py` & `acondbs-0.4.4/tests/models/product/product_relations/test_add_reverse_automatically.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,23 @@
-import pytest
-
 from itertools import permutations
 
+import pytest
+
 from acondbs.db.sa import sa
-from acondbs.models import (
-    ProductType,
-    Product,
-    ProductRelation,
-    ProductRelationType,
-)
+from acondbs.models import Product, ProductRelation, ProductRelationType, ProductType
 
-##__________________________________________________________________||
 params = list(permutations([1, 2, 3]))
 # i.e., [(1, 2, 3), (1, 3, 2), (2, 1, 3), (2, 3, 1), (3, 1, 2), (3, 2, 1)]
 
 ids = ["-".join(["{}".format(e) for e in p]) for p in params]
 # i.e., ['1-2-3', '1-3-2', '2-1-3', '2-3-1', '3-1-2', '3-2-1']
 
 
 @pytest.mark.parametrize("perm", params, ids=ids)
 def test_permutations(app_empty, perm):
-
     app = app_empty
 
     #
     # +---------+                 +--------+
     # |         |  --(child)-->   |        |
     # | parent1 |       |         | child1 |
     # |         |  <-(parent)--   |        |
@@ -70,18 +63,16 @@
 
         assert parent1 is child1.relations[0].other
 
         assert parent1.relations[0] is child1.relations[0].reverse
         assert parent1.relations[0].reverse is child1.relations[0]
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize("perm", params, ids=ids)
 def test_self_reverse_type(app_empty, perm):
-
     app = app_empty
 
     #
     # +----------+                 +----------+
     # |          |  --(sibling)--> |          |
     # | sibling1 |       |         | sibling2 |
     # |          |  <-(sibling)--  |          |
@@ -127,18 +118,16 @@
 
         assert sibling1 is sibling2.relations[0].other
 
         assert sibling1.relations[0] is sibling2.relations[0].reverse
         assert sibling1.relations[0].reverse is sibling2.relations[0]
 
 
-##__________________________________________________________________||
 @pytest.mark.xfail(reason="events won't be triggered by foreign keys")
 def test_id(app_empty):
-
     # This test doesn't pass because the "set" events to the
     # relationships won't be triggered when the foreign keys are set.
 
     # It might be possible to pass this test with before_flush().
     # Useful links about before_flush():
     # https://docs.sqlalchemy.org/en/14/orm/session_events.html#persistence-events
     # https://stackoverflow.com/questions/36731020/sqlalchemy-orm-event-hook-for-attribute-persisted
@@ -187,17 +176,15 @@
 
         assert parent1 is child1.relations[0].other
 
         assert parent1.relations[0] is child1.relations[0].reverse
         assert parent1.relations[0].reverse is child1.relations[0]
 
 
-##__________________________________________________________________||
 def test_attach_to_self(app_empty):
-
     app = app_empty
 
     #
     # +---------+                 +--------+
     # |         |  --(child)-->   |        |
     # | parent1 |       |         | child1 |
     # |         |  <-(parent)--   |        |
@@ -238,10 +225,7 @@
 
         assert child1 is parent1.relations[0].other
 
         assert parent1 is child1.relations[0].other
 
         assert parent1.relations[0] is child1.relations[0].reverse
         assert parent1.relations[0].reverse is child1.relations[0]
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/product_relations/test_constraint.py` & `acondbs-0.4.4/tests/models/product/product_relations/test_constraint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import pytest
-
 from sqlalchemy import exc
 
-from acondbs.models import Product, ProductRelation, ProductRelationType
-
 from acondbs.db.sa import sa
+from acondbs.models import Product, ProductRelation, ProductRelationType
 
 
-##__________________________________________________________________||
 def test_constraint(app):
-
     #                              +--------+
     #               --(child)-->   |        |
     #                    |         | child1 |
     #  +---------+  <-(parent)--   |        |
     #  |         |                 +--------+
     #  | parent1 |
     #  |         |                 +--------+
@@ -31,10 +27,7 @@
         relation = ProductRelation()
         relation.type_ = type_
         relation.self_ = parent1
         relation.other = child1
 
         with pytest.raises(exc.IntegrityError):
             sa.session.commit()
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/product_relations/test_delete_cascade.py` & `acondbs-0.4.4/tests/models/product/product_relations/test_delete_cascade.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from acondbs.db.sa import sa
 from acondbs.models import Product, ProductRelation
 
 
-##__________________________________________________________________||
 def test_cascade_delete_children(app):
-
     #                              +--------+
     #               --(child)-->   |        |
     #                    |         | child1 |
     #  +---------+  <-(parent)--   |        |
     #  |         |                 +--------+
     #  | parent1 |
     #  |         |                 +--------+
@@ -33,15 +31,14 @@
     #  +---------+  --(child)-->   |        |
     #                    |         | child2 |
     #               <-(parent)--   |        |
     #                              +--------+
 
     # assert
     with app.app_context():
-
         parent1 = Product.query.filter_by(name="parent1").one_or_none()
         child1 = Product.query.filter_by(name="child1").one_or_none()
         child2 = Product.query.filter_by(name="child2").one_or_none()
 
         assert parent1 is not None
         assert child1 is None
         assert child2 is not None
@@ -66,32 +63,29 @@
     #  | parent1 |
     #  |         |
     #  +---------+
     #
 
     # assert
     with app.app_context():
-
         parent1 = Product.query.filter_by(name="parent1").one_or_none()
         child1 = Product.query.filter_by(name="child1").one_or_none()
         child2 = Product.query.filter_by(name="child2").one_or_none()
 
         assert parent1 is not None
         assert child1 is None
         assert child2 is None
 
         relations = ProductRelation.query.all()
         assert 0 == len(relations)
 
         assert 0 == len(parent1.relations)
 
 
-##__________________________________________________________________||
 def test_cascade_delete_parent(app):
-
     #                              +--------+
     #               --(child)-->   |        |
     #                    |         | child1 |
     #  +---------+  <-(parent)--   |        |
     #  |         |                 +--------+
     #  | parent1 |
     #  |         |                 +--------+
@@ -116,30 +110,27 @@
     #                              |        |
     #                              | child2 |
     #                              |        |
     #                              +--------+
 
     # assert
     with app.app_context():
-
         parent1 = Product.query.filter_by(name="parent1").one_or_none()
         child1 = Product.query.filter_by(name="child1").one_or_none()
         child2 = Product.query.filter_by(name="child2").one_or_none()
 
         assert parent1 is None
         assert child1 is not None
         assert child2 is not None
 
         relations = ProductRelation.query.all()
         assert 0 == len(relations)
 
 
-##__________________________________________________________________||
 def test_cascade_delete_relations(app):
-
     #                              +--------+
     #               --(child)-->   |        |
     #                    |         | child1 |
     #  +---------+  <-(parent)--   |        |
     #  |         |                 +--------+
     #  | parent1 |
     #  |         |                 +--------+
@@ -164,15 +155,14 @@
     #  +---------+  --(child)-->   |        |
     #                    |         | child2 |
     #               <-(parent)--   |        |
     #                              +--------+
 
     # assert
     with app.app_context():
-
         parent1 = Product.query.filter_by(name="parent1").one_or_none()
         child1 = Product.query.filter_by(name="child1").one_or_none()
         child2 = Product.query.filter_by(name="child2").one_or_none()
 
         assert parent1 is not None
         assert child1 is not None
         assert child2 is not None
@@ -201,21 +191,17 @@
     #  +---------+                 |        |
     #                              | child2 |
     #                              |        |
     #                              +--------+
 
     # assert
     with app.app_context():
-
         parent1 = Product.query.filter_by(name="parent1").one_or_none()
         child1 = Product.query.filter_by(name="child1").one_or_none()
         child2 = Product.query.filter_by(name="child2").one_or_none()
 
         assert parent1 is not None
         assert child1 is not None
         assert child2 is not None
 
         relations = ProductRelation.query.all()
         assert 0 == len(relations)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/product_relations/test_delete_nullable.py` & `acondbs-0.4.4/tests/models/product/product_relations/test_delete_nullable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import pytest
-
 from sqlalchemy import exc
 
 from acondbs.db.sa import sa
 from acondbs.models import Product, ProductRelationType
 
 
-##__________________________________________________________________||
 def test_delete_type(app):
     """assert ProductRelationType can only be deleted if relations of the
     type don't exist
 
     """
 
     #                              +--------+
@@ -89,10 +87,7 @@
         parent1 = Product.query.filter_by(name="parent1").one_or_none()
         child1 = Product.query.filter_by(name="child1").one_or_none()
         child2 = Product.query.filter_by(name="child2").one_or_none()
 
         assert parent1 is not None
         assert child1 is not None
         assert child2 is not None
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/product_relations/test_example_how_to_query.py` & `acondbs-0.4.4/tests/models/product/product_relations/test_example_how_to_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from acondbs.models import Product, ProductRelation, ProductRelationType
 
 
-##__________________________________________________________________||
 def test_example_how_to_query(app):
-
     #                              +--------+
     #               --(child)-->   |        |
     #                    |         | child1 |
     #  +---------+  <-(parent)--   |        |
     #  |         |                 +--------+
     #  | parent1 |
     #  |         |                 +--------+
     #  +---------+  --(child)-->   |        |
     #                    |         | child2 |
     #               <-(parent)--   |        |
     #                              +--------+
 
     with app.app_context():
-
         parent1 = Product.query.filter_by(name="parent1").first()
         child1 = Product.query.filter_by(name="child1").first()
         child2 = Product.query.filter_by(name="child2").first()
 
         # Product relations with the type name "child"
         relations = (
             ProductRelation.query.join(ProductRelationType)
@@ -49,10 +46,7 @@
                 (Product.product_id == ProductRelation.self_product_id),
             )
             .join(ProductRelationType)
             .filter(ProductRelationType.name == "child")
             .all()
         )
         assert [parent1] == products
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/product_relations/test_relations.py` & `acondbs-0.4.4/tests/models/product/product_relations/test_relations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from acondbs.models import Product
 
 
-##__________________________________________________________________||
 def test_relations(app):
-
     #                              +--------+
     #               --(child)-->   |        |
     #                    |         | child1 |
     #  +---------+  <-(parent)--   |        |
     #  |         |                 +--------+
     #  | parent1 |
     #  |         |                 +--------+
@@ -37,10 +35,7 @@
         assert parent1 is child2.relations[0].other
 
         assert parent1.relations[0] is child1.relations[0].reverse
         assert parent1.relations[0].reverse is child1.relations[0]
 
         assert parent1.relations[1] is child2.relations[0].reverse
         assert parent1.relations[1].reverse is child2.relations[0]
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/product_type/test_model.py` & `acondbs-0.4.4/tests/models/product/product_type/test_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from acondbs.db.sa import sa
 from acondbs.models import ProductType
 
 
-##__________________________________________________________________||
 def test_column(app_empty):
     app = app_empty
 
     with app.app_context():
         model = ProductType(
             name="map",
             order=2,
@@ -41,10 +40,7 @@
         sa.session.add(model)
         sa.session.commit()
         type_id = model.type_id
 
     with app.app_context():
         model = ProductType.query.filter_by(type_id=type_id).one()
         repr(model)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/products/test_products.py` & `acondbs-0.4.4/tests/models/product/products/test_products.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import pytest
-
 from sqlalchemy import exc
 
 from acondbs.db.sa import sa
-from acondbs.models import ProductType, Product, GitHubUser
+from acondbs.models import GitHubUser, Product, ProductType
 
 
-##__________________________________________________________________||
 def test_product(app_empty):
     app = app_empty
 
     type_map = ProductType(name="map")
     map1 = Product(name="map1", type_=type_map)
 
     with app.app_context():
@@ -21,15 +19,14 @@
         map1 = Product.query.filter_by(name="map1").one_or_none()
         assert map1 is not None
         type_map = map1.type_
         assert "map" == type_map.name
         assert [map1] == type_map.products
 
 
-##__________________________________________________________________||
 def test_constraint_type_required_add(app_empty):
     app = app_empty
 
     map1 = Product(name="map1")
 
     with app.app_context():
         sa.session.add(map1)
@@ -37,15 +34,14 @@
             sa.session.commit()
 
     with app.app_context():
         map1 = Product.query.filter_by(name="map1").one_or_none()
         assert map1 is None
 
 
-##__________________________________________________________________||
 def test_constraint_type_required_delete(app_empty):
     app = app_empty
 
     type_map = ProductType(name="map")
     map1 = Product(name="map1", type_=type_map)
 
     with app.app_context():
@@ -82,15 +78,14 @@
     # delete the type
     with app.app_context():
         type_map = ProductType.query.filter_by(name="map").one()
         sa.session.delete(type_map)
         sa.session.commit()
 
 
-##__________________________________________________________________||
 def test_git_hub_user(app_empty):
     app = app_empty
 
     user1 = GitHubUser(login="user1", git_hub_id="04:User1")
     user2 = GitHubUser(login="user2", git_hub_id="04:User2")
 
     type_map = ProductType(name="map")
@@ -115,10 +110,7 @@
         sa.session.commit()
 
     with app.app_context():
         map1 = Product.query.filter_by(name="map1").one()
         user2 = GitHubUser.query.filter_by(login="user2").one()
         assert user2 == map1.updating_git_hub_user
         assert [map1] == user2.updated_products
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/test_product_file_paths.py` & `acondbs-0.4.4/tests/models/product/test_product_file_paths.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import pytest
 
 from acondbs.db.sa import sa
-from acondbs.models import ProductType, Product, ProductFilePath
+from acondbs.models import Product, ProductFilePath, ProductType
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app_empty):
-
     y = app_empty
 
     # product --- path1
     #          |
     #          +- path2
     type1 = ProductType(name="type1")
     product = Product(name="product", type_=type1)
@@ -22,43 +20,39 @@
     # commit
     with y.app_context():
         sa.session.add(product)
         sa.session.commit()
     yield y
 
 
-##__________________________________________________________________||
 def test_relations(app):
-
     with app.app_context():
         product = Product.query.filter_by(name="product").one_or_none()
         assert "product" == product.name
         assert 2 == len(product.paths)
         path1, path2 = product.paths
         assert "/path1" == path1.path
         assert "/path2" == path2.path
         assert product is path1.product
         assert product is path2.product
 
 
 def test_delete_product(app):
-
     with app.app_context():
         product = Product.query.filter_by(name="product").one_or_none()
         sa.session.delete(product)
         sa.session.commit()
 
     with app.app_context():
         product = Product.query.filter_by(name="product").one_or_none()
         assert product is None
         assert [] == ProductFilePath.query.all()
 
 
 def test_delete_path(app):
-
     with app.app_context():
         path1 = ProductFilePath.query.filter_by(path="/path1").one_or_none()
         sa.session.delete(path1)
         sa.session.commit()
 
     with app.app_context():
         product = Product.query.filter_by(name="product").one_or_none()
@@ -71,18 +65,15 @@
 
     with app.app_context():
         product = Product.query.filter_by(name="product").one_or_none()
         assert product is not None
         assert [] == ProductFilePath.query.all()
 
 
-##__________________________________________________________________||
 def test_repr(app_empty):
     app = app_empty
     path = ProductFilePath(path="/abcdef/abcdef/abcdef/abcdef/abcdef/abcdef/path.txt")
     assert repr(path) == "<ProductFilePath '...f/abcdef/path.txt'>"
     path = ProductFilePath(path="path.txt")
     assert repr(path) == "<ProductFilePath 'path.txt'>"
     path = ProductFilePath()
     assert repr(path) == "<ProductFilePath None>"
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/type_field_association/conftest.py` & `acondbs-0.4.4/tests/models/product/type_field_association/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import pytest
 
 from acondbs.db.sa import sa
-from acondbs.models import ProductType, FieldType, Field, TypeFieldAssociation
+from acondbs.models import Field, FieldType, ProductType, TypeFieldAssociation
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app_empty):
-
     y = app_empty
 
     field1 = Field(name="field1", type_=FieldType.UnicodeText)
     field2 = Field(name="field2", type_=FieldType.Integer)
 
     assoc1 = TypeFieldAssociation(iid=1, field=field1)
     assoc2 = TypeFieldAssociation(iid=2, field=field2)
@@ -24,10 +22,7 @@
     with y.app_context():
         sa.session.add(field1)
         sa.session.add(field2)
         sa.session.add(type1)
         sa.session.commit()
 
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/product/type_field_association/test_model.py` & `acondbs-0.4.4/tests/models/product/type_field_association/test_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from sqlalchemy import exc
-
 import pytest
+from sqlalchemy import exc
 
 from acondbs.db.sa import sa
-from acondbs.models import ProductType, FieldType, Field, TypeFieldAssociation
+from acondbs.models import Field, FieldType, ProductType, TypeFieldAssociation
 
 
-##__________________________________________________________________||
 def test_column(app_empty):
     app = app_empty
 
     with app.app_context():
         field1 = Field(name="field1", type_=FieldType.UnicodeText)
         type1 = ProductType(name="type1")
         model = TypeFieldAssociation(
@@ -38,15 +36,14 @@
     type1 = ProductType(name="type1")
 
     model.type_ = type1
     model.field = field1
     repr(model)
 
 
-##__________________________________________________________________||
 def test_relationship(app):
     with app.app_context():
         field1 = Field.query.filter_by(name="field1").one()
         field2 = Field.query.filter_by(name="field2").one()
         type1 = ProductType.query.filter_by(name="type1").one()
         assoc1 = TypeFieldAssociation.query.filter_by(iid=1).one()
         assoc2 = TypeFieldAssociation.query.filter_by(iid=2).one()
@@ -55,29 +52,27 @@
         assert field2.entry_types == [assoc2]
         assert assoc1.type_ is type1
         assert assoc1.field is field1
         assert assoc2.type_ is type1
         assert assoc2.field is field2
 
 
-##__________________________________________________________________||
 def test_unique_constraint(app_empty):
     # A type cannot have multiple same field.
     app = app_empty
     with app.app_context():
         field1 = Field(name="field1", type_=FieldType.UnicodeText)
         assoc1 = TypeFieldAssociation(field=field1)
         assoc2 = TypeFieldAssociation(field=field1)
         type1 = ProductType(name="type1", fields=[assoc1, assoc2])
         sa.session.add(type1)
         with pytest.raises(exc.IntegrityError):
             sa.session.commit()
 
 
-##__________________________________________________________________||
 def test_cascade_deleting_type(app):
     """test delete a type
 
     When a type is deleted, its associations should be automatically
     deleted while the fields themselves should still exist.
 
     """
@@ -115,15 +110,14 @@
         assert association2.type_ is type1
         assert association2.field is field2
         assert type1.fields == [association2]
         assert TypeFieldAssociation.query.all() == [association2]
         # association1 is deleted from the DB
 
 
-##__________________________________________________________________||
 def test_nullable_deleting_field(app):
     """test delete a field
 
     A field cannot be deleted if it is associated
 
     """
 
@@ -132,10 +126,7 @@
         sa.session.delete(field1)
         with pytest.raises(exc.IntegrityError):
             sa.session.commit()
 
     with app.app_context():
         field1 = Field.query.filter_by(name="field1").one()
         assert field1.entry_types
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/snapshots/snap_test_models.py` & `acondbs-0.4.4/tests/models/snapshots/snap_test_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_table_names 1'] = [
     'product_types',
     'products',
     'product_file_paths',
     'product_relation_types',
@@ -24,9 +23,9 @@
     'type_field_association',
     'github_tokens',
     'github_orgs',
     'github_users',
     'github_org_memberships',
     'account_admins',
     'web_config',
-    'log'
+    'log',
 ]
```

### Comparing `acondbs-0.4.3/tests/models/test_add_owners.py` & `acondbs-0.4.4/tests/models/test_add_owners.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """Assert owners specified in the config file are added as admins in DB
 """
 
 from pathlib import Path
+
 import pytest
 
 from acondbs import create_app
 from acondbs.db.ops import define_tables
 from acondbs.db.sa import sa
 from acondbs.models import AccountAdmin
 
 from ..constants import SAMPLE_DIR
 
 
-##__________________________________________________________________||
 def test_no_error_in_create_app():
     """Assert an error does not occur in create_app() when tables are not defined"""
     config_path = Path(SAMPLE_DIR, "config.py")
     kwargs = dict(
         SQLALCHEMY_DATABASE_URI="sqlite:///:memory:",
         ACONDBS_OWNERS_GITHUB_LOGINS="octocat,dojocat",
     )
     app = create_app(config_path, **kwargs)  # noqa: F841
 
 
-##__________________________________________________________________||
 params = [
     [{"ACONDBS_OWNERS_GITHUB_LOGINS": ""}, {"octocat"}],
     [{"ACONDBS_OWNERS_GITHUB_LOGINS": ","}, {"octocat"}],
     [{"ACONDBS_OWNERS_GITHUB_LOGINS": "octocat"}, {"octocat"}],
     [{"ACONDBS_OWNERS_GITHUB_LOGINS": "octocat  "}, {"octocat"}],
     [{"ACONDBS_OWNERS_GITHUB_LOGINS": "dojocat"}, {"octocat", "dojocat"}],
     [
@@ -49,26 +48,21 @@
 def test_add_owners_to_db_as_admins(kwargs, expected, tmpdir_factory):
     config_path = Path(SAMPLE_DIR, "config.py")
 
     # use a file because, with memory, a DB will be recreated in the
     # second create_app().
     tmpdir = str(tmpdir_factory.mktemp("models"))
     tmp_database_path = Path(tmpdir, "product.sqlite3")
-    kwargs.update(
-        dict(SQLALCHEMY_DATABASE_URI=f"sqlite:///{tmp_database_path}")
-    )
+    kwargs.update(dict(SQLALCHEMY_DATABASE_URI=f"sqlite:///{tmp_database_path}"))
 
     # define tables and add a admin
     app_ = create_app(config_path, **kwargs)
     with app_.app_context():
         define_tables()
 
         octocat = AccountAdmin(git_hub_login="octocat")
         sa.session.add(octocat)
         sa.session.commit()
 
     app = create_app(config_path, **kwargs)
     with app.app_context():
         assert expected == {e.git_hub_login for e in AccountAdmin.query.all()}
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/models/web/web_config/test_model.py` & `acondbs-0.4.4/tests/models/web/web_config/test_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import json
 
 from acondbs.db.sa import sa
 from acondbs.models import WebConfig
 
-
 SAMPLE_CONFIG_JSON = json.dumps(
     {
         "head_title": "Head Title",
         "toolbar_title": "Toolbar Title",
     },
     indent=2,
 )
 
 
-##__________________________________________________________________||
 def test_column(app_empty):
     app = app_empty
 
     with app.app_context():
         model = WebConfig(json=SAMPLE_CONFIG_JSON)
         sa.session.add(model)
         sa.session.commit()
@@ -39,10 +37,7 @@
         sa.session.add(model)
         sa.session.commit()
         id_ = model.id_
 
     with app.app_context():
         model = WebConfig.query.filter_by(id_=id_).one()
         repr(model)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/ops/conftest.py` & `acondbs-0.4.4/tests/ops/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import datetime
+
 import pytest
 
-from acondbs import create_app
+from acondbs import create_app, ops
 from acondbs.db.ops import define_tables
-from acondbs.models import FieldType
-from acondbs import ops
-
 from acondbs.db.sa import sa
-from acondbs.models import GitHubUser
+from acondbs.models import FieldType, GitHubUser
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app_empty():
     database_uri = "sqlite:///:memory:"
     y = create_app(SQLALCHEMY_DATABASE_URI=database_uri)
     with y.app_context():
         define_tables()
     yield y
@@ -87,10 +84,7 @@
                 5: 1056,
                 8: datetime.datetime(2021, 10, 17, 11, 1, 30),
             },
         )
         ops.commit()
 
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/ops/test_field.py` & `acondbs-0.4.4/tests/ops/test_field.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import pytest
 
 from acondbs import ops
-from acondbs.models import FieldType, Field
+from acondbs.models import Field, FieldType
 
-
-##__________________________________________________________________||
 params = [
     pytest.param(FieldType.Float, id="by-enum"),
     pytest.param(4, id="by-int"),
 ]
 
 
 @pytest.mark.parametrize("type_", params)
@@ -26,40 +24,35 @@
     with app.app_context():
         model = Field.query.filter_by(field_id=field_id).one()
         assert model.name == "new_field"
         assert model.type_ == FieldType.Float
         assert model.field_id == field_id
 
 
-##__________________________________________________________________||
 def test_fixture(app):
     with app.app_context():
         assert Field.query.count() == 9
 
 
-##__________________________________________________________________||
 def test_update(app):
-
     with app.app_context():
         model = Field.query.filter_by(name="number").one()
         field_id = model.field_id
 
     with app.app_context():
         model = ops.update_field(field_id=field_id, name="number_renamed")
         ops.commit()
 
     with app.app_context():
         model = Field.query.filter_by(field_id=field_id).one()
         assert model.name == "number_renamed"
         assert model.field_id == field_id
 
 
-##__________________________________________________________________||
 def test_delete(app):
-
     with app.app_context():
         model = ops.create_field(name="to_be_deleted", type_=FieldType.Float)
         ops.commit()
         field_id = model.field_id
 
     with app.app_context():
         count = Field.query.count()
@@ -67,10 +60,7 @@
         ops.commit()
         assert ret is None
 
     with app.app_context():
         model = Field.query.filter_by(field_id=field_id).one_or_none()
         assert model is None
         assert Field.query.count() == count - 1
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/ops/test_log.py` & `acondbs-0.4.4/tests/ops/test_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from acondbs import ops
-
 from acondbs.models import Log
 
 
 def test_create(app):
     with app.app_context():
         count = Log.query.count()
         model = ops.create_log(level="ERROR", message="An exception occurred")
```

### Comparing `acondbs-0.4.3/tests/ops/test_product.py` & `acondbs-0.4.4/tests/ops/test_product.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 import datetime
+
 import pytest
 
 from acondbs import ops
+from acondbs.models import FieldType, GitHubUser, Product, ProductType
 from acondbs.ops.product import _normalize_paths
-from acondbs.models import Product, ProductType, FieldType, GitHubUser
-
 
-##__________________________________________________________________||
 params = [
     pytest.param([], [], id="empty"),
     pytest.param(["/a/b/c"], ["/a/b/c"], id="one"),
     pytest.param([" /a/b/c  "], ["/a/b/c"], id="unstripped"),
-    pytest.param(
-        ["/d/e", "/a/b/c", "/f/g"], ["/d/e", "/a/b/c", "/f/g"], id="multiple"
-    ),
-    pytest.param(
-        ["/a/b/c", "", "/f/g"], ["/a/b/c", "/f/g"], id="empty-member"
-    ),
+    pytest.param(["/d/e", "/a/b/c", "/f/g"], ["/d/e", "/a/b/c", "/f/g"], id="multiple"),
+    pytest.param(["/a/b/c", "", "/f/g"], ["/a/b/c", "/f/g"], id="empty-member"),
     pytest.param(
         ["/a/b/c", "  ", "/f/g"],
         ["/a/b/c", "/f/g"],
         id="empty-unstripped-member",
     ),
-    pytest.param(
-        ["/d/e", "/a/b/c", "/d/e"], ["/d/e", "/a/b/c"], id="duplicate"
-    ),
+    pytest.param(["/d/e", "/a/b/c", "/d/e"], ["/d/e", "/a/b/c"], id="duplicate"),
     pytest.param(
         ["  /d/e ", "/a/b/c", "/d/e"],
         ["/d/e", "/a/b/c"],
         id="duplicate-unstripped",
     ),
 ]
 
 
 @pytest.mark.parametrize("paths, ret", params)
 def test_normalize_paths(paths, ret):
     assert _normalize_paths(paths) == ret
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(None, id="none"),
     pytest.param({}, id="empty"),
     pytest.param({1: "An attribute"}, id="one"),
     pytest.param({1: "An attribute", 3: False}, id="two"),
     pytest.param(
         {
@@ -80,17 +72,15 @@
 
 
 params = [
     pytest.param(None, id="none"),
     pytest.param([], id="empty"),
     pytest.param(["/a/b/c"], id="one"),
     pytest.param(["/d/e", "/a/b/c", "/f/g"], id="multiple"),
-    pytest.param(
-        ["  /d/e ", " ", "/a/b/c", "/f/g", "/d/e"], id="not-normalized"
-    ),
+    pytest.param(["  /d/e ", " ", "/a/b/c", "/f/g", "/d/e"], id="not-normalized"),
 ]
 
 
 @pytest.mark.parametrize("paths", params)
 def test_create_paths(app, paths):
     return _test_create(app, paths=paths)
 
@@ -103,15 +93,14 @@
 def _test_create(
     app,
     paths=None,
     relations=None,
     attributes=None,
     posting_git_hub_user_id=None,
 ):
-
     kwargs = {"type_id": 1, "name": "new-product"}
 
     if paths is not None:
         kwargs["paths"] = paths
 
     if relations is not None:
         kwargs["relations"] = relations
@@ -159,23 +148,20 @@
         else:
             assert model.relations == []
 
         if attributes is None:
             attributes = {}
         expected_ids = [(a.iid, a.field_id) for a in model.type_.fields]
         # list of (type_field_association.iid, field.field_id)
-        expected = {
-            fid: (aid, attributes.get(fid)) for aid, fid in expected_ids
-        }
+        expected = {fid: (aid, attributes.get(fid)) for aid, fid in expected_ids}
         actual = _extract_attributes(model)
         # actual_field_ids = list(actual.keys())
         assert actual == expected
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(None, id="none"),
     pytest.param({}, id="empty"),
     pytest.param({1: "An attribute"}, id="one"),
     pytest.param({1: "An attribute", 3: False}, id="two"),
     pytest.param(
         {
@@ -246,17 +232,15 @@
     pytest.param(None, id="none"),
     pytest.param([], id="empty"),
     pytest.param(["/d/e", "/a/b/c"], id="same"),
     pytest.param(["/a/b/c", "/d/e"], id="same-perm"),
     pytest.param(["/a/b/c"], id="remove"),
     pytest.param(["/d/e", "/a/b/c", "/f/g"], id="add"),
     pytest.param(["/d/e", "/f/g", "/a/b/c"], id="add-perm"),
-    pytest.param(
-        ["  /d/e ", " ", "/a/b/c", "/f/g", "/d/e"], id="not-normalized"
-    ),
+    pytest.param(["  /d/e ", " ", "/a/b/c", "/f/g", "/d/e"], id="not-normalized"),
 ]
 
 
 @pytest.mark.parametrize("paths", params)
 def test_update_paths(app, paths):
     return _test_update(app, paths=paths)
 
@@ -269,15 +253,14 @@
 def _test_update(
     app,
     paths=None,
     relations=None,
     attributes=None,
     updating_git_hub_user_id=None,
 ):
-
     product_id = 1
     kwargs = {"product_id": product_id, "name": "new-name"}
 
     if paths is not None:
         kwargs["paths"] = paths
 
     if relations is not None:
@@ -292,20 +275,17 @@
     with app.app_context():
         count = Product.query.count()
 
         model = Product.query.filter_by(product_id=product_id).one()
         paths_old = [p.path for p in model.paths]
         path_ids_old = {p.path: p.path_id for p in model.paths}
 
-        relations_old = {
-            (r.type_id, r.other_product_id) for r in model.relations
-        }
+        relations_old = {(r.type_id, r.other_product_id) for r in model.relations}
         relation_ids_old = {
-            (r.type_id, r.other_product_id): r.relation_id
-            for r in model.relations
+            (r.type_id, r.other_product_id): r.relation_id for r in model.relations
         }
 
         attributes_old = _extract_attributes(model)
 
         model = ops.update_product(**kwargs)
         assert model.name == "new-name"
         ops.commit()
@@ -331,20 +311,16 @@
             kept = [p for p in paths_old if p in paths]
             expected = kept + _normalize_paths(paths)
             expected = list(dict.fromkeys(expected))  # uniq order preserved
         else:
             expected = paths_old
         actual = [p.path for p in model.paths]
         assert actual == expected
-        expected_path_ids = {
-            k: v for k, v in path_ids_old.items() if k in expected
-        }
-        path_ids = {
-            p.path: p.path_id for p in model.paths if p.path in path_ids_old
-        }
+        expected_path_ids = {k: v for k, v in path_ids_old.items() if k in expected}
+        path_ids = {p.path: p.path_id for p in model.paths if p.path in path_ids_old}
         assert path_ids == expected_path_ids
 
         if relations is not None:
             expected = {(r["type_id"], r["product_id"]) for r in relations}
         else:
             expected = relations_old
         actual = {(r.type_id, r.other_product_id) for r in model.relations}
@@ -364,17 +340,15 @@
         expected = attributes_old.copy()
         update = {k: (expected[k][0], v) for k, v in attributes.items()}
         expected.update(update)
         actual = _extract_attributes(model)
         assert actual == expected
 
 
-##__________________________________________________________________||
 def test_delete(app):
-
     with app.app_context():
         model = ops.create_product(type_id=1, name="to_be_deleted")
         ops.commit()
         product_id = model.product_id
 
     with app.app_context():
         count = Product.query.count()
@@ -383,47 +357,40 @@
 
     with app.app_context():
         model = Product.query.filter_by(product_id=product_id).one_or_none()
         assert model is None
         assert Product.query.count() == (count - 1)
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize("updating_git_hub_user_id", [None, 2])
 def test_convert_user(app, updating_git_hub_user_id):
-    return _test_convert(
-        app, updating_git_hub_user_id=updating_git_hub_user_id
-    )
+    return _test_convert(app, updating_git_hub_user_id=updating_git_hub_user_id)
 
 
 def _test_convert(
     app,
     updating_git_hub_user_id=None,
 ):
-
     product_id = 1
     type_id = 2
     kwargs = {"product_id": product_id, "type_id": type_id}
 
     if updating_git_hub_user_id:
         kwargs["updating_git_hub_user_id"] = updating_git_hub_user_id
 
     attr_names = [
-        a.attribute_class.backref_column
-        for a in FieldType.__members__.values()
+        a.attribute_class.backref_column for a in FieldType.__members__.values()
     ]
     # e.g., 'attributes_unicode_text', 'attributes_boolean'
 
     with app.app_context():
         model = Product.query.filter_by(product_id=product_id).one()
         assert not model.type_.type_id == type_id
         value_dict = {
-            e.field_id: e.value
-            for attr in attr_names
-            for e in getattr(model, attr)
+            e.field_id: e.value for attr in attr_names for e in getattr(model, attr)
         }
 
         product_type = ProductType.query.filter_by(type_id=type_id).one()
         expected_field_values = [
             (assoc.field_id, value_dict.get(assoc.field_id))
             for assoc in product_type.fields
         ]
@@ -445,32 +412,25 @@
         else:
             assert model.updating_git_hub_user is None
 
         expected_ids = [(a.iid, a.field_id) for a in model.type_.fields]
         attrs = [e for attr in attr_names for e in getattr(model, attr)]
         for attr in attrs:
             assert attr.type_field_association.type_ == model.type_
-        actual_ids = [
-            (e.type_field_association.iid, e.field_id) for e in attrs
-        ]
+        actual_ids = [(e.type_field_association.iid, e.field_id) for e in attrs]
         assert set(expected_ids) == set(actual_ids)
         actual_field_values = [(a.field_id, a.value) for a in attrs]
         assert set(expected_field_values) == set(actual_field_values)
 
 
-##__________________________________________________________________||
 def _extract_attributes(model):
     attr_names = [
-        a.attribute_class.backref_column
-        for a in FieldType.__members__.values()
+        a.attribute_class.backref_column for a in FieldType.__members__.values()
     ]
     # e.g., 'attributes_unicode_text', 'attributes_boolean'
 
     attrs = [e for attr in attr_names for e in getattr(model, attr)]
     # e.g., AttributeUnicodeText
 
     ret = {a.field_id: (a.type_field_association_iid, a.value) for a in attrs}
 
     return ret
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/ops/test_product_file_path.py` & `acondbs-0.4.4/tests/ops/test_product_file_path.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from acondbs import ops
-
 from acondbs.models import ProductFilePath
 
 
 def test_create(app):
     with app.app_context():
         count = ProductFilePath.query.count()
         model = ops.create_product_file_path(path="/new/path")
```

### Comparing `acondbs-0.4.3/tests/ops/test_product_relation.py` & `acondbs-0.4.4/tests/ops/test_product_relation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from acondbs import ops
-
 from acondbs.models import ProductRelation
 
 
 def test_create(app):
     with app.app_context():
         count = ProductRelation.query.count()
         model = ops.create_product_relation(
@@ -26,11 +25,9 @@
         relation_id = model.relation_id
 
         ops.delete_product_relation(relation_id=relation_id)
         ops.commit()
 
     with app.app_context():
         assert ProductRelation.query.count() == (count - 2)
-        model = ProductRelation.query.filter_by(
-            relation_id=relation_id
-        ).one_or_none()
+        model = ProductRelation.query.filter_by(relation_id=relation_id).one_or_none()
         assert model is None
```

### Comparing `acondbs-0.4.3/tests/ops/test_product_relation_type.py` & `acondbs-0.4.4/tests/ops/test_product_relation_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import pytest
 
 from acondbs import ops
 from acondbs.models import ProductRelationType
 
 
-##__________________________________________________________________||
 def test_fixture(app):
     with app.app_context():
         assert ProductRelationType.query.count() == 2
 
 
-##__________________________________________________________________||
 def test_create(app):
     type_ = {"name": "doctor"}
     reverse = {"name": "patient"}
 
     with app.app_context():
         count = ProductRelationType.query.count()
         model = ops.create_product_relation_type(type_, reverse)
@@ -69,36 +67,30 @@
             ops.create_product_relation_type(type_)
             ops.commit()
 
     with app.app_context():
         assert ProductRelationType.query.count() == count
 
 
-##__________________________________________________________________||
 def test_update(app):
-
     type_id = 1
 
     with app.app_context():
         count = ProductRelationType.query.count()
-        model = ops.update_product_relation_type(
-            type_id=type_id, name="renamed"
-        )
+        model = ops.update_product_relation_type(type_id=type_id, name="renamed")
         ops.commit()
         assert model.type_id == type_id
 
     with app.app_context():
         assert ProductRelationType.query.count() == count
         model = ProductRelationType.query.filter_by(type_id=type_id).one()
         assert model.name == "renamed"
 
 
-##__________________________________________________________________||
 def test_delete(app):
-
     with app.app_context():
         model = ops.create_product_relation_type(
             type_={"name": "to_be_deleted"},
             reverse={"name": "reverse"},
         )
         ops.commit()
         type_id = model.type_id
@@ -106,10 +98,7 @@
     with app.app_context():
         count = ProductRelationType.query.count()
         ops.delete_product_relation_type(type_id=type_id)
         ops.commit()
 
     with app.app_context():
         assert ProductRelationType.query.count() == count - 2
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/ops/test_web_config.py` & `acondbs-0.4.4/tests/ops/test_web_config.py`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.3/tests/schema/auth/query/test_admin.py` & `acondbs-0.4.4/tests/schema/auth/query/test_admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 
 from ...funcs import assert_query
 
 QUERY = "{ isAdmin }"
 
-##__________________________________________________________________||
+
 params = [
     pytest.param(
         {"query": QUERY},
         {"Authorization": "Bearer 90b2ee5fed25506df04fd37343bb68d1803dd97f"},
         False,
         id="octocat",
     ),
@@ -33,10 +33,7 @@
 ]
 
 
 @pytest.mark.parametrize("data, headers, error", params)
 @pytest.mark.asyncio
 async def test_schema(app, snapshot, data, headers, error):
     await assert_query(app, snapshot, data, headers, error)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/auth/query/test_is_signed_in.py` & `acondbs-0.4.4/tests/schema/auth/query/test_is_signed_in.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
 
 from ...funcs import assert_query
 
 QUERY = "{ isSignedIn }"
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": QUERY},
         {"Authorization": "Bearer 90b2ee5fed25506df04fd37343bb68d1803dd97f"},
         id="octocat",
     ),
     pytest.param(
@@ -30,10 +29,7 @@
 ]
 
 
 @pytest.mark.parametrize("data, headers", params)
 @pytest.mark.asyncio
 async def test_schema(app, snapshot, data, headers):
     await assert_query(app, snapshot, data, headers)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/conftest.py` & `acondbs-0.4.4/tests/auth/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 import pytest
 
 from acondbs import create_app
 from acondbs.db.ops import define_tables
-
 from acondbs.db.sa import sa
-from acondbs.models import GitHubToken, GitHubUser, AccountAdmin
+from acondbs.models import AccountAdmin, GitHubToken, GitHubUser
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app_empty():
     database_uri = "sqlite:///:memory:"
     y = create_app(SQLALCHEMY_DATABASE_URI=database_uri)
     with y.app_context():
         define_tables()
     yield y
 
 
 @pytest.fixture
-def app_users(app_empty):
+def app(app_empty):
     y = app_empty
 
     # user1: octocat - admin
     user1 = GitHubUser(login="octocat", git_hub_id="04:User583231")
-    token1 = GitHubToken(  # noqa: F841
+    token1 = GitHubToken(
         token="90b2ee5fed25506df04fd37343bb68d1803dd97f", scope="", user=user1
     )
     admin1 = AccountAdmin(git_hub_login="octocat")
 
     # user2: dojocat - not admin
     user2 = GitHubUser(login="dojocat", git_hub_id="04:User9758946")
-    token2 = GitHubToken(  # noqa: F841
+    token2 = GitHubToken(
         token="0fb8c9e16d6f7c4961c4c49212bf197d79f14080", scope="", user=user2
     )
 
     with y.app_context():
         sa.session.add(user1)
         sa.session.add(admin1)
         sa.session.add(user2)
         sa.session.commit()
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/funcs.py` & `acondbs-0.4.4/tests/schema/funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from async_asgi_testclient import TestClient
 from a2wsgi import WSGIMiddleware
-
+from async_asgi_testclient import TestClient
 
 HEADERS_DEFAULT = {"Content-Type:": "application/json"}
 
 
-##__________________________________________________________________||
 async def assert_query(app, snapshot, data, headers=None, error=False):
     if not headers:
         headers = {}
 
     app = WSGIMiddleware(app)  # convert a wsgi app to an asgi app
 
     headers_custom = headers
@@ -50,10 +48,7 @@
         app, snapshot, data_mutation, headers_mutation, error=not success
     )
 
     if success:
         mock_request_backup_db.assert_called_once()
 
     await assert_query(app, snapshot, data_query, headers_query)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/github/conftest.py` & `acondbs-0.4.4/tests/schema/github/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import pytest
 
 from acondbs import create_app
 from acondbs.db.ops import define_tables
 from acondbs.db.sa import sa
 from acondbs.models import (
+    AccountAdmin,
     GitHubOrg,
-    GitHubUser,
     GitHubOrgMembership,
     GitHubToken,
-    AccountAdmin,
+    GitHubUser,
 )
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app_empty():
     database_uri = "sqlite:///:memory:"
     y = create_app(
         SQLALCHEMY_DATABASE_URI=database_uri,
         GITHUB_AUTH_AUTHORIZE_URL="https://github.com/login/oauth/authorize",
         GITHUB_AUTH_TOKEN_URL="https://github.com/login/oauth/access_token",
@@ -27,15 +26,14 @@
     with y.app_context():
         define_tables()
     yield y
 
 
 @pytest.fixture
 def app(app_empty):
-
     y = app_empty
 
     #
     #  +------+
     #  |      |       +-------+       +--------+
     #  | org1 | ----- |       | --+-- | token1 |
     #  |      |       | user1 |   |   +--------+
@@ -102,10 +100,7 @@
         sa.session.add(user1)
         sa.session.add(user2)
         sa.session.add(user3)
         sa.session.add(admin1)
         sa.session.add(admin2)
         sa.session.commit()
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/github/mutation/snapshots/snap_test_add_git_hub_admin_app_token.py` & `acondbs-0.4.4/tests/schema/github/mutation/snapshots/snap_test_delete_git_hub_admin_app_token.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,112 +1,80 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_error[one] 1'] = {
+snapshots['test_schema_error[delete] 1'] = {
     'data': {
         'allGitHubTokens': {
             'edges': [
                 {
                     'node': {
                         'scope': 'read:org',
                         'tokenId': '1',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
                     }
                 },
                 {
                     'node': {
                         'scope': '',
                         'tokenId': '2',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
                     }
                 },
                 {
                     'node': {
                         'scope': '',
                         'tokenId': '3',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
                     }
                 },
                 {
                     'node': {
                         'scope': '',
                         'tokenId': '4',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
                     }
-                }
+                },
             ],
-            'totalCount': 4
+            'totalCount': 4,
         }
     }
 }
 
-snapshots['test_schema_error[one] 2'] = [
-    (
-        (
-            'code_01234'
-        ,),
-        {
-        }
-    )
-]
-
-snapshots['test_schema_success[one] 1'] = {
-    'data': {
-        'addGitHubAdminAppToken': {
-            'ok': True
-        }
-    }
+snapshots['test_schema_success[delete] 1'] = {
+    'data': {'deleteGitHubAdminAppToken': {'ok': True}}
 }
 
-snapshots['test_schema_success[one] 2'] = {
+snapshots['test_schema_success[delete] 2'] = {
     'data': {
         'allGitHubTokens': {
             'edges': [
                 {
                     'node': {
-                        'scope': 'read:org',
-                        'tokenId': '1',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
-                    }
-                },
-                {
-                    'node': {
                         'scope': '',
                         'tokenId': '2',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
                     }
                 },
                 {
                     'node': {
                         'scope': '',
                         'tokenId': '3',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
                     }
                 },
                 {
                     'node': {
                         'scope': '',
                         'tokenId': '4',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
                     }
-                }
+                },
             ],
-            'totalCount': 4
+            'totalCount': 3,
         }
     }
 }
-
-snapshots['test_schema_success[one] 3'] = [
-    (
-        (
-            'code_01234'
-        ,),
-        {
-        }
-    )
-]
```

### Comparing `acondbs-0.4.3/tests/schema/github/mutation/snapshots/snap_test_delete_git_hub_admin_app_token.py` & `acondbs-0.4.4/tests/schema/github/query/snapshots/snap_test_all_git_hub_tokens.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,72 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_error[delete] 1'] = {
+snapshots['test_schema[filter] 1'] = {
     'data': {
         'allGitHubTokens': {
             'edges': [
                 {
                     'node': {
                         'scope': 'read:org',
+                        'timeCreated': '2021-01-04T14:32:20',
                         'tokenId': '1',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
-                    }
-                },
-                {
-                    'node': {
-                        'scope': '',
-                        'tokenId': '2',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
-                    }
-                },
-                {
-                    'node': {
-                        'scope': '',
-                        'tokenId': '3',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
-                    }
-                },
-                {
-                    'node': {
-                        'scope': '',
-                        'tokenId': '4',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
+                        'user': {'login': 'user1'},
                     }
                 }
             ],
-            'totalCount': 4
-        }
-    }
-}
-
-snapshots['test_schema_success[delete] 1'] = {
-    'data': {
-        'deleteGitHubAdminAppToken': {
-            'ok': True
+            'totalCount': 1,
         }
     }
 }
 
-snapshots['test_schema_success[delete] 2'] = {
+snapshots['test_schema[simple] 1'] = {
     'data': {
         'allGitHubTokens': {
             'edges': [
                 {
                     'node': {
+                        'scope': 'read:org',
+                        'timeCreated': '2021-01-04T14:32:20',
+                        'tokenId': '1',
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
+                        'user': {'login': 'user1'},
+                    }
+                },
+                {
+                    'node': {
                         'scope': '',
+                        'timeCreated': '2021-01-04T14:32:20',
                         'tokenId': '2',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
+                        'user': {'login': 'user1'},
                     }
                 },
                 {
                     'node': {
                         'scope': '',
+                        'timeCreated': '2021-01-04T14:32:20',
                         'tokenId': '3',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
+                        'user': {'login': 'user2'},
                     }
                 },
                 {
                     'node': {
                         'scope': '',
+                        'timeCreated': '2021-01-04T14:32:20',
                         'tokenId': '4',
-                        'tokenMasked': 'XXXXXXXXXXXXXXX'
+                        'tokenMasked': 'XXXXXXXXXXXXXXX',
+                        'user': {'login': 'user3'},
                     }
-                }
+                },
             ],
-            'totalCount': 3
+            'totalCount': 4,
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/github/mutation/test_add_git_hub_admin_app_token.py` & `acondbs-0.4.4/tests/schema/github/mutation/test_add_git_hub_admin_app_token.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import pytest
 import unittest.mock as mock
 
+import pytest
+
 from ...funcs import assert_mutation
 
 ADD_GIT_HUB_ADMIN_APP_TOKEN = """
 mutation AddGitHubAdminAppToken($code: String!) {
   addGitHubAdminAppToken(code: $code) {
     ok
   }
@@ -25,23 +26,21 @@
   }
 }
 """
 
 HEADERS = {"Authorization": "Bearer token1"}  # user1
 
 
-##__________________________________________________________________||
 @pytest.fixture(autouse=True)
 def mock_store_token_for_code(monkeypatch):
     y = mock.Mock()
     monkeypatch.setattr("acondbs.schema.github.mutation.store_token_for_code", y)
     yield y
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": ADD_GIT_HUB_ADMIN_APP_TOKEN, "variables": {"code": "code_01234"}},
         {"query": ALL_GITHUB_ADMIN_APP_TOKENS},
         id="one",
     ),
 ]
@@ -66,15 +65,14 @@
         HEADERS,
         mock_request_backup_db,
         success=True,
     )
     snapshot.assert_match(mock_store_token_for_code.call_args_list)
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": ADD_GIT_HUB_ADMIN_APP_TOKEN, "variables": {"code": "code_01234"}},
         {"query": ALL_GITHUB_ADMIN_APP_TOKENS},
         id="one",
     ),
 ]
@@ -98,10 +96,7 @@
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success=False,
     )
     snapshot.assert_match(mock_store_token_for_code.call_args_list)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/github/mutation/test_authenticate_with_git_hub.py` & `acondbs-0.4.4/tests/schema/github/mutation/test_authenticate_with_git_hub.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 import textwrap
-from async_asgi_testclient import TestClient
-
-from a2wsgi import WSGIMiddleware
+import unittest.mock as mock
 
 import pytest
-import unittest.mock as mock
+from a2wsgi import WSGIMiddleware
+from async_asgi_testclient import TestClient
 
 
-##__________________________________________________________________||
 @pytest.fixture(autouse=True)
 def mock_authenticate(monkeypatch):
     y = mock.Mock()
     monkeypatch.setattr("acondbs.schema.github.mutation.authenticate", y)
     yield y
 
 
-##__________________________________________________________________||
 @pytest.mark.asyncio
 async def test_auth(app, mock_authenticate):
-
     query = textwrap.dedent(
         """
         mutation AuthenticateWithGitHub($code: String!) {
           authenticateWithGitHub(code: $code) {
             authPayload {
               token
             }
@@ -47,10 +43,7 @@
     headers = {"Content-Type:": "application/json"}
 
     async with TestClient(app) as client:
         resp = await client.post("/graphql", json=data, headers=headers)
 
     assert {"data": expected} == resp.json()
     assert [mock.call("h443xg9c")] == mock_authenticate.call_args_list
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/github/mutation/test_delete_git_hub_admin_app_token.py` & `acondbs-0.4.4/tests/schema/github/mutation/test_delete_git_hub_admin_app_token.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         scope
       }
     }
   }
 }
 """
 
-##__________________________________________________________________||
+
 params = [
     pytest.param(
         {"query": DELETE_GIT_HUB_ADMIN_APP_TOKEN, "variables": {"tokenId": 1}},
         {"Authorization": "Bearer token1"},
         {"query": ALL_GITHUB_ADMIN_APP_TOKENS},
         {"Authorization": "Bearer token4"},
         id="delete",
@@ -46,28 +46,26 @@
     snapshot,
     data_mutation,
     headers_mutation,
     data_query,
     headers_query,
     mock_request_backup_db,
 ):
-
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         headers_mutation,
         data_query,
         headers_query,
         mock_request_backup_db,
         success=True,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": DELETE_GIT_HUB_ADMIN_APP_TOKEN, "variables": {"tokenId": 999}},
         {"Authorization": "Bearer token1"},
         {"query": ALL_GITHUB_ADMIN_APP_TOKENS},
         {"Authorization": "Bearer token4"},
         id="delete",
@@ -84,21 +82,17 @@
     snapshot,
     data_mutation,
     headers_mutation,
     data_query,
     headers_query,
     mock_request_backup_db,
 ):
-
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         headers_mutation,
         data_query,
         headers_query,
         mock_request_backup_db,
         success=False,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/github/query/test_all_git_hub_orgs.py` & `acondbs-0.4.4/tests/schema/github/query/test_all_git_hub_orgs.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,28 +21,22 @@
         }
       }
     }
   }
 }
 '''
 
-HEADERS = {
-    "Authorization": "Bearer token1"  # user1
-}
+HEADERS = {"Authorization": "Bearer token1"}  # user1
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": ALL_GITHUB_ORGS},
         id="one",
     ),
 ]
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize("data", params)
 @pytest.mark.asyncio
 async def test_schema(app, snapshot, data):
     await assert_query(app, snapshot, data, HEADERS)
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/github/query/test_all_git_hub_tokens.py` & `acondbs-0.4.4/tests/schema/github/query/test_all_git_hub_tokens.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,32 +42,26 @@
     }
   }
 }
 """
     + GITHUB_TOKEN_FRAGMENT
 )
 
-HEADERS = {
-    "Authorization": "Bearer token1"  # user1
-}
+HEADERS = {"Authorization": "Bearer token1"}  # user1
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": ALL_GITHUB_TOKENS},
         id="simple",
     ),
     pytest.param(
         {"query": ALL_GITHUB_TOKENS_WITH_ORG_ACCESS},
         id="filter",
     ),
 ]
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize("data", params)
 @pytest.mark.asyncio
 async def test_schema(app, snapshot, data):
     await assert_query(app, snapshot, data, HEADERS)
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/github/query/test_all_git_hub_users.py` & `acondbs-0.4.4/tests/schema/github/query/test_all_git_hub_users.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,61 +15,59 @@
         }
       }
     }
   }
 }
 '''
 
-ALL_GITHUB_USERS = '''
+ALL_GITHUB_USERS = (
+    '''
 {
   allGitHubUsers {
     totalCount
     edges {
       node {
         ...GitHubUserFragment
       }
     }
   }
 }
-''' + GITHUB_USER_FRAGMENT
+'''
+    + GITHUB_USER_FRAGMENT
+)
 
-ALL_GITHUB_USERS_WITH_FILTER = '''
+ALL_GITHUB_USERS_WITH_FILTER = (
+    '''
 query AllGitHubUsers($orgMember: Boolean){
   allGitHubUsers(filters: { orgMember: $orgMember }) {
     totalCount
     edges {
       node {
         ...GitHubUserFragment
       }
     }
   }
 }
-''' + GITHUB_USER_FRAGMENT
+'''
+    + GITHUB_USER_FRAGMENT
+)
+
+HEADERS = {"Authorization": "Bearer token1"}  # user1
 
-HEADERS = {
-    "Authorization": "Bearer token1"  # user1
-}
 
-##__________________________________________________________________||
 params = [
-    pytest.param(
-        {"query": ALL_GITHUB_USERS},
-        id='one'
-    ),
+    pytest.param({"query": ALL_GITHUB_USERS}, id='one'),
     pytest.param(
         {"query": ALL_GITHUB_USERS_WITH_FILTER, 'variables': {'orgMember': True}},
-        id='filter-on'
+        id='filter-on',
     ),
     pytest.param(
         {"query": ALL_GITHUB_USERS_WITH_FILTER, 'variables': {'orgMember': False}},
-        id='filter-off'
+        id='filter-off',
     ),
 ]
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize("data", params)
 @pytest.mark.asyncio
 async def test_schema(app, snapshot, data):
     await assert_query(app, snapshot, data, HEADERS)
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/github/query/test_git_hub_viewer.py` & `acondbs-0.4.4/tests/schema/github/query/test_git_hub_viewer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 
 from ...funcs import assert_query
 
 QUERY = "{ gitHubViewer { login name avatarUrl } }"
 
-##__________________________________________________________________||
+
 params = [
     pytest.param(
         {"query": QUERY},
         {"Authorization": "Bearer token1"},
         id="one",
     ),
 ]
@@ -16,15 +16,14 @@
 
 @pytest.mark.parametrize("data, headers", params)
 @pytest.mark.asyncio
 async def test_success(app, snapshot, data, headers):
     await assert_query(app, snapshot, data, headers)
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": QUERY},
         {"Authorization": "Bearer no-such-token"},
         id="wrong-token",
     ),
     pytest.param(
@@ -35,10 +34,7 @@
 ]
 
 
 @pytest.mark.parametrize("data, headers", params)
 @pytest.mark.asyncio
 async def test_error(app, snapshot, data, headers):
     await assert_query(app, snapshot, data, headers, error=True)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/misc/mutation/log/snapshots/snap_test_create.py` & `acondbs-0.4.4/tests/schema/misc/mutation/log/snapshots/snap_test_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_schema_success[one] 1'] = {
     'data': {
         'createLog': {
             'log': {
                 'id_': '3',
                 'level': 'ERROR',
                 'message': 'An exception is raised',
-                'time': '2021-01-04T14:32:20'
+                'time': '2021-01-04T14:32:20',
             },
-            'ok': True
+            'ok': True,
         }
     }
 }
 
 snapshots['test_schema_success[one] 2'] = {
     'data': {
         'allLogs': {
             'edges': [
                 {
                     'node': {
                         'id_': '1',
                         'level': 'DEBUG',
                         'message': 'A debug message!',
-                        'time': '2021-01-04T14:32:20'
+                        'time': '2021-01-04T14:32:20',
                     }
                 },
                 {
                     'node': {
                         'id_': '2',
                         'level': 'ERROR',
                         'message': 'An error message!',
-                        'time': '2021-01-04T14:32:20'
+                        'time': '2021-01-04T14:32:20',
                     }
                 },
                 {
                     'node': {
                         'id_': '3',
                         'level': 'ERROR',
                         'message': 'An exception is raised',
-                        'time': '2021-01-04T14:32:20'
+                        'time': '2021-01-04T14:32:20',
                     }
-                }
+                },
             ],
-            'totalCount': 3
+            'totalCount': 3,
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/misc/mutation/log/snapshots/snap_test_delete.py` & `acondbs-0.4.4/tests/schema/misc/mutation/log/snapshots/snap_test_delete.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_success[one] 1'] = {
-    'data': {
-        'deleteLog': {
-            'ok': True
-        }
-    }
-}
+snapshots['test_schema_success[one] 1'] = {'data': {'deleteLog': {'ok': True}}}
 
 snapshots['test_schema_success[one] 2'] = {
     'data': {
         'allLogs': {
             'edges': [
                 {
                     'node': {
                         'id_': '1',
                         'level': 'DEBUG',
                         'message': 'A debug message!',
-                        'time': '2021-01-04T14:32:20'
+                        'time': '2021-01-04T14:32:20',
                     }
                 }
             ],
-            'totalCount': 1
+            'totalCount': 1,
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/misc/mutation/log/test_create.py` & `acondbs-0.4.4/tests/schema/misc/mutation/log/test_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import pytest
 
 from ....funcs import assert_mutation
-
 from ...gql import MUTATION_CREATE_LOG, QUERY_ALL_LOGS
 
-HEADERS_MUTATION = {
-}
+HEADERS_MUTATION = {}
 
 HEADERS_QUERY = {
     "Authorization": "Bearer 90b2ee5fed25506df04fd37343bb68d1803dd97f"  # octocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_CREATE_LOG,
             "variables": {
                 "input": {
                     "level": "ERROR",
@@ -31,22 +28,18 @@
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS_MUTATION,
         data_query,
         HEADERS_QUERY,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/misc/mutation/log/test_delete.py` & `acondbs-0.4.4/tests/schema/misc/mutation/log/test_delete.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import pytest
 
 from ....funcs import assert_mutation
-
 from ...gql import MUTATION_DELETE_LOG, QUERY_ALL_LOGS
 
 HEADERS = {
     "Authorization": "Bearer 90b2ee5fed25506df04fd37343bb68d1803dd97f"  # octocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_DELETE_LOG,
             "variables": {
                 "id_": 2,
             },
@@ -25,22 +23,18 @@
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/misc/query/snapshots/snap_test_all_logs.py` & `acondbs-0.4.4/tests/schema/misc/query/snapshots/snap_test_all_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_schema[one] 1'] = {
     'data': {
         'allLogs': {
             'edges': [
                 {
                     'node': {
                         'id_': '1',
                         'level': 'DEBUG',
                         'message': 'A debug message!',
-                        'time': '2021-01-04T14:32:20'
+                        'time': '2021-01-04T14:32:20',
                     }
                 },
                 {
                     'node': {
                         'id_': '2',
                         'level': 'ERROR',
                         'message': 'An error message!',
-                        'time': '2021-01-04T14:32:20'
+                        'time': '2021-01-04T14:32:20',
                     }
-                }
+                },
             ],
-            'totalCount': 2
+            'totalCount': 2,
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/misc/query/test_all_logs.py` & `acondbs-0.4.4/tests/schema/product/query/test_all_product_relation_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 import pytest
 
 from ...funcs import assert_query
-
 from ..gql import (
-    QUERY_ALL_LOGS,
+    QUERY_ALL_PRODUCT_RELATION_TYPES,
+    QUERY_ALL_PRODUCT_RELATION_TYPES_TOTAL_COUNT,
 )
 
 HEADERS = {
-    "Authorization": "Bearer 90b2ee5fed25506df04fd37343bb68d1803dd97f"  # octocat
+    "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
-        {
-            #
-            "query": QUERY_ALL_LOGS
-        },
-        id="one",
+        {"query": QUERY_ALL_PRODUCT_RELATION_TYPES},
+        id="query",
+    ),
+    pytest.param(
+        {"query": QUERY_ALL_PRODUCT_RELATION_TYPES_TOTAL_COUNT},
+        id="total-count",
     ),
 ]
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize("data", params)
 @pytest.mark.asyncio
 async def test_schema(app, snapshot, data):
     await assert_query(app, snapshot, data, HEADERS)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/gql/__init__.py` & `acondbs-0.4.4/tests/schema/product/gql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,54 +2,52 @@
 
 """
 
 from .fragments import (  # noqa: F401
     FRAGMENT_FIELD,
     FRAGMENT_FIELD_CONNECTION,
     FRAGMENT_PRODUCT,
-    FRAGMENT_PRODUCT_SHALLOW,
     FRAGMENT_PRODUCT_CONNECTION,
     FRAGMENT_PRODUCT_CONNECTION_SHALLOW,
-    FRAGMENT_PRODUCT_RELATION_TYPE,
-    FRAGMENT_PRODUCT_RELATION_TYPE_CONNECTION,
     FRAGMENT_PRODUCT_RELATION,
     FRAGMENT_PRODUCT_RELATION_CONNECTION,
+    FRAGMENT_PRODUCT_RELATION_TYPE,
+    FRAGMENT_PRODUCT_RELATION_TYPE_CONNECTION,
+    FRAGMENT_PRODUCT_SHALLOW,
     FRAGMENT_PRODUCT_TYPE,
     FRAGMENT_PRODUCT_TYPE_CONNECTION,
 )
-
+from .mutations import (  # noqa: F401
+    MUTATION_CONVERT_PRODUCT_TYPE,
+    MUTATION_CREATE_FIELD,
+    MUTATION_CREATE_PRODUCT,
+    MUTATION_CREATE_PRODUCT_RELATION,
+    MUTATION_CREATE_PRODUCT_RELATION_TYPES,
+    MUTATION_CREATE_PRODUCT_TYPE,
+    MUTATION_DELETE_FIELD,
+    MUTATION_DELETE_PRODUCT,
+    MUTATION_DELETE_PRODUCT_RELATION,
+    MUTATION_DELETE_PRODUCT_RELATION_TYPES,
+    MUTATION_DELETE_PRODUCT_TYPE,
+    MUTATION_UPDATE_FIELD,
+    MUTATION_UPDATE_PRODUCT,
+    MUTATION_UPDATE_PRODUCT_RELATION_TYPE,
+    MUTATION_UPDATE_PRODUCT_TYPE,
+)
 from .queries import (  # noqa: F401
     QUERY_ALL_FIELDS,
-    QUERY_ALL_PRODUCTS,
-    QUERY_ALL_PRODUCTS_SHALLOW,
-    QUERY_ALL_PRODUCTS_TOTAL_COUNT,
     QUERY_ALL_PRODUCT_FILE_PATHS,
-    QUERY_ALL_PRODUCT_RELATIONS,
-    QUERY_ALL_PRODUCT_RELATIONS_TOTAL_COUNT,
     QUERY_ALL_PRODUCT_RELATION_TYPES,
     QUERY_ALL_PRODUCT_RELATION_TYPES_TOTAL_COUNT,
+    QUERY_ALL_PRODUCT_RELATIONS,
+    QUERY_ALL_PRODUCT_RELATIONS_TOTAL_COUNT,
     QUERY_ALL_PRODUCT_TYPES,
+    QUERY_ALL_PRODUCTS,
+    QUERY_ALL_PRODUCTS_SHALLOW,
+    QUERY_ALL_PRODUCTS_TOTAL_COUNT,
     QUERY_FIELD,
     QUERY_PRODUCT,
-    QUERY_PRODUCT_SHALLOW,
     QUERY_PRODUCT_RELATION,
     QUERY_PRODUCT_RELATION_TYPE,
+    QUERY_PRODUCT_SHALLOW,
     QUERY_PRODUCT_TYPE,
 )
-
-from .mutations import (  # noqa: F401
-    MUTATION_CREATE_PRODUCT,
-    MUTATION_DELETE_PRODUCT,
-    MUTATION_UPDATE_PRODUCT,
-    MUTATION_CREATE_PRODUCT_RELATION_TYPES,
-    MUTATION_UPDATE_PRODUCT_RELATION_TYPE,
-    MUTATION_DELETE_PRODUCT_RELATION_TYPES,
-    MUTATION_CREATE_PRODUCT_RELATION,
-    MUTATION_DELETE_PRODUCT_RELATION,
-    MUTATION_CREATE_PRODUCT_TYPE,
-    MUTATION_UPDATE_PRODUCT_TYPE,
-    MUTATION_DELETE_PRODUCT_TYPE,
-    MUTATION_CREATE_FIELD,
-    MUTATION_UPDATE_FIELD,
-    MUTATION_DELETE_FIELD,
-    MUTATION_CONVERT_PRODUCT_TYPE,
-)
```

### Comparing `acondbs-0.4.3/tests/schema/product/gql/fragments/__init__.py` & `acondbs-0.4.4/tests/schema/product/gql/fragments/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 from .fragment_field import FRAGMENT_FIELD  # noqa: F401
 from .fragment_field_connection import FRAGMENT_FIELD_CONNECTION  # noqa: F401
 from .fragment_product import FRAGMENT_PRODUCT  # noqa: F401
-from .fragment_product_shallow import FRAGMENT_PRODUCT_SHALLOW  # noqa: F401
 from .fragment_product_connection import FRAGMENT_PRODUCT_CONNECTION  # noqa: F401
-from .fragment_product_connection_shallow import FRAGMENT_PRODUCT_CONNECTION_SHALLOW  # noqa: F401
-from .fragment_product_relation_type import FRAGMENT_PRODUCT_RELATION_TYPE  # noqa: F401
-from .fragment_product_relation_type_connection import FRAGMENT_PRODUCT_RELATION_TYPE_CONNECTION  # noqa: F401
+from .fragment_product_connection_shallow import (  # noqa: F401
+    FRAGMENT_PRODUCT_CONNECTION_SHALLOW,
+)
 from .fragment_product_relation import FRAGMENT_PRODUCT_RELATION  # noqa: F401
-from .fragment_product_relation_connection import FRAGMENT_PRODUCT_RELATION_CONNECTION  # noqa: F401
+from .fragment_product_relation_connection import (  # noqa: F401
+    FRAGMENT_PRODUCT_RELATION_CONNECTION,
+)
+from .fragment_product_relation_type import FRAGMENT_PRODUCT_RELATION_TYPE  # noqa: F401
+from .fragment_product_relation_type_connection import (  # noqa: F401
+    FRAGMENT_PRODUCT_RELATION_TYPE_CONNECTION,
+)
+from .fragment_product_shallow import FRAGMENT_PRODUCT_SHALLOW  # noqa: F401
 from .fragment_product_type import FRAGMENT_PRODUCT_TYPE  # noqa: F401
-from .fragment_product_type_connection import FRAGMENT_PRODUCT_TYPE_CONNECTION  # noqa: F401
+from .fragment_product_type_connection import (  # noqa: F401
+    FRAGMENT_PRODUCT_TYPE_CONNECTION,
+)
```

### Comparing `acondbs-0.4.3/tests/schema/product/gql/fragments/fragment_product.py` & `acondbs-0.4.4/tests/schema/product/gql/fragments/fragment_product.py`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.3/tests/schema/product/gql/mutations/__init__.py` & `acondbs-0.4.4/tests/schema/product/gql/mutations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # fmt: off
+from .mutation_convert_product_type import MUTATION_CONVERT_PRODUCT_TYPE  # noqa: F401
+from .mutation_create_field import MUTATION_CREATE_FIELD  # noqa: F401
 from .mutation_create_product import MUTATION_CREATE_PRODUCT  # noqa: F401
-from .mutation_delete_product import MUTATION_DELETE_PRODUCT  # noqa: F401
-from .mutation_update_product import MUTATION_UPDATE_PRODUCT  # noqa: F401
-from .mutation_create_product_relation_types import MUTATION_CREATE_PRODUCT_RELATION_TYPES  # noqa: F401
-from .mutation_update_product_relation_type import MUTATION_UPDATE_PRODUCT_RELATION_TYPE  # noqa: F401
-from .mutation_delete_product_relation_types import MUTATION_DELETE_PRODUCT_RELATION_TYPES  # noqa: F401
-from .mutation_create_product_relation import MUTATION_CREATE_PRODUCT_RELATION  # noqa: F401
-from .mutation_delete_product_relation import MUTATION_DELETE_PRODUCT_RELATION  # noqa: F401
+from .mutation_create_product_relation import (  # noqa: F401
+    MUTATION_CREATE_PRODUCT_RELATION,
+)
+from .mutation_create_product_relation_types import (  # noqa: F401
+    MUTATION_CREATE_PRODUCT_RELATION_TYPES,
+)
 from .mutation_create_product_type import MUTATION_CREATE_PRODUCT_TYPE  # noqa: F401
-from .mutation_update_product_type import MUTATION_UPDATE_PRODUCT_TYPE  # noqa: F401
+from .mutation_delete_field import MUTATION_DELETE_FIELD  # noqa: F401
+from .mutation_delete_product import MUTATION_DELETE_PRODUCT  # noqa: F401
+from .mutation_delete_product_relation import (  # noqa: F401
+    MUTATION_DELETE_PRODUCT_RELATION,
+)
+from .mutation_delete_product_relation_types import (  # noqa: F401
+    MUTATION_DELETE_PRODUCT_RELATION_TYPES,
+)
 from .mutation_delete_product_type import MUTATION_DELETE_PRODUCT_TYPE  # noqa: F401
-from .mutation_create_field import MUTATION_CREATE_FIELD  # noqa: F401
 from .mutation_update_field import MUTATION_UPDATE_FIELD  # noqa: F401
-from .mutation_delete_field import MUTATION_DELETE_FIELD  # noqa: F401
-from .mutation_convert_product_type import MUTATION_CONVERT_PRODUCT_TYPE  # noqa: F401
+from .mutation_update_product import MUTATION_UPDATE_PRODUCT  # noqa: F401
+from .mutation_update_product_relation_type import (  # noqa: F401
+    MUTATION_UPDATE_PRODUCT_RELATION_TYPE,
+)
+from .mutation_update_product_type import MUTATION_UPDATE_PRODUCT_TYPE  # noqa: F401
```

### Comparing `acondbs-0.4.3/tests/schema/product/gql/queries/__init__.py` & `acondbs-0.4.4/tests/schema/product/gql/queries/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # fmt: off
 from .query_all_fields import QUERY_ALL_FIELDS  # noqa: F401
+from .query_all_product_file_paths import QUERY_ALL_PRODUCT_FILE_PATHS  # noqa: F401
+from .query_all_product_relation_types import (  # noqa: F401
+    QUERY_ALL_PRODUCT_RELATION_TYPES,
+)
+from .query_all_product_relation_types_total_count import (  # noqa: F401
+    QUERY_ALL_PRODUCT_RELATION_TYPES_TOTAL_COUNT,
+)
+from .query_all_product_relations import QUERY_ALL_PRODUCT_RELATIONS  # noqa: F401
+from .query_all_product_relations_total_count import (  # noqa: F401
+    QUERY_ALL_PRODUCT_RELATIONS_TOTAL_COUNT,
+)
+from .query_all_product_types import QUERY_ALL_PRODUCT_TYPES  # noqa: F401
 from .query_all_products import QUERY_ALL_PRODUCTS  # noqa: F401
 from .query_all_products_shallow import QUERY_ALL_PRODUCTS_SHALLOW  # noqa: F401
 from .query_all_products_total_count import QUERY_ALL_PRODUCTS_TOTAL_COUNT  # noqa: F401
-from .query_all_product_file_paths import QUERY_ALL_PRODUCT_FILE_PATHS  # noqa: F401
-from .query_all_product_relations import QUERY_ALL_PRODUCT_RELATIONS  # noqa: F401
-from .query_all_product_relations_total_count import QUERY_ALL_PRODUCT_RELATIONS_TOTAL_COUNT  # noqa: F401
-from .query_all_product_relation_types import QUERY_ALL_PRODUCT_RELATION_TYPES  # noqa: F401
-from .query_all_product_relation_types_total_count import QUERY_ALL_PRODUCT_RELATION_TYPES_TOTAL_COUNT  # noqa: F401
-from .query_all_product_types import  QUERY_ALL_PRODUCT_TYPES  # noqa: F401
 from .query_field import QUERY_FIELD  # noqa: F401
 from .query_product import QUERY_PRODUCT  # noqa: F401
-from .query_product_shallow import QUERY_PRODUCT_SHALLOW  # noqa: F401
 from .query_product_relation import QUERY_PRODUCT_RELATION  # noqa: F401
 from .query_product_relation_type import QUERY_PRODUCT_RELATION_TYPE  # noqa: F401
+from .query_product_shallow import QUERY_PRODUCT_SHALLOW  # noqa: F401
 from .query_product_type import QUERY_PRODUCT_TYPE  # noqa: F401
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/field/conftest.py` & `acondbs-0.4.4/tests/schema/product/mutation/field/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pytest
 
 from acondbs import ops
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app_users):
     y = app_users
     with y.app_context():
         ops.create_field(
             field_id=1,
             name="contact",
@@ -21,10 +20,7 @@
         ops.create_field(
             field_id=3,
             name="date_produced",
             type_=ops.FieldType.Date,
         )
         ops.commit()
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/field/snapshots/snap_test_create_field.py` & `acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_all_product_file_paths.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,121 +1,81 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_error[by-enum-int] 1'] = {
+snapshots['test_schema[all] 1'] = {
     'data': {
-        'allFields': {
+        'allProductFilePaths': {
             'edges': [
                 {
                     'node': {
-                        'fieldId': '1',
-                        'name': 'contact',
-                        'type_': 'UNICODE_TEXT'
+                        'note': None,
+                        'path': 'site2:/another/way/map1',
+                        'pathId': '1',
+                        'product': {'name': 'map1'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '2',
-                        'name': 'produced_by',
-                        'type_': 'UNICODE_TEXT'
+                        'note': None,
+                        'path': 'site1:/path/to/map2',
+                        'pathId': '2',
+                        'product': {'name': 'map2'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '3',
-                        'name': 'date_produced',
-                        'type_': 'DATE'
-                    }
-                }
-            ],
-            'totalCount': 3
-        }
-    }
-}
-
-snapshots['test_schema_error[enum-nonexistent] 1'] = {
-    'data': {
-        'allFields': {
-            'edges': [
-                {
-                    'node': {
-                        'fieldId': '1',
-                        'name': 'contact',
-                        'type_': 'UNICODE_TEXT'
+                        'note': None,
+                        'path': 'site1:/path/to/map3',
+                        'pathId': '3',
+                        'product': {'name': 'map3'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '2',
-                        'name': 'produced_by',
-                        'type_': 'UNICODE_TEXT'
+                        'note': None,
+                        'path': 'site2:/another/way/map3',
+                        'pathId': '4',
+                        'product': {'name': 'map3'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '3',
-                        'name': 'date_produced',
-                        'type_': 'DATE'
-                    }
-                }
-            ],
-            'totalCount': 3
-        }
-    }
-}
-
-snapshots['test_schema_success[by-enum-name] 1'] = {
-    'data': {
-        'createField': {
-            'field': {
-                'fieldId': '4',
-                'name': 'author',
-                'type_': 'UNICODE_TEXT'
-            },
-            'ok': True
-        }
-    }
-}
-
-snapshots['test_schema_success[by-enum-name] 2'] = {
-    'data': {
-        'allFields': {
-            'edges': [
-                {
-                    'node': {
-                        'fieldId': '1',
-                        'name': 'contact',
-                        'type_': 'UNICODE_TEXT'
+                        'note': None,
+                        'path': 'site1:/path/to/beam1',
+                        'pathId': '5',
+                        'product': {'name': 'beam1'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '2',
-                        'name': 'produced_by',
-                        'type_': 'UNICODE_TEXT'
+                        'note': None,
+                        'path': 'site2:/another/way/beam1',
+                        'pathId': '6',
+                        'product': {'name': 'beam1'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '3',
-                        'name': 'date_produced',
-                        'type_': 'DATE'
+                        'note': None,
+                        'path': 'site1:/path/to/beam2',
+                        'pathId': '7',
+                        'product': {'name': 'beam2'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '4',
-                        'name': 'author',
-                        'type_': 'UNICODE_TEXT'
+                        'note': 'sample comment',
+                        'path': 'site1:/path/to/map1',
+                        'pathId': '8',
+                        'product': {'name': 'map1'},
                     }
-                }
+                },
             ],
-            'totalCount': 4
+            'totalCount': 8,
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/field/snapshots/snap_test_delete_field.py` & `acondbs-0.4.4/tests/schema/github/query/snapshots/snap_test_all_git_hub_orgs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,44 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_error[non-existent-field] 1'] = {
+snapshots['test_schema[one] 1'] = {
     'data': {
-        'allFields': {
+        'allGitHubOrgs': {
             'edges': [
                 {
                     'node': {
-                        'fieldId': '1',
-                        'name': 'contact',
-                        'type_': 'UNICODE_TEXT'
+                        'login': 'org1',
+                        'memberships': {
+                            'edges': [{'node': {'member': {'login': 'user1'}}}],
+                            'totalCount': 1,
+                        },
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '2',
-                        'name': 'produced_by',
-                        'type_': 'UNICODE_TEXT'
+                        'login': 'org2',
+                        'memberships': {
+                            'edges': [
+                                {'node': {'member': {'login': 'user1'}}},
+                                {'node': {'member': {'login': 'user2'}}},
+                            ],
+                            'totalCount': 2,
+                        },
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '3',
-                        'name': 'date_produced',
-                        'type_': 'DATE'
-                    }
-                }
-            ],
-            'totalCount': 3
-        }
-    }
-}
-
-snapshots['test_schema_success[one] 1'] = {
-    'data': {
-        'deleteField': {
-            'ok': True
-        }
-    }
-}
-
-snapshots['test_schema_success[one] 2'] = {
-    'data': {
-        'allFields': {
-            'edges': [
-                {
-                    'node': {
-                        'fieldId': '2',
-                        'name': 'produced_by',
-                        'type_': 'UNICODE_TEXT'
+                        'login': 'org3',
+                        'memberships': {'edges': [], 'totalCount': 0},
                     }
                 },
-                {
-                    'node': {
-                        'fieldId': '3',
-                        'name': 'date_produced',
-                        'type_': 'DATE'
-                    }
-                }
             ],
-            'totalCount': 2
+            'totalCount': 3,
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/field/snapshots/snap_test_update_field.py` & `acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_all_product_relations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,74 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_error[empty-input] 1'] = {
+snapshots['test_schema[query] 1'] = {
     'data': {
-        'allFields': {
+        'allProductRelations': {
             'edges': [
                 {
                     'node': {
-                        'fieldId': '1',
-                        'name': 'contact',
-                        'type_': 'UNICODE_TEXT'
+                        'other': {'name': 'beam1', 'productId': '4'},
+                        'relationId': '1',
+                        'reverse': {'relationId': '2'},
+                        'self_': {'name': 'map1', 'productId': '1'},
+                        'type_': {'name': 'child', 'typeId': '2'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '2',
-                        'name': 'produced_by',
-                        'type_': 'UNICODE_TEXT'
+                        'other': {'name': 'map1', 'productId': '1'},
+                        'relationId': '2',
+                        'reverse': {'relationId': '1'},
+                        'self_': {'name': 'beam1', 'productId': '4'},
+                        'type_': {'name': 'parent', 'typeId': '1'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '3',
-                        'name': 'date_produced',
-                        'type_': 'DATE'
-                    }
-                }
-            ],
-            'totalCount': 3
-        }
-    }
-}
-
-snapshots['test_schema_error[non-existent-field] 1'] = {
-    'data': {
-        'allFields': {
-            'edges': [
-                {
-                    'node': {
-                        'fieldId': '1',
-                        'name': 'contact',
-                        'type_': 'UNICODE_TEXT'
+                        'other': {'name': 'beam2', 'productId': '5'},
+                        'relationId': '3',
+                        'reverse': {'relationId': '4'},
+                        'self_': {'name': 'map1', 'productId': '1'},
+                        'type_': {'name': 'child', 'typeId': '2'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '2',
-                        'name': 'produced_by',
-                        'type_': 'UNICODE_TEXT'
+                        'other': {'name': 'map1', 'productId': '1'},
+                        'relationId': '4',
+                        'reverse': {'relationId': '3'},
+                        'self_': {'name': 'beam2', 'productId': '5'},
+                        'type_': {'name': 'parent', 'typeId': '1'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '3',
-                        'name': 'date_produced',
-                        'type_': 'DATE'
-                    }
-                }
-            ],
-            'totalCount': 3
-        }
-    }
-}
-
-snapshots['test_schema_success[one] 1'] = {
-    'data': {
-        'updateField': {
-            'field': {
-                'fieldId': '1',
-                'name': 'author',
-                'type_': 'UNICODE_TEXT'
-            },
-            'ok': True
-        }
-    }
-}
-
-snapshots['test_schema_success[one] 2'] = {
-    'data': {
-        'allFields': {
-            'edges': [
-                {
-                    'node': {
-                        'fieldId': '1',
-                        'name': 'author',
-                        'type_': 'UNICODE_TEXT'
+                        'other': {'name': 'beam2', 'productId': '5'},
+                        'relationId': '5',
+                        'reverse': {'relationId': '6'},
+                        'self_': {'name': 'beam1', 'productId': '4'},
+                        'type_': {'name': 'child', 'typeId': '2'},
                     }
                 },
                 {
                     'node': {
-                        'fieldId': '2',
-                        'name': 'produced_by',
-                        'type_': 'UNICODE_TEXT'
+                        'other': {'name': 'beam1', 'productId': '4'},
+                        'relationId': '6',
+                        'reverse': {'relationId': '5'},
+                        'self_': {'name': 'beam2', 'productId': '5'},
+                        'type_': {'name': 'parent', 'typeId': '1'},
                     }
                 },
-                {
-                    'node': {
-                        'fieldId': '3',
-                        'name': 'date_produced',
-                        'type_': 'DATE'
-                    }
-                }
-            ],
-            'totalCount': 3
+            ]
         }
     }
 }
+
+snapshots['test_schema[total-count] 1'] = {
+    'data': {'allProductRelations': {'totalCount': 6}}
+}
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/field/test_create_field.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_relation/test_create_product_relation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,103 @@
 import pytest
 
 from ....funcs import assert_mutation
-
-from ...gql import MUTATION_CREATE_FIELD, QUERY_ALL_FIELDS
+from ...gql import (
+    FRAGMENT_PRODUCT_RELATION_CONNECTION,
+    MUTATION_CREATE_PRODUCT_RELATION,
+)
+
+QEURY = (
+    """
+{
+  allProductRelations {
+    ...fragmentProductRelationConnection
+  }
+}
+"""
+    + FRAGMENT_PRODUCT_RELATION_CONNECTION
+)
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
-            "query": MUTATION_CREATE_FIELD,
+            "query": MUTATION_CREATE_PRODUCT_RELATION,
             "variables": {
-                "input": {
-                    "name": "author",
-                    "type_": "UNICODE_TEXT",
-                }
+                "input": {"typeId": 1, "selfProductId": 5, "otherProductId": 1}
             },
         },
-        {"query": QUERY_ALL_FIELDS},
-        id="by-enum-name",
+        {"query": QEURY},
+        id="create",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
-            "query": MUTATION_CREATE_FIELD,
+            "query": MUTATION_CREATE_PRODUCT_RELATION,
+            "variables": {
+                "input": {"typeId": 20, "selfProductId": 5, "otherProductId": 1}
+            },
+        },
+        {"query": QEURY},
+        id="error-type_id-nonexistent",
+    ),
+    pytest.param(
+        {
+            "query": MUTATION_CREATE_PRODUCT_RELATION,
             "variables": {
-                "input": {
-                    "name": "author",
-                    "type_": 1,
-                }
+                "input": {"typeId": 1, "selfProductId": 10, "otherProductId": 1}
             },
         },
-        {"query": QUERY_ALL_FIELDS},
-        id="by-enum-int",
+        {"query": QEURY},
+        id="error-self_product_id-nonexistent",
     ),
     pytest.param(
         {
-            "query": MUTATION_CREATE_FIELD,
+            "query": MUTATION_CREATE_PRODUCT_RELATION,
             "variables": {
-                "input": {
-                    "name": "author",
-                    "type_": "NONEXISTENT_ENUM",
-                }
+                "input": {"typeId": 1, "selfProductId": 5, "otherProductId": 20}
             },
         },
-        {"query": QUERY_ALL_FIELDS},
-        id="enum-nonexistent",
+        {"query": QEURY},
+        id="error-otheer_product_id-nonexistent",
+    ),
+    pytest.param(
+        {
+            "query": MUTATION_CREATE_PRODUCT_RELATION,
+            "variables": {
+                "input": {"typeId": 2, "selfProductId": 1, "otherProductId": 4}
+            },
+        },
+        {"query": QEURY},
+        id="error-duplicate",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_error(
@@ -89,10 +110,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/field/test_delete_field.py` & `acondbs-0.4.4/tests/schema/product/mutation/field/test_update_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 import pytest
 
 from ....funcs import assert_mutation
-
-from ...gql import MUTATION_DELETE_FIELD, QUERY_ALL_FIELDS
+from ...gql import MUTATION_UPDATE_FIELD, QUERY_ALL_FIELDS
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
-            "query": MUTATION_DELETE_FIELD,
+            "query": MUTATION_UPDATE_FIELD,
             "variables": {
                 "fieldId": 1,
+                "input": {
+                    "name": "author",
+                },
             },
         },
         {"query": QUERY_ALL_FIELDS},
         id="one",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
-            "query": MUTATION_DELETE_FIELD,
+            "query": MUTATION_UPDATE_FIELD,
+            "variables": {
+                "fieldId": 1,
+                "input": {},
+            },
+        },
+        {"query": QUERY_ALL_FIELDS},
+        id="empty-input",
+    ),
+    pytest.param(
+        {
+            "query": MUTATION_UPDATE_FIELD,
             "variables": {
                 "fieldId": 333,
+                "input": {
+                    "name": "author",
+                },
             },
         },
         {"query": QUERY_ALL_FIELDS},
         id="non-existent-field",
     ),
 ]
 
@@ -70,10 +83,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/field/test_update_field.py` & `acondbs-0.4.4/tests/schema/product/mutation/field/test_delete_field.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,55 @@
 import pytest
 
 from ....funcs import assert_mutation
-
-from ...gql import MUTATION_UPDATE_FIELD, QUERY_ALL_FIELDS
+from ...gql import MUTATION_DELETE_FIELD, QUERY_ALL_FIELDS
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
-            "query": MUTATION_UPDATE_FIELD,
+            "query": MUTATION_DELETE_FIELD,
             "variables": {
                 "fieldId": 1,
-                "input": {
-                    "name": "author",
-                },
             },
         },
         {"query": QUERY_ALL_FIELDS},
         id="one",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
-            "query": MUTATION_UPDATE_FIELD,
-            "variables": {
-                "fieldId": 1,
-                "input": {},
-            },
-        },
-        {"query": QUERY_ALL_FIELDS},
-        id="empty-input",
-    ),
-    pytest.param(
-        {
-            "query": MUTATION_UPDATE_FIELD,
+            "query": MUTATION_DELETE_FIELD,
             "variables": {
                 "fieldId": 333,
-                "input": {
-                    "name": "author",
-                },
             },
         },
         {"query": QUERY_ALL_FIELDS},
         id="non-existent-field",
     ),
 ]
 
@@ -87,10 +66,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product/conftest.py` & `acondbs-0.4.4/tests/schema/product/query/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,61 @@
-import pytest
-
 import datetime
 
-from acondbs.db.sa import sa
-from acondbs.models import (
-    GitHubUser,
-    GitHubToken,
-)
+import pytest
 
 from acondbs import ops
 
 
-##__________________________________________________________________||
 @pytest.fixture
-def app(app_empty):
-
-    y = app_empty
-
-    user1 = GitHubUser(login="user1", git_hub_id="04:User1")
-    token1 = GitHubToken(
-        token="39d86487d76a84087f1da599c872dac4473e5f07", scope="", user=user1
-    )
+def app(app_users):
+    y = app_users
 
-    with y.app_context():
-        sa.session.add(user1)
-        sa.session.add(token1)
-        sa.session.commit()
-
-    # map1 -> beam1
-    #   |        |
-    #   +--------+---> beam2
+    # Relation types:
+    #   parent <-> child
+    #   plaintiff <-> defendant
+
+    # Products and Relations:
+    #   map1 -> beam1
+    #     |        |
+    #     +--------+---> beam2
     #
-    # map2
-    # map3
+    #   map2
+    #   map3
 
     with y.app_context():
         ops.create_product_relation_type(
             type_={
                 "type_id": 1,
                 "name": "parent",
+                "indef_article": "a",
+                "singular": "parent",
+                "plural": "parents",
             },
             reverse={
                 "type_id": 2,
                 "name": "child",
+                "indef_article": "a",
+                "singular": "child",
+                "plural": "children",
+            },
+        )
+        ops.create_product_relation_type(
+            type_={
+                "type_id": 3,
+                "name": "plaintiff",
+                "indef_article": "a",
+                "singular": "plaintiff",
+                "plural": "plaintiffs",
+            },
+            reverse={
+                "type_id": 4,
+                "name": "defendant",
+                "indef_article": "a",
+                "singular": "defendant",
+                "plural": "defendants",
             },
         )
         ops.commit()
 
     with y.app_context():
         ops.create_field(
             field_id=1,
@@ -65,30 +74,40 @@
         )
         ops.commit()
 
     with y.app_context():
         ops.create_product_type(
             type_id=1,
             name="map",
+            order=2,
+            indef_article="a",
+            singular="map",
+            plural="maps",
+            icon="mdi-map",
             field_ids=[1, 2, 3],
         )
         ops.create_product_type(
             type_id=2,
             name="beam",
+            order=1,
+            indef_article="a",
+            singular="beam",
+            plural="beams",
+            icon="mdi-spotlight-beam",
             field_ids=[1, 2, 3],
         )
         ops.commit()
 
     with y.app_context():
         ops.create_product(
             type_id=1,
             product_id=1,
             name="map1",
             attributes={3: datetime.date(2020, 2, 1)},
-            paths=["site1:/path/to/map1", "site2:/another/way/map1"],
+            paths=["site2:/another/way/map1"],
         )
         ops.create_product(
             type_id=1,
             product_id=2,
             name="map2",
             attributes={3: datetime.date(2020, 2, 10)},
             paths=["site1:/path/to/map2"],
@@ -113,14 +132,22 @@
             name="beam2",
             attributes={3: datetime.date(2020, 3, 4)},
             paths=["site1:/path/to/beam2"],
         )
         ops.commit()
 
     with y.app_context():
+        ops.create_product_file_path(
+            product_id=1,
+            path="site1:/path/to/map1",
+            note="sample comment",
+        )
+        ops.commit()
+
+    with y.app_context():
         ops.create_product_relation(
             type_id=1,
             self_product_id=4,
             other_product_id=1,
         )
         ops.create_product_relation(
             type_id=1,
@@ -131,10 +158,7 @@
             type_id=1,
             self_product_id=5,
             other_product_id=4,
         )
         ops.commit()
 
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product/snapshots/snap_test_convert_product_type.py` & `acondbs-0.4.4/tests/schema/product/mutation/product/snapshots/snap_test_convert_product_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,911 +1,711 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_schema_success[convert] 1'] = {
     'data': {
         'convertProductType': {
             'ok': True,
             'product': {
-                'attributesBoolean': {
-                    'edges': [
-                    ]
-                },
+                'attributesBoolean': {'edges': []},
                 'attributesDate': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'date_produced',
-                                    'type_': 'DATE'
-                                },
+                                'field': {'name': 'date_produced', 'type_': 'DATE'},
                                 'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'date_produced',
-                                        'type_': 'DATE'
-                                    }
+                                    'field': {'name': 'date_produced', 'type_': 'DATE'}
                                 },
-                                'value': '2020-02-01'
+                                'value': '2020-02-01',
                             }
                         }
                     ]
                 },
-                'attributesDateTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesFloat': {
-                    'edges': [
-                    ]
-                },
-                'attributesInteger': {
-                    'edges': [
-                    ]
-                },
-                'attributesTime': {
-                    'edges': [
-                    ]
-                },
+                'attributesDateTime': {'edges': []},
+                'attributesFloat': {'edges': []},
+                'attributesInteger': {'edges': []},
+                'attributesTime': {'edges': []},
                 'attributesUnicodeText': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'contact',
-                                    'type_': 'UNICODE_TEXT'
-                                },
+                                'field': {'name': 'contact', 'type_': 'UNICODE_TEXT'},
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'contact',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
                         },
                         {
                             'node': {
                                 'field': {
                                     'name': 'produced_by',
-                                    'type_': 'UNICODE_TEXT'
+                                    'type_': 'UNICODE_TEXT',
                                 },
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'produced_by',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
-                        }
+                        },
                     ]
                 },
                 'name': 'map1',
                 'note': None,
                 'paths': {
                     'edges': [
                         {
                             'node': {
                                 'note': None,
                                 'path': 'site1:/path/to/map1',
-                                'pathId': '1'
+                                'pathId': '1',
                             }
                         },
                         {
                             'node': {
                                 'note': None,
                                 'path': 'site2:/another/way/map1',
-                                'pathId': '2'
+                                'pathId': '2',
                             }
-                        }
+                        },
                     ]
                 },
                 'postingGitHubUser': None,
                 'productId': '1',
                 'relations': {
                     'edges': [
                         {
                             'node': {
                                 'other': {
                                     'name': 'beam1',
                                     'productId': '4',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'beam', 'typeId': '2'},
                                 },
                                 'otherProductId': 4,
                                 'relationId': '1',
                                 'reverse': {
                                     'relationId': '2',
                                     'typeId': 1,
-                                    'type_': {
-                                        'name': 'parent',
-                                        'typeId': '1'
-                                    }
+                                    'type_': {'name': 'parent', 'typeId': '1'},
                                 },
                                 'reverseRelationId': 2,
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'child',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'child', 'typeId': '2'},
                             }
                         },
                         {
                             'node': {
                                 'other': {
                                     'name': 'beam2',
                                     'productId': '5',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'beam', 'typeId': '2'},
                                 },
                                 'otherProductId': 5,
                                 'relationId': '3',
                                 'reverse': {
                                     'relationId': '4',
                                     'typeId': 1,
-                                    'type_': {
-                                        'name': 'parent',
-                                        'typeId': '1'
-                                    }
+                                    'type_': {'name': 'parent', 'typeId': '1'},
                                 },
                                 'reverseRelationId': 4,
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'child',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'child', 'typeId': '2'},
                             }
-                        }
+                        },
                     ]
                 },
                 'timePosted': '2021-01-04T14:32:20',
                 'timeUpdated': '2021-01-04T14:32:20',
                 'typeId': 2,
-                'type_': {
-                    'name': 'beam',
-                    'typeId': '2'
-                },
-                'updatingGitHubUser': {
-                    'login': 'user1'
-                }
-            }
+                'type_': {'name': 'beam', 'typeId': '2'},
+                'updatingGitHubUser': {'login': 'user1'},
+            },
         }
     }
 }
 
 snapshots['test_schema_success[convert] 2'] = {
     'data': {
         'allProducts': {
             'edges': [
                 {
                     'node': {
-                        'attributesBoolean': {
-                            'edges': [
-                            ]
-                        },
+                        'attributesBoolean': {'edges': []},
                         'attributesDate': {
                             'edges': [
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'date_produced',
-                                            'type_': 'DATE'
+                                            'type_': 'DATE',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'date_produced',
-                                                'type_': 'DATE'
+                                                'type_': 'DATE',
                                             }
                                         },
-                                        'value': '2020-02-01'
+                                        'value': '2020-02-01',
                                     }
                                 }
                             ]
                         },
-                        'attributesDateTime': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesFloat': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesInteger': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesTime': {
-                            'edges': [
-                            ]
-                        },
+                        'attributesDateTime': {'edges': []},
+                        'attributesFloat': {'edges': []},
+                        'attributesInteger': {'edges': []},
+                        'attributesTime': {'edges': []},
                         'attributesUnicodeText': {
                             'edges': [
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'contact',
-                                            'type_': 'UNICODE_TEXT'
+                                            'type_': 'UNICODE_TEXT',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'contact',
-                                                'type_': 'UNICODE_TEXT'
+                                                'type_': 'UNICODE_TEXT',
                                             }
                                         },
-                                        'value': None
+                                        'value': None,
                                     }
                                 },
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'produced_by',
-                                            'type_': 'UNICODE_TEXT'
+                                            'type_': 'UNICODE_TEXT',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'produced_by',
-                                                'type_': 'UNICODE_TEXT'
+                                                'type_': 'UNICODE_TEXT',
                                             }
                                         },
-                                        'value': None
+                                        'value': None,
                                     }
-                                }
+                                },
                             ]
                         },
                         'name': 'map1',
                         'note': None,
                         'paths': {
                             'edges': [
                                 {
                                     'node': {
                                         'note': None,
                                         'path': 'site1:/path/to/map1',
-                                        'pathId': '1'
+                                        'pathId': '1',
                                     }
                                 },
                                 {
                                     'node': {
                                         'note': None,
                                         'path': 'site2:/another/way/map1',
-                                        'pathId': '2'
+                                        'pathId': '2',
                                     }
-                                }
+                                },
                             ]
                         },
                         'postingGitHubUser': None,
                         'productId': '1',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
                                         'other': {
                                             'name': 'beam1',
                                             'productId': '4',
                                             'typeId': 2,
-                                            'type_': {
-                                                'name': 'beam',
-                                                'typeId': '2'
-                                            }
+                                            'type_': {'name': 'beam', 'typeId': '2'},
                                         },
                                         'otherProductId': 4,
                                         'relationId': '1',
                                         'reverse': {
                                             'relationId': '2',
                                             'typeId': 1,
-                                            'type_': {
-                                                'name': 'parent',
-                                                'typeId': '1'
-                                            }
+                                            'type_': {'name': 'parent', 'typeId': '1'},
                                         },
                                         'reverseRelationId': 2,
                                         'typeId': 2,
-                                        'type_': {
-                                            'name': 'child',
-                                            'typeId': '2'
-                                        }
+                                        'type_': {'name': 'child', 'typeId': '2'},
                                     }
                                 },
                                 {
                                     'node': {
                                         'other': {
                                             'name': 'beam2',
                                             'productId': '5',
                                             'typeId': 2,
-                                            'type_': {
-                                                'name': 'beam',
-                                                'typeId': '2'
-                                            }
+                                            'type_': {'name': 'beam', 'typeId': '2'},
                                         },
                                         'otherProductId': 5,
                                         'relationId': '3',
                                         'reverse': {
                                             'relationId': '4',
                                             'typeId': 1,
-                                            'type_': {
-                                                'name': 'parent',
-                                                'typeId': '1'
-                                            }
+                                            'type_': {'name': 'parent', 'typeId': '1'},
                                         },
                                         'reverseRelationId': 4,
                                         'typeId': 2,
-                                        'type_': {
-                                            'name': 'child',
-                                            'typeId': '2'
-                                        }
+                                        'type_': {'name': 'child', 'typeId': '2'},
                                     }
-                                }
+                                },
                             ]
                         },
                         'timePosted': '2021-01-04T14:32:20',
                         'timeUpdated': '2021-01-04T14:32:20',
                         'typeId': 2,
-                        'type_': {
-                            'name': 'beam',
-                            'typeId': '2'
-                        },
-                        'updatingGitHubUser': {
-                            'login': 'user1'
-                        }
+                        'type_': {'name': 'beam', 'typeId': '2'},
+                        'updatingGitHubUser': {'login': 'user1'},
                     }
                 },
                 {
                     'node': {
-                        'attributesBoolean': {
-                            'edges': [
-                            ]
-                        },
+                        'attributesBoolean': {'edges': []},
                         'attributesDate': {
                             'edges': [
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'date_produced',
-                                            'type_': 'DATE'
+                                            'type_': 'DATE',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'date_produced',
-                                                'type_': 'DATE'
+                                                'type_': 'DATE',
                                             }
                                         },
-                                        'value': '2020-02-10'
+                                        'value': '2020-02-10',
                                     }
                                 }
                             ]
                         },
-                        'attributesDateTime': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesFloat': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesInteger': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesTime': {
-                            'edges': [
-                            ]
-                        },
+                        'attributesDateTime': {'edges': []},
+                        'attributesFloat': {'edges': []},
+                        'attributesInteger': {'edges': []},
+                        'attributesTime': {'edges': []},
                         'attributesUnicodeText': {
                             'edges': [
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'contact',
-                                            'type_': 'UNICODE_TEXT'
+                                            'type_': 'UNICODE_TEXT',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'contact',
-                                                'type_': 'UNICODE_TEXT'
+                                                'type_': 'UNICODE_TEXT',
                                             }
                                         },
-                                        'value': None
+                                        'value': None,
                                     }
                                 },
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'produced_by',
-                                            'type_': 'UNICODE_TEXT'
+                                            'type_': 'UNICODE_TEXT',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'produced_by',
-                                                'type_': 'UNICODE_TEXT'
+                                                'type_': 'UNICODE_TEXT',
                                             }
                                         },
-                                        'value': None
+                                        'value': None,
                                     }
-                                }
+                                },
                             ]
                         },
                         'name': 'map2',
                         'note': None,
                         'paths': {
                             'edges': [
                                 {
                                     'node': {
                                         'note': None,
                                         'path': 'site1:/path/to/map2',
-                                        'pathId': '3'
+                                        'pathId': '3',
                                     }
                                 }
                             ]
                         },
                         'postingGitHubUser': None,
                         'productId': '2',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
+                        'relations': {'edges': []},
                         'timePosted': '2021-01-04T14:32:20',
                         'timeUpdated': None,
                         'typeId': 1,
-                        'type_': {
-                            'name': 'map',
-                            'typeId': '1'
-                        },
-                        'updatingGitHubUser': None
+                        'type_': {'name': 'map', 'typeId': '1'},
+                        'updatingGitHubUser': None,
                     }
                 },
                 {
                     'node': {
-                        'attributesBoolean': {
-                            'edges': [
-                            ]
-                        },
+                        'attributesBoolean': {'edges': []},
                         'attributesDate': {
                             'edges': [
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'date_produced',
-                                            'type_': 'DATE'
+                                            'type_': 'DATE',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'date_produced',
-                                                'type_': 'DATE'
+                                                'type_': 'DATE',
                                             }
                                         },
-                                        'value': '2020-03-19'
+                                        'value': '2020-03-19',
                                     }
                                 }
                             ]
                         },
-                        'attributesDateTime': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesFloat': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesInteger': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesTime': {
-                            'edges': [
-                            ]
-                        },
+                        'attributesDateTime': {'edges': []},
+                        'attributesFloat': {'edges': []},
+                        'attributesInteger': {'edges': []},
+                        'attributesTime': {'edges': []},
                         'attributesUnicodeText': {
                             'edges': [
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'contact',
-                                            'type_': 'UNICODE_TEXT'
+                                            'type_': 'UNICODE_TEXT',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'contact',
-                                                'type_': 'UNICODE_TEXT'
+                                                'type_': 'UNICODE_TEXT',
                                             }
                                         },
-                                        'value': None
+                                        'value': None,
                                     }
                                 },
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'produced_by',
-                                            'type_': 'UNICODE_TEXT'
+                                            'type_': 'UNICODE_TEXT',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'produced_by',
-                                                'type_': 'UNICODE_TEXT'
+                                                'type_': 'UNICODE_TEXT',
                                             }
                                         },
-                                        'value': None
+                                        'value': None,
                                     }
-                                }
+                                },
                             ]
                         },
                         'name': 'map3',
                         'note': None,
                         'paths': {
                             'edges': [
                                 {
                                     'node': {
                                         'note': None,
                                         'path': 'site1:/path/to/map3',
-                                        'pathId': '4'
+                                        'pathId': '4',
                                     }
                                 },
                                 {
                                     'node': {
                                         'note': None,
                                         'path': 'site2:/another/way/map3',
-                                        'pathId': '5'
+                                        'pathId': '5',
                                     }
-                                }
+                                },
                             ]
                         },
                         'postingGitHubUser': None,
                         'productId': '3',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
+                        'relations': {'edges': []},
                         'timePosted': '2021-01-04T14:32:20',
                         'timeUpdated': None,
                         'typeId': 1,
-                        'type_': {
-                            'name': 'map',
-                            'typeId': '1'
-                        },
-                        'updatingGitHubUser': None
+                        'type_': {'name': 'map', 'typeId': '1'},
+                        'updatingGitHubUser': None,
                     }
                 },
                 {
                     'node': {
-                        'attributesBoolean': {
-                            'edges': [
-                            ]
-                        },
+                        'attributesBoolean': {'edges': []},
                         'attributesDate': {
                             'edges': [
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'date_produced',
-                                            'type_': 'DATE'
+                                            'type_': 'DATE',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'date_produced',
-                                                'type_': 'DATE'
+                                                'type_': 'DATE',
                                             }
                                         },
-                                        'value': '2020-02-05'
+                                        'value': '2020-02-05',
                                     }
                                 }
                             ]
                         },
-                        'attributesDateTime': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesFloat': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesInteger': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesTime': {
-                            'edges': [
-                            ]
-                        },
+                        'attributesDateTime': {'edges': []},
+                        'attributesFloat': {'edges': []},
+                        'attributesInteger': {'edges': []},
+                        'attributesTime': {'edges': []},
                         'attributesUnicodeText': {
                             'edges': [
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'contact',
-                                            'type_': 'UNICODE_TEXT'
+                                            'type_': 'UNICODE_TEXT',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'contact',
-                                                'type_': 'UNICODE_TEXT'
+                                                'type_': 'UNICODE_TEXT',
                                             }
                                         },
-                                        'value': None
+                                        'value': None,
                                     }
                                 },
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'produced_by',
-                                            'type_': 'UNICODE_TEXT'
+                                            'type_': 'UNICODE_TEXT',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'produced_by',
-                                                'type_': 'UNICODE_TEXT'
+                                                'type_': 'UNICODE_TEXT',
                                             }
                                         },
-                                        'value': None
+                                        'value': None,
                                     }
-                                }
+                                },
                             ]
                         },
                         'name': 'beam1',
                         'note': None,
                         'paths': {
                             'edges': [
                                 {
                                     'node': {
                                         'note': None,
                                         'path': 'site1:/path/to/beam1',
-                                        'pathId': '6'
+                                        'pathId': '6',
                                     }
                                 },
                                 {
                                     'node': {
                                         'note': None,
                                         'path': 'site2:/another/way/beam1',
-                                        'pathId': '7'
+                                        'pathId': '7',
                                     }
-                                }
+                                },
                             ]
                         },
                         'postingGitHubUser': None,
                         'productId': '4',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
                                         'other': {
                                             'name': 'map1',
                                             'productId': '1',
                                             'typeId': 2,
-                                            'type_': {
-                                                'name': 'beam',
-                                                'typeId': '2'
-                                            }
+                                            'type_': {'name': 'beam', 'typeId': '2'},
                                         },
                                         'otherProductId': 1,
                                         'relationId': '2',
                                         'reverse': {
                                             'relationId': '1',
                                             'typeId': 2,
-                                            'type_': {
-                                                'name': 'child',
-                                                'typeId': '2'
-                                            }
+                                            'type_': {'name': 'child', 'typeId': '2'},
                                         },
                                         'reverseRelationId': 1,
                                         'typeId': 1,
-                                        'type_': {
-                                            'name': 'parent',
-                                            'typeId': '1'
-                                        }
+                                        'type_': {'name': 'parent', 'typeId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
                                         'other': {
                                             'name': 'beam2',
                                             'productId': '5',
                                             'typeId': 2,
-                                            'type_': {
-                                                'name': 'beam',
-                                                'typeId': '2'
-                                            }
+                                            'type_': {'name': 'beam', 'typeId': '2'},
                                         },
                                         'otherProductId': 5,
                                         'relationId': '5',
                                         'reverse': {
                                             'relationId': '6',
                                             'typeId': 1,
-                                            'type_': {
-                                                'name': 'parent',
-                                                'typeId': '1'
-                                            }
+                                            'type_': {'name': 'parent', 'typeId': '1'},
                                         },
                                         'reverseRelationId': 6,
                                         'typeId': 2,
-                                        'type_': {
-                                            'name': 'child',
-                                            'typeId': '2'
-                                        }
+                                        'type_': {'name': 'child', 'typeId': '2'},
                                     }
-                                }
+                                },
                             ]
                         },
                         'timePosted': '2021-01-04T14:32:20',
                         'timeUpdated': None,
                         'typeId': 2,
-                        'type_': {
-                            'name': 'beam',
-                            'typeId': '2'
-                        },
-                        'updatingGitHubUser': None
+                        'type_': {'name': 'beam', 'typeId': '2'},
+                        'updatingGitHubUser': None,
                     }
                 },
                 {
                     'node': {
-                        'attributesBoolean': {
-                            'edges': [
-                            ]
-                        },
+                        'attributesBoolean': {'edges': []},
                         'attributesDate': {
                             'edges': [
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'date_produced',
-                                            'type_': 'DATE'
+                                            'type_': 'DATE',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'date_produced',
-                                                'type_': 'DATE'
+                                                'type_': 'DATE',
                                             }
                                         },
-                                        'value': '2020-03-04'
+                                        'value': '2020-03-04',
                                     }
                                 }
                             ]
                         },
-                        'attributesDateTime': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesFloat': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesInteger': {
-                            'edges': [
-                            ]
-                        },
-                        'attributesTime': {
-                            'edges': [
-                            ]
-                        },
+                        'attributesDateTime': {'edges': []},
+                        'attributesFloat': {'edges': []},
+                        'attributesInteger': {'edges': []},
+                        'attributesTime': {'edges': []},
                         'attributesUnicodeText': {
                             'edges': [
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'contact',
-                                            'type_': 'UNICODE_TEXT'
+                                            'type_': 'UNICODE_TEXT',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'contact',
-                                                'type_': 'UNICODE_TEXT'
+                                                'type_': 'UNICODE_TEXT',
                                             }
                                         },
-                                        'value': None
+                                        'value': None,
                                     }
                                 },
                                 {
                                     'node': {
                                         'field': {
                                             'name': 'produced_by',
-                                            'type_': 'UNICODE_TEXT'
+                                            'type_': 'UNICODE_TEXT',
                                         },
                                         'typeFieldAssociation': {
                                             'field': {
                                                 'name': 'produced_by',
-                                                'type_': 'UNICODE_TEXT'
+                                                'type_': 'UNICODE_TEXT',
                                             }
                                         },
-                                        'value': None
+                                        'value': None,
                                     }
-                                }
+                                },
                             ]
                         },
                         'name': 'beam2',
                         'note': None,
                         'paths': {
                             'edges': [
                                 {
                                     'node': {
                                         'note': None,
                                         'path': 'site1:/path/to/beam2',
-                                        'pathId': '8'
+                                        'pathId': '8',
                                     }
                                 }
                             ]
                         },
                         'postingGitHubUser': None,
                         'productId': '5',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
                                         'other': {
                                             'name': 'map1',
                                             'productId': '1',
                                             'typeId': 2,
-                                            'type_': {
-                                                'name': 'beam',
-                                                'typeId': '2'
-                                            }
+                                            'type_': {'name': 'beam', 'typeId': '2'},
                                         },
                                         'otherProductId': 1,
                                         'relationId': '4',
                                         'reverse': {
                                             'relationId': '3',
                                             'typeId': 2,
-                                            'type_': {
-                                                'name': 'child',
-                                                'typeId': '2'
-                                            }
+                                            'type_': {'name': 'child', 'typeId': '2'},
                                         },
                                         'reverseRelationId': 3,
                                         'typeId': 1,
-                                        'type_': {
-                                            'name': 'parent',
-                                            'typeId': '1'
-                                        }
+                                        'type_': {'name': 'parent', 'typeId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
                                         'other': {
                                             'name': 'beam1',
                                             'productId': '4',
                                             'typeId': 2,
-                                            'type_': {
-                                                'name': 'beam',
-                                                'typeId': '2'
-                                            }
+                                            'type_': {'name': 'beam', 'typeId': '2'},
                                         },
                                         'otherProductId': 4,
                                         'relationId': '6',
                                         'reverse': {
                                             'relationId': '5',
                                             'typeId': 2,
-                                            'type_': {
-                                                'name': 'child',
-                                                'typeId': '2'
-                                            }
+                                            'type_': {'name': 'child', 'typeId': '2'},
                                         },
                                         'reverseRelationId': 5,
                                         'typeId': 1,
-                                        'type_': {
-                                            'name': 'parent',
-                                            'typeId': '1'
-                                        }
+                                        'type_': {'name': 'parent', 'typeId': '1'},
                                     }
-                                }
+                                },
                             ]
                         },
                         'timePosted': '2021-01-04T14:32:20',
                         'timeUpdated': None,
                         'typeId': 2,
-                        'type_': {
-                            'name': 'beam',
-                            'typeId': '2'
-                        },
-                        'updatingGitHubUser': None
+                        'type_': {'name': 'beam', 'typeId': '2'},
+                        'updatingGitHubUser': None,
                     }
-                }
+                },
             ]
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product/snapshots/snap_test_create_product.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_type/snapshots/snap_test_create_product_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1296 +1,855 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_error[error-no-name] 1'] = {
+snapshots['test_schema_error[error-already-exist] 1'] = {
     'data': {
-        'allProductFilePaths': {
-            'edges': [
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                }
-            ]
-        },
-        'allProductRelations': {
+        'allProductTypes': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam1'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                            ]
+                        },
+                        'icon': 'mdi-spotlight-beam',
+                        'indefArticle': 'a',
+                        'name': 'beam',
+                        'order': 1,
+                        'plural': 'beams',
+                        'products': {'edges': []},
+                        'singular': 'beam',
+                        'typeId': '2',
+                    }
+                },
+                {
+                    'node': {
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                            ]
+                        },
+                        'icon': 'mdi-map',
+                        'indefArticle': 'a',
+                        'name': 'map',
+                        'order': 2,
+                        'plural': 'maps',
+                        'products': {
+                            'edges': [
+                                {'node': {'name': 'map1'}},
+                                {'node': {'name': 'map2'}},
+                                {'node': {'name': 'map3'}},
+                            ]
                         },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                }
-            ]
-        },
-        'allProducts': {
-            'edges': [
-                {
-                    'node': {
-                        'name': 'map1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map3'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam1'
+                        'singular': 'map',
+                        'typeId': '1',
                     }
                 },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                }
-            ]
+            ],
+            'totalCount': 2,
         }
     }
 }
 
-snapshots['test_schema_error[error-the-same-type-and-name] 1'] = {
+snapshots['test_schema_error[non-existent-field] 1'] = {
     'data': {
-        'allProductFilePaths': {
-            'edges': [
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                }
-            ]
-        },
-        'allProductRelations': {
+        'allProductTypes': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'map1'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                            ]
+                        },
+                        'icon': 'mdi-spotlight-beam',
+                        'indefArticle': 'a',
+                        'name': 'beam',
+                        'order': 1,
+                        'plural': 'beams',
+                        'products': {'edges': []},
+                        'singular': 'beam',
+                        'typeId': '2',
+                    }
+                },
+                {
+                    'node': {
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                            ]
+                        },
+                        'icon': 'mdi-map',
+                        'indefArticle': 'a',
+                        'name': 'map',
+                        'order': 2,
+                        'plural': 'maps',
+                        'products': {
+                            'edges': [
+                                {'node': {'name': 'map1'}},
+                                {'node': {'name': 'map2'}},
+                                {'node': {'name': 'map3'}},
+                            ]
                         },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                }
-            ]
-        },
-        'allProducts': {
-            'edges': [
-                {
-                    'node': {
-                        'name': 'map1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map3'
+                        'singular': 'map',
+                        'typeId': '1',
                     }
                 },
-                {
-                    'node': {
-                        'name': 'beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                }
-            ]
+            ],
+            'totalCount': 2,
         }
     }
 }
 
 snapshots['test_schema_success[create] 1'] = {
     'data': {
-        'createProduct': {
+        'createProductType': {
             'ok': True,
-            'product': {
-                'attributesBoolean': {
-                    'edges': [
-                    ]
-                },
-                'attributesDate': {
-                    'edges': [
-                        {
-                            'node': {
-                                'field': {
-                                    'name': 'date_produced',
-                                    'type_': 'DATE'
-                                },
-                                'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'date_produced',
-                                        'type_': 'DATE'
-                                    }
-                                },
-                                'value': '2020-02-20'
-                            }
-                        }
-                    ]
-                },
-                'attributesDateTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesFloat': {
-                    'edges': [
-                    ]
-                },
-                'attributesInteger': {
-                    'edges': [
-                    ]
-                },
-                'attributesTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesUnicodeText': {
+            'productType': {
+                'fields': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'contact',
-                                    'type_': 'UNICODE_TEXT'
-                                },
-                                'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'contact',
-                                        'type_': 'UNICODE_TEXT'
-                                    }
-                                },
-                                'value': 'contact-person'
+                                'field': {'name': 'contact', 'type_': 'UNICODE_TEXT'},
+                                'type_': {'name': 'compass'},
                             }
                         },
                         {
                             'node': {
                                 'field': {
                                     'name': 'produced_by',
-                                    'type_': 'UNICODE_TEXT'
-                                },
-                                'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'produced_by',
-                                        'type_': 'UNICODE_TEXT'
-                                    }
+                                    'type_': 'UNICODE_TEXT',
                                 },
-                                'value': 'producer'
-                            }
-                        }
-                    ]
-                },
-                'name': 'beam111',
-                'note': '- Item 1',
-                'paths': {
-                    'edges': [
-                        {
-                            'node': {
-                                'note': None,
-                                'path': '/path/to/new/product1',
-                                'pathId': '9'
+                                'type_': {'name': 'compass'},
                             }
                         },
                         {
                             'node': {
-                                'note': None,
-                                'path': '/another/location/of/product1',
-                                'pathId': '10'
-                            }
-                        }
-                    ]
-                },
-                'postingGitHubUser': {
-                    'login': 'user1'
-                },
-                'productId': '6',
-                'relations': {
-                    'edges': [
-                        {
-                            'node': {
-                                'other': {
-                                    'name': 'map1',
-                                    'productId': '1',
-                                    'typeId': 1,
-                                    'type_': {
-                                        'name': 'map',
-                                        'typeId': '1'
-                                    }
-                                },
-                                'otherProductId': 1,
-                                'relationId': '8',
-                                'reverse': {
-                                    'relationId': '7',
-                                    'typeId': 2,
-                                    'type_': {
-                                        'name': 'child',
-                                        'typeId': '2'
-                                    }
-                                },
-                                'reverseRelationId': 7,
-                                'typeId': 1,
-                                'type_': {
-                                    'name': 'parent',
-                                    'typeId': '1'
-                                }
+                                'field': {'name': 'date_produced', 'type_': 'DATE'},
+                                'type_': {'name': 'compass'},
                             }
                         },
-                        {
-                            'node': {
-                                'other': {
-                                    'name': 'beam2',
-                                    'productId': '5',
-                                    'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
-                                },
-                                'otherProductId': 5,
-                                'relationId': '10',
-                                'reverse': {
-                                    'relationId': '9',
-                                    'typeId': 2,
-                                    'type_': {
-                                        'name': 'child',
-                                        'typeId': '2'
-                                    }
-                                },
-                                'reverseRelationId': 9,
-                                'typeId': 1,
-                                'type_': {
-                                    'name': 'parent',
-                                    'typeId': '1'
-                                }
-                            }
-                        }
                     ]
                 },
-                'timePosted': '2021-01-04T14:32:20',
-                'timeUpdated': None,
-                'typeId': 2,
-                'type_': {
-                    'name': 'beam',
-                    'typeId': '2'
-                },
-                'updatingGitHubUser': None
-            }
+                'icon': 'mdi-compass',
+                'indefArticle': 'a',
+                'name': 'compass',
+                'order': 5,
+                'plural': 'compasses',
+                'products': {'edges': []},
+                'singular': 'compass',
+                'typeId': '3',
+            },
         }
     }
 }
 
 snapshots['test_schema_success[create] 2'] = {
     'data': {
-        'allProductFilePaths': {
-            'edges': [
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': '/path/to/new/product1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': '/another/location/of/product1'
-                    }
-                }
-            ]
-        },
-        'allProductRelations': {
+        'allProductTypes': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam111'
-                        },
-                        'self_': {
-                            'name': 'map1'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                            ]
                         },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'icon': 'mdi-spotlight-beam',
+                        'indefArticle': 'a',
+                        'name': 'beam',
+                        'order': 1,
+                        'plural': 'beams',
+                        'products': {'edges': []},
+                        'singular': 'beam',
+                        'typeId': '2',
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                            ]
                         },
-                        'self_': {
-                            'name': 'beam111'
+                        'icon': 'mdi-map',
+                        'indefArticle': 'a',
+                        'name': 'map',
+                        'order': 2,
+                        'plural': 'maps',
+                        'products': {
+                            'edges': [
+                                {'node': {'name': 'map1'}},
+                                {'node': {'name': 'map2'}},
+                                {'node': {'name': 'map3'}},
+                            ]
                         },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'singular': 'map',
+                        'typeId': '1',
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam111'
-                        },
-                        'self_': {
-                            'name': 'beam2'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'compass'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'compass'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'compass'},
+                                    }
+                                },
+                            ]
                         },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'icon': 'mdi-compass',
+                        'indefArticle': 'a',
+                        'name': 'compass',
+                        'order': 5,
+                        'plural': 'compasses',
+                        'products': {'edges': []},
+                        'singular': 'compass',
+                        'typeId': '3',
                     }
                 },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam111'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                }
-            ]
-        },
-        'allProducts': {
-            'edges': [
-                {
-                    'node': {
-                        'name': 'map1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map3'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam111'
-                    }
-                }
-            ]
+            ],
+            'totalCount': 3,
         }
     }
 }
 
-snapshots['test_schema_success[minimum] 1'] = {
+snapshots['test_schema_success[empty-fields] 1'] = {
     'data': {
-        'createProduct': {
+        'createProductType': {
             'ok': True,
-            'product': {
-                'attributesBoolean': {
-                    'edges': [
-                    ]
-                },
-                'attributesDate': {
-                    'edges': [
-                        {
-                            'node': {
-                                'field': {
-                                    'name': 'date_produced',
-                                    'type_': 'DATE'
-                                },
-                                'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'date_produced',
-                                        'type_': 'DATE'
-                                    }
-                                },
-                                'value': None
-                            }
-                        }
-                    ]
-                },
-                'attributesDateTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesFloat': {
-                    'edges': [
-                    ]
-                },
-                'attributesInteger': {
-                    'edges': [
-                    ]
-                },
-                'attributesTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesUnicodeText': {
-                    'edges': [
-                        {
-                            'node': {
-                                'field': {
-                                    'name': 'contact',
-                                    'type_': 'UNICODE_TEXT'
-                                },
-                                'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'contact',
-                                        'type_': 'UNICODE_TEXT'
-                                    }
-                                },
-                                'value': None
-                            }
-                        },
-                        {
-                            'node': {
-                                'field': {
-                                    'name': 'produced_by',
-                                    'type_': 'UNICODE_TEXT'
-                                },
-                                'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'produced_by',
-                                        'type_': 'UNICODE_TEXT'
-                                    }
-                                },
-                                'value': None
-                            }
-                        }
-                    ]
-                },
-                'name': 'product1',
-                'note': None,
-                'paths': {
-                    'edges': [
-                    ]
-                },
-                'postingGitHubUser': {
-                    'login': 'user1'
-                },
-                'productId': '6',
-                'relations': {
-                    'edges': [
-                    ]
-                },
-                'timePosted': '2021-01-04T14:32:20',
-                'timeUpdated': None,
-                'typeId': 1,
-                'type_': {
-                    'name': 'map',
-                    'typeId': '1'
-                },
-                'updatingGitHubUser': None
-            }
+            'productType': {
+                'fields': {'edges': []},
+                'icon': 'mdi-compass',
+                'indefArticle': 'a',
+                'name': 'compass',
+                'order': 5,
+                'plural': 'compasses',
+                'products': {'edges': []},
+                'singular': 'compass',
+                'typeId': '3',
+            },
         }
     }
 }
 
-snapshots['test_schema_success[minimum] 2'] = {
+snapshots['test_schema_success[empty-fields] 2'] = {
     'data': {
-        'allProductFilePaths': {
-            'edges': [
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                }
-            ]
-        },
-        'allProductRelations': {
+        'allProductTypes': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam1'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                            ]
                         },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'icon': 'mdi-spotlight-beam',
+                        'indefArticle': 'a',
+                        'name': 'beam',
+                        'order': 1,
+                        'plural': 'beams',
+                        'products': {'edges': []},
+                        'singular': 'beam',
+                        'typeId': '2',
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                            ]
                         },
-                        'self_': {
-                            'name': 'beam2'
+                        'icon': 'mdi-map',
+                        'indefArticle': 'a',
+                        'name': 'map',
+                        'order': 2,
+                        'plural': 'maps',
+                        'products': {
+                            'edges': [
+                                {'node': {'name': 'map1'}},
+                                {'node': {'name': 'map2'}},
+                                {'node': {'name': 'map3'}},
+                            ]
                         },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                }
-            ]
-        },
-        'allProducts': {
-            'edges': [
-                {
-                    'node': {
-                        'name': 'map1'
+                        'singular': 'map',
+                        'typeId': '1',
                     }
                 },
                 {
                     'node': {
-                        'name': 'map2'
+                        'fields': {'edges': []},
+                        'icon': 'mdi-compass',
+                        'indefArticle': 'a',
+                        'name': 'compass',
+                        'order': 5,
+                        'plural': 'compasses',
+                        'products': {'edges': []},
+                        'singular': 'compass',
+                        'typeId': '3',
                     }
                 },
-                {
-                    'node': {
-                        'name': 'map3'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'product1'
-                    }
-                }
-            ]
+            ],
+            'totalCount': 3,
         }
     }
 }
 
-snapshots['test_schema_success[the-same-name-different-type] 1'] = {
+snapshots['test_schema_success[field-ids-unsorted-duplicate] 1'] = {
     'data': {
-        'createProduct': {
+        'createProductType': {
             'ok': True,
-            'product': {
-                'attributesBoolean': {
-                    'edges': [
-                    ]
-                },
-                'attributesDate': {
-                    'edges': [
-                        {
-                            'node': {
-                                'field': {
-                                    'name': 'date_produced',
-                                    'type_': 'DATE'
-                                },
-                                'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'date_produced',
-                                        'type_': 'DATE'
-                                    }
-                                },
-                                'value': None
-                            }
-                        }
-                    ]
-                },
-                'attributesDateTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesFloat': {
-                    'edges': [
-                    ]
-                },
-                'attributesInteger': {
-                    'edges': [
-                    ]
-                },
-                'attributesTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesUnicodeText': {
+            'productType': {
+                'fields': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'contact',
-                                    'type_': 'UNICODE_TEXT'
-                                },
-                                'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'contact',
-                                        'type_': 'UNICODE_TEXT'
-                                    }
-                                },
-                                'value': 'contact-person'
+                                'field': {'name': 'contact', 'type_': 'UNICODE_TEXT'},
+                                'type_': {'name': 'compass'},
                             }
                         },
                         {
                             'node': {
                                 'field': {
                                     'name': 'produced_by',
-                                    'type_': 'UNICODE_TEXT'
-                                },
-                                'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'produced_by',
-                                        'type_': 'UNICODE_TEXT'
-                                    }
+                                    'type_': 'UNICODE_TEXT',
                                 },
-                                'value': 'pwg-pmn'
-                            }
-                        }
-                    ]
-                },
-                'name': 'map1',
-                'note': None,
-                'paths': {
-                    'edges': [
-                        {
-                            'node': {
-                                'note': None,
-                                'path': '/path/to/new/product1',
-                                'pathId': '9'
+                                'type_': {'name': 'compass'},
                             }
                         },
                         {
                             'node': {
-                                'note': None,
-                                'path': '/another/location/of/product1',
-                                'pathId': '10'
+                                'field': {'name': 'date_produced', 'type_': 'DATE'},
+                                'type_': {'name': 'compass'},
                             }
-                        }
-                    ]
-                },
-                'postingGitHubUser': {
-                    'login': 'user1'
-                },
-                'productId': '6',
-                'relations': {
-                    'edges': [
+                        },
                     ]
                 },
-                'timePosted': '2021-01-04T14:32:20',
-                'timeUpdated': None,
-                'typeId': 2,
-                'type_': {
-                    'name': 'beam',
-                    'typeId': '2'
-                },
-                'updatingGitHubUser': None
-            }
+                'icon': 'mdi-compass',
+                'indefArticle': 'a',
+                'name': 'compass',
+                'order': 5,
+                'plural': 'compasses',
+                'products': {'edges': []},
+                'singular': 'compass',
+                'typeId': '3',
+            },
         }
     }
 }
 
-snapshots['test_schema_success[the-same-name-different-type] 2'] = {
+snapshots['test_schema_success[field-ids-unsorted-duplicate] 2'] = {
     'data': {
-        'allProductFilePaths': {
+        'allProductTypes': {
             'edges': [
                 {
                     'node': {
-                        'path': 'site1:/path/to/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': '/path/to/new/product1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': '/another/location/of/product1'
-                    }
-                }
-            ]
-        },
-        'allProductRelations': {
-            'edges': [
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
-                    }
-                },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam1'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                            ]
                         },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'icon': 'mdi-spotlight-beam',
+                        'indefArticle': 'a',
+                        'name': 'beam',
+                        'order': 1,
+                        'plural': 'beams',
+                        'products': {'edges': []},
+                        'singular': 'beam',
+                        'typeId': '2',
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                            ]
                         },
-                        'self_': {
-                            'name': 'map1'
+                        'icon': 'mdi-map',
+                        'indefArticle': 'a',
+                        'name': 'map',
+                        'order': 2,
+                        'plural': 'maps',
+                        'products': {
+                            'edges': [
+                                {'node': {'name': 'map1'}},
+                                {'node': {'name': 'map2'}},
+                                {'node': {'name': 'map3'}},
+                            ]
                         },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'singular': 'map',
+                        'typeId': '1',
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'compass'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'compass'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'compass'},
+                                    }
+                                },
+                            ]
                         },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'icon': 'mdi-compass',
+                        'indefArticle': 'a',
+                        'name': 'compass',
+                        'order': 5,
+                        'plural': 'compasses',
+                        'products': {'edges': []},
+                        'singular': 'compass',
+                        'typeId': '3',
                     }
                 },
+            ],
+            'totalCount': 3,
+        }
+    }
+}
+
+snapshots['test_schema_success[no-fields] 1'] = {
+    'data': {
+        'createProductType': {
+            'ok': True,
+            'productType': {
+                'fields': {'edges': []},
+                'icon': 'mdi-compass',
+                'indefArticle': 'a',
+                'name': 'compass',
+                'order': 5,
+                'plural': 'compasses',
+                'products': {'edges': []},
+                'singular': 'compass',
+                'typeId': '3',
+            },
+        }
+    }
+}
+
+snapshots['test_schema_success[no-fields] 2'] = {
+    'data': {
+        'allProductTypes': {
+            'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam1'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                            ]
                         },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'icon': 'mdi-spotlight-beam',
+                        'indefArticle': 'a',
+                        'name': 'beam',
+                        'order': 1,
+                        'plural': 'beams',
+                        'products': {'edges': []},
+                        'singular': 'beam',
+                        'typeId': '2',
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                            ]
                         },
-                        'self_': {
-                            'name': 'beam2'
+                        'icon': 'mdi-map',
+                        'indefArticle': 'a',
+                        'name': 'map',
+                        'order': 2,
+                        'plural': 'maps',
+                        'products': {
+                            'edges': [
+                                {'node': {'name': 'map1'}},
+                                {'node': {'name': 'map2'}},
+                                {'node': {'name': 'map3'}},
+                            ]
                         },
-                        'type_': {
-                            'name': 'parent'
-                        }
-                    }
-                }
-            ]
-        },
-        'allProducts': {
-            'edges': [
-                {
-                    'node': {
-                        'name': 'map1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map2'
+                        'singular': 'map',
+                        'typeId': '1',
                     }
                 },
                 {
                     'node': {
-                        'name': 'map3'
+                        'fields': {'edges': []},
+                        'icon': 'mdi-compass',
+                        'indefArticle': 'a',
+                        'name': 'compass',
+                        'order': 5,
+                        'plural': 'compasses',
+                        'products': {'edges': []},
+                        'singular': 'compass',
+                        'typeId': '3',
                     }
                 },
-                {
-                    'node': {
-                        'name': 'beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map1'
-                    }
-                }
-            ]
+            ],
+            'totalCount': 3,
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product/snapshots/snap_test_update_product.py` & `acondbs-0.4.4/tests/schema/product/mutation/product/snapshots/snap_test_update_product.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,2054 +1,1195 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_schema_error[error-constraint] 1'] = {
     'data': {
         'allProductFilePaths': {
             'edges': [
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                }
+                {'node': {'path': 'site1:/path/to/map1'}},
+                {'node': {'path': 'site2:/another/way/map1'}},
+                {'node': {'path': 'site1:/path/to/map2'}},
+                {'node': {'path': 'site1:/path/to/map3'}},
+                {'node': {'path': 'site2:/another/way/map3'}},
+                {'node': {'path': 'site1:/path/to/beam1'}},
+                {'node': {'path': 'site2:/another/way/beam1'}},
+                {'node': {'path': 'site1:/path/to/beam2'}},
             ]
         },
         'allProductRelations': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'map1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'map1'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'map1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'map1'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
-                }
+                },
             ]
         },
         'allProducts': {
             'edges': [
-                {
-                    'node': {
-                        'name': 'map1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map3'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                }
+                {'node': {'name': 'map1'}},
+                {'node': {'name': 'map2'}},
+                {'node': {'name': 'map3'}},
+                {'node': {'name': 'beam1'}},
+                {'node': {'name': 'beam2'}},
             ]
-        }
+        },
     }
 }
 
 snapshots['test_schema_success[delete-paths] 1'] = {
     'data': {
         'updateProduct': {
             'ok': True,
             'product': {
-                'attributesBoolean': {
-                    'edges': [
-                    ]
-                },
+                'attributesBoolean': {'edges': []},
                 'attributesDate': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'date_produced',
-                                    'type_': 'DATE'
-                                },
+                                'field': {'name': 'date_produced', 'type_': 'DATE'},
                                 'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'date_produced',
-                                        'type_': 'DATE'
-                                    }
+                                    'field': {'name': 'date_produced', 'type_': 'DATE'}
                                 },
-                                'value': '2020-02-01'
+                                'value': '2020-02-01',
                             }
                         }
                     ]
                 },
-                'attributesDateTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesFloat': {
-                    'edges': [
-                    ]
-                },
-                'attributesInteger': {
-                    'edges': [
-                    ]
-                },
-                'attributesTime': {
-                    'edges': [
-                    ]
-                },
+                'attributesDateTime': {'edges': []},
+                'attributesFloat': {'edges': []},
+                'attributesInteger': {'edges': []},
+                'attributesTime': {'edges': []},
                 'attributesUnicodeText': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'contact',
-                                    'type_': 'UNICODE_TEXT'
-                                },
+                                'field': {'name': 'contact', 'type_': 'UNICODE_TEXT'},
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'contact',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
                         },
                         {
                             'node': {
                                 'field': {
                                     'name': 'produced_by',
-                                    'type_': 'UNICODE_TEXT'
+                                    'type_': 'UNICODE_TEXT',
                                 },
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'produced_by',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
-                        }
+                        },
                     ]
                 },
                 'name': 'map1',
                 'note': None,
-                'paths': {
-                    'edges': [
-                    ]
-                },
+                'paths': {'edges': []},
                 'postingGitHubUser': None,
                 'productId': '1',
                 'relations': {
                     'edges': [
                         {
                             'node': {
                                 'other': {
                                     'name': 'beam1',
                                     'productId': '4',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'beam', 'typeId': '2'},
                                 },
                                 'otherProductId': 4,
                                 'relationId': '1',
                                 'reverse': {
                                     'relationId': '2',
                                     'typeId': 1,
-                                    'type_': {
-                                        'name': 'parent',
-                                        'typeId': '1'
-                                    }
+                                    'type_': {'name': 'parent', 'typeId': '1'},
                                 },
                                 'reverseRelationId': 2,
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'child',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'child', 'typeId': '2'},
                             }
                         },
                         {
                             'node': {
                                 'other': {
                                     'name': 'beam2',
                                     'productId': '5',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'beam', 'typeId': '2'},
                                 },
                                 'otherProductId': 5,
                                 'relationId': '3',
                                 'reverse': {
                                     'relationId': '4',
                                     'typeId': 1,
-                                    'type_': {
-                                        'name': 'parent',
-                                        'typeId': '1'
-                                    }
+                                    'type_': {'name': 'parent', 'typeId': '1'},
                                 },
                                 'reverseRelationId': 4,
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'child',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'child', 'typeId': '2'},
                             }
-                        }
+                        },
                     ]
                 },
                 'timePosted': '2021-01-04T14:32:20',
                 'timeUpdated': '2021-01-04T14:32:20',
                 'typeId': 1,
-                'type_': {
-                    'name': 'map',
-                    'typeId': '1'
-                },
-                'updatingGitHubUser': {
-                    'login': 'user1'
-                }
-            }
+                'type_': {'name': 'map', 'typeId': '1'},
+                'updatingGitHubUser': {'login': 'user1'},
+            },
         }
     }
 }
 
 snapshots['test_schema_success[delete-paths] 2'] = {
     'data': {
         'allProductFilePaths': {
             'edges': [
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                }
+                {'node': {'path': 'site1:/path/to/map2'}},
+                {'node': {'path': 'site1:/path/to/map3'}},
+                {'node': {'path': 'site2:/another/way/map3'}},
+                {'node': {'path': 'site1:/path/to/beam1'}},
+                {'node': {'path': 'site2:/another/way/beam1'}},
+                {'node': {'path': 'site1:/path/to/beam2'}},
             ]
         },
         'allProductRelations': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'map1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'map1'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'map1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'map1'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
-                }
+                },
             ]
         },
         'allProducts': {
             'edges': [
-                {
-                    'node': {
-                        'name': 'map1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map3'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                }
+                {'node': {'name': 'map1'}},
+                {'node': {'name': 'map2'}},
+                {'node': {'name': 'map3'}},
+                {'node': {'name': 'beam1'}},
+                {'node': {'name': 'beam2'}},
             ]
-        }
+        },
     }
 }
 
 snapshots['test_schema_success[delete-relations] 1'] = {
     'data': {
         'updateProduct': {
             'ok': True,
             'product': {
-                'attributesBoolean': {
-                    'edges': [
-                    ]
-                },
+                'attributesBoolean': {'edges': []},
                 'attributesDate': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'date_produced',
-                                    'type_': 'DATE'
-                                },
+                                'field': {'name': 'date_produced', 'type_': 'DATE'},
                                 'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'date_produced',
-                                        'type_': 'DATE'
-                                    }
+                                    'field': {'name': 'date_produced', 'type_': 'DATE'}
                                 },
-                                'value': '2020-03-04'
+                                'value': '2020-03-04',
                             }
                         }
                     ]
                 },
-                'attributesDateTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesFloat': {
-                    'edges': [
-                    ]
-                },
-                'attributesInteger': {
-                    'edges': [
-                    ]
-                },
-                'attributesTime': {
-                    'edges': [
-                    ]
-                },
+                'attributesDateTime': {'edges': []},
+                'attributesFloat': {'edges': []},
+                'attributesInteger': {'edges': []},
+                'attributesTime': {'edges': []},
                 'attributesUnicodeText': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'contact',
-                                    'type_': 'UNICODE_TEXT'
-                                },
+                                'field': {'name': 'contact', 'type_': 'UNICODE_TEXT'},
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'contact',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
                         },
                         {
                             'node': {
                                 'field': {
                                     'name': 'produced_by',
-                                    'type_': 'UNICODE_TEXT'
+                                    'type_': 'UNICODE_TEXT',
                                 },
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'produced_by',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
-                        }
+                        },
                     ]
                 },
                 'name': 'beam2',
                 'note': None,
                 'paths': {
                     'edges': [
                         {
                             'node': {
                                 'note': None,
                                 'path': 'site1:/path/to/beam2',
-                                'pathId': '8'
+                                'pathId': '8',
                             }
                         }
                     ]
                 },
                 'postingGitHubUser': None,
                 'productId': '5',
-                'relations': {
-                    'edges': [
-                    ]
-                },
+                'relations': {'edges': []},
                 'timePosted': '2021-01-04T14:32:20',
                 'timeUpdated': '2021-01-04T14:32:20',
                 'typeId': 2,
-                'type_': {
-                    'name': 'beam',
-                    'typeId': '2'
-                },
-                'updatingGitHubUser': {
-                    'login': 'user1'
-                }
-            }
+                'type_': {'name': 'beam', 'typeId': '2'},
+                'updatingGitHubUser': {'login': 'user1'},
+            },
         }
     }
 }
 
 snapshots['test_schema_success[delete-relations] 2'] = {
     'data': {
         'allProductFilePaths': {
             'edges': [
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                }
+                {'node': {'path': 'site1:/path/to/map1'}},
+                {'node': {'path': 'site2:/another/way/map1'}},
+                {'node': {'path': 'site1:/path/to/map2'}},
+                {'node': {'path': 'site1:/path/to/map3'}},
+                {'node': {'path': 'site2:/another/way/map3'}},
+                {'node': {'path': 'site1:/path/to/beam1'}},
+                {'node': {'path': 'site2:/another/way/beam1'}},
+                {'node': {'path': 'site1:/path/to/beam2'}},
             ]
         },
         'allProductRelations': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'map1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'map1'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'parent'},
                     }
-                }
+                },
             ]
         },
         'allProducts': {
             'edges': [
-                {
-                    'node': {
-                        'name': 'map1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map3'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                }
+                {'node': {'name': 'map1'}},
+                {'node': {'name': 'map2'}},
+                {'node': {'name': 'map3'}},
+                {'node': {'name': 'beam1'}},
+                {'node': {'name': 'beam2'}},
             ]
-        }
+        },
     }
 }
 
 snapshots['test_schema_success[update-name] 1'] = {
     'data': {
         'updateProduct': {
             'ok': True,
             'product': {
-                'attributesBoolean': {
-                    'edges': [
-                    ]
-                },
+                'attributesBoolean': {'edges': []},
                 'attributesDate': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'date_produced',
-                                    'type_': 'DATE'
-                                },
+                                'field': {'name': 'date_produced', 'type_': 'DATE'},
                                 'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'date_produced',
-                                        'type_': 'DATE'
-                                    }
+                                    'field': {'name': 'date_produced', 'type_': 'DATE'}
                                 },
-                                'value': '2020-02-01'
+                                'value': '2020-02-01',
                             }
                         }
                     ]
                 },
-                'attributesDateTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesFloat': {
-                    'edges': [
-                    ]
-                },
-                'attributesInteger': {
-                    'edges': [
-                    ]
-                },
-                'attributesTime': {
-                    'edges': [
-                    ]
-                },
+                'attributesDateTime': {'edges': []},
+                'attributesFloat': {'edges': []},
+                'attributesInteger': {'edges': []},
+                'attributesTime': {'edges': []},
                 'attributesUnicodeText': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'contact',
-                                    'type_': 'UNICODE_TEXT'
-                                },
+                                'field': {'name': 'contact', 'type_': 'UNICODE_TEXT'},
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'contact',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
                         },
                         {
                             'node': {
                                 'field': {
                                     'name': 'produced_by',
-                                    'type_': 'UNICODE_TEXT'
+                                    'type_': 'UNICODE_TEXT',
                                 },
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'produced_by',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
-                        }
+                        },
                     ]
                 },
                 'name': 'new-name',
                 'note': None,
                 'paths': {
                     'edges': [
                         {
                             'node': {
                                 'note': None,
                                 'path': 'site1:/path/to/map1',
-                                'pathId': '1'
+                                'pathId': '1',
                             }
                         },
                         {
                             'node': {
                                 'note': None,
                                 'path': 'site2:/another/way/map1',
-                                'pathId': '2'
+                                'pathId': '2',
                             }
-                        }
+                        },
                     ]
                 },
                 'postingGitHubUser': None,
                 'productId': '1',
                 'relations': {
                     'edges': [
                         {
                             'node': {
                                 'other': {
                                     'name': 'beam1',
                                     'productId': '4',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'beam', 'typeId': '2'},
                                 },
                                 'otherProductId': 4,
                                 'relationId': '1',
                                 'reverse': {
                                     'relationId': '2',
                                     'typeId': 1,
-                                    'type_': {
-                                        'name': 'parent',
-                                        'typeId': '1'
-                                    }
+                                    'type_': {'name': 'parent', 'typeId': '1'},
                                 },
                                 'reverseRelationId': 2,
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'child',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'child', 'typeId': '2'},
                             }
                         },
                         {
                             'node': {
                                 'other': {
                                     'name': 'beam2',
                                     'productId': '5',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'beam', 'typeId': '2'},
                                 },
                                 'otherProductId': 5,
                                 'relationId': '3',
                                 'reverse': {
                                     'relationId': '4',
                                     'typeId': 1,
-                                    'type_': {
-                                        'name': 'parent',
-                                        'typeId': '1'
-                                    }
+                                    'type_': {'name': 'parent', 'typeId': '1'},
                                 },
                                 'reverseRelationId': 4,
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'child',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'child', 'typeId': '2'},
                             }
-                        }
+                        },
                     ]
                 },
                 'timePosted': '2021-01-04T14:32:20',
                 'timeUpdated': '2021-01-04T14:32:20',
                 'typeId': 1,
-                'type_': {
-                    'name': 'map',
-                    'typeId': '1'
-                },
-                'updatingGitHubUser': {
-                    'login': 'user1'
-                }
-            }
+                'type_': {'name': 'map', 'typeId': '1'},
+                'updatingGitHubUser': {'login': 'user1'},
+            },
         }
     }
 }
 
 snapshots['test_schema_success[update-name] 2'] = {
     'data': {
         'allProductFilePaths': {
             'edges': [
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                }
+                {'node': {'path': 'site1:/path/to/map1'}},
+                {'node': {'path': 'site2:/another/way/map1'}},
+                {'node': {'path': 'site1:/path/to/map2'}},
+                {'node': {'path': 'site1:/path/to/map3'}},
+                {'node': {'path': 'site2:/another/way/map3'}},
+                {'node': {'path': 'site1:/path/to/beam1'}},
+                {'node': {'path': 'site2:/another/way/beam1'}},
+                {'node': {'path': 'site1:/path/to/beam2'}},
             ]
         },
         'allProductRelations': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'new-name'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'new-name'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'new-name'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'new-name'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'new-name'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'new-name'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'new-name'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'new-name'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
-                }
+                },
             ]
         },
         'allProducts': {
             'edges': [
-                {
-                    'node': {
-                        'name': 'new-name'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map3'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                }
+                {'node': {'name': 'new-name'}},
+                {'node': {'name': 'map2'}},
+                {'node': {'name': 'map3'}},
+                {'node': {'name': 'beam1'}},
+                {'node': {'name': 'beam2'}},
             ]
-        }
+        },
     }
 }
 
 snapshots['test_schema_success[update-paths] 1'] = {
     'data': {
         'updateProduct': {
             'ok': True,
             'product': {
-                'attributesBoolean': {
-                    'edges': [
-                    ]
-                },
+                'attributesBoolean': {'edges': []},
                 'attributesDate': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'date_produced',
-                                    'type_': 'DATE'
-                                },
+                                'field': {'name': 'date_produced', 'type_': 'DATE'},
                                 'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'date_produced',
-                                        'type_': 'DATE'
-                                    }
+                                    'field': {'name': 'date_produced', 'type_': 'DATE'}
                                 },
-                                'value': '2020-02-01'
+                                'value': '2020-02-01',
                             }
                         }
                     ]
                 },
-                'attributesDateTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesFloat': {
-                    'edges': [
-                    ]
-                },
-                'attributesInteger': {
-                    'edges': [
-                    ]
-                },
-                'attributesTime': {
-                    'edges': [
-                    ]
-                },
+                'attributesDateTime': {'edges': []},
+                'attributesFloat': {'edges': []},
+                'attributesInteger': {'edges': []},
+                'attributesTime': {'edges': []},
                 'attributesUnicodeText': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'contact',
-                                    'type_': 'UNICODE_TEXT'
-                                },
+                                'field': {'name': 'contact', 'type_': 'UNICODE_TEXT'},
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'contact',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
                         },
                         {
                             'node': {
                                 'field': {
                                     'name': 'produced_by',
-                                    'type_': 'UNICODE_TEXT'
+                                    'type_': 'UNICODE_TEXT',
                                 },
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'produced_by',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
-                        }
+                        },
                     ]
                 },
                 'name': 'map1',
                 'note': None,
                 'paths': {
                     'edges': [
                         {
                             'node': {
                                 'note': None,
                                 'path': 'site1:/path/to/map1',
-                                'pathId': '1'
+                                'pathId': '1',
                             }
                         },
                         {
                             'node': {
                                 'note': None,
                                 'path': 'site2:/updated/way/map1',
-                                'pathId': '9'
+                                'pathId': '9',
                             }
                         },
                         {
                             'node': {
                                 'note': None,
                                 'path': 'site4:/additional/map1',
-                                'pathId': '10'
+                                'pathId': '10',
                             }
-                        }
+                        },
                     ]
                 },
                 'postingGitHubUser': None,
                 'productId': '1',
                 'relations': {
                     'edges': [
                         {
                             'node': {
                                 'other': {
                                     'name': 'beam1',
                                     'productId': '4',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'beam', 'typeId': '2'},
                                 },
                                 'otherProductId': 4,
                                 'relationId': '1',
                                 'reverse': {
                                     'relationId': '2',
                                     'typeId': 1,
-                                    'type_': {
-                                        'name': 'parent',
-                                        'typeId': '1'
-                                    }
+                                    'type_': {'name': 'parent', 'typeId': '1'},
                                 },
                                 'reverseRelationId': 2,
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'child',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'child', 'typeId': '2'},
                             }
                         },
                         {
                             'node': {
                                 'other': {
                                     'name': 'beam2',
                                     'productId': '5',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'beam', 'typeId': '2'},
                                 },
                                 'otherProductId': 5,
                                 'relationId': '3',
                                 'reverse': {
                                     'relationId': '4',
                                     'typeId': 1,
-                                    'type_': {
-                                        'name': 'parent',
-                                        'typeId': '1'
-                                    }
+                                    'type_': {'name': 'parent', 'typeId': '1'},
                                 },
                                 'reverseRelationId': 4,
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'child',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'child', 'typeId': '2'},
                             }
-                        }
+                        },
                     ]
                 },
                 'timePosted': '2021-01-04T14:32:20',
                 'timeUpdated': '2021-01-04T14:32:20',
                 'typeId': 1,
-                'type_': {
-                    'name': 'map',
-                    'typeId': '1'
-                },
-                'updatingGitHubUser': {
-                    'login': 'user1'
-                }
-            }
+                'type_': {'name': 'map', 'typeId': '1'},
+                'updatingGitHubUser': {'login': 'user1'},
+            },
         }
     }
 }
 
 snapshots['test_schema_success[update-paths] 2'] = {
     'data': {
         'allProductFilePaths': {
             'edges': [
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/updated/way/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site4:/additional/map1'
-                    }
-                }
+                {'node': {'path': 'site1:/path/to/map1'}},
+                {'node': {'path': 'site1:/path/to/map2'}},
+                {'node': {'path': 'site1:/path/to/map3'}},
+                {'node': {'path': 'site2:/another/way/map3'}},
+                {'node': {'path': 'site1:/path/to/beam1'}},
+                {'node': {'path': 'site2:/another/way/beam1'}},
+                {'node': {'path': 'site1:/path/to/beam2'}},
+                {'node': {'path': 'site2:/updated/way/map1'}},
+                {'node': {'path': 'site4:/additional/map1'}},
             ]
         },
         'allProductRelations': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'map1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'map1'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'map1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'map1'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
-                }
+                },
             ]
         },
         'allProducts': {
             'edges': [
-                {
-                    'node': {
-                        'name': 'map1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map3'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                }
+                {'node': {'name': 'map1'}},
+                {'node': {'name': 'map2'}},
+                {'node': {'name': 'map3'}},
+                {'node': {'name': 'beam1'}},
+                {'node': {'name': 'beam2'}},
             ]
-        }
+        },
     }
 }
 
 snapshots['test_schema_success[update-relations] 1'] = {
     'data': {
         'updateProduct': {
             'ok': True,
             'product': {
-                'attributesBoolean': {
-                    'edges': [
-                    ]
-                },
+                'attributesBoolean': {'edges': []},
                 'attributesDate': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'date_produced',
-                                    'type_': 'DATE'
-                                },
+                                'field': {'name': 'date_produced', 'type_': 'DATE'},
                                 'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'date_produced',
-                                        'type_': 'DATE'
-                                    }
+                                    'field': {'name': 'date_produced', 'type_': 'DATE'}
                                 },
-                                'value': '2020-03-04'
+                                'value': '2020-03-04',
                             }
                         }
                     ]
                 },
-                'attributesDateTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesFloat': {
-                    'edges': [
-                    ]
-                },
-                'attributesInteger': {
-                    'edges': [
-                    ]
-                },
-                'attributesTime': {
-                    'edges': [
-                    ]
-                },
+                'attributesDateTime': {'edges': []},
+                'attributesFloat': {'edges': []},
+                'attributesInteger': {'edges': []},
+                'attributesTime': {'edges': []},
                 'attributesUnicodeText': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'contact',
-                                    'type_': 'UNICODE_TEXT'
-                                },
+                                'field': {'name': 'contact', 'type_': 'UNICODE_TEXT'},
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'contact',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
                         },
                         {
                             'node': {
                                 'field': {
                                     'name': 'produced_by',
-                                    'type_': 'UNICODE_TEXT'
+                                    'type_': 'UNICODE_TEXT',
                                 },
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'produced_by',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
-                        }
+                        },
                     ]
                 },
                 'name': 'beam2',
                 'note': None,
                 'paths': {
                     'edges': [
                         {
                             'node': {
                                 'note': None,
                                 'path': 'site1:/path/to/beam2',
-                                'pathId': '8'
+                                'pathId': '8',
                             }
                         }
                     ]
                 },
                 'postingGitHubUser': None,
                 'productId': '5',
                 'relations': {
                     'edges': [
                         {
                             'node': {
                                 'other': {
                                     'name': 'beam1',
                                     'productId': '4',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'beam', 'typeId': '2'},
                                 },
                                 'otherProductId': 4,
                                 'relationId': '6',
                                 'reverse': {
                                     'relationId': '5',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'child',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'child', 'typeId': '2'},
                                 },
                                 'reverseRelationId': 5,
                                 'typeId': 1,
-                                'type_': {
-                                    'name': 'parent',
-                                    'typeId': '1'
-                                }
+                                'type_': {'name': 'parent', 'typeId': '1'},
                             }
                         },
                         {
                             'node': {
                                 'other': {
                                     'name': 'map2',
                                     'productId': '2',
                                     'typeId': 1,
-                                    'type_': {
-                                        'name': 'map',
-                                        'typeId': '1'
-                                    }
+                                    'type_': {'name': 'map', 'typeId': '1'},
                                 },
                                 'otherProductId': 2,
                                 'relationId': '8',
                                 'reverse': {
                                     'relationId': '7',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'child',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'child', 'typeId': '2'},
                                 },
                                 'reverseRelationId': 7,
                                 'typeId': 1,
-                                'type_': {
-                                    'name': 'parent',
-                                    'typeId': '1'
-                                }
+                                'type_': {'name': 'parent', 'typeId': '1'},
                             }
-                        }
+                        },
                     ]
                 },
                 'timePosted': '2021-01-04T14:32:20',
                 'timeUpdated': '2021-01-04T14:32:20',
                 'typeId': 2,
-                'type_': {
-                    'name': 'beam',
-                    'typeId': '2'
-                },
-                'updatingGitHubUser': {
-                    'login': 'user1'
-                }
-            }
+                'type_': {'name': 'beam', 'typeId': '2'},
+                'updatingGitHubUser': {'login': 'user1'},
+            },
         }
     }
 }
 
 snapshots['test_schema_success[update-relations] 2'] = {
     'data': {
         'allProductFilePaths': {
             'edges': [
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                }
+                {'node': {'path': 'site1:/path/to/map1'}},
+                {'node': {'path': 'site2:/another/way/map1'}},
+                {'node': {'path': 'site1:/path/to/map2'}},
+                {'node': {'path': 'site1:/path/to/map3'}},
+                {'node': {'path': 'site2:/another/way/map3'}},
+                {'node': {'path': 'site1:/path/to/beam1'}},
+                {'node': {'path': 'site2:/another/way/beam1'}},
+                {'node': {'path': 'site1:/path/to/beam2'}},
             ]
         },
         'allProductRelations': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'map1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'map1'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'map2'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'map2'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map2'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'map2'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
-                }
+                },
             ]
         },
         'allProducts': {
             'edges': [
-                {
-                    'node': {
-                        'name': 'map1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map3'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                }
+                {'node': {'name': 'map1'}},
+                {'node': {'name': 'map2'}},
+                {'node': {'name': 'map3'}},
+                {'node': {'name': 'beam1'}},
+                {'node': {'name': 'beam2'}},
             ]
-        }
+        },
     }
 }
 
 snapshots['test_schema_success[update] 1'] = {
     'data': {
         'updateProduct': {
             'ok': True,
             'product': {
-                'attributesBoolean': {
-                    'edges': [
-                    ]
-                },
+                'attributesBoolean': {'edges': []},
                 'attributesDate': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'date_produced',
-                                    'type_': 'DATE'
-                                },
+                                'field': {'name': 'date_produced', 'type_': 'DATE'},
                                 'typeFieldAssociation': {
-                                    'field': {
-                                        'name': 'date_produced',
-                                        'type_': 'DATE'
-                                    }
+                                    'field': {'name': 'date_produced', 'type_': 'DATE'}
                                 },
-                                'value': '2020-02-01'
+                                'value': '2020-02-01',
                             }
                         }
                     ]
                 },
-                'attributesDateTime': {
-                    'edges': [
-                    ]
-                },
-                'attributesFloat': {
-                    'edges': [
-                    ]
-                },
-                'attributesInteger': {
-                    'edges': [
-                    ]
-                },
-                'attributesTime': {
-                    'edges': [
-                    ]
-                },
+                'attributesDateTime': {'edges': []},
+                'attributesFloat': {'edges': []},
+                'attributesInteger': {'edges': []},
+                'attributesTime': {'edges': []},
                 'attributesUnicodeText': {
                     'edges': [
                         {
                             'node': {
-                                'field': {
-                                    'name': 'contact',
-                                    'type_': 'UNICODE_TEXT'
-                                },
+                                'field': {'name': 'contact', 'type_': 'UNICODE_TEXT'},
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'contact',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': 'new-contact'
+                                'value': 'new-contact',
                             }
                         },
                         {
                             'node': {
                                 'field': {
                                     'name': 'produced_by',
-                                    'type_': 'UNICODE_TEXT'
+                                    'type_': 'UNICODE_TEXT',
                                 },
                                 'typeFieldAssociation': {
                                     'field': {
                                         'name': 'produced_by',
-                                        'type_': 'UNICODE_TEXT'
+                                        'type_': 'UNICODE_TEXT',
                                     }
                                 },
-                                'value': None
+                                'value': None,
                             }
-                        }
+                        },
                     ]
                 },
                 'name': 'map1',
                 'note': '- updated note 123',
                 'paths': {
                     'edges': [
                         {
                             'node': {
                                 'note': None,
                                 'path': 'site1:/path/to/map1',
-                                'pathId': '1'
+                                'pathId': '1',
                             }
                         },
                         {
                             'node': {
                                 'note': None,
                                 'path': 'site2:/another/way/map1',
-                                'pathId': '2'
+                                'pathId': '2',
                             }
-                        }
+                        },
                     ]
                 },
                 'postingGitHubUser': None,
                 'productId': '1',
                 'relations': {
                     'edges': [
                         {
                             'node': {
                                 'other': {
                                     'name': 'beam1',
                                     'productId': '4',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'beam', 'typeId': '2'},
                                 },
                                 'otherProductId': 4,
                                 'relationId': '1',
                                 'reverse': {
                                     'relationId': '2',
                                     'typeId': 1,
-                                    'type_': {
-                                        'name': 'parent',
-                                        'typeId': '1'
-                                    }
+                                    'type_': {'name': 'parent', 'typeId': '1'},
                                 },
                                 'reverseRelationId': 2,
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'child',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'child', 'typeId': '2'},
                             }
                         },
                         {
                             'node': {
                                 'other': {
                                     'name': 'beam2',
                                     'productId': '5',
                                     'typeId': 2,
-                                    'type_': {
-                                        'name': 'beam',
-                                        'typeId': '2'
-                                    }
+                                    'type_': {'name': 'beam', 'typeId': '2'},
                                 },
                                 'otherProductId': 5,
                                 'relationId': '3',
                                 'reverse': {
                                     'relationId': '4',
                                     'typeId': 1,
-                                    'type_': {
-                                        'name': 'parent',
-                                        'typeId': '1'
-                                    }
+                                    'type_': {'name': 'parent', 'typeId': '1'},
                                 },
                                 'reverseRelationId': 4,
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'child',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'child', 'typeId': '2'},
                             }
-                        }
+                        },
                     ]
                 },
                 'timePosted': '2021-01-04T14:32:20',
                 'timeUpdated': '2021-01-04T14:32:20',
                 'typeId': 1,
-                'type_': {
-                    'name': 'map',
-                    'typeId': '1'
-                },
-                'updatingGitHubUser': {
-                    'login': 'user1'
-                }
-            }
+                'type_': {'name': 'map', 'typeId': '1'},
+                'updatingGitHubUser': {'login': 'user1'},
+            },
         }
     }
 }
 
 snapshots['test_schema_success[update] 2'] = {
     'data': {
         'allProductFilePaths': {
             'edges': [
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map2'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/map3'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site2:/another/way/beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'path': 'site1:/path/to/beam2'
-                    }
-                }
+                {'node': {'path': 'site1:/path/to/map1'}},
+                {'node': {'path': 'site2:/another/way/map1'}},
+                {'node': {'path': 'site1:/path/to/map2'}},
+                {'node': {'path': 'site1:/path/to/map3'}},
+                {'node': {'path': 'site2:/another/way/map3'}},
+                {'node': {'path': 'site1:/path/to/beam1'}},
+                {'node': {'path': 'site2:/another/way/beam1'}},
+                {'node': {'path': 'site1:/path/to/beam2'}},
             ]
         },
         'allProductRelations': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'map1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'map1'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'map1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'map1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'map1'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2'
-                        },
-                        'self_': {
-                            'name': 'beam1'
-                        },
-                        'type_': {
-                            'name': 'child'
-                        }
+                        'other': {'name': 'beam2'},
+                        'self_': {'name': 'beam1'},
+                        'type_': {'name': 'child'},
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1'
-                        },
-                        'self_': {
-                            'name': 'beam2'
-                        },
-                        'type_': {
-                            'name': 'parent'
-                        }
+                        'other': {'name': 'beam1'},
+                        'self_': {'name': 'beam2'},
+                        'type_': {'name': 'parent'},
                     }
-                }
+                },
             ]
         },
         'allProducts': {
             'edges': [
-                {
-                    'node': {
-                        'name': 'map1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map2'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'map3'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam1'
-                    }
-                },
-                {
-                    'node': {
-                        'name': 'beam2'
-                    }
-                }
+                {'node': {'name': 'map1'}},
+                {'node': {'name': 'map2'}},
+                {'node': {'name': 'map3'}},
+                {'node': {'name': 'beam1'}},
+                {'node': {'name': 'beam2'}},
             ]
-        }
+        },
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product/test_convert_product_type.py` & `acondbs-0.4.4/tests/schema/product/mutation/product/test_convert_product_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import pytest
 
 from ....funcs import assert_mutation
-
 from ...gql import MUTATION_CONVERT_PRODUCT_TYPE, QUERY_ALL_PRODUCTS
 
 HEADERS = {
     "Authorization": "Bearer 39d86487d76a84087f1da599c872dac4473e5f07",  # user1
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_CONVERT_PRODUCT_TYPE,
             "variables": {
                 "productId": 1,
                 "typeId": 2,
@@ -37,10 +35,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product/test_create_product.py` & `acondbs-0.4.4/tests/schema/product/mutation/product/test_create_product.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
 from ....funcs import assert_mutation
-
 from ...gql import MUTATION_CREATE_PRODUCT
 
 QEURY = """
 {
   allProducts {
     edges {
       node {
@@ -37,15 +36,14 @@
   }
 }
 """
 
 HEADERS = {"Authorization": "Bearer 39d86487d76a84087f1da599c872dac4473e5f07"}  # user1
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_CREATE_PRODUCT,
             "variables": {
                 "input": {
                     "typeId": 2,
@@ -128,15 +126,14 @@
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_CREATE_PRODUCT,
             "variables": {
                 "input": {
                     "typeId": 1,
@@ -174,10 +171,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product/test_delete_product.py` & `acondbs-0.4.4/tests/schema/product/mutation/product/test_delete_product.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
 from ....funcs import assert_mutation
-
 from ...gql import MUTATION_DELETE_PRODUCT
 
 QEURY = """
 {
   allProducts {
     edges {
       node {
@@ -38,15 +37,14 @@
 }
 """
 
 
 HEADERS = {"Authorization": "Bearer 39d86487d76a84087f1da599c872dac4473e5f07"}  # user1
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": MUTATION_DELETE_PRODUCT, "variables": {"productId": 1}},
         {"query": QEURY},
         id="delete",
     ),
 ]
@@ -66,15 +64,14 @@
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": MUTATION_DELETE_PRODUCT, "variables": {"productId": 512}},
         {"query": QEURY},
         id="error",
     ),
 ]
@@ -92,10 +89,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product/test_update_product.py` & `acondbs-0.4.4/tests/schema/product/mutation/product/test_update_product.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
 from ....funcs import assert_mutation
-
 from ...gql import MUTATION_UPDATE_PRODUCT
 
 QEURY = """
 {
   allProducts {
     edges {
       node {
@@ -39,15 +38,14 @@
 """
 
 HEADERS = {
     "Authorization": "Bearer 39d86487d76a84087f1da599c872dac4473e5f07",  # user1
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_UPDATE_PRODUCT,
             "variables": {
                 "productId": 1,
                 "input": {
@@ -152,15 +150,14 @@
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_UPDATE_PRODUCT,
             "variables": {
                 "productId": 1,
                 "input": {
@@ -186,10 +183,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_file_path/snapshots/snap_test_create_product_file_path.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_relation/snapshots/snap_test_delete_product_relation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,83 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_error[createProductFilePath-noSuchField] 1'] = {
+snapshots['test_schema_success[create] 1'] = {
+    'data': {'deleteProductRelation': {'ok': True}}
+}
+
+snapshots['test_schema_success[create] 2'] = {
     'data': {
-        'allProductFilePaths': {
+        'allProductRelations': {
             'edges': [
                 {
                     'node': {
-                        'productId': 1001
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1012
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1012
+                        'other': {'name': 'beam2', 'productId': '5'},
+                        'relationId': '3',
+                        'reverse': {'relationId': '4'},
+                        'self_': {'name': 'beam1', 'productId': '4'},
+                        'type_': {'name': 'child', 'typeId': '2'},
                     }
                 },
                 {
                     'node': {
-                        'productId': 1013
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1070
+                        'other': {'name': 'beam1', 'productId': '4'},
+                        'relationId': '4',
+                        'reverse': {'relationId': '3'},
+                        'self_': {'name': 'beam2', 'productId': '5'},
+                        'type_': {'name': 'parent', 'typeId': '1'},
                     }
                 },
+            ]
+        }
+    }
+}
+
+snapshots['test_schema_error[error-nonexistent] 1'] = {
+    'data': {
+        'allProductRelations': {
+            'edges': [
                 {
                     'node': {
-                        'productId': 1120
+                        'other': {'name': 'beam1', 'productId': '4'},
+                        'relationId': '1',
+                        'reverse': {'relationId': '2'},
+                        'self_': {'name': 'map1', 'productId': '1'},
+                        'type_': {'name': 'child', 'typeId': '2'},
                     }
                 },
                 {
                     'node': {
-                        'productId': 1130
+                        'other': {'name': 'map1', 'productId': '1'},
+                        'relationId': '2',
+                        'reverse': {'relationId': '1'},
+                        'self_': {'name': 'beam1', 'productId': '4'},
+                        'type_': {'name': 'parent', 'typeId': '1'},
                     }
                 },
                 {
                     'node': {
-                        'productId': 1150
+                        'other': {'name': 'beam2', 'productId': '5'},
+                        'relationId': '3',
+                        'reverse': {'relationId': '4'},
+                        'self_': {'name': 'beam1', 'productId': '4'},
+                        'type_': {'name': 'child', 'typeId': '2'},
                     }
                 },
                 {
                     'node': {
-                        'productId': 1002
+                        'other': {'name': 'beam1', 'productId': '4'},
+                        'relationId': '4',
+                        'reverse': {'relationId': '3'},
+                        'self_': {'name': 'beam2', 'productId': '5'},
+                        'type_': {'name': 'parent', 'typeId': '1'},
                     }
                 },
-                {
-                    'node': {
-                        'productId': 1002
-                    }
-                }
             ]
         }
     }
 }
-
-snapshots['test_schema_success[createProductFilePath] 1'] = {
-    'data': {
-        'createProductFilePath': {
-            'productFilePath': {
-                'path': 'nersc:/go/to/my/new_product_v1'
-            }
-        }
-    }
-}
-
-snapshots['test_schema_success[createProductFilePath] 2'] = {
-    'data': {
-        'product': {
-            'name': '20180101',
-            'note': '- test entry',
-            'paths': {
-                'edges': [
-                    {
-                        'node': {
-                            'note': '- Note 1',
-                            'path': 'nersc:/go/to/my/new_product_v1',
-                            'product': {
-                                'productId': '1010'
-                            }
-                        }
-                    }
-                ]
-            },
-            'timePosted': '2018-01-01T15:32:10'
-        }
-    }
-}
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_file_path/snapshots/snap_test_delete_product_file_path.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_file_path/snapshots/snap_test_create_product_file_path.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,55 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_error[deleteProductFilePath-error] 1'] = {
+snapshots['test_schema_error[createProductFilePath-noSuchField] 1'] = {
     'data': {
         'allProductFilePaths': {
             'edges': [
-                {
-                    'node': {
-                        'productId': 1001
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1012
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1012
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1013
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1070
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1120
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1130
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1150
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1002
-                    }
-                },
-                {
-                    'node': {
-                        'productId': 1002
-                    }
-                }
+                {'node': {'productId': 1001}},
+                {'node': {'productId': 1012}},
+                {'node': {'productId': 1012}},
+                {'node': {'productId': 1013}},
+                {'node': {'productId': 1070}},
+                {'node': {'productId': 1120}},
+                {'node': {'productId': 1130}},
+                {'node': {'productId': 1150}},
+                {'node': {'productId': 1002}},
+                {'node': {'productId': 1002}},
             ]
         }
     }
 }
 
-snapshots['test_schema_success[deleteProductFilePath] 1'] = {
+snapshots['test_schema_success[createProductFilePath] 1'] = {
     'data': {
-        'deleteProductFilePath': {
-            'ok': True
+        'createProductFilePath': {
+            'productFilePath': {'path': 'nersc:/go/to/my/new_product_v1'}
         }
     }
 }
 
-snapshots['test_schema_success[deleteProductFilePath] 2'] = {
+snapshots['test_schema_success[createProductFilePath] 2'] = {
     'data': {
         'product': {
-            'name': 'lat20190213',
-            'note': '''- This is a dummy test with a lat map
-- This should not depend on any beam''',
+            'name': '20180101',
+            'note': '- test entry',
             'paths': {
                 'edges': [
+                    {
+                        'node': {
+                            'note': '- Note 1',
+                            'path': 'nersc:/go/to/my/new_product_v1',
+                            'product': {'productId': '1010'},
+                        }
+                    }
                 ]
             },
-            'timePosted': '2019-02-13T10:05:23'
+            'timePosted': '2018-01-01T15:32:10',
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_file_path/snapshots/snap_test_update_product_file_path.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_file_path/snapshots/snap_test_update_product_file_path.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_schema_error[updateProductFilePath-immutableField] 1'] = {
     'data': {
         'product': {
             'paths': {
                 'edges': [
                     {
                         'node': {
                             'note': '',
                             'path': 'nersc:/go/to/my/maps',
-                            'product': {
-                                'productId': '1001'
-                            }
+                            'product': {'productId': '1001'},
                         }
                     }
                 ]
             }
         }
     }
 }
 
 snapshots['test_schema_success[updateProductFilePath] 1'] = {
     'data': {
         'updateProductFilePath': {
-            'productFilePath': {
-                'path': 'nersc:/go/to/my/new_product_v2'
-            }
+            'productFilePath': {'path': 'nersc:/go/to/my/new_product_v2'}
         }
     }
 }
 
 snapshots['test_schema_success[updateProductFilePath] 2'] = {
     'data': {
         'product': {
@@ -45,18 +40,16 @@
 - This should not depend on any beam''',
             'paths': {
                 'edges': [
                     {
                         'node': {
                             'note': '- Note 1 updated',
                             'path': 'nersc:/go/to/my/new_product_v2',
-                            'product': {
-                                'productId': '1001'
-                            }
+                            'product': {'productId': '1001'},
                         }
                     }
                 ]
             },
-            'timePosted': '2019-02-13T10:05:23'
+            'timePosted': '2019-02-13T10:05:23',
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_file_path/test_create_product_file_path.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_file_path/test_update_product_file_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,90 @@
-import pytest
 import textwrap
 
+import pytest
+
 from ....funcs import assert_mutation
 
 HEADERS = {"Authorization": "Bearer token123"}  # octocat
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": textwrap.dedent(
                 """
                   mutation m {
-                    createProductFilePath(input: {
-                      path: "nersc:/go/to/my/new_product_v1",
-                      note: "- Note 1",
-                      productId: 1010
+                    updateProductFilePath(pathId: 1, input: {
+                      path: "nersc:/go/to/my/new_product_v2",
+                      note: "- Note 1 updated",
                     }) { productFilePath { path } }
                   }
-                """
+                """,
             ),
         },
         {
             "query": textwrap.dedent(
                 """
                   {
-                    product(productId: 1010) {
+                    product(productId: 1001) {
                       name timePosted note
                       paths { edges { node { path note product { productId } } } }
                     }
                   }
                 """,
             )
         },
-        id="createProductFilePath",
+        id="updateProductFilePath",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
-    ## To find the token
-    # from acondbs.models import GitHubUser
-    # with app.app_context():
-    #     user1 = GitHubUser.query.filter_by(login='octocat').one()
-    #     print(user1)
-    #     print(user1.tokens[0].token)
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": textwrap.dedent(
                 """
                   mutation m {
-                    createProductFilePath(input: {
-                      path: "nersc:/go/to/my/new_product_v1",
-                      note: "- Note 1",
-                      productId: 1010,
-                      noSuchField: "xxx"
+                    updateProductFilePath(pathId: 1, input: {
+                      productId: 1012
                     }) { productFilePath { path } }
                   }
                 """,
             )
         },
         {
             "query": textwrap.dedent(
                 """
                   {
-                    allProductFilePaths {
-                      edges {
-                        node {
-                          productId
-                        }
-                      }
+                    product(productId: 1001) {
+                      paths { edges { node { path note product { productId } } } }
                     }
                   }
                 """,
             )
         },
-        id="createProductFilePath-noSuchField",
+        id="updateProductFilePath-immutableField",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_error(
@@ -114,10 +97,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_file_path/test_delete_product_file_path.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_file_path/test_delete_product_file_path.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import pytest
 import textwrap
 
+import pytest
 
 from ....funcs import assert_mutation
 
 HEADERS = {"Authorization": "Bearer token123"}  # octocat
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": textwrap.dedent(
                 """
                   mutation m {
                     deleteProductFilePath(pathId: 1) { ok }
@@ -37,29 +36,27 @@
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": textwrap.dedent(
                 """
                   mutation m {
                     deleteProductFilePath(pathId: 15) { ok }
@@ -99,10 +96,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_file_path/test_update_product_file_path.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_file_path/test_create_product_file_path.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,105 @@
-import pytest
 import textwrap
 
+import pytest
+
 from ....funcs import assert_mutation
 
 HEADERS = {"Authorization": "Bearer token123"}  # octocat
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": textwrap.dedent(
                 """
                   mutation m {
-                    updateProductFilePath(pathId: 1, input: {
-                      path: "nersc:/go/to/my/new_product_v2",
-                      note: "- Note 1 updated",
+                    createProductFilePath(input: {
+                      path: "nersc:/go/to/my/new_product_v1",
+                      note: "- Note 1",
+                      productId: 1010
                     }) { productFilePath { path } }
                   }
-                """,
+                """
             ),
         },
         {
             "query": textwrap.dedent(
                 """
                   {
-                    product(productId: 1001) {
+                    product(productId: 1010) {
                       name timePosted note
                       paths { edges { node { path note product { productId } } } }
                     }
                   }
                 """,
             )
         },
-        id="updateProductFilePath",
+        id="createProductFilePath",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
+    ## To find the token
+    # from acondbs.models import GitHubUser
+    # with app.app_context():
+    #     user1 = GitHubUser.query.filter_by(login='octocat').one()
+    #     print(user1)
+    #     print(user1.tokens[0].token)
 
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": textwrap.dedent(
                 """
                   mutation m {
-                    updateProductFilePath(pathId: 1, input: {
-                      productId: 1012
+                    createProductFilePath(input: {
+                      path: "nersc:/go/to/my/new_product_v1",
+                      note: "- Note 1",
+                      productId: 1010,
+                      noSuchField: "xxx"
                     }) { productFilePath { path } }
                   }
                 """,
             )
         },
         {
             "query": textwrap.dedent(
                 """
                   {
-                    product(productId: 1001) {
-                      paths { edges { node { path note product { productId } } } }
+                    allProductFilePaths {
+                      edges {
+                        node {
+                          productId
+                        }
+                      }
                     }
                   }
                 """,
             )
         },
-        id="updateProductFilePath-immutableField",
+        id="createProductFilePath-noSuchField",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_error(
@@ -99,10 +112,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_relation/conftest.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_relation/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import pytest
 
 from acondbs import ops
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app_users):
-
     y = app_users
 
     # map1 -> beam1
     #            |
     #            +---> beam2
     #
     # map2
@@ -67,10 +65,7 @@
             type_id=1,
             self_product_id=5,
             other_product_id=4,
         )
         ops.commit()
 
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_relation/snapshots/snap_test_delete_product_relation.py` & `acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_all_product_relation_types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,154 +1,106 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_success[create] 1'] = {
-    'data': {
-        'deleteProductRelation': {
-            'ok': True
-        }
-    }
-}
-
-snapshots['test_schema_success[create] 2'] = {
+snapshots['test_schema[query] 1'] = {
     'data': {
-        'allProductRelations': {
+        'allProductRelationTypes': {
             'edges': [
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2',
-                            'productId': '5'
-                        },
-                        'relationId': '3',
-                        'reverse': {
-                            'relationId': '4'
-                        },
-                        'self_': {
-                            'name': 'beam1',
-                            'productId': '4'
-                        },
-                        'type_': {
-                            'name': 'child',
-                            'typeId': '2'
-                        }
+                        'indefArticle': 'a',
+                        'name': 'parent',
+                        'plural': 'parents',
+                        'relations': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
+                                    }
+                                },
+                            ]
+                        },
+                        'reverse': {'name': 'child', 'typeId': '2'},
+                        'singular': 'parent',
+                        'typeId': '1',
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam1',
-                            'productId': '4'
-                        },
-                        'relationId': '4',
-                        'reverse': {
-                            'relationId': '3'
-                        },
-                        'self_': {
-                            'name': 'beam2',
-                            'productId': '5'
-                        },
-                        'type_': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        }
-                    }
-                }
-            ]
-        }
-    }
-}
-
-snapshots['test_schema_error[error-nonexistent] 1'] = {
-    'data': {
-        'allProductRelations': {
-            'edges': [
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam1',
-                            'productId': '4'
-                        },
-                        'relationId': '1',
-                        'reverse': {
-                            'relationId': '2'
-                        },
-                        'self_': {
-                            'name': 'map1',
-                            'productId': '1'
-                        },
-                        'type_': {
-                            'name': 'child',
-                            'typeId': '2'
-                        }
+                        'indefArticle': 'a',
+                        'name': 'child',
+                        'plural': 'children',
+                        'relations': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
+                                    }
+                                },
+                            ]
+                        },
+                        'reverse': {'name': 'parent', 'typeId': '1'},
+                        'singular': 'child',
+                        'typeId': '2',
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'map1',
-                            'productId': '1'
-                        },
-                        'relationId': '2',
-                        'reverse': {
-                            'relationId': '1'
-                        },
-                        'self_': {
-                            'name': 'beam1',
-                            'productId': '4'
-                        },
-                        'type_': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        }
+                        'indefArticle': 'a',
+                        'name': 'plaintiff',
+                        'plural': 'plaintiffs',
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'defendant', 'typeId': '4'},
+                        'singular': 'plaintiff',
+                        'typeId': '3',
                     }
                 },
                 {
                     'node': {
-                        'other': {
-                            'name': 'beam2',
-                            'productId': '5'
-                        },
-                        'relationId': '3',
-                        'reverse': {
-                            'relationId': '4'
-                        },
-                        'self_': {
-                            'name': 'beam1',
-                            'productId': '4'
-                        },
-                        'type_': {
-                            'name': 'child',
-                            'typeId': '2'
-                        }
+                        'indefArticle': 'a',
+                        'name': 'defendant',
+                        'plural': 'defendants',
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'plaintiff', 'typeId': '3'},
+                        'singular': 'defendant',
+                        'typeId': '4',
                     }
                 },
-                {
-                    'node': {
-                        'other': {
-                            'name': 'beam1',
-                            'productId': '4'
-                        },
-                        'relationId': '4',
-                        'reverse': {
-                            'relationId': '3'
-                        },
-                        'self_': {
-                            'name': 'beam2',
-                            'productId': '5'
-                        },
-                        'type_': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        }
-                    }
-                }
             ]
         }
     }
 }
+
+snapshots['test_schema[total-count] 1'] = {
+    'data': {'allProductRelationTypes': {'totalCount': 4}}
+}
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_relation/test_delete_product_relation.py` & `acondbs-0.4.4/tests/schema/product/mutation/field/test_create_field.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,78 @@
 import pytest
 
 from ....funcs import assert_mutation
-
-from ...gql import FRAGMENT_PRODUCT_RELATION_CONNECTION, MUTATION_DELETE_PRODUCT_RELATION
-
-QEURY = (
-    """
-{
-  allProductRelations {
-    ...fragmentProductRelationConnection
-  }
-}
-"""
-    + FRAGMENT_PRODUCT_RELATION_CONNECTION
-)
+from ...gql import MUTATION_CREATE_FIELD, QUERY_ALL_FIELDS
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
-        {"query": MUTATION_DELETE_PRODUCT_RELATION, "variables": {"relationId": 2}},
-        {"query": QEURY},
-        id="create",
+        {
+            "query": MUTATION_CREATE_FIELD,
+            "variables": {
+                "input": {
+                    "name": "author",
+                    "type_": "UNICODE_TEXT",
+                }
+            },
+        },
+        {"query": QUERY_ALL_FIELDS},
+        id="by-enum-name",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
-        {"query": MUTATION_DELETE_PRODUCT_RELATION, "variables": {"relationId": 120}},
-        {"query": QEURY},
-        id="error-nonexistent",
+        {
+            "query": MUTATION_CREATE_FIELD,
+            "variables": {
+                "input": {
+                    "name": "author",
+                    "type_": 1,
+                }
+            },
+        },
+        {"query": QUERY_ALL_FIELDS},
+        id="by-enum-int",
+    ),
+    pytest.param(
+        {
+            "query": MUTATION_CREATE_FIELD,
+            "variables": {
+                "input": {
+                    "name": "author",
+                    "type_": "NONEXISTENT_ENUM",
+                }
+            },
+        },
+        {"query": QUERY_ALL_FIELDS},
+        id="enum-nonexistent",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_error(
@@ -71,10 +85,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/conftest.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import pytest
 
 from acondbs import ops
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app_users):
-
     y = app_users
 
     # Relation types:
     #   parent <-> child
     #   plaintiff <-> defendant
 
     # Relations:
@@ -90,10 +88,7 @@
             type_id=1,
             self_product_id=5,
             other_product_id=4,
         )
         ops.commit()
 
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/snapshots/snap_test_create_product_relation_types.py` & `acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_all_products.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,701 +1,651 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_error[error-already-exist] 1'] = {
+snapshots['test_schema[deep] 1'] = {
     'data': {
-        'allProductRelationTypes': {
+        'allProducts': {
             'edges': [
                 {
                     'node': {
-                        'indefArticle': 'a',
-                        'name': 'parent',
-                        'plural': 'parents',
-                        'relations': {
+                        'attributesBoolean': {'edges': []},
+                        'attributesDate': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
                                         },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'date_produced',
+                                                'type_': 'DATE',
+                                            }
+                                        },
+                                        'value': '2020-02-01',
                                     }
-                                },
+                                }
+                            ]
+                        },
+                        'attributesDateTime': {'edges': []},
+                        'attributesFloat': {'edges': []},
+                        'attributesInteger': {'edges': []},
+                        'attributesTime': {'edges': []},
+                        'attributesUnicodeText': {
+                            'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
                                         },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'contact',
+                                                'type_': 'UNICODE_TEXT',
+                                            }
+                                        },
+                                        'value': None,
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
                                         },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'produced_by',
+                                                'type_': 'UNICODE_TEXT',
+                                            }
+                                        },
+                                        'value': None,
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'child',
-                            'typeId': '2'
-                        },
-                        'singular': 'parent',
-                        'typeId': '1'
-                    }
-                },
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'child',
-                        'plural': 'children',
-                        'relations': {
+                        'name': 'map1',
+                        'note': None,
+                        'paths': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'note': None,
+                                        'path': 'site2:/another/way/map1',
+                                        'pathId': '1',
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'note': 'sample comment',
+                                        'path': 'site1:/path/to/map1',
+                                        'pathId': '8',
                                     }
                                 },
+                            ]
+                        },
+                        'postingGitHubUser': None,
+                        'productId': '1',
+                        'relations': {
+                            'edges': [
                                 {
                                     'node': {
                                         'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
+                                            'name': 'beam1',
+                                            'productId': '4',
+                                            'typeId': 2,
+                                            'type_': {'name': 'beam', 'typeId': '2'},
                                         },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'otherProductId': 4,
+                                        'relationId': '1',
+                                        'reverse': {
+                                            'relationId': '2',
+                                            'typeId': 1,
+                                            'type_': {'name': 'parent', 'typeId': '1'},
+                                        },
+                                        'reverseRelationId': 2,
+                                        'typeId': 2,
+                                        'type_': {'name': 'child', 'typeId': '2'},
                                     }
                                 },
                                 {
                                     'node': {
                                         'other': {
                                             'name': 'beam2',
-                                            'productId': '5'
+                                            'productId': '5',
+                                            'typeId': 2,
+                                            'type_': {'name': 'beam', 'typeId': '2'},
                                         },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'otherProductId': 5,
+                                        'relationId': '3',
+                                        'reverse': {
+                                            'relationId': '4',
+                                            'typeId': 1,
+                                            'type_': {'name': 'parent', 'typeId': '1'},
+                                        },
+                                        'reverseRelationId': 4,
+                                        'typeId': 2,
+                                        'type_': {'name': 'child', 'typeId': '2'},
                                     }
-                                }
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        },
-                        'singular': 'child',
-                        'typeId': '2'
-                    }
-                },
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'plaintiff',
-                        'plural': 'plaintiffs',
-                        'relations': {
-                            'edges': [
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'defendant',
-                            'typeId': '4'
-                        },
-                        'singular': 'plaintiff',
-                        'typeId': '3'
+                        'timePosted': '2021-01-04T14:32:20',
+                        'timeUpdated': None,
+                        'typeId': 1,
+                        'type_': {'name': 'map', 'typeId': '1'},
+                        'updatingGitHubUser': None,
                     }
                 },
                 {
                     'node': {
-                        'indefArticle': 'a',
-                        'name': 'defendant',
-                        'plural': 'defendants',
-                        'relations': {
+                        'attributesBoolean': {'edges': []},
+                        'attributesDate': {
                             'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'date_produced',
+                                                'type_': 'DATE',
+                                            }
+                                        },
+                                        'value': '2020-02-10',
+                                    }
+                                }
                             ]
                         },
-                        'reverse': {
-                            'name': 'plaintiff',
-                            'typeId': '3'
-                        },
-                        'singular': 'defendant',
-                        'typeId': '4'
-                    }
-                }
-            ]
-        }
-    }
-}
-
-snapshots['test_schema_error[error-reverse-and-self_reverse] 1'] = {
-    'data': {
-        'allProductRelationTypes': {
-            'edges': [
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'parent',
-                        'plural': 'parents',
-                        'relations': {
+                        'attributesDateTime': {'edges': []},
+                        'attributesFloat': {'edges': []},
+                        'attributesInteger': {'edges': []},
+                        'attributesTime': {'edges': []},
+                        'attributesUnicodeText': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
                                         },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'contact',
+                                                'type_': 'UNICODE_TEXT',
+                                            }
+                                        },
+                                        'value': None,
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
                                         },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'produced_by',
+                                                'type_': 'UNICODE_TEXT',
+                                            }
+                                        },
+                                        'value': None,
                                     }
                                 },
+                            ]
+                        },
+                        'name': 'map2',
+                        'note': None,
+                        'paths': {
+                            'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'note': None,
+                                        'path': 'site1:/path/to/map2',
+                                        'pathId': '2',
                                     }
                                 }
                             ]
                         },
-                        'reverse': {
-                            'name': 'child',
-                            'typeId': '2'
-                        },
-                        'singular': 'parent',
-                        'typeId': '1'
+                        'postingGitHubUser': None,
+                        'productId': '2',
+                        'relations': {'edges': []},
+                        'timePosted': '2021-01-04T14:32:20',
+                        'timeUpdated': None,
+                        'typeId': 1,
+                        'type_': {'name': 'map', 'typeId': '1'},
+                        'updatingGitHubUser': None,
                     }
                 },
                 {
                     'node': {
-                        'indefArticle': 'a',
-                        'name': 'child',
-                        'plural': 'children',
-                        'relations': {
+                        'attributesBoolean': {'edges': []},
+                        'attributesDate': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
                                         },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'date_produced',
+                                                'type_': 'DATE',
+                                            }
+                                        },
+                                        'value': '2020-03-19',
                                     }
-                                },
+                                }
+                            ]
+                        },
+                        'attributesDateTime': {'edges': []},
+                        'attributesFloat': {'edges': []},
+                        'attributesInteger': {'edges': []},
+                        'attributesTime': {'edges': []},
+                        'attributesUnicodeText': {
+                            'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
                                         },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'contact',
+                                                'type_': 'UNICODE_TEXT',
+                                            }
+                                        },
+                                        'value': None,
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
                                         },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'produced_by',
+                                                'type_': 'UNICODE_TEXT',
+                                            }
+                                        },
+                                        'value': None,
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        },
-                        'singular': 'child',
-                        'typeId': '2'
-                    }
-                },
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'plaintiff',
-                        'plural': 'plaintiffs',
-                        'relations': {
+                        'name': 'map3',
+                        'note': None,
+                        'paths': {
                             'edges': [
+                                {
+                                    'node': {
+                                        'note': None,
+                                        'path': 'site1:/path/to/map3',
+                                        'pathId': '3',
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'note': None,
+                                        'path': 'site2:/another/way/map3',
+                                        'pathId': '4',
+                                    }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'defendant',
-                            'typeId': '4'
-                        },
-                        'singular': 'plaintiff',
-                        'typeId': '3'
+                        'postingGitHubUser': None,
+                        'productId': '3',
+                        'relations': {'edges': []},
+                        'timePosted': '2021-01-04T14:32:20',
+                        'timeUpdated': None,
+                        'typeId': 1,
+                        'type_': {'name': 'map', 'typeId': '1'},
+                        'updatingGitHubUser': None,
                     }
                 },
                 {
                     'node': {
-                        'indefArticle': 'a',
-                        'name': 'defendant',
-                        'plural': 'defendants',
-                        'relations': {
+                        'attributesBoolean': {'edges': []},
+                        'attributesDate': {
                             'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'date_produced',
+                                                'type_': 'DATE',
+                                            }
+                                        },
+                                        'value': '2020-02-05',
+                                    }
+                                }
                             ]
                         },
-                        'reverse': {
-                            'name': 'plaintiff',
-                            'typeId': '3'
-                        },
-                        'singular': 'defendant',
-                        'typeId': '4'
-                    }
-                }
-            ]
-        }
-    }
-}
-
-snapshots['test_schema_success[reverse] 1'] = {
-    'data': {
-        'createProductRelationTypes': {
-            'ok': True,
-            'productRelationType': {
-                'indefArticle': 'a',
-                'name': 'doctor',
-                'plural': 'doctors',
-                'relations': {
-                    'edges': [
-                    ]
-                },
-                'reverse': {
-                    'name': 'patient',
-                    'typeId': '6'
-                },
-                'singular': 'doctor',
-                'typeId': '5'
-            }
-        }
-    }
-}
-
-snapshots['test_schema_success[reverse] 2'] = {
-    'data': {
-        'allProductRelationTypes': {
-            'edges': [
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'parent',
-                        'plural': 'parents',
-                        'relations': {
+                        'attributesDateTime': {'edges': []},
+                        'attributesFloat': {'edges': []},
+                        'attributesInteger': {'edges': []},
+                        'attributesTime': {'edges': []},
+                        'attributesUnicodeText': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
                                         },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'contact',
+                                                'type_': 'UNICODE_TEXT',
+                                            }
+                                        },
+                                        'value': None,
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
                                         },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'produced_by',
+                                                'type_': 'UNICODE_TEXT',
+                                            }
+                                        },
+                                        'value': None,
                                     }
                                 },
+                            ]
+                        },
+                        'name': 'beam1',
+                        'note': None,
+                        'paths': {
+                            'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'note': None,
+                                        'path': 'site1:/path/to/beam1',
+                                        'pathId': '5',
                                     }
-                                }
+                                },
+                                {
+                                    'node': {
+                                        'note': None,
+                                        'path': 'site2:/another/way/beam1',
+                                        'pathId': '6',
+                                    }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'child',
-                            'typeId': '2'
-                        },
-                        'singular': 'parent',
-                        'typeId': '1'
-                    }
-                },
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'child',
-                        'plural': 'children',
+                        'postingGitHubUser': None,
+                        'productId': '4',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
                                         'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
                                             'name': 'map1',
-                                            'productId': '1'
-                                        }
-                                    }
-                                },
-                                {
-                                    'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
+                                            'productId': '1',
+                                            'typeId': 1,
+                                            'type_': {'name': 'map', 'typeId': '1'},
                                         },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'otherProductId': 1,
+                                        'relationId': '2',
+                                        'reverse': {
+                                            'relationId': '1',
+                                            'typeId': 2,
+                                            'type_': {'name': 'child', 'typeId': '2'},
+                                        },
+                                        'reverseRelationId': 1,
+                                        'typeId': 1,
+                                        'type_': {'name': 'parent', 'typeId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
                                         'other': {
                                             'name': 'beam2',
-                                            'productId': '5'
+                                            'productId': '5',
+                                            'typeId': 2,
+                                            'type_': {'name': 'beam', 'typeId': '2'},
                                         },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'otherProductId': 5,
+                                        'relationId': '5',
+                                        'reverse': {
+                                            'relationId': '6',
+                                            'typeId': 1,
+                                            'type_': {'name': 'parent', 'typeId': '1'},
+                                        },
+                                        'reverseRelationId': 6,
+                                        'typeId': 2,
+                                        'type_': {'name': 'child', 'typeId': '2'},
                                     }
-                                }
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        },
-                        'singular': 'child',
-                        'typeId': '2'
-                    }
-                },
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'plaintiff',
-                        'plural': 'plaintiffs',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'defendant',
-                            'typeId': '4'
-                        },
-                        'singular': 'plaintiff',
-                        'typeId': '3'
-                    }
-                },
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'defendant',
-                        'plural': 'defendants',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'plaintiff',
-                            'typeId': '3'
-                        },
-                        'singular': 'defendant',
-                        'typeId': '4'
-                    }
-                },
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'doctor',
-                        'plural': 'doctors',
-                        'relations': {
-                            'edges': [
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'patient',
-                            'typeId': '6'
-                        },
-                        'singular': 'doctor',
-                        'typeId': '5'
+                        'timePosted': '2021-01-04T14:32:20',
+                        'timeUpdated': None,
+                        'typeId': 2,
+                        'type_': {'name': 'beam', 'typeId': '2'},
+                        'updatingGitHubUser': None,
                     }
                 },
                 {
                     'node': {
-                        'indefArticle': 'a',
-                        'name': 'patient',
-                        'plural': 'patients',
-                        'relations': {
+                        'attributesBoolean': {'edges': []},
+                        'attributesDate': {
                             'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'date_produced',
+                                                'type_': 'DATE',
+                                            }
+                                        },
+                                        'value': '2020-03-04',
+                                    }
+                                }
                             ]
                         },
-                        'reverse': {
-                            'name': 'doctor',
-                            'typeId': '5'
-                        },
-                        'singular': 'patient',
-                        'typeId': '6'
-                    }
-                }
-            ]
-        }
-    }
-}
-
-snapshots['test_schema_success[self_reverse] 1'] = {
-    'data': {
-        'createProductRelationTypes': {
-            'ok': True,
-            'productRelationType': {
-                'indefArticle': 'a',
-                'name': 'spouse',
-                'plural': 'spouses',
-                'relations': {
-                    'edges': [
-                    ]
-                },
-                'reverse': {
-                    'name': 'spouse',
-                    'typeId': '5'
-                },
-                'singular': 'spouse',
-                'typeId': '5'
-            }
-        }
-    }
-}
-
-snapshots['test_schema_success[self_reverse] 2'] = {
-    'data': {
-        'allProductRelationTypes': {
-            'edges': [
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'parent',
-                        'plural': 'parents',
-                        'relations': {
+                        'attributesDateTime': {'edges': []},
+                        'attributesFloat': {'edges': []},
+                        'attributesInteger': {'edges': []},
+                        'attributesTime': {'edges': []},
+                        'attributesUnicodeText': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
                                         },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'contact',
+                                                'type_': 'UNICODE_TEXT',
+                                            }
+                                        },
+                                        'value': None,
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
                                         },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'typeFieldAssociation': {
+                                            'field': {
+                                                'name': 'produced_by',
+                                                'type_': 'UNICODE_TEXT',
+                                            }
+                                        },
+                                        'value': None,
                                     }
                                 },
+                            ]
+                        },
+                        'name': 'beam2',
+                        'note': None,
+                        'paths': {
+                            'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'note': None,
+                                        'path': 'site1:/path/to/beam2',
+                                        'pathId': '7',
                                     }
                                 }
                             ]
                         },
-                        'reverse': {
-                            'name': 'child',
-                            'typeId': '2'
-                        },
-                        'singular': 'parent',
-                        'typeId': '1'
-                    }
-                },
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'child',
-                        'plural': 'children',
+                        'postingGitHubUser': None,
+                        'productId': '5',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
                                         'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
                                             'name': 'map1',
-                                            'productId': '1'
-                                        }
-                                    }
-                                },
-                                {
-                                    'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
+                                            'productId': '1',
+                                            'typeId': 1,
+                                            'type_': {'name': 'map', 'typeId': '1'},
                                         },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'otherProductId': 1,
+                                        'relationId': '4',
+                                        'reverse': {
+                                            'relationId': '3',
+                                            'typeId': 2,
+                                            'type_': {'name': 'child', 'typeId': '2'},
+                                        },
+                                        'reverseRelationId': 3,
+                                        'typeId': 1,
+                                        'type_': {'name': 'parent', 'typeId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
                                         'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        },
-                                        'self_': {
                                             'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                            'productId': '4',
+                                            'typeId': 2,
+                                            'type_': {'name': 'beam', 'typeId': '2'},
+                                        },
+                                        'otherProductId': 4,
+                                        'relationId': '6',
+                                        'reverse': {
+                                            'relationId': '5',
+                                            'typeId': 2,
+                                            'type_': {'name': 'child', 'typeId': '2'},
+                                        },
+                                        'reverseRelationId': 5,
+                                        'typeId': 1,
+                                        'type_': {'name': 'parent', 'typeId': '1'},
                                     }
-                                }
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        },
-                        'singular': 'child',
-                        'typeId': '2'
-                    }
-                },
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'plaintiff',
-                        'plural': 'plaintiffs',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'defendant',
-                            'typeId': '4'
-                        },
-                        'singular': 'plaintiff',
-                        'typeId': '3'
-                    }
-                },
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'defendant',
-                        'plural': 'defendants',
-                        'relations': {
-                            'edges': [
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'plaintiff',
-                            'typeId': '3'
-                        },
-                        'singular': 'defendant',
-                        'typeId': '4'
+                        'timePosted': '2021-01-04T14:32:20',
+                        'timeUpdated': None,
+                        'typeId': 2,
+                        'type_': {'name': 'beam', 'typeId': '2'},
+                        'updatingGitHubUser': None,
                     }
                 },
-                {
-                    'node': {
-                        'indefArticle': 'a',
-                        'name': 'spouse',
-                        'plural': 'spouses',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'spouse',
-                            'typeId': '5'
-                        },
-                        'singular': 'spouse',
-                        'typeId': '5'
-                    }
-                }
             ]
         }
     }
 }
+
+snapshots['test_schema[filters-type_id-first-two] 1'] = {
+    'data': {
+        'allProducts': {
+            'edges': [
+                {'node': {'name': 'map1', 'productId': '1', 'typeId': 1}},
+                {'node': {'name': 'map2', 'productId': '2', 'typeId': 1}},
+            ]
+        }
+    }
+}
+
+snapshots['test_schema[filters-type_id-sort] 1'] = {
+    'data': {
+        'allProducts': {
+            'edges': [
+                {'node': {'name': 'map1', 'productId': '1', 'typeId': 1}},
+                {'node': {'name': 'map2', 'productId': '2', 'typeId': 1}},
+                {'node': {'name': 'map3', 'productId': '3', 'typeId': 1}},
+            ]
+        }
+    }
+}
+
+snapshots['test_schema[filters-type_name-first-two] 1'] = {
+    'data': {
+        'allProducts': {
+            'edges': [
+                {'node': {'name': 'map1', 'productId': '1', 'typeId': 1}},
+                {'node': {'name': 'map2', 'productId': '2', 'typeId': 1}},
+            ]
+        }
+    }
+}
+
+snapshots['test_schema[filters-type_name-sort] 1'] = {
+    'data': {
+        'allProducts': {
+            'edges': [
+                {'node': {'name': 'map1', 'productId': '1', 'typeId': 1}},
+                {'node': {'name': 'map2', 'productId': '2', 'typeId': 1}},
+                {'node': {'name': 'map3', 'productId': '3', 'typeId': 1}},
+            ]
+        }
+    }
+}
+
+snapshots['test_schema[first-two-sort] 1'] = {
+    'data': {
+        'allProducts': {
+            'edges': [
+                {'node': {'name': 'map1', 'productId': '1', 'typeId': 1}},
+                {'node': {'name': 'map2', 'productId': '2', 'typeId': 1}},
+            ]
+        }
+    }
+}
+
+snapshots['test_schema[first-two] 1'] = {
+    'data': {
+        'allProducts': {
+            'edges': [
+                {'node': {'name': 'map1', 'productId': '1', 'typeId': 1}},
+                {'node': {'name': 'map2', 'productId': '2', 'typeId': 1}},
+            ]
+        }
+    }
+}
+
+snapshots['test_schema[total-count] 1'] = {'data': {'allProducts': {'totalCount': 3}}}
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/snapshots/snap_test_delete_product_relation_types.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/snapshots/snap_test_create_product_relation_types.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,429 +1,454 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_error[error-nonexistent] 1'] = {
+snapshots['test_schema_error[error-already-exist] 1'] = {
     'data': {
         'allProductRelationTypes': {
             'edges': [
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'parent',
                         'plural': 'parents',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'child',
-                            'typeId': '2'
-                        },
+                        'reverse': {'name': 'child', 'typeId': '2'},
                         'singular': 'parent',
-                        'typeId': '1'
+                        'typeId': '1',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'child',
                         'plural': 'children',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        },
+                        'reverse': {'name': 'parent', 'typeId': '1'},
                         'singular': 'child',
-                        'typeId': '2'
+                        'typeId': '2',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'plaintiff',
                         'plural': 'plaintiffs',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'defendant',
-                            'typeId': '4'
-                        },
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'defendant', 'typeId': '4'},
                         'singular': 'plaintiff',
-                        'typeId': '3'
+                        'typeId': '3',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'defendant',
                         'plural': 'defendants',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'plaintiff',
-                            'typeId': '3'
-                        },
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'plaintiff', 'typeId': '3'},
                         'singular': 'defendant',
-                        'typeId': '4'
+                        'typeId': '4',
                     }
-                }
+                },
             ]
         }
     }
 }
 
-snapshots['test_schema_error[error-unempty] 1'] = {
+snapshots['test_schema_error[error-reverse-and-self_reverse] 1'] = {
     'data': {
         'allProductRelationTypes': {
             'edges': [
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'parent',
                         'plural': 'parents',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'child',
-                            'typeId': '2'
-                        },
+                        'reverse': {'name': 'child', 'typeId': '2'},
                         'singular': 'parent',
-                        'typeId': '1'
+                        'typeId': '1',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'child',
                         'plural': 'children',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        },
+                        'reverse': {'name': 'parent', 'typeId': '1'},
                         'singular': 'child',
-                        'typeId': '2'
+                        'typeId': '2',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'plaintiff',
                         'plural': 'plaintiffs',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'defendant',
-                            'typeId': '4'
-                        },
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'defendant', 'typeId': '4'},
                         'singular': 'plaintiff',
-                        'typeId': '3'
+                        'typeId': '3',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'defendant',
                         'plural': 'defendants',
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'plaintiff', 'typeId': '3'},
+                        'singular': 'defendant',
+                        'typeId': '4',
+                    }
+                },
+            ]
+        }
+    }
+}
+
+snapshots['test_schema_success[reverse] 1'] = {
+    'data': {
+        'createProductRelationTypes': {
+            'ok': True,
+            'productRelationType': {
+                'indefArticle': 'a',
+                'name': 'doctor',
+                'plural': 'doctors',
+                'relations': {'edges': []},
+                'reverse': {'name': 'patient', 'typeId': '6'},
+                'singular': 'doctor',
+                'typeId': '5',
+            },
+        }
+    }
+}
+
+snapshots['test_schema_success[reverse] 2'] = {
+    'data': {
+        'allProductRelationTypes': {
+            'edges': [
+                {
+                    'node': {
+                        'indefArticle': 'a',
+                        'name': 'parent',
+                        'plural': 'parents',
                         'relations': {
                             'edges': [
+                                {
+                                    'node': {
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
+                                    }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'plaintiff',
-                            'typeId': '3'
+                        'reverse': {'name': 'child', 'typeId': '2'},
+                        'singular': 'parent',
+                        'typeId': '1',
+                    }
+                },
+                {
+                    'node': {
+                        'indefArticle': 'a',
+                        'name': 'child',
+                        'plural': 'children',
+                        'relations': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
+                                    }
+                                },
+                            ]
                         },
+                        'reverse': {'name': 'parent', 'typeId': '1'},
+                        'singular': 'child',
+                        'typeId': '2',
+                    }
+                },
+                {
+                    'node': {
+                        'indefArticle': 'a',
+                        'name': 'plaintiff',
+                        'plural': 'plaintiffs',
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'defendant', 'typeId': '4'},
+                        'singular': 'plaintiff',
+                        'typeId': '3',
+                    }
+                },
+                {
+                    'node': {
+                        'indefArticle': 'a',
+                        'name': 'defendant',
+                        'plural': 'defendants',
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'plaintiff', 'typeId': '3'},
                         'singular': 'defendant',
-                        'typeId': '4'
+                        'typeId': '4',
                     }
-                }
+                },
+                {
+                    'node': {
+                        'indefArticle': 'a',
+                        'name': 'doctor',
+                        'plural': 'doctors',
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'patient', 'typeId': '6'},
+                        'singular': 'doctor',
+                        'typeId': '5',
+                    }
+                },
+                {
+                    'node': {
+                        'indefArticle': 'a',
+                        'name': 'patient',
+                        'plural': 'patients',
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'doctor', 'typeId': '5'},
+                        'singular': 'patient',
+                        'typeId': '6',
+                    }
+                },
             ]
         }
     }
 }
 
-snapshots['test_schema_success[delete] 1'] = {
+snapshots['test_schema_success[self_reverse] 1'] = {
     'data': {
-        'deleteProductRelationTypes': {
-            'ok': True
+        'createProductRelationTypes': {
+            'ok': True,
+            'productRelationType': {
+                'indefArticle': 'a',
+                'name': 'spouse',
+                'plural': 'spouses',
+                'relations': {'edges': []},
+                'reverse': {'name': 'spouse', 'typeId': '5'},
+                'singular': 'spouse',
+                'typeId': '5',
+            },
         }
     }
 }
 
-snapshots['test_schema_success[delete] 2'] = {
+snapshots['test_schema_success[self_reverse] 2'] = {
     'data': {
         'allProductRelationTypes': {
             'edges': [
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'parent',
                         'plural': 'parents',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'child',
-                            'typeId': '2'
-                        },
+                        'reverse': {'name': 'child', 'typeId': '2'},
                         'singular': 'parent',
-                        'typeId': '1'
+                        'typeId': '1',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'child',
                         'plural': 'children',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        },
+                        'reverse': {'name': 'parent', 'typeId': '1'},
                         'singular': 'child',
-                        'typeId': '2'
+                        'typeId': '2',
                     }
-                }
+                },
+                {
+                    'node': {
+                        'indefArticle': 'a',
+                        'name': 'plaintiff',
+                        'plural': 'plaintiffs',
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'defendant', 'typeId': '4'},
+                        'singular': 'plaintiff',
+                        'typeId': '3',
+                    }
+                },
+                {
+                    'node': {
+                        'indefArticle': 'a',
+                        'name': 'defendant',
+                        'plural': 'defendants',
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'plaintiff', 'typeId': '3'},
+                        'singular': 'defendant',
+                        'typeId': '4',
+                    }
+                },
+                {
+                    'node': {
+                        'indefArticle': 'a',
+                        'name': 'spouse',
+                        'plural': 'spouses',
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'spouse', 'typeId': '5'},
+                        'singular': 'spouse',
+                        'typeId': '5',
+                    }
+                },
             ]
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/snapshots/snap_test_update_product_relation_type.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/snapshots/snap_test_delete_product_relation_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,365 +1,274 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema_error[error-immutable-field] 1'] = {
+snapshots['test_schema_error[error-nonexistent] 1'] = {
     'data': {
         'allProductRelationTypes': {
             'edges': [
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'parent',
                         'plural': 'parents',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'child',
-                            'typeId': '2'
-                        },
+                        'reverse': {'name': 'child', 'typeId': '2'},
                         'singular': 'parent',
-                        'typeId': '1'
+                        'typeId': '1',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'child',
                         'plural': 'children',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        },
+                        'reverse': {'name': 'parent', 'typeId': '1'},
                         'singular': 'child',
-                        'typeId': '2'
+                        'typeId': '2',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'plaintiff',
                         'plural': 'plaintiffs',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'defendant',
-                            'typeId': '4'
-                        },
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'defendant', 'typeId': '4'},
                         'singular': 'plaintiff',
-                        'typeId': '3'
+                        'typeId': '3',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'defendant',
                         'plural': 'defendants',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'plaintiff',
-                            'typeId': '3'
-                        },
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'plaintiff', 'typeId': '3'},
                         'singular': 'defendant',
-                        'typeId': '4'
+                        'typeId': '4',
                     }
-                }
-            ]
-        }
-    }
-}
-
-snapshots['test_schema_success[update] 1'] = {
-    'data': {
-        'updateProductRelationType': {
-            'ok': True,
-            'productRelationType': {
-                'indefArticle': 'an',
-                'name': 'parent',
-                'plural': 'mmaps',
-                'relations': {
-                    'edges': [
-                        {
-                            'node': {
-                                'other': {
-                                    'name': 'map1',
-                                    'productId': '1'
-                                },
-                                'self_': {
-                                    'name': 'beam1',
-                                    'productId': '4'
-                                }
-                            }
-                        },
-                        {
-                            'node': {
-                                'other': {
-                                    'name': 'map1',
-                                    'productId': '1'
-                                },
-                                'self_': {
-                                    'name': 'beam2',
-                                    'productId': '5'
-                                }
-                            }
-                        },
-                        {
-                            'node': {
-                                'other': {
-                                    'name': 'beam1',
-                                    'productId': '4'
-                                },
-                                'self_': {
-                                    'name': 'beam2',
-                                    'productId': '5'
-                                }
-                            }
-                        }
-                    ]
-                },
-                'reverse': {
-                    'name': 'child',
-                    'typeId': '2'
                 },
-                'singular': 'mmap',
-                'typeId': '1'
-            }
+            ]
         }
     }
 }
 
-snapshots['test_schema_success[update] 2'] = {
+snapshots['test_schema_error[error-unempty] 1'] = {
     'data': {
         'allProductRelationTypes': {
             'edges': [
                 {
                     'node': {
-                        'indefArticle': 'an',
+                        'indefArticle': 'a',
                         'name': 'parent',
-                        'plural': 'mmaps',
+                        'plural': 'parents',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        }
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'child',
-                            'typeId': '2'
-                        },
-                        'singular': 'mmap',
-                        'typeId': '1'
+                        'reverse': {'name': 'child', 'typeId': '2'},
+                        'singular': 'parent',
+                        'typeId': '1',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'child',
                         'plural': 'children',
                         'relations': {
                             'edges': [
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        },
-                                        'self_': {
-                                            'name': 'map1',
-                                            'productId': '1'
-                                        }
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
                                     }
                                 },
                                 {
                                     'node': {
-                                        'other': {
-                                            'name': 'beam2',
-                                            'productId': '5'
-                                        },
-                                        'self_': {
-                                            'name': 'beam1',
-                                            'productId': '4'
-                                        }
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
                                     }
-                                }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'parent',
-                            'typeId': '1'
-                        },
+                        'reverse': {'name': 'parent', 'typeId': '1'},
                         'singular': 'child',
-                        'typeId': '2'
+                        'typeId': '2',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'plaintiff',
                         'plural': 'plaintiffs',
-                        'relations': {
-                            'edges': [
-                            ]
-                        },
-                        'reverse': {
-                            'name': 'defendant',
-                            'typeId': '4'
-                        },
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'defendant', 'typeId': '4'},
                         'singular': 'plaintiff',
-                        'typeId': '3'
+                        'typeId': '3',
                     }
                 },
                 {
                     'node': {
                         'indefArticle': 'a',
                         'name': 'defendant',
                         'plural': 'defendants',
+                        'relations': {'edges': []},
+                        'reverse': {'name': 'plaintiff', 'typeId': '3'},
+                        'singular': 'defendant',
+                        'typeId': '4',
+                    }
+                },
+            ]
+        }
+    }
+}
+
+snapshots['test_schema_success[delete] 1'] = {
+    'data': {'deleteProductRelationTypes': {'ok': True}}
+}
+
+snapshots['test_schema_success[delete] 2'] = {
+    'data': {
+        'allProductRelationTypes': {
+            'edges': [
+                {
+                    'node': {
+                        'indefArticle': 'a',
+                        'name': 'parent',
+                        'plural': 'parents',
                         'relations': {
                             'edges': [
+                                {
+                                    'node': {
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'map1', 'productId': '1'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'beam2', 'productId': '5'},
+                                    }
+                                },
                             ]
                         },
-                        'reverse': {
-                            'name': 'plaintiff',
-                            'typeId': '3'
+                        'reverse': {'name': 'child', 'typeId': '2'},
+                        'singular': 'parent',
+                        'typeId': '1',
+                    }
+                },
+                {
+                    'node': {
+                        'indefArticle': 'a',
+                        'name': 'child',
+                        'plural': 'children',
+                        'relations': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam1', 'productId': '4'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'map1', 'productId': '1'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'other': {'name': 'beam2', 'productId': '5'},
+                                        'self_': {'name': 'beam1', 'productId': '4'},
+                                    }
+                                },
+                            ]
                         },
-                        'singular': 'defendant',
-                        'typeId': '4'
+                        'reverse': {'name': 'parent', 'typeId': '1'},
+                        'singular': 'child',
+                        'typeId': '2',
                     }
-                }
+                },
             ]
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/test_create_product_relation_types.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/test_create_product_relation_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import pytest
 
 from ....funcs import assert_mutation
-
 from ...gql import (
     FRAGMENT_PRODUCT_RELATION_TYPE_CONNECTION,
     MUTATION_CREATE_PRODUCT_RELATION_TYPES,
 )
 
-##__________________________________________________________________||
 QEURY = (
     """
 {
   allProductRelationTypes {
    ...fragmentProductRelationTypeConnection
   }
 }
@@ -20,15 +18,14 @@
 )
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_CREATE_PRODUCT_RELATION_TYPES,
             "variables": {
                 "type": {
                     "name": "doctor",
@@ -67,29 +64,27 @@
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_CREATE_PRODUCT_RELATION_TYPES,
             "variables": {
                 "type": {
                     "name": "parent",
@@ -145,10 +140,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_relation_type/test_delete_product_relation_types.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_relation_type/test_update_product_relation_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import pytest
 
 from ....funcs import assert_mutation
-
 from ...gql import (
     FRAGMENT_PRODUCT_RELATION_TYPE_CONNECTION,
-    MUTATION_DELETE_PRODUCT_RELATION_TYPES,
+    MUTATION_UPDATE_PRODUCT_RELATION_TYPE,
 )
 
-##__________________________________________________________________||
 QEURY = (
     """
 {
   allProductRelationTypes {
    ...fragmentProductRelationTypeConnection
   }
 }
@@ -20,54 +18,64 @@
 )
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
-        {"query": MUTATION_DELETE_PRODUCT_RELATION_TYPES, "variables": {"typeId": 3}},
+        {
+            "query": MUTATION_UPDATE_PRODUCT_RELATION_TYPE,
+            "variables": {
+                "typeId": 1,
+                "input": {
+                    "indefArticle": "an",
+                    "singular": "mmap",
+                    "plural": "mmaps",
+                },
+            },
+        },
         {"query": QEURY},
-        id="delete",
+        id="update",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
-        {"query": MUTATION_DELETE_PRODUCT_RELATION_TYPES, "variables": {"typeId": 512}},
+        {
+            "query": MUTATION_UPDATE_PRODUCT_RELATION_TYPE,
+            "variables": {
+                "typeId": 1,
+                "input": {
+                    "name": "mmap",
+                },
+            },
+        },
         {"query": QEURY},
-        id="error-nonexistent",
-    ),
-    pytest.param(
-        {"query": MUTATION_DELETE_PRODUCT_RELATION_TYPES, "variables": {"typeId": 1}},
-        {"query": QEURY},
-        id="error-unempty",
+        id="error-immutable-field",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_error(
@@ -80,10 +88,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_type/conftest.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_type/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-import pytest
-
 import datetime
 
+import pytest
+
 from acondbs import ops
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app_users):
-
     y = app_users
 
     with y.app_context():
-
         ops.create_field(
             field_id=1,
             name="contact",
             type_=ops.FieldType.UnicodeText,
         )
         ops.create_field(
             field_id=2,
@@ -38,15 +35,14 @@
             name="field_five",
             type_=ops.FieldType.UnicodeText,
         )
 
         ops.commit()
 
     with y.app_context():
-
         ops.create_product_type(
             type_id=1,
             name="map",
             order=2,
             indef_article="a",
             singular="map",
             plural="maps",
@@ -80,10 +76,7 @@
             type_id=1,
             name="map3",
             attributes={3: datetime.date(2020, 3, 3)},
         )
         ops.commit()
 
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_type/test_create_product_type.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_type/test_create_product_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import pytest
 
 from ....funcs import assert_mutation
-
 from ...gql import MUTATION_CREATE_PRODUCT_TYPE, QUERY_ALL_PRODUCT_TYPES
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_CREATE_PRODUCT_TYPE,
             "variables": {
                 "input": {
                     "name": "compass",
@@ -86,29 +84,27 @@
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_CREATE_PRODUCT_TYPE,
             "variables": {
                 "input": {
                     "name": "map",
@@ -156,10 +152,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_type/test_delete_product_type.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_type/test_delete_product_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
 from ....funcs import assert_mutation
-
 from ...gql import MUTATION_DELETE_PRODUCT_TYPE
 
 QEURY = """
 {
   allProductTypes {
     edges {
       node {
@@ -18,44 +17,41 @@
 """
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": MUTATION_DELETE_PRODUCT_TYPE, "variables": {"typeId": 2}},
         {"query": QEURY},
         id="delete",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": MUTATION_DELETE_PRODUCT_TYPE, "variables": {"typeId": 12}},
         {"query": QEURY},
         id="error-nonexistent",
     ),
     pytest.param(
@@ -78,10 +74,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/mutation/product_type/test_update_product_type.py` & `acondbs-0.4.4/tests/schema/product/mutation/product_type/test_update_product_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 import pytest
 
 from ....funcs import assert_mutation
-
-from ...gql import (
-    MUTATION_UPDATE_PRODUCT_TYPE,
-    QUERY_ALL_PRODUCT_TYPES,
-)
-
+from ...gql import MUTATION_UPDATE_PRODUCT_TYPE, QUERY_ALL_PRODUCT_TYPES
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_UPDATE_PRODUCT_TYPE,
             "variables": {
                 "typeId": 1,
                 "input": {
@@ -75,29 +69,27 @@
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_UPDATE_PRODUCT_TYPE,
             "variables": {
                 "typeId": 5,
                 "input": {
@@ -128,10 +120,7 @@
         data_mutation,
         HEADERS,
         data_query,
         HEADERS,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_product.py` & `acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_product.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,212 +1,140 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_schema[deep] 1'] = {
     'data': {
         'product': {
-            'attributesBoolean': {
-                'edges': [
-                ]
-            },
+            'attributesBoolean': {'edges': []},
             'attributesDate': {
                 'edges': [
                     {
                         'node': {
-                            'field': {
-                                'name': 'date_produced',
-                                'type_': 'DATE'
-                            },
+                            'field': {'name': 'date_produced', 'type_': 'DATE'},
                             'typeFieldAssociation': {
-                                'field': {
-                                    'name': 'date_produced',
-                                    'type_': 'DATE'
-                                }
+                                'field': {'name': 'date_produced', 'type_': 'DATE'}
                             },
-                            'value': '2020-02-01'
+                            'value': '2020-02-01',
                         }
                     }
                 ]
             },
-            'attributesDateTime': {
-                'edges': [
-                ]
-            },
-            'attributesFloat': {
-                'edges': [
-                ]
-            },
-            'attributesInteger': {
-                'edges': [
-                ]
-            },
-            'attributesTime': {
-                'edges': [
-                ]
-            },
+            'attributesDateTime': {'edges': []},
+            'attributesFloat': {'edges': []},
+            'attributesInteger': {'edges': []},
+            'attributesTime': {'edges': []},
             'attributesUnicodeText': {
                 'edges': [
                     {
                         'node': {
-                            'field': {
-                                'name': 'contact',
-                                'type_': 'UNICODE_TEXT'
-                            },
+                            'field': {'name': 'contact', 'type_': 'UNICODE_TEXT'},
                             'typeFieldAssociation': {
-                                'field': {
-                                    'name': 'contact',
-                                    'type_': 'UNICODE_TEXT'
-                                }
+                                'field': {'name': 'contact', 'type_': 'UNICODE_TEXT'}
                             },
-                            'value': None
+                            'value': None,
                         }
                     },
                     {
                         'node': {
-                            'field': {
-                                'name': 'produced_by',
-                                'type_': 'UNICODE_TEXT'
-                            },
+                            'field': {'name': 'produced_by', 'type_': 'UNICODE_TEXT'},
                             'typeFieldAssociation': {
                                 'field': {
                                     'name': 'produced_by',
-                                    'type_': 'UNICODE_TEXT'
+                                    'type_': 'UNICODE_TEXT',
                                 }
                             },
-                            'value': None
+                            'value': None,
                         }
-                    }
+                    },
                 ]
             },
             'name': 'map1',
             'note': None,
             'paths': {
                 'edges': [
                     {
                         'node': {
                             'note': None,
                             'path': 'site2:/another/way/map1',
-                            'pathId': '1'
+                            'pathId': '1',
                         }
                     },
                     {
                         'node': {
                             'note': 'sample comment',
                             'path': 'site1:/path/to/map1',
-                            'pathId': '8'
+                            'pathId': '8',
                         }
-                    }
+                    },
                 ]
             },
             'postingGitHubUser': None,
             'productId': '1',
             'relations': {
                 'edges': [
                     {
                         'node': {
                             'other': {
                                 'name': 'beam1',
                                 'productId': '4',
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'beam',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'beam', 'typeId': '2'},
                             },
                             'otherProductId': 4,
                             'relationId': '1',
                             'reverse': {
                                 'relationId': '2',
                                 'typeId': 1,
-                                'type_': {
-                                    'name': 'parent',
-                                    'typeId': '1'
-                                }
+                                'type_': {'name': 'parent', 'typeId': '1'},
                             },
                             'reverseRelationId': 2,
                             'typeId': 2,
-                            'type_': {
-                                'name': 'child',
-                                'typeId': '2'
-                            }
+                            'type_': {'name': 'child', 'typeId': '2'},
                         }
                     },
                     {
                         'node': {
                             'other': {
                                 'name': 'beam2',
                                 'productId': '5',
                                 'typeId': 2,
-                                'type_': {
-                                    'name': 'beam',
-                                    'typeId': '2'
-                                }
+                                'type_': {'name': 'beam', 'typeId': '2'},
                             },
                             'otherProductId': 5,
                             'relationId': '3',
                             'reverse': {
                                 'relationId': '4',
                                 'typeId': 1,
-                                'type_': {
-                                    'name': 'parent',
-                                    'typeId': '1'
-                                }
+                                'type_': {'name': 'parent', 'typeId': '1'},
                             },
                             'reverseRelationId': 4,
                             'typeId': 2,
-                            'type_': {
-                                'name': 'child',
-                                'typeId': '2'
-                            }
+                            'type_': {'name': 'child', 'typeId': '2'},
                         }
-                    }
+                    },
                 ]
             },
             'timePosted': '2021-01-04T14:32:20',
             'timeUpdated': None,
             'typeId': 1,
-            'type_': {
-                'name': 'map',
-                'typeId': '1'
-            },
-            'updatingGitHubUser': None
+            'type_': {'name': 'map', 'typeId': '1'},
+            'updatingGitHubUser': None,
         }
     }
 }
 
-snapshots['test_schema[product_id-name-nonexistent] 1'] = {
-    'data': {
-        'product': None
-    }
-}
+snapshots['test_schema[product_id-name-nonexistent] 1'] = {'data': {'product': None}}
 
 snapshots['test_schema[product_id-name] 1'] = {
-    'data': {
-        'product': {
-            'name': 'map1',
-            'productId': '1',
-            'typeId': 1
-        }
-    }
+    'data': {'product': {'name': 'map1', 'productId': '1', 'typeId': 1}}
 }
 
-snapshots['test_schema[product_id-nonexistent] 1'] = {
-    'data': {
-        'product': None
-    }
-}
+snapshots['test_schema[product_id-nonexistent] 1'] = {'data': {'product': None}}
 
 snapshots['test_schema[type_id-name] 1'] = {
-    'data': {
-        'product': {
-            'name': 'map1',
-            'productId': '1',
-            'typeId': 1
-        }
-    }
+    'data': {'product': {'name': 'map1', 'productId': '1', 'typeId': 1}}
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_product_relation.py` & `acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_product_relation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,21 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema[type_id-nonexistent] 1'] = {
-    'data': {
-        'productRelation': None
-    }
-}
+snapshots['test_schema[type_id-nonexistent] 1'] = {'data': {'productRelation': None}}
 
 snapshots['test_schema[type_id] 1'] = {
     'data': {
         'productRelation': {
-            'other': {
-                'name': 'beam1',
-                'productId': '4'
-            },
+            'other': {'name': 'beam1', 'productId': '4'},
             'relationId': '1',
-            'reverse': {
-                'relationId': '2'
-            },
-            'self_': {
-                'name': 'map1',
-                'productId': '1'
-            },
-            'type_': {
-                'name': 'child',
-                'typeId': '2'
-            }
+            'reverse': {'relationId': '2'},
+            'self_': {'name': 'map1', 'productId': '1'},
+            'type_': {'name': 'child', 'typeId': '2'},
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/query/snapshots/snap_test_product_relation_type.py` & `acondbs-0.4.4/tests/schema/product/query/snapshots/snap_test_all_product_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,182 +1,114 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
-snapshots['test_schema[name] 1'] = {
-    'data': {
-        'productRelationType': {
-            'indefArticle': 'a',
-            'name': 'parent',
-            'plural': 'parents',
-            'relations': {
-                'edges': [
-                    {
-                        'node': {
-                            'other': {
-                                'name': 'map1',
-                                'productId': '1'
-                            },
-                            'self_': {
-                                'name': 'beam1',
-                                'productId': '4'
-                            }
-                        }
-                    },
-                    {
-                        'node': {
-                            'other': {
-                                'name': 'map1',
-                                'productId': '1'
-                            },
-                            'self_': {
-                                'name': 'beam2',
-                                'productId': '5'
-                            }
-                        }
-                    },
-                    {
-                        'node': {
-                            'other': {
-                                'name': 'beam1',
-                                'productId': '4'
-                            },
-                            'self_': {
-                                'name': 'beam2',
-                                'productId': '5'
-                            }
-                        }
-                    }
-                ]
-            },
-            'reverse': {
-                'name': 'child',
-                'typeId': '2'
-            },
-            'singular': 'parent',
-            'typeId': '1'
-        }
-    }
-}
-
-snapshots['test_schema[type_id-and-name-nonexistent)] 1'] = {
-    'data': {
-        'productRelationType': None
-    }
-}
-
-snapshots['test_schema[type_id-and-name] 1'] = {
+snapshots['test_schema[sort-order] 1'] = {
     'data': {
-        'productRelationType': {
-            'indefArticle': 'a',
-            'name': 'parent',
-            'plural': 'parents',
-            'relations': {
-                'edges': [
-                    {
-                        'node': {
-                            'other': {
-                                'name': 'map1',
-                                'productId': '1'
-                            },
-                            'self_': {
-                                'name': 'beam1',
-                                'productId': '4'
-                            }
-                        }
-                    },
-                    {
-                        'node': {
-                            'other': {
-                                'name': 'map1',
-                                'productId': '1'
-                            },
-                            'self_': {
-                                'name': 'beam2',
-                                'productId': '5'
-                            }
-                        }
-                    },
-                    {
-                        'node': {
-                            'other': {
-                                'name': 'beam1',
-                                'productId': '4'
-                            },
-                            'self_': {
-                                'name': 'beam2',
-                                'productId': '5'
-                            }
-                        }
+        'allProductTypes': {
+            'edges': [
+                {
+                    'node': {
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'beam'},
+                                    }
+                                },
+                            ]
+                        },
+                        'icon': 'mdi-spotlight-beam',
+                        'indefArticle': 'a',
+                        'name': 'beam',
+                        'order': 1,
+                        'plural': 'beams',
+                        'products': {
+                            'edges': [
+                                {'node': {'name': 'beam1'}},
+                                {'node': {'name': 'beam2'}},
+                            ]
+                        },
+                        'singular': 'beam',
+                        'typeId': '2',
                     }
-                ]
-            },
-            'reverse': {
-                'name': 'child',
-                'typeId': '2'
-            },
-            'singular': 'parent',
-            'typeId': '1'
-        }
-    }
-}
-
-snapshots['test_schema[type_id] 1'] = {
-    'data': {
-        'productRelationType': {
-            'indefArticle': 'a',
-            'name': 'parent',
-            'plural': 'parents',
-            'relations': {
-                'edges': [
-                    {
-                        'node': {
-                            'other': {
-                                'name': 'map1',
-                                'productId': '1'
-                            },
-                            'self_': {
-                                'name': 'beam1',
-                                'productId': '4'
-                            }
-                        }
-                    },
-                    {
-                        'node': {
-                            'other': {
-                                'name': 'map1',
-                                'productId': '1'
-                            },
-                            'self_': {
-                                'name': 'beam2',
-                                'productId': '5'
-                            }
-                        }
-                    },
-                    {
-                        'node': {
-                            'other': {
-                                'name': 'beam1',
-                                'productId': '4'
-                            },
-                            'self_': {
-                                'name': 'beam2',
-                                'productId': '5'
-                            }
-                        }
+                },
+                {
+                    'node': {
+                        'fields': {
+                            'edges': [
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'contact',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'produced_by',
+                                            'type_': 'UNICODE_TEXT',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                                {
+                                    'node': {
+                                        'field': {
+                                            'name': 'date_produced',
+                                            'type_': 'DATE',
+                                        },
+                                        'type_': {'name': 'map'},
+                                    }
+                                },
+                            ]
+                        },
+                        'icon': 'mdi-map',
+                        'indefArticle': 'a',
+                        'name': 'map',
+                        'order': 2,
+                        'plural': 'maps',
+                        'products': {
+                            'edges': [
+                                {'node': {'name': 'map1'}},
+                                {'node': {'name': 'map2'}},
+                                {'node': {'name': 'map3'}},
+                            ]
+                        },
+                        'singular': 'map',
+                        'typeId': '1',
                     }
-                ]
-            },
-            'reverse': {
-                'name': 'child',
-                'typeId': '2'
-            },
-            'singular': 'parent',
-            'typeId': '1'
+                },
+            ],
+            'totalCount': 2,
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/product/query/test_all_product_relation_types.py` & `acondbs-0.4.4/tests/schema/product/query/test_field.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import pytest
 
 from ...funcs import assert_query
-
-from ..gql import (
-    QUERY_ALL_PRODUCT_RELATION_TYPES,
-    QUERY_ALL_PRODUCT_RELATION_TYPES_TOTAL_COUNT,
-)
+from ..gql import QUERY_FIELD
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
-        {"query": QUERY_ALL_PRODUCT_RELATION_TYPES},
-        id="query",
+        {
+            #
+            "query": QUERY_FIELD,
+            "variables": {"fieldId": 1},
+        },
+        id="by-field-id",
     ),
     pytest.param(
-        {"query": QUERY_ALL_PRODUCT_RELATION_TYPES_TOTAL_COUNT},
-        id="total-count",
+        {
+            #
+            "query": QUERY_FIELD,
+            "variables": {"name": "contact"},
+        },
+        id="by-name",
     ),
 ]
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize("data", params)
 @pytest.mark.asyncio
 async def test_schema(app, snapshot, data):
     await assert_query(app, snapshot, data, HEADERS)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/query/test_all_products.py` & `acondbs-0.4.4/tests/schema/product/query/test_all_products.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import pytest
 
 from ...funcs import assert_query
-
 from ..gql import (
     QUERY_ALL_PRODUCTS,
     QUERY_ALL_PRODUCTS_SHALLOW,
     QUERY_ALL_PRODUCTS_TOTAL_COUNT,
 )
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             #
             "query": QUERY_ALL_PRODUCTS
         },
         id="deep",
@@ -99,15 +97,11 @@
             },
         },
         id="total-count",
     ),
 ]
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize("data", params)
 @pytest.mark.asyncio
 async def test_schema(app, snapshot, data):
     await assert_query(app, snapshot, data, HEADERS)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/query/test_field.py` & `acondbs-0.4.4/tests/schema/product/query/test_product_relation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import pytest
 
 from ...funcs import assert_query
-
-from ..gql import QUERY_FIELD
+from ..gql import QUERY_PRODUCT_RELATION
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             #
-            "query": QUERY_FIELD,
-            "variables": {"fieldId": 1},
+            "query": QUERY_PRODUCT_RELATION,
+            "variables": {"relationId": 1},
         },
-        id="by-field-id",
+        id="type_id",
     ),
     pytest.param(
         {
             #
-            "query": QUERY_FIELD,
-            "variables": {"name": "contact"},
+            "query": QUERY_PRODUCT_RELATION,
+            "variables": {"relationId": 222},
         },
-        id="by-name",
+        id="type_id-nonexistent",
     ),
 ]
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize("data", params)
 @pytest.mark.asyncio
 async def test_schema(app, snapshot, data):
     await assert_query(app, snapshot, data, HEADERS)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/query/test_product.py` & `acondbs-0.4.4/tests/schema/product/query/test_product.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import pytest
 
 from ...funcs import assert_query
-
 from ..gql import QUERY_PRODUCT, QUERY_PRODUCT_SHALLOW
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             #
             "query": QUERY_PRODUCT,
             "variables": {"productId": 1},
         },
@@ -50,15 +48,11 @@
             "variables": {"productId": 1, "name": "map2"},
         },
         id="product_id-name-nonexistent",
     ),
 ]
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize("data", params)
 @pytest.mark.asyncio
 async def test_schema(app, snapshot, data):
     await assert_query(app, snapshot, data, HEADERS)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/product/query/test_product_type.py` & `acondbs-0.4.4/tests/schema/product/query/test_product_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
 from ...funcs import assert_query
-
 from ..gql import QUERY_PRODUCT_TYPE
 
 HEADERS = {
     "Authorization": "Bearer 0fb8c9e16d6f7c4961c4c49212bf197d79f14080"  # dojocat
 }
 
 
@@ -27,15 +26,14 @@
       }
     }
   }
 }
 """
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             #
             "query": QUERY_PRODUCT_TYPE,
             "variables": {"typeId": 1},
         },
@@ -71,15 +69,11 @@
             "query": QUERY_PRODUCT_TYPE_SORT_PRODUCTS,
         },
         id="type_id-sort-products",
     ),
 ]
 
 
-##__________________________________________________________________||
 @pytest.mark.parametrize("data", params)
 @pytest.mark.asyncio
 async def test_schema(app, snapshot, data):
     await assert_query(app, snapshot, data, HEADERS)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/snapshots/snap_test_error.py` & `acondbs-0.4.4/tests/schema/snapshots/snap_test_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_schema[one] 1'] = {
     'data': {
         'allLogs': {
             'edges': [
                 {
@@ -49,15 +48,15 @@
                       "column": 3
                     }
                   ]
                 }
               ]
             }
 ''',
-                        'time': '2021-01-04T14:32:20'
+                        'time': '2021-01-04T14:32:20',
                     }
                 }
             ],
-            'totalCount': 1
+            'totalCount': 1,
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/test_error.py` & `acondbs-0.4.4/tests/schema/test_error.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import pytest
 
 from .funcs import assert_mutation
-
 from .misc.gql import QUERY_ALL_LOGS
 
-##__________________________________________________________________||
 QUERY = """
 {
   noSuchField
 }
 """.strip()
 
 HEADERS = {
@@ -16,47 +14,39 @@
 }
 
 HEADERS_QUERY = {
     "Authorization": "Bearer 90b2ee5fed25506df04fd37343bb68d1803dd97f"  # octocat
 }
 
 
-##__________________________________________________________________||
 @pytest.fixture
 def app(app_users):
     y = app_users
     yield y
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": QUERY,
             "variables": {"var1": 100},
         },
         {"query": QUERY_ALL_LOGS},
         id="one",
     ),
 ]
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
-async def test_schema(
-    app, snapshot, data_mutation, data_query, mock_request_backup_db
-):
-
+async def test_schema(app, snapshot, data_mutation, data_query, mock_request_backup_db):
     success = False
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS,
         data_query,
         HEADERS_QUERY,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/test_schema.py` & `acondbs-0.4.4/tests/schema/test_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,14 @@
       }
     }
   }
 }
 '''
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {"query": QUERY},
         {"Authorization": "Bearer 90b2ee5fed25506df04fd37343bb68d1803dd97f"},
         id="admin",
     ),
     pytest.param(
@@ -57,10 +56,7 @@
 ]
 
 
 @pytest.mark.parametrize("data, headers", params)
 @pytest.mark.asyncio
 async def test_schema(app_users, snapshot, data, headers):
     await assert_query(app_users, snapshot, data, headers)
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/test_version.py` & `acondbs-0.4.4/tests/schema/test_version.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import pytest
-
-from async_asgi_testclient import TestClient
 from a2wsgi import WSGIMiddleware
+from async_asgi_testclient import TestClient
 
 import acondbs
 
 QUERY = "{ version }"
 
 
-##__________________________________________________________________||
 @pytest.mark.asyncio
 async def test_schema(app):
-
     app = WSGIMiddleware(app)  # convert a wsgi app to an asgi app
 
     headers = {
         "Content-Type:": "application/json",
         "Authorization": "Bearer token123",  # octocat
     }
 
@@ -23,10 +20,7 @@
     expected = {"data": {"version": acondbs.__version__}}
 
     async with TestClient(app) as client:
         resp = await client.post("/graphql", json=data, headers=headers)
 
     assert resp.status_code == 200
     assert resp.json() == expected
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/web/mutation/web_config/conftest.py` & `acondbs-0.4.4/tests/schema/web/query/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import json
 
 import pytest
 
 from acondbs import ops
 
 
-##__________________________________________________________________||
 @pytest.fixture
-def app(app_users):
-    y = app_users
+def app(app_empty):
+    y = app_empty
 
     config_json = json.dumps(
         {
             "headTitle": "Head Title",
             "toolbarTitle": "Toolbar Title",
             "devtoolLoadingstate": True,
             "productCreationDialog": False,
@@ -23,10 +22,7 @@
     )
 
     with y.app_context():
         ops.save_web_config(json=config_json)
         ops.commit()
 
     yield y
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/tests/schema/web/mutation/web_config/snapshots/snap_test_save.py` & `acondbs-0.4.4/tests/schema/web/mutation/web_config/snapshots/snap_test_save.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 # snapshottest: v1 - https://goo.gl/zC4yUc
 from __future__ import unicode_literals
 
 from snapshottest import Snapshot
 
-
 snapshots = Snapshot()
 
 snapshots['test_schema_success[one] 1'] = {
     'data': {
         'saveWebConfig': {
             'ok': True,
             'webConfig': {
@@ -16,16 +15,16 @@
                 'json': '''{
   "headTitle": "Saved Head Title",
   "toolbarTitle": "Saved Toolbar Title",
   "devtoolLoadingstate": false,
   "productCreationDialog": false,
   "productUpdateDialog": false,
   "productDeletionDialog": false
-}'''
-            }
+}''',
+            },
         }
     }
 }
 
 snapshots['test_schema_success[one] 2'] = {
     'data': {
         'webConfig': {
@@ -33,11 +32,11 @@
             'json': '''{
   "headTitle": "Saved Head Title",
   "toolbarTitle": "Saved Toolbar Title",
   "devtoolLoadingstate": false,
   "productCreationDialog": false,
   "productUpdateDialog": false,
   "productDeletionDialog": false
-}'''
+}''',
         }
     }
 }
```

### Comparing `acondbs-0.4.3/tests/schema/web/mutation/web_config/test_save.py` & `acondbs-0.4.4/tests/schema/web/mutation/web_config/test_save.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 
 import pytest
 
 from ....funcs import assert_mutation
-
 from ...gql import MUTATION_SAVE_WEB_CONFIG, QUERY_WEB_CONFIG
 
 HEADERS_MUTATION = {
     "Authorization": "Bearer 90b2ee5fed25506df04fd37343bb68d1803dd97f"  # octocat
 }
 
 HEADERS_QUERY = {}
@@ -21,15 +20,14 @@
         "productUpdateDialog": False,
         "productDeletionDialog": False,
     },
     indent=2,
 )
 
 
-##__________________________________________________________________||
 params = [
     pytest.param(
         {
             "query": MUTATION_SAVE_WEB_CONFIG,
             "variables": {
                 "json": CONFIG_JSON,
             },
@@ -41,22 +39,18 @@
 
 
 @pytest.mark.parametrize("data_mutation, data_query", params)
 @pytest.mark.asyncio
 async def test_schema_success(
     app, snapshot, data_mutation, data_query, mock_request_backup_db
 ):
-
     success = True
     await assert_mutation(
         app,
         snapshot,
         data_mutation,
         HEADERS_MUTATION,
         data_query,
         HEADERS_QUERY,
         mock_request_backup_db,
         success,
     )
-
-
-##__________________________________________________________________||
```

### Comparing `acondbs-0.4.3/versioneer.py` & `acondbs-0.4.4/versioneer.py`

 * *Files identical despite different names*

