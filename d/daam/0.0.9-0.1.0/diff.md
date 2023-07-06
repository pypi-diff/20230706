# Comparing `tmp/daam-0.0.9.tar.gz` & `tmp/daam-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daam-0.0.9.tar", last modified: Wed Nov 30 18:18:52 2022, max compression
+gzip compressed data, was "daam-0.1.0.tar", last modified: Thu Jul  6 06:52:30 2023, max compression
```

## Comparing `daam-0.0.9.tar` & `daam-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 18:18:52.236800 daam-0.0.9/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     1066 2022-11-30 04:07:37.000000 daam-0.0.9/LICENSE
--rw-rw-r--   0 ralph     (1000) ralph     (1000)       25 2022-11-30 17:57:37.000000 daam-0.0.9/MANIFEST.in
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      284 2022-11-30 18:18:52.236800 daam-0.0.9/PKG-INFO
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     4042 2022-11-30 17:50:24.000000 daam-0.0.9/README.md
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 18:18:52.236800 daam-0.0.9/daam/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      112 2022-11-30 04:07:37.000000 daam-0.0.9/daam/__init__.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)       22 2022-11-30 18:18:29.000000 daam-0.0.9/daam/_version.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3350 2022-11-30 17:11:02.000000 daam-0.0.9/daam/evaluate.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)    13631 2022-11-30 17:50:24.000000 daam-0.0.9/daam/experiment.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3685 2022-11-30 17:10:08.000000 daam-0.0.9/daam/hook.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 18:18:52.236800 daam-0.0.9/daam/run/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2022-11-30 04:07:37.000000 daam-0.0.9/daam/run/__init__.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3274 2022-11-30 04:07:37.000000 daam-0.0.9/daam/run/evaluate.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     8895 2022-11-30 18:17:13.000000 daam-0.0.9/daam/run/generate.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)    12293 2022-11-30 18:17:10.000000 daam-0.0.9/daam/trace.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3536 2022-11-30 17:10:08.000000 daam-0.0.9/daam/utils.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 18:18:52.236800 daam-0.0.9/daam.egg-info/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      284 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/PKG-INFO
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      399 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/SOURCES.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        1 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/dependency_links.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)       48 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/entry_points.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      102 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/requires.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        5 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/top_level.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      102 2022-11-30 17:10:08.000000 daam-0.0.9/requirements.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)       38 2022-11-30 18:18:52.236800 daam-0.0.9/setup.cfg
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      602 2022-11-30 17:10:08.000000 daam-0.0.9/setup.py
+drwxr-xr-x   0 ralph     (1000) ralph     (1000)        0 2023-07-06 06:52:30.159692 daam-0.1.0/
+-rw-r--r--   0 ralph     (1000) ralph     (1000)     1066 2023-04-08 21:28:40.000000 daam-0.1.0/LICENSE
+-rw-r--r--   0 ralph     (1000) ralph     (1000)       25 2023-04-08 21:28:40.000000 daam-0.1.0/MANIFEST.in
+-rw-r--r--   0 ralph     (1000) ralph     (1000)      284 2023-07-06 06:52:30.159692 daam-0.1.0/PKG-INFO
+-rw-r--r--   0 ralph     (1000) ralph     (1000)     4530 2023-07-06 06:51:12.000000 daam-0.1.0/README.md
+drwxr-xr-x   0 ralph     (1000) ralph     (1000)        0 2023-07-06 06:52:30.149692 daam-0.1.0/daam/
+-rw-r--r--   0 ralph     (1000) ralph     (1000)      145 2023-04-08 21:28:40.000000 daam-0.1.0/daam/__init__.py
+-rw-r--r--   0 ralph     (1000) ralph     (1000)       22 2023-07-06 06:50:03.000000 daam-0.1.0/daam/_version.py
+-rw-r--r--   0 ralph     (1000) ralph     (1000)     3709 2023-04-08 21:28:40.000000 daam-0.1.0/daam/evaluate.py
+-rw-r--r--   0 ralph     (1000) ralph     (1000)    13524 2023-04-08 21:28:40.000000 daam-0.1.0/daam/experiment.py
+-rw-r--r--   0 ralph     (1000) ralph     (1000)     5773 2023-04-08 21:28:40.000000 daam-0.1.0/daam/heatmap.py
+-rw-r--r--   0 ralph     (1000) ralph     (1000)     3796 2023-06-08 03:58:59.000000 daam-0.1.0/daam/hook.py
+drwxr-xr-x   0 ralph     (1000) ralph     (1000)        0 2023-07-06 06:52:30.159692 daam-0.1.0/daam/run/
+-rw-r--r--   0 ralph     (1000) ralph     (1000)        0 2023-04-08 21:28:40.000000 daam-0.1.0/daam/run/__init__.py
+-rw-r--r--   0 ralph     (1000) ralph     (1000)     8326 2023-04-08 22:48:15.000000 daam-0.1.0/daam/run/demo.py
+-rw-r--r--   0 ralph     (1000) ralph     (1000)     3274 2023-04-08 21:28:40.000000 daam-0.1.0/daam/run/evaluate.py
+-rw-r--r--   0 ralph     (1000) ralph     (1000)     9652 2023-04-08 22:52:27.000000 daam-0.1.0/daam/run/generate.py
+-rw-r--r--   0 ralph     (1000) ralph     (1000)    10772 2023-06-08 03:58:59.000000 daam-0.1.0/daam/trace.py
+-rw-r--r--   0 ralph     (1000) ralph     (1000)     2891 2023-07-06 06:48:31.000000 daam-0.1.0/daam/utils.py
+drwxr-xr-x   0 ralph     (1000) ralph     (1000)        0 2023-07-06 06:52:30.149692 daam-0.1.0/daam.egg-info/
+-rw-r--r--   0 ralph     (1000) ralph     (1000)      284 2023-07-06 06:52:30.000000 daam-0.1.0/daam.egg-info/PKG-INFO
+-rw-r--r--   0 ralph     (1000) ralph     (1000)      432 2023-07-06 06:52:30.000000 daam-0.1.0/daam.egg-info/SOURCES.txt
+-rw-r--r--   0 ralph     (1000) ralph     (1000)        1 2023-07-06 06:52:30.000000 daam-0.1.0/daam.egg-info/dependency_links.txt
+-rw-r--r--   0 ralph     (1000) ralph     (1000)       79 2023-07-06 06:52:30.000000 daam-0.1.0/daam.egg-info/entry_points.txt
+-rw-r--r--   0 ralph     (1000) ralph     (1000)      122 2023-07-06 06:52:30.000000 daam-0.1.0/daam.egg-info/requires.txt
+-rw-r--r--   0 ralph     (1000) ralph     (1000)        5 2023-07-06 06:52:30.000000 daam-0.1.0/daam.egg-info/top_level.txt
+-rw-r--r--   0 ralph     (1000) ralph     (1000)      122 2023-07-06 06:49:34.000000 daam-0.1.0/requirements.txt
+-rw-r--r--   0 ralph     (1000) ralph     (1000)       38 2023-07-06 06:52:30.159692 daam-0.1.0/setup.cfg
+-rw-r--r--   0 ralph     (1000) ralph     (1000)      648 2023-04-08 21:28:40.000000 daam-0.1.0/setup.py
```

### Comparing `daam-0.0.9/LICENSE` & `daam-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `daam-0.0.9/README.md` & `daam-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # What the DAAM: Interpreting Stable Diffusion Using Cross Attention
 
-[![HF Spaces](https://img.shields.io/badge/HuggingFace%20Space-online-green.svg)](https://huggingface.co/spaces/tetrisd/Diffusion-Attentive-Attribution-Maps) [![Citation](https://img.shields.io/badge/Citation-arXiv-orange.svg)](https://gist.githubusercontent.com/daemon/1d126b5d72eb40300af5cccb92a232c6/raw/cd276203a7109bd9512f14afc86eebe8f13049ce/daam-citation.bib) [![PyPi version](https://badgen.net/pypi/v/daam?color=blue)](https://pypi.org/project/daam) [![Downloads](https://static.pepy.tech/badge/daam)](https://pepy.tech/project/daam)
+[![HF Spaces](https://img.shields.io/badge/HuggingFace%20Space-online-green.svg)](https://huggingface.co/spaces/tetrisd/Diffusion-Attentive-Attribution-Maps) [![Citation](https://img.shields.io/badge/Citation-arXiv-orange.svg)](https://gist.githubusercontent.com/daemon/c526f4f9ab2d5e946e6bae90a9a02571/raw/02dcc6cb09a39559b39449a7d27d3b950bec39bd/daam-citation.bib) [![PyPi version](https://badgen.net/pypi/v/daam?color=blue)](https://pypi.org/project/daam) [![Downloads](https://static.pepy.tech/badge/daam)](https://pepy.tech/project/daam)
 
 ![example image](example.jpg)
 
-### Updated to support Stable Diffusion V2!
+### Updated to support Diffusers 0.16.1!
 
 I regularly update this codebase. Please submit an issue if you have any questions.
 
 In [our paper](https://arxiv.org/abs/2210.04885), we propose diffusion attentive attribution maps (DAAM), a cross attention-based approach for interpreting Stable Diffusion.
 Check out our demo: https://huggingface.co/spaces/tetrisd/Diffusion-Attentive-Attribution-Maps.
-Our [documentation](https://castorini.github.io/daam/) is hosted by GitHub pages.
-See [1littlecoder's video](https://www.youtube.com/watch?v=J2WtkA1Xfew) for a code demonstration and Colab notebook of DAAM.
+See our [documentation](https://castorini.github.io/daam/), hosted by GitHub pages, and [our Colab notebook](https://colab.research.google.com/drive/1miGauqa07uHnDoe81NmbmtTtnupmlipv?usp=sharing), updated for v0.0.11.
 
-## Using DAAM as a CLI Utility
+## Getting Started
+First, install [PyTorch](https://pytorch.org) for your platform.
+Then, install DAAM with `pip install daam`, unless you want an editable version of the library, in which case do `git clone https://github.com/castorini/daam && pip install -e daam`.
+Finally, login using `huggingface-cli login` to get many stable diffusion models -- you'll need to get a token at [HuggingFace.co](https://huggingface.co/).
+
+### Running the Website Demo
+Simply run `daam-demo` in a shell and navigate to http://localhost:8080.
+The same demo as the one on HuggingFace Spaces will show up.
 
+### Using DAAM as a CLI Utility
 DAAM comes with a simple generation script for people who want to quickly try it out.
-First, install [PyTorch](https://pytorch.org) for your platform.
-Then, install DAAM with `pip install daam`.
-Now, try running
+Try running
 ```bash
 $ mkdir -p daam-test && cd daam-test
 $ daam "A dog running across the field."
 $ ls
-a.heat_map.png    generation.pt         output.png  seed.txt
-dog.heat_map.png  jumping.heat_map.png  prompt.txt
+a.heat_map.png    field.heat_map.png    generation.pt   output.png  seed.txt
+dog.heat_map.png  running.heat_map.png  prompt.txt
 ```
 Your current working directory will now contain the generated image as `output.png` and a DAAM map for every word, as well as some auxiliary data.
 You can see more options for `daam` by running `daam -h`.
 
-## Using DAAM as a Library
-
-First, install [PyTorch <= 1.13.0](https://pytorch.org) for your platform.
-Then, install DAAM with `pip install daam`. If you want an editable version, then do `git clone https://github.com/castorini/daam && pip install -e daam`.
+### Using DAAM as a Library
 
-Using DAAM as a library is easy.
-You'll first need to login using `huggingface-cli login` to get many stable diffusion models.
-Next, import and call DAAM as follows:
+Import and use DAAM as follows:
 
 ```python
-from daam import trace, set_seed, plot_overlay_heat_map, expand_image
+from daam import trace, set_seed
 from diffusers import StableDiffusionPipeline
 from matplotlib import pyplot as plt
 import torch
 
 
 model_id = 'stabilityai/stable-diffusion-2-base'
 device = 'cuda'
@@ -54,16 +54,16 @@
 prompt = 'A dog runs across the field'
 gen = set_seed(0)  # for reproducibility
 
 with torch.cuda.amp.autocast(dtype=torch.float16), torch.no_grad():
     with trace(pipe) as tc:
         out = pipe(prompt, num_inference_steps=30, generator=gen)
         heat_map = tc.compute_global_heat_map()
-        heat_map = expand_image(heat_map.compute_word_heat_map('dog'))
-        plot_overlay_heat_map(out.images[0], heat_map)
+        heat_map = heat_map.compute_word_heat_map('dog')
+        heat_map.plot_overlay(out.images[0])
         plt.show()
 ```
 
 You can also serialize and deserialize the DAAM maps pretty easily:
 
 ```python
 from daam import GenerationExperiment, trace
@@ -73,19 +73,26 @@
     exp = tc.to_experiment('experiment-dir')
     exp.save()  # experiment-dir now contains all the data and heat maps
 
 exp = GenerationExperiment.load('experiment-dir')  # load the experiment
 ```
 
 We'll continue adding docs.
-In the meantime, check out the `GenerationExperiment`, `HeatMap`, and `DiffusionHeatMapHooker` classes, as well as the `daam/run/*.py` example scripts.
+In the meantime, check out the `GenerationExperiment`, `GlobalHeatMap`, and `DiffusionHeatMapHooker` classes, as well as the `daam/run/*.py` example scripts.
 Our datasets are here: https://git.uwaterloo.ca/r33tang/daam-data
 
+## See Also
+- [DAAM-i2i](https://github.com/RishiDarkDevil/daam-i2i), an extension of DAAM to image-to-image attribution.
+
+- [Furkan's video](https://www.youtube.com/watch?v=XiKyEKJrTLQ) on easily getting started with DAAM.
+
+- [1littlecoder's video](https://www.youtube.com/watch?v=J2WtkA1Xfew) for a code demonstration and Colab notebook of an older version of DAAM.
+
 ## Citation
 ```
 @article{tang2022daam,
   title={What the {DAAM}: Interpreting Stable Diffusion Using Cross Attention},
-  author={Tang, Raphael and Pandey, Akshat and Jiang, Zhiying and Yang, Gefei and Kumar, Karun and Lin, Jimmy and Ture, Ferhan},
+  author={Tang, Raphael and Liu, Linqing and Pandey, Akshat and Jiang, Zhiying and Yang, Gefei and Kumar, Karun and Stenetorp, Pontus and Lin, Jimmy and Ture, Ferhan},
   journal={arXiv:2210.04885},
   year={2022}
 }
 ```
```

### Comparing `daam-0.0.9/daam/evaluate.py` & `daam-0.1.0/daam/evaluate.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,41 @@
 from scipy.optimize import linear_sum_assignment
 import PIL.Image as Image
 import numpy as np
 import torch
 import torch.nn.functional as F
 
 
-__all__ = ['compute_iou', 'MeanEvaluator', 'load_mask']
+__all__ = ['compute_iou', 'MeanEvaluator', 'load_mask', 'compute_ioa']
 
 
 def compute_iou(a: torch.Tensor, b: torch.Tensor) -> float:
     if a.shape[0] != b.shape[0]:
         a = F.interpolate(a.unsqueeze(0).unsqueeze(0).float(), size=b.shape, mode='bicubic').squeeze()
         a[a < 1] = 0
         a[a >= 1] = 1
 
     intersection = (a * b).sum()
     union = a.sum() + b.sum() - intersection
 
     return (intersection / (union + 1e-8)).item()
 
 
+def compute_ioa(a: torch.Tensor, b: torch.Tensor) -> float:
+    if a.shape[0] != b.shape[0]:
+        a = F.interpolate(a.unsqueeze(0).unsqueeze(0).float(), size=b.shape, mode='bicubic').squeeze()
+        a[a < 1] = 0
+        a[a >= 1] = 1
+
+    intersection = (a * b).sum()
+    area = a.sum()
+
+    return (intersection / (area + 1e-8)).item()
+
+
 def load_mask(path: str) -> torch.Tensor:
     mask = np.array(Image.open(path))
     mask = torch.from_numpy(mask).float()[:, :, 3]  # use alpha channel
     mask = (mask > 0).float()
 
     return mask
```

### Comparing `daam-0.0.9/daam/experiment.py` & `daam-0.1.0/daam/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import json
 
 from transformers import PreTrainedTokenizer, AutoTokenizer
 import PIL.Image
 import numpy as np
 import torch
 
+from .utils import auto_autocast
 from .evaluate import load_mask
-from .utils import plot_overlay_heat_map, expand_image
 
 
 __all__ = ['GenerationExperiment', 'COCO80_LABELS', 'COCOSTUFF27_LABELS', 'COCO80_INDICES', 'build_word_list_coco80']
 
 
 COCO80_LABELS: List[str] = [
     'person', 'bicycle', 'car', 'motorcycle', 'airplane', 'bus', 'train', 'truck', 'boat', 'traffic light',
@@ -125,16 +125,16 @@
     def nsfw(self) -> bool:
         return np.sum(np.array(self.image)) == 0
 
     def heat_map(self, tokenizer: AutoTokenizer = None):
         if tokenizer is None:
             tokenizer = self.tokenizer
 
-        from daam import HeatMap
-        return HeatMap(tokenizer, self.prompt, self.global_heat_map)
+        from daam import GlobalHeatMap
+        return GlobalHeatMap(tokenizer, self.prompt, self.global_heat_map)
 
     def clear_checkpoint(self):
         path = self if isinstance(self, Path) else self.path
 
         (path / 'generation.pt').unlink(missing_ok=True)
 
     def save(self, path: str = None, heat_maps: bool = True, tokenizer: AutoTokenizer = None):
@@ -225,24 +225,23 @@
             self,
             word: str,
             tokenizer: PreTrainedTokenizer = None,
             crop: int = None,
             output_prefix: str = '',
             absolute: bool = False
     ) -> Path:
-        from .trace import HeatMap  # because of cyclical import
+        from .trace import GlobalHeatMap  # because of cyclical import
 
         if tokenizer is None:
             tokenizer = self.tokenizer
 
-        with torch.cuda.amp.autocast(dtype=torch.float32):
-            heat_map = HeatMap(tokenizer, self.prompt, self.global_heat_map)
-            heat_map = expand_image(heat_map.compute_word_heat_map(word), absolute=absolute, out=self.image.size[0])
+        with auto_autocast(dtype=torch.float32):
             path = self.path / self.subtype / f'{output_prefix}{word.lower()}.heat_map.png'
-            plot_overlay_heat_map(self.image, heat_map, word, path, crop=crop, color_normalize=not absolute)
+            heat_map = GlobalHeatMap(tokenizer, self.prompt, self.global_heat_map)
+            heat_map.compute_word_heat_map(word).expand_as(self.image, color_normalize=not absolute, out_file=path, plot=True)
 
         return path
 
     def save_all_heat_maps(self, tokenizer: PreTrainedTokenizer = None, crop: int = None) -> Dict[str, Path]:
         path_map = {}
 
         if tokenizer is None:
```

### Comparing `daam-0.0.9/daam/hook.py` & `daam-0.1.0/daam/hook.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Generic, TypeVar, Callable, Union, Any
 import functools
 import itertools
 
 from diffusers import UNet2DConditionModel
-from diffusers.models.attention import CrossAttention
+from diffusers.models.attention_processor import Attention
 import torch.nn as nn
 
 
 __all__ = ['ObjectHooker', 'ModuleLocator', 'AggregateHooker', 'UNetCrossAttentionLocator']
 
 
 ModuleType = TypeVar('ModuleType')
@@ -78,38 +78,39 @@
         for h in self.module:
             h.unhook()
 
     def register_hook(self, hook: ObjectHooker):
         self.module.append(hook)
 
 
-class UNetCrossAttentionLocator(ModuleLocator[CrossAttention]):
-    def __init__(self, restrict: bool = None):
+class UNetCrossAttentionLocator(ModuleLocator[Attention]):
+    def __init__(self, restrict: bool = None, locate_middle_block: bool = False):
         self.restrict = restrict
         self.layer_names = []
+        self.locate_middle_block = locate_middle_block
 
-    def locate(self, model: UNet2DConditionModel) -> List[CrossAttention]:
+    def locate(self, model: UNet2DConditionModel) -> List[Attention]:
         """
         Locate all cross-attention modules in a UNet2DConditionModel.
 
         Args:
             model (`UNet2DConditionModel`): The model to locate the cross-attention modules in.
 
         Returns:
-            `List[CrossAttention]`: The list of cross-attention modules.
+            `List[Attention]`: The list of cross-attention modules.
         """
         self.layer_names.clear()
         blocks_list = []
         up_names = ['up'] * len(model.up_blocks)
         down_names = ['down'] * len(model.up_blocks)
 
-        # The middle block was not found to be useful.
         for unet_block, name in itertools.chain(
                 zip(model.up_blocks, up_names),
-                zip(model.down_blocks, down_names)
+                zip(model.down_blocks, down_names),
+                zip([model.mid_block], ['mid']) if self.locate_middle_block else [],
         ):
             if 'CrossAttn' in unet_block.__class__.__name__:
                 blocks = []
 
                 for spatial_transformer in unet_block.attentions:
                     for transformer_block in spatial_transformer.transformer_blocks:
                         blocks.append(transformer_block.attn2)
```

### Comparing `daam-0.0.9/daam/run/evaluate.py` & `daam-0.1.0/daam/run/evaluate.py`

 * *Files identical despite different names*

### Comparing `daam-0.0.9/daam/run/generate.py` & `daam-0.1.0/daam/run/generate.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,47 +11,52 @@
 from tqdm import tqdm
 import inflect
 import numpy as np
 import torch
 
 from daam import trace
 from daam.experiment import GenerationExperiment, build_word_list_coco80
-from daam.utils import set_seed, cached_nlp
+from daam.utils import set_seed, cached_nlp, auto_device, auto_autocast
 
 
 def main():
-    actions = ['quickgen', 'prompt', 'coco', 'template', 'cconj', 'coco-unreal', 'stdin']
+    actions = ['quickgen', 'prompt', 'coco', 'template', 'cconj', 'coco-unreal', 'stdin', 'regenerate']
     model_id_map = {
         'v1': 'runwayml/stable-diffusion-v1-5',
         'v2-base': 'stabilityai/stable-diffusion-2-base',
-        'v2-large': 'stabilityai/stable-diffusion-2'
+        'v2-large': 'stabilityai/stable-diffusion-2',
+        'v2-1-base': 'stabilityai/stable-diffusion-2-1-base',
+        'v2-1-large': 'stabilityai/stable-diffusion-2-1'
     }
 
     parser = argparse.ArgumentParser()
     parser.add_argument('prompt', nargs='?', type=str)
     parser.add_argument('--action', '-a', type=str, choices=actions, default=actions[0])
     parser.add_argument('--low-memory', action='store_true')
-    parser.add_argument('--model', type=str, default='v2-base', choices=list(model_id_map.keys()))
+    parser.add_argument('--model', type=str, default='v2-1-base', choices=list(model_id_map.keys()))
     parser.add_argument('--output-folder', '-o', type=str)
     parser.add_argument('--input-folder', '-i', type=str, default='input')
     parser.add_argument('--seed', '-s', type=int, default=0)
     parser.add_argument('--gen-limit', type=int, default=1000)
     parser.add_argument('--template', type=str, default='{numeral} {noun}')
     parser.add_argument('--template-data-file', '-tdf', type=str, default='template.tsv')
-    parser.add_argument('--regenerate', action='store_true')
     parser.add_argument('--seed-offset', type=int, default=0)
-    parser.add_argument('--num-timesteps', type=int, default=30)
+    parser.add_argument('--num-timesteps', '-n', type=int, default=30)
     parser.add_argument('--all-heads', action='store_true')
     parser.add_argument('--word', type=str)
     parser.add_argument('--random-seed', action='store_true')
+    parser.add_argument('--truth-only', action='store_true')
+    parser.add_argument('--save-heads', action='store_true')
+    parser.add_argument('--load-heads', action='store_true')
     args = parser.parse_args()
 
     eng = inflect.engine()
     args.lemma = cached_nlp(args.word)[0].lemma_ if args.word else None
     model_id = model_id_map[args.model]
+    seeds = []
 
     if args.action.startswith('coco'):
         with (Path(args.input_folder) / 'captions_val2014.json').open() as f:
             captions = json.load(f)['annotations']
 
         random.shuffle(captions)
         new_captions = []
@@ -141,14 +146,27 @@
             prompt = f'{a1} {w1} and {a2} {w2}'
             prompts.append((prompt_id, prompt))
     elif args.action == 'quickgen':
         if args.output_folder is None:
             args.output_folder = '.'
 
         prompts = [('.', args.prompt)]
+    elif args.action == 'regenerate':
+        prompts = []
+
+        for exp_folder in Path(args.input_folder).iterdir():
+            if not GenerationExperiment.contains_truth_mask(exp_folder) and args.truth_only:
+                continue
+
+            prompt = GenerationExperiment.read_prompt(exp_folder)
+            prompts.append((exp_folder.name, prompt))
+            seeds.append(GenerationExperiment.read_seed(exp_folder))
+
+        if args.output_folder is None:
+            args.output_folder = args.input_folder
     else:
         prompts = [('prompt', input('> '))]
 
     if args.output_folder is None:
         args.output_folder = 'output'
 
     new_prompts = []
@@ -171,35 +189,34 @@
             if found:
                 new_prompts.append((prompt_id, prompt))
 
         prompts = new_prompts
 
     prompts = prompts[:args.gen_limit]
     pipe = StableDiffusionPipeline.from_pretrained(model_id, use_auth_token=True)
-    pipe = pipe.to('cuda')
+    pipe = auto_device(pipe)
 
-    with torch.cuda.amp.autocast(dtype=torch.float16), torch.no_grad():
-        for prompt_id, prompt in tqdm(prompts):
+    with auto_autocast(dtype=torch.float16), torch.no_grad():
+        for gen_idx, (prompt_id, prompt) in enumerate(tqdm(prompts)):
             seed = int(time.time()) if args.random_seed else args.seed
-            gen = set_seed(seed)  # Uncomment this for seed fix
             prompt = prompt.replace(',', ' ,').replace('.', ' .').strip()
 
+            if seeds and gen_idx < len(seeds):
+                seed = seeds[gen_idx]
+
+            gen = set_seed(seed)
+
             if args.action == 'cconj':
                 seed = int(prompt_id.split('-')[1]) + args.seed_offset
                 gen = set_seed(seed)
 
             prompt_id = str(prompt_id)
 
-            if args.regenerate and not GenerationExperiment.contains_truth_mask(args.output_folder, prompt_id):
-                continue
-            elif args.regenerate:
-                print(f'Regenerating {prompt_id}')
-
-            with trace(pipe, low_memory=args.low_memory) as tc:
-                out = pipe(prompt, num_inference_steps=args.num_timesteps, generator=gen)
+            with trace(pipe, low_memory=args.low_memory, save_heads=args.save_heads, load_heads=args.load_heads) as tc:
+                out = pipe(prompt, num_inference_steps=args.num_timesteps, generator=gen, callback=tc.time_callback)
                 exp = tc.to_experiment(args.output_folder, id=prompt_id, seed=seed)
                 exp.save(args.output_folder, heat_maps=args.action == 'quickgen')
 
                 if args.all_heads:
                     exp.clear_checkpoint()
 
                 for word in prompt.split():
```

### Comparing `daam-0.0.9/daam/trace.py` & `daam-0.1.0/daam/trace.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,67 @@
-from collections import defaultdict
 from pathlib import Path
-from typing import List, Type, Any, Dict, Tuple, Set, Union
+from typing import List, Type, Any, Dict, Tuple, Union
 import math
 
 from diffusers import StableDiffusionPipeline
-from diffusers.models.attention import CrossAttention
+from diffusers.models.attention_processor import Attention
 import numpy as np
 import PIL.Image as Image
 import torch
 import torch.nn.functional as F
 
+from .utils import cache_dir, auto_autocast
 from .experiment import GenerationExperiment
+from .heatmap import RawHeatMapCollection, GlobalHeatMap
 from .hook import ObjectHooker, AggregateHooker, UNetCrossAttentionLocator
-from .utils import compute_token_merge_indices
 
 
-__all__ = ['trace', 'DiffusionHeatMapHooker', 'HeatMap', 'RawHeatMapCollection']
-
-
-class HeatMap:
-    def __init__(self, tokenizer: Any, prompt: str, heat_maps: torch.Tensor):
-        self.tokenizer = tokenizer
-        self.heat_maps = heat_maps
-        self.prompt = prompt
-
-    def compute_word_heat_map(self, word: str, word_idx: int = None) -> torch.Tensor:
-        merge_idxs = compute_token_merge_indices(self.tokenizer, self.prompt, word, word_idx)
-        return self.heat_maps[merge_idxs].mean(0)
-
-
-RawHeatMapKey = Tuple[int, int, int]  # factor, layer, head
-
-
-class RawHeatMapCollection:
-    def __init__(self):
-        self.ids_to_heatmaps: Dict[RawHeatMapKey, torch.Tensor] = defaultdict(lambda: 0.0)
-        self.ids_to_num_maps: Dict[RawHeatMapKey, int] = defaultdict(lambda: 0)
-
-    def update(self, factor: int, layer_idx: int, head_idx: int, heatmap: torch.Tensor):
-        with torch.cuda.amp.autocast(dtype=torch.float32):
-            self.ids_to_heatmaps[(factor, layer_idx, head_idx)] = self.ids_to_heatmaps[(factor, layer_idx, head_idx)] + heatmap
-
-    def factors(self) -> Set[int]:
-        return set(key[0] for key in self.ids_to_heatmaps.keys())
-
-    def layers(self) -> Set[int]:
-        return set(key[1] for key in self.ids_to_heatmaps.keys())
-
-    def heads(self) -> Set[int]:
-        return set(key[2] for key in self.ids_to_heatmaps.keys())
-
-    def __iter__(self):
-        return iter(self.ids_to_heatmaps.items())
-
-    def clear(self):
-        self.ids_to_heatmaps.clear()
-        self.ids_to_num_maps.clear()
+__all__ = ['trace', 'DiffusionHeatMapHooker', 'GlobalHeatMap']
 
 
 class DiffusionHeatMapHooker(AggregateHooker):
-    def __init__(self, pipeline: StableDiffusionPipeline, low_memory: bool = False):
+    def __init__(
+            self,
+            pipeline:
+            StableDiffusionPipeline,
+            low_memory: bool = False,
+            load_heads: bool = False,
+            save_heads: bool = False,
+            data_dir: str = None
+    ):
         self.all_heat_maps = RawHeatMapCollection()
         h = (pipeline.unet.config.sample_size * pipeline.vae_scale_factor)
         self.latent_hw = 4096 if h == 512 else 9216  # 64x64 or 96x96 depending on if it's 2.0-v or 2.0
-        self.locator = UNetCrossAttentionLocator(restrict={0} if low_memory else None)
+        locate_middle = load_heads or save_heads
+        self.locator = UNetCrossAttentionLocator(restrict={0} if low_memory else None, locate_middle_block=locate_middle)
         self.last_prompt: str = ''
         self.last_image: Image = None
+        self.time_idx = 0
+        self._gen_idx = 0
 
         modules = [
             UNetCrossAttentionHooker(
                 x,
-                self.all_heat_maps,
+                self,
                 layer_idx=idx,
-                latent_hw=self.latent_hw
+                latent_hw=self.latent_hw,
+                load_heads=load_heads,
+                save_heads=save_heads,
+                data_dir=data_dir
             ) for idx, x in enumerate(self.locator.locate(pipeline.unet))
         ]
 
         modules.append(PipelineHooker(pipeline, self))
 
         super().__init__(modules)
         self.pipe = pipeline
 
+    def time_callback(self, *args, **kwargs):
+        self.time_idx += 1
+
     @property
     def layer_names(self):
         return self.locator.layer_names
 
     def to_experiment(self, path, seed=None, id='.', subtype='.', **compute_kwargs):
         # type: (Union[Path, str], int, str, str, Dict[str, Any]) -> GenerationExperiment
         """Exports the last generation call to a serializable generation experiment."""
@@ -97,15 +74,15 @@
             id=id,
             subtype=subtype,
             path=path,
             tokenizer=self.pipe.tokenizer,
         )
 
     def compute_global_heat_map(self, prompt=None, factors=None, head_idx=None, layer_idx=None, normalize=False):
-        # type: (str, List[float], int, int, bool) -> HeatMap
+        # type: (str, List[float], int, int, bool) -> GlobalHeatMap
         """
         Compute the global heat map for the given prompt, aggregating across time (inference steps) and space (different
         spatial transformer block heat maps).
 
         Args:
             prompt: The prompt to compute the heat map for. If none, uses the last prompt that was used for generation.
             factors: Restrict the application to heat maps with spatial factors in this set. If `None`, use all sizes.
@@ -124,15 +101,15 @@
             factors = {0, 1, 2, 4, 8, 16, 32, 64}
         else:
             factors = set(factors)
 
         all_merges = []
         x = int(np.sqrt(self.latent_hw))
 
-        with torch.cuda.amp.autocast(dtype=torch.float32):
+        with auto_autocast(dtype=torch.float32):
             for (factor, layer, head), heat_map in heat_maps:
                 if factor in factors and (head_idx is None or head_idx == head) and (layer_idx is None or layer_idx == layer):
                     heat_map = heat_map.unsqueeze(1)
                     # The clamping fixes undershoot.
                     all_merges.append(F.interpolate(heat_map, size=(x, x), mode='bicubic').clamp_(min=0))
 
             try:
@@ -145,15 +122,15 @@
 
             maps = maps.mean(0)[:, 0]
             maps = maps[:len(self.pipe.tokenizer.tokenize(prompt)) + 2]  # 1 for SOS and 1 for padding
 
             if normalize:
                 maps = maps / (maps[1:-1].sum(0, keepdim=True) + 1e-6)  # drop out [SOS] and [PAD] for proper probabilities
 
-        return HeatMap(self.pipe.tokenizer, prompt, maps)
+        return GlobalHeatMap(self.pipe.tokenizer, prompt, maps)
 
 
 class PipelineHooker(ObjectHooker[StableDiffusionPipeline]):
     def __init__(self, pipeline: StableDiffusionPipeline, parent_trace: 'trace'):
         super().__init__(pipeline)
         self.heat_maps = parent_trace.all_heat_maps
         self.parent_trace = parent_trace
@@ -180,29 +157,44 @@
         return ret
 
     def _hook_impl(self):
         self.monkey_patch('run_safety_checker', self._hooked_run_safety_checker)
         self.monkey_patch('_encode_prompt', self._hooked_encode_prompt)
 
 
-class UNetCrossAttentionHooker(ObjectHooker[CrossAttention]):
+class UNetCrossAttentionHooker(ObjectHooker[Attention]):
     def __init__(
             self,
-            module: CrossAttention,
-            heat_maps: 'RawHeatMapCollection',
+            module: Attention,
+            parent_trace: 'trace',
             context_size: int = 77,
             layer_idx: int = 0,
-            latent_hw: int = 9216
+            latent_hw: int = 9216,
+            load_heads: bool = False,
+            save_heads: bool = False,
+            data_dir: Union[str, Path] = None,
     ):
         super().__init__(module)
-        self.heat_maps = heat_maps
+        self.heat_maps = parent_trace.all_heat_maps
         self.context_size = context_size
         self.layer_idx = layer_idx
         self.latent_hw = latent_hw
 
+        self.load_heads = load_heads
+        self.save_heads = save_heads
+        self.trace = parent_trace
+
+        if data_dir is not None:
+            data_dir = Path(data_dir)
+        else:
+            data_dir = cache_dir() / 'heads'
+
+        self.data_dir = data_dir
+        self.data_dir.mkdir(parents=True, exist_ok=True)
+
     @torch.no_grad()
     def _unravel_attn(self, x):
         # type: (torch.Tensor) -> torch.Tensor
         # x shape: (heads, height * width, tokens)
         """
         Unravels the attention, returning it as a collection of heat maps.
 
@@ -213,96 +205,85 @@
         Returns:
             `List[Tuple[int, torch.Tensor]]`: the list of heat maps across heads.
         """
         h = w = int(math.sqrt(x.size(1)))
         maps = []
         x = x.permute(2, 0, 1)
 
-        with torch.cuda.amp.autocast(dtype=torch.float32):
+        with auto_autocast(dtype=torch.float32):
             for map_ in x:
                 map_ = map_.view(map_.size(0), h, w)
                 map_ = map_[map_.size(0) // 2:]  # Filter out unconditional
                 maps.append(map_)
 
         maps = torch.stack(maps, 0)  # shape: (tokens, heads, height, width)
         return maps.permute(1, 0, 2, 3).contiguous()  # shape: (heads, tokens, height, width)
 
-    def _hooked_sliced_attention(hk_self, self, query, key, value, sequence_length, dim):
-        batch_size_attention = query.shape[0]
-        hidden_states = torch.zeros(
-            (batch_size_attention, sequence_length, dim // self.heads), device=query.device, dtype=query.dtype
-        )
-        slice_size = self._slice_size if self._slice_size is not None else hidden_states.shape[0]
-        for i in range(hidden_states.shape[0] // slice_size):
-            start_idx = i * slice_size
-            end_idx = (i + 1) * slice_size
-            attn_slice = torch.baddbmm(
-                torch.empty(slice_size, query.shape[1], key.shape[1], dtype=query.dtype, device=query.device),
-                query[start_idx:end_idx],
-                key[start_idx:end_idx].transpose(-1, -2),
-                beta=0,
-                alpha=self.scale,
-            )
-            attn_slice = attn_slice.softmax(dim=-1)
-            factor = int(math.sqrt(hk_self.latent_hw // attn_slice.shape[1]))
-
-            if attn_slice.shape[-1] == hk_self.context_size:
-                # shape: (batch_size, 64 // factor, 64 // factor, 77)
-                maps = hk_self._unravel_attn(attn_slice)
-
-                for head_idx, heatmap in enumerate(maps):
-                    hk_self.heat_maps.update(factor, hk_self.layer_idx, head_idx, heatmap)
-
-            attn_slice = torch.bmm(attn_slice, value[start_idx:end_idx])
-
-            hidden_states[start_idx:end_idx] = attn_slice
-
-        # reshape hidden_states
-        hidden_states = self.reshape_batch_dim_to_heads(hidden_states)
-        return hidden_states
-
-    def _hooked_attention(hk_self, self, query, key, value):
-        """
-        Monkey-patched version of :py:func:`.CrossAttention._attention` to capture attentions and aggregate them.
+    def _save_attn(self, attn_slice: torch.Tensor):
+        torch.save(attn_slice, self.data_dir / f'{self.trace._gen_idx}.pt')
 
-        Args:
-            hk_self (`UNetCrossAttentionHooker`): pointer to the hook itself.
-            self (`CrossAttention`): pointer to the module.
-            query (`torch.Tensor`): the query tensor.
-            key (`torch.Tensor`): the key tensor.
-            value (`torch.Tensor`): the value tensor.
-        """
+    def _load_attn(self) -> torch.Tensor:
+        return torch.load(self.data_dir / f'{self.trace._gen_idx}.pt')
 
-        attention_scores = torch.baddbmm(
-            torch.empty(query.shape[0], query.shape[1], key.shape[1], dtype=query.dtype, device=query.device),
-            query,
-            key.transpose(-1, -2),
-            beta=0,
-            alpha=self.scale,
-        )
-        attn_slice = attention_scores.softmax(dim=-1)
-        factor = int(math.sqrt(hk_self.latent_hw // attn_slice.shape[1]))
+    def __call__(
+            self,
+            attn: Attention,
+            hidden_states,
+            encoder_hidden_states=None,
+            attention_mask=None,
+    ):
+        """Capture attentions and aggregate them."""
+        batch_size, sequence_length, _ = hidden_states.shape
+        attention_mask = attn.prepare_attention_mask(attention_mask, sequence_length, batch_size)
+        query = attn.to_q(hidden_states)
+
+        if encoder_hidden_states is None:
+            encoder_hidden_states = hidden_states
+        elif attn.norm_cross is not None:
+            encoder_hidden_states = attn.norm_cross(encoder_hidden_states)
+
+        key = attn.to_k(encoder_hidden_states)
+        value = attn.to_v(encoder_hidden_states)
+
+        query = attn.head_to_batch_dim(query)
+        key = attn.head_to_batch_dim(key)
+        value = attn.head_to_batch_dim(value)
+
+        attention_probs = attn.get_attention_scores(query, key, attention_mask)
+
+        # DAAM save heads
+        if self.save_heads:
+            self._save_attn(attention_probs)
+        elif self.load_heads:
+            attention_probs = self._load_attn()
+
+        # compute shape factor
+        factor = int(math.sqrt(self.latent_hw // attention_probs.shape[1]))
+        self.trace._gen_idx += 1
 
-        if attn_slice.shape[-1] == hk_self.context_size:
+        # skip if too large
+        if attention_probs.shape[-1] == self.context_size and factor != 8:
             # shape: (batch_size, 64 // factor, 64 // factor, 77)
-            maps = hk_self._unravel_attn(attn_slice)
+            maps = self._unravel_attn(attention_probs)
 
             for head_idx, heatmap in enumerate(maps):
-                hk_self.heat_maps.update(factor, hk_self.layer_idx, head_idx, heatmap)
+                self.heat_maps.update(factor, self.layer_idx, head_idx, heatmap)
+
+        hidden_states = torch.bmm(attention_probs, value)
+        hidden_states = attn.batch_to_head_dim(hidden_states)
 
-        # compute attention output
-        hidden_states = torch.bmm(attn_slice, value)
+        # linear proj
+        hidden_states = attn.to_out[0](hidden_states)
+        # dropout
+        hidden_states = attn.to_out[1](hidden_states)
 
-        # reshape hidden_states
-        hidden_states = self.reshape_batch_dim_to_heads(hidden_states)
         return hidden_states
 
     def _hook_impl(self):
-        self.monkey_patch('_attention', self._hooked_attention)
-        self.monkey_patch('_sliced_attention', self._hooked_sliced_attention)
+        self.module.set_processor(self)
 
     @property
     def num_heat_maps(self):
         return len(next(iter(self.heat_maps.values())))
 
 
 trace: Type[DiffusionHeatMapHooker] = DiffusionHeatMapHooker
```

### Comparing `daam-0.0.9/daam/utils.py` & `daam-0.1.0/daam/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,43 @@
 from functools import lru_cache
 from pathlib import Path
+import os
+import sys
 import random
+from typing import TypeVar
 
 import PIL.Image
 import matplotlib.pyplot as plt
 import numpy as np
 import spacy
 import torch
 import torch.nn.functional as F
 
 
-__all__ = ['expand_image', 'set_seed', 'compute_token_merge_indices', 'plot_overlay_heat_map', 'plot_mask_heat_map',
-           'cached_nlp']
+__all__ = ['set_seed', 'compute_token_merge_indices', 'plot_mask_heat_map', 'cached_nlp', 'cache_dir', 'auto_device', 'auto_autocast']
 
 
-def expand_image(im: torch.Tensor, out: int = 512, absolute: bool = False, threshold: float = None) -> torch.Tensor:
-    im = im.unsqueeze(0).unsqueeze(0)
-    im = F.interpolate(im.float().detach(), size=(out, out), mode='bicubic')
+T = TypeVar('T')
 
-    if not absolute:
-        im = (im - im.min()) / (im.max() - im.min() + 1e-8)
 
-    if threshold:
-        im = (im > threshold).float()
+def auto_device(obj: T = torch.device('cpu')) -> T:
+    if isinstance(obj, torch.device):
+        return torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
-    im = im.cpu().detach()
+    if torch.cuda.is_available():
+        return obj.to('cuda')
 
-    return im.squeeze()
+    return obj
 
 
-def plot_overlay_heat_map(im, heat_map, word=None, out_file=None, crop=None, color_normalize=True):
-    # type: (PIL.Image.Image | np.ndarray, torch.Tensor, str, Path, int, bool) -> None
-    plt.clf()
-    plt.rcParams.update({'font.size': 24})
+def auto_autocast(*args, **kwargs):
+    if not torch.cuda.is_available():
+        kwargs['enabled'] = False
 
-    with torch.cuda.amp.autocast(dtype=torch.float32):
-        im = np.array(im)
-
-        if crop is not None:
-            heat_map = heat_map.squeeze()[crop:-crop, crop:-crop]
-            im = im[crop:-crop, crop:-crop]
-
-        if color_normalize:
-            plt.imshow(heat_map.squeeze().cpu().numpy(), cmap='jet')
-        else:
-            heat_map = heat_map.clamp_(min=0, max=1)
-            plt.imshow(heat_map.squeeze().cpu().numpy(), cmap='jet', vmin=0.0, vmax=1.0)
-
-        im = torch.from_numpy(im).float() / 255
-        im = torch.cat((im, (1 - heat_map.unsqueeze(-1))), dim=-1)
-        plt.imshow(im)
-
-        if word is not None:
-            plt.title(word)
-
-        if out_file is not None:
-            plt.savefig(out_file)
+    return torch.cuda.amp.autocast(*args, **kwargs)
 
 
 def plot_mask_heat_map(im: PIL.Image.Image, heat_map: torch.Tensor, threshold: float = 0.4):
     im = torch.from_numpy(np.array(im)).float() / 255
     mask = (heat_map.squeeze() > threshold).float()
     im = im * mask.unsqueeze(-1)
     plt.imshow(im)
@@ -67,65 +45,61 @@
 
 def set_seed(seed: int) -> torch.Generator:
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)
 
-    gen = torch.Generator(device='cuda')
+    gen = torch.Generator(device=auto_device())
     gen.manual_seed(seed)
 
     return gen
 
 
-def compute_token_merge_indices(tokenizer, prompt: str, word: str, word_idx: int = None):
-    prompt = prompt.lower()
-    tokens = tokenizer.tokenize(prompt)
-    word = word.lower()
-    merge_idxs = []
-    curr_idx = 0
-    curr_token = ''
+def cache_dir() -> Path:
+    # *nix
+    if os.name == 'posix' and sys.platform != 'darwin':
+        xdg = os.environ.get('XDG_CACHE_HOME', os.path.expanduser('~/.cache'))
+        return Path(xdg, 'daam')
+    elif sys.platform == 'darwin':
+        # Mac OS
+        return Path(os.path.expanduser('~'), 'Library/Caches/daam')
+    else:
+        # Windows
+        local = os.environ.get('LOCALAPPDATA', None) \
+                or os.path.expanduser('~\\AppData\\Local')
+        return Path(local, 'daam')
+
 
+def compute_token_merge_indices(tokenizer, prompt: str, word: str, word_idx: int = None, offset_idx: int = 0):
+    merge_idxs = []
+    tokens = tokenizer.tokenize(prompt.lower())
     if word_idx is None:
-        try:
-            word_idx = prompt.split().index(word)
-        except:
-            for punct in ('.', ',', '!', '?'):
-                try:
-                    word_idx = prompt.split().index(word + punct)
-                    break
-                except:
-                    pass
-
-        if word_idx is None:
-            raise ValueError(f'Couldn\'t find "{word}" in "{prompt}"')
-
-    for idx, token in enumerate(tokens):
-        merge_idxs.append(idx)
-
-        if '</w>' in token:
-            curr_token += token[:-4]
-
-            if curr_idx == word_idx and curr_token == word:
-                break
-
-            curr_token = ''
-            curr_idx += 1
-            merge_idxs.clear()
-        else:
-            curr_token += token
-            merge_idxs.append(idx)
+        word = word.lower()
+        search_tokens = tokenizer.tokenize(word)
+        start_indices = [x + offset_idx for x in range(len(tokens)) if tokens[x:x + len(search_tokens)] == search_tokens]
+        for indice in start_indices:
+            merge_idxs += [i + indice for i in range(0, len(search_tokens))]
+        if not merge_idxs:
+            raise ValueError(f'Search word {word} not found in prompt!')
+    else:
+        merge_idxs.append(word_idx)
 
-    return [x + 1 for x in merge_idxs]  # Offset by 1.
+    return [x + 1 for x in merge_idxs], word_idx  # Offset by 1.
 
 
 nlp = None
 
 
 @lru_cache(maxsize=100000)
 def cached_nlp(prompt: str, type='en_core_web_md'):
     global nlp
 
     if nlp is None:
-        nlp = spacy.load(type)
+        try:
+            nlp = spacy.load(type)
+        except OSError:
+            import os
+            os.system(f'python -m spacy download {type}')
+            nlp = spacy.load(type)
 
     return nlp(prompt)
```

### Comparing `daam-0.0.9/setup.py` & `daam-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,10 +10,11 @@
     description='What the DAAM: Interpreting Stable Diffusion Using Cross Attention.',
     install_requires=open('requirements.txt').read().strip().splitlines(),
     packages=setuptools.find_packages(),
     python_requires='>=3.8',
     entry_points={
         'console_scripts': [
             'daam = daam.run.generate:main',
+            'daam-demo = daam.run.demo:main',
         ]
     }
 )
```

