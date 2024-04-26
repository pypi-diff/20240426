# Comparing `tmp/datalibro_utils-2.3.1.tar.gz` & `tmp/datalibro_utils-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalibro_utils-2.3.1.tar", last modified: Sun Apr  7 05:56:42 2024, max compression
+gzip compressed data, was "datalibro_utils-2.3.2.tar", last modified: Fri Apr 26 10:19:15 2024, max compression
```

## Comparing `datalibro_utils-2.3.1.tar` & `datalibro_utils-2.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 05:56:42.250104 datalibro_utils-2.3.1/
--rw-rw-rw-   0        0        0      301 2024-04-07 05:56:42.249112 datalibro_utils-2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1145 2023-11-01 08:51:17.000000 datalibro_utils-2.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 05:56:42.241937 datalibro_utils-2.3.1/datalibro_utils/
--rw-rw-rw-   0        0        0      180 2023-12-08 10:02:45.000000 datalibro_utils-2.3.1/datalibro_utils/__init__.py
--rw-rw-rw-   0        0        0     7743 2023-11-01 08:48:50.000000 datalibro_utils-2.3.1/datalibro_utils/datalibro_auth.py
--rw-rw-rw-   0        0        0     6617 2024-02-02 10:06:27.000000 datalibro_utils-2.3.1/datalibro_utils/dlbi.py
--rw-rw-rw-   0        0        0     1404 2023-11-01 08:51:17.000000 datalibro_utils-2.3.1/datalibro_utils/email.py
--rw-rw-rw-   0        0        0    13183 2024-04-07 05:56:09.000000 datalibro_utils-2.3.1/datalibro_utils/mapping.py
--rw-rw-rw-   0        0        0      866 2023-11-06 04:16:52.000000 datalibro_utils-2.3.1/datalibro_utils/openai.py
--rw-rw-rw-   0        0        0     2316 2023-10-27 10:47:34.000000 datalibro_utils-2.3.1/datalibro_utils/pet_sys.py
--rw-rw-rw-   0        0        0       80 2023-06-28 06:14:01.000000 datalibro_utils-2.3.1/datalibro_utils/test.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:56:42.249112 datalibro_utils-2.3.1/datalibro_utils.egg-info/
--rw-rw-rw-   0        0        0      301 2024-04-07 05:56:42.000000 datalibro_utils-2.3.1/datalibro_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-04-07 05:56:42.000000 datalibro_utils-2.3.1/datalibro_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 05:56:42.000000 datalibro_utils-2.3.1/datalibro_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-07 05:56:42.000000 datalibro_utils-2.3.1/datalibro_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-07 05:56:42.000000 datalibro_utils-2.3.1/datalibro_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 05:56:42.250104 datalibro_utils-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0      399 2024-04-07 05:56:25.000000 datalibro_utils-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:19:15.424294 datalibro_utils-2.3.2/
+-rw-rw-rw-   0        0        0      301 2024-04-26 10:19:15.424294 datalibro_utils-2.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1145 2023-11-01 08:51:17.000000 datalibro_utils-2.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 10:19:15.418261 datalibro_utils-2.3.2/datalibro_utils/
+-rw-rw-rw-   0        0        0      180 2023-12-08 10:02:45.000000 datalibro_utils-2.3.2/datalibro_utils/__init__.py
+-rw-rw-rw-   0        0        0     7743 2023-11-01 08:48:50.000000 datalibro_utils-2.3.2/datalibro_utils/datalibro_auth.py
+-rw-rw-rw-   0        0        0     6590 2024-04-26 10:08:14.000000 datalibro_utils-2.3.2/datalibro_utils/dlbi.py
+-rw-rw-rw-   0        0        0     1404 2023-11-01 08:51:17.000000 datalibro_utils-2.3.2/datalibro_utils/email.py
+-rw-rw-rw-   0        0        0    13183 2024-04-07 05:56:09.000000 datalibro_utils-2.3.2/datalibro_utils/mapping.py
+-rw-rw-rw-   0        0        0      866 2023-11-06 04:16:52.000000 datalibro_utils-2.3.2/datalibro_utils/openai.py
+-rw-rw-rw-   0        0        0     2316 2023-10-27 10:47:34.000000 datalibro_utils-2.3.2/datalibro_utils/pet_sys.py
+-rw-rw-rw-   0        0        0       80 2023-06-28 06:14:01.000000 datalibro_utils-2.3.2/datalibro_utils/test.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:19:15.422908 datalibro_utils-2.3.2/datalibro_utils.egg-info/
+-rw-rw-rw-   0        0        0      301 2024-04-26 10:19:15.000000 datalibro_utils-2.3.2/datalibro_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-26 10:19:15.000000 datalibro_utils-2.3.2/datalibro_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 10:19:15.000000 datalibro_utils-2.3.2/datalibro_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-26 10:19:15.000000 datalibro_utils-2.3.2/datalibro_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-26 10:19:15.000000 datalibro_utils-2.3.2/datalibro_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 10:19:15.424800 datalibro_utils-2.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      399 2024-04-26 10:19:06.000000 datalibro_utils-2.3.2/setup.py
```

### Comparing `datalibro_utils-2.3.1/README.md` & `datalibro_utils-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.1/datalibro_utils/datalibro_auth.py` & `datalibro_utils-2.3.2/datalibro_utils/datalibro_auth.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.1/datalibro_utils/dlbi.py` & `datalibro_utils-2.3.2/datalibro_utils/dlbi.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 from dateutil.relativedelta import relativedelta
 from datetime import date
 import time
 import plotly.express as px
 
 palette = ['#EB8957', '#F2C865', '#9ABC77', '#60A78C', '#5D8F8D', '#5D758E', '#3E7B9D', '#E7514B', '#E4793F','#EB993D', ]
 main_color = '#549084'
-# relative date
-today = date.today()
-relative_date = today + relativedelta(months=-1)
 
 def header(header):
      st.markdown(f'<p style="background-color:{main_color};color:#f9f9f9;font-size:24px;text-align:center;border-radius:10px">{header}</p>', unsafe_allow_html=True)
 
 def get_data_labels():
      return st.sidebar.toggle('Data Labels', value=True)
 
@@ -44,16 +41,16 @@
             label_visibility="hidden",
             key=col_name
         )
     if "(ALL)" in selection:
         selection = unique_values
     return selection
 
-def time_range_filter(s_date, relative_date=relative_date):
-    date_range = st.date_input('**Date Range**', (relative_date, today))
+def time_range_filter(s_date, relative_date=date.today() + relativedelta(months=-1)):
+    date_range = st.date_input('**Date Range**', (relative_date, date.today()))
     st.caption(f"*Date range from {min(s_date)} to {max(s_date)}")
     return date_range
 
 def cols_filter(df, filter_cols):
     return {col: add_multiselect(col, df) for col in filter_cols}
 
 def get_mask(df, date_col, date_range, selections):
@@ -93,15 +90,15 @@
     list_ani_val = [int(value/10), int(value/4), int(value/3*2)]
     with st.empty():
         for val in list_ani_val:
             st.metric(':rainbow['+label+']', f'{val:,}')
             time.sleep(0.08)
         st.metric(label, f'{value:,}')
 
-def side_control(df, date_col, view_size_cols, relative_date=relative_date, start_time_size=0, multi_pages=None):
+def side_control(df, date_col, view_size_cols, relative_date=date.today() + relativedelta(months=-1), start_time_size=0, multi_pages=None):
     with st.sidebar:
         data_labels = get_data_labels()
         page_selection = None
         if multi_pages:
             page_selection = st.radio(
                 "**Page**",
                 multi_pages
```

### Comparing `datalibro_utils-2.3.1/datalibro_utils/email.py` & `datalibro_utils-2.3.2/datalibro_utils/email.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.1/datalibro_utils/mapping.py` & `datalibro_utils-2.3.2/datalibro_utils/mapping.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.1/datalibro_utils/openai.py` & `datalibro_utils-2.3.2/datalibro_utils/openai.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.1/datalibro_utils/pet_sys.py` & `datalibro_utils-2.3.2/datalibro_utils/pet_sys.py`

 * *Files identical despite different names*

