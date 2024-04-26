# Comparing `tmp/africanwhisper-0.9.0.tar.gz` & `tmp/africanwhisper-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.9.0.tar", last modified: Tue Apr 16 13:21:46 2024, max compression
+gzip compressed data, was "africanwhisper-0.9.1.tar", last modified: Fri Apr 26 18:33:56 2024, max compression
```

## Comparing `africanwhisper-0.9.0.tar` & `africanwhisper-0.9.1.tar`

### file list

```diff
@@ -1,33 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.667922 africanwhisper-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-16 13:21:46.667922 africanwhisper-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-16 13:21:46.667922 africanwhisper-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.663922 africanwhisper-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.667922 africanwhisper-0.9.0/src/africanwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-16 13:21:46.000000 africanwhisper-0.9.0/src/africanwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-16 13:21:46.000000 africanwhisper-0.9.0/src/africanwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:21:46.000000 africanwhisper-0.9.0/src/africanwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-16 13:21:46.000000 africanwhisper-0.9.0/src/africanwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 13:21:46.000000 africanwhisper-0.9.0/src/africanwhisper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.663922 africanwhisper-0.9.0/src/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/deployment/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/deployment/speech_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.663922 africanwhisper-0.9.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/tests/test_load_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.667922 africanwhisper-0.9.0/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/audio_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/gradio_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/gradio_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/wandb_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/whisper_model_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.398248 africanwhisper-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-04-26 18:33:56.398248 africanwhisper-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-26 18:33:56.398248 africanwhisper-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.390248 africanwhisper-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.394248 africanwhisper-0.9.1/src/africanwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-04-26 18:33:56.000000 africanwhisper-0.9.1/src/africanwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-26 18:33:56.000000 africanwhisper-0.9.1/src/africanwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:33:56.000000 africanwhisper-0.9.1/src/africanwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-26 18:33:56.000000 africanwhisper-0.9.1/src/africanwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 18:33:56.000000 africanwhisper-0.9.1/src/africanwhisper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.394248 africanwhisper-0.9.1/src/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/peft_speech_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/peft_speech_inference_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/speech_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/speech_inference_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/transcription_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.394248 africanwhisper-0.9.1/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_audio_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_model_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_transcription_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.394248 africanwhisper-0.9.1/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/audio_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/gradio_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/gradio_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/wandb_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/whisper_model_prep.py
```

### Comparing `africanwhisper-0.9.0/LICENSE` & `africanwhisper-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.0/PKG-INFO` & `africanwhisper-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.9.0
+Version: 0.9.1
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -27,16 +27,20 @@
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
 Requires-Dist: yt-dlp==2023.11.14
 Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: fastapi==0.110.1
-Requires-Dist: uvicorn==0.29.0
+Requires-Dist: faster-whisper==1.0.0
+Requires-Dist: pyannote.audio==3.1.1
+Requires-Dist: nltk==3.8.1
+Requires-Dist: torchvision==0.17.2
+Requires-Dist: ctranslate2==4.1.0
+Requires-Dist: pandas==2.2.1
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
@@ -266,35 +270,37 @@
 - To get the Gradio inference URL:
 ```bash
 python -m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE 
 ```
 - **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
 - **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
 
-- To launch the REST API endpoint locally:
 
 ```bash
 cd src/deployment
 ```
 - Create a `.env` file using `nano .env` command and add these keys and save the file.
 ```python
 MODEL_NAME = "your-finetuned-model"
 HUGGINGFACE_READ_TOKEN = "huggingface-read-token"
 ```
 
-- Run this command to launch the endpoint:
+- To perform transcriptions and translations:
+
 ```bash
-uvicorn main:app --host 0.0.0.0 --port 8000
-```
+# If your model is peft finetuned
+python -m deployment.peft_speech_inference_cli --audio_file audio-filename --task 
 
-- Test it out by accessing the Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or a .wav file and a task either `transcribe` or `translate`. Alternatively, you can use Postman with the URL `http://localhost:8000/speechinference`.
+# If your model is fully finetuned
+python -m deployment.speech_inference_cli --audio_file audio-filename --task task --perform_diarization --perform_alignment
+```
 
 ## 🛳️ Deployment
 
-- To deploy your fine-tuned model (assuming it's on Hugging Face Hub) as a REST API endpoint, follow these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
+- To deploy your fine-tuned model as a REST API endpoint, follow these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
 
 
 ## Contributing 
 Contributions are welcome and encouraged.
 
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.9.0 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.9.1 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
 jiwer==3.0.3 Requires-Dist: bitsandbytes==0.42.0 Requires-Dist:
 accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: numpy==1.26.4
 Requires-Dist: wandb==0.16.6 Requires-Dist: holoviews==1.18.3 Requires-Dist:
 panel==1.3.8 Requires-Dist: gradio==4.24.0 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0 Requires-Dist: tensorflow==2.16.1 Requires-
 Dist: keras==3.1.1 Requires-Dist: scipy==1.12.0 Requires-Dist: tensorflow-
 probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14 Requires-Dist: python-
-dotenv==1.0.1 Requires-Dist: fastapi==0.110.1 Requires-Dist: uvicorn==0.29.0
+dotenv==1.0.1 Requires-Dist: faster-whisper==1.0.0 Requires-Dist:
+pyannote.audio==3.1.1 Requires-Dist: nltk==3.8.1 Requires-Dist:
+torchvision==0.17.2 Requires-Dist: ctranslate2==4.1.0 Requires-Dist:
+pandas==2.2.1
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 *Enhancing Automatic Speech Recognition (ASR): translation and transcription
 capabilities for African languages by providing seamless fine-tuning and
 deploying pipelines for Whisper Model*.
 ![Diagram](diagram-1.png) ## Features - ð§ Fine-tune the [Whisper](https://
@@ -112,26 +115,25 @@
 ) choco install ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop
 install ffmpeg ``` - To get the Gradio inference URL: ```bash python -
 m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --
 huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE ``` - **--
 model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
 This should match the model's identifier on the Hugging Face Model Hub. - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face. - To
-launch the REST API endpoint locally: ```bash cd src/deployment ``` - Create a
-`.env` file using `nano .env` command and add these keys and save the file.
-```python MODEL_NAME = "your-finetuned-model" HUGGINGFACE_READ_TOKEN =
-"huggingface-read-token" ``` - Run this command to launch the endpoint: ```bash
-uvicorn main:app --host 0.0.0.0 --port 8000 ``` - Test it out by accessing the
-Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or
-a .wav file and a task either `transcribe` or `translate`. Alternatively, you
-can use Postman with the URL `http://localhost:8000/speechinference`. ##
-ð³ï¸ Deployment - To deploy your fine-tuned model (assuming it's on Hugging
-Face Hub) as a REST API endpoint, follow these [instructions](https://
-github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
+access. It allows you to download datasets and models from Hugging Face.
+```bash cd src/deployment ``` - Create a `.env` file using `nano .env` command
+and add these keys and save the file. ```python MODEL_NAME = "your-finetuned-
+model" HUGGINGFACE_READ_TOKEN = "huggingface-read-token" ``` - To perform
+transcriptions and translations: ```bash # If your model is peft finetuned
+python -m deployment.peft_speech_inference_cli --audio_file audio-filename --
+task # If your model is fully finetuned python -
+m deployment.speech_inference_cli --audio_file audio-filename --task task --
+perform_diarization --perform_alignment ``` ## ð³ï¸ Deployment - To deploy
+your fine-tuned model as a REST API endpoint, follow these [instructions]
+(https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
 Contributing Contributions are welcome and encouraged. Before contributing,
 please take a moment to review our [Contribution Guidelines](https://
 github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for
 important information on how to contribute to this project. If you're unsure
 about anything or need assistance, don't hesitate to reach out to us or open an
 issue to discuss your ideas. We look forward to your contributions! ## License
 This project is licensed under the MIT License - see the [LICENSE](https://
```

### Comparing `africanwhisper-0.9.0/README.md` & `africanwhisper-0.9.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -230,35 +230,37 @@
 - To get the Gradio inference URL:
 ```bash
 python -m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE 
 ```
 - **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
 - **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
 
-- To launch the REST API endpoint locally:
 
 ```bash
 cd src/deployment
 ```
 - Create a `.env` file using `nano .env` command and add these keys and save the file.
 ```python
 MODEL_NAME = "your-finetuned-model"
 HUGGINGFACE_READ_TOKEN = "huggingface-read-token"
 ```
 
-- Run this command to launch the endpoint:
+- To perform transcriptions and translations:
+
 ```bash
-uvicorn main:app --host 0.0.0.0 --port 8000
-```
+# If your model is peft finetuned
+python -m deployment.peft_speech_inference_cli --audio_file audio-filename --task 
 
-- Test it out by accessing the Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or a .wav file and a task either `transcribe` or `translate`. Alternatively, you can use Postman with the URL `http://localhost:8000/speechinference`.
+# If your model is fully finetuned
+python -m deployment.speech_inference_cli --audio_file audio-filename --task task --perform_diarization --perform_alignment
+```
 
 ## 🛳️ Deployment
 
-- To deploy your fine-tuned model (assuming it's on Hugging Face Hub) as a REST API endpoint, follow these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
+- To deploy your fine-tuned model as a REST API endpoint, follow these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
 
 
 ## Contributing 
 Contributions are welcome and encouraged.
 
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -96,26 +96,25 @@
 ) choco install ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop
 install ffmpeg ``` - To get the Gradio inference URL: ```bash python -
 m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --
 huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE ``` - **--
 model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
 This should match the model's identifier on the Hugging Face Model Hub. - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face. - To
-launch the REST API endpoint locally: ```bash cd src/deployment ``` - Create a
-`.env` file using `nano .env` command and add these keys and save the file.
-```python MODEL_NAME = "your-finetuned-model" HUGGINGFACE_READ_TOKEN =
-"huggingface-read-token" ``` - Run this command to launch the endpoint: ```bash
-uvicorn main:app --host 0.0.0.0 --port 8000 ``` - Test it out by accessing the
-Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or
-a .wav file and a task either `transcribe` or `translate`. Alternatively, you
-can use Postman with the URL `http://localhost:8000/speechinference`. ##
-ð³ï¸ Deployment - To deploy your fine-tuned model (assuming it's on Hugging
-Face Hub) as a REST API endpoint, follow these [instructions](https://
-github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
+access. It allows you to download datasets and models from Hugging Face.
+```bash cd src/deployment ``` - Create a `.env` file using `nano .env` command
+and add these keys and save the file. ```python MODEL_NAME = "your-finetuned-
+model" HUGGINGFACE_READ_TOKEN = "huggingface-read-token" ``` - To perform
+transcriptions and translations: ```bash # If your model is peft finetuned
+python -m deployment.peft_speech_inference_cli --audio_file audio-filename --
+task # If your model is fully finetuned python -
+m deployment.speech_inference_cli --audio_file audio-filename --task task --
+perform_diarization --perform_alignment ``` ## ð³ï¸ Deployment - To deploy
+your fine-tuned model as a REST API endpoint, follow these [instructions]
+(https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
 Contributing Contributions are welcome and encouraged. Before contributing,
 please take a moment to review our [Contribution Guidelines](https://
 github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for
 important information on how to contribute to this project. If you're unsure
 about anything or need assistance, don't hesitate to reach out to us or open an
 issue to discuss your ideas. We look forward to your contributions! ## License
 This project is licensed under the MIT License - see the [LICENSE](https://
```

### Comparing `africanwhisper-0.9.0/setup.cfg` & `africanwhisper-0.9.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = africanwhisper
 author = Kevin Kibe
-version = 0.9.0
+version = 0.9.1
 author_email = keviinkibe@gmail.com
 description = A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/African-Whisper
 license = MIT
 
@@ -31,16 +31,20 @@
 	tf-keras==2.16.0
 	tensorflow==2.16.1
 	keras==3.1.1
 	scipy==1.12.0
 	tensorflow-probability==0.24.0
 	yt-dlp==2023.11.14
 	python-dotenv==1.0.1
-	fastapi==0.110.1
-	uvicorn==0.29.0
+	faster-whisper==1.0.0
+	pyannote.audio==3.1.1
+	nltk==3.8.1
+	torchvision==0.17.2
+	ctranslate2==4.1.0
+	pandas==2.2.1
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `africanwhisper-0.9.0/src/africanwhisper.egg-info/PKG-INFO` & `africanwhisper-0.9.1/src/africanwhisper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.9.0
+Version: 0.9.1
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -27,16 +27,20 @@
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
 Requires-Dist: yt-dlp==2023.11.14
 Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: fastapi==0.110.1
-Requires-Dist: uvicorn==0.29.0
+Requires-Dist: faster-whisper==1.0.0
+Requires-Dist: pyannote.audio==3.1.1
+Requires-Dist: nltk==3.8.1
+Requires-Dist: torchvision==0.17.2
+Requires-Dist: ctranslate2==4.1.0
+Requires-Dist: pandas==2.2.1
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
@@ -266,35 +270,37 @@
 - To get the Gradio inference URL:
 ```bash
 python -m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE 
 ```
 - **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
 - **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
 
-- To launch the REST API endpoint locally:
 
 ```bash
 cd src/deployment
 ```
 - Create a `.env` file using `nano .env` command and add these keys and save the file.
 ```python
 MODEL_NAME = "your-finetuned-model"
 HUGGINGFACE_READ_TOKEN = "huggingface-read-token"
 ```
 
-- Run this command to launch the endpoint:
+- To perform transcriptions and translations:
+
 ```bash
-uvicorn main:app --host 0.0.0.0 --port 8000
-```
+# If your model is peft finetuned
+python -m deployment.peft_speech_inference_cli --audio_file audio-filename --task 
 
-- Test it out by accessing the Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or a .wav file and a task either `transcribe` or `translate`. Alternatively, you can use Postman with the URL `http://localhost:8000/speechinference`.
+# If your model is fully finetuned
+python -m deployment.speech_inference_cli --audio_file audio-filename --task task --perform_diarization --perform_alignment
+```
 
 ## 🛳️ Deployment
 
-- To deploy your fine-tuned model (assuming it's on Hugging Face Hub) as a REST API endpoint, follow these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
+- To deploy your fine-tuned model as a REST API endpoint, follow these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
 
 
 ## Contributing 
 Contributions are welcome and encouraged.
 
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.9.0 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.9.1 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
 jiwer==3.0.3 Requires-Dist: bitsandbytes==0.42.0 Requires-Dist:
 accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: numpy==1.26.4
 Requires-Dist: wandb==0.16.6 Requires-Dist: holoviews==1.18.3 Requires-Dist:
 panel==1.3.8 Requires-Dist: gradio==4.24.0 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0 Requires-Dist: tensorflow==2.16.1 Requires-
 Dist: keras==3.1.1 Requires-Dist: scipy==1.12.0 Requires-Dist: tensorflow-
 probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14 Requires-Dist: python-
-dotenv==1.0.1 Requires-Dist: fastapi==0.110.1 Requires-Dist: uvicorn==0.29.0
+dotenv==1.0.1 Requires-Dist: faster-whisper==1.0.0 Requires-Dist:
+pyannote.audio==3.1.1 Requires-Dist: nltk==3.8.1 Requires-Dist:
+torchvision==0.17.2 Requires-Dist: ctranslate2==4.1.0 Requires-Dist:
+pandas==2.2.1
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 *Enhancing Automatic Speech Recognition (ASR): translation and transcription
 capabilities for African languages by providing seamless fine-tuning and
 deploying pipelines for Whisper Model*.
 ![Diagram](diagram-1.png) ## Features - ð§ Fine-tune the [Whisper](https://
@@ -112,26 +115,25 @@
 ) choco install ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop
 install ffmpeg ``` - To get the Gradio inference URL: ```bash python -
 m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --
 huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE ``` - **--
 model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
 This should match the model's identifier on the Hugging Face Model Hub. - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face. - To
-launch the REST API endpoint locally: ```bash cd src/deployment ``` - Create a
-`.env` file using `nano .env` command and add these keys and save the file.
-```python MODEL_NAME = "your-finetuned-model" HUGGINGFACE_READ_TOKEN =
-"huggingface-read-token" ``` - Run this command to launch the endpoint: ```bash
-uvicorn main:app --host 0.0.0.0 --port 8000 ``` - Test it out by accessing the
-Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or
-a .wav file and a task either `transcribe` or `translate`. Alternatively, you
-can use Postman with the URL `http://localhost:8000/speechinference`. ##
-ð³ï¸ Deployment - To deploy your fine-tuned model (assuming it's on Hugging
-Face Hub) as a REST API endpoint, follow these [instructions](https://
-github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
+access. It allows you to download datasets and models from Hugging Face.
+```bash cd src/deployment ``` - Create a `.env` file using `nano .env` command
+and add these keys and save the file. ```python MODEL_NAME = "your-finetuned-
+model" HUGGINGFACE_READ_TOKEN = "huggingface-read-token" ``` - To perform
+transcriptions and translations: ```bash # If your model is peft finetuned
+python -m deployment.peft_speech_inference_cli --audio_file audio-filename --
+task # If your model is fully finetuned python -
+m deployment.speech_inference_cli --audio_file audio-filename --task task --
+perform_diarization --perform_alignment ``` ## ð³ï¸ Deployment - To deploy
+your fine-tuned model as a REST API endpoint, follow these [instructions]
+(https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
 Contributing Contributions are welcome and encouraged. Before contributing,
 please take a moment to review our [Contribution Guidelines](https://
 github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for
 important information on how to contribute to this project. If you're unsure
 about anything or need assistance, don't hesitate to reach out to us or open an
 issue to discuss your ideas. We look forward to your contributions! ## License
 This project is licensed under the MIT License - see the [LICENSE](https://
```

### Comparing `africanwhisper-0.9.0/src/africanwhisper.egg-info/SOURCES.txt` & `africanwhisper-0.9.1/src/africanwhisper.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,18 +4,28 @@
 setup.cfg
 src/africanwhisper.egg-info/PKG-INFO
 src/africanwhisper.egg-info/SOURCES.txt
 src/africanwhisper.egg-info/dependency_links.txt
 src/africanwhisper.egg-info/requires.txt
 src/africanwhisper.egg-info/top_level.txt
 src/deployment/__init__.py
+src/deployment/app.py
 src/deployment/main.py
+src/deployment/peft_speech_inference.py
+src/deployment/peft_speech_inference_cli.py
 src/deployment/speech_inference.py
+src/deployment/speech_inference_cli.py
+src/deployment/transcription_model.py
 src/tests/__init__.py
+src/tests/test_audio_processor.py
+src/tests/test_data_prep.py
 src/tests/test_load_dataset.py
+src/tests/test_model_optimization.py
+src/tests/test_model_prep.py
+src/tests/test_transcription_pipeline.py
 src/training/__init__.py
 src/training/audio_data_processor.py
 src/training/collator.py
 src/training/data_prep.py
 src/training/evaluation.py
 src/training/gradio_demo.py
 src/training/gradio_inference.py
```

### Comparing `africanwhisper-0.9.0/src/deployment/main.py` & `africanwhisper-0.9.1/src/deployment/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 from fastapi import FastAPI, UploadFile, HTTPException, Response
 from pydantic import BaseModel
 import tempfile
-from speech_inference import SpeechInference
+from deployment.peft_speech_inference import SpeechInference
 import logging
 from dotenv import load_dotenv
 import uvicorn
 import time
 import prometheus_client
 from prometheus_client import Histogram, Counter
 load_dotenv()
 
 app = FastAPI(debug=True)
+# FOR PEFT FINETUNED MODELS
 
 request_time = Histogram('request_processing_seconds', 'Time spent processing request')
 request_count = prometheus_client.Counter("request_count", "number_of_requests")
 errors_counter = Counter('app_errors_total', 'Total number of errors in the application')
 successful_requests_counter = Counter('app_successful_requests_total', 'Total number of successful requests in the application')
 
 model_name = os.getenv("MODEL_NAME")
@@ -68,8 +69,8 @@
 
 @app.get("/metrics")
 def metrics():
     return Response(
         content = prometheus_client.generate_latest())
 
 if __name__ == "__main__":
-    uvicorn.run(app, host = "0.0.0.0", port = 8000)
+    uvicorn.run(app, host = "0.0.0.0", port = 8000)
```

### Comparing `africanwhisper-0.9.0/src/deployment/speech_inference.py` & `africanwhisper-0.9.1/src/deployment/peft_speech_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,12 +92,12 @@
         Returns:
             Transcription: The transcription output.
         """
         transcription = pipe(
                 input,
                 chunk_length_s=30,
                 batch_size=24,
-                return_timestamps=True,
+                return_timestamps="word",
                 generate_kwargs={"task": task}
             )
         transcription = Transcription(**transcription)
         return transcription
```

### Comparing `africanwhisper-0.9.0/src/tests/test_load_dataset.py` & `africanwhisper-0.9.1/src/tests/test_load_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,63 @@
 import unittest
 from training.load_data import Dataset
+# import os
+from dotenv import load_dotenv
+load_dotenv()
 
 class TestDatasetManager(unittest.TestCase):
+    """Test cases for the Dataset class."""
+
     def setUp(self):
+        """Set up an instance of Dataset for testing."""
         self.dataset_manager = Dataset(
-            huggingface_token="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",
+            huggingface_token="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",
             dataset_name="mozilla-foundation/common_voice_16_1",
-            language_abbr=["yi","ti"]
+            language_abbr=["yi", "ti"]
         )
 
     def test_load_dataset(self):
-        # Arrange
+        """Test loading the dataset and verifying its contents."""
         # Act
         data = self.dataset_manager.load_dataset()
+
         # Assert
-        self.assertIsNotNone(data)
-        self.assertTrue("train" in data)
-        self.assertTrue("test" in data)
+        self.assertIsNotNone(data, "The loaded dataset should not be None.")
+        self.assertIn("train", data, "The dataset should contain a 'train' split.")
+        self.assertIn("test", data, "The dataset should contain a 'test' split.")
 
     def test_count_examples(self):
+        """Test counting examples in a dataset."""
         # Arrange
         class MockDataset:
+            """A mock dataset class to simulate iteration."""
             def __iter__(self):
                 return iter(range(10))
+
         # Act
         count = self.dataset_manager.count_examples(MockDataset())
+
         # Assert
-        self.assertEqual(count, 10)
+        self.assertEqual(count, 10, "The count of examples should be equal to 10.")
 
     def test_dataset_structure(self):
+        """Test the structure of the loaded dataset."""
         # Arrange
-        expected_features = ['client_id', 'path', 'audio', 'sentence', 'up_votes', 'down_votes', 'age', 'gender', 'accent', 'locale', 'segment', 'variant']
+        expected_features = [
+            'client_id', 'path', 'audio', 'sentence', 'up_votes', 'down_votes',
+            'age', 'gender', 'accent', 'locale', 'segment', 'variant'
+        ]
+
         # Act
         dataset = self.dataset_manager.load_dataset()
+
         # Assert
+        # Check train dataset features
         train_features = list(dataset['train'].features.keys())
-        self.assertEqual(train_features, expected_features)
+        self.assertListEqual(train_features, expected_features, "The train dataset features should match the expected features.")
 
+        # Check test dataset features
         test_features = list(dataset['test'].features.keys())
-        self.assertEqual(test_features, expected_features)
+        self.assertListEqual(test_features, expected_features, "The test dataset features should match the expected features.")
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `africanwhisper-0.9.0/src/training/audio_data_processor.py` & `africanwhisper-0.9.1/src/training/audio_data_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 class AudioDataProcessor:
     """
     Processes audio datasets for use in whisper models, including cleaning and resampling.
 
     """
 
     def __init__(
-        self, dataset: DatasetDict, feature_extractor, tokenizer: PreTrainedTokenizer, feature_processor 
+        self, dataset: DatasetDict, feature_extractor, tokenizer: PreTrainedTokenizer, feature_processor
     ):
         """
         Initializes the DatasetProcessor with the dataset, feature extractor, and tokenizer.
 
         Parameters:
             dataset (DatasetDict): The dataset to process.
             feature_extractor (PreTrainedFeatureExtractor): The feature extractor for audio data.
             tokenizer (PreTrainedTokenizer): The tokenizer for text data.
         """
         self.dataset = dataset
         self.feature_extractor = feature_extractor
         self.tokenizer = tokenizer
         self.processor = feature_processor
-    
-    
+
+
     def resampled_dataset(self, sample: Dict[str, Any]) -> DatasetDict:
         """
         Resamples the audio data to the required sampling rate and extracts features using the feature extractor.
 
         Parameters:
             example (dict): A single sample from the dataset, containing 'audio' and 'sentence' keys.
 
@@ -47,8 +47,8 @@
 
         tokenized_sentence = self.tokenizer(sample["sentence"]).input_ids
 
         sample["input_features"] = audio_features
         sample["labels"] = tokenized_sentence
 
         return sample
-    
+
```

### Comparing `africanwhisper-0.9.0/src/training/collator.py` & `africanwhisper-0.9.1/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.0/src/training/data_prep.py` & `africanwhisper-0.9.1/src/training/data_prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                                          with the audio samples.
 
         Returns:
             DatasetDict: A dictionary containing the preprocessed 'train' and 'test' splits of the dataset,
                         ready for use in model training and evaluation. Each split has been cleaned and
                         processed to include only the necessary features for model input.
         """
-        
+
         dataset = self.data_loader.load_dataset()
         print(f"Training dataset size: {self.data_loader.count_examples(dataset['train'])}")
         print(f"Test dataset size: {self.data_loader.count_examples(dataset['test'])}")
         processor = AudioDataProcessor(dataset, feature_extractor, tokenizer, processor)
         dataset['train']= dataset['train'].map(processor.resampled_dataset, remove_columns=list(next(iter(dataset['train'])).keys()))
         dataset['test']= dataset['test'].map(processor.resampled_dataset)
         return dataset
```

### Comparing `africanwhisper-0.9.0/src/training/evaluation.py` & `africanwhisper-0.9.1/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.0/src/training/gradio_demo.py` & `africanwhisper-0.9.1/src/training/gradio_demo.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.0/src/training/gradio_inference.py` & `africanwhisper-0.9.1/src/training/gradio_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,60 +34,60 @@
 
     def transcribe(self, inputs, task):
         if inputs is None:
             raise gr.Error("No audio file submitted! Please upload or record an audio file before submitting your request.")
         text = self.pipe(
                         inputs,
                         chunk_length_s=30,
-                        batch_size=24, 
+                        batch_size=24,
                         return_timestamps=True,
                         generate_kwargs={"task": task}
                         )["text"]
         return  text
-    
+
     def _return_yt_html_embed(self, yt_url):
         video_id = yt_url.split("?v=")[-1]
         HTML_str = (
             f'<center> <iframe width="500" height="320" src="https://www.youtube.com/embed/{video_id}"> </iframe>'
             " </center>"
         )
         return HTML_str
 
     def download_yt_audio(self, yt_url, filename):
         YT_LENGTH_LIMIT_S = 3600
         info_loader = youtube_dl.YoutubeDL()
-        
+
         try:
             info = info_loader.extract_info(yt_url, download=False)
         except youtube_dl.utils.DownloadError as err:
             raise gr.Error(str(err))
-        
+
         file_length = info["duration_string"]
         file_h_m_s = file_length.split(":")
         file_h_m_s = [int(sub_length) for sub_length in file_h_m_s]
-        
+
         if len(file_h_m_s) == 1:
             file_h_m_s.insert(0, 0)
         if len(file_h_m_s) == 2:
             file_h_m_s.insert(0, 0)
         file_length_s = file_h_m_s[0] * 3600 + file_h_m_s[1] * 60 + file_h_m_s[2]
-        
+
         if file_length_s > YT_LENGTH_LIMIT_S:
             yt_length_limit_hms = time.strftime("%HH:%MM:%SS", time.gmtime(YT_LENGTH_LIMIT_S))
             file_length_hms = time.strftime("%HH:%MM:%SS", time.gmtime(file_length_s))
             raise gr.Error(f"Maximum YouTube length is {yt_length_limit_hms}, got {file_length_hms} YouTube video.")
-        
+
         ydl_opts = {"outtmpl": filename, "format": "worstvideo[ext=mp4]+bestaudio[ext=m4a]/best[ext=mp4]/best"}
-        
+
         with youtube_dl.YoutubeDL(ydl_opts) as ydl:
             try:
                 ydl.download([yt_url])
             except youtube_dl.utils.ExtractorError as err:
                 raise gr.Error(str(err))
-            
+
     def yt_transcribe(self, yt_url, task, max_filesize=75.0):
         BATCH_SIZE = 8
         html_embed_str = self._return_yt_html_embed(yt_url)
 
         with tempfile.TemporaryDirectory() as tmpdirname:
             filepath = os.path.join(tmpdirname, "video.mp4")
             self.download_yt_audio(yt_url, filepath)
```

### Comparing `africanwhisper-0.9.0/src/training/load_data.py` & `africanwhisper-0.9.1/src/training/load_data.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.0/src/training/main.py` & `africanwhisper-0.9.1/src/training/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "--dataset_name",
         type=str,
         default="mozilla-foundation/common_voice_16_1",
         help="Name of the dataset to be downloaded from Hugging Face.",
     )
     parser.add_argument(
         "--language_abbr",
-        nargs='+',  
+        nargs='+',
         required=True,
         help="Abbreviation(s) of the language(s) for the dataset.",
     )
     parser.add_argument(
         "--model_id",
         type=str,
         default="openai/whisper-small",
```

### Comparing `africanwhisper-0.9.0/src/training/model_trainer.py` & `africanwhisper-0.9.1/src/training/model_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,16 @@
         self.model_id = model_id
         self.tokenizer = tokenizer
         self.feature_processor = feature_processor
         self.feature_extractor = feature_extractor
         self.huggingface_write_token = huggingface_write_token
         self.use_peft = use_peft
         self.model_prep = WhisperModelPrep(
-            self.model_id, 
-            "transcribe", 
+            self.model_id,
+            "transcribe",
             self.use_peft
         )
 
     def compute_metrics(self, pred) -> dict:
         """
         Computes the Word Error Rate (WER) metric for the model predictions.
 
@@ -87,15 +87,15 @@
         )
         label_str = self.tokenizer.batch_decode(
             label_ids, skip_special_tokens=True, normalize=True
         )
         metric = evaluate.load("wer")
         wer = 100 * metric.compute(predictions=pred_str, references=label_str)
         return {"wer": wer}
-    
+
 
     def compute_spectrograms(self, example: Dict[str, Any]) -> Dict[str, Any]:
         """
         Computes spectrograms from audio waveform.
 
         Args:
             example (dict): A dictionary containing audio waveform data.
@@ -151,14 +151,17 @@
             eval_steps=25,
             logging_steps=25,
             load_best_model_at_end=True,
             metric_for_best_model="wer",
             greater_is_better=False,
             push_to_hub=True,
             hub_token=self.huggingface_write_token,
+            hub_strategy = "checkpoint",
+            save_safetensors = False,
+            resume_from_checkpoint  = "last-checkpoint",
             report_to="wandb",
             remove_unused_columns=False,
             ignore_data_skip=True,
         )
 
         eval_dataset = self.dataset["test"].map(self.compute_spectrograms)
```

### Comparing `africanwhisper-0.9.0/src/training/wandb_callback.py` & `africanwhisper-0.9.1/src/training/wandb_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         slider.jslink(hv_audio, value="time", bidirectional=True)
         slider.jslink(line_audio, value="glyph.location")
         slider.jslink(line_spec, value="glyph.location")
 
         time = np.linspace(0, audio_duration, num=len(audio_array))
         line_plot_hv = (
-            hv.Curve((time, audio_array), ["Time (s)", "amplitude"]).opts(
+        hv.Curve((time, audio_array), kdims=["Time (s)"], vdims=["amplitude"]).opts(
                 width=500, height=150, axiswise=True
             )
             * line_audio
         )
 
         hv_spec_gram = (
             hv.Image(
```

### Comparing `africanwhisper-0.9.0/src/training/whisper_model_prep.py` & `africanwhisper-0.9.1/src/training/whisper_model_prep.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,28 @@
         processing_task (str): Specific task for the Whisper model to execute.
 
     """
 
     def __init__(
         self,
         model_id: str,
-        # language_abbr: str,
         processing_task: str,
         use_peft: bool,
     ):
         """Sets up the dataset and configuration for processing with the Whisper model.
 
         Parameters
         ----------
             dataset (DatasetDict): The dataset to be prepared.
             model_id (str, optional): Whisper model identifier.
             language_code (str, optional): Dataset language ISO code.
             processing_task (str, optional): Task for the Whisper model.
 
         """
         self.model_id = model_id
-        # self.language_abbr = language_abbr
         self.processing_task = processing_task
         self.use_peft = use_peft
 
     def initialize_feature_extractor(self) -> WhisperFeatureExtractor:
         """Creates and retrieves a feature extractor based on the Whisper model.
 
         Returns
@@ -117,8 +115,8 @@
                 self.model_id
             )
             model.config.forced_decoder_ids = None
             model.config.suppress_tokens = []
             model.generation_config.language = "en"
             model.generation_config.task = "translate"
 
-        return model
+        return model
```

