# Comparing `tmp/simplebox-0.0.1a198-py3-none-any.whl.zip` & `tmp/simplebox-0.0.1a199-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 280629 bytes, number of entries: 156
--rw-rw-rw-  2.0 fat     5191 b- defN 24-Apr-24 14:18 simplebox/__init__.py
+Zip file size: 280696 bytes, number of entries: 156
+-rw-rw-rw-  2.0 fat     5191 b- defN 24-Apr-26 15:42 simplebox/__init__.py
 -rw-rw-rw-  2.0 fat     2090 b- defN 24-Apr-07 16:46 simplebox/backend.py
 -rw-rw-rw-  2.0 fat    17626 b- defN 24-Apr-07 16:46 simplebox/character.py
 -rw-rw-rw-  2.0 fat     4829 b- defN 24-Apr-14 15:04 simplebox/classes.py
 -rw-rw-rw-  2.0 fat    16962 b- defN 24-Apr-20 14:21 simplebox/cmd.py
 -rw-rw-rw-  2.0 fat     5481 b- defN 23-Nov-14 15:01 simplebox/converter.py
 -rw-rw-rw-  2.0 fat     1638 b- defN 24-Apr-07 15:02 simplebox/enums.py
 -rw-rw-rw-  2.0 fat      306 b- defN 23-May-31 16:53 simplebox/generic.py
--rw-rw-rw-  2.0 fat    57692 b- defN 24-Apr-24 14:50 simplebox/http.py
+-rw-rw-rw-  2.0 fat    58109 b- defN 24-Apr-26 15:42 simplebox/http.py
 -rw-rw-rw-  2.0 fat     3672 b- defN 23-Sep-07 15:33 simplebox/jsonparser.py
 -rw-rw-rw-  2.0 fat    21577 b- defN 24-Apr-14 14:30 simplebox/number.py
 -rw-rw-rw-  2.0 fat     1006 b- defN 24-Apr-07 17:05 simplebox/singleton.py
 -rw-rw-rw-  2.0 fat     1400 b- defN 24-Apr-07 17:02 simplebox/version.py
 -rw-rw-rw-  2.0 fat     4561 b- defN 24-Apr-14 15:04 simplebox/void.py
 -rw-rw-rw-  2.0 fat       86 b- defN 24-Mar-27 14:40 simplebox/_h2/__init__.py
 -rw-rw-rw-  2.0 fat     5764 b- defN 24-Mar-27 14:40 simplebox/_h2/config.py
@@ -147,12 +147,12 @@
 -rw-rw-rw-  2.0 fat     2173 b- defN 24-Apr-07 15:48 simplebox/utils/enums.py
 -rw-rw-rw-  2.0 fat     2997 b- defN 24-Apr-07 15:48 simplebox/utils/locks.py
 -rw-rw-rw-  2.0 fat    11999 b- defN 24-Apr-07 15:48 simplebox/utils/objects.py
 -rw-rw-rw-  2.0 fat     3258 b- defN 24-Apr-14 14:42 simplebox/utils/optionals.py
 -rw-rw-rw-  2.0 fat    19546 b- defN 24-Apr-07 15:48 simplebox/utils/strings.py
 -rw-rw-rw-  2.0 fat      247 b- defN 23-Feb-28 15:31 simplebox/valid/__init__.py
 -rw-rw-rw-  2.0 fat    16632 b- defN 24-Apr-15 17:12 simplebox/valid/_validator.py
--rw-rw-rw-  2.0 fat     1358 b- defN 24-Apr-24 17:23 simplebox-0.0.1a198.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 17:23 simplebox-0.0.1a198.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-24 17:23 simplebox-0.0.1a198.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    13587 b- defN 24-Apr-24 17:23 simplebox-0.0.1a198.dist-info/RECORD
-156 files, 1110355 bytes uncompressed, 259189 bytes compressed:  76.7%
+-rw-rw-rw-  2.0 fat     1358 b- defN 24-Apr-26 16:21 simplebox-0.0.1a199.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-26 16:21 simplebox-0.0.1a199.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-26 16:21 simplebox-0.0.1a199.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    13587 b- defN 24-Apr-26 16:21 simplebox-0.0.1a199.dist-info/RECORD
+156 files, 1110772 bytes uncompressed, 259256 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -450,20 +450,20 @@
 
 Filename: simplebox/valid/__init__.py
 Comment: 
 
 Filename: simplebox/valid/_validator.py
 Comment: 
 
-Filename: simplebox-0.0.1a198.dist-info/METADATA
+Filename: simplebox-0.0.1a199.dist-info/METADATA
 Comment: 
 
-Filename: simplebox-0.0.1a198.dist-info/WHEEL
+Filename: simplebox-0.0.1a199.dist-info/WHEEL
 Comment: 
 
-Filename: simplebox-0.0.1a198.dist-info/top_level.txt
+Filename: simplebox-0.0.1a199.dist-info/top_level.txt
 Comment: 
 
-Filename: simplebox-0.0.1a198.dist-info/RECORD
+Filename: simplebox-0.0.1a199.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplebox/__init__.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
-__version__ = "0.0.1.alpha198"
+__version__ = "0.0.1.alpha199"
 
 banner = f"""
  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------. 
 | .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. |
 | |    _______   | || |     _____    | || | ____    ____ | || |   ______     | || |   _____      | || |  _________   | || |   ______     | || |     ____     | || |  ____  ____  | |
 | |   /  ___  |  | || |    |_   _|   | || ||_   \  /   _|| || |  |_   __ \   | || |  |_   _|     | || | |_   ___  |  | || |  |_   _ \    | || |   .'    `.   | || | |_  _||_  _| | |
 | |  |  (__ \_|  | || |      | |     | || |  |   \/   |  | || |    | |__) |  | || |    | |       | || |   | |_  \_|  | || |    | |_) |   | || |  /  .--.  \  | || |   \ \  / /   | |
```

## simplebox/http.py

```diff
@@ -100,20 +100,28 @@
     Usage:
         RestOptions(params={}, data={}, ...)
     """
 
     def __init__(self, params: dict = None, data: dict = None, headers: dict = None, cookies: dict = None,
                  files: dict = None, auth: tuple = None, timeout: float or tuple = None, allow_redirects: bool = True,
                  proxies: dict = None, hooks: dict = None, stream: bool = None, verify: bool = None, cert: str = None,
-                 json: dict = None, restful: dict = None, *args, **kwargs):
+                 json: dict = None, restful: dict = None, **kwargs):
         super().__init__()
         self.update(params=params, data=data, headers=headers, cookies=cookies, files=files, auth=auth,
                     timeout=timeout, allow_redirects=allow_redirects, proxies=proxies, hooks=hooks, stream=stream,
                     verify=verify, cert=cert, json=json, restful=restful, **kwargs)
 
+    def add(self, key, value) -> 'RestOptions':
+        self.setdefault(key, value)
+        return self
+
+    def modify(self, key, value) -> 'RestOptions':
+        self[key] = value
+        return self
+
     @property
     def opts_no_none(self) -> Dictionary:
         tmp = Dictionary()
         for k, v in self.items():
             if v:
                 tmp[k] = v
         return tmp
@@ -312,19 +320,19 @@
 
 
 class Rest(object):
     """
     A simple http request frame.
     """
 
-    def __init__(self, file: str = None, server_name: str = None, host: str = None, herders: dict = None,
+    def __init__(self, file: str = None, server_name: str = None, host: str = None, headers: dict = None,
                  cookies: dict = None, check_status: bool = False, encoding: str = "utf-8", description: str = None,
                  restful: dict = None, http2: bool = False, retry_times: int = 10, retry_interval: int = 5,
                  retry_exit_code_range: list = None, retry_exception_retry: bool = True,
-                 retry_check_handler: Callable[[Any], bool] = None):
+                 retry_check_handler: Callable[[Any], bool] = None, verify: bool = None, ):
         """
             def retry(times: int = 10, interval: int = 5, exit_code_range: list = None, exception_retry: bool = True,
               check_handler: Callable[[Any], bool] = None) -> T:
         Build a request client.
         :param file: The path where the interface configuration file is stored.
                      configuration format：
                         [
@@ -372,23 +380,24 @@
         self.__http2: Optional[bool] = None
         self.__session: Optional[Session] = None
         self.__retry_times: Optional[int] = None
         self.__retry_interval: Optional[int] = None
         self.__retry_exit_code_range: Optional[list] = None
         self.__retry_exception_retry: Optional[bool] = None
         self.__retry_check_handler: Optional[Callable[[Any], bool]] = None
-        self.__initialize(file, server_name, host, herders, cookies, check_status, encoding, description, restful,
+        self.__verify: Optional[bool] = None
+        self.__initialize(file, server_name, host, headers, cookies, check_status, encoding, description, restful,
                           http2, retry_times, retry_interval, retry_exit_code_range, retry_exception_retry,
-                          retry_check_handler)
+                          retry_check_handler, verify)
 
     def __initialize(self, file: str = None, server_name: str = None, host: str = None, headers: dict[str, str] = None,
                      cookies: dict[str, str] = None, check_status: bool = False, encoding: str = "utf-8",
                      description: str = None, restful: dict = None, http2: bool = False, retry_times: int = 10,
                      retry_interval: int = 5, retry_exit_code_range: list = None, retry_exception_retry: bool = True,
-                     retry_check_handler: Callable[[Any], bool] = None):
+                     retry_check_handler: Callable[[Any], bool] = None, verify: bool = None):
         self.__restful = restful or RestFul()
         self.__check_status: bool = check_status if isinstance(check_status, bool) else False
         self.__encoding: str = encoding if isinstance(encoding, str) else "utf-8"
         self.__server_name: str = server_name
         self.__server_list: list[dict[str, str]] = []
         self.__server: dict[str, dict[Any, Any]] = {}
         self.__host: str = host
@@ -398,15 +407,16 @@
         self.__http2: bool = http2 if isinstance(http2, bool) else False
         self.__retry_times: int = retry_times if isinstance(retry_times, int) else 10
         self.__retry_interval: int = retry_interval if isinstance(retry_interval, int) else 5
         self.__retry_exit_code_range: int = retry_times if isinstance(retry_exit_code_range, list) else (i for i in
                                                                                                          range(200,
                                                                                                                300))
         self.__retry_exception_retry: int = retry_times if isinstance(retry_exception_retry, bool) else True
-        self.__retry_check_handler: int = retry_times
+        self.__retry_check_handler: Callable[[Any], bool] = retry_check_handler
+        self.__verify: bool = verify
         self.__session: Session = Session()
         if http2:
             scheme = urlparse(self.__host).scheme
             if scheme != _Constant.HTTPS:
                 raise HttpException(f"http2 need https protocol, but found '{scheme}'")
             self.__session.mount(f"{_Constant.HTTPS}://", HTTP20Adapter())
         if file:
@@ -996,15 +1006,15 @@
         url: str = urljoin(host_, api_)
         check_status_: bool = self.__check_status if not check_status else check_status
         encoding_: str = self.__encoding if not encoding else encoding
         optional_args_tmp = {}
         for k, v in deepcopy(optional_args).items():
             if k in _OPTIONAL_ARGS_KEYS and v:
                 optional_args_tmp[k] = v
-
+        optional_args_tmp['verify'] = self.__verify
         resp = None
         rest_resp = RestResponse(None)
         url: str = url.format(**self.__restful_handler(restful, optional_args.get(_Constant.RESTFUL)))
         # noinspection PyBroadException
         try:
             resp: Response or None = self.__action(method_.lower(), url, **optional_args_tmp)
             if check_status_:
```

## Comparing `simplebox-0.0.1a198.dist-info/METADATA` & `simplebox-0.0.1a199.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplebox
-Version: 0.0.1a198
+Version: 0.0.1a199
 Summary: 简易工具箱。
 Author: fuck
 License: MIT Licence
 Keywords: pip,simplebox,backend,fast,fasttools,box,simple
 Platform: any
 Requires-Python: >=3.9
 Requires-Dist: psutil (==5.9.2)
```

## Comparing `simplebox-0.0.1a198.dist-info/RECORD` & `simplebox-0.0.1a199.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-simplebox/__init__.py,sha256=MORHnsLeXA-rCbm2bPLRQ2UCB3r0yjV_zyIv8ESvtps,5191
+simplebox/__init__.py,sha256=uoiioA0RpIUBTiWHPNhGjxM5mS2XMsyys5GRwZosywE,5191
 simplebox/backend.py,sha256=yR3gveO0iKcTKWKW5K57513u-s7O3oGes84Kp8HUZho,2090
 simplebox/character.py,sha256=NEbQqFmD3rpkl_E3MeES7rRfAmtc_DJHoKcF8GNK92g,17626
 simplebox/classes.py,sha256=vGD0PVglh-Nlz8I3PTqDmDquQf_Z2BNoXIvp9aRS140,4829
 simplebox/cmd.py,sha256=5SK-ne4vAyjNdEztS0TyMWUuQC6bBc4RCtnbdQBvVF4,16962
 simplebox/converter.py,sha256=DZ_sb-ZBIorTZAlpuNyGjxnlPAjtSp7yKMIDSiwws0g,5481
 simplebox/enums.py,sha256=KzziG7TboPMIENPrc4HrsUagSEMd4JfLFG6Bn2T0HAs,1638
 simplebox/generic.py,sha256=tBDzlqFHQ7I6bb8_iC9PEqyMaD0sxJee9a7zR3YwxRw,306
-simplebox/http.py,sha256=mvofzgSQMetUPcZWebVsx-QdrnYGA_GTGBG9ZUe879c,57692
+simplebox/http.py,sha256=Dkfrbw-gq48fBipaJDPFJikH8Q0vObN7Sd2MYlqBMd0,58109
 simplebox/jsonparser.py,sha256=zMV14sTgmQn_E2mafTOvlw8SlxXSYUPOQFfeFKOoYk4,3672
 simplebox/number.py,sha256=hpSLKIoRFnjt-lk4SUCvYNKbcBD8lP_vaOFtD4JQIUQ,21577
 simplebox/singleton.py,sha256=zhyjjhQfg9Y1UYgYFYF31ybNjX0A0oMzBaOG1UZerXo,1006
 simplebox/version.py,sha256=5H3eNzxQOzLT5meyjzOZ1-dg1R9U3h5lCGNzWXwU4Lg,1400
 simplebox/void.py,sha256=wHIojA2oOc5jRYetX4xJxIYFHZNtrYb6hLHSP-HiJfc,4561
 simplebox/_h2/__init__.py,sha256=7aSRL7tUP7vhMpV5uORROh1XlS-pzzxzS0F4mSAFa70,86
 simplebox/_h2/config.py,sha256=9zQSxQ2bpFs07AoPSGa5s6sFzkmRkD8GS5sJAPD10YQ,5764
@@ -146,11 +146,11 @@
 simplebox/utils/enums.py,sha256=rwMAmDqUFy2iJey9v0aThBCAFcR-tKqVI9LELw4BKcw,2173
 simplebox/utils/locks.py,sha256=YNT_ZMV52n9MRsizOYweyxMh5Bb__EC8epJWA-dmXXk,2997
 simplebox/utils/objects.py,sha256=FEECiUsCV9ENU_sqIHdPNIYaGbqTgzOqD5fmwEmqmr8,11999
 simplebox/utils/optionals.py,sha256=XDlteLGkfbWHOgJPdGykE-a79Ae-P7Fbfsabmiwdjuw,3258
 simplebox/utils/strings.py,sha256=yvdvMVI-ULs-DIWElpmjdYHp9CPLbETc5M-16L9gflk,19546
 simplebox/valid/__init__.py,sha256=7deSv2vW7Wj-83Db3JbO0SZK9Pf-G9pDqbCAgkxr8PI,247
 simplebox/valid/_validator.py,sha256=xj3ju6Lpx73bF3NZR9eGHJl_pTk6kPMsFL4hrhbM2cw,16632
-simplebox-0.0.1a198.dist-info/METADATA,sha256=NHA5VtyXHbkD0YYcgeuWFpTNhf4H7UvXFA1_vlf3DfY,1358
-simplebox-0.0.1a198.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-simplebox-0.0.1a198.dist-info/top_level.txt,sha256=96Ce93hfSG2V2dNspzU_GDarYqtHFh9siA46UaMcdjo,10
-simplebox-0.0.1a198.dist-info/RECORD,,
+simplebox-0.0.1a199.dist-info/METADATA,sha256=Tx97lCpqlusLrMxvvf6dMY0dA5d845NiwtkcuQQPhuI,1358
+simplebox-0.0.1a199.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+simplebox-0.0.1a199.dist-info/top_level.txt,sha256=96Ce93hfSG2V2dNspzU_GDarYqtHFh9siA46UaMcdjo,10
+simplebox-0.0.1a199.dist-info/RECORD,,
```

