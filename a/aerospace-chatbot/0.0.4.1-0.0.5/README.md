# Comparing `tmp/aerospace_chatbot-0.0.4.1.tar.gz` & `tmp/aerospace_chatbot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerospace_chatbot-0.0.4.1.tar", max compression
+gzip compressed data, was "aerospace_chatbot-0.0.5.tar", max compression
```

## Comparing `aerospace_chatbot-0.0.4.1.tar` & `aerospace_chatbot-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-04-11 05:19:38.306973 aerospace_chatbot-0.0.4.1/LICENSE
--rw-r--r--   0        0        0      506 2024-04-14 01:32:23.236876 aerospace_chatbot-0.0.4.1/README.md
--rw-r--r--   0        0        0     1308 2024-04-14 02:29:31.648239 aerospace_chatbot-0.0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-31 15:24:34.392942 aerospace_chatbot-0.0.4.1/src/aerospace_chatbot/__init__.py
--rw-r--r--   0        0        0    38333 2024-04-14 02:30:08.758046 aerospace_chatbot-0.0.4.1/src/aerospace_chatbot/admin.py
--rw-r--r--   0        0        0    39957 2024-04-14 01:32:23.240643 aerospace_chatbot-0.0.4.1/src/aerospace_chatbot/data_processing.py
--rw-r--r--   0        0        0      919 2024-03-31 15:24:34.393743 aerospace_chatbot-0.0.4.1/src/aerospace_chatbot/prompts.py
--rw-r--r--   0        0        0    14875 2024-04-14 01:32:23.241786 aerospace_chatbot-0.0.4.1/src/aerospace_chatbot/queries.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 aerospace_chatbot-0.0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-11 05:19:38.306973 aerospace_chatbot-0.0.5/LICENSE
+-rw-r--r--   0        0        0      506 2024-04-14 01:32:23.236876 aerospace_chatbot-0.0.5/README.md
+-rw-r--r--   0        0        0     1290 2024-04-26 14:27:49.251082 aerospace_chatbot-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-31 15:24:34.392942 aerospace_chatbot-0.0.5/src/aerospace_chatbot/__init__.py
+-rw-r--r--   0        0        0    39473 2024-04-26 14:27:49.252138 aerospace_chatbot-0.0.5/src/aerospace_chatbot/admin.py
+-rw-r--r--   0        0        0    40050 2024-04-26 14:27:49.252611 aerospace_chatbot-0.0.5/src/aerospace_chatbot/data_processing.py
+-rw-r--r--   0        0        0      919 2024-03-31 15:24:34.393743 aerospace_chatbot-0.0.5/src/aerospace_chatbot/prompts.py
+-rw-r--r--   0        0        0    13109 2024-04-26 14:27:49.253020 aerospace_chatbot-0.0.5/src/aerospace_chatbot/queries.py
+-rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 aerospace_chatbot-0.0.5/PKG-INFO
```

### Comparing `aerospace_chatbot-0.0.4.1/LICENSE` & `aerospace_chatbot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aerospace_chatbot-0.0.4.1/pyproject.toml` & `aerospace_chatbot-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "aerospace-chatbot"
-version = "0.0.4.1"
+version = "0.0.5"
 description = "Aerospace engineering chatbot and AI tools."
 authors = ["dsmueller <dsm@danmueller.pro>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dan-s-mueller/aerospace_chatbot/tree/main"
 repository = "https://github.com/dan-s-mueller/aerospace_chatbot/tree/main"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.9.7 || >3.9.7,<3.12"
+python = ">3.9.7,<3.12"
 python-dotenv = "^1.0.0"
 ipywidgets = "^8.1.1"
 tiktoken = "^0.5.2"
 watchdog = "^3.0.0"
 chromadb = "^0.4.22"
 jsonlines = "^4.0.0"
 pypdf = "^3.17.4"
```

### Comparing `aerospace_chatbot-0.0.4.1/src/aerospace_chatbot/admin.py` & `aerospace_chatbot-0.0.5/src/aerospace_chatbot/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from pinecone import Pinecone
 import chromadb
 from langchain_openai import ChatOpenAI
 
 from langchain_openai import OpenAIEmbeddings
 from langchain_voyageai import VoyageAIEmbeddings
 from langchain_community.embeddings import HuggingFaceInferenceAPIEmbeddings
+from ragatouille import RAGPretrainedModel
 
 class SecretKeyException(Exception):
     """Exception raised for secret key related errors.
 
     Attributes:
         message -- explanation of the error
         id -- unique identifier for the error
@@ -82,15 +83,15 @@
         logging.info('Index type: '+sb_out['index_type'])
 
         if embeddings:
             # Embeddings
             st.sidebar.title('Embeddings',help='See embedding leaderboard here for performance overview: https://huggingface.co/spaces/mteb/leaderboard')
             if sb_out['index_type']=='RAGatouille':    # Default to selecting hugging face model for RAGatouille, otherwise select alternates
                 sb_out['query_model']=st.sidebar.selectbox('Hugging face rag models', 
-                                                        databases[sb_out['index_type']]['hf_rag_models'], 
+                                                        databases[sb_out['index_type']]['embedding_models'], 
                                                         index=0,
                                                         help="Models listed are compatible with the selected index type.")
                 sb_out['embedding_name']=sb_out['query_model']
             else:
                 sb_out['query_model']=st.sidebar.selectbox('Embedding model family', 
                                                         databases[sb_out['index_type']]['embedding_models'], 
                                                         index=0,
@@ -164,16 +165,18 @@
                             if index['status']['state']=='Ready':
                                 name.append(index['name'])
                         sb_out['index_selected']=st.sidebar.selectbox('Index selected',name,index=0,help='Select the index to use for the application.')
                 elif sb_out['index_type']=='RAGatouille':
                     indices=show_ragatouille_indexes(format=False)
                     if len(indices)>0:
                         name=[]
-                        for index in indices:
-                            name.append(index)
+                        for index in indices['message']:
+                            # Be compatible with embedding types already used. Pinecone only supports lowercase.
+                            if index.startswith((sb_out['index_type'] + '-' + sb_out['embedding_name'].replace('/', '-')).lower()):    
+                                name.append(index)
                         sb_out['index_selected']=st.sidebar.selectbox('Index selected',name,index=0,help='Select the index to use for the application.')
                     else:
                         st.sidebar.markdown('No collections found.',help='Check the status on Home.')
             else:
                 raise ValueError('Embeddings must be enabled to select an index name.')
         if llm:
             # LLM
@@ -207,14 +210,16 @@
                     search_type = st.sidebar.selectbox('Search Type', ['similarity', 'mmr'], index=0,help='Select the search type for the application.')
                     sb_out['model_options']={'output_level':output_level,
                                             'k':k,
                                             'search_type':search_type,
                                             'temperature':temperature}
                 else:
                     sb_out['model_options']={'output_level':output_level,
+                                             'k':k,
+                                            'search_type':None,
                                             'temperature':temperature}
     else:
         if embeddings or rag_type or index_name or llm or model_options:
             # Must have vector database for any of this functionality.
             raise ValueError('Vector database must be enabled to use these options.')
 
     # Secret keys, which does not rely on vector_database
@@ -377,15 +382,16 @@
     Returns:
         query_model: The selected query model based on the provided parameters.
 
     Raises:
         NotImplementedError: If the query model is not recognized.
     """
     if sb['index_type'] == 'RAGatouille':
-        query_model = sb['query_model']
+        query_model = RAGPretrainedModel.from_pretrained(sb['embedding_name'],
+                                                         index_root=os.path.join(os.getenv('LOCAL_DB_PATH'),'.ragatouille'))
     elif sb['query_model'] == 'OpenAI':
         query_model = OpenAIEmbeddings(model=sb['embedding_name'], openai_api_key=secrets['OPENAI_API_KEY'])
     elif sb['query_model'] == 'Voyage':
         query_model = VoyageAIEmbeddings(model=sb['embedding_name'], voyage_api_key=secrets['VOYAGE_API_KEY'], truncation=False)
     elif sb['query_model'] == 'Hugging Face':
         query_model = HuggingFaceInferenceAPIEmbeddings(model_name=sb['embedding_name'], api_key=secrets['HUGGINGFACEHUB_API_TOKEN'])
     else:
@@ -466,25 +472,30 @@
 
     Raises:
         ValueError: If the ragatouille vector database needs to be reset.
 
     """
     if os.getenv('LOCAL_DB_PATH') is None or os.getenv('LOCAL_DB_PATH')=='':
         ragatouille_status = {'status': False, 'message': 'Local database path is not set.'}
-    try:
+    else:
         db_folder_path=os.getenv('LOCAL_DB_PATH')
-        path=os.path.join(db_folder_path,'.ragatouille/colbert/indexes')
-        indexes = []
-        for item in os.listdir(path):
-            item_path = os.path.join(path, item)
-            if os.path.isdir(item_path):
-                indexes.append(item)
-        ragatouille_status = {'status': True, 'indexes': indexes}
-    except Exception as e:
-        ragatouille_status = {'status': False, 'message': 'No indexes found.'}
+        try:
+            path=os.path.join(db_folder_path,'.ragatouille/colbert/indexes')
+            indexes = []
+            for item in os.listdir(path):
+                item_path = os.path.join(path, item)
+                if os.path.isdir(item_path):
+                    indexes.append(item)
+            if len(indexes)>0:
+                ragatouille_status = {'status': True, 'message': indexes}
+            else:
+                ragatouille_status = {'status': False, 'message': 'No indexes found.'}  # if .ragatouille structure exists but is empty
+        except:
+            ragatouille_status = {'status': False, 'message': 'No indexes found.'}  # if .ragatouille structure does not exist yet
+
     if format:
         return _format_ragatouille_status(ragatouille_status)
     else:
         return ragatouille_status
 def st_connection_status_expander(expanded: bool = True, delete_buttons: bool = False, set_secrets: bool = False):
     """
     Expands a Streamlit expander widget to display connection status information.
@@ -530,14 +541,15 @@
         else:
             db_folder_path=os.getenv('LOCAL_DB_PATH')
 
         # Show key status
         st.markdown("**API key status** (Indicates status of local variable. It does not guarantee the key itself is correct):")
         st.markdown(test_key_status())
 
+        # TODO the try statements below sometimes allow delete to be pressed but the index which does exist isn't deleted. Update so an error is thrown if the index is not deleted.
         # Pinecone
         st.markdown(show_pinecone_indexes())
         try:
             pinecone_indexes = [obj.name for obj in show_pinecone_indexes(format=False)['message']]
             if delete_buttons:
                 pinecone_index_name = st.selectbox('Pinecone index to delete', pinecone_indexes)
                 if st.button('Delete Pinecone index', help='This is permanent!'):
@@ -569,19 +581,20 @@
                     st.markdown(f"Database {chroma_db_name} has been deleted.")
         except:
             pass
         
         # Ragatouille
         st.markdown(show_ragatouille_indexes())
         try:
-            ragatouille_indexes = [obj.name for obj in show_ragatouille_indexes(format=False)['message']]
-            if delete_buttons:
+            ragatouille_index_data=show_ragatouille_indexes(format=False)
+            ragatouille_indexes = [obj for obj in ragatouille_index_data['message']]
+            if delete_buttons and ragatouille_index_data['status']==True:
                 ragatouille_name = st.selectbox('RAGatouille database to delete', ragatouille_indexes)
                 if st.button('Delete RAGatouille database', help='This is permanent!'):
-                    data_processing.delete_index('Ragatouille', ragatouille_name, "Standard", local_db_path=db_folder_path)
+                    data_processing.delete_index('RAGatouille', ragatouille_name, "Standard", local_db_path=db_folder_path)
                     st.markdown(f"Index {ragatouille_name} has been deleted.")
         except:
             pass
 
         # Local database path
         st.markdown(f"Local database path: {os.environ['LOCAL_DB_PATH']}")
 def st_setup_page(page_title: str, home_dir:str, sidebar_config: dict = None):
@@ -746,15 +759,15 @@
 
     Returns:
         str: A formatted string representation of the ragatouille status.
 
     """
     index_description=''
     if ragatouille_status['status']:
-        for index in ragatouille_status['indexes']:
+        for index in ragatouille_status['message']:
             name = index
             status = ":heavy_check_mark:"
             index_description += f"- {name}: ({status})\n"
         markdown_string = f"**Ragatouille Indexes**\n{index_description}"
     else:
         message = ragatouille_status['message']
         markdown_string = f"**Ragatouille Indexes**\n- {message} :x:"
```

### Comparing `aerospace_chatbot-0.0.4.1/src/aerospace_chatbot/data_processing.py` & `aerospace_chatbot-0.0.5/src/aerospace_chatbot/data_processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from prompts import SUMMARIZE_TEXT
 
-import os, logging, re, shutil, random
+import os, re, shutil, random
 import hashlib
 import uuid
 from pathlib import Path
-from typing import List
+from typing import List, Union
 
 from tenacity import retry, stop_after_attempt, wait_exponential
 
 from pinecone import Pinecone as pinecone_client
 from pinecone import PodSpec
 
 import chromadb
@@ -39,16 +39,15 @@
 
 from ragxplorer import RAGxplorer, rag
 import pandas as pd
 
 
 def load_docs(index_type:str,
               docs:List[str],
-              query_model:any,
-              embedding_name:str,
+              query_model:object,
               rag_type:str='Standard',
               index_name:str=None,
               n_merge_pages:int=None,
               chunk_method:str='character_recursive',
               chunk_size:int=500,
               chunk_overlap:int=0,
               clear:bool=False,
@@ -59,16 +58,15 @@
               show_progress:bool=False):
     """
     Loads documents into the specified index.
 
     Args:
         index_type (str): The type of index to use.
         docs: The documents to load.
-        query_model: The query model to use.
-        embedding_name: The name of the embedding model to use.
+        query_model (object): The query model to use.
         rag_type (str, optional): The type of RAG (Retrieval-Augmented Generation) to use. Defaults to 'Standard'.
         index_name (str, optional): The name of the index. Defaults to None.
         n_merge_pages (int, optional): Number of pages to to merge when loading. Defaults to 0.
         chunk_method (str, optional): The method to chunk the documents. Defaults to 'character_recursive'.
         chunk_size (int, optional): The size of each chunk. Defaults to 500.
         chunk_overlap (int, optional): The overlap between chunks. Defaults to 0.
         clear (bool, optional): Whether to clear the index before loading new documents. Defaults to False.
@@ -101,28 +99,27 @@
         index_name = index_name + '-parent-child'
     if rag_type == 'Summary':
         index_name = index_name + llm.model_name.replace('/', '-') + '-summary' 
 
     # Initialize client an upsert docs
     vectorstore = initialize_database(index_type, 
                                       index_name, 
-                                      query_model, 
-                                      embedding_name,
+                                      query_model,
                                       rag_type=rag_type,
                                       clear=clear, 
                                       local_db_path=local_db_path,
                                       init_ragatouille=True,
                                       show_progress=show_progress)
-    vectorstore, retriever = upsert_docs(index_type,
-                                         index_name,
-                                         vectorstore,
-                                         chunker,
-                                         batch_size=batch_size,
-                                         show_progress=show_progress,
-                                         local_db_path=local_db_path)
+    vectorstore, _ = upsert_docs(index_type,
+                                 index_name,
+                                 vectorstore,
+                                 chunker,
+                                 batch_size=batch_size,
+                                 show_progress=show_progress,
+                                 local_db_path=local_db_path)
     return vectorstore
 def chunk_docs(docs: List[str],
                rag_type:str='Standard',
                chunk_method:str='character_recursive',
                file_out:str=None,
                n_merge_pages:int=None,
                chunk_size:int=500,
@@ -192,15 +189,15 @@
                                                            chunk_overlap=chunk_overlap,
                                                            add_start_index=True)
             page_chunks = text_splitter.split_documents(pages)
             for i, chunk in enumerate(page_chunks):
                 if show_progress:
                     progress_percentage = i / len(page_chunks)
                     my_bar.progress(progress_percentage, text=f'Chunking documents...{progress_percentage*100:.2f}%')
-                chunk.page_content += str(chunk.metadata)    # Add metadata to the end of the page content, some RAG models don't have metadata.
+                # chunk.page_content += str(chunk.metadata)    # Add metadata to the end of the page content, some RAG models don't have metadata.
                 chunks.append(chunk)    # Not sanitized because the page already was
         elif chunk_method=='None':
             text_splitter = None
             chunks = pages  # No chunking, take whole pages as documents
         else:
             raise NotImplementedError
         
@@ -283,28 +280,26 @@
                 'pages':{'doc_ids':doc_ids,'docs':pages},
                 'summaries':summary_docs,
                 'llm':llm}
     else:
         raise NotImplementedError
 def initialize_database(index_type: str, 
                         index_name: str, 
-                        query_model: str,
-                        embedding_name: str,
+                        query_model: object,
                         rag_type: str,
                         local_db_path: str = None, 
                         clear: bool = False,
                         init_ragatouille: bool = False,
                         show_progress: bool = False):
     """Initializes the database based on the specified parameters.
 
     Args:
         index_type (str): The type of index to use (e.g., "Pinecone", "ChromaDB", "RAGatouille").
         index_name (str): The name of the index.
-        query_model (str): The query model to use.
-        embedding_name (str): The name of the embedding model to use.
+        query_model (object): The query model to use.
         rag_type (str): The type of RAG model to use.
         local_db_path (str, optional): The path to the local database. Defaults to None.
         clear (bool, optional): Whether to clear the index. Defaults to False.
         init_ragatouille (bool, optional): Whether to initialize the RAGatouille model. Defaults to False.
         show_progress (bool, optional): Whether to show the progress bar. Defaults to False.
 
     Returns:
@@ -324,15 +319,15 @@
             delete_index(index_type, index_name, rag_type, local_db_path=local_db_path)
         pc = pinecone_client(api_key=os.getenv('PINECONE_API_KEY'))
         
         try:
             pc.describe_index(index_name)
         except:
             pc.create_index(index_name,
-                            dimension=_embedding_size(query_model,embedding_name),
+                            dimension=_embedding_size(query_model),
                             spec=PodSpec(environment="us-west1-gcp", pod_type="p1.x1"))
         
         index = pc.Index(index_name)
         vectorstore=PineconeVectorStore(index,
                                         index_name=index_name, 
                                         embedding=query_model,
                                         text_key='page_content',
@@ -349,29 +344,33 @@
                                 embedding_function=query_model)     
         if show_progress:
             progress_percentage = 1
             my_bar.progress(progress_percentage, text=f'{progress_text}{progress_percentage*100:.2f}%')   
     elif index_type == "RAGatouille":
         if clear:
             delete_index(index_type, index_name, rag_type, local_db_path=local_db_path)
-        if init_ragatouille:    # Used if the index is not already set
-            vectorstore = RAGPretrainedModel.from_pretrained(query_model,verbose=0)
-        else:   # Used if the index is already set
-            vectorstore = query_model    # The index is picked up directly.
+        if init_ragatouille:    
+            # Used if the index is not already set, initializes root folder and embedding model
+            vectorstore = query_model
+        else:   
+            # Used if the index is already set, loads the index directly
+            vectorstore = RAGPretrainedModel.from_index(index_path=os.path.join(local_db_path,
+                                                                                '.ragatouille/colbert/indexes',
+                                                                                index_name))
         if show_progress:
             progress_percentage = 1
             my_bar.progress(progress_percentage, text=f'{progress_text}{progress_percentage*100:.2f}%')
     else:
         raise NotImplementedError
 
     if show_progress:
         my_bar.empty()
     return vectorstore
 
-@retry(stop=stop_after_attempt(15), wait=wait_exponential(multiplier=1,max=60))
+@retry(stop=stop_after_attempt(5), wait=wait_exponential(multiplier=1,max=60))
 def upsert_docs_pinecone(index_name: str,
                          vectorstore: any, 
                          chunker: dict, 
                          batch_size: int = 50, 
                          local_db_path: str = '.'):
     """
     Upserts documents into Pinecone index. Refactored spearately from upsert_docs to allow for tenacity retries.
@@ -471,28 +470,24 @@
                                           ids=chunk_batch_ids)
                 if show_progress:
                     progress_percentage = i / len(chunker['chunks'])
                     my_bar.progress(progress_percentage, text=f'{progress_text}{progress_percentage*100:.2f}%')
             retriever = vectorstore.as_retriever()
         elif index_type == "RAGatouille":
             # Create an index from the vectorstore.
+            # This will default to split documents into 256 tokens each.
             vectorstore.index(
                 collection=[chunk.page_content for chunk in chunker['chunks']],
                 document_ids=[_stable_hash_meta(chunk.metadata) for chunk in chunker['chunks']],
                 index_name=index_name,
-                max_document_length=chunker['splitters']._chunk_size,
                 overwrite_index=True,
                 split_documents=True,
+                document_metadatas=[chunk.metadata for chunk in chunker['chunks']]
             )
 
-            # Move the directory to the db folder
-            try:
-                shutil.move('.ragatouille', local_db_path)
-            except shutil.Error:
-                pass    # If it already exists, don't do anything
             retriever = vectorstore.as_langchain_retriever()
         else:
             raise NotImplementedError
     elif chunker['rag'] == 'Parent-Child':
         if index_type == 'Pincone':
             if show_progress:
                 progress_text = "Upsert in progress to Pinecone..."
@@ -594,31 +589,32 @@
                 shutil.rmtree(Path(local_db_path).resolve() / 'local_file_store' / index_name)
             except Exception as e:
                 # print(f"Error occurred while deleting ChromaDB local_file_store collection: {e}")
                 pass    # No need to do anything if it doesn't exist
     elif index_type == "ChromaDB":  
         try:
             persistent_client = chromadb.PersistentClient(path=os.path.join(local_db_path,'chromadb'))
-            indices = persistent_client.list_collections()
-            for idx in indices:
-                if index_name in idx.name:
-                    persistent_client.delete_collection(name=idx.name)
+            # indices = persistent_client.list_collections()
+            # for idx in indices:
+            #     if index_name in idx.name:
+                    # persistent_client.delete_collection(name=idx.name)
+            persistent_client.delete_collection(name=index_name)
         except Exception as e:
             # print(f"Error occurred while deleting ChromaDB collection: {e}")
             pass
         # Delete local file store if they exist
         if rag_type == 'Parent-Child' or rag_type == 'Summary':
             try:
                 shutil.rmtree(Path(local_db_path).resolve() / 'local_file_store' / index_name)
             except Exception as e:
                 # print(f"Error occurred while deleting ChromaDB local_file_store collection: {e}")
                 pass    # No need to do anything if it doesn't exist
     elif index_type == "RAGatouille":
         try:
-            ragatouille_path = os.path.join(local_db_path, '.ragatouille')
+            ragatouille_path = os.path.join(local_db_path, '.ragatouille/colbert/indexes', index_name)
             shutil.rmtree(ragatouille_path)
         except Exception as e:
             # print(f"Error occurred while deleting RAGatouille index: {e}")
             pass
     else:
         raise NotImplementedError
 def reduce_vector_query_size(rx_client:RAGxplorer,
@@ -802,56 +798,58 @@
     if len(text) == 0:
         return None
     alphanumeric_pct = sum(c.isalnum() for c in text) / len(text)
     if num_words < 5 or alphanumeric_pct < 0.3:
         return None
     else:
         return page
-def _embedding_size(embedding_family:any,embedding_name:str):
+def _embedding_size(embedding_family:Union[OpenAIEmbeddings,
+                                           VoyageAIEmbeddings,
+                                           HuggingFaceInferenceAPIEmbeddings]):
     """
     Returns the size of the embedding for a given embedding model.
 
     Args:
         embedding_family (object): The embedding model to get the size for.
-        embedding_name (str): The name of the embedding model.
 
     Returns:
         int: The size of the embedding.
 
     Raises:
         NotImplementedError: If the embedding model is not supported.
     """
-    exception_embedding_name=NotImplementedError(f"The embedding name '{embedding_name}' is not available in config.json")
-
     # https://platform.openai.com/docs/models/embeddings
     if isinstance(embedding_family,OpenAIEmbeddings):
-        if embedding_name=="text-embedding-ada-002":
+        name=embedding_family.model
+        if name=="text-embedding-ada-002":
             return 1536
-        elif embedding_name=="text-embedding-3-small":
+        elif name=="text-embedding-3-small":
             return 1536
-        elif embedding_name=="text-embedding-3-large":
+        elif name=="text-embedding-3-large":
             return 3072
         else:
-            raise exception_embedding_name
+            raise NotImplementedError(f"The embedding model '{name}' is not available in config.json")
     # https://docs.voyageai.com/embeddings/
     elif isinstance(embedding_family,VoyageAIEmbeddings):
-        if embedding_name=="voyage-2":
+        name=embedding_family.model
+        if name=="voyage-2":
             return 1024 
-        elif embedding_name=="voyage-large-2":
+        elif name=="voyage-large-2":
             return 1536
         else:
-            raise exception_embedding_name
+            raise NotImplementedError(f"The embedding model '{name}' is not available in config.json")
     # See model pages for embedding sizes
     elif isinstance(embedding_family,HuggingFaceInferenceAPIEmbeddings):
-        if embedding_name=="sentence-transformers/all-MiniLM-L6-v2":
+        name=embedding_family.model_name
+        if name=="sentence-transformers/all-MiniLM-L6-v2":
             return 384
-        elif embedding_name=="mixedbread-ai/mxbai-embed-large-v1":
+        elif name=="mixedbread-ai/mxbai-embed-large-v1":
             return 1024
         else:
-            raise exception_embedding_name
+            raise NotImplementedError(f"The embedding model '{name}' is not available in config.json")
     else:
         raise NotImplementedError(f"The embedding family '{embedding_family}' is not available in config.json")
 
 def _stable_hash_meta(metadata: dict) -> str:
     """
     Stable hash of metadata from Langchain Document.
```

### Comparing `aerospace_chatbot-0.0.4.1/src/aerospace_chatbot/prompts.py` & `aerospace_chatbot-0.0.5/src/aerospace_chatbot/prompts.py`

 * *Files identical despite different names*

### Comparing `aerospace_chatbot-0.0.4.1/src/aerospace_chatbot/queries.py` & `aerospace_chatbot-0.0.5/src/aerospace_chatbot/queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,177 +67,147 @@
         vectorstore (VectorStore): The vector store for document retrieval.
         retriever (Retriever): The retriever for document retrieval.
         memory (ConversationBufferMemory): The memory for conversation history.
         conversational_qa_chain (Chain): The chain for conversational QA.
 
     """
     def __init__(self, 
-                 index_type,
-                 index_name,
-                 query_model,
-                 embedding_name,
+                 index_type:str,
+                 index_name:str,
+                 query_model:object,
                  llm:ChatOpenAI,
-                 rag_type='Standard',
-                 k=6,
-                 search_type='similarity',
-                 fetch_k=50,
-                 temperature=0,
-                 local_db_path='.'):
+                 rag_type:str='Standard',
+                 k:int=6,
+                 search_type:str='similarity',
+                 fetch_k:int=50,
+                 temperature:int=0,
+                 local_db_path:str='.'):
         """
         Initializes a new instance of the QA_Model class.
 
         Args:
             index_type (str): The type of index.
             index_name (str): The name of the index.
-            query_model (str): The query model.
-            embedding_name (str): The name of the embedding.
+            query_model (object): The query model.
             llm (ChatOpenAI): The language model for generating responses.
             rag_type (str, optional): The type of RAG model. Defaults to 'Standard'.
-            k (int, optional): The number of retriever results to consider. Defaults to 6.
-            search_type (str, optional): The type of search to perform. Defaults to 'similarity'.
-            fetch_k (int, optional): The number of documents to fetch from the retriever. Defaults to 50.
+            k (int, optional): The number of retriever results to consider. Defaults to 6. 
+            search_type (str, optional): The type of search to perform. Defaults to 'similarity'. Does not apply to RAGatouille.
+            fetch_k (int, optional): The number of documents to fetch from the retriever. Defaults to 50. Does not apply to RAGatouille.
             temperature (int, optional): The temperature for response generation. Defaults to 0.
             local_db_path (str, optional): The path to the local database. Defaults to '.'.
 
         """
         self.index_type=index_type
         self.index_name=index_name
         self.query_model=query_model
-        self.embedding_name=embedding_name
         self.llm=llm
         self.rag_type=rag_type
         self.k=k
         self.search_type=search_type
         self.fetch_k=fetch_k
         self.temperature=temperature
         self.local_db_path=local_db_path
-        self.sources=[]
+        self.memory=None
+        self.result=None
+        self.sources=None
+        self.ai_response=None
+
 
         # Define retriever search parameters
         search_kwargs = _process_retriever_args(self.search_type,
                                                 self.k,
                                                 self.fetch_k)
 
         # Read in from the vector database
         self.vectorstore=data_processing.initialize_database(self.index_type,
                                                              self.index_name,
                                                              self.query_model,
-                                                             self.embedding_name,
                                                              self.rag_type,
                                                              local_db_path=self.local_db_path,
                                                              init_ragatouille=False)  
+
         if self.rag_type=='Standard':  
             if self.index_type=='ChromaDB' or self.index_type=='Pinecone':
-                self.retriever=self.vectorstore.as_retriever(search_type=self.search_type)
+                self.retriever=self.vectorstore.as_retriever(search_type=self.search_type,
+                                                             search_kwargs=search_kwargs)
             elif self.index_type=='RAGatouille':
-                self.retriever=self.vectorstore.as_langchain_retriever()
+                self.retriever=self.vectorstore.as_langchain_retriever(k=search_kwargs['k'])  
         elif self.rag_type=='Parent-Child' or self.rag_type=='Summary':
             self.lfs = LocalFileStore(Path(self.local_db_path).resolve() / 'local_file_store' / self.index_name)
             self.retriever = MultiVectorRetriever(
                                 vectorstore=self.vectorstore,
                                 byte_store=self.lfs,
                                 id_key="doc_id",
-                            )
+                                search_type=self.search_type,
+                                search_kwargs=search_kwargs)
         else:
             raise NotImplementedError
 
         # Intialize memory
         self.memory = ConversationBufferMemory(
                         return_messages=True, output_key='answer', input_key='question')
 
         # Assemble main chain
         self.conversational_qa_chain=_define_qa_chain(self.llm,
                                                       self.retriever,
-                                                      self.memory,
-                                                      kwargs=search_kwargs)
+                                                      self.memory)
     def query_docs(self,query): 
         """
         Executes a query and retrieves the relevant documents.
 
         Args:
             query (str): The query string.
 
         Returns:
             None
         """       
         self.memory.load_memory_variables({})
         self.result = self.conversational_qa_chain.invoke({'question': query})
 
-        if self.index_type!='RAGatouille':
-            self.sources = '\n'.join(str(data.metadata) for data in self.result['references'])
-            if self.llm.__class__.__name__=='ChatOpenAI':
-                self.ai_response = self.result['answer'].content + '\n\nSources:\n' + self.sources
-            else:
-                raise NotImplementedError
+        self.sources = '\n'.join(str(data.metadata) for data in self.result['references'])
+        if self.llm.__class__.__name__=='ChatOpenAI':
+            self.ai_response = self.result['answer'].content + '\n\nSources:\n' + self.sources
         else:
-            # RAGatouille doesn't have metadata, need to extract from context first.
-            extracted_metadata = []
-            pattern = r'\{([^}]*)\}(?=[^{}]*$)' # Regular expression pattern to match the last curly braces
-
-            for ref in self.result['references']:
-                match = re.search(pattern, ref.page_content)
-                if match:
-                    extracted_metadata.append("{"+match.group(1)+"}")
-            self.sources = '\n'.join(extracted_metadata)
-
-            if self.llm.__class__.__name__=='ChatOpenAI':
-                self.ai_response=self.result['answer'].content + '\n\nSources:\n' + self.sources
-            else:
-                raise NotImplementedError
+            raise NotImplementedError
 
         self.memory.save_context({'question': query}, {'answer': self.ai_response})
+        
     def update_model(self,
-                     llm:ChatOpenAI,
-                     search_type='similarity',
-                     k=6,
-                     fetch_k=50):
+                     llm:ChatOpenAI):
         """
-        Updates the model with new parameters.
+        Updates with a new LLM.
 
         Args:
             llm (ChatOpenAI): The language model for generating responses.
-            search_type (str, optional): The type of search to perform. Defaults to 'similarity'.
-            k (int, optional): The number of retriever results to consider. Defaults to 6.
-            fetch_k (int, optional): The number of documents to fetch from the retriever. Defaults to 50.
 
         Returns:
             None
         """
+        # TODO add in updated retrieval parameters
         self.llm=llm
-        self.search_type=search_type
-        self.k=k
-        self.fetch_k=fetch_k
 
-        # Define retriever search parameters
-        search_kwargs = _process_retriever_args(search_type=self.search_type,
-                                                k=self.k,
-                                                fetch_k=self.fetch_k)
-        
         # Update conversational retrieval chain
         self.conversational_qa_chain=_define_qa_chain(self.llm,
                                                       self.retriever,
-                                                      self.memory,
-                                                      kwargs=search_kwargs)
-        logging.info('Updated qa chain: '+str(self.conversational_qa_chain))
+                                                      self.memory)
     def generate_alternative_questions(self,
-                                       prompt:str,
-                                       response=None):
+                                       prompt:str):
         """
         Generates alternative questions based on a prompt.
 
         Args:
             prompt (str): The prompt for generating alternative questions.
-            response (str, optional): The response context. Defaults to None.
 
         Returns:
             str: The generated alternative questions.
         """
-        if response:
+        if self.ai_response:
             prompt_template=GENERATE_SIMILAR_QUESTIONS_W_CONTEXT
-            invoke_dict={'question':prompt,'context':response}
+            invoke_dict={'question':prompt,'context':self.ai_response}
         else:
             prompt_template=GENERATE_SIMILAR_QUESTIONS
             invoke_dict={'question':prompt}
         
         chain = (
                 prompt_template
                 | self.llm
@@ -263,23 +233,21 @@
     Returns:
         str: The combined string of all the documents.
     """
     doc_strings = [format_document(doc, document_prompt) for doc in docs]
     return document_separator.join(doc_strings)
 def _define_qa_chain(llm,
                      retriever,
-                     memory,
-                     kwargs=None):
+                     memory):
     """Defines the conversational QA chain.
 
     Args:
         llm: The language model component.
         retriever: The document retriever component.
         memory: The memory component.
-        kwargs: Optional keyword arguments.
 
     Returns:
         The conversational QA chain.
 
     Raises:
         None.
     """
@@ -341,12 +309,12 @@
     #         filter_items.append(filter_item)
     #     filter={'$or':filter_items}
     # else:
     #     filter=None
 
     # Implement filtering and number of documents to return
     if search_type=='mmr':
-        search_kwargs={'k':k,'fetch_k':fetch_k,'filter':filter} # See as_retriever docs for parameters
+        search_kwargs={'k':k,'fetch_k':fetch_k} # See as_retriever docs for parameters
     else:
-        search_kwargs={'k':k,'filter':filter} # See as_retriever docs for parameters
+        search_kwargs={'k':k} # See as_retriever docs for parameters
     
     return search_kwargs
```

### Comparing `aerospace_chatbot-0.0.4.1/PKG-INFO` & `aerospace_chatbot-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: aerospace-chatbot
-Version: 0.0.4.1
+Version: 0.0.5
 Summary: Aerospace engineering chatbot and AI tools.
 Home-page: https://github.com/dan-s-mueller/aerospace_chatbot/tree/main
 License: MIT
 Author: dsmueller
 Author-email: dsm@danmueller.pro
-Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*, !=3.12.*
+Requires-Python: >3.9.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chromadb (>=0.4.22,<0.5.0)
 Requires-Dist: huggingface-hub (>=0.20.3,<0.21.0)
 Requires-Dist: ipykernel (>=6.29.3,<7.0.0)
 Requires-Dist: ipywidgets (>=8.1.1,<9.0.0)
 Requires-Dist: jsonlines (>=4.0.0,<5.0.0)
```

