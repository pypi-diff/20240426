# Comparing `tmp/gpt3_tokenizer-0.1.4.tar.gz` & `tmp/gpt3_tokenizer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt3_tokenizer-0.1.4.tar", max compression
+gzip compressed data, was "gpt3_tokenizer-0.1.5.tar", max compression
```

## Comparing `gpt3_tokenizer-0.1.4.tar` & `gpt3_tokenizer-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-05-16 00:41:06.027226 gpt3_tokenizer-0.1.4/LICENSE
--rw-r--r--   0        0        0      984 2023-05-16 00:41:06.027226 gpt3_tokenizer-0.1.4/README.rst
--rw-r--r--   0        0        0      125 2023-05-16 00:41:06.027226 gpt3_tokenizer-0.1.4/gpt3_tokenizer/__init__.py
--rw-r--r--   0        0        0     2015 2023-05-16 00:41:06.027226 gpt3_tokenizer-0.1.4/gpt3_tokenizer/_entry.py
--rw-r--r--   0        0        0     3202 2023-05-16 00:41:06.027226 gpt3_tokenizer-0.1.4/gpt3_tokenizer/_functions.py
--rw-r--r--   0        0        0  1042301 2023-05-16 00:41:06.035225 gpt3_tokenizer-0.1.4/gpt3_tokenizer/data/encoder.json
--rw-r--r--   0        0        0   456318 2023-05-16 00:41:06.039225 gpt3_tokenizer-0.1.4/gpt3_tokenizer/data/vocab.bpe
--rw-r--r--   0        0        0     1307 2023-05-16 00:50:16.998990 gpt3_tokenizer-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 gpt3_tokenizer-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-26 15:50:07.758283 gpt3_tokenizer-0.1.5/LICENSE
+-rw-r--r--   0        0        0      967 2024-04-26 16:01:08.220435 gpt3_tokenizer-0.1.5/README.rst
+-rw-r--r--   0        0        0      125 2024-04-26 15:50:07.758489 gpt3_tokenizer-0.1.5/gpt3_tokenizer/__init__.py
+-rw-r--r--   0        0        0     1869 2024-04-26 16:09:26.280525 gpt3_tokenizer-0.1.5/gpt3_tokenizer/_entry.py
+-rw-r--r--   0        0        0     3279 2024-04-26 16:14:26.381264 gpt3_tokenizer-0.1.5/gpt3_tokenizer/_functions.py
+-rw-r--r--   0        0        0  1042301 2024-04-26 15:50:07.761234 gpt3_tokenizer-0.1.5/gpt3_tokenizer/data/encoder.json
+-rw-r--r--   0        0        0   456318 2024-04-26 15:50:07.762646 gpt3_tokenizer-0.1.5/gpt3_tokenizer/data/vocab.bpe
+-rw-r--r--   0        0        0     1318 2024-04-26 18:04:16.123739 gpt3_tokenizer-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 gpt3_tokenizer-0.1.5/PKG-INFO
```

### Comparing `gpt3_tokenizer-0.1.4/LICENSE` & `gpt3_tokenizer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt3_tokenizer-0.1.4/README.rst` & `gpt3_tokenizer-0.1.5/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 gpt3_tokenizer
 ===============
 | An `OpenAI`_ GPT3 helper library for encoding/decoding strings and counting tokens.
 | Counting tokens gives the same output as OpenAI's `tokenizer`_
 |
-| Tested with versions: **2.7.12**, **2.7.18** and all **3.x.x** versions
+| Supported python versions: **>=2.7 <3.0** OR **>=3.3**
 
 Installing
 --------------
 .. code-block:: bash
 
     pip install gpt3_tokenizer
```

### Comparing `gpt3_tokenizer-0.1.4/gpt3_tokenizer/_entry.py` & `gpt3_tokenizer-0.1.5/gpt3_tokenizer/_entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,65 @@
 from builtins import str
 
 import regex
 
-from gpt3_tokenizer._functions import (_DEFAULT_ENCODING, _bpe,
-                                       _bytes_to_unicode, _dict_zip,
-                                       _encode_string, _get_bpe_merges,
-                                       _init_encoder)
+from gpt3_tokenizer._functions import (
+    _DEFAULT_ENCODING,
+    _bpe,
+    _bytes_to_unicode,
+    _dict_zip,
+    _encode_string,
+    _get_bpe_merges,
+    _init_encoder,
+)
 
 _bpe_merges = _get_bpe_merges()
 _bpe_ranks = _dict_zip(_bpe_merges, range(0, len(_bpe_merges)))
 _REGEX_PATTERN = r"'s|'t|'re|'ve|'m|'ll|'d| ?\p{L}+| ?\p{N}+| ?[^\s\p{L}\p{N}]+|\s+(?!\S)|\s+"
 _encoder = _init_encoder()
-_decoder = {v: k for k,v in _encoder.items()}
+_decoder = {v: k for k, v in _encoder.items()}
 _byte_encoder = _bytes_to_unicode()
-_byte_decoder = {v: k for k,v in _byte_encoder.items()}
+_byte_decoder = {v: k for k, v in _byte_encoder.items()}
+
 
 def encode(text):
-    """ 
-        Transforms a string into an array of tokens 
-        :param text: string to be encoded
-        :type text: str
-        :returns: an array of ints (tokens)
+    """
+    Transforms a string into an array of tokens
+    :param text: string to be encoded
+    :type text: str
+    :returns: an array of ints (tokens)
     """
     if not isinstance(text, str):
-        text = text.decode(_DEFAULT_ENCODING)    
+        text = text.decode(_DEFAULT_ENCODING)
     bpe_tokens = []
     regex_compiled = regex.compile(_REGEX_PATTERN, regex.UNICODE)
     matches = regex_compiled.findall(text)
     for token in matches:
-        token = ''.join([_byte_encoder[x] for x in _encode_string(token)])
-        new_tokens = [_encoder[x] for x in _bpe(token, _bpe_ranks).split(' ')]
+        token = "".join([_byte_encoder[x] for x in _encode_string(token)])
+        new_tokens = [_encoder[x] for x in _bpe(token, _bpe_ranks).split(" ")]
         bpe_tokens.extend(new_tokens)
     return bpe_tokens
 
+
 def decode(tokens):
-    """ 
-        Transforms back an array of tokens into the original string
-        :param tokens: an array of ints
-        :type tokens: list
-        :returns: the original text which was encoded before
     """
-    text = ''.join([_decoder[x] for x in tokens])
+    Transforms back an array of tokens into the original string
+    :param tokens: an array of ints
+    :type tokens: list
+    :returns: the original text which was encoded before
+    """
+    text = "".join([_decoder[x] for x in tokens])
     textarr = [int(_byte_decoder[x]) for x in list(text)]
     text = bytearray(textarr).decode("utf-8")
     return text
 
+
 def count_tokens(text):
-    """ 
-        Returns an integer representing the tokens count of a given string 
-        :param text: string to count tokens from
-        :type text: str
-        :returns: int representing the tokens count
-        
+    """
+    Returns an integer representing the tokens count of a given string
+    :param text: string to count tokens from
+    :type text: str
+    :returns: int representing the tokens count
+
     """
     encoded = encode(text)
     return len(encoded)
```

### Comparing `gpt3_tokenizer-0.1.4/gpt3_tokenizer/_functions.py` & `gpt3_tokenizer-0.1.5/gpt3_tokenizer/_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,60 +6,69 @@
 from itertools import chain
 
 import regex
 import six
 
 _DEFAULT_ENCODING = "utf-8"
 
+
 def _init_encoder():
-    with open(os.path.join(os.path.dirname(__file__), 'data/encoder.json'), 'r') as f:
+    with open(os.path.join(os.path.dirname(__file__), "data/encoder.json"), "r", encoding=_DEFAULT_ENCODING) as f:
         encoder = json.load(f)
         return encoder
 
+
 def _get_bpe_merges():
-    with open(os.path.join(os.path.dirname(__file__), "data/vocab.bpe"), "r") as f:
-        bpe_lines = f.readlines()    
-        sliced = bpe_lines[1:len(bpe_lines)-1]
+    with open(os.path.join(os.path.dirname(__file__), "data/vocab.bpe"), "r", encoding=_DEFAULT_ENCODING) as f:
+        bpe_lines = f.readlines()
+        sliced = bpe_lines[1 : len(bpe_lines) - 1]
         bpe_merges = [regex.split(r"(\s+)", s) for s in sliced]
         final_merges = []
         for merge in bpe_merges:
             final_merges.append([m for m in merge if len(m.strip()) > 0])
         return final_merges
 
+
 def _dict_zip(x, y):
     result = {}
     for i in y:
         key = tuple(x[i])
         result[key] = y[i]
     return result
 
+
 cache = {}
 
+
 def _encode_string(token):
     return [str(t) for t in list(bytearray(token.encode(_DEFAULT_ENCODING)))]
 
+
 def _range(x, y):
     res = [val for val in range(y)][x:]
     return res
 
+
 def _ord(x):
     if not isinstance(x, str):
         x = x.decode(_DEFAULT_ENCODING)
     res = ord(x[0])
     return res
 
+
 def _get_pairs(word):
     pairs = []
     prev_char = word[0]
     for i in range(1, len(word)):
         ch = word[i]
         pairs.append([prev_char, ch])
         prev_char = ch
     return pairs
 
+
 def _bpe(token, bpe_ranks):
     if token in cache:
         return cache[token]
     word = list(token)
     pairs = _get_pairs(word)
     if not pairs:
         return token
@@ -87,40 +96,42 @@
             except:
                 pass
             if j == -1:
                 new_word.extend(word[i:])
                 break
             new_word.extend(word[i:j])
             i = j
-            if word[i] == first and i < len(word)-1 and word[i+1] == second:
-                new_word.append(first+second)
+            if word[i] == first and i < len(word) - 1 and word[i + 1] == second:
+                new_word.append(first + second)
                 i += 2
             else:
                 new_word.append(word[i])
                 i += 1
 
         word = new_word
         if len(word) == 1:
             break
         pairs = _get_pairs(word)
-    
-    word = ' '.join(word)
+
+    word = " ".join(word)
     cache[token] = word
     return word
 
 
 def _bytes_to_unicode():
-    bs = list(chain(_range(_ord('!'), _ord('~') + 1), _range(_ord('¡'), _ord('¬') + 1), _range(_ord('®'), _ord('ÿ') + 1)))
+    bs = list(
+        chain(_range(_ord("!"), _ord("~") + 1), _range(_ord("¡"), _ord("¬") + 1), _range(_ord("®"), _ord("ÿ") + 1))
+    )
     cs = bs[:]
     n = 0
     b = 0
-    while b < 2 ** 8:
+    while b < 2**8:
         if not b in bs:
             bs.append(b)
-            cs.append(2 ** 8 + n)
+            cs.append(2**8 + n)
             n += 1
         b += 1
 
     cs = list(map(lambda x: six.unichr(x), cs))
     result = {}
     for i in range(len(bs)):
         result[str(bs[i])] = cs[i]
```

### Comparing `gpt3_tokenizer-0.1.4/gpt3_tokenizer/data/encoder.json` & `gpt3_tokenizer-0.1.5/gpt3_tokenizer/data/encoder.json`

 * *Files identical despite different names*

### Comparing `gpt3_tokenizer-0.1.4/gpt3_tokenizer/data/vocab.bpe` & `gpt3_tokenizer-0.1.5/gpt3_tokenizer/data/vocab.bpe`

 * *Files identical despite different names*

### Comparing `gpt3_tokenizer-0.1.4/pyproject.toml` & `gpt3_tokenizer-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt3_tokenizer"
-version = "0.1.4"
+version = "0.1.5"
 description = "Encoder/Decoder and tokens counter for GPT3"
 authors = ["Alison Ferrenha"]
 readme = "README.rst"
 license = "MIT"
 keywords = ["openai", "gpt", "gpt-3", "gpt3", "gpt4", "gpt-4", "tokenizer"]
 homepage = "https://github.com/alisonjf/gpt3-tokenizer"
 repository = "https://github.com/alisonjf/gpt3-tokenizer"
@@ -19,30 +19,26 @@
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     "Operating System :: OS Independent",
 ]
 
-include = [
-    "LICENSE",
-]
+include = ["LICENSE"]
 
-packages = [
-    { include = "gpt3_tokenizer" },
-]
+packages = [{ include = "gpt3_tokenizer" }]
 
 [tool.poetry.dependencies]
-python = ">=2.7"
+python = ">=2.7,<3.0.dev0 || >=3.3.dev0"
 future = "^0.18.3"
 six = "^1.16.0"
-regex  = [
+regex = [
     { version = "2021.11.10", python = "<3" },
-    { version = "*", python = ">=3" }
+    { version = "*", python = ">=3" },
 ]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.distutils.bdist_wheel]
-universal = true
+universal = true
```

