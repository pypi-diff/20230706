# Comparing `tmp/psh-pytorch-0.0.2.tar.gz` & `tmp/psh-pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psh-pytorch-0.0.2.tar", last modified: Tue Jul  4 01:11:00 2023, max compression
+gzip compressed data, was "psh-pytorch-0.0.3.tar", last modified: Thu Jul  6 14:53:40 2023, max compression
```

## Comparing `psh-pytorch-0.0.2.tar` & `psh-pytorch-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/
--rw-rw-r--   0 david     (1000) david     (1000)     1065 2023-07-03 13:56:32.000000 psh-pytorch-0.0.2/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)     2411 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1904 2023-07-03 23:21:44.000000 psh-pytorch-0.0.2/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      730 2023-07-04 01:10:49.000000 psh-pytorch-0.0.2/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       23 2023-07-03 19:52:00.000000 psh-pytorch-0.0.2/requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/setup.cfg
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/src/psh_pytorch/
--rw-rw-r--   0 david     (1000) david     (1000)       35 2023-07-03 21:42:08.000000 psh-pytorch-0.0.2/src/psh_pytorch/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    16062 2023-07-04 00:22:51.000000 psh-pytorch-0.0.2/src/psh_pytorch/psh.py
--rw-rw-r--   0 david     (1000) david     (1000)     1969 2023-07-04 00:21:40.000000 psh-pytorch-0.0.2/src/psh_pytorch/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     2411 2023-07-04 01:11:00.000000 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      336 2023-07-04 01:11:00.000000 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-04 01:11:00.000000 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       24 2023-07-04 01:11:00.000000 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       12 2023-07-04 01:11:00.000000 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/tests/
--rw-rw-r--   0 david     (1000) david     (1000)     3432 2023-07-04 00:55:28.000000 psh-pytorch-0.0.2/tests/test_2d.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 14:53:40.365934 psh-pytorch-0.0.3/
+-rw-rw-r--   0 david     (1000) david     (1000)     1065 2023-07-03 13:56:32.000000 psh-pytorch-0.0.3/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)     2554 2023-07-06 14:53:40.365934 psh-pytorch-0.0.3/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     2047 2023-07-04 18:26:24.000000 psh-pytorch-0.0.3/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      682 2023-07-06 14:52:29.000000 psh-pytorch-0.0.3/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)       98 2023-07-06 14:50:29.000000 psh-pytorch-0.0.3/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-07-06 14:53:40.365934 psh-pytorch-0.0.3/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 14:53:40.365934 psh-pytorch-0.0.3/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 14:53:40.365934 psh-pytorch-0.0.3/src/psh_pytorch/
+-rw-rw-r--   0 david     (1000) david     (1000)       98 2023-07-04 19:49:06.000000 psh-pytorch-0.0.3/src/psh_pytorch/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    20166 2023-07-06 14:47:39.000000 psh-pytorch-0.0.3/src/psh_pytorch/psh.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1951 2023-07-05 14:27:36.000000 psh-pytorch-0.0.3/src/psh_pytorch/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 14:53:40.365934 psh-pytorch-0.0.3/src/psh_pytorch.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     2554 2023-07-06 14:53:40.000000 psh-pytorch-0.0.3/src/psh_pytorch.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      381 2023-07-06 14:53:40.000000 psh-pytorch-0.0.3/src/psh_pytorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-06 14:53:40.000000 psh-pytorch-0.0.3/src/psh_pytorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       17 2023-07-06 14:53:40.000000 psh-pytorch-0.0.3/src/psh_pytorch.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       12 2023-07-06 14:53:40.000000 psh-pytorch-0.0.3/src/psh_pytorch.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 14:53:40.365934 psh-pytorch-0.0.3/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     4868 2023-07-04 18:26:24.000000 psh-pytorch-0.0.3/tests/test_2d_bulb.py
+-rw-rw-r--   0 david     (1000) david     (1000)      433 2023-07-04 18:26:24.000000 psh-pytorch-0.0.3/tests/test_empty.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1384 2023-07-06 14:47:29.000000 psh-pytorch-0.0.3/tests/test_utils.py
```

### Comparing `psh-pytorch-0.0.2/LICENSE` & `psh-pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psh-pytorch-0.0.2/PKG-INFO` & `psh-pytorch-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psh-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Perfect Spatial Hashing in PyTorch
 Author-email: David Li <david@davidl.me>
 Project-URL: Homepage, https://github.com/dli7319/psh-pytorch
 Project-URL: Bug Tracker, https://github.com/dli7319/psh-pytorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,18 +45,27 @@
 #   Note that values are unmasked
 masked_values = values * sparsity.unsqueeze(-1)
 ```
 
 ## Examples
 See `examples/` for a simple example of how to use the library.
 
+If you clone the repository, you can run the example with:
+```bash
+python -m examples.2D_bulb
+```
+
 ## Limitations
 
 1. Currently, interpolation is not supported. Hence, you must use long indices and there are no gradients with respect to the indices.
 
+## Development
+
+* Run tests with `pytest`.
+
 ## Acknowledgement
 If you find this library useful, please consider citing the original paper:
 ```bibtex
 @article{lefebvre2006perfect,
 author = {Lefebvre, Sylvain and Hoppe, Hugues},
 title = {Perfect Spatial Hashing},
 year = {2006},
```

### Comparing `psh-pytorch-0.0.2/README.md` & `psh-pytorch-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,18 +31,27 @@
 #   Note that values are unmasked
 masked_values = values * sparsity.unsqueeze(-1)
 ```
 
 ## Examples
 See `examples/` for a simple example of how to use the library.
 
+If you clone the repository, you can run the example with:
+```bash
+python -m examples.2D_bulb
+```
+
 ## Limitations
 
 1. Currently, interpolation is not supported. Hence, you must use long indices and there are no gradients with respect to the indices.
 
+## Development
+
+* Run tests with `pytest`.
+
 ## Acknowledgement
 If you find this library useful, please consider citing the original paper:
 ```bibtex
 @article{lefebvre2006perfect,
 author = {Lefebvre, Sylvain and Hoppe, Hugues},
 title = {Perfect Spatial Hashing},
 year = {2006},
```

### Comparing `psh-pytorch-0.0.2/src/psh_pytorch/psh.py` & `psh-pytorch-0.0.3/src/psh_pytorch/psh.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,116 @@
-from typing import Optional
+from typing import Optional, Callable
 
 import numpy as np
 import torch
 from torch import nn
 import tqdm
 
 from . import utils
 
 
 class PerfectSpatialHash(nn.Module):
-    def __init__(self, occupancy_grid: torch.Tensor, feature_channels: int,
+    def __init__(self, occupancy_grid: Optional[torch.Tensor], feature_channels: int,
                  fast_construction: bool = True,
-                 offset_table_size: Optional[int] = None,
                  fast_construction_offset_table_progression: float = 1.1,
-                 verbose=False):
+                 dimensions: Optional[int] = None,
+                 hash_table_size: Optional[int] = None,
+                 offset_table_size: Optional[int] = None,
+                 build_offset_table: bool = True,
+                 verbose: bool = False):
         """Initialize the perfect hash.
 
         Args:
             occupancy_grid: The occupancy grid as D-dimensional tensor.
             feature_channels: The number of channels of the hash table.
             fast_construction: If true, avoids binary searching over the offset table size.
-            offset_table_size: (Optional) The initial size of the offset table to test.
             fast_construction_offset_table_progression: (Optional) The progression factor of the offset table size.
+            build_offset_table: (Optional) Whether to compute the offset table. Requires the occupancy grid.
+            dimensions: (Optional) The number of dimensions of the hash table. Infered from the occupancy grid
+              if available.
+            hash_table_size: (Optional) The size of the hash table to initialize. Infered from the occupancy
+              grid if available.
+            offset_table_size: (Optional) The initial size of the offset table to test. Infered from the occupancy
+              grid if unspecified.
             verbose: (Optional) Whether to print additional information.
         """
         super().__init__()
-        self.dimensions = len(occupancy_grid.shape)
+        if occupancy_grid is not None:
+            self.dimensions = len(occupancy_grid.shape)
+            num_values = torch.sum(occupancy_grid).item()
+            device = occupancy_grid.device
+            occupancy_grid = occupancy_grid.bool()
+        else:
+            assert dimensions is not None, "Either occupancy_grid or dimensions must be specified."
+            assert hash_table_size is not None, "Either occupancy_grid or hash_table_size must be specified."
+            assert offset_table_size is not None, "Either occupancy_grid or offset_table_size must be specified."
+            assert not build_offset_table, "Cannot build offset table without occupancy grid."
+            self.dimensions = dimensions
+            num_values = 1
+            device = torch.device("cpu")
         self.verbose = verbose
-        device = occupancy_grid.device
-        occupancy_grid = occupancy_grid.bool()
-
-        self.num_values = torch.sum(occupancy_grid).item()
-        self.verbose and print("Number of values:", self.num_values)
+        self.verbose and print("Number of values:", num_values)
 
-        self.hash_table_size = int(np.ceil(
-            self.num_values ** (1 / self.dimensions)))
+        self.hash_table_size = hash_table_size or int(np.ceil(
+            num_values ** (1 / self.dimensions)))
         self.verbose and print("Hash table size:", self.hash_table_size)
         if self.hash_table_size > 256:
             self.hash_table_size = int(np.ceil(
-                (1.01 * self.num_values) ** (1 / self.dimensions)))
+                (1.01 * num_values) ** (1 / self.dimensions)))
         self.hash_table = nn.Parameter(torch.zeros(
             (self.hash_table_size,) * self.dimensions + (feature_channels,),
             dtype=torch.float32, device=device))
 
         sigma = 1 / (2 * self.dimensions)
         initial_offset_table_size = offset_table_size or int(np.ceil(
-            (sigma * self.num_values) ** (1 / self.dimensions)))
+            (sigma * num_values) ** (1 / self.dimensions)))
         self.offset_table_size = initial_offset_table_size
         self.verbose and print("Offset table size:", self.offset_table_size)
         self.offset_table = nn.Parameter(torch.zeros(
             (self.offset_table_size,) * self.dimensions + (self.dimensions,),
             dtype=torch.uint8, device=device), requires_grad=False)
 
         self.m0 = torch.ones((self.dimensions,),
                              dtype=torch.float32, device=device)
         self.m1 = torch.ones((self.dimensions,),
                              dtype=torch.float32, device=device)
         self.oscale = np.ceil(self.hash_table_size / 255)
 
-        while not self._build_offset_table(occupancy_grid):
+        while build_offset_table and not self._build_offset_table(occupancy_grid):
             # Increase the offset table size.
             new_offset_table_size = int(max(
                 np.round(fast_construction_offset_table_progression *
                          self.offset_table_size),
                 self.offset_table_size + 1))
             self.verbose and print(
                 f"Increasing offset table size to {new_offset_table_size}")
             self.offset_table_size = new_offset_table_size
             self.offset_table = nn.Parameter(torch.zeros(
                 (self.offset_table_size,) *
                 self.dimensions + (self.dimensions,),
                 dtype=torch.uint8, device=device), requires_grad=False)
         # Reset the hash table.
         self.hash_table.data = torch.rand_like(self.hash_table.data)
-        if not fast_construction:
+        if build_offset_table and not fast_construction:
             # TODO: Binary search for the offset table size.
-            low = initial_offset_table_size
-            high = self.offset_table_size + 1
+            # low = initial_offset_table_size
+            # high = self.offset_table_size + 1
             raise NotImplementedError("Slow construction not implemented yet.")
 
-        self.sparsity_encoding = self._build_sparsity_encoding(occupancy_grid)
+        if build_offset_table:
+            self.sparsity_encoding = self._build_sparsity_encoding(
+                occupancy_grid)
+        else:
+            self.sparsity_encoding = nn.Parameter(torch.zeros(
+                tuple(self.hash_table.shape[:-1]) + (2,),
+                dtype=torch.uint8, device=device),
+                requires_grad=False)
+
+        self._register_load_state_dict_pre_hook(
+            self._update_parameter_sizes_from_state_dict)
 
     def _build_offset_table(self, occupancy_grid: torch.Tensor) -> bool:
         """Build the offset table.
 
         Returns:
             bool: True if the offset table was built successfully.
         """
@@ -112,15 +139,15 @@
             indices = occupied_indices[pixels]
             indices_h0 = (indices * self.m0).long() % self.hash_table_size
             indices_h0 = utils.ravel_multi_index(
                 indices_h0, self.hash_table.shape[:-1])
             if (torch.bincount(indices_h0) > 1).any():
                 return False
 
-        offset_table_assigned = torch.zeros_like(self.offset_table[:, :, 0])
+        offset_table_assigned = torch.zeros_like(self.offset_table[..., 0])
 
         current_index = 0
         # Assign the first offset.
         self.offset_table[offset_table_indices_sorted[current_index]] = torch.randint(
             0, 256, (self.dimensions,), dtype=torch.uint8, device=self.offset_table.device)
         used_pixels = occupied_indices_ohashed_raveled == ordering[current_index]
         self.hash_table.data[self.compute_hash(
@@ -153,86 +180,111 @@
                 self.hash_table.data[hash_index.unbind(-1)] = 1
                 self.offset_table[current_offset_index.unbind(-1)] = offset
                 offset_table_assigned[current_offset_index.unbind(-1)] = 1
                 offset_assigned = True
                 return True
 
             # Heuristic 1: Try the neighboring pixels.
-            if not offset_assigned:
-                if len(pixel_indices) < 10:
-                    for pixel_index in pixel_indices:
-                        for direction in range(self.dimensions):
-                            direction_offset = torch.zeros(
-                                (self.dimensions,), dtype=torch.long, device=self.offset_table.device)
-                            direction_offset[direction] = 1
-                            index = (pixel_index +
-                                     direction_offset).clamp(0, occupancy_grid_size - 1)
-                            oindex = (
-                                index * self.m1).long() % self.offset_table_size
-                            if (offset_table_assigned[oindex.unbind(-1)] and
-                                    assign_offset(self.offset_table[oindex.unbind(-1)].clone())):
-                                break
-                            direction_offset[direction] = -1
-                            index = (pixel_index +
-                                     direction_offset).clamp(0, occupancy_grid_size - 1)
-                            oindex = (
-                                index * self.m1).long() % self.offset_table_size
-                            if (offset_table_assigned[oindex.unbind(-1)] and
-                                    assign_offset(self.offset_table[oindex.unbind(-1)].clone())):
-                                break
+            offset_assigned or self._assign_offset_from_neighboring_pixels(
+                pixel_indices, offset_table_assigned,
+                occupancy_grid_size, assign_offset)
 
             # Heuristic 2: Try the neighboring offsets.
-            if not offset_assigned:
-                for direction in range(self.dimensions):
-                    direction_offset = torch.zeros(
-                        (self.dimensions,), dtype=torch.long, device=self.offset_table.device)
-                    direction_offset[direction] = 1
-                    index = (current_offset_index +
-                             direction_offset).clamp(0, self.offset_table_size - 1)
-                    if (offset_table_assigned[index.unbind(-1)] and
-                            assign_offset(self.offset_table[index.unbind(-1)].clone())):
-                        break
-                    direction_offset[direction] = -1
-                    index = (current_offset_index +
-                             direction_offset).clamp(0, self.offset_table_size - 1)
-                    if (offset_table_assigned[index.unbind(-1)] and
-                            assign_offset(self.offset_table[index.unbind(-1)].clone())):
-                        break
+            offset_assigned or self._assign_offset_from_neighboring_offsets(
+                current_offset_index, offset_table_assigned, assign_offset)
 
             # Heuristic 3: Try random offsets.
-            if not offset_assigned:
-                for _ in range(100):
-                    random_offset = torch.randint(
-                        0, 256, (self.dimensions,), dtype=torch.uint8, device=self.offset_table.device)
-                    if assign_offset(random_offset):
-                        break
+            offset_assigned or self._assign_offset_from_random_offsets(
+                assign_offset)
 
             # Heuristic 4: Find empty positions in the hash table.
-            if not offset_assigned:
-                for _ in range(100):
-                    random_pixel = torch.randint(
-                        0, 256, (self.dimensions,), dtype=torch.uint8, device=self.offset_table.device)
-                    # Hashed position of the pixel.
-                    random_pixel_hashed = (
-                        random_pixel * self.m0).long() % self.hash_table_size
-                    # Check if the position is empty.
-                    if self.hash_table[random_pixel_hashed.unbind(-1)][0].item() == 0:
-                        offset = (random_pixel_hashed -
-                                  pixel_indices_hashed[0] + 10 * 255) % 256
-                        if assign_offset(offset):
-                            break
+            offset_assigned or self._assign_offset_from_random_pixels(
+                pixel_indices_hashed, assign_offset)
 
             if not offset_assigned:
                 self.verbose and print(f"Could not assign offset with index {current_index} and " +
                                        f"pixels {occupied_indices_bincount[ordering[current_index]].item()}]")
                 return False
-        # if self.verbose:
-        #     print("offset_table_assigned", offset_table_assigned)
         return True
 
+    def _assign_offset_from_neighboring_pixels(self, pixel_indices: torch.Tensor,
+                                               offset_table_assigned: torch.Tensor,
+                                               occupancy_grid_size: int,
+                                               assign_offset: Callable[[torch.Tensor], bool]) -> bool:
+        """Heuristic: Assign an offset to the current pixel from neighboring pixels."""
+        if len(pixel_indices) >= 10:
+            return False
+        for pixel_index in pixel_indices:
+            for direction in range(self.dimensions):
+                direction_offset = torch.zeros(
+                    (self.dimensions,), dtype=torch.long, device=self.offset_table.device)
+                direction_offset[direction] = 1
+                index = (pixel_index +
+                            direction_offset).clamp(0, occupancy_grid_size - 1)
+                oindex = (
+                    index * self.m1).long() % self.offset_table_size
+                if (offset_table_assigned[oindex.unbind(-1)] and
+                        assign_offset(self.offset_table[oindex.unbind(-1)].clone())):
+                    return True
+                direction_offset[direction] = -1
+                index = (pixel_index +
+                            direction_offset).clamp(0, occupancy_grid_size - 1)
+                oindex = (
+                    index * self.m1).long() % self.offset_table_size
+                if (offset_table_assigned[oindex.unbind(-1)] and
+                        assign_offset(self.offset_table[oindex.unbind(-1)].clone())):
+                    return True
+        return False
+
+    def _assign_offset_from_neighboring_offsets(self,
+                                                current_offset_index: torch.Tensor,
+                                                offset_table_assigned: torch.Tensor,
+                                                assign_offset: Callable[[torch.Tensor], bool]) -> bool:
+        """Heuristic: Assign an offset to the current pixel from neighboring offsets."""
+        for direction in range(self.dimensions):
+            direction_offset = torch.zeros(
+                (self.dimensions,), dtype=torch.long, device=self.offset_table.device)
+            direction_offset[direction] = 1
+            index = (current_offset_index +
+                     direction_offset).clamp(0, self.offset_table_size - 1)
+            if (offset_table_assigned[index.unbind(-1)] and
+                    assign_offset(self.offset_table[index.unbind(-1)].clone())):
+                return True
+            direction_offset[direction] = -1
+            index = (current_offset_index +
+                     direction_offset).clamp(0, self.offset_table_size - 1)
+            if (offset_table_assigned[index.unbind(-1)] and
+                    assign_offset(self.offset_table[index.unbind(-1)].clone())):
+                return True
+        return False
+
+    def _assign_offset_from_random_offsets(self, assign_offset: Callable[[torch.Tensor], bool]) -> bool:
+        for _ in range(100):
+            random_offset = torch.randint(
+                0, 256, (self.dimensions,), dtype=torch.uint8, device=self.offset_table.device)
+            if assign_offset(random_offset):
+                return True
+        return False
+
+    def _assign_offset_from_random_pixels(self, pixel_indices_hashed: torch.Tensor,
+                                          assign_offset: Callable[[torch.Tensor], bool]) -> bool:
+        for _ in range(100):
+            random_pixel = torch.randint(
+                0, 256, (self.dimensions,), dtype=torch.uint8, device=self.offset_table.device)
+            # Hashed position of the pixel.
+            random_pixel_hashed = (
+                random_pixel * self.m0).long() % self.hash_table_size
+            # Check if the position is empty.
+            if self.hash_table[random_pixel_hashed.unbind(-1)][0].item() == 0:
+                offset = (random_pixel_hashed -
+                          pixel_indices_hashed[0] + 10 * 255) % 256
+                if assign_offset(offset):
+                    return True
+        return False
+
     def _build_sparsity_encoding(self, occupancy_grid: torch.Tensor):
         sparsity_k = torch.zeros(
             self.hash_table[..., 0].shape, dtype=torch.uint8, device=self.hash_table.device)
         sparsity_hk = torch.zeros(
             self.hash_table[..., 0].shape, dtype=torch.uint8, device=self.hash_table.device)
 
         occupied_indices = occupancy_grid.nonzero(as_tuple=False)
@@ -322,7 +374,32 @@
             positions (torch.Tensor): Positions to check.
 
         Returns:
             bool: True if there are collisions, False otherwise.
         """
         hash_indices = self.compute_hash(positions)
         return torch.unique(hash_indices, dim=0).shape[0] != hash_indices.shape[0]
+
+    def _update_parameter_sizes_from_state_dict(self,
+                                                state_dict, prefix,
+                                                local_metadata, strict,
+                                                missing_keys, unexpected_keys, error_msgs):
+        print(list(state_dict.keys()))
+        new_hash_table = state_dict[prefix + "hash_table"]
+        new_sparsity_encoding = state_dict[prefix + "sparsity_encoding"]
+        if self.hash_table_size != new_hash_table.shape[0]:
+            self.hash_table_size = new_hash_table.shape[0]
+            self.hash_table.data = torch.zeros(
+                new_hash_table.shape,
+                dtype=self.hash_table.dtype,
+                device=self.hash_table.device)
+            self.sparsity_encoding.data = torch.zeros(
+                new_sparsity_encoding.shape,
+                dtype=self.sparsity_encoding.dtype,
+                device=self.sparsity_encoding.device)
+        new_offset_table = state_dict[prefix + "offset_table"]
+        if self.offset_table_size != new_offset_table.shape[0]:
+            self.offset_table_size = new_offset_table.shape[0]
+            self.offset_table.data = torch.zeros(
+                new_offset_table.shape,
+                dtype=self.offset_table.dtype,
+                device=self.offset_table.device)
```

### Comparing `psh-pytorch-0.0.2/src/psh_pytorch/utils.py` & `psh-pytorch-0.0.3/src/psh_pytorch/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,58 @@
-from typing import Union
+from typing import Union, Sequence
 
 import torch
 
 
-C1 = [827, 887, 433, 673, 431,
-      271, 587, 607, 859, 953]
+C1 = [79, 23, 71, 31, 11, 64, 41, 67, 89, 43]
 
 
 def ravel_multi_index(multi_index, dims):
     """Convert a multidimensional index into a single index.
 
     Args:
         multi_index (torch.Tensor): The multidimensional index as (N, D) tensor.
         dims (torch.Tensor): The dimensions of the multidimensional index.
 
     Returns:
         torch.Tensor: The single index as (N,) tensor.
     """
     dims_cumprod = torch.tensor(
-        dims[:0:-1], device=multi_index.device).cumprod(0)
-    return torch.sum(multi_index[..., :-1] * dims_cumprod, dim=-1) + multi_index[..., -1]
+        tuple(dims[1:]) + (1,), device=multi_index.device)
+    dims_cumprod = dims_cumprod.flip(0).cumprod(0).flip(0)
+    return torch.sum(multi_index * dims_cumprod, dim=-1)
 
 
 def unravel_index(index, dims):
     """Convert a single index into a multidimensional index.
 
     Args:
         index (torch.Tensor): The single index as (N,) tensor.
         dims (torch.Tensor): The dimensions of the multidimensional index.
 
     Returns:
         torch.Tensor: The multidimensional index as (N, D) tensor.
     """
-    dims_cumprod = torch.tensor(
-        dims[:0:-1], device=index.device).cumprod(0)
-    multi_index = torch.zeros(
-        (*index.shape, len(dims)), device=index.device, dtype=torch.long)
-    for i, dim in enumerate(dims_cumprod):
-        multi_index[..., i] = index // dim
-        index = index % dim
-    multi_index[..., -1] = index
-    return multi_index
+    dims_cumprod = torch.tensor(tuple(dims) + (1, ), device=index.device)
+    dims_cumprod = dims_cumprod.flip(0).cumprod(0).flip(0)
+    return index.unsqueeze(-1) % dims_cumprod[:-1] // dims_cumprod[1:]
 
 
-def sparsity_hash(k: Union[int, torch.Tensor], p: torch.Tensor) -> torch.Tensor:
+def sparsity_hash(k: Union[int, torch.Tensor], p: torch.Tensor,
+                  primes: Union[Sequence[int], torch.Tensor] = C1) -> torch.Tensor:
     """Hash function used for sparsity encoding
 
     Args:
         k: Which hash to use.
         p: Points to hash as (N, D) tensor.
+        primes: (Optional) The primes to use for the hash.
 
     Returns:
         torch.Tensor: The hash as (N,) tensor.
     """
-    if isinstance(k, int):
-        k = torch.tensor(k, device=p.device, dtype=torch.uint8)
-    d = p.shape[-1]
-    k = k.float().unsqueeze(-1)
+    k = torch.as_tensor(k, device=p.device, dtype=torch.float32)
+    k = k.reshape((-1,) * (p.dim() - 1) + (1,))
     p = p.float()
-    primes_tensor = torch.tensor(C1[:d], device=p.device, dtype=torch.float)
-    hk = (p * (p + k * primes_tensor).rsqrt()).sum(dim=-1).frac()
+    primes = (torch.as_tensor(primes[:p.shape[-1]])
+              .to(device=p.device, dtype=torch.float))
+    hk = (p * (p + k * primes).rsqrt()).sum(dim=-1).frac()
     return (256 * hk).clamp(0, 255).to(torch.uint8)
```

### Comparing `psh-pytorch-0.0.2/src/psh_pytorch.egg-info/PKG-INFO` & `psh-pytorch-0.0.3/src/psh_pytorch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psh-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Perfect Spatial Hashing in PyTorch
 Author-email: David Li <david@davidl.me>
 Project-URL: Homepage, https://github.com/dli7319/psh-pytorch
 Project-URL: Bug Tracker, https://github.com/dli7319/psh-pytorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,18 +45,27 @@
 #   Note that values are unmasked
 masked_values = values * sparsity.unsqueeze(-1)
 ```
 
 ## Examples
 See `examples/` for a simple example of how to use the library.
 
+If you clone the repository, you can run the example with:
+```bash
+python -m examples.2D_bulb
+```
+
 ## Limitations
 
 1. Currently, interpolation is not supported. Hence, you must use long indices and there are no gradients with respect to the indices.
 
+## Development
+
+* Run tests with `pytest`.
+
 ## Acknowledgement
 If you find this library useful, please consider citing the original paper:
 ```bibtex
 @article{lefebvre2006perfect,
 author = {Lefebvre, Sylvain and Hoppe, Hugues},
 title = {Perfect Spatial Hashing},
 year = {2006},
```

### Comparing `psh-pytorch-0.0.2/tests/test_2d.py` & `psh-pytorch-0.0.3/tests/test_2d_bulb.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from PIL import Image
 import numpy as np
 import torch
 from psh_pytorch import PerfectSpatialHash
 
 
-class Test2D(unittest.TestCase):
+class Test2DBulb(unittest.TestCase):
     def setUp(self):
         torch.manual_seed(0)
         self.device = device = torch.device("cpu")
         bulb_image_path = "examples/data/bulb.png"
         bulb_image = np.array(Image.open(bulb_image_path),
                               dtype=np.float32) / 255.0
         self.bulb_image = torch.from_numpy(bulb_image).to(device)
@@ -22,14 +22,23 @@
             self.bulb_image[:, :, 3], 3)
 
         self.indices = torch.stack(torch.meshgrid(torch.arange(128, device=device),
                                                   torch.arange(
             128, device=device),
             indexing='ij'), -1)
 
+    def test_hashtable_offsettable_sizes(self):
+        """
+        Check that the hash table and offset table sizes are not too big.
+        """
+        self.assertLessEqual(self.spatial_hash.hash_table_size, 38,
+                             "Hash table size is too big.")
+        self.assertLessEqual(self.spatial_hash.offset_table_size, 30,
+                             "Offset table size is too big.")
+
     def test_collisions(self):
         """
         Check that there are no collisions in the hash table.
         """
         self.assertFalse(self.spatial_hash.check_collisions(
             self.bulb_valid_pixels))
 
@@ -76,10 +85,30 @@
         self.spatial_hash.hash_table.data -= 0.01 * self.spatial_hash.hash_table.grad
         values, sparsity = self.spatial_hash(self.indices.reshape(-1, 2))
         reconstruction = (values * sparsity.unsqueeze(-1)).reshape(128, 128, 3)
         new_loss = torch.sum((reconstruction - gt_image)**2)
         self.assertLess(new_loss, loss,
                         f"New Loss ({new_loss}) >= Old Loss ({loss})")
 
+    def test_load_from_state_dict(self):
+        """
+        Test that we can load from a state dict.
+        """
+        state_dict = self.spatial_hash.state_dict()
+        new_spatial_hash = PerfectSpatialHash(
+            self.bulb_image[:, :, 3], 3,
+            build_offset_table=False)
+        new_spatial_hash.load_state_dict(state_dict)
+
+        self.assertTrue(torch.allclose(self.spatial_hash.hash_table,
+                                       new_spatial_hash.hash_table),
+                        "Hash table not equal after loading from state dict.")
+        self.assertTrue(torch.allclose(self.spatial_hash.offset_table,
+                                       new_spatial_hash.offset_table),
+                        "Offset table not equal after loading from state dict.")
+        self.assertTrue(torch.allclose(self.spatial_hash.sparsity_encoding,
+                                       new_spatial_hash.sparsity_encoding),
+                        "Sparsity encoding not equal after loading from state dict.")
+
 
 if __name__ == '__main__':
     unittest.main()
```

