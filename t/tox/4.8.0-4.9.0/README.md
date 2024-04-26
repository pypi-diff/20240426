# Comparing `tmp/tox-4.8.0.tar.gz` & `tmp/tox-4.9.0.tar.gz`

## Comparing `tox-4.8.0.tar` & `tox-4.9.0.tar`

### file list

```diff
@@ -1,221 +1,221 @@
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tox-4.8.0/tox.ini
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/__main__.py
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/provision.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/py.typed
--rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/pytest.py
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/report.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/run.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/__init__.py
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/main.py
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/of_type.py
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/set_env.py
--rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/sets.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/cli/__init__.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/cli/env_var.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/cli/ini.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/cli/parse.py
--rw-r--r--   0        0        0    13744 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/cli/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/loader/__init__.py
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/loader/api.py
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/loader/convert.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/loader/memory.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/loader/section.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/loader/str_convert.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/loader/stringify.py
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/loader/ini/__init__.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/loader/ini/factor.py
--rw-r--r--   0        0        0    13385 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/loader/ini/replace.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/source/__init__.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/source/api.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/source/discover.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/source/ini.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/source/ini_section.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/source/legacy_toml.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/source/setup_cfg.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/config/source/tox_ini.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/execute/__init__.py
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/execute/api.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/execute/pep517_backend.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/execute/request.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/execute/stream.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/execute/util.py
--rw-r--r--   0        0        0    14187 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/execute/local_sub_process/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/execute/local_sub_process/read_via_thread.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/execute/local_sub_process/read_via_thread_unix.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/execute/local_sub_process/read_via_thread_windows.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/journal/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/journal/env.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/journal/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/plugin/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/plugin/inline.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/plugin/manager.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/plugin/spec.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/__init__.py
--rw-r--r--   0        0        0    18458 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/env_select.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/__init__.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/depends.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/devenv.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/exec_.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/legacy.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/list_env.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/quickstart.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/show_config.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/version_flag.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/run/__init__.py
--rw-r--r--   0        0        0    17665 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/run/common.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/run/parallel.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/run/sequential.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/session/cmd/run/single.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/__init__.py
--rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/api.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/errors.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/info.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/installer.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/package.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/register.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/runner.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/__init__.py
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/api.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/package.py
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/pip/__init__.py
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/pip/pip_install.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/pip/req_file.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/pip/req/__init__.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/pip/req/args.py
--rw-r--r--   0        0        0    19719 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/pip/req/file.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/pip/req/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/virtual_env/api.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/virtual_env/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
--rw-r--r--   0        0        0    18379 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/virtual_env/package/pyproject.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/tox_env/python/virtual_env/package/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/util/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/util/ci.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/util/cpu.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/util/file_view.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/util/graph.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/util/path.py
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 tox-4.8.0/src/tox/util/spinner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/__init__.py
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 tox-4.8.0/tests/conftest.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tox-4.8.0/tests/test_call_modes.py
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 tox-4.8.0/tests/test_provision.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 tox-4.8.0/tests/test_report.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tox-4.8.0/tests/test_run.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.8.0/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/__init__.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/conftest.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/test_main.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/test_of_types.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/test_set_env.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/test_sets.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/cli/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/cli/conftest.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/cli/test_cli_env_var.py
--rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/cli/test_cli_ini.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/cli/test_parse.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/cli/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/__init__.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/test_loader.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/test_memory_loader.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/test_section.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/test_str_convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/__init__.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/conftest.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/test_factor.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/test_ini_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/replace/__init__.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/replace/conftest.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/replace/test_replace.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/replace/test_replace_env_var.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/replace/test_replace_os_pathsep.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/replace/test_replace_os_sep.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/replace/test_replace_posargs.py
--rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/replace/test_replace_tox_env.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/loader/ini/replace/test_replace_tty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/source/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/source/test_discover.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/source/test_legacy_toml.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/source/test_setup_cfg.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tox-4.8.0/tests/config/source/test_source_ini.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 tox-4.8.0/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox-4.8.0/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox-4.8.0/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.8.0/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox-4.8.0/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/execute/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.8.0/tests/execute/conftest.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.8.0/tests/execute/test_request.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.8.0/tests/execute/test_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/execute/local_subprocess/__init__.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tox-4.8.0/tests/execute/local_subprocess/bad_process.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 tox-4.8.0/tests/execute/local_subprocess/local_subprocess_sigint.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox-4.8.0/tests/execute/local_subprocess/test_execute_util.py
--rw-r--r--   0        0        0    14176 2020-02-02 00:00:00.000000 tox-4.8.0/tests/execute/local_subprocess/test_local_subprocess.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tox-4.8.0/tests/execute/local_subprocess/tty_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/journal/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.8.0/tests/journal/test_main_journal.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.8.0/tests/plugin/conftest.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 tox-4.8.0/tests/plugin/test_inline.py
--rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 tox-4.8.0/tests/plugin/test_plugin.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tox-4.8.0/tests/plugin/test_plugin_custom_config_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/pytest_/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 tox-4.8.0/tests/pytest_/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/__init__.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/test_env_select.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/test_session_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/__init__.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/test_depends.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/test_devenv.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/test_exec_.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/test_legacy.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/test_list_envs.py
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/test_parallel.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/test_quickstart.py
--rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/test_sequential.py
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/test_show_config.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/test_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/run/__init__.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tox-4.8.0/tests/session/cmd/run/test_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/test_api.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/test_info.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/test_register.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/test_tox_env_api.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/test_tox_env_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/__init__.py
--rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/test_python_api.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/test_python_runner.py
--rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/pip/test_pip_install.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/pip/test_req_file.py
--rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/pip/req/test_file.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/test-pkg/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/virtual_env/test_setuptools.py
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/virtual_env/package/conftest.py
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
--rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 tox-4.8.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 tox-4.8.0/tests/type_check/add_config_container_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.8.0/tests/util/__init__.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 tox-4.8.0/tests/util/test_ci.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tox-4.8.0/tests/util/test_cpu.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.8.0/tests/util/test_graph.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tox-4.8.0/tests/util/test_path.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 tox-4.8.0/tests/util/test_spinner.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.8.0/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.8.0/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.8.0/README.md
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 tox-4.8.0/pyproject.toml
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tox-4.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 tox-4.9.0/tox.ini
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/__main__.py
+-rw-r--r--   0        0        0     5916 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/provision.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/py.typed
+-rw-r--r--   0        0        0    19388 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/pytest.py
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/report.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/run.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/__init__.py
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/main.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/of_type.py
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/set_env.py
+-rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/sets.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/cli/__init__.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/cli/env_var.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/cli/ini.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/cli/parse.py
+-rw-r--r--   0        0        0    13586 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/cli/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/loader/__init__.py
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/loader/api.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/loader/convert.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/loader/memory.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/loader/section.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/loader/str_convert.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/loader/stringify.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/loader/ini/factor.py
+-rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/loader/ini/replace.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/source/__init__.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/source/api.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/source/discover.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/source/ini.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/source/ini_section.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/source/legacy_toml.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/source/setup_cfg.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/config/source/tox_ini.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/execute/__init__.py
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/execute/api.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/execute/pep517_backend.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/execute/request.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/execute/stream.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/execute/util.py
+-rw-r--r--   0        0        0    14187 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/execute/local_sub_process/__init__.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/execute/local_sub_process/read_via_thread.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/execute/local_sub_process/read_via_thread_unix.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/execute/local_sub_process/read_via_thread_windows.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/journal/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/journal/env.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/journal/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/plugin/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/plugin/inline.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/plugin/manager.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/plugin/spec.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/__init__.py
+-rw-r--r--   0        0        0    19066 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/env_select.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/depends.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/devenv.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/exec_.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/legacy.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/list_env.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/quickstart.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/show_config.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/version_flag.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0    17665 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/run/common.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/run/parallel.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/run/sequential.py
+-rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/session/cmd/run/single.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/__init__.py
+-rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/api.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/errors.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/info.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/installer.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/package.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/register.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/runner.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/__init__.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/api.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/package.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/pip/__init__.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/pip/pip_install.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/pip/req_file.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/pip/req/__init__.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/pip/req/args.py
+-rw-r--r--   0        0        0    19719 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/pip/req/file.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/pip/req/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/virtual_env/api.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/virtual_env/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
+-rw-r--r--   0        0        0    18216 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/virtual_env/package/pyproject.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/tox_env/python/virtual_env/package/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/util/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/util/ci.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/util/cpu.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/util/file_view.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/util/graph.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/util/path.py
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 tox-4.9.0/src/tox/util/spinner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 tox-4.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tox-4.9.0/tests/test_call_modes.py
+-rw-r--r--   0        0        0     9667 2020-02-02 00:00:00.000000 tox-4.9.0/tests/test_provision.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 tox-4.9.0/tests/test_report.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tox-4.9.0/tests/test_run.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.9.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/__init__.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/conftest.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/test_main.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/test_of_types.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/test_set_env.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/test_sets.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/cli/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/cli/conftest.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/cli/test_cli_env_var.py
+-rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/cli/test_cli_ini.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/cli/test_parse.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/cli/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/__init__.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/test_loader.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/test_memory_loader.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/test_section.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/test_str_convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/conftest.py
+-rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/test_factor.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/test_ini_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/replace/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/replace/conftest.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/replace/test_replace.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/replace/test_replace_env_var.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/replace/test_replace_os_pathsep.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/replace/test_replace_os_sep.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/replace/test_replace_posargs.py
+-rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/replace/test_replace_tox_env.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/loader/ini/replace/test_replace_tty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/source/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/source/test_discover.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/source/test_legacy_toml.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/source/test_setup_cfg.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tox-4.9.0/tests/config/source/test_source_ini.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.9.0/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox-4.9.0/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox-4.9.0/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.9.0/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox-4.9.0/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/execute/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.9.0/tests/execute/conftest.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.9.0/tests/execute/test_request.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.9.0/tests/execute/test_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/execute/local_subprocess/__init__.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tox-4.9.0/tests/execute/local_subprocess/bad_process.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 tox-4.9.0/tests/execute/local_subprocess/local_subprocess_sigint.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox-4.9.0/tests/execute/local_subprocess/test_execute_util.py
+-rw-r--r--   0        0        0    14182 2020-02-02 00:00:00.000000 tox-4.9.0/tests/execute/local_subprocess/test_local_subprocess.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tox-4.9.0/tests/execute/local_subprocess/tty_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/journal/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.9.0/tests/journal/test_main_journal.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.9.0/tests/plugin/conftest.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 tox-4.9.0/tests/plugin/test_inline.py
+-rw-r--r--   0        0        0     9288 2020-02-02 00:00:00.000000 tox-4.9.0/tests/plugin/test_plugin.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tox-4.9.0/tests/plugin/test_plugin_custom_config_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/pytest_/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 tox-4.9.0/tests/pytest_/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/__init__.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/test_env_select.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/test_session_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/test_depends.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/test_devenv.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/test_exec_.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/test_legacy.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/test_list_envs.py
+-rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/test_parallel.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/test_quickstart.py
+-rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/test_sequential.py
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/test_show_config.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/test_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tox-4.9.0/tests/session/cmd/run/test_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/test_api.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/test_info.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/test_register.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/test_tox_env_api.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/test_tox_env_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/__init__.py
+-rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/test_python_api.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/test_python_runner.py
+-rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/pip/test_pip_install.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/pip/test_req_file.py
+-rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/pip/req/test_file.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/test-pkg/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/virtual_env/test_setuptools.py
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/virtual_env/package/conftest.py
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
+-rw-r--r--   0        0        0    11304 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 tox-4.9.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 tox-4.9.0/tests/type_check/add_config_container_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.9.0/tests/util/__init__.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 tox-4.9.0/tests/util/test_ci.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tox-4.9.0/tests/util/test_cpu.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.9.0/tests/util/test_graph.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tox-4.9.0/tests/util/test_path.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 tox-4.9.0/tests/util/test_spinner.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.9.0/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.9.0/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.9.0/README.md
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 tox-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 tox-4.9.0/PKG-INFO
```

### Comparing `tox-4.8.0/tox.ini` & `tox-4.9.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 commands =
     pre-commit run --all-files --show-diff-on-failure {posargs}
     python -c 'print(r"hint: run {envbindir}{/}pre-commit install to add checks as pre-commit hook")'
 
 [testenv:type]
 description = run type check on code base
 deps =
-    mypy==1.4.1
-    types-cachetools>=5.3.0.5
+    mypy==1.5
+    types-cachetools>=5.3.0.6
     types-chardet>=5.0.4.6
 commands =
     mypy src/tox
     mypy tests
 
 [testenv:docs]
 description = build documentation
```

### Comparing `tox-4.8.0/src/tox/provision.py` & `tox-4.9.0/src/tox/provision.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """This package handles provisioning an appropriate tox version per requirements."""
 from __future__ import annotations
 
 import json
 import logging
 import sys
+from importlib.metadata import PackageNotFoundError, distribution
 from pathlib import Path
 from typing import TYPE_CHECKING, List, cast
 
 from packaging.requirements import Requirement
 from packaging.utils import canonicalize_name
 from packaging.version import Version
 
@@ -15,19 +16,14 @@
 from tox.execute.api import StdinSource
 from tox.plugin import impl
 from tox.report import HandledError
 from tox.tox_env.errors import Skip
 from tox.tox_env.python.pip.req_file import PythonDeps
 from tox.tox_env.python.runner import PythonRun
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from importlib.metadata import PackageNotFoundError, distribution
-else:  # pragma: no cover (py38+)
-    from importlib_metadata import PackageNotFoundError, distribution
-
 if TYPE_CHECKING:
     from argparse import ArgumentParser
 
     from tox.session.state import State
 
 
 @impl
```

### Comparing `tox-4.8.0/src/tox/pytest.py` & `tox-4.9.0/src/tox/pytest.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,56 +8,44 @@
 import socket
 import sys
 import textwrap
 import warnings
 from contextlib import closing, contextmanager
 from pathlib import Path
 from types import ModuleType, TracebackType
-from typing import TYPE_CHECKING, Any, Callable, Iterator, Sequence, cast
+from typing import TYPE_CHECKING, Any, Callable, Iterator, Protocol, Sequence, cast
 
 import pytest
-from _pytest.capture import CaptureFixture as _CaptureFixture
 from _pytest.fixtures import SubRequest
-from _pytest.logging import LogCaptureFixture
-from _pytest.monkeypatch import MonkeyPatch
-from _pytest.tmpdir import TempPathFactory
 from devpi_process import IndexServer
 from virtualenv.info import fs_supports_symlink
 
 import tox.run
 from tox.execute.api import Execute, ExecuteInstance, ExecuteOptions, ExecuteStatus, Outcome
 from tox.execute.request import ExecuteRequest, shell_cmd
 from tox.plugin import manager
 from tox.report import LOGGER, OutErr
 from tox.run import run as tox_run
 from tox.run import setup_state as previous_setup_state
 from tox.session.cmd.run.parallel import ENV_VAR_KEY
 from tox.tox_env import api as tox_env_api
 from tox.tox_env.api import ToxEnv
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from typing import Protocol
-else:  # pragma: no cover (<py38)
-    from typing_extensions import Protocol
-
 if TYPE_CHECKING:
     from unittest.mock import MagicMock
 
-    from _pytest.config import Config as PyTestConfig
-    from _pytest.config.argparsing import Parser
-    from _pytest.python import Function
     from pytest_mock import MockerFixture
 
     from tox.config.sets import EnvConfigSet
     from tox.execute.stream import SyncWrite
     from tox.session.state import State
 
-    CaptureFixture = _CaptureFixture[str]
+    CaptureFixture = pytest.CaptureFixture[str]
 else:
-    CaptureFixture = _CaptureFixture
+    CaptureFixture = pytest.CaptureFixture
 
 os.environ["PIP_DISABLE_PIP_VERSION_CHECK"] = "1"
 os.environ["PIP_NO_PYTHON_VERSION_WARNING"] = "1"
 
 if fs_supports_symlink():  # pragma: no cover # used to speed up test suite run time where possible
     os.environ["VIRTUALENV_SYMLINK_APP_DATA"] = "1"
     os.environ["VIRTUALENV_SYMLINKS"] = "1"
@@ -116,37 +104,37 @@
             msg += f" miss {miss}"
         if diff:
             msg += f" diff {diff}"
         pytest.fail(msg)
 
 
 @pytest.fixture(autouse=True)
-def check_os_environ_stable(monkeypatch: MonkeyPatch) -> Iterator[None]:  # noqa: PT004
+def check_os_environ_stable(monkeypatch: pytest.MonkeyPatch) -> Iterator[None]:  # noqa: PT004
     with check_os_environ():
         yield
         monkeypatch.undo()
 
 
 @pytest.fixture(autouse=True)
-def no_color(monkeypatch: MonkeyPatch, check_os_environ_stable: None) -> None:  # noqa: ARG001, PT004
+def no_color(monkeypatch: pytest.MonkeyPatch, check_os_environ_stable: None) -> None:  # noqa: ARG001, PT004
     monkeypatch.setenv("NO_COLOR", "yes")
 
 
 class ToxProject:
     def __init__(  # noqa: PLR0913
         self,
         files: dict[str, Any],
         base: Path | None,
         path: Path,
         capfd: CaptureFixture,
-        monkeypatch: MonkeyPatch,
+        monkeypatch: pytest.MonkeyPatch,
         mocker: MockerFixture,
     ) -> None:
         self.path: Path = path
-        self.monkeypatch: MonkeyPatch = monkeypatch
+        self.monkeypatch: pytest.MonkeyPatch = monkeypatch
         self.mocker = mocker
         self._capfd = capfd
         self._setup_files(self.path, base, files)
 
     @staticmethod
     def _setup_files(dest: Path, base: Path | None, content: dict[str, Any]) -> None:
         if base is not None:
@@ -422,74 +410,74 @@
         ...
 
 
 @pytest.fixture(name="tox_project")
 def init_fixture(
     tmp_path: Path,
     capfd: CaptureFixture,
-    monkeypatch: MonkeyPatch,
+    monkeypatch: pytest.MonkeyPatch,
     mocker: MockerFixture,
 ) -> ToxProjectCreator:
     def _init(files: dict[str, Any], base: Path | None = None, prj_path: Path | None = None) -> ToxProject:
         """Create tox  projects."""
         return ToxProject(files, base, prj_path or tmp_path / "p", capfd, monkeypatch, mocker)
 
     return _init
 
 
 @pytest.fixture()
-def empty_project(tox_project: ToxProjectCreator, monkeypatch: MonkeyPatch) -> ToxProject:
+def empty_project(tox_project: ToxProjectCreator, monkeypatch: pytest.MonkeyPatch) -> ToxProject:
     project = tox_project({"tox.ini": ""})
     monkeypatch.chdir(project.path)
     return project
 
 
 _RUN_INTEGRATION_TEST_FLAG = "--run-integration"
 
 
-def pytest_addoption(parser: Parser) -> None:
+def pytest_addoption(parser: pytest.Parser) -> None:
     parser.addoption(_RUN_INTEGRATION_TEST_FLAG, action="store_true", help="run the integration tests")
 
 
-def pytest_configure(config: PyTestConfig) -> None:
+def pytest_configure(config: pytest.Config) -> None:
     config.addinivalue_line("markers", "integration")
     config.addinivalue_line("markers", "plugin_test")
 
 
 @pytest.hookimpl(trylast=True)  # type: ignore[misc] # not typed decorator
-def pytest_collection_modifyitems(config: PyTestConfig, items: list[Function]) -> None:
+def pytest_collection_modifyitems(config: pytest.Config, items: list[pytest.Function]) -> None:
     # do not require flags if called directly
     if len(items) == 1:  # pragma: no cover # hard to test
         return
 
     skip_int = pytest.mark.skip(reason=f"integration tests not run (no {_RUN_INTEGRATION_TEST_FLAG} flag)")
 
-    def is_integration(test_item: Function) -> bool:
+    def is_integration(test_item: pytest.Function) -> bool:
         return test_item.get_closest_marker("integration") is not None
 
     integration_enabled = config.getoption(_RUN_INTEGRATION_TEST_FLAG)
     if not integration_enabled:  # pragma: no cover # hard to test
         for item in items:
             if is_integration(item):
                 item.add_marker(skip_int)
     # run integration tests (is_integration is True) after unit tests (False)
     items.sort(key=is_integration)
 
 
-def enable_pypi_server(monkeypatch: MonkeyPatch, url: str | None) -> None:
+def enable_pypi_server(monkeypatch: pytest.MonkeyPatch, url: str | None) -> None:
     if url is None:  # pragma: no cover # only one of the branches can be hit depending on env
         monkeypatch.delenv("PIP_INDEX_URL", raising=False)
     else:  # pragma: no cover
         monkeypatch.setenv("PIP_INDEX_URL", url)
     monkeypatch.setenv("PIP_RETRIES", str(5))
     monkeypatch.setenv("PIP_TIMEOUT", str(2))
 
 
 @pytest.fixture(scope="session")
-def pypi_server(tmp_path_factory: TempPathFactory) -> Iterator[IndexServer]:
+def pypi_server(tmp_path_factory: pytest.TempPathFactory) -> Iterator[IndexServer]:
     # takes around 2.5s
     path = tmp_path_factory.mktemp("pypi")
     with IndexServer(path) as server:
         server.create_index("empty", "volatile=False")
         yield server
 
 
@@ -497,28 +485,28 @@
 def _invalid_index_fake_port() -> int:  # noqa: PT005
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as socket_handler:
         socket_handler.bind(("", 0))
         return cast(int, socket_handler.getsockname()[1])
 
 
 @pytest.fixture(autouse=True)
-def disable_pip_pypi_access(_invalid_index_fake_port: int, monkeypatch: MonkeyPatch) -> tuple[str, str | None]:
+def disable_pip_pypi_access(_invalid_index_fake_port: int, monkeypatch: pytest.MonkeyPatch) -> tuple[str, str | None]:
     """Set a fake pip index url, tests that want to use a pypi server should create and overwrite this."""
     previous_url = os.environ.get("PIP_INDEX_URL")
     new_url = f"http://localhost:{_invalid_index_fake_port}/bad-pypi-server"
     monkeypatch.setenv("PIP_INDEX_URL", new_url)
     monkeypatch.setenv("PIP_RETRIES", str(0))
     monkeypatch.setenv("PIP_TIMEOUT", str(0.001))
     return new_url, previous_url
 
 
 @pytest.fixture(name="enable_pip_pypi_access")
 def enable_pip_pypi_access_fixture(
     disable_pip_pypi_access: tuple[str, str | None],
-    monkeypatch: MonkeyPatch,
+    monkeypatch: pytest.MonkeyPatch,
 ) -> str | None:
     """Set a fake pip index url, tests that want to use a pypi server should create and overwrite this."""
     _, previous_url = disable_pip_pypi_access
     enable_pypi_server(monkeypatch, previous_url)
     return previous_url
 
 
@@ -528,14 +516,18 @@
     assert caller_module is not None  # noqa: S101
     plugin = ModuleType(f"{caller_module.__name__}|{frame_info[3]}")
     plugin.__file__ = caller_module.__file__
     plugin.__dict__.update({f.__name__: f for f in args})
     mocker.patch("tox.plugin.manager.load_inline", return_value=plugin)
 
 
+LogCaptureFixture = pytest.LogCaptureFixture
+TempPathFactory = pytest.TempPathFactory
+MonkeyPatch = pytest.MonkeyPatch
+
 __all__ = (
     "CaptureFixture",
     "LogCaptureFixture",
     "TempPathFactory",
     "MonkeyPatch",
     "SubRequest",
     "ToxRunOutcome",
```

### Comparing `tox-4.8.0/src/tox/report.py` & `tox-4.9.0/src/tox/report.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/run.py` & `tox-4.9.0/src/tox/run.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/main.py` & `tox-4.9.0/src/tox/config/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/of_type.py` & `tox-4.9.0/src/tox/config/of_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Group together configuration values (such as base tox configuration, tox environment configs)."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from itertools import product
-from typing import TYPE_CHECKING, Any, Callable, Generic, Iterable, TypeVar, cast
+from typing import TYPE_CHECKING, Callable, Generic, Iterable, TypeVar, cast
 
 from tox.config.loader.api import ConfigLoadArgs, Loader
 
 if TYPE_CHECKING:
     from tox.config.loader.convert import Factory
     from tox.config.main import Config  # pragma: no cover
 
@@ -23,18 +23,18 @@
         self.keys = keys
         self.desc = desc
 
     @abstractmethod
     def __call__(self, conf: Config, loaders: list[Loader[T]], args: ConfigLoadArgs) -> T:
         raise NotImplementedError
 
-    def __eq__(self, o: Any) -> bool:
-        return type(self) == type(o) and (self.keys, self.desc) == (o.keys, o.desc)
+    def __eq__(self, o: object) -> bool:
+        return type(self) == type(o) and (self.keys, self.desc) == (o.keys, o.desc)  # type: ignore[attr-defined]
 
-    def __ne__(self, o: Any) -> bool:
+    def __ne__(self, o: object) -> bool:
         return not (self == o)
 
 
 class ConfigConstantDefinition(ConfigDefinition[T]):
     """A configuration definition whose value is defined upfront (such as the tox environment name)."""
 
     def __init__(
@@ -50,16 +50,16 @@
         self,
         conf: Config,  # noqa: ARG002
         loaders: list[Loader[T]],  # noqa: ARG002
         args: ConfigLoadArgs,  # noqa: ARG002
     ) -> T:
         return self.value() if callable(self.value) else self.value
 
-    def __eq__(self, o: Any) -> bool:
-        return type(self) == type(o) and super().__eq__(o) and self.value == o.value
+    def __eq__(self, o: object) -> bool:
+        return type(self) == type(o) and super().__eq__(o) and self.value == o.value  # type: ignore[attr-defined]
 
 
 _PLACE_HOLDER = object()
 
 
 class ConfigDynamicDefinition(ConfigDefinition[T]):
     """A configuration definition that comes from a source (such as in memory, an ini file, a toml file, etc.)."""
@@ -108,19 +108,20 @@
             self._cache = value
         return cast(T, self._cache)
 
     def __repr__(self) -> str:
         values = ((k, v) for k, v in vars(self).items() if k != "post_process" and v is not None)
         return f"{type(self).__name__}({', '.join(f'{k}={v}' for k, v in values)})"
 
-    def __eq__(self, o: Any) -> bool:
+    def __eq__(self, o: object) -> bool:
         return (
             type(self) == type(o)
             and super().__eq__(o)
-            and (self.of_type, self.default, self.post_process) == (o.of_type, o.default, o.post_process)
+            and (self.of_type, self.default, self.post_process)
+            == (o.of_type, o.default, o.post_process)  # type: ignore[attr-defined]
         )
 
 
 __all__ = [
     "ConfigLoadArgs",
     "ConfigDefinition",
     "ConfigDynamicDefinition",
```

### Comparing `tox-4.8.0/src/tox/config/set_env.py` & `tox-4.9.0/src/tox/config/set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/sets.py` & `tox-4.9.0/src/tox/config/sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/types.py` & `tox-4.9.0/src/tox/config/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from collections import OrderedDict
-from typing import Any, Iterator, Sequence
+from typing import Iterator, Sequence
 
 from tox.execute.request import shell_cmd
 
 
 class Command:
     """A command to execute."""
 
@@ -17,18 +17,21 @@
         """
         self.ignore_exit_code: bool = args[0] == "-"  #: a flag indicating if the exit code should be ignored
         self.args: list[str] = args[1:] if self.ignore_exit_code else args  #: the command line arguments
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}(args={(['-'] if self.ignore_exit_code else [])+ self.args!r})"
 
-    def __eq__(self, other: Any) -> bool:
-        return type(self) == type(other) and (self.args, self.ignore_exit_code) == (other.args, other.ignore_exit_code)
+    def __eq__(self, other: object) -> bool:
+        return type(self) == type(other) and (self.args, self.ignore_exit_code) == (
+            other.args,  # type: ignore[attr-defined]
+            other.ignore_exit_code,  # type: ignore[attr-defined]
+        )
 
-    def __ne__(self, other: Any) -> bool:
+    def __ne__(self, other: object) -> bool:
         return not (self == other)
 
     @property
     def shell(self) -> str:
         """:return: a shell representation of the command (platform dependent)"""
         return shell_cmd(self.args)
 
@@ -43,18 +46,18 @@
         :param envs: the list of tox environments
         """
         self.envs = list(OrderedDict((e, None) for e in envs).keys())
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.envs!r})"
 
-    def __eq__(self, other: Any) -> bool:
-        return type(self) == type(other) and self.envs == other.envs
+    def __eq__(self, other: object) -> bool:
+        return type(self) == type(other) and self.envs == other.envs  # type: ignore[attr-defined]
 
-    def __ne__(self, other: Any) -> bool:
+    def __ne__(self, other: object) -> bool:
         return not (self == other)
 
     def __iter__(self) -> Iterator[str]:
         """:return: iterator that goes through the defined env-list"""
         return iter(self.envs)
```

### Comparing `tox-4.8.0/src/tox/config/cli/env_var.py` & `tox-4.9.0/src/tox/config/cli/env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/cli/ini.py` & `tox-4.9.0/src/tox/config/cli/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/cli/parse.py` & `tox-4.9.0/src/tox/config/cli/parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/cli/parser.py` & `tox-4.9.0/src/tox/config/cli/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,22 @@
 
 import argparse
 import logging
 import os
 import sys
 from argparse import SUPPRESS, Action, ArgumentDefaultsHelpFormatter, ArgumentParser, Namespace
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Sequence, Tuple, Type, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Literal, Optional, Sequence, Tuple, Type, TypeVar, cast
 
 from tox.config.loader.str_convert import StrConvert
 from tox.plugin import NAME
 
 from .env_var import get_env_var
 from .ini import IniConfig
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from typing import Literal
-else:  # pragma: no cover (py38+)
-    from typing_extensions import Literal
-
 if TYPE_CHECKING:
     from tox.session.state import State
 
 
 class ArgumentParserWithEnvAndConfig(ArgumentParser):
     """Argument parser which updates its defaults by checking the configuration files and environmental variables."""
```

### Comparing `tox-4.8.0/src/tox/config/loader/api.py` & `tox-4.9.0/src/tox/config/loader/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,20 +34,24 @@
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}('{self}')"
 
     def __str__(self) -> str:
         return f"{self.namespace}{'.' if self.namespace else ''}{self.key}={self.value}"
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if type(self) != type(other):
             return False
-        return (self.namespace, self.key, self.value) == (other.namespace, other.key, other.value)
+        return (self.namespace, self.key, self.value) == (
+            other.namespace,  # type: ignore[attr-defined]
+            other.key,  # type: ignore[attr-defined]
+            other.value,  # type: ignore[attr-defined]
+        )
 
-    def __ne__(self, other: Any) -> bool:
+    def __ne__(self, other: object) -> bool:
         return not (self == other)
 
 
 class ConfigLoadArgs:
     """Arguments that help loading a configuration value."""
 
     def __init__(self, chain: list[str] | None, name: str | None, env_name: str | None) -> None:
```

### Comparing `tox-4.8.0/src/tox/config/loader/convert.py` & `tox-4.9.0/src/tox/config/loader/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 from __future__ import annotations
 
-import sys
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from pathlib import Path
-from typing import Any, Callable, Dict, Generic, Iterator, List, Optional, Set, TypeVar, Union, cast
+from typing import Any, Callable, Dict, Generic, Iterator, List, Literal, Optional, Set, TypeVar, Union, cast
 
 from tox.config.types import Command, EnvList
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from typing import Literal
-else:  # pragma: no cover (py38+)
-    from typing_extensions import Literal
-
-
 _NO_MAPPING = object()
 T = TypeVar("T")
 V = TypeVar("V")
 
 Factory = Optional[Callable[[object], T]]  # note the argument is anything, due e.g. memory loader can inject anything
```

### Comparing `tox-4.8.0/src/tox/config/loader/memory.py` & `tox-4.9.0/src/tox/config/loader/memory.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/loader/section.py` & `tox-4.9.0/src/tox/config/loader/section.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from __future__ import annotations
 
-from typing import Any, TypeVar
+from typing import TYPE_CHECKING
 
-_Section = TypeVar("_Section", bound="Section")
+if TYPE_CHECKING:
+    import sys
+
+    if sys.version_info >= (3, 11):  # pragma: no cover (py311+)
+        from typing import Self
+    else:  # pragma: no cover (<py311)
+        from typing_extensions import Self
 
 
 class Section:
     """tox configuration section."""
 
     SEP = ":"  #: string used to separate the prefix and the section in the key
 
     def __init__(self, prefix: str | None, name: str) -> None:
         self._prefix = prefix
         self._name = name
 
     @classmethod
-    def from_key(cls: type[_Section], key: str) -> _Section:
+    def from_key(cls: type[Self], key: str) -> Self:
         """
         Create a section from a section key.
 
         :param key: the section key
         :return: the constructed section
         """
         sep_at = key.find(cls.SEP)
@@ -46,15 +52,15 @@
 
     def __str__(self) -> str:
         return self.key
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(prefix={self._prefix!r}, name={self._name!r})"
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         return isinstance(other, self.__class__) and (self._prefix, self._name) == (
             other._prefix,
             other.name,
         )
 
 
 __all__ = [
```

### Comparing `tox-4.8.0/src/tox/config/loader/str_convert.py` & `tox-4.9.0/src/tox/config/loader/str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/loader/stringify.py` & `tox-4.9.0/src/tox/config/loader/stringify.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/loader/ini/__init__.py` & `tox-4.9.0/src/tox/config/loader/ini/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/loader/ini/factor.py` & `tox-4.9.0/src/tox/config/loader/ini/factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/loader/ini/replace.py` & `tox-4.9.0/src/tox/config/loader/ini/replace.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     def __init__(self, expr: Sequence[MatchArg], term_pos: int | None = None) -> None:
         self.expr = expr
         self.term_pos = term_pos
 
     def __repr__(self) -> str:
         return f"MatchExpression(expr={self.expr!r}, term_pos={self.term_pos!r})"
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if isinstance(other, type(self)):
             return self.expr == other.expr
         return NotImplemented
 
     @classmethod
     def _next_replace_expression(cls, value: str) -> MatchExpression | None:
         """Process a curly brace replacement expression."""
```

### Comparing `tox-4.8.0/src/tox/config/source/api.py` & `tox-4.9.0/src/tox/config/source/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/source/discover.py` & `tox-4.9.0/src/tox/config/source/discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/source/ini.py` & `tox-4.9.0/src/tox/config/source/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/source/ini_section.py` & `tox-4.9.0/src/tox/config/source/ini_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/source/legacy_toml.py` & `tox-4.9.0/src/tox/config/source/legacy_toml.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/config/source/setup_cfg.py` & `tox-4.9.0/src/tox/config/source/setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/execute/api.py` & `tox-4.9.0/src/tox/execute/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/execute/pep517_backend.py` & `tox-4.9.0/src/tox/execute/pep517_backend.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/execute/request.py` & `tox-4.9.0/src/tox/execute/request.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/execute/stream.py` & `tox-4.9.0/src/tox/execute/stream.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,22 @@
 from contextlib import contextmanager
 from threading import Event, Lock, Timer
 from typing import IO, TYPE_CHECKING, Iterator
 
 from colorama import Fore
 
 if TYPE_CHECKING:
+    import sys
     from types import TracebackType
 
+    if sys.version_info >= (3, 11):  # pragma: no cover (py311+)
+        from typing import Self
+    else:  # pragma: no cover (<py311)
+        from typing_extensions import Self
+
 
 class SyncWrite:
     """
     Make sure data collected is synced in-memory and to the target stream on every newline and time period.
 
     Used to propagate executed commands output to the standard output/error streams visible to the user.
     """
@@ -29,15 +35,15 @@
         self._at: int = 0
         self._color: str | None = color
         self.name = name
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(name={self.name!r}, target={self._target!r}, color={self._color!r})"
 
-    def __enter__(self) -> SyncWrite:
+    def __enter__(self) -> Self:
         if self._target_enabled:
             self._start()
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
```

### Comparing `tox-4.8.0/src/tox/execute/util.py` & `tox-4.9.0/src/tox/execute/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/execute/local_sub_process/__init__.py` & `tox-4.9.0/src/tox/execute/local_sub_process/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/execute/local_sub_process/read_via_thread.py` & `tox-4.9.0/src/tox/execute/local_sub_process/read_via_thread.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,35 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from threading import Event, Thread
 from typing import TYPE_CHECKING, Callable
 
 if TYPE_CHECKING:
+    import sys
     from types import TracebackType
 
+    if sys.version_info >= (3, 11):  # pragma: no cover (py311+)
+        from typing import Self
+    else:  # pragma: no cover (<py311)
+        from typing_extensions import Self
+
+
 WAIT_GENERAL = 0.05  # stop thread join every so often (give chance to a signal interrupt)
 
 
 class ReadViaThread(ABC):
     def __init__(self, file_no: int, handler: Callable[[bytes], None], name: str, drain: bool) -> None:  # noqa: FBT001
         self.file_no = file_no
         self.stop = Event()
         self.thread = Thread(target=self._read_stream, name=f"tox-r-{name}-{file_no}")
         self.handler = handler
         self._on_exit_drain = drain
 
-    def __enter__(self) -> ReadViaThread:
+    def __enter__(self) -> Self:
         self.thread.start()
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
```

### Comparing `tox-4.8.0/src/tox/execute/local_sub_process/read_via_thread_unix.py` & `tox-4.9.0/src/tox/execute/local_sub_process/read_via_thread_unix.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/execute/local_sub_process/read_via_thread_windows.py` & `tox-4.9.0/src/tox/execute/local_sub_process/read_via_thread_windows.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/journal/env.py` & `tox-4.9.0/src/tox/journal/env.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/journal/main.py` & `tox-4.9.0/src/tox/journal/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/plugin/__init__.py` & `tox-4.9.0/src/tox/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/plugin/inline.py` & `tox-4.9.0/src/tox/plugin/inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/plugin/manager.py` & `tox-4.9.0/src/tox/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/plugin/spec.py` & `tox-4.9.0/src/tox/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/env_select.py` & `tox-4.9.0/src/tox/session/env_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 import re
 from collections import Counter
 from dataclasses import dataclass
 from itertools import chain
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Iterator, List, cast
+from typing import TYPE_CHECKING, Dict, Iterable, Iterator, List, cast
 
 from tox.config.loader.str_convert import StrConvert
 from tox.config.types import EnvList
 from tox.report import HandledError
 from tox.tox_env.api import ToxEnvCreateArgs
 from tox.tox_env.errors import Skip
 from tox.tox_env.package import PackageToxEnv
@@ -42,18 +42,18 @@
 
     def __str__(self) -> str:
         return "ALL" if self.is_all else ("<env_list>" if self.is_default_list else ",".join(self))
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({'' if self.is_default_list else repr(str(self))})"
 
-    def __eq__(self, other: Any) -> bool:
-        return type(self) == type(other) and self._names == other._names
+    def __eq__(self, other: object) -> bool:
+        return type(self) == type(other) and self._names == other._names  # type: ignore[attr-defined]
 
-    def __ne__(self, other: Any) -> bool:
+    def __ne__(self, other: object) -> bool:
         return not (self == other)
 
     @property
     def is_all(self) -> bool:
         return self._names is not None and "ALL" in self._names
 
     @property
@@ -148,14 +148,23 @@
             yield (self._provision[1],), False
         env_list, everything_active = self._state.conf.core["env_list"], False
         if self._cli_envs is None or self._cli_envs.is_default_list:
             yield env_list, True
         elif self._cli_envs.is_all:
             everything_active = True
         else:
+            cli_envs_not_in_config = set(self._cli_envs) - set(self._state.conf)
+            if cli_envs_not_in_config:
+                # allow cli_envs matching ".pkg" and starting with "py" to be implicitly created.
+                disallowed_cli_envs = [
+                    env for env in cli_envs_not_in_config if not env.startswith("py") and env not in (".pkg",)
+                ]
+                if disallowed_cli_envs:
+                    msg = f"provided environments not found in configuration file: {disallowed_cli_envs}"
+                    raise HandledError(msg)
             yield self._cli_envs, True
         yield self._state.conf, everything_active
         label_envs = dict.fromkeys(chain.from_iterable(self._state.conf.core["labels"].values()))
         if label_envs:
             yield label_envs.keys(), False
 
     def _env_name_to_active(self) -> dict[str, bool]:
```

### Comparing `tox-4.8.0/src/tox/session/state.py` & `tox-4.9.0/src/tox/session/state.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/depends.py` & `tox-4.9.0/src/tox/session/cmd/depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/devenv.py` & `tox-4.9.0/src/tox/session/cmd/devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/exec_.py` & `tox-4.9.0/src/tox/session/cmd/exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/legacy.py` & `tox-4.9.0/src/tox/session/cmd/legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/list_env.py` & `tox-4.9.0/src/tox/session/cmd/list_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/quickstart.py` & `tox-4.9.0/src/tox/session/cmd/quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/show_config.py` & `tox-4.9.0/src/tox/session/cmd/show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/version_flag.py` & `tox-4.9.0/src/tox/session/cmd/version_flag.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/run/common.py` & `tox-4.9.0/src/tox/session/cmd/run/common.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/run/parallel.py` & `tox-4.9.0/src/tox/session/cmd/run/parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/run/sequential.py` & `tox-4.9.0/src/tox/session/cmd/run/sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/session/cmd/run/single.py` & `tox-4.9.0/src/tox/session/cmd/run/single.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,20 +46,20 @@
             tox_env.setup()
             code, outcomes = run_commands(tox_env, no_test)
         except Skip as exception:
             LOGGER.warning("skipped because %s", exception)
             code = 0
             skipped = True
         except ToxBackendFailed as exception:
-            LOGGER.error("%s", exception)
+            LOGGER.error("%s", exception)  # noqa: TRY400
             raise SystemExit(exception.code)  # noqa: B904, TRY200
         except Fail as exception:
-            LOGGER.error("failed with %s", exception)
+            LOGGER.error("failed with %s", exception)  # noqa: TRY400
             code = 1
-        except Exception:  # pragma: no cover  # noqa: BLE001
+        except Exception:  # pragma: no cover
             LOGGER.exception("internal error")  # pragma: no cover
             code = 2  # pragma: no cover
         finally:
             tox_env.teardown()
     except SystemExit as exception:  # setup command fails (interrupted or via invocation)
         code = cast(int, exception.code)
     return skipped, code, outcomes
```

### Comparing `tox-4.8.0/src/tox/tox_env/api.py` & `tox-4.9.0/src/tox/tox_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/info.py` & `tox-4.9.0/src/tox/tox_env/info.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/installer.py` & `tox-4.9.0/src/tox/tox_env/installer.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/package.py` & `tox-4.9.0/src/tox/tox_env/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/register.py` & `tox-4.9.0/src/tox/tox_env/register.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/runner.py` & `tox-4.9.0/src/tox/tox_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/util.py` & `tox-4.9.0/src/tox/tox_env/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/python/api.py` & `tox-4.9.0/src/tox/tox_env/python/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/python/package.py` & `tox-4.9.0/src/tox/tox_env/python/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/python/runner.py` & `tox-4.9.0/src/tox/tox_env/python/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/python/pip/pip_install.py` & `tox-4.9.0/src/tox/tox_env/python/pip/pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/python/pip/req_file.py` & `tox-4.9.0/src/tox/tox_env/python/pip/req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/python/pip/req/args.py` & `tox-4.9.0/src/tox/tox_env/python/pip/req/args.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/python/pip/req/file.py` & `tox-4.9.0/src/tox/tox_env/python/pip/req/file.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/python/pip/req/util.py` & `tox-4.9.0/src/tox/tox_env/python/pip/req/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/python/virtual_env/api.py` & `tox-4.9.0/src/tox/tox_env/python/virtual_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/python/virtual_env/runner.py` & `tox-4.9.0/src/tox/tox_env/python/virtual_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py` & `tox-4.9.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import glob
 import shutil
-import sys
 import tarfile
 from functools import partial
 from io import TextIOWrapper
 from pathlib import Path
 from typing import TYPE_CHECKING, Generator, Iterator, List, cast
 from zipfile import ZipFile
 
@@ -30,18 +29,15 @@
 
     from tox.config.sets import EnvConfigSet
     from tox.tox_env.api import ToxEnvCreateArgs
     from tox.tox_env.package import Package, PackageToxEnv
     from tox.tox_env.register import ToxEnvRegister
     from tox.tox_env.runner import RunToxEnv
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from importlib.metadata import Distribution
-else:  # pragma: no cover (py38+)
-    from importlib_metadata import Distribution
+from importlib.metadata import Distribution
 
 
 class VirtualEnvCmdBuilder(PythonPackageToxEnv, VirtualEnv):
     def __init__(self, create_args: ToxEnvCreateArgs) -> None:
         super().__init__(create_args)
         self._sdist_meta_tox_env: Pep517VirtualEnvPackager | None = None
```

### Comparing `tox-4.8.0/src/tox/tox_env/python/virtual_env/package/pyproject.py` & `tox-4.9.0/src/tox/tox_env/python/virtual_env/package/pyproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,15 @@
     from tox.config.sets import EnvConfigSet
     from tox.execute.api import ExecuteStatus
     from tox.tox_env.api import ToxEnvCreateArgs
     from tox.tox_env.package import Package, PackageToxEnv
     from tox.tox_env.register import ToxEnvRegister
     from tox.tox_env.runner import RunToxEnv
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from importlib.metadata import Distribution, PathDistribution
-else:  # pragma: no cover (<py38)
-    from importlib_metadata import Distribution, PathDistribution
+from importlib.metadata import Distribution, PathDistribution
 
 if sys.version_info >= (3, 11):  # pragma: no cover (py311+)
     import tomllib
 else:  # pragma: no cover (py311+)
     import tomli as tomllib
 
 ConfigSettings = Optional[Dict[str, Any]]
```

### Comparing `tox-4.8.0/src/tox/tox_env/python/virtual_env/package/util.py` & `tox-4.9.0/src/tox/tox_env/python/virtual_env/package/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/util/ci.py` & `tox-4.9.0/src/tox/util/ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/util/file_view.py` & `tox-4.9.0/src/tox/util/file_view.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/util/graph.py` & `tox-4.9.0/src/tox/util/graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/util/path.py` & `tox-4.9.0/src/tox/util/path.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/src/tox/util/spinner.py` & `tox-4.9.0/src/tox/util/spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/conftest.py` & `tox-4.9.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import os
 import sys
 from pathlib import Path
-from typing import TYPE_CHECKING, Callable, Iterator, Sequence
+from typing import TYPE_CHECKING, Callable, Iterator, Protocol, Sequence
 from unittest.mock import patch
 from uuid import uuid4
 
 import pytest
 from distlib.scripts import ScriptMaker
 from filelock import FileLock
 from virtualenv import cli_run
@@ -15,16 +15,14 @@
 from tox.config.cli.parser import Parsed
 from tox.config.main import Config
 from tox.config.source import discover_source
 from tox.tox_env.python.api import PythonInfo, VersionInfo
 from tox.tox_env.python.virtual_env.api import VirtualEnv
 
 if TYPE_CHECKING:
-    from _pytest.monkeypatch import MonkeyPatch
-    from _pytest.tmpdir import TempPathFactory
     from pytest_mock import MockerFixture
 
     from tox.config.loader.api import Override
 
 pytest_plugins = "tox.pytest"
 HERE = Path(__file__).absolute().parent
 
@@ -33,33 +31,27 @@
 def value_error() -> Callable[[str], str]:
     def _fmt(msg: str) -> str:
         return f'ValueError("{msg}"{"," if sys.version_info < (3, 7) else ""})'
 
     return _fmt
 
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from typing import Protocol
-else:  # pragma: no cover (<py38)
-    from typing_extensions import Protocol
-
-
 collect_ignore = []
 if sys.implementation.name == "pypy":
     # time-machine causes segfaults on PyPy
     collect_ignore.append("util/test_spinner.py")
 
 
 class ToxIniCreator(Protocol):
     def __call__(self, conf: str, override: Sequence[Override] | None = None) -> Config:
         ...
 
 
 @pytest.fixture()
-def tox_ini_conf(tmp_path: Path, monkeypatch: MonkeyPatch) -> ToxIniCreator:
+def tox_ini_conf(tmp_path: Path, monkeypatch: pytest.MonkeyPatch) -> ToxIniCreator:
     def func(conf: str, override: Sequence[Override] | None = None) -> Config:
         dest = tmp_path / "c"
         dest.mkdir()
         config_file = dest / "tox.ini"
         config_file.write_bytes(conf.encode("utf-8"))
         with monkeypatch.context() as context:
             context.chdir(tmp_path)
@@ -113,38 +105,38 @@
         mocker.patch.object(VirtualEnv, "_get_python", get_python)
         return prev_ver, impl
 
     return _func
 
 
 @pytest.fixture(scope="session", autouse=True)
-def _do_not_share_virtualenv_for_parallel_runs(tmp_path_factory: TempPathFactory, worker_id: str) -> None:
+def _do_not_share_virtualenv_for_parallel_runs(tmp_path_factory: pytest.TempPathFactory, worker_id: str) -> None:
     # virtualenv uses locks to manage access to its cache, when running with xdist this may throw off test timings
     if worker_id != "master":  # pragma: no branch
         temp_app_data = str(tmp_path_factory.mktemp(f"virtualenv-app-{worker_id}"))  # pragma: no cover
         os.environ["VIRTUALENV_APP_DATA"] = temp_app_data  # pragma: no cover
         seed_env_folder = str(tmp_path_factory.mktemp(f"seed-cache-{worker_id}"))  # pragma: no cover
         args = [seed_env_folder, "--without-pip", "--activators", ""]  # pragma: no cover
         cli_run(args, setup_logging=False)  # pragma: no cover
 
 
 @pytest.fixture(scope="session")
-def fake_exe_on_path(tmp_path_factory: TempPathFactory) -> Iterator[Path]:
+def fake_exe_on_path(tmp_path_factory: pytest.TempPathFactory) -> Iterator[Path]:
     tmp_path = Path(tmp_path_factory.mktemp("a"))
     cmd_name = uuid4().hex
     maker = ScriptMaker(None, str(tmp_path))
     maker.set_mode = True
     maker.variants = {""}
     maker.make(f"{cmd_name} = b:c")
     with patch.dict(os.environ, {"PATH": f"{tmp_path}{os.pathsep}{os.environ['PATH']}"}):
         yield tmp_path / cmd_name
 
 
 @pytest.fixture(scope="session")
-def demo_pkg_inline_wheel(tmp_path_factory: TempPathFactory, demo_pkg_inline: Path) -> Path:
+def demo_pkg_inline_wheel(tmp_path_factory: pytest.TempPathFactory, demo_pkg_inline: Path) -> Path:
     return build_pkg(tmp_path_factory.mktemp("dist"), demo_pkg_inline, ["wheel"])
 
 
 def build_pkg(dist_dir: Path, of: Path, distributions: list[str], isolation: bool = True) -> Path:
     from build.__main__ import build_package
 
     build_package(str(of), str(dist_dir), distributions=distributions, isolation=isolation)
```

### Comparing `tox-4.8.0/tests/test_provision.py` & `tox-4.9.0/tests/test_provision.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,15 @@
 from packaging.requirements import Requirement
 
 if TYPE_CHECKING:
     from devpi_process import Index, IndexServer
 
     from tox.pytest import MonkeyPatch, TempPathFactory, ToxProjectCreator
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from importlib.metadata import Distribution
-else:  # pragma: no cover (<py38)
-    from importlib_metadata import Distribution
+from importlib.metadata import Distribution
 
 ROOT = Path(__file__).parents[1]
 
 
 @contextmanager
 def elapsed(msg: str) -> Iterator[None]:
     start = time.monotonic()
```

### Comparing `tox-4.8.0/tests/test_report.py` & `tox-4.9.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/test_run.py` & `tox-4.9.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/test_version.py` & `tox-4.9.0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/test_main.py` & `tox-4.9.0/tests/config/test_main.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/test_of_types.py` & `tox-4.9.0/tests/config/test_of_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/test_set_env.py` & `tox-4.9.0/tests/config/test_set_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from __future__ import annotations
 
-import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 from unittest.mock import ANY
 
 import pytest
 
 from tox.config.set_env import SetEnv
 
 if TYPE_CHECKING:
     from pytest_mock import MockerFixture
 
     from tox.pytest import MonkeyPatch, ToxProjectCreator
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from typing import Protocol
-else:  # pragma: no cover (<py38)
-    from typing_extensions import Protocol
+from typing import Protocol
 
 
 def test_set_env_explicit() -> None:
     set_env = SetEnv("\nA=1\nB = 2\nC= 3\nD= 4", "py", "py", Path())
     set_env.update({"E": "5 ", "F": "6"}, override=False)
 
     keys = list(set_env)
```

### Comparing `tox-4.8.0/tests/config/test_sets.py` & `tox-4.9.0/tests/config/test_sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/test_types.py` & `tox-4.9.0/tests/config/test_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/cli/conftest.py` & `tox-4.9.0/tests/config/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/cli/test_cli_env_var.py` & `tox-4.9.0/tests/config/cli/test_cli_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/cli/test_cli_ini.py` & `tox-4.9.0/tests/config/cli/test_cli_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/cli/test_parse.py` & `tox-4.9.0/tests/config/cli/test_parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/cli/test_parser.py` & `tox-4.9.0/tests/config/cli/test_parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/test_loader.py` & `tox-4.9.0/tests/config/loader/test_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/test_memory_loader.py` & `tox-4.9.0/tests/config/loader/test_memory_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/test_section.py` & `tox-4.9.0/tests/config/loader/test_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/test_str_convert.py` & `tox-4.9.0/tests/config/loader/test_str_convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 
 from tox.config.loader.str_convert import StrConvert
 from tox.config.types import Command, EnvList
 
 if TYPE_CHECKING:
     from tox.pytest import MonkeyPatch, SubRequest, ToxProjectCreator
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from typing import Literal
-else:  # pragma: no cover (py38+)
-    from typing_extensions import Literal
+from typing import Literal
 
 
 @pytest.mark.parametrize(
     ("raw", "value", "of_type"),
     [
         ("true", True, bool),
         ("false", False, bool),
```

### Comparing `tox-4.8.0/tests/config/loader/ini/conftest.py` & `tox-4.9.0/tests/config/loader/ini/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/ini/test_factor.py` & `tox-4.9.0/tests/config/loader/ini/test_factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/ini/test_ini_loader.py` & `tox-4.9.0/tests/config/loader/ini/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/ini/replace/conftest.py` & `tox-4.9.0/tests/config/loader/ini/replace/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from __future__ import annotations
 
-import sys
 from typing import TYPE_CHECKING
 
 import pytest
 
 from tox.config.cli.parser import Parsed
 from tox.config.loader.api import ConfigLoadArgs
 from tox.config.main import Config
 from tox.config.source.tox_ini import ToxIni
 
 if TYPE_CHECKING:
     from pathlib import Path
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from typing import Protocol
-else:  # pragma: no cover (<py38)
-    from typing_extensions import Protocol
+from typing import Protocol
 
 
 class ReplaceOne(Protocol):
     def __call__(self, conf: str, pos_args: list[str] | None = None) -> str:
         ...
```

### Comparing `tox-4.8.0/tests/config/loader/ini/replace/test_replace.py` & `tox-4.9.0/tests/config/loader/ini/replace/test_replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/ini/replace/test_replace_env_var.py` & `tox-4.9.0/tests/config/loader/ini/replace/test_replace_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/ini/replace/test_replace_os_sep.py` & `tox-4.9.0/tests/config/loader/ini/replace/test_replace_os_sep.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/ini/replace/test_replace_posargs.py` & `tox-4.9.0/tests/config/loader/ini/replace/test_replace_posargs.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/ini/replace/test_replace_tox_env.py` & `tox-4.9.0/tests/config/loader/ini/replace/test_replace_tox_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/loader/ini/replace/test_replace_tty.py` & `tox-4.9.0/tests/config/loader/ini/replace/test_replace_tty.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/source/test_discover.py` & `tox-4.9.0/tests/config/source/test_discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/source/test_setup_cfg.py` & `tox-4.9.0/tests/config/source/test_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/config/source/test_source_ini.py` & `tox-4.9.0/tests/config/source/test_source_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/demo_pkg_inline/build.py` & `tox-4.9.0/tests/demo_pkg_inline/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,24 +66,21 @@
     wheel: f"""
         Wheel-Version: 1.0
         Generator: {name}-{version}
         Root-Is-Purelib: true
         Tag: py{sys.version_info[0]}-none-any
        """,
     f"{dist_info}/top_level.txt": name,
-    record: """
-        {0}/__init__.py,,
-        {1}/METADATA,,
-        {1}/WHEEL,,
-        {1}/top_level.txt,,
-        {1}/RECORD,,
-       """.format(
-        name,
-        dist_info,
-    ),
+    record: f"""
+        {name}/__init__.py,,
+        {dist_info}/METADATA,,
+        {dist_info}/WHEEL,,
+        {dist_info}/top_level.txt,,
+        {dist_info}/RECORD,,
+       """,
 }
 
 
 def build_wheel(
     wheel_directory: str,
     config_settings: dict[str, str] | None = None,  # noqa: ARG001
     metadata_directory: str | None = None,
```

### Comparing `tox-4.8.0/tests/execute/test_request.py` & `tox-4.9.0/tests/execute/test_request.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/execute/local_subprocess/bad_process.py` & `tox-4.9.0/tests/execute/local_subprocess/bad_process.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/execute/local_subprocess/local_subprocess_sigint.py` & `tox-4.9.0/tests/execute/local_subprocess/local_subprocess_sigint.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/execute/local_subprocess/test_execute_util.py` & `tox-4.9.0/tests/execute/local_subprocess/test_execute_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/execute/local_subprocess/test_local_subprocess.py` & `tox-4.9.0/tests/execute/local_subprocess/test_local_subprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,20 +111,20 @@
     executor = LocalSubProcessExecutor(colored=False)
     request = ExecuteRequest(
         cmd=[
             sys.executable,
             "-c",
             (
                 "import sys; import time; from datetime import datetime; import os;"
-                "print('e' * {0}, file=sys.stderr);"
-                "print('o' * {0}, file=sys.stdout);"
+                f"print('e' * {count}, file=sys.stderr);"
+                f"print('o' * {count}, file=sys.stdout);"
                 "time.sleep(0.5);"
-                "print('a' * {0}, file=sys.stderr);"
-                "print('b' * {0}, file=sys.stdout);"
-            ).format(count),
+                f"print('a' * {count}, file=sys.stderr);"
+                f"print('b' * {count}, file=sys.stdout);"
+            ),
         ],
         cwd=Path(),
         env=os_env,
         stdin=StdinSource.OFF,
         run_id="",
     )
     out_err = FakeOutErr()
```

### Comparing `tox-4.8.0/tests/journal/test_main_journal.py` & `tox-4.9.0/tests/journal/test_main_journal.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/plugin/test_inline.py` & `tox-4.9.0/tests/plugin/test_inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/plugin/test_plugin.py` & `tox-4.9.0/tests/plugin/test_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,24 @@
     def tox_env_teardown(tox_env: ToxEnv) -> None:
         assert isinstance(tox_env, ToxEnv)
         logging.warning("teardown")
 
     plugins = tuple(v for v in locals().values() if callable(v) and hasattr(v, "tox_impl"))
     assert len(plugins) == 8
     register_inline_plugin(mocker, *plugins)
-    project = tox_project({"tox.ini": "[testenv]\npackage=skip\ncommands=python -c 'print(1)'"})
+
+    tox_ini = """
+        [tox]
+        env_list=a,b
+        [testenv]
+        package=skip
+        commands=python -c 'print(1)'
+        env_list=a,b
+    """
+    project = tox_project({"tox.ini": tox_ini})
     result = project.run("r", "-e", "a,b")
     result.assert_success()
     cmd = "print(1)" if sys.platform == "win32" else "'print(1)'"
     expected = [
         "ROOT: tox_register_tox_env",
         "ROOT: tox_add_option",
         "ROOT: tox_add_core_config",
```

### Comparing `tox-4.8.0/tests/plugin/test_plugin_custom_config_set.py` & `tox-4.9.0/tests/plugin/test_plugin_custom_config_set.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/pytest_/test_init.py` & `tox-4.9.0/tests/pytest_/test_init.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/session/test_env_select.py` & `tox-4.9.0/tests/session/test_env_select.py`

 * *Files 12% similar despite different names*

```diff
@@ -128,7 +128,39 @@
 
 def test_env_select_lazily_looks_at_envs() -> None:
     state = State(get_options(), [])
     env_selector = EnvSelector(state)
     # late-assigning env should be reflected in env_selector
     state.conf.options.env = CliEnv("py")
     assert set(env_selector.iter()) == {"py"}
+
+
+def test_cli_env_can_be_specified_in_default(tox_project: ToxProjectCreator) -> None:
+    proj = tox_project({"tox.ini": "[tox]\nenv_list=exists"})
+    outcome = proj.run("r", "-e", "exists")
+    outcome.assert_success()
+    assert "exists" in outcome.out
+    assert not outcome.err
+
+
+def test_cli_env_can_be_specified_in_additional_environments(tox_project: ToxProjectCreator) -> None:
+    proj = tox_project({"tox.ini": "[testenv:exists]"})
+    outcome = proj.run("r", "-e", "exists")
+    outcome.assert_success()
+    assert "exists" in outcome.out
+    assert not outcome.err
+
+
+def test_cli_env_not_in_tox_config_fails(tox_project: ToxProjectCreator) -> None:
+    proj = tox_project({"tox.ini": ""})
+    outcome = proj.run("r", "-e", "does_not_exist")
+    outcome.assert_failed(code=-2)
+    assert "provided environments not found in configuration file: ['does_not_exist']" in outcome.out, outcome.out
+
+
+@pytest.mark.parametrize("env_name", ["py", "py310", ".pkg"])
+def test_allowed_implicit_cli_envs(env_name: str, tox_project: ToxProjectCreator) -> None:
+    proj = tox_project({"tox.ini": ""})
+    outcome = proj.run("r", "-e", env_name)
+    outcome.assert_success()
+    assert env_name in outcome.out
+    assert not outcome.err
```

### Comparing `tox-4.8.0/tests/session/test_session_common.py` & `tox-4.9.0/tests/session/test_session_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/session/cmd/test_depends.py` & `tox-4.9.0/tests/session/cmd/test_depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/session/cmd/test_devenv.py` & `tox-4.9.0/tests/session/cmd/test_devenv.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 
 if TYPE_CHECKING:
     from tox.pytest import ToxProjectCreator
 
 
 def test_devenv_fail_multiple_target(tox_project: ToxProjectCreator) -> None:
-    outcome = tox_project({"tox.ini": ""}).run("d", "-e", "a,b")
+    outcome = tox_project({"tox.ini": "[tox]\nenv_list=a,b"}).run("d", "-e", "a,b")
     outcome.assert_failed()
     msg = "ROOT: HandledError| exactly one target environment allowed in devenv mode but found a, b\n"
     outcome.assert_out_err(msg, "")
 
 
 @pytest.mark.integration()
 def test_devenv_ok(tox_project: ToxProjectCreator, enable_pip_pypi_access: str | None) -> None:  # noqa: ARG001
```

### Comparing `tox-4.8.0/tests/session/cmd/test_exec_.py` & `tox-4.9.0/tests/session/cmd/test_exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/session/cmd/test_legacy.py` & `tox-4.9.0/tests/session/cmd/test_legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/session/cmd/test_list_envs.py` & `tox-4.9.0/tests/session/cmd/test_list_envs.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/session/cmd/test_parallel.py` & `tox-4.9.0/tests/session/cmd/test_parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             "tox.ini": ini,
             "pyproject.toml": (demo_pkg_inline / "pyproject.toml").read_text(),
             "build.py": (demo_pkg_inline / "build.py").read_text(),
         },
     )
     cmd = ["-c", str(proj.path / "tox.ini"), "p", "-p", "1", "-e", f"py,py{sys.version_info[0]},dep"]
     process = Popen([sys.executable, "-m", "tox", *cmd], stdout=PIPE, stderr=PIPE, universal_newlines=True)
-    while not marker.exists():
+    while not marker.exists() and (process.poll() is None):
         sleep(0.05)
     process.send_signal(SIGINT)
     out, err = process.communicate()
     assert process.returncode != 0
     assert "KeyboardInterrupt" in err, err
     assert "KeyboardInterrupt - teardown started\n" in out, out
     assert "interrupt tox environment: py\n" in out, out
```

### Comparing `tox-4.8.0/tests/session/cmd/test_quickstart.py` & `tox-4.9.0/tests/session/cmd/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/session/cmd/test_sequential.py` & `tox-4.9.0/tests/session/cmd/test_sequential.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,15 @@
     result = proj.run("r")
     result.assert_success()
 
 
 def test_platform_does_not_match_package_env(tox_project: ToxProjectCreator, demo_pkg_inline: Path) -> None:
     toml = (demo_pkg_inline / "pyproject.toml").read_text()
     build = (demo_pkg_inline / "build.py").read_text()
-    ini = "[testenv]\npackage=wheel\n[testenv:.pkg]\nplatform=wrong_platform"
+    ini = "[tox]\nenv_list=a,b\n[testenv]\npackage=wheel\n[testenv:.pkg]\nplatform=wrong_platform"
     proj = tox_project({"tox.ini": ini, "pyproject.toml": toml, "build.py": build})
     result = proj.run("r", "-e", "a,b")
     result.assert_failed()  # tox run fails as all envs are skipped
     assert "a: SKIP" in result.out
     assert "b: SKIP" in result.out
     msg = f"skipped because platform {sys.platform} does not match wrong_platform for package environment .pkg"
     assert f"a: {msg}" in result.out
@@ -426,15 +426,15 @@
 
 def test_sequential_help(tox_project: ToxProjectCreator) -> None:
     outcome = tox_project({"tox.ini": ""}).run("r", "-h")
     outcome.assert_success()
 
 
 def test_sequential_clears_pkg_at_most_once(tox_project: ToxProjectCreator, demo_pkg_inline: Path) -> None:
-    project = tox_project({"tox.ini": ""})
+    project = tox_project({"tox.ini": "[tox]\nenv_list=a,b"})
     result = project.run("r", "--root", str(demo_pkg_inline), "-e", "a,b", "-r")
     result.assert_success()
 
 
 def test_sequential_inserted_env_vars(tox_project: ToxProjectCreator, demo_pkg_inline: Path) -> None:
     ini = """
     [testenv]
```

### Comparing `tox-4.8.0/tests/session/cmd/test_show_config.py` & `tox-4.9.0/tests/session/cmd/test_show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/session/cmd/test_state.py` & `tox-4.9.0/tests/session/cmd/test_state.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/session/cmd/run/test_common.py` & `tox-4.9.0/tests/session/cmd/run/test_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/test_api.py` & `tox-4.9.0/tests/tox_env/test_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/test_register.py` & `tox-4.9.0/tests/tox_env/test_register.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/test_tox_env_api.py` & `tox-4.9.0/tests/tox_env/test_tox_env_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/test_tox_env_runner.py` & `tox-4.9.0/tests/tox_env/test_tox_env_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/python/test_python_api.py` & `tox-4.9.0/tests/tox_env/python/test_python_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/python/test_python_runner.py` & `tox-4.9.0/tests/tox_env/python/test_python_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/python/pip/test_pip_install.py` & `tox-4.9.0/tests/tox_env/python/pip/test_pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/python/pip/test_req_file.py` & `tox-4.9.0/tests/tox_env/python/pip/test_req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/python/pip/req/test_file.py` & `tox-4.9.0/tests/tox_env/python/pip/req/test_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/python/virtual_env/test_setuptools.py` & `tox-4.9.0/tests/tox_env/python/virtual_env/test_setuptools.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py` & `tox-4.9.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/python/virtual_env/package/conftest.py` & `tox-4.9.0/tests/tox_env/python/virtual_env/package/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 from typing import TYPE_CHECKING
 
 import pytest
 
 if TYPE_CHECKING:
     from pathlib import Path
 
-    from _pytest.tmpdir import TempPathFactory
-
 
 @pytest.fixture(scope="session")
-def pkg_with_extras_project(tmp_path_factory: TempPathFactory) -> Path:
+def pkg_with_extras_project(tmp_path_factory: pytest.TempPathFactory) -> Path:
     py_ver = ".".join(str(i) for i in sys.version_info[0:2])
     setup_cfg = f"""
     [metadata]
     name = demo
     version = 1.0.0
     [options]
     packages = find:
```

### Comparing `tox-4.8.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py` & `tox-4.9.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py` & `tox-4.9.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     assert found_calls == expected_calls
 
     args = execute_calls.call_args_list[-3][0][3].cmd
     assert args == ["python", "-I", "-m", "pip", "install", *deps]
 
 
 def test_pyproject_no_build_editable_fallback(tox_project: ToxProjectCreator, demo_pkg_inline: Path) -> None:
-    proj = tox_project({"tox.ini": ""}, base=demo_pkg_inline)
+    proj = tox_project({"tox.ini": "[tox]\nenv_list=a,b"}, base=demo_pkg_inline)
     execute_calls = proj.patch_execute(lambda r: 0 if "install" in r.run_id else None)
     result = proj.run("r", "-e", "a,b", "--notest", "--develop")
     result.assert_success()
     warning = (
         ".pkg: package config for a, b is editable, however the build backend build does not support PEP-660, "
         "falling back to editable-legacy - change your configuration to it"
     )
```

### Comparing `tox-4.8.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py` & `tox-4.9.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 from pyproject_api import SubprocessFrontend
 
 from tox.tox_env.python.virtual_env.package.util import dependencies_with_extras
 
 if TYPE_CHECKING:
     from pathlib import Path
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from importlib.metadata import Distribution, PathDistribution
-else:  # pragma: no cover (<py38)
-    from importlib_metadata import Distribution, PathDistribution
+from importlib.metadata import Distribution, PathDistribution
 
 
 @pytest.fixture(scope="session")
 def pkg_with_extras(pkg_with_extras_project: Path) -> PathDistribution:
     frontend = SubprocessFrontend(*SubprocessFrontend.create_args_from_folder(pkg_with_extras_project)[:-1])
     meta = pkg_with_extras_project / "meta"
     result = frontend.prepare_metadata_for_build_wheel(meta)
```

### Comparing `tox-4.8.0/tests/util/test_ci.py` & `tox-4.9.0/tests/util/test_ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/util/test_cpu.py` & `tox-4.9.0/tests/util/test_cpu.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/util/test_graph.py` & `tox-4.9.0/tests/util/test_graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/tests/util/test_spinner.py` & `tox-4.9.0/tests/util/test_spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/LICENSE` & `tox-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/README.md` & `tox-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tox-4.8.0/pyproject.toml` & `tox-4.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.3",
-  "hatchling>=1.17.1",
+  "hatchling>=1.18",
 ]
 
 [project]
 name = "tox"
 description = "tox is a generic virtualenv management and test command line tool"
 readme.content-type = "text/markdown"
 readme.file = "README.md"
@@ -20,79 +20,78 @@
 maintainers = [
   { name = "Anthony Sottile", email = "asottile@umich.edu" },
   { name = "Bernát Gábor", email = "gaborjbernat@gmail.com" },
   { name = "Jürgen Gmach", email = "juergen.gmach@googlemail.com" },
   { name = "Oliver Bestwalter", email = "oliver@bestwalter.de" },
 ]
 authors = [{ name = "Bernát Gábor", email = "gaborjbernat@gmail.com" }]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Framework :: tox",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Testing",
   "Topic :: Utilities",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "cachetools>=5.3.1",
-  "chardet>=5.1",
+  "chardet>=5.2",
   "colorama>=0.4.6",
   "filelock>=3.12.2",
-  'importlib-metadata>=6.7; python_version < "3.8"',
+  'importlib-metadata>=6.8; python_version < "3.8"',
   "packaging>=23.1",
-  "platformdirs>=3.9.1",
+  "platformdirs>=3.10",
   "pluggy>=1.2",
   "pyproject-api>=1.5.3",
   'tomli>=2.0.1; python_version < "3.11"',
   'typing-extensions>=4.7.1; python_version < "3.8"',
-  "virtualenv>=20.24.1",
+  "virtualenv>=20.24.3",
 ]
 optional-dependencies.docs = [
-  "furo>=2023.5.20",
-  "sphinx>=7.0.1",
+  "furo>=2023.7.26",
+  "sphinx>=7.1.2",
   "sphinx-argparse-cli>=1.11.1",
-  "sphinx-autodoc-typehints!=1.23.4,>=1.23.3",
+  "sphinx-autodoc-typehints!=1.23.4,>=1.24",
   "sphinx-copybutton>=0.5.2",
   "sphinx-inline-tabs>=2023.4.21",
   "sphinxcontrib-towncrier>=0.2.1a0",
   "towncrier>=23.6",
 ]
 optional-dependencies.testing = [
   "build[virtualenv]>=0.10",
   "covdefaults>=2.3",
   "detect-test-pollution>=1.1.1",
   "devpi-process>=0.3.1",
   "diff-cover>=7.7",
   "distlib>=0.3.7",
   "flaky>=3.7",
   "hatch-vcs>=0.3",
-  "hatchling>=1.17.1",
+  "hatchling>=1.18",
   "psutil>=5.9.5",
   "pytest>=7.4",
   "pytest-cov>=4.1",
   "pytest-mock>=3.11.1",
   "pytest-xdist>=3.3.1",
   "re-assert>=1.1",
-  'time-machine>=2.10; implementation_name != "pypy"',
-  "wheel>=0.40",
+  'time-machine>=2.12; implementation_name != "pypy"',
+  "wheel>=0.41.1",
 ]
 urls.Documentation = "https://tox.wiki"
 urls.Homepage = "http://tox.readthedocs.org"
 urls."Release Notes" = "https://tox.wiki/en/latest/changelog.html"
 urls.Source = "https://github.com/tox-dev/tox"
 urls.Tracker = "https://github.com/tox-dev/tox/issues"
 scripts.tox = "tox.run:run"
@@ -105,15 +104,15 @@
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
 select = ["ALL"]
 line-length = 120
-target-version = "py37"
+target-version = "py38"
 isort = {known-first-party = ["tox", "tests"], required-imports = ["from __future__ import annotations"]}
 ignore = [
   "INP001",  # no implicit namespaces here
   "D",  # ignore documentation for now
   "ANN401",  # Dynamically typed expressions (typing.Any) are disallowed in `arg`"
   "ANN101",  # Missing type annotation for `self` in method
   "ANN102",  # Missing type annotation for `cls` in classmethod"
```

### Comparing `tox-4.8.0/PKG-INFO` & `tox-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox
-Version: 4.8.0
+Version: 4.9.0
 Summary: tox is a generic virtualenv management and test command line tool
 Project-URL: Documentation, https://tox.wiki
 Project-URL: Homepage, http://tox.readthedocs.org
 Project-URL: Release Notes, https://tox.wiki/en/latest/changelog.html
 Project-URL: Source, https://github.com/tox-dev/tox
 Project-URL: Tracker, https://github.com/tox-dev/tox/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
@@ -16,63 +16,62 @@
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: cachetools>=5.3.1
-Requires-Dist: chardet>=5.1
+Requires-Dist: chardet>=5.2
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: filelock>=3.12.2
-Requires-Dist: importlib-metadata>=6.7; python_version < '3.8'
+Requires-Dist: importlib-metadata>=6.8; python_version < '3.8'
 Requires-Dist: packaging>=23.1
-Requires-Dist: platformdirs>=3.9.1
+Requires-Dist: platformdirs>=3.10
 Requires-Dist: pluggy>=1.2
 Requires-Dist: pyproject-api>=1.5.3
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Requires-Dist: typing-extensions>=4.7.1; python_version < '3.8'
-Requires-Dist: virtualenv>=20.24.1
+Requires-Dist: virtualenv>=20.24.3
 Provides-Extra: docs
-Requires-Dist: furo>=2023.5.20; extra == 'docs'
+Requires-Dist: furo>=2023.7.26; extra == 'docs'
 Requires-Dist: sphinx-argparse-cli>=1.11.1; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23.3; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.24; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs>=2023.4.21; extra == 'docs'
-Requires-Dist: sphinx>=7.0.1; extra == 'docs'
+Requires-Dist: sphinx>=7.1.2; extra == 'docs'
 Requires-Dist: sphinxcontrib-towncrier>=0.2.1a0; extra == 'docs'
 Requires-Dist: towncrier>=23.6; extra == 'docs'
 Provides-Extra: testing
 Requires-Dist: build[virtualenv]>=0.10; extra == 'testing'
 Requires-Dist: covdefaults>=2.3; extra == 'testing'
 Requires-Dist: detect-test-pollution>=1.1.1; extra == 'testing'
 Requires-Dist: devpi-process>=0.3.1; extra == 'testing'
 Requires-Dist: diff-cover>=7.7; extra == 'testing'
 Requires-Dist: distlib>=0.3.7; extra == 'testing'
 Requires-Dist: flaky>=3.7; extra == 'testing'
 Requires-Dist: hatch-vcs>=0.3; extra == 'testing'
-Requires-Dist: hatchling>=1.17.1; extra == 'testing'
+Requires-Dist: hatchling>=1.18; extra == 'testing'
 Requires-Dist: psutil>=5.9.5; extra == 'testing'
 Requires-Dist: pytest-cov>=4.1; extra == 'testing'
 Requires-Dist: pytest-mock>=3.11.1; extra == 'testing'
 Requires-Dist: pytest-xdist>=3.3.1; extra == 'testing'
 Requires-Dist: pytest>=7.4; extra == 'testing'
 Requires-Dist: re-assert>=1.1; extra == 'testing'
-Requires-Dist: time-machine>=2.10; implementation_name != 'pypy' and extra == 'testing'
-Requires-Dist: wheel>=0.40; extra == 'testing'
+Requires-Dist: time-machine>=2.12; implementation_name != 'pypy' and extra == 'testing'
+Requires-Dist: wheel>=0.41.1; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # tox
 
 [![PyPI](https://img.shields.io/pypi/v/tox)](https://pypi.org/project/tox/)
 [![Supported Python
 versions](https://img.shields.io/pypi/pyversions/tox.svg)](https://pypi.org/project/tox/)
```

