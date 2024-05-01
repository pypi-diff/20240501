# Comparing `tmp/infini_transformer_pytorch-0.0.1.tar.gz` & `tmp/infini_transformer_pytorch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infini_transformer_pytorch-0.0.1.tar", last modified: Wed May  1 20:56:37 2024, max compression
+gzip compressed data, was "infini_transformer_pytorch-0.0.2.tar", last modified: Wed May  1 21:05:49 2024, max compression
```

## Comparing `infini_transformer_pytorch-0.0.1.tar` & `infini_transformer_pytorch-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:56:37.448586 infini_transformer_pytorch-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 20:56:30.000000 infini_transformer_pytorch-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 20:56:37.448586 infini_transformer_pytorch-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-01 20:56:30.000000 infini_transformer_pytorch-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:56:37.448586 infini_transformer_pytorch-0.0.1/infini_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 20:56:30.000000 infini_transformer_pytorch-0.0.1/infini_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-05-01 20:56:30.000000 infini_transformer_pytorch-0.0.1/infini_transformer_pytorch/infini_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:56:37.448586 infini_transformer_pytorch-0.0.1/infini_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 20:56:37.000000 infini_transformer_pytorch-0.0.1/infini_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 20:56:37.000000 infini_transformer_pytorch-0.0.1/infini_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:56:37.000000 infini_transformer_pytorch-0.0.1/infini_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 20:56:37.000000 infini_transformer_pytorch-0.0.1/infini_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 20:56:37.000000 infini_transformer_pytorch-0.0.1/infini_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:56:37.452586 infini_transformer_pytorch-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 20:56:30.000000 infini_transformer_pytorch-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:05:49.921339 infini_transformer_pytorch-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 21:05:44.000000 infini_transformer_pytorch-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 21:05:49.921339 infini_transformer_pytorch-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-01 21:05:44.000000 infini_transformer_pytorch-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:05:49.917339 infini_transformer_pytorch-0.0.2/infini_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 21:05:44.000000 infini_transformer_pytorch-0.0.2/infini_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-01 21:05:44.000000 infini_transformer_pytorch-0.0.2/infini_transformer_pytorch/infini_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:05:49.917339 infini_transformer_pytorch-0.0.2/infini_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 21:05:49.000000 infini_transformer_pytorch-0.0.2/infini_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 21:05:49.000000 infini_transformer_pytorch-0.0.2/infini_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:05:49.000000 infini_transformer_pytorch-0.0.2/infini_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 21:05:49.000000 infini_transformer_pytorch-0.0.2/infini_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 21:05:49.000000 infini_transformer_pytorch-0.0.2/infini_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:05:49.921339 infini_transformer_pytorch-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 21:05:44.000000 infini_transformer_pytorch-0.0.2/setup.py
```

### Comparing `infini_transformer_pytorch-0.0.1/LICENSE` & `infini_transformer_pytorch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.1/PKG-INFO` & `infini_transformer_pytorch-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.1/README.md` & `infini_transformer_pytorch-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.1/infini_transformer_pytorch/infini_transformer.py` & `infini_transformer_pytorch-0.0.2/infini_transformer_pytorch/infini_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 class CausalAttention(Module):
     def __init__(
         self,
         dim,
         *,
         dim_head = 128,
         heads = 8,
-        head_gate_init_value = 10.
+        head_gate_init_value = 10.,
+        use_mem_delta_rule = False
     ):
         super().__init__()
         dim_inner = dim_head * heads
         self.scale = dim_head ** -0.5
         self.norm = RMSNorm(dim)
 
         self.rotary_emb = RotaryEmbedding(dim_head)
@@ -70,14 +71,16 @@
         self.to_out = nn.Linear(dim_inner, dim, bias = False)
 
         self.split_heads = Rearrange('b n (qkv h d) -> qkv b h n d', qkv = 3, h = heads)
         self.merge_heads = Rearrange('b h n d -> b n (h d)')
 
         self.head_gates = nn.Parameter(torch.ones(heads) * head_gate_init_value)
 
+        self.use_mem_delta_rule = use_mem_delta_rule
+
     def forward(
         self,
         x,
         past_memories: Optional[Memories] = None,
         eps = 1e-10
     ) -> Tuple[Tensor, Memories]:
         """
@@ -135,32 +138,42 @@
         if exists(past_memories):
             past_memories_kv, past_memories_norm = past_memories
 
             mem_out_unnormed = einsum(q, past_memories_kv, 'b h n dk, b h dk dv -> b h n dv')
             mem_norm = einsum(q, past_memories_norm, 'b h n d, b h d -> b h n')
 
             mem_norm = rearrange(mem_norm, '... -> ... 1')
-            mem_out = mem_out_unnormed / mem_norm.clamp(min = eps)
+            mem_out = mem_out_unnormed / mem_norm.clamp(min = eps) # eq (3)
 
             # now combine the present output of queries with the outputs querying the past compressed key/value memories
             # in paper, they use a sigmoid gating scheme with learned gate per head
 
             gates = rearrange(self.head_gates, 'h -> h 1 1')
             gates = gates.sigmoid()
 
-            out = out * gates + mem_out * (1. - gates)
+            out = out * gates + mem_out * (1. - gates)  # eq (6)
 
         # create the next memories
 
+        if exists(past_memories) and self.use_mem_delta_rule:
+            # eq (5) - the delta rule
+            v_unnormed = einsum(k, past_memories_kv, 'b h n dk, b h dk dv -> b h n dv')
+            v_norm = einsum(k, past_memories_norm, 'b h n d, b h d -> b h n')
+
+            v_norm = rearrange(v_norm, '... -> ... 1')
+            delta_v = v_unnormed / v_norm.clamp(min = eps)
+
+            v = v - delta_v
+
         new_memories_kv = einsum(k, v, '... n dk, ... n dv -> ... dk dv')
         new_memories_norm = reduce(k, 'b h n d -> b h d', 'sum')
 
         if exists(past_memories):
-            new_memories_kv = new_memories_kv + past_memories_kv
-            new_memories_norm = new_memories_norm + past_memories_norm
+            new_memories_kv = new_memories_kv + past_memories_kv          # eq (4)
+            new_memories_norm = new_memories_norm + past_memories_norm    # eq (4)
 
         new_memories = (new_memories_kv, new_memories_norm)
 
         # merge heads and combine
 
         out = self.merge_heads(out)
         out = self.to_out(out)
@@ -174,28 +187,30 @@
         self,
         *,
         num_tokens,
         dim,
         depth,
         dim_head = 128,
         heads = 8,
-        ff_mult = 4
+        ff_mult = 4,
+        use_mem_delta_rule = False  # in the paper, the delta rule didn't seem to do that much, but will include for completeness
     ):
         super().__init__()
 
         self.token_emb = nn.Embedding(num_tokens, dim)
 
         self.layers = ModuleList([])
 
         for _ in range(depth):
 
             attn = CausalAttention(
                 dim = dim,
                 dim_head = dim_head,
-                heads = heads
+                heads = heads,
+                use_mem_delta_rule = use_mem_delta_rule
             )
 
             ff = FeedForward(
                 dim = dim,
                 mult = ff_mult
             )
```

### Comparing `infini_transformer_pytorch-0.0.1/infini_transformer_pytorch.egg-info/PKG-INFO` & `infini_transformer_pytorch-0.0.2/infini_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.1/setup.py` & `infini_transformer_pytorch-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'infini-transformer-pytorch',
   packages = find_packages(exclude = []),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'Infini-Transformer in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/infini-transformer-pytorch',
   keywords = [
```

