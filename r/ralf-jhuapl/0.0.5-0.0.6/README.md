# Comparing `tmp/ralf-jhuapl-0.0.5.tar.gz` & `tmp/ralf-jhuapl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralf-jhuapl-0.0.5.tar", last modified: Thu Sep 21 13:30:36 2023, max compression
+gzip compressed data, was "ralf-jhuapl-0.0.6.tar", last modified: Thu Apr 25 23:10:40 2024, max compression
```

## Comparing `ralf-jhuapl-0.0.5.tar` & `ralf-jhuapl-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3094 2023-07-09 19:35:10.666199 ralf-jhuapl-0.0.5/.gitignore
--rw-r--r--   0        0        0      705 2023-05-01 22:24:53.483639 ralf-jhuapl-0.0.5/.readthedocs.yaml
--rw-r--r--   0        0        0     1112 2023-05-02 23:47:05.913100 ralf-jhuapl-0.0.5/LICENSE
--rw-r--r--   0        0        0     3387 2023-09-20 01:45:46.163505 ralf-jhuapl-0.0.5/README.md
--rw-r--r--   0        0        0   162364 2023-05-01 22:24:53.484177 ralf-jhuapl-0.0.5/assets/ralf_logo_v1.png
--rw-r--r--   0        0        0   186140 2023-05-01 22:24:53.484562 ralf-jhuapl-0.0.5/assets/ralf_logo_v2.png
--rwxr-xr-x   0        0        0      855 2023-09-20 21:05:53.743341 ralf-jhuapl-0.0.5/demos/classifier_demo.py
--rwxr-xr-x   0        0        0     1774 2023-09-20 12:59:32.242777 ralf-jhuapl-0.0.5/demos/dispatcher_demo.py
--rw-r--r--   0        0        0      123 2023-07-09 19:35:10.667671 ralf-jhuapl-0.0.5/demos/ralf_data/models.yml
--rw-r--r--   0        0        0      451 2023-05-08 19:23:25.306521 ralf-jhuapl-0.0.5/demos/ralf_data/prompts.yml
--rw-r--r--   0        0        0      634 2023-05-01 22:24:53.485531 ralf-jhuapl-0.0.5/docs/Makefile
--rw-r--r--   0        0        0       49 2023-05-01 22:24:53.485776 ralf-jhuapl-0.0.5/docs/api/modules.rst
--rw-r--r--   0        0        0      522 2023-05-01 22:24:53.485919 ralf-jhuapl-0.0.5/docs/api/ralf.rst
--rw-r--r--   0        0        0     2177 2023-09-21 13:23:11.793976 ralf-jhuapl-0.0.5/docs/conf.py
--rw-r--r--   0        0        0     2494 2023-09-21 12:49:36.041532 ralf-jhuapl-0.0.5/docs/index.rst
--rw-r--r--   0        0        0     1605 2023-05-03 02:40:43.168068 ralf-jhuapl-0.0.5/docs/introduction/quickstart.rst
--rw-r--r--   0        0        0      800 2023-05-01 22:24:53.486292 ralf-jhuapl-0.0.5/docs/make.bat
--rw-r--r--   0        0        0       49 2023-05-01 22:24:53.486355 ralf-jhuapl-0.0.5/docs/modules.rst
--rw-r--r--   0        0        0      545 2023-05-01 22:24:53.486421 ralf-jhuapl-0.0.5/docs/ralf.rst
--rw-r--r--   0        0        0     1285 2023-05-01 22:24:53.486534 ralf-jhuapl-0.0.5/docs/tutorials/actions.rst
--rw-r--r--   0        0        0     4654 2023-05-01 22:24:53.486634 ralf-jhuapl-0.0.5/docs/tutorials/classification.ipynb
--rw-r--r--   0        0        0    14124 2023-07-09 19:35:10.668191 ralf-jhuapl-0.0.5/docs/tutorials/executing_actions.ipynb
--rw-r--r--   0        0        0      854 2023-09-20 19:11:46.989769 ralf-jhuapl-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1154 2023-09-21 13:23:00.883237 ralf-jhuapl-0.0.5/ralf/__init__.py
--rw-r--r--   0        0        0     8111 2023-09-20 13:25:03.405291 ralf-jhuapl-0.0.5/ralf/classifier.py
--rw-r--r--   0        0        0      145 2023-09-20 13:56:19.971039 ralf-jhuapl-0.0.5/ralf/config.yml
--rw-r--r--   0        0        0    16758 2023-09-20 14:14:22.690980 ralf-jhuapl-0.0.5/ralf/dispatcher.py
--rw-r--r--   0        0        0     8567 2023-09-20 21:02:26.219797 ralf-jhuapl-0.0.5/ralf/utils.py
--rw-r--r--   0        0        0       56 2023-05-01 22:24:53.487331 ralf-jhuapl-0.0.5/requirements.txt
--rw-r--r--   0        0        0     4033 1970-01-01 00:00:00.000000 ralf-jhuapl-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3094 2023-07-09 19:35:10.666199 ralf-jhuapl-0.0.6/.gitignore
+-rw-r--r--   0        0        0      705 2023-05-01 22:24:53.483639 ralf-jhuapl-0.0.6/.readthedocs.yaml
+-rw-r--r--   0        0        0     1112 2023-05-02 23:47:05.913100 ralf-jhuapl-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3686 2024-04-25 23:09:47.263749 ralf-jhuapl-0.0.6/README.md
+-rw-r--r--   0        0        0   162364 2023-05-01 22:24:53.484177 ralf-jhuapl-0.0.6/assets/ralf_logo_v1.png
+-rw-r--r--   0        0        0   186140 2023-05-01 22:24:53.484562 ralf-jhuapl-0.0.6/assets/ralf_logo_v2.png
+-rwxr-xr-x   0        0        0      867 2024-04-25 22:44:22.802154 ralf-jhuapl-0.0.6/demos/classifier_demo.py
+-rwxr-xr-x   0        0        0     1774 2023-09-20 12:59:32.242777 ralf-jhuapl-0.0.6/demos/dispatcher_demo.py
+-rw-r--r--   0        0        0      127 2024-04-25 22:44:22.802783 ralf-jhuapl-0.0.6/demos/ralf_data/models.yml
+-rw-r--r--   0        0        0      451 2023-05-08 19:23:25.306521 ralf-jhuapl-0.0.6/demos/ralf_data/prompts.yml
+-rw-r--r--   0        0        0      634 2023-05-01 22:24:53.485531 ralf-jhuapl-0.0.6/docs/Makefile
+-rw-r--r--   0        0        0       49 2023-05-01 22:24:53.485776 ralf-jhuapl-0.0.6/docs/api/modules.rst
+-rw-r--r--   0        0        0      522 2023-05-01 22:24:53.485919 ralf-jhuapl-0.0.6/docs/api/ralf.rst
+-rw-r--r--   0        0        0     2177 2024-04-25 22:46:09.791920 ralf-jhuapl-0.0.6/docs/conf.py
+-rw-r--r--   0        0        0     2494 2023-09-21 12:49:36.041532 ralf-jhuapl-0.0.6/docs/index.rst
+-rw-r--r--   0        0        0     1605 2023-05-03 02:40:43.168068 ralf-jhuapl-0.0.6/docs/introduction/quickstart.rst
+-rw-r--r--   0        0        0      800 2023-05-01 22:24:53.486292 ralf-jhuapl-0.0.6/docs/make.bat
+-rw-r--r--   0        0        0       49 2023-05-01 22:24:53.486355 ralf-jhuapl-0.0.6/docs/modules.rst
+-rw-r--r--   0        0        0      545 2023-05-01 22:24:53.486421 ralf-jhuapl-0.0.6/docs/ralf.rst
+-rw-r--r--   0        0        0     1285 2023-05-01 22:24:53.486534 ralf-jhuapl-0.0.6/docs/tutorials/actions.rst
+-rw-r--r--   0        0        0     4654 2023-05-01 22:24:53.486634 ralf-jhuapl-0.0.6/docs/tutorials/classification.ipynb
+-rw-r--r--   0        0        0    14124 2023-07-09 19:35:10.668191 ralf-jhuapl-0.0.6/docs/tutorials/executing_actions.ipynb
+-rw-r--r--   0        0        0      854 2024-04-25 22:46:11.871614 ralf-jhuapl-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1154 2024-04-25 22:44:42.031924 ralf-jhuapl-0.0.6/ralf/__init__.py
+-rw-r--r--   0        0        0     8111 2023-09-20 13:25:03.405291 ralf-jhuapl-0.0.6/ralf/classifier.py
+-rw-r--r--   0        0        0       72 2024-04-25 22:44:22.803965 ralf-jhuapl-0.0.6/ralf/config.yml
+-rw-r--r--   0        0        0    17758 2024-04-25 22:44:22.804697 ralf-jhuapl-0.0.6/ralf/dispatcher.py
+-rw-r--r--   0        0        0     8477 2024-04-25 22:44:22.805495 ralf-jhuapl-0.0.6/ralf/utils.py
+-rw-r--r--   0        0        0       64 2024-04-25 22:44:22.806459 ralf-jhuapl-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     4332 1970-01-01 00:00:00.000000 ralf-jhuapl-0.0.6/PKG-INFO
```

### Comparing `ralf-jhuapl-0.0.5/.gitignore` & `ralf-jhuapl-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/.readthedocs.yaml` & `ralf-jhuapl-0.0.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/LICENSE` & `ralf-jhuapl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/README.md` & `ralf-jhuapl-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     pip install ralf-jhuapl
 
 #### Install from Source
 
 Alternatively, you can build the package from source. First, clone the Github repository:
 
-    git clone https://gitlab.jhuapl.edu/ralf/ralf
+    git clone https://github.com/jhuapl-fomo/ralf.git
 
 Next, install the requirements using ``pip``:
     
     cd ralf
     pip install -r requirements.txt
 
 Then, build the package using ``flit`` and install it using ``pip``:
@@ -57,19 +57,26 @@
     pip install .
 
 Or if you would like an editable installation, you can instead use:
 
     pip install -e .
 
 ### OpenAI Configuration
-**ralf** currently relies on language models provided by OpenAI. 
-In order to access the models, you must store your OpenAI API key as an 
+**ralf** currently relies on language models provided by OpenAI, either directly
+via the OpenAI API or through Microsoft Azure. In either case, you must save your API key as an
 environment variable by executing the following in bash:
 
-    echo "export OPENAI_API_KEY='yourkey'" >> ~/.bashrc
+    echo "export OPENAI_API_KEY='your_key'" >> ~/.bashrc
+    source ~/.bashrc
+
+### OpenAI Configuration (Azure)
+If you are accessing OpenAI models through Azure, you must additionally provide
+the URL for your Azure endpoint.
+
+    echo "export OPENAI_API_KEY='https://yourendpoint.openai.azure.com/'" >> ~/.bashrc
     source ~/.bashrc
 
 ### Running the Demos
 To test if installation was successful, try running the demo scripts:
 
     cd demos
     python dispatcher_demo.py
```

### Comparing `ralf-jhuapl-0.0.5/assets/ralf_logo_v1.png` & `ralf-jhuapl-0.0.6/assets/ralf_logo_v1.png`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/assets/ralf_logo_v2.png` & `ralf-jhuapl-0.0.6/assets/ralf_logo_v2.png`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/demos/classifier_demo.py` & `ralf-jhuapl-0.0.6/demos/classifier_demo.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 A demonstration of using ZeroShotClassifier for sentiment classification.
 """
 
 from ralf import classifier
 
 # Define the zero shot classifer
 sentiment_classifier = classifier.ZeroShotClassifier(
-    completion_model_config={'model':'gpt-4'}
+    completion_model_config={'model':'gpt-35-turbo-0125'}
 )
 
 # Add classes with zero or more examples of each
 sentiment_classifier.add_class("positive", examples=["this couldn't be better"])
 sentiment_classifier.add_class("negative", examples=["I'm unimpressed.",
                                                      "not her best work..."])
 sentiment_classifier.add_class("neutral")
```

### Comparing `ralf-jhuapl-0.0.5/demos/dispatcher_demo.py` & `ralf-jhuapl-0.0.6/demos/dispatcher_demo.py`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/docs/Makefile` & `ralf-jhuapl-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/docs/api/ralf.rst` & `ralf-jhuapl-0.0.6/docs/api/ralf.rst`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/docs/conf.py` & `ralf-jhuapl-0.0.6/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'ralf'
 copyright = '2023, Johns Hopkins University Applied Physics Laboratory'
 author = 'JHUAPL'
 
 # The full version, including alpha/beta/rc tags
-release = '0.0.5'
+release = '0.0.6'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `ralf-jhuapl-0.0.5/docs/index.rst` & `ralf-jhuapl-0.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/docs/introduction/quickstart.rst` & `ralf-jhuapl-0.0.6/docs/introduction/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/docs/make.bat` & `ralf-jhuapl-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/docs/ralf.rst` & `ralf-jhuapl-0.0.6/docs/ralf.rst`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/docs/tutorials/actions.rst` & `ralf-jhuapl-0.0.6/docs/tutorials/actions.rst`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/docs/tutorials/classification.ipynb` & `ralf-jhuapl-0.0.6/docs/tutorials/classification.ipynb`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/docs/tutorials/executing_actions.ipynb` & `ralf-jhuapl-0.0.6/docs/tutorials/executing_actions.ipynb`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/pyproject.toml` & `ralf-jhuapl-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/ralf/__init__.py` & `ralf-jhuapl-0.0.6/ralf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

### Comparing `ralf-jhuapl-0.0.5/ralf/classifier.py` & `ralf-jhuapl-0.0.6/ralf/classifier.py`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.5/ralf/dispatcher.py` & `ralf-jhuapl-0.0.6/ralf/dispatcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,36 +2,25 @@
 import yaml
 import time
 import inspect
 from dataclasses import dataclass, asdict
 from pathlib import Path
 from typing import Optional, Union, Tuple
 
+from openai import OpenAI, AzureOpenAI
 import openai
 
 import ralf.utils as ru
 
 ############################
 ##  OpenAI Configuration  ##
 ############################
 
-# Load the OpenAI API key
-try:
-    openai.api_key = os.environ["OPENAI_API_KEY"]
-except KeyError:
-    print(
-        "You must save your OpenAI API key as an environment "
-        "variable. Please see README for details.\n"
-    )
-    raise SystemExit(1)
-if len(os.environ["OPENAI_API_KEY"]) < 35: 
-    openai.api_type = "azure"
-    openai.api_base = ru.cfg['openai_api_base']
-    openai.api_version = "2023-05-15"  # subject to change
-
+class OpenAIConfigurationError(Exception):
+    pass
 
 ###############
 ##  Helpers  ##
 ###############
 
 def determine_model_type(model_name: str) -> str:
     """Determines the endpoint type given an OpenAI model name
@@ -58,14 +47,70 @@
     :type response: str
 
     :return: the cleaned foundation model completion
     :rtype: str
     """
     return response.strip()
 
+def azure_create(task, **kwargs):
+
+    # endpoints to the model server
+    try:
+        client = AzureOpenAI(
+            azure_endpoint=os.environ["OPENAI_AZURE_ENDPOINT"],
+            api_key=os.environ["OPENAI_API_KEY"],
+            api_version="2024-02-01"
+        )
+    except KeyError:
+        print(
+            "You must specify an Azure endpoint URL as an environment "
+            "variable. Please see README for details.\n"
+        )
+        return None
+
+    # submit the query to the model server
+    return openai_create(task, client, **kwargs)
+
+def openai_create(task, client=None, **kwargs):
+    # endpoints to the model server
+    try:
+        if client is None:
+            client = OpenAI(api_key=os.environ["OPENAI_API_KEY"])
+    except KeyError:
+        print(
+            "You must save your OpenAI API key as an environment "
+            "variable. Please see README for details.\n"
+        )
+        return None
+
+    if task == "completion":
+        task_func = client.completions.create
+    elif task == "chatcompletion":
+        task_func = client.chat.completions.create
+    else:
+        raise ValueError(f"{task} is not a recognized OpenAI task")
+
+    # submit the query to the model server
+    try:
+        response = task_func(**kwargs)
+        return response
+    except openai.APITimeoutError as e:
+        print(e)
+    except openai.BadRequestError as e:
+        print(e)
+    except openai.AuthenticationError as e:
+        print(e)
+    except openai.PermissionDeniedError as e:
+        print(e)
+    except openai.RateLimitError as e:
+        print(e)
+    except openai.APIError as e:
+        print(e)
+    return None
+
 
 #########################
 ##  The Action Report  ##
 ##       Class         ##
 #########################
 
 @dataclass
@@ -183,94 +228,87 @@
                 report.model_config = model_config
 
             task = determine_model_type(model_config['model'])
             completion = None
 
             if task == 'completion':
                 if prompt:
-                    response = self.submit_openai_request(
+                    response = self.submit_llm_request(
                         task=task,
                         prompt=prompt,
                         **model_config
                     )
                     if response:
-                        completion = response.choices[0].text
+                        try:
+                            completion = response["choices"][0]["text"]
+                        except:
+                            completion = response.choices[0].text
                 else:
                     raise Exception("Message prompt format cannot be used for completion")
 
             elif task == 'chatcompletion':
                 if messages:
-                    response = self.submit_openai_request(
+                    response = self.submit_llm_request(
                         task=task,
                         messages=messages,
                         **model_config
                     )
                     if response:
-                        completion = response['choices'][0]['message']['content']
+                        try:
+                            completion = response["choices"][0]["message"]["content"]
+                        except:
+                            completion = response.choices[0].message.content
 
                 else:
-                    response = self.submit_openai_request(
+                    response = self.submit_llm_request(
                         task=task,
                         messages=[
                             {"role": "system", "content": ru.cfg['default_system_message']},
                             {"role": "user", "content": prompt}
                         ],
                         **model_config
                     )
                     if response:
-                        completion = response['choices'][0]['message']['content']
+                        try:
+                            completion = response["choices"][0]["message"]["content"]
+                        except:
+                            completion = response.choices[0].message.content
 
             else:
                 raise ValueError("No such OpenAI model type.")
 
             return {self.output_name : completion if completion else f"No response from OpenAI to {task}"}
         else:
             # Calling a Python action
             return {self.output_name : self.func(context[self.input_name])}
 
-    def submit_openai_request(self, task, retries=10, **kwargs):
-
-        errors = 0
-
-        if task == "completion":
-            task_func = openai.Completion.create
-        elif task == "chatcompletion":
-            task_func = openai.ChatCompletion.create
+    def submit_llm_request(self, task, retries=10, service=None, **kwargs):
+        if not service:
+            service = "azure" if len(os.environ.get("OPENAI_API_KEY", "")) <= 32 else "openai"
+        if service == "openai":
+            service_func = openai_create
+        elif service == "azure":
+            service_func = azure_create
+        # TODO: add support for local models here
         else:
-            raise ValueError(f"{task} is not a recognized OpenAI task")
-
+            raise ValueError(f"{service} is not a recognized LLM service")
+        
+        errors = 0
         while retries + 1 > 0:
-            try:
-                response = task_func(**kwargs, request_timeout=self.request_timeout)
+            response = service_func(task, **kwargs, timeout=ru.cfg['timeout_limit'])
+            if response:
                 return response
-            except openai.error.Timeout:
-                print(f"OpenAI timeout error: ", end="")
-            except openai.error.APIError:
-                print(f"OpenAI API error: ", end="")
-            except openai.error.APIConnectionError:
-                print(f"OpenAI API connection error: ", end="")
-            except openai.error.InvalidRequestError:
-                print(f"OpenAI invalid request error: ", end="")
-            except openai.error.AuthenticationError:
-                print(f"OpenAI authentication error: ", end="")
-            except openai.error.PermissionError:
-                print(f"OpenAI permission error: ", end="")
-            except openai.error.RateLimitError:
-                print(f"OpenAI rate limit error: ", end="")
-            except openai.error.ServiceUnavailableError:
-                print(f"OpenAI service unavailable error: ", end="")
 
             # exponential backoff
             delay = 2**(errors/2)
             print(f"Retrying in {delay:.2f} {'second' if int(delay) == 1 else 'seconds'} ({retries} {'retry' if retries == 1 else 'retries'} remaining)")
             time.sleep(delay)
             retries -= 1
             errors += 1
 
-
 #######################
 ##  The Dispatcher   ##
 ##       Class       ##
 #######################
 
 class ActionDispatcher:
     def __init__(self, dir: Optional[str] = None) -> None:
```

### Comparing `ralf-jhuapl-0.0.5/ralf/utils.py` & `ralf-jhuapl-0.0.6/ralf/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,48 +23,46 @@
     cfg = yaml.load(f, Loader=yaml.FullLoader)
 
 DEFAULT_ENCODER = SentenceTransformer('all-MiniLM-L6-v2', device='cpu')
 
 if len(os.environ["OPENAI_API_KEY"]) < 35:
     # using models through Azure    
     DEFAULT_ACTION_MODEL = {
-        "model": "gpt-35-turbo-0613",
-        "deployment_id": "gpt-35-turbo-0613",
+        "model": "gpt-35-turbo-0125",
+        # "deployment_id": "gpt-35-turbo-0125",
         "temperature": 0.7,
         "max_tokens": 256,
         "top_p": 1.0,
         "frequency_penalty": 0.0,
         "presence_penalty": 0.0,
     }
 
     DEFAULT_CLASSIFIER_MODEL = {
-        "model": "gpt-35-turbo-0613",
-        "deployment_id": "gpt-35-turbo-0613",
+        "model": "gpt-35-turbo-0125",
+        # "deployment_id": "gpt-35-turbo-0125",
         "temperature": 0.0,
         "max_tokens": 100,
         "top_p": 1.0,
         "frequency_penalty": 0.0,
         "presence_penalty": 0.0,
         "stop": ['.'],
     }
 else:
     # using models through OpenAI directly
     DEFAULT_ACTION_MODEL = {
         "model": "gpt-3.5-turbo-0613",
-        #"deployment_id": "gpt-35-turbo-0613",
         "temperature": 0.7,
         "max_tokens": 256,
         "top_p": 1.0,
         "frequency_penalty": 0.0,
         "presence_penalty": 0.0,
     }
 
     DEFAULT_CLASSIFIER_MODEL = {
         "model": "text-davinci-003",
-        #"deployment_id": "gpt-35-turbo-0613",
         "temperature": 0.0,
         "max_tokens": 100,
         "top_p": 1.0,
         "frequency_penalty": 0.0,
         "presence_penalty": 0.0,
         "stop": ['.'],
     }
```

### Comparing `ralf-jhuapl-0.0.5/PKG-INFO` & `ralf-jhuapl-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralf-jhuapl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A lightweight library to support the development of applications using LLMs.
 Author-email: JHUAPL <ralf@jhuapl.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 
     pip install ralf-jhuapl
 
 #### Install from Source
 
 Alternatively, you can build the package from source. First, clone the Github repository:
 
-    git clone https://gitlab.jhuapl.edu/ralf/ralf
+    git clone https://github.com/jhuapl-fomo/ralf.git
 
 Next, install the requirements using ``pip``:
     
     cd ralf
     pip install -r requirements.txt
 
 Then, build the package using ``flit`` and install it using ``pip``:
@@ -75,19 +75,26 @@
     pip install .
 
 Or if you would like an editable installation, you can instead use:
 
     pip install -e .
 
 ### OpenAI Configuration
-**ralf** currently relies on language models provided by OpenAI. 
-In order to access the models, you must store your OpenAI API key as an 
+**ralf** currently relies on language models provided by OpenAI, either directly
+via the OpenAI API or through Microsoft Azure. In either case, you must save your API key as an
 environment variable by executing the following in bash:
 
-    echo "export OPENAI_API_KEY='yourkey'" >> ~/.bashrc
+    echo "export OPENAI_API_KEY='your_key'" >> ~/.bashrc
+    source ~/.bashrc
+
+### OpenAI Configuration (Azure)
+If you are accessing OpenAI models through Azure, you must additionally provide
+the URL for your Azure endpoint.
+
+    echo "export OPENAI_API_KEY='https://yourendpoint.openai.azure.com/'" >> ~/.bashrc
     source ~/.bashrc
 
 ### Running the Demos
 To test if installation was successful, try running the demo scripts:
 
     cd demos
     python dispatcher_demo.py
```

