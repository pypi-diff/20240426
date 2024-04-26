# Comparing `tmp/kgdata-7.0.0.tar.gz` & `tmp/kgdata-7.0.1.tar.gz`

## Comparing `kgdata-7.0.0.tar` & `kgdata-7.0.1.tar`

### file list

```diff
@@ -1,177 +1,181 @@
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 kgdata-7.0.0/Cargo.toml
--rw-r--r--   0     1001      127    56429 2024-03-28 22:37:14.000000 kgdata-7.0.0/Cargo.lock
--rw-r--r--   0     1001      127     1064 2024-03-28 22:37:14.000000 kgdata-7.0.0/LICENSE
--rw-r--r--   0     1001      127      839 2024-03-28 22:37:14.000000 kgdata-7.0.0/README.md
--rw-r--r--   0     1001      127    33619 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/conversions.rs
--rw-r--r--   0     1001      127     2536 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/interface.rs
--rw-r--r--   0     1001      127     4415 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/mod.rs
--rw-r--r--   0     1001      127     6266 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/predefined_db.rs
--rw-r--r--   0     1001      127     4987 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/readonly_rocksdb_dict.rs
--rw-r--r--   0     1001      127     6211 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/remotedb/ipcserde.rs
--rw-r--r--   0     1001      127      926 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/remotedb/mod.rs
--rw-r--r--   0     1001      127     6376 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/remotedb/nngserver.rs
--rw-r--r--   0     1001      127    11896 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/remotedb/remote_rocksdb_dict.rs
--rw-r--r--   0     1001      127     2177 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/remotedb/request.rs
--rw-r--r--   0     1001      127     6487 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/remotedb/response.rs
--rw-r--r--   0     1001      127     8671 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/remotedb/shmemhelper.rs
--rw-r--r--   0     1001      127     2842 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/db/remotedb/zeromqserver.rs
--rw-r--r--   0     1001      127     1648 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/error.rs
--rw-r--r--   0     1001      127      662 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/lib.rs
--rw-r--r--   0     1001      127      732 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/main.rs
--rw-r--r--   0     1001      127     2566 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/mapreduce/dataset.rs
--rw-r--r--   0     1001      127      580 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/mapreduce/filterop.rs
--rw-r--r--   0     1001      127      721 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/mapreduce/foldop.rs
--rw-r--r--   0     1001      127     2788 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/mapreduce/functions.rs
--rw-r--r--   0     1001      127     1188 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/mapreduce/mapop.rs
--rw-r--r--   0     1001      127      468 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/mapreduce/miscop.rs
--rw-r--r--   0     1001      127     4851 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/mapreduce/mod.rs
--rw-r--r--   0     1001      127      630 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/mapreduce/sortop.rs
--rw-r--r--   0     1001      127      534 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/models/class.rs
--rw-r--r--   0     1001      127     1936 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/models/entity.rs
--rw-r--r--   0     1001      127      248 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/models/entity_link.rs
--rw-r--r--   0     1001      127      426 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/models/entity_metadata.rs
--rw-r--r--   0     1001      127      686 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/models/kgns.rs
--rw-r--r--   0     1001      127      560 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/models/mod.rs
--rw-r--r--   0     1001      127      648 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/models/multilingual.rs
--rw-r--r--   0     1001      127     3434 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/models/property.rs
--rw-r--r--   0     1001      127     5919 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/models/value.rs
--rw-r--r--   0     1001      127      944 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/pyo3helper/hashbrown.rs
--rw-r--r--   0     1001      127     4371 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/pyo3helper/macros/list.rs
--rw-r--r--   0     1001      127     5848 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/pyo3helper/macros/map.rs
--rw-r--r--   0     1001      127     6339 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/pyo3helper/macros/mod.rs
--rw-r--r--   0     1001      127     2133 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/pyo3helper/macros/set.rs
--rw-r--r--   0     1001      127      784 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/pyo3helper/mod.rs
--rw-r--r--   0     1001      127      805 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/pyo3helper/strview.rs
--rw-r--r--   0     1001      127      682 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/pyo3helper/usizeview.rs
--rw-r--r--   0     1001      127       33 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/python/mod.rs
--rw-r--r--   0     1001      127     1286 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/python/models/class.rs
--rw-r--r--   0     1001      127      419 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/python/models/conversions.rs
--rw-r--r--   0     1001      127     2378 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/python/models/entity.rs
--rw-r--r--   0     1001      127     1133 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/python/models/entity_metadata.rs
--rw-r--r--   0     1001      127    10911 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/python/models/iterators.rs
--rw-r--r--   0     1001      127     1358 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/python/models/mod.rs
--rw-r--r--   0     1001      127     2433 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/python/models/multilingual.rs
--rw-r--r--   0     1001      127     1827 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/python/models/property.rs
--rw-r--r--   0     1001      127     8042 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/python/models/value.rs
--rw-r--r--   0     1001      127     7062 2024-03-28 22:37:14.000000 kgdata-7.0.0/src/python/scripts.rs
--rw-r--r--   0     1001      127     1555 2024-03-28 22:37:14.000000 kgdata-7.0.0/pyproject.toml
--rw-r--r--   0     1001      127     6044 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/core/models.pyi
--rw-r--r--   0     1001      127       27 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/core/__init__.pyi
--rw-r--r--   0     1001      127     1385 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/core/base.pyi
--rw-r--r--   0     1001      127        0 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/__init__.py
--rw-r--r--   0     1001      127    10033 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/db.py
--rw-r--r--   0     1001      127     3748 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/models/ont_class.py
--rw-r--r--   0     1001      127        0 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/models/__init__.py
--rw-r--r--   0     1001      127     3000 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/models/multilingual.py
--rw-r--r--   0     1001      127     4546 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/models/ont_property.py
--rw-r--r--   0     1001      127     5241 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/models/entity.py
--rw-r--r--   0     1001      127        0 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/models/__init__.py
--rw-r--r--   0     1001      127     1356 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/models/page_article.py
--rw-r--r--   0     1001      127     3776 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/models/linked_html_table.py
--rw-r--r--   0     1001      127     4433 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/models/html_article.py
--rw-r--r--   0     1001      127     1318 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/relational_tables.py
--rw-r--r--   0     1001      127      224 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/__init__.py
--rw-r--r--   0     1001      127     3570 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/html_articles.py
--rw-r--r--   0     1001      127     2290 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/article_aliases.py
--rw-r--r--   0     1001      127     2212 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/article_metadata.py
--rw-r--r--   0     1001      127     2765 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/article_links.py
--rw-r--r--   0     1001      127     2267 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/easy_tables_metadata.py
--rw-r--r--   0     1001      127      108 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/__main__.py
--rw-r--r--   0     1001      127     8554 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/easy_tables.py
--rw-r--r--   0     1001      127     2822 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/html_tables.py
--rw-r--r--   0     1001      127     4810 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/linked_relational_tables.py
--rw-r--r--   0     1001      127     4168 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/grouped_articles.py.deprecated
--rw-r--r--   0     1001      127     3025 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/articles.py.deprecated
--rw-r--r--   0     1001      127     1907 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/datasets/article_degrees.py
--rw-r--r--   0     1001      127     2908 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/misc.py
--rw-r--r--   0     1001      127     2432 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/config.py
--rw-r--r--   0     1001      127       42 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/prelude.py
--rw-r--r--   0     1001      127     5053 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikipedia/wikiapi.py
--rw-r--r--   0     1001      127        0 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/__init__.py
--rw-r--r--   0     1001      127     1760 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/page_ids.py
--rw-r--r--   0     1001      127      954 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/entity_labels.py
--rw-r--r--   0     1001      127        0 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/__init__.py
--rw-r--r--   0     1001      127      587 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/wikilink_dump.py
--rw-r--r--   0     1001      127     1644 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/class_count.py
--rw-r--r--   0     1001      127     7066 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/meta_graph.py
--rw-r--r--   0     1001      127     1730 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/mapping_extractor_dump.py
--rw-r--r--   0     1001      127      832 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/page_id_dump.py
--rw-r--r--   0     1001      127     6863 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/ontology_dump.py
--rw-r--r--   0     1001      127     1843 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/entity_metadata.py
--rw-r--r--   0     1001      127     1725 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/generic_extractor_dump.py
--rw-r--r--   0     1001      127     6968 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/entities.py
--rw-r--r--   0     1001      127     4202 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/entity_all_types.py
--rw-r--r--   0     1001      127      995 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/entity_types.py
--rw-r--r--   0     1001      127     2715 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/__main__.py
--rw-r--r--   0     1001      127     5895 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/properties.py
--rw-r--r--   0     1001      127     7788 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/meta_graph_stats.py
--rw-r--r--   0     1001      127     3513 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/entity_degrees.py
--rw-r--r--   0     1001      127     3348 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/classes.py
--rw-r--r--   0     1001      127     1582 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/entity_types_and_degrees.py
--rw-r--r--   0     1001      127     2223 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/entity_redirections.py
--rw-r--r--   0     1001      127     3862 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/datasets/wikilinks.py
--rw-r--r--   0     1001      127     2167 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/__main__.py
--rw-r--r--   0     1001      127     3679 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dbpedia/config.py
--rw-r--r--   0     1001      127        0 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/py.typed
--rw-r--r--   0     1001      127      328 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/spark/__init__.py
--rw-r--r--   0     1001      127     4253 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/spark/rdd_alike.py
--rw-r--r--   0     1001      127    20035 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/spark/common.py
--rw-r--r--   0     1001      127    24898 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/spark/extended_rdd.py
--rw-r--r--   0     1001      127    24445 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/dataset.py
--rw-r--r--   0     1001      127     1677 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/misc/hierarchy.py
--rw-r--r--   0     1001      127     2243 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/misc/modification.py
--rw-r--r--   0     1001      127        0 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/misc/__init__.py
--rw-r--r--   0     1001      127     1272 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/misc/query.py
--rw-r--r--   0     1001      127     2388 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/misc/resource.py
--rw-r--r--   0     1001      127     1478 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/misc/funcs.py
--rw-r--r--   0     1001      127    18184 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/misc/download.py
--rw-r--r--   0     1001      127     7492 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/misc/ntriples_parser.py
--rw-r--r--   0     1001      127        0 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/__init__.py
--rw-r--r--   0     1001      127    12208 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/db.py
--rw-r--r--   0     1001      127     1138 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/models/__init__.py
--rw-r--r--   0     1001      127     7623 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/models/wdproperty.py
--rw-r--r--   0     1001      127     1792 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/models/wdclass.py
--rw-r--r--   0     1001      127     2148 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/models/wdstatement.py
--rw-r--r--   0     1001      127     9107 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/models/wdvalue.py
--rw-r--r--   0     1001      127     1377 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/models/propertystats.py
--rw-r--r--   0     1001      127     8071 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/models/wdentity.py
--rw-r--r--   0     1001      127     1231 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/models/wdentitymetadata.py
--rw-r--r--   0     1001      127      639 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/models/wdentitylabel.py
--rw-r--r--   0     1001      127      428 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/models/wdentitylink.py
--rw-r--r--   0     1001      127     1786 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/wikidata_prefixes.yml
--rw-r--r--   0     1001      127     3095 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/page_ids.py
--rw-r--r--   0     1001      127     1046 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_labels.py
--rw-r--r--   0     1001      127        0 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/__init__.py
--rw-r--r--   0     1001      127     1579 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/class_count.py
--rw-r--r--   0     1001      127     5369 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/meta_graph.py
--rw-r--r--   0     1001      127     3490 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_outlinks.py
--rw-r--r--   0     1001      127     1953 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/property_domains.py
--rw-r--r--   0     1001      127     1543 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/page_dump.py
--rw-r--r--   0     1001      127     2509 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/property_ranges.py
--rw-r--r--   0     1001      127     1559 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_redirection_dump.py
--rw-r--r--   0     1001      127     1833 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_metadata.py
--rw-r--r--   0     1001      127     2662 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_ids.py
--rw-r--r--   0     1001      127    11156 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entities.py
--rw-r--r--   0     1001      127     5703 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/main_property_connections.py
--rw-r--r--   0     1001      127     2198 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_all_types.py
--rw-r--r--   0     1001      127      993 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_types.py
--rw-r--r--   0     1001      127     1025 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/__main__.py
--rw-r--r--   0     1001      127     3954 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/properties.py
--rw-r--r--   0     1001      127     1686 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_dump.py
--rw-r--r--   0     1001      127     7754 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/meta_graph_stats.py
--rw-r--r--   0     1001      127     3400 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_degrees.py
--rw-r--r--   0     1001      127     1695 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/property_count.py
--rw-r--r--   0     1001      127     3952 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/classes.py
--rw-r--r--   0     1001      127     8824 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_pagerank.py
--rw-r--r--   0     1001      127     1764 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_types_and_degrees.py
--rw-r--r--   0     1001      127      949 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/ontology_count.py
--rw-r--r--   0     1001      127     7003 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_redirections.py
--rw-r--r--   0     1001      127     3241 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/entity_wiki_aliases.py
--rw-r--r--   0     1001      127     5789 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/datasets/cross_wiki_mapping.py
--rw-r--r--   0     1001      127     7940 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/__main__.py
--rw-r--r--   0     1001      127     6627 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/extra_ent_db.py
--rw-r--r--   0     1001      127     3824 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/wikidata/config.py
--rw-r--r--   0     1001      127     1444 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/config.py
--rw-r--r--   0     1001      127     7241 2024-03-28 22:37:14.000000 kgdata-7.0.0/kgdata/splitter.py
--rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 kgdata-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 kgdata-7.0.1/Cargo.toml
+-rw-r--r--   0     1001      127    56429 2024-04-26 15:45:38.000000 kgdata-7.0.1/Cargo.lock
+-rw-r--r--   0     1001      127     1064 2024-04-26 15:45:38.000000 kgdata-7.0.1/LICENSE
+-rw-r--r--   0     1001      127      839 2024-04-26 15:45:38.000000 kgdata-7.0.1/README.md
+-rw-r--r--   0     1001      127    33619 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/conversions.rs
+-rw-r--r--   0     1001      127     2536 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/interface.rs
+-rw-r--r--   0     1001      127     4415 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/mod.rs
+-rw-r--r--   0     1001      127     6266 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/predefined_db.rs
+-rw-r--r--   0     1001      127     4987 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/readonly_rocksdb_dict.rs
+-rw-r--r--   0     1001      127     6211 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/ipcserde.rs
+-rw-r--r--   0     1001      127      926 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/mod.rs
+-rw-r--r--   0     1001      127     6376 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/nngserver.rs
+-rw-r--r--   0     1001      127    11896 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/remote_rocksdb_dict.rs
+-rw-r--r--   0     1001      127     2177 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/request.rs
+-rw-r--r--   0     1001      127     6487 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/response.rs
+-rw-r--r--   0     1001      127     8671 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/shmemhelper.rs
+-rw-r--r--   0     1001      127     2842 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/zeromqserver.rs
+-rw-r--r--   0     1001      127     1648 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/error.rs
+-rw-r--r--   0     1001      127      662 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/lib.rs
+-rw-r--r--   0     1001      127      732 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/main.rs
+-rw-r--r--   0     1001      127     2566 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/dataset.rs
+-rw-r--r--   0     1001      127      580 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/filterop.rs
+-rw-r--r--   0     1001      127      721 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/foldop.rs
+-rw-r--r--   0     1001      127     2788 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/functions.rs
+-rw-r--r--   0     1001      127     1188 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/mapop.rs
+-rw-r--r--   0     1001      127      468 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/miscop.rs
+-rw-r--r--   0     1001      127     4851 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/mod.rs
+-rw-r--r--   0     1001      127      630 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/sortop.rs
+-rw-r--r--   0     1001      127      534 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/class.rs
+-rw-r--r--   0     1001      127     1936 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/entity.rs
+-rw-r--r--   0     1001      127      248 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/entity_link.rs
+-rw-r--r--   0     1001      127      426 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/entity_metadata.rs
+-rw-r--r--   0     1001      127      686 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/kgns.rs
+-rw-r--r--   0     1001      127      560 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/mod.rs
+-rw-r--r--   0     1001      127      648 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/multilingual.rs
+-rw-r--r--   0     1001      127     3434 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/property.rs
+-rw-r--r--   0     1001      127     5919 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/value.rs
+-rw-r--r--   0     1001      127      944 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/hashbrown.rs
+-rw-r--r--   0     1001      127     4371 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/macros/list.rs
+-rw-r--r--   0     1001      127     5848 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/macros/map.rs
+-rw-r--r--   0     1001      127     6339 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/macros/mod.rs
+-rw-r--r--   0     1001      127     2133 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/macros/set.rs
+-rw-r--r--   0     1001      127      784 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/mod.rs
+-rw-r--r--   0     1001      127      805 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/strview.rs
+-rw-r--r--   0     1001      127      682 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/usizeview.rs
+-rw-r--r--   0     1001      127       33 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/mod.rs
+-rw-r--r--   0     1001      127     1286 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/class.rs
+-rw-r--r--   0     1001      127      419 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/conversions.rs
+-rw-r--r--   0     1001      127     2378 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/entity.rs
+-rw-r--r--   0     1001      127     1133 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/entity_metadata.rs
+-rw-r--r--   0     1001      127    10911 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/iterators.rs
+-rw-r--r--   0     1001      127     1358 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/mod.rs
+-rw-r--r--   0     1001      127     2433 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/multilingual.rs
+-rw-r--r--   0     1001      127     1827 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/property.rs
+-rw-r--r--   0     1001      127     8042 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/value.rs
+-rw-r--r--   0     1001      127     7062 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/scripts.rs
+-rw-r--r--   0     1001      127     1585 2024-04-26 15:45:38.000000 kgdata-7.0.1/pyproject.toml
+-rw-r--r--   0     1001      127       42 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/prelude.py
+-rw-r--r--   0     1001      127     2499 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/config.py
+-rw-r--r--   0     1001      127     2908 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/misc.py
+-rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/__init__.py
+-rw-r--r--   0     1001      127     2212 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/article_metadata.py
+-rw-r--r--   0     1001      127     2427 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/mention_to_articles.py
+-rw-r--r--   0     1001      127     4810 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/linked_relational_tables.py
+-rw-r--r--   0     1001      127     3025 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/articles.py.deprecated
+-rw-r--r--   0     1001      127     4168 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/grouped_articles.py.deprecated
+-rw-r--r--   0     1001      127     2267 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/easy_tables_metadata.py
+-rw-r--r--   0     1001      127     2290 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/article_aliases.py
+-rw-r--r--   0     1001      127     3570 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/html_articles.py
+-rw-r--r--   0     1001      127     2765 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/article_links.py
+-rw-r--r--   0     1001      127      224 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/__init__.py
+-rw-r--r--   0     1001      127     8554 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/easy_tables.py
+-rw-r--r--   0     1001      127      108 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/__main__.py
+-rw-r--r--   0     1001      127     2822 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/html_tables.py
+-rw-r--r--   0     1001      127     1907 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/article_degrees.py
+-rw-r--r--   0     1001      127     1318 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/relational_tables.py
+-rw-r--r--   0     1001      127     5053 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/wikiapi.py
+-rw-r--r--   0     1001      127     1356 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/models/page_article.py
+-rw-r--r--   0     1001      127     3776 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/models/linked_html_table.py
+-rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/models/__init__.py
+-rw-r--r--   0     1001      127     4433 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/models/html_article.py
+-rw-r--r--   0     1001      127    10271 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/db.py
+-rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/py.typed
+-rw-r--r--   0     1001      127    13686 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/db.py
+-rw-r--r--   0     1001      127     6627 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/extra_ent_db.py
+-rw-r--r--   0     1001      127     1786 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/wikidata_prefixes.yml
+-rw-r--r--   0     1001      127     4138 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/config.py
+-rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/__init__.py
+-rw-r--r--   0     1001      127     8586 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/__main__.py
+-rw-r--r--   0     1001      127     3490 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_outlinks.py
+-rw-r--r--   0     1001      127     5703 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/main_property_connections.py
+-rw-r--r--   0     1001      127     1833 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_metadata.py
+-rw-r--r--   0     1001      127     1906 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_types_and_degrees.py
+-rw-r--r--   0     1001      127     3952 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/classes.py
+-rw-r--r--   0     1001      127     3954 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/properties.py
+-rw-r--r--   0     1001      127     1559 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_redirection_dump.py
+-rw-r--r--   0     1001      127      993 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_types.py
+-rw-r--r--   0     1001      127     1543 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/page_dump.py
+-rw-r--r--   0     1001      127    11156 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entities.py
+-rw-r--r--   0     1001      127     1686 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_dump.py
+-rw-r--r--   0     1001      127     2509 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/property_ranges.py
+-rw-r--r--   0     1001      127     5369 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/meta_graph.py
+-rw-r--r--   0     1001      127     3400 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_degrees.py
+-rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/__init__.py
+-rw-r--r--   0     1001      127     1953 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/property_domains.py
+-rw-r--r--   0     1001      127     2662 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_ids.py
+-rw-r--r--   0     1001      127     1557 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/norm_mentions.py
+-rw-r--r--   0     1001      127     2198 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_all_types.py
+-rw-r--r--   0     1001      127     1025 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/__main__.py
+-rw-r--r--   0     1001      127     7003 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_redirections.py
+-rw-r--r--   0     1001      127     3095 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/page_ids.py
+-rw-r--r--   0     1001      127     7754 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/meta_graph_stats.py
+-rw-r--r--   0     1001      127     3241 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_wiki_aliases.py
+-rw-r--r--   0     1001      127     5789 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/cross_wiki_mapping.py
+-rw-r--r--   0     1001      127     1046 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_labels.py
+-rw-r--r--   0     1001      127     1930 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/triple_truthy_dump.py
+-rw-r--r--   0     1001      127     2743 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/mention_to_entities.py
+-rw-r--r--   0     1001      127     1579 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/class_count.py
+-rw-r--r--   0     1001      127     1695 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/property_count.py
+-rw-r--r--   0     1001      127     8824 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_pagerank.py
+-rw-r--r--   0     1001      127      949 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/ontology_count.py
+-rw-r--r--   0     1001      127      639 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdentitylabel.py
+-rw-r--r--   0     1001      127     8071 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdentity.py
+-rw-r--r--   0     1001      127     1231 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdentitymetadata.py
+-rw-r--r--   0     1001      127     7623 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdproperty.py
+-rw-r--r--   0     1001      127     1138 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/__init__.py
+-rw-r--r--   0     1001      127     1377 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/propertystats.py
+-rw-r--r--   0     1001      127     2148 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdstatement.py
+-rw-r--r--   0     1001      127     9107 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdvalue.py
+-rw-r--r--   0     1001      127     2024 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdclass.py
+-rw-r--r--   0     1001      127      428 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdentitylink.py
+-rw-r--r--   0     1001      127     7241 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/splitter.py
+-rw-r--r--   0     1001      127     2243 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/modification.py
+-rw-r--r--   0     1001      127     2388 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/resource.py
+-rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/__init__.py
+-rw-r--r--   0     1001      127     7492 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/ntriples_parser.py
+-rw-r--r--   0     1001      127     1478 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/funcs.py
+-rw-r--r--   0     1001      127     1677 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/hierarchy.py
+-rw-r--r--   0     1001      127    18184 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/download.py
+-rw-r--r--   0     1001      127     1272 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/query.py
+-rw-r--r--   0     1001      127     3679 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/config.py
+-rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/__init__.py
+-rw-r--r--   0     1001      127     2371 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/__main__.py
+-rw-r--r--   0     1001      127     1843 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_metadata.py
+-rw-r--r--   0     1001      127     1582 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_types_and_degrees.py
+-rw-r--r--   0     1001      127     3348 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/classes.py
+-rw-r--r--   0     1001      127     5891 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/properties.py
+-rw-r--r--   0     1001      127      995 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_types.py
+-rw-r--r--   0     1001      127     1725 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/generic_extractor_dump.py
+-rw-r--r--   0     1001      127     6968 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entities.py
+-rw-r--r--   0     1001      127     7066 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/meta_graph.py
+-rw-r--r--   0     1001      127     3862 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/wikilinks.py
+-rw-r--r--   0     1001      127     3513 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_degrees.py
+-rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/__init__.py
+-rw-r--r--   0     1001      127     1730 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/mapping_extractor_dump.py
+-rw-r--r--   0     1001      127      587 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/wikilink_dump.py
+-rw-r--r--   0     1001      127     4202 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_all_types.py
+-rw-r--r--   0     1001      127     2715 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/__main__.py
+-rw-r--r--   0     1001      127     6863 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/ontology_dump.py
+-rw-r--r--   0     1001      127     2223 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_redirections.py
+-rw-r--r--   0     1001      127     1760 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/page_ids.py
+-rw-r--r--   0     1001      127     7788 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/meta_graph_stats.py
+-rw-r--r--   0     1001      127      954 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_labels.py
+-rw-r--r--   0     1001      127      832 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/page_id_dump.py
+-rw-r--r--   0     1001      127     1644 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/class_count.py
+-rw-r--r--   0     1001      127     1444 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/config.py
+-rw-r--r--   0     1001      127    24445 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dataset.py
+-rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/__init__.py
+-rw-r--r--   0     1001      127    20035 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/spark/common.py
+-rw-r--r--   0     1001      127      328 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/spark/__init__.py
+-rw-r--r--   0     1001      127     4253 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/spark/rdd_alike.py
+-rw-r--r--   0     1001      127    24898 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/spark/extended_rdd.py
+-rw-r--r--   0     1001      127       27 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/core/__init__.pyi
+-rw-r--r--   0     1001      127     1385 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/core/base.pyi
+-rw-r--r--   0     1001      127     6044 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/core/models.pyi
+-rw-r--r--   0     1001      127     3748 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/models/ont_class.py
+-rw-r--r--   0     1001      127     3000 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/models/multilingual.py
+-rw-r--r--   0     1001      127     5241 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/models/entity.py
+-rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/models/__init__.py
+-rw-r--r--   0     1001      127     4587 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/models/ont_property.py
+-rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 kgdata-7.0.1/PKG-INFO
```

### Comparing `kgdata-7.0.0/Cargo.toml` & `kgdata-7.0.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/Cargo.lock` & `kgdata-7.0.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/LICENSE` & `kgdata-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/README.md` & `kgdata-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/conversions.rs` & `kgdata-7.0.1/src/conversions.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/interface.rs` & `kgdata-7.0.1/src/db/interface.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/mod.rs` & `kgdata-7.0.1/src/db/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/predefined_db.rs` & `kgdata-7.0.1/src/db/predefined_db.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/readonly_rocksdb_dict.rs` & `kgdata-7.0.1/src/db/readonly_rocksdb_dict.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/remotedb/ipcserde.rs` & `kgdata-7.0.1/src/db/remotedb/ipcserde.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/remotedb/mod.rs` & `kgdata-7.0.1/src/db/remotedb/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/remotedb/nngserver.rs` & `kgdata-7.0.1/src/db/remotedb/nngserver.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/remotedb/remote_rocksdb_dict.rs` & `kgdata-7.0.1/src/db/remotedb/remote_rocksdb_dict.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/remotedb/request.rs` & `kgdata-7.0.1/src/db/remotedb/request.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/remotedb/response.rs` & `kgdata-7.0.1/src/db/remotedb/response.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/remotedb/shmemhelper.rs` & `kgdata-7.0.1/src/db/remotedb/shmemhelper.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/db/remotedb/zeromqserver.rs` & `kgdata-7.0.1/src/db/remotedb/zeromqserver.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/error.rs` & `kgdata-7.0.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/lib.rs` & `kgdata-7.0.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/main.rs` & `kgdata-7.0.1/src/main.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/mapreduce/dataset.rs` & `kgdata-7.0.1/src/mapreduce/dataset.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/mapreduce/filterop.rs` & `kgdata-7.0.1/src/mapreduce/filterop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/mapreduce/foldop.rs` & `kgdata-7.0.1/src/mapreduce/foldop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/mapreduce/functions.rs` & `kgdata-7.0.1/src/mapreduce/functions.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/mapreduce/mapop.rs` & `kgdata-7.0.1/src/mapreduce/mapop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/mapreduce/mod.rs` & `kgdata-7.0.1/src/mapreduce/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/mapreduce/sortop.rs` & `kgdata-7.0.1/src/mapreduce/sortop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/models/class.rs` & `kgdata-7.0.1/src/models/class.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/models/entity.rs` & `kgdata-7.0.1/src/models/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/models/kgns.rs` & `kgdata-7.0.1/src/models/kgns.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/models/mod.rs` & `kgdata-7.0.1/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/models/multilingual.rs` & `kgdata-7.0.1/src/models/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/models/property.rs` & `kgdata-7.0.1/src/models/property.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/models/value.rs` & `kgdata-7.0.1/src/models/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/pyo3helper/hashbrown.rs` & `kgdata-7.0.1/src/pyo3helper/hashbrown.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/pyo3helper/macros/list.rs` & `kgdata-7.0.1/src/pyo3helper/macros/list.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/pyo3helper/macros/map.rs` & `kgdata-7.0.1/src/pyo3helper/macros/map.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/pyo3helper/macros/mod.rs` & `kgdata-7.0.1/src/pyo3helper/macros/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/pyo3helper/macros/set.rs` & `kgdata-7.0.1/src/pyo3helper/macros/set.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/pyo3helper/mod.rs` & `kgdata-7.0.1/src/pyo3helper/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/pyo3helper/strview.rs` & `kgdata-7.0.1/src/pyo3helper/strview.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/pyo3helper/usizeview.rs` & `kgdata-7.0.1/src/pyo3helper/usizeview.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/python/models/class.rs` & `kgdata-7.0.1/src/python/models/class.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/python/models/entity.rs` & `kgdata-7.0.1/src/python/models/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/python/models/entity_metadata.rs` & `kgdata-7.0.1/src/python/models/entity_metadata.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/python/models/iterators.rs` & `kgdata-7.0.1/src/python/models/iterators.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/python/models/mod.rs` & `kgdata-7.0.1/src/python/models/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/python/models/multilingual.rs` & `kgdata-7.0.1/src/python/models/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/python/models/property.rs` & `kgdata-7.0.1/src/python/models/property.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/python/models/value.rs` & `kgdata-7.0.1/src/python/models/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/src/python/scripts.rs` & `kgdata-7.0.1/src/python/scripts.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/pyproject.toml` & `kgdata-7.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kgdata"
-version = "7.0.0"
+version = "7.0.1"
 description = "Library to process dumps of knowledge graphs (Wikipedia, DBpedia, Wikidata)"
 readme = "README.md"
 authors = [{ name = "Binh Vu", email = "binh@toan2.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -13,15 +13,15 @@
 requires-python = ">=3.10"
 
 dependencies = [
     'orjson >= 3.9.0, < 4.0.0',
     'tqdm >= 4.64.0, < 5.0.0',
     'beautifulsoup4 >= 4.9.3, < 5.0.0',
     'loguru >= 0.7.0, < 0.8.0',
-    'rdflib >= 6.1.1, < 7.0.0',
+    'rdflib >= 7.0.0, < 8.0.0',
     'six >= 1.16.0, < 2.0.0',
     'ruamel.yaml >= 0.17.21, < 0.18.0',
     'chardet >= 5.0.0, < 6.0.0',
     'ujson >= 5.5.0, < 6.0.0',
     'redis >= 3.5.3, < 4.0.0',
     'numpy >= 1.22.3, < 2.0.0',
     'requests >= 2.28.0, < 3.0.0',
@@ -29,27 +29,28 @@
     'click >= 8.1.3, < 9.0.0',
     'parsimonious >= 0.8.1, < 0.9.0',
     'hugedict >= 2.12.10, < 3.0.0',
     'rsoup >= 3.1.7, < 4.0.0',
     'lxml >= 4.9.0, < 5.0.0',
     'ray >= 2.0.1, < 3.0.0',
     'pqdict >= 1.3.0, < 2.0.0',
+    'ftfy >= 6.1.3, < 7.0.0',
 ]
 
 [project.urls]
 homepage = "https://github.com/binh-vu/kgdata"
 repository = "https://github.com/binh-vu/kgdata"
 
 [project.optional-dependencies]
 dev = [
     'python-dotenv >= 0.19.0, < 0.20.0',
     'pytest >= 7.1.3, < 8.0.0',
     'black >= 22.10.0, < 23.0.0',
 ]
-spark = ['pyspark >= 3.4.1, < 4.0.0']
+spark = ['pyspark >= 3.5.0, < 4.0.0']
 all = ["kgdata[dev,spark]"]
 
 [tool.maturin]
 module-name = "kgdata.core"
 features = ["extension-module"]
 
 [build-system]
```

### Comparing `kgdata-7.0.0/kgdata/core/models.pyi` & `kgdata-7.0.1/kgdata/core/models.pyi`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/core/base.pyi` & `kgdata-7.0.1/kgdata/core/base.pyi`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/db.py` & `kgdata-7.0.1/kgdata/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,19 @@
 )
 get_entity_label_db = partial(
     get_rocksdb,
     deser_value=partial(str, encoding="utf-8"),
     ser_value=str.encode,
     dbopts=small_dbopts,
 )
+get_entity_type_db: make_get_rocksdb[list[str]] = make_get_rocksdb(
+    deser_value=orjson.loads,
+    ser_value=orjson.dumps,
+    dbopts=small_dbopts,
+)
 get_entity_redirection_db = partial(
     get_rocksdb,
     deser_value=partial(str, encoding="utf-8"),
     ser_value=str.encode,
     dbopts=small_dbopts,
 )
 get_entity_metadata_db = partial(
@@ -256,15 +261,17 @@
     def entity_metadata(self):
         return get_entity_metadata_db(
             self.database_dir / "entity_metadata.db", read_only=self.read_only
         )
 
     @cached_property
     def entity_types(self):
-        raise NotImplementedError()
+        return get_entity_type_db(
+            self.database_dir / "entity_types.db", read_only=self.read_only
+        )
 
     @cached_property
     def ontcount(self):
         raise NotImplementedError()
 
     def get_default_props(self):
         return {p.id: p for p in get_default_props()}
```

### Comparing `kgdata-7.0.0/kgdata/models/ont_class.py` & `kgdata-7.0.1/kgdata/models/ont_class.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/models/multilingual.py` & `kgdata-7.0.1/kgdata/models/multilingual.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/models/ont_property.py` & `kgdata-7.0.1/kgdata/models/ont_property.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     id: str
     label: MultiLingualString
     description: MultiLingualString
     aliases: MultiLingualStringList
     datatype: str
     instanceof: list[str]
     parents: list[str]
+    # do not include the property itself
     ancestors: dict[str, int]
     inverse_properties: list[str]
     related_properties: list[str]
     equivalent_properties: list[str]
 
     # domains
     domains: list[str]
```

### Comparing `kgdata-7.0.0/kgdata/models/entity.py` & `kgdata-7.0.1/kgdata/models/entity.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/models/page_article.py` & `kgdata-7.0.1/kgdata/wikipedia/models/page_article.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/models/linked_html_table.py` & `kgdata-7.0.1/kgdata/wikipedia/models/linked_html_table.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/models/html_article.py` & `kgdata-7.0.1/kgdata/wikipedia/models/html_article.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/relational_tables.py` & `kgdata-7.0.1/kgdata/wikipedia/datasets/relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/html_articles.py` & `kgdata-7.0.1/kgdata/wikipedia/datasets/html_articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/article_aliases.py` & `kgdata-7.0.1/kgdata/wikipedia/datasets/article_aliases.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/article_metadata.py` & `kgdata-7.0.1/kgdata/wikipedia/datasets/article_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/article_links.py` & `kgdata-7.0.1/kgdata/wikipedia/datasets/article_links.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/easy_tables_metadata.py` & `kgdata-7.0.1/kgdata/wikipedia/datasets/easy_tables_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/easy_tables.py` & `kgdata-7.0.1/kgdata/wikipedia/datasets/easy_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/html_tables.py` & `kgdata-7.0.1/kgdata/wikipedia/datasets/html_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/linked_relational_tables.py` & `kgdata-7.0.1/kgdata/wikipedia/datasets/linked_relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/grouped_articles.py.deprecated` & `kgdata-7.0.1/kgdata/wikipedia/datasets/grouped_articles.py.deprecated`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/articles.py.deprecated` & `kgdata-7.0.1/kgdata/wikipedia/datasets/articles.py.deprecated`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/datasets/article_degrees.py` & `kgdata-7.0.1/kgdata/wikipedia/datasets/article_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/misc.py` & `kgdata-7.0.1/kgdata/wikipedia/misc.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikipedia/config.py` & `kgdata-7.0.1/kgdata/wikipedia/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         self.grouped_articles = datadir / "grouped_articles"
         self.html_articles = datadir / "html_articles"
         self.html_tables = datadir / "html_tables"
         self.article_metadata = datadir / "article_metadata"
         self.article_links = datadir / "article_links"
         self.article_aliases = datadir / "article_aliases"
         self.article_degrees = datadir / "article_degrees"
+        self.mention_to_articles = datadir / "mention_to_articles"
         self.relational_tables = datadir / "relational_tables"
         self.linked_relational_tables = datadir / "linked_relational_tables"
         self.easy_tables = datadir / "easy_tables"
         self.easy_tables_metadata = datadir / "easy_tables_metadata"
 
     @lru_cache
     def get_dump_date(self):
```

### Comparing `kgdata-7.0.0/kgdata/wikipedia/wikiapi.py` & `kgdata-7.0.1/kgdata/wikipedia/wikiapi.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/page_ids.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/entity_labels.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_labels.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/wikilink_dump.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/wikilink_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/class_count.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/class_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/meta_graph.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/meta_graph.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/mapping_extractor_dump.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/mapping_extractor_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/page_id_dump.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/page_id_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/ontology_dump.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/ontology_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/entity_metadata.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/generic_extractor_dump.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/generic_extractor_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/entities.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/entity_all_types.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_all_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/entity_types.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/__main__.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/properties.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,19 @@
         if default_lang in description.lang2value:
             description.lang = default_lang
         else:
             # to handle case where there is no description in default language
             description.lang = default_lang
             description.lang2value[default_lang] = ""
 
-    domains = None
+    domains = []
     if rdfs_domain in resource.props:
         domains = [str(term) for term in resource.props.get(rdfs_domain, [])]
 
-    ranges = None
+    ranges = []
     if (
         OWL.ObjectProperty in resource.props.get(rdf_type, [])
         and rdfs_range in resource.props
     ):
         ranges = [str(term) for term in resource.props.get(rdfs_range, [])]
 
     return OntologyProperty(
```

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/meta_graph_stats.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/meta_graph_stats.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/entity_degrees.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/classes.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/entity_types_and_degrees.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_types_and_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/entity_redirections.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_redirections.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/datasets/wikilinks.py` & `kgdata-7.0.1/kgdata/dbpedia/datasets/wikilinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dbpedia/__main__.py` & `kgdata-7.0.1/kgdata/dbpedia/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,11 +74,20 @@
         "entity_redirections",
         format={
             "record_type": {"type": "tuple2", "key": None, "value": None},
             "is_sorted": False,
         },
     )
 )
+dbpedia.add_command(
+    dataset2db(
+        "entity_types",
+        format={
+            "record_type": {"type": "tuple2", "key": None, "value": None},
+            "is_sorted": False,
+        },
+    )
+)
 
 if __name__ == "__main__":
     init_env_logger()
     dbpedia()
```

### Comparing `kgdata-7.0.0/kgdata/dbpedia/config.py` & `kgdata-7.0.1/kgdata/dbpedia/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/spark/rdd_alike.py` & `kgdata-7.0.1/kgdata/spark/rdd_alike.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/spark/common.py` & `kgdata-7.0.1/kgdata/spark/common.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/spark/extended_rdd.py` & `kgdata-7.0.1/kgdata/spark/extended_rdd.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/dataset.py` & `kgdata-7.0.1/kgdata/dataset.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/misc/hierarchy.py` & `kgdata-7.0.1/kgdata/misc/hierarchy.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/misc/modification.py` & `kgdata-7.0.1/kgdata/misc/modification.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/misc/query.py` & `kgdata-7.0.1/kgdata/misc/query.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/misc/resource.py` & `kgdata-7.0.1/kgdata/misc/resource.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/misc/funcs.py` & `kgdata-7.0.1/kgdata/misc/funcs.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/misc/download.py` & `kgdata-7.0.1/kgdata/misc/download.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/misc/ntriples_parser.py` & `kgdata-7.0.1/kgdata/misc/ntriples_parser.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/db.py` & `kgdata-7.0.1/kgdata/wikidata/db.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,20 +36,22 @@
     ser_to_dict,
     ser_to_tuple,
     small_dbopts,
     unpack_float,
     unpack_int,
 )
 from kgdata.models.entity import EntityOutLinks
+from kgdata.wikidata.datasets.mention_to_entities import MentionToEntities
 from kgdata.wikidata.extra_ent_db import EntAttr, get_entity_attr_db
 from kgdata.wikidata.models import WDClass, WDProperty
 from kgdata.wikidata.models.wdentity import WDEntity
 from kgdata.wikidata.models.wdentitylabel import WDEntityLabel
 from kgdata.wikidata.models.wdentitylink import WDEntityWikiLink
 from kgdata.wikidata.models.wdentitymetadata import WDEntityMetadata
+from sm.misc.funcs import import_func
 
 V = TypeVar("V", WDEntity, WDClass, WDProperty, WDEntityLabel, WDEntityWikiLink)
 
 
 class WDProxyDB(RocksDBDict, HugeMutableMapping[str, V]):
     def set_extract_ent_from_entity(self, func: Callable[[WDEntity], V]):
         self.extract_ent_from_entity = func
@@ -241,14 +243,34 @@
     dbopts=small_dbopts,
 )
 get_prop_domain_db = make_get_rocksdb(
     deser_value=orjson.loads,
     ser_value=orjson.dumps,
     dbopts=small_dbopts,
 )
+get_mention_to_entities_db: make_get_rocksdb[list[tuple[str, tuple[int, int]]]] = (
+    make_get_rocksdb(
+        deser_value=orjson.loads,
+        ser_value=orjson.dumps,
+        dbopts=small_dbopts,
+    )
+)
+get_norm_mentions_db: make_get_rocksdb[list[tuple[str, tuple[int, int]]]] = (
+    make_get_rocksdb(
+        deser_value=orjson.loads,
+        ser_value=orjson.dumps,
+        dbopts=small_dbopts,
+    )
+)
+get_label2ids_db = partial(
+    get_rocksdb,
+    deser_value=orjson.loads,
+    ser_value=orjson.dumps,
+    dbopts=small_dbopts,
+)
 
 
 class WikidataDB(GenericDB):
     """Helper class to make it easier to load all Wikidata databases stored in a directory.
     The Wikidata database is expected to be stored in the directory under specific names.
 
     It makes use of the `functools.cached_property` decorator to cache the database objects
@@ -345,14 +367,32 @@
 
     @cached_property
     def entity_outlinks(self):
         return get_entity_outlinks_db(
             self.database_dir / "entity_outlinks.db", read_only=self.read_only
         )
 
+    @cached_property
+    def mention_to_entities(self):
+        return get_mention_to_entities_db(
+            self.database_dir / "mention_to_entities.db", read_only=self.read_only
+        )
+
+    @cached_property
+    def norm_mentions(self):
+        return get_norm_mentions_db(
+            self.database_dir / "norm_mentions.db", read_only=self.read_only
+        )
+
+    @cached_property
+    def label2ids(self):
+        return get_label2ids_db(
+            self.database_dir / "label2ids.db", read_only=self.read_only
+        )
+
     @overload
     def attr(
         self, attr: Literal["aliases", "instanceof"]
     ) -> HugeMutableMapping[str, list[str]]: ...
 
     @overload
     def attr(
@@ -382,22 +422,29 @@
 
 if __name__ == "__main__":
     import click
 
     @click.command()
     @click.option("-d", "--data-dir", required=True, help="database directory")
     @click.option("-n", "--dbname", required=True, help="database name")
+    @click.option("-f", "--format", default="", help="function to format the value")
     @click.argument("keys", nargs=-1)
-    def cli(data_dir: str, dbname: str, keys: list[str]):
+    def cli(data_dir: str, dbname: str, format: str, keys: list[str]):
+        if format == "":
+            fmt = str
+        else:
+            fmt1 = import_func(format)
+            fmt = lambda x: v.decode() if isinstance((v := fmt1(x)), bytes) else v
+
         db = getattr(WikidataDB(data_dir), dbname)
         if len(keys) > 0:
             for k in keys:
                 print("key:", k)
-                print("value:", db[k])
+                print("value:", fmt(db[k]))
                 print("")
         else:
             for k in db.keys():
                 print("key:", k)
-                print("value:", db[k])
+                print("value:", fmt(db[k]))
                 break
 
     cli()
```

### Comparing `kgdata-7.0.0/kgdata/wikidata/models/__init__.py` & `kgdata-7.0.1/kgdata/wikidata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/models/wdproperty.py` & `kgdata-7.0.1/kgdata/wikidata/models/wdproperty.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/models/wdclass.py` & `kgdata-7.0.1/kgdata/wikidata/models/wdclass.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,7 +52,16 @@
             aliases=self.aliases,
             parents=self.parents,
             properties=self.properties,
             different_froms=self.different_froms,
             equivalent_classes=self.equivalent_classes,
             ancestors=self.ancestors,
         )
+
+    def fmt(self):
+        return "\n".join(
+            [
+                f"label: {self.label} ({self.id})",
+                f"description: {self.description}",
+                f"parents: {self.parents}",
+            ]
+        )
```

### Comparing `kgdata-7.0.0/kgdata/wikidata/models/wdstatement.py` & `kgdata-7.0.1/kgdata/wikidata/models/wdstatement.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/models/wdvalue.py` & `kgdata-7.0.1/kgdata/wikidata/models/wdvalue.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/models/propertystats.py` & `kgdata-7.0.1/kgdata/wikidata/models/propertystats.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/models/wdentity.py` & `kgdata-7.0.1/kgdata/wikidata/models/wdentity.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/models/wdentitymetadata.py` & `kgdata-7.0.1/kgdata/wikidata/models/wdentitymetadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/models/wdentitylabel.py` & `kgdata-7.0.1/kgdata/wikidata/models/wdentitylabel.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/wikidata_prefixes.yml` & `kgdata-7.0.1/kgdata/wikidata/wikidata_prefixes.yml`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/page_ids.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_labels.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_labels.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/class_count.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/class_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/meta_graph.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/meta_graph.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_outlinks.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_outlinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/property_domains.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/property_domains.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/page_dump.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/page_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/property_ranges.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/property_ranges.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_redirection_dump.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_redirection_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_metadata.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_ids.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entities.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/main_property_connections.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/main_property_connections.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_all_types.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_all_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_types.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/__main__.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/properties.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/properties.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_dump.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/meta_graph_stats.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/meta_graph_stats.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_degrees.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/property_count.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/property_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/classes.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_pagerank.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_pagerank.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_types_and_degrees.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_types_and_degrees.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from kgdata.wikidata.datasets.entity_all_types import EntityAllTypes, entity_all_types
 from kgdata.wikidata.datasets.entity_degrees import EntityDegree, entity_degrees
 
 
 @dataclass
 class EntityTypeAndDegree(Record):
     id: str
+    # mapping from type to distance of the correct types
+    # zero is the type of that entity, 1 is the parent type, 2 is grand parent, etc.
     types: dict[str, int]
     indegree: int
     outdegree: int
 
     wikipedia_indegree: Optional[int] = None
     wikipedia_outdegree: Optional[int] = None
```

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/ontology_count.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/ontology_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_redirections.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_redirections.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/entity_wiki_aliases.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/entity_wiki_aliases.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/datasets/cross_wiki_mapping.py` & `kgdata-7.0.1/kgdata/wikidata/datasets/cross_wiki_mapping.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/__main__.py` & `kgdata-7.0.1/kgdata/wikidata/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,31 @@
 import os
 import shutil
 from operator import itemgetter
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional, cast, get_args
 
 import click
+import serde.jl
+import serde.json
 from hugedict.prelude import (
     RocksDBDict,
     RocksDBOptions,
     init_env_logger,
     rocksdb_build_sst_file,
     rocksdb_ingest_sst_files,
 )
-from timer import Timer
-
-import serde.jl
-import serde.json
 from kgdata.config import init_dbdir_from_env
 from kgdata.db import build_database
 from kgdata.wikidata.config import WikidataDirCfg
 from kgdata.wikidata.datasets.class_count import class_count
 from kgdata.wikidata.datasets.property_count import property_count
 from kgdata.wikidata.db import WikidataDB, get_ontcount_db, pack_int
 from kgdata.wikidata.extra_ent_db import EntAttr, build_extra_ent_db
+from timer import Timer
 
 if TYPE_CHECKING:
     from hugedict.core.rocksdb import FileFormat
 
 
 def dataset2db(
     dataset: str,
@@ -188,14 +187,42 @@
         format={
             "record_type": {"type": "tuple2", "key": None, "value": None},
             "is_sorted": False,
             "number_type": "u32",
         },
     )
 )
+wikidata.add_command(
+    dataset2db(
+        dataset="mention_to_entities",
+        dbname="mention_to_entities",
+        format={
+            "record_type": {
+                "type": "ndjson",
+                "key": "mention",
+                "value": "target_entities",
+            },
+            "is_sorted": False,
+        },
+    )
+)
+wikidata.add_command(
+    dataset2db(
+        dataset="norm_mentions",
+        dbname="norm_mentions",
+        format={
+            "record_type": {
+                "type": "tuple2",
+                "key": None,
+                "value": None,
+            },
+            "is_sorted": False,
+        },
+    )
+)
 
 
 @click.command(name="ontcount")
 @click.option("-d", "--directory", default="", help="Wikidata directory")
 @click.option("-o", "--output", help="Output directory")
 @click.option(
     "-c",
@@ -218,15 +245,14 @@
     options = cast(
         RocksDBDict,
         get_ontcount_db(dbpath, create_if_missing=True, read_only=False),
     ).options
     gc.collect()
 
     import ray
-
     from sm.misc.ray_helper import ray_map, ray_put
 
     ray.init()
 
     def _build_sst_file(
         infile: str, temp_dir: str, posfix: str, options: RocksDBOptions
     ):
```

### Comparing `kgdata-7.0.0/kgdata/wikidata/extra_ent_db.py` & `kgdata-7.0.1/kgdata/wikidata/extra_ent_db.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/wikidata/config.py` & `kgdata-7.0.1/kgdata/wikidata/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         # directorys contain dumps and their splitted files
         # for the name of the dumps, see the corresponding function `self.get_X_file` in this class
         self.dumps = datadir / "000_dumps"
         self.modification = datadir / "001_modifications"
         self.entity_dump = datadir / "012_entity_dump"
         self.page_dump = datadir / "010_page_dump"
         self.entity_redirection_dump = datadir / "011_entity_redirection_dump"
+        self.triple_truthy_dump = datadir / "013_triple_truthy_dump"
 
         self.page_ids = datadir / "020_page_ids"
         self.entity_ids = datadir / "021_entity_ids"
         self.entity_redirections = datadir / "022_entity_redirections"
         self.entities = datadir / "023_entities"
         self.entity_types = datadir / "024_entity_types"
 
@@ -49,14 +50,17 @@
         self.entity_degrees = datadir / "075_entity_degrees"
         self.entity_types_and_degrees = datadir / "076_entity_types_and_degrees"
         self.entity_wiki_aliases = datadir / "077_entity_wiki_aliases"
 
         self.meta_graph = datadir / "080_meta_graph"
         self.meta_graph_stats = datadir / "081_meta_graph_stats"
 
+        self.mention_to_entities = datadir / "090_mention_to_entities"
+        self.norm_mentions = datadir / "091_norm_mentions"
+
         # deprecated
         self.wp2wd = datadir / "wp2wd"
         self.search = datadir / "search"
 
     @lru_cache
     def get_dump_date(self):
         res = re.findall(r"\d{8}", str(self.datadir))
@@ -65,14 +69,17 @@
 
     def get_entity_dump_file(self):
         try:
             return self._get_file(self.dumps / "*wikidata-*all*.json.zst")
         except:
             return self._get_file(self.dumps / "*wikidata-*all*.json.bz2")
 
+    def get_triple_truthy_dump_file(self):
+        return self._get_file(self.dumps / "*wikidata-*truthy*.nt.*")
+
     def get_page_dump_file(self):
         return self._get_file(self.dumps / "*wikidatawiki-*page*.sql.gz")
 
     def get_redirect_dump_file(self):
         return self._get_file(self.dumps / "*wikidatawiki-*redirect*.sql.gz")
 
     def _get_file(self, file: Union[str, Path]):
```

### Comparing `kgdata-7.0.0/kgdata/config.py` & `kgdata-7.0.1/kgdata/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/kgdata/splitter.py` & `kgdata-7.0.1/kgdata/splitter.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.0/PKG-INFO` & `kgdata-7.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.3
 Name: kgdata
-Version: 7.0.0
+Version: 7.0.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: orjson >=3.9.0, <4.0.0
 Requires-Dist: tqdm >=4.64.0, <5.0.0
 Requires-Dist: beautifulsoup4 >=4.9.3, <5.0.0
 Requires-Dist: loguru >=0.7.0, <0.8.0
-Requires-Dist: rdflib >=6.1.1, <7.0.0
+Requires-Dist: rdflib >=7.0.0, <8.0.0
 Requires-Dist: six >=1.16.0, <2.0.0
 Requires-Dist: ruamel-yaml >=0.17.21, <0.18.0
 Requires-Dist: chardet >=5.0.0, <6.0.0
 Requires-Dist: ujson >=5.5.0, <6.0.0
 Requires-Dist: redis >=3.5.3, <4.0.0
 Requires-Dist: numpy >=1.22.3, <2.0.0
 Requires-Dist: requests >=2.28.0, <3.0.0
@@ -19,18 +19,19 @@
 Requires-Dist: click >=8.1.3, <9.0.0
 Requires-Dist: parsimonious >=0.8.1, <0.9.0
 Requires-Dist: hugedict >=2.12.10, <3.0.0
 Requires-Dist: rsoup >=3.1.7, <4.0.0
 Requires-Dist: lxml >=4.9.0, <5.0.0
 Requires-Dist: ray >=2.0.1, <3.0.0
 Requires-Dist: pqdict >=1.3.0, <2.0.0
+Requires-Dist: ftfy >=6.1.3, <7.0.0
 Requires-Dist: python-dotenv >=0.19.0, <0.20.0 ; extra == 'dev'
 Requires-Dist: pytest >=7.1.3, <8.0.0 ; extra == 'dev'
 Requires-Dist: black >=22.10.0, <23.0.0 ; extra == 'dev'
-Requires-Dist: pyspark >=3.4.1, <4.0.0 ; extra == 'spark'
+Requires-Dist: pyspark >=3.5.0, <4.0.0 ; extra == 'spark'
 Requires-Dist: kgdata[dev,spark] ; extra == 'all'
 Provides-Extra: dev
 Provides-Extra: spark
 Provides-Extra: all
 License-File: LICENSE
 License-File: LICENSE
 Summary: Library to process dumps of knowledge graphs (Wikipedia, DBpedia, Wikidata)
```

