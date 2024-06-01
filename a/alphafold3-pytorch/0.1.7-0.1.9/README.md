# Comparing `tmp/alphafold3_pytorch-0.1.7.tar.gz` & `tmp/alphafold3_pytorch-0.1.9.tar.gz`

## Comparing `alphafold3_pytorch-0.1.7.tar` & `alphafold3_pytorch-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/.env.sample
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/Dockerfile
--rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/alphafold3.png
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/contribute.sh
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/.github/workflows/test.yml
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/alphafold3_pytorch/__init__.py
--rw-r--r--   0        0        0   105991 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/alphafold3_pytorch/alphafold3.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/alphafold3_pytorch/attention.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/alphafold3_pytorch/life.py
--rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/alphafold3_pytorch/trainer.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/alphafold3_pytorch/typing.py
--rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/docs/alphafold3-supplementary.pdf
--rw-r--r--   0        0        0    16404 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/tests/test_af3.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/tests/test_trainer.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/LICENSE
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/README.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/.env.sample
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/Dockerfile
+-rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/alphafold3.png
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/contribute.sh
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/alphafold3_pytorch/__init__.py
+-rw-r--r--   0        0        0   105991 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/alphafold3_pytorch/alphafold3.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/alphafold3_pytorch/attention.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/alphafold3_pytorch/life.py
+-rw-r--r--   0        0        0    14134 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/alphafold3_pytorch/trainer.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/alphafold3_pytorch/typing.py
+-rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/docs/alphafold3-supplementary.pdf
+-rw-r--r--   0        0        0    16404 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/tests/test_af3.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/tests/test_trainer.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/LICENSE
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.9/PKG-INFO
```

### Comparing `alphafold3_pytorch-0.1.7/Dockerfile` & `alphafold3_pytorch-0.1.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.7/alphafold3.png` & `alphafold3_pytorch-0.1.9/alphafold3.png`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.7/.github/workflows/publish.yml` & `alphafold3_pytorch-0.1.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.7/alphafold3_pytorch/__init__.py` & `alphafold3_pytorch-0.1.9/alphafold3_pytorch/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     DistogramHead,
     Alphafold3
 )
 
 from alphafold3_pytorch.trainer import (
     Trainer,
     DataLoader,
-    Alphafold3Input
+    AtomInput
 )
 
 __all__ = [
     Attention,
     Attend,
     RelativePositionEncoding,
     SmoothLDDTLoss,
@@ -62,10 +62,10 @@
     DiffusionTransformer,
     DiffusionModule,
     ElucidatedAtomDiffusion,
     InputFeatureEmbedder,
     ConfidenceHead,
     DistogramHead,
     Alphafold3,
-    Alphafold3Input,
+    AtomInput,
     Trainer
 ]
```

### Comparing `alphafold3_pytorch-0.1.7/alphafold3_pytorch/alphafold3.py` & `alphafold3_pytorch-0.1.9/alphafold3_pytorch/alphafold3.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.7/alphafold3_pytorch/attention.py` & `alphafold3_pytorch-0.1.9/alphafold3_pytorch/attention.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.7/alphafold3_pytorch/life.py` & `alphafold3_pytorch-0.1.9/alphafold3_pytorch/life.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.7/alphafold3_pytorch/trainer.py` & `alphafold3_pytorch-0.1.9/alphafold3_pytorch/trainer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
+from functools import wraps
 from pathlib import Path
 
 from alphafold3_pytorch.alphafold3 import Alphafold3
 from alphafold3_pytorch.attention import pad_at_dim
 
 from typing import TypedDict, List
+
 from alphafold3_pytorch.typing import (
     typecheck,
+    beartype_isinstance,
     Int, Bool, Float
 )
 
 import torch
 from torch import Tensor
 from torch.optim import Adam, Optimizer
 from torch.utils.data import Dataset, DataLoader as OrigDataLoader
@@ -21,25 +24,25 @@
 from ema_pytorch import EMA
 
 from lightning import Fabric
 
 # constants
 
 @typecheck
-class Alphafold3Input(TypedDict):
+class AtomInput(TypedDict):
     atom_inputs:                Float['m dai']
-    molecule_atom_lens:          Int[' n']
+    molecule_atom_lens:         Int[' n']
     atompair_inputs:            Float['m m dapi'] | Float['nw w (w*2) dapi']
-    additional_molecule_feats:   Float['n 10']
+    additional_molecule_feats:  Float['n 10']
     templates:                  Float['t n n dt']
     msa:                        Float['s n dm']
     template_mask:              Bool[' t'] | None
     msa_mask:                   Bool[' s'] | None
     atom_pos:                   Float['m 3'] | None
-    molecule_atom_indices:       Int[' n'] | None
+    molecule_atom_indices:      Int[' n'] | None
     distance_labels:            Int['n n'] | None
     pae_labels:                 Int['n n'] | None
     pde_labels:                 Int[' n'] | None
     resolved_labels:            Int[' n'] | None
 
 # helpers
 
@@ -73,46 +76,76 @@
 
     return past_losses
 
 # dataloader and collation fn
 
 @typecheck
 def collate_af3_inputs(
-    inputs: List[Alphafold3Input],
-    int_pad_value = -1
+    inputs: List,
+    int_pad_value = -1,
+    map_input_fn: Callable | None = None
 ):
+
+    if exists(map_input_fn):
+        inputs = [map_input_fn(i) for i in inputs]
+
+    # make sure all inputs are AtomInput
+
+    assert all([beartype_isinstance(i, AtomInput) for i in inputs])
+
     # separate input dictionary into keys and values
 
     keys = inputs[0].keys()
     inputs = [i.values() for i in inputs]
 
     outputs = []
 
     for grouped in zip(*inputs):
         # if all None, just return None
 
-        if not any([*map(exists, grouped)]):
+        not_none_grouped = [*filter(exists, grouped)]
+
+        if len(not_none_grouped) == 0:
             outputs.append(None)
             continue
 
+        # default to empty tensor for any Nones
+
+        one_tensor = not_none_grouped[0]
+
+        dtype = one_tensor.dtype
+        ndim = one_tensor.ndim
+
         # use -1 for padding int values, for assuming int are labels - if not, handle within alphafold3
 
-        pad_value = int_pad_value if grouped[0].dtype in (torch.int, torch.long) else 0
+        if dtype in (torch.int, torch.long):
+            pad_value = int_pad_value
+        elif dtype == torch.bool:
+            pad_value = False
+        else:
+            pad_value = 0.
 
         # get the max lengths across all dimensions
 
-        shapes_as_tensor = torch.stack([Tensor(tuple(g.shape)) for g in grouped], dim = -1)
+        shapes_as_tensor = torch.stack([Tensor(tuple(g.shape) if exists(g) else ((0,) * ndim)).int() for g in grouped], dim = -1)
+
+        max_lengths = shapes_as_tensor.amax(dim = -1)
 
-        max_lengths = shapes_as_tensor.int().amax(dim = -1)
+        default_tensor = torch.full(max_lengths.tolist(), pad_value, dtype = dtype)
 
         # pad across all dimensions
 
         padded_inputs = []
 
         for inp in grouped:
+
+            if not exists(inp):
+                padded_inputs.append(default_tensor)
+                continue
+
             for dim, max_length in enumerate(max_lengths.tolist()):
                 inp = pad_at_dim(inp, (0, max_length - inp.shape[dim]), value = pad_value, dim = dim)
 
             padded_inputs.append(inp)
 
         # stack
 
@@ -120,16 +153,26 @@
 
         outputs.append(stacked)
 
     # reconstitute dictionary
 
     return dict(tuple(zip(keys, outputs)))
 
-def DataLoader(*args, **kwargs):
-    return OrigDataLoader(*args, collate_fn = collate_af3_inputs, **kwargs)
+@typecheck
+def DataLoader(
+    *args,
+    map_input_fn: Callable | None = None,
+    **kwargs
+):
+    collate_fn = collate_af3_inputs
+
+    if exists(map_input_fn):
+        collate_fn = partial(collate_fn, map_input_fn = map_input_fn)
+
+    return OrigDataLoader(*args, collate_fn = collate_fn, **kwargs)
 
 # default scheduler used in paper w/ warmup
 
 def default_lambda_lr_fn(steps):
     # 1000 step warmup
 
     if steps < 1000:
@@ -150,14 +193,15 @@
         self,
         model: Alphafold3,
         *,
         dataset: Dataset,
         num_train_steps: int,
         batch_size: int,
         grad_accum_every: int = 1,
+        map_dataset_input_fn: Callable | None = None,
         valid_dataset: Dataset | None = None,
         valid_every: int = 1000,
         test_dataset: Dataset | None = None,
         optimizer: Optimizer | None = None,
         scheduler: LRScheduler | None = None,
         ema_decay = 0.999,
         lr = 1.8e-3,
@@ -204,35 +248,42 @@
                 model.parameters(),
                 lr = lr,
                 **default_adam_kwargs
             )
 
         self.optimizer = optimizer
 
+        # if map dataset function given, curry into DataLoader
+
+        DataLoader_ = DataLoader
+
+        if exists(map_dataset_input_fn):
+            DataLoader_ = partial(DataLoader_, map_input_fn = map_dataset_input_fn)
+
         # train dataloader
 
-        self.dataloader = DataLoader(dataset, batch_size = batch_size, shuffle = True, drop_last = True)
+        self.dataloader = DataLoader_(dataset, batch_size = batch_size, shuffle = True, drop_last = True)
 
         # validation dataloader on the EMA model
 
         self.valid_every = valid_every
 
         self.needs_valid = exists(valid_dataset)
 
         if self.needs_valid and self.is_main:
             self.valid_dataset_size = len(valid_dataset)
-            self.valid_dataloader = DataLoader(valid_dataset, batch_size = batch_size)
+            self.valid_dataloader = DataLoader_(valid_dataset, batch_size = batch_size)
 
         # testing dataloader on EMA model
 
         self.needs_test = exists(test_dataset)
 
         if self.needs_test and self.is_main:
             self.test_dataset_size = len(test_dataset)
-            self.test_dataloader = DataLoader(test_dataset, batch_size = batch_size)
+            self.test_dataloader = DataLoader_(test_dataset, batch_size = batch_size)
 
         # training steps and num gradient accum steps
 
         self.num_train_steps = num_train_steps
         self.grad_accum_every = grad_accum_every
 
         # setup fabric
```

### Comparing `alphafold3_pytorch-0.1.7/alphafold3_pytorch/typing.py` & `alphafold3_pytorch-0.1.9/alphafold3_pytorch/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from functools import wraps
 from environs import Env
 
 from torch import Tensor
 
 from beartype import beartype
+from beartype.door import is_bearable
+
 from jaxtyping import (
     Float,
     Int,
     Bool,
     jaxtyped
 )
 
 # environment
 
 env = Env()
 env.read_env()
 
 # function
 
+def always(value):
+    def inner(*args, **kwargs):
+        return value
+    return inner
+
 def null_decorator(fn):
     @wraps(fn)
     def inner(*args, **kwargs):
         return fn(*args, **kwargs)
     return inner
 
 # jaxtyping is a misnomer, works for pytorch
@@ -39,13 +46,16 @@
 
 # use env variable TYPECHECK to control whether to use beartype + jaxtyping
 
 should_typecheck = env.bool('TYPECHECK', False)
 
 typecheck = jaxtyped(typechecker = beartype) if should_typecheck else null_decorator
 
+beartype_isinstance = is_bearable if should_typecheck else always(True)
+
 __all__ = [
     Float,
     Int,
     Bool,
-    typecheck
+    typecheck,
+    beartype_isinstance
 ]
```

### Comparing `alphafold3_pytorch-0.1.7/docs/alphafold3-supplementary.pdf` & `alphafold3_pytorch-0.1.9/docs/alphafold3-supplementary.pdf`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.7/tests/test_af3.py` & `alphafold3_pytorch-0.1.9/tests/test_af3.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.7/tests/test_trainer.py` & `alphafold3_pytorch-0.1.9/tests/test_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 os.environ['TYPECHECK'] = 'True'
 
 from pathlib import Path
-from random import randrange
+from random import randrange, random
 
 import pytest
 import torch
 from torch.utils.data import Dataset
 
 from alphafold3_pytorch import (
     Alphafold3,
-    Alphafold3Input,
+    AtomInput,
     DataLoader,
     Trainer
 )
 
 # mock dataset
 
 class MockAtomDataset(Dataset):
@@ -41,28 +41,31 @@
         molecule_atom_lens = torch.randint(1, self.atoms_per_window, (seq_len,))
         additional_molecule_feats = torch.randn(seq_len, 10)
 
         templates = torch.randn(2, seq_len, seq_len, 44)
         template_mask = torch.ones((2,)).bool()
 
         msa = torch.randn(7, seq_len, 64)
-        msa_mask = torch.ones((7,)).bool()
+
+        msa_mask = None
+        if random() > 0.5:
+            msa_mask = torch.ones((7,)).bool()
 
         # required for training, but omitted on inference
 
         atom_pos = torch.randn(atom_seq_len, 3)
         molecule_atom_indices = molecule_atom_lens - 1
 
         distance_labels = torch.randint(0, 37, (seq_len, seq_len))
         pae_labels = torch.randint(0, 64, (seq_len, seq_len))
         pde_labels = torch.randint(0, 64, (seq_len, seq_len))
         plddt_labels = torch.randint(0, 50, (seq_len,))
         resolved_labels = torch.randint(0, 2, (seq_len,))
 
-        return Alphafold3Input(
+        return AtomInput(
             atom_inputs = atom_inputs,
             atompair_inputs = atompair_inputs,
             molecule_atom_lens = molecule_atom_lens,
             additional_molecule_feats = additional_molecule_feats,
             templates = templates,
             template_mask = template_mask,
             msa = msa,
```

### Comparing `alphafold3_pytorch-0.1.7/.gitignore` & `alphafold3_pytorch-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.7/LICENSE` & `alphafold3_pytorch-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.7/README.md` & `alphafold3_pytorch-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.7/pyproject.toml` & `alphafold3_pytorch-0.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alphafold3-pytorch"
-version = "0.1.7"
+version = "0.1.9"
 description = "Alphafold 3 - Pytorch"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { file = "LICENSE" }
```

### Comparing `alphafold3_pytorch-0.1.7/PKG-INFO` & `alphafold3_pytorch-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: alphafold3-pytorch
-Version: 0.1.7
+Version: 0.1.9
 Summary: Alphafold 3 - Pytorch
 Project-URL: Homepage, https://pypi.org/project/alphafold3-pytorch/
 Project-URL: Repository, https://github.com/lucidrains/alphafold3-pytorch
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.1.7 Summary:
+Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.1.9 Summary:
 Alphafold 3 - Pytorch Project-URL: Homepage, https://pypi.org/project/
 alphafold3-pytorch/ Project-URL: Repository, https://github.com/lucidrains/
 alphafold3-pytorch Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

