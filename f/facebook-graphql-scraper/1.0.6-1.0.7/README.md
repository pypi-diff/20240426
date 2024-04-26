# Comparing `tmp/facebook-graphql-scraper-1.0.6.tar.gz` & `tmp/facebook-graphql-scraper-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-1.0.6.tar", last modified: Tue Apr  9 11:38:40 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-1.0.7.tar", last modified: Fri Apr 26 08:57:21 2024, max compression
```

## Comparing `facebook-graphql-scraper-1.0.6.tar` & `facebook-graphql-scraper-1.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 11:38:40.368506 facebook-graphql-scraper-1.0.6/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.6/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     5413 2024-04-09 11:38:40.368268 facebook-graphql-scraper-1.0.6/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     4925 2024-04-09 11:37:14.000000 facebook-graphql-scraper-1.0.6/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 11:38:40.365899 facebook-graphql-scraper-1.0.6/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     5413 2024-04-09 11:38:40.000000 facebook-graphql-scraper-1.0.6/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      662 2024-04-09 11:38:40.000000 facebook-graphql-scraper-1.0.6/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-09 11:38:40.000000 facebook-graphql-scraper-1.0.6/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-09 11:38:40.000000 facebook-graphql-scraper-1.0.6/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 11:38:40.366450 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 11:38:40.366684 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/base/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     4816 2024-04-03 08:03:10.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 11:38:40.367114 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/pages/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     4903 2024-04-03 10:04:53.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/pages/page_optional.py
--rw-r--r--   0 renren     (501) staff       (20)     1257 2024-04-09 11:37:14.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/test_program.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 11:38:40.367353 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/tests/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/tests/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 11:38:40.367909 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/utils/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3504 2024-04-09 11:37:14.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-1.0.6/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-09 11:38:40.368761 facebook-graphql-scraper-1.0.6/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)      863 2024-04-09 11:37:14.000000 facebook-graphql-scraper-1.0.6/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.108841 facebook-graphql-scraper-1.0.7/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.7/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     7036 2024-04-26 08:57:21.108485 facebook-graphql-scraper-1.0.7/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     6548 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.103835 facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     7036 2024-04-26 08:57:21.000000 facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      657 2024-04-26 08:57:21.000000 facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-26 08:57:21.000000 facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-26 08:57:21.000000 facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.104665 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.105337 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/base/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     1367 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/example.py
+-rw-r--r--   0 renren     (501) staff       (20)     9668 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.106037 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/pages/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     4746 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/pages/page_optional.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.106520 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/tests/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/tests/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.107733 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     2883 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3813 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     6324 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-26 08:57:21.108959 facebook-graphql-scraper-1.0.7/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)      863 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/setup.py
```

### Comparing `facebook-graphql-scraper-1.0.6/LICENSE` & `facebook-graphql-scraper-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.6/PKG-INFO` & `facebook-graphql-scraper-1.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 1.0.6
+Version: 1.0.7
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/FB_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -38,134 +38,143 @@
 - **Pleas setup driver path at first**
 - **Log in with your account credentials**: login facebook account
 - **Without logging in**: Without logging in, click the X icon to 
 - **Difference**: The difference between these two methods is that for some personal accounts, you cannot browse the user's posts without logging into a Facebook account.
 
 ```python
 # -*- coding: utf-8 -*-
-import os
 from fb_graphql_scraper.facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
-from dotenv import load_dotenv
 
-## Without logging in account version
-facebook_user_name = "KaiCenatOfficial"
-facebook_user_id = "100087298771006"
-# Please setup your driver path
-driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
-url = "https://www.facebook.com/"
-res = fb_graphql_scraper.get_user_posts(
-    fb_username_or_userid=facebook_user_name, 
-    loop_times=50,
-    driver_path=driver_path,
-)
-res
-
-# ## Load account info
-# load_dotenv()
-# fb_account = os.getenv("FBACCOUNT") # Facebook帳號密碼
-# pwd = os.getenv("FBPASSWORD")
-## Log in account version.
-# facebook_user_name = "KaiCenatOfficial"
-# # facebook_user_id = "100087298771006"
-# # Please setup your driver path
-# driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
-# url = "https://www.facebook.com/"
-# res = fb_graphql_scraper.get_user_posts(
-#     fb_username_or_userid=facebook_user_name, 
-#     loop_times=50,
-#     driver_path=driver_path,
-#     fb_account=fb_account,
-#     pwd=pwd
-# )
-# res
+
+## Example.1 - without logging in
+if __name__ == "__main__":
+    facebook_user_name = "love.yuweishao"
+    facebook_user_id = "100044253168423"
+    days_limit = 30 # Number of days within which to scrape posts
+    driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver" 
+    fb_spider = fb_graphql_scraper(driver_path=driver_path)
+    res = fb_spider.get_user_posts(fb_username_or_userid=facebook_user_name, days_limit=days_limit,display_progress=True)
+    print(res)
+
+
+## Example.2 - login in your facebook account to collect data
+# if __name__ == "__main__":
+    # facebook_user_name = "love.yuweishao"
+    # facebook_user_id = "100044253168423"
+    # fb_account = "facebook_account"
+    # fb_pwd = "facebook_paswword"
+    # days_limit = 30 # Number of days within which to scrape posts
+    # driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver" 
+    # fb_spider = fb_graphql_scraper(fb_account=fb_account,fb_pwd=fb_pwd,driver_path=driver_path)
+    # res = fb_spider.get_user_posts(fb_username_or_userid=facebook_user_name, days_limit=days_limit,display_progress=True)
+    # print(res)
+    
+
+
 ```
 
 ### Optional parameters
 
 - **fb_username_or_userid**: groups, fan page, account User-ID or User-Name.
 - **timeout**: How many seconds to wait before timing out. Default is 600.
 - **looptimes**: The program scrolls down Facebook pages..
 
 
-## Post example
+## Result example
 
 ```python
-[{'post_id': '385393337713956',
-  'post_url': 'https://www.facebook.com/385393337713956',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-31 16:00:39'),
-  'published_date2': '2024-03-31',
-  'time': 1711900839,
-  'reaction_count.count': 1224,
-  'comment_rendering_instance.comments.total_count': 37,
-  'share_count.count': 32,
-  'sub_reactions': {'讚': 802,
-   '哈': 406,
-   '大心': 9,
-   '怒': 3,
-   '加油': 2,
-   '哇': 2,
-   '嗚': '0'},
-  'context': 'Druski Plays "What\'s In The Box?" 😱',
-  'video_view_count': 15870},
- {'post_id': '387206327532657',
-  'post_url': 'https://www.facebook.com/387206327532657',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-30 12:01:06'),
-  'published_date2': '2024-03-30',
-  'time': 1711800066,
-  'reaction_count.count': 7153,
-  'comment_rendering_instance.comments.total_count': 154,
-  'share_count.count': 67,
-  'sub_reactions': {'讚': 5674,
-   '哈': 1307,
-   '大心': 121,
-   '嗚': 22,
-   '加油': 21,
-   '哇': 8,
-   '怒': '0'},
-  'context': 'Kai Cenat Asks Tyla Out On A Date 😍 #viralreelsfb #comedy #kaicenat #reelsfb',
-  'video_view_count': 73898},
- {'post_id': '385387707714519',
-  'post_url': 'https://www.facebook.com/385387707714519',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-29 17:01:39'),
-  'published_date2': '2024-03-29',
-  'time': 1711731699,
-  'reaction_count.count': 1000,
-  'comment_rendering_instance.comments.total_count': 47,
-  'share_count.count': 15,
-  'sub_reactions': {'讚': 762,
-   '哈': 194,
-   '大心': 34,
-   '哇': 7,
-   '加油': 2,
-   '嗚': 1,
-   '怒': '0'},
-  'context': 'Chunkz Gets Hypnotised 😱',
-  'video_view_count': 13763},
- {'post_id': '384078261178797',
-  'post_url': 'https://www.facebook.com/384078261178797',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-28 17:00:21'),
-  'published_date2': '2024-03-28',
-  'time': 1711645221,
-  'reaction_count.count': 2587,
-  'comment_rendering_instance.comments.total_count': 77,
-  'share_count.count': 45,
-  'sub_reactions': {'讚': 1905,
-   '哈': 477,
-   '大心': 186,
-   '加油': 15,
-   '哇': 4,
-   '怒': '0',
-   '嗚': '0'},
-  'context': 'Trying The New Ice Spice Drink 😳',
-  'video_view_count': 125605}
-]
+{'fb_username_or_userid': 'love.yuweishao',
+ 'profile': ['任何工作事宜請洽 高先生',
+  '聯絡信箱：hawa00328@gmail.com',
+  '聯絡電話：0975-386-266',
+  '粉絲專頁',
+  ' · 演員',
+  'hawa00328@gmail.com',
+  '1,497,248 位追蹤者'],
+ 'data': [{'post_id': '993720562113040',
+   'post_url': 'https://www.facebook.com/993720562113040',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-24 17:42:14'),
+   'published_date2': '2024-04-24',
+   'time': 1713980534,
+   'reaction_count.count': 3884,
+   'comment_rendering_instance.comments.total_count': 34,
+   'share_count.count': 10,
+   'sub_reactions': {'讚': 3652, '大心': 226, '加油': 5, '哈': 1},
+   'context': 'breathe and life',
+   'video_view_count': nan},
+  {'post_id': '993371658814597',
+   'post_url': 'https://www.facebook.com/993371658814597',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-24 03:55:34'),
+   'published_date2': '2024-04-24',
+   'time': 1713930934,
+   'reaction_count.count': 5043,
+   'comment_rendering_instance.comments.total_count': 41,
+   'share_count.count': 29,
+   'sub_reactions': {'讚': 4632, '大心': 397, '加油': 8, '哇': 4, '哈': 2},
+   'context': '夏季的雨天總讓人難以預期\n每日帶不帶傘的莫非定律 \n空間裡的黏膩和潮濕點滴\n通通都被D-26匯集在一起\n陰晴不定的天氣就交給最懂你的HYD❤️\n\nhttps://reurl.cc/Gjd9nv\nHYD 品宅趣\n#HYD #雙效清淨 #輕量設計 #除濕機',
+   'video_view_count': nan},
+  {'post_id': '992770662208030',
+   'post_url': 'https://www.facebook.com/992770662208030',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-23 04:33:52'),
+   'published_date2': '2024-04-23',
+   'time': 1713846832,
+   'reaction_count.count': 3286,
+   'comment_rendering_instance.comments.total_count': 32,
+   'share_count.count': 5,
+   'sub_reactions': {'讚': 3150, '大心': 61, '加油': 59, '嗚': 13, '哇': 2, '哈': 1},
+   'context': None,
+   'video_view_count': nan},
+  {'post_id': '992336592251437',
+   'post_url': 'https://www.facebook.com/992336592251437',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-22 09:57:32'),
+   'published_date2': '2024-04-22',
+   'time': 1713779852,
+   'reaction_count.count': 11892,
+   'comment_rendering_instance.comments.total_count': 102,
+   'share_count.count': 31,
+   'sub_reactions': {'讚': 11164, '大心': 701, '加油': 15, '哈': 6, '哇': 5, '嗚': 1},
+   'context': '母が撮った写真はとてもきれいです.🌸',
+   'video_view_count': nan},
+  {'post_id': '991854065633023',
+   'post_url': 'https://www.facebook.com/991854065633023',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-21 12:34:39'),
+   'published_date2': '2024-04-21',
+   'time': 1713702879,
+   'reaction_count.count': 5250,
+   'comment_rendering_instance.comments.total_count': 43,
+   'share_count.count': 13,
+   'sub_reactions': {'讚': 4873, '大心': 364, '加油': 6, '哈': 4, '哇': 3},
+   'context': '愛生活也愛工作🖤\n\n@michaelkors \n#MichaelKors',
+   'video_view_count': nan}]
+}
 ```
 
 ### Notes
 - If you choose to collect data by logging into your account, you may face the risk of your account being blocked, even if this program only scrolls through Facebook web pages.
 - Reaction Categories (EN): [`like`, `love`, `haha`, `sorry`, `wow`, `angry`, `care`]
 - Reaction Categories (TW): [`讚`, `哈`, `怒`, `大心`, `加油`, `哇`, `嗚`]
```

### Comparing `facebook-graphql-scraper-1.0.6/README.md` & `facebook-graphql-scraper-1.0.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -23,134 +23,143 @@
 - **Pleas setup driver path at first**
 - **Log in with your account credentials**: login facebook account
 - **Without logging in**: Without logging in, click the X icon to 
 - **Difference**: The difference between these two methods is that for some personal accounts, you cannot browse the user's posts without logging into a Facebook account.
 
 ```python
 # -*- coding: utf-8 -*-
-import os
 from fb_graphql_scraper.facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
-from dotenv import load_dotenv
 
-## Without logging in account version
-facebook_user_name = "KaiCenatOfficial"
-facebook_user_id = "100087298771006"
-# Please setup your driver path
-driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
-url = "https://www.facebook.com/"
-res = fb_graphql_scraper.get_user_posts(
-    fb_username_or_userid=facebook_user_name, 
-    loop_times=50,
-    driver_path=driver_path,
-)
-res
-
-# ## Load account info
-# load_dotenv()
-# fb_account = os.getenv("FBACCOUNT") # Facebook帳號密碼
-# pwd = os.getenv("FBPASSWORD")
-## Log in account version.
-# facebook_user_name = "KaiCenatOfficial"
-# # facebook_user_id = "100087298771006"
-# # Please setup your driver path
-# driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
-# url = "https://www.facebook.com/"
-# res = fb_graphql_scraper.get_user_posts(
-#     fb_username_or_userid=facebook_user_name, 
-#     loop_times=50,
-#     driver_path=driver_path,
-#     fb_account=fb_account,
-#     pwd=pwd
-# )
-# res
+
+## Example.1 - without logging in
+if __name__ == "__main__":
+    facebook_user_name = "love.yuweishao"
+    facebook_user_id = "100044253168423"
+    days_limit = 30 # Number of days within which to scrape posts
+    driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver" 
+    fb_spider = fb_graphql_scraper(driver_path=driver_path)
+    res = fb_spider.get_user_posts(fb_username_or_userid=facebook_user_name, days_limit=days_limit,display_progress=True)
+    print(res)
+
+
+## Example.2 - login in your facebook account to collect data
+# if __name__ == "__main__":
+    # facebook_user_name = "love.yuweishao"
+    # facebook_user_id = "100044253168423"
+    # fb_account = "facebook_account"
+    # fb_pwd = "facebook_paswword"
+    # days_limit = 30 # Number of days within which to scrape posts
+    # driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver" 
+    # fb_spider = fb_graphql_scraper(fb_account=fb_account,fb_pwd=fb_pwd,driver_path=driver_path)
+    # res = fb_spider.get_user_posts(fb_username_or_userid=facebook_user_name, days_limit=days_limit,display_progress=True)
+    # print(res)
+    
+
+
 ```
 
 ### Optional parameters
 
 - **fb_username_or_userid**: groups, fan page, account User-ID or User-Name.
 - **timeout**: How many seconds to wait before timing out. Default is 600.
 - **looptimes**: The program scrolls down Facebook pages..
 
 
-## Post example
+## Result example
 
 ```python
-[{'post_id': '385393337713956',
-  'post_url': 'https://www.facebook.com/385393337713956',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-31 16:00:39'),
-  'published_date2': '2024-03-31',
-  'time': 1711900839,
-  'reaction_count.count': 1224,
-  'comment_rendering_instance.comments.total_count': 37,
-  'share_count.count': 32,
-  'sub_reactions': {'讚': 802,
-   '哈': 406,
-   '大心': 9,
-   '怒': 3,
-   '加油': 2,
-   '哇': 2,
-   '嗚': '0'},
-  'context': 'Druski Plays "What\'s In The Box?" 😱',
-  'video_view_count': 15870},
- {'post_id': '387206327532657',
-  'post_url': 'https://www.facebook.com/387206327532657',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-30 12:01:06'),
-  'published_date2': '2024-03-30',
-  'time': 1711800066,
-  'reaction_count.count': 7153,
-  'comment_rendering_instance.comments.total_count': 154,
-  'share_count.count': 67,
-  'sub_reactions': {'讚': 5674,
-   '哈': 1307,
-   '大心': 121,
-   '嗚': 22,
-   '加油': 21,
-   '哇': 8,
-   '怒': '0'},
-  'context': 'Kai Cenat Asks Tyla Out On A Date 😍 #viralreelsfb #comedy #kaicenat #reelsfb',
-  'video_view_count': 73898},
- {'post_id': '385387707714519',
-  'post_url': 'https://www.facebook.com/385387707714519',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-29 17:01:39'),
-  'published_date2': '2024-03-29',
-  'time': 1711731699,
-  'reaction_count.count': 1000,
-  'comment_rendering_instance.comments.total_count': 47,
-  'share_count.count': 15,
-  'sub_reactions': {'讚': 762,
-   '哈': 194,
-   '大心': 34,
-   '哇': 7,
-   '加油': 2,
-   '嗚': 1,
-   '怒': '0'},
-  'context': 'Chunkz Gets Hypnotised 😱',
-  'video_view_count': 13763},
- {'post_id': '384078261178797',
-  'post_url': 'https://www.facebook.com/384078261178797',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-28 17:00:21'),
-  'published_date2': '2024-03-28',
-  'time': 1711645221,
-  'reaction_count.count': 2587,
-  'comment_rendering_instance.comments.total_count': 77,
-  'share_count.count': 45,
-  'sub_reactions': {'讚': 1905,
-   '哈': 477,
-   '大心': 186,
-   '加油': 15,
-   '哇': 4,
-   '怒': '0',
-   '嗚': '0'},
-  'context': 'Trying The New Ice Spice Drink 😳',
-  'video_view_count': 125605}
-]
+{'fb_username_or_userid': 'love.yuweishao',
+ 'profile': ['任何工作事宜請洽 高先生',
+  '聯絡信箱：hawa00328@gmail.com',
+  '聯絡電話：0975-386-266',
+  '粉絲專頁',
+  ' · 演員',
+  'hawa00328@gmail.com',
+  '1,497,248 位追蹤者'],
+ 'data': [{'post_id': '993720562113040',
+   'post_url': 'https://www.facebook.com/993720562113040',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-24 17:42:14'),
+   'published_date2': '2024-04-24',
+   'time': 1713980534,
+   'reaction_count.count': 3884,
+   'comment_rendering_instance.comments.total_count': 34,
+   'share_count.count': 10,
+   'sub_reactions': {'讚': 3652, '大心': 226, '加油': 5, '哈': 1},
+   'context': 'breathe and life',
+   'video_view_count': nan},
+  {'post_id': '993371658814597',
+   'post_url': 'https://www.facebook.com/993371658814597',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-24 03:55:34'),
+   'published_date2': '2024-04-24',
+   'time': 1713930934,
+   'reaction_count.count': 5043,
+   'comment_rendering_instance.comments.total_count': 41,
+   'share_count.count': 29,
+   'sub_reactions': {'讚': 4632, '大心': 397, '加油': 8, '哇': 4, '哈': 2},
+   'context': '夏季的雨天總讓人難以預期\n每日帶不帶傘的莫非定律 \n空間裡的黏膩和潮濕點滴\n通通都被D-26匯集在一起\n陰晴不定的天氣就交給最懂你的HYD❤️\n\nhttps://reurl.cc/Gjd9nv\nHYD 品宅趣\n#HYD #雙效清淨 #輕量設計 #除濕機',
+   'video_view_count': nan},
+  {'post_id': '992770662208030',
+   'post_url': 'https://www.facebook.com/992770662208030',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-23 04:33:52'),
+   'published_date2': '2024-04-23',
+   'time': 1713846832,
+   'reaction_count.count': 3286,
+   'comment_rendering_instance.comments.total_count': 32,
+   'share_count.count': 5,
+   'sub_reactions': {'讚': 3150, '大心': 61, '加油': 59, '嗚': 13, '哇': 2, '哈': 1},
+   'context': None,
+   'video_view_count': nan},
+  {'post_id': '992336592251437',
+   'post_url': 'https://www.facebook.com/992336592251437',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-22 09:57:32'),
+   'published_date2': '2024-04-22',
+   'time': 1713779852,
+   'reaction_count.count': 11892,
+   'comment_rendering_instance.comments.total_count': 102,
+   'share_count.count': 31,
+   'sub_reactions': {'讚': 11164, '大心': 701, '加油': 15, '哈': 6, '哇': 5, '嗚': 1},
+   'context': '母が撮った写真はとてもきれいです.🌸',
+   'video_view_count': nan},
+  {'post_id': '991854065633023',
+   'post_url': 'https://www.facebook.com/991854065633023',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-21 12:34:39'),
+   'published_date2': '2024-04-21',
+   'time': 1713702879,
+   'reaction_count.count': 5250,
+   'comment_rendering_instance.comments.total_count': 43,
+   'share_count.count': 13,
+   'sub_reactions': {'讚': 4873, '大心': 364, '加油': 6, '哈': 4, '哇': 3},
+   'context': '愛生活也愛工作🖤\n\n@michaelkors \n#MichaelKors',
+   'video_view_count': nan}]
+}
 ```
 
 ### Notes
 - If you choose to collect data by logging into your account, you may face the risk of your account being blocked, even if this program only scrolls through Facebook web pages.
 - Reaction Categories (EN): [`like`, `love`, `haha`, `sorry`, `wow`, `angry`, `care`]
 - Reaction Categories (TW): [`讚`, `哈`, `怒`, `大心`, `加油`, `哇`, `嗚`]
```

### Comparing `facebook-graphql-scraper-1.0.6/facebook_graphql_scraper.egg-info/PKG-INFO` & `facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 1.0.6
+Version: 1.0.7
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/FB_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -38,134 +38,143 @@
 - **Pleas setup driver path at first**
 - **Log in with your account credentials**: login facebook account
 - **Without logging in**: Without logging in, click the X icon to 
 - **Difference**: The difference between these two methods is that for some personal accounts, you cannot browse the user's posts without logging into a Facebook account.
 
 ```python
 # -*- coding: utf-8 -*-
-import os
 from fb_graphql_scraper.facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
-from dotenv import load_dotenv
 
-## Without logging in account version
-facebook_user_name = "KaiCenatOfficial"
-facebook_user_id = "100087298771006"
-# Please setup your driver path
-driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
-url = "https://www.facebook.com/"
-res = fb_graphql_scraper.get_user_posts(
-    fb_username_or_userid=facebook_user_name, 
-    loop_times=50,
-    driver_path=driver_path,
-)
-res
-
-# ## Load account info
-# load_dotenv()
-# fb_account = os.getenv("FBACCOUNT") # Facebook帳號密碼
-# pwd = os.getenv("FBPASSWORD")
-## Log in account version.
-# facebook_user_name = "KaiCenatOfficial"
-# # facebook_user_id = "100087298771006"
-# # Please setup your driver path
-# driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
-# url = "https://www.facebook.com/"
-# res = fb_graphql_scraper.get_user_posts(
-#     fb_username_or_userid=facebook_user_name, 
-#     loop_times=50,
-#     driver_path=driver_path,
-#     fb_account=fb_account,
-#     pwd=pwd
-# )
-# res
+
+## Example.1 - without logging in
+if __name__ == "__main__":
+    facebook_user_name = "love.yuweishao"
+    facebook_user_id = "100044253168423"
+    days_limit = 30 # Number of days within which to scrape posts
+    driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver" 
+    fb_spider = fb_graphql_scraper(driver_path=driver_path)
+    res = fb_spider.get_user_posts(fb_username_or_userid=facebook_user_name, days_limit=days_limit,display_progress=True)
+    print(res)
+
+
+## Example.2 - login in your facebook account to collect data
+# if __name__ == "__main__":
+    # facebook_user_name = "love.yuweishao"
+    # facebook_user_id = "100044253168423"
+    # fb_account = "facebook_account"
+    # fb_pwd = "facebook_paswword"
+    # days_limit = 30 # Number of days within which to scrape posts
+    # driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver" 
+    # fb_spider = fb_graphql_scraper(fb_account=fb_account,fb_pwd=fb_pwd,driver_path=driver_path)
+    # res = fb_spider.get_user_posts(fb_username_or_userid=facebook_user_name, days_limit=days_limit,display_progress=True)
+    # print(res)
+    
+
+
 ```
 
 ### Optional parameters
 
 - **fb_username_or_userid**: groups, fan page, account User-ID or User-Name.
 - **timeout**: How many seconds to wait before timing out. Default is 600.
 - **looptimes**: The program scrolls down Facebook pages..
 
 
-## Post example
+## Result example
 
 ```python
-[{'post_id': '385393337713956',
-  'post_url': 'https://www.facebook.com/385393337713956',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-31 16:00:39'),
-  'published_date2': '2024-03-31',
-  'time': 1711900839,
-  'reaction_count.count': 1224,
-  'comment_rendering_instance.comments.total_count': 37,
-  'share_count.count': 32,
-  'sub_reactions': {'讚': 802,
-   '哈': 406,
-   '大心': 9,
-   '怒': 3,
-   '加油': 2,
-   '哇': 2,
-   '嗚': '0'},
-  'context': 'Druski Plays "What\'s In The Box?" 😱',
-  'video_view_count': 15870},
- {'post_id': '387206327532657',
-  'post_url': 'https://www.facebook.com/387206327532657',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-30 12:01:06'),
-  'published_date2': '2024-03-30',
-  'time': 1711800066,
-  'reaction_count.count': 7153,
-  'comment_rendering_instance.comments.total_count': 154,
-  'share_count.count': 67,
-  'sub_reactions': {'讚': 5674,
-   '哈': 1307,
-   '大心': 121,
-   '嗚': 22,
-   '加油': 21,
-   '哇': 8,
-   '怒': '0'},
-  'context': 'Kai Cenat Asks Tyla Out On A Date 😍 #viralreelsfb #comedy #kaicenat #reelsfb',
-  'video_view_count': 73898},
- {'post_id': '385387707714519',
-  'post_url': 'https://www.facebook.com/385387707714519',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-29 17:01:39'),
-  'published_date2': '2024-03-29',
-  'time': 1711731699,
-  'reaction_count.count': 1000,
-  'comment_rendering_instance.comments.total_count': 47,
-  'share_count.count': 15,
-  'sub_reactions': {'讚': 762,
-   '哈': 194,
-   '大心': 34,
-   '哇': 7,
-   '加油': 2,
-   '嗚': 1,
-   '怒': '0'},
-  'context': 'Chunkz Gets Hypnotised 😱',
-  'video_view_count': 13763},
- {'post_id': '384078261178797',
-  'post_url': 'https://www.facebook.com/384078261178797',
-  'username_or_userid': 'KaiCenatOfficial',
-  'published_date': Timestamp('2024-03-28 17:00:21'),
-  'published_date2': '2024-03-28',
-  'time': 1711645221,
-  'reaction_count.count': 2587,
-  'comment_rendering_instance.comments.total_count': 77,
-  'share_count.count': 45,
-  'sub_reactions': {'讚': 1905,
-   '哈': 477,
-   '大心': 186,
-   '加油': 15,
-   '哇': 4,
-   '怒': '0',
-   '嗚': '0'},
-  'context': 'Trying The New Ice Spice Drink 😳',
-  'video_view_count': 125605}
-]
+{'fb_username_or_userid': 'love.yuweishao',
+ 'profile': ['任何工作事宜請洽 高先生',
+  '聯絡信箱：hawa00328@gmail.com',
+  '聯絡電話：0975-386-266',
+  '粉絲專頁',
+  ' · 演員',
+  'hawa00328@gmail.com',
+  '1,497,248 位追蹤者'],
+ 'data': [{'post_id': '993720562113040',
+   'post_url': 'https://www.facebook.com/993720562113040',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-24 17:42:14'),
+   'published_date2': '2024-04-24',
+   'time': 1713980534,
+   'reaction_count.count': 3884,
+   'comment_rendering_instance.comments.total_count': 34,
+   'share_count.count': 10,
+   'sub_reactions': {'讚': 3652, '大心': 226, '加油': 5, '哈': 1},
+   'context': 'breathe and life',
+   'video_view_count': nan},
+  {'post_id': '993371658814597',
+   'post_url': 'https://www.facebook.com/993371658814597',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-24 03:55:34'),
+   'published_date2': '2024-04-24',
+   'time': 1713930934,
+   'reaction_count.count': 5043,
+   'comment_rendering_instance.comments.total_count': 41,
+   'share_count.count': 29,
+   'sub_reactions': {'讚': 4632, '大心': 397, '加油': 8, '哇': 4, '哈': 2},
+   'context': '夏季的雨天總讓人難以預期\n每日帶不帶傘的莫非定律 \n空間裡的黏膩和潮濕點滴\n通通都被D-26匯集在一起\n陰晴不定的天氣就交給最懂你的HYD❤️\n\nhttps://reurl.cc/Gjd9nv\nHYD 品宅趣\n#HYD #雙效清淨 #輕量設計 #除濕機',
+   'video_view_count': nan},
+  {'post_id': '992770662208030',
+   'post_url': 'https://www.facebook.com/992770662208030',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-23 04:33:52'),
+   'published_date2': '2024-04-23',
+   'time': 1713846832,
+   'reaction_count.count': 3286,
+   'comment_rendering_instance.comments.total_count': 32,
+   'share_count.count': 5,
+   'sub_reactions': {'讚': 3150, '大心': 61, '加油': 59, '嗚': 13, '哇': 2, '哈': 1},
+   'context': None,
+   'video_view_count': nan},
+  {'post_id': '992336592251437',
+   'post_url': 'https://www.facebook.com/992336592251437',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-22 09:57:32'),
+   'published_date2': '2024-04-22',
+   'time': 1713779852,
+   'reaction_count.count': 11892,
+   'comment_rendering_instance.comments.total_count': 102,
+   'share_count.count': 31,
+   'sub_reactions': {'讚': 11164, '大心': 701, '加油': 15, '哈': 6, '哇': 5, '嗚': 1},
+   'context': '母が撮った写真はとてもきれいです.🌸',
+   'video_view_count': nan},
+  {'post_id': '991854065633023',
+   'post_url': 'https://www.facebook.com/991854065633023',
+   'username_or_userid': 'love.yuweishao',
+   'owing_profile': {'__typename': 'User',
+    'name': '邵雨薇',
+    'short_name': '邵雨薇',
+    'id': '100044253168423'},
+   'published_date': Timestamp('2024-04-21 12:34:39'),
+   'published_date2': '2024-04-21',
+   'time': 1713702879,
+   'reaction_count.count': 5250,
+   'comment_rendering_instance.comments.total_count': 43,
+   'share_count.count': 13,
+   'sub_reactions': {'讚': 4873, '大心': 364, '加油': 6, '哈': 4, '哇': 3},
+   'context': '愛生活也愛工作🖤\n\n@michaelkors \n#MichaelKors',
+   'video_view_count': nan}]
+}
 ```
 
 ### Notes
 - If you choose to collect data by logging into your account, you may face the risk of your account being blocked, even if this program only scrolls through Facebook web pages.
 - Reaction Categories (EN): [`like`, `love`, `haha`, `sorry`, `wow`, `angry`, `care`]
 - Reaction Categories (TW): [`讚`, `哈`, `怒`, `大心`, `加油`, `哇`, `嗚`]
```

### Comparing `facebook-graphql-scraper-1.0.6/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 README.md
 setup.py
 facebook_graphql_scraper.egg-info/PKG-INFO
 facebook_graphql_scraper.egg-info/SOURCES.txt
 facebook_graphql_scraper.egg-info/dependency_links.txt
 facebook_graphql_scraper.egg-info/top_level.txt
 fb_graphql_scraper/__init__.py
+fb_graphql_scraper/example.py
 fb_graphql_scraper/facebook_graphql_scraper.py
-fb_graphql_scraper/test_program.py
 fb_graphql_scraper/base/__init__.py
 fb_graphql_scraper/base/base_page.py
 fb_graphql_scraper/pages/__init__.py
 fb_graphql_scraper/pages/page_optional.py
 fb_graphql_scraper/tests/__init__.py
 fb_graphql_scraper/utils/__init__.py
 fb_graphql_scraper/utils/locator.py
```

### Comparing `facebook-graphql-scraper-1.0.6/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/base/base_page.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.6/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/pages/page_optional.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,57 +5,54 @@
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.keys import Keys
 import time
 
 
 class PageOptional(object):
-    def __init__(self, url_in: str, driver=None, fb_account: str = None, pwd: str = None):
+    def __init__(self, driver=None, fb_account: str = None, fb_pwd: str = None):
         self.locator = PageLocators
         self.xpath_elements = PageXpath
         self.class_elements = PageClass
         self.page_text = PageText
         self.driver = driver
-        self.url = url_in
-        self.driver.get(url=self.url)
         self.fb_account = fb_account
-        self.pwd = pwd
-        time.sleep(3)
+        self.fb_pwd = fb_pwd
 
         # Loggin account
-        if self.fb_account and self.pwd:
+        if self.fb_account and self.fb_pwd:
+            login_page_url = "https://www.facebook.com/login"
+            self.driver.get(url=login_page_url)
             self.login_page()
 
-        # 免登入帳號, 適用不需登入帳號的爬蟲目標 / Without logging, click X button
-        else:
-            self.click_reject_login_button()
-
     def login_page(self):
         try:
-            self.login_account(user=self.fb_account, password=self.pwd,
-                               user_element=self.locator.LOGGINUSR1, pwd_element=self.locator.LOGGINPWD1)
-        except:
-            self.login_account(user=self.fb_account, password=self.pwd,
-                               user_element=self.locator.LOGGINUSR2, pwd_element=self.locator.LOGGINPWD2)
+            self.login_account(user=self.fb_account, 
+                               password=self.fb_pwd,
+            )
+            time.sleep(5)
+        except Exception as e:
+            print(f"Login faield, message: {e}")
 
     def clean_requests(self):
+        print(f"Before cleaning driver requests, the number of requests are: {len(self.driver.requests)}")
         try:
             print("Try to clear driver requests..")
             del self.driver.requests
-            print("Clear")
+            print(f"Clear, the number of requests are: {len(self.driver.requests)}")
         except Exception as e:
             print(f"Clear unsuccessfully, message: {e}")
 
     def get_in_url(self):
         self.driver.get(url=self.url)
 
-    def login_account(self, user: str, password: str, user_element, pwd_element):
-        user_element = self.driver.find_element(By.XPATH, user_element)
+    def login_account(self, user: str, password: str):
+        user_element = self.driver.find_element(By.NAME, "email")
         user_element.send_keys(user)
-        password_element = self.driver.find_element(By.XPATH, pwd_element)
+        password_element = self.driver.find_element(By.NAME, "pass")
         password_element.send_keys(password)
         password_element.send_keys(Keys.ENTER)
 
     def scroll_window(self):
         self.driver.execute_script(
             "window.scrollTo(0,document.body.scrollHeight)")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `facebook-graphql-scraper-1.0.6/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/locator.py`

 * *Files 23% similar despite different names*

```diff
@@ -33,25 +33,22 @@
 
 class PageLocators(object):
     CLOSELOGIN = (
         By.XPATH, "/html/body/div[1]/div/div[1]/div/div[5]/div/div/div[1]/div/div[2]/div/div/div/div[1]/div/i")
     DISPLAY_MORE = (
         By.XPATH, f"//div[@class='{PageClass.DISPLAY_MORE}' and @role='{PageRoleValue.DISPLAY_MORE}' and text()='{PageText.DISPLAY_MORE}']")
 
-    # LOGGINUSR1 = (
-    #     "/html/body/div[1]/div[1]/div[1]/div/div[3]/div[2]/form/div[2]/div[1]/input")  # user1
-    # LOGGINPWD1 = (
-    #     "/html/body/div[1]/div[1]/div[1]/div/div[3]/div[2]/form/div[2]/div[2]/div/div/input")  # pwd1
-    
     LOGGINUSR1 = (
         "/html/body/div[1]/div[1]/div[1]/div/div/div/div[2]/div/div[1]/form/div[1]/div[1]/input"
     )
-    
     LOGGINPWD1 = (
         "/html/body/div[1]/div[1]/div[1]/div/div/div/div[2]/div/div[1]/form/div[1]/div[2]/div/input"
     )
     
-
     LOGGINUSR2 = (
         "/html/body/div[1]/div/div[1]/div/div[5]/div/div/div[1]/div/div[2]/div/div/div/div[2]/form/div/div[3]/div/label/div/div/input")
     LOGGINPWD2 = (
         "/html/body/div[1]/div/div[1]/div/div[5]/div/div/div[1]/div/div[2]/div/div/div/div[2]/form/div/div[4]/div/label/div/div/input")
+
+    # version.3: facebook login page
+    LOGGINUSR3 = (By.NAME, "email")
+    LOGGINPWD3 = (By.NAME, "pass")
```

### Comparing `facebook-graphql-scraper-1.0.6/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,51 +4,56 @@
 import json
 from fb_graphql_scraper.utils.utils import *
 
 
 class RequestsParser(object):
     def __init__(self, driver) -> None:
         self.driver = driver
-        self.res_new = []
-        self.feedback_list = []
-        self.context_list = []
-        self.creation_list = []
-        self.author_id_list = []
-        self.author_id_list2 = []
         self.reaction_names = ["讚", "哈", "怒", "大心", "加油", "哇", "嗚"]
         self.en_reaction_names = ["like", "haha", "angry", "love", "care", "sorry", "wow"]
 
     def get_graphql_body_content(self, req_response, req_url):
         target_url = "https://www.facebook.com/api/graphql/"
         if req_response and req_url == target_url:
             response = req_response
             body = decode(response.body, response.headers.get(
                 'Content-Encoding', 'identity'))
             body_content = body.decode("utf-8").split("\n")
             return body_content
         return None
+    
+    def clean_res(self):
+        self.res_new = []
+        self.feedback_list = []
+        self.context_list = []
+        self.creation_list = []
+        self.author_id_list = []
+        self.author_id_list2 = []
+        self.owning_profile = []
 
     def parse_body(self, body_content):
         for each_body in body_content:
             json_data = json.loads(each_body)
             self.res_new.append(json_data)
             try:
                 each_res = json_data['data']['node'].copy()
                 each_feedback = find_feedback_with_subscription_target_id(
                     each_res)
                 if each_feedback:
                     self.feedback_list.append(each_feedback)
                     message_text = find_message_text(json_data)
                     creation_time = find_creation(json_data)
+                    owing_profile = find_owning_profile(json_data)
                     if message_text:
                         self.context_list.append(message_text)
                     elif not message_text:
                         self.context_list.append(None)
                     if creation_time:
                         self.creation_list.append(creation_time)
+                    self.owning_profile.append(owing_profile)
 
             # Did not display or record error message at here
             except Exception as e:
                 pass
 
     def collect_posts(self):
         res_out = []
@@ -71,19 +76,28 @@
             'comment_rendering_instance.comments.total_count',
             'share_count.count',
             'top_reactions.edges',
             'video_view_count'
         ]]
         return df_res
 
-    def process_reactions(self, reactions_in):
-        reaction_names = self.reaction_names
-        en_reaction_names = self.en_reaction_names # if you are in U.S, use self.en_reaction_names
+    def process_reactions(self, reactions_in) -> dict:
+        """Extract sub reaction value: 
+        Args:
+            reactions_in (_type_): _description_
+        Returns:
+            _dict_: {
+                "like": value, 
+                "haha": value, 
+                "angry": value, 
+                "love": value, 
+                "care": value, 
+                "sorry": value, 
+                "wow": value
+        }
+        Note: 
+        """
         reaction_hash = {}
         for each_react in reactions_in:
             reaction_hash[each_react['node']['localized_name']
                           ] = each_react['reaction_count']  # get reaction value
-
-        # for k in reaction_names:
-        #     if k not in reaction_hash and k not in en_reaction_names:
-        #         reaction_hash[k] = '0'
         return reaction_hash
```

### Comparing `facebook-graphql-scraper-1.0.6/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,38 +101,39 @@
             result = find_actors(item)
             if result:
                 return result
     # If no matching condition is found, return None
     return None
 
 
-def find_profile_id(data):
+def find_owning_profile(data):
     if isinstance(data, dict):
-        # If it's a dictionary, check if it contains the 'profile_id' key
-        if 'profile_id' in data:
-            # If the value of the 'profile_id' key is a dictionary
-            if isinstance(data['profile_id'], dict):
-                # Return the value of the 'profile_id' key
-                return data['profile_id']
+        # If it's a dictionary, check if it contains the 'story' key
+        if 'owning_profile' in data:
+            # If the value of the 'story' key is a dictionary and contains the 'actors' key
+            if isinstance(data['owning_profile'], dict):
+                # Return the value of the 'id' key under 'actors'
+                return data['owning_profile']
 
         # If no matching condition is found, recursively check each value in the dictionary
         for value in data.values():
-            result = find_profile_id(value)
+            result = find_owning_profile(value)
             if result:
                 return result
 
     elif isinstance(data, list):
         # If it's a list, recursively check each element in the list
         for item in data:
-            result = find_profile_id(item)
+            result = find_owning_profile(item)
             if result:
                 return result
     # If no matching condition is found, return None
     return None
 
+
 def timeout(timelimit):
     def decorator(func):
         def decorated(*args, **kwargs):
             with futures.ThreadPoolExecutor(max_workers=1) as executor:
                 future = executor.submit(func, *args, **kwargs)
                 try:
                     result = future.result(timelimit)
@@ -143,13 +144,28 @@
                     pass
                 executor._threads.clear()
                 futures.thread._threads_queues.clear()
                 return result
         return decorated
     return decorator
 
+
 def get_current_time(timezone="Asia/Taipei"):
     current_time_utc = datetime.utcnow()
     target_timezone = pytz.timezone(timezone)
     target_current_time = current_time_utc.replace(
         tzinfo=pytz.utc).astimezone(target_timezone)
     return target_current_time
+
+
+def days_difference_from_now(tmp_creation_array: list) -> int:
+    timestamp = min(tmp_creation_array)
+    current_date_time = datetime.now()
+    date_time_obj = datetime.fromtimestamp(timestamp)
+    difference = current_date_time - date_time_obj
+    return difference.days
+
+
+def is_date_exceed_limit(max_days_ago, days_limit: int = 61):
+    if max_days_ago > days_limit:
+        return True
+    return False
```

### Comparing `facebook-graphql-scraper-1.0.6/setup.py` & `facebook-graphql-scraper-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='1.0.6',
+    version='1.0.7',
     packages=[
         "fb_graphql_scraper",
         "fb_graphql_scraper.pages",
         "fb_graphql_scraper.base",
         "fb_graphql_scraper.tests", 
         "fb_graphql_scraper.utils",
         ],
```

