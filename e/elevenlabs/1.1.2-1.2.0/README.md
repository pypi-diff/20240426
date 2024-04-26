# Comparing `tmp/elevenlabs-1.1.2.tar.gz` & `tmp/elevenlabs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-1.1.2.tar", max compression
+gzip compressed data, was "elevenlabs-1.2.0.tar", max compression
```

## Comparing `elevenlabs-1.1.2.tar` & `elevenlabs-1.2.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
--rw-r--r--   0        0        0     1067 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/LICENSE
--rw-r--r--   0        0        0     9366 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/README.md
--rw-r--r--   0        0        0      659 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     6099 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/__init__.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/audio_native/__init__.py
--rw-r--r--   0        0        0    13835 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/audio_native/client.py
--rw-r--r--   0        0        0     8308 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/base_client.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/chapters/__init__.py
--rw-r--r--   0        0        0    36523 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/chapters/client.py
--rw-r--r--   0        0        0    20882 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/client.py
--rw-r--r--   0        0        0     1006 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/core/api_error.py
--rw-r--r--   0        0        0     1683 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/core/request_options.py
--rw-r--r--   0        0        0     7123 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/core/unchecked_base_model.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/dubbing/__init__.py
--rw-r--r--   0        0        0    29012 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/dubbing/client.py
--rw-r--r--   0        0        0      164 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/environment.py
--rw-r--r--   0        0        0      170 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/history/__init__.py
--rw-r--r--   0        0        0    29127 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/history/client.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/models/__init__.py
--rw-r--r--   0        0        0     5233 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/models/client.py
--rw-r--r--   0        0        0     2715 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/play.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/projects/__init__.py
--rw-r--r--   0        0        0    64179 2024-04-18 10:58:07.094267 elevenlabs-1.1.2/src/elevenlabs/projects/client.py
--rw-r--r--   0        0        0      851 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/pronunciation_dictionary/__init__.py
--rw-r--r--   0        0        0    39904 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/pronunciation_dictionary/client.py
--rw-r--r--   0        0        0      977 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/pronunciation_dictionary/types/__init__.py
--rw-r--r--   0        0        0     1657 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/pronunciation_dictionary/types/body_add_rules_to_the_pronunciation_dictionary_v_1_pronunciation_dictionaries_pronunciation_dictionary_id_add_rules_post_rules_item.py
--rw-r--r--   0        0        0        0 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/py.typed
--rw-r--r--   0        0        0     5093 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/realtime_tts.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/samples/__init__.py
--rw-r--r--   0        0        0    11435 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/samples/client.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/speech_to_speech/__init__.py
--rw-r--r--   0        0        0    27624 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/speech_to_speech/client.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/text_to_speech/__init__.py
--rw-r--r--   0        0        0    20893 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/text_to_speech/client.py
--rw-r--r--   0        0        0     7085 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/__init__.py
--rw-r--r--   0        0        0      188 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/accent.py
--rw-r--r--   0        0        0      977 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/add_project_response_model.py
--rw-r--r--   0        0        0     1057 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
--rw-r--r--   0        0        0      955 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py
--rw-r--r--   0        0        0      918 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/add_voice_response_model.py
--rw-r--r--   0        0        0      158 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/age.py
--rw-r--r--   0        0        0      979 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/audio_native_create_project_response_model.py
--rw-r--r--   0        0        0      130 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
--rw-r--r--   0        0        0     1568 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/audio_output.py
--rw-r--r--   0        0        0      177 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/category.py
--rw-r--r--   0        0        0     1195 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/chapter_response.py
--rw-r--r--   0        0        0     1010 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/chapter_snapshot_response.py
--rw-r--r--   0        0        0     1018 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/chapter_snapshots_response.py
--rw-r--r--   0        0        0      161 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/chapter_state.py
--rw-r--r--   0        0        0     1028 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/chapter_statistics_response.py
--rw-r--r--   0        0        0      146 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/currency.py
--rw-r--r--   0        0        0      949 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/do_dubbing_response.py
--rw-r--r--   0        0        0     1006 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/dubbing_metadata_response.py
--rw-r--r--   0        0        0      211 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
--rw-r--r--   0        0        0     1081 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/feedback_item.py
--rw-r--r--   0        0        0     1836 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/fine_tuning_response.py
--rw-r--r--   0        0        0      220 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/finetuning_state.py
--rw-r--r--   0        0        0      148 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/gender.py
--rw-r--r--   0        0        0     2290 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/generation_config.py
--rw-r--r--   0        0        0      987 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/get_chapters_response.py
--rw-r--r--   0        0        0     1071 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/get_library_voices_response.py
--rw-r--r--   0        0        0      987 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/get_projects_response.py
--rw-r--r--   0        0        0     1159 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py
--rw-r--r--   0        0        0     1067 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
--rw-r--r--   0        0        0     1072 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/get_speech_history_response.py
--rw-r--r--   0        0        0      952 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/get_voices_response.py
--rw-r--r--   0        0        0      101 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/history.py
--rw-r--r--   0        0        0      991 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/history_item.py
--rw-r--r--   0        0        0     1009 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/http_validation_error.py
--rw-r--r--   0        0        0      947 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/invoice.py
--rw-r--r--   0        0        0      930 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/language_response.py
--rw-r--r--   0        0        0     1764 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/library_voice_response.py
--rw-r--r--   0        0        0     1010 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/manual_verification_file_response.py
--rw-r--r--   0        0        0     1085 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/manual_verification_response.py
--rw-r--r--   0        0        0     1670 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/model.py
--rw-r--r--   0        0        0     2215 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/normalized_alignment.py
--rw-r--r--   0        0        0      173 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/optimize_streaming_latency.py
--rw-r--r--   0        0        0      405 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/output_format.py
--rw-r--r--   0        0        0     1277 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/project_extended_response_model.py
--rw-r--r--   0        0        0     1258 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/project_response.py
--rw-r--r--   0        0        0      990 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/project_snapshot_response.py
--rw-r--r--   0        0        0     1018 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/project_snapshots_response.py
--rw-r--r--   0        0        0      161 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/project_state.py
--rw-r--r--   0        0        0      965 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py
--rw-r--r--   0        0        0      987 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py
--rw-r--r--   0        0        0      973 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
--rw-r--r--   0        0        0     1488 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/realtime_voice_settings.py
--rw-r--r--   0        0        0     1006 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/recording_response.py
--rw-r--r--   0        0        0      958 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py
--rw-r--r--   0        0        0      217 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/review_status.py
--rw-r--r--   0        0        0     2361 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/send_text.py
--rw-r--r--   0        0        0      144 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/source.py
--rw-r--r--   0        0        0     1864 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/speech_history_item_response.py
--rw-r--r--   0        0        0      223 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
--rw-r--r--   0        0        0     1078 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/sso_provider_db_model.py
--rw-r--r--   0        0        0      170 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/sso_provider_db_model_provider_type.py
--rw-r--r--   0        0        0     1878 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/subscription.py
--rw-r--r--   0        0        0     1610 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/subscription_response.py
--rw-r--r--   0        0        0      197 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/subscription_response_model_billing_period.py
--rw-r--r--   0        0        0      253 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/subscription_status.py
--rw-r--r--   0        0        0     1140 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/user.py
--rw-r--r--   0        0        0     1028 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1119 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/verification_attempt_response.py
--rw-r--r--   0        0        0     2088 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/voice.py
--rw-r--r--   0        0        0      945 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/voice_generation_parameter_option_response.py
--rw-r--r--   0        0        0     1324 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/voice_generation_parameter_response.py
--rw-r--r--   0        0        0      213 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/voice_response_model_safety_control.py
--rw-r--r--   0        0        0     1101 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/voice_sample.py
--rw-r--r--   0        0        0     1082 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/voice_settings.py
--rw-r--r--   0        0        0     2484 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/voice_sharing_response.py
--rw-r--r--   0        0        0      193 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/voice_sharing_state.py
--rw-r--r--   0        0        0     1244 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/types/voice_verification_response.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/user/__init__.py
--rw-r--r--   0        0        0     9553 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/user/client.py
--rw-r--r--   0        0        0       78 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/version.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/voice_generation/__init__.py
--rw-r--r--   0        0        0    20474 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/voice_generation/client.py
--rw-r--r--   0        0        0       65 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/voices/__init__.py
--rw-r--r--   0        0        0    62073 2024-04-18 10:58:07.098267 elevenlabs-1.1.2/src/elevenlabs/voices/client.py
--rw-r--r--   0        0        0     9958 1970-01-01 00:00:00.000000 elevenlabs-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-26 14:24:09.383905 elevenlabs-1.2.0/LICENSE
+-rw-r--r--   0        0        0     9366 2024-04-26 14:24:09.383905 elevenlabs-1.2.0/README.md
+-rw-r--r--   0        0        0      658 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5583 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/audio_native/__init__.py
+-rw-r--r--   0        0        0    13857 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/audio_native/client.py
+-rw-r--r--   0        0        0     8308 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/base_client.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/chapters/__init__.py
+-rw-r--r--   0        0        0    36655 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/chapters/client.py
+-rw-r--r--   0        0        0    20882 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/client.py
+-rw-r--r--   0        0        0     1006 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/api_error.py
+-rw-r--r--   0        0        0     1683 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/unchecked_base_model.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/dubbing/__init__.py
+-rw-r--r--   0        0        0    29465 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/dubbing/client.py
+-rw-r--r--   0        0        0      164 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/environment.py
+-rw-r--r--   0        0        0      170 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/history/__init__.py
+-rw-r--r--   0        0        0    29717 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/history/client.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/models/__init__.py
+-rw-r--r--   0        0        0     5255 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/models/client.py
+-rw-r--r--   0        0        0     2715 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/play.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/projects/__init__.py
+-rw-r--r--   0        0        0    64289 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/projects/client.py
+-rw-r--r--   0        0        0      303 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/pronunciation_dictionary/__init__.py
+-rw-r--r--   0        0        0    38937 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/pronunciation_dictionary/client.py
+-rw-r--r--   0        0        0      344 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/pronunciation_dictionary/types/__init__.py
+-rw-r--r--   0        0        0     1192 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/pronunciation_dictionary/types/pronunciation_dictionary_rule.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/py.typed
+-rw-r--r--   0        0        0     5093 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/realtime_tts.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/samples/__init__.py
+-rw-r--r--   0        0        0    11479 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/samples/client.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/speech_to_speech/__init__.py
+-rw-r--r--   0        0        0    29158 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/speech_to_speech/client.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/text_to_speech/__init__.py
+-rw-r--r--   0        0        0    24639 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/text_to_speech/client.py
+-rw-r--r--   0        0        0     7085 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/__init__.py
+-rw-r--r--   0        0        0      188 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/accent.py
+-rw-r--r--   0        0        0      977 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/add_project_response_model.py
+-rw-r--r--   0        0        0     1057 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
+-rw-r--r--   0        0        0      955 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py
+-rw-r--r--   0        0        0      918 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/add_voice_response_model.py
+-rw-r--r--   0        0        0      158 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/age.py
+-rw-r--r--   0        0        0      979 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/audio_native_create_project_response_model.py
+-rw-r--r--   0        0        0      130 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
+-rw-r--r--   0        0        0     1568 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/audio_output.py
+-rw-r--r--   0        0        0      177 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/category.py
+-rw-r--r--   0        0        0     1195 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/chapter_response.py
+-rw-r--r--   0        0        0     1010 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/chapter_snapshot_response.py
+-rw-r--r--   0        0        0     1018 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/chapter_snapshots_response.py
+-rw-r--r--   0        0        0      161 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/chapter_state.py
+-rw-r--r--   0        0        0     1028 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/chapter_statistics_response.py
+-rw-r--r--   0        0        0      146 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/currency.py
+-rw-r--r--   0        0        0      949 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/do_dubbing_response.py
+-rw-r--r--   0        0        0     1006 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/dubbing_metadata_response.py
+-rw-r--r--   0        0        0      211 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0     1081 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/feedback_item.py
+-rw-r--r--   0        0        0     1836 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/fine_tuning_response.py
+-rw-r--r--   0        0        0      220 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/finetuning_state.py
+-rw-r--r--   0        0        0      148 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/gender.py
+-rw-r--r--   0        0        0     2290 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/generation_config.py
+-rw-r--r--   0        0        0      987 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_chapters_response.py
+-rw-r--r--   0        0        0     1071 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_library_voices_response.py
+-rw-r--r--   0        0        0      987 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_projects_response.py
+-rw-r--r--   0        0        0     1159 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py
+-rw-r--r--   0        0        0     1067 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
+-rw-r--r--   0        0        0     1072 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_speech_history_response.py
+-rw-r--r--   0        0        0      952 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_voices_response.py
+-rw-r--r--   0        0        0      101 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/history.py
+-rw-r--r--   0        0        0      991 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/history_item.py
+-rw-r--r--   0        0        0     1009 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/http_validation_error.py
+-rw-r--r--   0        0        0      947 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/invoice.py
+-rw-r--r--   0        0        0      930 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/language_response.py
+-rw-r--r--   0        0        0     1764 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/library_voice_response.py
+-rw-r--r--   0        0        0     1010 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/manual_verification_file_response.py
+-rw-r--r--   0        0        0     1085 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/manual_verification_response.py
+-rw-r--r--   0        0        0     1670 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/model.py
+-rw-r--r--   0        0        0     2215 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/normalized_alignment.py
+-rw-r--r--   0        0        0      173 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/optimize_streaming_latency.py
+-rw-r--r--   0        0        0      405 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/output_format.py
+-rw-r--r--   0        0        0     1277 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/project_extended_response_model.py
+-rw-r--r--   0        0        0     1258 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/project_response.py
+-rw-r--r--   0        0        0      990 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/project_snapshot_response.py
+-rw-r--r--   0        0        0     1018 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/project_snapshots_response.py
+-rw-r--r--   0        0        0      161 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/project_state.py
+-rw-r--r--   0        0        0      965 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py
+-rw-r--r--   0        0        0      987 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py
+-rw-r--r--   0        0        0      973 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
+-rw-r--r--   0        0        0     1488 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/realtime_voice_settings.py
+-rw-r--r--   0        0        0     1006 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/recording_response.py
+-rw-r--r--   0        0        0      958 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py
+-rw-r--r--   0        0        0      217 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/review_status.py
+-rw-r--r--   0        0        0     2361 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/send_text.py
+-rw-r--r--   0        0        0      144 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/source.py
+-rw-r--r--   0        0        0     1864 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/speech_history_item_response.py
+-rw-r--r--   0        0        0      223 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
+-rw-r--r--   0        0        0     1078 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/sso_provider_db_model.py
+-rw-r--r--   0        0        0      170 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/sso_provider_db_model_provider_type.py
+-rw-r--r--   0        0        0     1878 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/subscription.py
+-rw-r--r--   0        0        0     1610 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/subscription_response.py
+-rw-r--r--   0        0        0      197 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0      253 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/subscription_status.py
+-rw-r--r--   0        0        0     1140 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/user.py
+-rw-r--r--   0        0        0     1028 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1119 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/verification_attempt_response.py
+-rw-r--r--   0        0        0     2088 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice.py
+-rw-r--r--   0        0        0      945 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_generation_parameter_option_response.py
+-rw-r--r--   0        0        0     1324 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_generation_parameter_response.py
+-rw-r--r--   0        0        0      213 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_response_model_safety_control.py
+-rw-r--r--   0        0        0     1101 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_sample.py
+-rw-r--r--   0        0        0     1082 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_settings.py
+-rw-r--r--   0        0        0     2484 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_sharing_response.py
+-rw-r--r--   0        0        0      193 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_sharing_state.py
+-rw-r--r--   0        0        0     1244 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_verification_response.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/user/__init__.py
+-rw-r--r--   0        0        0     9597 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/user/client.py
+-rw-r--r--   0        0        0       78 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/version.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/voice_generation/__init__.py
+-rw-r--r--   0        0        0    21042 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/voice_generation/client.py
+-rw-r--r--   0        0        0       65 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/voices/__init__.py
+-rw-r--r--   0        0        0    62413 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/voices/client.py
+-rw-r--r--   0        0        0     9958 1970-01-01 00:00:00.000000 elevenlabs-1.2.0/PKG-INFO
```

### Comparing `elevenlabs-1.1.2/LICENSE` & `elevenlabs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/README.md` & `elevenlabs-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/__init__.py` & `elevenlabs-1.2.0/src/elevenlabs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,33 +95,30 @@
     user,
     voice_generation,
     voices,
 )
 from .environment import ElevenLabsEnvironment
 from .play import play, save, stream
 from .pronunciation_dictionary import (
-    BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem,
-    BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem_Alias,
-    BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem_Phoneme,
+    PronunciationDictionaryRule,
+    PronunciationDictionaryRule_Alias,
+    PronunciationDictionaryRule_Phoneme,
 )
 from .version import __version__
 
 __all__ = [
     "Accent",
     "AddProjectResponseModel",
     "AddPronunciationDictionaryResponseModel",
     "AddPronunciationDictionaryRulesResponseModel",
     "AddVoiceResponseModel",
     "Age",
     "AudioNativeCreateProjectResponseModel",
     "AudioNativeGetEmbedCodeResponseModel",
     "AudioOutput",
-    "BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem",
-    "BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem_Alias",
-    "BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem_Phoneme",
     "Category",
     "ChapterResponse",
     "ChapterSnapshotResponse",
     "ChapterSnapshotsResponse",
     "ChapterState",
     "ChapterStatisticsResponse",
     "Currency",
@@ -156,14 +153,17 @@
     "ProjectExtendedResponseModel",
     "ProjectResponse",
     "ProjectSnapshotResponse",
     "ProjectSnapshotsResponse",
     "ProjectState",
     "PronunciationDictionaryAliasRuleRequestModel",
     "PronunciationDictionaryPhonemeRuleRequestModel",
+    "PronunciationDictionaryRule",
+    "PronunciationDictionaryRule_Alias",
+    "PronunciationDictionaryRule_Phoneme",
     "PronunciationDictionaryVersionLocator",
     "RealtimeVoiceSettings",
     "RecordingResponse",
     "RemovePronunciationDictionaryRulesResponseModel",
     "ReviewStatus",
     "SendText",
     "Source",
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/audio_native/client.py` & `elevenlabs-1.2.0/src/elevenlabs/audio_native/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,16 +76,16 @@
             api_key="YOUR_API_KEY",
         )
         client.audio_native.create(
             name="name",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/audio-native"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/audio-native"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "name": name,
@@ -208,16 +208,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.audio_native.create(
             name="name",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/audio-native"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/audio-native"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "name": name,
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/base_client.py` & `elevenlabs-1.2.0/src/elevenlabs/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: ElevenLabsEnvironment = ElevenLabsEnvironment.PRODUCTION,
         api_key: typing.Optional[str] = os.getenv("ELEVEN_API_KEY"),
         timeout: typing.Optional[float] = None,
-        follow_redirects: typing.Optional[bool] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.Client] = None
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = SyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
             api_key=api_key,
             httpx_client=httpx_client
@@ -113,15 +113,15 @@
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: ElevenLabsEnvironment = ElevenLabsEnvironment.PRODUCTION,
         api_key: typing.Optional[str] = os.getenv("ELEVEN_API_KEY"),
         timeout: typing.Optional[float] = None,
-        follow_redirects: typing.Optional[bool] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.AsyncClient] = None
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = AsyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
             api_key=api_key,
             httpx_client=httpx_client
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/chapters/client.py` & `elevenlabs-1.2.0/src/elevenlabs/chapters/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,16 @@
             api_key="YOUR_API_KEY",
         )
         client.chapters.get_all(
             project_id="project_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/projects/{jsonable_encoder(project_id)}/chapters"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -98,16 +98,16 @@
         )
         client.chapters.get(
             project_id="project_id",
             chapter_id="chapter_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/chapters/{jsonable_encoder(chapter_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -156,16 +156,16 @@
         )
         client.chapters.delete(
             project_id="project_id",
             chapter_id="chapter_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/chapters/{jsonable_encoder(chapter_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -214,16 +214,16 @@
         )
         client.chapters.convert(
             project_id="project_id",
             chapter_id="chapter_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/chapters/{jsonable_encoder(chapter_id)}/convert",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
@@ -275,16 +275,16 @@
         )
         client.chapters.get_all_snapshots(
             project_id="project_id",
             chapter_id="chapter_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/chapters/{jsonable_encoder(chapter_id)}/snapshots",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -347,16 +347,16 @@
             chapter_snapshot_id="chapter_snapshot_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if convert_to_mpeg is not OMIT:
             _request["convert_to_mpeg"] = convert_to_mpeg
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/chapters/{jsonable_encoder(chapter_id)}/snapshots/{jsonable_encoder(chapter_snapshot_id)}/stream",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -413,16 +413,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.chapters.get_all(
             project_id="project_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/projects/{jsonable_encoder(project_id)}/chapters"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -470,16 +470,16 @@
         )
         await client.chapters.get(
             project_id="project_id",
             chapter_id="chapter_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/chapters/{jsonable_encoder(chapter_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -528,16 +528,16 @@
         )
         await client.chapters.delete(
             project_id="project_id",
             chapter_id="chapter_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/chapters/{jsonable_encoder(chapter_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -586,16 +586,16 @@
         )
         await client.chapters.convert(
             project_id="project_id",
             chapter_id="chapter_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/chapters/{jsonable_encoder(chapter_id)}/convert",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
@@ -647,16 +647,16 @@
         )
         await client.chapters.get_all_snapshots(
             project_id="project_id",
             chapter_id="chapter_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/chapters/{jsonable_encoder(chapter_id)}/snapshots",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -719,16 +719,16 @@
             chapter_snapshot_id="chapter_snapshot_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if convert_to_mpeg is not OMIT:
             _request["convert_to_mpeg"] = convert_to_mpeg
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/chapters/{jsonable_encoder(chapter_id)}/snapshots/{jsonable_encoder(chapter_snapshot_id)}/stream",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/client.py` & `elevenlabs-1.2.0/src/elevenlabs/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/core/__init__.py` & `elevenlabs-1.2.0/src/elevenlabs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/core/client_wrapper.py` & `elevenlabs-1.2.0/src/elevenlabs/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "elevenlabs",
-            "X-Fern-SDK-Version": "v1.1.2",
+            "X-Fern-SDK-Version": "v1.2.0",
         }
         if self._api_key is not None:
             headers["xi-api-key"] = self._api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/core/datetime_utils.py` & `elevenlabs-1.2.0/src/elevenlabs/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/core/file.py` & `elevenlabs-1.2.0/src/elevenlabs/core/file.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/core/http_client.py` & `elevenlabs-1.2.0/src/elevenlabs/core/http_client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/core/jsonable_encoder.py` & `elevenlabs-1.2.0/src/elevenlabs/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/core/request_options.py` & `elevenlabs-1.2.0/src/elevenlabs/core/request_options.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/core/unchecked_base_model.py` & `elevenlabs-1.2.0/src/elevenlabs/core/unchecked_base_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/dubbing/client.py` & `elevenlabs-1.2.0/src/elevenlabs/dubbing/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,16 +86,16 @@
             api_key="YOUR_API_KEY",
         )
         client.dubbing.dub_a_video_or_an_audio_file(
             target_lang="target_lang",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/dubbing"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/dubbing"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "mode": mode,
@@ -186,16 +186,16 @@
             api_key="YOUR_API_KEY",
         )
         client.dubbing.get_dubbing_project_metadata(
             dubbing_id="dubbing_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/dubbing/{jsonable_encoder(dubbing_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -240,16 +240,16 @@
             api_key="YOUR_API_KEY",
         )
         client.dubbing.delete_dubbing_project(
             dubbing_id="dubbing_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/dubbing/{jsonable_encoder(dubbing_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -275,15 +275,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_dubbed_file(
         self, dubbing_id: str, language_code: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
+    ) -> typing.Iterator[bytes]:
         """
         Returns dubbed file as a streamed file. Videos will be returned in MP4 format and audio only dubs will be returned in MP3.
 
         Parameters:
             - dubbing_id: str. ID of the dubbing project.
 
             - language_code: str. ID of the language.
@@ -292,21 +292,21 @@
         ---
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.dubbing.get_dubbed_file(
-            dubbing_id="dubbing_id",
-            language_code="language_code",
+            dubbing_id="string",
+            language_code="string",
         )
         """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+        with self._client_wrapper.httpx_client.stream(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/dubbing/{jsonable_encoder(dubbing_id)}/audio/{jsonable_encoder(language_code)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -318,26 +318,29 @@
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(
-                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        ) as _response:
+            if 200 <= _response.status_code < 300:
+                for _chunk in _response.iter_bytes():
+                    yield _chunk
+                return
+            _response.read()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
+            try:
+                _response_json = _response.json()
+            except JSONDecodeError:
+                raise ApiError(status_code=_response.status_code, body=_response.text)
+            raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncDubbingClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def dub_a_video_or_an_audio_file(
@@ -402,16 +405,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.dubbing.dub_a_video_or_an_audio_file(
             target_lang="target_lang",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/dubbing"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/dubbing"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "mode": mode,
@@ -502,16 +505,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.dubbing.get_dubbing_project_metadata(
             dubbing_id="dubbing_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/dubbing/{jsonable_encoder(dubbing_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -556,16 +559,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.dubbing.delete_dubbing_project(
             dubbing_id="dubbing_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/dubbing/{jsonable_encoder(dubbing_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -591,15 +594,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_dubbed_file(
         self, dubbing_id: str, language_code: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
+    ) -> typing.AsyncIterator[bytes]:
         """
         Returns dubbed file as a streamed file. Videos will be returned in MP4 format and audio only dubs will be returned in MP3.
 
         Parameters:
             - dubbing_id: str. ID of the dubbing project.
 
             - language_code: str. ID of the language.
@@ -608,21 +611,21 @@
         ---
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.dubbing.get_dubbed_file(
-            dubbing_id="dubbing_id",
-            language_code="language_code",
+            dubbing_id="string",
+            language_code="string",
         )
         """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+        async with self._client_wrapper.httpx_client.stream(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/dubbing/{jsonable_encoder(dubbing_id)}/audio/{jsonable_encoder(language_code)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -634,19 +637,22 @@
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(
-                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        ) as _response:
+            if 200 <= _response.status_code < 300:
+                async for _chunk in _response.aiter_bytes():
+                    yield _chunk
+                return
+            await _response.aread()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
+            try:
+                _response_json = _response.json()
+            except JSONDecodeError:
+                raise ApiError(status_code=_response.status_code, body=_response.text)
+            raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/history/client.py` & `elevenlabs-1.2.0/src/elevenlabs/history/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.history.get_all()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "page_size": page_size,
                         "start_after_history_item_id": start_after_history_item_id,
                         "voice_id": voice_id,
                         **(
@@ -110,16 +110,16 @@
             api_key="YOUR_API_KEY",
         )
         client.history.get(
             history_item_id="history_item_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -162,16 +162,16 @@
             api_key="YOUR_API_KEY",
         )
         client.history.delete(
             history_item_id="history_item_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -212,20 +212,20 @@
         ---
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.history.get_audio(
-            history_item_id="history_item_id",
+            history_item_id="string",
         )
         """
         with self._client_wrapper.httpx_client.stream(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}/audio"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -242,14 +242,18 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 for _chunk in _response.iter_bytes():
                     yield _chunk
                 return
             _response.read()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def download(
@@ -278,16 +282,16 @@
             history_item_ids=["history_item_ids"],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"history_item_ids": history_item_ids}
         if output_format is not OMIT:
             _request["output_format"] = output_format
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history/download"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history/download"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -348,16 +352,16 @@
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.history.get_all()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "page_size": page_size,
                         "start_after_history_item_id": start_after_history_item_id,
                         "voice_id": voice_id,
                         **(
@@ -411,16 +415,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.history.get(
             history_item_id="history_item_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -465,16 +469,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.history.delete(
             history_item_id="history_item_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -515,20 +519,20 @@
         ---
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.history.get_audio(
-            history_item_id="history_item_id",
+            history_item_id="string",
         )
         """
         async with self._client_wrapper.httpx_client.stream(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}/audio"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -545,14 +549,18 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 async for _chunk in _response.aiter_bytes():
                     yield _chunk
                 return
             await _response.aread()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def download(
@@ -581,16 +589,16 @@
             history_item_ids=["history_item_ids"],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"history_item_ids": history_item_ids}
         if output_format is not OMIT:
             _request["output_format"] = output_format
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history/download"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history/download"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/models/client.py` & `elevenlabs-1.2.0/src/elevenlabs/models/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.models.get_all()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/models"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/models"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -81,16 +81,16 @@
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.models.get_all()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/models"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/models"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/play.py` & `elevenlabs-1.2.0/src/elevenlabs/play.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/projects/client.py` & `elevenlabs-1.2.0/src/elevenlabs/projects/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.projects.get_all()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/projects"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/projects"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -84,15 +84,15 @@
         default_model_id: str,
         quality_preset: typing.Optional[str] = None,
         title: typing.Optional[str] = None,
         author: typing.Optional[str] = None,
         isbn_number: typing.Optional[str] = None,
         acx_volume_normalization: typing.Optional[bool] = None,
         volume_normalization: typing.Optional[bool] = None,
-        pronunciation_dictionary_locators: typing.List[str],
+        pronunciation_dictionary_locators: typing.Optional[typing.List[str]] = None,
         callback_url: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddProjectResponseModel:
         """
         Creates a new project, it can be either initialized as blank, from a document or from a URL.
 
         Parameters:
@@ -120,15 +120,15 @@
 
             - isbn_number: typing.Optional[str]. An optional ISBN number of the project you want to create, this will be added as metadata to the mp3 file on project / chapter download.
 
             - acx_volume_normalization: typing.Optional[bool]. [Deprecated] When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
 
             - volume_normalization: typing.Optional[bool]. When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
 
-            - pronunciation_dictionary_locators: typing.List[str]. A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
+            - pronunciation_dictionary_locators: typing.Optional[typing.List[str]]. A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
 
             - callback_url: typing.Optional[str]. A url that will be called by our service when the project is converted with a json containing the status of the conversion
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from elevenlabs.client import ElevenLabs
 
@@ -136,20 +136,19 @@
             api_key="YOUR_API_KEY",
         )
         client.projects.add(
             name="name",
             default_title_voice_id="default_title_voice_id",
             default_paragraph_voice_id="default_paragraph_voice_id",
             default_model_id="default_model_id",
-            pronunciation_dictionary_locators=["pronunciation_dictionary_locators"],
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/projects/add"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/projects/add"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "name": name,
@@ -235,16 +234,16 @@
             api_key="YOUR_API_KEY",
         )
         client.projects.get(
             project_id="project_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/projects/{jsonable_encoder(project_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -287,16 +286,16 @@
             api_key="YOUR_API_KEY",
         )
         client.projects.delete(
             project_id="project_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/projects/{jsonable_encoder(project_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -339,16 +338,16 @@
             api_key="YOUR_API_KEY",
         )
         client.projects.convert(
             project_id="project_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/projects/{jsonable_encoder(project_id)}/convert"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
@@ -396,16 +395,16 @@
             api_key="YOUR_API_KEY",
         )
         client.projects.get_snapshots(
             project_id="project_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/projects/{jsonable_encoder(project_id)}/snapshots"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -463,16 +462,16 @@
             project_snapshot_id="project_snapshot_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if convert_to_mpeg is not OMIT:
             _request["convert_to_mpeg"] = convert_to_mpeg
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/snapshots/{jsonable_encoder(project_snapshot_id)}/stream",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -527,16 +526,16 @@
         )
         client.projects.stream_archive(
             project_id="project_id",
             project_snapshot_id="project_snapshot_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/snapshots/{jsonable_encoder(project_snapshot_id)}/archive",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
@@ -598,16 +597,16 @@
                     pronunciation_dictionary_id="pronunciation_dictionary_id",
                     version_id="version_id",
                 )
             ],
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/update-pronunciation-dictionaries",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"pronunciation_dictionary_locators": pronunciation_dictionary_locators})
@@ -658,16 +657,16 @@
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.projects.get_all()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/projects"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/projects"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -704,15 +703,15 @@
         default_model_id: str,
         quality_preset: typing.Optional[str] = None,
         title: typing.Optional[str] = None,
         author: typing.Optional[str] = None,
         isbn_number: typing.Optional[str] = None,
         acx_volume_normalization: typing.Optional[bool] = None,
         volume_normalization: typing.Optional[bool] = None,
-        pronunciation_dictionary_locators: typing.List[str],
+        pronunciation_dictionary_locators: typing.Optional[typing.List[str]] = None,
         callback_url: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddProjectResponseModel:
         """
         Creates a new project, it can be either initialized as blank, from a document or from a URL.
 
         Parameters:
@@ -740,15 +739,15 @@
 
             - isbn_number: typing.Optional[str]. An optional ISBN number of the project you want to create, this will be added as metadata to the mp3 file on project / chapter download.
 
             - acx_volume_normalization: typing.Optional[bool]. [Deprecated] When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
 
             - volume_normalization: typing.Optional[bool]. When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
 
-            - pronunciation_dictionary_locators: typing.List[str]. A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
+            - pronunciation_dictionary_locators: typing.Optional[typing.List[str]]. A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
 
             - callback_url: typing.Optional[str]. A url that will be called by our service when the project is converted with a json containing the status of the conversion
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from elevenlabs.client import AsyncElevenLabs
 
@@ -756,20 +755,19 @@
             api_key="YOUR_API_KEY",
         )
         await client.projects.add(
             name="name",
             default_title_voice_id="default_title_voice_id",
             default_paragraph_voice_id="default_paragraph_voice_id",
             default_model_id="default_model_id",
-            pronunciation_dictionary_locators=["pronunciation_dictionary_locators"],
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/projects/add"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/projects/add"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "name": name,
@@ -855,16 +853,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.projects.get(
             project_id="project_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/projects/{jsonable_encoder(project_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -907,16 +905,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.projects.delete(
             project_id="project_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/projects/{jsonable_encoder(project_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -959,16 +957,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.projects.convert(
             project_id="project_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/projects/{jsonable_encoder(project_id)}/convert"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
@@ -1016,16 +1014,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.projects.get_snapshots(
             project_id="project_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/projects/{jsonable_encoder(project_id)}/snapshots"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -1083,16 +1081,16 @@
             project_snapshot_id="project_snapshot_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if convert_to_mpeg is not OMIT:
             _request["convert_to_mpeg"] = convert_to_mpeg
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/snapshots/{jsonable_encoder(project_snapshot_id)}/stream",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -1147,16 +1145,16 @@
         )
         await client.projects.stream_archive(
             project_id="project_id",
             project_snapshot_id="project_snapshot_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/snapshots/{jsonable_encoder(project_snapshot_id)}/archive",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
@@ -1218,16 +1216,16 @@
                     pronunciation_dictionary_id="pronunciation_dictionary_id",
                     version_id="version_id",
                 )
             ],
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/update-pronunciation-dictionaries",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"pronunciation_dictionary_locators": pronunciation_dictionary_locators})
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/pronunciation_dictionary/client.py` & `elevenlabs-1.2.0/src/elevenlabs/pronunciation_dictionary/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 from ..types.add_pronunciation_dictionary_rules_response_model import AddPronunciationDictionaryRulesResponseModel
 from ..types.get_pronunciation_dictionaries_metadata_response_model import (
     GetPronunciationDictionariesMetadataResponseModel,
 )
 from ..types.get_pronunciation_dictionary_metadata_response import GetPronunciationDictionaryMetadataResponse
 from ..types.http_validation_error import HttpValidationError
 from ..types.remove_pronunciation_dictionary_rules_response_model import RemovePronunciationDictionaryRulesResponseModel
-from .types.body_add_rules_to_the_pronunciation_dictionary_v_1_pronunciation_dictionaries_pronunciation_dictionary_id_add_rules_post_rules_item import (
-    BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem,
-)
+from .types.pronunciation_dictionary_rule import PronunciationDictionaryRule
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class PronunciationDictionaryClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
@@ -58,16 +56,16 @@
             api_key="YOUR_API_KEY",
         )
         client.pronunciation_dictionary.add_from_file(
             name="name",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", "v1/pronunciation-dictionaries/add-from-file"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(remove_none_from_dict({"name": name, "description": description}))
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -102,43 +100,41 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add_rules_to_the_pronunciation_dictionary(
         self,
         pronunciation_dictionary_id: str,
         *,
-        rules: typing.Sequence[
-            BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem
-        ],
+        rules: typing.Sequence[PronunciationDictionaryRule],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddPronunciationDictionaryRulesResponseModel:
         """
         Add rules to the pronunciation dictionary
 
         Parameters:
             - pronunciation_dictionary_id: str. The id of the pronunciation dictionary
 
-            - rules: typing.Sequence[BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem]. List of pronunciation rules. Rule can be either:
-                                                                                                                                                             an alias rule: {'string_to_replace': 'a', 'type': 'alias', 'alias': 'b', }
-                                                                                                                                                             or a phoneme rule: {'string_to_replace': 'a', 'type': 'phoneme', 'phoneme': 'b', 'alphabet': 'ipa' }
+            - rules: typing.Sequence[PronunciationDictionaryRule]. List of pronunciation rules. Rule can be either:
+                                                                       an alias rule: {'string_to_replace': 'a', 'type': 'alias', 'alias': 'b', }
+                                                                       or a phoneme rule: {'string_to_replace': 'a', 'type': 'phoneme', 'phoneme': 'b', 'alphabet': 'ipa' }
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.pronunciation_dictionary.add_rules_to_the_pronunciation_dictionary(
             pronunciation_dictionary_id="pronunciation_dictionary_id",
             rules=[],
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/pronunciation-dictionaries/{jsonable_encoder(pronunciation_dictionary_id)}/add-rules",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"rules": rules})
@@ -197,16 +193,16 @@
         )
         client.pronunciation_dictionary.remove_rules_from_the_pronunciation_dictionary(
             pronunciation_dictionary_id="pronunciation_dictionary_id",
             rule_strings=["rule_strings"],
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/pronunciation-dictionaries/{jsonable_encoder(pronunciation_dictionary_id)}/remove-rules",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"rule_strings": rule_strings})
@@ -239,15 +235,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_pls_file_with_a_pronunciation_dictionary_version_rules(
         self, dictionary_id: str, version_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> typing.Any:
+    ) -> str:
         """
         Get PLS file with a pronunciation dictionary version rules
 
         Parameters:
             - dictionary_id: str. The id of the pronunciation dictionary
 
             - version_id: str. The id of the version of the pronunciation dictionary
@@ -256,21 +252,21 @@
         ---
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.pronunciation_dictionary.get_pls_file_with_a_pronunciation_dictionary_version_rules(
-            dictionary_id="dictionary_id",
-            version_id="version_id",
+            dictionary_id="string",
+            version_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/pronunciation-dictionaries/{jsonable_encoder(dictionary_id)}/{jsonable_encoder(version_id)}/download",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -284,15 +280,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            return _response.text  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -316,18 +312,18 @@
             api_key="YOUR_API_KEY",
         )
         client.pronunciation_dictionary.get(
             pronunciation_dictionary_id="pronunciation_dictionary_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"v1/pronunciation-dictionaries/{jsonable_encoder(pronunciation_dictionary_id)}",
+                f"v1/pronunciation-dictionaries/{jsonable_encoder(pronunciation_dictionary_id)}/",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -375,16 +371,16 @@
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.pronunciation_dictionary.get_all()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/pronunciation-dictionaries"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/pronunciation-dictionaries/"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         "page_size": page_size,
                         **(
                             request_options.get("additional_query_parameters", {})
@@ -451,16 +447,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.pronunciation_dictionary.add_from_file(
             name="name",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", "v1/pronunciation-dictionaries/add-from-file"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(remove_none_from_dict({"name": name, "description": description}))
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -495,43 +491,41 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add_rules_to_the_pronunciation_dictionary(
         self,
         pronunciation_dictionary_id: str,
         *,
-        rules: typing.Sequence[
-            BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem
-        ],
+        rules: typing.Sequence[PronunciationDictionaryRule],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddPronunciationDictionaryRulesResponseModel:
         """
         Add rules to the pronunciation dictionary
 
         Parameters:
             - pronunciation_dictionary_id: str. The id of the pronunciation dictionary
 
-            - rules: typing.Sequence[BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem]. List of pronunciation rules. Rule can be either:
-                                                                                                                                                             an alias rule: {'string_to_replace': 'a', 'type': 'alias', 'alias': 'b', }
-                                                                                                                                                             or a phoneme rule: {'string_to_replace': 'a', 'type': 'phoneme', 'phoneme': 'b', 'alphabet': 'ipa' }
+            - rules: typing.Sequence[PronunciationDictionaryRule]. List of pronunciation rules. Rule can be either:
+                                                                       an alias rule: {'string_to_replace': 'a', 'type': 'alias', 'alias': 'b', }
+                                                                       or a phoneme rule: {'string_to_replace': 'a', 'type': 'phoneme', 'phoneme': 'b', 'alphabet': 'ipa' }
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.pronunciation_dictionary.add_rules_to_the_pronunciation_dictionary(
             pronunciation_dictionary_id="pronunciation_dictionary_id",
             rules=[],
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/pronunciation-dictionaries/{jsonable_encoder(pronunciation_dictionary_id)}/add-rules",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"rules": rules})
@@ -590,16 +584,16 @@
         )
         await client.pronunciation_dictionary.remove_rules_from_the_pronunciation_dictionary(
             pronunciation_dictionary_id="pronunciation_dictionary_id",
             rule_strings=["rule_strings"],
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/pronunciation-dictionaries/{jsonable_encoder(pronunciation_dictionary_id)}/remove-rules",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"rule_strings": rule_strings})
@@ -632,15 +626,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_pls_file_with_a_pronunciation_dictionary_version_rules(
         self, dictionary_id: str, version_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> typing.Any:
+    ) -> str:
         """
         Get PLS file with a pronunciation dictionary version rules
 
         Parameters:
             - dictionary_id: str. The id of the pronunciation dictionary
 
             - version_id: str. The id of the version of the pronunciation dictionary
@@ -649,21 +643,21 @@
         ---
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.pronunciation_dictionary.get_pls_file_with_a_pronunciation_dictionary_version_rules(
-            dictionary_id="dictionary_id",
-            version_id="version_id",
+            dictionary_id="string",
+            version_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/pronunciation-dictionaries/{jsonable_encoder(dictionary_id)}/{jsonable_encoder(version_id)}/download",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -677,15 +671,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            return _response.text  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -709,18 +703,18 @@
             api_key="YOUR_API_KEY",
         )
         await client.pronunciation_dictionary.get(
             pronunciation_dictionary_id="pronunciation_dictionary_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"v1/pronunciation-dictionaries/{jsonable_encoder(pronunciation_dictionary_id)}",
+                f"v1/pronunciation-dictionaries/{jsonable_encoder(pronunciation_dictionary_id)}/",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -768,16 +762,16 @@
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.pronunciation_dictionary.get_all()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/pronunciation-dictionaries"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/pronunciation-dictionaries/"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         "page_size": page_size,
                         **(
                             request_options.get("additional_query_parameters", {})
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/realtime_tts.py` & `elevenlabs-1.2.0/src/elevenlabs/realtime_tts.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/samples/client.py` & `elevenlabs-1.2.0/src/elevenlabs/samples/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
         )
         client.samples.delete(
             voice_id="voice_id",
             sample_id="sample_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/{jsonable_encoder(voice_id)}/samples/{jsonable_encoder(sample_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -96,16 +96,16 @@
         )
         client.samples.get_audio(
             voice_id="voice_id",
             sample_id="sample_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/{jsonable_encoder(voice_id)}/samples/{jsonable_encoder(sample_id)}/audio",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -159,16 +159,16 @@
         )
         await client.samples.delete(
             voice_id="voice_id",
             sample_id="sample_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/{jsonable_encoder(voice_id)}/samples/{jsonable_encoder(sample_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -217,16 +217,16 @@
         )
         await client.samples.get_audio(
             voice_id="voice_id",
             sample_id="sample_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/{jsonable_encoder(voice_id)}/samples/{jsonable_encoder(sample_id)}/audio",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/speech_to_speech/client.py` & `elevenlabs-1.2.0/src/elevenlabs/speech_to_speech/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 from .. import core
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
+from ..errors.unprocessable_entity_error import UnprocessableEntityError
+from ..types.http_validation_error import HttpValidationError
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class SpeechToSpeechClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
@@ -66,20 +69,22 @@
         ---
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.speech_to_speech.convert(
-            voice_id="voice_id",
+            voice_id="string",
+            optimize_streaming_latency=1,
+            output_format="string",
         )
         """
         with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
@@ -113,14 +118,18 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 for _chunk in _response.iter_bytes():
                     yield _chunk
                 return
             _response.read()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def convert_as_stream(
@@ -170,20 +179,22 @@
         ---
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.speech_to_speech.convert_as_stream(
-            voice_id="voice_id",
+            voice_id="string",
+            optimize_streaming_latency=1,
+            output_format="string",
         )
         """
         with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}/stream"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
@@ -217,14 +228,18 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 for _chunk in _response.iter_bytes():
                     yield _chunk
                 return
             _response.read()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -279,20 +294,22 @@
         ---
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.speech_to_speech.convert(
-            voice_id="voice_id",
+            voice_id="string",
+            optimize_streaming_latency=1,
+            output_format="string",
         )
         """
         async with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
@@ -326,14 +343,18 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 async for _chunk in _response.aiter_bytes():
                     yield _chunk
                 return
             await _response.aread()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def convert_as_stream(
@@ -383,20 +404,22 @@
         ---
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.speech_to_speech.convert_as_stream(
-            voice_id="voice_id",
+            voice_id="string",
+            optimize_streaming_latency=1,
+            output_format="string",
         )
         """
         async with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}/stream"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
@@ -430,12 +453,16 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 async for _chunk in _response.aiter_bytes():
                     yield _chunk
                 return
             await _response.aread()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/text_to_speech/client.py` & `elevenlabs-1.2.0/src/elevenlabs/text_to_speech/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
+from ..errors.unprocessable_entity_error import UnprocessableEntityError
+from ..types.http_validation_error import HttpValidationError
 from ..types.optimize_streaming_latency import OptimizeStreamingLatency
 from ..types.output_format import OutputFormat
 from ..types.pronunciation_dictionary_version_locator import PronunciationDictionaryVersionLocator
 from ..types.voice_settings import VoiceSettings
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
@@ -52,34 +55,50 @@
 
             - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
 
             - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.text_to_speech.convert(
-            voice_id="voice_id",
-            text="text",
+            voice_id="string",
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="string",
+            model_id="string",
+            voice_settings=VoiceSettings(
+                stability=1.1,
+                similarity_boost=1.1,
+                style=1.1,
+                use_speaker_boost=True,
+            ),
+            pronunciation_dictionary_locators=[
+                PronunciationDictionaryVersionLocator(
+                    pronunciation_dictionary_id="string",
+                    version_id="string",
+                )
+            ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"text": text}
         if model_id is not OMIT:
             _request["model_id"] = model_id
         if voice_settings is not OMIT:
             _request["voice_settings"] = voice_settings
         if pronunciation_dictionary_locators is not OMIT:
             _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
@@ -112,14 +131,18 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 for _chunk in _response.iter_bytes():
                     yield _chunk
                 return
             _response.read()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def convert_as_stream(
@@ -152,34 +175,50 @@
 
             - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
 
             - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.text_to_speech.convert_as_stream(
-            voice_id="voice_id",
-            text="text",
+            voice_id="string",
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="string",
+            model_id="string",
+            voice_settings=VoiceSettings(
+                stability=1.1,
+                similarity_boost=1.1,
+                style=1.1,
+                use_speaker_boost=True,
+            ),
+            pronunciation_dictionary_locators=[
+                PronunciationDictionaryVersionLocator(
+                    pronunciation_dictionary_id="string",
+                    version_id="string",
+                )
+            ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"text": text}
         if model_id is not OMIT:
             _request["model_id"] = model_id
         if voice_settings is not OMIT:
             _request["voice_settings"] = voice_settings
         if pronunciation_dictionary_locators is not OMIT:
             _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}/stream"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
@@ -212,14 +251,18 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 for _chunk in _response.iter_bytes():
                     yield _chunk
                 return
             _response.read()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -257,34 +300,50 @@
 
             - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
 
             - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.text_to_speech.convert(
-            voice_id="voice_id",
-            text="text",
+            voice_id="string",
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="string",
+            model_id="string",
+            voice_settings=VoiceSettings(
+                stability=1.1,
+                similarity_boost=1.1,
+                style=1.1,
+                use_speaker_boost=True,
+            ),
+            pronunciation_dictionary_locators=[
+                PronunciationDictionaryVersionLocator(
+                    pronunciation_dictionary_id="string",
+                    version_id="string",
+                )
+            ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"text": text}
         if model_id is not OMIT:
             _request["model_id"] = model_id
         if voice_settings is not OMIT:
             _request["voice_settings"] = voice_settings
         if pronunciation_dictionary_locators is not OMIT:
             _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         async with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
@@ -317,14 +376,18 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 async for _chunk in _response.aiter_bytes():
                     yield _chunk
                 return
             await _response.aread()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def convert_as_stream(
@@ -357,34 +420,50 @@
 
             - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
 
             - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.text_to_speech.convert_as_stream(
-            voice_id="voice_id",
-            text="text",
+            voice_id="string",
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="string",
+            model_id="string",
+            voice_settings=VoiceSettings(
+                stability=1.1,
+                similarity_boost=1.1,
+                style=1.1,
+                use_speaker_boost=True,
+            ),
+            pronunciation_dictionary_locators=[
+                PronunciationDictionaryVersionLocator(
+                    pronunciation_dictionary_id="string",
+                    version_id="string",
+                )
+            ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"text": text}
         if model_id is not OMIT:
             _request["model_id"] = model_id
         if voice_settings is not OMIT:
             _request["voice_settings"] = voice_settings
         if pronunciation_dictionary_locators is not OMIT:
             _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         async with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}/stream"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
@@ -417,12 +496,16 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 async for _chunk in _response.aiter_bytes():
                     yield _chunk
                 return
             await _response.aread()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/__init__.py` & `elevenlabs-1.2.0/src/elevenlabs/types/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/add_project_response_model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/add_project_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/add_voice_response_model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/add_voice_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/audio_native_create_project_response_model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/audio_native_create_project_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/audio_output.py` & `elevenlabs-1.2.0/src/elevenlabs/types/audio_output.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/chapter_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/chapter_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/chapter_snapshot_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/chapter_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/chapter_snapshots_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/chapter_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/chapter_statistics_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/chapter_statistics_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/do_dubbing_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/do_dubbing_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/dubbing_metadata_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/dubbing_metadata_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/feedback_item.py` & `elevenlabs-1.2.0/src/elevenlabs/types/feedback_item.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/fine_tuning_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/fine_tuning_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/generation_config.py` & `elevenlabs-1.2.0/src/elevenlabs/types/generation_config.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/get_chapters_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/get_chapters_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/get_library_voices_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/get_library_voices_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/get_projects_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/get_projects_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/get_speech_history_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/get_speech_history_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/get_voices_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/get_voices_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/history_item.py` & `elevenlabs-1.2.0/src/elevenlabs/types/history_item.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/http_validation_error.py` & `elevenlabs-1.2.0/src/elevenlabs/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/invoice.py` & `elevenlabs-1.2.0/src/elevenlabs/types/invoice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/language_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/language_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/library_voice_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/library_voice_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/manual_verification_file_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/manual_verification_file_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/manual_verification_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/manual_verification_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/normalized_alignment.py` & `elevenlabs-1.2.0/src/elevenlabs/types/normalized_alignment.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/project_extended_response_model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/project_extended_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/project_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/project_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/project_snapshot_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/project_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/project_snapshots_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/project_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/pronunciation_dictionary_version_locator.py` & `elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_version_locator.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/realtime_voice_settings.py` & `elevenlabs-1.2.0/src/elevenlabs/types/realtime_voice_settings.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/recording_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/recording_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/send_text.py` & `elevenlabs-1.2.0/src/elevenlabs/types/send_text.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/speech_history_item_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/speech_history_item_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/sso_provider_db_model.py` & `elevenlabs-1.2.0/src/elevenlabs/types/sso_provider_db_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/subscription.py` & `elevenlabs-1.2.0/src/elevenlabs/types/subscription.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/subscription_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/subscription_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/user.py` & `elevenlabs-1.2.0/src/elevenlabs/types/user.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/validation_error.py` & `elevenlabs-1.2.0/src/elevenlabs/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/verification_attempt_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/verification_attempt_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/voice.py` & `elevenlabs-1.2.0/src/elevenlabs/types/voice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/voice_generation_parameter_option_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/voice_generation_parameter_option_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/voice_generation_parameter_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/voice_generation_parameter_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/voice_sample.py` & `elevenlabs-1.2.0/src/elevenlabs/types/voice_sample.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/voice_settings.py` & `elevenlabs-1.2.0/src/elevenlabs/types/voice_settings.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/voice_sharing_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/voice_sharing_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/types/voice_verification_response.py` & `elevenlabs-1.2.0/src/elevenlabs/types/voice_verification_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.1.2/src/elevenlabs/user/client.py` & `elevenlabs-1.2.0/src/elevenlabs/user/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.user.get_subscription()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/user/subscription"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/user/subscription"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -77,16 +77,16 @@
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.user.get()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/user"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/user"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -128,16 +128,16 @@
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.user.get_subscription()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/user/subscription"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/user/subscription"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -174,16 +174,16 @@
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.user.get()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/user"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/user"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/voice_generation/client.py` & `elevenlabs-1.2.0/src/elevenlabs/voice_generation/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voice_generation.generate_parameters()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice/parameters"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -100,23 +100,23 @@
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voice_generation.generate(
             gender="male",
-            accent="accent",
+            accent="string",
             age="young",
             accent_strength=1.1,
-            text="text",
+            text="string",
         )
         """
         with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(
                 {"gender": gender, "accent": accent, "age": age, "accent_strength": accent_strength, "text": text}
             )
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -141,14 +141,18 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 for _chunk in _response.iter_bytes():
                     yield _chunk
                 return
             _response.read()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_a_previously_generated_voice(
@@ -189,16 +193,16 @@
             "voice_name": voice_name,
             "voice_description": voice_description,
             "generated_voice_id": generated_voice_id,
         }
         if labels is not OMIT:
             _request["labels"] = labels
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/create-voice"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/create-voice"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -248,16 +252,16 @@
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voice_generation.generate_parameters()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice/parameters"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -310,23 +314,23 @@
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voice_generation.generate(
             gender="male",
-            accent="accent",
+            accent="string",
             age="young",
             accent_strength=1.1,
-            text="text",
+            text="string",
         )
         """
         async with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(
                 {"gender": gender, "accent": accent, "age": age, "accent_strength": accent_strength, "text": text}
             )
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -351,14 +355,18 @@
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 async for _chunk in _response.aiter_bytes():
                     yield _chunk
                 return
             await _response.aread()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_a_previously_generated_voice(
@@ -399,16 +407,16 @@
             "voice_name": voice_name,
             "voice_description": voice_description,
             "generated_voice_id": generated_voice_id,
         }
         if labels is not OMIT:
             _request["labels"] = labels
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/create-voice"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/create-voice"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
```

### Comparing `elevenlabs-1.1.2/src/elevenlabs/voices/client.py` & `elevenlabs-1.2.0/src/elevenlabs/voices/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.get_all()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -84,16 +84,16 @@
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.get_default_settings()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices/settings/default"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices/settings/default"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -130,16 +130,16 @@
             api_key="YOUR_API_KEY",
         )
         client.voices.get_settings(
             voice_id="voice_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/settings"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -190,16 +190,18 @@
             api_key="YOUR_API_KEY",
         )
         client.voices.get(
             voice_id="voice_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"
+            ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "with_settings": with_settings,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
@@ -249,16 +251,18 @@
             api_key="YOUR_API_KEY",
         )
         client.voices.delete(
             voice_id="voice_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -305,16 +309,16 @@
         )
         client.voices.edit_settings(
             voice_id="voice_id",
             request=VoiceSettings(),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/settings/edit"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -377,16 +381,16 @@
             api_key="YOUR_API_KEY",
         )
         client.voices.add(
             name="name",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices/add"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices/add"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(remove_none_from_dict({"name": name, "description": description, "labels": labels}))
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(remove_none_from_dict({"name": name, "description": description, "labels": labels})),
@@ -452,16 +456,16 @@
         )
         client.voices.edit(
             voice_id="voice_id",
             name="name",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/edit"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(remove_none_from_dict({"name": name, "description": description, "labels": labels}))
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -524,16 +528,16 @@
         client.voices.add_sharing_voice(
             public_user_id="public_user_id",
             voice_id="voice_id",
             new_name="new_name",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/add/{jsonable_encoder(public_user_id)}/{jsonable_encoder(voice_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"new_name": new_name})
@@ -625,16 +629,16 @@
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.get_shared()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/shared-voices"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/shared-voices"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "page_size": page_size,
                         "category": category,
                         "gender": gender,
                         "age": age,
@@ -698,16 +702,16 @@
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.get_all()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -744,16 +748,16 @@
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.get_default_settings()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices/settings/default"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices/settings/default"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -792,16 +796,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.voices.get_settings(
             voice_id="voice_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/settings"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -852,16 +856,18 @@
             api_key="YOUR_API_KEY",
         )
         await client.voices.get(
             voice_id="voice_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"
+            ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "with_settings": with_settings,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
@@ -911,16 +917,18 @@
             api_key="YOUR_API_KEY",
         )
         await client.voices.delete(
             voice_id="voice_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -967,16 +975,16 @@
         )
         await client.voices.edit_settings(
             voice_id="voice_id",
             request=VoiceSettings(),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/settings/edit"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -1039,16 +1047,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.voices.add(
             name="name",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices/add"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices/add"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(remove_none_from_dict({"name": name, "description": description, "labels": labels}))
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(remove_none_from_dict({"name": name, "description": description, "labels": labels})),
@@ -1114,16 +1122,16 @@
         )
         await client.voices.edit(
             voice_id="voice_id",
             name="name",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/edit"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             data=jsonable_encoder(remove_none_from_dict({"name": name, "description": description, "labels": labels}))
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -1186,16 +1194,16 @@
         await client.voices.add_sharing_voice(
             public_user_id="public_user_id",
             voice_id="voice_id",
             new_name="new_name",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/add/{jsonable_encoder(public_user_id)}/{jsonable_encoder(voice_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"new_name": new_name})
@@ -1287,16 +1295,16 @@
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.get_shared()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/shared-voices"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/shared-voices"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "page_size": page_size,
                         "category": category,
                         "gender": gender,
                         "age": age,
```

### Comparing `elevenlabs-1.1.2/PKG-INFO` & `elevenlabs-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 1.1.2
+Version: 1.2.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

