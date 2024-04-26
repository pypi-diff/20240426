# Comparing `tmp/text_lloom-0.7.1.tar.gz` & `tmp/text_lloom-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_lloom-0.7.1.tar", max compression
+gzip compressed data, was "text_lloom-0.7.2.tar", max compression
```

## Comparing `text_lloom-0.7.1.tar` & `text_lloom-0.7.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.7.1/README.md
--rw-r--r--   0        0        0      546 2024-04-22 09:07:17.168243 text_lloom-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.7.1/src/text_lloom/__init__.py
--rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.7.1/src/text_lloom/concept.py
--rw-r--r--   0        0        0    57605 2024-04-22 08:37:58.216130 text_lloom-0.7.1/src/text_lloom/concept_induction.py
--rw-r--r--   0        0        0     8078 2024-04-22 08:18:42.690605 text_lloom-0.7.1/src/text_lloom/llm.py
--rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.7.1/src/text_lloom/prompts.py
--rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.7.1/src/text_lloom/static/index.css
--rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.7.1/src/text_lloom/static/index.js
--rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.7.1/src/text_lloom/static/index_select.css
--rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.7.1/src/text_lloom/static/index_select.js
--rw-r--r--   0        0        0    29130 2024-04-22 07:18:08.926897 text_lloom-0.7.1/src/text_lloom/workbench.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 text_lloom-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.7.2/README.md
+-rw-r--r--   0        0        0      546 2024-04-26 11:54:39.443185 text_lloom-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.7.2/src/text_lloom/__init__.py
+-rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.7.2/src/text_lloom/concept.py
+-rw-r--r--   0        0        0    58656 2024-04-26 11:32:12.086284 text_lloom-0.7.2/src/text_lloom/concept_induction.py
+-rw-r--r--   0        0        0     8216 2024-04-26 11:49:39.075606 text_lloom-0.7.2/src/text_lloom/llm.py
+-rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.7.2/src/text_lloom/prompts.py
+-rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.7.2/src/text_lloom/static/index.css
+-rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.7.2/src/text_lloom/static/index.js
+-rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.7.2/src/text_lloom/static/index_select.css
+-rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.7.2/src/text_lloom/static/index_select.js
+-rw-r--r--   0        0        0    30201 2024-04-26 11:47:07.423672 text_lloom-0.7.2/src/text_lloom/workbench.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 text_lloom-0.7.2/PKG-INFO
```

### Comparing `text_lloom-0.7.1/pyproject.toml` & `text_lloom-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "text_lloom"
-version = "0.7.1"
+version = "0.7.2"
 description = "Concept Induction to analyze unstructured text"
 authors = ["Michelle Lam <mlam4@cs.stanford.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 hdbscan = "^0.8.33"
```

### Comparing `text_lloom-0.7.1/src/text_lloom/__init__.py` & `text_lloom-0.7.2/src/text_lloom/__init__.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.1/src/text_lloom/concept.py` & `text_lloom-0.7.2/src/text_lloom/concept.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.1/src/text_lloom/concept_induction.py` & `text_lloom-0.7.2/src/text_lloom/concept_induction.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,15 +171,19 @@
             "n_quotes": n_quotes, 
             "seeding_phrase": seeding_phrase.upper()
         } for ex in text_df[doc_col].tolist()
     ]
     
     # Run prompts
     prompt_template = filter_prompt
-    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
+    if sess is not None:
+        rate_limits = sess.rate_limits
+    else:
+        rate_limits = None
+    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
 
     # Process results
     ex_ids = [ex_id for ex_id in text_df[doc_id_col].tolist()]
     for ex_id, res in zip(ex_ids, res_text):
         cur_filtered_list = json_load(res, top_level_key="relevant_quotes")
         if cur_filtered_list is not None:
             cur_filtered = "\n".join(cur_filtered_list)
@@ -225,15 +229,19 @@
             "n_words": n_words_per_bullet
         }
         arg_dicts.append(arg_dict)
         all_ex_ids.append(ex_id)
     
     # Run prompts
     prompt_template = summarize_prompt
-    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
+    if sess is not None:
+        rate_limits = sess.rate_limits
+    else:
+        rate_limits = None
+    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
 
     # Process results
     for ex_id, res in zip(all_ex_ids, res_text):
         cur_bullets_list = json_load(res, top_level_key="bullets")
         if cur_bullets_list is not None:
             for bullet in cur_bullets_list:
                 # Expand each bullet into its own row
@@ -348,15 +356,19 @@
                 "n_concepts_phrase": get_n_concepts_phrase(cur_df),
                 "seed_phrase": seed_phrase
             }
             arg_dicts.append(arg_dict)
 
     # Run prompts
     prompt_template = synthesize_prompt
-    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
+    if sess is not None:
+        rate_limits = sess.rate_limits
+    else:
+        rate_limits = None
+    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
 
     # Process results
     concepts = {}
     rows = []
     logs = ""
     for cur_cluster_id, res in zip(cluster_ids, res_text):
         cur_concepts = json_load(res, top_level_key="patterns")
@@ -462,15 +474,19 @@
     concepts_list_str = "\n".join(concepts_list)
     arg_dicts = [{
         "themes": concepts_list_str,
     }]
 
     # Run prompts
     prompt_template = review_remove_prompt
-    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
+    if sess is not None:
+        rate_limits = sess.rate_limits
+    else:
+        rate_limits = None
+    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
 
     # Process results
     res = res_text[0]
     concepts_to_remove = json_load(res, top_level_key="remove")
 
     if concept_df is not None:
         concept_df_out = concept_df.copy()
@@ -510,15 +526,19 @@
     concepts_list_str = "\n".join(concepts_list)
     arg_dicts = [{
         "themes": concepts_list_str,
     }]
 
     # Run prompts
     prompt_template = review_merge_prompt
-    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
+    if sess is not None:
+        rate_limits = sess.rate_limits
+    else:
+        rate_limits = None
+    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
 
     # Process results
     res = res_text[0]
     concepts_to_merge = json_load(res, top_level_key="merge")
 
     if concept_df is not None:
         concept_df_out = concept_df.copy()
@@ -569,25 +589,25 @@
     save_progress(sess, concept_df_out, step_name="Review-merge", start=start, res=res_full, model_name=model_name)
     return concepts, concept_df_out, concepts_to_merge
 
 # Model selects the best concepts up to `max_concepts`
 # Input: concepts (concept_id -> Concept)
 # Parameters: max_concepts, model_name
 # Output: selected_concepts: dict (concept_id -> Concept)
-async def review_select(concepts, max_concepts, model_name):
+async def review_select(concepts, max_concepts, model_name, rate_limits=None):
     concepts_list = [f"- Name: {c.name}, Prompt: {c.prompt}" for c in concepts.values()]
     concepts_list_str = "\n".join(concepts_list)
     arg_dicts = [{
         "themes": concepts_list_str,
         "max_concepts": max_concepts,
     }]
 
     # Run prompts
     prompt_template = review_select_prompt
-    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
+    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
 
     # Process results
     res = res_text[0]
     selected_concept_names = json_load(res, top_level_key="selected")
 
     selected_concepts = []
     for c_id, c in concepts.items():
@@ -705,15 +725,19 @@
     ]
 
     # Run prompts in parallel to score each example
     if get_highlights:
         prompt_template = score_highlight_prompt
     else:
         prompt_template = score_no_highlight_prompt
-    results, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, batch_num=batch_i)
+    if sess is not None:
+        rate_limits = sess.rate_limits
+    else:
+        rate_limits = None
+    results, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, batch_num=batch_i, rate_limits=rate_limits)
 
     # Parse results
     # Cols: doc_id, text, concept_id, concept_name, concept_prompt, score, highlight
     score_df = None
     for i, res in enumerate(results):
         in_df = in_dfs[i]
         cur_score_df = get_score_df(res, in_df, concept, concept_id, text_col, doc_id_col, get_highlights)
@@ -821,15 +845,19 @@
         "concept_prompt": concept_prompt,
         "examples": cur_df[highlight_col].tolist(),
         "summary_length": summary_length
     }]
     
     # Run prompts
     prompt_template = summarize_concept_prompt
-    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
+    if sess is not None:
+        rate_limits = sess.rate_limits
+    else:
+        rate_limits = None
+    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
 
     # Process results
     res = res_text[0]
     cur_summary = json_load(res, top_level_key="summary")
     if cur_summary is not None:
         if sess is not None:
             sess.concepts[concept_id].summary = cur_summary
@@ -946,15 +974,19 @@
     ]
 
     if debug:
         print(arg_dicts)
 
     # Run prompts
     prompt_template = concept_auto_eval_prompt
-    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
+    if sess is not None:
+        rate_limits = sess.rate_limits
+    else:
+        rate_limits = None
+    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
     
     res_text = res_text[0]
     if debug:
         print(res_text)
 
     # Return the concept coverage and mapping from concepts to items
     concepts_found = {}
```

### Comparing `text_lloom-0.7.1/src/text_lloom/llm.py` & `text_lloom-0.7.2/src/text_lloom/llm.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,44 +30,43 @@
 
 # CONSTANTS ================================
 SYS_TEMPLATE = "You are a helpful assistant who helps with identifying patterns in text examples."
 
 RATE_LIMITS = {
     # https://platform.openai.com/account/limits
     # (n_requests, wait_time_secs)
-    "gpt-3.5-turbo": (300, 10), # = 300*6 = 1800 rpm (max 10k requests per minute for org)
-    "gpt-4": (20, 10), # = 20*6 = 120 rpm (max 10k requests per minute for org)
-    "gpt-4-turbo-preview": (20, 10), # = 20*6 = 120 rpm, testing purposes
+    "gpt-3.5-turbo": (300, 10), # = 300*6 = 1800 rpm
+    "gpt-4": (20, 10), # = 20*6 = 120 rpm
+    "gpt-4-turbo-preview": (20, 10), # = 20*6 = 120 rpm
+    "gpt-4-turbo": (20, 10), # = 20*6 = 120 rpm
 }
 
 CONTEXT_WINDOW = {
     # https://platform.openai.com/docs/models
     # Total tokens shared between input and output
     "gpt-3.5-turbo": 16385,  # Max 4096 output tokens
     "gpt-4": 8192, 
     "gpt-4-turbo-preview": 128000,  # Max 4096 output tokens
+    "gpt-4-turbo": 128000,  # Max 4096 output tokens
 }
 
 COSTS = {
     # https://openai.com/pricing
     "gpt-3.5-turbo": [0.0005/1000, 0.0015/1000],
     "gpt-4": [0.03/1000, 0.06/1000],
     "gpt-4-turbo-preview": [0.01/1000, 0.03/1000],
+    "gpt-4-turbo": [0.01/1000, 0.03/1000],
 }
 
 EMBED_COSTS = {
     "text-embedding-ada-002": (0.00010/1000),
     "text-embedding-3-small": (0.00002/1000),
     "text-embedding-3-large": (0.00013/1000),
 }
 
-def get_system_prompt():
-    system_message_prompt = SystemMessagePromptTemplate.from_template(SYS_TEMPLATE)
-    return system_message_prompt
-
 def get_token_estimate(text, model_name):
     # Fetch the number of tokens used by a prompt
     encoding = tiktoken.encoding_for_model(model_name)
     tokens = encoding.encode(text)
     num_tokens = len(tokens)
     return num_tokens
 
@@ -142,19 +141,20 @@
             except Exception as e:
                 print("Exception", e)
 
     return wrapper
 
 # CUSTOM LLM API WRAPPERS ================================
 
-async def base_api_wrapper(cur_prompt, model_name):
+async def base_api_wrapper(cur_prompt, model_name, temperature):
     # Wrapper for calling the base OpenAI API
     cur_prompt = truncate_prompt(cur_prompt, model_name, out_token_alloc=1500)
     res = await client.chat.completions.create(
         model=model_name,
+        temperature=temperature,
         messages=[
             {"role": "system", "content": SYS_TEMPLATE},
             {"role": "user", "content": cur_prompt},
         ]
     )
     return res
 
@@ -166,23 +166,23 @@
 def truncate_prompt(prompt, model_name, out_token_alloc):
     # Truncate a prompt to fit within a maximum number of tokens
     max_tokens = CONTEXT_WINDOW[model_name] - out_token_alloc
     prompt, n_tokens = truncate_text_tokens(prompt, model_name, max_tokens)
     return prompt
 
 # Internal function making calls to LLM; runs a single LLM query
-async def multi_query_gpt(model_name, prompt_template, arg_dict, batch_num=None, wait_time=None, debug=False):
+async def multi_query_gpt(model_name, prompt_template, arg_dict, batch_num=None, wait_time=None, temperature=0, debug=False):
     if wait_time is not None:
         if debug:
             print(f"Batch {batch_num}, wait time {wait_time}")
         await asyncio.sleep(wait_time)  # wait asynchronously
 
     try: 
         prompt = prompt_template.format(**arg_dict)
-        res = await base_api_wrapper(prompt, model_name)
+        res = await base_api_wrapper(prompt, model_name, temperature)
     except Exception as e:
         print("Error", e)
         return None
     
     return res
 
 def get_res_str(res):
@@ -191,35 +191,38 @@
 
 def process_results(results):
     # Extract just the text generations from response JSONs
     # Insert None if the result is None
     res_text = [(get_res_str(res) if res else None) for res in results]
     return res_text
 
-async def multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, temperature=0, batch_num=None, batched=True, debug=False):
+async def multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=None, temperature=0, batch_num=None, batched=True, debug=False):
     # Run multiple LLM queries
     if debug:
         print("model_name", model_name)
+    
+    if rate_limits is None:
+        rate_limits = RATE_LIMITS  # Use default values
 
     if not batched:
         # Non-batched version
-        tasks = [multi_query_gpt(model_name, prompt_template, args) for args in arg_dicts]
+        tasks = [multi_query_gpt(model_name, prompt_template, args, temperature=temperature) for args in arg_dicts]
     else:
         # Batched version
-        n_requests, wait_time_secs = RATE_LIMITS[model_name]
+        n_requests, wait_time_secs = rate_limits[model_name]
         tasks = []
         arg_dict_batches = [arg_dicts[i:i + n_requests] for i in range(0, len(arg_dicts), n_requests)]
         for inner_batch_num, cur_arg_dicts in enumerate(arg_dict_batches):
             if batch_num is None:
                 wait_time = wait_time_secs * inner_batch_num
             else:
                 wait_time = wait_time_secs * batch_num
             if debug:
                 wait_time = 0 # Debug mode
-            cur_tasks = [multi_query_gpt(model_name, prompt_template, arg_dict=args, batch_num=batch_num, wait_time=wait_time) for args in cur_arg_dicts]
+            cur_tasks = [multi_query_gpt(model_name, prompt_template, arg_dict=args, batch_num=batch_num, wait_time=wait_time, temperature=temperature) for args in cur_arg_dicts]
             tasks.extend(cur_tasks)
 
     res_full = await asyncio.gather(*tasks)
 
     res_text = process_results(res_full)
     return res_text, res_full
```

### Comparing `text_lloom-0.7.1/src/text_lloom/prompts.py` & `text_lloom-0.7.2/src/text_lloom/prompts.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.1/src/text_lloom/static/index.css` & `text_lloom-0.7.2/src/text_lloom/static/index.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.1/src/text_lloom/static/index.js` & `text_lloom-0.7.2/src/text_lloom/static/index.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.1/src/text_lloom/static/index_select.css` & `text_lloom-0.7.2/src/text_lloom/static/index_select.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.1/src/text_lloom/static/index_select.js` & `text_lloom-0.7.2/src/text_lloom/static/index_select.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.1/src/text_lloom/workbench.py` & `text_lloom-0.7.2/src/text_lloom/workbench.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,39 +13,55 @@
 
 
 # Local imports
 if __package__ is None or __package__ == '':
     # uses current directory visibility
     from concept_induction import *
     from concept import Concept
-    from llm import get_token_estimate, EMBED_COSTS
+    from llm import get_token_estimate, EMBED_COSTS, RATE_LIMITS
 else:
     # uses current package visibility
     from .concept_induction import *
     from .concept import Concept
-    from .llm import get_token_estimate, EMBED_COSTS
+    from .llm import get_token_estimate, EMBED_COSTS, RATE_LIMITS
 
 # WORKBENCH class ================================
 class lloom:
     def __init__(
         self,
         df: pd.DataFrame,
         text_col: str,
         id_col: str = None,
-        save_path: str = None,
+        distill_model_name = "gpt-3.5-turbo",
+        embed_model_name = "text-embedding-3-large",
+        synth_model_name = "gpt-4-turbo",
+        score_model_name = "gpt-3.5-turbo",
+        rate_limits = {}, # D_i = "model-name": (n_requests, wait_time_secs)
         debug: bool = False,
     ):
         # Settings
-        self.model_name = "gpt-3.5-turbo"
-        self.embed_model_name = "text-embedding-3-large"
-        self.synth_model_name = "gpt-4-turbo-preview"
-        self.score_model_name = "gpt-3.5-turbo"
-        self.use_base_api = True
+        self.distill_model_name = distill_model_name  # Distill operators (filter and summarize)
+        self.embed_model_name = embed_model_name  # Cluster operator
+        self.synth_model_name = synth_model_name  # Synthesize operator
+        self.score_model_name = score_model_name  # Score operator
         self.debug = debug  # Whether to run in debug mode
 
+        # Rate limits
+        # n_requests: number of requests allowed in one batch
+        # wait_time_secs: time period (in seconds) to wait before making more requests
+        # RPM (Requests per minute) = n_requests * (60 / wait_time_secs)
+        if len(rate_limits) == 0:
+            rate_limits = RATE_LIMITS  # Use default values set from llm.py
+        else:
+            # Intersect user-provided rate_limits with full set of options set in default RATE_LIMITS
+            for k, v in RATE_LIMITS.items():
+                if k not in rate_limits:
+                    rate_limits[k] = v  # Add in defaults for any missing values
+        self.rate_limits = rate_limits
+
         # Input data
         self.doc_id_col = id_col
         self.doc_col = text_col
         df = self.preprocess_df(df)
         self.in_df = df
         self.df_to_score = df  # Default to df for concept scoring
 
@@ -154,25 +170,25 @@
         est_bullet_tokens = 10  # Tokens for a bullet point
         est_n_clusters = 4  # Estimate of number of clusters
         est_concept_tokens = 40  # Tokens for one generated concept JSON
 
         # Filter: generate filter_n_quotes for each doc
         est_cost = {}
         
-        filter_in_tokens = np.sum([get_token_estimate(filter_prompt + doc, self.model_name) for doc in self.in_df[self.doc_col].tolist()])
+        filter_in_tokens = np.sum([get_token_estimate(filter_prompt + doc, self.distill_model_name) for doc in self.in_df[self.doc_col].tolist()])
         quotes_tokens_per_doc = params["filter_n_quotes"] * est_quote_tokens 
         filter_out_tokens = quotes_tokens_per_doc * len(self.in_df)
-        est_cost["distill_filter"] = calc_cost_by_tokens(self.model_name, filter_in_tokens, filter_out_tokens)
+        est_cost["distill_filter"] = calc_cost_by_tokens(self.distill_model_name, filter_in_tokens, filter_out_tokens)
 
         # Summarize: create n_bullets for each doc
-        summ_prompt_tokens = get_token_estimate(summarize_prompt, self.model_name)
+        summ_prompt_tokens = get_token_estimate(summarize_prompt, self.distill_model_name)
         summ_in_tokens = np.sum([(summ_prompt_tokens + quotes_tokens_per_doc) for _ in range(len(self.in_df))])
         bullets_tokens_per_doc = params["summ_n_bullets"] * est_bullet_tokens
         summ_out_tokens = bullets_tokens_per_doc * len(self.in_df)
-        est_cost["distill_summarize"] = calc_cost_by_tokens(self.model_name, summ_in_tokens, summ_out_tokens)
+        est_cost["distill_summarize"] = calc_cost_by_tokens(self.distill_model_name, summ_in_tokens, summ_out_tokens)
 
         # Cluster: embed each bullet point
         cluster_rate = EMBED_COSTS[self.embed_model_name] 
         cluster_tokens = bullets_tokens_per_doc * len(self.in_df) * cluster_rate
         est_cost["cluster"] = (cluster_tokens, 0)
 
         # Synthesize: create n_concepts for each of the est_n_clusters
@@ -306,15 +322,15 @@
             step_name = "Distill-filter"
             self.print_step_name(step_name)
             with self.spinner_wrapper() as spinner:
                 df_filtered = await distill_filter(
                     text_df=self.in_df, 
                     doc_col=self.doc_col,
                     doc_id_col=self.doc_id_col,
-                    model_name=self.model_name,
+                    model_name=self.distill_model_name,
                     n_quotes=params["filter_n_quotes"],
                     seed=seed,
                     sess=self,
                 )
                 self.df_to_score = df_filtered  # Change to use filtered df for concept scoring
                 self.df_filtered = df_filtered
                 spinner.text = "Done"
@@ -328,15 +344,15 @@
         step_name = "Distill-summarize"
         self.print_step_name(step_name)
         with self.spinner_wrapper() as spinner:
             df_bullets = await distill_summarize(
                 text_df=self.df_filtered, 
                 doc_col=self.doc_col,
                 doc_id_col=self.doc_id_col,
-                model_name=self.model_name,
+                model_name=self.distill_model_name,
                 n_bullets=params["summ_n_bullets"],
                 seed=seed,
                 sess=self,
             )
             self.df_bullets = df_bullets
             spinner.text = "Done"
             spinner.ok("✅")
@@ -433,15 +449,15 @@
         concepts_json = self.__concepts_to_json()
         w = get_select_widget(concepts_json)
         self.select_widget = w
         return w
 
     async def select_auto(self, max_concepts):
         # Select the best concepts up to max_concepts
-        selected_concepts = await review_select(self.concepts, max_concepts, self.synth_model_name)
+        selected_concepts = await review_select(self.concepts, max_concepts, self.synth_model_name, self.rate_limits)
 
         # Handle if selection failed
         if len(selected_concepts) == 0:
             concept_ids = list(self.concepts.keys())
             selected_concepts = random.sample(concept_ids, max_concepts)
 
         # Activate only the selected concepts
```

### Comparing `text_lloom-0.7.1/PKG-INFO` & `text_lloom-0.7.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_lloom
-Version: 0.7.1
+Version: 0.7.2
 Summary: Concept Induction to analyze unstructured text
 Author: Michelle Lam
 Author-email: mlam4@cs.stanford.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

