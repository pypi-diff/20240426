# Comparing `tmp/Fr1997v011-1.3.1.tar.gz` & `tmp/Fr1997v011-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.3.1.tar", last modified: Wed Apr 24 10:40:21 2024, max compression
+gzip compressed data, was "Fr1997v011-1.3.6.tar", last modified: Thu Apr 25 09:03:52 2024, max compression
```

## Comparing `Fr1997v011-1.3.1.tar` & `Fr1997v011-1.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 10:40:21.290806 Fr1997v011-1.3.1/
-drwxrwxrwx   0        0        0        0 2024-04-24 10:40:21.266722 Fr1997v011-1.3.1/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-24 10:40:20.000000 Fr1997v011-1.3.1/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-24 10:40:21.000000 Fr1997v011-1.3.1/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 10:40:20.000000 Fr1997v011-1.3.1/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-24 10:40:20.000000 Fr1997v011-1.3.1/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-24 10:40:20.000000 Fr1997v011-1.3.1/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-24 10:40:21.288285 Fr1997v011-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-24 02:47:42.000000 Fr1997v011-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 10:40:21.271737 Fr1997v011-1.3.1/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.3.1/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:40:21.281767 Fr1997v011-1.3.1/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       63 2024-04-23 10:58:22.000000 Fr1997v011-1.3.1/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   169672 2024-04-24 10:40:19.000000 Fr1997v011-1.3.1/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:40:21.284769 Fr1997v011-1.3.1/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.3.1/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-24 10:40:21.290806 Fr1997v011-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-24 02:39:08.000000 Fr1997v011-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:03:52.574529 Fr1997v011-1.3.6/
+drwxrwxrwx   0        0        0        0 2024-04-25 09:03:52.563980 Fr1997v011-1.3.6/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-25 09:03:52.000000 Fr1997v011-1.3.6/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-25 09:03:52.000000 Fr1997v011-1.3.6/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 09:03:52.000000 Fr1997v011-1.3.6/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 07:26:41.000000 Fr1997v011-1.3.6/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-25 09:03:52.000000 Fr1997v011-1.3.6/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-25 09:03:52.573529 Fr1997v011-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-25 03:54:38.000000 Fr1997v011-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 09:03:52.566482 Fr1997v011-1.3.6/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.3.6/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:03:52.569529 Fr1997v011-1.3.6/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.3.6/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   172885 2024-04-25 09:03:50.000000 Fr1997v011-1.3.6/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:03:52.571529 Fr1997v011-1.3.6/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.3.6/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 09:03:52.574529 Fr1997v011-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-25 03:54:32.000000 Fr1997v011-1.3.6/setup.py
```

### Comparing `Fr1997v011-1.3.1/LICENSE` & `Fr1997v011-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.3.1/README.md` & `Fr1997v011-1.3.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.3.1.tar.gz
+pip install dist/Fr1997v011-1.3.6.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.3.1/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.3.6/fr1997_mode/mode_func/all_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from urllib import parse  # 三位
 from urllib.parse import quote  # 两位
 from urllib.parse import urlparse, quote
 
 # 腾讯云cos  pip install -U cos-python-sdk-v5
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
+from django.http import JsonResponse
 
 """
     pip3 install redis
     pip3 install pymysql
     pip3 install elasticsearch
     pip3 install python-memcached
     pip3 install PyExecJS
@@ -3775,18 +3776,26 @@
             print('Fr包err cnd获取路径失败', E)
 
 
 # FastGpt
 class FastGptAuto:
 
     def __init__(self, **kwargs):
-        self.conn_tp = kwargs.get('conn_tp', 1)  # 2测试
+        self.run_path = kwargs.get('run_path', 2)  # 2测试 01正式
         self.avatar = "/icon/logo.svg"
-        self.base_url = 'https://aitest.dso100.com/api'
-        self.authorization = 'fastgpt-nE4z8uvJrrh5N1OvvdjDFG7Y055Rj9xVVXKeVSghM1cFAr1zXRUMdxm5v7a6pC'
+
+        # 正式|测试
+        if self.run_path == 2:
+            self.conn_tp = 0
+            self.base_url = 'http://101.35.29.36:3020/api'
+            self.authorization = 'fastgpt-xBfm0yXYOSTIRNl4JBGAKBKk5Ga6klbezPhWknV7gsTiUdsQOVVkvcVjtrYioRrp'
+        else:
+            self.conn_tp = ModeFunc().path
+            self.base_url = 'https://aitest.dso100.com/api'
+            self.authorization = 'fastgpt-nE4z8uvJrrh5N1OvvdjDFG7Y055Rj9xVVXKeVSghM1cFAr1zXRUMdxm5v7a6pC'
 
         self.user_text_table = 'cd_douyin_user_video_text'
         self.es_user_text_table = 'douyin_user_video_text'
         self.all_dataset_table = 'cd_fast_article_dataset'
 
     # 通过后台生成的token https://aitest.dso100.com/account?currentTab=apikey
     def get_header(self):
@@ -3830,21 +3839,36 @@
                 data_data = response.json()
                 code = data_data['code']
                 if code == 200:
                     return data_data
         return {'code': 500}
 
     # 应用 修改 【知识库】 【提示词】
-    def app_update(self, app_id, dataset_id, cue_word):
+    def app_update(self, app_id, dataset_ids, cue_word):
         sql = 'SELECT name,json_data FROM `cd_python_json` where `name` = "fastgpt_app_update_json"'
         all_data = mode_pro.mysql_db(method="s", table="cd_python_json", sql=sql)
         for at in all_data:
             fastgpt_app_create_json = json.loads(at[1])
             fastgpt_app_create_json['modules'][2]['inputs'][7]['value'] = cue_word
-            fastgpt_app_create_json['modules'][3]['inputs'][1]['value'][0]['datasetId'] = dataset_id
+            # dataset_ids = '662732843f901b42fce83f3c,6627514c3f901b42fce89e27'
+            dataset_ids_list = dataset_ids.split(',')
+            for dt_id in dataset_ids_list:
+                fastgpt_app_create_json['modules'][3]['inputs'][1]['value'].append({
+                    "datasetId": dt_id,
+                    "vectorModel": {
+                        "model": "text-embedding-ada-002",
+                        "name": "Embedding-2",
+                        "inputPrice": 0,
+                        "outputPrice": 0,
+                        "defaultToken": 700,
+                        "maxToken": 3000,
+                        "weight": 100,
+                        "defaultConfig": {}
+                    }
+                })
             response = requests.post(f'{self.base_url}/core/app/update?appId={app_id}', headers=self.get_token_header(),
                                      json=fastgpt_app_create_json)
             if response.status_code == 200:
                 data_data = response.json()
                 code = data_data['code']
                 if code == 200:
                     return data_data
@@ -4214,14 +4238,81 @@
                         })
                         continue
 
         if save_data:
             mode_pro.mysql_db(method='up', table=self.all_dataset_table, conn_tp=self.conn_tp, save_data=save_data)
 
 
+class RetJson:
+
+    @classmethod
+    def data_list(cls, data):
+        if data is None:
+            return []
+        return data
+
+    @classmethod
+    def data_dict(cls, data):
+        if data is None:
+            return {}
+        return data
+
+    @classmethod
+    def ret_json(cls, code, msg, data_list, data_dict, code_remark=None):
+        data_list = cls.data_list(data_list)
+        data_dict = cls.data_dict(data_dict)
+        if code_remark:
+            return JsonResponse({
+                'code': code,
+                'msg': msg,
+                'code_remark': code_remark,
+                'data_list': data_list,
+                'data_dict': data_dict
+            })
+        return JsonResponse({
+            'code': code,
+            'msg': msg,
+            'data_list': data_list,
+            'data_dict': data_dict
+        })
+
+    @classmethod
+    def code200(cls, msg='ok', data_list=None, data_dict=None):
+        print(data_list, data_dict)
+        return cls.ret_json(200, msg, data_list, data_dict)
+
+    @classmethod
+    def code201(cls, msg='ok', data_list=None, data_dict=None):
+        return cls.ret_json(201, msg, data_list, data_dict, 201)
+
+    @classmethod
+    def code202(cls, msg='ok', data_list=None, data_dict=None):
+        return cls.ret_json(202, msg, data_list, data_dict, 202)
+
+    @classmethod
+    def code400(cls, msg='err', data_list=None, data_dict=None):
+        return cls.ret_json(400, msg, data_list, data_dict)
+
+    @classmethod
+    def code404(cls, msg='err', data_list=None, data_dict=None):
+        return cls.ret_json(404, msg, data_list, data_dict, 404)
+
+    @classmethod
+    def code500(cls, msg='err', data_list=None, data_dict=None):
+        return cls.ret_json(500, msg, data_list, data_dict)
+
+    @classmethod
+    def code501(cls, msg='err', data_list=None, data_dict=None):
+        return cls.ret_json(501, msg, data_list, data_dict, 501)
+
+    @classmethod
+    def code502(cls, msg='err', data_list=None, data_dict=None):
+        return cls.ret_json(502, msg, data_list, data_dict, 502)
+
+
 # myself 高阳本人信息
 class MyGy:
 
     def __init__(self, **kwargs):
         self.fr1997_config_dict = cache_get("fr1997_config_dict")
 
     # 获取信息
@@ -4239,13 +4330,14 @@
 mode_text = TextJike()  # 文本处理
 mode_data = DataJike()  # 数据处理
 mode_spider = SpiderJike()  # 数据请求
 mode_django = DjangoJike()  # django配置
 mode_douyin = DouyinJike()  # douyin配置
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
-mode_fastgpt = FastGptAuto()  # fastgpt
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
+mode_fastgpt = FastGptAuto(run_path=1)  # fastgpt
+mode_fastgpt_test = FastGptAuto(run_path=2)  # fastgpt test
 
 mode_pro = ModeFunc()  # main
```

