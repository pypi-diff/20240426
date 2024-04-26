# Comparing `tmp/django_quotes-0.4.2.tar.gz` & `tmp/django_quotes-0.5.0.tar.gz`

## Comparing `django_quotes-0.4.2.tar` & `django_quotes-0.5.0.tar`

### file list

```diff
@@ -1,67 +1,70 @@
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/__init__.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/admin.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/apps.py
--rw-r--r--   0        0        0    21793 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/py.typed
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/receivers.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/rules.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/signals.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/urls.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/utils.py
--rw-r--r--   0        0        0    12651 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/views.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/api/__init__.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/api/serializers.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/api/views.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/management/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/management/commands/__init__.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/management/commands/makemarkov.py
--rw-r--r--   0        0        0    13189 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0001_squashed_0005_alter_groupmarkovmodel_created_and_more.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0003_alter_source_slug_alter_sourcegroup_slug.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0004_quote_pub_date.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0005_alter_groupmarkovmodel_created_and_more.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0006_alter_source_description_rendered.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0007_source_text_model_sourcegroup_text_model.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0008_auto_20240404_1952.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model_squashed_0012_remove_sourcemarkovmodel_source_and_more.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0010_alter_source_text_model_alter_sourcegroup_text_model.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0011_alter_source_text_model_alter_sourcegroup_text_model.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0012_remove_sourcemarkovmodel_source_and_more.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/0013_remove_quote_quote_rendered_and_more.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/static/.gitkeep
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/base.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/base.html
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/group_create.html
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/group_delete.html
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/group_detail.html
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/group_list.html
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/group_update.html
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/quote_create.html
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/quote_delete.html
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/quote_detail.html
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/quote_list.html
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/quote_update.html
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/source_create.html
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/source_delete.html
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/source_detail.html
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/source_list.html
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 django_quotes-0.4.2/src/django_quotes/templates/quotes/source_update.html
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/api_router.py
--rw-r--r--   0        0        0    10257 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/django_settings.py
--rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/test_api.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/test_docs.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/test_management.py
--rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/test_models.py
--rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/test_signals.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/test_utils.py
--rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/test_views.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/urls.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/factories/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 django_quotes-0.4.2/tests/factories/users.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 django_quotes-0.4.2/.gitignore
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 django_quotes-0.4.2/LICENSE
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 django_quotes-0.4.2/README.md
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 django_quotes-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 django_quotes-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/__init__.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/admin.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/apps.py
+-rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/py.typed
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/receivers.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/rules.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/signals.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/tasks.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/urls.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/utils.py
+-rw-r--r--   0        0        0    12651 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/views.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/api/__init__.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/api/serializers.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/api/views.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/management/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/management/commands/__init__.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/management/commands/makemarkov.py
+-rw-r--r--   0        0        0    13189 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0001_squashed_0005_alter_groupmarkovmodel_created_and_more.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0003_alter_source_slug_alter_sourcegroup_slug.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0004_quote_pub_date.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0005_alter_groupmarkovmodel_created_and_more.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0006_alter_source_description_rendered.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0007_source_text_model_sourcegroup_text_model.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0008_auto_20240404_1952.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model_squashed_0012_remove_sourcemarkovmodel_source_and_more.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0010_alter_source_text_model_alter_sourcegroup_text_model.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0011_alter_source_text_model_alter_sourcegroup_text_model.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0012_remove_sourcemarkovmodel_source_and_more.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0013_remove_quote_quote_rendered_and_more.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0014_alter_source_text_model_alter_sourcegroup_text_model.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/static/.gitkeep
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/base.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/base.html
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/group_create.html
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/group_delete.html
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/group_detail.html
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/group_list.html
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/group_update.html
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_create.html
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_delete.html
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_detail.html
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_list.html
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_update.html
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/source_create.html
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/source_delete.html
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/source_detail.html
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/source_list.html
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/source_update.html
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/api_router.py
+-rw-r--r--   0        0        0    10257 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/django_settings.py
+-rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_api.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_docs.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_management.py
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_models.py
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_signals.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_tasks.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_utils.py
+-rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_views.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/urls.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/factories/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/factories/users.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 django_quotes-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 django_quotes-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 django_quotes-0.5.0/README.md
+-rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 django_quotes-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 django_quotes-0.5.0/PKG-INFO
```

### Comparing `django_quotes-0.4.2/src/django_quotes/admin.py` & `django_quotes-0.5.0/src/django_quotes/admin.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/apps.py` & `django_quotes-0.5.0/src/django_quotes/apps.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/models.py` & `django_quotes-0.5.0/src/django_quotes/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,32 @@
 # SPDX-License-Identifier: BSD-3-Clause
 
 from __future__ import annotations
 
 import random
 from typing import TYPE_CHECKING, Any
 
+import markovify
 import rules
 from asgiref.sync import async_to_sync
 
 if TYPE_CHECKING:
     from django.db.models.manager import RelatedManager
 from django.conf import settings
 from django.db import models
+from django.db.models import Count
 from django.utils import timezone
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 from loguru import logger
 from markdown import markdown
 from rules.contrib.models import RulesModelBase, RulesModelMixin
 
 from django_markov.models import MarkovTextModel
+from django_markov.text_models import POSifiedText
 from django_quotes.rules import (  # is_character_owner,; is_group_owner_and_authenticated,
     is_owner,
     is_owner_or_public,
 )
 from django_quotes.signals import quote_random_retrieved
 from django_quotes.utils import generate_unique_slug_for_model
 
@@ -38,14 +41,22 @@
 if hasattr(settings, "MAX_QUOTES_FOR_RANDOM_SET"):  # pragma: nocover
     MAX_QUOTES_FOR_RANDOM_SET = settings.MAX_QUOTES_FOR_RANDOM_SET
 
 if hasattr(settings, "MAX_QUOTES_FOR_RANDOM_GROUP_SET"):  # pragma: nocover
     MAX_QUOTES_FOR_RANDOM_GROUP_SET = settings.MAX_QUOTES_FOR_RANDOM_GROUP_SET
 
 
+class QuoteCorpusError(Exception):
+    """
+    An exception raised when a quote corpus fails to generate.
+    """
+
+    pass
+
+
 class AbstractOwnerModel(models.Model):
     """
     Abstract model for representing an entity owned by a user with toggles for either allowing submissions for it
     and public access. Defaults to completely private by default.
 
     Attributes:
         public (bool): is this object public to any authenticated user? Default: False
@@ -84,14 +95,15 @@
         id (int): Database primary key for the object.
         name (str): Human readable string to name the group. This will be converted to a slug prefix.
         description (str): A description of the group for convenience. Markdown can be used here for styling.
         owner (User): The user that created the group and therefore owns it.
         public (bool): Is this group public or private. Defaults to False.
         allow_submissions (bool): Allow other users to submit characters to this. Not yet implemented.
         slug (str): A unique slug to represent this group. Generated automatically from name.
+        text_model (MarkovTextModel | None): The current text model.
         created (datetime): When this object was first created. Auto-generated.
         modified (datetime): Last time this object was modified. Auto-generated.
 
     """
 
     if TYPE_CHECKING:
         source_set: RelatedManager[Source]
@@ -113,30 +125,30 @@
         max_length=70,
         editable=False,
         blank=True,
         help_text=_("Unique slug for this group."),
     )
     text_model = models.OneToOneField(
         MarkovTextModel,
-        on_delete=models.CASCADE,
+        on_delete=models.SET_NULL,
         null=True,
         blank=True,
         help_text=_("The markov model for this group."),
     )
 
     class Meta:
         rules_permissions = {
             "add": rules.is_authenticated,
             "read": is_owner_or_public,
             "edit": is_owner,
             "delete": is_owner,
         }
         ordering = ["name"]
 
-    def __str__(self):  # pragma: nocover
+    def __str__(self):  # no cov
         return self.name
 
     def save(self, *args, **kwargs):
         """Save and create slug if missing."""
         if not self.slug:  # Once this slug is set, it does not change except through devil pacts
             logger.debug("Group is being saved and a slug was provided.")
             self.slug = generate_unique_slug_for_model(model_class=type(self), text=self.name)
@@ -152,15 +164,15 @@
             try:
                 del self.__dict__[prop]
             except KeyError:  # pragma: nocover
                 pass
 
     @property
     def description_rendered(self) -> str:
-        """Return the markdown rendered version of the string."""
+        """Return the markdown rendered version of the description."""
         if self.description is None or self.description == "":
             return ""
         return markdown(self.description)
 
     @cached_property
     def total_sources(self) -> int:
         """Total number of sources for the group."""
@@ -183,25 +195,51 @@
             self.markov_sources > 0
             and self.text_model is not None
             and Quote.objects.filter(source__in=self.source_set.filter(allow_markov=True)).count() > 10  # noqa:PLR2004
         ):
             return True
         return False
 
-    async def aupdate_markov_model(self) -> None:
-        """Updates the related MarkovTextModel."""
+    async def aupdate_markov_model(self, additional_model: MarkovTextModel | None = None) -> None:
+        """Updates the related MarkovTextModel.
+
+        Args:
+            additional_model (MarkovTextModel | None): An additional model to include in the combination. Useful for
+                pre_save signals for a source that is newly enabling allow_markov.
+        """
         if self.text_model is not None:
-            markov_sources = self.source_set.filter(allow_markov=True)
+            sources = (
+                self.source_set.select_related("text_model")
+                .prefetch_related("quote_set")
+                .filter(allow_markov=True, text_model__data__isnull=False)
+            )
+            markov_sources = sources.annotate(num_quotes=Count("quote")).filter(num_quotes__gt=10)
+            models_to_combine = []
+            if additional_model is not None:
+                models_to_combine.append(additional_model)
             if await markov_sources.aexists():
-                quotes = Quote.objects.filter(source__in=markov_sources)
-                await self.text_model.aupdate_model_from_corpus(corpus_entries=[quote.quote async for quote in quotes])
+                models_to_combine += [source.text_model async for source in markov_sources]
+            if len(models_to_combine) > 0:
+                if len(models_to_combine) > 1:
+                    new_text_model, num_combined = await self.text_model.acombine_models(
+                        models_to_combine, mode="strict", return_type="text_model"
+                    )
+                    if not isinstance(new_text_model, POSifiedText):  # no cov
+                        msg = "Only an instance of POSifiedText is allowed when updating the SourceGroup text_model!"
+                        raise TypeError(msg)
+                    self.text_model.data = new_text_model.to_json()  # type: ignore
+                else:
+                    # There is a only a single source
+                    source = models_to_combine[0]
+                    self.text_model.data = source.data
+                await self.text_model.asave()
 
-    def update_markov_model(self) -> None:
+    def update_markov_model(self, additional_model: MarkovTextModel | None = None) -> None:
         """Updates the related MarkovTextModel."""
-        async_to_sync(self.aupdate_markov_model)()
+        async_to_sync(self.aupdate_markov_model)(additional_model=additional_model)
 
     def generate_markov_sentence(self, max_characters: int = 280, tries: int = 20) -> str | None:
         """
         Generate a markov sentence based on quotes from markov enabled characters for the group.
 
         Args:
             max_characters (int): Maximum characters allowed in the resulting sentence.
@@ -263,14 +301,15 @@
         group (SourceGroup): The parent ``SourceGroup``.
         slug (str): Slug made up of a generated version of the character name and the group slug prefix.
         description (str): Description for the character. Markdown can be used for styling.
         allow_markov (bool): Allow markov quotes to be requested from this character? Default False.
         owner (User): The user that created and owns this character.
         public (bool): Is the character public to other users? Defaults to False.
         allow_submissions (bool): Allow other users to submit quotes for this character? Defaults to False.
+        text_model (MarkovTextModel | None): The current text_model.
         created (datetime): When this object was first created. Auto-generated.
         modified (datetime): Last time this object was modified. Auto-generated.
 
     """
 
     if TYPE_CHECKING:
         quote_set: RelatedManager[Quote]
@@ -294,40 +333,40 @@
     group = models.ForeignKey(
         SourceGroup,
         on_delete=models.CASCADE,
         help_text=_("The group this character belongs to."),
     )
     text_model = models.OneToOneField(
         MarkovTextModel,
-        on_delete=models.CASCADE,
+        on_delete=models.SET_NULL,
         null=True,
         blank=True,
         help_text=_("The text model for this character."),
     )
 
     class Meta:
         rules_permissions = {
             "add": rules.is_authenticated,
             "read": is_owner_or_public,
             "edit": is_owner,
             "delete": is_owner,
         }
 
-    def __str__(self):  # pragma: nocover
+    def __str__(self):  # no cov
         return self.name
 
     def save(self, *args, **kwargs):
         """Save and create slug, if missing."""
         if not self.slug:
             self.slug = generate_unique_slug_for_model(type(self), text=f"{self.group.slug} {self.name}")
         super().save(*args, **kwargs)
 
     @property
     def description_rendered(self) -> str:
-        """Return the markdown rendered version of the string."""
+        """Return the markdown rendered version of the description."""
         if self.description is None or self.description == "":
             return ""
         return markdown(self.description)
 
     @property
     def markov_ready(self) -> bool:
         """
@@ -351,25 +390,65 @@
             return True
         return False
 
     async def aupdate_markov_model(self) -> None:
         """
         Process all quotes into the associated model.
         """
-        if self.allow_markov and self.text_model is not None:
-            await self.text_model.aupdate_model_from_corpus(
-                corpus_entries=[quote.quote async for quote in self.quote_set.all()], char_limit=0, store_compiled=False
+        if await self._amarkov_ready():
+            await self.text_model.aupdate_model_from_corpus(  # type: ignore
+                corpus_entries=[quote.quote async for quote in self.quote_set.all()],
+                char_limit=0,
+                store_compiled=False,
             )
 
     def update_markov_model(self) -> None:
         """
         Sync wrapper around `aupdate_markov_model`.
         """
         async_to_sync(self.aupdate_markov_model)()
 
+    async def aadd_new_quote_to_model(self, quote_to_add: Quote) -> None:
+        """Allows adding a new quote to the source's (and group's) text model without parsing the whole corpus.
+        Note that deleting or editing a quote will still require a full re-ingest of the corpus to remove old data.
+
+        Args:
+            quote_to_add (Quote): A quote to add to the source text model.
+        """
+        if self.allow_markov and await self.quote_set.acount() > 10 and self.text_model is not None:  # noqa: PLR2004
+            if not self.text_model.data:
+                await self.aupdate_markov_model()
+                await self.group.aupdate_markov_model()
+            else:
+                if self.group.text_model is None:  # no cov
+                    self.group.text_model = await MarkovTextModel.objects.acreate()
+                source_model = POSifiedText.from_json(self.text_model.data)
+                group_model = POSifiedText.from_json(self.group.text_model.data)
+                quote_model = POSifiedText(quote_to_add.quote)
+                try:
+                    combined_source_model = markovify.combine([source_model, quote_model])
+                    combined_group_model = markovify.combine([group_model, quote_model])
+                except ValueError as ve:
+                    msg = f"Unable to combine models: {ve}"
+                    raise QuoteCorpusError(msg) from ve
+                self.text_model.data = combined_source_model.to_json()  # type: ignore
+                self.group.text_model.data = combined_group_model.to_json()  # type: ignore
+                await self.text_model.asave()
+                await self.group.text_model.asave()
+
+    def add_new_quote_to_model(self, quote_to_add: Quote) -> None:
+        """Sync wrapper for `aadd_new_quote_to_model`.
+        Allows adding a new quote to the source's text model without parsing the whole corpus.
+        Note that deleting or editing a quote will still require a full re-ingest of the corpus to remove old data.
+
+        Args:
+            quote_to_add (Quote): A quote to add to the source text model.
+        """
+        async_to_sync(self.aadd_new_quote_to_model)(quote_to_add)
+
     def get_markov_sentence(self, max_characters: int | None = 280, tries: int = 20) -> str | None:
         """
         If valid, generate a markov sentence. If not, return None.
 
         Args:
             max_characters (int | None): Maximum number of characters allowed in
                 resulting sentence.
@@ -423,16 +502,17 @@
 class Quote(AbstractOwnerModel, RulesModelMixin, TimeStampedModel, metaclass=RulesModelBase):
     """
     A quote from a given source. A user must own the related source to add or delete a quote.
 
     Attributes:
         id (int): Database primary key for the object.
         quote (str): The quote text to use. You can use Markdown for styling. Must be <= 280 characters for tweets
-        citation (str): Optional description of quote source, e.g. episode number or book title.
-        citation_url (str): Optional accompanying URL for the citation.
+        citation (str | None): Optional description of quote source, e.g. episode number or book title.
+        citation_url (str | None): Optional accompanying URL for the citation.
+        pub_date (datetime| None): Date and time when the quote was published.
         source (Source): The source of this quote.
         owner (User): The user that created and owns this quote.
         created (datetime): When this object was first created. Auto-generated.
         modified (datetime): Last time this object was modified. Auto-generated.
 
     """
 
@@ -465,20 +545,20 @@
         rules_permissions = {
             # "add": is_character_owner,
             "read": is_owner_or_public,
             "edit": is_owner,
             "delete": is_owner,
         }
 
-    def __str__(self):  # pragma: nocover
+    def __str__(self):  # no cov
         return f"{self.source.name}: {self.quote}"
 
     @property
     def quote_rendered(self) -> str:
-        """Return the markdown rendered version of the string."""
+        """Return the markdown rendered version of the quote."""
         if self.quote is None or self.quote == "":
             return ""
         return markdown(self.quote)
 
 
 class QuoteStats(TimeStampedModel):
     """
@@ -496,15 +576,15 @@
         Quote,
         on_delete=models.CASCADE,
         related_name="stats",
         help_text=_("The Quote the stats related to."),
     )
     times_used = models.PositiveIntegerField(default=0, help_text=_("Times used for random quotes, etc."))
 
-    def __str__(self):  # pragma: nocover
+    def __str__(self):  # no cov
         return f"Stats for Quote {self.quote.id}"
 
 
 class GroupStats(TimeStampedModel):
     """
     An object for using to track usage stats for ``CharacterGroup``.
 
@@ -519,15 +599,15 @@
         default=0, help_text=_("Number of time child quotes have been requested.")
     )
     quotes_generated = models.PositiveIntegerField(
         default=0,
         help_text=_("Number of times markov generated quotes have been requested."),
     )
 
-    def __str__(self):  # pragma: nocover
+    def __str__(self):  # no cov
         return f"Stats for Group {self.group.name}"
 
 
 class SourceStats(TimeStampedModel):
     """
     An object for using to track usage stats for ``Character``.
 
@@ -542,9 +622,9 @@
         default=0, help_text=_("Number of time child quotes have been requested.")
     )
     quotes_generated = models.PositiveIntegerField(
         default=0,
         help_text=_("Number of times markov generated quotes have been requested."),
     )
 
-    def __str__(self):  # pragma: nocover
+    def __str__(self):  # no cov
         return f"Stats for Source {self.source.name}"
```

### Comparing `django_quotes-0.4.2/src/django_quotes/receivers.py` & `django_quotes-0.5.0/src/django_quotes/receivers.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # All rights reserved.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import transaction
 from django.db.models import F
-from django.db.models.signals import post_save, pre_save
+from django.db.models.signals import post_save, pre_delete, pre_save
 from django.dispatch import receiver
 
 from django_markov.models import MarkovTextModel, sentence_generated
 from django_quotes.models import (
     GroupStats,
     Quote,
     QuoteStats,
@@ -20,26 +20,18 @@
     SourceGroup,
     SourceStats,
 )
 from django_quotes.signals import quote_random_retrieved
 
 
 @receiver(pre_save, sender=SourceGroup)
-def initialize_group_markov_object(sender, instance, *args, **kwargs):
-    """
-    Creates the one-to-one object for the group markov model.
-    """
-    if not instance.text_model:
-        instance.text_model = MarkovTextModel.objects.create()
-
-
 @receiver(pre_save, sender=Source)
 def initialize_markov_object(sender, instance, *args, **kwargs):
     """
-    Creates the one-to-one object to accompany the source object.
+    Creates the one-to-one object for the group markov model.
     """
     if not instance.text_model:
         instance.text_model = MarkovTextModel.objects.create()
 
 
 @receiver(post_save, sender=SourceGroup)
 @receiver(post_save, sender=Source)
@@ -101,21 +93,26 @@
         group_stats.quotes_generated = F("quotes_generated") + 1
         group_stats.save()
         if source_stats is not None:
             source_stats.quotes_generated = F("quotes_generated") + 1
             source_stats.save()
 
 
-# @receiver(post_save, sender=Quote)
-# def update_markov_model_on_quote_change(sender, instance, created, *args, **kwargs):
-#     if instance.character.allow_markov:
-#         cmm = CharacterMarkovModel.objects.get(character=instance.character)
-#         cmm.generate_model_from_corpus()
-
-
 @receiver(pre_save, sender=Source)
 def update_markov_model_for_character_enabling_markov(sender, instance, *args, **kwargs):
+    """
+    When updating a source to allow_markov, trigger markov model updates.
+    """
     if instance.id and instance.allow_markov:
         old_version = Source.objects.get(id=instance.id)
         if not old_version.allow_markov:
             instance.update_markov_model()
-            instance.group.update_markov_model()
+            instance.text_model.refresh_from_db()
+            instance.group.update_markov_model(additional_model=instance.text_model)
+
+
+@receiver(pre_delete, sender=Source)
+@receiver(pre_delete, sender=SourceGroup)
+def delete_markov_models_before_orphaning(sender, instance, *args, **kwargs):
+    """When deleting a source or source group, ensure that its text_model is deleted first."""
+    if instance.text_model is not None:
+        instance.text_model.delete()
```

### Comparing `django_quotes-0.4.2/src/django_quotes/rules.py` & `django_quotes-0.5.0/src/django_quotes/rules.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/signals.py` & `django_quotes-0.5.0/src/django_quotes/signals.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/urls.py` & `django_quotes-0.5.0/src/django_quotes/urls.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/utils.py` & `django_quotes-0.5.0/src/django_quotes/utils.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/views.py` & `django_quotes-0.5.0/src/django_quotes/views.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/api/serializers.py` & `django_quotes-0.5.0/src/django_quotes/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/api/views.py` & `django_quotes-0.5.0/src/django_quotes/api/views.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/management/commands/makemarkov.py` & `django_quotes-0.5.0/src/django_quotes/management/commands/makemarkov.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0001_squashed_0005_alter_groupmarkovmodel_created_and_more.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0001_squashed_0005_alter_groupmarkovmodel_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0003_alter_source_slug_alter_sourcegroup_slug.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0003_alter_source_slug_alter_sourcegroup_slug.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0004_quote_pub_date.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0004_quote_pub_date.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0005_alter_groupmarkovmodel_created_and_more.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0005_alter_groupmarkovmodel_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0006_alter_source_description_rendered.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0006_alter_source_description_rendered.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0007_source_text_model_sourcegroup_text_model.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0007_source_text_model_sourcegroup_text_model.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0008_auto_20240404_1952.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0008_auto_20240404_1952.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model_squashed_0012_remove_sourcemarkovmodel_source_and_more.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model_squashed_0012_remove_sourcemarkovmodel_source_and_more.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0010_alter_source_text_model_alter_sourcegroup_text_model.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0010_alter_source_text_model_alter_sourcegroup_text_model.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0011_alter_source_text_model_alter_sourcegroup_text_model.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0011_alter_source_text_model_alter_sourcegroup_text_model.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0012_remove_sourcemarkovmodel_source_and_more.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0012_remove_sourcemarkovmodel_source_and_more.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/migrations/0013_remove_quote_quote_rendered_and_more.py` & `django_quotes-0.5.0/src/django_quotes/migrations/0013_remove_quote_quote_rendered_and_more.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/group_create.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/group_create.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/group_delete.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/group_delete.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/group_detail.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/group_detail.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/group_list.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/group_list.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/group_update.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/group_update.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/quote_create.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_create.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/quote_delete.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_delete.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/quote_detail.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_detail.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/quote_list.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_list.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/quote_update.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_update.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/source_create.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/source_create.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/source_delete.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/source_delete.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/source_detail.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/source_detail.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/source_list.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/source_list.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/src/django_quotes/templates/quotes/source_update.html` & `django_quotes-0.5.0/src/django_quotes/templates/quotes/source_update.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/tests/api_router.py` & `django_quotes-0.5.0/tests/api_router.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/tests/django_settings.py` & `django_quotes-0.5.0/tests/django_settings.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/tests/test_api.py` & `django_quotes-0.5.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/tests/test_management.py` & `django_quotes-0.5.0/tests/test_management.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-#
 # test_management.py
 #
 # Copyright (c) 2024 Daniel Andrlik
 # All rights reserved.
 #
 # SPDX-License-Identifier: BSD-3-Clause
-#
 
 from io import StringIO
 
 import pytest
 from django.core.management import call_command
 from django_quotes.models import SourceGroup
 
 from django_markov.models import MarkovTextModel
 
 pytestmark = pytest.mark.django_db(transaction=True)
 
 
 def test_markov_command(property_group):
     pgmm = property_group.text_model
-    source = property_group.source_set.filter(allow_markov=True)[0]
+    source = property_group.source_set.select_related("text_model").filter(allow_markov=True)[0]
     group_modify = pgmm.modified
     cmm = source.text_model
     char_modify = cmm.modified
     nochangegroup = SourceGroup.objects.create(
         name="So Alone", owner=property_group.owner, text_model=MarkovTextModel.objects.create()
     )
     nochange_modify = nochangegroup.text_model.modified
```

### Comparing `django_quotes-0.4.2/tests/test_signals.py` & `django_quotes-0.5.0/tests/test_signals.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c) 2024 Daniel Andrlik
 # All rights reserved.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import pytest
 from django.contrib.auth import get_user_model
+from django.core.exceptions import ObjectDoesNotExist
 from django_quotes.models import (
     GroupStats,
     Quote,
     QuoteStats,
     Source,
     SourceGroup,
     SourceStats,
@@ -144,45 +145,24 @@
         MarkovTextModel, instance=statable_source.text_model, char_limit=280, sentence="We all go mad sometimes."
     )
     statable_source.refresh_from_db()
     assert char_quotes_generated < statable_source.stats.quotes_generated
     assert group_quotes_generated < statable_source.group.stats.quotes_generated
 
 
-# def test_quote_create_edit_markov_generation_signal(property_group):
-#     source = property_group.source_set.filter(allow_markov=True)[0]
-#     cmodel_lastmodify = SourceMarkovModel.objects.get(source=source).modified
-#     gmodel_lastmodify = GroupMarkovModel.objects.get(group=property_group).modified
-#     q = Quote.objects.create(
-#         quote="I am a new quote, full of exciting things to think about.",
-#         source=source,
-#         owner=property_group.owner,
-#         citation="Some episode",
-#     )
-#     assert (
-#         cmodel_lastmodify
-#         < SourceMarkovModel.objects.get(source=source).modified
-#     )
-#     assert (
-#         gmodel_lastmodify < GroupMarkovModel.objects.get(group=property_group).modified
-#     )
-#     cmodel_lastmodify = SourceMarkovModel.objects.get(source=source).modified
-#     gmodel_lastmodify = GroupMarkovModel.objects.get(group=property_group).modified
-#     q.quote = "Let's change things up a bit with a new quote."
-#     q.save()
-#     assert (
-#         cmodel_lastmodify
-#         < SourceMarkovModel.objects.get(source=source).modified
-#     )
-#     assert (
-#         gmodel_lastmodify < GroupMarkovModel.objects.get(group=property_group).modified
-#     )
-#
-#
 def test_source_set_to_allow_markov_regenerates_models(property_group):
-    source = property_group.source_set.filter(allow_markov=False)[0]
+    source = property_group.source_set.select_related("text_model").filter(allow_markov=False)[0]
     cmodel_lastmodify = source.text_model.modified
     gmodel_lastmodify = property_group.text_model.modified
     source.allow_markov = True
     source.save()
     assert cmodel_lastmodify < MarkovTextModel.objects.get(pk=source.text_model.pk).modified
     assert gmodel_lastmodify < MarkovTextModel.objects.get(pk=property_group.text_model.pk).modified
+
+
+def test_delete_orphaned_text_models(property_group):
+    source = property_group.source_set.select_related("text_model").filter(allow_markov=True).first()
+    assert source.text_model is not None
+    model_id = source.text_model.id
+    source.delete()
+    with pytest.raises(ObjectDoesNotExist):
+        MarkovTextModel.objects.get(pk=model_id)
```

### Comparing `django_quotes-0.4.2/tests/test_utils.py` & `django_quotes-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/tests/test_views.py` & `django_quotes-0.5.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/tests/urls.py` & `django_quotes-0.5.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/tests/factories/users.py` & `django_quotes-0.5.0/tests/factories/users.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/.gitignore` & `django_quotes-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/LICENSE` & `django_quotes-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/README.md` & `django_quotes-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django_quotes-0.4.2/pyproject.toml` & `django_quotes-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-quotes"
-version = "0.4.2"
+version = "0.5.0"
 description = """A reusable Django app to collect quotes for use in random retrieval or generation of sentences using \
     Markov Chains."""
 authors = [{ name = "Daniel Andrlik", email = "daniel@andrlik.org" }]
 dependencies = [
     "django-markov>=0.2.2",
     "rules>=3.1",
     "Markdown>=3.3.6",
@@ -92,14 +92,15 @@
     "pyright>=1.1.357",
     "django-types>=0.19.1",
     "django-stubs-ext>=4.2.7",
     "mike>=2.0.0",
     "markdown-extensions>=0.0.1",
     "mkdocs-gen-files>=0.5.0",
     "mkdocs-literate-nav>=0.6.1",
+    "pytest-asyncio>=0.23.6",
 ]
 
 [tool.coverage.run]
 source = ["src/django_quotes"]
 omit = ["*migrations*", "*tests*", "*staticfiles*"]
 
 [tool.coverage.report]
@@ -245,15 +246,15 @@
 reportIncompatibleMethodOverride = false
 
 [tool.django-stubs]
 django_settings_module = "tests.django_settings"
 
 
 [tool.bumpversion]
-current_version = "0.4.2"
+current_version = "0.5.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
```

### Comparing `django_quotes-0.4.2/PKG-INFO` & `django_quotes-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-quotes
-Version: 0.4.2
+Version: 0.5.0
 Summary: A reusable Django app to collect quotes for use in random retrieval or generation of sentences using Markov Chains.
 Project-URL: Repository, https://github.com/andrlik/django-quotes
 Project-URL: Homepage, https://github.com/andrlik/django-quotes
 Project-URL: Documentation, https://andrlik.github.io/django-quotes/
 Author-email: Daniel Andrlik <daniel@andrlik.org>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
```

