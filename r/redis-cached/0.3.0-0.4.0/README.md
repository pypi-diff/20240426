# Comparing `tmp/redis_cached-0.3.0.tar.gz` & `tmp/redis_cached-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_cached-0.3.0.tar", max compression
+gzip compressed data, was "redis_cached-0.4.0.tar", max compression
```

## Comparing `redis_cached-0.3.0.tar` & `redis_cached-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-12-12 12:36:44.895347 redis_cached-0.3.0/LICENSE
--rw-r--r--   0        0        0     1868 2023-12-25 11:21:56.894497 redis_cached-0.3.0/README.md
--rw-r--r--   0        0        0      623 2024-02-26 02:18:05.113729 redis_cached-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       42 2023-12-16 12:12:55.831020 redis_cached-0.3.0/redis_cached/__init__.py
--rw-r--r--   0        0        0     2401 2024-01-12 08:17:55.206429 redis_cached-0.3.0/redis_cached/core.py
--rw-r--r--   0        0        0     1078 2024-02-26 02:18:05.110346 redis_cached-0.3.0/redis_cached/redis.py
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 redis_cached-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-12-12 12:36:44.895347 redis_cached-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2185 2024-04-26 07:30:19.823667 redis_cached-0.4.0/README.md
+-rw-r--r--   0        0        0      623 2024-04-26 07:30:19.824574 redis_cached-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-26 07:30:19.824920 redis_cached-0.4.0/redis_cached/__init__.py
+-rw-r--r--   0        0        0     3378 2024-04-26 07:30:19.825139 redis_cached-0.4.0/redis_cached/core.py
+-rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 redis_cached-0.4.0/PKG-INFO
```

### Comparing `redis_cached-0.3.0/LICENSE` & `redis_cached-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_cached-0.3.0/README.md` & `redis_cached-0.4.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -18,48 +18,60 @@
 
 # Usage
 
 Basic usage:
 
 ```python
 import asyncio
-from redis_cached import cached, invalidate_cache
+from redis_cached import Cache
 
-@cached(5)
-async def add_one(x):
-    return x + 1
+cache = Cache()
+
+@cache.cached(5)
+async def get_user_data(user_id: int):
+    # expensive API call here
+    return {'user_id': user_id, 'name': 'John Doe'}
 
 async def main():
-    result = await add_one(x=2)  # result is cached for 5 seconds
+    user_data = await get_user_data(user_id=1)  # result is cached for 5 seconds
     
-    # Pass the same kwargs to this func to invalidate the cache
-    await invalidate_cache('add_one', x=2)
+    # To invalidate the cache for the user with ID 1, pass the same kwargs:
+    await cache.invalidate_cache('get_user_data', user_id=1)
 
 asyncio.run(main())
 ```
 
 
-Optionally, add salt to the decorator to avoid clashing with the same-named functions in other modules or other apps that use the same Redis or KeyDB database:
+Optionally, add salt to `cache_key_salt` to avoid clashing with the same-named functions in other modules or other apps that use the same Redis database.
+
+You can also use your custom-configured async Redis instance with the cache.
 
 ```python
 import asyncio
-from redis_cached import cached, invalidate_cache
-
-CACHE_SALT = 'XnsJ-7C9PIU0qhDwh9YhJQ'
-
-@cached(5, cache_key_salt=CACHE_SALT)
-async def add_one(x):
-    return x + 1
+from redis.asyncio.client import Redis
+from redis_cached import Cache
 
-async def invalidate_add_one(**kwargs):
-    await invalidate_cache('add_one', cache_key_salt=CACHE_SALT, **kwargs)
+custom_redis = Redis(
+    host='localhost',
+    port=6379,
+    db=0
+)
+cache = Cache(
+    cache_key_salt='qhDwh9Y',
+    redis_=custom_redis
+)
+
+@cache.cached(5)
+async def get_user_data(user_id: int):
+    # expensive API call here
+    return {'user_id': user_id, 'name': 'John Doe'}
 
 async def main():
-    result = await add_one(x=2)  # cached
-    await invalidate_add_one(x=2)  # invalidated
+    user_data = await get_user_data(user_id=1)  # cached
+    await cache.invalidate_cache('get_user_data', user_id=1)  # invalidated
 
 asyncio.run(main())
 ```
 
 # Contributing
 
-Contributions are welcome. Please refer to [maintenance readme](./maintenance/README.md) for more details.
+Contributions are welcome. Please refer to the [maintenance readme](./maintenance/README.md) for more details.
```

### Comparing `redis_cached-0.3.0/pyproject.toml` & `redis_cached-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-cached"
-version = "0.3.0"
+version = "0.4.0"
 description = "Python cache decorator and other itils with support for Redis or KeyDB"
 authors = ["Dmitry Babanov <85852989+dmitrybabanovforreal@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/dmitrybabanovforreal/redis-cached"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

