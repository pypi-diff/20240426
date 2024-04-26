# Comparing `tmp/bestdori-api-0.2.0.tar.gz` & `tmp/bestdori-api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bestdori-api-0.2.0.tar", last modified: Wed Apr 24 14:38:04 2024, max compression
+gzip compressed data, was "bestdori-api-1.0.0.tar", last modified: Thu Apr 25 16:09:35 2024, max compression
```

## Comparing `bestdori-api-0.2.0.tar` & `bestdori-api-1.0.0.tar`

### file list

```diff
@@ -1,47 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.480966 bestdori-api-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-24 14:38:04.480966 bestdori-api-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.476966 bestdori-api-0.2.0/bestdori/
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.476966 bestdori-api-0.2.0/bestdori/ayachan/
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.476966 bestdori-api-0.2.0/bestdori/ayachan/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/utils/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/comics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/costumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/eventarchives.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/logincampaigns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/miracleticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/missions.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/player.py
--rw-r--r--   0 runner    (1001) docker     (127)    17948 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/post.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/songmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.476966 bestdori-api-0.2.0/bestdori/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/content.py
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.476966 bestdori-api-0.2.0/bestdori_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-24 14:38:04.000000 bestdori-api-0.2.0/bestdori_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-24 14:38:04.000000 bestdori-api-0.2.0/bestdori_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:38:04.000000 bestdori-api-0.2.0/bestdori_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 14:38:04.000000 bestdori-api-0.2.0/bestdori_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:38:04.480966 bestdori-api-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/bestdori/
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/bestdori/ayachan/
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/bestdori/ayachan/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/comics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/costumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/eventarchives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20223 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/logincampaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/miracleticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/missions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34492 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/songmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/bestdori/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22048 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/bestdori_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-25 16:09:34.000000 bestdori-api-1.0.0/bestdori_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-25 16:09:35.000000 bestdori-api-1.0.0/bestdori_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:09:34.000000 bestdori-api-1.0.0/bestdori_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 16:09:34.000000 bestdori-api-1.0.0/bestdori_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/setup.py
```

### Comparing `bestdori-api-0.2.0/LICENSE` & `bestdori-api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bestdori-api-0.2.0/PKG-INFO` & `bestdori-api-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori-api
-Version: 0.2.0
+Version: 1.0.0
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori-api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
         
@@ -34,50 +34,44 @@
         
         <a href="https://www.python.org/downloads/">
           <img src="https://img.shields.io/pypi/pyversions/bestdori-api" alt="Python Version">
         </a>
         
         </p>
         
-        > bestdori_api 已更名为 bestdori-api
-        > 若安装过之前的 `bestdori_api` 包，请使用指令
-        > ```bash
-        > pip uninstall bestdori_api
-        > ```
-        > 
-        > 卸载原 `bestdori_api` 包后，重新安装 `bestdori-api` 包
-        > 否则可能导致未知的冲突问题
+        > bestdori-api 现已全面支持同步与异步
+        > 异步使用方法与同步类似，可几乎无缝切换
         
         ## 简介
         
         这是一个用 Python 编写的调用 [Bestdori](https://bestdori.com/) 各种 API 与资源下载的库，大致包括了社区帖子的处理以及各种 [BanG Dream！少女乐团派对](https://zh.moegirl.org.cn/BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81) 游戏内资源的获取。
         **警告：此模块目前仍然亟待完善与测试，请不要将其当做一个稳定的库使用。**
         
         ### 目前已有的 API 与功能
         
         |API 类别|是否完善|支持的内容|
         |:-------|:-----:|:------|
-        |用户|👍|登录、查询、帖子获取、信息获取|
+        |用户|👍👍|登录、查询、帖子获取、信息获取|
         |帖子|👍|搜索、获取、发表、评论、喜欢|
         |谱面|👍|社区谱面获取、音源与封面获取、规整化、数据统计、格式互转|
-        |故事|👎👎|社区故事获取|
-        |角色|🤔|信息获取、资源获取|
-        |卡牌|👎|信息获取、资源获取|
-        |服装|👎👎|信息获取|
-        |活动|🤔|信息获取、资源获取|
-        |活动数据|👎|数据获取|
-        |招募|🤔|数据获取、资源获取|
-        |歌曲|🤔|信息获取、资源获取|
-        |歌曲 Meta|👎👎|数据获取|
-        |登录奖励|🤔|信息获取、资源获取|
-        |自选券|🤔|信息获取|
-        |漫画|🤔|信息获取、图片获取|
-        |任务|🤔|信息获取|
-        |ayachan|🤔|谱面分析、测试服上传、难度分析|
-        |其他资源|👎👎|仅小部分资源有单独获取|
+        |故事|👍|社区故事获取|
+        |角色|👍|信息获取、资源获取|
+        |卡牌|👍|信息获取、资源获取|
+        |服装|👍|信息获取|
+        |活动|👍|信息获取、资源获取|
+        |活动数据|👍|数据获取|
+        |招募|👍|数据获取、资源获取|
+        |歌曲|👍|信息获取、资源获取|
+        |歌曲 Meta|👍|数据获取|
+        |登录奖励|👍|信息获取、资源获取|
+        |自选券|👍|信息获取|
+        |漫画|👍👍|信息获取、图片获取|
+        |任务|👍|信息获取|
+        |ayachan|👍👍👍|谱面分析、测试服上传、难度分析|
+        |其他资源|👍|部分独立资源的单独获取|
         
         ## 快速使用
         
         以下将以获取社区自制谱面 [[FULL] 光の中へ](https://bestdori.com/community/charts/111533/WindowsSov8-FULL) 的信息为例。
         
         首先，使用以下指令安装本模块：
         ```bash
@@ -130,16 +124,18 @@
         如果想要获取这个自制谱面的谱面，或者想要获取它的音源与封面，以下代码将会进行获取：
         ```python
         from bestdori.post import Post
         
         def main() -> None:
             # 实例化 Post 类
             p = Post(id='111533')
-            # 调用方法获取谱面
-            chart = p.get_chart() # 获取的将是一个谱面实例
+            # 调用方法获取信息（所有属性化方法在使用前必须获取一次信息）
+            p.get_details()
+            # 通过属性获取谱面
+            chart = p.chart # 获取的将是一个谱面实例
             # 调用方法获取音源与封面
             info = p.get_song() # 获取的将是一个包含了音源与封面的 bytes 字典
         
         main()
         ```
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,41 +1,39 @@
-Metadata-Version: 2.1 Name: bestdori-api Version: 0.2.0 Summary: Bestdori
+Metadata-Version: 2.1 Name: bestdori-api Version: 1.0.0 Summary: Bestdori
 çåç§ API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ Home-page: https://
 github.com/WindowsSov8forUs/bestdori-api Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
                    æå¶ä»éè¦çæ¥å£è¯·åæ¶æåº**
           _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
-> bestdori_api å·²æ´åä¸º bestdori-api > è¥å®è£è¿ä¹åç `bestdori_api`
-åï¼è¯·ä½¿ç¨æä»¤ > ```bash > pip uninstall bestdori_api > ``` > >
-å¸è½½å `bestdori_api` ååï¼éæ°å®è£ `bestdori-api` å >
-å¦åå¯è½å¯¼è´æªç¥çå²çªé®é¢ ## ç®ä» è¿æ¯ä¸ä¸ªç¨ Python
-ç¼åçè°ç¨ [Bestdori](https://bestdori.com/) åç§ API
-ä¸èµæºä¸è½½çåºï¼å¤§è´åæ¬äºç¤¾åºå¸å­çå¤çä»¥ååç§ [BanG
-Dreamï¼å°å¥³ä¹å¢æ´¾å¯¹](https://zh.moegirl.org.cn/
+> bestdori-api ç°å·²å¨é¢æ¯æåæ­¥ä¸å¼æ­¥ >
+å¼æ­¥ä½¿ç¨æ¹æ³ä¸åæ­¥ç±»ä¼¼ï¼å¯å ä¹æ ç¼åæ¢ ## ç®ä»
+è¿æ¯ä¸ä¸ªç¨ Python ç¼åçè°ç¨ [Bestdori](https://bestdori.com/) åç§
+API ä¸èµæºä¸è½½çåºï¼å¤§è´åæ¬äºç¤¾åºå¸å­çå¤çä»¥ååç§
+[BanG Dreamï¼å°å¥³ä¹å¢æ´¾å¯¹](https://zh.moegirl.org.cn/
 BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81)
 æ¸¸æåèµæºçè·åã
 **è­¦åï¼æ­¤æ¨¡åç®åä»ç¶äºå¾å®åä¸æµè¯ï¼è¯·ä¸è¦å°å¶å½åä¸ä¸ªç¨³å®çåºä½¿ç¨ã**
 ### ç®åå·²æç API ä¸åè½ |API ç±»å«|æ¯å¦å®å|æ¯æçåå®¹| |:-
 ------|:-----:|:------
-| |ç¨æ·|ð|ç»å½ãæ¥è¯¢ãå¸å­è·åãä¿¡æ¯è·å|
+| |ç¨æ·|ðð|ç»å½ãæ¥è¯¢ãå¸å­è·åãä¿¡æ¯è·å|
 |å¸å­|ð|æç´¢ãè·åãåè¡¨ãè¯è®ºãåæ¬¢|
 |è°±é¢|ð|ç¤¾åºè°±é¢è·åãé³æºä¸å°é¢è·åãè§æ´åãæ°æ®ç»è®¡ãæ ¼å¼äºè½¬|
-|æäº|ðð|ç¤¾åºæäºè·å| |è§è²|ð¤|ä¿¡æ¯è·åãèµæºè·å|
-|å¡ç|ð|ä¿¡æ¯è·åãèµæºè·å| |æè£|ðð|ä¿¡æ¯è·å|
-|æ´»å¨|ð¤|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
-|æå|ð¤|æ°æ®è·åãèµæºè·å|
-|æ­æ²|ð¤|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ðð|æ°æ®è·å|
-|ç»å½å¥å±|ð¤|ä¿¡æ¯è·åãèµæºè·å| |èªéå¸|ð¤|ä¿¡æ¯è·å|
-|æ¼«ç»|ð¤|ä¿¡æ¯è·åãå¾çè·å| |ä»»å¡|ð¤|ä¿¡æ¯è·å|
-|ayachan|ð¤|è°±é¢åæãæµè¯æä¸ä¼ ãé¾åº¦åæ|
-|å¶ä»èµæº|ðð|ä»å°é¨åèµæºæåç¬è·å| ## å¿«éä½¿ç¨
+|æäº|ð|ç¤¾åºæäºè·å| |è§è²|ð|ä¿¡æ¯è·åãèµæºè·å|
+|å¡ç|ð|ä¿¡æ¯è·åãèµæºè·å| |æè£|ð|ä¿¡æ¯è·å|
+|æ´»å¨|ð|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
+|æå|ð|æ°æ®è·åãèµæºè·å|
+|æ­æ²|ð|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ð|æ°æ®è·å|
+|ç»å½å¥å±|ð|ä¿¡æ¯è·åãèµæºè·å| |èªéå¸|ð|ä¿¡æ¯è·å|
+|æ¼«ç»|ðð|ä¿¡æ¯è·åãå¾çè·å| |ä»»å¡|ð|ä¿¡æ¯è·å|
+|ayachan|ððð|è°±é¢åæãæµè¯æä¸ä¼ ãé¾åº¦åæ|
+|å¶ä»èµæº|ð|é¨åç¬ç«èµæºçåç¬è·å| ## å¿«éä½¿ç¨
 ä»¥ä¸å°ä»¥è·åç¤¾åºèªå¶è°±é¢ [[FULL] åã®ä¸­ã¸](https://
 bestdori.com/community/charts/111533/WindowsSov8-FULL) çä¿¡æ¯ä¸ºä¾ã
 é¦åï¼ä½¿ç¨ä»¥ä¸æä»¤å®è£æ¬æ¨¡åï¼ ```bash $ pip3 install bestdori-
 api ``` æ¥ä¸æ¥å¨ä¸ä¸ª Python
 èæ¬æä»¶ä¸­ï¼ä½¿ç¨å¦ä¸ä»£ç è·åæå®å¸å­çå¨é¨ä¿¡æ¯ï¼è¿éæä»¬å·²ç¥è¯¥å¸å­ç
 ID ä¸º `111533`ï¼ï¼ ```python from bestdori.post import Post def main() -
 > None: # å®ä¾å Post ç±» p = Post(id='111533') # è°ç¨æ¹æ³è·åä¿¡æ¯
@@ -45,14 +43,16 @@
 'custom', 'audio': 'https://bestdori.com/api/upload/file/
 e4a080f84bfa2ca47b23b390a464c819ec17e70b', 'cover': 'https://bestdori.com/api/
 upload/file/e3535ebb4c740c4757371026a1df9ffb08010307' }, 'artists':
 'çµæãã³ã', 'diff': 4, 'level': 30, 'chart': [ { 'bpm': 191, 'beat': 0,
 'type': 'BPM' }, { 'beat': 192, 'lane': 3. 'type': 'Single' }, ... ], ... } ```
 å¦ææ³è¦è·åè¿ä¸ªèªå¶è°±é¢çè°±é¢ï¼æèæ³è¦è·åå®çé³æºä¸å°é¢ï¼ä»¥ä¸ä»£ç å°ä¼è¿è¡è·åï¼
 ```python from bestdori.post import Post def main() -> None: # å®ä¾å Post
-ç±» p = Post(id='111533') # è°ç¨æ¹æ³è·åè°±é¢ chart = p.get_chart() #
+ç±» p = Post(id='111533') #
+è°ç¨æ¹æ³è·åä¿¡æ¯ï¼ææå±æ§åæ¹æ³å¨ä½¿ç¨åå¿é¡»è·åä¸æ¬¡ä¿¡æ¯ï¼
+p.get_details() # éè¿å±æ§è·åè°±é¢ chart = p.chart #
 è·åçå°æ¯ä¸ä¸ªè°±é¢å®ä¾ # è°ç¨æ¹æ³è·åé³æºä¸å°é¢ info =
 p.get_song() # è·åçå°æ¯ä¸ä¸ªåå«äºé³æºä¸å°é¢ç bytes å­å¸
 main() ``` Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown
```

### Comparing `bestdori-api-0.2.0/README.md` & `bestdori-api-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,50 +26,44 @@
 
 <a href="https://www.python.org/downloads/">
   <img src="https://img.shields.io/pypi/pyversions/bestdori-api" alt="Python Version">
 </a>
 
 </p>
 
-> bestdori_api 已更名为 bestdori-api
-> 若安装过之前的 `bestdori_api` 包，请使用指令
-> ```bash
-> pip uninstall bestdori_api
-> ```
-> 
-> 卸载原 `bestdori_api` 包后，重新安装 `bestdori-api` 包
-> 否则可能导致未知的冲突问题
+> bestdori-api 现已全面支持同步与异步
+> 异步使用方法与同步类似，可几乎无缝切换
 
 ## 简介
 
 这是一个用 Python 编写的调用 [Bestdori](https://bestdori.com/) 各种 API 与资源下载的库，大致包括了社区帖子的处理以及各种 [BanG Dream！少女乐团派对](https://zh.moegirl.org.cn/BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81) 游戏内资源的获取。
 **警告：此模块目前仍然亟待完善与测试，请不要将其当做一个稳定的库使用。**
 
 ### 目前已有的 API 与功能
 
 |API 类别|是否完善|支持的内容|
 |:-------|:-----:|:------|
-|用户|👍|登录、查询、帖子获取、信息获取|
+|用户|👍👍|登录、查询、帖子获取、信息获取|
 |帖子|👍|搜索、获取、发表、评论、喜欢|
 |谱面|👍|社区谱面获取、音源与封面获取、规整化、数据统计、格式互转|
-|故事|👎👎|社区故事获取|
-|角色|🤔|信息获取、资源获取|
-|卡牌|👎|信息获取、资源获取|
-|服装|👎👎|信息获取|
-|活动|🤔|信息获取、资源获取|
-|活动数据|👎|数据获取|
-|招募|🤔|数据获取、资源获取|
-|歌曲|🤔|信息获取、资源获取|
-|歌曲 Meta|👎👎|数据获取|
-|登录奖励|🤔|信息获取、资源获取|
-|自选券|🤔|信息获取|
-|漫画|🤔|信息获取、图片获取|
-|任务|🤔|信息获取|
-|ayachan|🤔|谱面分析、测试服上传、难度分析|
-|其他资源|👎👎|仅小部分资源有单独获取|
+|故事|👍|社区故事获取|
+|角色|👍|信息获取、资源获取|
+|卡牌|👍|信息获取、资源获取|
+|服装|👍|信息获取|
+|活动|👍|信息获取、资源获取|
+|活动数据|👍|数据获取|
+|招募|👍|数据获取、资源获取|
+|歌曲|👍|信息获取、资源获取|
+|歌曲 Meta|👍|数据获取|
+|登录奖励|👍|信息获取、资源获取|
+|自选券|👍|信息获取|
+|漫画|👍👍|信息获取、图片获取|
+|任务|👍|信息获取|
+|ayachan|👍👍👍|谱面分析、测试服上传、难度分析|
+|其他资源|👍|部分独立资源的单独获取|
 
 ## 快速使用
 
 以下将以获取社区自制谱面 [[FULL] 光の中へ](https://bestdori.com/community/charts/111533/WindowsSov8-FULL) 的信息为例。
 
 首先，使用以下指令安装本模块：
 ```bash
@@ -122,14 +116,16 @@
 如果想要获取这个自制谱面的谱面，或者想要获取它的音源与封面，以下代码将会进行获取：
 ```python
 from bestdori.post import Post
 
 def main() -> None:
     # 实例化 Post 类
     p = Post(id='111533')
-    # 调用方法获取谱面
-    chart = p.get_chart() # 获取的将是一个谱面实例
+    # 调用方法获取信息（所有属性化方法在使用前必须获取一次信息）
+    p.get_details()
+    # 通过属性获取谱面
+    chart = p.chart # 获取的将是一个谱面实例
     # 调用方法获取音源与封面
     info = p.get_song() # 获取的将是一个包含了音源与封面的 bytes 字典
 
 main()
 ```
```

#### html2text {}

```diff
@@ -1,37 +1,35 @@
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
                    æå¶ä»éè¦çæ¥å£è¯·åæ¶æåº**
           _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
-> bestdori_api å·²æ´åä¸º bestdori-api > è¥å®è£è¿ä¹åç `bestdori_api`
-åï¼è¯·ä½¿ç¨æä»¤ > ```bash > pip uninstall bestdori_api > ``` > >
-å¸è½½å `bestdori_api` ååï¼éæ°å®è£ `bestdori-api` å >
-å¦åå¯è½å¯¼è´æªç¥çå²çªé®é¢ ## ç®ä» è¿æ¯ä¸ä¸ªç¨ Python
-ç¼åçè°ç¨ [Bestdori](https://bestdori.com/) åç§ API
-ä¸èµæºä¸è½½çåºï¼å¤§è´åæ¬äºç¤¾åºå¸å­çå¤çä»¥ååç§ [BanG
-Dreamï¼å°å¥³ä¹å¢æ´¾å¯¹](https://zh.moegirl.org.cn/
+> bestdori-api ç°å·²å¨é¢æ¯æåæ­¥ä¸å¼æ­¥ >
+å¼æ­¥ä½¿ç¨æ¹æ³ä¸åæ­¥ç±»ä¼¼ï¼å¯å ä¹æ ç¼åæ¢ ## ç®ä»
+è¿æ¯ä¸ä¸ªç¨ Python ç¼åçè°ç¨ [Bestdori](https://bestdori.com/) åç§
+API ä¸èµæºä¸è½½çåºï¼å¤§è´åæ¬äºç¤¾åºå¸å­çå¤çä»¥ååç§
+[BanG Dreamï¼å°å¥³ä¹å¢æ´¾å¯¹](https://zh.moegirl.org.cn/
 BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81)
 æ¸¸æåèµæºçè·åã
 **è­¦åï¼æ­¤æ¨¡åç®åä»ç¶äºå¾å®åä¸æµè¯ï¼è¯·ä¸è¦å°å¶å½åä¸ä¸ªç¨³å®çåºä½¿ç¨ã**
 ### ç®åå·²æç API ä¸åè½ |API ç±»å«|æ¯å¦å®å|æ¯æçåå®¹| |:-
 ------|:-----:|:------
-| |ç¨æ·|ð|ç»å½ãæ¥è¯¢ãå¸å­è·åãä¿¡æ¯è·å|
+| |ç¨æ·|ðð|ç»å½ãæ¥è¯¢ãå¸å­è·åãä¿¡æ¯è·å|
 |å¸å­|ð|æç´¢ãè·åãåè¡¨ãè¯è®ºãåæ¬¢|
 |è°±é¢|ð|ç¤¾åºè°±é¢è·åãé³æºä¸å°é¢è·åãè§æ´åãæ°æ®ç»è®¡ãæ ¼å¼äºè½¬|
-|æäº|ðð|ç¤¾åºæäºè·å| |è§è²|ð¤|ä¿¡æ¯è·åãèµæºè·å|
-|å¡ç|ð|ä¿¡æ¯è·åãèµæºè·å| |æè£|ðð|ä¿¡æ¯è·å|
-|æ´»å¨|ð¤|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
-|æå|ð¤|æ°æ®è·åãèµæºè·å|
-|æ­æ²|ð¤|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ðð|æ°æ®è·å|
-|ç»å½å¥å±|ð¤|ä¿¡æ¯è·åãèµæºè·å| |èªéå¸|ð¤|ä¿¡æ¯è·å|
-|æ¼«ç»|ð¤|ä¿¡æ¯è·åãå¾çè·å| |ä»»å¡|ð¤|ä¿¡æ¯è·å|
-|ayachan|ð¤|è°±é¢åæãæµè¯æä¸ä¼ ãé¾åº¦åæ|
-|å¶ä»èµæº|ðð|ä»å°é¨åèµæºæåç¬è·å| ## å¿«éä½¿ç¨
+|æäº|ð|ç¤¾åºæäºè·å| |è§è²|ð|ä¿¡æ¯è·åãèµæºè·å|
+|å¡ç|ð|ä¿¡æ¯è·åãèµæºè·å| |æè£|ð|ä¿¡æ¯è·å|
+|æ´»å¨|ð|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
+|æå|ð|æ°æ®è·åãèµæºè·å|
+|æ­æ²|ð|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ð|æ°æ®è·å|
+|ç»å½å¥å±|ð|ä¿¡æ¯è·åãèµæºè·å| |èªéå¸|ð|ä¿¡æ¯è·å|
+|æ¼«ç»|ðð|ä¿¡æ¯è·åãå¾çè·å| |ä»»å¡|ð|ä¿¡æ¯è·å|
+|ayachan|ððð|è°±é¢åæãæµè¯æä¸ä¼ ãé¾åº¦åæ|
+|å¶ä»èµæº|ð|é¨åç¬ç«èµæºçåç¬è·å| ## å¿«éä½¿ç¨
 ä»¥ä¸å°ä»¥è·åç¤¾åºèªå¶è°±é¢ [[FULL] åã®ä¸­ã¸](https://
 bestdori.com/community/charts/111533/WindowsSov8-FULL) çä¿¡æ¯ä¸ºä¾ã
 é¦åï¼ä½¿ç¨ä»¥ä¸æä»¤å®è£æ¬æ¨¡åï¼ ```bash $ pip3 install bestdori-
 api ``` æ¥ä¸æ¥å¨ä¸ä¸ª Python
 èæ¬æä»¶ä¸­ï¼ä½¿ç¨å¦ä¸ä»£ç è·åæå®å¸å­çå¨é¨ä¿¡æ¯ï¼è¿éæä»¬å·²ç¥è¯¥å¸å­ç
 ID ä¸º `111533`ï¼ï¼ ```python from bestdori.post import Post def main() -
 > None: # å®ä¾å Post ç±» p = Post(id='111533') # è°ç¨æ¹æ³è·åä¿¡æ¯
@@ -41,11 +39,13 @@
 'custom', 'audio': 'https://bestdori.com/api/upload/file/
 e4a080f84bfa2ca47b23b390a464c819ec17e70b', 'cover': 'https://bestdori.com/api/
 upload/file/e3535ebb4c740c4757371026a1df9ffb08010307' }, 'artists':
 'çµæãã³ã', 'diff': 4, 'level': 30, 'chart': [ { 'bpm': 191, 'beat': 0,
 'type': 'BPM' }, { 'beat': 192, 'lane': 3. 'type': 'Single' }, ... ], ... } ```
 å¦ææ³è¦è·åè¿ä¸ªèªå¶è°±é¢çè°±é¢ï¼æèæ³è¦è·åå®çé³æºä¸å°é¢ï¼ä»¥ä¸ä»£ç å°ä¼è¿è¡è·åï¼
 ```python from bestdori.post import Post def main() -> None: # å®ä¾å Post
-ç±» p = Post(id='111533') # è°ç¨æ¹æ³è·åè°±é¢ chart = p.get_chart() #
+ç±» p = Post(id='111533') #
+è°ç¨æ¹æ³è·åä¿¡æ¯ï¼ææå±æ§åæ¹æ³å¨ä½¿ç¨åå¿é¡»è·åä¸æ¬¡ä¿¡æ¯ï¼
+p.get_details() # éè¿å±æ§è·åè°±é¢ chart = p.chart #
 è·åçå°æ¯ä¸ä¸ªè°±é¢å®ä¾ # è°ç¨æ¹æ³è·åé³æºä¸å°é¢ info =
 p.get_song() # è·åçå°æ¯ä¸ä¸ªåå«äºé³æºä¸å°é¢ç bytes å­å¸
 main() ```
```

### Comparing `bestdori-api-0.2.0/bestdori/__init__.py` & `bestdori-api-1.0.0/bestdori/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     logincampaigns,
     miracleticket,
     comics,
     missions,
     models
 )
 
-from .utils._settings import settings
+from . import settings as settings
 
 __all__ = [
     'User',
     'Me',
     'Post',
     'Chart',
     'Character',
```

### Comparing `bestdori-api-0.2.0/bestdori/ayachan/exceptions.py` & `bestdori-api-1.0.0/bestdori/ayachan/exceptions.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-0.2.0/bestdori/ayachan/utils/network.py` & `bestdori-api-1.0.0/bestdori/eventarchives.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,175 +1,221 @@
-'''`bestdori.ayachan.utils.network`
+'''`bestdori.eventarchives`
 
-向 ayachan 发送请求相关模块'''
-from json import dumps
-from io import BufferedReader
-from typing import Any, Union, Literal, Optional, cast
+BanG Dream! 活动数据相关操作'''
+from typing import Any, Literal
 
-from httpx import Client, Request, Response, HTTPStatusError
+from httpx import Response
 
-from ._settings import settings
-from ...exceptions import AssetsNotExistError
+from .utils.utils import API
+from .utils.network import Api
+from .post import get_list, get_list_async
+from .exceptions import (
+    EventNotExistError
+)
+
+# 获取总活动数据信息
+def get_all(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
+    '''获取总活动信息
 
-# 向 ayachan 发送 API 请求类
-class Api:
-    '''向 ayachan 发送 API 请求类
+    参数:
+        index (Literal[5], optional): 指定获取哪种 `all.json`
+            `5`: 获取所有已有活动数据的简洁信息 `all.5.json`
+
+    返回:
+        dict[str, dict[str, Any]]: 获取到的总活动信息
+    '''
+    return Api(API['all']['archives'].format(index=index)).get().json()
+
+# 异步获取总活动数据信息
+async def get_all_async(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
+    '''获取总活动信息
 
     参数:
-        api (str): 请求的 API 地址
-        proxy (Optional[Union[dict[str, str], str]]): 代理服务器
+        index (Literal[5], optional): 指定获取哪种 `all.json`
+            `5`: 获取所有已有活动数据的简洁信息 `all.5.json`
+
+    返回:
+        dict[str, dict[str, Any]]: 获取到的总活动信息
+    '''
+    response = await Api(API['all']['archives'].format(index=index)).aget()
+    if isinstance(response, Response):
+        return response.json()
+    else:
+        return await response.json()
+
+# 活动数据类
+class EventArchive:
+    '''活动数据类
+
+    参数:
+        id (int): 活动 ID
     '''
-    api: str
-    '''请求的 API 地址'''
-    proxy: Optional[Union[dict[str, str], str]]=None
-    '''代理服务器'''
     # 初始化
-    def __init__(
-        self,
-        api: str,
-        proxy: Optional[Union[dict[str, str], str]]=None
-    ) -> None:
-        '''初始化'''
-        self.api = api
-        self.proxy = proxy or settings.proxy
+    def __init__(self, id: int) -> None:
+        '''活动数据类
+
+        参数:
+            id (int): 活动 ID
+        '''
+        self.id: int = id
+        '''活动 ID'''
+        self.__info: dict[str, Any] = {}
+        '''活动信息'''
         return
     
-    # 请求发送
-    def request(
+    # 获取活动数据信息
+    def get_info(self) -> dict[str, Any]:
+        '''获取活动数据信息
+
+        返回:
+            dict[str, Any]: 活动数据信息
+        '''
+        _all = get_all()
+        if str(self.id) not in _all:
+            raise EventNotExistError(self.id)
+        self.__info = _all[str(self.id)]
+        
+        return self.__info
+    
+    # 异步获取活动数据信息
+    async def get_info_async(self) -> dict[str, Any]:
+        '''获取活动数据信息
+
+        返回:
+            dict[str, Any]: 活动数据信息
+        '''
+        _all = await get_all_async()
+        if str(self.id) not in _all:
+            raise EventNotExistError(self.id)
+        self.__info = _all[str(self.id)]
+        
+        return self.__info
+    
+    # 获取排名分数线
+    def get_top(
         self,
-        method: Literal['get', 'post'],
-        *,
-        params: Optional[dict[str, Any]]=None,
-        data: Optional[Any]=None,
-        files: Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]]=None,
-        json: Optional[Any]=None
-    ) -> Response:
-        '''请求发送
+        server: Literal[0, 1, 2, 3, 4],
+        mid: Literal['0']='0',
+        latest: Literal['1']='1'
+    ) -> dict[str, list[dict[str, Any]]]:
+        '''获取排名分数线
 
         参数:
-            method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
-            params (Optional[dict[str, Any]], optional): 调用参数
-            data (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
-            files (Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
-            json (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
+            server (Literal[0, 1, 2, 3, 4]): 指定服务器
+                `0`: 日服
+                `1`: 英服
+                `2`: 台服
+                `3`: 国服
+                `4`: 韩服
+            mid (Literal[&#39;0&#39;], optional): 指定是否为中间分数线，默认为 `0`
+            latest (Literal[&#39;1&#39;], optional): 指定是否为最终分数线，默认为 `1`
 
         返回:
-            Response: 收到的响应
-        '''
-        # 处理接收到的 API
-        if self.api.startswith('http://') or self.api.startswith('https://'):
-            self.api = self.api
-        else:
-            self.api = 'https://api.ayachan.fun/' + self.api
-        # 构建一个请求体
-        request = Request(
-            method,
-            self.api,
-            params=params,
-            data=(
-                cast(dict, dumps(data)) if data is not None and 'sonolus' not in self.api
-                else data
-            ),
-            files=files,
-            json=json,
-            headers=(
-                {
-                    'Content-Type': 'multipart/form-data; boundary=----WebKitFormBoundaryxjpDgorEXUAUIbBN'
-                } if 'sonolus' in self.api and method == 'post' else None
-            )
+            dict[str, list[dict[str, Any]]]: 排名分数线数据
+        '''
+        return Api(API['events']['top']).get(
+            params={
+                'server': server,
+                'event': self.id,
+                'mid': mid,
+                'latest': latest
+            }
+        ).json()
+    
+    # 异步获取排名分数线
+    async def get_top_async(
+        self,
+        server: Literal[0, 1, 2, 3, 4],
+        mid: Literal['0']='0',
+        latest: Literal['1']='1'
+    ) -> dict[str, list[dict[str, Any]]]:
+        '''获取排名分数线
+
+        参数:
+            server (Literal[0, 1, 2, 3, 4]): 指定服务器
+                `0`: 日服
+                `1`: 英服
+                `2`: 台服
+                `3`: 国服
+                `4`: 韩服
+            mid (Literal[&#39;0&#39;], optional): 指定是否为中间分数线，默认为 `0`
+            latest (Literal[&#39;1&#39;], optional): 指定是否为最终分数线，默认为 `1`
+
+        返回:
+            dict[str, list[dict[str, Any]]]: 排名分数线数据
+        '''
+        response = await Api(API['events']['top']).aget(
+            params={
+                'server': server,
+                'event': self.id,
+                'mid': mid,
+                'latest': latest
+            }
         )
-        # 构建代理服务器字典
-        if isinstance(self.proxy, str):
-            proxies = {'http://': self.proxy, 'https://': self.proxy}
-        elif isinstance(self.proxy, dict):
-            proxies = self.proxy
+        if isinstance(response, Response):
+            return response.json()
         else:
-            proxies = None
-        
-        # 发送请求并获取响应
-        with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
-            response = client.send(request)
-        
-        # 处理接收到的响应
-        response.raise_for_status()
-        return response
-
-# 获取 ayachan 资源数据
-class Assets:
-    '''获取 Bestdori 资源数据
+            return await response.json()
 
-    参数:
-        url (str): 请求的资源地址
-        proxy (Optional[Union[dict[str, str], str]]): 代理服务器
-    '''
-    url: str
-    '''请求的资源地址'''
-    proxy: Optional[Union[dict[str, str], str]]=None
-    '''代理服务器'''
-    # 初始化
-    def __init__(
+    # 获取活动数据评论
+    def get_comment(
         self,
-        url: str,
-        proxy: Optional[Union[dict[str, str], str]]=None
-    ) -> None:
-        '''获取 Bestdori 资源数据
+        limit: int=20,
+        offset: int=0,
+        order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
+    ) -> dict[str, Any]:
+        '''获取动数据评论
 
         参数:
-            url (str): 请求的资源地址
-            proxy (Optional[Union[dict[str, str], str]]): 代理服务器
-        '''
-        self.url = url
-        self.proxy = proxy or settings.proxy
-        return
-    
-    # 获取资源连接
-    def get_url(self) -> str:
-        '''获取资源连接
+            limit (int, optional): 展示出的评论数，默认为 20
+            offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
+            order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            str: 获取的资源连接 `str`
+            dict[str, Any]: 搜索结果
+                ```python
+                {
+                    "result": ... # bool 是否有响应
+                    "count": ... # int 搜索到的评论总数
+                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                }
+                ```
         '''
-        # 处理接收到的 URL
-        if self.api.startswith('http://') or self.api.startswith('https://'):
-            self.api = self.api
-        else:
-            self.api = 'https://api.ayachan.fun/' + self.api
-        return self.url
+        return get_list(
+            category_id=str(self.id),
+            category_name='EVENTARCHIVE_COMMENT',
+            limit=limit,
+            offset=offset,
+            order=order
+        )
     
-    # 获取资源
-    def get(self) -> bytes:
-        '''获取资源
+    # 异步获取活动数据评论
+    async def get_comment_async(
+        self,
+        limit: int=20,
+        offset: int=0,
+        order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
+    ) -> dict[str, Any]:
+        '''获取动数据评论
+
+        参数:
+            limit (int, optional): 展示出的评论数，默认为 20
+            offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
+            order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            bytes: 获取的资源字节数据 `bytes`
+            dict[str, Any]: 搜索结果
+                ```python
+                {
+                    "result": ... # bool 是否有响应
+                    "count": ... # int 搜索到的评论总数
+                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                }
+                ```
         '''
-        # 处理接收到的 URL
-        if self.api.startswith('http://') or self.api.startswith('https://'):
-            self.api = self.api
-        else:
-            self.api = 'https://api.ayachan.fun/' + self.api
-        # 构建一个请求体
-        request = Request('get', self.url)
-        # 构建代理服务器字典
-        if isinstance(self.proxy, str):
-            proxies = {'http://': self.proxy, 'https://': self.proxy}
-        elif isinstance(self.proxy, dict):
-            proxies = self.proxy
-        else:
-            proxies = None
-        
-        # 发送请求并获取响应
-        with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
-            response = client.send(request)
-        
-        try:
-            response.raise_for_status()
-        except HTTPStatusError as exception:
-            if exception.response.status_code == 404:
-                raise AssetsNotExistError(self.url)
-            else:
-                raise exception
-        # 检测响应资源是否存在
-        content_type = response.headers.get('content-type', None)
-        if content_type is None or content_type == 'text/html':
-            raise AssetsNotExistError(self.url)
-        return response.content
+        return await get_list_async(
+            category_id=str(self.id),
+            category_name='EVENTARCHIVE_COMMENT',
+            limit=limit,
+            offset=offset,
+            order=order
+        )
```

### Comparing `bestdori-api-0.2.0/bestdori/ayachan/utils/utils.py` & `bestdori-api-1.0.0/bestdori/ayachan/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-0.2.0/bestdori/cards.py` & `bestdori-api-1.0.0/bestdori/utils/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,265 +1,269 @@
-'''`bestdori.cards`
+'''`bestdori.utils`
 
-BanG Dream! 卡牌相关操作'''
-from typing import Any, Literal
+杂项模块'''
+from typing import Literal, Any
 
-from .post import get_list
-from .utils.utils import API, RES, ASSETS
-from .utils.network import Api, Res, Assets
-from .exceptions import (
-    NoDataException,
-    CardNotExistError
+from httpx import Response
+
+from .utils import API, RES,ASSETS
+from .network import Api, Res, Assets
+from bestdori.exceptions import (
+    AssetsNotExistError
 )
 
-# 获取总卡牌信息
-def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
-    '''获取总卡牌信息
-
-    参数:
-        index (Literal[0, 5], optional): 指定获取哪种 `all.json`
-            `0`: 仅获取所有已有卡牌 ID `all.0.json`
-            `5`: 获取所有已有卡牌的简洁信息 `all.5.json`
-
-    返回:
-        dict[str, dict[str, Any]]: 获取到的总卡牌信息
-    '''
-    return Api(API['cards']['all'].format(index=index)).request('get').json()
-
-# 获取属性图标
-def get_attribute_icon(attribute: Literal['powerful', 'pure', 'cool', 'happy']) -> bytes:
-    '''获取属性图标
-
-    参数:
-        attribute (Literal[&#39;powerful&#39;, &#39;pure&#39;, &#39;cool&#39;, &#39;happy&#39;]): 属性名称
-            `powerful`: POWERFUL
-            `pure`: PURE
-            `cool`: COOL
-            `happy`: HAPPY
-
-    返回:
-        bytes: 属性图标字节数据
-    '''
-    return Res(RES['icon']['svg'].format(name=f'{attribute}')).get()
-
-# 获取星星图标
-def get_star_icon(star: Literal['star', 'star_trained']) -> bytes:
-    '''获取星星图标
-
-    参数:
-        star (Literal[&#39;star&#39;, &#39;star_trained&#39;]): 星标种类
-            `star`: 普通星标
-            `star_trained`: 训练后星标
-
-    返回:
-        bytes: 星星图标字节数据
-    '''
-    return Res(RES['icon']['png'].format(name=f'{star}')).get()
-
-# 获取卡牌完整边框
-def get_frame(level: Literal[1, 2, 3, 4, 5]) -> bytes:
-    '''获取卡牌完整边框
-
-    参数:
-        level (Literal[1, 2, 3, 4, 5]): 边框星级
-
-    返回:
-        bytes: 卡牌完整边框字节数据
-    '''
-    return Res(RES['image']['png'].format(name=f'frame-{level}')).get()
-
-# 获取卡牌缩略图边框
-def get_card_frame(level: Literal[1, 2, 3, 4, 5]) -> bytes:
-    '''获取卡牌缩略图边框
-
-    参数:
-        level (Literal[1, 2, 3, 4, 5]): 边框星级
-
-    返回:
-        bytes: 卡牌缩略图边框字节数据
-    '''
-    return Res(RES['image']['png'].format(name=f'card-{level}')).get()
-
-# 卡牌类
-class Card:
-    '''卡牌类
-
-    参数:
-        id (int): 卡牌 ID
-    '''
-    # 初始化
-    def __init__(self, id: int) -> None:
-        '''卡牌类
-
-        参数:
-            id (int): 卡牌 ID
-        '''
-        self.id: int = id
-        '''卡牌 ID'''
-        self._info: dict[str, Any] = {}
-        '''卡牌信息'''
-        # 检测 ID 是否存在
-        all_id = get_all(0)
-        if not str(id) in all_id.keys():
-            raise CardNotExistError(id)
-        return
-    
-    # 获取卡牌信息
-    def get_info(self) -> dict[str, Any]:
-        '''获取卡牌信息
-
-        返回:
-            dict[str, Any]: 卡牌详细信息
-        '''
-        if len(self._info) <= 0:
-            # 如果没有卡牌信息存储
-            response = Api(
-                API['cards']['info'].format(id=self.id)
-            ).request('get')
-            self._info = dict(response.json())
-        return self._info
-    
-    # 获取卡牌评论
-    def get_comment(
-        self,
-        limit: int=20,
-        offset: int=0,
-        order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
-        '''获取卡牌评论
-
-        参数:
-            limit (int, optional): 展示出的评论数，默认为 20
-            offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
-            order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
-
-        返回:
-            dict[str, Any]: 搜索结果
-                ```python
-                result: bool # 是否有响应
-                count: int # 搜索到的评论总数
-                posts: list[dict[str, Any]] # 列举出的评论
-                ```
-        '''
-        return get_list(
-            category_name='CARD_COMMENT',
-            category_id=str(self.id),
-            order=order,
-            limit=limit,
-            offset=offset
-        )
-    
-    # 获取卡牌标题
-    @property
-    def prefix(self) -> str:
-        '''获取卡牌标题
-
-        返回:
-            str: 卡牌标题
-        '''
-        info = self.get_info()
-        # 获取 prefix 数据
-        if (prefix := info.get('prefix', None)) is None:
-            raise NoDataException('卡牌标题')
-        # 获取第一个非 None 卡牌标题
-        try:
-            return next(filter(lambda x: x is not None, prefix))
-        except StopIteration:
-            raise NoDataException('卡牌标题')
-    
-    # 获取卡牌所在服务器
-    @property
-    def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
-        '''获取卡牌所在服务器
-
-        返回:
-            Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
-        '''
-        info = self.get_info()
-        # 获取 releasedAt 数据
-        if (released_at := info.get('releasedAt', None)) is None:
-            raise NoDataException('卡牌发布时间')
-        # 根据 releasedAt 数据判断服务器
-        if released_at[0] is not None: return 'jp'
-        elif released_at[1] is not None: return 'en'
-        elif released_at[2] is not None: return 'tw'
-        elif released_at[3] is not None: return 'cn'
-        elif released_at[4] is not None: return 'kr'
-        else:
-            raise NoDataException('卡牌所在服务器')
-    
-    # 获取卡牌完整图片
-    def get_card(self, type: Literal['normal', 'after_training']) -> bytes:
-        '''获取卡牌完整图片
-
-        参数:
-            type (Literal[&#39;normal&#39;, &#39;after_training&#39;]): 指定特训前或特训后
-
-        返回:
-            bytes: 卡牌完整图片字节数据 `bytes`
-        '''
-        # 获取卡牌数据包名称
-        info = self.get_info()
-        if (resource_set_name := info.get('resourceSetName', None)) is None:
-            raise ValueError('无法获取卡牌数据包名称。')
-        return Assets(
-            ASSETS['characters']['resourceset'].format(
-                resource_set_name=resource_set_name, name='card', type=type
-            ), self.server
-        ).get()
-    
-    # 获取卡牌无背景图片
-    def get_trim(self, type: Literal['normal', 'after_training']) -> bytes:
-        '''获取卡牌无背景图片
-
-        参数:
-            type (Literal[&#39;normal&#39;, &#39;after_training&#39;]): 指定特训前或特训后
-
-        返回:
-            bytes: 卡牌无背景图片字节数据 `bytes`
-        '''
-        # 获取卡牌数据包名称
-        info = self.get_info()
-        if (resource_set_name := info.get('resourceSetName', None)) is None:
-            raise ValueError('无法获取卡牌数据包名称。')
-        return Assets(
-            ASSETS['characters']['resourceset'].format(
-                resource_set_name=resource_set_name, name='trim', type=type
-            ), self.server
-        ).get()
-    
-    # 获取卡牌缩略图图片
-    def get_thumb(self, type: Literal['normal', 'after_training']) -> bytes:
-        '''获取卡牌缩略图图片
-
-        参数:
-            type (Literal[&#39;normal&#39;, &#39;after_training&#39;]): 指定特训前或特训后
-
-        返回:
-            bytes: 卡牌缩略图图片字节数据 `bytes`
-        '''
-        # 获取卡牌数据包名称
-        info = self.get_info()
-        if (resource_set_name := info.get('resourceSetName', None)) is None:
-            raise ValueError('无法获取卡牌数据包名称。')
-        return Assets(
-            ASSETS['thumb']['chara'].format(
-                id=str(int(self.id) // 50), resource_set_name=resource_set_name, type=type
-            ), self.server
-        ).get()
-    
-    # 获取 LIVE 服装图片
-    def get_livesd(self) -> bytes:
-        '''获取 LIVE 服装图片
-
-        返回:
-            bytes: 卡牌 LIVE 服装图片字节数据 `bytes`
-        '''
-        # 获取卡牌 livesd 数据包名称
-        info = self.get_info()
-        if (sd_resource_name := info.get('sdResourceName', None)) is None:
-            raise ValueError('无法获取卡牌 livesd 数据包名称。')
-        return Assets(
-            ASSETS['characters']['livesd'].format(
-                sd_resource_name=sd_resource_name
-            ), self.server
-        ).get()
+# 将十六进制颜色代码转换为 RGB 元组
+def hexto_rgb(hex: str) -> tuple[int, int, int]:
+    '''将十六进制颜色代码转换为 RGB 元组
+
+    参数:
+        hex (str): 十六进制颜色代码
+
+    返回:
+        tuple[int, int, int]: RGB 元组
+    '''
+    if hex[0] == '#':
+        hex = hex[1:]
+    if len(hex) == 3:
+        hex = hex[0] * 2 + hex[1] * 2 + hex[2] * 2
+    rgb = tuple(int(hex[i:i+2], 16) for i in (0, 2, 4))
+    if len(rgb) != 3:
+        raise ValueError('十六进制颜色代码')
+    return rgb
+
+# 获取称号资源
+def get_degree(
+    degree_name: str,
+    server: Literal['jp', 'en', 'tw', 'cn', 'kr']
+) -> bytes:
+    '''获取称号资源
+
+    参数:
+        degree_name (str): 称号名称
+        
+        server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
+            `jp`: 日服
+            `en`: 英服
+            `tw`: 台服
+            `cn`: 国服
+            `kr`: 韩服
+
+    返回:
+        bytes: 称号资源字节数据 `bytes`
+    '''
+    try:
+        return Assets(ASSETS['thumb']['degree'].format(degree_name=degree_name), server).get()
+    except AssetsNotExistError:
+        raise AssetsNotExistError(f'称号 {degree_name}-{server}')
+
+# 异步获取称号资源
+async def get_degree_async(
+    degree_name: str,
+    server: Literal['jp', 'en', 'tw', 'cn', 'kr']
+) -> bytes:
+    '''获取称号资源
+
+    参数:
+        degree_name (str): 称号名称
+        
+        server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
+            `jp`: 日服
+            `en`: 英服
+            `tw`: 台服
+            `cn`: 国服
+            `kr`: 韩服
+
+    返回:
+        bytes: 称号资源字节数据 `bytes`
+    '''
+    try:
+        return await Assets(ASSETS['thumb']['degree'].format(degree_name=degree_name), server).aget()
+    except AssetsNotExistError:
+        raise AssetsNotExistError(f'称号 {degree_name}-{server}')
+
+# 获取总技能信息
+def get_skill_all(index: Literal[10]=10) -> dict[str, dict[str, Any]]:
+    '''获取总技能信息
+
+    参数:
+        index (Literal[10], optional): 指定获取哪种 `all.json`
+            `10`: 获取所有已有技能的信息 `all.5.json`
+
+    返回:
+        dict[str, dict[str, Any]]: 获取到的总技能信息
+    '''
+    return Api(API['all']['skills'].format(index=index)).get().json()
+
+# 异步获取总技能信息
+async def get_skill_all_async(index: Literal[10]=10) -> dict[str, dict[str, Any]]:
+    '''获取总技能信息
+
+    参数:
+        index (Literal[10], optional): 指定获取哪种 `all.json`
+            `10`: 获取所有已有技能的信息 `all.5.json`
+
+    返回:
+        dict[str, dict[str, Any]]: 获取到的总技能信息
+    '''
+    response = await Api(API['all']['skills'].format(index=index)).aget()
+    if isinstance(response, Response): return response.json()
+    return await response.json()
+
+# 获取总乐队信息
+def get_bands_all(index: Literal[1]=1) -> dict[str, dict[str, Any]]:
+    '''获取总乐队信息
+
+    参数:
+        index (Literal[1], optional): 指定获取哪种 `all.json`
+            `1`: 获取所有已有乐队的名称信息 `all.1.json`，默认为该项
+
+    返回:
+        dict[str, dict[str, Any]]: 获取到的总乐队信息
+    '''
+    return Api(API['bands']['all'].format(index=index)).get().json()
+
+# 异步获取总乐队信息
+async def get_bands_all_async(index: Literal[1]=1) -> dict[str, dict[str, Any]]:
+    '''获取总乐队信息
+
+    参数:
+        index (Literal[1], optional): 指定获取哪种 `all.json`
+            `1`: 获取所有已有乐队的名称信息 `all.1.json`，默认为该项
+
+    返回:
+        dict[str, dict[str, Any]]: 获取到的总乐队信息
+    '''
+    response = await Api(API['bands']['all'].format(index=index)).aget()
+    if isinstance(response, Response): return response.json()
+    return await response.json()
+
+# 获取主要乐队信息
+def get_bands_main(index: Literal[1]=1) -> dict[str, dict[str, Any]]:
+    '''获取主要乐队信息
+
+    参数:
+        index (Literal[1], optional): 指定获取哪种 `main.json`
+            `1`: 获取所有主要乐队的名称信息 `main.1.json`，默认为该项
+
+    返回:
+        dict[str, dict[str, Any]]: 获取到的主要乐队信息
+    '''
+    return Api(API['bands']['main'].format(index=index)).get().json()
+
+# 异步获取主要乐队信息
+async def get_bands_main_async(index: Literal[1]=1) -> dict[str, dict[str, Any]]:
+    '''获取主要乐队信息
+
+    参数:
+        index (Literal[1], optional): 指定获取哪种 `main.json`
+            `1`: 获取所有主要乐队的名称信息 `main.1.json`，默认为该项
+
+    返回:
+        dict[str, dict[str, Any]]: 获取到的主要乐队信息
+    '''
+    response = await Api(API['bands']['main'].format(index=index)).aget()
+    if isinstance(response, Response): return response.json()
+    return await response.json()
+
+# 获取乐队 logo
+def get_band_logo(
+    id: int,
+    type: Literal['logoS', 'logoL', 'logoL_Mask'],
+    server: Literal['jp', 'en', 'tw', 'cn', 'kr']
+) -> bytes:
+    '''获取乐队 logo
+
+    参数:
+        id (int): 乐队 ID
+        
+        type (Literal[&#39;logoS&#39;, &#39;logoL&#39;, &#39;logoL_Mask&#39;]): logo 类型
+            `logoS`: 小 logo
+            `logoL`: 大 logo
+            `logoL_Mask`: 大 logo 遮罩
+        
+        server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
+
+    返回:
+        bytes: 乐队 logo 字节数据 `bytes`
+    '''
+    return Assets(ASSETS['band']['logo'].format(id=id, type=type), server).get()
+
+# 异步获取乐队 logo
+async def get_band_logo_async(
+    id: int,
+    type: Literal['logoS', 'logoL', 'logoL_Mask'],
+    server: Literal['jp', 'en', 'tw', 'cn', 'kr']
+) -> bytes:
+    '''获取乐队 logo
+
+    参数:
+        id (int): 乐队 ID
+        
+        type (Literal[&#39;logoS&#39;, &#39;logoL&#39;, &#39;logoL_Mask&#39;]): logo 类型
+            `logoS`: 小 logo
+            `logoL`: 大 logo
+            `logoL_Mask`: 大 logo 遮罩
+        
+        server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
+
+    返回:
+        bytes: 乐队 logo 字节数据 `bytes`
+    '''
+    return await Assets(ASSETS['band']['logo'].format(id=id, type=type), server).aget()
+
+# 获取乐队图标
+def get_band_icon(id: str) -> bytes:
+    '''获取乐队图标
+
+    参数:
+        id (str): 乐队 ID
+
+    返回:
+        bytes: 乐队图标字节数据
+    '''
+    return Res(RES['icon']['svg'].format(name=f'band_{id}')).get()
+
+# 异步获取乐队图标
+async def get_band_icon_async(id: str) -> bytes:
+    '''获取乐队图标
+
+    参数:
+        id (str): 乐队 ID
+
+    返回:
+        bytes: 乐队图标字节数据
+    '''
+    return await Res(RES['icon']['svg'].format(name=f'band_{id}')).aget()
+
+# 获取服务器图标
+def get_server_icon(server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> bytes:
+    '''获取服务器图标
+
+    参数:
+        server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 服务器名称
+            `jp`: 日服
+            `en`: 英服
+            `tw`: 台服
+            `cn`: 国服
+            `kr`: 韩服
+
+    返回:
+        bytes: 服务器图标字节数据
+    '''
+    return Res(RES['icon']['svg'].format(name=server)).get()
+
+# 异步获取服务器图标
+async def get_server_icon_async(server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> bytes:
+    '''获取服务器图标
+
+    参数:
+        server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 服务器名称
+            `jp`: 日服
+            `en`: 英服
+            `tw`: 台服
+            `cn`: 国服
+            `kr`: 韩服
+
+    返回:
+        bytes: 服务器图标字节数据
+    '''
+    return await Res(RES['icon']['svg'].format(name=server)).aget()
```

### Comparing `bestdori-api-0.2.0/bestdori/charts.py` & `bestdori-api-1.0.0/bestdori/charts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 '''`bestdori.charts`
 
 谱面相关操作'''
 from json import dumps, loads
 from typing import Any, Literal
 
-from .utils.note import *
+from httpx import Response
+
+from .models.note import *
 from .utils.utils import API
 from .utils.network import Api
 
 # 谱面数据类
 class Statistics:
     '''谱面数据类
 
@@ -280,9 +282,31 @@
         参数:
             id (int): 谱面 ID
             diff (Literal[&#39;easy&#39;, &#39;normal&#39;, &#39;hard&#39;, &#39;expert&#39;, &#39;special&#39;], optional): 难度名称
 
         返回:
             Chart: 获取到的谱面对象 `bestdori.chart.Chart`
         '''
-        response = Api(API['charts']['info'].format(id=id, diff=diff)).request('get')
+        response = Api(API['charts']['info'].format(id=id, diff=diff)).get()
         return cls.normalize(response.json())
+    
+    # 异步获取官方谱面
+    @classmethod
+    async def get_chart_async(
+        cls,
+        id: int,
+        diff: Literal['easy', 'normal', 'hard', 'expert', 'special']='expert'
+    ) -> 'Chart':
+        '''获取官方谱面
+
+        参数:
+            id (int): 谱面 ID
+            diff (Literal[&#39;easy&#39;, &#39;normal&#39;, &#39;hard&#39;, &#39;expert&#39;, &#39;special&#39;], optional): 难度名称
+
+        返回:
+            Chart: 获取到的谱面对象 `bestdori.chart.Chart`
+        '''
+        response = await Api(API['charts']['info'].format(id=id, diff=diff)).aget()
+        if isinstance(response, Response):
+            return cls.normalize(response.json())
+        else:
+            return cls.normalize(await response.json())
```

### Comparing `bestdori-api-0.2.0/bestdori/comics.py` & `bestdori-api-1.0.0/bestdori/missions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,219 +1,206 @@
-'''`bestdori.comics`
+'''`bestdori.missions`
 
-BanG Dream! 漫画相关操作'''
+BanG Dream! 任务相关操作'''
 from typing import Any, Literal
 
-from .post import get_list
-from .utils.utils import API, ASSETS
-from .utils.network import Api, Assets
+from aiohttp import ClientResponseError
+from httpx import Response, HTTPStatusError
+
+from .utils.utils import API
+from .utils.network import Api
+from .post import get_list, get_list_async
 from .exceptions import (
     NoDataException,
-    ComicNotExistError,
-    ServerNotAvailableError
+    MissionNotExistError
 )
 
-# 获取总漫画信息
-def get_all(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
-    '''获取总漫画信息
+# 获取总任务信息
+def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+    '''获取总任务信息
 
     参数:
-        index (Literal[5], optional): 指定获取哪种 `all.json`
-            `5`: 获取所有已有漫画信息 `all.5.json`
+        index (Literal[0, 5], optional): 指定获取哪种 `all.json`
+            `0`: 仅获取所有已有任务 ID `all.0.json`
+            `5`: 获取所有已有任务的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总漫画信息
+        dict[str, dict[str, Any]]: 获取到的总任务信息
     '''
-    return Api(API['all']['comics'].format(index=index)).request('get').json()
+    return Api(API['missions']['all'].format(index=index)).get().json()
+
+# 异步获取总任务信息
+async def get_all_async(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+    '''获取总任务信息
 
-# 漫画类
-class Comic:
-    '''漫画类
+    参数:
+        index (Literal[0, 5], optional): 指定获取哪种 `all.json`
+            `0`: 仅获取所有已有任务 ID `all.0.json`
+            `5`: 获取所有已有任务的简洁信息 `all.5.json`
+
+    返回:
+        dict[str, dict[str, Any]]: 获取到的总任务信息
+    '''
+    response = await Api(API['missions']['all'].format(index=index)).aget()
+    if isinstance(response, Response): return response.json()
+    return await response.json()
+
+# 任务类
+class Mission:
+    '''任务类
 
     参数:
-        id (int): 漫画 ID
+        id (int): 任务 ID
     '''
     # 初始化
     def __init__(self, id: int) -> None:
-        '''漫画类
+        '''任务类
 
         参数:
-            id (int): 漫画 ID
+            id (int): 任务 ID
         '''
         self.id: int = id
-        '''漫画 ID'''
-        self._info: dict[str, Any] = {}
-        '''漫画信息'''
-        # 检测 ID 是否存在
-        all_ = get_all(5)
-        if not str(id) in all_.keys():
-            raise ComicNotExistError(id)
-        self._info = all_[str(id)]
+        '''任务 ID'''
+        self.__info: dict[str, Any] = {}
+        '''任务信息'''
         return
     
-    # 获取漫画信息
+    # 任务标题
+    @property
+    def title(self) -> str:
+        '''任务标题'''
+        info = self.__info
+        # 获取 title 数据
+        if (title := info.get('title', None)) is None:
+            raise NoDataException('任务标题')
+        # 获取第一个非 None 任务标题
+        try:
+            return next(filter(lambda x: x is not None, title))
+        except StopIteration:
+            raise NoDataException('任务标题')
+    
+    # 任务所在默认服务器
+    @property
+    def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
+        '''任务所在默认服务器'''
+        info = self.__info
+        # 获取 startAt 数据
+        if (start_at := info.get('startAt', None)) is None:
+            raise NoDataException('任务起始时间')
+        # 根据 startAt 数据判断服务器
+        if start_at[0] is not None: return 'jp'
+        elif start_at[1] is not None: return 'en'
+        elif start_at[2] is not None: return 'tw'
+        elif start_at[3] is not None: return 'cn'
+        elif start_at[4] is not None: return 'kr'
+        else:
+            raise NoDataException('任务所在服务器')
+    
+    # 获取任务信息
     def get_info(self) -> dict[str, Any]:
-        '''获取漫画信息
+        '''获取任务信息
 
         返回:
-            dict[str, Any]: 漫画详细信息
+            dict[str, Any]: 任务详细信息
         '''
-        return self._info
+        try:
+            response = Api(
+                API['missions']['info'].format(id=self.id)
+            ).get()
+        except HTTPStatusError as exception:
+            if exception.response.status_code == 404:
+                raise MissionNotExistError(self.id)
+            raise exception
+        
+        self.__info = dict(response.json())
+        return self.__info
+    
+    # 异步获取任务信息
+    async def get_info_async(self) -> dict[str, Any]:
+        '''获取任务信息
+
+        返回:
+            dict[str, Any]: 任务详细信息
+        '''
+        try:
+            response = await Api(
+                API['missions']['info'].format(id=self.id)
+            ).aget()
+        except HTTPStatusError as exception:
+            if exception.response.status_code == 404:
+                raise MissionNotExistError(self.id)
+            raise exception
+        except ClientResponseError as exception:
+            if exception.status == 404:
+                raise MissionNotExistError(self.id)
+            raise exception
+        
+        if isinstance(response, Response):
+            self.__info = dict(response.json())
+        else:
+            self.__info = dict(await response.json())
+        return self.__info
     
-    # 获取漫画评论
+    # 获取任务评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
     ) -> dict[str, Any]:
-        '''获取漫画评论
+        '''获取任务评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
             dict[str, Any]: 搜索结果
-            ```python
-            result: bool # 是否有响应
-            count: int # 搜索到的评论总数
-            posts: list[dict[str, Any]] # 列举出的评论
-            ```
+                ```python
+                {
+                    "result": ... # bool 是否有响应
+                    "count": ... # int 搜索到的评论总数
+                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                }
+                ```
         '''
         return get_list(
-            category_name='COMIC_COMMENT',
+            category_name='MISSION_COMMENT',
             category_id=str(self.id),
             order=order,
             limit=limit,
             offset=offset
         )
     
-    # 获取漫画标题
-    @property
-    def title(self) -> str:
-        '''获取漫画标题
-
-        返回:
-            str: 漫画标题
-        '''
-        info = self.get_info()
-        # 获取 title 数据
-        if (title := info.get('title', None)) is None:
-            raise NoDataException('漫画标题')
-        # 获取第一个非 None 漫画标题
-        try:
-            return next(filter(lambda x: x is not None, title))
-        except StopIteration:
-            raise NoDataException('漫画标题')
-    
-    # 获取漫画副标题
-    @property
-    def sub_title(self) -> str:
-        '''获取漫画副标题
-
-        返回:
-            str: 漫画副标题
-        '''
-        info = self.get_info()
-        # 获取 subTitle 数据
-        if (sub_title := info.get('subTitle', None)) is None:
-            raise NoDataException('漫画副标题')
-        # 获取第一个非 None 漫画副标题
-        try:
-            return next(filter(lambda x: x is not None, sub_title))
-        except StopIteration:
-            raise NoDataException('漫画副标题')
-    
-    # 获取漫画默认服务器
-    @property
-    def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
-        '''获取漫画默认服务器
-
-        返回:
-            Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
-        '''
-        info = self.get_info()
-        # 获取 publicStartAt 数据
-        if (public_start_at := info.get('publicStartAt', None)) is None:
-            raise NoDataException('漫画 ID 列表')
-        # 根据 publicStartAt 数据判断服务器
-        if public_start_at[0] is not None: return 'jp'
-        elif public_start_at[1] is not None: return 'en'
-        elif public_start_at[2] is not None: return 'tw'
-        elif public_start_at[3] is not None: return 'cn'
-        elif public_start_at[4] is not None: return 'kr'
-        else:
-            raise NoDataException('漫画所在服务器')
-
-    # 获取漫画类型
-    @property
-    def type(self) -> Literal['singleframe', 'fourframe']:
-        '''获取漫画类型
-
-        返回:
-            Literal[&#39;singleframe&#39;, &#39;fourframe&#39;]: 漫画类型
-        '''
-        # 获取漫画数据包名称
-        info = self.get_info()
-        if (asset_bundle_name := info.get('assetBundleName', None)) is None:
-            raise ValueError('无法获取漫画数据包名称。')
-        # 判断漫画类型
-        if 'fourframe' in asset_bundle_name:
-            return 'fourframe'
-        else:
-            return 'singleframe'
-    
-    # 获取漫画缩略图图像
-    def get_thumbnail(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> bytes:
-        '''获取漫画缩略图图像
-
-        参数:
-            server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
-
-        返回:
-            bytes: 漫画缩略图图像字节数据 `bytes`
-        '''
-        # 获取漫画数据包名称
-        info = self.get_info()
-        if (asset_bundle_name := info.get('assetBundleName', None)) is None:
-            raise ValueError('无法获取漫画数据包名称。')
-        # 判断服务器
-        if (public_start_at := info.get('publicStartAt', None)) is None:
-            raise ValueError('无法获取漫画起始时间。')
-        SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
-        index = SERVERS.index(server)
-        if public_start_at[index] is None:
-            raise ServerNotAvailableError(f'漫画 {self.title}', server)
-        return Assets(
-            ASSETS['comic']['thumbnail'].format(
-                type=self.type, asset_bundle_name=asset_bundle_name
-            ), server
-        ).get()
-    
-    # 获取漫画图像
-    def get(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> bytes:
-        '''获取漫画图像
+    # 异步获取任务评论
+    async def get_comment_async(
+        self,
+        limit: int=20,
+        offset: int=0,
+        order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
+    ) -> dict[str, Any]:
+        '''获取任务评论
 
         参数:
-            server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
+            limit (int, optional): 展示出的评论数，默认为 20
+            offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
+            order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            bytes: 漫画图像字节数据 `bytes`
+            dict[str, Any]: 搜索结果
+                ```python
+                {
+                    "result": ... # bool 是否有响应
+                    "count": ... # int 搜索到的评论总数
+                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                }
+                ```
         '''
-        # 获取漫画数据包名称
-        info = self.get_info()
-        if (asset_bundle_name := info.get('assetBundleName', None)) is None:
-            raise ValueError('无法获取漫画数据包名称。')
-        # 判断服务器
-        if (public_start_at := info.get('publicStartAt', None)) is None:
-            raise ValueError('无法获取漫画起始时间。')
-        SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
-        index = SERVERS.index(server)
-        if public_start_at[index] is None:
-            raise ServerNotAvailableError(f'漫画 {self.title}', server)
-        return Assets(
-            ASSETS['comic']['comic'].format(
-                type=self.type, asset_bundle_name=asset_bundle_name
-            ), server
-        ).get()
+        return await get_list_async(
+            category_name='MISSION_COMMENT',
+            category_id=str(self.id),
+            order=order,
+            limit=limit,
+            offset=offset
+        )
+
```

### Comparing `bestdori-api-0.2.0/bestdori/exceptions.py` & `bestdori-api-1.0.0/bestdori/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,16 +315,16 @@
         super().__init__(msg)
         return
 
 # 没有获取到 ContentType
 class NoContentTypeError(RequestError):
     '''没有获取到 ContentType'''
     # 初始化
-    def __init__(self, response: Response) -> None:
-        msg = f'没有获取到 {response.url} 的 ContentType'
+    def __init__(self, url: str) -> None:
+        msg = f'没有获取到 {url} 的 ContentType'
         super().__init__(msg)
         return
 
 # 请求错误集合
 REQUEST_EXCEPTION: dict[str, type[RequestException]] = {
     'REQUEST_INVALID': RequestInvalidError,
     'LOGIN_REQUIRED': LoginRequiredError,
```

### Comparing `bestdori-api-0.2.0/bestdori/player.py` & `bestdori-api-1.0.0/bestdori/player.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,73 @@
 '''`bestdori.player`
 
 BanG Dream! 玩家信息相关操作'''
 
 from typing import Any, Optional
 
+from httpx import Response
+
 from .utils.utils import API
 from .utils.network import Api
 from .exceptions import PlayerNotExistError
 
 class Player:
     '''玩家类
 
     参数:
         id (int): 玩家 ID
         server (str): 服务器
     '''
     def __init__(self, id: int, server: str) -> None:
         self.id: int = id
         self.server: str = server
-        self._info: Optional[dict[str, Any]] = None
+        self.__info: Optional[dict[str, Any]] = None
+    
+    def get_info(self) -> dict[str, Any]:
+        '''获取玩家信息
+
+        返回:
+            dict[str, Any]: 玩家信息
+        '''
+        params = {
+            'mode': 2
+        }
+        _info = Api(
+            API['player']['info'].format(server=self.server, id=self.id)
+        ).get(params=params).json()
+        if not _info.get('result', False):
+            raise ValueError(f'Invalid Server: {self.server}')
+        _data: dict[str, Any] = _info.get('data', {})
+        _profile: Optional[dict[str, Any]] = _data.get('profile', None)
+        if _profile is None:
+            raise PlayerNotExistError(self.server, self.id)
+        self.__info = _profile
+        
+        return self.__info
     
-    def get(self) -> dict[str, Any]:
+    async def get_info_async(self) -> dict[str, Any]:
         '''获取玩家信息
 
         返回:
             dict[str, Any]: 玩家信息
         '''
-        if self._info is None:
-            params = {
-                'mode': 2
-            }
-            _info = Api(
-                API['player']['info'].format(server=self.server, id=self.id)
-            ).request('get', params=params).json()
-            if not _info.get('result', False):
-                raise ValueError(f'Invalid Server: {self.server}')
-            _data: dict[str, Any] = _info.get('data', {})
-            _profile: Optional[dict[str, Any]] = _data.get('profile', None)
-            if _profile is None:
-                raise PlayerNotExistError(self.server, self.id)
-            self._info = _profile
+        params = {
+            'mode': 2
+        }
+        response = await Api(
+            API['player']['info'].format(server=self.server, id=self.id)
+        ).aget(params=params)
+        
+        if isinstance(response, Response):
+            _info = response.json()
+        else:
+            _info = await response.json()
+        
+        if not _info.get('result', False):
+            raise ValueError(f'Invalid Server: {self.server}')
+        _data: dict[str, Any] = _info.get('data', {})
+        _profile: Optional[dict[str, Any]] = _data.get('profile', None)
+        if _profile is None:
+            raise PlayerNotExistError(self.server, self.id)
+        self.__info = _profile
         
-        return self._info
+        return self.__info
```

### Comparing `bestdori-api-0.2.0/bestdori/songs.py` & `bestdori-api-1.0.0/bestdori/songs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 '''`bestdori.songs`
 
 BanG Dream! 歌曲相关操作'''
 from typing import Any, Literal
 
-from httpx._exceptions import HTTPStatusError
+from aiohttp import ClientResponseError
+from httpx import Response, HTTPStatusError
 
 from .charts import Chart
-from .post import get_list
-from .utils.utils import ASSETS, API
-from .utils.network import Assets, Api
+from .utils.utils import API, ASSETS
+from .utils.network import Api, Assets
+from .post import get_list, get_list_async
 from .exceptions import (
     NoDataException,
     DiffNotExistError,
     SongNotExistError
 )
 
 # 获取总歌曲信息
@@ -24,15 +25,34 @@
             `0`: 仅获取所有已有歌曲 ID `all.0.json`
             `5`: 获取所有已有歌曲的简洁信息 `all.5.json`，默认为该项
             `7`: 获取所有已有歌曲的较为详细信息 `all.7.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总歌曲信息
     '''
-    return Api(API['songs']['all'].format(index=index)).request('get').json()
+    return Api(API['songs']['all'].format(index=index)).get().json()
+
+# 异步获取总歌曲信息
+async def get_all_async(index: Literal[0, 5, 7]=5) -> dict[str, dict[str, Any]]:
+    '''获取总歌曲信息
+
+    参数:
+        index (Literal[0, 5], optional): 指定获取哪种 `all.json`
+            `0`: 仅获取所有已有歌曲 ID `all.0.json`
+            `5`: 获取所有已有歌曲的简洁信息 `all.5.json`，默认为该项
+            `7`: 获取所有已有歌曲的较为详细信息 `all.7.json`
+
+    返回:
+        dict[str, dict[str, Any]]: 获取到的总歌曲信息
+    '''
+    response = await Api(API['songs']['all'].format(index=index)).aget()
+    if isinstance(response, Response):
+        return response.json()
+    else:
+        return await response.json()
 
 # 歌曲封面内部类
 class Jacket:
     '''歌曲封面类
 
     参数:
         url (str): 封面链接
@@ -50,33 +70,41 @@
         '''数据包序列号'''
         self._jacket_image: str = jacket_image
         '''封面文件名'''
         self._server: Literal['jp', 'en', 'tw', 'cn', 'kr'] = server
         '''封面所在服务器'''
         return
     
-    # 获取封面 url
+    # 封面 url
     @property
     def url(self) -> str:
-        '''获取封面 url'''
+        '''封面 url'''
         return Assets(
             ASSETS['songs']['musicjacket'].format(
                 index=self._index, jacket_image=self._jacket_image
             ), self._server
         ).get_url()
     
     # 获取封面字节数据
-    @property
-    def bytes(self) -> bytes:
+    def get_bytes(self) -> bytes:
         '''获取封面字节数据'''
         return Assets(
             ASSETS['songs']['musicjacket'].format(
                 index=self._index, jacket_image=self._jacket_image
             ), self._server
         ).get()
+    
+    # 异步获取封面字节数据
+    async def get_bytes_async(self) -> bytes:
+        '''获取封面字节数据'''
+        return await Assets(
+            ASSETS['songs']['musicjacket'].format(
+                index=self._index, jacket_image=self._jacket_image
+            ), self._server
+        ).aget()
 
 # 歌曲类
 class Song:
     '''歌曲类
 
     参数:
         id (int): 歌曲 ID
@@ -86,76 +114,118 @@
         '''歌曲类
 
         参数:
             id (int): 歌曲 ID
         '''
         self.id: int = id
         '''歌曲 ID'''
-        self._info: dict[str, Any] = {}
+        self.__info: dict[str, Any] = {}
         '''歌曲信息'''
-        # 检测 ID 是否存在
-        all_id = get_all(0)
-        if not str(id) in all_id.keys():
-            raise SongNotExistError(id)
         return
     
     # 获取歌曲信息
     def get_info(self) -> dict[str, Any]:
         '''获取歌曲信息
 
         返回:
             dict[str, Any]: 歌曲详细信息
         '''
-        if len(self._info) <= 0:
-            # 如果没有歌曲信息存储
+        try:
             response = Api(
                 API['songs']['info'].format(id=self.id)
-            ).request('get')
-            self._info = dict(response.json())
-        return self._info
+            ).get()
+        except HTTPStatusError as exception:
+            if exception.response.status_code == 404:
+                raise SongNotExistError(self.id)
+            else:
+                raise exception
+        
+        self.__info = dict(response.json())
+        return self.__info
     
-    # 获取歌曲所在服务器
-    @property
-    def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
-        '''获取歌曲所在服务器
+    # 异步获取歌曲信息
+    async def get_info_async(self) -> dict[str, Any]:
+        '''获取歌曲信息
 
         返回:
-            Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
+            dict[str, Any]: 歌曲详细信息
         '''
-        info = self.get_info()
+        try:
+            response = await Api(
+                API['songs']['info'].format(id=self.id)
+            ).aget()
+        except HTTPStatusError as exception:
+            if exception.response.status_code == 404:
+                raise SongNotExistError(self.id)
+            else:
+                raise exception
+        except ClientResponseError as exception:
+            if exception.status == 404:
+                raise SongNotExistError(self.id)
+            else:
+                raise exception
+        
+        if isinstance(response, Response):
+            self.__info = dict(response.json())
+        else:
+            self.__info = dict(await response.json())
+        return self.__info
+    
+    # 歌曲所在默认服务器
+    @property
+    def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
+        '''歌曲所在默认服务器'''
+        info = self.__info
         # 获取 publishedAt 数据
         if (published_at := info.get('publishedAt', None)) is None:
             raise NoDataException('歌曲发布时间')
         # 根据 publishedAt 数据判断服务器
         if published_at[0] is not None: return 'jp'
         elif published_at[1] is not None: return 'en'
         elif published_at[2] is not None: return 'tw'
         elif published_at[3] is not None: return 'cn'
         elif published_at[4] is not None: return 'kr'
         else:
             raise NoDataException('歌曲服务器')
     
-    # 获取歌曲名称
+    # 歌曲名称
     @property
     def name(self) -> str:
-        '''获取歌曲名称
-
-        返回:
-            str: 歌曲名称
-        '''
-        info = self.get_info()
+        '''歌曲名称'''
+        info = self.__info
         # 获取 musicTitle 数据
         if (music_title := info.get('musicTitle', None)) is None:
             raise NoDataException('歌曲名称')
         # 获取第一个非 None 歌曲名称
         try:
             return next(filter(lambda x: x is not None, music_title))
         except StopIteration:
             raise NoDataException('歌曲名称')
     
+    # 歌曲封面
+    @property
+    def jacket(self) -> list[Jacket]:
+        '''歌曲封面'''
+        # 获取数据包序列号
+        quotient, remainder = divmod(self.id, 10)
+        if remainder == 0:
+            index = self.id
+        else:
+            index = (quotient + 1) * 10
+        
+        info = self.__info
+        if (jacket_image := info.get('jacketImage', None)) is None:
+            raise NoDataException('歌曲封面资源')
+        jacket: list[Jacket] = []
+        
+        for image in jacket_image:
+            jacket.append(Jacket(index, image, self.server))
+        
+        return jacket
+    
     # 获取歌曲谱面
     def get_chart(
         self,
         diff: Literal['easy', 'normal', 'hard', 'expert', 'special']='expert'
     ) -> Chart:
         '''获取歌曲谱面
 
@@ -171,47 +241,61 @@
         except HTTPStatusError as e:
             if e.response.status_code == 404:
                 # 难度不存在
                 raise DiffNotExistError(diff)
             else:
                 raise e
     
-    # 获取歌曲封面
-    def get_jacket(self) -> list[Jacket]:
-        '''获取歌曲封面
+    # 异步获取歌曲谱面
+    async def get_chart_async(
+        self,
+        diff: Literal['easy', 'normal', 'hard', 'expert', 'special']='expert'
+    ) -> Chart:
+        '''获取歌曲谱面
+
+        参数:
+            diff (Literal[&#39;easy&#39;, &#39;normal&#39;, &#39;hard&#39;, &#39;expert&#39;, &#39;special&#39;], optional): 难度名称
 
         返回:
-            Jacket: 歌曲封面对象 `Jacket`
+            Chart: 获取到的谱面对象
         '''
-        # 获取数据包序列号
-        quotient, remainder = divmod(self.id, 10)
-        if remainder == 0:
-            index = self.id
-        else:
-            index = (quotient + 1) * 10
-        
-        info = self.get_info()
-        if (jacket_image := info.get('jacketImage', None)) is None:
-            raise NoDataException('歌曲封面资源')
-        jacket: list[Jacket] = []
-        
-        for image in jacket_image:
-            jacket.append(Jacket(index, image, self.server))
-        
-        return jacket
+        try:
+            chart = await Chart.get_chart_async(self.id, diff)
+            return chart
+        except HTTPStatusError as e:
+            if e.response.status_code == 404:
+                # 难度不存在
+                raise DiffNotExistError(diff)
+            else:
+                raise e
+        except ClientResponseError as e:
+            if e.status == 404:
+                # 难度不存在
+                raise DiffNotExistError(diff)
+            else:
+                raise e
     
     # 获取歌曲音频
     def get_bgm(self) -> bytes:
         '''获取歌曲音频
 
         返回:
             bytes: 歌曲音频字节数据 `bytes`
         '''
         return Assets(ASSETS['songs']['sound'].format(id=self.id), self.server).get()
     
+    # 异步获取歌曲音频
+    async def get_bgm_async(self) -> bytes:
+        '''获取歌曲音频
+
+        返回:
+            bytes: 歌曲音频字节数据 `bytes`
+        '''
+        return await Assets(ASSETS['songs']['sound'].format(id=self.id), self.server).aget()
+    
     # 获取歌曲评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
     ) -> dict[str, Any]:
@@ -221,19 +305,53 @@
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
             dict[str, Any]: 搜索结果
                 ```python
-                result: bool # 是否有响应
-                count: int # 搜索到的评论总数
-                posts: list[dict[str, Any]] # 列举出的评论
+                {
+                    "result": ... # bool 是否有响应
+                    "count": ... # int 搜索到的评论总数
+                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                }
                 ```
         '''
         return get_list(
             category_name='SONG_COMMENT',
             category_id=str(self.id),
             order=order,
             limit=limit,
             offset=offset
         )
+    
+    # 异步获取歌曲评论
+    async def get_comment_async(
+        self,
+        limit: int=20,
+        offset: int=0,
+        order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
+    ) -> dict[str, Any]:
+        '''获取歌曲评论
+
+        参数:
+            limit (int, optional): 展示出的评论数，默认为 20
+            offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
+            order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
+
+        返回:
+            dict[str, Any]: 搜索结果
+                ```python
+                {
+                    "result": ... # bool 是否有响应
+                    "count": ... # int 搜索到的评论总数
+                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                }
+                ```
+        '''
+        return await get_list_async(
+            category_name='SONG_COMMENT',
+            category_id=str(self.id),
+            order=order,
+            limit=limit,
+            offset=offset
+        )
```

### Comparing `bestdori-api-0.2.0/bestdori/upload.py` & `bestdori-api-1.0.0/bestdori/upload.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 '''`bestdori.upload`
 
 Bestdori 文件相关操作'''
+from typing import Union
 from pathlib import Path
 from hashlib import sha1
 from io import BufferedReader
-from typing import TYPE_CHECKING, Union
+
+from httpx import Response
 
 from .user import Me
+from . import settings
 from .utils.utils import API
 from .utils.network import Api
-from .utils._settings import settings
 from .exceptions import AlreadyUploadedError
 
-if TYPE_CHECKING:
-    from .user import Me
-
 # 从 Bestdori 获取指定哈希文件字节
 def download(hash: str) -> bytes:
     '''从 Bestdori 获取指定哈希文件字节
 
     参数:
         hash (str): 文件哈希值
 
     返回:
         bytes: 文件字节 `bytes`
     '''
-    return Api(API['upload']['file'].format(hash=hash)).request('get').content
+    return Api(API['upload']['file'].format(hash=hash)).get().content
+
+# 异步从 Bestdori 获取指定哈希文件字节
+async def adownload(hash: str) -> bytes:
+    '''从 Bestdori 获取指定哈希文件字节
+
+    参数:
+        hash (str): 文件哈希值
+
+    返回:
+        bytes: 文件字节 `bytes`
+    '''
+    response = await Api(API['upload']['file'].format(hash=hash)).aget()
+    if isinstance(response, Response): return response.content
+    return await response.read()
 
 # 通过哈希值构建 Bestdori 文件 URL
 def hash_to_url(hash: str) -> str:
     '''通过哈希值构建 Bestdori 文件 URL
 
     参数:
         hash (str): 文件哈希值
@@ -95,47 +108,105 @@
         '''
         try:
             cookies = settings._cookies()
         except:
             if settings._username is None or settings._password is None:
                 raise ValueError('未添加用户信息。')
             else:
-                settings._me = Me(settings._username, settings._password)
+                settings._me = Me.login(settings._username, settings._password)
                 cookies = settings._cookies()
         
         if self._reader.closed:
             raise ValueError('文件流已关闭。')
         
         # 构建上传负载
         payload = {
             'ver': self._ver,
             'hash': self._hash,
             'size': self._size
         }
         # 发送预上传请求
         try:
-            Api(API['upload']['prepare']).request('post', cookies=cookies, data=payload)
+            Api(API['upload']['prepare']).post(cookies=cookies, data=payload)
         except AlreadyUploadedError:
             self._reader.close()
             return self._hash
         # 发送上传请求
         with self._reader:
-            response = Api(API['upload']['upload']).request(
-                'post',
+            response = Api(API['upload']['upload']).post(
                 files={
                     'file': (self._name, self._reader)
                 },
                 cookies=cookies
             )
         # 获取文件的哈希值
         hash_get = response.json()['hash']
         #重复查询至多 5 次上传状态
         for _ in range(5):
             # 发送上传状态查询请求
-            response = Api(API['upload']['status'].format(hash=hash_get)).request('get')
+            response = Api(API['upload']['status'].format(hash=hash_get)).get()
             # 获取上传状态
             status = response.json()['status']
             # 若上传成功则返回
             if status == 'available':
                 return hash_get
         
         raise TimeoutError(f'上传文件 {self._name} 超时。')
+    
+    # 异步上传文件
+    async def aupload(self) -> str:
+        '''上传文件
+
+        返回:
+            str: 上传文件的哈希值
+        '''
+        try:
+            cookies = settings._cookies()
+        except:
+            if settings._username is None or settings._password is None:
+                raise ValueError('未添加用户信息。')
+            else:
+                settings._me = await Me.alogin(settings._username, settings._password)
+                cookies = settings._cookies()
+        
+        if self._reader.closed:
+            raise ValueError('文件流已关闭。')
+        
+        # 构建上传负载
+        payload = {
+            'ver': self._ver,
+            'hash': self._hash,
+            'size': self._size
+        }
+        # 发送预上传请求
+        try:
+            await Api(API['upload']['prepare']).apost(cookies=cookies, data=payload)
+        except AlreadyUploadedError:
+            self._reader.close()
+            return self._hash
+        # 发送上传请求
+        with self._reader:
+            response = await Api(API['upload']['upload']).apost(
+                files={
+                    'file': (self._name, self._reader)
+                },
+                cookies=cookies
+            )
+        # 获取文件的哈希值
+        if isinstance(response, Response):
+            hash_get = response.json()['hash']
+        else:
+            hash_get = (await response.json())['hash']
+        #重复查询至多 5 次上传状态
+        for _ in range(5):
+            # 发送上传状态查询请求
+            response = await Api(API['upload']['status'].format(hash=hash_get)).aget()
+            # 获取上传状态
+            if isinstance(response, Response):
+                status = response.json()['status']
+            else:
+                status = (await response.json())['status']
+            # 若上传成功则返回
+            if status == 'available':
+                return hash_get
+        
+        raise TimeoutError(f'上传文件 {self._name} 超时。')
```

### Comparing `bestdori-api-0.2.0/bestdori/utils/network.py` & `bestdori-api-1.0.0/bestdori/ayachan/utils/network.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,337 +1,348 @@
-'''`bestdori.utils.network`
+'''`bestdori.ayachan.utils.network`
 
-向 Bestdori 发送请求相关模块'''
+向 ayachan 发送请求相关模块'''
 from json import dumps
 from io import BufferedReader
 from typing import Any, Union, Literal, Optional, cast
 
 from httpx import HTTPStatusError
-from httpx._models import Cookies
-from httpx import Response, Request, Client
+from aiohttp import ClientResponseError
+from aiohttp import ClientSession, ClientResponse
+from httpx import Client, Request, Response, AsyncClient
+
+from . import settings
+from bestdori.exceptions import AssetsNotExistError
+from bestdori.settings import AsyncClient as ClientSetting
 
-from ._settings import settings
-from ..exceptions import (
-    REQUEST_EXCEPTION,
-    RequestException,
-    NoContentTypeError,
-    AssetsNotExistError
-)
-
-# 向 Bestdori 发送 API 请求类
+# 向 ayachan 发送 API 请求类
 class Api:
-    '''向 Bestdori 发送 API 请求类
+    '''向 ayachan 发送 API 请求类
 
     参数:
         api (str): 请求的 API 地址
-        proxy (Optional[Union[dict[str, str], str]]): 代理服务器
     '''
     api: str
     '''请求的 API 地址'''
-    proxy: Optional[Union[dict[str, str], str]]=None
+    _proxies: Optional[Union[dict[str, str], str]]=None
     '''代理服务器'''
-    headers: dict[str, str]
-    '''请求头'''
     # 初始化
     def __init__(
         self,
-        api: str,
-        proxy: Optional[Union[dict[str, str], str]]=None
+        api: str
     ) -> None:
         '''初始化'''
         self.api = api
-        self.proxy = proxy or settings.proxy
-        self.headers = {'Content-Type': 'application/json;charset=UTF-8'}
+        if isinstance(settings.proxy, str):
+            self._proxies = {'http://': settings.proxy, 'https://': settings.proxy}
+        elif isinstance(settings.proxy, dict):
+            self._proxies = settings.proxy
         return
     
+    # 处理 url
+    @property
+    def _url(self) -> str:
+        # 处理接收到的 API
+        _url = self.api
+        if _url.startswith('http://') or _url.startswith('https://'):
+            return _url
+        else:
+            _url = 'https://api.ayachan.fun/' + self.api
+            return _url
+    
     # 请求发送
-    def request(
+    def _request(
         self,
         method: Literal['get', 'post'],
         *,
-        cookies: Optional[Cookies]=None,
         params: Optional[dict[str, Any]]=None,
-        data: Optional[dict[str, Any]]=None,
-        files: Optional[dict[str, tuple[str, BufferedReader]]]=None
+        data: Optional[Any]=None,
+        files: Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]]=None,
+        json: Optional[Any]=None
     ) -> Response:
         '''请求发送
 
         参数:
             method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
-            cookies (Optional[Cookies], optional): Cookies
             params (Optional[dict[str, Any]], optional): 调用参数
-            data (Optional[dict[str, Any]], optional): 调用参数，将以 `json` 字符串形式发送
-            files (Optional[dict[str, tuple[str, BufferedReader]]], optional): 发送文件参数
+            data (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
+            files (Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
+            json (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
 
         返回:
             Response: 收到的响应
         '''
-        # 处理接收到的 API
-        if self.api.startswith('http://') or self.api.startswith('https://'):
-            self.api = self.api
-        else:
-            self.api = 'https://bestdori.com/api/' + self.api
         # 构建一个请求体
         request = Request(
             method,
-            self.api,
-            cookies=cookies,
+            self._url,
             params=params,
-            data=cast(dict, dumps(data)) if data is not None else data,
+            data=(
+                cast(dict, dumps(data)) if data is not None and 'sonolus' not in self.api
+                else data
+            ),
             files=files,
-            headers=self.headers if not self.api.endswith('/upload') else None
+            json=json,
+            headers=(
+                {
+                    'Content-Type': 'multipart/form-data; boundary=----WebKitFormBoundaryxjpDgorEXUAUIbBN'
+                } if 'sonolus' in self.api and method == 'post' else None
+            )
         )
-        # 构建代理服务器字典
-        if isinstance(self.proxy, str):
-            proxies = {'http://': self.proxy, 'https://': self.proxy}
-        elif isinstance(self.proxy, dict):
-            proxies = self.proxy
-        else:
-            proxies = None
         
         # 发送请求并获取响应
-        with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
+        with Client(proxies=cast(dict, self._proxies), timeout=settings.timeout, trust_env=False) as client:
             response = client.send(request)
         
         # 处理接收到的响应
         response.raise_for_status()
-        # 判断接收到的响应是否为 json 格式
-        if 'application/json' not in (content_type := response.headers.get('content-type', None)):
-            if content_type is not None:
-                return response
-            else:
-                raise NoContentTypeError(response)
+        return response
+    
+    # 异步请求发送
+    async def _request_async(
+        self,
+        method: Literal['get', 'post'],
+        *,
+        params: Optional[dict[str, Any]]=None,
+        data: Optional[Any]=None,
+        files: Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]]=None,
+        json: Optional[Any]=None
+    ) -> Union[Response, ClientResponse]:
+        '''请求发送
+
+        参数:
+            method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
+            params (Optional[dict[str, Any]], optional): 调用参数
+            data (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
+            files (Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
+            json (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
+
+        返回:
+            Response: 收到的响应
+        '''
+        if settings.async_client == ClientSetting.HTTPX:
+            # 构建一个请求体
+            request = Request(
+                method,
+                self._url,
+                params=params,
+                data=(
+                    cast(dict, dumps(data)) if data is not None and 'sonolus' not in self.api
+                    else data
+                ),
+                files=files,
+                json=json,
+                headers=(
+                    {
+                        'Content-Type': 'multipart/form-data; boundary=----WebKitFormBoundaryxjpDgorEXUAUIbBN'
+                    } if 'sonolus' in self.api and method == 'post' else None
+                )
+            )
+            
+            # 发送请求并获取响应
+            async with AsyncClient(proxies=cast(dict, self._proxies), timeout=settings.timeout, trust_env=False) as client:
+                response = await client.send(request)
+            
+                # 处理接收到的响应
+                response.raise_for_status()
+        else:
+            async with ClientSession() as session:
+                async with session.request(
+                    method,
+                    self._url,
+                    params=params,
+                    data=(
+                        cast(dict, dumps(data)) if data is not None and 'sonolus' not in self.api
+                        else data
+                    ),
+                    files=files,
+                    json=json,
+                    headers=(
+                        {
+                            'Content-Type': 'multipart/form-data; boundary=----WebKitFormBoundaryxjpDgorEXUAUIbBN'
+                        } if 'sonolus' in self.api and method == 'post' else None
+                    )
+                ) as response:
+                    response.raise_for_status()
         
-        if isinstance((response_data := response.json()), dict):
-            if (result := response_data.get('result', None)) is not None:
-                if result is False:
-                    if (code := response_data.get('code', None)) is not None:
-                        if code in REQUEST_EXCEPTION.keys(): # 若错误码已被记录
-                            exception_class = REQUEST_EXCEPTION[code]
-                            if params is not None:
-                                raise exception_class(self.api, **params)
-                            elif data is not None:
-                                raise exception_class(self.api, **data)
-                            else:
-                                raise exception_class(self.api)
-                        else:
-                            raise RequestException(self.api, code)
-                    else:
-                        raise RequestException(self.api)
         return response
 
-# 获取 Bestdori 资源数据
+    def get(
+        self,
+        params: Optional[dict[str, Any]]=None
+    ) -> Response:
+        '''发送 GET 请求
+
+        参数:
+            params (Optional[dict[str, Any]], optional): 调用参数
+
+        返回:
+            Response: 收到的响应
+        '''
+        return self._request('get', params=params)
+    
+    async def aget(
+        self,
+        params: Optional[dict[str, Any]]=None
+    ) -> Union[Response, ClientResponse]:
+        '''发送 GET 请求
+
+        参数:
+            params (Optional[dict[str, Any]], optional): 调用参数
+
+        返回:
+            Response: 收到的响应
+        '''
+        return await self._request_async('get', params=params)
+    
+    def post(
+        self,
+        data: Optional[Any]=None,
+        files: Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]]=None,
+        json: Optional[Any]=None
+    ) -> Response:
+        '''发送 POST 请求
+
+        参数:
+            data (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
+            files (Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
+            json (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
+
+        返回:
+            Response: 收到的响应
+        '''
+        return self._request('post', data=data, files=files, json=json)
+    
+    async def apost(
+        self,
+        data: Optional[Any]=None,
+        files: Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]]=None,
+        json: Optional[Any]=None
+    ) -> Union[Response, ClientResponse]:
+        '''发送 POST 请求
+
+        参数:
+            data (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
+            files (Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
+            json (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
+
+        返回:
+            Response: 收到的响应
+        '''
+        return await self._request_async('post', data=data, files=files, json=json)
+
+# 获取 ayachan 资源数据
 class Assets:
     '''获取 Bestdori 资源数据
 
     参数:
         url (str): 请求的资源地址
-        server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 资源所在服务器
         proxy (Optional[Union[dict[str, str], str]]): 代理服务器
     '''
     url: str
     '''请求的资源地址'''
-    server: Literal['jp', 'en', 'tw', 'cn', 'kr', 'llsif']
-    '''资源所在服务器'''
-    proxy: Optional[Union[dict[str, str], str]]=None
+    _proxies: Optional[Union[dict[str, str], str]]=None
     '''代理服务器'''
     # 初始化
     def __init__(
         self,
-        url: str,
-        server: Literal['jp', 'en', 'tw', 'cn', 'kr', 'llsif'],
-        proxy: Optional[Union[dict[str, str], str]]=None
+        url: str
     ) -> None:
         '''获取 Bestdori 资源数据
 
         参数:
             url (str): 请求的资源地址
-            server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;, &#39;llsif&#39;]): 资源所在服务器
             proxy (Optional[Union[dict[str, str], str]]): 代理服务器
         '''
         self.url = url
-        self.server = server
-        self.proxy = proxy or settings.proxy
+        if isinstance(settings.proxy, str):
+            self._proxies = {'http://': settings.proxy, 'https://': settings.proxy}
+        elif isinstance(settings.proxy, dict):
+            self._proxies = settings.proxy
         return
     
     # 获取资源连接
     def get_url(self) -> str:
         '''获取资源连接
 
         返回:
             str: 获取的资源连接 `str`
         '''
-        # 如果服务器为 llsif 则转接方法
-        if self.server == 'llsif':
-            return self._get_niconi_url()
-        
-        # 处理接收到的 URL
-        if self.url.startswith('http://') or self.url.startswith('https://'):
-            self.url = self.url
-        else:
-            self.url = f'https://bestdori.com/assets/{self.server}/' + self.url
-        return self.url
-    
-    # 从 card.niconi.co.ni 获取资源连接
-    def _get_niconi_url(self) -> str:
-        '''从 card.niconi.co.ni 获取资源连接
-
-        返回:
-            str: 获取的资源连接 `str`
-        '''
         # 处理接收到的 URL
         if self.url.startswith('http://') or self.url.startswith('https://'):
-            self.url = self.url
+            return self.url
         else:
-            self.url = f'https://card.niconi.co.ni/asset/' + self.url
-        return self.url
+            return 'https://api.ayachan.fun/' + self.url
     
     # 获取资源
     def get(self) -> bytes:
         '''获取资源
 
         返回:
             bytes: 获取的资源字节数据 `bytes`
         '''
-        # 如果服务器为 llsif 则转接方法
-        if self.server == 'llsif':
-            return self._get_from_niconi()
-        
-        # 处理接收到的 URL
-        if self.url.startswith('http://') or self.url.startswith('https://'):
-            self.url = self.url
-        else:
-            self.url = f'https://bestdori.com/assets/{self.server}/' + self.url
         # 构建一个请求体
-        request = Request('get', self.url)
-        # 构建代理服务器字典
-        if isinstance(self.proxy, str):
-            proxies = {'http://': self.proxy, 'https://': self.proxy}
-        elif isinstance(self.proxy, dict):
-            proxies = self.proxy
-        else:
-            proxies = None
+        request = Request('get', self.get_url())
         
         # 发送请求并获取响应
-        with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
+        with Client(proxies=cast(dict, self._proxies), timeout=settings.timeout, trust_env=False) as client:
             response = client.send(request)
         
         try:
             response.raise_for_status()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
                 raise AssetsNotExistError(self.url)
             else:
                 raise exception
-        
         # 检测响应资源是否存在
         content_type = response.headers.get('content-type', None)
         if content_type is None or content_type == 'text/html':
             raise AssetsNotExistError(self.url)
         return response.content
     
-    # 从 card.niconi.co.ni 获取资源
-    def _get_from_niconi(self) -> bytes:
-        '''从 card.niconi.co.ni 获取资源
-
-        返回:
-            bytes: 获取的资源字节数据 `bytes`
-        '''
-        # 处理接收到的 URL
-        if self.url.startswith('http://') or self.url.startswith('https://'):
-            self.url = self.url
-        else:
-            self.url = f'https://card.niconi.co.ni/asset/' + self.url
-        # 构建一个请求体
-        request = Request('get', self.url)
-        # 构建代理服务器字典
-        if self.proxy is not None:
-            proxies = {'http://': self.proxy, 'https://': self.proxy}
-        else:
-            proxies = None
-        
-        # 发送请求并获取响应
-        with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
-            response = client.send(request)
-        
-        try:
-            response.raise_for_status()
-        except HTTPStatusError as exception:
-            if exception.response.status_code == 404:
-                raise AssetsNotExistError(self.url)
-            else:
-                raise exception
-        # 检测响应资源是否存在
-        content_type = response.headers.get('content-type', None)
-        if content_type is None or content_type == 'text/html':
-            raise AssetsNotExistError(self.url)
-        return response.content
-
-# 获取 Bestdori res 资源数据
-class Res:
-    '''获取 Bestdori res 资源数据
-
-    参数:
-        url (str): 请求的 res 资源地址
-        proxy (Optional[Union[dict[str, str], str]]): 代理服务器
-    '''
-    url: str
-    '''请求的资源地址'''
-    proxy: Optional[Union[dict[str, str], str]]=None
-    '''代理服务器'''
-    # 初始化
-    def __init__(
-        self,
-        url: str,
-        proxy: Optional[Union[dict[str, str], str]]=None
-    ) -> None:
-        '''获取 Bestdori 资源数据
-
-        参数:
-            url (str): 请求的资源地址
-            proxy (Optional[str]): 代理服务器
-        '''
-        self.url = url
-        self.proxy = proxy or settings.proxy
-        return
-    
-    # 获取资源
-    def get(self) -> bytes:
+    # 异步获取资源
+    async def aget(self) -> bytes:
         '''获取资源
 
         返回:
             bytes: 获取的资源字节数据 `bytes`
         '''
-        # 处理接收到的 URL
-        if self.url.startswith('http://') or self.url.startswith('https://'):
-            self.url = self.url
+        if settings.async_client == ClientSetting.HTTPX:
+            # 构建一个请求体
+            request = Request('get', self.url)
+            
+            # 发送请求并获取响应
+            async with AsyncClient(proxies=cast(dict, self._proxies), timeout=settings.timeout, trust_env=False) as client:
+                response = await client.send(request)
+            
+            try:
+                response.raise_for_status()
+            except HTTPStatusError as exception:
+                if exception.response.status_code == 404:
+                    raise AssetsNotExistError(self.url)
+                else:
+                    raise exception
         else:
-            self.url = f'https://bestdori.com/res/' + self.url
-        # 构建一个请求体
-        request = Request(
-            'get',
-            self.url
-        )
-        # 构建代理服务器字典
-        if isinstance(self.proxy, str):
-            proxies = {'http://': self.proxy, 'https://': self.proxy}
-        elif isinstance(self.proxy, dict):
-            proxies = self.proxy
-        else:
-            proxies = None
-        
-        # 发送请求并获取响应
-        with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
-            response = client.send(request)
+            # 发送请求并获取响应
+            async with ClientSession() as session:
+                response = await session.request(
+                    'get',
+                    self.get_url(),
+                    proxy=self._proxies,
+                )
+                try:
+                    response.raise_for_status()
+                except ClientResponseError as exception:
+                    if exception.status == 404:
+                        raise AssetsNotExistError(self.url)
+                    else:
+                        raise exception
         
-        try:
-            response.raise_for_status()
-        except HTTPStatusError as exception:
-            if exception.response.status_code == 404:
-                raise AssetsNotExistError(self.url)
-            else:
-                raise exception
         # 检测响应资源是否存在
         content_type = response.headers.get('content-type', None)
         if content_type is None or content_type == 'text/html':
             raise AssetsNotExistError(self.url)
-        return response.content
+        
+        if isinstance(response, Response):
+            return response.content
+        return await response.read()
```

### Comparing `bestdori-api-0.2.0/bestdori/utils/utils.py` & `bestdori-api-1.0.0/bestdori/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-0.2.0/bestdori_api.egg-info/PKG-INFO` & `bestdori-api-1.0.0/bestdori_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori-api
-Version: 0.2.0
+Version: 1.0.0
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori-api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
         
@@ -34,50 +34,44 @@
         
         <a href="https://www.python.org/downloads/">
           <img src="https://img.shields.io/pypi/pyversions/bestdori-api" alt="Python Version">
         </a>
         
         </p>
         
-        > bestdori_api 已更名为 bestdori-api
-        > 若安装过之前的 `bestdori_api` 包，请使用指令
-        > ```bash
-        > pip uninstall bestdori_api
-        > ```
-        > 
-        > 卸载原 `bestdori_api` 包后，重新安装 `bestdori-api` 包
-        > 否则可能导致未知的冲突问题
+        > bestdori-api 现已全面支持同步与异步
+        > 异步使用方法与同步类似，可几乎无缝切换
         
         ## 简介
         
         这是一个用 Python 编写的调用 [Bestdori](https://bestdori.com/) 各种 API 与资源下载的库，大致包括了社区帖子的处理以及各种 [BanG Dream！少女乐团派对](https://zh.moegirl.org.cn/BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81) 游戏内资源的获取。
         **警告：此模块目前仍然亟待完善与测试，请不要将其当做一个稳定的库使用。**
         
         ### 目前已有的 API 与功能
         
         |API 类别|是否完善|支持的内容|
         |:-------|:-----:|:------|
-        |用户|👍|登录、查询、帖子获取、信息获取|
+        |用户|👍👍|登录、查询、帖子获取、信息获取|
         |帖子|👍|搜索、获取、发表、评论、喜欢|
         |谱面|👍|社区谱面获取、音源与封面获取、规整化、数据统计、格式互转|
-        |故事|👎👎|社区故事获取|
-        |角色|🤔|信息获取、资源获取|
-        |卡牌|👎|信息获取、资源获取|
-        |服装|👎👎|信息获取|
-        |活动|🤔|信息获取、资源获取|
-        |活动数据|👎|数据获取|
-        |招募|🤔|数据获取、资源获取|
-        |歌曲|🤔|信息获取、资源获取|
-        |歌曲 Meta|👎👎|数据获取|
-        |登录奖励|🤔|信息获取、资源获取|
-        |自选券|🤔|信息获取|
-        |漫画|🤔|信息获取、图片获取|
-        |任务|🤔|信息获取|
-        |ayachan|🤔|谱面分析、测试服上传、难度分析|
-        |其他资源|👎👎|仅小部分资源有单独获取|
+        |故事|👍|社区故事获取|
+        |角色|👍|信息获取、资源获取|
+        |卡牌|👍|信息获取、资源获取|
+        |服装|👍|信息获取|
+        |活动|👍|信息获取、资源获取|
+        |活动数据|👍|数据获取|
+        |招募|👍|数据获取、资源获取|
+        |歌曲|👍|信息获取、资源获取|
+        |歌曲 Meta|👍|数据获取|
+        |登录奖励|👍|信息获取、资源获取|
+        |自选券|👍|信息获取|
+        |漫画|👍👍|信息获取、图片获取|
+        |任务|👍|信息获取|
+        |ayachan|👍👍👍|谱面分析、测试服上传、难度分析|
+        |其他资源|👍|部分独立资源的单独获取|
         
         ## 快速使用
         
         以下将以获取社区自制谱面 [[FULL] 光の中へ](https://bestdori.com/community/charts/111533/WindowsSov8-FULL) 的信息为例。
         
         首先，使用以下指令安装本模块：
         ```bash
@@ -130,16 +124,18 @@
         如果想要获取这个自制谱面的谱面，或者想要获取它的音源与封面，以下代码将会进行获取：
         ```python
         from bestdori.post import Post
         
         def main() -> None:
             # 实例化 Post 类
             p = Post(id='111533')
-            # 调用方法获取谱面
-            chart = p.get_chart() # 获取的将是一个谱面实例
+            # 调用方法获取信息（所有属性化方法在使用前必须获取一次信息）
+            p.get_details()
+            # 通过属性获取谱面
+            chart = p.chart # 获取的将是一个谱面实例
             # 调用方法获取音源与封面
             info = p.get_song() # 获取的将是一个包含了音源与封面的 bytes 字典
         
         main()
         ```
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,41 +1,39 @@
-Metadata-Version: 2.1 Name: bestdori-api Version: 0.2.0 Summary: Bestdori
+Metadata-Version: 2.1 Name: bestdori-api Version: 1.0.0 Summary: Bestdori
 çåç§ API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ Home-page: https://
 github.com/WindowsSov8forUs/bestdori-api Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
                    æå¶ä»éè¦çæ¥å£è¯·åæ¶æåº**
           _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
-> bestdori_api å·²æ´åä¸º bestdori-api > è¥å®è£è¿ä¹åç `bestdori_api`
-åï¼è¯·ä½¿ç¨æä»¤ > ```bash > pip uninstall bestdori_api > ``` > >
-å¸è½½å `bestdori_api` ååï¼éæ°å®è£ `bestdori-api` å >
-å¦åå¯è½å¯¼è´æªç¥çå²çªé®é¢ ## ç®ä» è¿æ¯ä¸ä¸ªç¨ Python
-ç¼åçè°ç¨ [Bestdori](https://bestdori.com/) åç§ API
-ä¸èµæºä¸è½½çåºï¼å¤§è´åæ¬äºç¤¾åºå¸å­çå¤çä»¥ååç§ [BanG
-Dreamï¼å°å¥³ä¹å¢æ´¾å¯¹](https://zh.moegirl.org.cn/
+> bestdori-api ç°å·²å¨é¢æ¯æåæ­¥ä¸å¼æ­¥ >
+å¼æ­¥ä½¿ç¨æ¹æ³ä¸åæ­¥ç±»ä¼¼ï¼å¯å ä¹æ ç¼åæ¢ ## ç®ä»
+è¿æ¯ä¸ä¸ªç¨ Python ç¼åçè°ç¨ [Bestdori](https://bestdori.com/) åç§
+API ä¸èµæºä¸è½½çåºï¼å¤§è´åæ¬äºç¤¾åºå¸å­çå¤çä»¥ååç§
+[BanG Dreamï¼å°å¥³ä¹å¢æ´¾å¯¹](https://zh.moegirl.org.cn/
 BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81)
 æ¸¸æåèµæºçè·åã
 **è­¦åï¼æ­¤æ¨¡åç®åä»ç¶äºå¾å®åä¸æµè¯ï¼è¯·ä¸è¦å°å¶å½åä¸ä¸ªç¨³å®çåºä½¿ç¨ã**
 ### ç®åå·²æç API ä¸åè½ |API ç±»å«|æ¯å¦å®å|æ¯æçåå®¹| |:-
 ------|:-----:|:------
-| |ç¨æ·|ð|ç»å½ãæ¥è¯¢ãå¸å­è·åãä¿¡æ¯è·å|
+| |ç¨æ·|ðð|ç»å½ãæ¥è¯¢ãå¸å­è·åãä¿¡æ¯è·å|
 |å¸å­|ð|æç´¢ãè·åãåè¡¨ãè¯è®ºãåæ¬¢|
 |è°±é¢|ð|ç¤¾åºè°±é¢è·åãé³æºä¸å°é¢è·åãè§æ´åãæ°æ®ç»è®¡ãæ ¼å¼äºè½¬|
-|æäº|ðð|ç¤¾åºæäºè·å| |è§è²|ð¤|ä¿¡æ¯è·åãèµæºè·å|
-|å¡ç|ð|ä¿¡æ¯è·åãèµæºè·å| |æè£|ðð|ä¿¡æ¯è·å|
-|æ´»å¨|ð¤|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
-|æå|ð¤|æ°æ®è·åãèµæºè·å|
-|æ­æ²|ð¤|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ðð|æ°æ®è·å|
-|ç»å½å¥å±|ð¤|ä¿¡æ¯è·åãèµæºè·å| |èªéå¸|ð¤|ä¿¡æ¯è·å|
-|æ¼«ç»|ð¤|ä¿¡æ¯è·åãå¾çè·å| |ä»»å¡|ð¤|ä¿¡æ¯è·å|
-|ayachan|ð¤|è°±é¢åæãæµè¯æä¸ä¼ ãé¾åº¦åæ|
-|å¶ä»èµæº|ðð|ä»å°é¨åèµæºæåç¬è·å| ## å¿«éä½¿ç¨
+|æäº|ð|ç¤¾åºæäºè·å| |è§è²|ð|ä¿¡æ¯è·åãèµæºè·å|
+|å¡ç|ð|ä¿¡æ¯è·åãèµæºè·å| |æè£|ð|ä¿¡æ¯è·å|
+|æ´»å¨|ð|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
+|æå|ð|æ°æ®è·åãèµæºè·å|
+|æ­æ²|ð|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ð|æ°æ®è·å|
+|ç»å½å¥å±|ð|ä¿¡æ¯è·åãèµæºè·å| |èªéå¸|ð|ä¿¡æ¯è·å|
+|æ¼«ç»|ðð|ä¿¡æ¯è·åãå¾çè·å| |ä»»å¡|ð|ä¿¡æ¯è·å|
+|ayachan|ððð|è°±é¢åæãæµè¯æä¸ä¼ ãé¾åº¦åæ|
+|å¶ä»èµæº|ð|é¨åç¬ç«èµæºçåç¬è·å| ## å¿«éä½¿ç¨
 ä»¥ä¸å°ä»¥è·åç¤¾åºèªå¶è°±é¢ [[FULL] åã®ä¸­ã¸](https://
 bestdori.com/community/charts/111533/WindowsSov8-FULL) çä¿¡æ¯ä¸ºä¾ã
 é¦åï¼ä½¿ç¨ä»¥ä¸æä»¤å®è£æ¬æ¨¡åï¼ ```bash $ pip3 install bestdori-
 api ``` æ¥ä¸æ¥å¨ä¸ä¸ª Python
 èæ¬æä»¶ä¸­ï¼ä½¿ç¨å¦ä¸ä»£ç è·åæå®å¸å­çå¨é¨ä¿¡æ¯ï¼è¿éæä»¬å·²ç¥è¯¥å¸å­ç
 ID ä¸º `111533`ï¼ï¼ ```python from bestdori.post import Post def main() -
 > None: # å®ä¾å Post ç±» p = Post(id='111533') # è°ç¨æ¹æ³è·åä¿¡æ¯
@@ -45,14 +43,16 @@
 'custom', 'audio': 'https://bestdori.com/api/upload/file/
 e4a080f84bfa2ca47b23b390a464c819ec17e70b', 'cover': 'https://bestdori.com/api/
 upload/file/e3535ebb4c740c4757371026a1df9ffb08010307' }, 'artists':
 'çµæãã³ã', 'diff': 4, 'level': 30, 'chart': [ { 'bpm': 191, 'beat': 0,
 'type': 'BPM' }, { 'beat': 192, 'lane': 3. 'type': 'Single' }, ... ], ... } ```
 å¦ææ³è¦è·åè¿ä¸ªèªå¶è°±é¢çè°±é¢ï¼æèæ³è¦è·åå®çé³æºä¸å°é¢ï¼ä»¥ä¸ä»£ç å°ä¼è¿è¡è·åï¼
 ```python from bestdori.post import Post def main() -> None: # å®ä¾å Post
-ç±» p = Post(id='111533') # è°ç¨æ¹æ³è·åè°±é¢ chart = p.get_chart() #
+ç±» p = Post(id='111533') #
+è°ç¨æ¹æ³è·åä¿¡æ¯ï¼ææå±æ§åæ¹æ³å¨ä½¿ç¨åå¿é¡»è·åä¸æ¬¡ä¿¡æ¯ï¼
+p.get_details() # éè¿å±æ§è·åè°±é¢ chart = p.chart #
 è·åçå°æ¯ä¸ä¸ªè°±é¢å®ä¾ # è°ç¨æ¹æ³è·åé³æºä¸å°é¢ info =
 p.get_song() # è·åçå°æ¯ä¸ä¸ªåå«äºé³æºä¸å°é¢ç bytes å­å¸
 main() ``` Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown
```

### Comparing `bestdori-api-0.2.0/bestdori_api.egg-info/SOURCES.txt` & `bestdori-api-1.0.0/bestdori_api.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,30 +10,27 @@
 bestdori/eventarchives.py
 bestdori/events.py
 bestdori/exceptions.py
 bestdori/gacha.py
 bestdori/logincampaigns.py
 bestdori/miracleticket.py
 bestdori/missions.py
-bestdori/models.py
 bestdori/player.py
 bestdori/post.py
+bestdori/settings.py
 bestdori/songmeta.py
 bestdori/songs.py
 bestdori/upload.py
 bestdori/user.py
 bestdori/ayachan/__init__.py
 bestdori/ayachan/exceptions.py
 bestdori/ayachan/utils/__init__.py
-bestdori/ayachan/utils/_settings.py
 bestdori/ayachan/utils/network.py
+bestdori/ayachan/utils/settings.py
 bestdori/ayachan/utils/utils.py
 bestdori/utils/__init__.py
-bestdori/utils/_settings.py
-bestdori/utils/content.py
 bestdori/utils/network.py
-bestdori/utils/note.py
 bestdori/utils/utils.py
 bestdori_api.egg-info/PKG-INFO
 bestdori_api.egg-info/SOURCES.txt
 bestdori_api.egg-info/dependency_links.txt
 bestdori_api.egg-info/top_level.txt
```

### Comparing `bestdori-api-0.2.0/setup.py` & `bestdori-api-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='bestdori-api',
-    version='0.2.0',
+    version='1.0.0',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Bestdori 的各种 API 调用整合，另外附带部分功能',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/bestdori-api',
     include_package_data=False,
```

