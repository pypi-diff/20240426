# Comparing `tmp/nucliadb_node_binding-3.0.3.post1190.tar.gz` & `tmp/nucliadb_node_binding-3.0.3.post1201.tar.gz`

## Comparing `nucliadb_node_binding-3.0.3.post1190.tar` & `nucliadb_node_binding-3.0.3.post1201.tar`

### file list

```diff
@@ -1,282 +1,283 @@
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2155 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127    27030 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127     9795 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1256 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    77311 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    10240 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    43352 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    19010 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    33352 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127     5528 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17053 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     8279 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9435 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3296 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     3957 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    17752 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      890 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     2424 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1487 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    10810 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13788 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2289 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     2361 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12553 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     3379 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2323 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      276 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1405 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5045 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8050 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1345 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/cache/mod.rs
--rw-r--r--   0     1001      127     3043 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
--rw-r--r--   0     1001      127    11037 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1771 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     2656 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18821 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    13730 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2581 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1465 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1488 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2757 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13672 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1935 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2417 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127     1070 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14103 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11755 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127    11615 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/settings.rs
--rw-r--r--   0     1001      127     1111 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    11409 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1122 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    26036 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    19677 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127     9609 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/shards/versions.rs
--rw-r--r--   0     1001      127    10170 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6396 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12731 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8173 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     6003 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     6862 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0     1001      127     5438 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     2681 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     4869 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2990 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15367 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2069 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8250 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2603 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     3559 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22731 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10377 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3391 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2046 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     9567 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3460 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127    12340 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    24470 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    14639 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1642 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    14175 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2777 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127    10613 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2304 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    20587 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    23710 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     6916 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127    10472 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     2165 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127     1278 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    17189 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    15869 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     1668 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/utils.rs
--rw-r--r--   0     1001      127     2884 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1024 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
--rw-r--r--   0     1001      127    42880 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/reader.rs
--rw-r--r--   0     1001      127     4407 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/schema.rs
--rw-r--r--   0     1001      127    21349 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
--rw-r--r--   0     1001      127    11723 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
--rw-r--r--   0     1001      127     2846 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
--rw-r--r--   0     1001      127     4090 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
--rw-r--r--   0     1001      127    17599 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    42935 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11391 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    18507 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1190/Cargo.toml
--rw-r--r--   0     1001      127     1553 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/Makefile
--rw-r--r--   0     1001      127       52 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/README.md
--rwxr-xr-x   0     1001      127      978 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/cov.sh
--rw-r--r--   0     1001      127     1309 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/pyproject.toml
--rw-r--r--   0     1001      127     2195 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1212 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/src/lib.rs
--rw-r--r--   0     1001      127     9405 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/src/reader.rs
--rw-r--r--   0     1001      127     2154 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/src/update.rs
--rw-r--r--   0     1001      127     9162 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-04-22 14:44:20.000000 nucliadb_node_binding-3.0.3.post1190/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1190/PKG-INFO
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17052 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     8007 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9435 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3297 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    42934 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11391 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    17965 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127    12340 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    24470 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11214 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    14639 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1642 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    14175 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2777 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127    10613 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2304 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    20587 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    23710 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     6916 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     1959 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127     4433 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0     1001      127    10472 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     2165 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127     1278 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    17188 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    15294 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     1668 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/utils.rs
+-rw-r--r--   0     1001      127     2884 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     2681 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     4869 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2990 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15367 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2069 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8250 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2603 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     3559 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     3957 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    17752 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      890 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     2424 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1487 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    10810 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13788 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2289 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     2361 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12553 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     3379 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2323 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      276 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1405 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     5045 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8050 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1345 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/cache/mod.rs
+-rw-r--r--   0     1001      127     3035 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    11029 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1771 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     1111 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/errors.rs
+-rw-r--r--   0     1001      127     2656 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18813 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    13722 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2581 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1504 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2757 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13672 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1070 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14103 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11755 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    11615 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1111 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    11409 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1127 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    27703 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    23537 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127     1720 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/shards/versioning.rs
+-rw-r--r--   0     1001      127    10170 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12731 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8173 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     6003 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     6862 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0     1001      127     5438 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1024 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
+-rw-r--r--   0     1001      127    42879 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/reader.rs
+-rw-r--r--   0     1001      127     4407 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/schema.rs
+-rw-r--r--   0     1001      127    21349 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
+-rw-r--r--   0     1001      127    11723 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
+-rw-r--r--   0     1001      127     2846 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
+-rw-r--r--   0     1001      127     4090 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
+-rw-r--r--   0     1001      127    17057 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2155 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127    27030 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127     9795 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1256 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    77311 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    10240 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    43352 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    19010 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    33352 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127     5528 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22730 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10109 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3391 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2043 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     9567 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3464 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1201/Cargo.toml
+-rw-r--r--   0     1001      127     1553 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/Makefile
+-rw-r--r--   0     1001      127       52 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/README.md
+-rwxr-xr-x   0     1001      127      978 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/cov.sh
+-rw-r--r--   0     1001      127     1309 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/pyproject.toml
+-rw-r--r--   0     1001      127     2195 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1212 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/src/lib.rs
+-rw-r--r--   0     1001      127     9405 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/src/reader.rs
+-rw-r--r--   0     1001      127     2154 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/src/update.rs
+-rw-r--r--   0     1001      127     9162 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-04-26 08:15:47.000000 nucliadb_node_binding-3.0.3.post1201/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1201/PKG-INFO
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         let node_values: Vec<_> = node_values.into_iter().collect();
         Ok(node_values)
     }
 }
 
 impl RelationsReaderService {
     #[tracing::instrument(skip_all)]
-    pub fn start(config: &RelationConfig) -> NodeResult<Self> {
+    pub fn open(config: &RelationConfig) -> NodeResult<Self> {
         if !config.path.exists() {
             return Err(node_error!("Invalid path {:?}", config.path));
         }
         let field_schema = Schema::new();
         let index = Index::open_in_dir(&config.path)?;
 
         let reader = index.reader_builder().reload_policy(ReloadPolicy::OnCommit).try_into()?;
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -106,39 +106,29 @@
         let safe_state = tantivy_replica::compute_safe_replica_state(params, &self.index)?;
         Ok(IndexFiles::Tantivy(safe_state))
     }
 }
 
 impl RelationsWriterService {
     #[tracing::instrument(skip_all)]
-    pub fn start(config: &RelationConfig) -> NodeResult<Self> {
-        let path = std::path::Path::new(&config.path);
-        if !path.exists() {
-            Self::new(config)
-        } else {
-            Self::open(config)
-        }
-    }
-
-    #[tracing::instrument(skip_all)]
     pub fn open(config: &RelationConfig) -> NodeResult<Self> {
         let field_schema = Schema::new();
         let index = Index::open_in_dir(&config.path)?;
         let writer = index.writer_with_num_threads(1, TANTIVY_INDEX_ARENA_MEMORY).unwrap();
 
         Ok(RelationsWriterService {
             index,
             writer,
             schema: field_schema,
             config: config.clone(),
         })
     }
 
     #[tracing::instrument(skip_all)]
-    fn new(config: &RelationConfig) -> NodeResult<Self> {
+    pub fn create(config: &RelationConfig) -> NodeResult<Self> {
         Self::try_create_index_dir(&config.path)?;
 
         let settings = IndexSettings {
             ..Default::default()
         };
         let field_schema = Schema::new();
         let mut index_builder = Index::builder().schema(field_schema.schema.clone());
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 fn create_reader() -> NodeResult<RelationsReaderService> {
     let dir = TempDir::new().unwrap();
     let config = RelationConfig {
         path: dir.path().join("relations"),
         channel: Channel::EXPERIMENTAL,
     };
 
-    let mut writer = RelationsWriterService::start(&config)?;
-    let reader = RelationsReaderService::start(&config)?;
+    let mut writer = RelationsWriterService::create(&config)?;
+    let reader = RelationsReaderService::open(&config)?;
 
     writer.set_resource(&Resource {
         resource: Some(ResourceId {
             uuid: "uuid".to_string(),
             shard_id: "shard_id".to_string(),
         }),
         relations: vec![
@@ -125,16 +125,16 @@
 fn test_start_new_reader_after_a_writer() -> NodeResult<()> {
     let dir = TempDir::new()?;
     let config = RelationConfig {
         path: dir.path().join("relations"),
         channel: Channel::EXPERIMENTAL,
     };
 
-    let _writer = RelationsWriterService::start(&config)?;
-    let reader: Result<RelationsReaderService, nucliadb_core::Error> = RelationsReaderService::start(&config);
+    let _writer = RelationsWriterService::create(&config)?;
+    let reader: Result<RelationsReaderService, nucliadb_core::Error> = RelationsReaderService::open(&config);
     assert!(reader.is_ok());
 
     Ok(())
 }
 
 #[test]
 fn test_stored_ids() -> NodeResult<()> {
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 fn test_index_docs() -> NodeResult<()> {
     let dir = TempDir::new().unwrap();
     let config = RelationConfig {
         path: dir.path().join("relations"),
         channel: Channel::EXPERIMENTAL,
     };
 
-    let mut writer = RelationsWriterService::start(&config).unwrap();
+    let mut writer = RelationsWriterService::create(&config).unwrap();
 
     writer.set_resource(&Resource {
         resource: Some(ResourceId {
             uuid: "uuid".to_string(),
             shard_id: "shard_id".to_string(),
         }),
         relations: vec![
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/cache/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/cache/reader_cache.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/cache/reader_cache.rs`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 use std::path::PathBuf;
 use std::sync::{Arc, Mutex, MutexGuard};
 
 use nucliadb_core::{node_error, NodeResult};
 
 use super::resource_cache::{CacheResult, ResourceCache};
 use crate::disk_structure;
+use crate::errors::ShardNotFoundError;
 use crate::settings::Settings;
-use crate::shards::errors::ShardNotFoundError;
 use crate::shards::metadata::ShardMetadata;
 use crate::shards::reader::ShardReader;
 use crate::shards::ShardId;
 
 pub struct ShardReaderCache {
     cache: Mutex<ResourceCache<ShardId, ShardReader>>,
     shards_path: PathBuf,
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/cache/resource_cache.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/cache/writer_cache.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/cache/writer_cache.rs`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 use std::time::Duration;
 
 use nucliadb_core::tracing::debug;
 use nucliadb_core::{node_error, NodeResult};
 
 use super::resource_cache::{CacheResult, ResourceCache, ResourceLoadGuard};
 use crate::disk_structure;
+use crate::errors::ShardNotFoundError;
 use crate::settings::Settings;
-use crate::shards::errors::ShardNotFoundError;
 use crate::shards::metadata::{ShardMetadata, ShardsMetadataManager};
 use crate::shards::writer::ShardWriter;
 use crate::shards::ShardId;
 
 /// This cache allows the user to block shards, ensuring that they will not be loaded from disk.
 /// Being able to do so is crucial, otherwise the only source of truth will be disk and that would
 /// not be thread-safe.
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 use crate::cache::ShardReaderCache;
+use crate::errors::ShardNotFoundError;
 use crate::grpc::update::{update_loop, UpdateParameters};
 use crate::settings::Settings;
-use crate::shards::errors::ShardNotFoundError;
 use crate::shards::reader::{ShardFileChunkIterator, ShardReader};
 use crate::telemetry::run_with_telemetry;
 use nucliadb_core::paragraphs::ParagraphIterator;
 use nucliadb_core::protos::node_reader_server::NodeReader;
 use nucliadb_core::protos::*;
 use nucliadb_core::texts::DocumentIterator;
 use nucliadb_core::tracing::{info_span, Span};
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 use crate::analytics::payload::AnalyticsEvent;
 use crate::analytics::sync::send_analytics_event;
 use crate::cache::ShardWriterCache;
+use crate::errors::ShardNotFoundError;
 use crate::grpc::collect_garbage::{garbage_collection_loop, GCParameters};
 use crate::merge::{global_merger, MergePriority, MergeRequest, MergeWaiter};
 use crate::settings::Settings;
-use crate::shards::errors::ShardNotFoundError;
 use crate::shards::metadata::ShardMetadata;
 use crate::shards::writer::ShardWriter;
 use crate::telemetry::run_with_telemetry;
 use crate::utils::{get_primary_node_id, list_shards, read_host_key};
 use nucliadb_core::protos::node_writer_server::NodeWriter;
 use nucliadb_core::protos::{
     garbage_collector_response, merge_response, op_status, EmptyQuery, GarbageCollectorResponse, MergeResponse,
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 //!
 //! As a high level interface, it provides a gRPC server to deploy the index in
 //! a distributed fashion. The API allows building other interfaces, as the
 //! already built PyO3 bindings.
 
 pub mod analytics;
 pub mod cache;
+pub mod errors;
 pub mod grpc;
 pub mod http_server;
 pub mod lifecycle;
 pub mod merge;
 pub mod node_metadata;
 pub mod replication;
 pub mod settings;
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/settings.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/settings.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,17 @@
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
+//
 
-//! This module provides tools for managing shards
-
-pub mod errors;
-pub mod metadata;
-pub mod shard_reader;
-pub mod shard_writer;
-pub mod versions;
-
-// Alias for more readable imports
-pub use {shard_reader as reader, shard_writer as writer};
-
-pub type ShardId = String;
+pub mod fuzzy_query;
+pub mod query_io;
+pub mod reader;
+pub mod schema;
+pub mod search_query;
+pub mod search_response;
+pub mod stop_words;
+pub mod writer;
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+use super::metadata::ShardMetadata;
+use super::versioning::Versions;
 use crate::disk_structure::*;
-use crate::shards::metadata::ShardMetadata;
-use crate::shards::versions::Versions;
 use crate::telemetry::run_with_telemetry;
 use crossbeam_utils::thread as crossbeam_thread;
 use nucliadb_core::paragraphs::*;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos;
 use nucliadb_core::protos::shard_created::{DocumentService, ParagraphService, RelationService, VectorService};
 use nucliadb_core::protos::{
@@ -45,20 +45,55 @@
 use nucliadb_protos::nodereader::{RelationNodeFilter, RelationPrefixSearchResponse};
 use nucliadb_protos::utils::relation_node::NodeType;
 use nucliadb_relations2::reader::HashedRelationNode;
 use std::collections::HashSet;
 use std::fs::{self, File};
 use std::io::{BufReader, Read};
 use std::path::{Path, PathBuf};
-use std::sync::Arc;
+use std::sync::{Arc, RwLock};
 
 const MAX_SUGGEST_COMPOUND_WORDS: usize = 3;
 const MIN_VIABLE_PREFIX_SUGGEST: usize = 1;
 const CHUNK_SIZE: usize = 65535;
 
+fn open_vectors_reader(version: u32, config: &VectorConfig) -> NodeResult<VectorsReaderPointer> {
+    match version {
+        1 => nucliadb_vectors::service::VectorReaderService::open(config)
+            .map(|i| Arc::new(RwLock::new(i)) as VectorsReaderPointer),
+        2 => nucliadb_vectors::service::VectorReaderService::open(config)
+            .map(|i| Arc::new(RwLock::new(i)) as VectorsReaderPointer),
+        v => Err(node_error!("Invalid vectors version {v}")),
+    }
+}
+fn open_paragraphs_reader(version: u32, config: &ParagraphConfig) -> NodeResult<ParagraphsReaderPointer> {
+    match version {
+        2 => nucliadb_paragraphs2::reader::ParagraphReaderService::open(config)
+            .map(|i| Arc::new(RwLock::new(i)) as ParagraphsReaderPointer),
+        3 => nucliadb_paragraphs3::reader::ParagraphReaderService::open(config)
+            .map(|i| Arc::new(RwLock::new(i)) as ParagraphsReaderPointer),
+        v => Err(node_error!("Invalid paragraphs version {v}")),
+    }
+}
+
+fn open_texts_reader(version: u32, config: &TextConfig) -> NodeResult<TextsReaderPointer> {
+    match version {
+        2 => nucliadb_texts2::reader::TextReaderService::open(config)
+            .map(|i| Arc::new(RwLock::new(i)) as TextsReaderPointer),
+        v => Err(node_error!("Invalid text reader version {v}")),
+    }
+}
+
+fn open_relations_reader(version: u32, config: &RelationConfig) -> NodeResult<RelationsReaderPointer> {
+    match version {
+        2 => nucliadb_relations2::reader::RelationsReaderService::open(config)
+            .map(|i| Arc::new(RwLock::new(i)) as RelationsReaderPointer),
+        v => Err(node_error!("Invalid relations version {v}")),
+    }
+}
+
 pub struct ShardFileChunkIterator {
     file_path: PathBuf,
     reader: BufReader<File>,
     chunk_size: usize,
     idx: i32,
 }
 
@@ -246,18 +281,18 @@
             normalize_vectors: metadata.normalize_vectors(),
         };
         let rsc = RelationConfig {
             path: shard_path.join(RELATIONS_DIR),
             channel,
         };
         let versions = Versions::load(&shard_path.join(VERSION_FILE))?;
-        let text_task = || Some(versions.get_texts_reader(&tsc));
-        let paragraph_task = || Some(versions.get_paragraphs_reader(&psc));
-        let vector_task = || Some(versions.get_vectors_reader(&vsc));
-        let relation_task = || Some(versions.get_relations_reader(&rsc));
+        let text_task = || Some(open_texts_reader(versions.texts, &tsc));
+        let paragraph_task = || Some(open_paragraphs_reader(versions.paragraphs, &psc));
+        let vector_task = || Some(open_vectors_reader(versions.vectors, &vsc));
+        let relation_task = || Some(open_relations_reader(versions.relations, &rsc));
 
         let info = info_span!(parent: &span, "text open");
         let text_task = || run_with_telemetry(info, text_task);
         let info = info_span!(parent: &span, "paragraph open");
         let paragraph_task = || run_with_telemetry(info, paragraph_task);
         let info = info_span!(parent: &span, "vector open");
         let vector_task = || run_with_telemetry(info, vector_task);
@@ -286,18 +321,18 @@
             metadata,
             root_path: shard_path.to_path_buf(),
             suffixed_root_path,
             text_reader: fields.unwrap(),
             paragraph_reader: paragraphs.unwrap(),
             vector_reader: vectors.unwrap(),
             relation_reader: relations.unwrap(),
-            document_version: versions.version_texts() as i32,
-            paragraph_version: versions.version_paragraphs() as i32,
-            vector_version: versions.version_vectors() as i32,
-            relation_version: versions.version_relations() as i32,
+            document_version: versions.texts as i32,
+            paragraph_version: versions.paragraphs as i32,
+            vector_version: versions.vectors as i32,
+            relation_version: versions.relations as i32,
         })
     }
 
     /// Return a list of queries to suggest from the original
     /// query. The query with more words will come first. `max_group`
     /// defines the limit of words a query can have.
     #[tracing::instrument(skip_all)]
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files 13% similar despite different names*

```diff
@@ -13,38 +13,73 @@
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 use std::collections::HashMap;
-use std::path::PathBuf;
-use std::sync::{Arc, Mutex, MutexGuard};
+use std::path::{Path, PathBuf};
+use std::sync::{Arc, Mutex, MutexGuard, RwLock};
 
 use nucliadb_core::paragraphs::*;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::shard_created::{DocumentService, ParagraphService, RelationService, VectorService};
 use nucliadb_core::protos::{OpStatus, Resource, ResourceId};
 use nucliadb_core::relations::*;
 use nucliadb_core::texts::*;
 use nucliadb_core::tracing::{self, *};
 use nucliadb_core::vectors::*;
 use nucliadb_core::{thread, IndexFiles};
 use nucliadb_procs::measure;
 use nucliadb_vectors::VectorErr;
 
+use super::metadata::ShardMetadata;
+use super::versioning::{self, Versions};
 use crate::disk_structure::*;
-use crate::shards::metadata::ShardMetadata;
-use crate::shards::versions::Versions;
 use crate::telemetry::run_with_telemetry;
 
 pub struct BlockingToken<'a>(MutexGuard<'a, ()>);
 
 const MAX_LABEL_LENGTH: usize = 32768; // Tantivy max is 2^16 - 4
 
+pub fn open_vectors_writer(version: u32, path: &Path, shard_id: String) -> NodeResult<VectorsWriterPointer> {
+    match version {
+        1 => nucliadb_vectors::service::VectorWriterService::open(path, shard_id)
+            .map(|i| Arc::new(RwLock::new(i)) as VectorsWriterPointer),
+        2 => nucliadb_vectors::service::VectorWriterService::open(path, shard_id)
+            .map(|i| Arc::new(RwLock::new(i)) as VectorsWriterPointer),
+        v => Err(node_error!("Invalid vectors version {v}")),
+    }
+}
+pub fn open_paragraphs_writer(version: u32, config: &ParagraphConfig) -> NodeResult<ParagraphsWriterPointer> {
+    match version {
+        2 => nucliadb_paragraphs2::writer::ParagraphWriterService::open(config)
+            .map(|i| Arc::new(RwLock::new(i)) as ParagraphsWriterPointer),
+        3 => nucliadb_paragraphs3::writer::ParagraphWriterService::open(config)
+            .map(|i| Arc::new(RwLock::new(i)) as ParagraphsWriterPointer),
+        v => Err(node_error!("Invalid paragraphs version {v}")),
+    }
+}
+
+pub fn open_texts_writer(version: u32, config: &TextConfig) -> NodeResult<TextsWriterPointer> {
+    match version {
+        2 => nucliadb_texts2::writer::TextWriterService::open(config)
+            .map(|i| Arc::new(RwLock::new(i)) as TextsWriterPointer),
+        v => Err(node_error!("Invalid text writer version {v}")),
+    }
+}
+
+pub fn open_relations_writer(version: u32, config: &RelationConfig) -> NodeResult<RelationsWriterPointer> {
+    match version {
+        2 => nucliadb_relations2::writer::RelationsWriterService::open(config)
+            .map(|i| Arc::new(RwLock::new(i)) as RelationsWriterPointer),
+        v => Err(node_error!("Invalid relations version {v}")),
+    }
+}
+
 fn remove_invalid_labels(resource: &mut Resource) {
     resource.labels.retain(|l| {
         if l.len() > MAX_LABEL_LENGTH {
             warn!("Label length ({}) longer than maximum, it will not be indexed", l.len());
             false
         } else {
             true
@@ -77,71 +112,14 @@
     relation_service_version: i32,
     pub gc_lock: tokio::sync::Mutex<()>, // lock to be able to do GC or not
     write_lock: Mutex<()>,               // be able to lock writes on the shard
 }
 
 impl ShardWriter {
     #[tracing::instrument(skip_all)]
-    fn initialize(
-        metadata: Arc<ShardMetadata>,
-        tsc: TextConfig,
-        psc: ParagraphConfig,
-        vsc: VectorConfig,
-        rsc: RelationConfig,
-    ) -> NodeResult<ShardWriter> {
-        let versions = Versions::load_or_create(&metadata.shard_path().join(VERSION_FILE), metadata.channel())?;
-        let text_task = || Some(versions.get_texts_writer(&tsc));
-        let paragraph_task = || Some(versions.get_paragraphs_writer(&psc));
-        let vector_task = || Some(versions.get_vectors_writer(&vsc));
-        let relation_task = || Some(versions.get_relations_writer(&rsc));
-
-        let span = tracing::Span::current();
-        let info = info_span!(parent: &span, "text start");
-        let text_task = || run_with_telemetry(info, text_task);
-        let info = info_span!(parent: &span, "paragraph start");
-        let paragraph_task = || run_with_telemetry(info, paragraph_task);
-        let info = info_span!(parent: &span, "vector start");
-        let vector_task = || run_with_telemetry(info, vector_task);
-        let info = info_span!(parent: &span, "relation start");
-        let relation_task = || run_with_telemetry(info, relation_task);
-
-        let mut text_result = None;
-        let mut paragraph_result = None;
-        let mut vector_result = None;
-        let mut relation_result = None;
-        thread::scope(|s| {
-            s.spawn(|_| text_result = text_task());
-            s.spawn(|_| paragraph_result = paragraph_task());
-            s.spawn(|_| vector_result = vector_task());
-            s.spawn(|_| relation_result = relation_task());
-        });
-
-        let fields = text_result.transpose()?;
-        let paragraphs = paragraph_result.transpose()?;
-        let vectors = vector_result.transpose()?;
-        let relations = relation_result.transpose()?;
-
-        Ok(ShardWriter {
-            id: metadata.id(),
-            path: metadata.shard_path(),
-            metadata,
-            text_writer: fields.unwrap(),
-            paragraph_writer: paragraphs.unwrap(),
-            vector_writer: vectors.unwrap(),
-            relation_writer: relations.unwrap(),
-            document_service_version: versions.version_texts() as i32,
-            paragraph_service_version: versions.version_paragraphs() as i32,
-            vector_service_version: versions.version_vectors() as i32,
-            relation_service_version: versions.version_relations() as i32,
-            gc_lock: tokio::sync::Mutex::new(()),
-            write_lock: Mutex::new(()),
-        })
-    }
-
-    #[tracing::instrument(skip_all)]
     pub fn document_version(&self) -> DocumentService {
         match self.document_service_version {
             0 => DocumentService::DocumentV0,
             1 => DocumentService::DocumentV1,
             2 => DocumentService::DocumentV2,
             i => panic!("Unknown document version {i}"),
         }
@@ -197,17 +175,70 @@
         let rsc = RelationConfig {
             path: path.join(RELATIONS_DIR),
             channel,
         };
 
         std::fs::create_dir(path)?;
 
-        let sw = ShardWriter::initialize(Arc::clone(&metadata), tsc, psc, vsc, rsc)?;
+        let versions = Versions {
+            paragraphs: versioning::PARAGRAPHS_VERSION,
+            vectors: versioning::VECTORS_VERSION,
+            texts: versioning::TEXTS_VERSION,
+            relations: versioning::RELATIONS_VERSION,
+        };
+        let versions_path = metadata.shard_path().join(VERSION_FILE);
+        Versions::create(&versions_path, versions)?;
+
+        let text_task = || Some(nucliadb_texts2::writer::TextWriterService::create(&tsc));
+        let paragraph_task = || Some(nucliadb_paragraphs3::writer::ParagraphWriterService::create(&psc));
+        let vector_task = || Some(nucliadb_vectors::service::VectorWriterService::create(&vsc));
+        let relation_task = || Some(nucliadb_relations2::writer::RelationsWriterService::create(&rsc));
+
+        let span = tracing::Span::current();
+        let info = info_span!(parent: &span, "text start");
+        let text_task = || run_with_telemetry(info, text_task);
+        let info = info_span!(parent: &span, "paragraph start");
+        let paragraph_task = || run_with_telemetry(info, paragraph_task);
+        let info = info_span!(parent: &span, "vector start");
+        let vector_task = || run_with_telemetry(info, vector_task);
+        let info = info_span!(parent: &span, "relation start");
+        let relation_task = || run_with_telemetry(info, relation_task);
+
+        let mut text_result = None;
+        let mut paragraph_result = None;
+        let mut vector_result = None;
+        let mut relation_result = None;
+        thread::scope(|s| {
+            s.spawn(|_| text_result = text_task());
+            s.spawn(|_| paragraph_result = paragraph_task());
+            s.spawn(|_| vector_result = vector_task());
+            s.spawn(|_| relation_result = relation_task());
+        });
+
+        let fields = text_result.transpose()?;
+        let paragraphs = paragraph_result.transpose()?;
+        let vectors = vector_result.transpose()?;
+        let relations = relation_result.transpose()?;
+
         metadata.serialize_metadata()?;
-        Ok(sw)
+        Ok(ShardWriter {
+            id: metadata.id(),
+            path: metadata.shard_path(),
+            metadata,
+            text_writer: Arc::new(RwLock::new(fields.unwrap())),
+            paragraph_writer: Arc::new(RwLock::new(paragraphs.unwrap())),
+            vector_writer: Arc::new(RwLock::new(vectors.unwrap())),
+            relation_writer: Arc::new(RwLock::new(relations.unwrap())),
+            document_service_version: versions.texts as i32,
+            paragraph_service_version: versions.paragraphs as i32,
+            vector_service_version: versions.vectors as i32,
+            relation_service_version: versions.relations as i32,
+            gc_lock: tokio::sync::Mutex::new(()),
+            write_lock: Mutex::new(()),
+        })
     }
 
     #[measure(actor = "shard", metric = "open")]
     pub fn open(metadata: Arc<ShardMetadata>) -> NodeResult<ShardWriter> {
         let path = metadata.shard_path();
         let tsc = TextConfig {
             path: path.join(TEXTS_DIR),
@@ -215,27 +246,68 @@
 
         let psc = ParagraphConfig {
             path: path.join(PARAGRAPHS_DIR),
         };
 
         let channel = metadata.channel();
 
-        let vsc = VectorConfig {
-            similarity: None,
-            path: path.join(VECTORS_DIR),
-            channel,
-            shard_id: metadata.id(),
-            normalize_vectors: metadata.normalize_vectors(),
-        };
         let rsc = RelationConfig {
             path: path.join(RELATIONS_DIR),
             channel,
         };
 
-        ShardWriter::initialize(metadata, tsc, psc, vsc, rsc)
+        let versions_path = metadata.shard_path().join(VERSION_FILE);
+        let versions = Versions::load(&versions_path)?;
+
+        let text_task = || Some(open_texts_writer(versions.texts, &tsc));
+        let paragraph_task = || Some(open_paragraphs_writer(versions.paragraphs, &psc));
+        let vector_task = || Some(open_vectors_writer(versions.vectors, &path.join(VECTORS_DIR), metadata.id()));
+        let relation_task = || Some(open_relations_writer(versions.relations, &rsc));
+
+        let span = tracing::Span::current();
+        let info = info_span!(parent: &span, "text start");
+        let text_task = || run_with_telemetry(info, text_task);
+        let info = info_span!(parent: &span, "paragraph start");
+        let paragraph_task = || run_with_telemetry(info, paragraph_task);
+        let info = info_span!(parent: &span, "vector start");
+        let vector_task = || run_with_telemetry(info, vector_task);
+        let info = info_span!(parent: &span, "relation start");
+        let relation_task = || run_with_telemetry(info, relation_task);
+
+        let mut text_result = None;
+        let mut paragraph_result = None;
+        let mut vector_result = None;
+        let mut relation_result = None;
+        thread::scope(|s| {
+            s.spawn(|_| text_result = text_task());
+            s.spawn(|_| paragraph_result = paragraph_task());
+            s.spawn(|_| vector_result = vector_task());
+            s.spawn(|_| relation_result = relation_task());
+        });
+
+        let fields = text_result.transpose()?;
+        let paragraphs = paragraph_result.transpose()?;
+        let vectors = vector_result.transpose()?;
+        let relations = relation_result.transpose()?;
+
+        Ok(ShardWriter {
+            id: metadata.id(),
+            path: metadata.shard_path(),
+            metadata,
+            text_writer: fields.unwrap(),
+            paragraph_writer: paragraphs.unwrap(),
+            vector_writer: vectors.unwrap(),
+            relation_writer: relations.unwrap(),
+            document_service_version: versions.texts as i32,
+            paragraph_service_version: versions.paragraphs as i32,
+            vector_service_version: versions.vectors as i32,
+            relation_service_version: versions.relations as i32,
+            gc_lock: tokio::sync::Mutex::new(()),
+            write_lock: Mutex::new(()),
+        })
     }
 
     #[measure(actor = "shard", metric = "set_resource")]
     #[tracing::instrument(skip_all)]
     pub fn set_resource(&self, mut resource: Resource) -> NodeResult<()> {
         let span = tracing::Span::current();
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
                 OrderField::Modified => segment_reader.fast_fields().date(modified).unwrap(),
             };
             move |doc: DocId| sorter(reader.get(doc).to_u64())
         })
     }
 
     #[tracing::instrument(skip_all)]
-    pub fn start(config: &TextConfig) -> NodeResult<Self> {
+    pub fn open(config: &TextConfig) -> NodeResult<Self> {
         if !config.path.exists() {
             return Err(node_error!("Invalid path {:?}", config.path));
         }
         let field_schema = TextSchema::new();
         let index = Index::open_in_dir(&config.path)?;
 
         let reader = index.reader_builder().reload_policy(ReloadPolicy::OnCommit).try_into()?;
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -152,39 +152,29 @@
         let safe_state = tantivy_replica::compute_safe_replica_state(params, &self.index)?;
         Ok(IndexFiles::Tantivy(safe_state))
     }
 }
 
 impl TextWriterService {
     #[tracing::instrument(skip_all)]
-    pub fn start(config: &TextConfig) -> NodeResult<Self> {
-        let path = std::path::Path::new(&config.path);
-        if !path.exists() {
-            Self::new(config)
-        } else {
-            Self::open(config)
-        }
-    }
-
-    #[tracing::instrument(skip_all)]
     pub fn open(config: &TextConfig) -> NodeResult<Self> {
         let field_schema = TextSchema::new();
         let index = Index::open_in_dir(&config.path)?;
         let writer = index.writer_with_num_threads(1, TANTIVY_INDEX_ARENA_MEMORY).unwrap();
 
         Ok(TextWriterService {
             index,
             writer,
             schema: field_schema,
             config: config.clone(),
         })
     }
 
     #[tracing::instrument(skip_all)]
-    fn new(config: &TextConfig) -> NodeResult<Self> {
+    pub fn create(config: &TextConfig) -> NodeResult<Self> {
         Self::try_create_index_dir(&config.path)?;
 
         let settings = IndexSettings {
             sort_by_field: Some(IndexSortByField {
                 field: "created".to_string(),
                 order: Order::Desc,
             }),
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 
 pub fn test_reader() -> TextReaderService {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let mut writer = TextWriterService::start(&config).unwrap();
+    let mut writer = TextWriterService::create(&config).unwrap();
     let resource = create_resource("shard".to_string());
     writer.set_resource(&resource).unwrap();
 
-    TextReaderService::start(&config).unwrap()
+    TextReaderService::open(&config).unwrap()
 }
 
 pub fn create_resource(shard_id: String) -> Resource {
     let resource_id = ResourceId {
         shard_id: shard_id.to_string(),
         uuid: "f56c58ac-b4f9-4d61-a077-ffccaadd0001".to_string(),
     };
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files 8% similar despite different names*

```diff
@@ -26,38 +26,38 @@
 #[test]
 fn test_start_new_reader_after_a_writer() {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let _writer = TextWriterService::start(&config).unwrap();
-    let reader = TextReaderService::start(&config);
+    let _writer = TextWriterService::create(&config).unwrap();
+    let reader = TextReaderService::open(&config);
     assert!(reader.is_ok());
 }
 
 #[test]
 fn test_open_multiple_readers() {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let _writer = TextWriterService::start(&config).unwrap();
-    let reader1 = TextReaderService::start(&config);
-    let reader2 = TextReaderService::start(&config);
-    let reader3 = TextReaderService::start(&config);
+    let _writer = TextWriterService::create(&config).unwrap();
+    let reader1 = TextReaderService::open(&config);
+    let reader2 = TextReaderService::open(&config);
+    let reader3 = TextReaderService::open(&config);
     assert!(reader1.is_ok());
     assert!(reader2.is_ok());
     assert!(reader3.is_ok());
 }
 
 #[test]
 fn test_start_new_reader_before_a_writer() {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let reader = TextReaderService::start(&config);
+    let reader = TextReaderService::open(&config);
     assert!(reader.is_err());
 }
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files 13% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 #[test]
 fn test_start_new_writer() {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let writer = TextWriterService::start(&config);
+    let writer = TextWriterService::create(&config);
     assert!(writer.is_ok());
 }
 
 #[test]
 fn test_open_writer_for_existent_index() {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let writer = TextWriterService::start(&config).unwrap();
+    let writer = TextWriterService::create(&config).unwrap();
     std::mem::drop(writer);
 
     let another_writer = TextWriterService::open(&config);
 
     assert!(another_writer.is_ok());
 }
 
@@ -59,46 +59,46 @@
 #[should_panic]
 fn test_two_simultaneous_writers() {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let _writer = TextWriterService::start(&config).unwrap();
+    let _writer = TextWriterService::create(&config).unwrap();
     let _another_writer = TextWriterService::open(&config);
 }
 
 #[test]
 fn test_set_resource() {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let mut writer = TextWriterService::start(&config).unwrap();
+    let mut writer = TextWriterService::create(&config).unwrap();
     let resource = common::create_resource("shard1".to_string());
     let result = writer.set_resource(&resource);
 
     assert!(result.is_ok());
 }
 
 // TODO: move to another test file and refactor
 #[test]
 fn test_old_writer_test() -> NodeResult<()> {
     let dir = TempDir::new().unwrap();
     let fsc = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let mut field_writer_service = TextWriterService::start(&fsc).unwrap();
+    let mut field_writer_service = TextWriterService::create(&fsc).unwrap();
     let resource1 = common::create_resource("shard1".to_string());
     let _ = field_writer_service.set_resource(&resource1);
     let _ = field_writer_service.set_resource(&resource1);
 
-    let field_reader_service = TextReaderService::start(&fsc).unwrap();
+    let field_reader_service = TextReaderService::open(&fsc).unwrap();
 
     let reader = field_reader_service;
     let searcher = reader.reader.searcher();
 
     let query =
         TermQuery::new(Term::from_field_text(field_writer_service.schema.text, "document"), IndexRecordOption::Basic);
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             score: neighbour.score(),
         })
     }
 }
 
 impl VectorReaderService {
     #[tracing::instrument(skip_all)]
-    pub fn start(config: &VectorConfig) -> NodeResult<Self> {
+    pub fn open(config: &VectorConfig) -> NodeResult<Self> {
         if !config.path.exists() {
             return Err(node_error!("Invalid path {:?}", config.path));
         }
         Ok(VectorReaderService {
             index: Reader::open(&config.path)?,
         })
     }
@@ -249,18 +249,18 @@
             relations: vec![],
             vectors: HashMap::default(),
             vectors_to_delete: HashMap::default(),
             shard_id: "DOC".to_string(),
             ..Default::default()
         };
         // insert - delete - insert sequence
-        let mut writer = VectorWriterService::start(&vsc).unwrap();
+        let mut writer = VectorWriterService::create(&vsc).unwrap();
         writer.set_resource(&resource).unwrap();
 
-        let reader = VectorReaderService::start(&vsc).unwrap();
+        let reader = VectorReaderService::open(&vsc).unwrap();
         let mut request = VectorSearchRequest {
             id: "".to_string(),
             vector_set: "".to_string(),
             vector: vec![4.0, 6.0, 7.0],
             field_labels: vec!["1".to_string()],
             key_filters: vec!["DOC/KEY/1".to_string()],
             page_number: 0,
@@ -332,18 +332,18 @@
             relations: vec![],
             vectors: HashMap::default(),
             vectors_to_delete: HashMap::default(),
             shard_id: "DOC".to_string(),
             ..Default::default()
         };
         // insert - delete - insert sequence
-        let mut writer = VectorWriterService::start(&vsc).unwrap();
+        let mut writer = VectorWriterService::create(&vsc).unwrap();
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
-        let reader = VectorReaderService::start(&vsc).unwrap();
+        let reader = VectorReaderService::open(&vsc).unwrap();
         let request = VectorSearchRequest {
             id: "".to_string(),
             vector_set: "".to_string(),
             vector: vec![4.0, 6.0, 7.0],
             field_labels: vec!["1".to_string()],
             page_number: 0,
             result_per_page: 20,
@@ -449,18 +449,18 @@
             sentences_to_delete: vec![],
             relations: vec![],
             vectors: HashMap::default(),
             vectors_to_delete: HashMap::default(),
             shard_id: "DOC".to_string(),
             ..Default::default()
         };
-        let mut writer = VectorWriterService::start(&vsc).unwrap();
+        let mut writer = VectorWriterService::create(&vsc).unwrap();
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
-        let reader = VectorReaderService::start(&vsc).unwrap();
+        let reader = VectorReaderService::open(&vsc).unwrap();
         let request = VectorSearchRequest {
             id: "".to_string(),
             vector_set: "".to_string(),
             vector: vec![4.0, 6.0, 7.0],
             field_labels: vec!["1".to_string()],
             page_number: 0,
             result_per_page: 20,
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -32,20 +32,21 @@
 use nucliadb_core::tracing::{self, *};
 use nucliadb_core::vectors::MergeMetrics;
 use nucliadb_core::vectors::*;
 use nucliadb_core::{IndexFiles, RawReplicaState};
 use nucliadb_procs::measure;
 use std::collections::HashMap;
 use std::fmt::Debug;
+use std::path::{Path, PathBuf};
 use std::time::Instant;
 use std::time::SystemTime;
 
 pub struct VectorWriterService {
     index: Writer,
-    config: VectorConfig,
+    path: PathBuf,
 }
 
 impl Debug for VectorWriterService {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("VectorWriterService").finish()
     }
 }
@@ -184,20 +185,20 @@
 
         let took = time.elapsed().as_secs_f64();
         debug!("Garbage collection {took} ms");
         Ok(())
     }
 
     fn get_segment_ids(&self) -> NodeResult<Vec<String>> {
-        Ok(replication::get_segment_ids(&self.config.path)?)
+        Ok(replication::get_segment_ids(&self.path)?)
     }
 
     fn get_index_files(&self, ignored_segment_ids: &[String]) -> NodeResult<IndexFiles> {
         // Should be called along with a lock at a higher level to be safe
-        let replica_state = replication::get_index_files(&self.config.path, "vectors", ignored_segment_ids)?;
+        let replica_state = replication::get_index_files(&self.path, "vectors", ignored_segment_ids)?;
 
         if replica_state.files.is_empty() {
             // exit with no changes
             return Ok(IndexFiles::Other(RawReplicaState::default()));
         }
 
         Ok(IndexFiles::Other(replica_state))
@@ -212,60 +213,42 @@
             report.push_str(&partial);
         }
         report.pop();
         report
     }
 
     #[tracing::instrument(skip_all)]
-    pub fn start(config: &VectorConfig) -> NodeResult<Self> {
-        let path = std::path::Path::new(&config.path);
-        if !path.exists() {
-            match VectorWriterService::new(config) {
-                Err(e) if path.exists() => {
-                    std::fs::remove_dir(path)?;
-                    Err(e)
-                }
-                Err(e) => Err(e),
-                Ok(v) => Ok(v),
-            }
-        } else {
-            VectorWriterService::open(config)
-        }
-    }
-
-    #[tracing::instrument(skip_all)]
-    pub fn new(config: &VectorConfig) -> NodeResult<Self> {
+    pub fn create(config: &VectorConfig) -> NodeResult<Self> {
         let path = std::path::Path::new(&config.path);
         if path.exists() {
             Err(node_error!("Shard does exist".to_string()))
         } else {
             let Some(similarity) = config.similarity.map(|i| i.into()) else {
                 return Err(node_error!("A similarity must be specified, {:?}", config.similarity));
             };
             let index_metadata = IndexMetadata {
                 similarity,
                 channel: config.channel,
                 normalize_vectors: config.normalize_vectors,
             };
             Ok(VectorWriterService {
                 index: Writer::new(path, index_metadata, config.shard_id.clone())?,
-                config: config.clone(),
+                path: path.to_path_buf(),
             })
         }
     }
 
     #[tracing::instrument(skip_all)]
-    pub fn open(config: &VectorConfig) -> NodeResult<Self> {
-        let path = std::path::Path::new(&config.path);
+    pub fn open(path: &Path, shard_id: String) -> NodeResult<Self> {
         if !path.exists() {
             Err(node_error!("Shard does not exist".to_string()))
         } else {
             Ok(VectorWriterService {
-                index: Writer::open(path, config.shard_id.clone())?,
-                config: config.clone(),
+                index: Writer::open(path, shard_id)?,
+                path: path.to_path_buf(),
             })
         }
     }
 }
 
 #[cfg(test)]
 mod tests {
@@ -333,15 +316,15 @@
             relations: vec![],
             vectors: HashMap::default(),
             vectors_to_delete: HashMap::default(),
             shard_id: "DOC".to_string(),
             ..Default::default()
         };
         // insert - delete - insert sequence
-        let mut writer = VectorWriterService::start(&vsc).unwrap();
+        let mut writer = VectorWriterService::create(&vsc).unwrap();
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
         let res = writer.delete_resource(&resource_id);
         assert!(res.is_ok());
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
     }
@@ -396,15 +379,15 @@
             relations: vec![],
             vectors: HashMap::default(),
             vectors_to_delete: HashMap::default(),
             shard_id: "DOC".to_string(),
             ..Default::default()
         };
         // insert - delete - insert sequence
-        let mut writer = VectorWriterService::start(&vsc).unwrap();
+        let mut writer = VectorWriterService::create(&vsc).unwrap();
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
         let res = writer.delete_resource(&resource_id);
         assert!(res.is_ok());
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/reader.rs`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 
         Ok(keys)
     }
 }
 
 impl ParagraphReaderService {
     #[tracing::instrument(skip_all)]
-    pub fn start(config: &ParagraphConfig) -> NodeResult<Self> {
+    pub fn open(config: &ParagraphConfig) -> NodeResult<Self> {
         if !config.path.exists() {
             return Err(node_error!("Invalid path {:?}", config.path));
         }
         let paragraph_schema = ParagraphSchema::default();
         let index = Index::open_in_dir(&config.path)?;
         let reader = index.reader_builder().reload_policy(ReloadPolicy::OnCommit).try_into()?;
         Ok(ParagraphReaderService {
@@ -604,18 +604,18 @@
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::start(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
         paragraph_writer_service.set_resource(&resource1)?;
-        let paragraph_reader_service = ParagraphReaderService::start(&psc).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&psc).unwrap();
         let context = ParagraphsContext::default();
 
         // Search on all paragraphs faceted
         let search = ProtosRequest {
             id: "shard1".to_string(),
             uuid: UUID.to_string(),
             body: "".to_string(),
@@ -665,19 +665,19 @@
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::start(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
         paragraph_writer_service.set_resource(&resource1)?;
 
-        let paragraph_reader_service = ParagraphReaderService::start(&psc).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&psc).unwrap();
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let mut context = ParagraphsContext::default();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
@@ -736,18 +736,18 @@
             path: dir.path().join("paragraphs"),
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
-        let mut paragraph_writer_service = ParagraphWriterService::start(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
         paragraph_writer_service.set_resource(&resource1)?;
-        let paragraph_reader_service = ParagraphReaderService::start(&psc).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&psc).unwrap();
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let empty_context = ParagraphsContext::default();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
         let faceted = Faceted {
@@ -990,20 +990,20 @@
             path: dir.path().join("paragraphs"),
         };
         let time_baseline = Timestamp {
             seconds: 2,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::start(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), time_baseline.clone());
 
         paragraph_writer_service.set_resource(&resource1)?;
 
-        let paragraph_reader_service = ParagraphReaderService::start(&psc).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&psc).unwrap();
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
         fn do_search(paragraph_reader_service: &ParagraphReaderService, timestamps: Timestamps) -> i32 {
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/set_query.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/set_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -153,31 +153,15 @@
         let safe_state = tantivy_replica::compute_safe_replica_state(params, &self.index)?;
         Ok(IndexFiles::Tantivy(safe_state))
     }
 }
 
 impl ParagraphWriterService {
     #[tracing::instrument(skip_all)]
-    pub fn start(config: &ParagraphConfig) -> NodeResult<Self> {
-        let path = std::path::Path::new(&config.path);
-        if !path.exists() {
-            match ParagraphWriterService::new(config) {
-                Err(e) if path.exists() => {
-                    std::fs::remove_dir(path)?;
-                    Err(e)
-                }
-                Err(e) => Err(e),
-                Ok(v) => Ok(v),
-            }
-        } else {
-            Ok(ParagraphWriterService::open(config)?)
-        }
-    }
-    #[tracing::instrument(skip_all)]
-    pub fn new(config: &ParagraphConfig) -> NodeResult<ParagraphWriterService> {
+    pub fn create(config: &ParagraphConfig) -> NodeResult<ParagraphWriterService> {
         let paragraph_schema = ParagraphSchema::default();
 
         fs::create_dir(&config.path)?;
 
         let mut index_builder = Index::builder().schema(paragraph_schema.schema.clone());
         let settings = IndexSettings {
             sort_by_field: Some(IndexSortByField {
@@ -446,15 +430,15 @@
     #[test]
     fn test_new_writer() -> NodeResult<()> {
         let dir = TempDir::new().unwrap();
         let psc = ParagraphConfig {
             path: dir.path().join("paragraphs"),
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::start(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
         let resource1 = create_resource("shard1".to_string());
         let _ = paragraph_writer_service.set_resource(&resource1);
         let _ = paragraph_writer_service.set_resource(&resource1);
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1201/tests/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-// Copyright (C) 2021 Bosutech XXI S.L.
-//
-// nucliadb is offered under the AGPL v3.0 and as commercial software.
-// For commercial licensing, contact us at info@nuclia.com.
-//
-// AGPL:
-// This program is free software: you can redistribute it and/or modify
-// it under the terms of the GNU Affero General Public License as
-// published by the Free Software Foundation, either version 3 of the
-// License, or (at your option) any later version.
-//
-// This program is distributed in the hope that it will be useful,
-// but WITHOUT ANY WARRANTY; without even the implied warranty of
-// MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-// GNU Affero General Public License for more details.
-//
-// You should have received a copy of the GNU Affero General Public License
-// along with this program. If not, see <http://www.gnu.org/licenses/>.
-//
-
-pub mod fuzzy_query;
-pub mod query_io;
-pub mod reader;
-pub mod schema;
-pub mod search_query;
-pub mod search_response;
-pub mod stop_words;
-pub mod writer;
+# Copyright (C) 2021 Bosutech XXI S.L.
+#
+# nucliadb is offered under the AGPL v3.0 and as commercial software.
+# For commercial licensing, contact us at info@nuclia.com.
+#
+# AGPL:
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
+#
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 
         Ok(keys)
     }
 }
 
 impl ParagraphReaderService {
     #[tracing::instrument(skip_all)]
-    pub fn start(config: &ParagraphConfig) -> NodeResult<Self> {
+    pub fn open(config: &ParagraphConfig) -> NodeResult<Self> {
         if !config.path.exists() {
             return Err(node_error!("Invalid path {:?}", config.path));
         }
         let paragraph_schema = ParagraphSchema::default();
         let index = Index::open_in_dir(&config.path)?;
         let reader = index.reader_builder().reload_policy(ReloadPolicy::OnCommit).try_into()?;
         Ok(ParagraphReaderService {
@@ -604,18 +604,18 @@
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::start(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
         let _ = paragraph_writer_service.set_resource(&resource1);
-        let paragraph_reader_service = ParagraphReaderService::start(&psc).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&psc).unwrap();
         let context = ParagraphsContext::default();
 
         // Search on all paragraphs faceted
         let search = ProtosRequest {
             id: "shard1".to_string(),
             uuid: UUID.to_string(),
             body: "".to_string(),
@@ -665,19 +665,19 @@
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::start(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
         let _ = paragraph_writer_service.set_resource(&resource1);
 
-        let paragraph_reader_service = ParagraphReaderService::start(&psc).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&psc).unwrap();
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let mut context = ParagraphsContext::default();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
@@ -736,18 +736,18 @@
             path: dir.path().join("paragraphs"),
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
-        let mut paragraph_writer_service = ParagraphWriterService::start(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
         let _ = paragraph_writer_service.set_resource(&resource1);
-        let paragraph_reader_service = ParagraphReaderService::start(&psc).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&psc).unwrap();
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let empty_context = ParagraphsContext::default();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
         let faceted = Faceted {
@@ -990,20 +990,20 @@
             path: dir.path().join("paragraphs"),
         };
         let time_baseline = Timestamp {
             seconds: 2,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::start(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), time_baseline.clone());
 
         let _ = paragraph_writer_service.set_resource(&resource1);
 
-        let paragraph_reader_service = ParagraphReaderService::start(&psc).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&psc).unwrap();
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
         fn do_search(paragraph_reader_service: &ParagraphReaderService, timestamps: Timestamps) -> i32 {
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -151,31 +151,15 @@
         let safe_state = tantivy_replica::compute_safe_replica_state(params, &self.index)?;
         Ok(IndexFiles::Tantivy(safe_state))
     }
 }
 
 impl ParagraphWriterService {
     #[tracing::instrument(skip_all)]
-    pub fn start(config: &ParagraphConfig) -> NodeResult<Self> {
-        let path = std::path::Path::new(&config.path);
-        if !path.exists() {
-            match ParagraphWriterService::new(config) {
-                Err(e) if path.exists() => {
-                    std::fs::remove_dir(path)?;
-                    Err(e)
-                }
-                Err(e) => Err(e),
-                Ok(v) => Ok(v),
-            }
-        } else {
-            Ok(ParagraphWriterService::open(config)?)
-        }
-    }
-    #[tracing::instrument(skip_all)]
-    pub fn new(config: &ParagraphConfig) -> NodeResult<ParagraphWriterService> {
+    pub fn create(config: &ParagraphConfig) -> NodeResult<ParagraphWriterService> {
         let paragraph_schema = ParagraphSchema::default();
 
         fs::create_dir(&config.path)?;
 
         let mut index_builder = Index::builder().schema(paragraph_schema.schema.clone());
         let settings = IndexSettings {
             sort_by_field: Some(IndexSortByField {
@@ -466,15 +450,15 @@
     #[test]
     fn test_new_writer() -> NodeResult<()> {
         let dir = TempDir::new().unwrap();
         let psc = ParagraphConfig {
             path: dir.path().join("paragraphs"),
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::start(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
         let resource1 = create_resource("shard1".to_string());
         let _ = paragraph_writer_service.set_resource(&resource1);
         let _ = paragraph_writer_service.set_resource(&resource1);
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1201/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1201/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "3.0.3-post1190"
+version = "3.0.3-post1201"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/CHANGELOG.md` & `nucliadb_node_binding-3.0.3.post1201/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/Makefile` & `nucliadb_node_binding-3.0.3.post1201/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/cov.sh` & `nucliadb_node_binding-3.0.3.post1201/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/pyproject.toml` & `nucliadb_node_binding-3.0.3.post1201/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/src/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1201/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/src/errors.rs` & `nucliadb_node_binding-3.0.3.post1201/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1201/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1201/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/src/update.rs` & `nucliadb_node_binding-3.0.3.post1201/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1201/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1190/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1201/tests/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,7 +13,10 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
+pytest_plugins = [
+    "nucliadb_node.tests.fixtures",
+]
```

### Comparing `nucliadb_node_binding-3.0.3.post1190/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1201/tests/integration/test_indexing.py`

 * *Files identical despite different names*

