# Comparing `tmp/Jvav-1.9.0.tar.gz` & `tmp/Jvav-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-pwvku5r0/Jvav-1.9.0.tar", last modified: Mon Apr 22 03:23:28 2024, max compression
+gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-t87o_kqr/Jvav-1.9.1.tar", last modified: Fri Apr 26 15:54:33 2024, max compression
```

## Comparing `Jvav-1.9.0.tar` & `Jvav-1.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-22 03:23:28.000000 Jvav-1.9.0/
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)      295 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/SOURCES.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/dependency_links.txt
--rw-r--r--   0 zh         (501) staff       (20)       39 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/entry_points.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.9.0/Jvav.egg-info/not-zip-safe
--rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/requires.txt
--rw-r--r--   0 zh         (501) staff       (20)       11 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/top_level.txt
--rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.9.0/LICENSE
--rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.9.0/MANIFEST.in
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-04-22 03:23:28.000000 Jvav-1.9.0/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-1.9.0/README.md
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-22 03:23:28.000000 Jvav-1.9.0/jvav/
--rw-r--r--   0 zh         (501) staff       (20)      507 2024-04-22 03:22:48.000000 Jvav-1.9.0/jvav/__init__.py
--rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.9.0/jvav/cmd.py
--rw-r--r--   0 zh         (501) staff       (20)    77360 2024-04-13 04:33:40.000000 Jvav-1.9.0/jvav/utils.py
--rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-22 03:22:14.000000 Jvav-1.9.0/requirements.txt
--rw-r--r--   0 zh         (501) staff       (20)       38 2024-04-22 03:23:28.000000 Jvav-1.9.0/setup.cfg
--rw-r--r--   0 zh         (501) staff       (20)     1345 2024-04-22 03:22:55.000000 Jvav-1.9.0/setup.py
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-26 15:54:33.000000 Jvav-1.9.1/
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)      295 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/SOURCES.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/dependency_links.txt
+-rw-r--r--   0 zh         (501) staff       (20)       39 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/entry_points.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.9.1/Jvav.egg-info/not-zip-safe
+-rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/requires.txt
+-rw-r--r--   0 zh         (501) staff       (20)       11 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/top_level.txt
+-rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.9.1/LICENSE
+-rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.9.1/MANIFEST.in
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-04-26 15:54:33.000000 Jvav-1.9.1/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-1.9.1/README.md
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-26 15:54:33.000000 Jvav-1.9.1/jvav/
+-rw-r--r--   0 zh         (501) staff       (20)      481 2024-04-26 15:54:07.000000 Jvav-1.9.1/jvav/__init__.py
+-rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.9.1/jvav/cmd.py
+-rw-r--r--   0 zh         (501) staff       (20)    74171 2024-04-26 15:52:16.000000 Jvav-1.9.1/jvav/utils.py
+-rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-22 03:22:14.000000 Jvav-1.9.1/requirements.txt
+-rw-r--r--   0 zh         (501) staff       (20)       38 2024-04-26 15:54:33.000000 Jvav-1.9.1/setup.cfg
+-rw-r--r--   0 zh         (501) staff       (20)     1345 2024-04-26 15:54:04.000000 Jvav-1.9.1/setup.py
```

### Comparing `Jvav-1.9.0/Jvav.egg-info/PKG-INFO` & `Jvav-1.9.1/Jvav.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.9.0
+Version: 1.9.1
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.9.0 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.9.1 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Jvav-1.9.0/LICENSE` & `Jvav-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.0/PKG-INFO` & `Jvav-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.9.0
+Version: 1.9.1
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.9.0 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.9.1 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Jvav-1.9.0/README.md` & `Jvav-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.0/jvav/cmd.py` & `Jvav-1.9.1/jvav/cmd.py`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.0/jvav/utils.py` & `Jvav-1.9.1/jvav/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1902,103 +1902,14 @@
             return GoogleTranslator(
                 source=from_lang, target=to_lang, proxies=self.proxy_json
             ).translate(text)
         except Exception as e:
             self.log.error(f"TransUtil: 翻译: {e}")
 
 
-class SjsUtil(BaseUtil):
-    BASE_URL = "https://xsijishe.com"
-    BASE_URL_RANK = BASE_URL + "/portal.php?mod=list&catid=2"
-
-    def get_rank_by_nex(self, nex) -> list:
-        """根据标签元素 nex 获取司机社排行榜
-
-        :return 排行榜列表
-        """
-        dd_list = nex.find_all("dd")
-        rank_list = []
-        for dd in dd_list:
-            try:
-                img = dd.find("img")["src"]
-                url = dd.find("h5").a["href"]
-                title = dd.find("h5").a.text
-                rank_list.append(
-                    {"img": img, "url": f"{SjsUtil.BASE_URL}/{url}", "title": title}
-                )
-            except Exception:
-                pass
-        return rank_list
-
-    def get_rank_by_nex_for_cosimg(self, nex) -> list:
-        """根据标签元素 nex 获取司机社排行榜 (cosimg)
-
-        :return 排行榜列表
-        """
-        dd_list = nex.find_all("dd")
-        rank_list = []
-        for dd in dd_list:
-            try:
-                img = dd.find("img")["src"]
-                url = dd.find("a")["href"]
-                title = dd.find("h5").text
-                rank_list.append(
-                    {"img": img, "url": f"{SjsUtil.BASE_URL}/{url}", "title": title}
-                )
-            except Exception:
-                pass
-        return rank_list
-
-    def get_rank(self, rank_type=1) -> typing.Tuple[int, list]:
-        """获取司机社排行榜
-
-        :param int rank_type: 排行榜类型 1.最新帖子 2.cos视图榜 3.动漫阅读榜 4.论坛帖子排行 5.热门出处悬赏
-        :return typing.Tuple[int, list]: 状态码和排行榜列表
-        列表单位结构:
-        {
-            "img": "",
-            "url": "",
-            "title": ""
-        }
-        """
-        code, resp = self.send_req(url=SjsUtil.BASE_URL_RANK)
-        if code != 200:
-            return code, None
-        try:
-            soup = self.get_soup(resp)
-            nex_ranklist_box = soup.find(class_="nex_ranklist_box")  # 最新帖子
-            nex_rank_cosimg = soup.find(class_="nex_rank_cosimg")  # cos视图榜
-            nex_mangalist = soup.find(class_="nex_mangalist")  # 动漫阅读榜
-            nex_threadbox = soup.find(class_="nex_threadbox")  # 论坛帖子排行
-            nex_artbox = soup.find(class_="nex_artbox")  # 热门出处悬赏
-            if rank_type == 1:
-                nex = nex_ranklist_box
-            elif rank_type == 2:
-                nex = nex_rank_cosimg
-            elif rank_type == 3:
-                nex = nex_mangalist
-            elif rank_type == 4:
-                nex = nex_threadbox
-            elif rank_type == 5:
-                nex = nex_artbox
-            else:
-                nex = nex_ranklist_box
-            if nex:
-                if rank_type == 2:
-                    rank_list = self.get_rank_by_nex_for_cosimg(nex)
-                else:
-                    rank_list = self.get_rank_by_nex(nex)
-                return 200, rank_list
-            else:
-                return 404, None
-        except Exception as e:
-            self.log.error(f"SjsUtil: 获取司机社排行榜失败: {e}")
-            return 404, None
-
-
 class SgpUtil(BaseUtil):
     BASE_URL = "http://www.fpie2.com"
     BASE_URL_SEARCH = "https://api.cbbee0.com/v1_2/articleSearch"
     BASE_URL_DETAIL = f"{BASE_URL}/play-details/1/"
 
     def get_video_by_av_id(self, av_id: str) -> typing.Tuple[int, str]:
         headers = {
```

### Comparing `Jvav-1.9.0/setup.py` & `Jvav-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requires = [i.strip() for i in r]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="Jvav",
-    version="1.9.0",
+    version="1.9.1",
     description="Useful tools for Jav.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/akynazh/jvav",
     download_url="https://github.com/akynazh/jvav/releases/latest",
     author="akynazh",
     author_email="akynazh@gmail.com",
```

