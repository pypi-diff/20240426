# Comparing `tmp/embtechx-1.0.5.tar.gz` & `tmp/embtechx-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embtechx-1.0.5.tar", last modified: Tue Apr 23 09:47:34 2024, max compression
+gzip compressed data, was "embtechx-1.0.6.tar", last modified: Fri Apr 26 09:11:06 2024, max compression
```

## Comparing `embtechx-1.0.5.tar` & `embtechx-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-23 09:47:34.848403 embtechx-1.0.5/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-23 09:47:34.847583 embtechx-1.0.5/PKG-INFO
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-23 09:47:34.837452 embtechx-1.0.5/embtechx/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      861 2024-04-23 09:46:37.000000 embtechx-1.0.5/embtechx/__init__.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     3126 2024-04-23 09:46:43.000000 embtechx-1.0.5/embtechx/dataframe.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     2441 2024-04-23 09:46:56.000000 embtechx-1.0.5/embtechx/domain_emb.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     7086 2024-04-23 09:47:07.000000 embtechx-1.0.5/embtechx/embedding.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     8300 2024-04-23 09:46:58.000000 embtechx-1.0.5/embtechx/evaluate.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     1672 2024-04-23 09:47:01.000000 embtechx-1.0.5/embtechx/search.py
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-23 09:47:34.847019 embtechx-1.0.5/embtechx.egg-info/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-23 09:47:34.000000 embtechx-1.0.5/embtechx.egg-info/PKG-INFO
--rw-r--r--   0 ninananakorn   (501) staff       (20)      295 2024-04-23 09:47:34.000000 embtechx-1.0.5/embtechx.egg-info/SOURCES.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-04-23 09:47:34.000000 embtechx-1.0.5/embtechx.egg-info/dependency_links.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       86 2024-04-23 09:47:34.000000 embtechx-1.0.5/embtechx.egg-info/requires.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)        9 2024-04-23 09:47:34.000000 embtechx-1.0.5/embtechx.egg-info/top_level.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-04-23 09:47:34.848507 embtechx-1.0.5/setup.cfg
--rw-r--r--   0 ninananakorn   (501) staff       (20)      364 2024-04-23 09:46:39.000000 embtechx-1.0.5/setup.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-26 09:11:06.220324 embtechx-1.0.6/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-26 09:11:06.219388 embtechx-1.0.6/PKG-INFO
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-26 09:11:06.212107 embtechx-1.0.6/embtechx/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      860 2024-04-26 09:10:00.000000 embtechx-1.0.6/embtechx/__init__.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     3126 2024-04-26 09:10:05.000000 embtechx-1.0.6/embtechx/dataframe.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     2445 2024-04-26 09:10:07.000000 embtechx-1.0.6/embtechx/domain_emb.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     7381 2024-04-26 09:10:50.000000 embtechx-1.0.6/embtechx/embedding.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     8300 2024-04-26 09:10:40.000000 embtechx-1.0.6/embtechx/evaluate.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     2184 2024-04-26 09:10:46.000000 embtechx-1.0.6/embtechx/search.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-26 09:11:06.218671 embtechx-1.0.6/embtechx.egg-info/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-26 09:11:06.000000 embtechx-1.0.6/embtechx.egg-info/PKG-INFO
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      295 2024-04-26 09:11:06.000000 embtechx-1.0.6/embtechx.egg-info/SOURCES.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-04-26 09:11:06.000000 embtechx-1.0.6/embtechx.egg-info/dependency_links.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       86 2024-04-26 09:11:06.000000 embtechx-1.0.6/embtechx.egg-info/requires.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)        9 2024-04-26 09:11:06.000000 embtechx-1.0.6/embtechx.egg-info/top_level.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-04-26 09:11:06.220415 embtechx-1.0.6/setup.cfg
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      364 2024-04-26 09:10:02.000000 embtechx-1.0.6/setup.py
```

### Comparing `embtechx-1.0.5/embtechx/__init__.py` & `embtechx-1.0.6/embtechx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 concat_df = emb_dataframe.concat_df
 
 from .embedding import emb_train
 embedding = emb_train.sentence_embedding
 create_test_train = emb_train.create_test_train
 train_model = emb_train.train_model
 train_model_customize = emb_train.train_model_customize
-
 train_model_only = emb_train.train_model_only
 train_model_only_customize = emb_train.train_model_only_customize
 
 from .evaluate import eval_model
 evaluate = eval_model.evaluate
 evaluate_svm = eval_model.accuracy_svm
 evaluate_knn = eval_model.accuracy_knn
```

### Comparing `embtechx-1.0.5/embtechx/dataframe.py` & `embtechx-1.0.6/embtechx/dataframe.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.5/embtechx/domain_emb.py` & `embtechx-1.0.6/embtechx/domain_emb.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 evaluate_knn = eval_model.accuracy_knn
 evaluate_naive_bayes = eval_model.accuracy_naive_bayes
 evaluate_pca = eval_model.evaluate_pca
 evaluate_tsne = eval_model.evaluate_tsne
 
 def domain_emb():
     domain_path = input("Enter the file path for a domain dataframe: ")
-    domain_name = input("Enter a name of the domain: ")
+    domain_name = input("Enter the name of the domain: ")
     domain_dataframe = create_df(domain_name, domain_path)
     misc_path = input("Enter the file path for a miscellaneous dataframe: ")
     domain_misc = create_misc(misc_path)
 
     test, train, file_path = train_model(domain_dataframe, domain_misc)
     file_path_before = file_path + "/before"
     file_path_after = file_path + "/after"
@@ -39,15 +39,15 @@
     print("After the training")
     evaluate(test_df_after, train_df)
     evaluate_pca(test_df_after)
     evaluate_tsne(test_df_after)
 
 def domain_emb_customize():
     domain_path = input("Enter the file path for a domain dataframe: ")
-    domain_name = input("Enter a name of the domain: ")
+    domain_name = input("Enter the name of the domain: ")
     domain_dataframe = create_df(domain_name, domain_path)
     misc_path = input("Enter the file path for a miscellaneous dataframe: ")
     domain_misc = create_misc(misc_path)
 
     test, train, file_path = train_model_customize(domain_dataframe, domain_misc)
     file_path_before = file_path + "/before"
     file_path_after = file_path + "/after"
```

### Comparing `embtechx-1.0.5/embtechx/embedding.py` & `embtechx-1.0.6/embtechx/embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from sentence_transformers import SentenceTransformer, InputExample, losses
+from sentence_transformers.evaluation import TripletEvaluator
 from torch.utils.data import DataLoader
 
 import time
 import pandas as pd
 from langdetect import *
 
 from .dataframe import emb_dataframe
@@ -100,17 +101,19 @@
         num_epochs = 30
         eval_steps = 100
         warmup_steps_n = int(len(triplet_df) * num_epochs * 0.1)
 
         train_dataloader = DataLoader(train_examples, shuffle=True, batch_size=train_batch_size)
         train_loss = losses.TripletLoss(model=model)
 
+        triplet_evaluator = TripletEvaluator.from_input_examples(train_examples)
+
         start_time = time.time()
 
-        model.fit(train_objectives=[(train_dataloader, train_loss)], epochs=num_epochs, \
+        model.fit(train_objectives=[(train_dataloader, train_loss)], evaluator=triplet_evaluator, epochs=num_epochs, \
                 evaluation_steps=eval_steps, warmup_steps=warmup_steps_n, \
                 callback=lambda score, epoch, steps: print(f"Score: {score}, Epoch: {epoch}, Step: {steps}"))
 
         model.save(file_path_after)
         
         time_taken = time.time()-start_time
         print()
@@ -118,15 +121,15 @@
             time_taken_hr = time_taken/3600
             print("Time taken:", round(time_taken_hr, 5), "hours")
         else:
             time_taken_min = time_taken/60
             print("Time taken:", round(time_taken_min, 5), "minutes")
 
     def train_model_only_customize(dataframe, file_path):
-        model_id = input("Enter the model’s name or a file path of the model you want to train: ")
+        model_id = input("Enter the model's name or a file path of the model you want to train: ")
         model = SentenceTransformer(model_id)
 
         file_path_before = file_path + "/before"
         file_path_after = file_path + "/after"
 
         model.save(file_path_before)
 
@@ -145,26 +148,28 @@
 
         triplet_df = pd.DataFrame(triplet_dict)
         
         train_examples = []
         for i in range(len(triplet_df)):
             train_examples.append(InputExample(texts = triplet_df.iloc[i].tolist()))
         
-        train_batch_size = int(input("Enter a batch size: "))
-        num_epochs = int(input("Enter an epoch size: "))
+        train_batch_size = int(input("Enter the batch size: "))
+        num_epochs = int(input("Enter the epoch number: "))
 
         eval_steps = 100
         warmup_steps_n = int(len(dataframe) * num_epochs * 0.1)
 
         train_dataloader = DataLoader(train_examples, shuffle=True, batch_size=train_batch_size)
         train_loss = losses.TripletLoss(model=model)
+        
+        triplet_evaluator = TripletEvaluator.from_input_examples(train_examples)
 
         start_time = time.time()
 
-        model.fit(train_objectives=[(train_dataloader, train_loss)], epochs=num_epochs, \
+        model.fit(train_objectives=[(train_dataloader, train_loss)], evaluator=triplet_evaluator, epochs=num_epochs, \
                 evaluation_steps=eval_steps, warmup_steps=warmup_steps_n, \
                 callback=lambda score, epoch, steps: print(f"Score: {score}, Epoch: {epoch}, Step: {steps}"))
 
         model.save(file_path_after)
         
         time_taken = time.time()-start_time
         print()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `embtechx-1.0.5/embtechx/evaluate.py` & `embtechx-1.0.6/embtechx/evaluate.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.5/embtechx/search.py` & `embtechx-1.0.6/embtechx/search.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,44 +3,50 @@
 
 from sklearn.neighbors import NearestNeighbors
 
 from .embedding import emb_train
 sentence_embedding = emb_train.sentence_embedding
 
 def find_related_sentences(dataframe, model_path):
-    model = SentenceTransformer(model_path)
+    embedding_model_path = model_path
+    model = SentenceTransformer(embedding_model_path)
 
     sentence = input("Enter a keyword: ")
     vector = model.encode(sentence)
     
     if "Embedding vector" not in dataframe.columns:           
         dataframe_v = dataframe.copy()
         dataframe_v = sentence_embedding(dataframe_v, model_path)
         embedding_vector = dataframe_v["Embedding vector"].tolist()
     else:
         dataframe_v = dataframe.copy()
         embedding_vector = dataframe_v["Embedding vector"].tolist()
     
-    knn_model = NearestNeighbors(n_neighbors=len(dataframe_v))
-    knn_model.fit(embedding_vector)
+    nn_model = NearestNeighbors(n_neighbors=len(dataframe_v))
+    nn_model.fit(embedding_vector)
 
-    distances, indices = knn_model.kneighbors([vector])
+    distances, indices = nn_model.kneighbors([vector])
 
     result = dataframe_v.iloc[indices[0]].copy()
     result["Distance"] = distances[0]
 
     result_df = result.loc[:, ["Text", "Domain", "Embedding vector", "Distance"]]
     result_df = result_df[result_df["Distance"] <= 1]
 
-    display(result_df)
-
     if len(result_df) == 0:
+        print("Sorry, there are no sentences related to the searched keyword.")
         exit()
     else: 
+        display(result_df)
         print()
         cont_or_no = input("Would you like to add more keywords? (yes/no): ")
         if cont_or_no == "y" or cont_or_no == "Y" or cont_or_no == "yes" or cont_or_no == "Yes" or cont_or_no == "YES":
-            find_related_sentences(result_df, model_path)
+            find_related_sentences(result_df, embedding_model_path)
         elif cont_or_no == "n" or cont_or_no == "N" or cont_or_no == "no" or cont_or_no == "No" or cont_or_no == "NO":
-            return result_df
+            save_df = input("Would you like to save the dataframe? (yes/no): ")
+            if save_df == "y" or save_df == "Y" or save_df == "yes" or save_df == "Yes" or save_df == "YES":
+                csv_path = input("Please enter the file path for saving the dataframe: ")
+                result_df.to_csv(csv_path + "/related_sentences.csv", index=False)
+            else:
+                exit()
         else:
             exit()
```

