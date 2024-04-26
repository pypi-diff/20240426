# Comparing `tmp/mlx_llm-1.0.1.tar.gz` & `tmp/mlx_llm-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_llm-1.0.1.tar", max compression
+gzip compressed data, was "mlx_llm-1.0.2.tar", max compression
```

## Comparing `mlx_llm-1.0.1.tar` & `mlx_llm-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     7020 2023-12-17 18:14:37.703503 mlx_llm-1.0.1/LICENSE
--rw-r--r--   0        0        0     4056 2024-04-26 07:52:59.042856 mlx_llm-1.0.1/README.md
--rw-r--r--   0        0        0     2346 2024-04-26 08:09:30.621084 mlx_llm-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-26 05:49:26.960495 mlx_llm-1.0.1/src/mlx_llm/__init__.py
--rw-r--r--   0        0        0       37 2024-04-25 18:15:52.521874 mlx_llm-1.0.1/src/mlx_llm/chat/__init__.py
--rw-r--r--   0        0        0     4271 2024-04-26 06:02:18.067844 mlx_llm-1.0.1/src/mlx_llm/chat/chat.py
--rw-r--r--   0        0        0      449 2024-04-25 16:44:44.347072 mlx_llm-1.0.1/src/mlx_llm/chat/utils.py
--rw-r--r--   0        0        0      132 2024-04-26 06:35:03.158299 mlx_llm-1.0.1/src/mlx_llm/model/__init__.py
--rw-r--r--   0        0        0      406 2024-04-26 07:13:29.372845 mlx_llm-1.0.1/src/mlx_llm/model/_config.py
--rw-r--r--   0        0        0     4566 2024-04-26 07:43:39.552282 mlx_llm-1.0.1/src/mlx_llm/model/_factory.py
--rw-r--r--   0        0        0    10710 2024-04-26 07:42:22.483139 mlx_llm-1.0.1/src/mlx_llm/model/_registry.py
--rw-r--r--   0        0        0     5552 2024-04-26 07:30:03.065063 mlx_llm-1.0.1/src/mlx_llm/model/_utils.py
--rw-r--r--   0        0        0     5934 2024-04-26 07:42:22.482723 mlx_llm-1.0.1/src/mlx_llm/model/converter.py
--rw-r--r--   0        0        0    11300 2024-04-26 06:49:40.965965 mlx_llm-1.0.1/src/mlx_llm/model/transformer.py
--rw-r--r--   0        0        0     1065 2024-04-26 05:55:40.693044 mlx_llm-1.0.1/src/mlx_llm/prompt/__init__.py
--rw-r--r--   0        0        0      287 2024-04-26 05:52:41.210662 mlx_llm-1.0.1/src/mlx_llm/prompt/_base.py
--rw-r--r--   0        0        0     4333 2024-04-26 05:55:40.705143 mlx_llm-1.0.1/src/mlx_llm/prompt/llama.py
--rw-r--r--   0        0        0     1689 2024-04-26 05:52:48.319890 mlx_llm-1.0.1/src/mlx_llm/prompt/mistral.py
--rw-r--r--   0        0        0      559 2024-04-25 17:27:39.446911 mlx_llm-1.0.1/src/mlx_llm/prompt/phi.py
--rw-r--r--   0        0        0        1 2024-04-24 20:26:31.246541 mlx_llm-1.0.1/src/mlx_llm/utils/__init__.py
--rw-r--r--   0        0        0     1235 2024-04-25 16:19:53.103298 mlx_llm-1.0.1/src/mlx_llm/utils/hf.py
--rw-r--r--   0        0        0     4810 2024-04-26 05:53:10.327572 mlx_llm-1.0.1/src/mlx_llm/utils/session.py
--rw-r--r--   0        0        0     1261 2024-02-09 16:22:28.193671 mlx_llm-1.0.1/src/mlx_llm/utils/time.py
--rw-r--r--   0        0        0     2129 2024-04-26 07:30:21.993340 mlx_llm-1.0.1/src/mlx_llm/utils/weights.py
--rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 mlx_llm-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7020 2023-12-17 18:14:37.703503 mlx_llm-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4056 2024-04-26 13:24:58.253104 mlx_llm-1.0.2/README.md
+-rw-r--r--   0        0        0     2346 2024-04-26 14:51:52.316959 mlx_llm-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-26 14:51:50.795408 mlx_llm-1.0.2/src/mlx_llm/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-26 13:24:58.257004 mlx_llm-1.0.2/src/mlx_llm/chat/__init__.py
+-rw-r--r--   0        0        0     4271 2024-04-26 13:24:58.257405 mlx_llm-1.0.2/src/mlx_llm/chat/chat.py
+-rw-r--r--   0        0        0      449 2024-04-26 13:24:58.258114 mlx_llm-1.0.2/src/mlx_llm/chat/utils.py
+-rw-r--r--   0        0        0      132 2024-04-26 13:24:58.258969 mlx_llm-1.0.2/src/mlx_llm/model/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-26 13:24:58.259541 mlx_llm-1.0.2/src/mlx_llm/model/_config.py
+-rw-r--r--   0        0        0     4566 2024-04-26 14:47:26.867923 mlx_llm-1.0.2/src/mlx_llm/model/_factory.py
+-rw-r--r--   0        0        0    12747 2024-04-26 14:50:42.817403 mlx_llm-1.0.2/src/mlx_llm/model/_registry.py
+-rw-r--r--   0        0        0     5552 2024-04-26 14:45:13.721964 mlx_llm-1.0.2/src/mlx_llm/model/_utils.py
+-rw-r--r--   0        0        0     5935 2024-04-26 14:32:00.243551 mlx_llm-1.0.2/src/mlx_llm/model/converter.py
+-rw-r--r--   0        0        0    12171 2024-04-26 14:32:00.299721 mlx_llm-1.0.2/src/mlx_llm/model/transformer.py
+-rw-r--r--   0        0        0     1122 2024-04-26 13:48:34.485319 mlx_llm-1.0.2/src/mlx_llm/prompt/__init__.py
+-rw-r--r--   0        0        0      287 2024-04-26 13:24:58.264679 mlx_llm-1.0.2/src/mlx_llm/prompt/_base.py
+-rw-r--r--   0        0        0     1691 2024-04-26 14:32:00.238359 mlx_llm-1.0.2/src/mlx_llm/prompt/gemma.py
+-rw-r--r--   0        0        0     4333 2024-04-26 13:24:58.265041 mlx_llm-1.0.2/src/mlx_llm/prompt/llama.py
+-rw-r--r--   0        0        0     1689 2024-04-26 13:24:58.265937 mlx_llm-1.0.2/src/mlx_llm/prompt/mistral.py
+-rw-r--r--   0        0        0      559 2024-04-26 13:24:58.266273 mlx_llm-1.0.2/src/mlx_llm/prompt/phi.py
+-rw-r--r--   0        0        0        1 2024-04-26 13:24:58.267232 mlx_llm-1.0.2/src/mlx_llm/utils/__init__.py
+-rw-r--r--   0        0        0     1235 2024-04-26 13:24:58.267997 mlx_llm-1.0.2/src/mlx_llm/utils/hf.py
+-rw-r--r--   0        0        0     4810 2024-04-26 13:24:58.268439 mlx_llm-1.0.2/src/mlx_llm/utils/session.py
+-rw-r--r--   0        0        0     1261 2024-02-09 16:22:28.193671 mlx_llm-1.0.2/src/mlx_llm/utils/time.py
+-rw-r--r--   0        0        0     2129 2024-04-26 13:24:58.269430 mlx_llm-1.0.2/src/mlx_llm/utils/weights.py
+-rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 mlx_llm-1.0.2/PKG-INFO
```

### Comparing `mlx_llm-1.0.1/LICENSE` & `mlx_llm-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/README.md` & `mlx_llm-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/pyproject.toml` & `mlx_llm-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlx_llm"
-version = "1.0.1"
+version = "1.0.2"
 description = "Large Language Models (LLMs) applications and tools running on Apple Silicon in real-time with Apple MLX"
 authors = ["Riccardo Musmeci <riccardomusmeci92@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "mlx_llm", from = "src" },
 ]
```

### Comparing `mlx_llm-1.0.1/src/mlx_llm/chat/chat.py` & `mlx_llm-1.0.2/src/mlx_llm/chat/chat.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/src/mlx_llm/model/_factory.py` & `mlx_llm-1.0.2/src/mlx_llm/model/_factory.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/src/mlx_llm/model/_registry.py` & `mlx_llm-1.0.2/src/mlx_llm/model/_registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from ._config import HFConfig, ModelConfig, QuantizeConfig
 from .converter import llama_to_mlxllm, mistral_to_mlxllm, phi3_to_mlxllm
 from .transformer import Transformer
 
 MODEL_ENTRYPOINTS = {}
 
+
 def register_model(name: Optional[str] = None) -> Callable:
     """Register a model entrypoint.
 
     Args:
         name (Optional[str], optional): mlx_llm model name. If None, is the same as the fn name. Defaults to None.
 
     Returns:
@@ -24,18 +25,15 @@
         return fn
 
     return wrapper
 
 
 @register_model("llama_2_7b_chat_hf")
 def llama_2_7b_chat(
-    vocab_size: int = 32000,
-    norm_eps: float = 1e-5,
-    rope_theta: float = 10000.0,
-    rope_traditional: bool = False
+    vocab_size: int = 32000, norm_eps: float = 1e-5, rope_theta: float = 10000.0, rope_traditional: bool = False
 ) -> Tuple[Transformer, ModelConfig]:
     """Create a LLaMA 2 7B chat model.
 
     Args:
         vocab_size (int, optional): vocab size. Defaults to 32000.
         norm_eps (float, optional): norm epsilon. Defaults to 1e-5.
         rope_theta (float, optional): rope theta. Defaults to 10000.0.
@@ -63,18 +61,15 @@
         converter=llama_to_mlxllm,
     )
     return model, config
 
 
 @register_model("llama_2_7b_hf")
 def llama_2_7b(
-    vocab_size: int = 32000,
-    norm_eps: float = 1e-5,
-    rope_theta: float = 10000.0,
-    rope_traditional: bool = False
+    vocab_size: int = 32000, norm_eps: float = 1e-5, rope_theta: float = 10000.0, rope_traditional: bool = False
 ) -> Tuple[Transformer, ModelConfig]:
     """Create a LLaMA 2 7B chat model.
 
     Args:
         vocab_size (int, optional): vocab size. Defaults to 32000.
         norm_eps (float, optional): norm epsilon. Defaults to 1e-5.
         rope_theta (float, optional): rope theta. Defaults to 10000.0.
@@ -102,18 +97,15 @@
         converter=llama_to_mlxllm,
     )
     return model, config
 
 
 @register_model("llama_3_8b")
 def llama_3_8b(
-    vocab_size: int = 128256,
-    norm_eps: float = 1e-5,
-    rope_theta: float = 500000.0,
-    rope_traditional: bool = False
+    vocab_size: int = 128256, norm_eps: float = 1e-5, rope_theta: float = 500000.0, rope_traditional: bool = False
 ) -> Tuple[Transformer, ModelConfig]:
     """Create a LLaMA 3 8B model.
 
     Args:
         vocab_size (int, optional): vocab size. Defaults to 128256.
         norm_eps (float, optional): norm epsilon. Defaults to 1e-5.
         rope_theta (float, optional): rope theta. Defaults to 500000.0.
@@ -141,18 +133,15 @@
         converter=llama_to_mlxllm,
     )
     return model, config
 
 
 @register_model("llama_3_8b_instruct")
 def llama_3_8b_instruct(
-    vocab_size: int = 128256,
-    norm_eps: float = 1e-5,
-    rope_theta: float = 500000.0,
-    rope_traditional: bool = False
+    vocab_size: int = 128256, norm_eps: float = 1e-5, rope_theta: float = 500000.0, rope_traditional: bool = False
 ) -> Tuple[Transformer, ModelConfig]:
     """Create a LLaMA 3 8B Instruct model.
 
     Args:
         vocab_size (int, optional): vocab size. Defaults to 128256.
         norm_eps (float, optional): norm epsilon. Defaults to 1e-5.
         rope_theta (int, optional): rope theta. Defaults to 500000.0.
@@ -181,18 +170,15 @@
         converter=llama_to_mlxllm,
     )
     return model, config
 
 
 @register_model("phi_3_mini_4k_instruct")
 def phi3_mini_4k_instruct(
-    vocab_size: int = 32064,
-    norm_eps: float = 1e-5,
-    rope_theta: float = 10000.0,
-    rope_traditional: bool = False
+    vocab_size: int = 32064, norm_eps: float = 1e-5, rope_theta: float = 10000.0, rope_traditional: bool = False
 ) -> Tuple[Transformer, ModelConfig]:
     """Create a Phi3 Mini 4k Instruct model.
 
     Args:
         vocab_size (int, optional): vocab size. Defaults to 32064.
         norm_eps (float, optional): norm epsilon. Defaults to 1e-5.
         rope_theta (float, optional): rope theta. Defaults to 10000.0.
@@ -220,18 +206,15 @@
         converter=phi3_to_mlxllm,
     )
     return model, config
 
 
 @register_model("phi_3_mini_128k_instruct")
 def phi3_mini_128k_instruct(
-    vocab_size: int = 32064,
-    norm_eps: float = 1e-5,
-    rope_theta: float = 10000.0,
-    rope_traditional: bool = False
+    vocab_size: int = 32064, norm_eps: float = 1e-5, rope_theta: float = 10000.0, rope_traditional: bool = False
 ) -> Tuple[Transformer, ModelConfig]:
     """Create a Phi3 Mini 128k Instruct model.
 
     Args:
         vocab_size (int, optional): vocab size. Defaults to 32064.
         norm_eps (float, optional): norm epsilon. Defaults to 1e-5.
         rope_theta (float, optional): rope theta. Defaults to 10000.0.
@@ -259,18 +242,15 @@
         converter=phi3_to_mlxllm,
     )
     return model, config
 
 
 @register_model("mistral_7b_instruct_v0.2")
 def mistral_7b_instruct_v02(
-    vocab_size: int = 32064,
-    norm_eps: float = 1e-5,
-    rope_theta: float = 10000.0,
-    rope_traditional: bool = False
+    vocab_size: int = 32064, norm_eps: float = 1e-5, rope_theta: float = 10000.0, rope_traditional: bool = False
 ) -> Tuple[Transformer, ModelConfig]:
     """Create a Mistral Instruct v0.2 Instruct model.
 
     Args:
         vocab_size (int, optional): vocab size. Defaults to 32000.
         norm_eps (float, optional): norm epsilon. Defaults to 1e-5.
         rope_theta (float, optional): rope theta. Defaults to 10000.0.
@@ -294,18 +274,15 @@
     config = ModelConfig(hf=HFConfig(repo_id="mistralai/Mistral-7B-Instruct-v0.2"), converter=mistral_to_mlxllm)
 
     return model, config
 
 
 @register_model("openhermes_2.5_mistral_7b")
 def openhermes_25_mistral_7b(
-    vocab_size: int = 32064,
-    norm_eps: float = 1e-5,
-    rope_theta: float = 10000.0,
-    rope_traditional: bool = False
+    vocab_size: int = 32064, norm_eps: float = 1e-5, rope_theta: float = 10000.0, rope_traditional: bool = False
 ) -> Tuple[Transformer, ModelConfig]:
     """Create a OpenHermes 2.5 Mistral 7B model.
 
     Args:
         vocab_size (int, optional): vocab size. Defaults to 32000.
         norm_eps (float, optional): norm epsilon. Defaults to 1e-5.
         rope_theta (float, optional): rope theta. Defaults to 10000.0.
@@ -329,18 +306,15 @@
     config = ModelConfig(hf=HFConfig(repo_id="teknium/OpenHermes-2.5-Mistral-7B"), converter=mistral_to_mlxllm)
 
     return model, config
 
 
 @register_model("tiny_llama_1.1B_chat_v1.0")
 def tiny_llama_11B_chat_v10(
-    vocab_size: int = 32000,
-    norm_eps: float = 1e-5,
-    rope_theta: float = 10000.0,
-    rope_traditional: bool = False
+    vocab_size: int = 32000, norm_eps: float = 1e-5, rope_theta: float = 10000.0, rope_traditional: bool = False
 ) -> Tuple[Transformer, ModelConfig]:
     """Create a Tiny Llama 1.1B Chat v1.0 model.
 
     Args:
         vocab_size (int, optional): vocab size. Defaults to 32000.
         norm_eps (float, optional): norm epsilon. Defaults to 1e-5.
         rope_theta (float, optional): rope theta. Defaults to 10000.0.
@@ -360,7 +334,75 @@
         rope_theta=rope_theta,
         rope_traditional=rope_traditional,
     )
 
     config = ModelConfig(hf=HFConfig(repo_id="TinyLlama/TinyLlama-1.1B-Chat-v1.0"), converter=llama_to_mlxllm)
 
     return model, config
+
+
+@register_model("gemma_1.1_2b_it")
+def gemma_2b_it(
+    vocab_size: int = 256000, norm_eps: float = 1e-6, rope_theta: float = 10000.0, rope_traditional: bool = False
+) -> Tuple[Transformer, ModelConfig]:
+    """Create a Gemma 2B (v1.1) model
+
+    Args:
+        vocab_size (int, optional): vocab size. Defaults to 256000.
+        norm_eps (float, optional): norm epsilon. Defaults to 1e-6.
+        rope_theta (float, optional): rope theta. Defaults to 10000.0.
+        rope_traditional (bool, optional): whether to use traditional rope. Defaults to False.
+
+    Returns:
+        Tuple[Transformer, ModelConfig]: model, config
+    """
+    model = Transformer(
+        dim=2048,
+        hidden_dim=16384,
+        vocab_size=vocab_size,
+        n_layers=18,
+        n_heads=8,
+        n_kv_heads=1,
+        head_dim=256,
+        norm_eps=norm_eps,
+        rope_theta=rope_theta,
+        rope_traditional=rope_traditional,
+        gemma=True,
+    )
+
+    config = ModelConfig(hf=HFConfig(repo_id="google/gemma-1.1-2b-it"), converter=llama_to_mlxllm)
+
+    return model, config
+
+
+@register_model("gemma_1.1_7b_it")
+def gemma_7b_it(
+    vocab_size: int = 256000, norm_eps: float = 1e-6, rope_theta: float = 10000.0, rope_traditional: bool = False
+) -> Tuple[Transformer, ModelConfig]:
+    """Create a Gemma /B (v1.1) model
+
+    Args:
+        vocab_size (int, optional): vocab size. Defaults to 256000.
+        norm_eps (float, optional): norm epsilon. Defaults to 1e-6.
+        rope_theta (float, optional): rope theta. Defaults to 10000.0.
+        rope_traditional (bool, optional): whether to use traditional rope. Defaults to False.
+
+    Returns:
+        Tuple[Transformer, ModelConfig]: model, config
+    """
+    model = Transformer(
+        dim=3072,
+        hidden_dim=24576,
+        vocab_size=vocab_size,
+        n_layers=28,
+        n_heads=16,
+        n_kv_heads=16,
+        head_dim=256,
+        norm_eps=norm_eps,
+        rope_theta=rope_theta,
+        rope_traditional=rope_traditional,
+        gemma=True,
+    )
+
+    config = ModelConfig(hf=HFConfig(repo_id="google/gemma-1.1-7b-it"), converter=llama_to_mlxllm)
+
+    return model, config
```

### Comparing `mlx_llm-1.0.1/src/mlx_llm/model/_utils.py` & `mlx_llm-1.0.2/src/mlx_llm/model/_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/src/mlx_llm/model/converter.py` & `mlx_llm-1.0.2/src/mlx_llm/model/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
                 model_weights[model_k] = w
         else:
             key_map = {"embed_tokens": "token_embed", "lm_head": "head", "norm": "norm"}
             model_k = f"{key_map[k_split[0]]}.{k_split[1]}"
             model_weights[model_k] = w
     return model_weights
 
+
 def phi3_to_mlxllm(weights_paths: List[str], verbose: bool = False) -> Dict[str, mx.array]:
     """Convert original Phi3 weights to MLX format.
 
     Args:
         weights_paths (List[str]): list of paths to original Phi3 weights
         verbose (bool, optional): whether to print information during conversion. Defaults to False.
```

### Comparing `mlx_llm-1.0.1/src/mlx_llm/model/transformer.py` & `mlx_llm-1.0.2/src/mlx_llm/model/transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 from typing import Dict, List, Optional, Tuple, Union
 
 import mlx.core as mx
 import mlx.nn as nn
 
 
+class RMSNorm(nn.Module):
+    def __init__(self, dims: int, eps: float = 1e-5):
+        super().__init__()
+        self.weight = mx.ones((dims,))
+        self.eps = eps
+
+    def __call__(self, x):
+        return mx.fast.rms_norm(x, 1.0 + self.weight, self.eps)
+
+
 class Attention(nn.Module):
     """Attention module
 
     Args:
         dim (int): model dimension
         n_heads (int): number of attention heads
         n_kv_heads (int): number of key-value heads
@@ -92,33 +102,38 @@
 
 class MLP(nn.Module):
     """MLP module
 
     Args:
         dim (int): model dimension
         hidden_dim (int): hidden dimension
+        gemma (bool, optional): use Gemma activation. Defaults to False.
     """
 
-    def __init__(self, dim: int, hidden_dim: int):
+    def __init__(self, dim: int, hidden_dim: int, gemma: bool = False):
         super().__init__()
 
         self.gate_proj = nn.Linear(dim, hidden_dim, bias=False)
         self.down_proj = nn.Linear(hidden_dim, dim, bias=False)
         self.up_proj = nn.Linear(dim, hidden_dim, bias=False)
+        self.gemma = gemma
 
     def __call__(self, x: mx.array) -> mx.array:
         """Forward pass
 
         Args:
             x (mx.array): input
 
         Returns:
             mx.array: output
         """
-        return self.down_proj(nn.silu(self.gate_proj(x)) * self.up_proj(x))
+        if self.gemma:
+            return self.down_proj(nn.gelu(self.gate_proj(x)) * self.up_proj(x))
+        else:
+            return self.down_proj(nn.silu(self.gate_proj(x)) * self.up_proj(x))
 
 
 class TransformerBlock(nn.Module):
     """Transformer block
 
     Args:
         dim (int): model dimension
@@ -126,45 +141,50 @@
         n_kv_heads (int): number of key-value heads
         hidden_dim (int): hidden dimension
         norm_eps (float): normalization epsilon
         head_dim (Optional[int], optional): head dimension. Defaults to None.
         rope_traditional (bool, optional): whether to use traditional RoPE. Defaults to False.
         rope_theta (float, optional): RoPE theta. Defaults to 1000.
         rope_scaling (Optional[Dict[str, Union[float, str]]], optional): RoPE scaling. Defaults to None.
+        gemma (bool, optional): whether using Gemma layers. Defaults to False.
     """
 
     def __init__(
         self,
         dim: int,
         n_heads: int,
         n_kv_heads: int,
         hidden_dim: int,
         norm_eps: float,
         head_dim: Optional[int] = None,
         rope_traditional: bool = False,
         rope_theta: float = 1000,
         rope_scaling: Optional[Dict[str, Union[float, str]]] = None,
+        gemma: bool = False,
     ) -> None:
         super().__init__()
         self.n_heads = n_heads
         self.dim = dim
         self.attention = Attention(
             dim=dim,
             n_heads=n_heads,
             n_kv_heads=n_kv_heads,
             head_dim=head_dim,
             rope_traditional=rope_traditional,
             rope_theta=rope_theta,
             rope_scaling=rope_scaling,
         )
-        self.mlp = MLP(dim=dim, hidden_dim=hidden_dim)
-        self.attention_norm = nn.RMSNorm(dim, eps=norm_eps)
-        # self.attention_norm = RMSNorm(dim, eps=norm_eps)
-        self.mlp_norm = nn.RMSNorm(dim, eps=norm_eps)
-        # self.mlp_norm = RMSNorm(dim, eps=norm_eps)
+        self.mlp = MLP(dim=dim, hidden_dim=hidden_dim, gemma=gemma)
+
+        if not gemma:
+            self.attention_norm = nn.RMSNorm(dim, eps=norm_eps)
+            self.mlp_norm = nn.RMSNorm(dim, eps=norm_eps)
+        else:
+            self.attention_norm = RMSNorm(dim, eps=norm_eps)
+            self.mlp_norm = RMSNorm(dim, eps=norm_eps)
 
     def __call__(
         self,
         x: mx.array,
         mask: Optional[mx.array] = None,
         kv_cache: Optional[Tuple[mx.array, mx.array]] = None,
     ) -> Tuple[mx.array, Tuple[mx.array, mx.array]]:
@@ -196,15 +216,15 @@
         n_heads (int): number of attention heads
         n_kv_heads (Optional[int]): number of key-value heads. If None, it is set to num_heads. Defaults to None.
         head_dim (Optional[int], optional): head dimension. Defaults to None.
         norm_eps (float): normalization epsilon. Defaults to 1e-5.
         rope_traditional (bool, optional): whether to use traditional RoPE. Defaults to False.
         rope_theta (float, optional): RoPE theta. Defaults to 1000.
         rope_scaling (Optional[Dict[str, Union[float, str]]], optional): RoPE scaling. Defaults to None.
-        embed_as_head (bool, optional): whether to embed as head (for Gemma models). Defaults to False.
+        gemma (bool, optional): whether to use Gemma Transformer. Defaults to False.
     """
 
     def __init__(
         self,
         dim: int,
         hidden_dim: int,
         vocab_size: int,
@@ -212,40 +232,46 @@
         n_heads: int,
         n_kv_heads: Optional[int] = None,
         head_dim: Optional[int] = None,
         norm_eps: float = 1e-5,
         rope_traditional: bool = False,
         rope_theta: float = 1000,
         rope_scaling: Optional[Dict[str, Union[float, str]]] = None,
-        embed_as_head: bool = False,
+        gemma: bool = False,
     ):
         super().__init__()
+        self.dim = dim
+        self.hidden_dim = hidden_dim
         self.vocab_size = vocab_size
         self.n_layers = n_layers
+        self.gemma = gemma
         assert self.vocab_size > 0
         if n_kv_heads is None:
             n_kv_heads = n_heads
-        self.token_embed = nn.Embedding(vocab_size, dim)
+        self.token_embed = nn.Embedding(vocab_size, self.dim)
         self.layers = [
             TransformerBlock(
                 dim=dim,
                 n_heads=n_heads,
                 n_kv_heads=n_kv_heads,
                 hidden_dim=hidden_dim,
                 norm_eps=norm_eps,
                 head_dim=head_dim,
                 rope_traditional=rope_traditional,
                 rope_theta=rope_theta,
                 rope_scaling=rope_scaling,
+                gemma=gemma,
             )
             for _ in range(n_layers)
         ]
-        self.norm = nn.RMSNorm(dim, eps=norm_eps)
-        # self.norm = nn.RMSNorm(dim, eps=norm_eps)
-        if not embed_as_head:
+        if not self.gemma:
+            self.norm = nn.RMSNorm(dim, eps=norm_eps)
+        else:
+            self.norm = RMSNorm(dim, eps=norm_eps)
+        if not self.gemma:
             self.head = nn.Linear(dim, vocab_size, bias=False)
         else:
             self.head = None  # type: ignore
 
     def embed(
         self, x: mx.array, kv_cache: Optional[List[Tuple[mx.array, mx.array]]] = None, norm: bool = False
     ) -> Tuple[mx.array, Optional[List[Tuple[mx.array, mx.array]]]]:
@@ -257,14 +283,17 @@
             norm (bool, optional): whether to normalize the output. Defaults to False.
 
         Returns:
             Tuple[mx.array, Optional[List[Tuple[mx.array, mx.array]]]]: output and key-value cache
         """
         h = self.token_embed(x)
 
+        if self.gemma:
+            h = h * (self.dim**0.5)
+
         mask = None
         if h.shape[1] > 1:
             mask = nn.MultiHeadAttention.create_additive_causal_mask(h.shape[1])
             mask = mask.astype(h.dtype)
 
         if kv_cache is None:
             kv_cache = [None] * len(self.layers)  # type: ignore
@@ -283,18 +312,18 @@
             x (mx.array): input tokens
             kv_cache (Optional[List[mx.array]], optional): key-value cache. Defaults to None.
 
         Returns:
             Tuple[mx.array, List[mx.array]]: output and key-value cache
         """
         x, kv_cache = self.embed(x, kv_cache=kv_cache, norm=True)
-        if self.head is not None:
-            out = self.head(x)
-        else:
+        if self.gemma is not None:
             out = self.token_embed.as_linear(x)
+        else:
+            out = self.head(x)
         return out, kv_cache  # type: ignore
 
     def generate(self, x: mx.array, temp: Optional[float] = 0.0):
         """Generate tokens from a given input
 
         Args:
             x (mx.array): input tokens
```

### Comparing `mlx_llm-1.0.1/src/mlx_llm/prompt/__init__.py` & `mlx_llm-1.0.2/src/mlx_llm/prompt/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from ._base import Prompt
 from .llama import LLaMA2Prompt, LLaMA3Prompt, TinyLLaMAPrompt
+from .gemma import GemmaPrompt
 from .mistral import MistralPrompt
 from .phi import Phi3Prompt
 
 PROMPT_ENTRYPOINTS = {
     "llama2": LLaMA2Prompt,
     "llama3": LLaMA3Prompt,
     "phi3": Phi3Prompt,
     "mistral": MistralPrompt,
     "tinyllama": TinyLLaMAPrompt,
+    "gemma": GemmaPrompt,
 }
 
 
 def create_prompt(model_name: str, system: str = "") -> Prompt:
     """Create prompt based on model family
 
     Args:
```

### Comparing `mlx_llm-1.0.1/src/mlx_llm/prompt/llama.py` & `mlx_llm-1.0.2/src/mlx_llm/prompt/llama.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/src/mlx_llm/prompt/mistral.py` & `mlx_llm-1.0.2/src/mlx_llm/prompt/mistral.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/src/mlx_llm/prompt/phi.py` & `mlx_llm-1.0.2/src/mlx_llm/prompt/phi.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/src/mlx_llm/utils/hf.py` & `mlx_llm-1.0.2/src/mlx_llm/utils/hf.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/src/mlx_llm/utils/session.py` & `mlx_llm-1.0.2/src/mlx_llm/utils/session.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/src/mlx_llm/utils/time.py` & `mlx_llm-1.0.2/src/mlx_llm/utils/time.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/src/mlx_llm/utils/weights.py` & `mlx_llm-1.0.2/src/mlx_llm/utils/weights.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.1/PKG-INFO` & `mlx_llm-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx_llm
-Version: 1.0.1
+Version: 1.0.2
 Summary: Large Language Models (LLMs) applications and tools running on Apple Silicon in real-time with Apple MLX
 Author: Riccardo Musmeci
 Author-email: riccardomusmeci92@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

