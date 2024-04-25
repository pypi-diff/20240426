# Comparing `tmp/omnivoreql-0.2.1-py3-none-any.whl.zip` & `tmp/omnivoreql-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 14962 bytes, number of entries: 8
--rw-r--r--  2.0 unx       35 b- defN 23-Jul-09 09:11 omnivoreql/__init__.py
--rw-r--r--  2.0 unx    11988 b- defN 23-Jul-09 09:11 omnivoreql/omnivoreql.py
--rw-r--r--  2.0 unx    53876 b- defN 23-Jul-09 09:11 omnivoreql/schema.gql
--rw-r--r--  2.0 unx     1065 b- defN 23-Jul-09 09:11 omnivoreql-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2302 b- defN 23-Jul-09 09:11 omnivoreql-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 09:11 omnivoreql-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-09 09:11 omnivoreql-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      639 b- defN 23-Jul-09 09:11 omnivoreql-0.2.1.dist-info/RECORD
-8 files, 70008 bytes uncompressed, 13850 bytes compressed:  80.2%
+Zip file size: 15355 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       35 b- defN 24-Apr-25 23:57 omnivoreql/__init__.py
+-rw-r--r--  2.0 unx    14051 b- defN 24-Apr-25 23:57 omnivoreql/omnivoreql.py
+-rw-r--r--  2.0 unx    53876 b- defN 24-Apr-25 23:57 omnivoreql/schema.gql
+-rw-r--r--  2.0 unx     1065 b- defN 24-Apr-25 23:57 omnivoreql-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2298 b- defN 24-Apr-25 23:57 omnivoreql-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 23:57 omnivoreql-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-25 23:57 omnivoreql-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      639 b- defN 24-Apr-25 23:57 omnivoreql-0.2.2.dist-info/RECORD
+8 files, 72067 bytes uncompressed, 14243 bytes compressed:  80.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: omnivoreql/omnivoreql.py
 Comment: 
 
 Filename: omnivoreql/schema.gql
 Comment: 
 
-Filename: omnivoreql-0.2.1.dist-info/LICENSE
+Filename: omnivoreql-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: omnivoreql-0.2.1.dist-info/METADATA
+Filename: omnivoreql-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: omnivoreql-0.2.1.dist-info/WHEEL
+Filename: omnivoreql-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: omnivoreql-0.2.1.dist-info/top_level.txt
+Filename: omnivoreql-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: omnivoreql-0.2.1.dist-info/RECORD
+Filename: omnivoreql-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omnivoreql/omnivoreql.py

```diff
@@ -1,30 +1,34 @@
 from gql import gql, Client
 from gql.transport.requests import RequestsHTTPTransport
 import uuid
 
 
 class OmnivoreQL:
-    def __init__(self, api_token: str, graphqlEndpointUrl: str = "https://api-prod.omnivore.app/api/graphql") -> None:
+    def __init__(self, api_token: str, graphql_endpoint_url: str = "https://api-prod.omnivore.app/api/graphql") -> None:
         """
         Initialize a new instance of the GraphQL client.
 
-        :param url: The URL of the Omnivore GraphQL endpoint.
         :param api_token: The API token to use for authentication.
+        :param graphql_endpoint_url: The URL of the Omnivore GraphQL endpoint.
         """
-        transport = RequestsHTTPTransport(url=graphqlEndpointUrl,
-                                          headers={
-                                              "content-type": "application/json",
-                                              "authorization": api_token
-                                          },
-                                          use_json=True)
+        transport = RequestsHTTPTransport(
+            url=graphql_endpoint_url,
+            headers={"content-type": "application/json", "authorization": api_token},
+            use_json=True,
+        )
         self.client = Client(transport=transport,
                              fetch_schema_from_transport=False)
 
     def save_url(self, url: str):
+        """
+        Save a URL to Omnivore.
+
+        :param url: The URL to save.
+        """
         mutation = gql(
             """
             mutation {
                 saveUrl(input: { clientRequestId: "%s", source: "api", url: "%s" }) {
                     ... on SaveSuccess {
                         url
                         clientRequestId
@@ -36,15 +40,44 @@
                 }
             }
         """
             % (uuid.uuid4(), url)
         )
         return self.client.execute(mutation)
 
+    def save_page(self, url: str, original_content: str):
+        """
+        Save a page with html content to Omnivore.
+
+        :param url: The URL of the page to save.
+        :param original_content: The original html content of the page.
+        """
+        mutation = gql(
+            """
+            mutation {
+                savePage(input: { clientRequestId: "%s", source: "api", url: "%s", originalContent:"%s" }) {
+                    ... on SaveSuccess {
+                        url
+                        clientRequestId
+                    }
+                    ... on SaveError {
+                        errorCodes
+                        message
+                    }
+                }
+            }
+        """
+            % (uuid.uuid4(), url, original_content)
+        )
+        return self.client.execute(mutation)
+
     def get_profile(self):
+        """
+        Get the profile of the current user.
+        """
         query = gql(
             """
             query Viewer {
             me {
                 id
                 name
                 isFullUser
@@ -57,14 +90,17 @@
             }
             }
         """
         )
         return self.client.execute(query)
 
     def get_labels(self):
+        """
+        Get the labels of the current user.
+        """
         query = gql(
             """
             query GetLabels { 
                 labels {
                     ... on LabelsSuccess {
                     labels {
                         ...LabelFields
@@ -82,14 +118,17 @@
                 description
                 createdAt
             }"""
         )
         return self.client.execute(query)
 
     def get_subscriptions(self):
+        """
+        Get the subscriptions of the current user.
+        """
         query = gql(
             """
                 query GetSubscriptions {
                 subscriptions(sort: { by: UPDATED_TIME }) {
                     ... on SubscriptionsSuccess {
                     subscriptions {
                         id
@@ -110,14 +149,23 @@
                 }
                 }
             """
         )
         return self.client.execute(query)
 
     def get_articles(self, limit: int = None, cursor: str = None, format: str = 'markdown', query: str = "in:inbox", include_content: bool = False):
+        """
+        Get articles for the current user.
+
+        :param limit: The number of articles to return.
+        :param cursor: The cursor to use for pagination.
+        :param format: The format of the articles to return.
+        :param query: The query to use for filtering articles. Example of query by date: 'in:inbox published:2024-03-01..*'. See https://docs.omnivore.app/using/search.html#filtering-by-save-publish-dates for more information.
+        :param include_content: Whether to include the content of the articles.
+        """
         q = gql(
             """
             query Search($after: String, $first: Int, $query: String, $format: String, $includeContent: Boolean) {
                 search(after: $after, first: $first, query: $query, format: $format, includeContent: $includeContent) {
                     ... on SearchSuccess {
                         edges {
                             cursor
@@ -211,15 +259,22 @@
         """
         )
         return self.client.execute(
             q, variable_values={
                 "first": limit, "after": cursor, "query": query, "format": format, "includeContent": include_content}
         )
 
-    def get_article(self, username: str, slug: str, format: str = None, include_friends_highlights: bool = False):
+    def get_article(self, username: str, slug: str, format: str = None):
+        """
+        Get an article by username and slug.
+
+        :param username: Omnivore username.
+        :param slug: The slug of the article.
+        :param format: The format of the article to return.
+        """
         query = gql(
             """
             query GetArticle($username: String!, $slug: String!, $format: String, $includeFriendsHighlights: Boolean) {
                 article(username: $username, slug: $slug, format: $format) {
                     ... on ArticleSuccess {
                         article {
                             ...ArticleFields
@@ -313,15 +368,21 @@
             variable_values={
                 "username": username,
                 "slug": slug,
                 "format": format,
             },
         )
 
-    def archive_article(self, article_id: str, toArchive: bool = True):
+    def archive_article(self, article_id: str, to_archive: bool = True):
+        """
+        Archive or unarchive an article.
+
+        :param article_id: The ID of the article to archive.
+        :param to_archive: Whether to archive or unarchive the article.
+        """
         mutation = gql(
             """
         mutation SetLinkArchived($input: ArchiveLinkInput!) {
             setLinkArchived(input: $input) {
                     ... on ArchiveLinkSuccess {
                         linkId
                         message
@@ -331,26 +392,31 @@
                         message
                     }
                 }
             }
         """)
         return self.client.execute(
             mutation,
-            variable_values={
-                "input": {
-                    "linkId": article_id,
-                    "archived": toArchive
-                }
-            }
+            variable_values={"input": {"linkId": article_id, "archived": to_archive}},
         )
 
     def unarchive_article(self, article_id: str):
+        """
+        Unarchive an article.
+
+        :param article_id: The ID of the article to unarchive.
+        """
         return self.archive_article(article_id, False)
 
     def delete_article(self, article_id: str):
+        """
+        Delete an article.
+
+        :param article_id: The ID of the article to delete.
+        """
         mutation = gql("""
             mutation SetBookmarkArticle($input: SetBookmarkArticleInput!) {
                 setBookmarkArticle(input: $input) {
                     ... on SetBookmarkArticleSuccess {
                         bookmarkedArticle {
                             id
                         }
```

## Comparing `omnivoreql-0.2.1.dist-info/LICENSE` & `omnivoreql-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `omnivoreql-0.2.1.dist-info/METADATA` & `omnivoreql-0.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.2.1
+Version: 0.2.2
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreQL/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreQL
@@ -13,16 +13,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gql (==3.4.1)
-Requires-Dist: requests-toolbelt (==1.0.0)
+Requires-Dist: gql ==3.4.1
+Requires-Dist: requests-toolbelt ==1.0.0
 
 # OmnivoreQL: Omnivore API client for Python
 
 This is a Python client for the [Omnivore API](https://omnivore.app).
 
 [![GitHub stars](https://img.shields.io/github/stars/yazdipour/omnivoreql.svg?style=social&label=Star)](https://github.com/yazdipour/omnivoreql/stargazers)
 [![Github Sponsor](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/yazdipour)
```

## Comparing `omnivoreql-0.2.1.dist-info/RECORD` & `omnivoreql-0.2.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 omnivoreql/__init__.py,sha256=dBGv0U-yx7ZToJUTQQ03Pf77pabVg1CkEKICawL7NH4,35
-omnivoreql/omnivoreql.py,sha256=Iji-NbChzLsVwu2HxhJfkq80Q8RBkta3BNNqw4B12yw,11988
+omnivoreql/omnivoreql.py,sha256=JZ2SKCydA3lrcscdARaxrxoEzTheGWmn-nJW1DxGdRk,14051
 omnivoreql/schema.gql,sha256=3O4dCsGQr79ueltDx3P6QNkr8K8FxlXcALffmlPCdc8,53876
-omnivoreql-0.2.1.dist-info/LICENSE,sha256=pPWe8Gord61PmdyBbCLoqBmbWncoKFFd_6k4qpQ4Tvw,1065
-omnivoreql-0.2.1.dist-info/METADATA,sha256=osPk-_-8OpW3GJKuunyAs9R6dJRb5cejQd4GpTc0rQE,2302
-omnivoreql-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-omnivoreql-0.2.1.dist-info/top_level.txt,sha256=U5IklQ1RU3J7NFK8peOJtY4FLDokJd8W_F5Gk888WJo,11
-omnivoreql-0.2.1.dist-info/RECORD,,
+omnivoreql-0.2.2.dist-info/LICENSE,sha256=pPWe8Gord61PmdyBbCLoqBmbWncoKFFd_6k4qpQ4Tvw,1065
+omnivoreql-0.2.2.dist-info/METADATA,sha256=ovPr60Rtr1eFOIB5M5XfqkYMwwjcCjr9bjvf0ZHELW0,2298
+omnivoreql-0.2.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+omnivoreql-0.2.2.dist-info/top_level.txt,sha256=U5IklQ1RU3J7NFK8peOJtY4FLDokJd8W_F5Gk888WJo,11
+omnivoreql-0.2.2.dist-info/RECORD,,
```

