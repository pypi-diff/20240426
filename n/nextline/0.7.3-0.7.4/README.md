# Comparing `tmp/nextline-0.7.3.tar.gz` & `tmp/nextline-0.7.4.tar.gz`

## Comparing `nextline-0.7.3.tar` & `nextline-0.7.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/__about__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/__init__.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/continuous.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/count.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/disable.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/events.py
--rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/py.typed
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/types.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/fsm/__init__.py
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/fsm/factory.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/fsm/state.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/__init__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/hook.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/spec.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/__init__.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/argument.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/registrars/__init__.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/registrars/prompt_info.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/registrars/prompt_notice.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/registrars/run_info.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/registrars/run_no.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/registrars/script.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/registrars/state_name.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/registrars/stdout.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/registrars/trace_info.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/registrars/trace_nos.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/session/__init__.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/session/monitor.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/plugin/plugins/session/session.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/__init__.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/call.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/commands.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/exc.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/path.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/runner.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/types.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/utils.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/hook.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/skip.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/spec.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/__init__.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/_script.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/compose.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/concurrency.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/filter.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/global_.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/local_.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/peek.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/repeat.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/pdb_/__init__.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/pdb_/custom.py
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/pdb_/factory.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/pdb_/prompt.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/spawned/plugin/plugins/pdb_/stream.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/__init__.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/func.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/multiprocessing_logging.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/path.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/peek.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/profile.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/queue.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/run.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/thread_exception.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/thread_task_id.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/timer.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/done_callback/__init__.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/done_callback/task.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/done_callback/thread.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/done_callback/union.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/pubsub/__init__.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/pubsub/broker.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 nextline-0.7.3/nextline/utils/pubsub/item.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 nextline-0.7.3/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline-0.7.3/LICENSE
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 nextline-0.7.3/README.md
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 nextline-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 nextline-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/__about__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/__init__.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/continuous.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/count.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/disable.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/events.py
+-rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/py.typed
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/types.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/fsm/__init__.py
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/fsm/factory.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/fsm/state.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/__init__.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/hook.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/spec.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/__init__.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/argument.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/registrars/__init__.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/registrars/prompt_info.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/registrars/prompt_notice.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/registrars/run_info.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/registrars/run_no.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/registrars/script.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/registrars/state_name.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/registrars/stdout.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/registrars/trace_info.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/registrars/trace_nos.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/session/__init__.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/session/monitor.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/plugin/plugins/session/session.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/__init__.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/call.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/commands.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/exc.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/path.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/runner.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/types.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/utils.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/hook.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/skip.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/spec.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/__init__.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/_script.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/compose.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/concurrency.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/filter.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/global_.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/local_.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/peek.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/repeat.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/pdb_/__init__.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/pdb_/custom.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/pdb_/factory.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/pdb_/prompt.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/spawned/plugin/plugins/pdb_/stream.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/__init__.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/func.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/multiprocessing_logging.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/path.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/peek.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/profile.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/queue.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/run.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/thread_exception.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/thread_task_id.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/timer.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/done_callback/__init__.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/done_callback/task.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/done_callback/thread.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/done_callback/union.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/pubsub/__init__.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/pubsub/broker.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 nextline-0.7.4/nextline/utils/pubsub/item.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 nextline-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline-0.7.4/LICENSE
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 nextline-0.7.4/README.md
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 nextline-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 nextline-0.7.4/PKG-INFO
```

### Comparing `nextline-0.7.3/nextline/continuous.py` & `nextline-0.7.4/nextline/continuous.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/count.py` & `nextline-0.7.4/nextline/count.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/events.py` & `nextline-0.7.4/nextline/events.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/main.py` & `nextline-0.7.4/nextline/main.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/types.py` & `nextline-0.7.4/nextline/types.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/fsm/factory.py` & `nextline-0.7.4/nextline/fsm/factory.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/fsm/state.py` & `nextline-0.7.4/nextline/fsm/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,17 @@
         await self._hook.ahook.kill(context=self._context)
 
     async def on_close_while_running(self, _: EventData) -> None:
         await self.run_finished.wait()
 
     async def wait(self) -> None:
         await self.run_finished.wait()
+    
+    async def on_enter_finished(self, _: EventData) -> None:
+        await self._hook.ahook.on_finished(context=self._context)
 
     async def on_exit_finished(self, _: EventData) -> None:
         await self._task
 
     def format_exception(self) -> Optional[str]:
         return self._hook.hook.format_exception(context=self._context)
```

### Comparing `nextline-0.7.3/nextline/plugin/hook.py` & `nextline-0.7.4/nextline/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/plugin/spec.py` & `nextline-0.7.4/nextline/plugin/spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,14 +105,21 @@
 @hookspec
 async def send_command(context: Context, command: spawned.Command) -> None:
     pass
 
 
 @hookspec
 async def on_end_run(context: Context) -> None:
+    '''The run is about to finish. The state is still 'running'.'''
+    pass
+
+
+@hookspec
+async def on_finished(context: Context) -> None:
+    '''The run has finished. The state is 'finished'.'''
     pass
 
 
 @hookspec(firstresult=True)
 def format_exception(context: Context) -> Optional[str]:
     pass
```

### Comparing `nextline-0.7.3/nextline/plugin/plugins/__init__.py` & `nextline-0.7.4/nextline/plugin/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/plugin/plugins/argument.py` & `nextline-0.7.4/nextline/plugin/plugins/argument.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/plugin/plugins/registrars/__init__.py` & `nextline-0.7.4/nextline/plugin/plugins/registrars/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/plugin/plugins/registrars/prompt_info.py` & `nextline-0.7.4/nextline/plugin/plugins/registrars/prompt_info.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/plugin/plugins/registrars/prompt_notice.py` & `nextline-0.7.4/nextline/plugin/plugins/registrars/prompt_notice.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/plugin/plugins/registrars/run_info.py` & `nextline-0.7.4/nextline/plugin/plugins/registrars/run_info.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/plugin/plugins/registrars/stdout.py` & `nextline-0.7.4/nextline/plugin/plugins/registrars/stdout.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/plugin/plugins/registrars/trace_info.py` & `nextline-0.7.4/nextline/plugin/plugins/registrars/trace_info.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/plugin/plugins/registrars/trace_nos.py` & `nextline-0.7.4/nextline/plugin/plugins/registrars/trace_nos.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/plugin/plugins/session/monitor.py` & `nextline-0.7.4/nextline/plugin/plugins/session/monitor.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/plugin/plugins/session/session.py` & `nextline-0.7.4/nextline/plugin/plugins/session/session.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/__init__.py` & `nextline-0.7.4/nextline/spawned/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/call.py` & `nextline-0.7.4/nextline/spawned/call.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/path.py` & `nextline-0.7.4/nextline/spawned/path.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/runner.py` & `nextline-0.7.4/nextline/spawned/runner.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/types.py` & `nextline-0.7.4/nextline/spawned/types.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/utils.py` & `nextline-0.7.4/nextline/spawned/utils.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/hook.py` & `nextline-0.7.4/nextline/spawned/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/skip.py` & `nextline-0.7.4/nextline/spawned/plugin/skip.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/spec.py` & `nextline-0.7.4/nextline/spawned/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/__init__.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/_script.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/_script.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/compose.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/compose.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/concurrency.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/concurrency.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/filter.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/filter.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/global_.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/global_.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/local_.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/local_.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/peek.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/peek.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/repeat.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/repeat.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/pdb_/custom.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/pdb_/custom.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/pdb_/factory.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/pdb_/factory.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/pdb_/prompt.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/pdb_/prompt.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/spawned/plugin/plugins/pdb_/stream.py` & `nextline-0.7.4/nextline/spawned/plugin/plugins/pdb_/stream.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/__init__.py` & `nextline-0.7.4/nextline/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/func.py` & `nextline-0.7.4/nextline/utils/func.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/multiprocessing_logging.py` & `nextline-0.7.4/nextline/utils/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/peek.py` & `nextline-0.7.4/nextline/utils/peek.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/queue.py` & `nextline-0.7.4/nextline/utils/queue.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/run.py` & `nextline-0.7.4/nextline/utils/run.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/thread_exception.py` & `nextline-0.7.4/nextline/utils/thread_exception.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/thread_task_id.py` & `nextline-0.7.4/nextline/utils/thread_task_id.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/timer.py` & `nextline-0.7.4/nextline/utils/timer.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/done_callback/task.py` & `nextline-0.7.4/nextline/utils/done_callback/task.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/done_callback/thread.py` & `nextline-0.7.4/nextline/utils/done_callback/thread.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/done_callback/union.py` & `nextline-0.7.4/nextline/utils/done_callback/union.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/pubsub/broker.py` & `nextline-0.7.4/nextline/utils/pubsub/broker.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/nextline/utils/pubsub/item.py` & `nextline-0.7.4/nextline/utils/pubsub/item.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/.gitignore` & `nextline-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/LICENSE` & `nextline-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/README.md` & `nextline-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/pyproject.toml` & `nextline-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nextline-0.7.3/PKG-INFO` & `nextline-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nextline
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Python library for controlling Python scripts execution
 Project-URL: Homepage, https://github.com/simonsobs/nextline#readme
 Project-URL: Issues, https://github.com/simonsobs/nextline/issues
 Project-URL: Source, https://github.com/simonsobs/nextline
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE
```

