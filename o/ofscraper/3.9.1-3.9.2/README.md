# Comparing `tmp/ofscraper-3.9.1.tar.gz` & `tmp/ofscraper-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.9.1.tar", max compression
+gzip compressed data, was "ofscraper-3.9.2.tar", max compression
```

## Comparing `ofscraper-3.9.1.tar` & `ofscraper-3.9.2.tar`

### file list

```diff
@@ -1,188 +1,189 @@
--rw-r--r--   0        0        0     1067 2024-04-24 16:29:27.777091 ofscraper-3.9.1/LICENSE
--rw-r--r--   0        0        0     4188 2024-04-24 16:29:27.777091 ofscraper-3.9.1/README.md
--rwxr-xr-x   0        0        0      283 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/__main__.py
--rw-r--r--   0        0        0     1064 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/actions/__init__.py
--rw-r--r--   0        0        0     8503 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/actions/like.py
--rw-r--r--   0        0        0    10058 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/actions/process.py
--rw-r--r--   0        0        0    22168 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/actions/scraper.py
--rw-r--r--   0        0        0    15380 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/api/archive.py
--rw-r--r--   0        0        0      274 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/api/common/logs.py
--rw-r--r--   0        0        0    14634 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1479 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/api/init.py
--rw-r--r--   0        0        0    14107 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/labels.py
--rw-r--r--   0        0        0     2912 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/me.py
--rw-r--r--   0        0        0    18532 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/messages.py
--rw-r--r--   0        0        0    13898 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/paid.py
--rw-r--r--   0        0        0     8079 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     6176 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1768 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/subscriptions/helpers.py
--rw-r--r--   0        0        0     3275 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/subscriptions/individual.py
--rw-r--r--   0        0        0    11196 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/subscriptions/lists.py
--rw-r--r--   0        0        0     8149 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/subscriptions/subscriptions.py
--rw-r--r--   0        0        0    16397 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     1453 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/base.py
--rw-r--r--   0        0        0      876 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/labels.py
--rw-r--r--   0        0        0    15565 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/media.py
--rw-r--r--   0        0        0     6005 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/models.py
--rw-r--r--   0        0        0     1771 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0    20557 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     5152 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/posts.py
--rw-r--r--   0        0        0      456 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/semaphoreDelayed.py
--rw-r--r--   0        0        0    15929 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/sessionmanager.py
--rw-r--r--   0        0        0    31982 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/table.py
--rw-r--r--   0        0        0    25956 2024-04-24 16:29:27.869090 ofscraper-3.9.1/ofscraper/commands/check.py
--rw-r--r--   0        0        0    10964 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/commands/manual.py
--rw-r--r--   0        0        0      430 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/commands/picker.py
--rwxr-xr-x   0        0        0     3941 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0       53 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/binary.py
--rw-r--r--   0        0        0     1655 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/config.py
--rw-r--r--   0        0        0      966 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/constants.py
--rw-r--r--   0        0        0       74 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/date.py
--rw-r--r--   0        0        0      184 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/download.py
--rw-r--r--   0        0        0      204 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/files.py
--rw-r--r--   0        0        0     1333 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/general.py
--rw-r--r--   0        0        0       93 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/logger.py
--rw-r--r--   0        0        0       69 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/metadata.py
--rw-r--r--   0        0        0      862 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/other_url.py
--rw-r--r--   0        0        0     1907 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/prompts.py
--rw-r--r--   0        0        0     1719 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/req.py
--rw-r--r--   0        0        0   265533 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/test_constants.py
--rw-r--r--   0        0        0      248 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/time.py
--rw-r--r--   0        0        0     3612 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/url.py
--rw-r--r--   0        0        0        1 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    14326 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/db/operations.py
--rw-r--r--   0        0        0      206 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/db/operations_/helpers.py
--rw-r--r--   0        0        0     8568 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/db/operations_/labels.py
--rw-r--r--   0        0        0    19112 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/media.py
--rw-r--r--   0        0        0     9805 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/merge.py
--rw-r--r--   0        0        0     8504 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/messages.py
--rw-r--r--   0        0        0     8928 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/others.py
--rw-r--r--   0        0        0    10366 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/posts.py
--rw-r--r--   0        0        0     6725 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/profile.py
--rw-r--r--   0        0        0     7485 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/stories.py
--rw-r--r--   0        0        0     4810 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/wrapper.py
--rw-r--r--   0        0        0    10851 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/alt_download.py
--rw-r--r--   0        0        0    10692 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/alt_downloadbatch.py
--rw-r--r--   0        0        0     4852 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/download.py
--rw-r--r--   0        0        0    17155 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/downloadbatch.py
--rw-r--r--   0        0        0     9116 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/downloadnormal.py
--rw-r--r--   0        0        0    10789 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/main_download.py
--rw-r--r--   0        0        0    11235 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/main_downloadbatch.py
--rw-r--r--   0        0        0     1261 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/classes/retries.py
--rw-r--r--   0        0        0     1193 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/classes/session.py
--rw-r--r--   0        0        0     3741 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/common/alt_common.py
--rw-r--r--   0        0        0     6486 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/common/general.py
--rw-r--r--   0        0        0     2054 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/common/main_common.py
--rw-r--r--   0        0        0     2403 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/globals.py
--rw-r--r--   0        0        0     9419 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/keyhelpers.py
--rw-r--r--   0        0        0     3431 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/log.py
--rw-r--r--   0        0        0      317 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/media.py
--rw-r--r--   0        0        0      790 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/message.py
--rw-r--r--   0        0        0     3884 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/metadata.py
--rw-r--r--   0        0        0     2590 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/paths.py
--rw-r--r--   0        0        0      453 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/progress.py
--rw-r--r--   0        0        0     1155 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/text.py
--rw-r--r--   0        0        0     7949 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/media/helpers.py
--rw-r--r--   0        0        0     5019 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/media/main.py
--rw-r--r--   0        0        0     2682 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/date.py
--rw-r--r--   0        0        0     2532 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/flags.py
--rw-r--r--   0        0        0      586 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/other.py
--rw-r--r--   0        0        0     6342 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/price.py
--rw-r--r--   0        0        0     1415 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/sort.py
--rw-r--r--   0        0        0     1122 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/subtype.py
--rw-r--r--   0        0        0     3462 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/models/retriver.py
--rw-r--r--   0        0        0     8003 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/models/selector.py
--rw-r--r--   0        0        0     2466 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/helpers/model_helpers.py
--rw-r--r--   0        0        0    15211 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/helpers/prompt_helpers.py
--rw-r--r--   0        0        0      846 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     7747 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0      917 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/actions.py
--rw-r--r--   0        0        0     6596 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/area.py
--rw-r--r--   0        0        0     8258 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/auth.py
--rw-r--r--   0        0        0     4622 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/binary.py
--rw-r--r--   0        0        0    27896 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/config.py
--rw-r--r--   0        0        0     1879 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/menu.py
--rw-r--r--   0        0        0     2615 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/merge.py
--rw-r--r--   0        0        0    16078 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/model.py
--rw-r--r--   0        0        0     4135 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/profile.py
--rw-r--r--   0        0        0     7609 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    10184 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0     1342 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      567 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/runner/exit.py
--rw-r--r--   0        0        0     1486 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/runner/load.py
--rw-r--r--   0        0        0     2748 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/runner/run.py
--rw-r--r--   0        0        0        1 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3803 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/actions.py
--rw-r--r--   0        0        0     1838 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/areas.py
--rw-r--r--   0        0        0       12 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/globals.py
--rw-r--r--   0        0        0     6624 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/common_args.py
--rw-r--r--   0        0        0    20010 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/main_args.py
--rw-r--r--   0        0        0     1318 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/manual_args.py
--rw-r--r--   0        0        0     1587 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/message_args.py
--rw-r--r--   0        0        0     1588 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/paid_args.py
--rw-r--r--   0        0        0     1955 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/post_args.py
--rw-r--r--   0        0        0     1641 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/story_args.py
--rw-r--r--   0        0        0     5623 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/helpers.py
--rw-r--r--   0        0        0     1928 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/parse.py
--rw-r--r--   0        0        0      395 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/quality.py
--rw-r--r--   0        0        0      863 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/read.py
--rw-r--r--   0        0        0      721 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/user.py
--rw-r--r--   0        0        0      261 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/write.py
--rw-r--r--   0        0        0     2148 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/context.py
--rw-r--r--   0        0        0     1680 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/data.py
--rw-r--r--   0        0        0     2034 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/file.py
--rw-r--r--   0        0        0     2844 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/helpers.py
--rw-r--r--   0        0        0     1756 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/make.py
--rw-r--r--   0        0        0     6940 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/request.py
--rw-r--r--   0        0        0      802 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/schema.py
--rw-r--r--   0        0        0     9824 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0     1780 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/cache.py
--rw-r--r--   0        0        0     1650 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/checkers.py
--rw-r--r--   0        0        0     2894 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/config.py
--rw-r--r--   0        0        0     1447 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/context.py
--rw-r--r--   0        0        0      522 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/custom.py
--rw-r--r--   0        0        0    23743 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/data.py
--rw-r--r--   0        0        0     2146 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/file.py
--rw-r--r--   0        0        0     2111 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/menu.py
--rw-r--r--   0        0        0     4797 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/schema.py
--rw-r--r--   0        0        0      405 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/wrapper.py
--rw-r--r--   0        0        0      499 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/console.py
--rw-r--r--   0        0        0      786 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/constants.py
--rw-r--r--   0        0        0     3401 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/context/exit.py
--rw-r--r--   0        0        0     1135 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/context/run_async.py
--rw-r--r--   0        0        0     1014 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/context/stdout.py
--rw-r--r--   0        0        0     3460 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/dates.py
--rw-r--r--   0        0        0     1040 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     1716 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/hash.py
--rw-r--r--   0        0        0     7231 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/classes.py
--rw-r--r--   0        0        0     2588 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/close.py
--rw-r--r--   0        0        0      477 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/globals.py
--rw-r--r--   0        0        0     1736 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/helpers.py
--rw-r--r--   0        0        0     2098 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/logger.py
--rw-r--r--   0        0        0     1672 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/logs.py
--rw-r--r--   0        0        0     5955 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/other.py
--rw-r--r--   0        0        0     3652 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/stdout.py
--rw-r--r--   0        0        0      617 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/manager.py
--rw-r--r--   0        0        0      388 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/me.py
--rw-r--r--   0        0        0     4200 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/menu.py
--rw-r--r--   0        0        0      659 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/merge.py
--rw-r--r--   0        0        0     1732 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/paths/check.py
--rw-r--r--   0        0        0     3092 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/paths/common.py
--rw-r--r--   0        0        0      279 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/paths/manage.py
--rw-r--r--   0        0        0     5218 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/paths/paths.py
--rw-r--r--   0        0        0     1058 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/profiles/data.py
--rw-r--r--   0        0        0     2785 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/profiles/manage.py
--rw-r--r--   0        0        0     1606 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/profiles/tools.py
--rw-r--r--   0        0        0    10649 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/progress.py
--rw-r--r--   0        0        0     4447 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/run.py
--rw-r--r--   0        0        0        1 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/sems.py
--rw-r--r--   0        0        0     1595 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     4038 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/settings.py
--rw-r--r--   0        0        0      417 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/system/free.py
--rw-r--r--   0        0        0     3285 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/system/network.py
--rw-r--r--   0        0        0     2472 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/system/system.py
--rw-r--r--   0        0        0     2052 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/text.py
--rw-r--r--   0        0        0     2142 2024-04-24 16:29:53.460801 ofscraper-3.9.1/pyproject.toml
--rw-r--r--   0        0        0     6388 1970-01-01 00:00:00.000000 ofscraper-3.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-25 04:16:10.584399 ofscraper-3.9.2/LICENSE
+-rw-r--r--   0        0        0     4188 2024-04-25 04:16:10.584399 ofscraper-3.9.2/README.md
+-rwxr-xr-x   0        0        0      283 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1064 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/__version__.pye
+-rw-r--r--   0        0        0        1 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/actions/__init__.py
+-rw-r--r--   0        0        0     8503 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/actions/like.py
+-rw-r--r--   0        0        0    10058 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/actions/process.py
+-rw-r--r--   0        0        0    22168 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/actions/scraper.py
+-rw-r--r--   0        0        0    15506 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/archive.py
+-rw-r--r--   0        0        0      274 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/common/logs.py
+-rw-r--r--   0        0        0    14634 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1479 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/init.py
+-rw-r--r--   0        0        0    14195 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2912 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/me.py
+-rw-r--r--   0        0        0    18639 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    13891 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     8079 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     6176 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1768 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/subscriptions/helpers.py
+-rw-r--r--   0        0        0     3275 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/subscriptions/individual.py
+-rw-r--r--   0        0        0    12641 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/subscriptions/lists.py
+-rw-r--r--   0        0        0     8169 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/subscriptions/subscriptions.py
+-rw-r--r--   0        0        0    16523 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     1453 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/classes/base.py
+-rw-r--r--   0        0        0      876 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0    15565 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     6005 2024-04-25 04:16:10.588399 ofscraper-3.9.2/ofscraper/classes/models.py
+-rw-r--r--   0        0        0     1771 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0    20557 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     5152 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0      456 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/classes/semaphoreDelayed.py
+-rw-r--r--   0        0        0    16772 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/classes/sessionmanager.py
+-rw-r--r--   0        0        0    31982 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    25956 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/commands/check.py
+-rw-r--r--   0        0        0    10964 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/commands/manual.py
+-rw-r--r--   0        0        0      430 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/commands/picker.py
+-rwxr-xr-x   0        0        0     3941 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0       53 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/binary.py
+-rw-r--r--   0        0        0     1655 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/config.py
+-rw-r--r--   0        0        0      966 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/constants.py
+-rw-r--r--   0        0        0       74 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/date.py
+-rw-r--r--   0        0        0      184 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/download.py
+-rw-r--r--   0        0        0      204 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/files.py
+-rw-r--r--   0        0        0     1333 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/general.py
+-rw-r--r--   0        0        0       93 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/logger.py
+-rw-r--r--   0        0        0       69 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/metadata.py
+-rw-r--r--   0        0        0      862 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/other_url.py
+-rw-r--r--   0        0        0     1907 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/prompts.py
+-rw-r--r--   0        0        0     1739 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/req.py
+-rw-r--r--   0        0        0   265533 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/test_constants.py
+-rw-r--r--   0        0        0      248 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/time.py
+-rw-r--r--   0        0        0     3612 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/const/url.py
+-rw-r--r--   0        0        0        1 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    14335 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/operations.py
+-rw-r--r--   0        0        0      206 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/operations_/helpers.py
+-rw-r--r--   0        0        0     8568 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/operations_/labels.py
+-rw-r--r--   0        0        0    19112 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/operations_/media.py
+-rw-r--r--   0        0        0     9805 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/operations_/merge.py
+-rw-r--r--   0        0        0     8504 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/operations_/messages.py
+-rw-r--r--   0        0        0     8928 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/operations_/others.py
+-rw-r--r--   0        0        0    10366 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/operations_/posts.py
+-rw-r--r--   0        0        0     6725 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/operations_/profile.py
+-rw-r--r--   0        0        0     7485 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/operations_/stories.py
+-rw-r--r--   0        0        0     4810 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/db/operations_/wrapper.py
+-rw-r--r--   0        0        0    10851 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/download/alt_download.py
+-rw-r--r--   0        0        0    10692 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/download/alt_downloadbatch.py
+-rw-r--r--   0        0        0     4852 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/download/download.py
+-rw-r--r--   0        0        0    17155 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/download/downloadbatch.py
+-rw-r--r--   0        0        0     9116 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/download/downloadnormal.py
+-rw-r--r--   0        0        0    10789 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/download/main_download.py
+-rw-r--r--   0        0        0    11235 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/download/main_downloadbatch.py
+-rw-r--r--   0        0        0     1261 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/download/shared/classes/retries.py
+-rw-r--r--   0        0        0     1193 2024-04-25 04:16:10.592399 ofscraper-3.9.2/ofscraper/download/shared/classes/session.py
+-rw-r--r--   0        0        0     3741 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/common/alt_common.py
+-rw-r--r--   0        0        0     6486 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/common/general.py
+-rw-r--r--   0        0        0     2054 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/common/main_common.py
+-rw-r--r--   0        0        0     2403 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/globals.py
+-rw-r--r--   0        0        0     9419 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/utils/keyhelpers.py
+-rw-r--r--   0        0        0     3431 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/utils/log.py
+-rw-r--r--   0        0        0      317 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/utils/media.py
+-rw-r--r--   0        0        0      790 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/utils/message.py
+-rw-r--r--   0        0        0     3884 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/utils/metadata.py
+-rw-r--r--   0        0        0     2590 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/utils/paths.py
+-rw-r--r--   0        0        0      453 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/utils/progress.py
+-rw-r--r--   0        0        0     1155 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/download/shared/utils/text.py
+-rw-r--r--   0        0        0     8076 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/filters/media/helpers.py
+-rw-r--r--   0        0        0     5019 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/filters/media/main.py
+-rw-r--r--   0        0        0     3132 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/filters/models/date.py
+-rw-r--r--   0        0        0     3142 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/filters/models/flags.py
+-rw-r--r--   0        0        0      953 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/filters/models/helpers.py
+-rw-r--r--   0        0        0      725 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/filters/models/other.py
+-rw-r--r--   0        0        0     7549 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/filters/models/price.py
+-rw-r--r--   0        0        0     1523 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/filters/models/sort.py
+-rw-r--r--   0        0        0     1455 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/filters/models/subtype.py
+-rw-r--r--   0        0        0     3457 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/models/retriver.py
+-rw-r--r--   0        0        0     8011 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/models/selector.py
+-rw-r--r--   0        0        0     2466 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/helpers/model_helpers.py
+-rw-r--r--   0        0        0    15211 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/helpers/prompt_helpers.py
+-rw-r--r--   0        0        0      846 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     7747 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0      917 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompt_groups/actions.py
+-rw-r--r--   0        0        0     6596 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompt_groups/area.py
+-rw-r--r--   0        0        0     8258 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompt_groups/auth.py
+-rw-r--r--   0        0        0     4622 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompt_groups/binary.py
+-rw-r--r--   0        0        0    27896 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompt_groups/config.py
+-rw-r--r--   0        0        0     1879 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompt_groups/menu.py
+-rw-r--r--   0        0        0     2615 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompt_groups/merge.py
+-rw-r--r--   0        0        0    16078 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompt_groups/model.py
+-rw-r--r--   0        0        0     4135 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompt_groups/profile.py
+-rw-r--r--   0        0        0     7609 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    10184 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0     1342 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      567 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/runner/exit.py
+-rw-r--r--   0        0        0     1486 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/runner/load.py
+-rw-r--r--   0        0        0     2748 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/runner/run.py
+-rw-r--r--   0        0        0        1 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3803 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/actions.py
+-rw-r--r--   0        0        0     1838 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/areas.py
+-rw-r--r--   0        0        0       12 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/globals.py
+-rw-r--r--   0        0        0     6624 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/groups/common_args.py
+-rw-r--r--   0        0        0    20010 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/groups/main_args.py
+-rw-r--r--   0        0        0     1318 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/groups/manual_args.py
+-rw-r--r--   0        0        0     1587 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/groups/message_args.py
+-rw-r--r--   0        0        0     1588 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/groups/paid_args.py
+-rw-r--r--   0        0        0     1955 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/groups/post_args.py
+-rw-r--r--   0        0        0     1641 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/groups/story_args.py
+-rw-r--r--   0        0        0     5623 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/helpers.py
+-rw-r--r--   0        0        0     1928 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/parse.py
+-rw-r--r--   0        0        0      395 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/quality.py
+-rw-r--r--   0        0        0      863 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/read.py
+-rw-r--r--   0        0        0      721 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/user.py
+-rw-r--r--   0        0        0      261 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/args/write.py
+-rw-r--r--   0        0        0     2148 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/auth/context.py
+-rw-r--r--   0        0        0     1680 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/auth/data.py
+-rw-r--r--   0        0        0     2034 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/auth/file.py
+-rw-r--r--   0        0        0     2844 2024-04-25 04:16:10.596399 ofscraper-3.9.2/ofscraper/utils/auth/helpers.py
+-rw-r--r--   0        0        0     1756 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/auth/make.py
+-rw-r--r--   0        0        0     6940 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/auth/request.py
+-rw-r--r--   0        0        0      802 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/auth/schema.py
+-rw-r--r--   0        0        0     9824 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0     1780 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/cache.py
+-rw-r--r--   0        0        0     1650 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/checkers.py
+-rw-r--r--   0        0        0     2894 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/config/config.py
+-rw-r--r--   0        0        0     1447 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/config/context.py
+-rw-r--r--   0        0        0      522 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/config/custom.py
+-rw-r--r--   0        0        0    24159 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/config/data.py
+-rw-r--r--   0        0        0     2146 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/config/file.py
+-rw-r--r--   0        0        0     2111 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/config/menu.py
+-rw-r--r--   0        0        0     4797 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/config/schema.py
+-rw-r--r--   0        0        0      405 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/config/wrapper.py
+-rw-r--r--   0        0        0      499 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      786 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/constants.py
+-rw-r--r--   0        0        0     3401 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/context/exit.py
+-rw-r--r--   0        0        0     1135 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/context/run_async.py
+-rw-r--r--   0        0        0     1014 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/context/stdout.py
+-rw-r--r--   0        0        0     3460 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0     1040 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     1716 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/hash.py
+-rw-r--r--   0        0        0     7231 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/logs/classes.py
+-rw-r--r--   0        0        0     2588 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/logs/close.py
+-rw-r--r--   0        0        0      477 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/logs/globals.py
+-rw-r--r--   0        0        0     1736 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/logs/helpers.py
+-rw-r--r--   0        0        0     2098 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/logs/logger.py
+-rw-r--r--   0        0        0     1672 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/logs/logs.py
+-rw-r--r--   0        0        0     5955 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/logs/other.py
+-rw-r--r--   0        0        0     3652 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/logs/stdout.py
+-rw-r--r--   0        0        0      617 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/manager.py
+-rw-r--r--   0        0        0      388 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/me.py
+-rw-r--r--   0        0        0     4200 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/menu.py
+-rw-r--r--   0        0        0      659 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/merge.py
+-rw-r--r--   0        0        0     1732 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/paths/check.py
+-rw-r--r--   0        0        0     3092 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/paths/common.py
+-rw-r--r--   0        0        0      279 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/paths/manage.py
+-rw-r--r--   0        0        0     5218 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/paths/paths.py
+-rw-r--r--   0        0        0     1058 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/profiles/data.py
+-rw-r--r--   0        0        0     2785 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/profiles/manage.py
+-rw-r--r--   0        0        0     1606 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/profiles/tools.py
+-rw-r--r--   0        0        0    10649 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/progress.py
+-rw-r--r--   0        0        0     4447 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/run.py
+-rw-r--r--   0        0        0        1 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/sems.py
+-rw-r--r--   0        0        0     1595 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     4038 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/settings.py
+-rw-r--r--   0        0        0      417 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/system/free.py
+-rw-r--r--   0        0        0     3285 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/system/network.py
+-rw-r--r--   0        0        0     2472 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/system/system.py
+-rw-r--r--   0        0        0     2052 2024-04-25 04:16:10.600399 ofscraper-3.9.2/ofscraper/utils/text.py
+-rw-r--r--   0        0        0     2142 2024-04-25 04:16:35.512403 ofscraper-3.9.2/pyproject.toml
+-rw-r--r--   0        0        0     6388 1970-01-01 00:00:00.000000 ofscraper-3.9.2/PKG-INFO
```

### Comparing `ofscraper-3.9.1/LICENSE` & `ofscraper-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/README.md` & `ofscraper-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/__version__.py` & `ofscraper-3.9.2/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/__version__.pye` & `ofscraper-3.9.2/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/actions/like.py` & `ofscraper-3.9.2/ofscraper/actions/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/actions/process.py` & `ofscraper-3.9.2/ofscraper/actions/process.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/actions/scraper.py` & `ofscraper-3.9.2/ofscraper/actions/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/api/archive.py` & `ofscraper-3.9.2/ofscraper/api/archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import ofscraper.db.operations as operations
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
 from ofscraper.utils.context.run_async import run
+from ofscraper.utils.logs.helpers import is_trace
 
 log = logging.getLogger("shared")
 
 
 sem = None
 
 
@@ -373,14 +374,16 @@
 
     finally:
         job_progress.remove_task(task) if job_progress and task else None
     return posts, new_tasks
 
 
 def trace_log_task(responseArray):
+    if not is_trace():
+        return
     chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
     for i in range(1, len(responseArray) + 1, chunk_size):
         # Calculate end index considering potential last chunk being smaller
         end_index = min(
             i + chunk_size - 1, len(responseArray)
         )  # Adjust end_index calculation
         chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
@@ -390,14 +393,16 @@
         log.trace(f"{common_logs.FINAL_RAW.format('Archived')}".format(posts=api_str))
         # Check if there are more elements remaining after this chunk
         if i + chunk_size > len(responseArray):
             break  # Exit the loop if we've processed all elements
 
 
 def trace_log_old(responseArray):
+    if not is_trace():
+        return
     chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
     for i in range(1, len(responseArray) + 1, chunk_size):
         # Calculate end index considering potential last chunk being smaller
         end_index = min(
             i + chunk_size - 1, len(responseArray)
         )  # Adjust end_index calculation
         chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
```

### Comparing `ofscraper-3.9.1/ofscraper/api/highlights.py` & `ofscraper-3.9.2/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/api/init.py` & `ofscraper-3.9.2/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/api/labels.py` & `ofscraper-3.9.2/ofscraper/api/labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import ofscraper.api.common.logs as common_logs
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 from ofscraper.utils.context.run_async import run
+from ofscraper.utils.logs.helpers import is_trace
 
 log = logging.getLogger("shared")
 
 
 @run
 async def get_labels_progress(model_id, c=None):
     labels_ = await get_labels_data_progress(model_id, c=c)
@@ -396,14 +397,16 @@
         list(unduped),
         expire=constants.getattr("THREE_DAY_SECONDS"),
     )
     cache.close()
 
 
 def trace_log_task(responseArray, header=None):
+    if not is_trace():
+        return
     chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
     for i in range(1, len(responseArray) + 1, chunk_size):
         # Calculate end index considering potential last chunk being smaller
         end_index = min(
             i + chunk_size - 1, len(responseArray)
         )  # Adjust end_index calculation
         chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
```

### Comparing `ofscraper-3.9.1/ofscraper/api/me.py` & `ofscraper-3.9.2/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/api/messages.py` & `ofscraper-3.9.2/ofscraper/api/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import asyncio
-import contextvars
 import logging
 import traceback
 
 import arrow
 
 import ofscraper.api.common.logs as common_logs
 import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.db.operations as operations
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
 from ofscraper.utils.context.run_async import run
+from ofscraper.utils.logs.helpers import is_trace
+
 
 log = logging.getLogger("shared")
 
 
 @run
 async def get_messages_progress(model_id, username, forced_after=None, c=None):
     global after
@@ -322,15 +323,14 @@
     )
     url = ep.format(model_id, message_id)
     log.debug(f"{message_id if message_id else 'init'} {url}")
     new_tasks = []
     await asyncio.sleep(1)
     try:
         async with c.requests_async(url=url) as r:
-
             task = (
                 job_progress.add_task(
                     f": Message ID-> {message_id if message_id else 'initial'}"
                 )
                 if job_progress
                 else None
             )
@@ -468,14 +468,16 @@
         log.debug(
             f"Setting date slightly before oldest missing item\nbecause {len(missing_items)} messages in db are marked as undownloaded"
         )
         return arrow.get(missing_items[0]["posted_at"]).float_timestamp
 
 
 def trace_log_task(responseArray):
+    if not is_trace():
+        return
     chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
     for i in range(1, len(responseArray) + 1, chunk_size):
         # Calculate end index considering potential last chunk being smaller
         end_index = min(
             i + chunk_size - 1, len(responseArray)
         )  # Adjust end_index calculation
         chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
@@ -485,14 +487,16 @@
         log.trace(f"{common_logs.FINAL_RAW.format('Messages')}".format(posts=api_str))
         # Check if there are more elements remaining after this chunk
         if i + chunk_size > len(responseArray):
             break  # Exit the loop if we've processed all elements
 
 
 def trace_log_old(responseArray):
+    if not is_trace():
+        return
     chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
     for i in range(1, len(responseArray) + 1, chunk_size):
         # Calculate end index considering potential last chunk being smaller
         end_index = min(
             i + chunk_size - 1, len(responseArray)
         )  # Adjust end_index calculation
         chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
```

### Comparing `ofscraper-3.9.1/ofscraper/api/paid.py` & `ofscraper-3.9.2/ofscraper/api/paid.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
                             )
                             new_tasks.extend(new_tasks_batch)
                             await asyncio.sleep(1)
                         except Exception as E:
                             await asyncio.sleep(1)
                             log.traceback_(E)
                             log.traceback_(traceback.format_exc())
-                            continue
+                            u
                     tasks = new_tasks
                 overall_progress.remove_task(page_task)
 
         log.debug(f"[bold]Paid Post count with Dupes[/bold] {len(output)} found")
         log.trace(
             "paid raw duped {posts}".format(
                 posts="\n\n".join(
```

### Comparing `ofscraper-3.9.1/ofscraper/api/pinned.py` & `ofscraper-3.9.2/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/api/profile.py` & `ofscraper-3.9.2/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/api/subscriptions/helpers.py` & `ofscraper-3.9.2/ofscraper/api/subscriptions/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/api/subscriptions/individual.py` & `ofscraper-3.9.2/ofscraper/api/subscriptions/individual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/api/subscriptions/lists.py` & `ofscraper-3.9.2/ofscraper/api/subscriptions/lists.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from rich.style import Style
 
 import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.console as console
 import ofscraper.utils.constants as constants
 from ofscraper.utils.context.run_async import run
+from ofscraper.utils.logs.helpers import is_trace
+
 
 log = logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
 
 
 @run
 async def get_otherlist():
@@ -120,21 +122,42 @@
                             output.extend(result)
                         except Exception as E:
                             log.traceback_(E)
                             log.traceback_(traceback.format_exc())
                             continue
                     tasks = new_tasks
     overall_progress.remove_task(page_task)
-    log.trace(
+    trace_log_list(output)
+    
+    log.debug(f"[bold]lists name count without Dupes[/bold] {len(output)} found")
+    return output
+
+def trace_log_list(responseArray):
+    if not is_trace():
+        return
+    chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
+    for i in range(1, len(responseArray) + 1, chunk_size):
+        # Calculate end index considering potential last chunk being smaller
+        end_index = min(
+            i + chunk_size - 1, len(responseArray)
+        )  # Adjust end_index calculation
+        chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
+        log.trace(
         "list unduped {posts}".format(
-            posts="\n\n".join(map(lambda x: f" list data raw:{x}", output))
+            posts="\n\n".join(map(lambda x: f" list data raw:{x}", chunk))
         )
     )
-    log.debug(f"[bold]lists name count without Dupes[/bold] {len(output)} found")
-    return output
+        # Check if there are more elements remaining after this chunk
+        if i + chunk_size > len(responseArray):
+            break  # Exit the loop if we've processed all elements
+
+
+
+
+
 
 
 async def scrape_for_list(c, job_progress, offset=0):
     attempt.set(0)
     new_tasks = []
     url = constants.getattr("listEP").format(offset)
     try:
@@ -150,15 +173,15 @@
                 f"offset:{offset} -> lists names found {list(map(lambda x:x['name'],out_list))}"
             )
             log.debug(f"offset:{offset} -> number of lists found {len(out_list)}")
             log.debug(
                 f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }"
             )
             log.trace(
-                "offset:{offset} -> label names raw: {posts}".format(
+                "offset:{offset} -> list names raw: {posts}".format(
                     offset=offset, posts=data
                 )
             )
 
             if data.get("hasMore") and len(out_list) > 0:
                 offset = offset + len(out_list)
                 new_tasks.append(
@@ -231,23 +254,39 @@
                             continue
                     tasks = new_tasks
 
     overall_progress.remove_task(page_task)
     outdict = {}
     for ele in output:
         outdict[ele["id"]] = ele
-    log.trace(
-        "users found {users}".format(
-            users="\n\n".join(map(lambda x: f"user data: {str(x)}", outdict.values()))
-        )
-    )
+    trace_log_usernames(outdict.values())
     log.debug(f"[bold]users count without Dupes[/bold] {len(outdict.values())} found")
     return outdict.values()
 
 
+def trace_log_usernames(responseArray):
+    if not is_trace():
+        return
+    chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
+    for i in range(1, len(responseArray) + 1, chunk_size):
+        # Calculate end index considering potential last chunk being smaller
+        end_index = min(
+            i + chunk_size - 1, len(responseArray)
+        )  # Adjust end_index calculation
+        chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
+        log.trace(
+        "users found {users}".format(
+            users="\n\n".join(map(lambda x: f"user data: {str(x)}", chunk))
+        )
+    
+    )
+        # Check if there are more elements remaining after this chunk
+        if i + chunk_size > len(responseArray):
+            break  # Exit the loop if we've processed all elements
+
 async def scrape_list_members(c, item, job_progress, offset=0):
     users = None
     attempt.set(0)
     new_tasks = []
     url = constants.getattr("listusersEP").format(item.get("id"), offset)
     try:
         attempt.set(attempt.get(0) + 1)
```

### Comparing `ofscraper-3.9.1/ofscraper/api/subscriptions/subscriptions.py` & `ofscraper-3.9.2/ofscraper/api/subscriptions/subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         log.debug(f"usernames active offset {offset}")
         async with c.requests_async(url=url) as r:
             subscriptions = (await r.json_())["list"]
             log.debug(
                 f"usernames retrived -> {list(map(lambda x:x.get('username'),subscriptions))}"
             )
             if len(subscriptions) == 0:
-                return subscriptions
+                return subscriptions,new_tasks
             elif recur is False:
                 pass
             elif (await r.json_())["hasMore"] is True:
                 new_tasks.append(
                     asyncio.create_task(
                         scrape_subscriptions_active(
                             c,
@@ -203,15 +203,15 @@
         async with c.requests_async(url=url) as r:
             subscriptions = (await r.json_())["list"]
             log.debug(
                 f"usernames retrived -> {list(map(lambda x:x.get('username'),subscriptions))}"
             )
 
             if len(subscriptions) == 0:
-                return subscriptions
+                return subscriptions,new_tasks
             elif recur is False:
                 pass
             elif (await r.json_())["hasMore"] is True:
                 new_tasks.append(
                     asyncio.create_task(
                         scrape_subscriptions_disabled(
                             c,
```

### Comparing `ofscraper-3.9.1/ofscraper/api/timeline.py` & `ofscraper-3.9.2/ofscraper/api/timeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import ofscraper.db.operations as operations
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
 from ofscraper.utils.context.run_async import run
+from ofscraper.utils.logs.helpers import is_trace
 
 log = logging.getLogger("shared")
 
 
 @run
 async def get_timeline_posts_progress(model_id, username, forced_after=None, c=None):
 
@@ -401,14 +402,16 @@
         log.traceback_(traceback.format_exc())
         raise E
     finally:
         job_progress.remove_task(task) if job_progress and task != None else None
 
 
 def trace_log_task(responseArray):
+    if not is_trace():
+        return
     chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
     for i in range(1, len(responseArray) + 1, chunk_size):
         # Calculate end index considering potential last chunk being smaller
         end_index = min(
             i + chunk_size - 1, len(responseArray)
         )  # Adjust end_index calculation
         chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
@@ -418,14 +421,16 @@
         log.trace(f"{common_logs.FINAL_RAW.format('Timeline')}".format(posts=api_str))
         # Check if there are more elements remaining after this chunk
         if i + chunk_size > len(responseArray):
             break  # Exit the loop if we've processed all elements
 
 
 def trace_log_old(responseArray):
+    if not is_trace():
+        return
     chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
     for i in range(1, len(responseArray) + 1, chunk_size):
         # Calculate end index considering potential last chunk being smaller
         end_index = min(
             i + chunk_size - 1, len(responseArray)
         )  # Adjust end_index calculation
         chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
```

### Comparing `ofscraper-3.9.1/ofscraper/classes/base.py` & `ofscraper-3.9.2/ofscraper/classes/base.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/classes/labels.py` & `ofscraper-3.9.2/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/classes/media.py` & `ofscraper-3.9.2/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/classes/models.py` & `ofscraper-3.9.2/ofscraper/classes/models.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.9.2/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/classes/placeholder.py` & `ofscraper-3.9.2/ofscraper/classes/placeholder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/classes/posts.py` & `ofscraper-3.9.2/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/classes/sessionmanager.py` & `ofscraper-3.9.2/ofscraper/classes/sessionmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,47 @@
-import asyncio
 import contextlib
+import time
+import asyncio
 import logging
 import ssl
 import threading
 import traceback
+import arrow
 
 import aiohttp
 import aiohttp.client_exceptions
 import certifi
 import httpx
 import tenacity
 from tenacity import AsyncRetrying, Retrying, retry_if_not_exception_type
 
 import ofscraper.utils.auth.request as auth_requests
 import ofscraper.utils.config.data as data
 import ofscraper.utils.constants as constants
 
+class SessionSleep():
+    def __init__(self):
+        self._sleep=None
+        self._last_date=None
+    def toomany_req(self):
+
+        if arrow.now().float_timestamp-self._last_date.float_timestamp<120:
+            return self._sleep
+        elif self._sleep is None:
+            self._sleep=constants.getattr("SESSION_SLEEP_INIT")
+        else:
+            self._sleep=self._sleep*2
+        self._last_date=arrow.now()
+        logging.getLogger("shared").debug(f"setting sleep to {self._sleep} seconds")
+        return self._sleep
+    @property
+    def sleep(self):
+        return self._sleep
+
+sleeper=SessionSleep()
 
 class CustomTenacity(AsyncRetrying):
     """
     A custom context manager using tenacity for asynchronous retries with wait strategies and stopping without exceptions.
     """
 
     def __init__(self, wait_random=None, wait_exponential=None, *args, **kwargs):
@@ -47,14 +69,15 @@
             )
             
         ):
             sleep = self.wait_exponential(retry_state)
         else:
             sleep = self.wait_random(retry_state)
         logging.getLogger("shared").debug(f"sleeping for {sleep} seconds before")
+        sleeper.toomany_req()
         return sleep
 
     def _after_func(self, retry_state) -> None:
         exception = retry_state.outcome.exception()
         if (
             isinstance(exception, (aiohttp.ClientResponseError, aiohttp.ClientError))
             and (
@@ -205,14 +228,15 @@
         wait_min=None,
         wait_max=None,
         log=None,
         total_timeout=None,
         connect_timeout=None,
         pool_connect_timeout=None,
         read_timeout=None,
+        sync_sem=None
     ):
         auth_requests.read_request_auth(forced=True) if sign else None
 
         headers = self._create_headers(headers, url, sign) if headers is None else None
         cookies = self._create_cookies() if cookies is None else None
         json = json or None
         params = params or None
@@ -234,14 +258,15 @@
                 else None
             ),
             reraise=True,
         ):
             r = None
             with _:
                 sync_sem.acquire()
+                time.sleep(sleeper.sleep) if sleeper.sleep else None
                 try:
                     r = self._httpx_funct(
                         method,
                         timeout=httpx.Timeout(
                             total_timeout or self._total_timeout,
                             connect=connect_timeout or self._connect_timeout,
                             pool=pool_connect_timeout or self._pool_connect_timeout,
@@ -318,14 +343,15 @@
                 else None
             ),
             reraise=True,
         ):
             with _:
                 r = None
                 await sem.acquire()
+                await asyncio.sleep(sleeper.sleep) if sleeper.sleep else None
                 try:
                     headers = (
                         self._create_headers(headers, url, sign)
                         if headers is None
                         else headers
                     )
                     cookies = self._create_cookies() if cookies is None else None
```

### Comparing `ofscraper-3.9.1/ofscraper/classes/table.py` & `ofscraper-3.9.2/ofscraper/classes/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/commands/check.py` & `ofscraper-3.9.2/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/commands/manual.py` & `ofscraper-3.9.2/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/commands/scraper.py` & `ofscraper-3.9.2/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/const/config.py` & `ofscraper-3.9.2/ofscraper/const/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/const/constants.py` & `ofscraper-3.9.2/ofscraper/const/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/const/general.py` & `ofscraper-3.9.2/ofscraper/const/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/const/other_url.py` & `ofscraper-3.9.2/ofscraper/const/other_url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/const/prompts.py` & `ofscraper-3.9.2/ofscraper/const/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/const/req.py` & `ofscraper-3.9.2/ofscraper/const/req.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 PROXY_MOUNTS = None
 PROXY_AUTH = None
 maxChunkSize = 1024 * 1024 * 10
 maxChunkSizeB = 1024 * 1024
 CHUNK_ITER = 10
 
 REQ_SEMAPHORE_MULTI = 5
-API_REQ_SEM_MAX = 12
+API_REQ_SEM_MAX = 8
 SCRAPE_PAID_SEMS = 10
 SUBSCRIPTION_SEMS = 5
 API_REQ_CHECK_MAX = 12
 LIKE_MAX_SEMS = 12
 MAX_SEMS_BATCH_DOWNLOAD = 12
 MAX_SEMS_SINGLE_THREAD_DOWNLOAD = 50
 MPD_MAX_SEMS = 4
 SESSION_MANAGER_SYNC_SEM_DEFAULT = 3
 SESSION_MANAGER_SEM_DEFAULT = 10
 
 OF_MIN_WAIT_SESSION_DEFAULT = 4
 OF_MAX_WAIT_SESSION_DEFAULT = 20
-OF_MIN_WAIT_EXPONENTIAL_SESSION_DEFAULT = 12
+OF_MIN_WAIT_EXPONENTIAL_SESSION_DEFAULT = 16
 OF_MAX_WAIT_EXPONENTIAL_SESSION_DEFAULT = 128
 OF_NUM_RETRIES_SESSION_DEFAULT = 10
 
 
 OF_MIN_WAIT_API = 10
 OF_MAX_WAIT_API = 20
 OF_AUTH_MIN_WAIT = 3
@@ -65,12 +65,13 @@
 
 
 MAX_THREAD_WORKERS = 20
 API_MAX_AREAS = 2
 API_TIMEOUT_PER_TASK = 500
 API_REQUEST_THREADONLY = ["Windows", "Linux", "Darwin"]
 
+SESSION_SLEEP_INIT=8
 # page must be 50 post, and 50 is a reasonable size for max number of pages
 REASONABLE_MAX_PAGE = 50
 MIN_PAGE_POST_COUNT = 50
 # messages
 REASONABLE_MAX_PAGE_MESSAGES = 80
```

### Comparing `ofscraper-3.9.1/ofscraper/const/test_constants.py` & `ofscraper-3.9.2/ofscraper/const/test_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -7328,15 +7328,15 @@
     "date",
     "metadata",
     "filter",
     "responsetype",
     "mp4decrypt",
     "discord",
     "ffmpeg",
-    "space-replacer",
+    "space_replacer",
     "code-execution",
     "threads",
     "custom",
     "private-key",
     "client-id",
     "key-mode-default",
     "dynamic-mode-default",
```

### Comparing `ofscraper-3.9.1/ofscraper/const/url.py` & `ofscraper-3.9.2/ofscraper/const/url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/db/operations.py` & `ofscraper-3.9.2/ofscraper/db/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import logging
 import pathlib
 import shutil
-import traceback
 
 import arrow
 from rich.console import Console
 
 import ofscraper.classes.labels as labels
 import ofscraper.classes.placeholder as placeholder
 import ofscraper.utils.cache as cache
@@ -103,15 +102,16 @@
         "posts_pinned",
         "products_model_id",
         "other_model_id",
         "stories_model_id",
         "messages_model_id",
         "labels_model_id",
         "media_posted_at",
-        "media_unlocked"
+        "media_unlocked",
+        "media_duration"
     ]
 
     groupB = [
         "profile_username_constraint_modified",
         "stories_model_id_constraint_added",
         "media_model_id_constraint_added",
         "labels_model_id_constraint_added",
```

### Comparing `ofscraper-3.9.1/ofscraper/db/operations_/labels.py` & `ofscraper-3.9.2/ofscraper/db/operations_/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/db/operations_/media.py` & `ofscraper-3.9.2/ofscraper/db/operations_/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/db/operations_/merge.py` & `ofscraper-3.9.2/ofscraper/db/operations_/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/db/operations_/messages.py` & `ofscraper-3.9.2/ofscraper/db/operations_/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/db/operations_/others.py` & `ofscraper-3.9.2/ofscraper/db/operations_/others.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/db/operations_/posts.py` & `ofscraper-3.9.2/ofscraper/db/operations_/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/db/operations_/profile.py` & `ofscraper-3.9.2/ofscraper/db/operations_/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/db/operations_/stories.py` & `ofscraper-3.9.2/ofscraper/db/operations_/stories.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/db/operations_/wrapper.py` & `ofscraper-3.9.2/ofscraper/db/operations_/wrapper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/alt_download.py` & `ofscraper-3.9.2/ofscraper/download/alt_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/alt_downloadbatch.py` & `ofscraper-3.9.2/ofscraper/download/alt_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/download.py` & `ofscraper-3.9.2/ofscraper/download/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/downloadbatch.py` & `ofscraper-3.9.2/ofscraper/download/downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/downloadnormal.py` & `ofscraper-3.9.2/ofscraper/download/downloadnormal.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/main_download.py` & `ofscraper-3.9.2/ofscraper/download/main_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/main_downloadbatch.py` & `ofscraper-3.9.2/ofscraper/download/main_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/classes/retries.py` & `ofscraper-3.9.2/ofscraper/download/shared/classes/retries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/classes/session.py` & `ofscraper-3.9.2/ofscraper/download/shared/classes/session.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/common/alt_common.py` & `ofscraper-3.9.2/ofscraper/download/shared/common/alt_common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/common/general.py` & `ofscraper-3.9.2/ofscraper/download/shared/common/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/common/main_common.py` & `ofscraper-3.9.2/ofscraper/download/shared/common/main_common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/globals.py` & `ofscraper-3.9.2/ofscraper/download/shared/globals.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/utils/keyhelpers.py` & `ofscraper-3.9.2/ofscraper/download/shared/utils/keyhelpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/utils/log.py` & `ofscraper-3.9.2/ofscraper/download/shared/utils/log.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/utils/message.py` & `ofscraper-3.9.2/ofscraper/download/shared/utils/message.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/utils/metadata.py` & `ofscraper-3.9.2/ofscraper/download/shared/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/utils/paths.py` & `ofscraper-3.9.2/ofscraper/download/shared/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/download/shared/utils/text.py` & `ofscraper-3.9.2/ofscraper/download/shared/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/filters/media/helpers.py` & `ofscraper-3.9.2/ofscraper/filters/media/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import re
 
 import arrow
 
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.constants as constants
 import ofscraper.utils.settings as settings
+from ofscraper.utils.logs.helpers import is_trace
+
 
 log = logging.getLogger("shared")
 
 
 def sort_media(media):
     return sorted(media, key=lambda x: x.date)
 
@@ -201,14 +203,16 @@
     elif item_sort == "filename-asc":
         return sorted(media, key=lambda x: x.filename)
     elif item_sort == "filename-desc":
         return sorted(media, key=lambda x: x.filename, reverse=True)
 
 
 def trace_log_media(count, media, filter_str):
+    if not is_trace():
+        return
     chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
     logformater = "{} id: {} postid: {} data: {} "
     for i in range(1, len(media) + 1, chunk_size):
         # Calculate end index considering potential last chunk being smaller
         end_index = min(i + chunk_size - 1, len(media))  # Adjust end_index calculation
         chunk = media[i - 1 : end_index]  # Adjust slice to start at i-1
         log.trace(
@@ -226,14 +230,16 @@
         )
         # Check if there are more elements remaining after this chunk
         if i + chunk_size > len(media):
             break  # Exit the loop if we've processed all elements
 
 
 def trace_log_post(count, media, filter_str):
+    if not is_trace():
+        return
     chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
     logformater = "{} id: {} data: {} "
     for i in range(1, len(media) + 1, chunk_size):
         # Calculate end index considering potential last chunk being smaller
         end_index = min(i + chunk_size - 1, len(media))  # Adjust end_index calculation
         chunk = media[i - 1 : end_index]  # Adjust slice to start at i-1
         log.trace(
```

### Comparing `ofscraper-3.9.1/ofscraper/filters/media/main.py` & `ofscraper-3.9.2/ofscraper/filters/media/main.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/filters/models/date.py` & `ofscraper-3.9.2/ofscraper/filters/models/date.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,71 +3,83 @@
 """
 
 import logging
 
 import arrow
 
 import ofscraper.utils.args.read as read_args
+from ofscraper.filters.models.helpers import trace_log_user
+
 
 
 def dateFilters(filterusername):
     log = logging.getLogger("shared")
 
-    log.debug(f"Last Seen After Filter: {read_args.retriveArgs().last_seen_after}")
+    log.debug(f"Last seen after filter: {read_args.retriveArgs().last_seen_after}")
     if read_args.retriveArgs().last_seen_after:
         filterusername = list(
             filter(
                 lambda x: x.final_last_seen >= read_args.retriveArgs().last_seen_after,
                 filterusername,
             )
         )
-        log.debug(f"last seen after username count: {len(filterusername)}")
-    log.debug(f"Last Seen Before Filter: {read_args.retriveArgs().last_seen_before}")
+        log.debug(f"Last seen after filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"last seen after")
+    log.debug(f"Last seen before filter: {read_args.retriveArgs().last_seen_before}")
     if read_args.retriveArgs().last_seen_before:
         filterusername = list(
             filter(
                 lambda x: x.final_last_seen <= read_args.retriveArgs().last_seen_before,
                 filterusername,
             )
         )
-        log.debug(f"last seen before username count: {len(filterusername)}")
+        log.debug(f"last seen before filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"last seen before")
+
 
-    log.debug(f"Subscribed After Filter: {read_args.retriveArgs().subscribed_after}")
+    log.debug(f"Subscribed after filter: {read_args.retriveArgs().subscribed_after}")
     if read_args.retriveArgs().subscribed_after:
         filterusername = list(
             filter(
                 lambda x: arrow.get(x.subscribed)
                 >= read_args.retriveArgs().subscribed_after,
                 filterusername,
             )
         )
-        log.debug(f"subscribed after username count: {len(filterusername)}")
-    log.debug(f"Subscribed Before Filter: {read_args.retriveArgs().subscribed_before}")
+        log.debug(f"subscribed after filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"subscribed after")
+
+    log.debug(f"Subscribed before filter: {read_args.retriveArgs().subscribed_before}")
     if read_args.retriveArgs().subscribed_before:
         filterusername = list(
             filter(
                 lambda x: x.final_last_seen
                 <= read_args.retriveArgs().subscribed_before,
                 filterusername,
             )
         )
-        log.debug(f"subscribed before username count: {len(filterusername)}")
+        log.debug(f"subscribed before filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"Subscribed before")
+
     log.debug(f"Expired After Filter: {read_args.retriveArgs().expired_after}")
     if read_args.retriveArgs().expired_after:
         filterusername = list(
             filter(
                 lambda x: arrow.get(x.expired) >= read_args.retriveArgs().expired_after,
                 filterusername,
             )
         )
-        log.debug(f"expired after username count: {len(filterusername)}")
+        log.debug(f"expired after filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"expired after")
+
     log.debug(f"Expired Before Filter: {read_args.retriveArgs().expired_before}")
     if read_args.retriveArgs().expired_before:
         filterusername = list(
             filter(
                 lambda x: arrow.get(x.expired)
                 <= read_args.retriveArgs().expired_before,
                 filterusername,
             )
         )
-        log.debug(f"expired before username count: {len(filterusername)}")
+        log.debug(f"expired before filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"expired before")
     return filterusername
```

### Comparing `ofscraper-3.9.1/ofscraper/filters/models/other.py` & `ofscraper-3.9.2/ofscraper/filters/models/other.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 other filters
 """
 
 import logging
 
 import ofscraper.utils.args.read as read_args
+from ofscraper.filters.models.helpers import trace_log_user
 
 
 def otherFilters(filterusername):
     log = logging.getLogger("shared")
     log.debug(f"Excluded usernames: {read_args.retriveArgs().excluded_username}")
     if len(read_args.retriveArgs().excluded_username) > 0:
         filterusername = list(
             filter(
                 lambda x: x.name not in read_args.retriveArgs().excluded_username,
                 filterusername,
             )
         )
-        log.debug(f"excluded username count: {len(filterusername)}")
+        log.debug(f"'excluded usernames' filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"Excluded usernames")
 
     return filterusername
```

### Comparing `ofscraper-3.9.1/ofscraper/filters/models/price.py` & `ofscraper-3.9.2/ofscraper/filters/models/price.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,162 +1,186 @@
 import logging
 
 import ofscraper.utils.args.read as read_args
+from ofscraper.filters.models.helpers import trace_log_user
 
 
 def pricePaidFreeFilterHelper(filterusername):
     log = logging.getLogger("shared")
 
-    log.debug(f"Current Price Filter: {read_args.retriveArgs().current_price}")
+    log.debug(f"Current price filter: {read_args.retriveArgs().current_price}")
     if read_args.retriveArgs().current_price == "paid":
         filterusername = list(
             filter(
                 lambda x: x.final_current_price > 0,
                 filterusername,
             )
         )
-        log.debug(f"currently paid filter username count: {len(filterusername)}")
+        log.debug(f"Currently paid filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"currently paid filter")
+
     elif read_args.retriveArgs().current_price == "free":
         filterusername = list(
             filter(
                 lambda x: x.final_current_price == 0,
                 filterusername,
             )
         )
         log.debug(f"currently free filter username count: {len(filterusername)}")
-    log.debug(f"Account Renewal Price Filter: {read_args.retriveArgs().renewal_price}")
+        trace_log_user(filterusername,"currently free filter")
+
+    log.debug(f"Account renewal price filter: {read_args.retriveArgs().renewal_price}")
     if read_args.retriveArgs().renewal_price == "paid":
         filterusername = list(
             filter(
                 lambda x: x.final_renewal_price > 0,
                 filterusername,
             ),
         )
 
-        log.debug(f"paid renewal filter username count: {len(filterusername)}")
+        log.debug(f"Paid renewal filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"paid renewal filter")
+
     elif read_args.retriveArgs().renewal_price == "free":
         filterusername = list(
             filter(
                 lambda x: x.final_renewal_price == 0,
                 filterusername,
             )
         )
-        log.debug(f"free renewal filter username count: {len(filterusername)}")
+        log.debug(f"Free renewal filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"free renewal filter")
 
-    log.debug(f"Regular Price Filter: {read_args.retriveArgs().regular_price}")
+    log.debug(f"Regular Price filter: {read_args.retriveArgs().regular_price}")
     if read_args.retriveArgs().regular_price == "paid":
         filterusername = list(filter(lambda x: x.final_regular_price, filterusername))
-        log.debug(f"paid regular price filter username count: {len(filterusername)}")
+        log.debug(f"Paid regular price filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"paid regular price filter")
+    
     elif read_args.retriveArgs().regular_price == "free":
         filterusername = list(
             filter(lambda x: x.final_regular_price == 0, filterusername)
         )
-        log.debug(f"free regular price filter username count: {len(filterusername)}")
-    log.debug(f"Promo Price Filter: {read_args.retriveArgs().promo_price}")
+        log.debug(f"Free regular price filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"free regular price filter")
+    log.debug(f"Promo price filter: {read_args.retriveArgs().promo_price}")
     if read_args.retriveArgs().promo_price == "paid":
         filterusername = list(
             filter(
                 lambda x: x.final_promo_price > 0,
                 filterusername,
             )
         )
 
-        log.debug(f"paid promo filter username count: {len(filterusername)}")
+        log.debug(f"Paid promo price filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"paid promo price filter")
+
     elif read_args.retriveArgs().promo_price == "free":
         filterusername = list(
             filter(
                 lambda x: x.final_promo_price == 0,
                 filterusername,
             )
         )
-        log.debug(f"free promo filter username count: {len(filterusername)}")
+        log.debug(f"Free promo price filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"free promo price filter")
+
     filterusername = priceMinMaxFilters(filterusername)
 
     return filterusername
 
 
 def priceMinMaxFilters(filterusername):
     log = logging.getLogger("shared")
-    log.debug(f"Promo Price min Filter: {read_args.retriveArgs().promo_price_min}")
+    log.debug(f"Promo price min filter: {read_args.retriveArgs().promo_price_min}")
     if read_args.retriveArgs().promo_price_min:
         filterusername = list(
             filter(
                 lambda x: x.final_promo_price
                 >= read_args.retriveArgs().promo_price_min,
                 filterusername,
             )
         )
-        log.debug(f"currently promo min filter: {len(filterusername)}")
-    log.debug(f"Promo Price max Filter: {read_args.retriveArgs().promo_price_max}")
+        log.debug(f"Promo price min filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"promo price min filter")
+
+    log.debug(f"Promo price max filter: {read_args.retriveArgs().promo_price_max}")
     if read_args.retriveArgs().promo_price_max:
         filterusername = list(
             filter(
                 lambda x: x.final_promo_price
                 <= read_args.retriveArgs().promo_price_max,
                 filterusername,
             )
         )
-        log.debug(f"currently promo max filter: {len(filterusername)}")
+        log.debug(f"Promo price max filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"promo price max filter")
 
-    log.debug(f"Regular Price min Filter: {read_args.retriveArgs().regular_price_min}")
+    log.debug(f"Regular price min filter: {read_args.retriveArgs().regular_price_min}")
     if read_args.retriveArgs().regular_price_min:
         filterusername = list(
             filter(
                 lambda x: x.final_regular_price
                 >= read_args.retriveArgs().regular_price_min,
                 filterusername,
             )
         )
-        log.debug(f"currently regular min filter: {len(filterusername)}")
-    log.debug(f"Regular Price max Filter: {read_args.retriveArgs().regular_price_max}")
+        log.debug(f"Regular price min filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"regular price min filter")
+    log.debug(f"Regular price max filter: {read_args.retriveArgs().regular_price_max}")
     if read_args.retriveArgs().regular_price_max:
         filterusername = list(
             filter(
                 lambda x: x.final_regular_price
                 <= read_args.retriveArgs().regular_price_max,
                 filterusername,
             )
         )
-        log.debug(f"currently regular max filter: {len(filterusername)}")
+        log.debug(f"Regular price max filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"regular price max filter")
 
-    log.debug(f"Renewal Price min Filter: {read_args.retriveArgs().renewal_price_min}")
+    log.debug(f"Renewal price min filter: {read_args.retriveArgs().renewal_price_min}")
     if read_args.retriveArgs().renewal_price_min:
         filterusername = list(
             filter(
                 lambda x: x.final_renewal_price
                 >= read_args.retriveArgs().renewal_price_min,
                 filterusername,
             )
         )
-        log.debug(f"currently renewal min filter: {len(filterusername)}")
-    log.debug(f"Renewal Price max Filter: {read_args.retriveArgs().renewal_price_max}")
+        log.debug(f"Renewal price min filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"renewal price min filter")
+    log.debug(f"Renewal price max filter: {read_args.retriveArgs().renewal_price_max}")
     if read_args.retriveArgs().renewal_price_max:
         filterusername = list(
             filter(
                 lambda x: x.final_renewal_price
                 <= read_args.retriveArgs().renewal_price_max,
                 filterusername,
             )
         )
-        log.debug(f"currently renewal max filter: {len(filterusername)}")
+        log.debug(f"Renewal price max filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"renewal price max filter")
 
-    log.debug(f"Current Price min Filter: {read_args.retriveArgs().current_price_min}")
+    log.debug(f"Current price min filter: {read_args.retriveArgs().current_price_min}")
     if read_args.retriveArgs().current_price_min:
         filterusername = list(
             filter(
                 lambda x: x.final_current_price
                 >= read_args.retriveArgs().current_price_min,
                 filterusername,
             )
         )
-        log.debug(f"currently current min filter: {len(filterusername)}")
-    log.debug(f"Current Price max Filter: {read_args.retriveArgs().current_price_max}")
+        log.debug(f"Current price min filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"current price min filter")
+    log.debug(f"Current price max filter: {read_args.retriveArgs().current_price_max}")
     if read_args.retriveArgs().current_price_max:
         filterusername = list(
             filter(
                 lambda x: x.final_current_price
                 <= read_args.retriveArgs().current_price_max,
                 filterusername,
             )
         )
-        log.debug(f"currently current max filter: {len(filterusername)}")
+        log.debug(f"current price max filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"current price max filter")
     return filterusername
```

### Comparing `ofscraper-3.9.1/ofscraper/filters/models/sort.py` & `ofscraper-3.9.2/ofscraper/filters/models/sort.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import ofscraper.utils.args.read as read_args
+import logging
 
 
 def sort_models_helper(models):
     sort = read_args.retriveArgs().sort
     reverse = read_args.retriveArgs().desc
+    logging.getLogger("shared").debug(f"sorting details  [name:{sort} direction:{reverse}]")
     if sort == "name":
         return sorted(models, reverse=reverse, key=lambda x: x.name)
 
     elif sort == "last-seen":
         return sorted(
             models,
             reverse=reverse,
```

### Comparing `ofscraper-3.9.1/ofscraper/filters/models/subtype.py` & `ofscraper-3.9.2/ofscraper/filters/models/subtype.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import logging
 
 import ofscraper.utils.args.read as read_args
+from ofscraper.filters.models.helpers import trace_log_user
+
 
 
 def subType(filterusername):
     log = logging.getLogger("shared")
     log.debug(f"Renewal: {read_args.retriveArgs().renewal}")
     if read_args.retriveArgs().renewal:
         filterusername = list(filter(lambda x: x.renewed, filterusername))
         log.debug(f"active renewal filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"active renewal filter")
+
     elif read_args.retriveArgs().renewal is False:
         filterusername = list(filter(lambda x: not x.renewed, filterusername))
         log.debug(f"disabled renewal filter username counta: {len(filterusername)}")
-    log.debug(f"Sub Status: {read_args.retriveArgs().sub_status}")
+        trace_log_user(filterusername,"disabled renewal filter")
+    
+    log.debug(f"Sub status: {read_args.retriveArgs().sub_status}")
     if read_args.retriveArgs().sub_status:
         filterusername = list(filter(lambda x: x.active, filterusername))
-        log.debug(f"active subscribtion filter username count: {len(filterusername)}")
+        log.debug(f"active subscription filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"active subscription filter")
 
     elif read_args.retriveArgs().sub_status is False:
         filterusername = list(filter(lambda x: not x.active, filterusername))
-        log.debug(f"expired subscribtion filter username count: {len(filterusername)}")
+        log.debug(f"expired subscription filter username count: {len(filterusername)}")
+        trace_log_user(filterusername,"expired subscription filter")
+
     return filterusername
```

### Comparing `ofscraper-3.9.1/ofscraper/models/retriver.py` & `ofscraper-3.9.2/ofscraper/models/retriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 async def get_via_individual():
     out = await individual.get_subscription()
     console.get_shared_console().print(
         "[yellow]Warning: Numbering on OF site can be iffy\nExample Including deactived accounts in expired\nSee: https://of-scraper.gitbook.io/of-scraper/faq#number-of-users-doesnt-match-account-number[/yellow]"
     )
     models_objects = list(map(lambda x: models.Model(x), out))
     if len(models_objects) == 0:
-        raise Exception("Provided usernames with did not yield any valid models")
+        raise Exception("Provided usernames did not yield any valid models")
     return models_objects
 
 
 def get_selected_model(parsed_subscriptions: list) -> tuple:
     """
     Prints user's subscriptions to console and accepts input from user corresponding
     to the model(s) whose content they would like to scrape.
```

### Comparing `ofscraper-3.9.1/ofscraper/models/selector.py` & `ofscraper-3.9.2/ofscraper/models/selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         read_args.retriveArgs().usernames = list(map(lambda x: x.name, selectedusers))
         PARSED_SUBS = selectedusers
         write_args.setArgs(args)
     elif "ALL" in args.usernames:
         PARSED_SUBS = filterNSort()
     elif args.usernames:
         usernameset = set(args.usernames)
-        PARSED_SUBS = list(filter(lambda x: x.name in usernameset, ALL_SUBS))
+        PARSED_SUBS = list(filter(lambda x: x.name or x.id in usernameset, ALL_SUBS))
     return PARSED_SUBS
 
 
 def setfilter(forced=False):
     global args
     while True:
         choice = prompts.decide_filters_menu()
```

### Comparing `ofscraper-3.9.1/ofscraper/prompts/helpers/model_helpers.py` & `ofscraper-3.9.2/ofscraper/prompts/helpers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/helpers/prompt_helpers.py` & `ofscraper-3.9.2/ofscraper/prompts/helpers/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/keybindings.py` & `ofscraper-3.9.2/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/promptConvert.py` & `ofscraper-3.9.2/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/actions.py` & `ofscraper-3.9.2/ofscraper/prompts/prompt_groups/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/area.py` & `ofscraper-3.9.2/ofscraper/prompts/prompt_groups/area.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/auth.py` & `ofscraper-3.9.2/ofscraper/prompts/prompt_groups/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/binary.py` & `ofscraper-3.9.2/ofscraper/prompts/prompt_groups/binary.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/config.py` & `ofscraper-3.9.2/ofscraper/prompts/prompt_groups/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     metadata: path to save db files
     discord: discord hook for logging
     -----------------------------------
     [File Options]:
     save_location: root directory for files
     dir_format: format of directories
     textlength: max length of text placeholder
-    space-replacer: space replacement for filenames
+    space_replacer: space replacement for filenames
     date: date format for placeholders
     text_type_default: toggle for word count type
     trunication_default: toggle for trunicating filenames
     audio: optional overwrites for audio
     videos: optional overwrites for video
     images: optional overwrties from images
     -----------------------------------
@@ -234,15 +234,15 @@
                 "default": data.get_textlength(),
                 "min_allowed": 0,
                 "validate": EmptyInputValidator(),
             },
             {
                 "type": "input",
                 "name": "space-replacer",
-                "message": "space-replacer: ",
+                "message": "space_replacer: ",
                 "option_instruction": "Replace any spaces in text with this character\n",
                 "default": data.get_spacereplacer(),
             },
             {
                 "type": "input",
                 "name": "date",
                 "message": "date: ",
```

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/menu.py` & `ofscraper-3.9.2/ofscraper/prompts/prompt_groups/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/merge.py` & `ofscraper-3.9.2/ofscraper/prompts/prompt_groups/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/model.py` & `ofscraper-3.9.2/ofscraper/prompts/prompt_groups/model.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/profile.py` & `ofscraper-3.9.2/ofscraper/prompts/prompt_groups/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.9.2/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.9.2/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/prompts/prompts.py` & `ofscraper-3.9.2/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/runner/exit.py` & `ofscraper-3.9.2/ofscraper/runner/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/runner/load.py` & `ofscraper-3.9.2/ofscraper/runner/load.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/runner/run.py` & `ofscraper-3.9.2/ofscraper/runner/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/actions.py` & `ofscraper-3.9.2/ofscraper/utils/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/areas.py` & `ofscraper-3.9.2/ofscraper/utils/args/areas.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/groups/common_args.py` & `ofscraper-3.9.2/ofscraper/utils/args/groups/common_args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/groups/main_args.py` & `ofscraper-3.9.2/ofscraper/utils/args/groups/main_args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/groups/manual_args.py` & `ofscraper-3.9.2/ofscraper/utils/args/groups/manual_args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/groups/message_args.py` & `ofscraper-3.9.2/ofscraper/utils/args/groups/message_args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/groups/paid_args.py` & `ofscraper-3.9.2/ofscraper/utils/args/groups/paid_args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/groups/post_args.py` & `ofscraper-3.9.2/ofscraper/utils/args/groups/post_args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/groups/story_args.py` & `ofscraper-3.9.2/ofscraper/utils/args/groups/story_args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/helpers.py` & `ofscraper-3.9.2/ofscraper/utils/args/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/parse.py` & `ofscraper-3.9.2/ofscraper/utils/args/parse.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/read.py` & `ofscraper-3.9.2/ofscraper/utils/args/read.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/args/user.py` & `ofscraper-3.9.2/ofscraper/utils/args/user.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/auth/context.py` & `ofscraper-3.9.2/ofscraper/utils/auth/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/auth/data.py` & `ofscraper-3.9.2/ofscraper/utils/auth/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/auth/file.py` & `ofscraper-3.9.2/ofscraper/utils/auth/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/auth/helpers.py` & `ofscraper-3.9.2/ofscraper/utils/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/auth/make.py` & `ofscraper-3.9.2/ofscraper/utils/auth/make.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/auth/request.py` & `ofscraper-3.9.2/ofscraper/utils/auth/request.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/auth/schema.py` & `ofscraper-3.9.2/ofscraper/utils/auth/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/binaries.py` & `ofscraper-3.9.2/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/cache.py` & `ofscraper-3.9.2/ofscraper/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/checkers.py` & `ofscraper-3.9.2/ofscraper/utils/checkers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/config/config.py` & `ofscraper-3.9.2/ofscraper/utils/config/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/config/context.py` & `ofscraper-3.9.2/ofscraper/utils/config/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/config/custom.py` & `ofscraper-3.9.2/ofscraper/utils/config/custom.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/config/data.py` & `ofscraper-3.9.2/ofscraper/utils/config/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 def get_filesize_limit(config=None, mediatype=ModuleNotFoundError):
     if config == False:
         return constants.FILE_SIZE_LIMIT_DEFAULT
     try:
         if config.get("file_size_max") != None:
             size = config.get("file_size_max")
 
-        elif config.get("overwrites", {}).get(mediatype, {}).get("file_size_max"):
-            return config.get("overwrites", {}).get(mediatype, {}).get("file_size_max")
+        elif config.get("overwrites", {}).get((mediatype or "").lower(), {}).get("file_size_max"):
+            return config.get("overwrites", {}).get((mediatype or "").lower(), {}).get("file_size_max")
         elif config.get("download_options", {}).get("file_size_max"):
             size = config.get("download_options", {}).get("file_size_max")
         return parse_size(
             str(
                 size
                 if size != None
                 else constants_attr.getattr("FILE_SIZE_MAX_DEFAULT")
@@ -54,16 +54,16 @@
 
 @wrapper.config_reader
 def get_filesize_min(config=None, mediatype=None):
     if config == False:
         return constants.FILE_SIZE_MIN_DEFAULT
     try:
         size = None
-        if config.get("overwrites", {}).get(mediatype, {}).get("file_size_min"):
-            size = config.get("overwrites", {}).get(mediatype, {}).get("file_size_min")
+        if config.get("overwrites", {}).get((mediatype or "").lower(), {}).get("file_size_min"):
+            size = config.get("overwrites", {}).get((mediatype or "").lower(), {}).get("file_size_min")
         elif config.get("file_size_min") != None:
             size = config.get("file_size_min")
 
         elif config.get("download_options", {}).get("file_size_min"):
             size = config.get("download_options", {}).get("file_size_min")
         return parse_size(
             str(
@@ -79,15 +79,15 @@
 @wrapper.config_reader
 def get_system_freesize(config=None, mediatype=None):
     if config == False:
         return constants.SYSTEM_FREEMIN_DEFAULT
     try:
         return parse_size(
             str(
-                config.get("overwrites", {}).get(mediatype, {}).get("system_free_min")
+                config.get("overwrites", {}).get((mediatype or "").lower(), {}).get("system_free_min")
                 or config.get("system_free_min")
                 or config.get("download_options", {}).get("system_free_min")
                 or constants_attr.getattr("SYSTEM_FREEMIN_DEFAULT")
             )
         )
     except Exception:
         return 0
@@ -292,31 +292,31 @@
 
 
 @wrapper.config_reader
 def responsetype(config=None, mediatype=None):
     if config == False:
         return constants.RESPONSE_TYPE_DEFAULT
     return (
-        config.get("overwrites", {}).get(mediatype, {}).get("responsetype", {})
+        config.get("overwrites", {}).get((mediatype or "").lower(), {}).get("responsetype", {})
         or config.get("responsetype", {})
         or constants_attr.getattr("RESPONSE_TYPE_DEFAULT")
     )
 
 
 @wrapper.config_reader
 def get_timeline_responsetype(config=None, mediatype=None):
     if config == False:
         return constants.RESPONSE_TYPE_DEFAULT["timeline"]
     return (
         config.get("overwrites", {})
-        .get(mediatype, {})
+        .get((mediatype or "").lower(), {})
         .get("responsetype", {})
         .get("post")
         or config.get("overwrites", {})
-        .get(mediatype, {})
+        .get((mediatype or "").lower(), {})
         .get("responsetype", {})
         .get("timeline")
         or config.get("timeline")
         or config.get("post")
         or config.get("responsetype", {}).get("timeline")
         or config.get("responsetype", {}).get("post")
         or constants_attr.getattr("RESPONSE_TYPE_DEFAULT")["timeline"]
@@ -325,138 +325,139 @@
 
 @wrapper.config_reader
 def get_post_responsetype(config=None, mediatype=None):
     if config == False:
         return constants.RESPONSE_TYPE_DEFAULT["timeline"]
     return (
         config.get("overwrites", {})
-        .get(mediatype, {})
+        .get((mediatype or "").lower(), {})
         .get("responsetype", {})
         .get("post")
-        or config.get("overwrites", {}).get(mediatype, {})
+        or config.get("overwrites", {}).get((mediatype or "").lower(), {})
         or config.get("post")
         or config.get("timeline").get("responsetype", {}).get("timeline")
         or config.get("responsetype", {}).get("post")
         or config.get("responsetype", {}).get("timeline")
         or constants_attr.getattr("RESPONSE_TYPE_DEFAULT")["timeline"]
     )
 
 
 @wrapper.config_reader
 def get_archived_responsetype(config=None, mediatype=None):
     if config == False:
         return constants.RESPONSE_TYPE_DEFAULT["archived"]
     return (
         config.get("overwrites", {})
-        .get(mediatype, {})
+        .get((mediatype or "").lower(), {})
         .get("responsetype", {})
         .get("archived")
         or config.get("archived")
         or config.get("responsetype", {}).get("archived")
         or constants_attr.getattr("RESPONSE_TYPE_DEFAULT")["archived"]
     )
 
 
 @wrapper.config_reader
 def get_stories_responsetype(config=None, mediatype=None):
     if config == False:
         return constants.RESPONSE_TYPE_DEFAULT["stories"]
     return (
         config.get("overwrites", {})
-        .get(mediatype, {})
+        .get((mediatype or "").lower(), {})
         .get("responsetype", {})
         .get("stories")
         or config.get("stories")
         or config.get("responsetype", {}).get("stories")
         or constants_attr.getattr("RESPONSE_TYPE_DEFAULT")["stories"]
     )
 
 
 @wrapper.config_reader
 def get_highlights_responsetype(config=None, mediatype=None):
     if config == False:
         return constants.RESPONSE_TYPE_DEFAULT["highlights"]
     return (
         config.get("overwrites", {})
-        .get(mediatype, {})
+        .get((mediatype or "").lower(), {})
         .get("responsetype", {})
         .get("highlights")
         or config.get("highlights")
         or config.get("responsetype", {}).get("highlights")
         or constants_attr.getattr("RESPONSE_TYPE_DEFAULT")["highlights"]
     )
 
 
 @wrapper.config_reader
 def get_paid_responsetype(config=None, mediatype=None):
     if config == False:
         return constants.RESPONSE_TYPE_DEFAULT["paid"]
     return (
         config.get("overwrites", {})
-        .get(mediatype, {})
+        .get((mediatype or "").lower(), {})
         .get("responsetype", {})
         .get("paid")
         or config.get("paid")
         or config.get("responsetype", {}).get("paid")
         or constants_attr.getattr("RESPONSE_TYPE_DEFAULT")["paid"]
     )
 
 
 @wrapper.config_reader
 def get_messages_progress_responsetype(config=None, mediatype=None):
     if config == False:
         return constants.RESPONSE_TYPE_DEFAULT["message"]
     return (
         config.get("overwrites", {})
-        .get(mediatype, {})
+        .get((mediatype or "").lower(), {})
         .get("responsetype", {})
         .get("message")
         or config.get("message")
         or config.get("responsetype", {}).get("message")
         or constants_attr.getattr("RESPONSE_TYPE_DEFAULT")["message"]
     )
 
 
 @wrapper.config_reader
 def get_profile_responsetype(config=None, mediatype=None):
     if config == False:
         return constants.RESPONSE_TYPE_DEFAULT["profile"]
     return (
         config.get("overwrites", {})
-        .get(mediatype, {})
+        .get((mediatype or "").lower(), {})
         .get("responsetype", {})
         .get("profile")
         or config.get("profile")
         or config.get("responsetype", {}).get("profile")
         or constants_attr.getattr("RESPONSE_TYPE_DEFAULT")["profile"]
     )
 
 
 @wrapper.config_reader
 def get_pinned_responsetype(config=None, mediatype=None):
     if config == False:
         return constants.RESPONSE_TYPE_DEFAULT["pinned"]
     return (
         config.get("overwrites", {})
-        .get(mediatype, {})
+        .get((mediatype or "").lower(), {})
         .get("responsetype", {})
         .get("pinned")
         or config.get("pinned")
         or config.get("responsetype", {}).get("pinned")
         or constants_attr.getattr("RESPONSE_TYPE_DEFAULT")["pinned"]
     )
 
 
 @wrapper.config_reader
 def get_spacereplacer(config=None, mediatype=None):
     if config == False:
         return constants.SPACE_REPLACER_DEFAULT
     return (
-        config.get("overwrites", {}).get(f"{mediatype}", {}).get("space-replacer")
-        or config.get("space-replacer")
+        config.get("overwrites", {}).get(f"{mediatype}", {}).get("space_replacer")
+        or config.get("space_replacer")
+        or config.get("file_options", {}).get("space_replacer")
         or config.get("file_options", {}).get("space-replacer")
         or constants_attr.getattr("SPACE_REPLACER_DEFAULT")
     )
 
 
 @wrapper.config_reader
 def get_private_key(config=None):
@@ -525,16 +526,16 @@
     )
 
 
 @wrapper.config_reader
 def get_part_file_clean(config=None, mediatype=None):
     if config == False:
         return constants.RESUME_DEFAULT
-    if config.get("overwrites", {}).get(mediatype, {}).get("auto_resume"):
-        return config.get("overwrites", {}).get(mediatype, {}).get("auto_resume")
+    if config.get("overwrites", {}).get((mediatype or "").lower(), {}).get("auto_resume"):
+        return config.get("overwrites", {}).get((mediatype or "").lower(), {}).get("auto_resume")
     elif config.get("auto_resume"):
         return config.get("auto_resume")
     elif config.get("download_options", {}).get("auto_resume") != None:
         return config.get("download_options", {}).get("auto_resume")
     elif config.get("partfileclean") != None:
         return config.get("partfileclean") == False
     return constants_attr.getattr("RESUME_DEFAULT")
@@ -646,15 +647,15 @@
 
 
 @wrapper.config_reader
 def get_TempDir(config=None, mediatype=None):
     if config == False:
         return constants.TEMP_FOLDER_DEFAULT
     return (
-        config.get("overwrites", {}).get(mediatype, {}).get("temp_dir")
+        config.get("overwrites", {}).get((mediatype or "").lower(), {}).get("temp_dir")
         or config.get("temp_dir")
         or config.get("advanced_options", {}).get("temp_dir")
         or constants_attr.getattr("TEMP_FOLDER_DEFAULT")
     )
 
 
 @wrapper.config_reader
@@ -726,14 +727,14 @@
         return constants_attr.getattr("MAX_COUNT_DEFAULT")
 
 
 @wrapper.config_reader
 def get_hash(config=None, mediatype=None):
     if config == False:
         return constants.HASHED_DEFAULT
-    elif config.get("overwrites", {}).get(mediatype, {}).get("remove_hash_match"):
-        return config.get("overwrites", {}).get(mediatype, {}).get("remove_hash_match")
+    elif config.get("overwrites", {}).get((mediatype or "").lower(), {}).get("remove_hash_match"):
+        return config.get("overwrites", {}).get((mediatype or "").lower(), {}).get("remove_hash_match")
     elif "remove_hash_match" in config:
         return config.get("remove_hash_match")
     elif "remove_hash_match" in config.get("advanced_options", {}):
         return config.get("advanced_options", {}).get("remove_hash_match")
     return constants.HASHED_DEFAULT
```

### Comparing `ofscraper-3.9.1/ofscraper/utils/config/file.py` & `ofscraper-3.9.2/ofscraper/utils/config/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/config/menu.py` & `ofscraper-3.9.2/ofscraper/utils/config/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/config/schema.py` & `ofscraper-3.9.2/ofscraper/utils/config/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         "metadata": data.get_metadata(config=config),
         "discord": data.get_discord(config=config),
         "file_options": {
             "save_location": common_paths.get_save_location(config=config),
             "dir_format": data.get_dirformat(config=config),
             "file_format": data.get_fileformat(config=config),
             "textlength": data.get_textlength(config=config),
-            "space-replacer": data.get_spacereplacer(config=config),
+            "space_replacer": data.get_spacereplacer(config=config),
             "date": data.get_date(config=config),
             "text_type_default": data.get_textType(config=config),
             "truncation_default": data.get_truncation(config=config),
         },
         "download_options": {
             "file_size_limit": data.get_filesize_limit(config=config),
             "file_size_min": data.get_filesize_min(config=config),
```

### Comparing `ofscraper-3.9.1/ofscraper/utils/constants.py` & `ofscraper-3.9.2/ofscraper/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/context/exit.py` & `ofscraper-3.9.2/ofscraper/utils/context/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/context/run_async.py` & `ofscraper-3.9.2/ofscraper/utils/context/run_async.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/context/stdout.py` & `ofscraper-3.9.2/ofscraper/utils/context/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/dates.py` & `ofscraper-3.9.2/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/encoding.py` & `ofscraper-3.9.2/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/hash.py` & `ofscraper-3.9.2/ofscraper/utils/hash.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/logs/classes.py` & `ofscraper-3.9.2/ofscraper/utils/logs/classes.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/logs/close.py` & `ofscraper-3.9.2/ofscraper/utils/logs/close.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/logs/helpers.py` & `ofscraper-3.9.2/ofscraper/utils/logs/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/logs/logger.py` & `ofscraper-3.9.2/ofscraper/utils/logs/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/logs/logs.py` & `ofscraper-3.9.2/ofscraper/utils/logs/logs.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/logs/other.py` & `ofscraper-3.9.2/ofscraper/utils/logs/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/logs/stdout.py` & `ofscraper-3.9.2/ofscraper/utils/logs/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/manager.py` & `ofscraper-3.9.2/ofscraper/utils/manager.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/menu.py` & `ofscraper-3.9.2/ofscraper/utils/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/merge.py` & `ofscraper-3.9.2/ofscraper/utils/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/paths/check.py` & `ofscraper-3.9.2/ofscraper/utils/paths/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/paths/common.py` & `ofscraper-3.9.2/ofscraper/utils/paths/common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/paths/paths.py` & `ofscraper-3.9.2/ofscraper/utils/paths/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/profiles/data.py` & `ofscraper-3.9.2/ofscraper/utils/profiles/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/profiles/manage.py` & `ofscraper-3.9.2/ofscraper/utils/profiles/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/profiles/tools.py` & `ofscraper-3.9.2/ofscraper/utils/profiles/tools.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/progress.py` & `ofscraper-3.9.2/ofscraper/utils/progress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/run.py` & `ofscraper-3.9.2/ofscraper/utils/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/separate.py` & `ofscraper-3.9.2/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/settings.py` & `ofscraper-3.9.2/ofscraper/utils/settings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/system/network.py` & `ofscraper-3.9.2/ofscraper/utils/system/network.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/system/system.py` & `ofscraper-3.9.2/ofscraper/utils/system/system.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/ofscraper/utils/text.py` & `ofscraper-3.9.2/ofscraper/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.1/pyproject.toml` & `ofscraper-3.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.9.1"
+version = "3.9.2"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.14"
```

### Comparing `ofscraper-3.9.1/PKG-INFO` & `ofscraper-3.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.9.1
+Version: 3.9.2
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ofscraper Version: 3.9.1 Summary: automatically
+Metadata-Version: 2.1 Name: ofscraper Version: 3.9.2 Summary: automatically
 scrape onlyfans Author: datawhores Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: pyinstaller Requires-Dist: aiofiles
 (>=23.2.1,<24.0.0) Requires-Dist: aiohttp[speedups] (>=3.8.5,<4.0.0) Requires-
 Dist: aioprocessing (>=2.0.1,<3.0.0) Requires-Dist: aiosqlite
 (>=0.20.0,<0.21.0) Requires-Dist: arrow (>=1.3.0,<2.0.0) Requires-Dist:
```

