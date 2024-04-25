# Comparing `tmp/relationalai-0.2.4.tar.gz` & `tmp/relationalai-0.2.5.tar.gz`

## Comparing `relationalai-0.2.4.tar` & `relationalai-0.2.5.tar`

### file list

```diff
@@ -1,441 +1,449 @@
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.4/README.md
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 relationalai-0.2.4/.github/actions/end-to-end/action.yml
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 relationalai-0.2.4/.github/workflows/end-to-end.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 relationalai-0.2.4/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/README.md
--rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/getting_started.md
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/_old/quickstart.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/README.md
--rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/configuration/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Property.md
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/README.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/enter__.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/exit__.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/iter__.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/model.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/results.md
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/ContextSelect/README.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/ContextSelect/add.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/ContextSelect/call__.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/ContextSelect/getattribute__.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Instance/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Instance/persist.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Instance/set.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Instance/unpersist.md
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/InstanceProperty/README.md
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/InstanceProperty/or_.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/Type.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/found.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/name.md
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/not_found.md
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/ordered_choice.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/query.md
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/read.md
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/rule.md
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/scope.md
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/union.md
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/README.md
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/add__.md
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/enter__.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/eq__.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/exit__.md
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/ge__.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/getattribute__.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/gt__.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/le__.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/lt__.md
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/mul__.md
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/ne__.md
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/pow__.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/radd__.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/rmul__.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/rpow__.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/rsub__.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/rtruediv__.md
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/sub__.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/truediv__.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/README.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/add.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/call__.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/extend.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/model.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/name.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/or__.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/PrimaryKey.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/README.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/Snowflake.md
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/README.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/Vars.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/alias.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/avg.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/count.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/max.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/min.md
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/rank_asc.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/rank_desc.md
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/sum.md
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/README.md
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/README.md
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_degree.md
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/degree.md
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/indegree.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/infomap.md
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/label_propagation.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/louvain.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/num_edges.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/num_nodes.md
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/outdegree.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/pagerank.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/README.md
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/add.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/call__.md
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/extend.md
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/set.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/to.md
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/Edge.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/Node.md
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/README.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/compute.md
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/fetch.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/id.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/model.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/undirected.md
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/visualize.md
--rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
--rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/README.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/concat.md
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/contains.md
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/ends_with.md
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/join.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/length.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/lowercase.md
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/replace.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/uppercase.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/faq/README.md
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/faq/engines.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/cdc.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/custom_snowflake_connection.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/fraud.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/graph_algos.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/load_raw.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/nested.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/or_types.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/remote_load_csv.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/requirements.txt
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/simple_recursion.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/simple_streamlit.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/solver.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/weighted_graph_algos.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/README.md
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/articles_graph.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/articles_graph_with_nlp.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/pyproject.toml
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/utils.py
--rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/daily_articles/04_04_2024.json
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/data/transactions.csv
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/ev_penetration/ev_penetration.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/ev_penetration/ev_penetration_csv.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/ev_penetration/state_stats.csv
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/imdb/README.md
--rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/imdb/imdb.csv
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/imdb/imdb.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/rel/foo.rel
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/rel/solver.rel
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/social-money-network/SF_pagerank.ipynb
--rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/social-money-network/Simulation-and-SF-Upload.ipynb
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/social-money-network/snowflake_pagerank.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/README.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/index.html
--rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/package-lock.json
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/package.json
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/tsconfig.json
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/vite.config.ts
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/.storybook/main.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/.storybook/preview-body.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/.storybook/preview-head.html
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/.storybook/preview.ts
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/App.styl
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/App.tsx
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/Selection.tsx
--rw-r--r--   0        0        0    10577 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/debugger_client.ts
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/index.css
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/index.tsx
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/logo.svg
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/util.styl
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/util.ts
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/ws.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/assets/favicon.png
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/EventList.styl
--rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/EventList.tsx
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/EventViewer.styl
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/EventViewer.tsx
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Sidebar.styl
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Sidebar.tsx
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.stories.tsx
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.styl
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.tsx
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/base.styl
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/base.tsx
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/index.tsx
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Accordion.stories.tsx
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Accordion.styl
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Accordion.tsx
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Button.styl
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Button.tsx
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Code.styl
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Code.tsx
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.stories.tsx
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.styl
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.tsx
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Field.stories.tsx
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Field.styl
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Field.tsx
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Icon.styl
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Icon.tsx
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.stories.tsx
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.styl
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.tsx
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.stories.tsx
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.styl
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.tsx
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/branch-improved.json
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/branch.json
--rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/fraud.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/index.ts
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/not_found.json
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/simple.json
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/union.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/types/json.d.ts
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/types/jsx.d.ts
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/types/mech.d.ts
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/__init__.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/emit.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/exec.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/__init__.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/compiler.py
--rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/debugging.py
--rw-r--r--   0        0        0    44988 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/dsl.py
--rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/errors.py
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/metagen.py
--rw-r--r--   0        0        0    27821 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/rel.py
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/rel2.py
--rw-r--r--   0        0        0    13261 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/rel_emitter.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/rel_utils.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/analysis/mechanistic.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/client.py
--rw-r--r--   0        0        0    17958 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/config.py
--rw-r--r--   0        0        0    36413 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/types.py
--rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/loaders/loader.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/loaders/types.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/std/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/std/aggregates.py
--rw-r--r--   0        0        0    15314 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/std/graphs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/std/strings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    52409 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/debugger_server.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/notes
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/util/snowflake_logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/README.md
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/conftest.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_graph_visualize.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_snapshots.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/agg_ordering.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/bool.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/bottom.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/export.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/first.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/multi_valued.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/not_found.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/persist.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/smoke.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/strings.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/top.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/union.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/weighted_graphs.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/basics.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/centrality.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/community.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/degree.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/link_prediction.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/similarity.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/test_core.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/test_examples.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/basic/smoketest.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/found/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/test/query0.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/init-cli/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/init-cli/azure_basic.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/init-cli/common.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.4/.gitignore
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/pypi/README.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.5/README.md
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 relationalai-0.2.5/.github/actions/end-to-end/action.yml
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 relationalai-0.2.5/.github/workflows/end-to-end.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 relationalai-0.2.5/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/README.md
+-rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/getting_started.md
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/README.md
+-rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/configuration/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Property.md
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/README.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/enter__.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/exit__.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/iter__.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/model.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/results.md
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/ContextSelect/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/ContextSelect/add.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/ContextSelect/call__.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/ContextSelect/getattribute__.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Instance/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Instance/persist.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Instance/set.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Instance/unpersist.md
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/InstanceProperty/README.md
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/InstanceProperty/or_.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/README.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/Type.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/found.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/name.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/not_found.md
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/ordered_choice.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/query.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/read.md
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/rule.md
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/scope.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/union.md
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/README.md
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/add__.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/enter__.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/eq__.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/exit__.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/ge__.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/getattribute__.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/gt__.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/le__.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/lt__.md
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/mul__.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/ne__.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/pow__.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/radd__.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/rmul__.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/rpow__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/rsub__.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/rtruediv__.md
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/sub__.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/truediv__.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/README.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/add.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/call__.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/extend.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/model.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/name.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/or__.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/PrimaryKey.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/README.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/Snowflake.md
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/README.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/Vars.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/alias.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/avg.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/count.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/max.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/min.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/rank_asc.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/rank_desc.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/sum.md
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/README.md
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/README.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_degree.md
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/degree.md
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/indegree.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/infomap.md
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/is_connected.md
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/is_reachable.md
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/label_propagation.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/louvain.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/num_edges.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/num_nodes.md
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/outdegree.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/pagerank.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/reachable_from.md
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/README.md
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/add.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/call__.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/extend.md
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/set.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/to.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/Edge.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/Node.md
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/README.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/compute.md
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/fetch.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/id.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/model.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/undirected.md
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/visualize.md
+-rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
+-rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/README.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/concat.md
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/contains.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/ends_with.md
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/join.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/length.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/lowercase.md
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/replace.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/uppercase.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/faq/README.md
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/faq/engines.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/cdc.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/custom_snowflake_connection.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/fraud.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/graph_algos.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/load_raw.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/nested.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/or_types.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/remote_load_csv.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/requirements.txt
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/simple_recursion.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/simple_streamlit.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/solver.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/weighted_graph_algos.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/README.md
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/articles_graph.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/articles_graph_with_nlp.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/pyproject.toml
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/utils.py
+-rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/daily_articles/04_04_2024.json
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/data/transactions.csv
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/ev_penetration/ev_penetration.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/ev_penetration/ev_penetration_csv.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/ev_penetration/state_stats.csv
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/imdb/README.md
+-rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/imdb/imdb.csv
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/imdb/imdb.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/rel/foo.rel
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/rel/solver.rel
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/social-money-network/SF_pagerank.ipynb
+-rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/social-money-network/Simulation-and-SF-Upload.ipynb
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/social-money-network/snowflake_pagerank.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/index.html
+-rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/package-lock.json
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/package.json
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/tsconfig.json
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/vite.config.ts
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/.storybook/main.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/.storybook/preview-body.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/.storybook/preview-head.html
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/.storybook/preview.ts
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/App.styl
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/App.tsx
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/Selection.tsx
+-rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/debugger_client.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/index.css
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/index.tsx
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/logo.svg
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/util.styl
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/util.ts
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/ws.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/assets/favicon.png
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/EventList.styl
+-rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/EventList.tsx
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/EventViewer.styl
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/EventViewer.tsx
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Sidebar.styl
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.stories.tsx
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.styl
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.tsx
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/base.styl
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/base.tsx
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/index.tsx
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Accordion.stories.tsx
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Accordion.styl
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Accordion.tsx
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Button.styl
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Button.tsx
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Code.styl
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Code.tsx
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.stories.tsx
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.styl
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.tsx
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Field.stories.tsx
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Field.styl
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Field.tsx
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Icon.styl
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Icon.tsx
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.stories.tsx
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.styl
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.tsx
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.stories.tsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.styl
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.tsx
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/branch-improved.json
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/branch.json
+-rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/fraud.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/index.ts
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/not_found.json
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/simple.json
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/union.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/types/json.d.ts
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/types/jsx.d.ts
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/types/mech.d.ts
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/emit.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/exec.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/compiler.py
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/debugging.py
+-rw-r--r--   0        0        0    45835 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/dsl.py
+-rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    27896 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/rel.py
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/rel2.py
+-rw-r--r--   0        0        0    13261 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/rel_emitter.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/rel_utils.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/analysis/mechanistic.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0    17970 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0    36499 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/types.py
+-rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/loaders/loader.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/loaders/types.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/std/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/std/aggregates.py
+-rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/std/graphs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/std/strings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    50224 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/debugger_server.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/notes
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/util/snowflake_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/README.md
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/conftest.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_graph_visualize.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_snapshots.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/agg_ordering.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/bool.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/bottom.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/export.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/first.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/multi_valued.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/not_found.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/out_of_context.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/persist.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/smoke.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/strings.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/top.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/union.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/weighted_graphs.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/basics.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/centrality.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/community.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/connectivity.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/degree.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/link_prediction.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/similarity.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/test_core.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/test_examples.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/basic/smoketest.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/found/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/test/query0.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/init-cli/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/init-cli/azure_basic.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/init-cli/common.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/pypi/README.md
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.5/PKG-INFO
```

### Comparing `relationalai-0.2.4/README.md` & `relationalai-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/.github/actions/end-to-end/action.yml` & `relationalai-0.2.5/.github/actions/end-to-end/action.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/.github/workflows/end-to-end.yml` & `relationalai-0.2.5/.github/workflows/end-to-end.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/.github/workflows/publish-to-pypi.yml` & `relationalai-0.2.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/.github/workflows/ruff.yml` & `relationalai-0.2.5/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/getting_started.md` & `relationalai-0.2.5/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.2.5/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/_old/metamodel.md` & `relationalai-0.2.5/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/_old/python_dsl.md` & `relationalai-0.2.5/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/_old/quickstart.md` & `relationalai-0.2.5/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/cli/README.md` & `relationalai-0.2.5/docs/api_reference/cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/configuration/README.md` & `relationalai-0.2.5/docs/api_reference/configuration/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Expression.md` & `relationalai-0.2.5/docs/api_reference/python/Expression.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Property.md` & `relationalai-0.2.5/docs/api_reference/python/Property.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/README.md` & `relationalai-0.2.5/docs/api_reference/python/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -82,28 +82,40 @@
 - [`aggregates.rank_desc()`](./std/aggregates/rank_desc.md)
 - [`aggregates.sum()`](./std/aggregates/sum.md)
 
 ### [`relationalai.std.graphs`](./std/graphs/README.md)
 
 - [`graphs.Compute`](./std/graphs/Compute/README.md)
   - [`graphs.Compute.adamic_adar()`](./std/graphs/Compute/adamic_adar.md)
+  - [`graphs.Compute.avg_degree()`](./std/graphs/Compute/avg_degree.md)
+  - [`graphs.Compute.avg_indegree()`](./std/graphs/Compute/avg_indegree.md)
+  - [`graphs.Compute.avg_outdegree()`](./std/graphs/Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./std/graphs/Compute/betweeness_centrality.md)
   - [`graphs.Compute.cosine_similarity()`](./std/graphs/Compute/cosine_similarity.md)
   - [`graphs.Compute.common_neighbor()`](./std/graphs/Compute/common_neighbor.md)
   - [`graphs.Compute.degree()`](./std/graphs/Compute/degree.md)
   - [`graphs.Compute.degree_centrality()`](./std/graphs/Compute/degree_centrality.md)
   - [`graphs.Compute.eigenvector_centrality()`](./std/graphs/Compute/eigenvector_centrality.md)
   - [`graphs.Compute.num_edges()`](./std/graphs//Compute/num_edges.md)
   - [`graphs.Compute.indegree()`](./std/graphs/Compute/indegree.md)
+  - [`graphs.Compute.is_connected()`](./std/graphs/Compute/is_connected.md)
+  - [`graphs.Compute.is_reachable()`](./std/graphs/Compute/is_reachable.md)
   - [`graphs.Compute.label_propagation()`](./std/graphs/Compute/label_propagation.md)
   - [`graphs.Compute.louvain()`](./std/graphs/Compute/louvain.md)
+  - [`graphs.Compute.max_degree()`](./std/graphs/Compute/max_degree.md)
+  - [`graphs.Compute.max_indegree()`](./std/graphs/Compute/max_indegree.md)
+  - [`graphs.Compute.max_outdegree()`](./std/graphs/Compute/max_outdegree.md)
+  - [`graphs.Compute.min_degree()`](./std/graphs/Compute/min_degree.md)
+  - [`graphs.Compute.min_indegree()`](./std/graphs/Compute/min_indegree.md)
+  - [`graphs.Compute.min_outdegree()`](./std/graphs/Compute/min_outdegree.md)
   - [`graphs.Compute.num_nodes()`](./std//graphs//Compute/num_nodes.md)
   - [`graphs.Compute.outdegree()`](./std/graphs/Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./std/graphs/Compute/pagerank.md)
   - [`graphs.Compute.preferential_attachment()`](./std/graphs/Compute/preferential_attachment.md)
+  - [`graphs.Compute.reachable_from()`](./std/graphs/Compute/reachable_from.md)
   - [`graphs.Compute.weakly_connected_component()`](./std/graphs/Compute/weakly_connected_component.md)
   - [`graphs.Compute.weighted_degree_centrality()`](./std/graphs/Compute/weighted_degree_centrality.md)
 - [`graphs.Edge`](./std/graphs/Edge/README.md)
   - [`graphs.Edge.add()`](./std/graphs/Edge/add.md)
   - [`graphs.Edge.extend()`](./std/graphs/Edge/extend.md)
 - [`graphs.EdgeInstance`](./std/graphs/EdgeInstance/README.md)
   - [`graphs.EdgeInstance.from_`](./std/graphs/EdgeInstance/from_.md)
```

### Comparing `relationalai-0.2.4/docs/api_reference/python/Context/README.md` & `relationalai-0.2.5/docs/api_reference/python/Context/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Context/enter__.md` & `relationalai-0.2.5/docs/api_reference/python/Context/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Context/exit__.md` & `relationalai-0.2.5/docs/api_reference/python/Context/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Context/iter__.md` & `relationalai-0.2.5/docs/api_reference/python/Context/iter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Context/model.md` & `relationalai-0.2.5/docs/api_reference/python/Context/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Context/results.md` & `relationalai-0.2.5/docs/api_reference/python/Context/results.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/ContextSelect/README.md` & `relationalai-0.2.5/docs/api_reference/python/ContextSelect/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/ContextSelect/add.md` & `relationalai-0.2.5/docs/api_reference/python/ContextSelect/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/ContextSelect/call__.md` & `relationalai-0.2.5/docs/api_reference/python/ContextSelect/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/ContextSelect/getattribute__.md` & `relationalai-0.2.5/docs/api_reference/python/ContextSelect/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Instance/README.md` & `relationalai-0.2.5/docs/api_reference/python/Instance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Instance/persist.md` & `relationalai-0.2.5/docs/api_reference/python/Instance/persist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Instance/set.md` & `relationalai-0.2.5/docs/api_reference/python/Instance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Instance/unpersist.md` & `relationalai-0.2.5/docs/api_reference/python/Instance/unpersist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/InstanceProperty/README.md` & `relationalai-0.2.5/docs/api_reference/python/InstanceProperty/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/InstanceProperty/or_.md` & `relationalai-0.2.5/docs/api_reference/python/InstanceProperty/or_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Model/README.md` & `relationalai-0.2.5/docs/api_reference/python/Model/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Model/Type.md` & `relationalai-0.2.5/docs/api_reference/python/Model/Type.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Model/found.md` & `relationalai-0.2.5/docs/api_reference/python/Model/found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Model/not_found.md` & `relationalai-0.2.5/docs/api_reference/python/Model/not_found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Model/ordered_choice.md` & `relationalai-0.2.5/docs/api_reference/python/Model/ordered_choice.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Model/query.md` & `relationalai-0.2.5/docs/api_reference/python/Model/query.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Model/read.md` & `relationalai-0.2.5/docs/api_reference/python/Model/read.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Model/rule.md` & `relationalai-0.2.5/docs/api_reference/python/Model/rule.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Model/scope.md` & `relationalai-0.2.5/docs/api_reference/python/Model/scope.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Model/union.md` & `relationalai-0.2.5/docs/api_reference/python/Model/union.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/README.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/add__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/add__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/enter__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/eq__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/eq__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/exit__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/ge__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/ge__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/getattribute__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/gt__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/gt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/le__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/le__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/lt__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/lt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/mul__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/mul__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/ne__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/ne__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/pow__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/pow__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/sub__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/sub__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Producer/truediv__.md` & `relationalai-0.2.5/docs/api_reference/python/Producer/truediv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Type/README.md` & `relationalai-0.2.5/docs/api_reference/python/Type/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Type/add.md` & `relationalai-0.2.5/docs/api_reference/python/Type/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Type/call__.md` & `relationalai-0.2.5/docs/api_reference/python/Type/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Type/extend.md` & `relationalai-0.2.5/docs/api_reference/python/Type/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/Type/or__.md` & `relationalai-0.2.5/docs/api_reference/python/Type/or__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/clients/README.md` & `relationalai-0.2.5/docs/api_reference/python/clients/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/PrimaryKey.md` & `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/PrimaryKey.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/README.md` & `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/Snowflake.md` & `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/Snowflake.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md` & `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md` & `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md` & `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md` & `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/README.md` & `relationalai-0.2.5/docs/api_reference/python/std/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,33 +19,37 @@
 
 - [`graphs.Compute`](./graphs/Compute/README.md)
   - [`graphs.Compute.adamic_adar()`](./graphs/Compute/adamic_adar.md)
   - [`graphs.Compute.avg_degree()`](./graphs/Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./graphs/Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./graphs/Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./graphs/Compute/betweeness_centrality.md)
+  - [`graphs.Compute.common_neighbor()`](./graphs/Compute/common_neighbor.md)
   - [`graphs.Compute.cosine_similarity()`](./graphs/Compute/cosine_similarity.md)
   - [`graphs.Compute.common_neighbor()`](./graphs/Compute/common_neighbor.md)
   - [`graphs.Compute.degree()`](./graphs/Compute/degree.md)
   - [`graphs.Compute.degree_centrality()`](./graphs/Compute/degree_centrality.md)
   - [`graphs.Compute.eigenvector_centrality()`](./graphs/Compute/eigenvector_centrality.md)
+  - [`graphs.Compute.is_connected()`](./graphs/Compute/is_connected.md)
+  - [`graphs.Compute.is_reachable()`](./graphs/Compute/is_reachable.md)
   - [`graphs.Compute.num_edges()`](./graphs/Compute/num_edges.md)
   - [`graphs.Compute.indegree()`](./graphs/Compute/indegree.md)
   - [`graphs.Compute.label_propagation()`](./graphs/Compute/label_propagation.md)
   - [`graphs.Compute.louvain()`](./graphs/Compute/louvain.md)
   - [`graphs.Compute.max_degree()`](./graphs/Compute/max_degree.md)
   - [`graphs.Compute.max_indegree()`](./graphs/Compute/max_indegree.md)
   - [`graphs.Compute.max_outdegree()`](./graphs/Compute/max_outdegree.md)
   - [`graphs.Compute.min_degree()`](./graphs/Compute/min_degree.md)
   - [`graphs.Compute.min_indegree()`](./graphs/Compute/min_indegree.md)
   - [`graphs.Compute.min_outdegree()`](./graphs/Compute/min_outdegree.md)
   - [`graphs.Compute.num_nodes()`](./graphs/Compute/num_nodes.md)
   - [`graphs.Compute.outdegree()`](./graphs/Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./graphs/Compute/pagerank.md)
   - [`graphs.Compute.preferential_attachment()`](./graphs/Compute/preferential_attachment.md)
+  - [`graphs.Compute.reachable_from()`](./graphs/Compute/reachable_from.md)
   - [`graphs.Compute.weakly_connected_component()`](./graphs/Compute/weakly_connected_component.md)
   - [`graphs.Compute.weighted_degree_centrality()`](./graphs/Compute/weighted_degree_centrality.md)
 - [`graphs.Edge`](./graphs/Edge/README.md)
   - [`graphs.Edge.__call__()`](./graphs/Edge/call__.md)
   - [`graphs.Edge.add()`](./graphs/Edge/add.md)
   - [`graphs.Edge.extend()`](./graphs/Edge/extend.md)
 - [`graphs.EdgeInstance`](./graphs/EdgeInstance/README.md)
```

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/Vars.md` & `relationalai-0.2.5/docs/api_reference/python/std/Vars.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/alias.md` & `relationalai-0.2.5/docs/api_reference/python/std/alias.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/aggregates/README.md` & `relationalai-0.2.5/docs/api_reference/python/std/aggregates/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/aggregates/avg.md` & `relationalai-0.2.5/docs/api_reference/python/std/aggregates/avg.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/aggregates/count.md` & `relationalai-0.2.5/docs/api_reference/python/std/aggregates/count.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/aggregates/max.md` & `relationalai-0.2.5/docs/api_reference/python/std/aggregates/max.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/aggregates/min.md` & `relationalai-0.2.5/docs/api_reference/python/std/aggregates/min.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/aggregates/rank_asc.md` & `relationalai-0.2.5/docs/api_reference/python/std/aggregates/rank_asc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/aggregates/rank_desc.md` & `relationalai-0.2.5/docs/api_reference/python/std/aggregates/rank_desc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/aggregates/sum.md` & `relationalai-0.2.5/docs/api_reference/python/std/aggregates/sum.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/README.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 [graphs](./Graph/README.md) from objects in a [model](../../Model/README.md) and doing graph analytics.
 
 - [`graphs.Compute`](./Compute/README.md)
   - [`graphs.Compute.avg_degree()`](./Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./Compute/betweeness_centrality.md)
+  - [`graphs.Compute.common_neighbor()`](./Compute/common_neighbor.md)
   - [`graphs.Compute.cosine_similarity()`](./Compute/cosine_similarity.md)
   - [`graphs.Compute.degree()`](./Compute/degree.md)
   - [`graphs.Compute.degree_centrality()`](./Compute/degree_centrality.md)
   - [`graphs.Compute.eigenvector_centrality()`](./Compute/eigenvector_centrality.md)
   - [`graph.Compute.indegree()`](./Compute/indegree.md)
+  - [`graphs.Compute.is_connected()`](./Compute/is_connected.md)
+  - [`graphs.Compute.is_reachable()`](./Compute/is_reachable.md)
   - [`graphs.Compute.label_propagation()`](./Compute/label_propagation.md)
   - [`graphs.Compute.louvain()`](./Compute/louvain.md)
   - [`graphs.Compute.max_degree()`](./Compute/max_degree.md)
   - [`graphs.Compute.max_indegree()`](./Compute/max_indegree.md)
   - [`graphs.Compute.max_outdegree()`](./Compute/max_outdegree.md)
   - [`graphs.Compute.min_degree()`](./Compute/min_degree.md)
   - [`graphs.Compute.min_indegree()`](./Compute/min_indegree.md)
   - [`graphs.Compute.min_outdegree()`](./Compute/min_outdegree.md)
   - [`graphs.Compute.outdegree()`](./Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./Compute/pagerank.md)
+  - [`graphs.Compute.preferential_attachment()`](./Compute/preferential_attachment.md)
+  - [`graphs.Compute.reachable_from()`](./Compute/reachable_from.md
   - [`graphs.Compute.weakly_connected_component()`](./Compute/weakly_connected_component.md)
 - [`graphs.Edge`](./Edge/README.md)
   - [`graphs.Edge.__call__()`](./Edge/call__.md)
   - [`graphs.Edge.add()`](./Edge/add.md)
   - [`graphs.Edge.extend()`](./Edge/extend.md)
 - [`graphs.EdgeInstance`](./EdgeInstance/README.md)
   - [`graphs.EdgeInstance.from_`](./EdgeInstance/from_.md)
```

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/README.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,28 +22,31 @@
 - [`Compute.avg_outdegree()`](./avg_outdegree.md)
 - [`Compute.betweeness_centrality()`](./betweeness_centrality.md)
 - [`Compute.common_neighbor()`](./common_neighbor.md)
 - [`Compute.cosine_similarity()`](./cosine_similarity.md)
 - [`Compute.degree()`](./degree.md)
 - [`Compute.degree_centrality()`](./degree_centrality.md)
 - [`Compute.eigenvector_centrality()`](./eigenvector_centrality.md)
+- [`Compute.is_connected()`](./is_connected.md)
+- [`Compute.is_reachable()`](./is_reachable.md)
 - [`Compute.num_edges()`](./num_edges.md)
 - [`Compute.indegree()`](./indegree.md)
 - [`Compute.label_propagation()`](./label_propagation.md)
 - [`Compute.louvain()`](./louvain.md)
 - [`Compute.max_degree()`](./max_degree.md)
 - [`Compute.max_indegree()`](./max_indegree.md)
 - [`Compute.max_outdegree()`](./max_outdegree.md)
 - [`Compute.min_degree()`](./min_degree.md)
 - [`Compute.min_indegree()`](./min_indegree.md)
 - [`Compute.min_outdegree()`](./min_outdegree.md)
 - [`Compute.num_nodes()`](./num_nodes.md)
 - [`Compute.outdegree()`](./outdegree.md)
 - [`Compute.pagerank()`](./pagerank.md)
 - [`Compute.preferential_attachment()`](./preferential_attachment.md)
+- [`Compute.reachable_from()`](./reachable_from.md)
 - [`Compute.weakly_connected_component()`](./weakly_connected_component.md)
 - [`Compute.weighted_degree_centrality()`](./weighted_degree_centrality.md)
 
 ## Example
 
 ```python
 import relationalai as rai
```

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/adamic_adar.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/adamic_adar.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_degree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_indegree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/common_neighbor.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/common_neighbor.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/degree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/degree_centrality.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/indegree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/infomap.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/infomap.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/label_propagation.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/label_propagation.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/louvain.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/louvain.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_degree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_indegree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_outdegree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_degree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_indegree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_outdegree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/num_edges.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/num_edges.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/num_nodes.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/num_nodes.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/outdegree.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/pagerank.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/pagerank.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/README.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/add.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/call__.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/extend.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/README.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/from_.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/from_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/set.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/to.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/to.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/Edge.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/Edge.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/Node.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/Node.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/README.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/compute.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/compute.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/fetch.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/fetch.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/id.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/id.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/model.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/undirected.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/undirected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/visualize.md` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/visualize.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png` & `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/strings/concat.md` & `relationalai-0.2.5/docs/api_reference/python/std/strings/concat.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/strings/contains.md` & `relationalai-0.2.5/docs/api_reference/python/std/strings/contains.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/strings/ends_with.md` & `relationalai-0.2.5/docs/api_reference/python/std/strings/ends_with.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/strings/join.md` & `relationalai-0.2.5/docs/api_reference/python/std/strings/join.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/strings/length.md` & `relationalai-0.2.5/docs/api_reference/python/std/strings/length.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/strings/lowercase.md` & `relationalai-0.2.5/docs/api_reference/python/std/strings/lowercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/strings/replace.md` & `relationalai-0.2.5/docs/api_reference/python/std/strings/replace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/api_reference/python/std/strings/uppercase.md` & `relationalai-0.2.5/docs/api_reference/python/std/strings/uppercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/docs/faq/engines.md` & `relationalai-0.2.5/docs/faq/engines.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/README.md` & `relationalai-0.2.5/examples/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/cdc.py` & `relationalai-0.2.5/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/custom_snowflake_connection.py` & `relationalai-0.2.5/examples/custom_snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/emit_playground.py` & `relationalai-0.2.5/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/found.py` & `relationalai-0.2.5/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/fraud.ipynb` & `relationalai-0.2.5/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/fraud.py` & `relationalai-0.2.5/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/graph_algos.py` & `relationalai-0.2.5/examples/graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/nested.py` & `relationalai-0.2.5/examples/nested.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/or_types.py` & `relationalai-0.2.5/examples/or_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/remote_load_csv.py` & `relationalai-0.2.5/examples/remote_load_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/simple_recursion.py` & `relationalai-0.2.5/examples/simple_recursion.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/simple_streamlit.py` & `relationalai-0.2.5/examples/simple_streamlit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/solver.py` & `relationalai-0.2.5/examples/solver.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/weighted_graph_algos.py` & `relationalai-0.2.5/examples/weighted_graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/articles_graph/README.md` & `relationalai-0.2.5/examples/articles_graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/articles_graph/articles_graph.py` & `relationalai-0.2.5/examples/articles_graph/articles_graph.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/articles_graph/articles_graph_with_nlp.py` & `relationalai-0.2.5/examples/articles_graph/articles_graph_with_nlp.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/articles_graph/utils.py` & `relationalai-0.2.5/examples/articles_graph/utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/articles_graph/daily_articles/04_04_2024.json` & `relationalai-0.2.5/examples/articles_graph/daily_articles/04_04_2024.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/data/people.csv` & `relationalai-0.2.5/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/data/transactions.csv` & `relationalai-0.2.5/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/ev_penetration/ev_penetration.py` & `relationalai-0.2.5/examples/ev_penetration/ev_penetration.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/ev_penetration/ev_penetration_csv.py` & `relationalai-0.2.5/examples/ev_penetration/ev_penetration_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/ev_penetration/state_stats.csv` & `relationalai-0.2.5/examples/ev_penetration/state_stats.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/imdb/README.md` & `relationalai-0.2.5/examples/imdb/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/imdb/imdb.csv` & `relationalai-0.2.5/examples/imdb/imdb.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/imdb/imdb.py` & `relationalai-0.2.5/examples/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/rel/solver.rel` & `relationalai-0.2.5/examples/rel/solver.rel`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/social-money-network/SF_pagerank.ipynb` & `relationalai-0.2.5/examples/social-money-network/SF_pagerank.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/social-money-network/Simulation-and-SF-Upload.ipynb` & `relationalai-0.2.5/examples/social-money-network/Simulation-and-SF-Upload.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/examples/social-money-network/snowflake_pagerank.py` & `relationalai-0.2.5/examples/social-money-network/snowflake_pagerank.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/package-lock.json` & `relationalai-0.2.5/frontend/debugger/package-lock.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/package.json` & `relationalai-0.2.5/frontend/debugger/package.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/tsconfig.json` & `relationalai-0.2.5/frontend/debugger/tsconfig.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/vite.config.ts` & `relationalai-0.2.5/frontend/debugger/vite.config.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/.storybook/main.ts` & `relationalai-0.2.5/frontend/debugger/.storybook/main.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/App.styl` & `relationalai-0.2.5/frontend/debugger/src/App.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/App.tsx` & `relationalai-0.2.5/frontend/debugger/src/App.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/Selection.tsx` & `relationalai-0.2.5/frontend/debugger/src/Selection.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/debugger_client.ts` & `relationalai-0.2.5/frontend/debugger/src/debugger_client.ts`

 * *Files 8% similar despite different names*

```diff
@@ -28,32 +28,35 @@
 //------------------------------------------------------------------------------
 // Messages
 //------------------------------------------------------------------------------
 
 export namespace Message {
     export interface Base {
         event: string,
-        span?: string[],
         selection_path: number[],
         span_type?: undefined,
         events?: undefined,
         [key: string]: unknown
     }
-
+    
     export interface SpanStart extends Base {
-        event: "span_start",
-        span: string[],
-        start_time: number,
+        event: "span_start";
+        span: {
+            type: string;
+            id: string;
+            parent_id: string | null;
+            start_timestamp: string;
+            attrs: { [key: string]: any };
+        };
     }
     export interface SpanEnd extends Base {
         event: "span_end",
-        span: string[],
-        start_time: number,
-        end_time: number,
-        elapsed: number,
+        id: string;
+        end_timestamp: string;
+        end_attrs: { [key: string]: any };
     }
 
     export interface Time extends Base {
         event: "time",
         type: string,
         elapsed: number,
         results?: ResultData
@@ -110,17 +113,16 @@
 // Spans
 //------------------------------------------------------------------------------
 
 export namespace Span {
     export interface Base {
         event: "span",
         span_type: string,
-        span: string[];
-        start_time: number,
-        end_time?: number,
+        start_time: Date,
+        end_time?: Date,
         elapsed?: number,
         selection_path: number[],
 
         events: (Span | Message.Event)[],
 
         last_dirty_clock?: number,
         [key: string]: unknown,
@@ -202,15 +204,15 @@
     constructor(ws_url: string) {
         this.connection = new Connection(ws_url);
         [this.messages, this.set_messages] = createSignal<Message[]>([], {equals: () => false});
         [this.root, this.set_root] = createStore<Span>({
             event: "span",
             span_type: "root",
             span: [],
-            start_time: 0,
+            start_time: new Date(0),
             events: [],
             selection_path: []
         });
         [this.connected, this.set_connected] = createSignal<boolean>(false, {equals: () => false});
 
         this.latest = createMemo(() => {
             return this.spans().findLast(Span.is_program);
@@ -224,41 +226,46 @@
         this.connection.onconnect = this.set_connected;
     }
 
     clear() {
         batch(() => {
             this.path = [];
             this.set_messages([]);
-            this.set_root({event: "span", span_type: "root", span: [], start_time: 0, events: []});
+            this.set_root({event: "span", span_type: "root", span: [], start_time: new Date(0), events: []});
         });
     }
 
     protected handle_span_start(msg: Message.SpanStart) {
         this.set_root(produce((root) => {
             let parent = get_in(root, this.path);
             if(!parent || !Span.is_span(parent)) throw new Error();
             this.path.push(parent.events.length);
-            let span_type = msg.span[msg.span.length - 1];
+            let span_type = msg.span.type;
             let sub: Span = {
-                ...msg,
+                ...msg.span.attrs,
+                start_time: new Date(msg.span.start_timestamp),
+                end_time: undefined,
                 span_type,
                 event: "span",
                 selection_path: this.path.slice(),
                 run: span_type === "program" ? ++this.run_counter : undefined,
                 events: []
             };
             parent.events.push(sub)
         }));
     }
 
     protected handle_span_end(msg: Message.SpanEnd) {
         this.set_root(produce((root) => {
             let start = get_in(root, this.path);
             if(!start || !Span.is_span(start)) throw new Error();
-            for (let key in msg) {
+            start.end_time = new Date(msg.end_timestamp);
+            start.elapsed = (start.end_time.getTime() - start.start_time.getTime()) / 1000;
+            
+            for (let key in msg.end_attrs) {
                 if (key === "span" || key === "event") continue;
                 start[key] = msg[key];
             }
             this.path.pop();
         }));
     }
 
@@ -269,14 +276,15 @@
             msg.selection_path = [...this.path, span.events.length],
             span.events.push(msg);
         }));
     }
 
     protected handle_message = (msg: Message) => {
         batch(() => {
+            console.log('msg', msg);
             if(msg.event === "span_start") this.handle_span_start(msg)
             else if(msg.event === "span_end") this.handle_span_end(msg)
             else this.handle_event(msg);
 
             this.set_messages((prev) => {
                 prev.push(msg);
                 return prev;
```

### Comparing `relationalai-0.2.4/frontend/debugger/src/logo.svg` & `relationalai-0.2.5/frontend/debugger/src/logo.svg`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/util.styl` & `relationalai-0.2.5/frontend/debugger/src/util.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/util.ts` & `relationalai-0.2.5/frontend/debugger/src/util.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/assets/favicon.png` & `relationalai-0.2.5/frontend/debugger/src/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/EventList.styl` & `relationalai-0.2.5/frontend/debugger/src/components/EventList.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/EventList.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/EventList.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/EventViewer.styl` & `relationalai-0.2.5/frontend/debugger/src/components/EventViewer.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/EventViewer.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/EventViewer.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Sidebar.styl` & `relationalai-0.2.5/frontend/debugger/src/components/Sidebar.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Sidebar.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/ScopeProvider.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/ScopeProvider.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.stories.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.styl` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/base.styl` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/base.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/base.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/base.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/index.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Accordion.stories.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Accordion.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Accordion.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Accordion.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Button.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Button.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Code.styl` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Code.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Code.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Code.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.stories.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.styl` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Field.stories.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Field.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Field.styl` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Field.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Field.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Field.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Icon.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Icon.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.stories.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.styl` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.stories.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.styl` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.tsx` & `relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/fixtures/branch-improved.json` & `relationalai-0.2.5/frontend/debugger/src/fixtures/branch-improved.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/fixtures/branch.json` & `relationalai-0.2.5/frontend/debugger/src/fixtures/branch.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/fixtures/fraud.json` & `relationalai-0.2.5/frontend/debugger/src/fixtures/fraud.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/fixtures/not_found.json` & `relationalai-0.2.5/frontend/debugger/src/fixtures/not_found.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/fixtures/simple.json` & `relationalai-0.2.5/frontend/debugger/src/fixtures/simple.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/fixtures/union.json` & `relationalai-0.2.5/frontend/debugger/src/fixtures/union.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/frontend/debugger/src/types/mech.d.ts` & `relationalai-0.2.5/frontend/debugger/src/types/mech.d.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/README.md` & `relationalai-0.2.5/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/emit.py` & `relationalai-0.2.5/src/gentest/emit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/exec.py` & `relationalai-0.2.5/src/gentest/exec.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/fixtures.py` & `relationalai-0.2.5/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/patch.py` & `relationalai-0.2.5/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/util.py` & `relationalai-0.2.5/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/cli/__main__.py` & `relationalai-0.2.5/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/cli/collect_failures.py` & `relationalai-0.2.5/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/cli/collect_tests.py` & `relationalai-0.2.5/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/cli/repro.py` & `relationalai-0.2.5/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/cli/watch.py` & `relationalai-0.2.5/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/gen/action.py` & `relationalai-0.2.5/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/gen/context.py` & `relationalai-0.2.5/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/gen/document.py` & `relationalai-0.2.5/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/gen/group_limited.py` & `relationalai-0.2.5/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/gen/ir.py` & `relationalai-0.2.5/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/gen/scope.py` & `relationalai-0.2.5/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/gen/task.py` & `relationalai-0.2.5/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/gen/test.py` & `relationalai-0.2.5/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/harness/database.py` & `relationalai-0.2.5/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/validate/diff.py` & `relationalai-0.2.5/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/validate/errors.py` & `relationalai-0.2.5/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/validate/mapping.py` & `relationalai-0.2.5/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/gentest/validate/roundtrip.py` & `relationalai-0.2.5/src/gentest/validate/roundtrip.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/__init__.py` & `relationalai-0.2.5/src/relationalai/__init__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/compiler.py` & `relationalai-0.2.5/src/relationalai/compiler.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/debugging.py` & `relationalai-0.2.5/src/relationalai/debugging.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,58 +86,62 @@
         return
 
     global TIP_SPAN
 
     span = Span(type, TIP_SPAN, kwargs)
     TIP_SPAN = span
 
-    event = {
+    logger.debug({
         "event": "span_start",
-        "span": [type],
-        "id": str(span.id),
-        "parent_id": str(span.parent.id) if span.parent else None,
-        "start_timestamp": datetime.datetime.utcnow(),
-        **kwargs,
-    }
-    logger.debug(event)
+        "span": span,
+    })
     return span
 
 def span_end(span):
     if not DEBUG:
         return
     
     global TIP_SPAN
     TIP_SPAN = span.parent
     span.mark_finished()
     
     logger.debug({
         "event": "span_end",
         "id": str(span.id),
-        "parent_id": str(span.parent.id) if span.parent else None,
-        "span": [span.type],
-        "start_timestamp": span.start_timestamp,
         "end_timestamp": span.end_timestamp,
-        "elapsed": span.end_timestamp - span.start_timestamp,
-        **span.attrs,
+        "end_attrs": span.end_attrs,
     })
 
 class Span:
     def __init__(self, type: str, parent, attrs: Dict):
         self.id = uuid.uuid4()
         self.parent = parent
         self.type = type
         self.attrs = attrs
+        # additional attributes added during the lifetime of the span
+        self.end_attrs = {}
         # Would use `datetime.datetime.now(datetime.UTC)`, but it only works in 3.11.
         self.start_timestamp = datetime.datetime.utcnow()
+        self.end_timestamp = None
     
     def mark_finished(self):
         self.end_timestamp = datetime.datetime.utcnow()
     
     def __setitem__(self, key, value):
-        self.attrs[key] = value
+        self.end_attrs[key] = value
+    
+    def to_json(self):
+        return {
+            "type": self.type,
+            "id": str(self.id),
+            "parent_id": str(self.parent.id) if self.parent else None,
+            "start_timestamp": self.start_timestamp.isoformat(),
+            "end_timestamp": None if self.end_timestamp is None else self.end_timestamp.isoformat(),
+            "attrs": self.attrs,
+        }
 
 @contextlib.contextmanager
 def span(type: str, **kwargs):
     cur = span_start(type, **kwargs)
     try:
         yield cur
     except Exception as err:
```

### Comparing `relationalai-0.2.4/src/relationalai/dsl.py` & `relationalai-0.2.5/src/relationalai/dsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,19 @@
         return self._wrapped_op(Builtins.div, other, self)
 
     def __pow__(self, other):
         return self._wrapped_op(Builtins.pow, self, other)
     def __rpow__(self, other):
         return self._wrapped_op(Builtins.pow, other, self)
 
+    def __mod__(self, other):
+        return self._wrapped_op(Builtins.mod, self, other)
+    def __rmod__(self, other):
+        return self._wrapped_op(Builtins.mod, other, self)
+
     def __neg__(self):
         return self._wrapped_op(Builtins.mult, self, -1)
 
     #--------------------------------------------------
     # Filter overloads
     #--------------------------------------------------
 
@@ -535,14 +540,19 @@
         #--------------------------------------------------
         self._var = self._action.entity
         if self._var.type == Builtins.Unknown and len(self._action.types):
             self._var.type = self._action.types[0]
         if not is_add:
             self._add_to_graph()
 
+    def _to_var(self):
+        if not self._graph._stack.contains(self._context):
+            Errors.variable_out_of_context(Errors.call_source(), self._var.name)
+        return self._var
+
     def _add_to_graph(self):
         for action in self._actions:
             self._graph._action(action)
 
     def __call__(self, *args, **kwargs):
         pass
 
@@ -581,26 +591,36 @@
 
 class InstanceProperty(Producer):
     def __init__(self, graph:'Graph', instance:Instance, name:str, var=None, scope:str=""):
         super().__init__(graph, ["or_", "in_", "add", "extend", "choose"])
         self._instance = instance
         self._prop = build.property_named(scope+name, instance._action.types)
         self._var = var or Var(self._prop.type, name=name)
+        self._check_context()
         self._scope = scope
         new = Instance(self._graph, ActionType.Get, [instance], {name: self._var}, scope=self._scope)
         self._action = new._action
 
+    def _check_context(self):
+        if not self._graph._stack.contains(self._instance._context):
+            name = f"{self._instance._var.name}.{self._var.name}"
+            Errors.variable_out_of_context(Errors.call_source(), name, is_property=True)
+
     def __call__(self, *args, **kwargs):
         raise Exception("Properties can't be called")
 
     def _make_sub(self, name: str, existing=None):
         if existing is not None and existing._instance._context is self._graph._stack.active():
             return existing
         return getattr(Instance(self._graph, ActionType.Get, [self], {}), name)
 
+    def _to_var(self):
+        self._check_context()
+        return self._var
+
     def or_(self, other):
         self._graph._remove_action(self._action)
         rel.pyrel_default(self._prop, other, self._instance, self)
         return self
 
     def in_(self, others):
         other_rel = InlineRelation(self._graph, [(x,) for x in others])
@@ -931,14 +951,19 @@
         self.items.append(("pop", item))
         if len(self.stack) == 0:
             compacted = self.compact()
             self.items.clear()
             if len(compacted.items):
                 return compacted
 
+    def contains(self, item):
+        for i in self.stack:
+            if i is item:
+                return True
+
     def active(self):
         try:
             cur = self.stack[-1]
             if cur is self._graph._temp_rule:
                 Errors.out_of_context(Errors.call_source())
             return cur
         except IndexError:
```

### Comparing `relationalai-0.2.4/src/relationalai/errors.py` & `relationalai-0.2.5/src/relationalai/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,14 +303,26 @@
         Looks like this [yellow]object[/yellow] is being used outside of a rule or query.
 
         {marked}
         """
         print_source_error(source, "Outside of context", content)
         exit()
 
+    @staticmethod
+    def variable_out_of_context(source, name:str, is_property=False):
+        marked = mark_source(source, source.line, source.line)
+        content = f"""
+        Looks like a variable representing [yellow bold]{name}[/yellow bold] is being used outside of the rule or query it was defined in.
+
+        {marked}
+        """
+        print_source_error(source, "Variable out of context", content)
+        raise RAIException("Variable out of context") from None
+
+
     #--------------------------------------------------
     # DSL reserved errors
     #--------------------------------------------------
 
     @staticmethod
     def reserved_property(source, property_name:str):
         marked = mark_source(source, source.line, source.line)
```

### Comparing `relationalai-0.2.4/src/relationalai/metagen.py` & `relationalai-0.2.5/src/relationalai/metagen.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/metamodel.py` & `relationalai-0.2.5/src/relationalai/metamodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,14 +415,16 @@
 
         self.plus = binary_op("+", True)
         self.minus = binary_op("-", True)
         self.mult = binary_op("*", True)
         self.div = binary_op("/", True)
 
         self.pow = binary_op("^", True)
+        self.mod = binary_op("modulo", True)
+        self.mod.parents = []
 
         self.count = aggregate("count")
         self.sum = aggregate("sum")
         self.avg = aggregate("average")
         self.min = aggregate("min")
         self.max = aggregate("max")
```

### Comparing `relationalai-0.2.4/src/relationalai/rel.py` & `relationalai-0.2.5/src/relationalai/rel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/rel2.py` & `relationalai-0.2.5/src/relationalai/rel2.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/rel_emitter.py` & `relationalai-0.2.5/src/relationalai/rel_emitter.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/rel_utils.py` & `relationalai-0.2.5/src/relationalai/rel_utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/analysis/mechanistic.py` & `relationalai-0.2.5/src/relationalai/analysis/mechanistic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/analysis/whynot.py` & `relationalai-0.2.5/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/clients/azure.py` & `relationalai-0.2.5/src/relationalai/clients/azure.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/clients/client.py` & `relationalai-0.2.5/src/relationalai/clients/client.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/clients/config.py` & `relationalai-0.2.5/src/relationalai/clients/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from tomlkit.items import Table
 
 
 #--------------------------------------------------
 # config defaults
 #--------------------------------------------------
 
+CONFIG_FILE = "raiconfig.toml"
 FIELD_PLACEHOLDER = ""
 
 snowflake_default_props = {
     "platform": "snowflake",
     "user": FIELD_PLACEHOLDER,
     "password": FIELD_PLACEHOLDER,
     "account": FIELD_PLACEHOLDER,
@@ -169,16 +170,16 @@
     Returns the absolute path to the file if found, otherwise None.
     """
     file_path = os.path.expanduser(f"~/{file}")
     if os.path.isfile(file_path):
         yield file_path
 
 def _find_config_file():
-    yield from _search_upwards_for_file("raiconfig.toml")
-    yield from _search_userdir_for_file(".rai/raiconfig.toml")
+    yield from _search_upwards_for_file(CONFIG_FILE)
+    yield from _search_userdir_for_file(f".rai/{CONFIG_FILE}")
 
 def _parse_and_map_config(file:str):
     """
     Parse the config file at `file` and return a dictionary of config values.
 
     Handles both TOML and INI files.
     """
@@ -309,16 +310,16 @@
         cfg, path = _get_full_config(profile)
         self.profile = profile or cfg.get("active_profile", "__top_level__")
         self.file_path = path
         self.props = cfg
 
     def cache_config_file_contents(self):
         self.original_toml = tomlkit.document()
-        if os.path.exists("raiconfig.toml"):
-            with open("raiconfig.toml", "r") as f:
+        if os.path.exists(CONFIG_FILE):
+            with open(CONFIG_FILE, "r") as f:
                 try:
                     content = f.read()
                     if not content.endswith("\n"):
                         content += "\n"
                     self.original_toml = tomlkit.parse(content)
                 except toml.TomlDecodeError as e:
                     raise Exception(f"Error parsing {self.file_path}: {e}")
@@ -474,15 +475,15 @@
                 new_document[key] = value
 
         if active_profile is not None:
             ensure_profiles_added()
             if profiles.get(active_profile) is None:
                 profiles.add(active_profile, active_profile_table)
 
-        with open("raiconfig.toml", "w") as f:
+        with open(CONFIG_FILE, "w") as f:
             f.write(new_document.as_string())
 
     def _fill_in_with_defaults(self, defaults: Dict[str, Any], **kwargs):
         props = {k: v for k, v in kwargs.items() if k in defaults}
         self.update({
             **defaults,
             **self.props,
@@ -499,8 +500,8 @@
         platform = self.get("platform", None)
         if platform == "azure":
             self.fill_in_with_azure_defaults()
         elif platform == "snowflake":
             self.fill_in_with_snowflake_defaults()
         else:
             self.set("platform", "snowflake")
-            self.fill_in_with_snowflake_defaults()
+            self.fill_in_with_snowflake_defaults()
```

### Comparing `relationalai-0.2.4/src/relationalai/clients/snowflake.py` & `relationalai-0.2.5/src/relationalai/clients/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -739,14 +739,15 @@
 class SnowflakeSchema:
     def __init__(self, parent, name):
         self._name = name
         self._parent = parent
         self._model = parent._model
         self._tables = {}
         self._imported = set()
+        self._table_info = defaultdict(lambda: {"pks": [], "fks": {}, "columns": {}})
 
     def _fetch_info(self):
         self._table_info = self._model._client.resources.schema_info(self._parent._name, self._name, self._imported)
 
     def _add(self, name, is_imported=False):
         name = name.lower()
         if name in self._tables:
```

### Comparing `relationalai-0.2.4/src/relationalai/clients/test.py` & `relationalai-0.2.5/src/relationalai/clients/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/clients/types.py` & `relationalai-0.2.5/src/relationalai/clients/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/loaders/csv.py` & `relationalai-0.2.5/src/relationalai/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/loaders/loader.py` & `relationalai-0.2.5/src/relationalai/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/loaders/types.py` & `relationalai-0.2.5/src/relationalai/loaders/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/std/aggregates.py` & `relationalai-0.2.5/src/relationalai/std/aggregates.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/std/graphs.py` & `relationalai-0.2.5/src/relationalai/std/graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,41 @@
     def num_nodes(self):
         return self._lib.num_nodes(self._graph)
 
     def num_edges(self):
         return self._lib.num_edges(self._graph)
 
     # --------------------------------------------------
+    # Connectivity
+    # --------------------------------------------------
+
+    def is_connected(self):
+        model = self._graph.model
+        with model.ordered_choice() as v:
+            with model.scope():
+                self._lib.is_connected(self._graph)
+                v.add(True)
+            with model.scope():
+                v.add(False)
+        return v
+
+    def reachable_from(self, node: dsl.Producer) -> dsl.Expression:
+        return self._lib.transitive_closure(self._graph, node)
+
+    def is_reachable(self, node1: dsl.Producer, node2: dsl.Producer) -> dsl.Expression:
+        model = self._graph.model
+        with model.ordered_choice() as v:
+            with model.scope():
+                self._lib.transitive_closure(self._graph, node1, node2)
+                v.add(True)
+            with model.scope():
+                v.add(False)
+        return v
+
+    # --------------------------------------------------
     # Link Prediction
     # --------------------------------------------------
 
     def adamic_adar(self, node1, node2):
         return self._lib.adamic_adar(self._graph, node1, node2)
 
     def preferential_attachment(self, node1, node2):
@@ -242,15 +269,15 @@
         return self._props[__name]
 
 #--------------------------------------------------
 # Graph
 #--------------------------------------------------
 
 class Graph:
-    def __init__(self, model:dsl.Graph, undirected=False, weighted=False, default_weight=1.0):
+    def __init__(self, model:dsl.Graph, undirected=False, weighted=False, default_weight=1.0, with_isolated_nodes=False):
         self.model = model
         self.id = dsl.next_id()
         self.compute = Compute(self)
         self.Node = dsl.Type(model, "nodes", scope=f"graph{self.id}_")
         self.Edge = Edge(self)
         self.undirected = undirected
         self.weighted = weighted
@@ -259,20 +286,24 @@
 
         graph_type = "::graphlib::undirected_graph" if undirected else "::graphlib::directed_graph"
         if weighted:
             create_graph = f"""{graph_type}[{self.Edge._prop("weight")._name}]"""
         else:
             create_graph = f"{graph_type}[{self.Edge._type._name}]"
 
+        node_def = ""
+        if with_isolated_nodes:
+            node_def = f"def {self._graph_ref()}[:node]: {{{self.Node._type.name}}}"
+
         self.model.install_raw(f"""
         declare {self.Node._type.name}
         declare {self.Edge._type._name}
         {f"declare {self.Edge._prop('weight')._name}" if weighted else ""}
         def {self._graph_ref()} {{{create_graph}}}
-        def {self._graph_ref()}[:node]: {{{self.Node._type.name}}}
+        {node_def}
         @inline
         def {self._lib_ref()} {{rel[:graphlib, {self._graph_ref()}]}}
         """)
 
         # Add a rule that makes all nodes used in edges are also added to
         # the nodes relation
         with model.rule():
```

### Comparing `relationalai-0.2.4/src/relationalai/std/strings.py` & `relationalai-0.2.5/src/relationalai/std/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/tools/cli.py` & `relationalai-0.2.5/src/relationalai/tools/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from rich.console import Console
 from rich import box as rich_box
 from rich.table import Table
 from ..tools import debugger as deb
 from ..clients import config, snowflake
 from ..clients.config import (
     FIELD_PLACEHOLDER,
+    CONFIG_FILE,
     ConfigFile,
     all_configs_including_legacy,
     get_from_snowflake_connections_toml,
     azure_default_props,
     snowflake_default_props,
 )
 from InquirerPy.base.control import Choice
@@ -372,102 +373,68 @@
     profile = controls.fuzzy("Use profile from ~/.snowflake/connections.toml", profiles, mandatory=False)
     if not profile:
         return
     cfg.profile = profile
     cfg.update(sf_config[profile])
     return True
 
-def get_default(value:str|None, list_of_values:Sequence[str]):
-    if value is None:
-        return None
-    list_of_values_lower = [v.lower() for v in list_of_values]
-    value_lower = value.lower()
-    if value_lower in list_of_values_lower:
-        return value
-
 def role_flow(provider:ResourceProvider, cfg:config.Config):
-    with Spinner("Fetching roles", "Fetched roles"):
-        try:
-            roles = cast(snowflake.Resources, provider).list_roles()
-        except Exception as e:
-            raise Exception(f"Error fetching roles: {e}")
-    role_names = [r["name"] for r in roles]
-    if len(role_names) == 0:
-        raise Exception("No roles found")
-    default = get_default(cfg.get("role", None), role_names)
-    role = controls.fuzzy("Select a role:", role_names, default=default, mandatory=False)
+    role = controls.fuzzy_with_refetch(
+            "Select a role:",
+            "roles",
+            lambda: [r["name"] for r in cast(snowflake.Resources, provider).list_roles()],
+            default=cfg.get("role", None),
+        )
     cfg.set("role", role or FIELD_PLACEHOLDER)
     provider.reset()
 
 def warehouse_flow(provider:ResourceProvider, cfg:config.Config):
-    rich.print("")
-    with Spinner("Fetching warehouses", "Fetched warehouses"):
-        try:
-            warehouses = cast(snowflake.Resources, provider).list_warehouses()
-        except Exception as e:
-            raise Exception(f"Error fetching warehouses: {e}")
-    rich.print("")
-    warehouse_names = [w["name"] for w in warehouses]
-    if len(warehouse_names) == 0:
-        raise Exception("No warehouses found")
-    default = get_default(cfg.get("warehouse", None), warehouse_names)
-    warehouse = controls.fuzzy("Select a warehouse:", warehouse_names, default=default, mandatory=False)
+    warehouse = controls.fuzzy_with_refetch(
+            "Select a warehouse:",
+            "warehouses",
+            lambda: [w["name"] for w in cast(snowflake.Resources, provider).list_warehouses()],
+            default=cfg.get("warehouse", None),
+        )
     cfg.set("warehouse", warehouse or FIELD_PLACEHOLDER)
 
 def rai_app_flow(provider:ResourceProvider, cfg:config.Config):
-    rich.print("")
-    with Spinner("Fetching installed apps", "Fetched apps"):
-        try:
-            apps = cast(snowflake.Resources, provider).list_apps()
-        except Exception as e:
-            raise Exception(f"Error fetching apps: {e}")
-    rich.print("")
-    app_names = [w["name"] for w in apps]
-    if len(app_names) == 0:
-        raise Exception("No apps found")
-    default = get_default(cfg.get("rai_app_name", None), app_names)
-    app = controls.fuzzy("Select RelationalAI app name:", app_names, default=default, mandatory=False)
+    app = controls.fuzzy_with_refetch(
+            "Select RelationalAI app name:",
+            "apps",
+            lambda: [w["name"] for w in cast(snowflake.Resources, provider).list_apps()],
+            default=cfg.get("rai_app_name", None),
+        )
     cfg.set("rai_app_name", app or FIELD_PLACEHOLDER)
     provider.reset()
 
 def spcs_flow(provider: ResourceProvider, cfg: config.Config):
 
     role_flow(provider, cfg)
     warehouse_flow(provider, cfg)
     rai_app_flow(provider, cfg)
 
 def engine_flow(provider:ResourceProvider, cfg:config.Config):
-    rich.print("")
-    with Spinner("Fetching engines", "Fetched engines"):
-        try:
-            engines = provider.list_engines()
-        except Exception as e:
-            raise Exception(f"Error fetching engines: {e}")
-
-    engine_names = ["Create a new engine"] + [engine.get("name") for engine in engines]
-    rich.print("")
-    default = get_default(cfg.get("engine", None), engine_names)
-    engine = controls.fuzzy("Select an engine:", choices=engine_names, default=default, mandatory=False)
+    engine = controls.fuzzy_with_refetch(
+        "Select an engine:",
+        "engines",
+        lambda: ["Create a new engine"] + [engine.get("name") for engine in provider.list_engines()],
+        default=cfg.get("engine", None),
+    )
     if engine == "Create a new engine":
         engine = controls.text("Engine name:", validator=ENGINE_NAME_REGEX.match, invalid_message=ENGINE_NAME_ERROR)
         engine_size = controls.fuzzy("Engine size:", choices=ENGINE_SIZES)
         engine_pool = ""
         if cfg.get("platform") == "snowflake":
             provider = cast(snowflake.Resources, provider)
-            rich.print("")
-            with Spinner(f"Fetching compute pools for engine size '{engine_size}'", f"Fetched compute pools for engine size '{engine_size}'"):
-                try:
-                    valid_pools = provider.list_valid_compute_pools_by_engine_size(engine_size)
-                except Exception as e:
-                    raise Exception(f"Error fetching compute pools: {e}")
-            if len(valid_pools) == 0:
-                rich.print(f"\n[yellow]No valid compute pools found for engine size '{engine_size}'\n")
-                exit(1)
-            rich.print("")
-            engine_pool = controls.fuzzy("Compute pool:", valid_pools, mandatory=False)
+            engine_pool = controls.fuzzy_with_refetch(
+                "Compute pool:",
+                "compute pools",
+                provider.list_valid_compute_pools_by_engine_size,
+                engine_size,
+            )
         rich.print("")
         with Spinner(f"Creating '{engine}' engine... (this may take several minutes)", f"Engine '{engine}' created"):
             try:
                 provider.create_engine(engine, engine_size, engine_pool)
             except Exception as e:
                 raise Exception(f"Error creating engine: {e}")
         rich.print("")
@@ -477,22 +444,22 @@
     current_dir = Path.cwd()
     prev_dir = None
     while current_dir != prev_dir:
         gitignore_path = current_dir / '.gitignore'
         if gitignore_path.exists():
             # if there is, check to see if raiconfig.toml is in it
             with open(gitignore_path, 'r') as gitignore_file:
-                if 'raiconfig.toml' in gitignore_file.read():
+                if CONFIG_FILE in gitignore_file.read():
                     return
                 else:
                     # if it's not, ask to add it
-                    add_to_gitignore = controls.confirm("Add raiconfig.toml to .gitignore?", default=True)
+                    add_to_gitignore = controls.confirm(f"Add {CONFIG_FILE} to .gitignore?", default=True)
                     if add_to_gitignore:
                         with open(gitignore_path, 'a') as gitignore_file:
-                            gitignore_file.write("\nraiconfig.toml")
+                            gitignore_file.write(f"\n{CONFIG_FILE}")
                     return
         prev_dir = current_dir
         current_dir = current_dir.parent
 
 def save_flow(cfg:config.Config, check_for_profile_overwrite:bool=True, update_active_profile:bool=True):
     if cfg.profile in cfg.get_profiles() and check_for_profile_overwrite:
         if not controls.confirm(f"Overwrite existing {cfg.profile} profile"):
@@ -533,15 +500,15 @@
         if platform == SNOWFLAKE:
             spcs_flow(provider, cfg)
         engine_flow(provider, cfg)
         save_flow(cfg)
 
         gitignore_flow()
         rich.print("")
-        rich.print("[green]✓ raiconfig.toml saved!")
+        rich.print(f"[green]✓ {CONFIG_FILE} saved!")
         rich.print("\n[dim]---------------------------------------------------\n")
     except Exception as e:
         rich.print("")
         rich.print("[yellow bold]Initialization aborted!")
         rich.print(f"[yellow]{e}")
         print(e.with_traceback(None))
         rich.print("")
@@ -550,15 +517,15 @@
         if save:
             if cfg.profile == "__top_level__":
                 cfg.profile = "partial"
             rich.print("")
             cfg.fill_in_with_defaults()
             save_flow(cfg, check_for_profile_overwrite=False, update_active_profile=False)
             gitignore_flow()
-            rich.print(f"[yellow bold]✓ Saved partial raiconfig.toml ({os.path.abspath('raiconfig.toml')})")
+            rich.print(f"[yellow bold]✓ Saved partial {CONFIG_FILE} ({os.path.abspath(CONFIG_FILE)})")
 
         divider()
 
 #--------------------------------------------------
 # Profile switcher
 #--------------------------------------------------
 
@@ -694,26 +661,36 @@
             table.add_row(f"[bold]{name}[red]", f"[red bold]{version} → {latest}")
         else:
             table.add_row(f"[bold]{name}", f"[green]{version}")
 
     divider()
     print_version("RelationalAI", __version__, latest_version("relationalai"))
     print_version("Rai-sdk", railib_version, latest_version("rai-sdk"))
+    print_version("Python", sys.version.split()[0])
 
-    if get_config().get("platform") == "snowflake":
-        # print()
-        with Spinner("Checking app version"):
-            try:
-                app_version = get_resource_provider().get_version()
-            except Exception as e:
-                rich.print(f"\n\n[yellow]Error fetching app version: {e}")
-                exit(1)
-        print_version("App", app_version)
+    try:
+        cfg = get_config(CONFIG_FILE)
+        if not cfg.file_path:
+            table.add_row("[bold]App", "No configuration file found. To create one, run: [green]rai init")
+        else:
+            platform = cfg.get("platform")
+            if platform == "snowflake":
+                # print()
+                with Spinner("Checking app version"):
+                    try:
+                        app_version = get_resource_provider().get_version()
+                    except Exception as e:
+                        rich.print(f"\n\n[yellow]Error fetching app version: {e}")
+                        exit(1)
+                print_version("App", app_version)
 
-    print_version("Python", sys.version.split()[0])
+    except Exception as e:
+        rich.print(f"[yellow]Error fetching platform: {e}")
+        divider()
+        exit(1)
 
     rich.print(table)
     divider()
 
 #--------------------------------------------------
 # Debugger
 #--------------------------------------------------
@@ -765,27 +742,20 @@
     if not size:
         size = controls.fuzzy("Engine size:", choices=ENGINE_SIZES)
         rich.print("")
     provider = get_resource_provider()
 
     if provider.config.get("platform") == "snowflake":
         provider = cast(snowflake.Resources, provider)
-        rich.print("")
-        with Spinner(f"Fetching compute pools for engine size '{size}'", f"Fetched compute pools for engine size '{size}'"):
-            try:
-                valid_pools = provider.list_valid_compute_pools_by_engine_size(size)
-            except Exception as e:
-                rich.print(f"\n\n[yellow]Error fetching compute pools: {e}")
-                exit(1)
-        if len(valid_pools) == 0:
-            rich.print(f"\n[yellow]No valid compute pools found for engine size '{size}'\n")
-            exit(1)
-        rich.print("")
-        pool = controls.fuzzy("Compute pool:", valid_pools)
-        rich.print("")
+        pool = controls.fuzzy_with_refetch(
+            "Compute pool:",
+            "compute pools",
+            provider.list_valid_compute_pools_by_engine_size,
+            size,
+        )
     else:
         pool = ""
 
     with Spinner(f"Creating '{name}' engine... (this may take several minutes)", f"Engine '{name}' created!"):
         try:
             provider.create_engine(name, size, pool)
         except Exception as e:
@@ -800,26 +770,19 @@
 
 @cli.command(name="engines:delete", help="Delete an engine")
 @click.option("--name", help="Name of the engine")
 def engines_delete(name):
     divider(flush=True)
     ensure_config()
     if not name:
-        with Spinner("Fetching engines"):
-            try:
-                engines = get_resource_provider().list_engines()
-            except Exception as e:
-                rich.print(f"\n\n[yellow]Error fetching engines: {e}")
-                exit(1)
-        if len(engines) == 0:
-            rich.print("[yellow]No engines found")
-            divider()
-            sys.exit(0)
-        name = controls.fuzzy("Select an engine:", [engine["name"] for engine in engines])
-        print("")
+        name = controls.fuzzy_with_refetch(
+            "Select an engine:",
+            "engines",
+            lambda: [engine["name"] for engine in get_resource_provider().list_engines()],
+        )
 
     with Spinner(f"Deleting '{name}' engine", f"Engine '{name}' deleted!"):
         try:
             get_resource_provider().delete_engine(name)
         except Exception as e:
             rich.print(f"\n\n[yellow]Error deleting engine: {e}")
     divider()
```

### Comparing `relationalai-0.2.4/src/relationalai/tools/cli_controls.py` & `relationalai-0.2.5/src/relationalai/tools/cli_controls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #pyright: reportPrivateImportUsage=false
 
 import io
 import os
 from re import Pattern
-from typing import Any, List, cast
+from typing import Sequence, cast, Any, List
 from pathlib import Path
 from InquirerPy.base.complex import FakeDocument
 from prompt_toolkit.key_binding import KeyPressEvent
 from prompt_toolkit.validation import ValidationError
 import rich
 from rich.console import Console
 import sys
@@ -15,14 +15,20 @@
 from InquirerPy.base.control import Choice
 import time
 import threading
 import itertools
 from ..debugging import jupyter
 
 #--------------------------------------------------
+# Constants
+#--------------------------------------------------
+
+REFETCH = "[REFETCH LIST]"
+
+#--------------------------------------------------
 # Style
 #--------------------------------------------------
 
 STYLE = inquirer_utils.get_style({
     "fuzzy_prompt": "#e5c07b"
 }, False)
 
@@ -40,14 +46,22 @@
     resolved_path = path.resolve()
     resolved_base = base.resolve()
     if resolved_base in resolved_path.parents or resolved_path == resolved_base:
         return resolved_path.relative_to(resolved_base)
     else:
         return resolved_path.absolute()
 
+def get_default(value:str|None, list_of_values:Sequence[str]):
+    if value is None:
+        return None
+    list_of_values_lower = [v.lower() for v in list_of_values]
+    value_lower = value.lower()
+    if value_lower in list_of_values_lower:
+        return value
+
 #--------------------------------------------------
 # Dividers
 #--------------------------------------------------
 
 def divider(console=None, flush=False):
     div = "\n[dim]---------------------------------------------------\n "
     if console is None:
@@ -130,14 +144,38 @@
         prompt = inquirer.fuzzy(message, choices=choices, default=default or "", max_height=8, border=True, style=STYLE, **kwargs)
         if scroll_to_ix is not None:
             prompt.content_control.selected_choice_index = scroll_to_ix
         return prompt.execute()
     except KeyboardInterrupt:
         return abort()
 
+def fuzzy_with_refetch(prompt: str, type: str, fn: callable = None, *args, **kwargs):
+    with Spinner(f"Fetching {type}", f"Fetched {type}"):
+        try:
+            items = fn(*args)
+        except Exception as e:
+            rich.print(f"\n\n[yellow]Error fetching {type}: {e}")
+            exit(1)
+    if len(items) == 0:
+        rich.print(f"\n[yellow]No valid {type} found\n")
+        exit(1)
+
+    items.insert(0, REFETCH)
+
+    passed_default = kwargs.get("default", None)
+    default = get_default(passed_default, items)
+
+    rich.print("")
+    result = fuzzy(prompt, items, default=default)
+    rich.print("")
+
+    while result == REFETCH:
+        result = fuzzy_with_refetch(prompt, type, fn, default=passed_default, *args)
+    return result
+
 def confirm(message:str, default:bool = False) -> bool:
     try:
         return inquirer.confirm(message, default=default, keybindings=default_bindings).execute()
     except KeyboardInterrupt:
         return abort()
 
 def text(message:str, default:str|None = None, validator:callable = None, invalid_message:str|None = None) -> str:
```

### Comparing `relationalai-0.2.4/src/relationalai/tools/debugger.py` & `relationalai-0.2.5/src/relationalai/tools/debugger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/tools/debugger_server.py` & `relationalai-0.2.5/src/relationalai/tools/debugger_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,16 +55,19 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         from relationalai.analysis.mechanistic import Mechanism
         self.Mechanism = Mechanism
 
     def emit(self, record):
         d = record.msg
-        if isinstance(d, dict) and d["event"] == "span_start" and "task" in d and "mech" not in d:
-            d["mech"] = self.Mechanism(d["task"])
+        if (isinstance(d, dict) and
+            d["event"] == "span_start" and
+            "task" in d["span"].attrs and
+            "mech" not in d["span"].attrs):
+            d["span"].attrs["mech"] = self.Mechanism(d["span"].attrs["task"])
         log_entry = self.format(record)
         asyncio.run(broadcast(log_entry))
 
 already_debugging = False
 def start_debugger_session(wait_for_connection = False, host = "0.0.0.0", port = 5678):
     global already_debugging
     if already_debugging:
```

### Comparing `relationalai-0.2.4/src/relationalai/tools/dev.py` & `relationalai-0.2.5/src/relationalai/tools/dev.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/src/relationalai/util/snowflake_logger.py` & `relationalai-0.2.5/src/relationalai/util/snowflake_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import threading
 import time
 
 import logging
 import traceback
 import uuid
 
+from relationalai.debugging import Span
+
 # Don't insert these as attrs since they get their own columns
 FILTER_ATTRS = {
     "event",
     "span",
     "id",
     "parent_id",
     "start_time",
@@ -26,18 +28,19 @@
         self.trace_id = uuid.uuid4()
         self.snowflake_conn = snowflake_conn
         self.queue = queue.Queue()
         self.is_shut_down = False
         self.sleep_interval_s = sleep_interval_s
         self.worker_thread = threading.Thread(target=self._consume_loop)
         self.worker_thread.start()
+        self.open_spans = {} # only accessed from worker thread
         print('snowflake logger started with trace id', self.trace_id)
     
     def emit(self, record):
-        if record.msg["event"] == "span_end":
+        if record.msg["event"] in ("span_start", "span_end"):
             self.queue.put(record.msg)
     
     def _consume_loop(self):
         while True:
             while not self.queue.empty():
                 try:
                     batch = self._get_batch()
@@ -62,29 +65,34 @@
     def _send_batch(self, batch):
         if not batch:
             return
         
         inserts = []
     
         for event in batch:
-            filtered_attrs = {}
-            for k, v in event.items():
-                if k not in FILTER_ATTRS:
-                    filtered_attrs[k] = v
-            span_key = get_key(event)
-            inserts.append({
-                "id": event["id"],
-                "parent_id": event["parent_id"],
-                "trace_id": str(self.trace_id),
-                "key": str(span_key) if span_key is not None else None,
-                "type": event["span"][0],
-                "start_ts": event["start_timestamp"],
-                "finish_ts": event["end_timestamp"],
-                "attrs": json.dumps(filtered_attrs, default=default_serialize),
-            })
+            if event["event"] == "span_start":
+                span = event["span"]
+                self.open_spans[str(span.id)] = span
+            elif event["event"] == "span_end":
+                span = self.open_spans.pop(event["id"])
+                filtered_attrs = {}
+                for k, v in span.attrs.items():
+                    if k not in FILTER_ATTRS:
+                        filtered_attrs[k] = v
+                span_key = get_key(span)
+                inserts.append({
+                    "id": str(span.id),
+                    "parent_id": None if span.parent is None else str(span.parent.id),
+                    "trace_id": str(self.trace_id),
+                    "key": str(span_key) if span_key is not None else None,
+                    "type": span.type,
+                    "start_ts": span.start_timestamp,
+                    "finish_ts": span.end_timestamp,
+                    "attrs": json.dumps(filtered_attrs, default=default_serialize),
+                })
         # execute
         if inserts:
             self.snowflake_conn.cursor().executemany(
                 """
                 INSERT INTO spans_raw (id, parent_id, trace_id, type, key, start_ts, finish_ts, attrs)
                 VALUES (%(id)s, %(parent_id)s, %(trace_id)s, %(type)s, %(key)s, %(start_ts)s, %(finish_ts)s, %(attrs)s)
                 """,
@@ -101,16 +109,16 @@
 # === helpers ===
 
 SPAN_KEYS = {
     'test': 'name',
     'run': 'idx',
 }
 
-def get_key(span):
-    type = span["span"][0]
+def get_key(span: 'Span'):
+    type = span.type
     if type in SPAN_KEYS:
         key = SPAN_KEYS[type]
-        return span[key]
+        return span.attrs[key]
     return None
 
 def default_serialize(obj):
     return '<skipped>'
```

### Comparing `relationalai-0.2.4/tests/conftest.py` & `relationalai-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/README.md` & `relationalai-0.2.5/tests/end2end/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/conftest.py` & `relationalai-0.2.5/tests/end2end/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_graph_visualize.py` & `relationalai-0.2.5/tests/end2end/test_graph_visualize.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_snapshots.py` & `relationalai-0.2.5/tests/end2end/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt` & `relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/bool.py` & `relationalai-0.2.5/tests/end2end/test_cases/bool.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/bottom.py` & `relationalai-0.2.5/tests/end2end/test_cases/bottom.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/export.py` & `relationalai-0.2.5/tests/end2end/test_cases/export.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/multi_valued.py` & `relationalai-0.2.5/tests/end2end/test_cases/multi_valued.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/not_found.py` & `relationalai-0.2.5/tests/end2end/test_cases/not_found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/persist.py` & `relationalai-0.2.5/tests/end2end/test_cases/persist.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/smoke.py` & `relationalai-0.2.5/tests/end2end/test_cases/smoke.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pyright: reportUnusedExpression=false
 import relationalai as rai
 
-model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
+model = rai.Model(name=globals().get("name", "test_smoke"), config=globals().get("config"))
 Person = model.Type("Person")
 Adult = model.Type("Adult")
 
 with model.rule():
     Person.add(name="Joe", age=74)
     Person.add(name="Bob", age=40)
     Person.add(name="Jane", age=10)
@@ -18,13 +18,13 @@
 with model.rule():
     p = Person()
     with p.age == 10:
         p.set(coolness=100)
 
 with model.query() as select:
     a = Adult()
-    10 <= p.age <= 80
+    10 <= a.age <= 80
     select(a, a.name, a.age)
 
 with model.query() as select:
     p = Person()
     select(p, p.coolness)
```

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/strings.py` & `relationalai-0.2.5/tests/end2end/test_cases/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/top.py` & `relationalai-0.2.5/tests/end2end/test_cases/top.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/union.py` & `relationalai-0.2.5/tests/end2end/test_cases/union.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/weighted_graphs.py` & `relationalai-0.2.5/tests/end2end/test_cases/weighted_graphs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/graphs/basics.py` & `relationalai-0.2.5/tests/end2end/test_cases/graphs/basics.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/graphs/centrality.py` & `relationalai-0.2.5/tests/end2end/test_cases/graphs/centrality.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/graphs/community.py` & `relationalai-0.2.5/tests/end2end/test_cases/graphs/community.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with model.rule():
     obj1 = Object.add(id=1)
     obj2 = Object.add(id=2)
     obj3 = Object.add(id=3)
     Relationship.add(from_=obj1, to=obj2)
 
-graph = std.graphs.Graph(model, undirected=True)
+graph = std.graphs.Graph(model, undirected=True, with_isolated_nodes=True)
 graph.Node.extend(Object)
 
 with model.rule():
     r = Relationship()
     graph.Edge.add(r.from_, r.to)
 
 for algo_name in ALGOS:
```

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/graphs/degree.py` & `relationalai-0.2.5/tests/end2end/test_cases/graphs/degree.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/graphs/link_prediction.py` & `relationalai-0.2.5/tests/end2end/test_cases/graphs/link_prediction.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/end2end/test_cases/graphs/similarity.py` & `relationalai-0.2.5/tests/end2end/test_cases/graphs/similarity.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/init-cli/azure_basic.py` & `relationalai-0.2.5/tests/init-cli/azure_basic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/init-cli/common.py` & `relationalai-0.2.5/tests/init-cli/common.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/roundtrip/test_document.py` & `relationalai-0.2.5/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/tests/roundtrip/test_task.py` & `relationalai-0.2.5/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.4/pyproject.toml` & `relationalai-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'relationalai'
-version = '0.2.4'
+version = '0.2.5'
 description = 'RelationalAI Library and CLI'
 readme="docs/pypi/README.md"
 authors = [
     { name="RelationalAI", email="support@relational.ai" },
 ]
 requires-python = ">= 3.10"
 dependencies = [
```

### Comparing `relationalai-0.2.4/PKG-INFO` & `relationalai-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: relationalai
-Version: 0.2.4
+Version: 0.2.5
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
 Requires-Dist: gravis
```

