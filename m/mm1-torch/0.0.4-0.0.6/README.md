# Comparing `tmp/mm1_torch-0.0.4.tar.gz` & `tmp/mm1_torch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mm1_torch-0.0.4.tar", max compression
+gzip compressed data, was "mm1_torch-0.0.6.tar", max compression
```

## Comparing `mm1_torch-0.0.4.tar` & `mm1_torch-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1074 2024-03-19 02:52:37.351297 mm1_torch-0.0.4/LICENSE
--rw-r--r--   0        0        0      991 2024-03-20 05:32:00.741887 mm1_torch-0.0.4/README.md
--rw-r--r--   0        0        0      245 2024-03-21 15:42:11.116066 mm1_torch-0.0.4/mm1_torch/__init__.py
--rw-r--r--   0        0        0    16307 2024-03-21 15:46:05.321811 mm1_torch-0.0.4/mm1_torch/main.py
--rw-r--r--   0        0        0     3004 2024-03-21 15:41:50.623525 mm1_torch-0.0.4/mm1_torch/moe.py
--rw-r--r--   0        0        0     1525 2024-03-20 05:05:09.187413 mm1_torch-0.0.4/mm1_torch/resblock_text.py
--rw-r--r--   0        0        0     1324 2024-03-21 15:46:20.648520 mm1_torch-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 mm1_torch-0.0.4/setup.py
--rw-r--r--   0        0        0     2109 1970-01-01 00:00:00.000000 mm1_torch-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-03-19 02:52:37.351297 mm1_torch-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1816 2024-03-23 16:37:08.726457 mm1_torch-0.0.6/README.md
+-rw-r--r--   0        0        0      194 2024-04-26 16:13:40.498053 mm1_torch-0.0.6/mm1_torch/__init__.py
+-rw-r--r--   0        0        0    14072 2024-04-26 16:13:41.012659 mm1_torch-0.0.6/mm1_torch/main.py
+-rw-r--r--   0        0        0     1525 2024-03-20 05:05:09.187413 mm1_torch-0.0.6/mm1_torch/resblock_text.py
+-rw-r--r--   0        0        0     1325 2024-04-26 16:16:36.351585 mm1_torch-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 mm1_torch-0.0.6/setup.py
+-rw-r--r--   0        0        0     2735 1970-01-01 00:00:00.000000 mm1_torch-0.0.6/PKG-INFO
```

### Comparing `mm1_torch-0.0.4/LICENSE` & `mm1_torch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mm1_torch-0.0.4/mm1_torch/main.py` & `mm1_torch-0.0.6/mm1_torch/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,91 +1,15 @@
 import torch
 from torch import Tensor, nn
 from zeta.nn import FeedForward, OutputHead, threed_to_text
 from zeta.nn.attention import Attention
 from zeta.structs import Encoder, ViTransformerWrapper
 
-from mm1_torch.moe import MoELayer
 from mm1_torch.resblock_text import TextResBlock1d
-
-# from torchscale.component.xmoe.moe_layer import MOELayer
-# from torchscale.component.xmoe.routing import Top2Gate
-# from torchscale.component.feedforward_network import make_experts
-# from torch import dist
-# from typing import Optional
-
-
-
-# def create_moe_layer(
-#     embed_dim: int = 512,
-#     moe_expert_count: int = 4,
-#     moe_gating_use_fp32: bool = True,
-#     moe_second_expert_policy: str = "all",
-#     moe_normalize_gate_prob_before_dropping: bool = True,
-#     moe_eval_capacity_token_fraction: float = 0.5,
-#     use_xmoe: bool = True,
-#     moe_capacity_factor: int = 2,
-#     moe_top2gating: bool = True,
-#     moe_expert_group: Optional[dist.ProcessGroup] = None,
-#     moe_all2all_group: Optional[dist.ProcessGroup] = None,
-#     moe_world_size: int = 3,
-#     moe_all2all_size: int = 1,
-#     *args,
-# ) -> str:
-#     gate = Top2Gate(
-#         embed_dim,
-#         moe_expert_count,
-#         moe_gating_use_fp32,
-#         moe_second_expert_policy,
-#         moe_normalize_gate_prob_before_dropping,
-#         moe_eval_capacity_token_fraction,
-#         use_xmoe=use_xmoe,
-#     )
-#     args = {
-#         "moe_expert_count": moe_expert_count,
-#         "moe_capacity_factor": moe_capacity_factor,
-#         "moe_top2gating": moe_top2gating,
-#         "moe_expert_group": moe_expert_group,
-#         "moe_all2all_group": moe_all2all_group,
-#         "moe_world_size": moe_world_size,
-#         "moe_all2all_size": moe_all2all_size,
-#         "args": args,
-#     }
-
-#     experts = make_experts(
-#         embed_dim=embed_dim, expert_ffn_dim=embed_dim
-#     )
-#     moe_layer = MOELayer(gate, experts, *args)
-#     return moe_layer
-
-
-# x = torch.randn(1, 100, 512)
-
-# # Create a model
-# model = create_moe_layer(
-#     embed_dim=512,
-#     moe_expert_count=4,
-#     moe_gating_use_fp32=True,
-#     moe_second_expert_policy="all",
-#     moe_normalize_gate_prob_before_dropping=True,
-#     moe_eval_capacity_token_fraction=0.5,
-#     use_xmoe=True,
-#     moe_capacity_factor=2,
-#     moe_top2gating=True,
-#     moe_expert_group=None,
-#     moe_all2all_group=None,
-#     moe_world_size=1,
-#     moe_all2all_size=1,
-# )
-
-# # Forward
-# out = model(x)
-
-# print(out.shape)
-# print(out)
+from zeta.nn.modules import NormalSparseMoE
 
 
 # constants
 def exists(x):
     return x is not None
 
 
@@ -96,54 +20,45 @@
 
 
 def identity(t, *args, **kwargs):
     return t
 
 
 # small helper modules
-
-
-def posemb_sincos_2d(
-    h: int,
-    w: int,
-    dim: int,
-    temperature: int = 10000,
-    dtype=torch.float32,
-):
+def posemb_sincos_1d(patches, temperature=10000, dtype=torch.float32):
     """
-    Generates positional embeddings using sine and cosine functions for a 2D grid.
+    Compute positional embeddings using sine and cosine functions for 1D patches.
 
     Args:
-        h (int): Height of the grid.
-        w (int): Width of the grid.
-        dim (int): Feature dimension. Must be a multiple of 4 for sincos embedding.
-        temperature (int, optional): Temperature parameter for the embedding. Defaults to 10000.
-        dtype (torch.dtype, optional): Data type of the output tensor. Defaults to torch.float32.
+        patches (torch.Tensor): Input patches of shape (batch_size, n, dim).
+        temperature (float, optional): Temperature parameter for the positional embeddings. Default is 10000.
+        dtype (torch.dtype, optional): Data type of the output tensor. Default is torch.float32.
 
     Returns:
-        torch.Tensor: Positional embeddings of shape (h * w, dim).
+        torch.Tensor: Positional embeddings of shape (batch_size, n, dim).
 
     Raises:
-        AssertionError: If the feature dimension is not a multiple of 4.
+        AssertionError: If the feature dimension is not a multiple of 2.
 
-    Example:
-        pe = posemb_sincos_2d(10, 10, 32)
     """
-    y, x = torch.meshgrid(
-        torch.arange(h), torch.arange(w), indexing="ij"
+    _, n, dim, device, dtype = (
+        *patches.shape,
+        patches.device,
+        patches.dtype,
     )
+
+    n = torch.arange(n, device=device)
     assert (
-        dim % 4
-    ) == 0, "feature dimension must be multiple of 4 for sincos emb"
-    omega = torch.arange(dim // 4) / (dim // 4 - 1)
+        dim % 2
+    ) == 0, "feature dimension must be multiple of 2 for sincos emb"
+    omega = torch.arange(dim // 2, device=device) / (dim // 2 - 1)
     omega = 1.0 / (temperature**omega)
 
-    y = y.flatten()[:, None] * omega[None, :]
-    x = x.flatten()[:, None] * omega[None, :]
-    pe = torch.cat((x.sin(), x.cos(), y.sin(), y.cos()), dim=1)
+    n = n.flatten()[:, None] * omega[None, :]
+    pe = torch.cat((n.sin(), n.cos()), dim=1)
     return pe.type(dtype)
 
 
 # D Abstractor
 class DAbstractor(nn.Module):
     """
     DAbstractor is a module that performs abstract reasoning on input data.
@@ -187,19 +102,15 @@
         self.dim = dim
         self.depth = depth
         self.heads = heads
         self.dropout = dropout
         self.dim_head = dim_head
         self.seq_len = seq_len
 
-        # Positional Embedding
-        # TODO: Implement
-
         # Attention
-        # self.attn = MultiQueryAttention(dim, heads, *args, **kwargs)
         self.attn = Attention(
             dim=dim,
             dim_head=dim_head,
             heads=heads,
             causal=True,
             qk_norm=True,
         )
@@ -221,14 +132,19 @@
             Tensor: The output of the DAbstractor module.
 
         """
         # b, c, h, w = x.shape
         b, s, d = x.shape
 
         # Positional Embedding
+        position_tokens = posemb_sincos_1d(x)
+        print(f"Positional Tokens: {position_tokens.shape}")
+
+        # Add positional embeddings
+        x += position_tokens
 
         # Adaptive pool
         x = nn.AdaptiveAvgPool1d(d)(x)
 
         # Attention
         x = self.attn(x)
 
@@ -360,15 +276,15 @@
                 for _ in range(self.depth)
             ]
         )
 
         # Expert layers
         self.expert_layers = nn.ModuleList(
             [
-                MoELayer(dim, num_experts, num_experts_per_tok)
+                NormalSparseMoE(dim, num_experts, hidden_dim=dim)
                 for _ in range(self.depth)
             ]
         )
 
         # Expert layers
         self.ffn_layers = nn.ModuleList(
             [
@@ -385,22 +301,26 @@
             x (Tensor): The input tensor.
 
         Returns:
             Tensor: The output tensor.
 
         """
         if self.use_feedforward:
-            for attn_layer, ffn in zip(self.attn_layers, self.ffn_layers):
+            for attn_layer, ffn in zip(
+                self.attn_layers, self.ffn_layers
+            ):
                 attn, _ = attn_layer(x)
                 attn = attn + x
                 expert = ffn(attn)
                 x = attn + expert
-                
-        else: 
-            for attn_layer, expert_layer in zip(self.attn_layers, self.expert_layers):
+
+        else:
+            for attn_layer, expert_layer in zip(
+                self.attn_layers, self.expert_layers
+            ):
                 attn, _ = attn_layer(x)
                 attn = attn + x
                 expert = expert_layer(attn)
                 x = attn + expert
 
         return x
 
@@ -549,12 +469,13 @@
             self.heads,
         )(image)
         print(f"Image Connector: {image.shape}")
 
         # Decoder
         x = self.decoder(x + image)
 
+        # Return logits
         if self.return_logits:
             return OutputHead(self.dim, -1)(x)
 
         else:
             return x
```

### Comparing `mm1_torch-0.0.4/mm1_torch/resblock_text.py` & `mm1_torch-0.0.6/mm1_torch/resblock_text.py`

 * *Files identical despite different names*

### Comparing `mm1_torch-0.0.4/pyproject.toml` & `mm1_torch-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mm1-torch"
-version = "0.0.4"
+version = "0.0.6"
 description = "MM1 - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/mm1"
 documentation = "https://github.com/kyegomez/mm1"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/mm1"
@@ -18,15 +18,15 @@
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.10"
 zetascale = "*"
 torch = "*"
 einops = "*"
 
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.6"
```

### Comparing `mm1_torch-0.0.4/PKG-INFO` & `mm1_torch-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: mm1-torch
-Version: 0.0.4
+Version: 0.0.6
 Summary: MM1 - Pytorch
 Home-page: https://github.com/kyegomez/mm1
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: einops
 Requires-Dist: torch
 Requires-Dist: zetascale
@@ -35,41 +31,41 @@
 `img -> encoder -> connector -> llm -> tokens` 
 
 ## install
 `pip3 install mm1-torch`
 
 ## usage
 ```python
-
 import torch
 from mm1_torch.main import MM1
 
 # Tensors
-x = torch.randint(0, 100, (1, 512))
-img = torch.randn(1, 3, 224, 224)
+x = torch.randint(0, 100, (1, 512))  # Create a random tensor of shape (1, 512)
+img = torch.randn(1, 3, 224, 224)  # Create a random image tensor of shape (1, 3, 224, 224)
 
 # Create a model
 model = MM1(
-    dim=512,
-    depth=12,
-    heads=8,
-    dim_head=64,
-    dropout=0.1,
-    num_experts=4,
-    num_experts_per_tok=2,
-    encoder_dim=512,
-    encoder_depth=12,
-    encoder_heads=8,
+    dim=512,  # Dimension of the input tensor
+    depth=12,  # Number of transformer layers
+    heads=8,  # Number of attention heads
+    dim_head=64,  # Dimension of each attention head
+    dropout=0.1,  # Dropout rate
+    num_experts=4,  # Number of experts in mixture-of-experts
+    num_experts_per_tok=2,  # Number of experts per token in mixture-of-experts
+    encoder_dim=512,  # Dimension of the encoder output
+    encoder_depth=12,  # Number of encoder transformer layers
+    encoder_heads=8,  # Number of encoder attention heads
+    use_moe=True,  # Whether to use mixture-of-experts
+    return_logits=True  # Whether to return logits or probabilities
 )
 
-
 # Forward
-out = model(x, img)
-print(out.shape)  # torch.Size([2, 3, 512])
-print(out)
+out = model(x, img)  # Forward pass through the model
+print(out.shape)  # Print the shape of the output tensor (torch.Size([2, 3, 512]))
+print(out)  # Print the output tensor
 ```
 
 ### `CAbstractor`
 
 ```python
 import torch
 from mm1_torch.main import CAbstractor
@@ -91,7 +87,13 @@
 
 ```
 
 
 # License
 MIT
 
+
+## Todo
+
+- [x] Implement the deformable attention
+- [ ] Create a training script for Huggingface datasets
+- [ ] Create unit tests for every module
```

