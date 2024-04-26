# Comparing `tmp/onnxscript-0.1.0.dev20240424.tar.gz` & `tmp/onnxscript-0.1.0.dev20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240424.tar", last modified: Wed Apr 24 00:01:52 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240425.tar", last modified: Thu Apr 25 00:01:47 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240424.tar` & `onnxscript-0.1.0.dev20240425.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.510317 onnxscript-0.1.0.dev20240424/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.514317 onnxscript-0.1.0.dev20240424/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.514317 onnxscript-0.1.0.dev20240424/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.514317 onnxscript-0.1.0.dev20240424/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.514317 onnxscript-0.1.0.dev20240424/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.506317 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.514317 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.538317 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.506317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.506317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.538317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.538317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.542317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.546317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.550317 onnxscript-0.1.0.dev20240424/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.550317 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.558317 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.562317 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4316 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.566317 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1253 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6926 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2170 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36263 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.566317 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5746 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1922 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24160 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41987 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-24 00:01:52.000000 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-24 00:01:52.000000 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 00:01:52.000000 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-24 00:01:52.000000 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-24 00:01:52.000000 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.058006 onnxscript-0.1.0.dev20240425/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-25 00:01:47.054006 onnxscript-0.1.0.dev20240425/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.018006 onnxscript-0.1.0.dev20240425/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.022006 onnxscript-0.1.0.dev20240425/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.022006 onnxscript-0.1.0.dev20240425/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.022006 onnxscript-0.1.0.dev20240425/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.022006 onnxscript-0.1.0.dev20240425/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.014006 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.026006 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.034006 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.014006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.014006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.034006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.034006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.038006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.038006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.042006 onnxscript-0.1.0.dev20240425/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.042006 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.046006 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.050006 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4316 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.050006 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1253 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6926 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2170 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36263 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.050006 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5746 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1922 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.054006 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24160 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41987 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.054006 onnxscript-0.1.0.dev20240425/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.054006 onnxscript-0.1.0.dev20240425/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.054006 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-25 00:01:46.000000 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-25 00:01:47.000000 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-25 00:01:46.000000 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-25 00:01:46.000000 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-25 00:01:46.000000 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-25 00:01:47.058006 onnxscript-0.1.0.dev20240425/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240424/LICENSE` & `onnxscript-0.1.0.dev20240425/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/PKG-INFO` & `onnxscript-0.1.0.dev20240425/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240424
+Version: 0.1.0.dev20240425
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240424/README.md` & `onnxscript-0.1.0.dev20240425/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240425/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240425/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240425/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240425/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240425/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240425/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240425/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240425/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240425/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240425/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240425/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240425/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240425/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240425/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/_convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/_core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240425/onnxscript/ir/serde.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240425/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/main.py` & `onnxscript-0.1.0.dev20240425/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240425/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240425/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240425/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240425/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240425/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240425/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240425/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240425/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript/values.py` & `onnxscript-0.1.0.dev20240425/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240425/onnxscript.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240424
+Version: 0.1.0.dev20240425
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240424/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240425/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/pyproject.toml` & `onnxscript-0.1.0.dev20240425/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240424/setup.py` & `onnxscript-0.1.0.dev20240425/setup.py`

 * *Files identical despite different names*
