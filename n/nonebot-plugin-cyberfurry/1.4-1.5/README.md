# Comparing `tmp/nonebot_plugin_cyberfurry-1.4.tar.gz` & `tmp/nonebot_plugin_cyberfurry-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cyberfurry-1.4.tar", last modified: Wed Apr 24 16:08:43 2024, max compression
+gzip compressed data, was "nonebot_plugin_cyberfurry-1.5.tar", last modified: Fri Apr 26 14:48:30 2024, max compression
```

## Comparing `nonebot_plugin_cyberfurry-1.4.tar` & `nonebot_plugin_cyberfurry-1.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:08:43.054686 nonebot_plugin_cyberfurry-1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44121 2024-04-24 16:08:43.054686 nonebot_plugin_cyberfurry-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:08:43.050686 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/callapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberfurry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberfurrymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberinit.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/plugins_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:08:43.054686 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44121 2024-04-24 16:08:43.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-24 16:08:43.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:08:43.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 16:08:43.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 16:08:43.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:08:43.054686 nonebot_plugin_cyberfurry-1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:48:30.543987 nonebot_plugin_cyberfurry-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44755 2024-04-26 14:48:30.543987 nonebot_plugin_cyberfurry-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:48:30.539986 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/callapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberauto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberfurry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberfurrymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/plugins_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:48:30.543987 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44755 2024-04-26 14:48:30.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-26 14:48:30.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:48:30.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-26 14:48:30.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 14:48:30.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:48:30.543987 nonebot_plugin_cyberfurry-1.5/setup.cfg
```

### Comparing `nonebot_plugin_cyberfurry-1.4/LICENSE` & `nonebot_plugin_cyberfurry-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.4/PKG-INFO` & `nonebot_plugin_cyberfurry-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.4
+Version: 1.5
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -685,14 +685,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot2
 Requires-Dist: nonebot-plugin-localstore
+Requires-Dist: nonebot-plugin-apscheduler
 Requires-Dist: aiohttp
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-cyberfurry/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/cubstaryow/nonebot-plugin-cyberfurry/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
@@ -712,22 +713,24 @@
 </a>
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 </div>
 
 ## 📖 介绍
 
-官方网站 : [CyberFurry](https://chat.wingmark.cn/)
+官方网站 : [CyberFurry](https://chat.wingmark.cn/ "cyberfurry™")
 
 API申请请通过官方群聊找 群主 申请
 
 ### ⚠ 重要
 
-请务必遵守 [用户协议](https://tailnet.cn/?page=yinyingzc)
+请务必遵守 [用户协议](https://tailnet.cn/?page=yinyingzc "cyberfurry用户协议")
 
+[指令表](#howtouser)
+[配置项](#set)
 
 easycf模型还未填坑,后续更新适配
 
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
@@ -765,32 +768,41 @@
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_cyberfurry"]
 
 </details>
 
 ## ⚙️ 配置
+<a id="set"></a>
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 
 > [!WARNING]
 > 若未配置必填项此插件将不会工作!!!!
 
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cf_appid | 是 | 无 | API的appid |
 | cf_token | 是 | 无 | API的token |
 | cubplugin_datadir | 否 | "" | 插件数据文件夹 |
 | cf_enableistome | 否 | False | 在消息是对bot时是否启用chat |
+| cf_auto | 否 | True | 是否启用主动推送(你今天还没找银影聊天耶.png) |
+| cf_autogrouplist | 否 | [] | 是否启用主动推送(群聊冒泡白名单列表) |
+
+
 
 
 ## 🎉 使用
+<a id="howtouser"></a>
+
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
 | cf刷新对话 | 群员 | 否 | 任意 | 刷新对话 |
- | cf设定模型 | 群员 | 否 | 任意 | 设定使用的yinying模型,注意,此为个人配置 |
- | cf当前模型 | 群员 | 否 | 任意 |  查看当前模型 |
- | cf设定 fur名字 fur种族 | 群员 | 否 | 任意 | 设定传入yinying的自身设定 |
+| cf设定模型 | 群员 | 否 | 任意 | 设定使用的yinying模型,注意,此为个人配置 |
+| cf当前模型 | 群员 | 否 | 任意 |  查看当前模型 |
+| cf模型列表 | 群员 | 否 | 任意 |  查看已加载的模型(包括自定义) |
+| cf设定 fur名字 fur种族 | 群员 | 否 | 任意 | 设定传入yinying的自身设定 |
+| (开启|关闭)对话推送服务 | 群员 | 否 | 私聊 | 让银影每天的(6,12,18,21)点十分找你然后抱怨你不找他聊天(在推送前触发对话则不会在下个时间点推送uwu) |
```

### Comparing `nonebot_plugin_cyberfurry-1.4/README.md` & `nonebot_plugin_cyberfurry-1.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 </a>
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 </div>
 
 ## 📖 介绍
 
-官方网站 : [CyberFurry](https://chat.wingmark.cn/)
+官方网站 : [CyberFurry](https://chat.wingmark.cn/ "cyberfurry™")
 
 API申请请通过官方群聊找 群主 申请
 
 ### ⚠ 重要
 
-请务必遵守 [用户协议](https://tailnet.cn/?page=yinyingzc)
+请务必遵守 [用户协议](https://tailnet.cn/?page=yinyingzc "cyberfurry用户协议")
 
+[指令表](#howtouser)
+[配置项](#set)
 
 easycf模型还未填坑,后续更新适配
 
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
@@ -72,32 +74,41 @@
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_cyberfurry"]
 
 </details>
 
 ## ⚙️ 配置
+<a id="set"></a>
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 
 > [!WARNING]
 > 若未配置必填项此插件将不会工作!!!!
 
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cf_appid | 是 | 无 | API的appid |
 | cf_token | 是 | 无 | API的token |
 | cubplugin_datadir | 否 | "" | 插件数据文件夹 |
 | cf_enableistome | 否 | False | 在消息是对bot时是否启用chat |
+| cf_auto | 否 | True | 是否启用主动推送(你今天还没找银影聊天耶.png) |
+| cf_autogrouplist | 否 | [] | 是否启用主动推送(群聊冒泡白名单列表) |
+
+
 
 
 ## 🎉 使用
+<a id="howtouser"></a>
+
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
 | cf刷新对话 | 群员 | 否 | 任意 | 刷新对话 |
- | cf设定模型 | 群员 | 否 | 任意 | 设定使用的yinying模型,注意,此为个人配置 |
- | cf当前模型 | 群员 | 否 | 任意 |  查看当前模型 |
- | cf设定 fur名字 fur种族 | 群员 | 否 | 任意 | 设定传入yinying的自身设定 |
+| cf设定模型 | 群员 | 否 | 任意 | 设定使用的yinying模型,注意,此为个人配置 |
+| cf当前模型 | 群员 | 否 | 任意 |  查看当前模型 |
+| cf模型列表 | 群员 | 否 | 任意 |  查看已加载的模型(包括自定义) |
+| cf设定 fur名字 fur种族 | 群员 | 否 | 任意 | 设定传入yinying的自身设定 |
+| (开启|关闭)对话推送服务 | 群员 | 否 | 私聊 | 让银影每天的(6,12,18,21)点十分找你然后抱怨你不找他聊天(在推送前触发对话则不会在下个时间点推送uwu) |
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
            # nonebot-plugin-cyberfurry _â¨ nonebotæä»¶ cyberfurry
              ä¸èµåç¼ç¼å¯¹è¯å§~ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç» å®æ¹ç½ç« : [CyberFurry](https://chat.wingmark.cn/
-) APIç³è¯·è¯·éè¿å®æ¹ç¾¤èæ¾ ç¾¤ä¸» ç³è¯· ### â  éè¦
-è¯·å¡å¿éµå® [ç¨æ·åè®®](https://tailnet.cn/?page=yinyingzc)
+"cyberfurryâ¢") APIç³è¯·è¯·éè¿å®æ¹ç¾¤èæ¾ ç¾¤ä¸» ç³è¯· ### â  éè¦
+è¯·å¡å¿éµå® [ç¨æ·åè®®](https://tailnet.cn/?page=yinyingzc
+"cyberfurryç¨æ·åè®®") [æä»¤è¡¨](#howtouser) [éç½®é¡¹](#set)
 easycfæ¨¡åè¿æªå¡«å,åç»­æ´æ°éé ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£
 å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-cyberfurry
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-cyberfurry pdm pdm add nonebot-plugin-cyberfurry
 poetry poetry add nonebot-plugin-cyberfurry conda conda install nonebot-plugin-
@@ -16,14 +17,21 @@
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_cyberfurry"] ##
 âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® > [!WARNING] >
 è¥æªéç½®å¿å¡«é¡¹æ­¤æä»¶å°ä¸ä¼å·¥ä½!!!! | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | cf_appid | æ¯ | æ  |
 APIçappid | | cf_token | æ¯ | æ  | APIçtoken | | cubplugin_datadir | å¦
 | "" | æä»¶æ°æ®æä»¶å¤¹ | | cf_enableistome | å¦ | False |
-å¨æ¶æ¯æ¯å¯¹botæ¶æ¯å¦å¯ç¨chat | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ |
-æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | /
-chat /cf /yy | ç¾¤å | å¦ | ä»»æ | è§¦åå¯¹è¯ | | cfå·æ°å¯¹è¯ | ç¾¤å
-| å¦ | ä»»æ | å·æ°å¯¹è¯ | | cfè®¾å®æ¨¡å | ç¾¤å | å¦ | ä»»æ |
+å¨æ¶æ¯æ¯å¯¹botæ¶æ¯å¦å¯ç¨chat | | cf_auto | å¦ | True |
+æ¯å¦å¯ç¨ä¸»å¨æ¨é(ä½ ä»å¤©è¿æ²¡æ¾é¶å½±èå¤©è¶.png) | |
+cf_autogrouplist | å¦ | [] | æ¯å¦å¯ç¨ä¸»å¨æ¨é
+(ç¾¤èåæ³¡ç½åååè¡¨) | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé
+| éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | /chat /cf
+/yy | ç¾¤å | å¦ | ä»»æ | è§¦åå¯¹è¯ | | cfå·æ°å¯¹è¯ | ç¾¤å | å¦ |
+ä»»æ | å·æ°å¯¹è¯ | | cfè®¾å®æ¨¡å | ç¾¤å | å¦ | ä»»æ |
 è®¾å®ä½¿ç¨çyinyingæ¨¡å,æ³¨æ,æ­¤ä¸ºä¸ªäººéç½® | | cfå½åæ¨¡å |
-ç¾¤å | å¦ | ä»»æ | æ¥çå½åæ¨¡å | | cfè®¾å® furåå­ furç§æ |
-ç¾¤å | å¦ | ä»»æ | è®¾å®ä¼ å¥yinyingçèªèº«è®¾å® |
+ç¾¤å | å¦ | ä»»æ | æ¥çå½åæ¨¡å | | cfæ¨¡ååè¡¨ | ç¾¤å | å¦ |
+ä»»æ | æ¥çå·²å è½½çæ¨¡å(åæ¬èªå®ä¹) | | cfè®¾å® furåå­
+furç§æ | ç¾¤å | å¦ | ä»»æ | è®¾å®ä¼ å¥yinyingçèªèº«è®¾å® | |
+(å¼å¯|å³é­)å¯¹è¯æ¨éæå¡ | ç¾¤å | å¦ | ç§è | è®©é¶å½±æ¯å¤©ç
+(6,12,18,21)ç¹ååæ¾ä½ ç¶åæ±æ¨ä½ ä¸æ¾ä»èå¤©
+(å¨æ¨éåè§¦åå¯¹è¯åä¸ä¼å¨ä¸ä¸ªæ¶é´ç¹æ¨éuwu) |
```

### Comparing `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/__init__.py` & `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,11 +22,20 @@
     # 插件配置项类，如无需配置可不填写。
 
     supported_adapters={"~onebot.v11" , "~telegram"},
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
 if config.cf_appid == "" or config.cf_token == "" :
-    logger.opt(colors=True).error("cyberfurry缺失核心配置!!!!!取消载入核心!!!")
+    logger.opt(colors=True).error(
+        "cyberfurry缺失核心配置!!!!!取消载入核心!!!"
+    )
 else:
     from .cyberinit import *
-    from .cyberhistory import *
+    from .cyberhistory import * 
+    
+if config.cf_auto:
+    from .cyberauto import *
+else:
+    logger.opt(colors=True).debug(
+        "<red>cyberfurry自动对话推送服务已关闭</red>"
+    )
```

### Comparing `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/callapi.py` & `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/callapi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberfurry.py` & `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberfurry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .data_source import aidata_demo, userdata_demo
 from .jsondata import (
     getdate, getqqdata,
     defqqname, defqqmodel,
     datetime, writehistory,
     loaddata, savedata,
-    driver
+    driver , setqqpushstatus
 )
 import time
 import json
 
 from loguru import logger
 
 from .callapi import api
@@ -142,20 +142,7 @@
                 cls.getsettimes(cls, user_id, settime=0, init=True)
             return content, times
     pass
 
 
 cf = cyberfurry()
 
-
-cfConAgeMap = {
-    "可爱兽太": 'child',
-    "青年": 'young',
-    "成熟稳重": 'adult'
-}
-cfConStyleMap = {
-    "活泼": 'vivid',
-    "富有情感": 'sentiment',
-    "助理": 'assistant',
-    "冷酷无情": 'chilly',
-    "社恐": 'social_anxiety'
-}
```

### Comparing `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberfurrymodel.py` & `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberfurrymodel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import json
 import os
+
+from loguru import logger
 from .config import config
 from .data_source import aidata_demo ,userdata_demo
 
 promptfile = os.path.dirname(__file__)+"/systemprompt.json"
 def getdata():
-    with open(promptfile, "r", encoding="utf-8") as f:
-        data = json.loads(f.read())
+    try:
+        with open(promptfile, "r", encoding="utf-8") as f:
+            data = json.loads(f.read())
+    except:
+        logger.warning("获取插件自带prompt文件数据出现错误!")
+        data = {}
     return data
 def loadcfprompt():
     data = getdata()
     redata = {}
     for temp in data:
         if temp['model'] == "cyberfurry":
             key = temp['model'] + "-" + temp["name"]
```

### Comparing `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberhistory.py` & `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberhistory.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberinit.py` & `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberinit.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,33 +24,42 @@
     rule=to_me() & Rule(is_enable),
     priority=900
 )
 
 run = on_command(
     "/chat",
     aliases={"/yy","/cf"} ,
-    block=True,
+    block=config.cf_enableistome,
     priority=25
 )
 init = on_command(
     "cf刷新对话",
     aliases={ "cf初始化"} ,
+    block=config.cf_enableistome,
     priority=25
 )
 set = on_command(
     "cf设定模型",
     aliases={ "cf切换模型"} ,
+    block=config.cf_enableistome,
     priority=25
 )
 getset = on_command(
     "cf当前模型",
+    block=config.cf_enableistome,
+    priority=25
+)
+getmodellist = on_command(
+    "cf模型列表",
+    block=config.cf_enableistome,
     priority=25
 )
 setuser = on_command(
     "cf设定",
+    block=config.cf_enableistome,
     priority=25
 )
 
 
 def checkmsg(word):
     blackkey = [
         "草你","草我","操","艹","撅","涩涩",
@@ -98,14 +107,15 @@
     userinfo = await bot.get_stranger_info(user_id=user_id)
     name = userinfo.get("nickname","未知")
     if len(msg) > 75:
         await matcher.send(MessageSegment.reply(event.message_id)+"太长力xw")
         return 0 
     retmsg , times = await cf.chat(user_id,name,msg)
     maxtimes = cf.maxtimes
+    setqqpushstatus(user_id, False)
     await matcher.send(
         MessageSegment.reply(event.message_id) +
         retmsg +
         (f"\n({times}/{maxtimes},将开启新对话)" if times >=maxtimes else f"\n({times}/{maxtimes}轮对话)")
     )
     
 @autorun.handle()
@@ -161,14 +171,23 @@
 ):
     user_id = str(event.user_id)
     msg="[幼龙云V5]"
     data = getqqdata(user_id)
     msg +=f"当前模型[{data['model']}]"
     await matcher.send(msg)
 
+@getmodellist.handle()
+async def cyberfurrygetmodellist(
+    event:MessageEvent,matcher:Matcher
+):
+    modellist = list(cf.model.keys())
+    msg =f"[cyberfurry]可用模型\n"
+    msg += "\n".join(modellist)
+    await matcher.send(msg)
+
 @set.handle()
 async def cyberfurryset(
     event:MessageEvent,matcher:Matcher,
     data: list = CommandArg()
 ):
     modelname = str(data[0])
     user_id = str(event.user_id)
@@ -176,15 +195,16 @@
     if cf.model.get(modelname,None) != None:
         try:
             defqqmodel(user_id,modelname)
         except:
             defqqname(user_id,{
             "name":"未知",
             "ethnic":"狼",
-            "model":modelname
+            "model":modelname,
+            "push" : False
             })
             msg +="\nWARN-你还未设置设定,请尽快设置\n"
         cf.initchat(user_id)
         msg +=f"设定模型[{modelname}]成功\n(已自动刷新对话)"
     else:
         msg +="模型不存在"
     await matcher.send(msg)
```

### Comparing `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/jsondata.py` & `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/jsondata.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,45 @@
 from loguru import logger
 from .plugins_data import initdata,wdata,rdata,driver,data_dir
 import os
 from datetime import datetime
 jsonname = "cyberfurry.json"
+tempname = "cybertemp.json"
 txtdir = "cyberfurry"
 bashdata = {
     "status":1,
     "userdata":{},
-    "userchat":{}
+    "autopush":[]
 }
 initdata(jsonname,bashdata)
+initdata(tempname,{})
+
+
+#====================推送服务========================
+
+def loadpushlist():
+    temp = rdata(jsonname)
+    return temp.get("autopush",[])
+
+def savepushlist(data):
+    temp = rdata(jsonname)
+    temp["autopush"]=data
+    wdata(jsonname,temp)
+
+def setqqpushstatus(
+    user_id :int|str,
+    push :bool = True,
+):
+    
+    temp = rdata(jsonname)
+    temp['userdata'][str(user_id)]["push"]=push
+    wdata(jsonname,temp)
+
+
+#====================历史对话文件存储 测试版========================
 txt_dir =  data_dir / txtdir
 if not os.path.isdir(txt_dir):
     os.mkdir(txt_dir)
 
 def writehistory(
     chat_id:str,
     text:str
@@ -45,25 +71,27 @@
     file_path=txt_dir / f"{user_id}"
     filelist = os.listdir(file_path)
     if filename+".txt" in filelist:
         return file_path / (filename+".txt")
     else:
         return False
 
+#==================== 核心数据文件存储 ========================
 def getdate():
-    now = datetime.now() # current date and time
+    now = datetime.now()
     date_time = now.strftime("%y%m%d")
     return (date_time)
 
 def defqqname(
     user_id :int|str,
     userdata :dict = {
         "name":"未知",
         "ethnic":"狼",
-        "model" :"yinyingllm-v2"
+        "model" :"yinyingllm-v2",
+        "push" : False
     }
 ):
     temp = rdata(jsonname)
     temp['userdata'][str(user_id)]=userdata
     wdata(jsonname,temp)
     return True
 
@@ -80,19 +108,21 @@
 def getqqdata(
     user_id :int|str,
 ):
     temp = rdata(jsonname)
     return temp['userdata'].get(str(user_id),{
         "name":"未知",
         "ethnic":"狼",
-        "model" :"yinyingllm-v2"
+        "model" :"yinyingllm-v2",
+        "push" : False
         }
     )
 
+#==================== 重启时的状态重启 ========================
 def loaddata():
-    temp = rdata(jsonname)
-    return temp.get("userchat",{})
+    temp = rdata(tempname)
+    return temp
 
 def savedata(data):
-    temp = rdata(jsonname)
-    temp["userchat"]=data
-    wdata(jsonname,temp)
+    temp = rdata(tempname)
+    temp=data
+    wdata(tempname,temp)
```

### Comparing `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/plugins_data.py` & `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/plugins_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     else:
         #os.mkdir(path_name)
         os.mkdir(data_dir)
         logger.opt(colors=True).debug(f"[plugin_data]初始化根目录\<{path_name}\>")
 
 def initdata(
     conf_name,
-    bashdata:dict={"status":1}
+    bashdata:dict | list={"status":1}
 ):
     conf_path = Path(data_dir / conf_name).absolute()
     config_init(conf_path,conf_name,"plugin_data",bashdata)
     return True
 
 def rdata(
     conf_name
@@ -49,15 +49,15 @@
         f.write(json.dumps(data, indent=4,ensure_ascii=False))
     return True
 
 def config_init(
     _path_ ,
     conf_name:str ,
     module_name:str="None" ,
-    data:dict={"status":1}
+    data:dict | list ={"status":1}
 ):
     if _path_.is_file():
         logger.opt(colors=True).debug(f"[cubutil]>>><W>{module_name}</>>>>{conf_name}-OK!")
     else:
         logger.opt(colors=True).debug(f"[cubutil]>>><W>{module_name}</>>>>Create-{conf_name}!")
         with open(_path_, "w", encoding="utf-8") as f:
             f.write(json.dumps(data, indent=4))
```

### Comparing `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/PKG-INFO` & `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.4
+Version: 1.5
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -685,14 +685,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot2
 Requires-Dist: nonebot-plugin-localstore
+Requires-Dist: nonebot-plugin-apscheduler
 Requires-Dist: aiohttp
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-cyberfurry/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/cubstaryow/nonebot-plugin-cyberfurry/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
@@ -712,22 +713,24 @@
 </a>
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 </div>
 
 ## 📖 介绍
 
-官方网站 : [CyberFurry](https://chat.wingmark.cn/)
+官方网站 : [CyberFurry](https://chat.wingmark.cn/ "cyberfurry™")
 
 API申请请通过官方群聊找 群主 申请
 
 ### ⚠ 重要
 
-请务必遵守 [用户协议](https://tailnet.cn/?page=yinyingzc)
+请务必遵守 [用户协议](https://tailnet.cn/?page=yinyingzc "cyberfurry用户协议")
 
+[指令表](#howtouser)
+[配置项](#set)
 
 easycf模型还未填坑,后续更新适配
 
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
@@ -765,32 +768,41 @@
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_cyberfurry"]
 
 </details>
 
 ## ⚙️ 配置
+<a id="set"></a>
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 
 > [!WARNING]
 > 若未配置必填项此插件将不会工作!!!!
 
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cf_appid | 是 | 无 | API的appid |
 | cf_token | 是 | 无 | API的token |
 | cubplugin_datadir | 否 | "" | 插件数据文件夹 |
 | cf_enableistome | 否 | False | 在消息是对bot时是否启用chat |
+| cf_auto | 否 | True | 是否启用主动推送(你今天还没找银影聊天耶.png) |
+| cf_autogrouplist | 否 | [] | 是否启用主动推送(群聊冒泡白名单列表) |
+
+
 
 
 ## 🎉 使用
+<a id="howtouser"></a>
+
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
 | cf刷新对话 | 群员 | 否 | 任意 | 刷新对话 |
- | cf设定模型 | 群员 | 否 | 任意 | 设定使用的yinying模型,注意,此为个人配置 |
- | cf当前模型 | 群员 | 否 | 任意 |  查看当前模型 |
- | cf设定 fur名字 fur种族 | 群员 | 否 | 任意 | 设定传入yinying的自身设定 |
+| cf设定模型 | 群员 | 否 | 任意 | 设定使用的yinying模型,注意,此为个人配置 |
+| cf当前模型 | 群员 | 否 | 任意 |  查看当前模型 |
+| cf模型列表 | 群员 | 否 | 任意 |  查看已加载的模型(包括自定义) |
+| cf设定 fur名字 fur种族 | 群员 | 否 | 任意 | 设定传入yinying的自身设定 |
+| (开启|关闭)对话推送服务 | 群员 | 否 | 私聊 | 让银影每天的(6,12,18,21)点十分找你然后抱怨你不找他聊天(在推送前触发对话则不会在下个时间点推送uwu) |
```

### Comparing `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt` & `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 nonebot_plugin_cyberfurry/__init__.py
 nonebot_plugin_cyberfurry/callapi.py
 nonebot_plugin_cyberfurry/config.py
+nonebot_plugin_cyberfurry/cyberauto.py
 nonebot_plugin_cyberfurry/cyberfurry.py
 nonebot_plugin_cyberfurry/cyberfurrymodel.py
 nonebot_plugin_cyberfurry/cyberhistory.py
 nonebot_plugin_cyberfurry/cyberinit.py
 nonebot_plugin_cyberfurry/data_source.py
 nonebot_plugin_cyberfurry/jsondata.py
 nonebot_plugin_cyberfurry/plugins_data.py
```

### Comparing `nonebot_plugin_cyberfurry-1.4/pyproject.toml` & `nonebot_plugin_cyberfurry-1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-cyberfurry"
-version = "1.4"
+version = "1.5"
 description = "nonebot插件 cyberfurry-与赛博狼狼对话吧~"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
@@ -15,12 +15,13 @@
   "Programming Language :: Python"
 ]
 
 dependencies = [
   "nonebot-adapter-onebot",
   "nonebot2",
   "nonebot-plugin-localstore",
+  "nonebot-plugin-apscheduler",
   "aiohttp"
 ]
 
 [project.urls]
 repository = "https://github.com/cubstaryow/nonebot-plugin-cyberfurry"
```

