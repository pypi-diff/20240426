# Comparing `tmp/resty_client-0.0.4.tar.gz` & `tmp/resty_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resty_client-0.0.4.tar", max compression
+gzip compressed data, was "resty_client-0.0.5.tar", max compression
```

## Comparing `resty_client-0.0.4.tar` & `resty_client-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     1090 2024-01-23 13:22:57.074926 resty_client-0.0.4/LICENSE
--rw-r--r--   0        0        0     1093 2024-04-25 08:58:55.181458 resty_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3194 2024-04-25 08:58:55.200458 resty_client-0.0.4/README.md
--rw-r--r--   0        0        0      126 2024-01-26 15:20:15.262707 resty_client-0.0.4/resty/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 15:14:08.249782 resty_client-0.0.4/resty/clients/__init__.py
--rw-r--r--   0        0        0      179 2024-04-22 14:23:32.487305 resty_client-0.0.4/resty/clients/httpx/__init__.py
--rw-r--r--   0        0        0     3351 2024-04-23 18:07:25.657688 resty_client-0.0.4/resty/clients/httpx/client.py
--rw-r--r--   0        0        0      557 2024-04-22 15:02:44.798358 resty_client-0.0.4/resty/constants.py
--rw-r--r--   0        0        0      370 2024-04-22 14:23:32.559298 resty_client-0.0.4/resty/enums.py
--rw-r--r--   0        0        0      729 2024-04-23 10:31:25.956591 resty_client-0.0.4/resty/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-26 15:14:08.265783 resty_client-0.0.4/resty/ext/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 15:14:08.265783 resty_client-0.0.4/resty/ext/django/__init__.py
--rw-r--r--   0        0        0      200 2024-04-22 14:23:32.601297 resty_client-0.0.4/resty/ext/django/middlewares/__init__.py
--rw-r--r--   0        0        0     1311 2024-04-23 16:28:55.203681 resty_client-0.0.4/resty/ext/django/middlewares/pagination.py
--rw-r--r--   0        0        0       69 2024-04-23 09:51:08.271071 resty_client-0.0.4/resty/managers/__init__.py
--rw-r--r--   0        0        0     4988 2024-04-25 08:58:55.194460 resty_client-0.0.4/resty/managers/manager.py
--rw-r--r--   0        0        0      328 2024-04-23 09:51:08.258984 resty_client-0.0.4/resty/middlewares/__init__.py
--rw-r--r--   0        0        0     1296 2024-04-23 16:28:55.207680 resty_client-0.0.4/resty/middlewares/manager.py
--rw-r--r--   0        0        0      264 2024-04-23 09:47:25.043213 resty_client-0.0.4/resty/middlewares/types.py
--rw-r--r--   0        0        0       81 2024-04-23 09:51:08.264970 resty_client-0.0.4/resty/serializers/__init__.py
--rw-r--r--   0        0        0     1390 2024-04-23 18:21:24.086198 resty_client-0.0.4/resty/serializers/serializer.py
--rw-r--r--   0        0        0     2861 2024-04-23 16:28:55.216676 resty_client-0.0.4/resty/types.py
--rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 resty_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-01-23 13:22:57.074926 resty_client-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1119 2024-04-26 19:35:16.403290 resty_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3906 2024-04-26 19:31:39.072847 resty_client-0.0.5/README.md
+-rw-r--r--   0        0        0      172 2024-04-26 09:56:00.652385 resty_client-0.0.5/resty/__init__.py
+-rw-r--r--   0        0        0      230 2024-04-26 09:22:05.024491 resty_client-0.0.5/resty/__version__.py
+-rw-r--r--   0        0        0       89 2024-04-25 16:40:33.939395 resty_client-0.0.5/resty/clients/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-25 15:52:51.149933 resty_client-0.0.5/resty/clients/httpx/__init__.py
+-rw-r--r--   0        0        0     2912 2024-04-26 08:35:43.160377 resty_client-0.0.5/resty/clients/httpx/clients.py
+-rw-r--r--   0        0        0      294 2024-04-25 15:59:43.497633 resty_client-0.0.5/resty/clients/types.py
+-rw-r--r--   0        0        0      371 2024-04-25 16:23:57.349870 resty_client-0.0.5/resty/constants.py
+-rw-r--r--   0        0        0      370 2024-04-22 14:23:32.559298 resty_client-0.0.5/resty/enums.py
+-rw-r--r--   0        0        0     1027 2024-04-26 12:14:34.090077 resty_client-0.0.5/resty/exceptions.py
+-rw-r--r--   0        0        0      251 2024-04-26 12:21:28.058775 resty_client-0.0.5/resty/managers/__init__.py
+-rw-r--r--   0        0        0     1395 2024-04-26 12:52:01.561816 resty_client-0.0.5/resty/managers/builders.py
+-rw-r--r--   0        0        0     7181 2024-04-26 15:18:16.950582 resty_client-0.0.5/resty/managers/managers.py
+-rw-r--r--   0        0        0     2837 2024-04-26 14:45:33.821123 resty_client-0.0.5/resty/managers/types.py
+-rw-r--r--   0        0        0      460 2024-04-26 09:56:25.334802 resty_client-0.0.5/resty/middlewares/__init__.py
+-rw-r--r--   0        0        0     1657 2024-04-25 18:35:38.358135 resty_client-0.0.5/resty/middlewares/managers.py
+-rw-r--r--   0        0        0     1374 2024-04-26 19:15:16.618265 resty_client-0.0.5/resty/middlewares/status.py
+-rw-r--r--   0        0        0     1250 2024-04-25 16:00:21.928605 resty_client-0.0.5/resty/middlewares/types.py
+-rw-r--r--   0        0        0      166 2024-04-26 10:30:15.667616 resty_client-0.0.5/resty/serializers/__init__.py
+-rw-r--r--   0        0        0      850 2024-04-26 10:37:30.410789 resty_client-0.0.5/resty/serializers/serializers.py
+-rw-r--r--   0        0        0      854 2024-04-26 10:24:34.542849 resty_client-0.0.5/resty/serializers/types.py
+-rw-r--r--   0        0        0      829 2024-04-26 14:16:08.475872 resty_client-0.0.5/resty/types.py
+-rw-r--r--   0        0        0     4302 1970-01-01 00:00:00.000000 resty_client-0.0.5/PKG-INFO
```

### Comparing `resty_client-0.0.4/LICENSE` & `resty_client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.4/pyproject.toml` & `resty_client-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resty-client"
-version = "0.0.4"
+version = "0.0.5"
 description = "RestyClient is a simple, easy-to-use Python library for interacting with REST APIs using Pydantic's powerful data validation and deserialization tools."
 authors = ["CrazyProger1 <crazyproger1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "resty" },
 ]
@@ -15,14 +15,15 @@
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.8.0"
 pytest = "^7.4.4"
 httpx = "^0.26.0"
 black = "^24.4.0"
 coverage = "^7.5.0"
+pytest-asyncio = "^0.23.6"
 
 [tool.ruff]
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
@@ -46,11 +47,10 @@
 ]
 
 [tool.mypy]
 files = ["resty"]
 show_error_codes = true
 strict = true
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `resty_client-0.0.4/README.md` & `resty_client-0.0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -44,157 +44,202 @@
 000002b0: 6974 6875 622e 636f 6d2f 7073 662f 626c  ithub.com/psf/bl
 000002c0: 6163 6b22 3e3c 696d 6720 7372 633d 2268  ack"><img src="h
 000002d0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
 000002e0: 6473 2e69 6f2f 6261 6467 652f 636f 6465  ds.io/badge/code
 000002f0: 2532 3073 7479 6c65 2d62 6c61 636b 2d30  %20style-black-0
 00000300: 3030 3030 302e 7376 6722 2061 6c74 3d22  00000.svg" alt="
 00000310: 436f 6465 2053 7479 6c65 223e 3c2f 613e  Code Style"></a>
-00000320: 0d0a 3c2f 703e 0d0a 0d0a 0d0a 5265 7374  ..</p>......Rest
-00000330: 792d 436c 6965 6e74 2069 7320 6120 7369  y-Client is a si
-00000340: 6d70 6c65 2c20 6561 7379 2d74 6f2d 7573  mple, easy-to-us
-00000350: 6520 5079 7468 6f6e 206c 6962 7261 7279  e Python library
-00000360: 2066 6f72 2069 6e74 6572 6163 7469 6e67   for interacting
-00000370: 2077 6974 6820 5245 5354 2041 5049 7320   with REST APIs 
-00000380: 7573 696e 6720 5079 6461 6e74 6963 2773  using Pydantic's
-00000390: 2070 6f77 6572 6675 6c20 6461 7461 0d0a   powerful data..
-000003a0: 7661 6c69 6461 7469 6f6e 2061 6e64 2064  validation and d
-000003b0: 6573 6572 6961 6c69 7a61 7469 6f6e 2074  eserialization t
-000003c0: 6f6f 6c73 2e20 5468 6973 206c 6962 7261  ools. This libra
-000003d0: 7279 2070 726f 7669 6465 7320 616e 2069  ry provides an i
-000003e0: 6e74 7569 7469 7665 2041 5049 2074 6861  ntuitive API tha
-000003f0: 7420 6d61 6b65 7320 6974 2065 6173 7920  t makes it easy 
-00000400: 746f 206d 616b 6520 4854 5450 2072 6571  to make HTTP req
-00000410: 7565 7374 730d 0a61 6e64 2068 616e 646c  uests..and handl
-00000420: 6520 6461 7461 206f 6e20 7468 6520 636c  e data on the cl
-00000430: 6965 6e74 2073 6964 652e 0d0a 0d0a 2323  ient side.....##
-00000440: 2046 6561 7475 7265 730d 0a0d 0a2d 204d   Features....- M
-00000450: 6964 646c 6577 6172 6520 7379 7374 656d  iddleware system
-00000460: 2c20 7768 6963 6820 616c 6c6f 7773 2079  , which allows y
-00000470: 6f75 2074 6f20 696d 706c 656d 656e 7420  ou to implement 
-00000480: 616e 7920 7061 6769 6e61 7469 6f6e 2c20  any pagination, 
-00000490: 6669 6c74 6572 696e 6720 6f72 2061 7574  filtering or aut
-000004a0: 6865 6e74 6963 6174 696f 6e2e 0d0a 2d20  hentication...- 
-000004b0: 506f 7765 7266 756c 2064 6174 6120 7661  Powerful data va
-000004c0: 6c69 6461 7469 6f6e 2026 2064 6573 6572  lidation & deser
-000004d0: 6961 6c69 7a61 7469 6f6e 2075 7369 6e67  ialization using
-000004e0: 2050 7964 616e 7469 630d 0a2d 2045 6173   Pydantic..- Eas
-000004f0: 792d 746f 2d55 7365 0d0a 0d0a 2323 2049  y-to-Use....## I
-00000500: 6e73 7461 6c6c 6174 696f 6e0d 0a0d 0a55  nstallation....U
-00000510: 7369 6e67 2070 6970 3a0d 0a0d 0a60 6060  sing pip:....```
-00000520: 7368 656c 6c0d 0a70 6970 2069 6e73 7461  shell..pip insta
-00000530: 6c6c 2072 6573 7479 2d63 6c69 656e 740d  ll resty-client.
-00000540: 0a60 6060 0d0a 0d0a 5573 696e 6720 506f  .```....Using Po
-00000550: 6574 7279 3a0d 0a0d 0a60 6060 7368 656c  etry:....```shel
-00000560: 6c0d 0a70 6f65 7472 7920 6164 6420 7265  l..poetry add re
-00000570: 7374 792d 636c 6965 6e74 0d0a 6060 600d  sty-client..```.
-00000580: 0a0d 0a23 2320 4765 7474 696e 672d 5374  ...## Getting-St
-00000590: 6172 7465 640d 0a0d 0a23 2323 2053 6368  arted....### Sch
-000005a0: 656d 610d 0a0d 0a60 6060 7079 7468 6f6e  ema....```python
-000005b0: 0d0a 6672 6f6d 2070 7964 616e 7469 6320  ..from pydantic 
-000005c0: 696d 706f 7274 2042 6173 654d 6f64 656c  import BaseModel
-000005d0: 0d0a 0d0a 0d0a 636c 6173 7320 5072 6f64  ......class Prod
-000005e0: 7563 7428 4261 7365 4d6f 6465 6c29 3a0d  uct(BaseModel):.
-000005f0: 0a20 2020 2069 643a 2069 6e74 207c 204e  .    id: int | N
-00000600: 6f6e 6520 3d20 4e6f 6e65 0d0a 2020 2020  one = None..    
-00000610: 6e61 6d65 3a20 7374 720d 0a20 2020 2064  name: str..    d
-00000620: 6573 6372 6970 7469 6f6e 3a20 7374 720d  escription: str.
-00000630: 0a20 2020 2063 6f64 653a 2073 7472 0d0a  .    code: str..
-00000640: 6060 600d 0a0d 0a23 2323 2053 6572 6961  ```....### Seria
-00000650: 6c69 7a65 720d 0a0d 0a60 6060 7079 7468  lizer....```pyth
-00000660: 6f6e 0d0a 6672 6f6d 2072 6573 7479 2e73  on..from resty.s
-00000670: 6572 6961 6c69 7a65 7273 2069 6d70 6f72  erializers impor
-00000680: 7420 5365 7269 616c 697a 6572 0d0a 0d0a  t Serializer....
-00000690: 0d0a 636c 6173 7320 5072 6f64 7563 7453  ..class ProductS
-000006a0: 6572 6961 6c69 7a65 7228 5365 7269 616c  erializer(Serial
-000006b0: 697a 6572 293a 0d0a 2020 2020 7363 6865  izer):..    sche
-000006c0: 6d61 203d 2050 726f 6475 6374 0d0a 6060  ma = Product..``
-000006d0: 600d 0a0d 0a23 2323 204d 616e 6167 6572  `....### Manager
-000006e0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
-000006f0: 726f 6d20 7265 7374 792e 656e 756d 7320  rom resty.enums 
-00000700: 696d 706f 7274 2028 0d0a 2020 2020 456e  import (..    En
-00000710: 6470 6f69 6e74 2c0d 0a20 2020 2046 6965  dpoint,..    Fie
-00000720: 6c64 0d0a 290d 0a66 726f 6d20 7265 7374  ld..)..from rest
-00000730: 792e 6d61 6e61 6765 7273 2069 6d70 6f72  y.managers impor
-00000740: 7420 4d61 6e61 6765 720d 0a0d 0a0d 0a63  t Manager......c
-00000750: 6c61 7373 2050 726f 6475 6374 4d61 6e61  lass ProductMana
-00000760: 6765 7228 4d61 6e61 6765 7229 3a0d 0a20  ger(Manager):.. 
-00000770: 2020 2073 6572 6961 6c69 7a65 7220 3d20     serializer = 
-00000780: 5072 6f64 7563 7453 6572 6961 6c69 7a65  ProductSerialize
-00000790: 720d 0a20 2020 2065 6e64 706f 696e 7473  r..    endpoints
-000007a0: 203d 207b 0d0a 2020 2020 2020 2020 456e   = {..        En
-000007b0: 6470 6f69 6e74 2e43 5245 4154 453a 2027  dpoint.CREATE: '
-000007c0: 2f70 726f 6475 6374 732f 272c 0d0a 2020  /products/',..  
-000007d0: 2020 2020 2020 456e 6470 6f69 6e74 2e52        Endpoint.R
-000007e0: 4541 443a 2027 2f70 726f 6475 6374 732f  EAD: '/products/
-000007f0: 272c 0d0a 2020 2020 2020 2020 456e 6470  ',..        Endp
-00000800: 6f69 6e74 2e52 4541 445f 4f4e 453a 2027  oint.READ_ONE: '
-00000810: 2f70 726f 6475 6374 732f 7b70 6b7d 2f27  /products/{pk}/'
-00000820: 2c0d 0a20 2020 2020 2020 2045 6e64 706f  ,..        Endpo
-00000830: 696e 742e 5550 4441 5445 3a20 272f 7072  int.UPDATE: '/pr
-00000840: 6f64 7563 7473 2f7b 706b 7d2f 272c 0d0a  oducts/{pk}/',..
-00000850: 2020 2020 2020 2020 456e 6470 6f69 6e74          Endpoint
-00000860: 2e44 454c 4554 453a 2027 2f70 726f 6475  .DELETE: '/produ
-00000870: 6374 732f 7b70 6b7d 2f27 2c0d 0a20 2020  cts/{pk}/',..   
-00000880: 207d 0d0a 2020 2020 6669 656c 6473 203d   }..    fields =
-00000890: 207b 0d0a 2020 2020 2020 2020 4669 656c   {..        Fiel
-000008a0: 642e 5052 494d 4152 593a 2027 6964 272c  d.PRIMARY: 'id',
-000008b0: 0d0a 2020 2020 7d0d 0a60 6060 0d0a 0d0a  ..    }..```....
-000008c0: 2323 2320 4352 5544 0d0a 0d0a 6060 6070  ### CRUD....```p
-000008d0: 7974 686f 6e0d 0a66 726f 6d20 6874 7470  ython..from http
-000008e0: 7820 696d 706f 7274 2041 7379 6e63 436c  x import AsyncCl
-000008f0: 6965 6e74 0d0a 0d0a 6672 6f6d 2072 6573  ient....from res
-00000900: 7479 2e63 6c69 656e 7473 2e68 7474 7078  ty.clients.httpx
-00000910: 2069 6d70 6f72 7420 5245 5354 436c 6965   import RESTClie
-00000920: 6e74 0d0a 0d0a 0d0a 6173 796e 6320 6465  nt......async de
-00000930: 6620 6d61 696e 2829 3a0d 0a20 2020 2078  f main():..    x
-00000940: 636c 6965 6e74 203d 2041 7379 6e63 436c  client = AsyncCl
-00000950: 6965 6e74 2862 6173 655f 7572 6c3d 2768  ient(base_url='h
-00000960: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00000970: 3830 3030 2f27 290d 0a20 2020 2072 6573  8000/')..    res
-00000980: 745f 636c 6965 6e74 203d 2052 4553 5443  t_client = RESTC
-00000990: 6c69 656e 7428 7863 6c69 656e 743d 7863  lient(xclient=xc
-000009a0: 6c69 656e 7429 0d0a 0d0a 2020 2020 7072  lient)....    pr
-000009b0: 6f64 7563 7420 3d20 5072 6f64 7563 7428  oduct = Product(
-000009c0: 0d0a 2020 2020 2020 2020 6e61 6d65 3d27  ..        name='
-000009d0: 4669 7273 7420 7072 6f64 272c 0d0a 2020  First prod',..  
-000009e0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-000009f0: 6e3d 274d 7920 4465 7363 272c 0d0a 2020  n='My Desc',..  
-00000a00: 2020 2020 2020 636f 6465 3d27 3132 3357        code='123W
-00000a10: 3331 5127 0d0a 2020 2020 290d 0a0d 0a20  31Q'..    ).... 
-00000a20: 2020 2023 2043 7265 6174 650d 0a20 2020     # Create..   
-00000a30: 2063 7265 6174 6564 203d 2061 7761 6974   created = await
-00000a40: 2050 726f 6475 6374 4d61 6e61 6765 722e   ProductManager.
-00000a50: 6372 6561 7465 2872 6573 745f 636c 6965  create(rest_clie
-00000a60: 6e74 2c20 7072 6f64 7563 7429 0d0a 0d0a  nt, product)....
-00000a70: 2020 2020 2320 5265 6164 0d0a 2020 2020      # Read..    
-00000a80: 6d79 5f70 726f 6475 6374 203d 2061 7761  my_product = awa
-00000a90: 6974 2050 726f 6475 6374 4d61 6e61 6765  it ProductManage
-00000aa0: 722e 7265 6164 5f6f 6e65 2872 6573 745f  r.read_one(rest_
-00000ab0: 636c 6965 6e74 2c20 6372 6561 7465 642e  client, created.
-00000ac0: 6964 290d 0a0d 0a20 2020 2066 6f72 2070  id)....    for p
-00000ad0: 726f 6420 696e 2061 7761 6974 2050 726f  rod in await Pro
-00000ae0: 6475 6374 4d61 6e61 6765 722e 7265 6164  ductManager.read
-00000af0: 2872 6573 745f 636c 6965 6e74 293a 0d0a  (rest_client):..
-00000b00: 2020 2020 2020 2020 7072 696e 7428 7072          print(pr
-00000b10: 6f64 2e6e 616d 6529 0d0a 0d0a 2020 2020  od.name)....    
-00000b20: 2320 5570 6461 7465 0d0a 2020 2020 6d79  # Update..    my
-00000b30: 5f70 726f 6475 6374 2e64 6573 6372 6970  _product.descrip
-00000b40: 7469 6f6e 203d 2027 5157 4552 5459 270d  tion = 'QWERTY'.
-00000b50: 0a20 2020 2061 7761 6974 2050 726f 6475  .    await Produ
-00000b60: 6374 4d61 6e61 6765 722e 7570 6461 7465  ctManager.update
-00000b70: 2872 6573 745f 636c 6965 6e74 2c20 6d79  (rest_client, my
-00000b80: 5f70 726f 6475 6374 290d 0a0d 0a20 2020  _product)....   
-00000b90: 2023 2044 656c 6574 650d 0a20 2020 2061   # Delete..    a
-00000ba0: 7761 6974 2050 726f 6475 6374 4d61 6e61  wait ProductMana
-00000bb0: 6765 722e 6465 6c65 7465 2872 6573 745f  ger.delete(rest_
-00000bc0: 636c 6965 6e74 2c20 6d79 5f70 726f 6475  client, my_produ
-00000bd0: 6374 2e69 6429 0d0a 6060 600d 0a0d 0a23  ct.id)..```....#
-00000be0: 2320 5374 6174 7573 0d0a 0d0a 6060 302e  # Status....``0.
-00000bf0: 302e 3460 6020 2d20 2a2a 5245 4c45 4153  0.4`` - **RELEAS
-00000c00: 4544 2a2a 0d0a 0d0a 2323 204c 6963 656e  ED**....## Licen
-00000c10: 6365 0d0a 0d0a 5265 7374 792d 436c 6965  ce....Resty-Clie
-00000c20: 6e74 2069 7320 7265 6c65 6173 6564 2075  nt is released u
-00000c30: 6e64 6572 2074 6865 204d 4954 204c 6963  nder the MIT Lic
-00000c40: 656e 7365 2e20 5365 6520 7468 6520 6275  ense. See the bu
-00000c50: 6e64 6c65 6420 5b4c 4943 454e 5345 5d28  ndled [LICENSE](
-00000c60: 4c49 4345 4e53 4529 2066 696c 6520 666f  LICENSE) file fo
-00000c70: 7220 6465 7461 696c 732e                 r details.
+00000320: 0d0a 3c69 6d67 2073 7263 3d22 6874 7470  ..<img src="http
+00000330: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000340: 696f 2f62 6164 6765 2f63 6f76 6572 6167  io/badge/coverag
+00000350: 652d 3130 3025 3235 2d62 7269 6768 7467  e-100%25-brightg
+00000360: 7265 656e 2220 616c 743d 2243 6f76 6572  reen" alt="Cover
+00000370: 6167 6522 2f3e 0d0a 3c2f 703e 0d0a 0d0a  age"/>..</p>....
+00000380: 0d0a 5265 7374 792d 436c 6965 6e74 2069  ..Resty-Client i
+00000390: 7320 6120 7369 6d70 6c65 2c20 6561 7379  s a simple, easy
+000003a0: 2d74 6f2d 7573 6520 5079 7468 6f6e 206c  -to-use Python l
+000003b0: 6962 7261 7279 2066 6f72 2069 6e74 6572  ibrary for inter
+000003c0: 6163 7469 6e67 2077 6974 6820 5245 5354  acting with REST
+000003d0: 2041 5049 7320 7573 696e 6720 5079 6461   APIs using Pyda
+000003e0: 6e74 6963 2773 2070 6f77 6572 6675 6c20  ntic's powerful 
+000003f0: 6461 7461 0d0a 7661 6c69 6461 7469 6f6e  data..validation
+00000400: 2061 6e64 2064 6573 6572 6961 6c69 7a61   and deserializa
+00000410: 7469 6f6e 2074 6f6f 6c73 2e20 5468 6973  tion tools. This
+00000420: 206c 6962 7261 7279 2070 726f 7669 6465   library provide
+00000430: 7320 616e 2069 6e74 7569 7469 7665 2041  s an intuitive A
+00000440: 5049 2074 6861 7420 6d61 6b65 7320 6974  PI that makes it
+00000450: 2065 6173 7920 746f 206d 616b 6520 4854   easy to make HT
+00000460: 5450 2072 6571 7565 7374 730d 0a61 6e64  TP requests..and
+00000470: 2068 616e 646c 6520 6461 7461 206f 6e20   handle data on 
+00000480: 7468 6520 636c 6965 6e74 2073 6964 652e  the client side.
+00000490: 0d0a 0d0a 2323 2046 6561 7475 7265 730d  ....## Features.
+000004a0: 0a0d 0a2d 204d 6964 646c 6577 6172 6520  ...- Middleware 
+000004b0: 7379 7374 656d 2c20 7768 6963 6820 616c  system, which al
+000004c0: 6c6f 7773 2079 6f75 2074 6f20 696d 706c  lows you to impl
+000004d0: 656d 656e 7420 616e 7920 7061 6769 6e61  ement any pagina
+000004e0: 7469 6f6e 2c20 6669 6c74 6572 696e 6720  tion, filtering 
+000004f0: 6f72 2061 7574 6865 6e74 6963 6174 696f  or authenticatio
+00000500: 6e2e 0d0a 2d20 506f 7765 7266 756c 2064  n...- Powerful d
+00000510: 6174 6120 7661 6c69 6461 7469 6f6e 2026  ata validation &
+00000520: 2064 6573 6572 6961 6c69 7a61 7469 6f6e   deserialization
+00000530: 2075 7369 6e67 2050 7964 616e 7469 630d   using Pydantic.
+00000540: 0a2d 2045 6173 792d 746f 2d55 7365 0d0a  .- Easy-to-Use..
+00000550: 0d0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000560: 6e0d 0a0d 0a55 7369 6e67 2070 6970 3a0d  n....Using pip:.
+00000570: 0a0d 0a60 6060 7368 656c 6c0d 0a70 6970  ...```shell..pip
+00000580: 2069 6e73 7461 6c6c 2072 6573 7479 2d63   install resty-c
+00000590: 6c69 656e 740d 0a60 6060 0d0a 0d0a 5573  lient..```....Us
+000005a0: 696e 6720 506f 6574 7279 3a0d 0a0d 0a60  ing Poetry:....`
+000005b0: 6060 7368 656c 6c0d 0a70 6f65 7472 7920  ``shell..poetry 
+000005c0: 6164 6420 7265 7374 792d 636c 6965 6e74  add resty-client
+000005d0: 0d0a 6060 600d 0a0d 0a23 2320 4765 7474  ..```....## Gett
+000005e0: 696e 672d 5374 6172 7465 640d 0a0d 0a53  ing-Started....S
+000005f0: 6565 205b 6578 616d 706c 6573 5d28 6578  ee [examples](ex
+00000600: 616d 706c 6573 2920 666f 7220 6d6f 7265  amples) for more
+00000610: 2e0d 0a0d 0a23 2323 2053 6368 656d 6173  .....### Schemas
+00000620: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
+00000630: 726f 6d20 7265 7374 792e 7479 7065 7320  rom resty.types 
+00000640: 696d 706f 7274 2053 6368 656d 610d 0a0d  import Schema...
+00000650: 0a0d 0a63 6c61 7373 2055 7365 7243 7265  ...class UserCre
+00000660: 6174 6553 6368 656d 6128 5363 6865 6d61  ateSchema(Schema
+00000670: 293a 0d0a 2020 2020 7573 6572 6e61 6d65  ):..    username
+00000680: 3a20 7374 720d 0a20 2020 2065 6d61 696c  : str..    email
+00000690: 3a20 7374 720d 0a20 2020 2070 6173 7377  : str..    passw
+000006a0: 6f72 643a 2073 7472 0d0a 2020 2020 6167  ord: str..    ag
+000006b0: 653a 2069 6e74 0d0a 0d0a 0d0a 636c 6173  e: int......clas
+000006c0: 7320 5573 6572 5265 6164 5363 6865 6d61  s UserReadSchema
+000006d0: 2853 6368 656d 6129 3a0d 0a20 2020 2069  (Schema):..    i
+000006e0: 643a 2069 6e74 0d0a 2020 2020 7573 6572  d: int..    user
+000006f0: 6e61 6d65 3a20 7374 720d 0a20 2020 2065  name: str..    e
+00000700: 6d61 696c 3a20 7374 720d 0a20 2020 2061  mail: str..    a
+00000710: 6765 3a20 696e 740d 0a0d 0a0d 0a63 6c61  ge: int......cla
+00000720: 7373 2055 7365 7255 7064 6174 6553 6368  ss UserUpdateSch
+00000730: 656d 6128 5363 6865 6d61 293a 0d0a 2020  ema(Schema):..  
+00000740: 2020 7573 6572 6e61 6d65 3a20 7374 7220    username: str 
+00000750: 3d20 4e6f 6e65 0d0a 2020 2020 656d 6169  = None..    emai
+00000760: 6c3a 2073 7472 203d 204e 6f6e 650d 0a60  l: str = None..`
+00000770: 6060 0d0a 0d0a 2323 2320 4d61 6e61 6765  ``....### Manage
+00000780: 720d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  r....```python..
+00000790: 6672 6f6d 2072 6573 7479 2e6d 616e 6167  from resty.manag
+000007a0: 6572 7320 696d 706f 7274 204d 616e 6167  ers import Manag
+000007b0: 6572 0d0a 6672 6f6d 2072 6573 7479 2e65  er..from resty.e
+000007c0: 6e75 6d73 2069 6d70 6f72 7420 456e 6470  nums import Endp
+000007d0: 6f69 6e74 2c20 4669 656c 640d 0a0d 0a0d  oint, Field.....
+000007e0: 0a63 6c61 7373 2055 7365 724d 616e 6167  .class UserManag
+000007f0: 6572 284d 616e 6167 6572 293a 0d0a 2020  er(Manager):..  
+00000800: 2020 656e 6470 6f69 6e74 7320 3d20 7b0d    endpoints = {.
+00000810: 0a20 2020 2020 2020 2045 6e64 706f 696e  .        Endpoin
+00000820: 742e 4352 4541 5445 3a20 2275 7365 7273  t.CREATE: "users
+00000830: 2f22 2c0d 0a20 2020 2020 2020 2045 6e64  /",..        End
+00000840: 706f 696e 742e 5245 4144 3a20 2275 7365  point.READ: "use
+00000850: 7273 2f22 2c0d 0a20 2020 2020 2020 2045  rs/",..        E
+00000860: 6e64 706f 696e 742e 5245 4144 5f4f 4e45  ndpoint.READ_ONE
+00000870: 3a20 2275 7365 7273 2f7b 706b 7d22 2c0d  : "users/{pk}",.
+00000880: 0a20 2020 2020 2020 2045 6e64 706f 696e  .        Endpoin
+00000890: 742e 5550 4441 5445 3a20 2275 7365 7273  t.UPDATE: "users
+000008a0: 2f7b 706b 7d22 2c0d 0a20 2020 2020 2020  /{pk}",..       
+000008b0: 2045 6e64 706f 696e 742e 4445 4c45 5445   Endpoint.DELETE
+000008c0: 3a20 2275 7365 7273 2f7b 706b 7d22 2c0d  : "users/{pk}",.
+000008d0: 0a20 2020 207d 0d0a 2020 2020 6669 656c  .    }..    fiel
+000008e0: 6473 203d 207b 0d0a 2020 2020 2020 2020  ds = {..        
+000008f0: 4669 656c 642e 5052 494d 4152 593a 2022  Field.PRIMARY: "
+00000900: 6964 222c 0d0a 2020 2020 7d0d 0a60 6060  id",..    }..```
+00000910: 0d0a 0d0a 2323 2320 4352 5544 0d0a 0d0a  ....### CRUD....
+00000920: 6060 6070 7974 686f 6e0d 0a69 6d70 6f72  ```python..impor
+00000930: 7420 6173 796e 6369 6f0d 0a0d 0a69 6d70  t asyncio....imp
+00000940: 6f72 7420 6874 7470 780d 0a0d 0a66 726f  ort httpx....fro
+00000950: 6d20 7265 7374 792e 636c 6965 6e74 732e  m resty.clients.
+00000960: 6874 7470 7820 696d 706f 7274 2052 4553  httpx import RES
+00000970: 5443 6c69 656e 740d 0a0d 0a0d 0a61 7379  TClient......asy
+00000980: 6e63 2064 6566 206d 6169 6e28 293a 0d0a  nc def main():..
+00000990: 2020 2020 636c 6965 6e74 203d 2052 4553      client = RES
+000009a0: 5443 6c69 656e 7428 6874 7470 782e 4173  TClient(httpx.As
+000009b0: 796e 6343 6c69 656e 7428 6261 7365 5f75  yncClient(base_u
+000009c0: 726c 3d22 6874 7470 733a 2f2f 6c6f 6361  rl="https://loca
+000009d0: 6c68 6f73 743a 3830 3030 2229 290d 0a0d  lhost:8000"))...
+000009e0: 0a20 2020 2072 6573 706f 6e73 6520 3d20  .    response = 
+000009f0: 6177 6169 7420 5573 6572 4d61 6e61 6765  await UserManage
+00000a00: 722e 6372 6561 7465 280d 0a20 2020 2020  r.create(..     
+00000a10: 2020 2063 6c69 656e 743d 636c 6965 6e74     client=client
+00000a20: 2c0d 0a20 2020 2020 2020 206f 626a 3d55  ,..        obj=U
+00000a30: 7365 7243 7265 6174 6553 6368 656d 6128  serCreateSchema(
+00000a40: 0d0a 2020 2020 2020 2020 2020 2020 7573  ..            us
+00000a50: 6572 6e61 6d65 3d22 6164 6d69 6e22 2c0d  ername="admin",.
+00000a60: 0a20 2020 2020 2020 2020 2020 2065 6d61  .            ema
+00000a70: 696c 3d22 6164 6d69 6e40 6164 6d69 6e2e  il="admin@admin.
+00000a80: 636f 6d22 2c0d 0a20 2020 2020 2020 2020  com",..         
+00000a90: 2020 2070 6173 7377 6f72 643d 2261 646d     password="adm
+00000aa0: 696e 222c 0d0a 2020 2020 2020 2020 2020  in",..          
+00000ab0: 2020 6167 653d 3139 2c0d 0a20 2020 2020    age=19,..     
+00000ac0: 2020 2029 2c0d 0a20 2020 2020 2020 2072     ),..        r
+00000ad0: 6573 706f 6e73 655f 7479 7065 3d55 7365  esponse_type=Use
+00000ae0: 7252 6561 6453 6368 656d 612c 0d0a 2020  rReadSchema,..  
+00000af0: 2020 290d 0a20 2020 2070 7269 6e74 2872    )..    print(r
+00000b00: 6573 706f 6e73 6529 2020 2320 6964 3d31  esponse)  # id=1
+00000b10: 2075 7365 726e 616d 653d 2761 646d 696e   username='admin
+00000b20: 2720 656d 6169 6c3d 2761 646d 696e 4061  ' email='admin@a
+00000b30: 646d 696e 2e63 6f6d 2720 6167 653d 3139  dmin.com' age=19
+00000b40: 0d0a 0d0a 2020 2020 7265 7370 6f6e 7365  ....    response
+00000b50: 203d 2061 7761 6974 2055 7365 724d 616e   = await UserMan
+00000b60: 6167 6572 2e72 6561 6428 0d0a 2020 2020  ager.read(..    
+00000b70: 2020 2020 636c 6965 6e74 3d63 6c69 656e      client=clien
+00000b80: 742c 0d0a 2020 2020 2020 2020 7265 7370  t,..        resp
+00000b90: 6f6e 7365 5f74 7970 653d 5573 6572 5265  onse_type=UserRe
+00000ba0: 6164 5363 6865 6d61 2c0d 0a20 2020 2029  adSchema,..    )
+00000bb0: 0d0a 0d0a 2020 2020 666f 7220 6f62 6a20  ....    for obj 
+00000bc0: 696e 2072 6573 706f 6e73 653a 0d0a 2020  in response:..  
+00000bd0: 2020 2020 2020 7072 696e 7428 6f62 6a29        print(obj)
+00000be0: 2020 2320 6964 3d31 2075 7365 726e 616d    # id=1 usernam
+00000bf0: 653d 2761 646d 696e 2720 656d 6169 6c3d  e='admin' email=
+00000c00: 2761 646d 696e 4061 646d 696e 2e63 6f6d  'admin@admin.com
+00000c10: 2720 6167 653d 3139 0d0a 0d0a 2020 2020  ' age=19....    
+00000c20: 7265 7370 6f6e 7365 203d 2061 7761 6974  response = await
+00000c30: 2055 7365 724d 616e 6167 6572 2e72 6561   UserManager.rea
+00000c40: 645f 6f6e 6528 0d0a 2020 2020 2020 2020  d_one(..        
+00000c50: 636c 6965 6e74 3d63 6c69 656e 742c 0d0a  client=client,..
+00000c60: 2020 2020 2020 2020 6f62 6a5f 6f72 5f70          obj_or_p
+00000c70: 6b3d 312c 0d0a 2020 2020 2020 2020 7265  k=1,..        re
+00000c80: 7370 6f6e 7365 5f74 7970 653d 5573 6572  sponse_type=User
+00000c90: 5265 6164 5363 6865 6d61 2c0d 0a20 2020  ReadSchema,..   
+00000ca0: 2029 0d0a 0d0a 2020 2020 7072 696e 7428   )....    print(
+00000cb0: 7265 7370 6f6e 7365 2920 2023 2069 643d  response)  # id=
+00000cc0: 3120 7573 6572 6e61 6d65 3d27 6164 6d69  1 username='admi
+00000cd0: 6e27 2065 6d61 696c 3d27 6164 6d69 6e40  n' email='admin@
+00000ce0: 6164 6d69 6e2e 636f 6d27 2061 6765 3d31  admin.com' age=1
+00000cf0: 390d 0a0d 0a20 2020 2072 6573 706f 6e73  9....    respons
+00000d00: 6520 3d20 6177 6169 7420 5573 6572 4d61  e = await UserMa
+00000d10: 6e61 6765 722e 7570 6461 7465 280d 0a20  nager.update(.. 
+00000d20: 2020 2020 2020 2063 6c69 656e 743d 636c         client=cl
+00000d30: 6965 6e74 2c0d 0a20 2020 2020 2020 206f  ient,..        o
+00000d40: 626a 3d55 7365 7255 7064 6174 6553 6368  bj=UserUpdateSch
+00000d50: 656d 6128 6964 3d31 2c20 7573 6572 6e61  ema(id=1, userna
+00000d60: 6d65 3d22 6164 6d69 6e31 3233 222c 2029  me="admin123", )
+00000d70: 2c0d 0a20 2020 2020 2020 2072 6573 706f  ,..        respo
+00000d80: 6e73 655f 7479 7065 3d55 7365 7252 6561  nse_type=UserRea
+00000d90: 6453 6368 656d 612c 0d0a 2020 2020 290d  dSchema,..    ).
+00000da0: 0a0d 0a20 2020 2070 7269 6e74 2872 6573  ...    print(res
+00000db0: 706f 6e73 6529 2020 2320 6964 3d31 2075  ponse)  # id=1 u
+00000dc0: 7365 726e 616d 653d 2761 646d 696e 3132  sername='admin12
+00000dd0: 3327 2065 6d61 696c 3d27 6164 6d69 6e40  3' email='admin@
+00000de0: 6164 6d69 6e2e 636f 6d27 2061 6765 3d31  admin.com' age=1
+00000df0: 390d 0a0d 0a20 2020 2061 7761 6974 2055  9....    await U
+00000e00: 7365 724d 616e 6167 6572 2e64 656c 6574  serManager.delet
+00000e10: 6528 0d0a 2020 2020 2020 2020 636c 6965  e(..        clie
+00000e20: 6e74 3d63 6c69 656e 742c 0d0a 2020 2020  nt=client,..    
+00000e30: 2020 2020 6f62 6a5f 6f72 5f70 6b3d 312c      obj_or_pk=1,
+00000e40: 0d0a 2020 2020 2020 2020 6578 7065 6374  ..        expect
+00000e50: 6564 5f73 7461 7475 733d 3230 342c 0d0a  ed_status=204,..
+00000e60: 2020 2020 290d 0a0d 0a0d 0a69 6620 5f5f      )......if __
+00000e70: 6e61 6d65 5f5f 203d 3d20 225f 5f6d 6169  name__ == "__mai
+00000e80: 6e5f 5f22 3a0d 0a20 2020 2061 7379 6e63  n__":..    async
+00000e90: 696f 2e72 756e 286d 6169 6e28 2929 0d0a  io.run(main())..
+00000ea0: 6060 600d 0a0d 0a23 2320 5374 6174 7573  ```....## Status
+00000eb0: 0d0a 0d0a 6060 302e 302e 3560 6020 2d20  ....``0.0.5`` - 
+00000ec0: 2a2a 5245 4c45 4153 4544 2a2a 0d0a 0d0a  **RELEASED**....
+00000ed0: 2323 204c 6963 656e 6365 0d0a 0d0a 5265  ## Licence....Re
+00000ee0: 7374 792d 436c 6965 6e74 2069 7320 7265  sty-Client is re
+00000ef0: 6c65 6173 6564 2075 6e64 6572 2074 6865  leased under the
+00000f00: 204d 4954 204c 6963 656e 7365 2e20 5365   MIT License. Se
+00000f10: 6520 7468 6520 6275 6e64 6c65 6420 5b4c  e the bundled [L
+00000f20: 4943 454e 5345 5d28 4c49 4345 4e53 4529  ICENSE](LICENSE)
+00000f30: 2066 696c 6520 666f 7220 6465 7461 696c   file for detail
+00000f40: 732e                                     s.
```

