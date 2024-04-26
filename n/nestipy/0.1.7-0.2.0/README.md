# Comparing `tmp/nestipy-0.1.7.tar.gz` & `tmp/nestipy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy-0.1.7.tar", max compression
+gzip compressed data, was "nestipy-0.2.0.tar", max compression
```

## Comparing `nestipy-0.1.7.tar` & `nestipy-0.2.0.tar`

### file list

```diff
@@ -1,179 +1,116 @@
--rw-r--r--   0        0        0     1054 2024-03-08 07:10:04.714124 nestipy-0.1.7/LICENSE
--rw-r--r--   0        0        0     2069 2024-03-08 07:10:04.714124 nestipy-0.1.7/README.md
--rw-r--r--   0        0        0      955 2024-03-08 15:07:01.860564 nestipy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.153461 nestipy-0.1.7/src/nestipy/__init__.py
--rw-r--r--   0        0        0     6162 2024-03-01 12:42:00.428783 nestipy-0.1.7/src/nestipy/cli/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     9425 2024-03-08 08:49:37.648272 nestipy-0.1.7/src/nestipy/cli/__pycache__/handler.cpython-311.pyc
--rw-r--r--   0        0        0     1652 2024-03-01 12:42:00.920929 nestipy-0.1.7/src/nestipy/cli/__pycache__/style.cpython-311.pyc
--rw-r--r--   0        0        0     2775 2024-02-29 12:35:05.153461 nestipy-0.1.7/src/nestipy/cli/cli.py
--rw-r--r--   0        0        0     5074 2024-03-08 07:10:04.730124 nestipy-0.1.7/src/nestipy/cli/handler.py
--rw-r--r--   0        0        0      502 2024-02-29 12:35:05.153461 nestipy-0.1.7/src/nestipy/cli/style.py
--rw-r--r--   0        0        0      102 2024-03-01 11:24:49.624082 nestipy-0.1.7/src/nestipy/common/__init__.py
--rw-r--r--   0        0        0      322 2024-03-01 12:17:25.314721 nestipy-0.1.7/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      652 2024-03-01 12:17:25.762807 nestipy-0.1.7/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
--rw-r--r--   0        0        0      424 2024-03-08 07:10:04.730124 nestipy-0.1.7/src/nestipy/common/context/__init__.py
--rw-r--r--   0        0        0     1424 2024-03-08 07:12:41.963785 nestipy-0.1.7/src/nestipy/common/context/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4782 2024-03-08 14:49:27.190674 nestipy-0.1.7/src/nestipy/common/context/__pycache__/request.cpython-311.pyc
--rw-r--r--   0        0        0     6923 2024-03-08 14:55:41.710555 nestipy-0.1.7/src/nestipy/common/context/__pycache__/response.cpython-311.pyc
--rw-r--r--   0        0        0     2140 2024-03-08 14:41:12.109968 nestipy-0.1.7/src/nestipy/common/context/request.py
--rw-r--r--   0        0        0     3760 2024-03-08 14:55:35.098293 nestipy-0.1.7/src/nestipy/common/context/response.py
--rw-r--r--   0        0        0      653 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/decorator/__init__.py
--rw-r--r--   0        0        0     1015 2024-03-08 07:12:41.951784 nestipy-0.1.7/src/nestipy/common/decorator/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      934 2024-03-01 12:17:25.314721 nestipy-0.1.7/src/nestipy/common/decorator/__pycache__/controller.cpython-311.pyc
--rw-r--r--   0        0        0     1075 2024-03-01 12:17:25.762807 nestipy-0.1.7/src/nestipy/common/decorator/__pycache__/dto.cpython-311.pyc
--rw-r--r--   0        0        0     1419 2024-03-08 07:12:41.967785 nestipy-0.1.7/src/nestipy/common/decorator/__pycache__/gateway.cpython-311.pyc
--rw-r--r--   0        0        0     1055 2024-03-01 12:17:25.334725 nestipy-0.1.7/src/nestipy/common/decorator/__pycache__/inject.cpython-311.pyc
--rw-r--r--   0        0        0      882 2024-03-01 12:17:25.330725 nestipy-0.1.7/src/nestipy/common/decorator/__pycache__/injectable.cpython-311.pyc
--rw-r--r--   0        0        0     3856 2024-03-08 07:12:42.567791 nestipy-0.1.7/src/nestipy/common/decorator/__pycache__/methods.cpython-311.pyc
--rw-r--r--   0        0        0     1101 2024-03-08 07:12:41.983785 nestipy-0.1.7/src/nestipy/common/decorator/__pycache__/middleware.cpython-311.pyc
--rw-r--r--   0        0        0     1396 2024-03-01 12:17:25.758806 nestipy-0.1.7/src/nestipy/common/decorator/__pycache__/module.cpython-311.pyc
--rw-r--r--   0        0        0     1924 2024-03-08 07:12:41.983785 nestipy-0.1.7/src/nestipy/common/decorator/__pycache__/use_gards.cpython-311.pyc
--rw-r--r--   0        0        0      354 2024-03-01 11:24:49.628082 nestipy-0.1.7/src/nestipy/common/decorator/catch.py
--rw-r--r--   0        0        0      379 2024-02-29 12:35:05.157461 nestipy-0.1.7/src/nestipy/common/decorator/controller.py
--rw-r--r--   0        0        0      495 2024-02-29 12:35:05.157461 nestipy-0.1.7/src/nestipy/common/decorator/dto.py
--rw-r--r--   0        0        0      587 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/decorator/gateway.py
--rw-r--r--   0        0        0      326 2024-02-29 12:35:05.157461 nestipy-0.1.7/src/nestipy/common/decorator/inject.py
--rw-r--r--   0        0        0      325 2024-02-29 12:35:05.157461 nestipy-0.1.7/src/nestipy/common/decorator/injectable.py
--rw-r--r--   0        0        0     1160 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/decorator/methods.py
--rw-r--r--   0        0        0      664 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/decorator/middleware.py
--rw-r--r--   0        0        0      848 2024-02-29 12:35:05.157461 nestipy-0.1.7/src/nestipy/common/decorator/module.py
--rw-r--r--   0        0        0      594 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/decorator/use_gards.py
--rw-r--r--   0        0        0       68 2024-02-29 12:35:05.157461 nestipy-0.1.7/src/nestipy/common/enum/__init__.py
--rw-r--r--   0        0        0      264 2024-03-01 12:17:25.318722 nestipy-0.1.7/src/nestipy/common/enum/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2024-03-01 12:17:25.318722 nestipy-0.1.7/src/nestipy/common/enum/__pycache__/platform.cpython-311.pyc
--rw-r--r--   0        0        0      101 2024-02-29 12:35:05.157461 nestipy-0.1.7/src/nestipy/common/enum/platform.py
--rw-r--r--   0        0        0      224 2024-02-29 12:35:05.157461 nestipy-0.1.7/src/nestipy/common/http_method.py
--rw-r--r--   0        0        0        0 2024-03-01 11:24:49.628082 nestipy-0.1.7/src/nestipy/common/params/__init__.py
--rw-r--r--   0        0        0      180 2024-03-01 12:17:25.766807 nestipy-0.1.7/src/nestipy/common/params/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      832 2024-03-01 12:17:25.766807 nestipy-0.1.7/src/nestipy/common/params/__pycache__/body.cpython-311.pyc
--rw-r--r--   0        0        0      257 2024-03-01 11:24:49.628082 nestipy-0.1.7/src/nestipy/common/params/body.py
--rw-r--r--   0        0        0        0 2024-03-01 11:24:49.628082 nestipy-0.1.7/src/nestipy/common/templates/__init__.py
--rw-r--r--   0        0        0      183 2024-03-01 12:42:00.916928 nestipy-0.1.7/src/nestipy/common/templates/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2905 2024-03-08 08:49:37.884268 nestipy-0.1.7/src/nestipy/common/templates/__pycache__/generator.cpython-311.pyc
--rw-r--r--   0        0        0     1068 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/templates/generator.py
--rw-r--r--   0        0        0     1072 2024-02-29 12:35:05.157461 nestipy-0.1.7/src/nestipy/common/templates/project/README.md
--rw-r--r--   0        0        0        0 2024-03-01 11:24:49.628082 nestipy-0.1.7/src/nestipy/common/templates/project/__init__.py
--rw-r--r--   0        0        0     2260 2024-03-07 07:31:13.933626 nestipy-0.1.7/src/nestipy/common/templates/project/__pycache__/app_controller.cpython-311.pyc
--rw-r--r--   0        0        0      730 2024-03-07 07:31:13.521612 nestipy-0.1.7/src/nestipy/common/templates/project/__pycache__/app_module.cpython-311.pyc
--rw-r--r--   0        0        0     1307 2024-03-07 07:31:13.933626 nestipy-0.1.7/src/nestipy/common/templates/project/__pycache__/app_service.cpython-311.pyc
--rw-r--r--   0        0        0      609 2024-03-07 07:31:13.969627 nestipy-0.1.7/src/nestipy/common/templates/project/__pycache__/main.cpython-311.pyc
--rw-r--r--   0        0        0      656 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/templates/project/app_controller.py
--rw-r--r--   0        0        0      219 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/templates/project/app_module.py
--rw-r--r--   0        0        0      384 2024-03-01 11:24:49.628082 nestipy-0.1.7/src/nestipy/common/templates/project/app_service.py
--rw-r--r--   0        0        0      249 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/templates/project/main.py
--rw-r--r--   0        0        0       14 2024-03-08 15:06:54.676433 nestipy-0.1.7/src/nestipy/common/templates/project/requirements.txt
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.157461 nestipy-0.1.7/src/nestipy/common/templates/project/src/__init__.py
--rw-r--r--   0        0        0      191 2024-03-01 11:24:23.348973 nestipy-0.1.7/src/nestipy/common/templates/project/src/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1020 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/templates/views/controller.txt
--rw-r--r--   0        0        0      187 2024-02-29 12:35:05.161460 nestipy-0.1.7/src/nestipy/common/templates/views/dto.txt
--rw-r--r--   0        0        0      322 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/templates/views/graphql_module.txt
--rw-r--r--   0        0        0      304 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/templates/views/graphql_service.txt
--rw-r--r--   0        0        0      119 2024-02-29 12:35:05.161460 nestipy-0.1.7/src/nestipy/common/templates/views/input.txt
--rw-r--r--   0        0        0      323 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/templates/views/module.txt
--rw-r--r--   0        0        0      703 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/templates/views/resolver.txt
--rw-r--r--   0        0        0      480 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/common/templates/views/service.txt
--rw-r--r--   0        0        0      178 2024-02-29 12:35:05.161460 nestipy-0.1.7/src/nestipy/common/templates/views/single_controller.txt
--rw-r--r--   0        0        0       97 2024-02-29 12:35:05.161460 nestipy-0.1.7/src/nestipy/common/templates/views/single_module.txt
--rw-r--r--   0        0        0      390 2024-02-29 12:35:05.161460 nestipy-0.1.7/src/nestipy/common/templates/views/single_resolver.txt
--rw-r--r--   0        0        0      137 2024-02-29 12:35:05.161460 nestipy-0.1.7/src/nestipy/common/templates/views/single_service.txt
--rw-r--r--   0        0        0      503 2024-02-29 12:35:05.161460 nestipy-0.1.7/src/nestipy/core/__init__.py
--rw-r--r--   0        0        0      746 2024-03-01 12:17:25.318722 nestipy-0.1.7/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16492 2024-03-08 15:06:08.859580 nestipy-0.1.7/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
--rw-r--r--   0        0        0     1929 2024-03-01 12:17:25.758806 nestipy-0.1.7/src/nestipy/core/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     1567 2024-03-01 12:17:25.318722 nestipy-0.1.7/src/nestipy/core/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     8980 2024-03-08 15:06:02.527459 nestipy-0.1.7/src/nestipy/core/app_context.py
--rw-r--r--   0        0        0      836 2024-02-29 12:35:05.161460 nestipy-0.1.7/src/nestipy/core/factory.py
--rw-r--r--   0        0        0       40 2024-02-29 12:35:05.161460 nestipy-0.1.7/src/nestipy/core/ioc/__init__.py
--rw-r--r--   0        0        0      239 2024-03-01 12:17:25.334725 nestipy-0.1.7/src/nestipy/core/ioc/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6413 2024-03-08 07:12:41.987785 nestipy-0.1.7/src/nestipy/core/ioc/__pycache__/container.cpython-311.pyc
--rw-r--r--   0        0        0     3979 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/core/ioc/container.py
--rw-r--r--   0        0        0      139 2024-02-29 12:35:05.161460 nestipy-0.1.7/src/nestipy/core/module/__init__.py
--rw-r--r--   0        0        0      346 2024-03-01 12:17:25.318722 nestipy-0.1.7/src/nestipy/core/module/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5172 2024-03-08 07:12:41.971785 nestipy-0.1.7/src/nestipy/core/module/__pycache__/compiler.cpython-311.pyc
--rw-r--r--   0        0        0     1681 2024-03-08 07:12:41.979785 nestipy-0.1.7/src/nestipy/core/module/__pycache__/hook_compiler.cpython-311.pyc
--rw-r--r--   0        0        0     1769 2024-03-08 13:41:17.100632 nestipy-0.1.7/src/nestipy/core/module/__pycache__/middleware.cpython-311.pyc
--rw-r--r--   0        0        0     5314 2024-03-08 13:46:57.359955 nestipy-0.1.7/src/nestipy/core/module/__pycache__/middleware_compiler.cpython-311.pyc
--rw-r--r--   0        0        0     1005 2024-03-01 12:17:25.322723 nestipy-0.1.7/src/nestipy/core/module/__pycache__/nestipy.cpython-311.pyc
--rw-r--r--   0        0        0      931 2024-03-01 12:17:25.330725 nestipy-0.1.7/src/nestipy/core/module/__pycache__/provider.cpython-311.pyc
--rw-r--r--   0        0        0    10726 2024-03-08 07:12:41.987785 nestipy-0.1.7/src/nestipy/core/module/__pycache__/provider_compiler.cpython-311.pyc
--rw-r--r--   0        0        0     2636 2024-03-08 07:10:04.734124 nestipy-0.1.7/src/nestipy/core/module/compiler.py
--rw-r--r--   0        0        0      646 2024-03-08 07:10:04.738124 nestipy-0.1.7/src/nestipy/core/module/hook_compiler.py
--rw-r--r--   0        0        0      576 2024-03-08 13:37:16.242046 nestipy-0.1.7/src/nestipy/core/module/middleware.py
--rw-r--r--   0        0        0     3303 2024-03-08 13:46:48.832043 nestipy-0.1.7/src/nestipy/core/module/middleware_compiler.py
--rw-r--r--   0        0        0      275 2024-03-01 11:24:49.632081 nestipy-0.1.7/src/nestipy/core/module/nestipy.py
--rw-r--r--   0        0        0      276 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/core/module/provider.py
--rw-r--r--   0        0        0     6293 2024-03-08 07:10:04.738124 nestipy-0.1.7/src/nestipy/core/module/provider_compiler.py
--rw-r--r--   0        0        0      216 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/core/platform/__init__.py
--rw-r--r--   0        0        0      437 2024-03-01 12:17:25.338726 nestipy-0.1.7/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3199 2024-03-08 07:12:41.991785 nestipy-0.1.7/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
--rw-r--r--   0        0        0     7185 2024-03-08 12:41:34.260097 nestipy-0.1.7/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
--rw-r--r--   0        0        0     7397 2024-03-08 07:12:41.995785 nestipy-0.1.7/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
--rw-r--r--   0        0        0     1071 2024-03-08 07:10:04.738124 nestipy-0.1.7/src/nestipy/core/platform/platform.py
--rw-r--r--   0        0        0     3838 2024-03-08 12:41:27.436121 nestipy-0.1.7/src/nestipy/core/platform/platform_fastapi.py
--rw-r--r--   0        0        0     3983 2024-03-08 07:10:04.738124 nestipy-0.1.7/src/nestipy/core/platform/platform_litestar.py
--rw-r--r--   0        0        0      710 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/core/utils.py
--rw-r--r--   0        0        0     1288 2024-03-08 14:49:28.294752 nestipy-0.1.7/src/nestipy/middlewares/__pycache__/cors.cpython-311.pyc
--rw-r--r--   0        0        0     1291 2024-03-08 14:49:28.294752 nestipy-0.1.7/src/nestipy/middlewares/__pycache__/hemlet.cpython-311.pyc
--rw-r--r--   0        0        0     2700 2024-03-08 14:49:28.294752 nestipy-0.1.7/src/nestipy/middlewares/__pycache__/rate_limit.cpython-311.pyc
--rw-r--r--   0        0        0      563 2024-03-08 14:47:40.446425 nestipy-0.1.7/src/nestipy/middlewares/cors.py
--rw-r--r--   0        0        0      578 2024-03-08 14:48:47.603786 nestipy-0.1.7/src/nestipy/middlewares/hemlet.py
--rw-r--r--   0        0        0     1194 2024-03-08 14:38:20.684464 nestipy-0.1.7/src/nestipy/middlewares/rate_limit.py
--rw-r--r--   0        0        0        0 2024-03-08 07:10:04.738124 nestipy-0.1.7/src/nestipy/plugins/beanie_module/__init__.py
--rw-r--r--   0        0        0      188 2024-03-08 07:12:43.667802 nestipy-0.1.7/src/nestipy/plugins/beanie_module/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4479 2024-03-08 07:12:43.667802 nestipy-0.1.7/src/nestipy/plugins/beanie_module/__pycache__/beanie_module.cpython-311.pyc
--rw-r--r--   0        0        0      218 2024-03-08 07:12:44.047806 nestipy-0.1.7/src/nestipy/plugins/beanie_module/__pycache__/constant.cpython-311.pyc
--rw-r--r--   0        0        0     2529 2024-03-08 07:10:04.738124 nestipy-0.1.7/src/nestipy/plugins/beanie_module/beanie_module.py
--rw-r--r--   0        0        0       46 2024-03-08 07:10:04.738124 nestipy-0.1.7/src/nestipy/plugins/beanie_module/constant.py
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/config_module/__init__.py
--rw-r--r--   0        0        0      188 2024-03-01 12:17:25.770808 nestipy-0.1.7/src/nestipy/plugins/config_module/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1384 2024-03-01 12:17:26.122875 nestipy-0.1.7/src/nestipy/plugins/config_module/__pycache__/config_module.cpython-311.pyc
--rw-r--r--   0        0        0     1072 2024-03-01 12:17:25.770808 nestipy-0.1.7/src/nestipy/plugins/config_module/__pycache__/config_service.cpython-311.pyc
--rw-r--r--   0        0        0      217 2024-03-01 12:17:25.770808 nestipy-0.1.7/src/nestipy/plugins/config_module/__pycache__/constant.cpython-311.pyc
--rw-r--r--   0        0        0      580 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/config_module/config_module.py
--rw-r--r--   0        0        0      313 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/config_module/config_service.py
--rw-r--r--   0        0        0       44 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/config_module/constant.py
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/database_module/__init__.py
--rw-r--r--   0        0        0       48 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/database_module/constant.py
--rw-r--r--   0        0        0      659 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/database_module/database_module.py
--rw-r--r--   0        0        0      285 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/database_module/database_service.py
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/dynamic_module/__init__.py
--rw-r--r--   0        0        0      189 2024-03-01 12:17:25.334725 nestipy-0.1.7/src/nestipy/plugins/dynamic_module/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2942 2024-03-01 12:17:25.338726 nestipy-0.1.7/src/nestipy/plugins/dynamic_module/__pycache__/dynamic_module.cpython-311.pyc
--rw-r--r--   0        0        0     1442 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/dynamic_module/dynamic_module.py
--rw-r--r--   0        0        0        0 2024-03-01 11:24:49.632081 nestipy-0.1.7/src/nestipy/plugins/masonite_orm_module/__init__.py
--rw-r--r--   0        0        0      194 2024-03-01 12:17:25.774809 nestipy-0.1.7/src/nestipy/plugins/masonite_orm_module/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4865 2024-03-01 12:17:25.774809 nestipy-0.1.7/src/nestipy/plugins/masonite_orm_module/__pycache__/masonite_orm_module.cpython-311.pyc
--rw-r--r--   0        0        0     2639 2024-03-01 11:24:49.632081 nestipy-0.1.7/src/nestipy/plugins/masonite_orm_module/masonite_orm_module.py
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/peewee_module/__init__.py
--rw-r--r--   0        0        0      188 2024-03-01 12:17:25.902833 nestipy-0.1.7/src/nestipy/plugins/peewee_module/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      218 2024-03-01 12:17:25.926838 nestipy-0.1.7/src/nestipy/plugins/peewee_module/__pycache__/constant.cpython-311.pyc
--rw-r--r--   0        0        0      466 2024-03-01 12:17:26.382924 nestipy-0.1.7/src/nestipy/plugins/peewee_module/__pycache__/decorator.cpython-311.pyc
--rw-r--r--   0        0        0     8461 2024-03-08 07:12:42.807793 nestipy-0.1.7/src/nestipy/plugins/peewee_module/__pycache__/peewee_module.cpython-311.pyc
--rw-r--r--   0        0        0      993 2024-03-01 12:17:25.926838 nestipy-0.1.7/src/nestipy/plugins/peewee_module/__pycache__/peewee_service.cpython-311.pyc
--rw-r--r--   0        0        0       46 2024-03-01 11:24:49.632081 nestipy-0.1.7/src/nestipy/plugins/peewee_module/constant.py
--rw-r--r--   0        0        0      125 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/peewee_module/decorator.py
--rw-r--r--   0        0        0     4566 2024-03-08 07:10:04.738124 nestipy-0.1.7/src/nestipy/plugins/peewee_module/peewee_module.py
--rw-r--r--   0        0        0      292 2024-03-01 11:24:49.632081 nestipy-0.1.7/src/nestipy/plugins/peewee_module/peewee_service.py
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.165460 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/__init__.py
--rw-r--r--   0        0        0      192 2024-03-01 12:17:26.122875 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12222 2024-03-08 08:20:23.362257 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/__pycache__/compiler.cpython-311.pyc
--rw-r--r--   0        0        0      226 2024-03-01 12:17:26.326913 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/__pycache__/constant.cpython-311.pyc
--rw-r--r--   0        0        0     3998 2024-03-01 12:17:26.382924 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/__pycache__/decorator.cpython-311.pyc
--rw-r--r--   0        0        0     2032 2024-03-01 12:17:26.126875 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/__pycache__/pubsub.cpython-311.pyc
--rw-r--r--   0        0        0     7348 2024-03-08 11:31:04.501852 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/__pycache__/strawberry_middleware.cpython-311.pyc
--rw-r--r--   0        0        0     3709 2024-03-08 07:12:42.871794 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/__pycache__/strawberry_module.cpython-311.pyc
--rw-r--r--   0        0        0     6023 2024-03-08 08:20:15.314789 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/compiler.py
--rw-r--r--   0        0        0       54 2024-02-29 12:35:05.169460 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/constant.py
--rw-r--r--   0        0        0     1500 2024-02-29 12:35:05.169460 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/decorator.py
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.169460 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/override/__init__.py
--rw-r--r--   0        0        0      201 2024-03-01 12:17:26.322913 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/override/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2742 2024-03-08 07:12:43.611801 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/override/__pycache__/field.cpython-311.pyc
--rw-r--r--   0        0        0     2388 2024-03-08 07:12:43.615801 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/override/__pycache__/resolver.cpython-311.pyc
--rw-r--r--   0        0        0     2097 2024-03-08 07:10:04.738124 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/override/field.py
--rw-r--r--   0        0        0     1341 2024-03-08 07:10:04.738124 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/override/resolver.py
--rw-r--r--   0        0        0      747 2024-02-29 12:35:05.169460 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/pubsub.py
--rw-r--r--   0        0        0     3812 2024-03-08 11:30:31.830322 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/strawberry_middleware.py
--rw-r--r--   0        0        0     1795 2024-03-08 07:10:04.738124 nestipy-0.1.7/src/nestipy/plugins/strawberry_module/strawberry_module.py
--rw-r--r--   0        0        0        0 2024-03-01 11:24:49.632081 nestipy-0.1.7/src/nestipy/types/__init__.py
--rw-r--r--   0        0        0     8809 2024-03-08 07:11:22.538957 nestipy-0.1.7/src/nestipy/types/asgi.py
--rw-r--r--   0        0        0     3441 1970-01-01 00:00:00.000000 nestipy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1913 2024-04-26 12:17:55.140372 nestipy-0.2.0/README.md
+-rw-r--r--   0        0        0     1046 2024-04-26 12:17:55.152372 nestipy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-29 12:35:05.153461 nestipy-0.2.0/src/nestipy/__init__.py
+-rw-r--r--   0        0        0     1151 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/__init__.py
+-rw-r--r--   0        0        0     1489 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      652 2024-03-29 11:21:44.572810 nestipy-0.2.0/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
+-rw-r--r--   0        0        0      978 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/config/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/decorator/__init__.py
+-rw-r--r--   0        0        0     2957 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/decorator/class_.py
+-rw-r--r--   0        0        0     1204 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/decorator/method.py
+-rw-r--r--   0        0        0      367 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/decorator.py
+-rw-r--r--   0        0        0      433 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/http.py
+-rw-r--r--   0        0        0      364 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/interface.py
+-rw-r--r--   0        0        0     2531 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/message.py
+-rw-r--r--   0        0        0      113 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/meta.py
+-rw-r--r--   0        0        0     1686 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/status.py
+-rw-r--r--   0        0        0      164 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/guards/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/guards/can_activate.py
+-rw-r--r--   0        0        0      332 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/guards/decorator.py
+-rw-r--r--   0        0        0       45 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/guards/meta.py
+-rw-r--r--   0        0        0      719 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/helpers/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/__init__.py
+-rw-r--r--   0        0        0     4503 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/multipart.py
+-rw-r--r--   0        0        0     4231 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/request.py
+-rw-r--r--   0        0        0     4989 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/response.py
+-rw-r--r--   0        0        0      478 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/test.py
+-rw-r--r--   0        0        0     1403 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/upload_file.py
+-rw-r--r--   0        0        0      303 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/websocket.py
+-rw-r--r--   0        0        0      199 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/interceptor/__init__.py
+-rw-r--r--   0        0        0      489 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/interceptor/decorator.py
+-rw-r--r--   0        0        0      352 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/interceptor/interface.py
+-rw-r--r--   0        0        0       52 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/interceptor/meta.py
+-rw-r--r--   0        0        0      168 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/middleware/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/middleware/cors.py
+-rw-r--r--   0        0        0      323 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/middleware/interface.py
+-rw-r--r--   0        0        0      100 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/middleware/meta.py
+-rw-r--r--   0        0        0      167 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/template/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/template/decorator.py
+-rw-r--r--   0        0        0      627 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/template/interface.py
+-rw-r--r--   0        0        0      109 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/template/meta.py
+-rw-r--r--   0        0        0     1590 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/utils.py
+-rw-r--r--   0        0        0      779 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/__init__.py
+-rw-r--r--   0        0        0      986 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16492 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
+-rw-r--r--   0        0        0     1929 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     1567 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      212 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/adapter/__init__.py
+-rw-r--r--   0        0        0     4224 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/adapter/blacksheep_adapter.py
+-rw-r--r--   0        0        0     3803 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/adapter/fastapi_adapter.py
+-rw-r--r--   0        0        0     5666 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/adapter/http_adapter.py
+-rw-r--r--   0        0        0      418 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/constant.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/context/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/context/argument_host.py
+-rw-r--r--   0        0        0      802 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/context/execution_context.py
+-rw-r--r--   0        0        0      369 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/context/http_argument_host.py
+-rw-r--r--   0        0        0       90 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/exception/__init__.py
+-rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/exception/processor.py
+-rw-r--r--   0        0        0       75 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/guards/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/guards/processor.py
+-rw-r--r--   0        0        0     2758 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/instance_loader.py
+-rw-r--r--   0        0        0       82 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/interceptor/__init__.py
+-rw-r--r--   0        0        0     2569 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/interceptor/processor.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/meta/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/meta/controller_metadata_creator.py
+-rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/meta/metadata_creator.py
+-rw-r--r--   0        0        0      771 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/meta/module_metadata_creator.py
+-rw-r--r--   0        0        0      374 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/meta/provider_metadata_creator.py
+-rw-r--r--   0        0        0      162 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/middleware/__init__.py
+-rw-r--r--   0        0        0     3949 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/middleware/executor.py
+-rw-r--r--   0        0        0     8673 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/nestipy_application.py
+-rw-r--r--   0        0        0      913 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/nestipy_factory.py
+-rw-r--r--   0        0        0       89 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/platform/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3199 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
+-rw-r--r--   0        0        0     7185 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
+-rw-r--r--   0        0        0     7397 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/router/__init__.py
+-rw-r--r--   0        0        0     2879 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/router/route_explorer.py
+-rw-r--r--   0        0        0      510 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/router/route_extractor.py
+-rw-r--r--   0        0        0     7859 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/router/router_proxy.py
+-rw-r--r--   0        0        0      184 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/template/__init__.py
+-rw-r--r--   0        0        0     1004 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/template/minimal_jinja.py
+-rw-r--r--   0        0        0     1457 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/template/processor.py
+-rw-r--r--   0        0        0      282 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/__init__.py
+-rw-r--r--   0        0        0     1533 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/decorator.py
+-rw-r--r--   0        0        0     2244 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/graphql_adapter.py
+-rw-r--r--   0        0        0     1111 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/graphql_asgi.py
+-rw-r--r--   0        0        0     1871 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/graphql_explorer.py
+-rw-r--r--   0        0        0      547 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/graphql_module.py
+-rw-r--r--   0        0        0     4326 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/graphql_proxy.py
+-rw-r--r--   0        0        0      289 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/meta.py
+-rw-r--r--   0        0        0     1531 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/playground/graphql-playground-default.html
+-rw-r--r--   0        0        0     3486 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/playground/graphql-playground-graphiql.html
+-rw-r--r--   0        0        0      704 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/pubsub.py
+-rw-r--r--   0        0        0      648 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/strawberry/__init__.py
+-rw-r--r--   0        0        0     2103 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/strawberry/strawberry_adapter.py
+-rw-r--r--   0        0        0     1588 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/strawberry/strawberry_asgi.py
+-rw-r--r--   0        0        0      110 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/test.py
+-rw-r--r--   0        0        0     1105 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/constant.py
+-rw-r--r--   0        0        0     3139 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/decorator.py
+-rw-r--r--   0        0        0     1500 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/document_builder.py
+-rw-r--r--   0        0        0      423 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/explorer.py
+-rw-r--r--   0        0        0     1323 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/swagger.html
+-rw-r--r--   0        0        0     2195 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/swagger_module.py
+-rw-r--r--   0        0        0     2728 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/test.py
+-rw-r--r--   0        0        0      220 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/types_/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/types_/handler.py
+-rw-r--r--   0        0        0      123 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/types_/http.py
+-rw-r--r--   0        0        0      254 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/websocket/__init__.py
+-rw-r--r--   0        0        0     2988 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/websocket/adapter.py
+-rw-r--r--   0        0        0      716 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/websocket/decorator.py
+-rw-r--r--   0        0        0     4517 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/websocket/proxy.py
+-rw-r--r--   0        0        0     3554 1970-01-01 00:00:00.000000 nestipy-0.2.0/PKG-INFO
```

### Comparing `nestipy-0.1.7/LICENSE` & `nestipy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy-0.1.7/pyproject.toml` & `nestipy-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 [tool.poetry]
 name = "nestipy"
-version = "0.1.7"
-description = "Nestipy is a Python framework built on top of Litestar that follows the modular architecture of NestJS"
+version = "0.2.0"
+description = "Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
-packages = [{include = "nestipy", from = "src"}]
+packages = [{ include = "nestipy", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 litestar = "^2.6.1"
-fastapi = "^0.109.2"
 pymysql = "^1.1.0"
-uvicorn = {extras = ["standard"], version = "^0.27.1"}
 peewee = "^3.17.1"
 python-dotenv = "^1.0.1"
 minijinja = "^1.0.8"
 pyee = "^11.1.0"
 snakecase = "^1.0.1"
-strawberry-graphql = "^0.219.2"
 pathlib2 = "^2.3.7.post1"
 questionary = "^2.0.1"
 click-aliases = "^1.0.4"
-fastapi-utils = "^0.2.1"
 masonite-orm = "^2.20.0"
 beanie = "^1.25.0"
 python-socketio = "^5.11.1"
 autopep8 = "^2.0.4"
 isort = "^5.13.2"
 autoflake = "^2.3.0"
+blacksheep = "^2.0.7"
+aiofiles = "^23.2.1"
+fastapi = "^0.110.0"
+uvicorn = { extras = ["standard"], version = "^0.29.0" }
+strawberry-graphql = "^0.225.0"
+ujson = "^5.9.0"
+aiofile = "^3.8.8"
+nestipy-ioc = "^0.1.30"
+nestipy-metadata = "^0.1.1"
+nestipy-dynamic-module = "^0.1.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.poetry.scripts]
-nestipy = "nestipy.cli.cli:main"
```

### Comparing `nestipy-0.1.7/src/nestipy/common/__pycache__/http_method.cpython-311.pyc` & `nestipy-0.2.0/src/nestipy/common/__pycache__/http_method.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.1.7/src/nestipy/core/__pycache__/app_context.cpython-311.pyc` & `nestipy-0.2.0/src/nestipy/core/__pycache__/app_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.1.7/src/nestipy/core/__pycache__/factory.cpython-311.pyc` & `nestipy-0.2.0/src/nestipy/core/__pycache__/factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.1.7/src/nestipy/core/__pycache__/utils.cpython-311.pyc` & `nestipy-0.2.0/src/nestipy/core/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.1.7/src/nestipy/core/module/compiler.py` & `nestipy-0.2.0/src/nestipy/core/instance_loader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,72 @@
-import inspect
-from typing import Callable, Any
-
-from pyee import EventEmitter
-
-from .hook_compiler import HookCompiler
-from .middleware import MiddlewareDict
-from .middleware_compiler import MiddlewareCompiler
-from .provider_compiler import ProviderCompiler
-from ..ioc import NestipyContainer
-from ...plugins.dynamic_module.dynamic_module import DynamicModule
-
-
-class ModuleCompiler:
-    # module: Any
-    middlewares: list[MiddlewareDict]
-
-    def __init__(self):
-        # self.module = module
-        self.container = NestipyContainer()
-        self.module_resolved = {}
-        self.hooks = {}
-        self.middlewares = []
-        self.ee = EventEmitter()
-        self.hook_compiler = HookCompiler(self)
-        self.middleware_compiler = MiddlewareCompiler(self)
-        self.provider_compiler = ProviderCompiler(self)
-
-    def modify_module_imports(self, module, global_modules):
-        self.remove_module_none_imported(module)
-        filtered_global_modules = [m for m in global_modules if m != module]
-        module_imports: list = (module.imports or [])
-        module_imports_with_global = filtered_global_modules + module_imports
-        setattr(module, 'imports', module_imports_with_global)
-        if issubclass(module, DynamicModule):
-            setattr(module, 'container__', self.container)
-
-    @classmethod
-    def remove_module_none_imported(cls, module):
-        setattr(module, 'imports', [im for im in (module.imports or []) if im is not None])
-
-    async def resolve_controllers_of_module(self, module):
-        controllers = [ctrl for ctrl in module.controllers if hasattr(ctrl, 'controller__')]
-        for ctrl in controllers:
-            if inspect.isclass(ctrl):
-                self.container.resolve(ctrl, module)
-            else:
-                token = ctrl.token__
-                self.container.resolve_method(ctrl, token=token)
-
-    @classmethod
-    def put_module_provider_instance(cls, module, token, instance, is_middleware=False):
-        if is_middleware:
-            cls.put_module_element(module, 'middleware_instances__', token, instance)
-        else:
-            cls.put_module_element(module, 'provider_instances__', token, instance)
+import enum
+import typing
+from typing import Type, Any
+
+from nestipy_dynamic_module import DynamicModule, MiddlewareConsumer, NestipyModule
+from nestipy_ioc import NestipyContainer, ModuleProviderDict
+from nestipy_metadata import ModuleMetadata, Reflect
+
+from ..graphql.graphql_module import GraphqlModule
+
+
+class InstanceType(enum.Enum):
+    providers: str = 'Provider'
+    controller: str = 'Controller',
+    module: str = 'Module'
+
+
+class InstanceLoader:
+    """
+    Create all instance of controller and providers, resolvers, middleware
+    use before route mapper
+    """
+    _is_controller: bool = False
+    _module_instances: list = []
+    graphql_instance: GraphqlModule = None
+
+    async def create_instances(self, modules: list[Type]) -> GraphqlModule:
+        for module in modules:
+            if isinstance(module, DynamicModule):
+                module = module.module
+            if module in self._module_instances:
+                continue
+            await self._create_providers(module)
+            self._is_controller = True
+            await self._create_controllers(module)
+            self._is_controller = False
+            instance = await self.create_instance(module)
+            self._module_instances.append(module)
+            if isinstance(instance, GraphqlModule):
+                self.graphql_instance = instance
+            imports = Reflect.get_metadata(module, ModuleMetadata.Imports, [])
+            await self.create_instances(imports)
+        return self.graphql_instance
+
+    async def _create_providers(self, module: Type) -> None:
+        for provider in Reflect.get_metadata(module, ModuleMetadata.Providers, []):
+            if isinstance(provider, ModuleProviderDict):
+                continue
+            await self.create_instance(provider)
+
+    async def _create_controllers(self, module: Type) -> None:
+        for controller in Reflect.get_metadata(module, ModuleMetadata.Controllers, []):
+            await self.create_instance(controller)
+
+    async def create_instance(self, class_ref: Type) -> object:
+        instance = await NestipyContainer.get_instance().get(class_ref)
+        await self.initialize_instance(class_ref, instance)
+        return instance
 
     @classmethod
-    def put_module_element(cls, module, element_type, key, value):
-        instances__ = {}
-        if hasattr(module, element_type):
-            instances__ = getattr(module, element_type)
-        instances__[key] = value
-        setattr(module, element_type, instances__)
-
-    # MIDDLEWARE
-
-    # COMPILE
-    async def compile(self, module):
-        await self.provider_compiler.compile(module, init=True)
-        return module
+    async def initialize_instance(cls, class_ref: Type, instance: Any) -> None:
+        # call configure for module
+        if issubclass(class_ref, NestipyModule):
+            consumer = MiddlewareConsumer(module=class_ref)
+            module = typing.cast(NestipyModule, instance)
+            module.configure(consumer)
+            await module.on_startup()
+
+    async def destroy(self):
+        for module in self._module_instances:
+            if isinstance(module, NestipyModule):
+                await module.on_shutdown()
```

### Comparing `nestipy-0.1.7/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc` & `nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.1.7/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc` & `nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.1.7/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc` & `nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.1.7/src/nestipy/middlewares/cors.py` & `nestipy-0.2.0/src/nestipy/common/middleware/cors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from typing import Callable, Awaitable, Any
+from typing import Type
 
-from nestipy.common import NestipyMiddleware
-from nestipy.common.context import Request, Response
+from nestipy.common.decorator import Injectable
 
+from nestipy.types_ import NextFn
+from nestipy.common.middleware.interface import NestipyMiddleware
+from nestipy.common.http_ import Request, Response
 
-class CORSMiddleware(NestipyMiddleware):
 
-    async def use(self, request: Request, response: Response, next_function: Callable[..., Awaitable]) -> None:
-        response.add_headers([
-            ('access-control-allow-origin', '*'),
-            ('access-control-allow-methods', 'GET, POST, PUT, DELETE, OPTIONS'),
-            ('access-control-allow-headers', 'Content-Type')
-        ])
-        await next_function()
+def cors() -> Type:
+    @Injectable()
+    class CorsMiddleware(NestipyMiddleware):
+        async def use(self, req: Request, res: Response, next_fn: NextFn):
+            result = await next_fn()
+            res.header('access-control-allow-origin', '*')
+            res.header('access-control-allow-headers', 'content-type')
+            res.header('access-control-allow-methods', 'GET, POST, PUT, DELETE, OPTIONS')
+            return result
+
+    return CorsMiddleware
```

### Comparing `nestipy-0.1.7/src/nestipy/plugins/strawberry_module/pubsub.py` & `nestipy-0.2.0/src/nestipy/graphql/pubsub.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import asyncio
 from typing import Any
 
 from pyee import EventEmitter
 
-STRAWBERRY_PUB_SUB = "STRAWBERRY_PUB_SUB"
-
 
 class PubSub:
     def __init__(self):
         self.ee = EventEmitter()
 
     async def asyncIterator(self, event: str):
         loop = asyncio.get_event_loop()
```

### Comparing `nestipy-0.1.7/PKG-INFO` & `nestipy-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,69 @@
 Metadata-Version: 2.1
 Name: nestipy
-Version: 0.1.7
-Summary: Nestipy is a Python framework built on top of Litestar that follows the modular architecture of NestJS
+Version: 0.2.0
+Summary: Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiofile (>=3.8.8,<4.0.0)
+Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: autoflake (>=2.3.0,<3.0.0)
 Requires-Dist: autopep8 (>=2.0.4,<3.0.0)
 Requires-Dist: beanie (>=1.25.0,<2.0.0)
+Requires-Dist: blacksheep (>=2.0.7,<3.0.0)
 Requires-Dist: click-aliases (>=1.0.4,<2.0.0)
-Requires-Dist: fastapi (>=0.109.2,<0.110.0)
-Requires-Dist: fastapi-utils (>=0.2.1,<0.3.0)
+Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: isort (>=5.13.2,<6.0.0)
 Requires-Dist: litestar (>=2.6.1,<3.0.0)
 Requires-Dist: masonite-orm (>=2.20.0,<3.0.0)
 Requires-Dist: minijinja (>=1.0.8,<2.0.0)
+Requires-Dist: nestipy-dynamic-module (>=0.1.3,<0.2.0)
+Requires-Dist: nestipy-ioc (>=0.1.30,<0.2.0)
+Requires-Dist: nestipy-metadata (>=0.1.1,<0.2.0)
 Requires-Dist: pathlib2 (>=2.3.7.post1,<3.0.0)
 Requires-Dist: peewee (>=3.17.1,<4.0.0)
 Requires-Dist: pyee (>=11.1.0,<12.0.0)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-socketio (>=5.11.1,<6.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: snakecase (>=1.0.1,<2.0.0)
-Requires-Dist: strawberry-graphql (>=0.219.2,<0.220.0)
-Requires-Dist: uvicorn[standard] (>=0.27.1,<0.28.0)
+Requires-Dist: strawberry-graphql (>=0.225.0,<0.226.0)
+Requires-Dist: ujson (>=5.9.0,<6.0.0)
+Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <a target="_blank"><img src="https://raw.githubusercontent.com/tsiresymila1/nestipy/main/nestipy.png" width="200" alt="Nestipy Logo" /></a></p>
+  <a target="_blank"><img src="https://raw.githubusercontent.com/nestipy/nestipy/release-v1/nestipy.png" width="200" alt="Nestipy Logo" /></a></p>
 <p align="center">
     <a href="https://pypi.org/project/nestipy">
         <img src="https://img.shields.io/pypi/v/nestipy?color=%2334D058&label=pypi%20package" alt="Version">
     </a>
     <a href="https://pypi.org/project/nestipy">
         <img src="https://img.shields.io/pypi/pyversions/nestipy.svg?color=%2334D058" alt="Python">
     </a>
     <a href="https://github.com/tsiresymila1/nestipy/blob/main/LICENSE">
         <img src="https://img.shields.io/github/license/tsiresymila1/nestipy" alt="License">
     </a>
 </p>
 
 ## Description
 
-<p>Nestipy is a Python framework built on top of Litestar that follows the modular architecture of NestJS</p>
-<p>Under the hood, Nestipy makes use of <a href="https://litestar.dev/" target="_blank">Litestar</a>, but also provides compatibility with a wide range of other libraries, like <a href="https://fastapi.tiangolo.com/" target="_blank">FastAPI</a>, allowing for easy use of the myriad of third-party plugins which are available.</p>
+<p>Nestipy is a Python framework built on top of FastAPI that follows the modular architecture of NestJS</p>
+<p>Under the hood, Nestipy makes use of <a href="https://fastapi.tiangolo.com/" target="_blank">FastAPI</a>, but also provides compatibility with a wide range of other libraries, like <a href="https://fastapi.tiangolo.com/" target="_blank">Blacksheep</a>, allowing for easy use of the myriad of third-party plugins which are available.</p>
 
 ## Getting started
 
 ```cmd
-    pip install nestipy
+    pip install nestipy-cli
     nestipy new my_app
     cd my_app
     python main.py
 ```
 
 ```
     ├── src
@@ -68,26 +74,24 @@
     ├── main.py
     ├── requirements.txt
     ├── README.md
     
        
 ```
 
-## [Documentation](https://tsiresymila1.github.io/nestipy)
+## Documentation
 
-## Issues
-
-Please make sure to read the [Issue Reporting Checklist](https://github.com/tsiresymila1/nestipy) before opening an
-issue. Issues not conforming to the guidelines may be closed immediately.
+View full documentation from [here](https://nestipy.github.io/nestipy).
 
 ## Support
 
 Nestipy is an MIT-licensed open source project. It can grow thanks to the sponsors and support from the amazing backers.
 If you'd like to join them, please [read more here].
 
 ## Stay in touch
 
 - Author - [Tsiresy Mila](https://tsiresymila.vercel.app)
 
 ## License
 
 Nestipy is [MIT licensed](LICENSE).
+
```

#### html2text {}

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1 Name: nestipy Version: 0.1.7 Summary: Nestipy is a Python
-framework built on top of Litestar that follows the modular architecture of
+Metadata-Version: 2.1 Name: nestipy Version: 0.2.0 Summary: Nestipy is a Python
+framework built on top of BlackSheep that follows the modular architecture of
 NestJS Author: tsiresymila Author-email: tsiresymila@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
-Dist: autoflake (>=2.3.0,<3.0.0) Requires-Dist: autopep8 (>=2.0.4,<3.0.0)
-Requires-Dist: beanie (>=1.25.0,<2.0.0) Requires-Dist: click-aliases
-(>=1.0.4,<2.0.0) Requires-Dist: fastapi (>=0.109.2,<0.110.0) Requires-Dist:
-fastapi-utils (>=0.2.1,<0.3.0) Requires-Dist: isort (>=5.13.2,<6.0.0) Requires-
-Dist: litestar (>=2.6.1,<3.0.0) Requires-Dist: masonite-orm (>=2.20.0,<3.0.0)
-Requires-Dist: minijinja (>=1.0.8,<2.0.0) Requires-Dist: pathlib2
-(>=2.3.7.post1,<3.0.0) Requires-Dist: peewee (>=3.17.1,<4.0.0) Requires-Dist:
-pyee (>=11.1.0,<12.0.0) Requires-Dist: pymysql (>=1.1.0,<2.0.0) Requires-Dist:
-python-dotenv (>=1.0.1,<2.0.0) Requires-Dist: python-socketio (>=5.11.1,<6.0.0)
-Requires-Dist: questionary (>=2.0.1,<3.0.0) Requires-Dist: snakecase
-(>=1.0.1,<2.0.0) Requires-Dist: strawberry-graphql (>=0.219.2,<0.220.0)
-Requires-Dist: uvicorn[standard] (>=0.27.1,<0.28.0) Description-Content-Type:
-text/markdown
+Dist: aiofile (>=3.8.8,<4.0.0) Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
+Requires-Dist: autoflake (>=2.3.0,<3.0.0) Requires-Dist: autopep8
+(>=2.0.4,<3.0.0) Requires-Dist: beanie (>=1.25.0,<2.0.0) Requires-Dist:
+blacksheep (>=2.0.7,<3.0.0) Requires-Dist: click-aliases (>=1.0.4,<2.0.0)
+Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: isort
+(>=5.13.2,<6.0.0) Requires-Dist: litestar (>=2.6.1,<3.0.0) Requires-Dist:
+masonite-orm (>=2.20.0,<3.0.0) Requires-Dist: minijinja (>=1.0.8,<2.0.0)
+Requires-Dist: nestipy-dynamic-module (>=0.1.3,<0.2.0) Requires-Dist: nestipy-
+ioc (>=0.1.30,<0.2.0) Requires-Dist: nestipy-metadata (>=0.1.1,<0.2.0)
+Requires-Dist: pathlib2 (>=2.3.7.post1,<3.0.0) Requires-Dist: peewee
+(>=3.17.1,<4.0.0) Requires-Dist: pyee (>=11.1.0,<12.0.0) Requires-Dist: pymysql
+(>=1.1.0,<2.0.0) Requires-Dist: python-dotenv (>=1.0.1,<2.0.0) Requires-Dist:
+python-socketio (>=5.11.1,<6.0.0) Requires-Dist: questionary (>=2.0.1,<3.0.0)
+Requires-Dist: snakecase (>=1.0.1,<2.0.0) Requires-Dist: strawberry-graphql
+(>=0.225.0,<0.226.0) Requires-Dist: ujson (>=5.9.0,<6.0.0) Requires-Dist:
+uvicorn[standard] (>=0.29.0,<0.30.0) Description-Content-Type: text/markdown
                                 [Nestipy Logo]
                           _[_V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_L_i_c_e_n_s_e_]
 ## Description
-Nestipy is a Python framework built on top of Litestar that follows the modular
+Nestipy is a Python framework built on top of FastAPI that follows the modular
 architecture of NestJS
-Under the hood, Nestipy makes use of _L_i_t_e_s_t_a_r, but also provides compatibility
-with a wide range of other libraries, like _F_a_s_t_A_P_I, allowing for easy use of
+Under the hood, Nestipy makes use of _F_a_s_t_A_P_I, but also provides compatibility
+with a wide range of other libraries, like _B_l_a_c_k_s_h_e_e_p, allowing for easy use of
 the myriad of third-party plugins which are available.
-## Getting started ```cmd pip install nestipy nestipy new my_app cd my_app
+## Getting started ```cmd pip install nestipy-cli nestipy new my_app cd my_app
 python main.py ``` ``` âââ src â âââ __init__.py âââ
 app_module.py âââ app_controller.py âââ app_service.py âââ
-main.py âââ requirements.txt âââ README.md ``` ## [Documentation]
-(https://tsiresymila1.github.io/nestipy) ## Issues Please make sure to read the
-[Issue Reporting Checklist](https://github.com/tsiresymila1/nestipy) before
-opening an issue. Issues not conforming to the guidelines may be closed
-immediately. ## Support Nestipy is an MIT-licensed open source project. It can
-grow thanks to the sponsors and support from the amazing backers. If you'd like
-to join them, please [read more here]. ## Stay in touch - Author - [Tsiresy
-Mila](https://tsiresymila.vercel.app) ## License Nestipy is [MIT licensed]
-(LICENSE).
+main.py âââ requirements.txt âââ README.md ``` ## Documentation
+View full documentation from [here](https://nestipy.github.io/nestipy). ##
+Support Nestipy is an MIT-licensed open source project. It can grow thanks to
+the sponsors and support from the amazing backers. If you'd like to join them,
+please [read more here]. ## Stay in touch - Author - [Tsiresy Mila](https://
+tsiresymila.vercel.app) ## License Nestipy is [MIT licensed](LICENSE).
```

