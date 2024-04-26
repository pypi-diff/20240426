# Comparing `tmp/langfun-0.0.2.dev20240424.tar.gz` & `tmp/langfun-0.0.2.dev20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240424.tar", last modified: Wed Apr 24 08:04:42 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240425.tar", last modified: Thu Apr 25 08:03:38 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240424.tar` & `langfun-0.0.2.dev20240425.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.729651 langfun-0.0.2.dev20240424/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-24 08:04:42.725651 langfun-0.0.2.dev20240424/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.705650 langfun-0.0.2.dev20240424/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.709651 langfun-0.0.2.dev20240424/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.709651 langfun-0.0.2.dev20240424/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.713651 langfun-0.0.2.dev20240424/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.717651 langfun-0.0.2.dev20240424/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55359 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.717651 langfun-0.0.2.dev20240424/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.717651 langfun-0.0.2.dev20240424/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/llms/openai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.717651 langfun-0.0.2.dev20240424/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.721651 langfun-0.0.2.dev20240424/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.725651 langfun-0.0.2.dev20240424/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20980 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19945 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18447 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13944 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.725651 langfun-0.0.2.dev20240424/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:04:42.725651 langfun-0.0.2.dev20240424/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-24 08:04:42.000000 langfun-0.0.2.dev20240424/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-24 08:04:42.000000 langfun-0.0.2.dev20240424/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:04:42.000000 langfun-0.0.2.dev20240424/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 08:04:42.000000 langfun-0.0.2.dev20240424/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 08:04:42.000000 langfun-0.0.2.dev20240424/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:04:42.729651 langfun-0.0.2.dev20240424/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-24 08:04:13.000000 langfun-0.0.2.dev20240424/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.245517 langfun-0.0.2.dev20240425/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-25 08:03:38.245517 langfun-0.0.2.dev20240425/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.225517 langfun-0.0.2.dev20240425/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.233517 langfun-0.0.2.dev20240425/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.233517 langfun-0.0.2.dev20240425/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.237517 langfun-0.0.2.dev20240425/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.237517 langfun-0.0.2.dev20240425/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60239 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22512 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.237517 langfun-0.0.2.dev20240425/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.241517 langfun-0.0.2.dev20240425/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/llms/openai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.241517 langfun-0.0.2.dev20240425/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.241517 langfun-0.0.2.dev20240425/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.245517 langfun-0.0.2.dev20240425/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19860 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18447 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13944 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.245517 langfun-0.0.2.dev20240425/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:38.245517 langfun-0.0.2.dev20240425/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-25 08:03:38.000000 langfun-0.0.2.dev20240425/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-25 08:03:38.000000 langfun-0.0.2.dev20240425/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:03:38.000000 langfun-0.0.2.dev20240425/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 08:03:38.000000 langfun-0.0.2.dev20240425/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 08:03:38.000000 langfun-0.0.2.dev20240425/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:03:38.245517 langfun-0.0.2.dev20240425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-25 08:03:13.000000 langfun-0.0.2.dev20240425/setup.py
```

### Comparing `langfun-0.0.2.dev20240424/LICENSE` & `langfun-0.0.2.dev20240425/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/PKG-INFO` & `langfun-0.0.2.dev20240425/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240424
+Version: 0.0.2.dev20240425
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: absl-py>=1.0.0
 Requires-Dist: google-generativeai>=0.3.2
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: openai==0.27.2
 Requires-Dist: pyglove>=0.4.5.dev20240423
 Requires-Dist: python-magic>=0.4.27
 Requires-Dist: requests>=2.31.0
 Requires-Dist: termcolor==1.1.0
```

### Comparing `langfun-0.0.2.dev20240424/README.md` & `langfun-0.0.2.dev20240425/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/__init__.py` & `langfun-0.0.2.dev20240425/langfun/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 from langfun.core import modalities
 
 Image = modalities.Image
 Video = modalities.Video
 PDF = modalities.PDF
 
 # Error types.
+MappingError = structured.MappingError
 SchemaError = structured.SchemaError
 JsonError = structured.JsonError
 CodeError = coding.CodeError
 
 # Placeholder for Google-internal imports.
 
 # pylint: enable=unused-import
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/__init__.py` & `langfun-0.0.2.dev20240425/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240425/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/component.py` & `langfun-0.0.2.dev20240425/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/component_test.py` & `langfun-0.0.2.dev20240425/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240425/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240425/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/console.py` & `langfun-0.0.2.dev20240425/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/console_test.py` & `langfun-0.0.2.dev20240425/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240425/langfun/core/eval/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """langfun eval framework."""
 
 # pylint: disable=g-importing-member
 # pylint: disable=g-bad-import-order
 
+from langfun.core.eval.base import app_run
+
 from langfun.core.eval.base import Evaluable
 from langfun.core.eval.base import Evaluation
 from langfun.core.eval.base import Suite
 from langfun.core.eval.base import Summary
 
 from langfun.core.eval.base import load
 from langfun.core.eval.base import monitor
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240425/langfun/core/eval/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 import io
 import os
 import re
 import threading
 import time
 from typing import Annotated, Any, Callable, Iterator, Literal, Optional, Sequence, Type, Union
 
+from absl import app
+from absl import flags
 import langfun.core as lf
 import langfun.core.coding as lf_coding
 from langfun.core.llms.cache import in_memory
 import langfun.core.structured as lf_structured
 import pyglove as pg
 
 
@@ -542,14 +544,24 @@
       if m.result is not None:
         s.write(
             '<div style="color: magenta; white-space: pre-wrap;'
             'padding: 10px; border: 1px solid; margin: 10px">'
         )
         s.write(pg.format(m.result))
         s.write('</div>')
+      if 'usage' in m.metadata:
+        s.write(
+            '<div style="background-color: #EEEEEE; color: black; '
+            'white-space: pre-wrap; padding: 10px; border: 0px solid; '
+            'margin: 10px">'
+            f'prompt: {m.usage.prompt_tokens} tokens, '
+            f'response: {m.usage.completion_tokens} tokens, '
+            f'total: {m.usage.total_tokens} tokens'
+            '</div>'
+        )
       s.write('</div>')
 
   @classmethod
   def from_dir(
       cls, maybe_dir: str, load_result: bool = True
   ) -> Optional['Evaluable']:
     exp_json = os.path.join(maybe_dir, Evaluable.EXPERIMENT_JSON)
@@ -806,14 +818,38 @@
   @property
   def failure_rate(self) -> float:
     """Returns the failure rate in range [0, 1]."""
     if self.num_completed == 0:
       return 0.0
     return self.num_failures / self.num_completed
 
+  @property
+  def has_usage(self) -> bool:
+    """Returns True if token usage is enabled."""
+    return self._num_usages > 0
+
+  @property
+  def average_prompt_tokens(self) -> int:
+    """Returns the average prompt tokens."""
+    if not self.has_usage:
+      return 0
+    return self._total_prompt_tokens // self._num_usages
+
+  @property
+  def average_completion_tokens(self) -> int:
+    """Returns the average completion tokens."""
+    if not self.has_usage:
+      return 0
+    return self._total_completion_tokens // self._num_usages
+
+  @property
+  def average_total_tokens(self) -> int:
+    """Returns the average total tokens."""
+    return self.average_prompt_tokens + self.average_completion_tokens
+
   @functools.cached_property
   def schema(self) -> lf_structured.Schema | None:
     """Schema."""
     if self.schema_fn is None:
       return None
 
     schema = self._call_schema_fn()
@@ -852,15 +888,19 @@
       if not hasattr(annotation, '__schema__'):
         raise TypeError(
             'The annotation returned by `schema_fn` must be a `pg.Object` '
             'subclassclass to be used for `lf.complete`. '
             'Encountered: {annotation!r}.'
         )
       self._maybe_adjust_schema_for_completion(annotation)
-    return lf_structured.Schema.from_value(annotation)
+    schema = lf_structured.Schema.from_value(annotation)
+    # NOTE(daiyip): add references to the dependent classes of the returned type
+    # to prevent unused subclasses get garbage collected by Python.
+    setattr(schema, '__dependencies__', schema.class_dependencies())
+    return schema
 
   def _maybe_adjust_schema_for_completion(self, cls):
     if (self.completion_prompt_field is None
         or self.completion_prompt_field in cls.__schema__):
       return
 
     fields = list(cls.__schema__.values())
@@ -929,14 +969,18 @@
     self.__dict__.pop('cache', None)
 
   def _reset(self):
     super()._reset()
     self._failures = []
     self._num_completed = 0
 
+    self._total_prompt_tokens = 0
+    self._total_completion_tokens = 0
+    self._num_usages = 0
+
   @property
   def failures_link(self) -> str | None:
     """Returns the link to the failures page."""
     if self.dir is None:
       return None
     return self.link(os.path.join(self.dir, Evaluation.FAILURES_HTML))
 
@@ -948,15 +992,15 @@
       verbose: bool,
       **kwargs,
   ) -> None:
     # Set the example for dryrun.
     example = example or self.examples[0]
 
     # We make a copy to avoid pollute the state of current object.
-    copy = self.clone()
+    copy: Evaluation = self.clone()
     copy.__dict__['examples'] = [example]
 
     # We set the symbolic parent of the cloned to access contextual information
     # when needed.
     copy.sym_setparent(self.sym_parent)
 
     # Process the input.
@@ -978,17 +1022,17 @@
       lf.console.write('')
       lf.console.write(
           str(output),
           title='OUTPUT',
           color='blue',
       )
 
-    # Audit the result.
-    copy.audit(example, output, output_message)
+    copy.audit(example, output_message, None, dryrun=True)
     result = copy.summarize()
+
     if verbose:
       lf.console.write('')
       lf.console.write(
           str(result),
           title='RESULT',
           color='magenta',
       )
@@ -1027,19 +1071,20 @@
             _process,
             examples,
             max_workers=self.max_workers,
             show_progress=progress_bar or False,
             status_fn=self._status,
         ):
           if error is not None:
-            self._failures.append((example, str(error)))
-          else:
-            output = message.text if self.schema is None else message.result
-            self.audit(example, output, message)
-          self._num_completed += 1
+            message = (
+                error.lm_response
+                if isinstance(error, lf_structured.MappingError)
+                else None
+            )
+          self.audit(example, message, error)
       finally:
         # Save cache upon completion or interruption.
         if self.dir and self.cache:
           self.cache.save()
 
     # Summarize result.
     self._result = self.summarize()
@@ -1134,14 +1179,27 @@
           use_cache=True,
           num_queries=self.cache.stats.num_queries,
           num_hits=self.cache.stats.num_hits,
           num_updates=self.cache.stats.num_updates,
       )
     else:
       cache_stats = dict(use_cache=False)
+
+    if self.has_usage:
+      usage = pg.Dict(
+          total_prompt_tokens=self._total_prompt_tokens,
+          total_completion_tokens=self._total_completion_tokens,
+          num_usages=self._num_usages,
+          average_prompt_tokens=self.average_prompt_tokens,
+          average_completion_tokens=self.average_completion_tokens,
+          average_total_tokens=self.average_total_tokens,
+      )
+    else:
+      usage = None
+
     result = pg.Dict(
         experiment_setup=pg.Dict(
             id=self.id,
             dir=self.dir,
             model=self.lm.model_id,
             prompt_template=lf.text_formatting.decolored(str(self.prompt)),
             method=self.method,
@@ -1149,14 +1207,15 @@
         ),
         cache_stats=cache_stats,
         metrics=pg.Dict(
             total=self.num_completed,
             failures=self.num_failures,
             failure_rate=self.failure_rate,
         ),
+        usage=usage,
     )
     return result
 
   def summarize_html(self) -> str:
     s = io.StringIO()
     definition = _html_repr(self, compact=False, escape=True)
     s.write('<div><table><tr><td>')
@@ -1170,42 +1229,92 @@
     else:
       s.write(
           f'<a target="_blank" title="{definition}" '
           f'href="{self.index_link}">{self.hash}</a>'
           '</td></tr><tr><td>'
       )
       self._render_metric(s)
+
+      # Summarize average usage.
+      if self.result.usage is not None:
+        self._render_usage(s)
+
     s.write('</td></tr></table></div>')
     return s.getvalue()
 
+  def _render_usage(self, s: io.StringIO) -> None:
+    """Renders usage in HTML."""
+    usage = self.result.usage
+    total = usage.total_prompt_tokens + usage.total_completion_tokens
+    s.write(
+        '&nbsp;<a title="'
+        f'# of usages: {usage.num_usages}&#013;'
+        f'total prompt: {usage.total_prompt_tokens}&#013;'
+        f'total response: {usage.total_completion_tokens}&#013;'
+        f'avg prompt: {usage.average_prompt_tokens}&#013;'
+        f'avg response: {usage.average_completion_tokens}'
+        f'" style="color:gray">({total} tokens)</a>'
+    )
+
   def _render_metric(self, s: io.StringIO) -> None:
     """Renders metrics in HTML."""
     assert self.result is not None
     m = self.result.metrics
     s.write(
         '<a title="Failures (%d/%d)" href="%s" style="color:red">%s</a>'
         % (
             m.failures,
             m.total,
             self.failures_link,
             f'%.{self.report_precision}f%% ' % (m.failure_rate * 100),
         )
     )
 
-  def audit(self, example: Any, output: Any, message: lf.Message) -> None:
+  def audit(
+      self,
+      example: Any,
+      message: lf.Message | None,
+      error: Exception | None = None,
+      dryrun: bool = False,
+  ) -> None:
     """Audits the example against the output. Subclasses should override.
 
     Args:
       example: The input object.
-      output: The output from LM. For `lf.call`, if `schema_fn` is not provided,
-        it will be the raw LM response string. Otherwise it will be the
-        structured output from the LM.
       message: The entire message returned by the LM, which could be used to
-        trace the LM input, response and parsed structure.
+        trace the LM input, response and parsed structure. If error is raised
+        before LLM could return a response, None will be its value.
+      error: The exception during processing the example.
+      dryrun: Whether or not audition takes place during dryrun.
     """
+    if error is not None:
+      self._failures.append((example, str(error)))
+      if isinstance(error, lf_structured.MappingError):
+        message = error.lm_response
+    else:
+      assert message is not None
+      output = message.text if self.schema is None else message.result
+      self.audit_processed(example, output, message, dryrun=dryrun)
+
+    # Audit usage.
+    if message is not None:
+      self.audit_usage(message, dryrun=dryrun)
+    self._num_completed += 1
+
+  def audit_usage(self, message: lf.Message, dryrun: bool = False) -> None:
+    for m in message.trace():
+      if 'usage' in m.metadata:
+        self._total_prompt_tokens += m.usage.prompt_tokens
+        self._total_completion_tokens += m.usage.completion_tokens
+        self._num_usages += 1
+
+  def audit_processed(
+      self, example: Any, output: Any, message: lf.Message, dryrun: bool = False
+  ) -> None:
+    """Audits a successfully processed example. Subclass should override."""
 
   def save(
       self, definition: bool = True, result: bool = True, report: bool = True
   ) -> None:
     """Save evaluation details."""
     super().save(definition, result, report)
 
@@ -1241,16 +1350,18 @@
     s.write(
         '<td>Method</td>'
         '<td>Inputs</td>'
         '<td>Model</td>'
         '<td>Prompt</td>'
         '<td>Schema</td>'
         '<td>Additional Args</td>'
-        '<td>Failures</td>'
     )
+    if self.result.usage is not None:
+      s.write('<td>Usage</td>')
+    s.write('<td>Failures</td>')
 
   def _render_result_row(self, s: io.StringIO) -> None:
     s.write(
         f'<td style="color:{self._method_color}">{self.method}</td>'
         f'<td style="color:darkgray">{_html_repr(self.inputs)}</td>'
         f'<td style="color:#494a5c">{_html_repr(self.lm)}</td>'
     )
@@ -1267,14 +1378,20 @@
         f'title="{schema_title}">'
         f'{_html_repr(self.schema_fn)}</td>'
     )
     s.write(
         '<td style="color:purple" '
         f'{_html_repr(self.additional_args, compact=False)}</td>'
     )
+    # Usage.
+    if self.result.usage is not None:
+      s.write('<td>')
+      self._render_usage(s)
+      s.write('</td>')
+
     # Failures.
     s.write(
         '<td><span style="color:orange">%s</span>%s</td>'
         % (
             f'%.{self.report_precision}f%%' % (self.failure_rate * 100),
             '<a href="%s">(%d/%d)</a>'
             % (self.failures_link, self.num_failures, self.num_completed),
@@ -1365,16 +1482,16 @@
       self,
       task: Type[Evaluation] | tuple[Type[Evaluation], ...] = Evaluation,
       lm: Union[
           lf.LanguageModel,
           Type[lf.LanguageModel],
           tuple[lf.LanguageModel | Type[lf.LanguageModel], ...],
       ] = lf.LanguageModel,
-      method: Union[str, tuple[str], None] = None,
-      schema_fn: Union[pg.Functor, tuple[pg.Functor], None] = None,
+      method: Union[str, tuple[str, ...], None] = None,
+      schema_fn: Union[pg.Functor, tuple[pg.Functor, ...], None] = None,
       completed: bool | None = None,
       pivot_field: str | None = None,
   ) -> 'Summary':
     """Creates a summary by selecting evaluations with conditions."""
 
     def _match_lm(lm, evaluation):
       if isinstance(lm, lf.LanguageModel):
@@ -1560,14 +1677,15 @@
     """Returns the JSON representation of the summary."""
     task_results = {}
     for task in sorted(self.tasks(), key=lambda cls: cls.__name__):
       results = []
       for entry in self.select(task=task).evaluations:
         results.append(
             pg.Dict(
+                id=entry.id,
                 experiment=entry,
                 dir=entry.dir,
                 metrics=entry.result.metrics if entry.result else None,
             )
         )
       task_results[task.__name__] = results
     return task_results
@@ -1785,7 +1903,47 @@
       save_as,
       filter,
       pivot_field=pivot_field,
       expect_new_dirs=expect_new_dirs,
       scan_interval=scan_interval,
       refresh_when_stop=refresh_when_stop,
   )
+
+
+def app_run(target: Evaluable):
+  """Runs the target evaluation as an absl app.
+
+  Args:
+    target: An Langfun evaluable object.
+  """
+  flags.DEFINE_string(
+      'root_dir', None, 'Root directory for running the evaluation.'
+  )
+
+  flags.DEFINE_bool(
+      'dryrun', False, 'If True, dryrun the experiment instead of running it.'
+  )
+
+  flags.DEFINE_bool(
+      'debug', False, 'If True, output prompt and response to the console.'
+  )
+
+  flags.DEFINE_bool(
+      'rerun',
+      False,
+      'If True, rerun the experiment even a cached result is found.',
+  )
+
+  FLAGS = flags.FLAGS  # pylint: disable=invalid-name
+
+  def _main(argv):
+    if len(argv) > 1:
+      raise app.UsageError('Too many command-line arguments.')
+
+    if FLAGS.root_dir:
+      target.rebind(root_dir=FLAGS.root_dir, raise_on_no_change=False)
+    if FLAGS.dryrun:
+      target.dryrun(debug=FLAGS.debug)
+    else:
+      target.run(debug=FLAGS.debug, rerun=FLAGS.rerun)
+
+  app.run(_main)
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240425/langfun/core/eval/base_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,22 @@
                 method='query',
                 schema_fn='answer_schema()',
             ),
             cache_stats=dict(
                 use_cache=True, num_queries=2, num_hits=0, num_updates=2
             ),
             metrics=dict(total=2, failures=1, failure_rate=0.5),
+            usage=dict(
+                total_prompt_tokens=774,
+                total_completion_tokens=25,
+                num_usages=2,
+                average_prompt_tokens=387,
+                average_completion_tokens=12,
+                average_total_tokens=399,
+            ),
         ),
     )
     self.assertTrue(
         os.path.exists(os.path.join(s.dir, base.Evaluation.EXPERIMENT_JSON)))
     self.assertTrue(
         os.path.exists(os.path.join(s.dir, base.Evaluation.RESULT_JSON)))
     self.assertTrue(
@@ -281,16 +289,19 @@
     self.assertEqual(s2.result, s.result)
 
   def test_run_with_filter(self):
     lm = fake.StaticResponse('Solution(final_answer=2)')
     s = eval_set(
         'run_filter_test', pg.oneof(['call', 'query']),
         schema_fn=answer_schema(), lm=lm)
+    result = s.run(
+        filter=lambda x: x.method == 'query', dryrun=True, summary=False
+    )
     self.assertEqual(
-        s.run(filter=lambda x: x.method == 'query', dryrun=True, summary=False),
+        result,
         {
             s.children[0].id: None,
             s.children[1].id: dict(
                 experiment_setup=dict(
                     id=s.children[1].id,
                     dir=s.children[1].dir,
                     model='StaticResponse',
@@ -298,15 +309,16 @@
                     method='query',
                     schema_fn='answer_schema()',
                 ),
                 cache_stats=dict(
                     use_cache=True, num_queries=2, num_hits=0, num_updates=2
                 ),
                 metrics=dict(total=2, failures=0, failure_rate=0.0),
-            )
+                usage=s.children[1].result.usage,
+            ),
         },
     )
 
   def test_search_space(self):
     lm = fake.StaticSequence([
         'Solution(final_answer=2)',
         '3',
@@ -332,15 +344,14 @@
         s.children[0].dir, os.path.join(s.root_dir, s.children[0].id)
     )
     # Test persistent hash.
     self.assertEqual(s.hash, 'b66a4e88')
 
     summary = s.run(verbose=True)
     self.assertEqual(len(summary.evaluations), 2)
-
     self.assertEqual(
         s.result,
         {
             s.children[0].id: dict(
                 experiment_setup=dict(
                     id=s.children[0].id,
                     dir=s.children[0].dir,
@@ -349,28 +360,30 @@
                     method='query',
                     schema_fn='answer_schema()',
                 ),
                 cache_stats=dict(
                     use_cache=True, num_queries=2, num_hits=0, num_updates=2
                 ),
                 metrics=dict(total=2, failures=1, failure_rate=0.5),
+                usage=s.children[0].result.usage,
             ),
             s.children[1].id: dict(
                 experiment_setup=dict(
                     id=s.children[1].id,
                     dir=s.children[1].dir,
                     model='StaticSequence',
                     prompt_template='Hello {{example.question}}',
                     method='query',
                     schema_fn='answer_schema()',
                 ),
                 cache_stats=dict(
                     use_cache=True, num_queries=2, num_hits=0, num_updates=2
                 ),
                 metrics=dict(total=2, failures=1, failure_rate=0.5),
+                usage=s.children[1].result.usage,
             ),
         },
     )
 
   def test_call(self):
     lm = fake.StaticSequence(['two'])
     s = eval_set('call_test1', 'call', schema_fn=None, lm=lm)
@@ -471,14 +484,15 @@
                 method='query',
                 schema_fn='answer_schema()',
             ),
             cache_stats=dict(
                 use_cache=True, num_queries=2, num_hits=0, num_updates=2
             ),
             metrics=dict(total=2, failures=1, failure_rate=0.5),
+            usage=s.children[0].result.usage,
         ),
         s.children[1].id: {
             s.children[1]
             .children[0]
             .id: dict(
                 experiment_setup=dict(
                     id=s.children[1].children[0].id,
@@ -488,14 +502,15 @@
                     method='call',
                     schema_fn='answer_schema()',
                 ),
                 cache_stats=dict(
                     use_cache=True, num_queries=4, num_hits=1, num_updates=3
                 ),
                 metrics=dict(total=2, failures=2, failure_rate=1.0),
+                usage=s.children[1].children[0].result.usage,
             ),
             s.children[1]
             .children[2]
             .id: dict(
                 experiment_setup=dict(
                     id=s.children[1].children[2].id,
                     dir=s.children[1].children[2].dir,
@@ -507,14 +522,15 @@
                 cache_stats=dict(
                     use_cache=True,
                     num_queries=2,
                     num_hits=0,
                     num_updates=2,
                 ),
                 metrics=dict(total=2, failures=1, failure_rate=0.5),
+                usage=s.children[1].children[2].result.usage,
             ),
         },
     }
     self.assertEqual(s.result, expected)
 
 
 class InputsFrom(unittest.TestCase):
@@ -678,9 +694,21 @@
     r = base.monitor_async(root_dir, summary_file, expect_new_dirs=True)
     self._eval_set(root_dir).run(summary=False)
     summary = r.stop()
     self.assertTrue(all(e.result for e in summary.evaluations))
     self.assertTrue(pg.io.path_exists(summary_file))
 
 
+class AppRunTest(unittest.TestCase):
+
+  def test_app_run(self):
+    lm = fake.StaticSequence(['two', 'Solution(final_answer=2)'])
+    try:
+      base.app_run(
+          eval_set('app_run_test', 'query', schema_fn=answer_schema(), lm=lm)
+      )
+    except SystemExit:
+      pass
+
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240425/langfun/core/eval/matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,34 @@
     return self.link(os.path.join(self.dir, Matching.MISMATCHES_HTML))
 
   def _reset(self) -> None:
     super()._reset()
     self._matches = []
     self._mismatches = []
 
-  def audit(self, example: Any, output: Any, message: lf.Message) -> None:
+  def audit_processed(
+      self, example: Any, output: Any, message: lf.Message, dryrun: bool = False
+  ) -> None:
     groundtruth = self.groundtruth(example)
     answer = self.answer(output, example)
+
+    if dryrun:
+      lf.console.write('')
+      lf.console.write(
+          str(groundtruth),
+          title='GROUDTRUTH',
+          color='green',
+      )
+      lf.console.write('')
+      lf.console.write(
+          str(answer),
+          title='ANSWER',
+          color='blue',
+      )
+
     if self.match(answer, groundtruth):
       self._matches.append((example, output, message))
     else:
       self._mismatches.append((example, output, message))
 
   def match(self, answer: Any, groundtruth: Any) -> bool:
     """Matches answer against the groundtruth. Subclasses can override."""
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240425/langfun/core/eval/matching_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,14 +121,15 @@
                 failures=1,
                 failure_rate=0.25,
                 num_matches=2,
                 match_rate=0.5,
                 num_mismatches=1,
                 mismatch_rate=0.25,
             ),
+            usage=s.result.usage,
         ),
     )
     self.assertTrue(
         os.path.exists(
             os.path.join(
                 s.dir, matching.Matching.EXPERIMENT_JSON
             )
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240425/langfun/core/eval/scoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,26 @@
       return 0
     return sum([i[2] for i in self._scored]) / self.num_scored
 
   def _reset(self) -> None:
     super()._reset()
     self._scored = []
 
-  def audit(self, example: Any, output: Any, message: lf.Message) -> None:
+  def audit_processed(
+      self, example: Any, output: Any, message: lf.Message, dryrun: bool = False
+  ) -> None:
     score = self.score(example, output)
+
+    if dryrun:
+      lf.console.write('')
+      lf.console.write(
+          str(score),
+          title='SCORE',
+          color='blue',
+      )
     self._scored.append((example, output, score, message))
 
   @abc.abstractmethod
   def score(self, example: Any, output: Any) -> float:
     """Scores the output against its input example."""
 
   def _status(self, progress: lf.concurrent.Progress) -> dict[str, Any]:
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240425/langfun/core/eval/scoring_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
                 total=2,
                 failures=0,
                 failure_rate=0.0,
                 num_scored=2,
                 score_rate=1.0,
                 avg_score=0.5,
             ),
+            usage=s.result.usage,
         ),
     )
     self.assertTrue(
         os.path.exists(
             os.path.join(
                 s.dir, scoring.Scoring.EXPERIMENT_JSON
             )
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240425/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240425/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/language_model.py` & `langfun-0.0.2.dev20240425/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240425/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240425/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240425/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240425/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240425/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/memory.py` & `langfun-0.0.2.dev20240425/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/message.py` & `langfun-0.0.2.dev20240425/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/message_test.py` & `langfun-0.0.2.dev20240425/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240425/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240425/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240425/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240425/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240425/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240425/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240425/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/modality.py` & `langfun-0.0.2.dev20240425/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240425/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240425/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240425/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/sampling.py` & `langfun-0.0.2.dev20240425/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240425/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 from langfun.core.structured.schema_generation import generate_class
 from langfun.core.structured.schema_generation import classgen_example
 from langfun.core.structured.schema_generation import default_classgen_examples
 
 from langfun.core.structured.function_generation import function_gen
 
 from langfun.core.structured.mapping import Mapping
+from langfun.core.structured.mapping import MappingError
 from langfun.core.structured.mapping import MappingExample
 
 from langfun.core.structured.parsing import ParseStructure
 from langfun.core.structured.parsing import ParseStructureJson
 from langfun.core.structured.parsing import ParseStructurePython
 from langfun.core.structured.parsing import parse
 from langfun.core.structured.parsing import call
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/completion_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 """Tests for langfun.core.structured.completion."""
 
 import inspect
 import unittest
 
 import langfun.core as lf
-from langfun.core import coding
 from langfun.core import modalities
 from langfun.core.llms import fake
 from langfun.core.structured import completion
 from langfun.core.structured import mapping
 from langfun.core.structured import schema as schema_lib
 import pyglove as pg
 
@@ -604,15 +603,15 @@
 
   def test_bad_transform(self):
     with lf.context(
         lm=fake.StaticSequence(['Activity(description=1)']),
         override_attrs=True,
     ):
       with self.assertRaisesRegex(
-          coding.CodeError,
+          mapping.MappingError,
           'Expect .* but encountered .*',
       ):
         completion.complete(Activity.partial(), autofix=0)
 
   def test_default(self):
     with lf.context(
         lm=fake.StaticSequence(['Activity(description=1)']),
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,51 @@
 import io
 from typing import Annotated, Any, Callable
 import langfun.core as lf
 from langfun.core.structured import schema as schema_lib
 import pyglove as pg
 
 
+class MappingError(Exception):  # pylint: disable=g-bad-exception-name
+  """Mapping error."""
+
+  def __init__(self, lm_response: lf.Message, cause: Exception):
+    self._lm_response = lm_response
+    self._cause = cause
+
+  @property
+  def lm_response(self) -> lf.Message:
+    """Returns the LM response that failed to be mapped."""
+    return self._lm_response
+
+  @property
+  def cause(self) -> Exception:
+    """Returns the cause of the error."""
+    return self._cause
+
+  def __str__(self) -> str:
+    return self.format(include_lm_response=True)
+
+  def format(self, include_lm_response: bool = True) -> str:
+    """Formats the mapping error."""
+    r = io.StringIO()
+    error_message = str(self.cause).rstrip()
+    r.write(
+        lf.colored(
+            f'{self.cause.__class__.__name__}: {error_message}', 'magenta'
+        )
+    )
+    if include_lm_response:
+      r.write('\n\n')
+      r.write(lf.colored('[LM Response]', 'blue', styles=['bold']))
+      r.write('\n')
+      r.write(lf.colored(self.lm_response.text, 'blue'))
+    return r.getvalue()
+
+
 @pg.use_init_args(['input', 'output', 'schema', 'context'])
 class MappingExample(lf.NaturalLanguageFormattable, lf.Component):
   """Mapping example between text, schema and structured value."""
 
   input: pg.typing.Annotated[
       pg.typing.Any(transform=schema_lib.mark_missing),
       (
@@ -304,15 +341,15 @@
   def transform_output(self, lm_output: lf.Message) -> lf.Message:
     """Transforms LM response into structure if schema is present."""
     try:
       lm_output = self.postprocess_response(lm_output)
       lm_output.result = self.postprocess_result(self.parse_result(lm_output))
     except Exception as e:  # pylint: disable=broad-exception-caught
       if self.default == lf.RAISE_IF_HAS_ERROR:
-        raise e
+        raise MappingError(lm_output, e) from e
       lm_output.result = self.default
     return lm_output
 
   def parse_result(self, lm_output: lf.Message) -> Any:
     """Parse result from LLM response."""
     schema = self.mapping_request.schema
     if schema is None:
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/mapping_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,18 +12,35 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for structured mapping example."""
 
 import inspect
 import unittest
 
+import langfun.core as lf
 from langfun.core.structured import mapping
 import pyglove as pg
 
 
+class MappingErrorTest(unittest.TestCase):
+
+  def test_format(self):
+    error = mapping.MappingError(
+        lf.AIMessage('hi'), ValueError('Cannot parse message.')
+    )
+    self.assertEqual(
+        lf.text_formatting.decolored(str(error)),
+        'ValueError: Cannot parse message.\n\n[LM Response]\nhi',
+    )
+    self.assertEqual(
+        lf.text_formatting.decolored(error.format(include_lm_response=False)),
+        'ValueError: Cannot parse message.',
+    )
+
+
 class MappingExampleTest(unittest.TestCase):
 
   def test_basics(self):
     m = mapping.MappingExample('Compute 1 + 1', '2')
     self.assertEqual(m.schema_repr(), '')
 
     m = mapping.MappingExample('Compute 1 + 1', '2', schema=int)
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/parsing_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,17 @@
 # limitations under the License.
 """Tests for structured parsing."""
 
 import inspect
 import unittest
 
 import langfun.core as lf
-from langfun.core import coding
 from langfun.core.llms import fake
 from langfun.core.structured import mapping
 from langfun.core.structured import parsing
-from langfun.core.structured import schema as schema_lib
 import pyglove as pg
 
 
 class Activity(pg.Object):
   description: str
 
 
@@ -251,15 +249,15 @@
 
   def test_bad_response(self):
     with lf.context(
         lm=fake.StaticResponse('a3'),
         override_attrs=True,
     ):
       with self.assertRaisesRegex(
-          coding.CodeError,
+          mapping.MappingError,
           'name .* is not defined',
       ):
         parsing.parse('three', int)
 
   def test_autofix(self):
     lm = fake.StaticSequence([
         '=3',
@@ -542,15 +540,15 @@
 
   def test_bad_response(self):
     with lf.context(
         lm=fake.StaticSequence(['`3`']),
         override_attrs=True,
     ):
       with self.assertRaisesRegex(
-          schema_lib.JsonError,
+          mapping.MappingError,
           'No JSON dict in the output',
       ):
         parsing.parse('three', int, protocol='json')
 
     with lf.context(
         lm=fake.StaticSequence(['`3`']),
         override_attrs=True,
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/prompting_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 # limitations under the License.
 """Tests for structured prompting."""
 
 import inspect
 import unittest
 
 import langfun.core as lf
-from langfun.core import coding
 from langfun.core import modalities
 from langfun.core.llms import fake
 from langfun.core.structured import mapping
 from langfun.core.structured import prompting
-from langfun.core.structured import schema as schema_lib
 import pyglove as pg
 
 
 class Activity(pg.Object):
   description: str
 
 
@@ -435,15 +433,15 @@
 
   def test_bad_response(self):
     with lf.context(
         lm=fake.StaticSequence(['a2']),
         override_attrs=True,
     ):
       with self.assertRaisesRegex(
-          coding.CodeError,
+          mapping.MappingError,
           'name .* is not defined',
       ):
         prompting.query('Compute 1 + 2', int)
 
   def test_autofix(self):
     lm = fake.StaticSequence([
         '=1',
@@ -673,15 +671,15 @@
 
   def test_bad_transform(self):
     with lf.context(
         lm=fake.StaticSequence(['3']),
         override_attrs=True,
     ):
       with self.assertRaisesRegex(
-          schema_lib.JsonError,
+          mapping.MappingError,
           'No JSON dict in the output',
       ):
         prompting.query('Compute 1 + 2', int, protocol='json')
 
   def test_query(self):
     lm = fake.StaticSequence(['{"result": 1}'])
     self.assertEqual(
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/schema_generation_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import inspect
 import unittest
 
-import langfun.core.coding as lf_coding
 from langfun.core.llms import fake
+from langfun.core.structured import mapping
 from langfun.core.structured import schema_generation
 
 
 class GenerateClassTest(unittest.TestCase):
 
   def test_generate_class_prompt(self):
     input_message = schema_generation.generate_class(
@@ -88,15 +88,15 @@
     cls = schema_generation.generate_class(
         'B',
         'Generate a B class with a field pointing to another class A',
         lm=lm,
     )
     self.assertIs(cls.__name__, 'B')
 
-    with self.assertRaises(lf_coding.CodeError):
+    with self.assertRaises(mapping.MappingError):
       schema_generation.generate_class(
           'Foo',
           'Generate a Foo class with a field pointing to another class A',
           lm=lm,
       )
```

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240425/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/subscription.py` & `langfun-0.0.2.dev20240425/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240425/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/template.py` & `langfun-0.0.2.dev20240425/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/template_test.py` & `langfun-0.0.2.dev20240425/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240425/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240425/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240425/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240425/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240425/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240425/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240425/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240425/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240425/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240425/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240425/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240425/langfun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240424
+Version: 0.0.2.dev20240425
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: absl-py>=1.0.0
 Requires-Dist: google-generativeai>=0.3.2
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: openai==0.27.2
 Requires-Dist: pyglove>=0.4.5.dev20240423
 Requires-Dist: python-magic>=0.4.27
 Requires-Dist: requests>=2.31.0
 Requires-Dist: termcolor==1.1.0
```

### Comparing `langfun-0.0.2.dev20240424/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240425/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240424/setup.py` & `langfun-0.0.2.dev20240425/setup.py`

 * *Files identical despite different names*

