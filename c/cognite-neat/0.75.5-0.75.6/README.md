# Comparing `tmp/cognite_neat-0.75.5.tar.gz` & `tmp/cognite_neat-0.75.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.75.5.tar", max compression
+gzip compressed data, was "cognite_neat-0.75.6.tar", max compression
```

## Comparing `cognite_neat-0.75.5.tar` & `cognite_neat-0.75.6.tar`

### file list

```diff
@@ -1,257 +1,257 @@
--rw-r--r--   0        0        0    11351 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/LICENSE
--rw-r--r--   0        0        0     6775 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/README.md
--rw-r--r--   0        0        0       61 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4606 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     4208 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/data_classes/configuration.py
--rw-r--r--   0        0        0     1675 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      554 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3529 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4646 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13661 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     8107 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12402 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1423704 2024-04-24 13:14:46.792801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js
--rw-r--r--   0        0        0     2667 2024-04-24 13:14:46.792801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt
--rw-r--r--   0        0        0  6282865 2024-04-24 13:14:46.816801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map
--rw-r--r--   0        0        0   240334 2024-04-24 13:14:46.820801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     1503 2024-04-24 13:14:46.824801 cognite_neat-0.75.5/cognite/neat/config.py
--rw-r--r--   0        0        0     1227 2024-04-24 13:14:46.824801 cognite_neat-0.75.5/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-04-24 13:14:46.824801 cognite_neat-0.75.5/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-04-24 13:14:46.824801 cognite_neat-0.75.5/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-24 13:14:46.828801 cognite_neat-0.75.5/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14947 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      149 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    13473 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/legacy/__init__.py
--rw-r--r--   0        0        0       73 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/legacy/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/__init__.py
--rw-r--r--   0        0        0      363 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_base.py
--rw-r--r--   0        0        0    11734 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_dexpi.py
--rw-r--r--   0        0        0    17695 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14909 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      701 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/__init__.py
--rw-r--r--   0        0        0    23859 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_asset_loader.py
--rw-r--r--   0        0        0     2399 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_base.py
--rw-r--r--   0        0        0     2837 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2321 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5023 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/models.py
--rw-r--r--   0        0        0    40480 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22715 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12995 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
--rw-r--r--   0        0        0     3327 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/validator.py
--rw-r--r--   0        0        0      149 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/__init__.py
--rw-r--r--   0        0        0    14289 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/__init__.py
--rw-r--r--   0        0        0     4765 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0    18719 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    14738 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/transformer.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/__init__.py
--rw-r--r--   0        0        0     8610 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1453 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_base.py
--rw-r--r--   0        0        0      102 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_core/__init__.py
--rw-r--r--   0        0        0      771 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
--rw-r--r--   0        0        0    36814 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8312 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0     6251 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2graphql.py
--rw-r--r--   0        0        0    18458 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0    28805 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3881 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     1085 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2triples.py
--rw-r--r--   0        0        0     5783 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/__init__.py
--rw-r--r--   0        0        0     2330 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_base.py
--rw-r--r--   0        0        0     6476 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_dict2rules.py
--rw-r--r--   0        0        0     7727 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0    12093 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_json2rules.py
--rw-r--r--   0        0        0       63 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9407 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10557 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1502 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0      421 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_xsd2rules.py
--rw-r--r--   0        0        0     1601 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      127 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/_base.py
--rw-r--r--   0        0        0    12382 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7351 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51091 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/tables.py
--rw-r--r--   0        0        0     4402 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/value_types.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0      176 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0      115 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/analysis/__init__.py
--rw-r--r--   0        0        0      673 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/analysis/_base.py
--rw-r--r--   0        0        0    19612 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/analysis/_information_rules.py
--rw-r--r--   0        0        0      374 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    65934 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      413 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1517 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1645 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    11853 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    13145 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    19900 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3038 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4090 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      408 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4267 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    10553 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12553 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6924 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11925 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7597 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7804 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7443 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     7110 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11480 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4197 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6158 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    15323 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3346 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     7493 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0     4893 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/_entity.py
--rw-r--r--   0        0        0     7228 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0      522 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/__init__.py
--rw-r--r--   0        0        0    11024 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_base.py
--rw-r--r--   0        0        0    56312 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_dms_architect_rules.py
--rw-r--r--   0        0        0    30789 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_dms_schema.py
--rw-r--r--   0        0        0     2567 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_domain_rules.py
--rw-r--r--   0        0        0    21658 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_information_rules.py
--rw-r--r--   0        0        0     1299 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/__init__.py
--rw-r--r--   0        0        0    12233 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_base.py
--rw-r--r--   0        0        0    10295 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_field.py
--rw-r--r--   0        0        0     6308 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_value.py
--rw-r--r--   0        0        0       68 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11063 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6319 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2722 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12826 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26857 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0    13659 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6568 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     3015 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0      257 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0     5161 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_loader.py
--rw-r--r--   0        0        0     6295 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_store.py
--rw-r--r--   0        0        0    16874 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/io_steps.py
--rw-r--r--   0        0        0    18678 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_exporter.py
--rw-r--r--   0        0        0    10812 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_importer.py
--rw-r--r--   0        0        0     4784 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_validator.py
--rw-r--r--   0        0        0      274 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/__init__.py
--rw-r--r--   0        0        0     3929 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
--rw-r--r--   0        0        0    29416 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
--rw-r--r--   0        0        0    27324 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_loader.py
--rw-r--r--   0        0        0    12728 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_store.py
--rw-r--r--   0        0        0     2361 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
--rw-r--r--   0        0        0    20706 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
--rw-r--r--   0        0        0    28111 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/rules_importer.py
--rw-r--r--   0        0        0     3010 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    10467 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4540 2024-04-24 13:14:47.236803 cognite_neat-0.75.5/pyproject.toml
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.75.5/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/LICENSE
+-rw-r--r--   0        0        0     6775 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/README.md
+-rw-r--r--   0        0        0       61 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4606 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     4208 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1675 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      554 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3529 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4646 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13661 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8107 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12402 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1423704 2024-04-26 08:02:28.908058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js
+-rw-r--r--   0        0        0     2667 2024-04-26 08:02:28.912058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt
+-rw-r--r--   0        0        0  6282865 2024-04-26 08:02:28.936058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map
+-rw-r--r--   0        0        0   240334 2024-04-26 08:02:28.936058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     1503 2024-04-26 08:02:28.944058 cognite_neat-0.75.6/cognite/neat/config.py
+-rw-r--r--   0        0        0     1227 2024-04-26 08:02:28.944058 cognite_neat-0.75.6/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-04-26 08:02:28.944058 cognite_neat-0.75.6/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-04-26 08:02:28.944058 cognite_neat-0.75.6/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-26 08:02:28.948058 cognite_neat-0.75.6/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14947 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14909 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23859 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2399 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2837 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40480 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22715 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12995 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3327 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14738 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36814 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5783 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2330 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7727 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19612 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1517 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1645 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    11893 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    13767 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    19900 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3038 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4090 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      408 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4057 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    10405 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12553 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6801 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11925 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7597 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7804 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7443 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     6987 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11085 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4074 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6158 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    15323 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     4492 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3346 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0     7493 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13763 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0     4893 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/_entity.py
+-rw-r--r--   0        0        0     7228 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0      522 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/__init__.py
+-rw-r--r--   0        0        0    11024 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_base.py
+-rw-r--r--   0        0        0    56198 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_dms_architect_rules.py
+-rw-r--r--   0        0        0    30789 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_dms_schema.py
+-rw-r--r--   0        0        0     2542 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_domain_rules.py
+-rw-r--r--   0        0        0    21577 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_information_rules.py
+-rw-r--r--   0        0        0     1299 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/__init__.py
+-rw-r--r--   0        0        0    12233 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_base.py
+-rw-r--r--   0        0        0    10295 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_field.py
+-rw-r--r--   0        0        0     6308 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_value.py
+-rw-r--r--   0        0        0       68 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11063 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6319 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2722 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12826 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26857 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    13659 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6568 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3015 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0      257 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0     5161 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_store.py
+-rw-r--r--   0        0        0    16874 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/io_steps.py
+-rw-r--r--   0        0        0    18678 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_exporter.py
+-rw-r--r--   0        0        0    10384 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_importer.py
+-rw-r--r--   0        0        0     4784 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_validator.py
+-rw-r--r--   0        0        0      274 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/__init__.py
+-rw-r--r--   0        0        0     3929 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
+-rw-r--r--   0        0        0    29416 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
+-rw-r--r--   0        0        0    27324 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_loader.py
+-rw-r--r--   0        0        0    12728 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_store.py
+-rw-r--r--   0        0        0     2361 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
+-rw-r--r--   0        0        0    20706 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
+-rw-r--r--   0        0        0    28111 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/rules_importer.py
+-rw-r--r--   0        0        0     3010 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    10467 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4540 2024-04-26 08:02:29.356060 cognite_neat-0.75.6/pyproject.toml
+-rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.75.6/PKG-INFO
```

### Comparing `cognite_neat-0.75.5/LICENSE` & `cognite_neat-0.75.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/README.md` & `cognite_neat-0.75.6/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/configuration.py` & `cognite_neat-0.75.6/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/data_classes/configuration.py` & `cognite_neat-0.75.6/cognite/neat/app/api/data_classes/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.75.6/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/explorer.py` & `cognite_neat-0.75.6/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.75.6/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.75.6/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.75.6/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.75.6/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.75.6/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.75.6/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.75.6/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.75.6/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.75.6/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.75.6/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/config.py` & `cognite_neat-0.75.6/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/constants.py` & `cognite_neat-0.75.6/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/exceptions.py` & `cognite_neat-0.75.6/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.75.6/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.75.6/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.75.6/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/exceptions.py` & `cognite_neat-0.75.6/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.75.6/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.75.6/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.75.6/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.75.6/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.75.6/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.75.6/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.75.6/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.75.6/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/exceptions.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_dexpi.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/__init__.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_asset_loader.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_base.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_exceptions.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/labels.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/models.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/rdf_to_dms.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/validator.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/__init__.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_base.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_graphdb_store.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_memory_store.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_oxigraph_store.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_oxrdflib.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/entity_matcher.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/transformer.py` & `cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/analysis.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/__init__.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-model.yaml` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/rules-template.xlsx` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/skos-rules.xlsx` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/wind-energy.owl` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exceptions.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/__init__.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_base.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_core/rules2labels.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2dms.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2excel.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2graphql.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2ontology.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2rules.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2triples.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_validation.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/__init__.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_base.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_dict2rules.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_dms2rules.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_graph2rules.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_json2rules.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_yaml2rules.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/models/_base.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/models/raw_rules.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/models/rdfpath.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/models/rules.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/legacy/rules/models/value_types.py` & `cognite_neat-0.75.6/cognite/neat/legacy/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/analysis/_base.py` & `cognite_neat-0.75.6/cognite/neat/rules/analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/analysis/_information_rules.py` & `cognite_neat-0.75.6/cognite/neat/rules/analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.75.6/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/exceptions.py` & `cognite_neat-0.75.6/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.75.6/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.75.6/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     TransformationLoader,
     ViewLoader,
 )
 
 from ._base import CDFExporter
 from ._models import UploadResult
 
-Component: TypeAlias = Literal["all", "spaces", "data_models", "views", "containers"]
+Component: TypeAlias = Literal["all", "spaces", "data_models", "views", "containers", "node_types"]
 
 
 class DMSExporter(CDFExporter[DMSSchema]):
     """Class for exporting rules object to CDF Data Model Storage (DMS).
 
     Args:
         export_components (frozenset[Literal["all", "spaces", "data_models", "views", "containers"]], optional):
@@ -95,15 +95,15 @@
         exclude = self._create_exclude_set()
         schema.to_zip(filepath, exclude=exclude)
 
     def _create_exclude_set(self):
         if "all" in self.export_components:
             exclude = set()
         else:
-            exclude = {"spaces", "data_models", "views", "containers"} - self.export_components
+            exclude = {"spaces", "data_models", "views", "containers", "node_types"} - self.export_components
         return exclude
 
     def export(self, rules: Rules) -> DMSSchema:
         if isinstance(rules, DMSRules):
             dms_rules = rules
         elif isinstance(rules, InformationRules):
             dms_rules = rules.as_dms_architect_rules()
@@ -114,20 +114,20 @@
             dms_rules.reference and dms_rules.metadata.external_id != dms_rules.reference.metadata.external_id
         )
         is_new_model = dms_rules.reference is None
         if is_new_model or is_solution_model:
             return dms_rules.as_schema(self.export_pipeline, self.instance_space)
 
         # This is an extension of an existing model.
-        reference_rules = cast(DMSRules, dms_rules.reference).copy(deep=True)
+        reference_rules = cast(DMSRules, dms_rules.reference).model_copy(deep=True)
         reference_schema = reference_rules.as_schema(self.export_pipeline)
 
         # Todo Move this to an appropriate location
         # Merging Reference with User Rules
-        combined_rules = dms_rules.copy(deep=True)
+        combined_rules = dms_rules.model_copy(deep=True)
         existing_containers = {container.class_ for container in combined_rules.containers or []}
         if combined_rules.containers is None:
             combined_rules.containers = SheetList[DMSContainer](data=[])
         for container in reference_rules.containers or []:
             if container.class_ not in existing_containers:
                 container.reference = None
                 combined_rules.containers.append(container)
```

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,19 @@
         styling: The styling to use for the Excel file. Defaults to "default". See below for details
             on the different styles.
         output_role: The role to use for the exported spreadsheet. If provided, the rules will be converted to
             this role formate before being written to excel. If not provided, the role from the rules will be used.
         new_model_id: The new model ID to use for the exported spreadsheet. This is only applicable if the input
             rules have 'is_reference' set. If provided, the model ID will be used to automatically create the
             new metadata sheet in the Excel file.
+        is_reference: If True, the rules are considered to be a reference model. The exported Excel file will
+            then contain empty sheets for the main rules and this data model will be dumped to the reference sheets.
+            This is useful when you are building a solution model based on an Enterprise model, then the
+            Enterprise model will serve as the reference model. It is also useful when you are extending an existing
+            model, then the existing model will serve as the reference model. Defaults to False.
 
     The following styles are available:
 
     - "none":    No styling is applied.
     - "minimal": Column widths are adjusted to fit the content, and the header row(s) is frozen.
     - "default": Minimal + headers are bold, increased size, and colored.
     - "maximal": Default + alternating row colors in the properties sheet for each class in addition to extra
@@ -50,21 +55,23 @@
     style_options = get_args(Style)
 
     def __init__(
         self,
         styling: Style = "default",
         output_role: RoleTypes | None = None,
         new_model_id: tuple[str, str, str] | None = None,
+        is_reference: bool = False,
     ):
         if styling not in self.style_options:
             raise ValueError(f"Invalid styling: {styling}. Valid options are {self.style_options}")
         self.styling = styling
         self._styling_level = self.style_options.index(styling)
         self.output_role = output_role
         self.new_model_id = new_model_id
+        self.is_reference = is_reference
 
     def export_to_file(self, rules: Rules, filepath: Path) -> None:
         """Exports transformation rules to excel file."""
         data = self.export(rules)
         try:
             data.save(filepath)
         finally:
@@ -75,15 +82,15 @@
         rules = self._convert_to_output_role(rules, self.output_role)
         workbook = Workbook()
         # Remove default sheet named "Sheet"
         workbook.remove(workbook["Sheet"])
 
         dumped_rules: dict[str, Any]
         dumped_reference_rules: dict[str, Any] | None = None
-        if rules.is_reference:
+        if self.is_reference:
             # Writes empty reference sheets
             dumped_rules = {
                 "Metadata": self._create_metadata_sheet_user_rules(rules),
             }
             dumped_rules["Metadata"]["role"] = (
                 self.output_role and self.output_role.value
             ) or rules.metadata.role.value
```

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.75.6/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,58 +16,51 @@
 
 class BaseImporter(ABC):
     """
     BaseImporter class which all importers inherit from.
     """
 
     @overload
-    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None, is_reference: bool = False) -> Rules:
+    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None) -> Rules:
         ...
 
     @overload
     def to_rules(
-        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None, is_reference: bool = False
+        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList]:
         ...
 
     @abstractmethod
     def to_rules(
-        self,
-        errors: Literal["raise", "continue"] = "continue",
-        role: RoleTypes | None = None,
-        is_reference: bool = False,
+        self, errors: Literal["raise", "continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList] | Rules:
         """
         Creates `Rules` object from the data for target role.
         """
         ...
 
     @classmethod
     def _to_output(
         cls,
         rules: Rules,
         issues: IssueList,
         errors: Literal["raise", "continue"] = "continue",
         role: RoleTypes | None = None,
-        is_reference: bool = False,
     ) -> tuple[Rules | None, IssueList] | Rules:
         """Converts the rules to the output format."""
 
         if rules.metadata.role is role or role is None:
             output = rules
         elif isinstance(rules, DMSRules) and role is RoleTypes.information_architect:
             output = rules.as_information_architect_rules()
         elif isinstance(rules, InformationRules) and role is RoleTypes.dms_architect:
             output = rules.as_dms_architect_rules()
         else:
             raise NotImplementedError(f"Role {role} is not supported for {type(rules).__name__} rules")
 
-        if is_reference:
-            output.is_reference = True
-
         if errors == "raise":
             return output
         else:
             return output, issues
 
     def _default_metadata(self):
         return {
```

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_dms2rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,28 +78,25 @@
     @classmethod
     def from_zip_file(cls, zip_file: str | Path) -> "DMSImporter":
         if Path(zip_file).suffix != ".zip":
             raise ValueError("File extension is not .zip")
         return cls(DMSSchema.from_zip(zip_file))
 
     @overload
-    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None, is_reference: bool = False) -> Rules:
+    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None) -> Rules:
         ...
 
     @overload
     def to_rules(
-        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None, is_reference: bool = False
+        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList]:
         ...
 
     def to_rules(
-        self,
-        errors: Literal["raise", "continue"] = "continue",
-        role: RoleTypes | None = None,
-        is_reference: bool = False,
+        self, errors: Literal["raise", "continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList] | Rules:
         if role is RoleTypes.domain_expert:
             raise ValueError(f"Role {role} is not supported for DMSImporter")
         issue_list = IssueList()
         data_model = self.schema.data_models[0]
 
         container_by_id = {container.as_id(): container for container in self.schema.containers}
@@ -206,15 +203,14 @@
         dms_rules = DMSRules(
             metadata=self.metadata or DMSMetadata.from_data_model(data_model),
             properties=properties,
             containers=SheetList[DMSContainer](
                 data=[DMSContainer.from_container(container) for container in self.schema.containers]
             ),
             views=SheetList[DMSView](data=[DMSView.from_view(view, data_model_view_ids) for view in self.schema.views]),
-            is_reference=is_reference,
         )
         output_rules: Rules
         if role is RoleTypes.information_architect:
             output_rules = dms_rules.as_information_architect_rules()
         else:
             output_rules = dms_rules
         if errors == "raise":
```

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,28 +115,25 @@
                         if isinstance(item, ValidationIssue):
                             issues.append(item)
                         else:
                             items.append(item)
         return cls(items, zip_file.stem, read_issues=issues)
 
     @overload
-    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None, is_reference: bool = False) -> Rules:
+    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None) -> Rules:
         ...
 
     @overload
     def to_rules(
-        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None, is_reference: bool = False
+        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList]:
         ...
 
     def to_rules(
-        self,
-        errors: Literal["raise", "continue"] = "continue",
-        role: RoleTypes | None = None,
-        is_reference: bool = False,
+        self, errors: Literal["raise", "continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList] | Rules:
         converter = _DTDLConverter(self._read_issues)
 
         converter.convert(self._items)
 
         metadata = self._default_metadata()
         metadata["schema"] = self._schema_completeness.value
@@ -157,8 +154,8 @@
             )
         if future.result == "failure":
             if errors == "continue":
                 return None, converter.issues
             else:
                 raise converter.issues.as_errors()
 
-        return self._to_output(rules, converter.issues, errors, role, is_reference)
+        return self._to_output(rules, converter.issues, errors, role)
```

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,28 +39,25 @@
     """
 
     def __init__(self, filepath: Path, make_compliant: bool = False):
         self.owl_filepath = filepath
         self.make_compliant = make_compliant
 
     @overload
-    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None, is_reference: bool = False) -> Rules:
+    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None) -> Rules:
         ...
 
     @overload
     def to_rules(
-        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None, is_reference: bool = False
+        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList]:
         ...
 
     def to_rules(
-        self,
-        errors: Literal["raise", "continue"] = "continue",
-        role: RoleTypes | None = None,
-        is_reference: bool = False,
+        self, errors: Literal["raise", "continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList] | Rules:
         graph = Graph()
         try:
             graph.parse(self.owl_filepath)
         except Exception as e:
             raise Exception(f"Could not parse owl file: {e}") from e
 
@@ -78,15 +75,15 @@
             "Properties": parse_owl_properties(graph, make_compliant=self.make_compliant),
         }
 
         if self.make_compliant:
             components = make_components_compliant(components)
 
         rules = InformationRules.model_validate(components)
-        return self._to_output(rules, IssueList(), errors, role, is_reference)
+        return self._to_output(rules, IssueList(), errors, role)
 
 
 def make_components_compliant(components: dict) -> dict:
     components = _add_missing_classes(components)
     components = _add_missing_value_types(components)
     components = _add_default_property_to_dangling_classes(components)
```

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,45 +148,39 @@
 
 
 class ExcelImporter(BaseImporter):
     def __init__(self, filepath: Path):
         self.filepath = filepath
 
     @overload
-    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None, is_reference: bool = False) -> Rules:
+    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None) -> Rules:
         ...
 
     @overload
     def to_rules(
         self,
         errors: Literal["continue"] = "continue",
         role: RoleTypes | None = None,
-        is_reference: bool = False,
     ) -> tuple[Rules | None, IssueList]:
         ...
 
     def to_rules(
-        self,
-        errors: Literal["raise", "continue"] = "continue",
-        role: RoleTypes | None = None,
-        is_reference: bool = False,
+        self, errors: Literal["raise", "continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList] | Rules:
         issue_list = IssueList(title=f"'{self.filepath.name}'")
         if not self.filepath.exists():
             issue_list.append(issues.spreadsheet_file.SpreadsheetNotFoundError(self.filepath))
             return self._return_or_raise(issue_list, errors)
 
-        user_result: ReadResult | None = None
-        if not is_reference:
-            user_result = SpreadsheetReader(issue_list, is_reference=False).read(self.filepath)
-            if user_result is None or issue_list.has_errors:
-                return self._return_or_raise(issue_list, errors)
+        user_result = SpreadsheetReader(issue_list, is_reference=False).read(self.filepath)
+        if user_result is None or issue_list.has_errors:
+            return self._return_or_raise(issue_list, errors)
 
         reference_result: ReadResult | None = None
-        if is_reference or (
+        if (
             user_result
             and user_result.role != RoleTypes.domain_expert
             and user_result.schema == SchemaCompleteness.extended
         ):
             reference_result = SpreadsheetReader(issue_list, is_reference=True).read(self.filepath)
             if issue_list.has_errors:
                 return self._return_or_raise(issue_list, errors)
@@ -226,15 +220,14 @@
             return self._return_or_raise(issue_list, errors)
 
         return self._to_output(
             rules,
             issue_list,
             errors=errors,
             role=role,
-            is_reference=is_reference,
         )
 
     @classmethod
     def _return_or_raise(cls, issue_list: IssueList, errors: Literal["raise", "continue"]) -> tuple[None, IssueList]:
         if errors == "raise":
             raise issue_list.as_errors()
         return None, issue_list
@@ -242,28 +235,25 @@
 
 class GoogleSheetImporter(BaseImporter):
     def __init__(self, sheet_id: str, skiprows: int = 1):
         self.sheet_id = sheet_id
         self.skiprows = skiprows
 
     @overload
-    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None, is_reference: bool = False) -> Rules:
+    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None) -> Rules:
         ...
 
     @overload
     def to_rules(
-        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None, is_reference: bool = False
+        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList]:
         ...
 
     def to_rules(
-        self,
-        errors: Literal["raise", "continue"] = "continue",
-        role: RoleTypes | None = None,
-        is_reference: bool = False,
+        self, errors: Literal["raise", "continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList] | Rules:
         local_import("gspread", "google")
         import gspread  # type: ignore[import]
 
         role = role or RoleTypes.domain_expert
         rules_model = cast(DomainRules | InformationRules | DMSRules, RULES_PER_ROLE[role])
 
@@ -280,8 +270,8 @@
         elif role == RoleTypes.information_architect:
             output = rules_model.model_validate(sheets)
         elif role == RoleTypes.dms_architect:
             output = rules_model.model_validate(sheets)
         else:
             raise ValueError(f"Role {role} is not valid.")
 
-        return self._to_output(output, IssueList(), errors=errors, role=role, is_reference=is_reference)
+        return self._to_output(output, IssueList(), errors=errors, role=role)
```

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.75.6/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,28 +41,25 @@
         if not filepath.is_file():
             return cls({}, [issues.fileread.FileNotAFileError(filepath)])
         elif filepath.suffix not in [".yaml", ".yml"]:
             return cls({}, [issues.fileread.InvalidFileFormatError(filepath, [".yaml", ".yml"])])
         return cls(yaml.safe_load(filepath.read_text()), filepaths=[filepath])
 
     @overload
-    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None, is_reference: bool = False) -> Rules:
+    def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None) -> Rules:
         ...
 
     @overload
     def to_rules(
-        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None, is_reference: bool = False
+        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList]:
         ...
 
     def to_rules(
-        self,
-        errors: Literal["raise", "continue"] = "continue",
-        role: RoleTypes | None = None,
-        is_reference: bool = False,
+        self, errors: Literal["raise", "continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList] | Rules:
         if any(issue for issue in self._read_issues if isinstance(issue, NeatValidationError)) or not self.raw_data:
             if errors == "raise":
                 raise self._read_issues.as_errors()
             return None, self._read_issues
         issue_list = IssueList(title="YAML Importer", issues=self._read_issues)
 
@@ -103,8 +100,8 @@
             rules = rules_model.model_validate(self.raw_data)
         if future.result == "failure":
             if errors == "continue":
                 return None, issue_list
             else:
                 raise issue_list.as_errors()
 
-        return self._to_output(rules, issue_list, errors, role, is_reference)
+        return self._to_output(rules, issue_list, errors, role)
```

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.75.6/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/issues/base.py` & `cognite_neat-0.75.6/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.75.6/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.75.6/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.75.6/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.75.6/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.75.6/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.75.6/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/_entity.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/_entity.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/rdfpath.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/rules/__init__.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_base.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_dms_architect_rules.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_dms_architect_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,14 @@
 
 class DMSRules(BaseRules):
     metadata: DMSMetadata = Field(alias="Metadata")
     properties: SheetList[DMSProperty] = Field(alias="Properties")
     views: SheetList[DMSView] = Field(alias="Views")
     containers: SheetList[DMSContainer] | None = Field(None, alias="Containers")
     reference: "DMSRules | None" = Field(None, alias="Reference")
-    is_reference: bool = False
 
     @model_validator(mode="after")
     def set_default_space_and_version(self) -> "DMSRules":
         default_space = self.metadata.space
         default_view_version = self.metadata.default_view_version
         for entity in self.properties:
             if entity.class_.prefix is Undefined or entity.class_.version is None:
@@ -579,15 +578,15 @@
             rules: DMSRules = self
         elif self.metadata.schema_ is SchemaCompleteness.extended:
             if not self.reference:
                 raise ValueError(
                     "The schema is set to 'extended', but no reference rules are provided to validate against"
                 )
             # This is an extension of the reference rules, we need to merge the two
-            rules = self.copy(deep=True)
+            rules = self.model_copy(deep=True)
             rules.properties.extend(self.reference.properties.data)
             existing_views = {view.view.as_id(False) for view in rules.views}
             rules.views.extend([view for view in self.reference.views if view.view.as_id(False) not in existing_views])
             if rules.containers and self.reference.containers:
                 existing_containers = {
                     container.container.as_id(self.metadata.space) for container in rules.containers.data
                 }
@@ -662,15 +661,14 @@
             containers.append(dumped)
 
         output = {
             "Metadata" if info.by_alias else "metadata": self.metadata.model_dump(**kwargs),
             "Properties" if info.by_alias else "properties": properties,
             "Views" if info.by_alias else "views": views,
             "Containers" if info.by_alias else "containers": containers,
-            "is_reference": self.is_reference,
         }
         if self.reference is not None:
             output["Reference" if info.by_alias else "reference"] = self.reference.model_dump(**kwargs)
         return output
 
     def as_schema(self, include_pipeline: bool = False, instance_space: str | None = None) -> DMSSchema:
         return _DMSExporter(include_pipeline, instance_space).to_schema(self)
@@ -678,15 +676,15 @@
     def as_information_architect_rules(self) -> "InformationRules":
         return _DMSRulesConverter(self).as_information_architect_rules()
 
     def as_domain_expert_rules(self) -> DomainRules:
         return _DMSRulesConverter(self).as_domain_rules()
 
     def reference_self(self) -> Self:
-        new_rules = self.copy(deep=True)
+        new_rules = self.model_copy(deep=True)
         for prop in new_rules.properties:
             prop.reference = ReferenceEntity(
                 prefix=prop.view.prefix, suffix=prop.view.suffix, version=prop.view.version, property_=prop.property_
             )
         view: DMSView
         for view in new_rules.views:
             view.reference = ReferenceEntity(
@@ -1132,15 +1130,14 @@
             )
 
         return InformationRules(
             metadata=metadata,
             properties=SheetList[InformationProperty](data=properties),
             classes=SheetList[InformationClass](data=classes),
             reference=self.dms.reference and self.dms.reference.as_information_architect_rules(),  # type: ignore[arg-type]
-            is_reference=self.dms.is_reference,
         )
 
     @classmethod
     def _get_class_reference(cls, view: DMSView) -> ReferenceEntity | None:
         parents_other_namespace = [parent for parent in view.implements or [] if parent.prefix != view.class_.prefix]
         if len(parents_other_namespace) == 0:
             return None
```

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_dms_schema.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_dms_schema.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_domain_rules.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_domain_rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
 
 class DomainRules(RuleModel):
     metadata: DomainMetadata = Field(alias="Metadata")
     properties: SheetList[DomainProperty] = Field(alias="Properties")
     classes: SheetList[DomainClass] | None = Field(None, alias="Classes")
     reference: "DomainRules | None" = Field(None, alias="Reference")
-    is_reference: bool = False
 
     @model_serializer(mode="plain", when_used="always")
     def domain_rules_serializer(self, info: SerializationInfo) -> dict[str, Any]:
         kwargs = vars(info)
         output: dict[str, Any] = {
             "Metadata" if info.by_alias else "metadata": self.metadata.model_dump(**kwargs),
             "Properties" if info.by_alias else "properties": [prop.model_dump(**kwargs) for prop in self.properties],
@@ -61,8 +60,8 @@
             output["Classes" if info.by_alias else "classes"] = [
                 cls.model_dump(**kwargs) for cls in self.classes or []
             ] or None
         return output
 
     def reference_self(self) -> "DomainRules":
         """DomainRules does not have reference field, so it returns a copy of itself."""
-        return self.copy(deep=True)
+        return self.model_copy(deep=True)
```

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_information_rules.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_information_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,14 @@
 
 class InformationRules(RuleModel):
     metadata: InformationMetadata = Field(alias="Metadata")
     properties: SheetList[InformationProperty] = Field(alias="Properties")
     classes: SheetList[InformationClass] = Field(alias="Classes")
     prefixes: dict[str, Namespace] = Field(default_factory=lambda: PREFIXES.copy())
     reference: "InformationRules | None" = Field(None, alias="Reference")
-    is_reference: bool = False
 
     @field_validator("prefixes", mode="before")
     def parse_str(cls, values: Any) -> Any:
         if isinstance(values, dict):
             return {key: Namespace(value) if isinstance(value, str) else value for key, value in values.items()}
         return values
 
@@ -351,15 +350,15 @@
     def as_domain_rules(self) -> DomainRules:
         return _InformationRulesConverter(self).as_domain_rules()
 
     def as_dms_architect_rules(self) -> "DMSRules":
         return _InformationRulesConverter(self).as_dms_architect_rules()
 
     def reference_self(self) -> "InformationRules":
-        new_self = self.copy(deep=True)
+        new_self = self.model_copy(deep=True)
         for prop in new_self.properties:
             prop.reference = ReferenceEntity(
                 prefix=prop.class_.prefix,
                 suffix=prop.class_.suffix,
                 version=prop.class_.version,
                 property_=prop.property_,
             )
@@ -447,15 +446,14 @@
             metadata=metadata,
             properties=SheetList[DMSProperty](
                 data=[prop for prop_set in properties_by_class.values() for prop in prop_set]
             ),
             views=SheetList[DMSView](data=views),
             containers=SheetList[DMSContainer](data=containers),
             reference=self.information.reference and self.information.reference.as_dms_architect_rules(),  # type: ignore[arg-type]
-            is_reference=self.information.is_reference,
         )
 
     @classmethod
     def _as_dms_property(cls, prop: InformationProperty) -> "DMSProperty":
         """This creates the first"""
 
         from ._dms_architect_rules import DMSProperty
```

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/__init__.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_base.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_field.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_value.py` & `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_value.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/utils/cdf.py` & `cognite_neat-0.75.6/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/utils/exceptions.py` & `cognite_neat-0.75.6/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.75.6/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/utils/text.py` & `cognite_neat-0.75.6/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/utils/utils.py` & `cognite_neat-0.75.6/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/utils/xml.py` & `cognite_neat-0.75.6/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.75.6/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/base.py` & `cognite_neat-0.75.6/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.75.6/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.75.6/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.75.6/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.75.6/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.75.6/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.75.6/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.75.6/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.75.6/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.75.6/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.75.6/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.75.6/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/manager.py` & `cognite_neat-0.75.6/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.75.6/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.75.6/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/model.py` & `cognite_neat-0.75.6/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_extractor.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_loader.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_store.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/io_steps.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_exporter.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_importer.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         # if role is None, it will be inferred from the rules file
         role = self.configs.get("Role")
         role_enum = None
         if role != "infer" and role is not None:
             role_enum = RoleTypes[role]
 
         excel_importer = importers.ExcelImporter(rules_file_path)
-        rules, issues = excel_importer.to_rules(role=role_enum, errors="continue")
+        rules, issues = excel_importer.to_rules(errors="continue", role=role_enum)
 
         if rules is None:
             output_dir = self.data_store_path / Path("staging")
             report_writer = FORMATTER_BY_NAME[self.configs["Report formatter"]]()
             report_writer.write_to_file(issues, file_or_dir_path=output_dir)
             report_file = report_writer.default_file_name
             error_text = (
@@ -147,15 +147,15 @@
         # if role is None, it will be inferred from the rules file
         role = self.configs.get("Role")
         role_enum = None
         if role != "infer" and role is not None:
             role_enum = RoleTypes[role]
 
         ontology_importer = importers.OWLImporter(filepath=rules_file_path, make_compliant=make_compliant)
-        rules, issues = ontology_importer.to_rules(role=role_enum, errors="continue")
+        rules, issues = ontology_importer.to_rules(errors="continue", role=role_enum)
 
         if rules is None:
             output_dir = self.data_store_path / Path("staging")
             report_writer = FORMATTER_BY_NAME[self.configs["Report formatter"]]()
             report_writer.write_to_file(issues, file_or_dir_path=output_dir)
             report_file = report_writer.default_file_name
             error_text = (
@@ -192,21 +192,14 @@
         ),
         Configurable(
             name="Role",
             value="infer",
             label="For what role Rules are intended?",
             options=["infer", *RoleTypes.__members__.keys()],
         ),
-        Configurable(
-            name="Reference",
-            value="false",
-            label="Whether the imported rules are a reference model or not. This is "
-            "used when you want to extend an existing model and this is the model that is being extended from.",
-            options=["true", "false"],
-        ),
     ]
 
     def run(self, cdf_client: CogniteClient) -> (FlowMessage, MultiRuleData):  # type: ignore[syntax, override]
         if self.configs is None or self.data_store_path is None:
             raise StepNotInitialized(type(self).__name__)
 
         datamodel_id_str = self.configs.get("Data model id")
@@ -218,25 +211,23 @@
         if datamodel_entity.space is Undefined:
             error_text = (
                 f"Data model id should be in the format 'my_space:my_data_model(version=1)' "
                 f"or 'my_space:my_data_model', failed to parse space from {datamodel_id_str}"
             )
             return FlowMessage(error_text=error_text, step_execution_status=StepExecutionStatus.ABORT_AND_FAIL)
 
-        is_reference = self.configs.get("Reference", "false") == "true"
-
         dms_importer = importers.DMSImporter.from_data_model_id(cdf_client, datamodel_entity.as_id())
 
         # if role is None, it will be inferred from the rules file
         role = self.configs.get("Role")
         role_enum = None
         if role != "infer" and role is not None:
             role_enum = RoleTypes[role]
 
-        rules, issues = dms_importer.to_rules(role=role_enum, errors="continue", is_reference=is_reference)
+        rules, issues = dms_importer.to_rules(errors="continue", role=role_enum)
 
         if rules is None:
             output_dir = self.data_store_path / Path("staging")
             report_writer = FORMATTER_BY_NAME[self.configs["Report formatter"]]()
             report_writer.write_to_file(issues, file_or_dir_path=output_dir)
             report_file = report_writer.default_file_name
             error_text = (
```

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_validator.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_extractor.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_loader.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_store.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_transformer.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/rules_exporter.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/rules_importer.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.75.6/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/tasks.py` & `cognite_neat-0.75.6/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/cognite/neat/workflows/triggers.py` & `cognite_neat-0.75.6/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.5/pyproject.toml` & `cognite_neat-0.75.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.75.5"
+version = "0.75.6"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.75.5/PKG-INFO` & `cognite_neat-0.75.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.75.5
+Version: 0.75.6
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

