# Comparing `tmp/opperai-0.3.1.tar.gz` & `tmp/opperai-0.3.3.tar.gz`

## Comparing `opperai-0.3.1.tar` & `opperai-0.3.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.3.1/pytest.ini
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.3.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/__init__.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/_client.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/_http_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/functions/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/functions/_async_functions.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/functions/_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/functions/decorator/__init__.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/functions/decorator/_decorator.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/functions/decorator/_schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/indexes/__init__.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/indexes/_async_indexes.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/indexes/_indexes.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/spans/__init__.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/spans/_async_spans.py
--rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/spans/_decorator.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/spans/_spans.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/types/exceptions.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/types/indexes.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/types/spans.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/types/validators.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.3.1/src/opperai/utils/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/test_async_functions.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/test_async_indexes.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/test_async_spans.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/test_decorator.py
--rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/test_functions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/test_indexes.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/test_spans.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/test_trace_decorator.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/test_types.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     9714 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.1/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.3.1/.gitignore
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.3.1/LICENSE
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 opperai-0.3.1/README.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 opperai-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 opperai-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.3.3/pytest.ini
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.3.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/__init__.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/_client.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/_http_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/_async_functions.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/decorator/__init__.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/decorator/_decorator.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/decorator/_schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/indexes/__init__.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/indexes/_async_indexes.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/indexes/_indexes.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/spans/__init__.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/spans/_async_spans.py
+-rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/spans/_decorator.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/spans/_spans.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/types/exceptions.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/types/indexes.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/types/spans.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/types/validators.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/utils/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/conftest.py
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_async_functions.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_async_indexes.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_async_spans.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_decorator.py
+-rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_functions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_indexes.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_spans.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_trace_decorator.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_types.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     9714 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.3.3/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 opperai-0.3.3/README.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 opperai-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 opperai-0.3.3/PKG-INFO
```

### Comparing `opperai-0.3.1/.github/workflows/publish.yml` & `opperai-0.3.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/_client.py` & `opperai-0.3.3/src/opperai/_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 from .functions._async_functions import AsyncFunctions
 from .functions._functions import Functions
 from .indexes._async_indexes import AsyncIndexes
 from .indexes._indexes import Indexes
 from .spans._async_spans import AsyncSpans
 from .spans._spans import Spans
 
-
 DEFAULT_API_URL = "https://api.opper.ai"
+DEFAULT_TIMEOUT = 120
 
 
 class AsyncClient:
     _instance = None
 
     functions: AsyncFunctions
     indexes: AsyncIndexes
     spans: AsyncSpans
 
     def __new__(
         cls,
         api_key: str = None,
         api_url: str = None,
         default_model: str = None,
-        timeout: int = 60,
+        timeout: int = DEFAULT_TIMEOUT,
     ):
         if api_key is None:
             api_key = os.getenv("OPPER_API_KEY")
             if api_key is None:
                 raise Exception(
                     "API key is not provided and OPPER_API_KEY environment variable is not set."
                 )
@@ -57,15 +57,15 @@
     spans: Spans
 
     def __new__(
         cls,
         api_key: str = None,
         api_url: str = None,
         default_model: str = None,
-        timeout: int = 60,
+        timeout: int = DEFAULT_TIMEOUT,
     ):
         if api_key is None:
             api_key = os.getenv("OPPER_API_KEY")
             if api_key is None:
                 raise Exception(
                     "API key is not provided and OPPER_API_KEY environment variable is not set."
                 )
```

### Comparing `opperai-0.3.1/src/opperai/_http_clients.py` & `opperai-0.3.3/src/opperai/_http_clients.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/functions/_async_functions.py` & `opperai-0.3.3/src/opperai/functions/_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/functions/_functions.py` & `opperai-0.3.3/src/opperai/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/functions/decorator/_decorator.py` & `opperai-0.3.3/src/opperai/functions/decorator/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/functions/decorator/_schemas.py` & `opperai-0.3.3/src/opperai/functions/decorator/_schemas.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/indexes/_async_indexes.py` & `opperai-0.3.3/src/opperai/indexes/_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/indexes/_indexes.py` & `opperai-0.3.3/src/opperai/indexes/_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/spans/_async_spans.py` & `opperai-0.3.3/src/opperai/spans/_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/spans/_decorator.py` & `opperai-0.3.3/src/opperai/spans/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/spans/_spans.py` & `opperai-0.3.3/src/opperai/spans/_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/types/__init__.py` & `opperai-0.3.3/src/opperai/types/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/types/indexes.py` & `opperai-0.3.3/src/opperai/types/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/types/spans.py` & `opperai-0.3.3/src/opperai/types/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/types/validators.py` & `opperai-0.3.3/src/opperai/types/validators.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/src/opperai/utils/__init__.py` & `opperai-0.3.3/src/opperai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/conftest.py` & `opperai-0.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/test_async_functions.py` & `opperai-0.3.3/tests/test_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/test_async_indexes.py` & `opperai-0.3.3/tests/test_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/test_async_spans.py` & `opperai-0.3.3/tests/test_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/test_decorator.py` & `opperai-0.3.3/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/test_functions.py` & `opperai-0.3.3/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/test_indexes.py` & `opperai-0.3.3/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/test_spans.py` & `opperai-0.3.3/tests/test_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/test_trace_decorator.py` & `opperai-0.3.3/tests/test_trace_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/test_types.py` & `opperai-0.3.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml` & `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/LICENSE` & `opperai-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/README.md` & `opperai-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `opperai-0.3.1/pyproject.toml` & `opperai-0.3.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "opperai"
-version = "0.3.1"
+version = "0.3.3"
 description = "Opper Python client"
 authors = [
   {name = "Opper", email = "opper@opper.ai"},
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `opperai-0.3.1/PKG-INFO` & `opperai-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opperai
-Version: 0.3.1
+Version: 0.3.3
 Summary: Opper Python client
 Project-URL: Homepage, https://opper.ai
 Project-URL: Documentation, https://docs.opper.ai
 Project-URL: Platform, https://platform.opper.ai
 Author-email: Opper <opper@opper.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

