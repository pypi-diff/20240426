# Comparing `tmp/bert4keras3-1.3-py3-none-any.whl.zip` & `tmp/bert4keras3-1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 43948 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      148 b- defN 24-Apr-25 09:18 bert4keras3/__init__.py
--rw-rw-rw-  2.0 fat    23204 b- defN 24-Apr-25 09:17 bert4keras3/backend.py
--rw-rw-rw-  2.0 fat    11442 b- defN 24-Apr-25 09:17 bert4keras3/layers.py
--rw-rw-rw-  2.0 fat     5211 b- defN 24-Apr-25 09:17 bert4keras3/models.py
--rw-rw-rw-  2.0 fat    30152 b- defN 24-Apr-25 09:17 bert4keras3/ops.py
--rw-rw-rw-  2.0 fat    27955 b- defN 24-Apr-25 09:17 bert4keras3/snippets.py
--rw-rw-rw-  2.0 fat    15509 b- defN 24-Apr-25 09:17 bert4keras3/tokenizers.py
--rw-rw-rw-  2.0 fat    28534 b- defN 24-Apr-25 09:17 bert4keras3/transformers.py
--rw-rw-rw-  2.0 fat    11358 b- defN 24-Apr-25 09:24 bert4keras3-1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      219 b- defN 24-Apr-25 09:24 bert4keras3-1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 09:24 bert4keras3-1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-25 09:24 bert4keras3-1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1037 b- defN 24-Apr-25 09:24 bert4keras3-1.3.dist-info/RECORD
-13 files, 154873 bytes uncompressed, 42240 bytes compressed:  72.7%
+Zip file size: 43971 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      150 b- defN 24-Apr-26 06:20 bert4keras3/__init__.py
+-rw-rw-rw-  2.0 fat    23204 b- defN 24-Apr-26 06:20 bert4keras3/backend.py
+-rw-rw-rw-  2.0 fat    11442 b- defN 24-Apr-26 06:20 bert4keras3/layers.py
+-rw-rw-rw-  2.0 fat     5211 b- defN 24-Apr-26 06:20 bert4keras3/models.py
+-rw-rw-rw-  2.0 fat    30152 b- defN 24-Apr-26 06:20 bert4keras3/ops.py
+-rw-rw-rw-  2.0 fat    27955 b- defN 24-Apr-26 06:20 bert4keras3/snippets.py
+-rw-rw-rw-  2.0 fat    15509 b- defN 24-Apr-26 06:20 bert4keras3/tokenizers.py
+-rw-rw-rw-  2.0 fat    28599 b- defN 24-Apr-26 06:20 bert4keras3/transformers.py
+-rw-rw-rw-  2.0 fat    11358 b- defN 24-Apr-26 06:22 bert4keras3-1.3.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      188 b- defN 24-Apr-26 06:22 bert4keras3-1.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-26 06:22 bert4keras3-1.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-26 06:22 bert4keras3-1.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1047 b- defN 24-Apr-26 06:22 bert4keras3-1.3.1.dist-info/RECORD
+13 files, 154919 bytes uncompressed, 42243 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: bert4keras3/tokenizers.py
 Comment: 
 
 Filename: bert4keras3/transformers.py
 Comment: 
 
-Filename: bert4keras3-1.3.dist-info/LICENSE
+Filename: bert4keras3-1.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: bert4keras3-1.3.dist-info/METADATA
+Filename: bert4keras3-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: bert4keras3-1.3.dist-info/WHEEL
+Filename: bert4keras3-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: bert4keras3-1.3.dist-info/top_level.txt
+Filename: bert4keras3-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bert4keras3-1.3.dist-info/RECORD
+Filename: bert4keras3-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bert4keras3/__init__.py

```diff
@@ -1,6 +1,6 @@
 #! -*- coding: utf-8 -*-
 
-__version__ = '1.3'
+__version__ = '1.1.2'
 
 from bert4keras3 import backend,layers,models,snippets,tokenizers
 from bert4keras3.backend import ops
```

## bert4keras3/transformers.py

```diff
@@ -482,15 +482,15 @@
     def slice_inputs(self,inputs,key,index):
         return ops.expand_dims(ops.take(inputs[key],index,axis=1),1)
     def get_new_inputs(self,inputs,key,xs,index=None):
         return inputs[:key]+[xs]+inputs[key+1:]
     def cache_call(self,inputs:list,input_lengths:list,end_token,
                    search_mode='greedy',k=1,progress_print=True,index_bias=0):
         old_flag = self.custom_position_ids
-        
+        #print(keras.mixed_precision.dtype_policy())
         if self.is_seq2seq:
             caches = self.initial_cache([inputs[1],inputs[0]])
             key = 1
         else:
             caches = self.initial_cache(inputs[:1])
             key = 0
         x = inputs[key]
@@ -575,32 +575,34 @@
                                             attention_mask=attention_mask,
                                             position_bias=position_bias)
                 
                 z,cache = out[:-1],out[-1]
                 
                 caches[i*j:i*j+j]=cache
             
+
             o = self.apply_final_layers(z)
             index += 1
 
             search_in = [o,index,inputs[key],flags]
 
             inputs[key],flags = self.Search(search_in,k=k,mode=search_mode)
 
             return (inputs, caches, index , flags)
         num_hidden_layers = self.num_hidden_layers
         class WhileLayer(keras.Layer):
             def call(self, x):
                 inputs, caches, index =  x[:]
-
                 flags = ops.ones([ops.shape(caches[0])[0],1],dtype='bool')
+                
                 if backlib=='torch':
                     while cond(inputs, caches, index , flags):
                         inputs, caches, index , flags = body(inputs, caches, index , flags)
                     return (inputs, caches, index)
+                
                 outs=ops.while_loop(
                     cond,
                     body,
                     loop_vars=(inputs, caches, index , flags),
                     maximum_iterations=length-index                                                                                                                                                                                                                                                                                                                                                       ,
                 )
                 if progress_print:
@@ -608,16 +610,16 @@
                 return outs[:3]
             def compute_output_shape(self, input_shape):
                 return input_shape
 
         out=self.apply(
             inputs=(inputs, caches, index),
             layer=WhileLayer,
-            dtype='float32',
-            name='WhileLayer'
+            name='WhileLayer',
+            
         )
 
         self.custom_position_ids = old_flag
         return ops.cast(out[0][key],'int32')
     def build_cache_model(self,input_lengths:list,end_token,
                           search_mode='greedy',k=1,progress_print=False,index_bias=0):
```

## Comparing `bert4keras3-1.3.dist-info/LICENSE` & `bert4keras3-1.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bert4keras3-1.3.dist-info/RECORD` & `bert4keras3-1.3.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-bert4keras3/__init__.py,sha256=cQCKzarpKN-VHmivGnetot0AdqJIjBwTz5CWB38gagc,148
+bert4keras3/__init__.py,sha256=CMb8S8X82Zw-9GhxgUom0I8qs7veKePBxPqa7nStNpk,150
 bert4keras3/backend.py,sha256=1ywO73bYuMXA5CpAkRNcxpOExa7WCKrj9ryooJxCzP0,23204
 bert4keras3/layers.py,sha256=wSLeVRzTvWoonglKhQl8sQ2HbmlZBJis7KNTOiiPwf8,11442
 bert4keras3/models.py,sha256=o7DHSr3Dvj7IIa5oVBqyO92fIm2oLU-pPoo5YsSlNaU,5211
 bert4keras3/ops.py,sha256=H1sbMv6WOJ5iGAB0rosPz9LoqdT0jS8knLRW_6XkFRU,30152
 bert4keras3/snippets.py,sha256=YwdYRvrewhM6g8ax9_Ath0HsJATzuyZksL5Dow9l65A,27955
 bert4keras3/tokenizers.py,sha256=PCxtC4L9tF2w-GUDujdPK8Z5WlnbaL8mYhRfHn1S_Qg,15509
-bert4keras3/transformers.py,sha256=QC9926N2XJokR5oS9ZdDSaxZwwA15MVdpLrPxcUArxk,28534
-bert4keras3-1.3.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-bert4keras3-1.3.dist-info/METADATA,sha256=5p3NMnrqU568-TO88A-cBR5kwse9zeq_dGkqIplgTcU,219
-bert4keras3-1.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-bert4keras3-1.3.dist-info/top_level.txt,sha256=cPWwwxSejEMpgAZFzYQc0WmhPrF3XwP3k1IwRO93gwQ,12
-bert4keras3-1.3.dist-info/RECORD,,
+bert4keras3/transformers.py,sha256=7nlSIl_NnHl-7hhVWHn9SsveYHOOtJSVNBrkpIRRdl4,28599
+bert4keras3-1.3.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+bert4keras3-1.3.1.dist-info/METADATA,sha256=V32Ldi5vzDLLmMf7ofkDPDo6XGEACz13-4I7hUs1G0I,188
+bert4keras3-1.3.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+bert4keras3-1.3.1.dist-info/top_level.txt,sha256=cPWwwxSejEMpgAZFzYQc0WmhPrF3XwP3k1IwRO93gwQ,12
+bert4keras3-1.3.1.dist-info/RECORD,,
```

