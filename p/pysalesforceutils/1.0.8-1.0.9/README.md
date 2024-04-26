# Comparing `tmp/pysalesforceutils-1.0.8.tar.gz` & `tmp/pysalesforceutils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysalesforceutils-1.0.8.tar", last modified: Tue Mar 16 11:37:57 2021, max compression
+gzip compressed data, was "dist/pysalesforceutils-1.0.9.tar", last modified: Thu Apr 15 18:02:37 2021, max compression
```

## Comparing `pysalesforceutils-1.0.8.tar` & `pysalesforceutils-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gbarger    (501) staff       (20)        0 2021-03-16 11:37:57.416644 pysalesforceutils-1.0.8/
--rw-r--r--   0 gbarger    (501) staff       (20)     2828 2021-03-16 11:37:57.416263 pysalesforceutils-1.0.8/PKG-INFO
--rw-r--r--   0 gbarger    (501) staff       (20)     2284 2019-04-19 00:36:59.000000 pysalesforceutils-1.0.8/README.md
-drwxr-xr-x   0 gbarger    (501) staff       (20)        0 2021-03-16 11:37:57.365320 pysalesforceutils-1.0.8/pysalesforceutils.egg-info/
--rw-r--r--   0 gbarger    (501) staff       (20)     2828 2021-03-16 11:37:56.000000 pysalesforceutils-1.0.8/pysalesforceutils.egg-info/PKG-INFO
--rw-r--r--   0 gbarger    (501) staff       (20)      307 2021-03-16 11:37:56.000000 pysalesforceutils-1.0.8/pysalesforceutils.egg-info/SOURCES.txt
--rw-r--r--   0 gbarger    (501) staff       (20)        1 2021-03-16 11:37:56.000000 pysalesforceutils-1.0.8/pysalesforceutils.egg-info/dependency_links.txt
--rw-r--r--   0 gbarger    (501) staff       (20)       22 2021-03-16 11:37:56.000000 pysalesforceutils-1.0.8/pysalesforceutils.egg-info/requires.txt
--rw-r--r--   0 gbarger    (501) staff       (20)       29 2021-03-16 11:37:56.000000 pysalesforceutils-1.0.8/pysalesforceutils.egg-info/top_level.txt
--rw-r--r--   0 gbarger    (501) staff       (20)   157838 2021-03-16 11:36:47.000000 pysalesforceutils-1.0.8/pysalesforceutils.py
--rw-r--r--   0 gbarger    (501) staff       (20)       38 2021-03-16 11:37:57.416788 pysalesforceutils-1.0.8/setup.cfg
--rw-r--r--   0 gbarger    (501) staff       (20)      584 2021-03-16 11:37:37.000000 pysalesforceutils-1.0.8/setup.py
-drwxr-xr-x   0 gbarger    (501) staff       (20)        0 2021-03-16 11:37:57.415612 pysalesforceutils-1.0.8/test/
--rw-r--r--   0 gbarger    (501) staff       (20)       36 2019-12-28 04:54:18.000000 pysalesforceutils-1.0.8/test/test_pysalesforce.py
--rw-r--r--   0 gbarger    (501) staff       (20)      124 2020-02-06 04:20:10.000000 pysalesforceutils-1.0.8/test/test_webservice.py
--rw-r--r--   0 gbarger    (501) staff       (20)     5094 2021-03-16 11:20:31.000000 pysalesforceutils-1.0.8/webservice.py
+drwxr-xr-x   0 gbarger    (501) staff       (20)        0 2021-04-15 18:02:37.000000 pysalesforceutils-1.0.9/
+-rw-r--r--   0 gbarger    (501) staff       (20)     2828 2021-04-15 18:02:37.000000 pysalesforceutils-1.0.9/PKG-INFO
+-rw-r--r--   0 gbarger    (501) staff       (20)   159549 2021-04-15 18:01:29.000000 pysalesforceutils-1.0.9/pysalesforceutils.py
+drwxr-xr-x   0 gbarger    (501) staff       (20)        0 2021-04-15 18:02:37.000000 pysalesforceutils-1.0.9/test/
+-rw-r--r--   0 gbarger    (501) staff       (20)       36 2019-12-28 04:54:18.000000 pysalesforceutils-1.0.9/test/test_pysalesforce.py
+-rw-r--r--   0 gbarger    (501) staff       (20)      124 2020-02-06 04:20:10.000000 pysalesforceutils-1.0.9/test/test_webservice.py
+-rw-r--r--   0 gbarger    (501) staff       (20)     5094 2021-03-16 11:20:31.000000 pysalesforceutils-1.0.9/webservice.py
+-rw-r--r--   0 gbarger    (501) staff       (20)     2284 2019-04-19 00:36:59.000000 pysalesforceutils-1.0.9/README.md
+-rw-r--r--   0 gbarger    (501) staff       (20)      584 2021-04-15 18:02:04.000000 pysalesforceutils-1.0.9/setup.py
+drwxr-xr-x   0 gbarger    (501) staff       (20)        0 2021-04-15 18:02:37.000000 pysalesforceutils-1.0.9/pysalesforceutils.egg-info/
+-rw-r--r--   0 gbarger    (501) staff       (20)     2828 2021-04-15 18:02:37.000000 pysalesforceutils-1.0.9/pysalesforceutils.egg-info/PKG-INFO
+-rw-r--r--   0 gbarger    (501) staff       (20)      307 2021-04-15 18:02:37.000000 pysalesforceutils-1.0.9/pysalesforceutils.egg-info/SOURCES.txt
+-rw-r--r--   0 gbarger    (501) staff       (20)       22 2021-04-15 18:02:37.000000 pysalesforceutils-1.0.9/pysalesforceutils.egg-info/requires.txt
+-rw-r--r--   0 gbarger    (501) staff       (20)       29 2021-04-15 18:02:37.000000 pysalesforceutils-1.0.9/pysalesforceutils.egg-info/top_level.txt
+-rw-r--r--   0 gbarger    (501) staff       (20)        1 2021-04-15 18:02:37.000000 pysalesforceutils-1.0.9/pysalesforceutils.egg-info/dependency_links.txt
+-rw-r--r--   0 gbarger    (501) staff       (20)       38 2021-04-15 18:02:37.000000 pysalesforceutils-1.0.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pysalesforceutils-1.0.8/PKG-INFO` & `pysalesforceutils-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysalesforceutils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python module to wrap the Salesforce APIs
 Home-page: https://github.com/gbarger/PySalesforce
 Author: Glen Barger
 Author-email: gbarger@gmail.com
 License: UNKNOWN
 Description: # PySalesforce
         **************
```

### Comparing `pysalesforceutils-1.0.8/README.md` & `pysalesforceutils-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pysalesforceutils-1.0.8/pysalesforceutils.egg-info/PKG-INFO` & `pysalesforceutils-1.0.9/pysalesforceutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysalesforceutils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python module to wrap the Salesforce APIs
 Home-page: https://github.com/gbarger/PySalesforce
 Author: Glen Barger
 Author-email: gbarger@gmail.com
 License: UNKNOWN
 Description: # PySalesforce
         **************
```

### Comparing `pysalesforceutils-1.0.8/pysalesforceutils.py` & `pysalesforceutils-1.0.9/pysalesforceutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -853,14 +853,49 @@
             response_text = "Update Successful"
         else:
             response_text = response.text
 
         return response_text
 
     @staticmethod
+    def get_sobject_rows(object_name, record_id_list_string, field_list_string, access_token, instance_url):
+        """
+        Provides the details requested for the specified record id list. In practice, if you
+        provide an explicit list of fields, it will be just like a query for that
+        record, but if you leave the fields blank, this will return a lot if not
+        all fields. I'm not sure about that because the description of what is
+        returned if you leave the fields empty isn't explained in the API documentation
+
+        Args:
+            object_name (str): The API name of the object.
+            record_id_list_string (str): The record id list you're trying to retrieve
+            field_list_string (str): List of comma separated values for fields
+                                     to retrieve
+            access_token (str): This is the access_token value received from the
+                                login response
+            instance_url (str): This is the instance_url value received from the
+                                login response
+
+        Returns:
+            dict: returns the record with the explicit field list, or all (or
+                a lot) of the fields if the field_list_string is None.
+        """
+
+        get_row_uri = '/composite/sobjects/' + object_name
+        header_details = Util.get_standard_header(access_token)
+
+        get_rows_uri = get_row_uri + '?ids=' + record_id_list_string + '&fields=' + field_list_string
+
+        response = webservice.Tools.get_http_response(
+            instance_url + Standard.base_standard_uri + 'v' + API_VERSION + get_rows_uri, header_details)
+        json_response = json.loads(response.text)
+
+        return json_response
+
+    @staticmethod
     def create_sobject_rows(records, all_or_none, run_assignment_rules, access_token, instance_url):
         """
         Creates a list of up to 200 records.
         documentation: https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/resources_composite_sobjects_collections.htm
 
         Args:
             records_json (object): The JSON describing the records you want to
@@ -1371,58 +1406,58 @@
         json_response = json.loads(response.text)
 
         return json_response
 
     @staticmethod
     def get_updated(object_name, start_date_time, end_date_time, access_token, instance_url):
         """
-        Retrieves the list of individual records that have been updated (added 
-        or changed) within the given timespan for the specified object. SObject 
+        Retrieves the list of individual records that have been updated (added
+        or changed) within the given timespan for the specified object. SObject
         Get Updated is available in API version 29.0 and later.
 
-        This resource is commonly used in data replication applications. Note 
+        This resource is commonly used in data replication applications. Note
         the following considerations:
-            * Results are returned for no more than 30 days previous to the day 
+            * Results are returned for no more than 30 days previous to the day
               the call is executed.
-            * Your client application can replicate any objects to which it has 
-              sufficient permissions. For example, to replicate all data for 
-              your organization, your client application must be logged in with 
-              “View All Data” access rights to the specified object. Similarly, 
+            * Your client application can replicate any objects to which it has
+              sufficient permissions. For example, to replicate all data for
+              your organization, your client application must be logged in with
+              “View All Data” access rights to the specified object. Similarly,
               the objects must be within your sharing rules.
-            * There is a limit of 600,000 IDs returned from this resource. If 
-              more than 600,000 IDs would be returned, EXCEEDED_ID_LIMIT is 
-              returned. You can correct the error by choosing start and end 
+            * There is a limit of 600,000 IDs returned from this resource. If
+              more than 600,000 IDs would be returned, EXCEEDED_ID_LIMIT is
+              returned. You can correct the error by choosing start and end
               dates that are closer together.
 
         Args:
             object_name (str): The name of the object to get updated records for.
 
-            startDateTime (datetime): Starting date/time (Coordinated Universal 
-                Time (UTC) time zone—not local— timezone) of the timespan for 
-                which to retrieve the data. The API ignores the seconds portion 
-                of the specified dateTime value (for example, 12:30:15 is 
+            startDateTime (datetime): Starting date/time (Coordinated Universal
+                Time (UTC) time zone—not local— timezone) of the timespan for
+                which to retrieve the data. The API ignores the seconds portion
+                of the specified dateTime value (for example, 12:30:15 is
                 interpreted as 12:30:00 UTC).
 
-            start_date_time (datetime): Ending date/time (Coordinated Universal 
-                Time (UTC) time zone—not local— timezone) of the timespan for 
-                which to retrieve the data. The API ignores the seconds portion 
-                of the specified dateTime value (for example, 12:35:15 is 
+            start_date_time (datetime): Ending date/time (Coordinated Universal
+                Time (UTC) time zone—not local— timezone) of the timespan for
+                which to retrieve the data. The API ignores the seconds portion
+                of the specified dateTime value (for example, 12:35:15 is
                 interpreted as 12:35:00 UTC).
 
             access_token (str): This is the access_token value received from the
                                 login response
 
             instance_url (str): This is the instance_url value received from the
                                 login response
 
         Returns:
-            dict: Returns a dictionary containing the record Ids that were 
+            dict: Returns a dictionary containing the record Ids that were
                 updated and the latest record updated in that window.
                 {
-                    'ids': ['<id 1>', ..., '<id N>'], 
+                    'ids': ['<id 1>', ..., '<id N>'],
                     'latestDateCovered': '2020-03-13T12:00:00.000+0000'
                 }
         """
         get_updated_uri = '/sobjects/' + object_name + '/updated/?start=' + \
             urllib.parse.quote(start_date_time.strftime('%Y-%m-%dT%H:%M:%SZ')) + '&end=' + \
             urllib.parse.quote(end_date_time.strftime('%Y-%m-%dT%H:%M:%SZ'))
 
@@ -1502,69 +1537,69 @@
         json_response = json.loads(response.text)
 
         return json_response
 
     @staticmethod
     def get_deleted(object_name, start_date_time, end_date_time, access_token, instance_url):
         """
-        Retrieves the list of individual records that have been deleted within 
-        the given timespan for the specified object. SObject Get Deleted is 
+        Retrieves the list of individual records that have been deleted within
+        the given timespan for the specified object. SObject Get Deleted is
         available in API version 29.0 and later.
 
-        This resource is commonly used in data replication applications. Note 
+        This resource is commonly used in data replication applications. Note
         the following considerations:
-            * Results are returned for no more than 30 days previous to the day 
+            * Results are returned for no more than 30 days previous to the day
               the call is executed.
-            * Your client application can replicate any objects to which it has 
-              sufficient permissions. For example, to replicate all data for 
-              your organization, your client application must be logged in with 
-              “View All Data” access rights to the specified object. Similarly, 
+            * Your client application can replicate any objects to which it has
+              sufficient permissions. For example, to replicate all data for
+              your organization, your client application must be logged in with
+              “View All Data” access rights to the specified object. Similarly,
               the objects must be within your sharing rules.
-            * There is a limit of 600,000 IDs returned from this resource. If 
-              more than 600,000 IDs would be returned, EXCEEDED_ID_LIMIT is 
-              returned. You can correct the error by choosing start and end 
+            * There is a limit of 600,000 IDs returned from this resource. If
+              more than 600,000 IDs would be returned, EXCEEDED_ID_LIMIT is
+              returned. You can correct the error by choosing start and end
               dates that are closer together.
 
         Args:
             object_name (str): The name of the object to get deleted records for.
 
-            startDateTime (datetime): Starting date/time (Coordinated Universal 
-                Time (UTC) time zone—not local— timezone) of the timespan for 
-                which to retrieve the data. The API ignores the seconds portion 
-                of the specified dateTime value (for example, 12:30:15 is 
+            startDateTime (datetime): Starting date/time (Coordinated Universal
+                Time (UTC) time zone—not local— timezone) of the timespan for
+                which to retrieve the data. The API ignores the seconds portion
+                of the specified dateTime value (for example, 12:30:15 is
                 interpreted as 12:30:00 UTC).
 
-            start_date_time (datetime): Ending date/time (Coordinated Universal 
-                Time (UTC) time zone—not local— timezone) of the timespan for 
-                which to retrieve the data. The API ignores the seconds portion 
-                of the specified dateTime value (for example, 12:35:15 is 
+            start_date_time (datetime): Ending date/time (Coordinated Universal
+                Time (UTC) time zone—not local— timezone) of the timespan for
+                which to retrieve the data. The API ignores the seconds portion
+                of the specified dateTime value (for example, 12:35:15 is
                 interpreted as 12:35:00 UTC).
 
             access_token (str): This is the access_token value received from the
                                 login response
 
             instance_url (str): This is the instance_url value received from the
                                 login response
 
         Returns:
-            dict: Returns a dictionary containing the record Ids that were 
+            dict: Returns a dictionary containing the record Ids that were
                 deleted and the latest record deleted in that window.
                 {
-                    'ids': ['<id 1>', ..., '<id N>'], 
+                    'ids': ['<id 1>', ..., '<id N>'],
                     'latestDateCovered': '2020-03-13T12:00:00.000+0000'
                 }
         """
         get_deleted_uri = '/sobjects/' + object_name + '/deleted/?start=' + \
             urllib.parse.quote(start_date_time.strftime('%Y-%m-%dT%H:%M:%SZ')) + '&end=' + \
             urllib.parse.quote(end_date_time.strftime('%Y-%m-%dT%H:%M:%SZ'))
 
         header_details = Util.get_standard_header(access_token)
 
         response = webservice.Tools.get_http_response(
-            instance_url + Standard.base_standard_uri + 'v' + API_VERSION + get_deleted_uri, 
+            instance_url + Standard.base_standard_uri + 'v' + API_VERSION + get_deleted_uri,
             header_details)
         json_response = json.loads(response.text)
 
         return json_response
 
     @staticmethod
     def graph_composite_request(request_body, access_token, instance_url):
@@ -1675,15 +1710,15 @@
 
             access_token (str): This is the access_token value received from the
                 login response
 
             instance_url (str): This is the instance_url value received from the
                 login response
         Returns:
-            dict: Returns a dictionary with the metadata description of the 
+            dict: Returns a dictionary with the metadata description of the
                 given object.
         """
         describe_uri = "/sobjects/{}/describe/".format(object_name)
 
         header_details = Util.get_standard_header(access_token)
 
         if modified_since_date:
```

### Comparing `pysalesforceutils-1.0.8/setup.py` & `pysalesforceutils-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pysalesforceutils',
-    version='1.0.8',
+    version='1.0.9',
     author='Glen Barger',
     author_email='gbarger@gmail.com',
     description='Python module to wrap the Salesforce APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/gbarger/PySalesforce',
     py_modules=[
```

### Comparing `pysalesforceutils-1.0.8/webservice.py` & `pysalesforceutils-1.0.9/webservice.py`

 * *Files identical despite different names*

