# Comparing `tmp/twitterexplorer-0.6.7.tar.gz` & `tmp/twitterexplorer-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitterexplorer-0.6.7.tar", last modified: Mon Mar  6 07:44:04 2023, max compression
+gzip compressed data, was "twitterexplorer-0.7.0.tar", last modified: Fri Apr 26 13:23:25 2024, max compression
```

## Comparing `twitterexplorer-0.6.7.tar` & `twitterexplorer-0.7.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ap         (501) staff       (20)        0 2023-03-06 07:44:04.512306 twitterexplorer-0.6.7/
--rw-r--r--   0 ap         (501) staff       (20)    35149 2022-03-09 18:04:12.000000 twitterexplorer-0.6.7/LICENSE
--rw-r--r--   0 ap         (501) staff       (20)     6115 2023-03-06 07:44:04.512183 twitterexplorer-0.6.7/PKG-INFO
--rw-r--r--   0 ap         (501) staff       (20)     5766 2023-02-02 19:05:33.000000 twitterexplorer-0.6.7/README.md
--rw-r--r--   0 ap         (501) staff       (20)       38 2023-03-06 07:44:04.512338 twitterexplorer-0.6.7/setup.cfg
--rw-r--r--   0 ap         (501) staff       (20)     1310 2023-03-06 07:41:49.000000 twitterexplorer-0.6.7/setup.py
-drwxr-xr-x   0 ap         (501) staff       (20)        0 2023-03-06 07:44:04.509250 twitterexplorer-0.6.7/twitterexplorer/
--rw-r--r--   0 ap         (501) staff       (20)       51 2023-01-29 12:30:05.000000 twitterexplorer-0.6.7/twitterexplorer/__init__.py
--rw-r--r--   0 ap         (501) staff       (20)       22 2023-03-06 07:43:07.000000 twitterexplorer-0.6.7/twitterexplorer/__version__.py
-drwxr-xr-x   0 ap         (501) staff       (20)        0 2023-03-06 07:44:04.510715 twitterexplorer-0.6.7/twitterexplorer/apps/
--rw-r--r--   0 ap         (501) staff       (20)        0 2023-02-02 18:13:22.000000 twitterexplorer-0.6.7/twitterexplorer/apps/__init__.py
--rw-r--r--   0 ap         (501) staff       (20)    13876 2023-02-12 14:04:34.000000 twitterexplorer-0.6.7/twitterexplorer/apps/collector.py
--rw-r--r--   0 ap         (501) staff       (20)    15240 2023-02-07 16:58:00.000000 twitterexplorer-0.6.7/twitterexplorer/apps/visualizer.py
--rw-r--r--   0 ap         (501) staff       (20)     1654 2023-01-29 19:40:52.000000 twitterexplorer-0.6.7/twitterexplorer/constants.py
--rw-r--r--   0 ap         (501) staff       (20)     1439 2023-01-29 12:46:10.000000 twitterexplorer-0.6.7/twitterexplorer/converters.py
--rw-r--r--   0 ap         (501) staff       (20)     2279 2023-01-29 19:39:29.000000 twitterexplorer-0.6.7/twitterexplorer/d3networks.py
--rw-r--r--   0 ap         (501) staff       (20)      547 2023-01-29 19:14:21.000000 twitterexplorer-0.6.7/twitterexplorer/defaults.py
--rw-r--r--   0 ap         (501) staff       (20)     4599 2023-01-30 08:22:02.000000 twitterexplorer-0.6.7/twitterexplorer/helpers.py
-drwxr-xr-x   0 ap         (501) staff       (20)        0 2023-03-06 07:44:04.511985 twitterexplorer-0.6.7/twitterexplorer/html/
--rw-r--r--   0 ap         (501) staff       (20)     2059 2022-03-24 14:02:48.000000 twitterexplorer-0.6.7/twitterexplorer/html/head.html
--rw-r--r--   0 ap         (501) staff       (20)     3698 2023-01-29 13:17:25.000000 twitterexplorer-0.6.7/twitterexplorer/html/htn_body.html
--rw-r--r--   0 ap         (501) staff       (20)    12807 2023-01-29 13:15:25.000000 twitterexplorer-0.6.7/twitterexplorer/html/htn_graph.js
--rw-r--r--   0 ap         (501) staff       (20)     5755 2022-11-20 11:10:44.000000 twitterexplorer-0.6.7/twitterexplorer/html/rtn_body.html
--rw-r--r--   0 ap         (501) staff       (20)    19984 2023-01-23 13:48:08.000000 twitterexplorer-0.6.7/twitterexplorer/html/rtn_graph.js
--rw-r--r--   0 ap         (501) staff       (20)    20204 2022-11-20 11:09:54.000000 twitterexplorer-0.6.7/twitterexplorer/html/rtn_graph_private.js
--rw-r--r--   0 ap         (501) staff       (20)    10444 2022-11-20 11:10:00.000000 twitterexplorer-0.6.7/twitterexplorer/html/style.css
--rw-r--r--   0 ap         (501) staff       (20)     3644 2022-06-27 14:12:19.000000 twitterexplorer-0.6.7/twitterexplorer/languages.json
--rw-r--r--   0 ap         (501) staff       (20)      757 2023-02-02 18:25:51.000000 twitterexplorer-0.6.7/twitterexplorer/launcher.py
--rw-r--r--   0 ap         (501) staff       (20)     1367 2023-01-27 17:08:54.000000 twitterexplorer-0.6.7/twitterexplorer/legacy.py
--rw-r--r--   0 ap         (501) staff       (20)    22559 2023-03-06 07:38:43.000000 twitterexplorer-0.6.7/twitterexplorer/networks.py
--rw-r--r--   0 ap         (501) staff       (20)     3742 2023-02-09 11:31:21.000000 twitterexplorer-0.6.7/twitterexplorer/plotting.py
--rw-r--r--   0 ap         (501) staff       (20)     3582 2023-01-27 15:54:41.000000 twitterexplorer-0.6.7/twitterexplorer/streamlitutils.py
--rw-r--r--   0 ap         (501) staff       (20)    18521 2023-02-12 14:14:39.000000 twitterexplorer-0.6.7/twitterexplorer/tweetcollector.py
-drwxr-xr-x   0 ap         (501) staff       (20)        0 2023-03-06 07:44:04.510112 twitterexplorer-0.6.7/twitterexplorer.egg-info/
--rw-r--r--   0 ap         (501) staff       (20)     6115 2023-03-06 07:44:04.000000 twitterexplorer-0.6.7/twitterexplorer.egg-info/PKG-INFO
--rw-r--r--   0 ap         (501) staff       (20)     1052 2023-03-06 07:44:04.000000 twitterexplorer-0.6.7/twitterexplorer.egg-info/SOURCES.txt
--rw-r--r--   0 ap         (501) staff       (20)        1 2023-03-06 07:44:04.000000 twitterexplorer-0.6.7/twitterexplorer.egg-info/dependency_links.txt
--rw-r--r--   0 ap         (501) staff       (20)       66 2023-03-06 07:44:04.000000 twitterexplorer-0.6.7/twitterexplorer.egg-info/entry_points.txt
--rw-r--r--   0 ap         (501) staff       (20)      124 2023-03-06 07:44:04.000000 twitterexplorer-0.6.7/twitterexplorer.egg-info/requires.txt
--rw-r--r--   0 ap         (501) staff       (20)       16 2023-03-06 07:44:04.000000 twitterexplorer-0.6.7/twitterexplorer.egg-info/top_level.txt
--rw-r--r--   0 ap         (501) staff       (20)        1 2023-02-02 19:12:34.000000 twitterexplorer-0.6.7/twitterexplorer.egg-info/zip-safe
+drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-26 13:23:25.465667 twitterexplorer-0.7.0/
+-rw-r--r--   0 ap         (501) staff       (20)    35149 2022-03-09 18:04:12.000000 twitterexplorer-0.7.0/LICENSE
+-rw-r--r--   0 ap         (501) staff       (20)     6344 2024-04-26 13:23:25.464744 twitterexplorer-0.7.0/PKG-INFO
+-rw-r--r--   0 ap         (501) staff       (20)     5766 2023-02-02 19:05:33.000000 twitterexplorer-0.7.0/README.md
+-rw-r--r--   0 ap         (501) staff       (20)       38 2024-04-26 13:23:25.465867 twitterexplorer-0.7.0/setup.cfg
+-rw-r--r--   0 ap         (501) staff       (20)     1310 2023-03-06 07:41:49.000000 twitterexplorer-0.7.0/setup.py
+drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-26 13:23:25.452182 twitterexplorer-0.7.0/twitterexplorer/
+-rw-r--r--   0 ap         (501) staff       (20)       51 2023-01-29 12:30:05.000000 twitterexplorer-0.7.0/twitterexplorer/__init__.py
+-rw-r--r--   0 ap         (501) staff       (20)       22 2024-04-26 13:07:18.000000 twitterexplorer-0.7.0/twitterexplorer/__version__.py
+drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-26 13:23:25.457044 twitterexplorer-0.7.0/twitterexplorer/apps/
+-rw-r--r--   0 ap         (501) staff       (20)        0 2023-02-02 18:13:22.000000 twitterexplorer-0.7.0/twitterexplorer/apps/__init__.py
+-rw-r--r--   0 ap         (501) staff       (20)    13876 2023-02-12 14:04:34.000000 twitterexplorer-0.7.0/twitterexplorer/apps/collector.py
+-rw-r--r--   0 ap         (501) staff       (20)    16222 2024-04-21 08:33:31.000000 twitterexplorer-0.7.0/twitterexplorer/apps/visualizer.py
+-rw-r--r--   0 ap         (501) staff       (20)     1654 2023-01-29 19:40:52.000000 twitterexplorer-0.7.0/twitterexplorer/constants.py
+-rw-r--r--   0 ap         (501) staff       (20)     5510 2024-04-22 12:52:58.000000 twitterexplorer-0.7.0/twitterexplorer/converters.py
+-rw-r--r--   0 ap         (501) staff       (20)     2279 2023-01-29 19:39:29.000000 twitterexplorer-0.7.0/twitterexplorer/d3networks.py
+-rw-r--r--   0 ap         (501) staff       (20)      547 2023-01-29 19:14:21.000000 twitterexplorer-0.7.0/twitterexplorer/defaults.py
+-rw-r--r--   0 ap         (501) staff       (20)     4599 2023-01-30 08:22:02.000000 twitterexplorer-0.7.0/twitterexplorer/helpers.py
+drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-26 13:23:25.462900 twitterexplorer-0.7.0/twitterexplorer/html/
+-rw-r--r--   0 ap         (501) staff       (20)     2059 2022-03-24 14:02:48.000000 twitterexplorer-0.7.0/twitterexplorer/html/head.html
+-rw-r--r--   0 ap         (501) staff       (20)     3701 2024-04-21 10:23:47.000000 twitterexplorer-0.7.0/twitterexplorer/html/htn_body.html
+-rw-r--r--   0 ap         (501) staff       (20)    13099 2024-04-21 08:31:53.000000 twitterexplorer-0.7.0/twitterexplorer/html/htn_graph.js
+-rw-r--r--   0 ap         (501) staff       (20)     5816 2023-04-06 10:02:16.000000 twitterexplorer-0.7.0/twitterexplorer/html/rtn_body.html
+-rw-r--r--   0 ap         (501) staff       (20)    20177 2024-04-19 14:50:09.000000 twitterexplorer-0.7.0/twitterexplorer/html/rtn_graph.js
+-rw-r--r--   0 ap         (501) staff       (20)    20204 2022-11-20 11:09:54.000000 twitterexplorer-0.7.0/twitterexplorer/html/rtn_graph_private.js
+-rw-r--r--   0 ap         (501) staff       (20)    10444 2022-11-20 11:10:00.000000 twitterexplorer-0.7.0/twitterexplorer/html/style.css
+-rw-r--r--   0 ap         (501) staff       (20)     3644 2022-06-27 14:12:19.000000 twitterexplorer-0.7.0/twitterexplorer/languages.json
+-rw-r--r--   0 ap         (501) staff       (20)      757 2023-02-02 18:25:51.000000 twitterexplorer-0.7.0/twitterexplorer/launcher.py
+-rw-r--r--   0 ap         (501) staff       (20)     1367 2023-01-27 17:08:54.000000 twitterexplorer-0.7.0/twitterexplorer/legacy.py
+-rw-r--r--   0 ap         (501) staff       (20)    23243 2024-04-21 08:35:00.000000 twitterexplorer-0.7.0/twitterexplorer/networks.py
+-rw-r--r--   0 ap         (501) staff       (20)     3742 2023-03-27 20:39:36.000000 twitterexplorer-0.7.0/twitterexplorer/plotting.py
+-rw-r--r--   0 ap         (501) staff       (20)     3622 2024-04-19 15:21:39.000000 twitterexplorer-0.7.0/twitterexplorer/streamlitutils.py
+-rw-r--r--   0 ap         (501) staff       (20)    18521 2023-02-12 14:14:39.000000 twitterexplorer-0.7.0/twitterexplorer/tweetcollector.py
+drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-26 13:23:25.463723 twitterexplorer-0.7.0/twitterexplorer.egg-info/
+-rw-r--r--   0 ap         (501) staff       (20)     6344 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/PKG-INFO
+-rw-r--r--   0 ap         (501) staff       (20)     1052 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 ap         (501) staff       (20)        1 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 ap         (501) staff       (20)       66 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/entry_points.txt
+-rw-r--r--   0 ap         (501) staff       (20)      124 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/requires.txt
+-rw-r--r--   0 ap         (501) staff       (20)       16 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/top_level.txt
+-rw-r--r--   0 ap         (501) staff       (20)        1 2023-02-02 19:12:34.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/zip-safe
```

### Comparing `twitterexplorer-0.6.7/LICENSE` & `twitterexplorer-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/PKG-INFO` & `twitterexplorer-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: twitterexplorer
-Version: 0.6.7
-Summary: A Python tool for interactive network visualizations of Twitter data.
-Home-page: http://github.com/pournaki/twitter-explorer
-Author: Armin Pournaki
-License: GPLv3
-Keywords: networks,social media
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![twitter explorer][title-img]][title-url]<br/>
 
 An interface to explore Twitter data through interactive network visualizations.
 
 ## Features
 
 The **twitter explorer** helps computational social scientists to:
```

### Comparing `twitterexplorer-0.6.7/README.md` & `twitterexplorer-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: twitterexplorer
+Version: 0.7.0
+Summary: A Python tool for interactive network visualizations of Twitter data.
+Home-page: http://github.com/pournaki/twitter-explorer
+Author: Armin Pournaki
+License: GPLv3
+Keywords: networks,social media
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: streamlit<2,>=1.7.0
+Requires-Dist: tweepy<5,>=4.6.0
+Requires-Dist: pandas<2,>=1.3.4
+Requires-Dist: python-igraph<1,>=0.9.8
+Requires-Dist: twitwi>=0.15.0
+Requires-Dist: twarc<3,>=2.9.4
+Requires-Dist: louvain>=0.8.0
+
 [![twitter explorer][title-img]][title-url]<br/>
 
 An interface to explore Twitter data through interactive network visualizations.
 
 ## Features
 
 The **twitter explorer** helps computational social scientists to:
```

### Comparing `twitterexplorer-0.6.7/setup.py` & `twitterexplorer-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/apps/collector.py` & `twitterexplorer-0.7.0/twitterexplorer/apps/collector.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/apps/visualizer.py` & `twitterexplorer-0.7.0/twitterexplorer/apps/visualizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import datetime as dt
 
 from twitterexplorer.legacy import *
 from twitterexplorer.helpers import *
 from twitterexplorer.streamlitutils import *
 from twitterexplorer.plotting import *
 from twitterexplorer.converters import twitterjsonl_to_twitwicsv
+from twitterexplorer.converters import zeeschuimerjsonl_to_twitwicsv
 from twitterexplorer.converters import export_graph
 from twitterexplorer.defaults import *
 from twitterexplorer.constants import *
 from twitterexplorer.__version__ import __version__
 from twitterexplorer.networks import InteractionNetwork
 from twitterexplorer.networks import SemanticNetwork
 
@@ -53,15 +54,15 @@
 
     st.write(f'`You selected {filename}.`<br>\
         `The file size is about {filesize}MB.`', unsafe_allow_html=True)
 
     outputdir = DEFAULT_OUTPUT_DIR
     projectdir = outputdir + project
 
-    @st.cache
+    @st.cache_data
     def load_data(path):
         try:
             df = pd.read_csv(path,
                              dtype=twitwi_schema,
                              usecols=cols_to_load,
                              low_memory=False,
                              # lineterminator='\n'
@@ -77,19 +78,24 @@
             df = df.drop_duplicates('id',keep='last')                
         return df    
 
     if filename[-3:] == "csv":
         df = load_data(filename)
     elif filename[-5:] == "jsonl":
         ## convert to twitwi csv
-        with st.spinner("Converting to twitwi csv..."):
+        with st.spinner("Converting raw API to twitwi csv..."):
             twitterjsonl_to_twitwicsv(filename)
         filename = filename.replace("jsonl","csv")
         df = load_data(filename)
-    
+    elif filename[-6:] == "ndjson":
+        ## convert to twitwi csv
+        with st.spinner("Converting Zeeschuimer to twitwi csv..."):
+            zeeschuimerjsonl_to_twitwicsv(filename)
+        filename = filename.replace("ndjson","csv")
+        df = load_data(filename)    
     timeseries = tweetdf_to_timeseries(df,frequency="1H")
     timeseries_plot = plot_timeseries(timeseries)
     st.altair_chart(timeseries_plot, use_container_width=True)
 
     langbars = plot_tweetlanguages(df)
     st.altair_chart(langbars, use_container_width=True)
 
@@ -189,15 +195,15 @@
             st.error("Please choose only one of the aggregations")
 
         st.write('<span style="text-decoration: underline;">Community detection</span>', 
                  unsafe_allow_html=True)
         rtn_louvain = st.checkbox("Louvain", key='rtn_louvain', help="Requires the installation of the 'louvain' package, currently not working on M1 machines.")
         rtn_leiden = st.checkbox("Leiden", key='rtn_leiden')
 
-        if st.button("Generate Interaction Network"):
+        if st.button("Generate interaction network"):
             if not os.path.exists(projectdir):
                 os.makedirs(projectdir)
 
             with st.spinner("Creating interaction network..."):
 
                 G = InteractionNetwork()
                 G.build_network(pandas_dataframe=df,
@@ -241,48 +247,58 @@
 
             if N_edges > 1e5:
                 st.warning("The network you are trying to visualize has \
                           more than 10,000 links. Consider using a stronger\
                           aggregation method if the interactive visualization is\
                           unresponsive.")
             
-    with st.expander("HASHTAG NETWORK"):
-        st.write("Undirected network in which nodes are hashtags. \
+    with st.expander("SEMANTIC NETWORK"):
+        coocurrence_type = st.selectbox(label='Coocurrence type',
+                                        options=['hashtag','mention'])
+        if coocurrence_type == 'hashtag':
+            cooc_savename = "co-hashtag-network"
+            st.write("Undirected network in which nodes are hashtags. \
                   A link is drawn between `i` and `j` if they appear in the same tweet.")
+        elif coocurrence_type == 'mention':
+            cooc_savename = "co-mention-network"            
+            st.write("Undirected network in which nodes are user screen names. \
+                  A link is drawn between `i` and `j` if they are mentioned in the same tweet.")
+
         st.write('<span style="text-decoration: underline;">Options</span>', 
                  unsafe_allow_html=True)
         htn_giantcomponent = st.checkbox("Giant component", key='htn_giantcomponent', help="Reduce the network to its largest connected component.")
         htn_export = st.checkbox("Export the graph to GML, GV and Edgelist",key="htn_export")
         node_thresh_htn = 0
         link_thresh_htn = 0
         node_thresh_htn = st.slider("Remove hashtags that appear less than x times", 
                                     0, 100, 1, 1, 
                                     key='n_thresh_htn')
         link_thresh_htn = st.slider("Remove edges that link hashtags less than than x times", 
                                     0, 50, 1, 1, 
                                     key='l_thresh_htn')
-        ht_to_remove = st.text_input(label="Hashtags to be removed from the graph, separated by '|'",
+        ht_to_remove = st.text_input(label="Nodes to be removed from the graph, separated by '|'",
                                      help="It is recommended to remove the hashtag used for the query.")
         if ht_to_remove != "":
             ht_to_remove_list = ht_to_remove.split("|")
         else:
             ht_to_remove_list = None
         st.write('<span style="text-decoration: underline;">Community detection</span>', 
                  unsafe_allow_html=True)
         htn_louvain = st.checkbox("Louvain", key='htn_louvain', help="Requires the installation of the 'louvain' package, currently not working on M1 machines.")
         htn_leiden = st.checkbox("Leiden", key='htn_leiden')
 
 
-        if st.button("Generate Hashtag Network"):
+        if st.button("Generate semantic network"):
             if not os.path.exists(projectdir):
                 os.makedirs(projectdir)
-            with st.spinner("Creating hashtag network..."):
+            with st.spinner("Creating semantic network..."):
                 H = SemanticNetwork()
                 ## build a network from the data
                 H.build_network(pandas_dataframe=df,
+                                network_type=coocurrence_type,
                                 language_filter=langselector_iso,
                                 hashtags_to_remove=ht_to_remove_list,
                                 starttime=ts0,
                                 endtime=ts1,
                                              )
                 H.reduce_network(giant_component=htn_giantcomponent,
                                  node_threshold=node_thresh_htn,
@@ -293,19 +309,19 @@
                                collected_on=collectedon)
 
             if langselector != [] and langselector != None:
                 if os.name == 'nt': # windows does not accept "|" in filenames
                     language_savesuffix = str(langselector_iso).replace("[","").replace("]","").replace(",","-").replace(" ","").replace("'","")
                 else:
                     language_savesuffix = str(langselector_iso).replace("[","").replace("]","").replace(",","|").replace(" ","").replace("'","")
-                savename = f"{projectdir}/{project}_nt{node_thresh_htn}_lt{link_thresh_htn}_HTN_{language_savesuffix}"
-                exportname = f"{projectdir}/export/{project}_nt{node_thresh_htn}_lt{link_thresh_htn}_HTN_{language_savesuffix}"
+                savename = f"{projectdir}/{project}_nt{node_thresh_htn}_lt{link_thresh_htn}_{cooc_savename}_{language_savesuffix}"
+                exportname = f"{projectdir}/export/{project}_nt{node_thresh_htn}_lt{link_thresh_htn}_{cooc_savename}_{language_savesuffix}"
             else:
-                savename = f"{projectdir}/{project}_nt{node_thresh_htn}_lt{link_thresh_htn}_HTN"
-                exportname = f"{projectdir}/export/{project}_nt{node_thresh_htn}_lt{link_thresh_htn}_HTN"                
+                savename = f"{projectdir}/{project}_nt{node_thresh_htn}_lt{link_thresh_htn}_{cooc_savename}"
+                exportname = f"{projectdir}/export/{project}_nt{node_thresh_htn}_lt{link_thresh_htn}_{cooc_savename}"                
             
             with st.spinner("Writing html..."):
                 st.success(f"`Saved the interactive hashtag network as to: {savename}.html`.")
                 H.write_html(savename + ".html")
 
             if htn_export:
                 exportdir = f"{projectdir}/export/"
```

### Comparing `twitterexplorer-0.6.7/twitterexplorer/constants.py` & `twitterexplorer-0.7.0/twitterexplorer/constants.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/d3networks.py` & `twitterexplorer-0.7.0/twitterexplorer/d3networks.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/defaults.py` & `twitterexplorer-0.7.0/twitterexplorer/defaults.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/helpers.py` & `twitterexplorer-0.7.0/twitterexplorer/helpers.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/html/head.html` & `twitterexplorer-0.7.0/twitterexplorer/html/head.html`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/html/htn_body.html` & `twitterexplorer-0.7.0/twitterexplorer/html/htn_body.html`

 * *Files 5% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 </div>
 <div class="borders">
 <div class= "subtitle" id="panel02">NETWORK MEASURES</div>
 <div class = "content" id="content02">
 </div>
 </div>
 <div class="borders">
-<div class= "subtitle" id="panel03">HASHTAG INFORMATION</div>
+<div class= "subtitle" id="panel03">NODE INFORMATION</div>
 <div class = "content" id="content03">
-    <div class="description"> Search hashtag</div>
+    <div class="description"> Search node</div>
         <input id="searchuser" type="search"/>
         <br>
         <a href="javascript:void(0);" onclick="zoomonuser()" class="button1">Zoom on node</a>
         <a href="javascript:void(0);" onclick="openhashtag()" class="button1">Open timeline</a> 
 <br><br>
     <div id="userinfostring"></div>        
 </div>
 </div>
 
-<div id="footer"><a href="https://twitterexplorer.org">twitter explorer v0.3.1</a></div></div>
-
+<!-- <div id="footer"><a href="https://twitterexplorer.org">twitter explorer v0.3.1</a></div> -->
+</div>
 <div id="graph" style="width:100%;height: 100%;position: absolute;"></div>
```

#### html2text {}

```diff
@@ -4,13 +4,12 @@
 
 Size scale
 [Unknown INPUT type]
 Node repulsion
 [Unknown INPUT type]
 _T_o_g_g_l_e_ _l_i_n_k_ _v_i_s_i_b_i_l_i_t_y
 NETWORK MEASURES
-HASHTAG INFORMATION
-Search hashtag
+NODE INFORMATION
+Search node
 [Unknown INPUT type]
 _Z_o_o_m_ _o_n_ _n_o_d_e _O_p_e_n_ _t_i_m_e_l_i_n_e
 
-_t_w_i_t_t_e_r_ _e_x_p_l_o_r_e_r_ _v_0_._3_._1
```

### Comparing `twitterexplorer-0.6.7/twitterexplorer/html/htn_graph.js` & `twitterexplorer-0.7.0/twitterexplorer/html/htn_graph.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,18 @@
 < script >
     var colorselector = document.getElementById("nodecolor");
 var nodescaling = 3;
 var darkmode = false
 
+if (data.graph.cooc == "mention") {
+    var prefix = "@"
+} else if (data.graph.cooc == "hashtag") {
+    var prefix = "#"
+}
+
 // get node color options
 ms = document.getElementById('nodecolor')
 if ('louvain_com' in data.nodes[0]) {
     ms.innerHTML += `<option value = "louvain_com">Louvain community</option>\n`
 }
 if ('leiden_com' in data.nodes[0]) {
     ms.innerHTML += `<option value = "leiden_com">Leiden community</option>\n`
@@ -30,15 +36,15 @@
 
         ctx.fillStyle = 'rgba(255, 255, 255, 0.8)';
         // ctx.fillRect(node.x - bckgDimensions[0] / 2, node.y - bckgDimensions[1] / 2, ...bckgDimensions);
 
         ctx.textAlign = 'center';
         ctx.textBaseline = 'middle';
         ctx.fillStyle = "black";
-        ctx.fillText("#" + label, node.x, node.y);
+        ctx.fillText(prefix + label, node.x, node.y);
     })
     .nodeId('id')
     .linkHoverPrecision(10)
     .linkColor(link => 'rgba(0,0,0,0.1)')
     .onNodeClick(node => {
         highlight(node)
     })
@@ -89,15 +95,15 @@
 
         ctx.fillStyle = 'rgba(255, 255, 255, 1.0)';
         // ctx.fillRect(node.x - bckgDimensions[0] / 2, node.y - bckgDimensions[1] / 2, ...bckgDimensions);
 
         ctx.textAlign = 'center';
         ctx.textBaseline = 'middle';
         ctx.fillStyle = colorbar[node.colorthat];
-        ctx.fillText("#" + label, node.x, node.y);
+        ctx.fillText(prefix + label, node.x, node.y);
     })
     // linkcolor depending on dark/lightmode
     var bodyelement = document.querySelector('body')
     var bodystyle = window.getComputedStyle(bodyelement)
     var bg = bodystyle.getPropertyValue('color')
     if (bg === 'rgb(0, 0, 0)') {
         var colorbar2 = ['rgba(0,0,0,0.05)', 'rgba(255,0,0,0.5)']
@@ -135,15 +141,15 @@
         } else {
             if (darkmode == true) {
                 ctx.fillStyle = "white";
             } else {
                 ctx.fillStyle = "black";
             }
         }
-        ctx.fillText("#" + label, node.x, node.y);
+        ctx.fillText(prefix + label, node.x, node.y);
     })
     if (darkmode == false) {
         Graph.linkColor(link => 'rgba(0,0,0,0.1)')
     } else {
         Graph.linkColor(link => 'rgba(255,255,255,0.2)')
     }
 
@@ -196,15 +202,15 @@
             if (bytype == "louvain_com") {
                 ctx.fillStyle = colorscale[node["louvain_com"]]
             } else if (bytype == "leiden_com") {
                 ctx.fillStyle = colorscale[node["leiden_com"]]
             } else {
                 ctx.fillStyle = "white"
             };
-            ctx.fillText("#" + label, node.x, node.y);
+            ctx.fillText(prefix + label, node.x, node.y);
         })
     } else {
         darkmode = false
         document.documentElement.setAttribute('data-theme', 'lighttheme');
         Graph.linkColor(() => 'rgba(0,0,0,0.2)');
         Graph.nodeCanvasObject((node, ctx, globalScale) => {
             const label = node.name;
@@ -221,15 +227,15 @@
             if (bytype == "louvain_com") {
                 ctx.fillStyle = colorscale[node["louvain_com"]]
             } else if (bytype == "leiden_com") {
                 ctx.fillStyle = colorscale[node["leiden_com"]]
             } else {
                 ctx.fillStyle = "black"
             };
-            ctx.fillText("#" + label, node.x, node.y);
+            ctx.fillText(prefix + label, node.x, node.y);
         })
     }
 }
 
 var colorscale = ['#e6194b', '#3cb44b', '#ffe119', '#4363d8', '#f58231', '#911eb4', '#46f0f0', '#f032e6', '#bcf60c', '#fabebe', '#008080', '#e6beff', '#9a6324', '#fffac8', '#800000', '#aaffc3', '#808000', '#ffd8b1', '#000075', '#808080', '#ffffff', '#000000']
 
 function changecolor(bytype) {
@@ -252,15 +258,15 @@
         if (bytype == "louvain_com") {
             ctx.fillStyle = colorscale[node["louvain_com"]]
         } else if (bytype == "leiden_com") {
             ctx.fillStyle = colorscale[node["leiden_com"]]
         } else {
             ctx.fillStyle = "black"
         };
-        ctx.fillText("#" + label, node.x, node.y);
+        ctx.fillText(prefix + label, node.x, node.y);
     })
 }
 
 document.getElementById("nodecolor").addEventListener("change", recolornodes);
 
 function recolornodes() {
 
@@ -281,15 +287,20 @@
         }
         changecolor("none")
     }
 }
 
 function openhashtag() {
     var hashtagname = document.getElementById("searchuser").value;
-    window.open(`https://twitter.com/search?q=%23${hashtagname}`, '_blank');
+    if (data.graph.cooc == "hashtag") {
+        window.open(`https://twitter.com/search?q=%23${hashtagname}`, '_blank');
+    } else if (data.graph.cooc == "mention") {
+        window.open(`https://twitter.com/${hashtagname}`, '_blank');
+    }
+
 }
 
 // NODE SIZE
 document.getElementById("slido").addEventListener("change", rescalenodes);
 
 function rescalenodes() {
     var colorselector = document.getElementById("nodecolor");
@@ -313,15 +324,15 @@
             ctx.fillStyle = colorscale[node["louvain_com"]];
         } else if (selectedoption == "leiden_com") {
             ctx.fillStyle = colorscale[node["leiden_com"]];
         } else {
             ctx.fillStyle = "black";
         }
 
-        ctx.fillText("#" + label, node.x, node.y);
+        ctx.fillText(prefix + label, node.x, node.y);
     })
 
 }
 
 function make_screenshot() {
     // var canvas = document.getElementsByClassName('force-graph-container')[0]['children'][0];
     var canvas = document.getElementById('graph')['children'][0]['children'][0]
```

### Comparing `twitterexplorer-0.6.7/twitterexplorer/html/rtn_body.html` & `twitterexplorer-0.7.0/twitterexplorer/html/rtn_body.html`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         <div class="description">Node size (variable scale)</div>
             <select id = "nodesize">
                 <option value = "none">None</option>
                 <option value = "in_degree" id="indegreeoption">In-Degree (number of times the user got retweeted)</option>
                 <option value = "out_degree" id="outdegreeoption">Out-Degree (number of times the user retweeted someone)</option>
                 <option value = "followers">Number of followers</option>
                 <option value = "friends">Number of followed accounts</option>
+                <option value = "pagerank">PageRank</option>
             </select>
         </div>
         <div class="description" id="scale">Size scale</div>
         <div class="slidecontainer">
           <input type="range" min="0.2" max="20" value="2" id="slido">
         </div>
         <a href="javascript:void(0);" onclick="toggle_linkvisibility()" class="button2">Toggle link visibility</a>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 VISUALIZATION OPTIONS
 Auto-color nodes by
 
 
 Node size (variable scale)
 [One of: None/In-Degree (number of times the user got retweeted)/Out-Degree
 (number of times the user retweeted someone)/Number of followers/Number of
-followed accounts]
+followed accounts/PageRank]
 Size scale
 [Unknown INPUT type]
 _T_o_g_g_l_e_ _l_i_n_k_ _v_i_s_i_b_i_l_i_t_y
 Filter edges by day (experimental feature)
 [Unknown INPUT type]
 NETWORK MEASURES
 ACCOUNT INFORMATION
```

### Comparing `twitterexplorer-0.6.7/twitterexplorer/html/rtn_graph.js` & `twitterexplorer-0.7.0/twitterexplorer/html/rtn_graph.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -326,14 +326,16 @@
         Graph.nodeVal(node => node[selectedoption] * 0.000005 * newscale)
     } else if (selectedoption === "friends") {
         Graph.nodeVal(node => node[selectedoption] * 0.001 * newscale)
     } else if (selectedoption === "out_degree") {
         Graph.nodeVal(node => node[selectedoption] * 0.1 * newscale)
     } else if (selectedoption === "in_degree") {
         Graph.nodeVal(node => node[selectedoption] * 0.1 * newscale)
+    } else if (selectedoption === "pagerank") {
+        Graph.nodeVal(node => node[selectedoption] * 10 * newscale)
     }
 }
 
 document.getElementById("nodesize").addEventListener("change", changenodesize);
 
 function changenodesize() {
     var sizeselector = document.getElementById("nodesize");
@@ -342,14 +344,16 @@
         Graph.nodeVal(node => node[selectedoption] * 0.00005)
     } else if (selectedoption === "friends") {
         Graph.nodeVal(node => node[selectedoption] * 0.001)
     } else if (selectedoption === "out_degree") {
         Graph.nodeVal(node => node[selectedoption] * 1.0)
     } else if (selectedoption === "in_degree") {
         Graph.nodeVal(node => node[selectedoption] * 1.0)
+    } else if (selectedoption === "pagerank") {
+        Graph.nodeVal(node => node[selectedoption] * 10)
     } else {
         Graph.nodeVal(node => 1.0)
     }
 }
 
 $(function() {
     var colval = "none";
```

### Comparing `twitterexplorer-0.6.7/twitterexplorer/html/rtn_graph_private.js` & `twitterexplorer-0.7.0/twitterexplorer/html/rtn_graph_private.js`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/html/style.css` & `twitterexplorer-0.7.0/twitterexplorer/html/style.css`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/languages.json` & `twitterexplorer-0.7.0/twitterexplorer/languages.json`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/launcher.py` & `twitterexplorer-0.7.0/twitterexplorer/launcher.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/legacy.py` & `twitterexplorer-0.7.0/twitterexplorer/legacy.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/networks.py` & `twitterexplorer-0.7.0/twitterexplorer/networks.py`

 * *Files 5% similar despite different names*

```diff
@@ -243,26 +243,28 @@
         private (boolean): if private is true, nodes with less than 5000 followers are rendered unclickable
         
         Returns:
         self._d3dict (graph in json format {'nodes':[], 'links':[]})
         """    
         G = self._graph
         d3graph = {'nodes': [], 'links': []}
+        pr = G.pagerank()
         for v in G.vs:
             ndict = {}
             node_id = v.index
             ndict["id"] = node_id
             ndict["twitter_id"] = v["name"]
             ndict["screen_name"] = v["screen_name"]
             ndict["followers"] = v["followers"]
             ndict["friends"] = v["friends"]
             ndict["interactions"] = v["interactions"]
             ndict["otweets"] = v["originaltweets"]        
             ndict["in_degree"] = G.degree(v, mode='in')
-            ndict["out_degree"] = G.degree(v, mode='out')            
+            ndict["out_degree"] = G.degree(v, mode='out')
+            ndict["pagerank"] = pr[node_id]            
             try:
                 ndict["in_degree_pa"] = v['in-degree-preagg']
                 ndict["out_degree_pa"] = v['out-degree-preagg']            
             except KeyError:
                 pass
             
             if private == True:
@@ -345,18 +347,20 @@
         self._removed_hashtags = []
         self._reduction_methods = {'giant_component':False,
                                    'node_threshold':0,
                                    'link_threshold':0}                                
         self._community_detection = {'louvain':False,
                                      'leiden':False}
         self._d3dict = None
-        
+        self._networktype = None
+        self._networktype_html = None
 
     def build_network(self, 
                       pandas_dataframe,
+                      network_type="hashtag",
                       hashtags_to_remove=None,
                       starttime=None,
                       endtime=None,
                       language_filter=None):
         """Generate Semantic Network from Twitter CSV data collection.
 
         Parameters:
@@ -366,23 +370,33 @@
         language_filter (list): list of ISO-code languages to keep
 
         Returns:
         self._graph (igraph graph object): retweet network where a link is created
         from i to j if i retweeted j
         """    
 
+        if network_type == "hashtag":
+            type_field = "hashtags"
+            self._networktype = "hashtag"            
+            self._networktype_html = "Co-hashtag network"
+        elif network_type == "mention":
+            type_field = "mentioned_names"
+            self._networktype = "mention"
+            self._networktype_html = "Co-mention network"
+
         hdf = pandas_dataframe.copy()
         if language_filter != None:
             hdf = hdf[hdf['lang'].isin(language_filter)]
 
         if starttime != None and endtime != None:
             hdf = hdf[(hdf['timestamp_utc'] >= starttime) & (hdf['timestamp_utc']<= endtime)]
-        hdf = hdf[hdf['hashtags'].notna()]
-        hdf = hdf[hdf['hashtags'].str.contains('|')]
-        cohashtags = list(hdf['hashtags'])
+        hdf = hdf[hdf[type_field].notna()]
+        hdf = hdf[hdf[type_field].str.contains('|')]        
+        hdf[type_field] = hdf[type_field].str.lower()
+        cohashtags = list(hdf[type_field])
         times = list(hdf['timestamp_utc'])
         edgelist = []
         for idx,cohashtag in enumerate(cohashtags):
             hashtaglist = cohashtag.split('|')
             combs = list(combinations(hashtaglist,2))
             for comb in combs:
                 comb = list(comb)
@@ -393,15 +407,15 @@
                               vertices=None, 
                               directed=False)
 
         ## remove certain hashtags from the network
         if hashtags_to_remove != None:
             nodes_to_remove = []
             for ht in hashtags_to_remove:                        
-                ht = ht.replace("#","")
+                ht = ht.replace("#","").replace("@","")
                 idx_of_ht = np.where(np.array(H.vs['name']) == ht)[0][0]
                 nodes_to_remove.append(idx_of_ht)
             H.delete_vertices(nodes_to_remove)
         
         self._graph = H
         self._removed_hashtags = hashtags_to_remove
 
@@ -524,15 +538,16 @@
             d3graph['links'].append(ldict)
         
         timestamps = self._graph.es['time']
         firstdate_str = str(dt.datetime.fromtimestamp(timestamps[-1]))[:16]
         lastdate_str = str(dt.datetime.fromtimestamp(timestamps[0]))[:16]        
 
         d3graph['graph'] = {}
-        d3graph['graph']['type'] = "Hashtag network"
+        d3graph['graph']['type'] = self._networktype_html
+        d3graph['graph']['cooc'] = self._networktype
         d3graph['graph']['N_nodes'] = len(d3graph["nodes"])
         d3graph['graph']['N_links'] = len(d3graph["links"])
         d3graph['graph']['keyword'] = search_query
         d3graph['graph']['collected_on'] = collected_on
         d3graph['graph']['first_tweet'] = firstdate_str
         d3graph['graph']['last_tweet'] = lastdate_str
         d3graph['version_number'] = __version__
```

### Comparing `twitterexplorer-0.6.7/twitterexplorer/plotting.py` & `twitterexplorer-0.7.0/twitterexplorer/plotting.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer/streamlitutils.py` & `twitterexplorer-0.7.0/twitterexplorer/streamlitutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,14 @@
         st.error("The `./data` folder does not exist. Please create it and insert \
                 your Twitter collections in jsonl format (API v1.1) or twitwi.")
     if '.DS_Store' in filenames:
         filenames.remove('.DS_Store')
     filenames = list(reversed(sorted(filenames)))
     filenames.insert(0,'---')
     selected_filename = st.selectbox(
-        'Select a tweet collection inside ./data in JSONL (raw Twitter API v1.1) or CSV (twitwi/minet standard)', 
+        'Select a tweet collection inside ./data ending with CSV (twitwi/minet standard), NDJSON (Zeeschuimer standard) or JSONL (raw Twitter API v1.1)', 
         filenames,
         help='The function that loads the data uses @st.cache to speed up \
               repeated loading of the same dataset. If your dataset has changed\
               in between two runs but the filename is the same, please clear\
               the cache by pressing C.')
     return os.path.join(folder_path, selected_filename)
```

### Comparing `twitterexplorer-0.6.7/twitterexplorer/tweetcollector.py` & `twitterexplorer-0.7.0/twitterexplorer/tweetcollector.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.6.7/twitterexplorer.egg-info/PKG-INFO` & `twitterexplorer-0.7.0/twitterexplorer.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 Metadata-Version: 2.1
 Name: twitterexplorer
-Version: 0.6.7
+Version: 0.7.0
 Summary: A Python tool for interactive network visualizations of Twitter data.
 Home-page: http://github.com/pournaki/twitter-explorer
 Author: Armin Pournaki
 License: GPLv3
 Keywords: networks,social media
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: streamlit<2,>=1.7.0
+Requires-Dist: tweepy<5,>=4.6.0
+Requires-Dist: pandas<2,>=1.3.4
+Requires-Dist: python-igraph<1,>=0.9.8
+Requires-Dist: twitwi>=0.15.0
+Requires-Dist: twarc<3,>=2.9.4
+Requires-Dist: louvain>=0.8.0
 
 [![twitter explorer][title-img]][title-url]<br/>
 
 An interface to explore Twitter data through interactive network visualizations.
 
 ## Features
```

### Comparing `twitterexplorer-0.6.7/twitterexplorer.egg-info/SOURCES.txt` & `twitterexplorer-0.7.0/twitterexplorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

