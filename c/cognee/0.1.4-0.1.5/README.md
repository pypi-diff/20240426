# Comparing `tmp/cognee-0.1.4.tar.gz` & `tmp/cognee-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognee-0.1.4.tar", max compression
+gzip compressed data, was "cognee-0.1.5.tar", max compression
```

## Comparing `cognee-0.1.4.tar` & `cognee-0.1.5.tar`

### file list

```diff
@@ -1,155 +1,170 @@
--rw-r--r--   0        0        0    11344 2024-03-30 14:25:45.849829 cognee-0.1.4/LICENSE
--rw-r--r--   0        0        0     3668 2024-04-24 17:34:59.318133 cognee-0.1.4/README.md
--rw-r--r--   0        0        0      249 2024-03-30 11:45:01.187785 cognee-0.1.4/cognee/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333367 cognee-0.1.4/cognee/api/__init__.py
--rw-r--r--   0        0        0     3242 2024-03-30 16:41:17.062218 cognee-0.1.4/cognee/api/client.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333421 cognee-0.1.4/cognee/api/v1/__init__.py
--rw-r--r--   0        0        0       21 2024-03-13 17:10:40.333706 cognee-0.1.4/cognee/api/v1/add/__init__.py
--rw-r--r--   0        0        0     4719 2024-04-24 17:34:59.318599 cognee-0.1.4/cognee/api/v1/add/add.py
--rw-r--r--   0        0        0     1517 2024-03-29 12:58:54.562218 cognee-0.1.4/cognee/api/v1/add/add_standalone.py
--rw-r--r--   0        0        0      626 2024-03-29 12:58:54.562387 cognee-0.1.4/cognee/api/v1/add/remember.py
--rw-r--r--   0        0        0     6957 2024-04-24 17:34:59.318939 cognee-0.1.4/cognee/api/v1/cognify/cognify.py
--rw-r--r--   0        0        0       27 2024-03-29 12:58:54.562770 cognee-0.1.4/cognee/api/v1/config/__init__.py
--rw-r--r--   0        0        0     2296 2024-04-24 17:34:59.319404 cognee-0.1.4/cognee/api/v1/config/config.py
--rw-r--r--   0        0        0      594 2024-04-20 17:06:04.933300 cognee-0.1.4/cognee/api/v1/datasets/datasets.py
--rw-r--r--   0        0        0       25 2024-03-29 16:33:26.552588 cognee-0.1.4/cognee/api/v1/prune/__init__.py
--rw-r--r--   0        0        0      965 2024-04-20 17:06:04.933673 cognee-0.1.4/cognee/api/v1/prune/prune.py
--rw-r--r--   0        0        0       39 2024-03-22 15:50:27.356555 cognee-0.1.4/cognee/api/v1/search/__init__.py
--rw-r--r--   0        0        0     3612 2024-04-24 17:34:59.319907 cognee-0.1.4/cognee/api/v1/search/search.py
--rw-r--r--   0        0        0     6471 2024-04-24 17:34:59.320284 cognee-0.1.4/cognee/config.py
--rw-r--r--   0        0        0     1778 2024-03-13 17:10:40.342297 cognee-0.1.4/cognee/fetch_secret.py
--rw-r--r--   0        0        0     7858 2024-04-24 17:34:59.320914 cognee-0.1.4/cognee/infrastructure/InfrastructureConfig.py
--rw-r--r--   0        0        0       56 2024-03-13 17:10:40.343200 cognee-0.1.4/cognee/infrastructure/__init__.py
--rw-r--r--   0        0        0      110 2024-03-29 12:58:54.563482 cognee-0.1.4/cognee/infrastructure/data/__init__.py
--rw-r--r--   0        0        0     4456 2024-04-24 17:34:59.321526 cognee-0.1.4/cognee/infrastructure/data/chunking/DefaultChunkEngine.py
--rw-r--r--   0        0        0      889 2024-03-13 17:10:40.343833 cognee-0.1.4/cognee/infrastructure/data/models/Data.py
--rw-r--r--   0        0        0      721 2024-03-13 17:10:40.344000 cognee-0.1.4/cognee/infrastructure/data/models/Dataset.py
--rw-r--r--   0        0        0      553 2024-03-13 17:10:40.344153 cognee-0.1.4/cognee/infrastructure/data/models/DatasetData.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344189 cognee-0.1.4/cognee/infrastructure/data/models/__init__.py
--rw-r--r--   0        0        0      756 2024-04-21 19:51:39.681809 cognee-0.1.4/cognee/infrastructure/data/utils/extract_keywords.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344241 cognee-0.1.4/cognee/infrastructure/databases/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344307 cognee-0.1.4/cognee/infrastructure/databases/graph/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-20 17:13:59.861624 cognee-0.1.4/cognee/infrastructure/databases/graph/get_graph_client.py
--rw-r--r--   0        0        0     1162 2024-04-20 17:06:04.935830 cognee-0.1.4/cognee/infrastructure/databases/graph/graph_db_interface.py
--rw-r--r--   0        0        0        0 2024-04-20 17:06:04.935887 cognee-0.1.4/cognee/infrastructure/databases/graph/neo4j_driver/__init__.py
--rw-r--r--   0        0        0     8109 2024-04-20 17:06:04.936346 cognee-0.1.4/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344904 cognee-0.1.4/cognee/infrastructure/databases/graph/networkx/__init__.py
--rw-r--r--   0        0        0     5212 2024-04-20 17:06:04.936777 cognee-0.1.4/cognee/infrastructure/databases/graph/networkx/adapter.py
--rw-r--r--   0        0        0      462 2024-03-13 17:10:40.345204 cognee-0.1.4/cognee/infrastructure/databases/relational/DatabaseEngine.py
--rw-r--r--   0        0        0       76 2024-03-13 17:10:40.345343 cognee-0.1.4/cognee/infrastructure/databases/relational/ModelBase.py
--rw-r--r--   0        0        0      170 2024-03-13 17:10:40.345690 cognee-0.1.4/cognee/infrastructure/databases/relational/__init__.py
--rw-r--r--   0        0        0     4539 2024-04-20 17:06:04.937151 cognee-0.1.4/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
--rw-r--r--   0        0        0     1006 2024-03-13 17:10:40.346527 cognee-0.1.4/cognee/infrastructure/databases/relational/relational_db_interface.py
--rw-r--r--   0        0        0     2847 2024-03-13 17:10:40.346830 cognee-0.1.4/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.346864 cognee-0.1.4/cognee/infrastructure/databases/relational/sqlite/__init__.py
--rw-r--r--   0        0        0       41 2024-03-13 17:10:40.347026 cognee-0.1.4/cognee/infrastructure/databases/relational/utils/__init__.py
--rw-r--r--   0        0        0      595 2024-03-13 17:10:40.347281 cognee-0.1.4/cognee/infrastructure/databases/relational/utils/with_rollback.py
--rw-r--r--   0        0        0      191 2024-03-29 14:26:49.588629 cognee-0.1.4/cognee/infrastructure/databases/vector/__init__.py
--rw-r--r--   0        0        0     1410 2024-04-20 17:06:04.937392 cognee-0.1.4/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
--rw-r--r--   0        0        0      237 2024-03-29 12:58:54.564681 cognee-0.1.4/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
--rw-r--r--   0        0        0      138 2024-03-22 15:50:27.357923 cognee-0.1.4/cognee/infrastructure/databases/vector/models/CollectionConfig.py
--rw-r--r--   0        0        0      261 2024-04-20 17:06:04.938241 cognee-0.1.4/cognee/infrastructure/databases/vector/models/DataPoint.py
--rw-r--r--   0        0        0      171 2024-03-22 15:50:27.358192 cognee-0.1.4/cognee/infrastructure/databases/vector/models/ScoredResult.py
--rw-r--r--   0        0        0      143 2024-03-22 15:50:27.358320 cognee-0.1.4/cognee/infrastructure/databases/vector/models/VectorConfig.py
--rw-r--r--   0        0        0      256 2024-03-13 17:10:40.348493 cognee-0.1.4/cognee/infrastructure/databases/vector/pinecone/adapter.py
--rw-r--r--   0        0        0     6114 2024-04-20 17:06:04.938634 cognee-0.1.4/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
--rw-r--r--   0        0        0       96 2024-04-20 17:06:04.938909 cognee-0.1.4/cognee/infrastructure/databases/vector/qdrant/__init__.py
--rw-r--r--   0        0        0     2195 2024-03-29 12:58:54.565755 cognee-0.1.4/cognee/infrastructure/databases/vector/vector_db_interface.py
--rw-r--r--   0        0        0     4664 2024-04-20 17:37:59.594359 cognee-0.1.4/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
--rw-r--r--   0        0        0       45 2024-03-22 15:50:27.359256 cognee-0.1.4/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
--rw-r--r--   0        0        0      185 2024-03-13 17:10:40.349945 cognee-0.1.4/cognee/infrastructure/files/__init__.py
--rw-r--r--   0        0        0      364 2024-03-13 17:10:40.350194 cognee-0.1.4/cognee/infrastructure/files/add_file_to_storage.py
--rw-r--r--   0        0        0      320 2024-03-13 17:10:40.350437 cognee-0.1.4/cognee/infrastructure/files/remove_file_from_storage.py
--rw-r--r--   0        0        0     1443 2024-04-20 17:06:04.939689 cognee-0.1.4/cognee/infrastructure/files/storage/LocalStorage.py
--rw-r--r--   0        0        0      640 2024-03-13 17:10:40.350788 cognee-0.1.4/cognee/infrastructure/files/storage/StorageManager.py
--rw-r--r--   0        0        0       39 2024-03-13 17:10:40.351087 cognee-0.1.4/cognee/infrastructure/files/storage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351134 cognee-0.1.4/cognee/infrastructure/files/utils/__init__.py
--rw-r--r--   0        0        0      392 2024-04-23 10:42:22.654946 cognee-0.1.4/cognee/infrastructure/files/utils/extract_text_from_file.py
--rw-r--r--   0        0        0      835 2024-04-23 10:42:22.655413 cognee-0.1.4/cognee/infrastructure/files/utils/get_file_metadata.py
--rw-r--r--   0        0        0       84 2024-03-13 17:10:40.351628 cognee-0.1.4/cognee/infrastructure/files/utils/get_file_size.py
--rw-r--r--   0        0        0      748 2024-03-29 12:58:54.566841 cognee-0.1.4/cognee/infrastructure/files/utils/guess_file_type.py
--rw-r--r--   0        0        0      825 2024-03-29 12:58:54.567011 cognee-0.1.4/cognee/infrastructure/files/utils/is_text_content.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351679 cognee-0.1.4/cognee/infrastructure/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 12:58:54.567125 cognee-0.1.4/cognee/infrastructure/llm/anthropic/__init__.py
--rw-r--r--   0        0        0     1768 2024-04-20 17:06:04.940078 cognee-0.1.4/cognee/infrastructure/llm/anthropic/adapter.py
--rw-r--r--   0        0        0     4308 2024-04-20 17:06:04.940411 cognee-0.1.4/cognee/infrastructure/llm/generic_llm_api/adapter.py
--rw-r--r--   0        0        0     1112 2024-04-20 17:06:04.940688 cognee-0.1.4/cognee/infrastructure/llm/get_llm_client.py
--rw-r--r--   0        0        0     1593 2024-04-20 17:06:04.941068 cognee-0.1.4/cognee/infrastructure/llm/llm_interface.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.352341 cognee-0.1.4/cognee/infrastructure/llm/openai/__init__.py
--rw-r--r--   0        0        0     4885 2024-04-20 17:06:04.941424 cognee-0.1.4/cognee/infrastructure/llm/openai/adapter.py
--rw-r--r--   0        0        0       90 2024-03-22 15:50:27.360221 cognee-0.1.4/cognee/infrastructure/llm/prompts/__init__.py
--rw-r--r--   0        0        0     5614 2024-03-13 17:10:40.353367 cognee-0.1.4/cognee/infrastructure/llm/prompts/classify_content.txt
--rw-r--r--   0        0        0     1323 2024-04-20 17:06:04.941763 cognee-0.1.4/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
--rw-r--r--   0        0        0     2192 2024-04-20 17:06:04.942070 cognee-0.1.4/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
--rw-r--r--   0        0        0      613 2024-03-22 15:50:27.360715 cognee-0.1.4/cognee/infrastructure/llm/prompts/read_query_prompt.py
--rw-r--r--   0        0        0      962 2024-03-22 15:50:27.360888 cognee-0.1.4/cognee/infrastructure/llm/prompts/render_prompt.py
--rw-r--r--   0        0        0       86 2024-03-22 15:50:27.361017 cognee-0.1.4/cognee/infrastructure/llm/prompts/summarize_content.txt
--rw-r--r--   0        0        0      889 2024-03-13 17:10:40.353850 cognee-0.1.4/cognee/infrastructure/pipeline/models/Operation.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353900 cognee-0.1.4/cognee/infrastructure/pipeline/models/_init_.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353968 cognee-0.1.4/cognee/modules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 08:53:16.821314 cognee-0.1.4/cognee/modules/cognify/__init__.py
--rw-r--r--   0        0        0     3298 2024-04-21 08:39:11.814707 cognee-0.1.4/cognee/modules/cognify/dataset.py
--rw-r--r--   0        0        0     2622 2024-04-21 08:53:49.473271 cognee-0.1.4/cognee/modules/cognify/evaluate.py
--rw-r--r--   0        0        0        1 2024-03-13 17:10:40.354160 cognee-0.1.4/cognee/modules/cognify/graph/__init__.py
--rw-r--r--   0        0        0     1186 2024-04-24 17:35:40.798253 cognee-0.1.4/cognee/modules/cognify/graph/add_classification_nodes.py
--rw-r--r--   0        0        0     4928 2024-04-24 17:35:40.798450 cognee-0.1.4/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py
--rw-r--r--   0        0        0      915 2024-04-24 17:35:40.798631 cognee-0.1.4/cognee/modules/cognify/graph/add_cognitive_layers.py
--rw-r--r--   0        0        0     1273 2024-04-24 17:34:59.322096 cognee-0.1.4/cognee/modules/cognify/graph/add_data_chunks.py
--rw-r--r--   0        0        0      797 2024-04-24 17:35:40.798810 cognee-0.1.4/cognee/modules/cognify/graph/add_document_node.py
--rw-r--r--   0        0        0     1948 2024-04-24 17:35:40.798974 cognee-0.1.4/cognee/modules/cognify/graph/add_label_nodes.py
--rw-r--r--   0        0        0     6969 2024-04-20 17:06:04.945151 cognee-0.1.4/cognee/modules/cognify/graph/add_node_connections.py
--rw-r--r--   0        0        0      798 2024-04-24 17:35:40.799140 cognee-0.1.4/cognee/modules/cognify/graph/add_summary_nodes.py
--rw-r--r--   0        0        0    10961 2024-04-20 17:06:04.945725 cognee-0.1.4/cognee/modules/cognify/graph/create.py
--rw-r--r--   0        0        0     1673 2024-04-20 17:06:04.946033 cognee-0.1.4/cognee/modules/cognify/graph/initialize_graph.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.355565 cognee-0.1.4/cognee/modules/cognify/llm/__init__.py
--rw-r--r--   0        0        0     1216 2024-04-20 17:06:04.946434 cognee-0.1.4/cognee/modules/cognify/llm/resolve_cross_graph_references.py
--rw-r--r--   0        0        0     7187 2024-04-21 13:31:24.978503 cognee-0.1.4/cognee/modules/cognify/test.py
--rw-r--r--   0        0        0     2669 2024-04-21 08:53:43.386066 cognee-0.1.4/cognee/modules/cognify/train.py
--rw-r--r--   0        0        0      960 2024-04-20 17:06:04.947116 cognee-0.1.4/cognee/modules/data/extraction/extract_categories.py
--rw-r--r--   0        0        0      490 2024-04-20 17:06:04.947749 cognee-0.1.4/cognee/modules/data/extraction/extract_cognitive_layers.py
--rw-r--r--   0        0        0      497 2024-04-20 17:06:04.948077 cognee-0.1.4/cognee/modules/data/extraction/extract_summary.py
--rw-r--r--   0        0        0      542 2024-04-20 17:06:04.948548 cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py
--rw-r--r--   0        0        0     1102 2024-04-24 17:35:40.799380 cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py
--rw-r--r--   0        0        0     4726 2024-04-24 17:35:40.799590 cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py
--rw-r--r--   0        0        0      638 2024-04-20 17:06:04.949628 cognee-0.1.4/cognee/modules/data/get_cognitive_layers.py
--rw-r--r--   0        0        0      516 2024-04-20 17:06:04.949924 cognee-0.1.4/cognee/modules/data/get_content_categories.py
--rw-r--r--   0        0        0      499 2024-04-20 17:06:04.950170 cognee-0.1.4/cognee/modules/data/get_content_summary.py
--rw-r--r--   0        0        0      895 2024-04-20 17:06:04.950394 cognee-0.1.4/cognee/modules/data/get_layer_graphs.py
--rw-r--r--   0        0        0       69 2024-03-30 11:42:14.111069 cognee-0.1.4/cognee/modules/discovery/__init__.py
--rw-r--r--   0        0        0      756 2024-03-30 11:49:14.418639 cognee-0.1.4/cognee/modules/discovery/discover_directory_datasets.py
--rw-r--r--   0        0        0       62 2024-03-29 12:58:54.570027 cognee-0.1.4/cognee/modules/ingestion/__init__.py
--rw-r--r--   0        0        0     1763 2024-03-29 12:58:54.570193 cognee-0.1.4/cognee/modules/ingestion/add_data_to_dataset.py
--rw-r--r--   0        0        0      490 2024-03-29 12:58:54.570428 cognee-0.1.4/cognee/modules/ingestion/classify.py
--rw-r--r--   0        0        0      780 2024-04-21 19:39:20.100717 cognee-0.1.4/cognee/modules/ingestion/data_types/BinaryData.py
--rw-r--r--   0        0        0      295 2024-04-21 19:33:23.824343 cognee-0.1.4/cognee/modules/ingestion/data_types/IngestionData.py
--rw-r--r--   0        0        0      764 2024-04-21 19:38:38.394049 cognee-0.1.4/cognee/modules/ingestion/data_types/TextData.py
--rw-r--r--   0        0        0      145 2024-03-13 17:10:40.359643 cognee-0.1.4/cognee/modules/ingestion/data_types/__init__.py
--rw-r--r--   0        0        0      125 2024-03-13 17:10:40.359841 cognee-0.1.4/cognee/modules/ingestion/exceptions.py
--rw-r--r--   0        0        0      275 2024-04-20 17:06:04.950837 cognee-0.1.4/cognee/modules/ingestion/identify.py
--rw-r--r--   0        0        0      796 2024-03-29 12:58:54.571415 cognee-0.1.4/cognee/modules/ingestion/save.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.360307 cognee-0.1.4/cognee/modules/memory/__init__.py
--rw-r--r--   0        0        0       55 2024-03-13 17:10:40.361059 cognee-0.1.4/cognee/modules/memory/vector/__init__.py
--rw-r--r--   0        0        0      378 2024-03-13 17:10:40.361283 cognee-0.1.4/cognee/modules/memory/vector/create_vector_memory.py
--rw-r--r--   0        0        0     1109 2024-04-20 17:06:04.951176 cognee-0.1.4/cognee/modules/search/CogneeSearch.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361325 cognee-0.1.4/cognee/modules/search/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361372 cognee-0.1.4/cognee/modules/search/graph/__init__.py
--rw-r--r--   0        0        0     2083 2024-04-20 17:23:41.887212 cognee-0.1.4/cognee/modules/search/graph/search_adjacent.py
--rw-r--r--   0        0        0     1869 2024-04-20 17:23:55.244065 cognee-0.1.4/cognee/modules/search/graph/search_categories.py
--rw-r--r--   0        0        0     2976 2024-04-20 17:23:50.632849 cognee-0.1.4/cognee/modules/search/graph/search_neighbour.py
--rw-r--r--   0        0        0     1747 2024-04-20 17:24:00.829943 cognee-0.1.4/cognee/modules/search/graph/search_summary.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361762 cognee-0.1.4/cognee/modules/search/vector/__init__.py
--rw-r--r--   0        0        0     1579 2024-04-20 17:45:36.721313 cognee-0.1.4/cognee/modules/search/vector/search_similarity.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.362031 cognee-0.1.4/cognee/modules/users/__init__.py
--rw-r--r--   0        0        0      179 2024-03-13 17:10:40.362758 cognee-0.1.4/cognee/modules/users/memory/__init__.py
--rw-r--r--   0        0        0      802 2024-03-13 17:10:40.362950 cognee-0.1.4/cognee/modules/users/memory/create_information_points.py
--rw-r--r--   0        0        0      229 2024-03-13 17:10:40.363108 cognee-0.1.4/cognee/modules/users/memory/is_existing_memory.py
--rw-r--r--   0        0        0      203 2024-03-13 17:10:40.363292 cognee-0.1.4/cognee/modules/users/memory/register_memory_for_user.py
--rw-r--r--   0        0        0   124245 2024-04-21 08:54:54.214070 cognee-0.1.4/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json
--rw-r--r--   0        0        0      182 2024-03-13 17:10:40.363716 cognee-0.1.4/cognee/root_dir.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.364048 cognee-0.1.4/cognee/shared/__init__.py
--rw-r--r--   0        0        0     8633 2024-04-24 17:35:40.799838 cognee-0.1.4/cognee/shared/data_models.py
--rw-r--r--   0        0        0      365 2024-03-22 15:50:27.366234 cognee-0.1.4/cognee/shared/encode_uuid.py
--rw-r--r--   0        0        0     5635 2024-04-20 17:06:04.953913 cognee-0.1.4/cognee/tests/test_library.py
--rw-r--r--   0        0        0     9360 2024-04-24 17:34:59.322831 cognee-0.1.4/cognee/utils.py
--rw-r--r--   0        0        0     3491 2024-04-24 17:36:10.281347 cognee-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7141 1970-01-01 00:00:00.000000 cognee-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-03-30 14:25:45.849829 cognee-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3668 2024-04-24 17:34:59.318133 cognee-0.1.5/README.md
+-rw-r--r--   0        0        0      249 2024-03-30 11:45:01.187785 cognee-0.1.5/cognee/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333367 cognee-0.1.5/cognee/api/__init__.py
+-rw-r--r--   0        0        0     4370 2024-04-25 22:16:19.632624 cognee-0.1.5/cognee/api/client.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333421 cognee-0.1.5/cognee/api/v1/__init__.py
+-rw-r--r--   0        0        0       21 2024-03-13 17:10:40.333706 cognee-0.1.5/cognee/api/v1/add/__init__.py
+-rw-r--r--   0        0        0     4716 2024-04-25 22:16:19.633201 cognee-0.1.5/cognee/api/v1/add/add.py
+-rw-r--r--   0        0        0     1517 2024-03-29 12:58:54.562218 cognee-0.1.5/cognee/api/v1/add/add_standalone.py
+-rw-r--r--   0        0        0      626 2024-03-29 12:58:54.562387 cognee-0.1.5/cognee/api/v1/add/remember.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.633260 cognee-0.1.5/cognee/api/v1/cognify/__init__.py
+-rw-r--r--   0        0        0     6990 2024-04-25 22:16:19.633740 cognee-0.1.5/cognee/api/v1/cognify/cognify.py
+-rw-r--r--   0        0        0       27 2024-03-29 12:58:54.562770 cognee-0.1.5/cognee/api/v1/config/__init__.py
+-rw-r--r--   0        0        0     2296 2024-04-24 17:34:59.319404 cognee-0.1.5/cognee/api/v1/config/config.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.633793 cognee-0.1.5/cognee/api/v1/datasets/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-20 17:06:04.933300 cognee-0.1.5/cognee/api/v1/datasets/datasets.py
+-rw-r--r--   0        0        0       25 2024-03-29 16:33:26.552588 cognee-0.1.5/cognee/api/v1/prune/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-20 17:06:04.933673 cognee-0.1.5/cognee/api/v1/prune/prune.py
+-rw-r--r--   0        0        0       39 2024-03-22 15:50:27.356555 cognee-0.1.5/cognee/api/v1/search/__init__.py
+-rw-r--r--   0        0        0     3611 2024-04-25 22:16:19.634363 cognee-0.1.5/cognee/api/v1/search/search.py
+-rw-r--r--   0        0        0     6489 2024-04-25 22:16:19.634966 cognee-0.1.5/cognee/config.py
+-rw-r--r--   0        0        0     1778 2024-03-13 17:10:40.342297 cognee-0.1.5/cognee/fetch_secret.py
+-rw-r--r--   0        0        0     7705 2024-04-25 22:16:19.635586 cognee-0.1.5/cognee/infrastructure/InfrastructureConfig.py
+-rw-r--r--   0        0        0       56 2024-03-13 17:10:40.343200 cognee-0.1.5/cognee/infrastructure/__init__.py
+-rw-r--r--   0        0        0      110 2024-03-29 12:58:54.563482 cognee-0.1.5/cognee/infrastructure/data/__init__.py
+-rw-r--r--   0        0        0     4456 2024-04-24 17:34:59.321526 cognee-0.1.5/cognee/infrastructure/data/chunking/DefaultChunkEngine.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.635699 cognee-0.1.5/cognee/infrastructure/data/chunking/__init__.py
+-rw-r--r--   0        0        0      889 2024-03-13 17:10:40.343833 cognee-0.1.5/cognee/infrastructure/data/models/Data.py
+-rw-r--r--   0        0        0      721 2024-03-13 17:10:40.344000 cognee-0.1.5/cognee/infrastructure/data/models/Dataset.py
+-rw-r--r--   0        0        0      553 2024-03-13 17:10:40.344153 cognee-0.1.5/cognee/infrastructure/data/models/DatasetData.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344189 cognee-0.1.5/cognee/infrastructure/data/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.635851 cognee-0.1.5/cognee/infrastructure/data/utils/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-21 19:51:39.681809 cognee-0.1.5/cognee/infrastructure/data/utils/extract_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344241 cognee-0.1.5/cognee/infrastructure/databases/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344307 cognee-0.1.5/cognee/infrastructure/databases/graph/__init__.py
+-rw-r--r--   0        0        0     1290 2024-04-25 22:16:19.636422 cognee-0.1.5/cognee/infrastructure/databases/graph/get_graph_client.py
+-rw-r--r--   0        0        0     1162 2024-04-20 17:06:04.935830 cognee-0.1.5/cognee/infrastructure/databases/graph/graph_db_interface.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:06:04.935887 cognee-0.1.5/cognee/infrastructure/databases/graph/neo4j_driver/__init__.py
+-rw-r--r--   0        0        0     8109 2024-04-20 17:06:04.936346 cognee-0.1.5/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344904 cognee-0.1.5/cognee/infrastructure/databases/graph/networkx/__init__.py
+-rw-r--r--   0        0        0     5337 2024-04-25 22:16:19.636869 cognee-0.1.5/cognee/infrastructure/databases/graph/networkx/adapter.py
+-rw-r--r--   0        0        0      462 2024-03-13 17:10:40.345204 cognee-0.1.5/cognee/infrastructure/databases/relational/DatabaseEngine.py
+-rw-r--r--   0        0        0       76 2024-03-13 17:10:40.345343 cognee-0.1.5/cognee/infrastructure/databases/relational/ModelBase.py
+-rw-r--r--   0        0        0      170 2024-03-13 17:10:40.345690 cognee-0.1.5/cognee/infrastructure/databases/relational/__init__.py
+-rw-r--r--   0        0        0     4539 2024-04-20 17:06:04.937151 cognee-0.1.5/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637021 cognee-0.1.5/cognee/infrastructure/databases/relational/duckdb/__init__.py
+-rw-r--r--   0        0        0     1006 2024-03-13 17:10:40.346527 cognee-0.1.5/cognee/infrastructure/databases/relational/relational_db_interface.py
+-rw-r--r--   0        0        0     2847 2024-03-13 17:10:40.346830 cognee-0.1.5/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.346864 cognee-0.1.5/cognee/infrastructure/databases/relational/sqlite/__init__.py
+-rw-r--r--   0        0        0       41 2024-03-13 17:10:40.347026 cognee-0.1.5/cognee/infrastructure/databases/relational/utils/__init__.py
+-rw-r--r--   0        0        0      595 2024-03-13 17:10:40.347281 cognee-0.1.5/cognee/infrastructure/databases/relational/utils/with_rollback.py
+-rw-r--r--   0        0        0      191 2024-03-29 14:26:49.588629 cognee-0.1.5/cognee/infrastructure/databases/vector/__init__.py
+-rw-r--r--   0        0        0     1410 2024-04-20 17:06:04.937392 cognee-0.1.5/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
+-rw-r--r--   0        0        0      237 2024-03-29 12:58:54.564681 cognee-0.1.5/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637164 cognee-0.1.5/cognee/infrastructure/databases/vector/embeddings/__init__.py
+-rw-r--r--   0        0        0     2791 2024-04-25 22:16:19.637628 cognee-0.1.5/cognee/infrastructure/databases/vector/lancedb/LanceDBAdapter.py
+-rw-r--r--   0        0        0      138 2024-03-22 15:50:27.357923 cognee-0.1.5/cognee/infrastructure/databases/vector/models/CollectionConfig.py
+-rw-r--r--   0        0        0      261 2024-04-20 17:06:04.938241 cognee-0.1.5/cognee/infrastructure/databases/vector/models/DataPoint.py
+-rw-r--r--   0        0        0      171 2024-03-22 15:50:27.358192 cognee-0.1.5/cognee/infrastructure/databases/vector/models/ScoredResult.py
+-rw-r--r--   0        0        0      143 2024-03-22 15:50:27.358320 cognee-0.1.5/cognee/infrastructure/databases/vector/models/VectorConfig.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637726 cognee-0.1.5/cognee/infrastructure/databases/vector/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637873 cognee-0.1.5/cognee/infrastructure/databases/vector/pinecone/__init__.py
+-rw-r--r--   0        0        0      256 2024-03-13 17:10:40.348493 cognee-0.1.5/cognee/infrastructure/databases/vector/pinecone/adapter.py
+-rw-r--r--   0        0        0     6658 2024-04-25 22:16:19.638528 cognee-0.1.5/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
+-rw-r--r--   0        0        0       96 2024-04-20 17:06:04.938909 cognee-0.1.5/cognee/infrastructure/databases/vector/qdrant/__init__.py
+-rw-r--r--   0        0        0     2195 2024-03-29 12:58:54.565755 cognee-0.1.5/cognee/infrastructure/databases/vector/vector_db_interface.py
+-rw-r--r--   0        0        0     4965 2024-04-25 22:16:19.639144 cognee-0.1.5/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
+-rw-r--r--   0        0        0       45 2024-03-22 15:50:27.359256 cognee-0.1.5/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
+-rw-r--r--   0        0        0      185 2024-03-13 17:10:40.349945 cognee-0.1.5/cognee/infrastructure/files/__init__.py
+-rw-r--r--   0        0        0      364 2024-03-13 17:10:40.350194 cognee-0.1.5/cognee/infrastructure/files/add_file_to_storage.py
+-rw-r--r--   0        0        0      320 2024-03-13 17:10:40.350437 cognee-0.1.5/cognee/infrastructure/files/remove_file_from_storage.py
+-rw-r--r--   0        0        0     1443 2024-04-20 17:06:04.939689 cognee-0.1.5/cognee/infrastructure/files/storage/LocalStorage.py
+-rw-r--r--   0        0        0      640 2024-03-13 17:10:40.350788 cognee-0.1.5/cognee/infrastructure/files/storage/StorageManager.py
+-rw-r--r--   0        0        0       39 2024-03-13 17:10:40.351087 cognee-0.1.5/cognee/infrastructure/files/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351134 cognee-0.1.5/cognee/infrastructure/files/utils/__init__.py
+-rw-r--r--   0        0        0      392 2024-04-23 10:42:22.654946 cognee-0.1.5/cognee/infrastructure/files/utils/extract_text_from_file.py
+-rw-r--r--   0        0        0      835 2024-04-23 10:42:22.655413 cognee-0.1.5/cognee/infrastructure/files/utils/get_file_metadata.py
+-rw-r--r--   0        0        0       84 2024-03-13 17:10:40.351628 cognee-0.1.5/cognee/infrastructure/files/utils/get_file_size.py
+-rw-r--r--   0        0        0      748 2024-03-29 12:58:54.566841 cognee-0.1.5/cognee/infrastructure/files/utils/guess_file_type.py
+-rw-r--r--   0        0        0      825 2024-03-29 12:58:54.567011 cognee-0.1.5/cognee/infrastructure/files/utils/is_text_content.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351679 cognee-0.1.5/cognee/infrastructure/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 12:58:54.567125 cognee-0.1.5/cognee/infrastructure/llm/anthropic/__init__.py
+-rw-r--r--   0        0        0     1768 2024-04-20 17:06:04.940078 cognee-0.1.5/cognee/infrastructure/llm/anthropic/adapter.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.639301 cognee-0.1.5/cognee/infrastructure/llm/generic_llm_api/__init__.py
+-rw-r--r--   0        0        0     4308 2024-04-20 17:06:04.940411 cognee-0.1.5/cognee/infrastructure/llm/generic_llm_api/adapter.py
+-rw-r--r--   0        0        0     1112 2024-04-20 17:06:04.940688 cognee-0.1.5/cognee/infrastructure/llm/get_llm_client.py
+-rw-r--r--   0        0        0     1593 2024-04-20 17:06:04.941068 cognee-0.1.5/cognee/infrastructure/llm/llm_interface.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.352341 cognee-0.1.5/cognee/infrastructure/llm/openai/__init__.py
+-rw-r--r--   0        0        0     4885 2024-04-20 17:06:04.941424 cognee-0.1.5/cognee/infrastructure/llm/openai/adapter.py
+-rw-r--r--   0        0        0       90 2024-03-22 15:50:27.360221 cognee-0.1.5/cognee/infrastructure/llm/prompts/__init__.py
+-rw-r--r--   0        0        0     5614 2024-03-13 17:10:40.353367 cognee-0.1.5/cognee/infrastructure/llm/prompts/classify_content.txt
+-rw-r--r--   0        0        0     1323 2024-04-20 17:06:04.941763 cognee-0.1.5/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
+-rw-r--r--   0        0        0     2192 2024-04-20 17:06:04.942070 cognee-0.1.5/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
+-rw-r--r--   0        0        0      613 2024-03-22 15:50:27.360715 cognee-0.1.5/cognee/infrastructure/llm/prompts/read_query_prompt.py
+-rw-r--r--   0        0        0      962 2024-03-22 15:50:27.360888 cognee-0.1.5/cognee/infrastructure/llm/prompts/render_prompt.py
+-rw-r--r--   0        0        0       86 2024-03-22 15:50:27.361017 cognee-0.1.5/cognee/infrastructure/llm/prompts/summarize_content.txt
+-rw-r--r--   0        0        0      889 2024-03-13 17:10:40.353850 cognee-0.1.5/cognee/infrastructure/pipeline/models/Operation.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.639465 cognee-0.1.5/cognee/infrastructure/pipeline/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353968 cognee-0.1.5/cognee/modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 08:53:16.821314 cognee-0.1.5/cognee/modules/cognify/__init__.py
+-rw-r--r--   0        0        0     3298 2024-04-21 08:39:11.814707 cognee-0.1.5/cognee/modules/cognify/dataset.py
+-rw-r--r--   0        0        0     2622 2024-04-21 08:53:49.473271 cognee-0.1.5/cognee/modules/cognify/evaluate.py
+-rw-r--r--   0        0        0        1 2024-03-13 17:10:40.354160 cognee-0.1.5/cognee/modules/cognify/graph/__init__.py
+-rw-r--r--   0        0        0     1186 2024-04-25 22:16:19.640140 cognee-0.1.5/cognee/modules/cognify/graph/add_classification_nodes.py
+-rw-r--r--   0        0        0     4928 2024-04-25 09:42:30.765000 cognee-0.1.5/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py
+-rw-r--r--   0        0        0     1138 2024-04-25 22:16:19.640702 cognee-0.1.5/cognee/modules/cognify/graph/add_cognitive_layers.py
+-rw-r--r--   0        0        0     2065 2024-04-25 22:16:19.641132 cognee-0.1.5/cognee/modules/cognify/graph/add_data_chunks.py
+-rw-r--r--   0        0        0      797 2024-04-25 09:42:30.766116 cognee-0.1.5/cognee/modules/cognify/graph/add_document_node.py
+-rw-r--r--   0        0        0     1948 2024-04-25 09:42:30.766655 cognee-0.1.5/cognee/modules/cognify/graph/add_label_nodes.py
+-rw-r--r--   0        0        0     6969 2024-04-20 17:06:04.945151 cognee-0.1.5/cognee/modules/cognify/graph/add_node_connections.py
+-rw-r--r--   0        0        0      798 2024-04-25 09:42:30.766937 cognee-0.1.5/cognee/modules/cognify/graph/add_summary_nodes.py
+-rw-r--r--   0        0        0    10961 2024-04-20 17:06:04.945725 cognee-0.1.5/cognee/modules/cognify/graph/create.py
+-rw-r--r--   0        0        0     1673 2024-04-20 17:06:04.946033 cognee-0.1.5/cognee/modules/cognify/graph/initialize_graph.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.355565 cognee-0.1.5/cognee/modules/cognify/llm/__init__.py
+-rw-r--r--   0        0        0     1216 2024-04-20 17:06:04.946434 cognee-0.1.5/cognee/modules/cognify/llm/resolve_cross_graph_references.py
+-rw-r--r--   0        0        0     7187 2024-04-21 13:31:24.978503 cognee-0.1.5/cognee/modules/cognify/test.py
+-rw-r--r--   0        0        0     2669 2024-04-21 08:53:43.386066 cognee-0.1.5/cognee/modules/cognify/train.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641213 cognee-0.1.5/cognee/modules/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641372 cognee-0.1.5/cognee/modules/data/extraction/__init__.py
+-rw-r--r--   0        0        0      960 2024-04-20 17:06:04.947116 cognee-0.1.5/cognee/modules/data/extraction/extract_categories.py
+-rw-r--r--   0        0        0      490 2024-04-20 17:06:04.947749 cognee-0.1.5/cognee/modules/data/extraction/extract_cognitive_layers.py
+-rw-r--r--   0        0        0      497 2024-04-20 17:06:04.948077 cognee-0.1.5/cognee/modules/data/extraction/extract_summary.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641459 cognee-0.1.5/cognee/modules/data/extraction/knowledge_graph/__init__.py
+-rw-r--r--   0        0        0      542 2024-04-20 17:06:04.948548 cognee-0.1.5/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py
+-rw-r--r--   0        0        0     1102 2024-04-25 09:42:30.767456 cognee-0.1.5/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py
+-rw-r--r--   0        0        0     4740 2024-04-25 22:16:19.641944 cognee-0.1.5/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py
+-rw-r--r--   0        0        0      638 2024-04-20 17:06:04.949628 cognee-0.1.5/cognee/modules/data/get_cognitive_layers.py
+-rw-r--r--   0        0        0      516 2024-04-20 17:06:04.949924 cognee-0.1.5/cognee/modules/data/get_content_categories.py
+-rw-r--r--   0        0        0      499 2024-04-20 17:06:04.950170 cognee-0.1.5/cognee/modules/data/get_content_summary.py
+-rw-r--r--   0        0        0      895 2024-04-20 17:06:04.950394 cognee-0.1.5/cognee/modules/data/get_layer_graphs.py
+-rw-r--r--   0        0        0       69 2024-03-30 11:42:14.111069 cognee-0.1.5/cognee/modules/discovery/__init__.py
+-rw-r--r--   0        0        0      756 2024-03-30 11:49:14.418639 cognee-0.1.5/cognee/modules/discovery/discover_directory_datasets.py
+-rw-r--r--   0        0        0       62 2024-03-29 12:58:54.570027 cognee-0.1.5/cognee/modules/ingestion/__init__.py
+-rw-r--r--   0        0        0     1763 2024-03-29 12:58:54.570193 cognee-0.1.5/cognee/modules/ingestion/add_data_to_dataset.py
+-rw-r--r--   0        0        0      490 2024-03-29 12:58:54.570428 cognee-0.1.5/cognee/modules/ingestion/classify.py
+-rw-r--r--   0        0        0      780 2024-04-21 19:39:20.100717 cognee-0.1.5/cognee/modules/ingestion/data_types/BinaryData.py
+-rw-r--r--   0        0        0      295 2024-04-21 19:33:23.824343 cognee-0.1.5/cognee/modules/ingestion/data_types/IngestionData.py
+-rw-r--r--   0        0        0      764 2024-04-21 19:38:38.394049 cognee-0.1.5/cognee/modules/ingestion/data_types/TextData.py
+-rw-r--r--   0        0        0      145 2024-03-13 17:10:40.359643 cognee-0.1.5/cognee/modules/ingestion/data_types/__init__.py
+-rw-r--r--   0        0        0      125 2024-03-13 17:10:40.359841 cognee-0.1.5/cognee/modules/ingestion/exceptions.py
+-rw-r--r--   0        0        0      275 2024-04-20 17:06:04.950837 cognee-0.1.5/cognee/modules/ingestion/identify.py
+-rw-r--r--   0        0        0      796 2024-03-29 12:58:54.571415 cognee-0.1.5/cognee/modules/ingestion/save.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.360307 cognee-0.1.5/cognee/modules/memory/__init__.py
+-rw-r--r--   0        0        0       55 2024-03-13 17:10:40.361059 cognee-0.1.5/cognee/modules/memory/vector/__init__.py
+-rw-r--r--   0        0        0      378 2024-03-13 17:10:40.361283 cognee-0.1.5/cognee/modules/memory/vector/create_vector_memory.py
+-rw-r--r--   0        0        0     1109 2024-04-20 17:06:04.951176 cognee-0.1.5/cognee/modules/search/CogneeSearch.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361325 cognee-0.1.5/cognee/modules/search/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361372 cognee-0.1.5/cognee/modules/search/graph/__init__.py
+-rw-r--r--   0        0        0     2083 2024-04-20 17:23:41.887212 cognee-0.1.5/cognee/modules/search/graph/search_adjacent.py
+-rw-r--r--   0        0        0     1869 2024-04-20 17:23:55.244065 cognee-0.1.5/cognee/modules/search/graph/search_categories.py
+-rw-r--r--   0        0        0     2976 2024-04-20 17:23:50.632849 cognee-0.1.5/cognee/modules/search/graph/search_neighbour.py
+-rw-r--r--   0        0        0     1747 2024-04-20 17:24:00.829943 cognee-0.1.5/cognee/modules/search/graph/search_summary.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361762 cognee-0.1.5/cognee/modules/search/vector/__init__.py
+-rw-r--r--   0        0        0     1579 2024-04-20 17:45:36.721313 cognee-0.1.5/cognee/modules/search/vector/search_similarity.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.362031 cognee-0.1.5/cognee/modules/users/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-13 17:10:40.362758 cognee-0.1.5/cognee/modules/users/memory/__init__.py
+-rw-r--r--   0        0        0      802 2024-03-13 17:10:40.362950 cognee-0.1.5/cognee/modules/users/memory/create_information_points.py
+-rw-r--r--   0        0        0      229 2024-03-13 17:10:40.363108 cognee-0.1.5/cognee/modules/users/memory/is_existing_memory.py
+-rw-r--r--   0        0        0      203 2024-03-13 17:10:40.363292 cognee-0.1.5/cognee/modules/users/memory/register_memory_for_user.py
+-rw-r--r--   0        0        0   124245 2024-04-21 08:54:54.214070 cognee-0.1.5/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json
+-rw-r--r--   0        0        0      182 2024-03-13 17:10:40.363716 cognee-0.1.5/cognee/root_dir.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.364048 cognee-0.1.5/cognee/shared/__init__.py
+-rw-r--r--   0        0        0     8633 2024-04-25 09:42:30.768854 cognee-0.1.5/cognee/shared/data_models.py
+-rw-r--r--   0        0        0      365 2024-03-22 15:50:27.366234 cognee-0.1.5/cognee/shared/encode_uuid.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.642031 cognee-0.1.5/cognee/tests/__init__.py
+-rw-r--r--   0        0        0      985 2024-04-25 22:16:19.642354 cognee-0.1.5/cognee/tests/test_data/Natural_language_processing.txt
+-rwxr-xr-x   0        0        0     5982 2024-04-25 22:16:19.642833 cognee-0.1.5/cognee/tests/test_library.py
+-rw-r--r--   0        0        0     9487 2024-04-25 22:16:19.643423 cognee-0.1.5/cognee/utils.py
+-rw-r--r--   0        0        0     3511 2024-04-25 22:16:30.618317 cognee-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7203 1970-01-01 00:00:00.000000 cognee-0.1.5/PKG-INFO
```

### Comparing `cognee-0.1.4/LICENSE` & `cognee-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/README.md` & `cognee-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/api/client.py` & `cognee-0.1.5/cognee/api/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """ FastAPI server for the Cognee API. """
+import os
 from uuid import UUID
 
+import aiohttp
 import uvicorn
 import logging
 
 # Set up logging
 logging.basicConfig(
     level=logging.INFO,  # Set the logging level (e.g., DEBUG, INFO, WARNING, ERROR, CRITICAL)
     format="%(asctime)s [%(levelname)s] %(message)s",  # Set the log message format
@@ -63,22 +65,45 @@
     query_params:  Dict[str, Any]
 @app.post("/add", response_model=dict)
 async def add(payload: AddPayload):
     """ This endpoint is responsible for adding data to the graph."""
     from v1.add.add import add
 
     try:
-        await add(
-            payload.data,
-            payload.dataset_name,
-        )
+        data = payload.data
+        if isinstance(data, str) and data.startswith('http'):
+            if 'github' in data:
+                # Perform git clone if the URL is from GitHub
+                repo_name = data.split('/')[-1].replace('.git', '')
+                os.system(f'git clone {data} .data/{repo_name}')
+                await add(
+                    "data://.data/",
+                    f"{repo_name}",
+                )
+            else:
+                # Fetch and store the data from other types of URL using curl
+                async with aiohttp.ClientSession() as session:
+                    async with session.get(data) as resp:
+                        if resp.status == 200:
+                            file_data = await resp.read()
+                            with open(f'.data/{data.split("/")[-1]}', 'wb') as f:
+                                f.write(file_data)
+                            await add(
+                                f"data://.data/",
+                                f"{data.split('/')[-1]}",
+                            )
+        else:
+            await add(
+                payload.data,
+                payload.dataset_name,
+            )
     except Exception as error:
         return JSONResponse(
             status_code = 409,
-            content = { "error": error }
+            content = { "error": str(error) }
         )
 
 @app.post("/cognify", response_model=dict)
 async def cognify(payload: CognifyPayload):
     """ This endpoint is responsible for the cognitive processing of the content."""
     from v1.cognify.cognify import cognify
```

### Comparing `cognee-0.1.4/cognee/api/v1/add/add.py` & `cognee-0.1.5/cognee/api/v1/add/add.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 import asyncio
 import dlt
 import duckdb
 import cognee.modules.ingestion as ingestion
 from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.files.storage import LocalStorage
 from cognee.modules.discovery import discover_directory_datasets
-
 from cognee.utils import send_telemetry
 
 
-
 async def add(data_path: Union[str, List[str]], dataset_name: str = None):
     if isinstance(data_path, str):
         # data_path is a data directory path
         if "data://" in data_path:
             return await add_data_directory(data_path.replace("data://", ""), dataset_name)
         # data_path is a file path
         if "file://" in data_path:
@@ -101,15 +99,15 @@
 
     run_info = pipeline.run(
         data_resources(processed_file_paths),
         table_name = "file_metadata",
         dataset_name = dataset_name.replace(" ", "_").replace(".", "_") if dataset_name is not None else "main_dataset",
         write_disposition = "merge",
     )
-    send_telemetry( "COGNEE_ADD")
+    send_telemetry("cognee.add")
 
     return run_info
 
 async def add_data_directory(data_path: str, dataset_name: str = None):
     datasets = discover_directory_datasets(data_path)
 
     results = []
```

### Comparing `cognee-0.1.4/cognee/api/v1/add/add_standalone.py` & `cognee-0.1.5/cognee/api/v1/add/add_standalone.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/api/v1/add/remember.py` & `cognee-0.1.5/cognee/api/v1/add/remember.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/api/v1/cognify/cognify.py` & `cognee-0.1.5/cognee/api/v1/cognify/cognify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 from uuid import uuid4
 from typing import List, Union
 import logging
 import instructor
+import nltk
 from openai import OpenAI
 from nltk.corpus import stopwords
 from cognee.config import Config
 from cognee.modules.cognify.graph.add_data_chunks import add_data_chunks
 from cognee.modules.cognify.graph.add_document_node import add_document_node
 from cognee.modules.cognify.graph.add_classification_nodes import add_classification_nodes
 from cognee.modules.cognify.graph.add_cognitive_layer_graphs import add_cognitive_layer_graphs
@@ -36,16 +37,21 @@
 USER_ID = "default_user"
 
 logger = logging.getLogger("cognify")
 
 async def cognify(datasets: Union[str, List[str]] = None):
     """This function is responsible for the cognitive processing of the content."""
     # Has to be loaded in advance, multithreading doesn't work without it.
+    nltk.download('stopwords', quiet=True)
     stopwords.ensure_loaded()
 
+    graph_db_type = infrastructure_config.get_config()["graph_engine"]
+
+    graph_client = await get_graph_client(graph_db_type)
+
     db_engine = infrastructure_config.get_config()["database_engine"]
 
     if datasets is None or len(datasets) == 0:
         datasets = db_engine.get_datasets()
 
     awaitables = []
 
@@ -63,20 +69,14 @@
     # datasets is a dataset name string
     dataset_name = datasets.replace(".", "_").replace(" ", "_")
 
     for added_dataset in added_datasets:
         if dataset_name in added_dataset:
             dataset_files.append((added_dataset, db_engine.get_files_metadata(added_dataset)))
 
-    awaitables = []
-
-    graph_db_type = infrastructure_config.get_config()["graph_engine"]
-
-    graph_client = await get_graph_client(graph_db_type)
-
     # await initialize_graph(USER_ID, graph_data_model, graph_client)
 
     data_chunks = {}
 
     chunk_engine = infrastructure_config.get_config()["chunk_engine"]
     chunk_strategy = infrastructure_config.get_config()["chunk_strategy"]
 
@@ -159,10 +159,10 @@
 
         await connect_nodes_in_graph(
             graph_client,
             relationships,
             score_threshold = infrastructure_config.get_config()["intra_layer_score_treshold"]
         )
 
-    send_telemetry( "COGNEE_COGNIFY")
+    send_telemetry("cognee.cognify")
 
     print(f"Chunk ({chunk_id}) cognified.")
```

### Comparing `cognee-0.1.4/cognee/api/v1/config/config.py` & `cognee-0.1.5/cognee/api/v1/config/config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/api/v1/datasets/datasets.py` & `cognee-0.1.5/cognee/api/v1/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/api/v1/prune/prune.py` & `cognee-0.1.5/cognee/api/v1/prune/prune.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/api/v1/search/search.py` & `cognee-0.1.5/cognee/api/v1/search/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     # Use asyncio.gather to run all scheduled tasks concurrently
     search_results = await asyncio.gather(*search_tasks)
 
     # Update the results set with the results from all tasks
     results.extend(search_results)
 
-    send_telemetry( "COGNEE_SEARCH")
+    send_telemetry("cognee.search")
 
     return results
 
 
 
 if __name__ == "__main__":
     async def main():
```

### Comparing `cognee-0.1.4/cognee/config.py` & `cognee-0.1.5/cognee/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
 
     system_root_directory = get_absolute_path(".cognee_system")
     data_root_directory = os.getenv("DATA_PATH", get_absolute_path(".data"))
 
     vectordb: str = os.getenv("VECTORDB", "weaviate")
 
-    qdrant_path: str = os.getenv("QDRANT_PATH")
-    qdrant_url: str = os.getenv("QDRANT_URL")
-    qdrant_api_key: str = os.getenv("QDRANT_API_KEY")
+    qdrant_path: str = os.getenv("QDRANT_PATH", None)
+    qdrant_url: str = os.getenv("QDRANT_URL", None)
+    qdrant_api_key: str = os.getenv("QDRANT_API_KEY", None)
 
     db_path = str = os.getenv("COGNEE_DB_PATH", "databases")
     db_name: str = os.getenv("DB_NAME", "cognee.db")
     db_host: str = os.getenv("DB_HOST", "localhost")
     db_port: str = os.getenv("DB_PORT", "5432")
     db_user: str = os.getenv("DB_USER", "cognee")
     db_password: str = os.getenv("DB_PASSWORD", "cognee")
```

### Comparing `cognee-0.1.4/cognee/fetch_secret.py` & `cognee-0.1.5/cognee/fetch_secret.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/InfrastructureConfig.py` & `cognee-0.1.5/cognee/infrastructure/InfrastructureConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,17 +90,14 @@
 
                 self.vector_engine = WeaviateAdapter(
                     config.weaviate_url,
                     config.weaviate_api_key,
                     embedding_engine = self.embedding_engine
                 )
             except (EnvironmentError, ModuleNotFoundError):
-                if config.qdrant_url is None and config.qdrant_api_key is None:
-                    raise EnvironmentError("Qdrant is not configured!")
-
                 self.vector_engine = QDrantAdapter(
                     qdrant_url = config.qdrant_url,
                     qdrant_api_key = config.qdrant_api_key,
                     embedding_engine = self.embedding_engine
                 )
 
         if (config_entity is None or config_entity == "database_directory_path") and self.database_directory_path is None:
```

### Comparing `cognee-0.1.4/cognee/infrastructure/data/chunking/DefaultChunkEngine.py` & `cognee-0.1.5/cognee/infrastructure/data/chunking/DefaultChunkEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/data/models/Data.py` & `cognee-0.1.5/cognee/infrastructure/data/models/Data.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/data/models/Dataset.py` & `cognee-0.1.5/cognee/infrastructure/data/models/Dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/data/models/DatasetData.py` & `cognee-0.1.5/cognee/infrastructure/data/models/DatasetData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/data/utils/extract_keywords.py` & `cognee-0.1.5/cognee/infrastructure/data/utils/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/graph/get_graph_client.py` & `cognee-0.1.5/cognee/infrastructure/databases/graph/get_graph_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,9 +23,12 @@
                 graph_database_username = config.graph_database_username,
                 graph_database_password = config.graph_database_password
             )
         except:
             pass
             
     graph_client = NetworkXAdapter(filename = graph_file_path)
-    await graph_client.load_graph_from_file()
+
+    if (graph_client.graph is None):
+        await graph_client.load_graph_from_file()
+
     return graph_client
```

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/graph/graph_db_interface.py` & `cognee-0.1.5/cognee/infrastructure/databases/graph/graph_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py` & `cognee-0.1.5/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/graph/networkx/adapter.py` & `cognee-0.1.5/cognee/infrastructure/databases/graph/networkx/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             cls._instance.filename = filename
         return cls._instance
 
     def __init__(self, filename = "cognee_graph.pkl"):
         self.filename = filename
-        self.graph = nx.MultiDiGraph()
 
     async def graph(self):
         return self.graph
 
     async def add_node(
         self,
         node_id: str,
@@ -109,35 +108,40 @@
         graph_data = nx.readwrite.json_graph.node_link_data(self.graph)
 
         async with aiofiles.open(file_path, "w") as file:
             await file.write(json.dumps(graph_data))
 
     async def load_graph_from_file(self, file_path: str = None):
         """Asynchronously load the graph from a file in JSON format."""
+        if file_path == self.filename:
+            return
+
         if not file_path:
             file_path = self.filename
         try:
             if os.path.exists(file_path):
                 async with aiofiles.open(file_path, "r") as file:
                     graph_data = json.loads(await file.read())
                     self.graph = nx.readwrite.json_graph.node_link_graph(graph_data)
-                    return self.graph
             else:
                 # Log that the file does not exist and an empty graph is initialized
                 logger.warning("File %s not found. Initializing an empty graph.", file_path)
                 self.graph = nx.MultiDiGraph()  # Use MultiDiGraph to keep it consistent with __init__
-                return self.graph
+                await self.save_graph_to_file(file_path)
         except Exception as error:
             logger.error("Failed to load graph from file: %s", file_path)
             # Initialize an empty graph in case of error
             self.graph = nx.MultiDiGraph()
-            return self.graph
+            await self.save_graph_to_file(file_path)
 
-    async def delete_graph(self, path: str = None):
+    async def delete_graph(self, file_path: str = None):
         """Asynchronously delete the graph file from the filesystem."""
-        if path is None:
-            path = self.filename  # Assuming self.filename is defined elsewhere and holds the default graph file path
+        if file_path is None:
+            file_path = self.filename  # Assuming self.filename is defined elsewhere and holds the default graph file path
         try:
-            await aiofiles_os.remove(path)
+            if os.path.exists(file_path):
+                await aiofiles_os.remove(file_path)
+
+            self.graph = None
             logger.info("Graph deleted successfully.")
         except Exception as error:
             logger.error("Failed to delete graph: %s", error)
```

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py` & `cognee-0.1.5/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/relational/relational_db_interface.py` & `cognee-0.1.5/cognee/infrastructure/databases/relational/relational_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py` & `cognee-0.1.5/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/relational/utils/with_rollback.py` & `cognee-0.1.5/cognee/infrastructure/databases/relational/utils/with_rollback.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py` & `cognee-0.1.5/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py` & `cognee-0.1.5/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,45 +39,56 @@
             self.qdrant_url = qdrant_url
 
         self.qdrant_api_key = qdrant_api_key
 
     def get_qdrant_client(self) -> AsyncQdrantClient:
         if self.qdrant_path is not None:
             return AsyncQdrantClient(
-                path = self.qdrant_path,
+                path = self.qdrant_path, port=6333
             )
         elif self.qdrant_url is not None:
             return AsyncQdrantClient(
                 url = self.qdrant_url,
                 api_key = self.qdrant_api_key,
+                port = 6333
             )
 
         return AsyncQdrantClient(
             location = ":memory:"
         )
 
     async def embed_data(self, data: List[str]) -> List[float]:
         return await self.embedding_engine.embed_text(data)
 
+    async def collection_exists(self, collection_name: str) -> bool:
+        client = self.get_qdrant_client()
+        result = await client.collection_exists(collection_name)
+        await client.close()
+        return result
+
     async def create_collection(
       self,
       collection_name: str,
     ):
         client = self.get_qdrant_client()
 
-        return await client.create_collection(
+        result = await client.create_collection(
             collection_name = collection_name,
             vectors_config = {
                 "text": models.VectorParams(
                     size = self.embedding_engine.get_vector_size(),
                     distance = "Cosine"
                 )
             }
         )
 
+        await client.close()
+
+        return result
+
     async def create_data_points(self, collection_name: str, data_points: List[DataPoint]):
         client = self.get_qdrant_client()
 
         data_vectors = await self.embed_data([data_point.get_embeddable_data() for data_point in data_points])
 
         def convert_to_qdrant_point(data_point: DataPoint):
             return models.PointStruct(
@@ -86,21 +97,27 @@
                 vector = {
                     "text": data_vectors[data_points.index(data_point)]
                 }
             )
 
         points = [convert_to_qdrant_point(point) for point in data_points]
 
-        return await client.upload_points(
+        result = await client.upload_points(
             collection_name = collection_name,
             points = points
         )
 
+        await client.close()
+
+        return result
+
     async def retrieve(self, collection_name: str, data_id: str):
-        results = await self.get_qdrant_client().retrieve(collection_name, [data_id], with_payload = True)
+        client = await self.get_qdrant_client()
+        results = client.retrieve(collection_name, [data_id], with_payload = True)
+        await client.close()
         return results[0] if len(results) > 0 else None
 
     async def search(
         self,
         collection_name: str,
         query_text: Optional[str] = None,
         query_vector: Optional[List[float]] = None,
@@ -108,24 +125,28 @@
         with_vector: bool = False
     ):
         if query_text is None and query_vector is None:
             raise ValueError("One of query_text or query_vector must be provided!")
 
         client = self.get_qdrant_client()
 
-        return await client.search(
+        result = await client.search(
             collection_name = collection_name,
             query_vector = models.NamedVector(
                 name = "text",
                 vector = query_vector if query_vector is not None else (await self.embed_data([query_text]))[0],
             ),
             limit = limit,
             with_vectors = with_vector
         )
 
+        await client.close()
+
+        return result
+
 
     async def batch_search(self, collection_name: str, query_texts: List[str], limit: int = None, with_vectors: bool = False):
         """
         Perform batch search in a Qdrant collection with dynamic search requests.
 
         Args:
         - collection_name (str): Name of the collection to search in.
@@ -155,16 +176,20 @@
 
         # Perform batch search with the dynamically generated requests
         results = await client.search_batch(
             collection_name = collection_name,
             requests = requests
         )
 
+        await client.close()
+
         return [filter(lambda result: result.score > 0.9, result_group) for result_group in results]
 
     async def prune(self):
         client = self.get_qdrant_client()
 
         response = await client.get_collections()
 
         for collection in response.collections:
             await client.delete_collection(collection.name)
+
+        await client.close()
```

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/vector/vector_db_interface.py` & `cognee-0.1.5/cognee/infrastructure/databases/vector/vector_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py` & `cognee-0.1.5/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,22 @@
             # },
             additional_config=wvc.init.AdditionalConfig(timeout=wvc.init.Timeout(init=30))
         )
 
     async def embed_data(self, data: List[str]) -> List[float]:
         return await self.embedding_engine.embed_text(data)
 
+    async def collection_exists(self, collection_name: str) -> bool:
+        event_loop = asyncio.get_event_loop()
+
+        def sync_collection_exists():
+            return self.client.collections.exists(collection_name)
+
+        return await event_loop.run_in_executor(None, sync_collection_exists)
+
     async def create_collection(self, collection_name: str):
         import weaviate.classes.config as wvcc
 
         event_loop = asyncio.get_event_loop()
 
         def sync_create_collection():
             return self.client.collections.create(
```

### Comparing `cognee-0.1.4/cognee/infrastructure/files/storage/LocalStorage.py` & `cognee-0.1.5/cognee/infrastructure/files/storage/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/files/storage/StorageManager.py` & `cognee-0.1.5/cognee/infrastructure/files/storage/StorageManager.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/files/utils/get_file_metadata.py` & `cognee-0.1.5/cognee/infrastructure/files/utils/get_file_metadata.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/files/utils/guess_file_type.py` & `cognee-0.1.5/cognee/infrastructure/files/utils/guess_file_type.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/files/utils/is_text_content.py` & `cognee-0.1.5/cognee/infrastructure/files/utils/is_text_content.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/llm/anthropic/adapter.py` & `cognee-0.1.5/cognee/infrastructure/llm/anthropic/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/llm/generic_llm_api/adapter.py` & `cognee-0.1.5/cognee/infrastructure/llm/generic_llm_api/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/llm/get_llm_client.py` & `cognee-0.1.5/cognee/infrastructure/llm/get_llm_client.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/llm/llm_interface.py` & `cognee-0.1.5/cognee/infrastructure/llm/llm_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/llm/openai/adapter.py` & `cognee-0.1.5/cognee/infrastructure/llm/openai/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/llm/prompts/classify_content.txt` & `cognee-0.1.5/cognee/infrastructure/llm/prompts/classify_content.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/llm/prompts/generate_cog_layers.txt` & `cognee-0.1.5/cognee/infrastructure/llm/prompts/generate_cog_layers.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt` & `cognee-0.1.5/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/llm/prompts/read_query_prompt.py` & `cognee-0.1.5/cognee/infrastructure/llm/prompts/read_query_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/llm/prompts/render_prompt.py` & `cognee-0.1.5/cognee/infrastructure/llm/prompts/render_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/infrastructure/pipeline/models/Operation.py` & `cognee-0.1.5/cognee/infrastructure/pipeline/models/Operation.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/dataset.py` & `cognee-0.1.5/cognee/modules/cognify/dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/evaluate.py` & `cognee-0.1.5/cognee/modules/cognify/evaluate.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/graph/add_classification_nodes.py` & `cognee-0.1.5/cognee/modules/cognify/graph/add_classification_nodes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 async def add_classification_nodes(graph_client, parent_node_id: str, categories: List) -> None:
     for category in categories:
-        data_type = category["data_type"].upper().replace(' ', '_')
-        category_name = category["category_name"].upper().replace(' ', '_').replace("'", "").replace("/", "_")
+        data_type = category["data_type"].upper().replace(" ", "_")
+        category_name = category["category_name"].upper().replace(" ", "_").replace("'", "").replace("/", "_")
 
         data_type_node_id = f"DATA_TYPE__{data_type}"
 
         data_type_node = await graph_client.extract_node(data_type_node_id)
 
         if not data_type_node:
             data_type_node = await graph_client.add_node(data_type_node_id, dict(name = data_type, entity_type = "DataType"))
```

### Comparing `cognee-0.1.4/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py` & `cognee-0.1.5/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/graph/add_cognitive_layers.py` & `cognee-0.1.5/cognee/modules/cognify/graph/add_cognitive_layers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+""" This module adds cognitive layers to the graph. """
 from typing import List
+import re
 
 async def add_cognitive_layers(graph_client, parent_node_id: str, cognitive_layers: List):
     cognitive_layer_nodes = [(
         generate_cognitive_layer_id(cognitive_layer.name),
         dict(
             id = generate_cognitive_layer_id(cognitive_layer.name),
             name = cognitive_layer.name,
@@ -16,9 +18,16 @@
         cognitive_layer_id,
         "decomposed_as",
         dict(relationship_name = "decomposed_as"),
     ) for (cognitive_layer_id, _) in cognitive_layer_nodes)
 
     return cognitive_layer_nodes
 
+
+def fix_layer_name(layer_name):
+    sanitized_name = re.sub(r'[^a-zA-Z0-9_]', '', layer_name)
+    return sanitized_name
+
+
 def generate_cognitive_layer_id(layer_id: str) -> str:
-    return f"COGNITIVE_LAYER__{layer_id.upper().replace(' ', '_')}".replace("'", "").replace("/", "_")
+    layer = f"COGNITIVE_LAYER__{layer_id.upper().replace(' ', '_')}".replace("'", "").replace("/", "_")
+    return fix_layer_name(layer)
```

### Comparing `cognee-0.1.4/cognee/modules/cognify/graph/add_data_chunks.py` & `cognee-0.1.5/cognee/modules/cognify/graph/add_data_chunks.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from typing import TypedDict
 from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.databases.vector import DataPoint
 
 class TextChunk(TypedDict):
     text: str
     chunk_id: str
@@ -10,14 +11,16 @@
 async def add_data_chunks(dataset_data_chunks: dict[str, list[TextChunk]]):
     vector_client = infrastructure_config.get_config("vector_engine")
 
     identified_chunks = []
 
     for (dataset_name, chunks) in dataset_data_chunks.items():
         try:
+        # if not await vector_client.collection_exists(dataset_name):
+        #     logging.error(f"Creating collection {str(dataset_name)}")
             await vector_client.create_collection(dataset_name)
         except Exception:
             pass
 
         dataset_chunks = [
             dict(
                 chunk_id = chunk["chunk_id"],
@@ -25,19 +28,33 @@
                 text = chunk["text"],
                 file_metadata = chunk["file_metadata"],
             ) for chunk in chunks
         ]
 
         identified_chunks.extend(dataset_chunks)
 
-        await vector_client.create_data_points(
-            dataset_name,
-            [
-                DataPoint(
-                    id = chunk["chunk_id"],
-                    payload = dict(text = chunk["text"]),
-                    embed_field = "text"
-                ) for chunk in dataset_chunks
-            ],
-        )
+        # if not await vector_client.collection_exists(dataset_name):
+        try:
+            logging.error("Collection still not found. Creating collection again.")
+            await vector_client.create_collection(dataset_name)
+        except:
+            pass
+
+        async def create_collection_retry(dataset_name, dataset_chunks):
+            await vector_client.create_data_points(
+                dataset_name,
+                [
+                    DataPoint(
+                        id = chunk["chunk_id"],
+                        payload = dict(text = chunk["text"]),
+                        embed_field = "text"
+                    ) for chunk in dataset_chunks
+                ],
+            )
+
+        try:
+            await create_collection_retry(dataset_name, dataset_chunks)
+        except Exception:
+            logging.error("Collection not found in create data points.")
+            await create_collection_retry(dataset_name, dataset_chunks)
 
     return identified_chunks
```

### Comparing `cognee-0.1.4/cognee/modules/cognify/graph/add_document_node.py` & `cognee-0.1.5/cognee/modules/cognify/graph/add_document_node.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/graph/add_label_nodes.py` & `cognee-0.1.5/cognee/modules/cognify/graph/add_label_nodes.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/graph/add_node_connections.py` & `cognee-0.1.5/cognee/modules/cognify/graph/add_node_connections.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/graph/add_summary_nodes.py` & `cognee-0.1.5/cognee/modules/cognify/graph/add_summary_nodes.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/graph/create.py` & `cognee-0.1.5/cognee/modules/cognify/graph/create.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/graph/initialize_graph.py` & `cognee-0.1.5/cognee/modules/cognify/graph/initialize_graph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/llm/resolve_cross_graph_references.py` & `cognee-0.1.5/cognee/modules/cognify/llm/resolve_cross_graph_references.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/test.py` & `cognee-0.1.5/cognee/modules/cognify/test.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/cognify/train.py` & `cognee-0.1.5/cognee/modules/cognify/train.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/data/extraction/extract_categories.py` & `cognee-0.1.5/cognee/modules/data/extraction/extract_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py` & `cognee-0.1.5/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py` & `cognee-0.1.5/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py` & `cognee-0.1.5/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 class ExtractKnowledgeGraph(dspy.Module):
     def __init__(self, lm = dspy.OpenAI(model = config.openai_model, api_key = config.openai_key, model_type = "chat", max_tokens = 4096)):
         super().__init__()
         self.lm = lm
         dspy.settings.configure(lm=self.lm)
         self.generate_graph = dspy.TypedChainOfThought(GraphFromText)
-        nltk.download('stopwords')
+        nltk.download("stopwords", quiet = True)
 
     def forward(self, context: str, question: str):
         context = remove_stop_words(context)
         context = trim_text_to_max_tokens(context, 1500, config.openai_model)
       
         with dspy.context(lm = self.lm):
             graph = self.generate_graph(text = context).graph
```

### Comparing `cognee-0.1.4/cognee/modules/data/get_cognitive_layers.py` & `cognee-0.1.5/cognee/modules/data/get_cognitive_layers.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/data/get_content_categories.py` & `cognee-0.1.5/cognee/modules/data/get_content_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/data/get_layer_graphs.py` & `cognee-0.1.5/cognee/modules/data/get_layer_graphs.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/discovery/discover_directory_datasets.py` & `cognee-0.1.5/cognee/modules/discovery/discover_directory_datasets.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/ingestion/add_data_to_dataset.py` & `cognee-0.1.5/cognee/modules/ingestion/add_data_to_dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/ingestion/data_types/BinaryData.py` & `cognee-0.1.5/cognee/modules/ingestion/data_types/BinaryData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/ingestion/data_types/TextData.py` & `cognee-0.1.5/cognee/modules/ingestion/data_types/TextData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/ingestion/save.py` & `cognee-0.1.5/cognee/modules/ingestion/save.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/search/CogneeSearch.py` & `cognee-0.1.5/cognee/modules/search/CogneeSearch.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/search/graph/search_adjacent.py` & `cognee-0.1.5/cognee/modules/search/graph/search_adjacent.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/search/graph/search_categories.py` & `cognee-0.1.5/cognee/modules/search/graph/search_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/search/graph/search_neighbour.py` & `cognee-0.1.5/cognee/modules/search/graph/search_neighbour.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/search/graph/search_summary.py` & `cognee-0.1.5/cognee/modules/search/graph/search_summary.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/search/vector/search_similarity.py` & `cognee-0.1.5/cognee/modules/search/vector/search_similarity.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/modules/users/memory/create_information_points.py` & `cognee-0.1.5/cognee/modules/users/memory/create_information_points.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json` & `cognee-0.1.5/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/shared/data_models.py` & `cognee-0.1.5/cognee/shared/data_models.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.4/cognee/tests/test_library.py` & `cognee-0.1.5/cognee/tests/test_library.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-
 async def  main():
     from os import path
-    from cognee import config, prune
-
-    data_directory_path = path.abspath("../.data")
-    config.data_root_directory(data_directory_path)
-
-    cognee_directory_path = path.abspath("../.cognee_system")
-    config.system_root_directory(cognee_directory_path)
-
-    await prune.prune_system()
-    from os import path
+    import pathlib
     import cognee
 
-    dataset_name = "explanations"
-    await cognee.add([path.abspath("../cognee/.test_data/Natural language processing.txt")], dataset_name)
-
+    print("Working dir: ", str(pathlib.Path(__file__).parent))
+    data_directory_path = str(pathlib.Path(path.join(pathlib.Path(__file__).parent, "../../.data")).resolve())
+    print("Data dir: ", data_directory_path)
+    cognee.config.data_root_directory(data_directory_path)
+
+    cognee_directory_path = str(pathlib.Path(path.join(pathlib.Path(__file__).parent, "../../.cognee_system")).resolve())
+    print("System dir: ", cognee_directory_path)
+    cognee.config.system_root_directory(cognee_directory_path)
+
+    await cognee.prune.prune_system()
+
+    dataset_name = "cs_explanations"
+    explanation_file_path = path.join(pathlib.Path(__file__).parent, "test_data/Natural_language_processing.txt")
+    await cognee.add([explanation_file_path], dataset_name)
+    
     dataset_name = "short_stories"
     # data_directory_path is defined above
     await cognee.add("data://" + data_directory_path, dataset_name)
 
     text_1 = """A quantum computer is a computer that takes advantage of quantum mechanical phenomena.
     At small scales, physical matter exhibits properties of both particles and waves, and quantum computing leverages this behavior, specifically quantum superposition and entanglement, using specialized hardware that supports the preparation and manipulation of quantum states.
     Classical physics cannot explain the operation of these quantum devices, and a scalable quantum computer could perform some calculations exponentially faster (with respect to input size scaling) than any modern "classical" computer. In particular, a large-scale quantum computer could break widely used encryption schemes and aid physicists in performing physical simulations; however, the current state of the technology is largely experimental and impractical, with several obstacles to useful applications. Moreover, scalable quantum computers do not hold promise for many practical tasks, and for many important tasks quantum speedups are proven impossible.
@@ -30,24 +32,23 @@
 
     text_2 = """A large language model (LLM) is a language model notable for its ability to achieve general-purpose language generation and other natural language processing tasks such as classification. LLMs acquire these abilities by learning statistical relationships from text documents during a computationally intensive self-supervised and semi-supervised training process. LLMs can be used for text generation, a form of generative AI, by taking an input text and repeatedly predicting the next token or word.
     LLMs are artificial neural networks. The largest and most capable, as of March 2024, are built with a decoder-only transformer-based architecture while some recent implementations are based on other architectures, such as recurrent neural network variants and Mamba (a state space model).
     Up to 2020, fine tuning was the only way a model could be adapted to be able to accomplish specific tasks. Larger sized models, such as GPT-3, however, can be prompt-engineered to achieve similar results.[6] They are thought to acquire knowledge about syntax, semantics and "ontology" inherent in human language corpora, but also inaccuracies and biases present in the corpora.
     Some notable LLMs are OpenAI's GPT series of models (e.g., GPT-3.5 and GPT-4, used in ChatGPT and Microsoft Copilot), Google's PaLM and Gemini (the latter of which is currently used in the chatbot of the same name), xAI's Grok, Meta's LLaMA family of open-source models, Anthropic's Claude models, Mistral AI's open source models, and Databricks' open source DBRX.
     """
 
-    dataset_name = "explanations"
+
+    dataset_name = "cs_explanations"
     await cognee.add(
         [
             text_1,
             text_2
         ],
         dataset_name
     )
 
-    graph = await cognee.cognify(dataset_name)
+    await cognee.cognify(["short_stories", "cs_explanations"])
 
 
 if __name__ == "__main__":
     import asyncio
     asyncio.run(main())
-
-
```

### Comparing `cognee-0.1.4/cognee/utils.py` & `cognee-0.1.5/cognee/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 """ This module contains utility functions for the cognee. """
 
 import os
+import uuid
+import datetime
 import graphistry
 import networkx as nx
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import tiktoken
 import nltk
 from posthog import Posthog
 
 from cognee.config import Config
-import uuid
-import datetime
 
 config = Config()
 config.load()
 
 
-def send_telemetry( posthog, event_name="COGNEE_ADD"):
+def send_telemetry(event_name: str):
     if os.getenv("TELEMETRY_DISABLED"):
         return
 
-    posthog = Posthog(project_api_key='phc_bbR86N876kwub62Lr3dhQ7zIeRyMMMm0fxXqxPqzLm3',
-                      host='https://eu.i.posthog.com')
+    env = os.getenv("ENV")
+    if env in ["local", "test", "dev"]:
+        return
+
+    posthog = Posthog(
+        project_api_key = "phc_bbR86N876kwub62Lr3dhQ7zIeRyMMMm0fxXqxPqzLm3",
+        host="https://eu.i.posthog.com"
+    )
 
     user_id = str(uuid.uuid4())
     current_time = datetime.datetime.now()
     properties = {
-        "time": current_time.strftime('%m/%d/%Y')
-
+        "time": current_time.strftime("%m/%d/%Y")
     }
 
     try:
         posthog.capture(user_id, event_name, properties)
     except Exception as e:
-        print('ERROR sending telemetric data to Posthog. See exception: %s', e)
+        print("ERROR sending telemetric data to Posthog. See exception: %s", e)
+
 def get_document_names(doc_input):
     """
     Get a list of document names.
 
     This function takes doc_input, which can be a folder path,
     a single document file path, or a document name as a string.
     It returns a list of document names based on the doc_input.
@@ -210,26 +216,26 @@
 
 def sanitize_df(df):
     """Replace NaNs and infinities in a DataFrame with None, making it JSON compliant."""
     return df.replace([np.inf, -np.inf, np.nan], None)
 
 
 def get_entities(tagged_tokens):
-    nltk.download("maxent_ne_chunker")
+    nltk.download("maxent_ne_chunker", quiet=True)
     from nltk.chunk import ne_chunk
     return ne_chunk(tagged_tokens)
 
 
 def extract_pos_tags(sentence):
     """Extract Part-of-Speech (POS) tags for words in a sentence."""
 
     # Ensure that the necessary NLTK resources are downloaded
-    nltk.download("words")
-    nltk.download("punkt")
-    nltk.download("averaged_perceptron_tagger")
+    nltk.download("words", quiet=True)
+    nltk.download("punkt", quiet=True)
+    nltk.download("averaged_perceptron_tagger", quiet=True)
 
     from nltk.tag import pos_tag
     from nltk.tokenize import word_tokenize
 
     # Tokenize the sentence into words
     tokens = word_tokenize(sentence)
 
@@ -258,15 +264,15 @@
     text (str): The text to analyze.
 
     Returns:
     dict: A dictionary containing the polarity scores for the text.
     """
     from nltk.sentiment import SentimentIntensityAnalyzer
 
-    nltk.download("vader_lexicon")
+    nltk.download("vader_lexicon", quiet=True)
 
     # Initialize the VADER Sentiment Intensity Analyzer
     sia = SentimentIntensityAnalyzer()
 
     # Obtain the polarity scores for the text
     polarity_scores = sia.polarity_scores(text)
```

### Comparing `cognee-0.1.4/pyproject.toml` & `cognee-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognee"
-version = "0.1.4"
+version = "0.1.5"
 description = "Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning."
 authors = ["Vasilije Markovic", "Boris Arzentar"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.cognee.ai"
 repository = "https://github.com/topoteretes/cognee"
 classifiers = [
@@ -40,15 +40,15 @@
 ruff = "^0.2.2"
 filetype = "^1.2.0"
 nltk = "^3.8.1"
 dlt = "^0.4.7"
 duckdb = {version = "^0.10.0", extras = ["dlt"]}
 overrides = "^7.7.0"
 aiofiles = "^23.2.1"
-qdrant-client = "^1.8.0"
+qdrant-client = "^1.9.0"
 duckdb-engine = "^0.11.2"
 graphistry = "^0.33.5"
 tenacity = "^8.2.3"
 weaviate-client = "^4.5.4"
 scikit-learn = "^1.4.1.post1"
 fastembed = "^0.2.5"
 pypdf = "^4.1.0"
@@ -58,14 +58,15 @@
 jinja2 = "^3.1.3"
 matplotlib = "^3.8.3"
 nest-asyncio = "^1.6.0"
 structlog = "^24.1.0"
 tiktoken = "^0.6.0"
 dspy-ai = "2.4.3"
 posthog = "^3.5.0"
+lancedb = "^0.6.10"
 
 
 [tool.poetry.extras]
 dbt = ["dbt-core", "dbt-redshift", "dbt-bigquery", "dbt-duckdb", "dbt-snowflake", "dbt-athena-community", "dbt-databricks"]
 gcp = ["grpcio", "google-cloud-bigquery", "db-dtypes", "gcsfs"]
 # bigquery is alias on gcp extras
 bigquery = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes", "gcsfs"]
```

### Comparing `cognee-0.1.4/PKG-INFO` & `cognee-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognee
-Version: 0.1.4
+Version: 0.1.5
 Summary: Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning.
 Home-page: https://www.cognee.ai
 License: Apache-2.0
 Author: Vasilije Markovic
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -55,29 +55,30 @@
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: graphistry (>=0.33.5,<0.34.0)
 Requires-Dist: graphviz (>=0.20.1,<0.21.0)
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: instructor (==1.2.1)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: lancedb (>=0.6.10,<0.7.0) ; extra == "lancedb"
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra == "neo4j"
 Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (==1.14.3)
 Requires-Dist: overrides (>=7.7.0,<8.0.0) ; extra == "notebook"
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: posthog (>=3.5.0,<4.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra == "bigquery" or extra == "parquet" or extra == "motherduck" or extra == "athena" or extra == "synapse"
 Requires-Dist: pydantic (>=2.5.0,<3.0.0)
 Requires-Dist: pylint (>=3.0.3,<4.0.0)
 Requires-Dist: pypdf (>=4.1.0,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.1)
-Requires-Dist: qdrant-client (>=1.8.0,<2.0.0)
+Requires-Dist: qdrant-client (>=1.9.0,<2.0.0)
 Requires-Dist: ruff (>=0.2.2,<0.3.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: uvicorn (==0.22.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognee Version: 0.1.4 Summary: Cognee - is a
+Metadata-Version: 2.1 Name: cognee Version: 0.1.5 Summary: Cognee - is a
 library for enriching LLM context with a semantic layer for better
 understanding and reasoning. Home-page: https://www.cognee.ai License: Apache-
 2.0 Author: Vasilije Markovic Requires-Python: >=3.9.0,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
@@ -23,25 +23,26 @@
 (>=0.4.7,<0.5.0) Requires-Dist: dspy-ai (==2.4.3) Requires-Dist: duckdb-engine
 (>=0.11.2,<0.12.0) Requires-Dist: duckdb[dlt] (>=0.10.0,<0.11.0) ; extra ==
 "duckdb" or extra == "motherduck" Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: fastembed (>=0.2.5,<0.3.0) Requires-Dist: filetype
 (>=1.2.0,<2.0.0) Requires-Dist: graphistry (>=0.33.5,<0.34.0) Requires-Dist:
 graphviz (>=0.20.1,<0.21.0) Requires-Dist: greenlet (>=3.0.3,<4.0.0) Requires-
 Dist: gunicorn (>=20.1.0,<21.0.0) Requires-Dist: instructor (==1.2.1) Requires-
-Dist: jinja2 (>=3.1.3,<4.0.0) Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
-Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra == "neo4j" Requires-Dist: nest-
-asyncio (>=1.6.0,<2.0.0) Requires-Dist: networkx (>=3.2.1,<4.0.0) Requires-
-Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist: openai (==1.14.3) Requires-Dist:
-overrides (>=7.7.0,<8.0.0) ; extra == "notebook" Requires-Dist: pandas
-(>=2.2.0,<3.0.0) Requires-Dist: posthog (>=3.5.0,<4.0.0) Requires-Dist: pyarrow
+Dist: jinja2 (>=3.1.3,<4.0.0) Requires-Dist: lancedb (>=0.6.10,<0.7.0) ; extra
+== "lancedb" Requires-Dist: matplotlib (>=3.8.3,<4.0.0) Requires-Dist: neo4j
+(>=5.18.0,<6.0.0) ; extra == "neo4j" Requires-Dist: nest-asyncio
+(>=1.6.0,<2.0.0) Requires-Dist: networkx (>=3.2.1,<4.0.0) Requires-Dist: nltk
+(>=3.8.1,<4.0.0) Requires-Dist: openai (==1.14.3) Requires-Dist: overrides
+(>=7.7.0,<8.0.0) ; extra == "notebook" Requires-Dist: pandas (>=2.2.0,<3.0.0)
+Requires-Dist: posthog (>=3.5.0,<4.0.0) Requires-Dist: pyarrow
 (>=15.0.0,<16.0.0) ; extra == "bigquery" or extra == "parquet" or extra ==
 "motherduck" or extra == "athena" or extra == "synapse" Requires-Dist: pydantic
 (>=2.5.0,<3.0.0) Requires-Dist: pylint (>=3.0.3,<4.0.0) Requires-Dist: pypdf
 (>=4.1.0,<5.0.0) Requires-Dist: python-dotenv (==1.0.1) Requires-Dist: qdrant-
-client (>=1.8.0,<2.0.0) Requires-Dist: ruff (>=0.2.2,<0.3.0) Requires-Dist:
+client (>=1.9.0,<2.0.0) Requires-Dist: ruff (>=0.2.2,<0.3.0) Requires-Dist:
 scikit-learn (>=1.4.1.post1,<2.0.0) Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0) Requires-Dist: tenacity
 (>=8.2.3,<9.0.0) Requires-Dist: tiktoken (>=0.6.0,<0.7.0) Requires-Dist:
 uvicorn (==0.22.0) Requires-Dist: weaviate-client (>=4.5.4,<5.0.0) ; extra ==
 "weaviate" Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-URL: Repository,
 https://github.com/topoteretes/cognee Description-Content-Type: text/markdown #
 cognee Deterministic LLMs Outputs for AI Engineers using graphs, LLMs and
```

