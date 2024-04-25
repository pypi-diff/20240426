# Comparing `tmp/echowarp-0.2.8-py3-none-any.whl.zip` & `tmp/echowarp-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,28 @@
-Zip file size: 5639 bytes, number of entries: 9
--rw-r--r--  2.0 unx      477 b- defN 24-Apr-24 21:53 echowarp/__init__.py
--rw-r--r--  2.0 unx      603 b- defN 24-Apr-24 21:53 echowarp/logging_config.py
--rw-r--r--  2.0 unx     2297 b- defN 24-Apr-24 21:53 echowarp/main.py
--rw-r--r--  2.0 unx     2470 b- defN 24-Apr-24 21:53 echowarp/settings.py
--rw-r--r--  2.0 unx     4454 b- defN 24-Apr-24 21:53 echowarp-0.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 21:53 echowarp-0.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Apr-24 21:53 echowarp-0.2.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-24 21:53 echowarp-0.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      705 b- defN 24-Apr-24 21:53 echowarp-0.2.8.dist-info/RECORD
-9 files, 11159 bytes uncompressed, 4423 bytes compressed:  60.4%
+Zip file size: 26789 bytes, number of entries: 26
+-rw-r--r--  2.0 unx      477 b- defN 24-Apr-25 22:35 echowarp/__init__.py
+-rw-r--r--  2.0 unx      603 b- defN 24-Apr-25 22:35 echowarp/logging_config.py
+-rw-r--r--  2.0 unx     2297 b- defN 24-Apr-25 22:35 echowarp/main.py
+-rw-r--r--  2.0 unx     2470 b- defN 24-Apr-25 22:35 echowarp/settings.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 22:35 echowarp/auth_and_heartbeat/__init__.py
+-rw-r--r--  2.0 unx     7070 b- defN 24-Apr-25 22:35 echowarp/auth_and_heartbeat/transport_base.py
+-rw-r--r--  2.0 unx     6932 b- defN 24-Apr-25 22:35 echowarp/auth_and_heartbeat/transport_client.py
+-rw-r--r--  2.0 unx     7540 b- defN 24-Apr-25 22:35 echowarp/auth_and_heartbeat/transport_server.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 22:35 echowarp/models/__init__.py
+-rw-r--r--  2.0 unx     5480 b- defN 24-Apr-25 22:35 echowarp/models/audio_device.py
+-rw-r--r--  2.0 unx     3420 b- defN 24-Apr-25 22:35 echowarp/models/default_values_and_options.py
+-rw-r--r--  2.0 unx     6464 b- defN 24-Apr-25 22:35 echowarp/models/json_message.py
+-rw-r--r--  2.0 unx      579 b- defN 24-Apr-25 22:35 echowarp/models/options_data_creater.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 22:35 echowarp/services/__init__.py
+-rw-r--r--  2.0 unx     9205 b- defN 24-Apr-25 22:35 echowarp/services/crypto_manager.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 22:35 echowarp/start_modes/__init__.py
+-rw-r--r--  2.0 unx     3741 b- defN 24-Apr-25 22:35 echowarp/start_modes/args_mode.py
+-rw-r--r--  2.0 unx     6007 b- defN 24-Apr-25 22:35 echowarp/start_modes/interactive_mode.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 22:35 echowarp/streamer/__init__.py
+-rw-r--r--  2.0 unx     3815 b- defN 24-Apr-25 22:35 echowarp/streamer/audio_client.py
+-rw-r--r--  2.0 unx     3855 b- defN 24-Apr-25 22:35 echowarp/streamer/audio_server.py
+-rw-r--r--  2.0 unx     5782 b- defN 24-Apr-25 22:36 echowarp-0.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 22:36 echowarp-0.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-25 22:36 echowarp-0.2.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-25 22:36 echowarp-0.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2273 b- defN 24-Apr-25 22:36 echowarp-0.2.9.dist-info/RECORD
+26 files, 78163 bytes uncompressed, 23051 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -6,23 +6,74 @@
 
 Filename: echowarp/main.py
 Comment: 
 
 Filename: echowarp/settings.py
 Comment: 
 
-Filename: echowarp-0.2.8.dist-info/METADATA
+Filename: echowarp/auth_and_heartbeat/__init__.py
 Comment: 
 
-Filename: echowarp-0.2.8.dist-info/WHEEL
+Filename: echowarp/auth_and_heartbeat/transport_base.py
 Comment: 
 
-Filename: echowarp-0.2.8.dist-info/entry_points.txt
+Filename: echowarp/auth_and_heartbeat/transport_client.py
 Comment: 
 
-Filename: echowarp-0.2.8.dist-info/top_level.txt
+Filename: echowarp/auth_and_heartbeat/transport_server.py
 Comment: 
 
-Filename: echowarp-0.2.8.dist-info/RECORD
+Filename: echowarp/models/__init__.py
+Comment: 
+
+Filename: echowarp/models/audio_device.py
+Comment: 
+
+Filename: echowarp/models/default_values_and_options.py
+Comment: 
+
+Filename: echowarp/models/json_message.py
+Comment: 
+
+Filename: echowarp/models/options_data_creater.py
+Comment: 
+
+Filename: echowarp/services/__init__.py
+Comment: 
+
+Filename: echowarp/services/crypto_manager.py
+Comment: 
+
+Filename: echowarp/start_modes/__init__.py
+Comment: 
+
+Filename: echowarp/start_modes/args_mode.py
+Comment: 
+
+Filename: echowarp/start_modes/interactive_mode.py
+Comment: 
+
+Filename: echowarp/streamer/__init__.py
+Comment: 
+
+Filename: echowarp/streamer/audio_client.py
+Comment: 
+
+Filename: echowarp/streamer/audio_server.py
+Comment: 
+
+Filename: echowarp-0.2.9.dist-info/METADATA
+Comment: 
+
+Filename: echowarp-0.2.9.dist-info/WHEEL
+Comment: 
+
+Filename: echowarp-0.2.9.dist-info/entry_points.txt
+Comment: 
+
+Filename: echowarp-0.2.9.dist-info/top_level.txt
+Comment: 
+
+Filename: echowarp-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `echowarp-0.2.8.dist-info/METADATA` & `echowarp-0.2.9.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echowarp
-Version: 0.2.8
+Version: 0.2.9
 Summary: Network audio streaming tool using UDP
 Home-page: https://github.com/lHumaNl/EchoWarp
 Author: lHumaNl
 Author-email: fisher_sam@mail.ru
 License: MIT
 Keywords: audio streaming network
 Classifier: Development Status :: 3 - Alpha
@@ -37,20 +37,64 @@
 
 ## Prerequisites
 
 - **Operating System**: Windows, Linux, or macOS.
 - **Python Version**: Python 3.6 or later.
 - **Dependencies**: Includes libraries like PyAudio, and Cryptography.
 
-## Installation
+## PyPi Repository
+
+EchoWarp is also available as a package on the Python Package Index (PyPi), which simplifies the installation process
+and manages dependencies automatically. This is the recommended method if you wish to include EchoWarp in your Python
+project.
+
+### Features of Installing via PyPi:
+
+- **Automatic Dependency Management**: All required libraries, such as PyAudio and Cryptography, are automatically
+  installed.
+- **Easy Updates**: Simplifies the process of obtaining the latest version of EchoWarp with a simple pip command.
+- **Isolation from System Python**: Installing via a virtual environment prevents any conflicts with system-wide Python
+  packages.
+
+### Installation with PyPi (pip)
+
+To install EchoWarp using pip, follow these steps:
+
+1. Set up a Python virtual environment (optional but recommended):
+
+```bash
+   python -m venv .venv
+   source .venv/bin/activate  # On Windows, use `.\.venv\Scripts\activate`
+```
+
+2. Install EchoWarp using pip:
+
+```bash
+   pip install echowarp
+```
+
+### Updating EchoWarp
+
+To update to the latest version of EchoWarp, simply run:
+
+```bash
+   pip install --upgrade echowarp
+```
+
+This ensures that you have the latest features and improvements.
+
+For more information and assistance, you can visit the EchoWarp PyPi page:
+https://pypi.org/project/echowarp/
+
+## Installation from source
 
 Clone the repository and set up a Python virtual environment:
 
 ```bash
-git clone https://github.com/yourgithub/EchoWarp.git
+git clone https://github.com/lHumaNl/EchoWarp.git
 cd EchoWarp
 python -m venv venv
 source venv/bin/activate  # On Windows, use `.\venv\Scripts\activate`
 pip install -r requirements.txt
 ```
 
 ## Usage
```

