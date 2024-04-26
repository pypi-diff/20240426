# Comparing `tmp/ezlocalai-0.1.7.tar.gz` & `tmp/ezlocalai-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezlocalai-0.1.7.tar", last modified: Tue Apr  2 03:25:30 2024, max compression
+gzip compressed data, was "ezlocalai-0.1.8.tar", last modified: Fri Apr 26 19:31:55 2024, max compression
```

## Comparing `ezlocalai-0.1.7.tar` & `ezlocalai-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:25:30.796721 ezlocalai-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/.env
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/Docker.md
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-04-02 03:25:30.796721 ezlocalai-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/Pipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/cuda-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/cuda.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/cuda118-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/deepseek.ps1
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/deepseek.yml
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/docker-compose-cuda.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/docker-compose-vulkan.yml
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:25:30.796721 ezlocalai-0.1.7/ezlocalai/
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/CTTS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/IMG.py
--rw-r--r--   0 runner    (1001) docker     (127)    13316 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/LLM.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/STT.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/VLM.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai-ngrok.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:25:30.796721 ezlocalai-0.1.7/ezlocalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-04-02 03:25:30.000000 ezlocalai-0.1.7/ezlocalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-02 03:25:30.000000 ezlocalai-0.1.7/ezlocalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:25:30.000000 ezlocalai-0.1.7/ezlocalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-02 03:25:30.000000 ezlocalai-0.1.7/ezlocalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 03:25:30.000000 ezlocalai-0.1.7/ezlocalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 03:25:30.796721 ezlocalai-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/start.ps1
--rw-r--r--   0 runner    (1001) docker     (127)  2999694 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/vulkan.Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:55.334488 ezlocalai-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/.env
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/Docker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-26 19:31:55.334488 ezlocalai-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/Pipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/cuda-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/cuda.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/deepseek.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/deepseek.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/docker-compose-cuda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:55.330488 ezlocalai-0.1.8/ezlocalai/
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/CTTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/Helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/IMG.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/LLM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/STT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/VLM.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai-ngrok.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:55.334488 ezlocalai-0.1.8/ezlocalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-26 19:31:55.000000 ezlocalai-0.1.8/ezlocalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-26 19:31:55.000000 ezlocalai-0.1.8/ezlocalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:31:55.000000 ezlocalai-0.1.8/ezlocalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-26 19:31:55.000000 ezlocalai-0.1.8/ezlocalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 19:31:55.000000 ezlocalai-0.1.8/ezlocalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:31:55.334488 ezlocalai-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/start.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)  2999708 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ui.py
```

### Comparing `ezlocalai-0.1.7/Docker.md` & `ezlocalai-0.1.8/Docker.md`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.7/Dockerfile` & `ezlocalai-0.1.8/Dockerfile`

 * *Files 11% similar despite different names*

```diff
@@ -8,12 +8,14 @@
 COPY requirements.txt .
 RUN --mount=type=cache,target=/root/.cache/pip,sharing=locked \
     python3 -m pip install --no-cache-dir -r requirements.txt
 RUN git clone https://github.com/Josh-XT/DeepSeek-VL deepseek && \
     cd deepseek && \
     pip install --no-cache-dir -e . && \
     cd ..
+RUN pip install spacy && \
+    python -m spacy download en_core_web_sm
 COPY . .
 ENV HOST 0.0.0.0
 EXPOSE 8091
 EXPOSE 8502
 CMD streamlit run ui.py & uvicorn app:app --host 0.0.0.0 --port 8091 --workers 1 --proxy-headers
```

### Comparing `ezlocalai-0.1.7/LICENSE` & `ezlocalai-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.7/PKG-INFO` & `ezlocalai-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: ezlocalai
-Version: 0.1.7
+Version: 0.1.8
 Summary: ezlocalai is an easy to set up local artificial intelligence server with OpenAI Style Endpoints.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: streamlit
-Requires-Dist: pydantic==2.6.3
+Requires-Dist: pydantic
 Requires-Dist: requests==2.31.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: faster-whisper==1.0.1
 Requires-Dist: pydub==0.25.1
 Requires-Dist: ffmpeg-python==0.2.0
-Requires-Dist: torch==2.2.1
-Requires-Dist: torchaudio==2.2.1
-Requires-Dist: transformers==4.38.2
+Requires-Dist: torch==2.3.0
+Requires-Dist: torchaudio==2.3.0
+Requires-Dist: transformers
 Requires-Dist: TTS==0.22.0
 Requires-Dist: sounddevice==0.4.6
 Requires-Dist: pyaudio==0.2.14
 Requires-Dist: webrtcvad==2.0.10
-Requires-Dist: pyngrok==7.1.5
-Requires-Dist: accelerate==0.27.2
+Requires-Dist: pyngrok==7.1.6
+Requires-Dist: accelerate
 Requires-Dist: python-multipart
-Requires-Dist: llama-cpp-python==0.2.55
+Requires-Dist: llama-cpp-python
 Requires-Dist: openai
+Requires-Dist: pdfplumber
+Requires-Dist: spacy
+Requires-Dist: optimum
+Requires-Dist: onnx
 
 # ezlocalai
 
 [![GitHub](https://img.shields.io/badge/GitHub-ezLocalai-blue?logo=github&style=plastic)](https://github.com/DevXT-LLC/ezlocalai) [![Dockerhub](https://img.shields.io/badge/Docker-ezlocalai-blue?logo=docker&style=plastic)](https://hub.docker.com/r/joshxt/ezlocalai)
 
 ezlocalai is an easy set up artificial intelligence server that allows you to easily run multimodal artificial intelligence from your computer. It is designed to be as easy as possible to get started with running local models. It automatically handles downloading the model of your choice and configuring the server based on your CPU, RAM, and GPU specifications. It also includes [OpenAI Style](https://pypi.org/project/openai/) endpoints for easy integration with other applications using ezlocalai as an OpenAI API proxy with any model. Additional functionality is built in for voice cloning text to speech and a voice to text for easy voice communication as well as image generation entirely offline after the initial setup.
 
 ## Prerequisites
 
 - [Git](https://git-scm.com/downloads)
-- [PowerShell 7.X](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.4)
 - [Docker Desktop](https://docs.docker.com/docker-for-windows/install/) (Windows or Mac)
 - [CUDA Toolkit](https://developer.nvidia.com/cuda-downloads) (NVIDIA GPU only)
 
 <details>
   <summary>Additional Linux Prerequisites</summary>
 
 - [Docker](https://docs.docker.com/get-docker/)
@@ -72,65 +75,51 @@
 Modify the `.env` file to your desired settings. Assumptions will be made on all of these values if you choose to accept the defaults.
 
 Replace the environment variables with your desired settings. Assumptions will be made on all of these values if you choose to accept the defaults.
 
 - `EZLOCALAI_URL` - The URL to use for the server. Default is `http://localhost:8091`.
 - `EZLOCALAI_API_KEY` - The API key to use for the server. If not set, the server will not require an API key when accepting requests.
 - `NGROK_TOKEN` - The ngrok token to use for the server. If not set, ngrok will not be used. Using ngrok will allow you to expose your ezlocalai server to the public with as simple as an API key. [Get your free NGROK_TOKEN here.](https://dashboard.ngrok.com/get-started/your-authtoken)
-- `DEFAULT_MODEL` - The default model to use when no model is specified. Default is `phi-2-dpo`.
+- `DEFAULT_MODEL` - The default model to use when no model is specified. Use the Hugging Face path. Default is `TheBloke/phi-2-dpo-GGUF`.
 - `LLM_MAX_TOKENS` - The maximum number of tokens to use for the language model. If set to `0`, it will automatically use the max tokens for the model. Default is `0`.
 - `WHISPER_MODEL` - The model to use for speech-to-text. Default is `base.en`.
 - `AUTO_UPDATE` - Whether or not to automatically update ezlocalai. Default is `true`.
 - `THREADS` - The number of CPU threads ezlocalai is allowed to use. Default is 4.
 - `GPU_LAYERS` (Only applicable to NVIDIA GPU) - The number of layers to use on the GPU. Default is `0`. Your `GPU_LAYERS` will automatically determine a number of layers to use based on your GPU's memory if it is set to `-1` and you have an NVIDIA GPU. If it is set to `-2`, it will use the maximum number of layers requested by the model.
 - `MAIN_GPU` (Only applicable to NVIDIA GPU) - The GPU to use for the language model. Default is `0`.
 - `IMG_ENABLED` - If set to true, models will choose to generate images when they want to based on the user input. **This is only available on GPU.** Default is `false`.
 - `SD_MODEL` - The stable diffusion model to use. Default is `stabilityai/sdxl-turbo`.
+- `VISION_MODEL` - The vision model to use. Default is None. Current options are `deepseek-ai/deepseek-vl-1.3b-chat` and `deepseek-ai/deepseek-vl-7b-chat`.
 
 </details>
 
 ## Usage
 
-```bash
-./start.ps1
-```
-
-Linux:
+### NVIDIA GPU
 
 ```bash
-sudo pwsh start.ps1
+docker-compose -f docker-compose-cuda.yml down
+docker-compose -f docker-compose-cuda.yml build
+docker-compose -f docker-compose-cuda.yml up
 ```
 
-### Deepseek VL Vision Models
-
-- <https://huggingface.co/deepseek-ai/deepseek-vl-1.3b-chat> (Default)
-- <https://huggingface.co/deepseek-ai/deepseek-vl-7b-chat>
-
-Functionality and endpoint request/response directly mimics the [OpenAI gpt-4-vision API](https://platform.openai.com/docs/guides/vision).
-
-**Only currently available with CUDA GPU.**
-
-Modify `deepseek.yml` if you want to run the 7b model instead of the 1.3b model or want to change any other settings. This also has image generation enabled by default, you can disable it by changing `IMG_ENABLED` to `false` in `deepseek.yml` to reduce video RAM usage. This configuration will fit on a ~16GB GPU.
+### CPU
 
 ```bash
-.\deepseek.ps1
+docker-compose down
+docker-compose build
+docker-compose up
 ```
 
-Linux:
-
-```bash
-sudo pwsh deepseek.ps1
-```
-
-For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb).
-
 ## OpenAI Style Endpoint Usage
 
 OpenAI Style endpoints available at `http://<YOUR LOCAL IP ADDRESS>:8091/v1/` by default. Documentation can be accessed at that <http://localhost:8091> when the server is running.
 
+For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb) once the server is running.
+
 ## Demo UI
 
 You can access the basic demo UI at <http://localhost:8502>, or your local IP address with port 8502.
 
 ## Workflow
 
 ```mermaid
```

### Comparing `ezlocalai-0.1.7/Pipes.py` & `ezlocalai-0.1.8/Pipes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 import os
 import logging
 from dotenv import load_dotenv
 from ezlocalai.LLM import LLM, is_vision_model
 from ezlocalai.STT import STT
 from ezlocalai.CTTS import CTTS
+from ezlocalai.Embedding import Embedding
 from pyngrok import ngrok
 import requests
 import base64
+import pdfplumber
+from typing import List
 
 try:
     from ezlocalai.IMG import IMG
 
     img_import_success = True
 except ImportError:
     img_import_success = False
 
 from ezlocalai.VLM import VLM
 
 
 class Pipes:
     def __init__(self):
         load_dotenv()
+        DEFAULT_MODEL = os.getenv("DEFAULT_MODEL", "TheBloke/phi-2-dpo-GGUF")
+        self.current_llm = DEFAULT_MODEL if DEFAULT_MODEL else "TheBloke/phi-2-dpo-GGUF"
+        logging.info(f"[LLM] {self.current_llm} model loading. Please wait...")
+        self.llm = LLM(model=self.current_llm)
+        logging.info(f"[LLM] {self.current_llm} model loaded successfully.")
+        self.embedder = Embedding()
         self.current_vlm = os.getenv("VISION_MODEL", "")
         logging.info(f"[VLM] {self.current_vlm} model loading. Please wait...")
         self.vlm = None
         if self.current_vlm != "":
             try:
                 self.vlm = VLM(model=self.current_vlm)
             except Exception as e:
@@ -47,34 +56,56 @@
         logging.info(f"[CTTS] xttsv2_2.0.2 model loading. Please wait...")
         self.ctts = CTTS()
         logging.info(f"[CTTS] xttsv2_2.0.2 model loaded successfully.")
         self.current_stt = os.getenv("WHISPER_MODEL", "base")
         logging.info(f"[STT] {self.current_stt} model loading. Please wait...")
         self.stt = STT(model=self.current_stt)
         logging.info(f"[STT] {self.current_stt} model loaded successfully.")
-        DEFAULT_MODEL = os.getenv("DEFAULT_MODEL", "phi-2-dpo")
-        self.current_llm = DEFAULT_MODEL if DEFAULT_MODEL else "phi-2-dpo"
-        # if self.vlm is not None:
-        #    self.llm = self.vlm
-        # else:
-        logging.info(f"[LLM] {self.current_llm} model loading. Please wait...")
-        self.llm = LLM(model=self.current_llm)
         if is_vision_model(self.current_llm):
             if self.vlm is None:
                 self.vlm = self.llm
-        logging.info(f"[LLM] {self.current_llm} model loaded successfully.")
         NGROK_TOKEN = os.environ.get("NGROK_TOKEN", "")
         if NGROK_TOKEN:
             ngrok.set_auth_token(NGROK_TOKEN)
             public_url = ngrok.connect(8091)
             logging.info(f"[ngrok] Public Tunnel: {public_url.public_url}")
             self.local_uri = public_url.public_url
         else:
             self.local_uri = os.environ.get("EZLOCALAI_URL", "http://localhost:8091")
 
+    async def pdf_to_audio(self, title, voice, pdf, chunk_size=200):
+        filename = f"{title}.pdf"
+        file_path = os.path.join(os.getcwd(), "outputs", filename)
+        pdf = pdf.split(",")[1]
+        pdf = base64.b64decode(pdf)
+        with open(file_path, "wb") as pdf_file:
+            pdf_file.write(pdf)
+        content = ""
+        if file_path.endswith(".pdf"):
+            with pdfplumber.open(file_path) as pdf:
+                content = "\n".join([page.extract_text() for page in pdf.pages])
+        if not content:
+            return
+        return await self.ctts.generate(
+            text=content,
+            voice=voice,
+            local_uri=self.local_uri,
+            output_file_name=f"{title}.wav",
+        )
+
+    async def audio_to_audio(self, voice, audio):
+        audio_type = audio.split(",")[0].split(":")[1].split(";")[0]
+        audio_format = audio_type.split("/")[1]
+        audio = audio.split(",")[1]
+        audio = base64.b64decode(audio)
+        text = self.stt.transcribe_audio(base64_audio=audio, audio_format=audio_format)
+        return await self.ctts.generate(
+            text=text, voice=voice, local_uri=self.local_uri
+        )
+
     async def get_response(self, data, completion_type="chat"):
         data["local_uri"] = self.local_uri
         images = []
         if "messages" in data:
             if isinstance(data["messages"][-1]["content"], list):
                 messages = data["messages"][-1]["content"]
                 for message in messages:
@@ -140,17 +171,17 @@
             ]
             new_messages[0]["content"].extend(images)
             image_description = self.vlm.chat(messages=new_messages)
             print(
                 f"Image Description: {image_description['choices'][0]['message']['content']}"
             )
             prompt = (
-                f"\n\nReference the uploaded image description for any questions about the uploaded image. Act as if you can see it. Uploaded Image Description: {image_description['choices'][0]['message']['content']} {data['messages'][-1]['content'][0]['text']}"
+                f"\n\nSee the uploaded image description for any questions about the uploaded image. Act as if you can see the image based on the description. Do not mention 'uploaded image description' in response. Uploaded Image Description: {image_description['choices'][0]['message']['content']}\n\n{data['messages'][-1]['content'][0]['text']}"
                 if completion_type == "chat"
-                else f"\n\nReference the uploaded image description for any questions about the uploaded image. Act as if you can see it. Uploaded Image Description: {image_description['choices'][0]['message']['content']} {data['prompt']}"
+                else f"\n\nSee the uploaded image description for any questions about the uploaded image. Act as if you can see the image based on the description. Do not mention 'uploaded image description' in response. Uploaded Image Description: {image_description['choices'][0]['message']['content']}\n\n{data['prompt']}"
             )
             print(f"Full Prompt: {prompt}")
             if completion_type == "chat":
                 data["messages"][-1]["content"] = prompt
             else:
                 data["prompt"] = prompt
         if completion_type == "chat":
```

### Comparing `ezlocalai-0.1.7/README.md` & `ezlocalai-0.1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 [![GitHub](https://img.shields.io/badge/GitHub-ezLocalai-blue?logo=github&style=plastic)](https://github.com/DevXT-LLC/ezlocalai) [![Dockerhub](https://img.shields.io/badge/Docker-ezlocalai-blue?logo=docker&style=plastic)](https://hub.docker.com/r/joshxt/ezlocalai)
 
 ezlocalai is an easy set up artificial intelligence server that allows you to easily run multimodal artificial intelligence from your computer. It is designed to be as easy as possible to get started with running local models. It automatically handles downloading the model of your choice and configuring the server based on your CPU, RAM, and GPU specifications. It also includes [OpenAI Style](https://pypi.org/project/openai/) endpoints for easy integration with other applications using ezlocalai as an OpenAI API proxy with any model. Additional functionality is built in for voice cloning text to speech and a voice to text for easy voice communication as well as image generation entirely offline after the initial setup.
 
 ## Prerequisites
 
 - [Git](https://git-scm.com/downloads)
-- [PowerShell 7.X](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.4)
 - [Docker Desktop](https://docs.docker.com/docker-for-windows/install/) (Windows or Mac)
 - [CUDA Toolkit](https://developer.nvidia.com/cuda-downloads) (NVIDIA GPU only)
 
 <details>
   <summary>Additional Linux Prerequisites</summary>
 
 - [Docker](https://docs.docker.com/get-docker/)
@@ -39,65 +38,51 @@
 Modify the `.env` file to your desired settings. Assumptions will be made on all of these values if you choose to accept the defaults.
 
 Replace the environment variables with your desired settings. Assumptions will be made on all of these values if you choose to accept the defaults.
 
 - `EZLOCALAI_URL` - The URL to use for the server. Default is `http://localhost:8091`.
 - `EZLOCALAI_API_KEY` - The API key to use for the server. If not set, the server will not require an API key when accepting requests.
 - `NGROK_TOKEN` - The ngrok token to use for the server. If not set, ngrok will not be used. Using ngrok will allow you to expose your ezlocalai server to the public with as simple as an API key. [Get your free NGROK_TOKEN here.](https://dashboard.ngrok.com/get-started/your-authtoken)
-- `DEFAULT_MODEL` - The default model to use when no model is specified. Default is `phi-2-dpo`.
+- `DEFAULT_MODEL` - The default model to use when no model is specified. Use the Hugging Face path. Default is `TheBloke/phi-2-dpo-GGUF`.
 - `LLM_MAX_TOKENS` - The maximum number of tokens to use for the language model. If set to `0`, it will automatically use the max tokens for the model. Default is `0`.
 - `WHISPER_MODEL` - The model to use for speech-to-text. Default is `base.en`.
 - `AUTO_UPDATE` - Whether or not to automatically update ezlocalai. Default is `true`.
 - `THREADS` - The number of CPU threads ezlocalai is allowed to use. Default is 4.
 - `GPU_LAYERS` (Only applicable to NVIDIA GPU) - The number of layers to use on the GPU. Default is `0`. Your `GPU_LAYERS` will automatically determine a number of layers to use based on your GPU's memory if it is set to `-1` and you have an NVIDIA GPU. If it is set to `-2`, it will use the maximum number of layers requested by the model.
 - `MAIN_GPU` (Only applicable to NVIDIA GPU) - The GPU to use for the language model. Default is `0`.
 - `IMG_ENABLED` - If set to true, models will choose to generate images when they want to based on the user input. **This is only available on GPU.** Default is `false`.
 - `SD_MODEL` - The stable diffusion model to use. Default is `stabilityai/sdxl-turbo`.
+- `VISION_MODEL` - The vision model to use. Default is None. Current options are `deepseek-ai/deepseek-vl-1.3b-chat` and `deepseek-ai/deepseek-vl-7b-chat`.
 
 </details>
 
 ## Usage
 
-```bash
-./start.ps1
-```
-
-Linux:
+### NVIDIA GPU
 
 ```bash
-sudo pwsh start.ps1
+docker-compose -f docker-compose-cuda.yml down
+docker-compose -f docker-compose-cuda.yml build
+docker-compose -f docker-compose-cuda.yml up
 ```
 
-### Deepseek VL Vision Models
-
-- <https://huggingface.co/deepseek-ai/deepseek-vl-1.3b-chat> (Default)
-- <https://huggingface.co/deepseek-ai/deepseek-vl-7b-chat>
-
-Functionality and endpoint request/response directly mimics the [OpenAI gpt-4-vision API](https://platform.openai.com/docs/guides/vision).
-
-**Only currently available with CUDA GPU.**
-
-Modify `deepseek.yml` if you want to run the 7b model instead of the 1.3b model or want to change any other settings. This also has image generation enabled by default, you can disable it by changing `IMG_ENABLED` to `false` in `deepseek.yml` to reduce video RAM usage. This configuration will fit on a ~16GB GPU.
+### CPU
 
 ```bash
-.\deepseek.ps1
+docker-compose down
+docker-compose build
+docker-compose up
 ```
 
-Linux:
-
-```bash
-sudo pwsh deepseek.ps1
-```
-
-For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb).
-
 ## OpenAI Style Endpoint Usage
 
 OpenAI Style endpoints available at `http://<YOUR LOCAL IP ADDRESS>:8091/v1/` by default. Documentation can be accessed at that <http://localhost:8091> when the server is running.
 
+For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb) once the server is running.
+
 ## Demo UI
 
 You can access the basic demo UI at <http://localhost:8502>, or your local IP address with port 8502.
 
 ## Workflow
 
 ```mermaid
```

### Comparing `ezlocalai-0.1.7/app.py` & `ezlocalai-0.1.8/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel
 from typing import List, Dict, Union, Optional
 from Pipes import Pipes
 import base64
 import os
 import logging
+import uuid
 from dotenv import load_dotenv
 
 load_dotenv()
-DEFAULT_MODEL = os.getenv("DEFAULT_MODEL", "phi-2-dpo")
+DEFAULT_MODEL = os.getenv("DEFAULT_MODEL", "TheBloke/phi-2-dpo-GGUF")
 WHISPER_MODEL = os.getenv("WHISPER_MODEL", "base")
 logging.basicConfig(
     level=os.environ.get("LOGLEVEL", "INFO"),
     format="%(asctime)s | %(levelname)s | %(message)s",
 )
 pipe = Pipes()
 logging.info(f"[ezlocalai] Server is ready.")
@@ -227,15 +228,15 @@
 
 @app.post(
     "/v1/embeddings",
     tags=["Embeddings"],
     dependencies=[Depends(verify_api_key)],
 )
 async def embedding(embedding: EmbeddingModel, user=Depends(verify_api_key)):
-    return pipe.llm.embedding(input=embedding.input)
+    return pipe.embedder.get_embeddings(input=embedding.input)
 
 
 # Audio Transcription endpoint
 # https://platform.openai.com/docs/api-reference/audio/createTranscription
 @app.post(
     "/v1/audio/transcriptions",
     tags=["Audio"],
@@ -300,14 +301,29 @@
 
 @app.post(
     "/v1/audio/speech",
     tags=["Audio"],
     dependencies=[Depends(verify_api_key)],
 )
 async def text_to_speech(tts: TextToSpeech, user=Depends(verify_api_key)):
+    if tts.input.startswith("data:"):
+        if "pdf" in tts.input:
+            audio = await pipe.pdf_to_audio(
+                title=tts.user if tts.user else f"{uuid.uuid4().hex}",
+                voice=tts.voice,
+                pdf=tts.input,
+                chunk_size=200,
+            )
+            return audio
+        if "audio/" in tts.input:
+            audio = await pipe.audio_to_audio(
+                voice=tts.voice,
+                audio=tts.input,
+            )
+            return audio
     audio = await pipe.ctts.generate(
         text=tts.input, voice=tts.voice, language=tts.language
     )
     return audio
 
 
 @app.get(
```

### Comparing `ezlocalai-0.1.7/cuda.Dockerfile` & `ezlocalai-0.1.8/cuda.Dockerfile`

 * *Files 26% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 
 WORKDIR /app
 ENV HOST=0.0.0.0 \
     CUDA_DOCKER_ARCH=all \
     LLAMA_CUBLAS=1
 COPY cuda-requirements.txt .
 RUN python3 -m pip install --upgrade pip cmake scikit-build setuptools wheel --no-cache-dir && \
-    CMAKE_ARGS="-DLLAMA_CUBLAS=on" FORCE_CMAKE=1 pip install llama-cpp-python==0.2.55 --no-cache-dir && \
+    CMAKE_ARGS="-DLLAMA_CUDA=on" FORCE_CMAKE=1 pip install llama-cpp-python --no-cache-dir && \
     pip install --no-cache-dir -r cuda-requirements.txt
 RUN git clone https://github.com/Josh-XT/DeepSeek-VL deepseek && \
     cd deepseek && \
     pip install --no-cache-dir -e . && \
     cd ..
+RUN pip install spacy && \
+    python -m spacy download en_core_web_sm
 COPY . .
 EXPOSE 8091
 EXPOSE 8502
 CMD streamlit run ui.py & uvicorn app:app --host 0.0.0.0 --port 8091 --workers 1 --proxy-headers
```

### Comparing `ezlocalai-0.1.7/deepseek.yml` & `ezlocalai-0.1.8/deepseek.yml`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
       context: .
       dockerfile: cuda.Dockerfile
     environment:
       - EZLOCALAI_URL=${EZLOCALAI_URL-http://localhost:8091}
       - EZLOCALAI_API_KEY=${EZLOCALAI_API_KEY-}
       - GPU_LAYERS=${GPU_LAYERS-0}
       - MAIN_GPU=${MAIN_GPU-0}
-      - DEFAULT_MODEL=${DEFAULT_MODEL-phi-2-dpo}
+      - DEFAULT_MODEL=${DEFAULT_MODEL-TheBloke/phi-2-dpo-GGUF}
       - LLM_MAX_TOKENS=${LLM_MAX_TOKENS-0}
       - WHISPER_MODEL=${WHISPER_MODEL-base.en}
       - IMG_ENABLED=${IMG_ENABLED-false}
       - SD_MODEL=${SD_MODEL-stabilityai/sdxl-turbo}
       - VISION_MODEL=${VISION_MODEL-deepseek-ai/deepseek-vl-1.3b-chat}
       - CUDA_DOCKER_ARCH=all
     restart: unless-stopped
```

### Comparing `ezlocalai-0.1.7/docker-compose-cuda.yml` & `ezlocalai-0.1.8/docker-compose-cuda.yml`

 * *Files 20% similar despite different names*

```diff
@@ -6,20 +6,21 @@
       context: .
       dockerfile: cuda.Dockerfile
     environment:
       - EZLOCALAI_URL=${EZLOCALAI_URL-http://localhost:8091}
       - EZLOCALAI_API_KEY=${EZLOCALAI_API_KEY-}
       - GPU_LAYERS=${GPU_LAYERS-0}
       - MAIN_GPU=${MAIN_GPU-0}
-      - DEFAULT_MODEL=${DEFAULT_MODEL-phi-2-dpo}
+      - DEFAULT_MODEL=${DEFAULT_MODEL-TheBloke/phi-2-dpo-GGUF}
       - LLM_MAX_TOKENS=${LLM_MAX_TOKENS-0}
       - WHISPER_MODEL=${WHISPER_MODEL-base.en}
       - IMG_ENABLED=${IMG_ENABLED-true}
       - SD_MODEL=${SD_MODEL}
       - VISION_MODEL=${VISION_MODEL}
+      - LLM_BATCH_SIZE=${LLM_BATCH_SIZE-1024}
       - CUDA_DOCKER_ARCH=all
     restart: unless-stopped
     ports:
       - "8091:8091"
       - "8502:8502"
     volumes:
       - ./models:/app/models
```

### Comparing `ezlocalai-0.1.7/docker-compose.yml` & `ezlocalai-0.1.8/docker-compose.yml`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 services:
   ezlocalai:
     image: joshxt/ezlocalai:latest
     environment:
       - EZLOCALAI_URL=${EZLOCALAI_URL-http://localhost:8091}
       - EZLOCALAI_API_KEY=${EZLOCALAI_API_KEY-}
-      - DEFAULT_MODEL=${DEFAULT_MODEL-phi-2-dpo}
+      - DEFAULT_MODEL=${DEFAULT_MODEL-TheBloke/phi-2-dpo-GGUF}
       - LLM_MAX_TOKENS=${LLM_MAX_TOKENS-0}
       - WHISPER_MODEL=${WHISPER_MODEL-base.en}
       - IMG_ENABLED=${IMG_ENABLED-false}
       - VISION_MODEL=${VISION_MODEL}
+      - LLM_BATCH_SIZE=${LLM_BATCH_SIZE-1024}
       - SD_MODEL=${SD_MODEL}
     restart: unless-stopped
     ports:
       - "8091:8091"
       - "8502:8502"
     volumes:
       - ./models:/app/models
```

### Comparing `ezlocalai-0.1.7/ezlocalai/CTTS.py` & `ezlocalai-0.1.8/ezlocalai/CTTS.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 import re
 import uuid
 import base64
 import torch
 import torchaudio
 import requests
 import logging
+from ezlocalai.Helpers import chunk_content
 from TTS.tts.configs.xtts_config import XttsConfig
 from TTS.tts.models.xtts import Xtts
+from typing import List
+import spacy
+from pydub import AudioSegment
 
 try:
     import deepspeed
 
     deepspeed_available = True
 except:
     deepspeed_available = False
@@ -69,16 +73,18 @@
 
     async def generate(
         self,
         text,
         voice="default",
         language="en",
         local_uri=None,
+        output_file_name=None,
     ):
-        output_file_name = f"{uuid.uuid4().hex}.wav"
+        if not output_file_name:
+            output_file_name = f"{uuid.uuid4().hex}.wav"
         output_file = os.path.join(self.output_folder, output_file_name)
         cleaned_string = re.sub(r"([!?.])\1+", r"\1", text)
         cleaned_string = re.sub(
             r'[^a-zA-Z0-9\s\.,;:!?\-\'"\u0400-\u04FFÀ-ÿ\u0150\u0151\u0170\u0171]\$',
             "",
             cleaned_string,
         )
@@ -91,28 +97,40 @@
             audio_path = os.path.join(self.voices_path, "default.wav")
         gpt_cond_latent, speaker_embedding = self.model.get_conditioning_latents(
             audio_path=[f"{audio_path}"],
             gpt_cond_len=self.model.config.gpt_cond_len,
             max_ref_length=self.model.config.max_ref_len,
             sound_norm_refs=self.model.config.sound_norm_refs,
         )
-        output = self.model.inference(
-            text=text,
-            language=language,
-            gpt_cond_latent=gpt_cond_latent,
-            speaker_embedding=speaker_embedding,
-            temperature=0.7,
-            length_penalty=float(self.model.config.length_penalty),
-            repetition_penalty=10.0,
-            top_k=int(self.model.config.top_k),
-            top_p=float(self.model.config.top_p),
-            enable_text_splitting=True,
-        )
-        torchaudio.save(output_file, torch.tensor(output["wav"]).unsqueeze(0), 24000)
-        torch.cuda.empty_cache()
+        text_chunks = chunk_content(text)
+        output_files = []
+        for chunk in text_chunks:
+            output = self.model.inference(
+                text=chunk,
+                language=language,
+                gpt_cond_latent=gpt_cond_latent,
+                speaker_embedding=speaker_embedding,
+                enable_text_splitting=True,
+                temperature=0.7,
+                repetition_penalty=10.0,
+            )
+            output_file_name = f"{uuid.uuid4().hex}.wav"
+            output_file = os.path.join(self.output_folder, output_file_name)
+            torchaudio.save(
+                output_file, torch.tensor(output["wav"]).unsqueeze(0), 24000
+            )
+            output_files.append(output_file)
+            torch.cuda.empty_cache()
+        combined_audio = AudioSegment.empty()
+        for file in output_files:
+            audio = AudioSegment.from_file(file)
+            combined_audio += audio
+            combined_audio += AudioSegment.silent(duration=1000)
+            os.remove(file)
+        combined_audio.export(output_file, format="wav")
         if local_uri:
             return f"{local_uri}/outputs/{output_file_name}"
         with open(output_file, "rb") as file:
             audio_data = file.read()
         os.remove(output_file)
         return base64.b64encode(audio_data).decode("utf-8")
```

### Comparing `ezlocalai-0.1.7/ezlocalai/IMG.py` & `ezlocalai-0.1.8/ezlocalai/IMG.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.7/ezlocalai/LLM.py` & `ezlocalai-0.1.8/ezlocalai/LLM.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,135 +1,107 @@
 from llama_cpp import Llama, llama_chat_format
+from huggingface_hub import hf_hub_download
 from bs4 import BeautifulSoup
 from typing import List, Optional, Dict
 import os
+import re
 import requests
 import psutil
 import torch
 import logging
 
 
-DEFAULT_MODEL = os.environ.get("DEFAULT_MODEL", "phi-2-dpo")
+DEFAULT_MODEL = os.environ.get("DEFAULT_MODEL", "TheBloke/phi-2-dpo-GGUF")
 
 
 def get_vision_models():
     return [
-        {"bakllava-1-7b": "mys/ggml_bakllava-1"},
-        {"llava-v1.5-7b": "mys/ggml_llava-v1.5-7b"},
-        {"llava-v1.5-13b": "mys/ggml_llava-v1.5-13b"},
+        "mys/ggml_bakllava-1",
+        "mys/ggml_llava-v1.5-7b",
+        "mys/ggml_llava-v1.5-13b",
     ]
 
 
 def get_models():
-    try:
-        response = requests.get(
-            "https://huggingface.co/TheBloke?search_models=GGUF&sort_models=modified"
-        )
-        soup = BeautifulSoup(response.text, "html.parser")
-    except:
-        soup = None
-    model_names = get_vision_models()
+    response = requests.get("https://huggingface.co/models?sort=modified&search=gguf")
+    soup = BeautifulSoup(response.text, "html.parser")
+    model_names = []
     if soup:
         for a_tag in soup.find_all("a", href=True):
             href = a_tag["href"]
-            if href.startswith("/TheBloke/") and href.endswith("-GGUF"):
-                base_name = href[10:-5]
-                model_names.append({base_name: href[1:]})
+            if href.endswith("-GGUF"):
+                model_names.append(href[1:])
+    model_names.append(get_vision_models())
     return model_names
 
 
 def is_vision_model(model_name="") -> bool:
     if model_name == "":
         return False
     model_name = model_name.lower()
     for model in get_vision_models():
         for key in model:
             if model_name == key.lower():
                 return True
     return False
 
 
-def get_model_url(model_name=""):
-    if model_name == "":
-        global DEFAULT_MODEL
-        model_name = DEFAULT_MODEL
-    model_url = ""
-    try:
-        models = get_models()
-        for model in models:
-            for key in model:
-                if model_name.lower() == key.lower():
-                    model_url = model[key]
-                    break
-        if model_url == "":
-            raise Exception(
-                f"Model not found. Choose from one of these models: {', '.join(models.keys())}"
-            )
-    except:
-        model_url = f"https://huggingface.co/TheBloke/{model_name}-GGUF"
-    return model_url
-
-
 def download_llm(model_name="", models_dir="models"):
     if model_name != "":
         global DEFAULT_MODEL
         model_name = DEFAULT_MODEL
+    if "/" not in model_name:
+        model_name = "TheBloke/" + model_name + "-GGUF"
     ram = round(psutil.virtual_memory().total / 1024**3)
     if ram > 16:
         default_quantization_type = "Q5_K_M"
     else:
         default_quantization_type = "Q4_K_M"
     quantization_type = os.environ.get("QUANT_TYPE", default_quantization_type)
-    model_url = get_model_url(model_name=model_name)
-    model_name = model_name.lower()
-    file_path = f"{models_dir}/{model_name}/{model_name}.{quantization_type}.gguf"
-    if not os.path.exists(models_dir):
-        os.makedirs(models_dir)
-    if not os.path.exists(f"{models_dir}/{model_name}"):
-        os.makedirs(f"{models_dir}/{model_name}")
-    if not os.path.exists(file_path):
-        clip_url = ""
-        if model_url.startswith("mys/"):
-            url = (
-                f"https://huggingface.co/{model_url}/resolve/main/ggml-model-q5_k.gguf"
-            )
-            clip_url = (
-                f"https://huggingface.co/{model_url}/resolve/main/mmproj-model-f16.gguf"
-            )
-        else:
-            url = (
-                (
-                    model_url
-                    if "https://" in model_url
-                    else f"https://huggingface.co/{model_url}/resolve/main/{model_name}.{quantization_type}.gguf"
-                )
-                if model_name != "mistrallite-7b"
-                else f"https://huggingface.co/TheBloke/MistralLite-7B-GGUF/resolve/main/mistrallite.{quantization_type}.gguf"
+    model = model_name.split("/")[-1].replace("-GGUF", "")
+    filename = model + f".{quantization_type}.gguf"
+    models_dir = os.path.join(models_dir, model)
+    os.makedirs(models_dir, exist_ok=True)
+    clip_file = None
+    if model_name.split("/")[0] == "mys":
+        filename = f"ggml-model-q5_k.gguf"
+        clip_file = f"mmproj-model-f16.gguf"
+    # Check if file exists
+    if clip_file:
+        if not os.path.exists(f"{models_dir}/{clip_file}"):
+            hf_hub_download(
+                repo_id=model_name,
+                filename=clip_file,
+                local_dir=models_dir,
+                local_dir_use_symlinks=False,
             )
-        logging.info(f"[LLM] Downloading {model_name}...")
-        with requests.get(url, stream=True, allow_redirects=True) as r:
-            with open(file_path, "wb") as f:
-                for chunk in r.iter_content(chunk_size=8192):
-                    f.write(chunk)
-        if clip_url != "":
-            logging.info(f"[LLM] Downloading {model_name} CLIP...")
-            with requests.get(clip_url, stream=True, allow_redirects=True) as r:
-                with open(
-                    f"{models_dir}/{model_name}/mmproj-model-f16.gguf", "wb"
-                ) as f:
-                    for chunk in r.iter_content(chunk_size=8192):
-                        f.write(chunk)
+    if os.path.exists(f"{models_dir}/{filename}"):
+        return f"{models_dir}/{filename}"
+    try:
+        file_path = hf_hub_download(
+            repo_id=model_name,
+            filename=filename,
+            local_dir=models_dir,
+            local_dir_use_symlinks=False,
+        )
+    except:
+        filename = model + f".q4_k_m.gguf"
+        file_path = hf_hub_download(
+            repo_id=model_name,
+            filename=filename,
+            local_dir=models_dir,
+            local_dir_use_symlinks=False,
+        )
     return file_path
 
 
 def get_clip_path(model_name="", models_dir="models"):
     if model_name == "":
         global DEFAULT_MODEL
         model_name = DEFAULT_MODEL
-    model_name = model_name.lower()
     if os.path.exists(f"{models_dir}/{model_name}/mmproj-model-f16.gguf"):
         return f"{models_dir}/{model_name}/mmproj-model-f16.gguf"
     else:
         return ""
 
 
 def clean(
@@ -139,14 +111,17 @@
         "<|im_end|>",
         "</|im_end|>",
         "</s>",
         "<s>",
         "User:",
         "### \n###",
         "[/INST]",
+        "<|eot_id|>",
+        "<|end_of_text|>",
+        "assistant\n\n",
     ],
 ):
     if message == "":
         return message
     for token in stop_tokens:
         if token in message:
             message = message.split(token)[0]
@@ -155,14 +130,16 @@
         message = message[3:]
     if message.endswith("\n\n"):
         message = message[:-4]
     if message.startswith(" "):
         message = message[1:]
     if message.endswith("\n"):
         message = message[:-3]
+    if "[Insert " in message:
+        message = re.sub(r"\[Insert.*?\]", "", message)
     return message
 
 
 class LLM:
     def __init__(
         self,
         stop: List[str] = [],
@@ -228,14 +205,17 @@
             "<|im_end|>",
             "</|im_end|>",
             "</s>",
             "<s>",
             "User:",
             "### \n###",
             "[/INST]",
+            "<|eot_id|>",
+            "<|end_of_text|>",
+            "assistant\n\n",
         ]
         if stop != []:
             if isinstance(stop, str):
                 self.params["stop"].append(stop)
             else:
                 try:
                     for stop_string in stop:
@@ -259,19 +239,18 @@
         self.params["n_gpu_layers"] = int(GPU_LAYERS) if GPU_LAYERS else 0
         self.params["main_gpu"] = int(MAIN_GPU) if MAIN_GPU else 0
         if "batch_size" in kwargs:
             self.params["n_batch"] = (
                 int(kwargs["batch_size"]) if kwargs["batch_size"] else 1024
             )
         else:
-            self.params["n_batch"] = 1024
+            self.params["n_batch"] = int(os.environ.get("LLM_BATCH_SIZE", 1024))
         if self.model_name != "":
             self.lcpp = Llama(
                 **self.params,
-                embedding=True,
                 chat_handler=chat_handler,
                 logits_all=True if chat_handler else False,
             )
         else:
             self.lcpp = None
         self.model_list = get_models()
 
@@ -364,23 +343,14 @@
         data = self.generate(prompt=user_input, **kwargs)
         data["choices"][0]["message"]["content"] = clean(
             message=data["choices"][0]["message"]["content"],
             stop_tokens=self.params["stop"],
         )
         return data
 
-    def embedding(self, input):
-        embeddings = self.lcpp.create_embedding(input=input, model=self.model_name)
-        embeddings["model"] = self.model_name
-        return embeddings
-
     def models(self):
-        model_list = []
-        for model in self.model_list:
-            for key in model:
-                model_list.append(key)
-        return model_list
+        return self.model_list
 
 
 if __name__ == "__main__":
     logging.info(f"[LLM] Downloading {DEFAULT_MODEL} model...")
     download_llm(model_name=DEFAULT_MODEL, models_dir="models")
```

### Comparing `ezlocalai-0.1.7/ezlocalai/STT.py` & `ezlocalai-0.1.8/ezlocalai/STT.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.7/ezlocalai/VLM.py` & `ezlocalai-0.1.8/ezlocalai/VLM.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,17 @@
     VLChatProcessor = None
 from transformers import AutoModelForCausalLM
 from datetime import datetime
 import requests
 import torch
 import PIL.Image
 import uuid
-import tiktoken
 import os
 import base64
-
-
-def get_tokens(text: str) -> int:
-    encoding = tiktoken.get_encoding("cl100k_base")
-    num_tokens = len(encoding.encode(text))
-    return num_tokens
+from ezlocalai.Helpers import get_tokens
 
 
 class VLM:
     def __init__(self, model="deepseek-ai/deepseek-vl-1.3b-chat"):
         self.model = model.split("/")[-1]
         self.params = {}
         os.makedirs(os.path.join(os.getcwd(), "outputs"), exist_ok=True)
@@ -90,15 +84,15 @@
         outputs = self.vl_gpt.language_model.generate(
             inputs_embeds=inputs_embeds,
             attention_mask=prepare_inputs.attention_mask,
             pad_token_id=self.tokenizer.eos_token_id,
             bos_token_id=self.tokenizer.bos_token_id,
             eos_token_id=self.tokenizer.eos_token_id,
             max_new_tokens=(
-                512 if "max_tokens" not in kwargs else int(kwargs["max_tokens"])
+                1024 if "max_tokens" not in kwargs else int(kwargs["max_tokens"])
             ),
             do_sample=False,
             use_cache=True,
         )
         answer = self.tokenizer.decode(
             outputs[0].cpu().tolist(), skip_special_tokens=True
         )
@@ -171,21 +165,12 @@
             },
         ]
         response = self.chat(
             messages=messages,
         )
         return response["choices"][0]["message"]["content"]
 
-    def embedding(self, input):
-        tokens = get_tokens(input)
-        return {
-            "object": "list",
-            "data": [{"object": "embedding", "index": 0, "embedding": []}],
-            "model": self.model,
-            "usage": {"prompt_tokens": tokens, "total_tokens": tokens},
-        }
-
     def models(self):
         return [
             "deepseek-ai/deepseek-vl-1.3b-chat",
             "deepseek-ai/deepseek-vl-7b-chat",
         ]
```

### Comparing `ezlocalai-0.1.7/ezlocalai-ngrok.ipynb` & `ezlocalai-0.1.8/ezlocalai-ngrok.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955770502645502%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'Set Runtime Python 3 with T4 GPU or higher.\\n')], "*

 * *            "delete: [4]}}, 1: {'source': {insert: [(1, '!pip install -qq scipy ftfy accelerate "*

 * *            'fastapi uvicorn pydantic requests tiktoken python-dotenv beautifulsoup4 '*

 * *            'faster-whisper pydub ffmpeg TTS sounddevice pyaudio webrtcvad pyngrok pdfplumber '*

 * *            "spacy python-multipart\\n')], delete: [1]}}, 2: {'source': {insert: [(6, 'Set the "*

 * *            '`LLM_TO_USE` with the nam […]*

```diff
@@ -4,27 +4,27 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# ezlocalai\n",
                 "\n",
                 "Open this notebook in [Google Colab.](https://colab.research.google.com/)\n",
                 "\n",
-                "Set the resources to T4 GPU, free tier.\n",
+                "Set Runtime Python 3 with T4 GPU or higher.\n",
                 "\n",
                 "It takes several minutes to install dependencies.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "!apt install -y portaudio19-dev ffmpeg libportaudio2 libasound-dev\n",
-                "!pip install -qq scipy ftfy accelerate fastapi uvicorn pydantic requests tiktoken python-dotenv beautifulsoup4 faster-whisper pydub ffmpeg TTS sounddevice pyaudio webrtcvad pyngrok\n",
+                "!pip install -qq scipy ftfy accelerate fastapi uvicorn pydantic requests tiktoken python-dotenv beautifulsoup4 faster-whisper pydub ffmpeg TTS sounddevice pyaudio webrtcvad pyngrok pdfplumber spacy python-multipart\n",
                 "!pip install -qq diffusers[\"torch\"] transformers torch torchvision torchaudio\n",
                 "!CMAKE_ARGS=\"-DLLAMA_CUBLAS=on\" FORCE_CMAKE=1 pip install llama-cpp-python\n",
                 "!rm -rf sample_data .config\n",
                 "!git clone https://github.com/DevXT-LLC/ezlocalai ."
             ]
         },
         {
@@ -33,41 +33,45 @@
             "source": [
                 "## Start the server\n",
                 "\n",
                 "Set the `NGROK_TOKEN` to use NGROK to expose your ezlocalai server to the public with as simple as an API key. [Get your free NGROK_TOKEN here.](https://dashboard.ngrok.com/get-started/your-authtoken)\n",
                 "\n",
                 "You can see the ngrok URL in the cell output after running the cell.\n",
                 "\n",
-                "Set the `LLM_TO_USE` with the name of the model from the models list. We will use `phi-2-dpo` for this example since it is a smaller model that can still be useful.\n"
+                "Set the `LLM_TO_USE` with the name of the model from the models list. We will use `Mistral-7B-Instruct-v0.2` for this example since it is a smaller model that can still be useful.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "LLM_TO_USE = \"phi-2-dpo\"\n",
+                "LLM_TO_USE = \"TheBloke/Mistral-7B-Instruct-v0.2-GGUF\"\n",
+                "VISION_MODEL = \"deepseek-ai/deepseek-vl-1.3b-chat\"\n",
                 "GPU_LAYERS = 10\n",
+                "LLM_MAX_TOKENS = 16384\n",
                 "\n",
                 "# Add your NGROK_TOKEN to your colab secrets if using Google Colab (Key logo on the left)\n",
                 "try:\n",
                 "    from google.colab import userdata\n",
                 "    NGROK_TOKEN = userdata.get('NGROK_TOKEN')\n",
                 "    if not NGROK_TOKEN:\n",
                 "        raise\n",
                 "except:\n",
                 "    # If you're not using Google Colab, enter your NGROK_TOKEN below.\n",
                 "    NGROK_TOKEN = \"Enter your ngrok token here\"\n",
                 "if NGROK_TOKEN != \"Enter your ngrok token here\":\n",
                 "    with open('.env', 'r') as file:\n",
                 "        filedata = file.read()\n",
                 "    filedata = filedata.replace('NGROK_TOKEN=\\n', f'NGROK_TOKEN={NGROK_TOKEN}\\n')\n",
-                "    filedata = filedata.replace('DEFAULT_MODEL=phi-2-dpo', f'DEFAULT_MODEL={LLM_TO_USE}')\n",
+                "    filedata = filedata.replace('DEFAULT_MODEL=TheBloke/phi-2-dpo-GGUF', f'DEFAULT_MODEL={LLM_TO_USE}')\n",
                 "    filedata = filedata.replace('GPU_LAYERS=0', f'GPU_LAYERS={GPU_LAYERS}')\n",
+                "    filedata = filedata.replace('LLM_MAX_TOKENS=0', f'LLM_MAX_TOKENS={LLM_MAX_TOKENS}')\n",
+                "    filedata = filedata.replace('VISION_MODEL=', f'VISION_MODEL={VISION_MODEL}')\n",
                 "    with open('.env', 'w') as file:\n",
                 "        file.write(filedata)\n",
                 "!uvicorn app:app --host 0.0.0.0 --port 8091 --workers 1 --proxy-headers"
             ]
         }
     ],
     "metadata": {
```

### Comparing `ezlocalai-0.1.7/ezlocalai.egg-info/PKG-INFO` & `ezlocalai-0.1.8/ezlocalai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: ezlocalai
-Version: 0.1.7
+Version: 0.1.8
 Summary: ezlocalai is an easy to set up local artificial intelligence server with OpenAI Style Endpoints.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: streamlit
-Requires-Dist: pydantic==2.6.3
+Requires-Dist: pydantic
 Requires-Dist: requests==2.31.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: faster-whisper==1.0.1
 Requires-Dist: pydub==0.25.1
 Requires-Dist: ffmpeg-python==0.2.0
-Requires-Dist: torch==2.2.1
-Requires-Dist: torchaudio==2.2.1
-Requires-Dist: transformers==4.38.2
+Requires-Dist: torch==2.3.0
+Requires-Dist: torchaudio==2.3.0
+Requires-Dist: transformers
 Requires-Dist: TTS==0.22.0
 Requires-Dist: sounddevice==0.4.6
 Requires-Dist: pyaudio==0.2.14
 Requires-Dist: webrtcvad==2.0.10
-Requires-Dist: pyngrok==7.1.5
-Requires-Dist: accelerate==0.27.2
+Requires-Dist: pyngrok==7.1.6
+Requires-Dist: accelerate
 Requires-Dist: python-multipart
-Requires-Dist: llama-cpp-python==0.2.55
+Requires-Dist: llama-cpp-python
 Requires-Dist: openai
+Requires-Dist: pdfplumber
+Requires-Dist: spacy
+Requires-Dist: optimum
+Requires-Dist: onnx
 
 # ezlocalai
 
 [![GitHub](https://img.shields.io/badge/GitHub-ezLocalai-blue?logo=github&style=plastic)](https://github.com/DevXT-LLC/ezlocalai) [![Dockerhub](https://img.shields.io/badge/Docker-ezlocalai-blue?logo=docker&style=plastic)](https://hub.docker.com/r/joshxt/ezlocalai)
 
 ezlocalai is an easy set up artificial intelligence server that allows you to easily run multimodal artificial intelligence from your computer. It is designed to be as easy as possible to get started with running local models. It automatically handles downloading the model of your choice and configuring the server based on your CPU, RAM, and GPU specifications. It also includes [OpenAI Style](https://pypi.org/project/openai/) endpoints for easy integration with other applications using ezlocalai as an OpenAI API proxy with any model. Additional functionality is built in for voice cloning text to speech and a voice to text for easy voice communication as well as image generation entirely offline after the initial setup.
 
 ## Prerequisites
 
 - [Git](https://git-scm.com/downloads)
-- [PowerShell 7.X](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.4)
 - [Docker Desktop](https://docs.docker.com/docker-for-windows/install/) (Windows or Mac)
 - [CUDA Toolkit](https://developer.nvidia.com/cuda-downloads) (NVIDIA GPU only)
 
 <details>
   <summary>Additional Linux Prerequisites</summary>
 
 - [Docker](https://docs.docker.com/get-docker/)
@@ -72,65 +75,51 @@
 Modify the `.env` file to your desired settings. Assumptions will be made on all of these values if you choose to accept the defaults.
 
 Replace the environment variables with your desired settings. Assumptions will be made on all of these values if you choose to accept the defaults.
 
 - `EZLOCALAI_URL` - The URL to use for the server. Default is `http://localhost:8091`.
 - `EZLOCALAI_API_KEY` - The API key to use for the server. If not set, the server will not require an API key when accepting requests.
 - `NGROK_TOKEN` - The ngrok token to use for the server. If not set, ngrok will not be used. Using ngrok will allow you to expose your ezlocalai server to the public with as simple as an API key. [Get your free NGROK_TOKEN here.](https://dashboard.ngrok.com/get-started/your-authtoken)
-- `DEFAULT_MODEL` - The default model to use when no model is specified. Default is `phi-2-dpo`.
+- `DEFAULT_MODEL` - The default model to use when no model is specified. Use the Hugging Face path. Default is `TheBloke/phi-2-dpo-GGUF`.
 - `LLM_MAX_TOKENS` - The maximum number of tokens to use for the language model. If set to `0`, it will automatically use the max tokens for the model. Default is `0`.
 - `WHISPER_MODEL` - The model to use for speech-to-text. Default is `base.en`.
 - `AUTO_UPDATE` - Whether or not to automatically update ezlocalai. Default is `true`.
 - `THREADS` - The number of CPU threads ezlocalai is allowed to use. Default is 4.
 - `GPU_LAYERS` (Only applicable to NVIDIA GPU) - The number of layers to use on the GPU. Default is `0`. Your `GPU_LAYERS` will automatically determine a number of layers to use based on your GPU's memory if it is set to `-1` and you have an NVIDIA GPU. If it is set to `-2`, it will use the maximum number of layers requested by the model.
 - `MAIN_GPU` (Only applicable to NVIDIA GPU) - The GPU to use for the language model. Default is `0`.
 - `IMG_ENABLED` - If set to true, models will choose to generate images when they want to based on the user input. **This is only available on GPU.** Default is `false`.
 - `SD_MODEL` - The stable diffusion model to use. Default is `stabilityai/sdxl-turbo`.
+- `VISION_MODEL` - The vision model to use. Default is None. Current options are `deepseek-ai/deepseek-vl-1.3b-chat` and `deepseek-ai/deepseek-vl-7b-chat`.
 
 </details>
 
 ## Usage
 
-```bash
-./start.ps1
-```
-
-Linux:
+### NVIDIA GPU
 
 ```bash
-sudo pwsh start.ps1
+docker-compose -f docker-compose-cuda.yml down
+docker-compose -f docker-compose-cuda.yml build
+docker-compose -f docker-compose-cuda.yml up
 ```
 
-### Deepseek VL Vision Models
-
-- <https://huggingface.co/deepseek-ai/deepseek-vl-1.3b-chat> (Default)
-- <https://huggingface.co/deepseek-ai/deepseek-vl-7b-chat>
-
-Functionality and endpoint request/response directly mimics the [OpenAI gpt-4-vision API](https://platform.openai.com/docs/guides/vision).
-
-**Only currently available with CUDA GPU.**
-
-Modify `deepseek.yml` if you want to run the 7b model instead of the 1.3b model or want to change any other settings. This also has image generation enabled by default, you can disable it by changing `IMG_ENABLED` to `false` in `deepseek.yml` to reduce video RAM usage. This configuration will fit on a ~16GB GPU.
+### CPU
 
 ```bash
-.\deepseek.ps1
+docker-compose down
+docker-compose build
+docker-compose up
 ```
 
-Linux:
-
-```bash
-sudo pwsh deepseek.ps1
-```
-
-For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb).
-
 ## OpenAI Style Endpoint Usage
 
 OpenAI Style endpoints available at `http://<YOUR LOCAL IP ADDRESS>:8091/v1/` by default. Documentation can be accessed at that <http://localhost:8091> when the server is running.
 
+For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb) once the server is running.
+
 ## Demo UI
 
 You can access the basic demo UI at <http://localhost:8502>, or your local IP address with port 8502.
 
 ## Workflow
 
 ```mermaid
```

### Comparing `ezlocalai-0.1.7/ezlocalai.egg-info/SOURCES.txt` & `ezlocalai-0.1.8/ezlocalai.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 LICENSE
 MANIFEST.in
 Pipes.py
 README.md
 app.py
 cuda-requirements.txt
 cuda.Dockerfile
-cuda118-requirements.txt
 deepseek.ps1
 deepseek.yml
+dev.yml
 docker-compose-cuda.yml
-docker-compose-vulkan.yml
 docker-compose.yml
 ezlocalai-ngrok.ipynb
 pyproject.toml
 requirements.txt
 setup.py
 start.ps1
 tests.ipynb
 ui.py
-vulkan.Dockerfile
 ezlocalai/CTTS.py
+ezlocalai/Embedding.py
+ezlocalai/Helpers.py
 ezlocalai/IMG.py
 ezlocalai/LLM.py
 ezlocalai/STT.py
 ezlocalai/VLM.py
 ezlocalai/__init__.py
 ezlocalai.egg-info/PKG-INFO
 ezlocalai.egg-info/SOURCES.txt
```

### Comparing `ezlocalai-0.1.7/setup.py` & `ezlocalai-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 
 with open(os.path.join(this_directory, "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ezlocalai",
-    version="0.1.7",
+    version="0.1.8",
     description="ezlocalai is an easy to set up local artificial intelligence server with OpenAI Style Endpoints.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     packages=find_packages(),
     python_requires=">=3.10",
```

### Comparing `ezlocalai-0.1.7/start.ps1` & `ezlocalai-0.1.8/start.ps1`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.7/tests.ipynb` & `ezlocalai-0.1.8/tests.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999844333748443%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(18, \'DEFAULT_LLM = os.getenv("DEFAULT_LLM", '*

 * *            '"TheBloke/phi-2-dpo-GGUF")\\n\')], delete: [18]}}}'}*

```diff
@@ -41,15 +41,15 @@
                 "DEFAULT_MAX_TOKENS = 256\n",
                 "DEFAULT_TEMPERATURE = 0.5\n",
                 "DEFAULT_TOP_P = 0.9\n",
                 "\n",
                 "# ------------------- DO NOT EDIT BELOW THIS LINE IN THIS CELL ------------------- #\n",
                 "EZLOCALAI_SERVER = os.getenv(\"EZLOCALAI_URL\", \"http://localhost:8091\")\n",
                 "EZLOCALAI_API_KEY = os.getenv(\"EZLOCALAI_API_KEY\", \"none\")\n",
-                "DEFAULT_LLM = os.getenv(\"DEFAULT_LLM\", \"phi-2-dpo\")\n",
+                "DEFAULT_LLM = os.getenv(\"DEFAULT_LLM\", \"TheBloke/phi-2-dpo-GGUF\")\n",
                 "openai.base_url = f\"{EZLOCALAI_SERVER}/v1/\"\n",
                 "openai.api_key = EZLOCALAI_API_KEY if EZLOCALAI_API_KEY else EZLOCALAI_SERVER\n",
                 "HEADERS = {\n",
                 "    \"Content-Type\": \"application/json\",\n",
                 "    \"Authorization\": f\"{EZLOCALAI_API_KEY}\",\n",
                 "    \"ngrok-skip-browser-warning\": \"true\",\n",
                 "}\n",
```

### Comparing `ezlocalai-0.1.7/ui.py` & `ezlocalai-0.1.8/ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,56 +2,66 @@
 import openai
 import requests
 import base64
 import os
 import re
 from datetime import datetime
 from dotenv import load_dotenv
+import time
 
 load_dotenv()
 # Show logo but resize to the screen https://devxt.com/wp-content/uploads/2023/01/Logo-1024x316.png
 st.image(
     "https://devxt.com/wp-content/uploads/2023/01/Logo-1024x316.png",
     width=300,
 )
 
-
 EZLOCALAI_SERVER = os.getenv("EZLOCALAI_URL", "http://localhost:8091")
 EZLOCALAI_API_KEY = os.getenv("EZLOCALAI_API_KEY", "none")
-DEFAULT_LLM = os.getenv("DEFAULT_LLM", "phi-2-dpo")
-VISION_MODEL = os.getenv("VISION_MODEL", "")
-if VISION_MODEL != "":
-    DEFAULT_LLM = VISION_MODEL
+DEFAULT_LLM = os.getenv("DEFAULT_MODEL", "TheBloke/phi-2-dpo-GGUF")
+VISION_MODEL = os.getenv("VISION_MODEL", None)
+SD_MODEL = os.getenv("SD_MODEL", "stabilityai/sdxl-turbo")
+IMG_ENABLED = os.getenv("IMG_ENABLED", "false")
+WHISPER_MODEL = os.getenv("WHISPER_MODEL", "base.en")
+
 if "/" in DEFAULT_LLM:
     link_to_model = f"https://huggingface.co/{DEFAULT_LLM}"
 else:
     link_to_model = f"https://huggingface.co/models?search={DEFAULT_LLM}"
 st.markdown(
     f"""
     [![GitHub](https://img.shields.io/badge/GitHub-ezLocalai-blue?logo=github&style=plastic)](https://github.com/DevXT-LLC/ezlocalai) [![Dockerhub](https://img.shields.io/badge/Docker-ezlocalai-blue?logo=docker&style=plastic)](https://hub.docker.com/r/joshxt/ezlocalai)
     ## ezLocal.ai Demo
-    **Current model:** [{DEFAULT_LLM}]({link_to_model})
+    **Language model:** [{DEFAULT_LLM}]({link_to_model})
     """
 )
-
-EZLOCALAI_SERVER = os.getenv("EZLOCALAI_URL", "http://localhost:8091")
-EZLOCALAI_API_KEY = os.getenv("EZLOCALAI_API_KEY", "none")
-DEFAULT_LLM = os.getenv("DEFAULT_LLM", "phi-2-dpo")
+if VISION_MODEL:
+    st.markdown(
+        f"""
+        **Vision model:** [{VISION_MODEL}](https://huggingface.co/{VISION_MODEL})
+        """
+    )
+if IMG_ENABLED.lower() == "true":
+    st.markdown(
+        f"""
+        **Image Generation model:** [{SD_MODEL}](https://huggingface.co/{SD_MODEL})
+        """
+    )
 openai.base_url = f"{EZLOCALAI_SERVER}/v1/"
 openai.api_key = EZLOCALAI_API_KEY if EZLOCALAI_API_KEY else EZLOCALAI_SERVER
 HEADERS = {
     "Content-Type": "application/json",
     "Authorization": f"{EZLOCALAI_API_KEY}",
     "ngrok-skip-browser-warning": "true",
 }
 waiting_for_server = False
 
 
 def get_voices():
-    return ["DukeNukem", "HAL9000"]
+    return ["Morgan_Freeman", "DukeNukem", "HAL9000"]
     # Commented for speed, but this works if we want to get the voices from the server
     """
     global EZLOCALAI_SERVER
     global HEADERS
     global waiting_for_server
     while True:
         try:
@@ -131,14 +141,15 @@
     voice_drop_down = st.selectbox(
         "Text-to-Speech Response Voice", ["None"] + get_voices(), index=0
     )
     uploaded_file = st.file_uploader("Upload an image")
     prompt = st.text_area("Your Message:", "Describe each stage of this image.")
     send = st.form_submit_button("Send")
     if prompt != "" and send:
+        start_time = time.time()
         st.markdown("---")
         st.spinner("Thinking...")
         messages = []
         if SYSTEM_MESSAGE != "":
             messages.append({"role": "system", "content": SYSTEM_MESSAGE})
         if uploaded_file:
             messages.append(
@@ -168,8 +179,17 @@
             temperature=DEFAULT_TEMPERATURE,
             max_tokens=DEFAULT_MAX_TOKENS,
             top_p=DEFAULT_TOP_P,
             stream=False,
             extra_body=extra_body,
         )
         display_content(response.choices[0].message.content)
+        end_time = time.time()  # Record the end time
+        elapsed_time = end_time - start_time
+        # If response time is longer than 60 seconds, split the response time into minutes and seconds
+        if elapsed_time > 60:
+            minutes = int(elapsed_time // 60)
+            seconds = elapsed_time % 60
+            st.success(f"Response time: {minutes} minutes and {seconds:.2f} seconds")
+        else:
+            st.success(f"Response time: {elapsed_time:.2f} seconds")
         st.balloons()
```

