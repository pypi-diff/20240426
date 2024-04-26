# Comparing `tmp/rule-based-retrieval-0.1.3.tar.gz` & `tmp/rule_based_retrieval-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rule-based-retrieval-0.1.3.tar", last modified: Tue Mar 26 00:13:14 2024, max compression
+gzip compressed data, was "rule_based_retrieval-0.1.4.tar", last modified: Fri Apr 26 05:14:53 2024, max compression
```

## Comparing `rule-based-retrieval-0.1.3.tar` & `rule_based_retrieval-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-03-26 00:13:14.827524 rule-based-retrieval-0.1.3/
--rw-rw-r--   0 tomsmoker   (501) staff       (20)     1065 2024-03-22 03:36:34.000000 rule-based-retrieval-0.1.3/LICENCE.md
--rw-r--r--   0 tomsmoker   (501) staff       (20)     7343 2024-03-26 00:13:14.827355 rule-based-retrieval-0.1.3/PKG-INFO
--rw-rw-r--   0 tomsmoker   (501) staff       (20)     5914 2024-03-26 00:05:39.000000 rule-based-retrieval-0.1.3/README.md
--rw-rw-r--   0 tomsmoker   (501) staff       (20)     2235 2024-03-22 03:36:34.000000 rule-based-retrieval-0.1.3/pyproject.toml
--rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-03-26 00:13:14.827568 rule-based-retrieval-0.1.3/setup.cfg
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-03-26 00:13:14.822249 rule-based-retrieval-0.1.3/src/
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-03-26 00:13:14.826615 rule-based-retrieval-0.1.3/src/rule_based_retrieval.egg-info/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     7343 2024-03-26 00:13:14.000000 rule-based-retrieval-0.1.3/src/rule_based_retrieval.egg-info/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)      543 2024-03-26 00:13:14.000000 rule-based-retrieval-0.1.3/src/rule_based_retrieval.egg-info/SOURCES.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-26 00:13:14.000000 rule-based-retrieval-0.1.3/src/rule_based_retrieval.egg-info/dependency_links.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-26 00:13:14.000000 rule-based-retrieval-0.1.3/src/rule_based_retrieval.egg-info/not-zip-safe
--rw-r--r--   0 tomsmoker   (501) staff       (20)      302 2024-03-26 00:13:14.000000 rule-based-retrieval-0.1.3/src/rule_based_retrieval.egg-info/requires.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)       11 2024-03-26 00:13:14.000000 rule-based-retrieval-0.1.3/src/rule_based_retrieval.egg-info/top_level.txt
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-03-26 00:13:14.824854 rule-based-retrieval-0.1.3/src/whyhow_rbr/
--rw-rw-r--   0 tomsmoker   (501) staff       (20)      280 2024-03-22 03:36:34.000000 rule-based-retrieval-0.1.3/src/whyhow_rbr/__init__.py
--rw-rw-r--   0 tomsmoker   (501) staff       (20)      814 2024-03-22 03:36:34.000000 rule-based-retrieval-0.1.3/src/whyhow_rbr/embedding.py
--rw-rw-r--   0 tomsmoker   (501) staff       (20)      365 2024-03-22 03:36:34.000000 rule-based-retrieval-0.1.3/src/whyhow_rbr/exceptions.py
--rw-rw-r--   0 tomsmoker   (501) staff       (20)     1944 2024-03-22 03:36:34.000000 rule-based-retrieval-0.1.3/src/whyhow_rbr/processing.py
--rw-rw-r--   0 tomsmoker   (501) staff       (20)    22695 2024-03-22 03:36:34.000000 rule-based-retrieval-0.1.3/src/whyhow_rbr/rag.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-03-26 00:13:14.826373 rule-based-retrieval-0.1.3/tests/
--rw-rw-r--   0 tomsmoker   (501) staff       (20)       28 2024-03-22 03:36:34.000000 rule-based-retrieval-0.1.3/tests/test_dummy.py
--rw-rw-r--   0 tomsmoker   (501) staff       (20)     1023 2024-03-22 03:36:34.000000 rule-based-retrieval-0.1.3/tests/test_embedding.py
--rw-rw-r--   0 tomsmoker   (501) staff       (20)     3090 2024-03-22 03:36:34.000000 rule-based-retrieval-0.1.3/tests/test_processing.py
--rw-rw-r--   0 tomsmoker   (501) staff       (20)    26054 2024-03-22 03:36:34.000000 rule-based-retrieval-0.1.3/tests/test_rag.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-26 05:14:53.745132 rule_based_retrieval-0.1.4/
+-rw-rw-r--   0 tomsmoker   (501) staff       (20)     1065 2024-03-22 03:36:34.000000 rule_based_retrieval-0.1.4/LICENCE.md
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     5015 2024-04-26 05:14:53.744920 rule_based_retrieval-0.1.4/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     3586 2024-04-26 05:06:37.000000 rule_based_retrieval-0.1.4/README.md
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     2235 2024-03-26 00:45:22.000000 rule_based_retrieval-0.1.4/pyproject.toml
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-04-26 05:14:53.745176 rule_based_retrieval-0.1.4/setup.cfg
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-26 05:14:53.738993 rule_based_retrieval-0.1.4/src/
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-26 05:14:53.743882 rule_based_retrieval-0.1.4/src/rule_based_retrieval.egg-info/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     5015 2024-04-26 05:14:53.000000 rule_based_retrieval-0.1.4/src/rule_based_retrieval.egg-info/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      572 2024-04-26 05:14:53.000000 rule_based_retrieval-0.1.4/src/rule_based_retrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-04-26 05:14:53.000000 rule_based_retrieval-0.1.4/src/rule_based_retrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-26 00:13:14.000000 rule_based_retrieval-0.1.4/src/rule_based_retrieval.egg-info/not-zip-safe
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      302 2024-04-26 05:14:53.000000 rule_based_retrieval-0.1.4/src/rule_based_retrieval.egg-info/requires.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       11 2024-04-26 05:14:53.000000 rule_based_retrieval-0.1.4/src/rule_based_retrieval.egg-info/top_level.txt
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-26 05:14:53.742189 rule_based_retrieval-0.1.4/src/whyhow_rbr/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      280 2024-04-26 05:12:02.000000 rule_based_retrieval-0.1.4/src/whyhow_rbr/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      814 2024-03-26 00:15:46.000000 rule_based_retrieval-0.1.4/src/whyhow_rbr/embedding.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1263 2024-04-26 05:06:37.000000 rule_based_retrieval-0.1.4/src/whyhow_rbr/exceptions.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1944 2024-03-26 00:41:23.000000 rule_based_retrieval-0.1.4/src/whyhow_rbr/processing.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)    22962 2024-04-26 05:06:37.000000 rule_based_retrieval-0.1.4/src/whyhow_rbr/rag.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)    28857 2024-04-26 05:06:37.000000 rule_based_retrieval-0.1.4/src/whyhow_rbr/rag_milvus.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-26 05:14:53.743388 rule_based_retrieval-0.1.4/tests/
+-rw-rw-r--   0 tomsmoker   (501) staff       (20)       28 2024-03-22 03:36:34.000000 rule_based_retrieval-0.1.4/tests/test_dummy.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1023 2024-03-26 00:15:46.000000 rule_based_retrieval-0.1.4/tests/test_embedding.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     3090 2024-03-26 00:45:22.000000 rule_based_retrieval-0.1.4/tests/test_processing.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)    26123 2024-04-26 05:06:37.000000 rule_based_retrieval-0.1.4/tests/test_rag.py
```

### Comparing `rule-based-retrieval-0.1.3/LICENCE.md` & `rule_based_retrieval-0.1.4/LICENCE.md`

 * *Files identical despite different names*

### Comparing `rule-based-retrieval-0.1.3/pyproject.toml` & `rule_based_retrieval-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rule-based-retrieval-0.1.3/src/rule_based_retrieval.egg-info/SOURCES.txt` & `rule_based_retrieval-0.1.4/src/rule_based_retrieval.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 src/rule_based_retrieval.egg-info/requires.txt
 src/rule_based_retrieval.egg-info/top_level.txt
 src/whyhow_rbr/__init__.py
 src/whyhow_rbr/embedding.py
 src/whyhow_rbr/exceptions.py
 src/whyhow_rbr/processing.py
 src/whyhow_rbr/rag.py
+src/whyhow_rbr/rag_milvus.py
 tests/test_dummy.py
 tests/test_embedding.py
 tests/test_processing.py
 tests/test_rag.py
```

### Comparing `rule-based-retrieval-0.1.3/src/whyhow_rbr/embedding.py` & `rule_based_retrieval-0.1.4/src/whyhow_rbr/embedding.py`

 * *Files identical despite different names*

### Comparing `rule-based-retrieval-0.1.3/src/whyhow_rbr/processing.py` & `rule_based_retrieval-0.1.4/src/whyhow_rbr/processing.py`

 * *Files identical despite different names*

### Comparing `rule-based-retrieval-0.1.3/src/whyhow_rbr/rag.py` & `rule_based_retrieval-0.1.4/src/whyhow_rbr/rag.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,17 @@
     @classmethod
     def convert_empty_to_none(cls, v: list[int] | None) -> list[int] | None:
         """Convert empty list to None."""
         if v is not None and not v:
             return None
         return v
 
-    def convert_empty_str_to_none(cls, s: list[str] | None) -> list[str] | None:
+    def convert_empty_str_to_none(
+        cls, s: list[str] | None
+    ) -> list[str] | None:
         """Convert empty string list to None."""
         if s is not None and not s:
             return None
         return s
 
     def to_filter(self) -> dict[str, list[dict[str, Any]]] | None:
         """Convert rule to Pinecone filter format."""
@@ -489,31 +491,28 @@
 
         response = index.upsert(
             upsert_documents, namespace=namespace, batch_size=batch_size
         )
         n_upserted = response["upserted_count"]
         logger.info(f"Upserted {n_upserted} documents")
 
-    def clean_text(
-        self,
-        text: str
-    ) -> str:
+    def clean_text(self, text: str) -> str:
         """Return a lower case version of text with punctuation removed.
 
         Parameters
         ----------
         text : str
             The raw text to be cleaned.
 
         Returns
         -------
         str: The cleaned text string.
         """
-        text_processed = re.sub('[^0-9a-zA-Z ]+', '', text.lower())
-        text_processed_further = re.sub(' +', ' ', text_processed)
+        text_processed = re.sub("[^0-9a-zA-Z ]+", "", text.lower())
+        text_processed_further = re.sub(" +", " ", text_processed)
         return text_processed_further
 
     def query(
         self,
         question: str,
         index: Index,
         namespace: str,
@@ -521,15 +520,15 @@
         top_k: int = 5,
         chat_model: str = "gpt-4-1106-preview",
         chat_temperature: float = 0.0,
         chat_max_tokens: int = 1000,
         chat_seed: int = 2,
         embedding_model: str = "text-embedding-3-small",
         process_rules_separately: bool = False,
-        keyword_trigger: bool = False
+        keyword_trigger: bool = False,
     ) -> QueryReturnType:
         """Query the index.
 
         Parameters
         ----------
         question : str
             The question to ask.
@@ -584,41 +583,45 @@
         Raises
         ------
         OpenAIException
             If there is an error with the OpenAI API. Some possible reasons
             include the chat model not finishing or the response not being
             valid JSON.
         """
-        logger.info(f'Raw rules: {rules}')
+        logger.info(f"Raw rules: {rules}")
 
         if rules is None:
             rules = []
 
         if keyword_trigger:
             triggered_rules = []
-            clean_question = self.clean_text(question).split(' ')
+            clean_question = self.clean_text(question).split(" ")
 
             for rule in rules:
                 if rule.keywords:
-                    clean_keywords = [self.clean_text(keyword) for keyword in rule.keywords]
+                    clean_keywords = [
+                        self.clean_text(keyword) for keyword in rule.keywords
+                    ]
 
                     if bool(set(clean_keywords) & set(clean_question)):
                         triggered_rules.append(rule)
 
             rules = triggered_rules
 
         rule_filters = [rule.to_filter() for rule in rules if rule is not None]
 
         question_embedding = generate_embeddings(
             openai_api_key=self.openai_client.api_key,
             chunks=[question],
             model=embedding_model,
         )[0]
 
-        matches = []  # Initialize matches outside the loop to collect matches from all queries
+        matches = (
+            []
+        )  # Initialize matches outside the loop to collect matches from all queries
         match_texts = []
 
         # Check if there are any rule filters, and if not, proceed with a default query
         if not rule_filters:
             # Perform a default query
             query_response = index.query(
                 namespace=namespace,
@@ -640,40 +643,48 @@
                         query_response = index.query(
                             namespace=namespace,
                             top_k=top_k,
                             vector=question_embedding,
                             filter=rule_filter,
                             include_metadata=True,
                         )
-                        matches.extend([
-                            PineconeMatch(**m.to_dict()) for m in query_response["matches"]
-                        ])
+                        matches.extend(
+                            [
+                                PineconeMatch(**m.to_dict())
+                                for m in query_response["matches"]
+                            ]
+                        )
                         match_texts += [m.metadata.text for m in matches]
-                match_texts = list(set(match_texts))  # Ensure unique match texts
+                match_texts = list(
+                    set(match_texts)
+                )  # Ensure unique match texts
             else:
                 if rule_filters:
                     combined_filters = []
                     for rule_filter in rule_filters:
                         if rule_filter:
                             combined_filters.append(rule_filter)
 
-                    rule_filter = {"$or": combined_filters} if combined_filters else None
+                    rule_filter = (
+                        {"$or": combined_filters} if combined_filters else None
+                    )
                 else:
                     rule_filter = None  # Fallback to a default query when no rules are provided or valid
 
                 if rule_filter is not None:
                     query_response = index.query(
                         namespace=namespace,
                         top_k=top_k,
                         vector=question_embedding,
                         filter=rule_filter,
                         include_metadata=True,
                     )
                     matches = [
-                        PineconeMatch(**m.to_dict()) for m in query_response["matches"]
+                        PineconeMatch(**m.to_dict())
+                        for m in query_response["matches"]
                     ]
                     match_texts = [m.metadata.text for m in matches]
 
         # Proceed to create prompt, send it to OpenAI, and handle the response
         prompt = self.create_prompt(question, match_texts)
         response = self.openai_client.chat.completions.create(
             model=chat_model,
```

### Comparing `rule-based-retrieval-0.1.3/tests/test_embedding.py` & `rule_based_retrieval-0.1.4/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `rule-based-retrieval-0.1.3/tests/test_processing.py` & `rule_based_retrieval-0.1.4/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `rule-based-retrieval-0.1.3/tests/test_rag.py` & `rule_based_retrieval-0.1.4/tests/test_rag.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,21 @@
 from pinecone import Index, NotFoundException, Pinecone
 
 from whyhow_rbr.exceptions import (
     IndexAlreadyExistsException,
     IndexNotFoundException,
     OpenAIException,
 )
-from whyhow_rbr.rag import Client, Output, PineconeDocument, PineconeMetadata, Rule
+from whyhow_rbr.rag import (
+    Client,
+    Output,
+    PineconeDocument,
+    PineconeMetadata,
+    Rule,
+)
 
 
 class TestRule:
     def test_default(self):
         rule = Rule()
 
         assert rule.filename is None
@@ -244,15 +250,17 @@
                 },
             ),
         ]
         fake_parse_and_split = Mock(return_value=parsed_docs)
         fake_clean_chunks = Mock(return_value=parsed_docs)
         fake_generate_embeddings = Mock(return_value=6 * [[2.2, 0.6]])
 
-        monkeypatch.setattr("whyhow_rbr.rag.parse_and_split", fake_parse_and_split)
+        monkeypatch.setattr(
+            "whyhow_rbr.rag.parse_and_split", fake_parse_and_split
+        )
         monkeypatch.setattr("whyhow_rbr.rag.clean_chunks", fake_clean_chunks)
         monkeypatch.setattr(
             "whyhow_rbr.rag.generate_embeddings", fake_generate_embeddings
         )
 
         client.upload_documents(
             index=fake_index,
@@ -305,15 +313,17 @@
                 },
             ),
         ]
         fake_parse_and_split = Mock(return_value=parsed_docs)
         fake_clean_chunks = Mock(return_value=parsed_docs)
         fake_generate_embeddings = Mock(return_value=5 * [[2.2, 0.6]])
 
-        monkeypatch.setattr("whyhow_rbr.rag.parse_and_split", fake_parse_and_split)
+        monkeypatch.setattr(
+            "whyhow_rbr.rag.parse_and_split", fake_parse_and_split
+        )
         monkeypatch.setattr("whyhow_rbr.rag.clean_chunks", fake_clean_chunks)
         monkeypatch.setattr(
             "whyhow_rbr.rag.generate_embeddings", fake_generate_embeddings
         )
 
         with pytest.raises(
             ValueError, match="Number of embeddings does not match"
```

