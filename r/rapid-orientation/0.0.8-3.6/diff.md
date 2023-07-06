# Comparing `tmp/rapid_orientation-0.0.8-py3-none-any.whl.zip` & `tmp/rapid_orientation-3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6289944 bytes, number of entries: 10
--rw-r--r--  2.0 unx      122 b- defN 23-Jul-06 10:34 rapid_orientation/__init__.py
--rw-r--r--  2.0 unx      350 b- defN 23-Jul-06 10:34 rapid_orientation/config.yaml
--rw-r--r--  2.0 unx     2755 b- defN 23-Jul-06 10:34 rapid_orientation/rapid_orientation.py
--rw-r--r--  2.0 unx     7714 b- defN 23-Jul-06 10:34 rapid_orientation/utils.py
+Zip file size: 6289921 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-15 14:14 rapid_orientation/__init__.py
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-15 14:14 rapid_orientation/config.yaml
+-rw-r--r--  2.0 unx     2804 b- defN 23-Jun-15 14:14 rapid_orientation/rapid_orientation.py
+-rw-r--r--  2.0 unx     7735 b- defN 23-Jun-15 14:14 rapid_orientation/utils.py
 -rw-rw-r--  2.0 unx  6792721 b- defN 23-Jan-20 13:53 rapid_orientation/models/rapid_orientation.onnx
--rw-r--r--  2.0 unx     2809 b- defN 23-Jul-06 10:34 rapid_orientation-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 10:34 rapid_orientation-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 23-Jul-06 10:34 rapid_orientation-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-Jul-06 10:34 rapid_orientation-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      898 b- defN 23-Jul-06 10:34 rapid_orientation-0.0.8.dist-info/RECORD
-10 files, 6807558 bytes uncompressed, 6288388 bytes compressed:  7.6%
+-rw-r--r--  2.0 unx     2808 b- defN 23-Jun-15 14:15 rapid_orientation-3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 14:15 rapid_orientation-3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-15 14:15 rapid_orientation-3.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-15 14:15 rapid_orientation-3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      888 b- defN 23-Jun-15 14:15 rapid_orientation-3.6.dist-info/RECORD
+10 files, 6807617 bytes uncompressed, 6288385 bytes compressed:  7.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: rapid_orientation/utils.py
 Comment: 
 
 Filename: rapid_orientation/models/rapid_orientation.onnx
 Comment: 
 
-Filename: rapid_orientation-0.0.8.dist-info/METADATA
+Filename: rapid_orientation-3.6.dist-info/METADATA
 Comment: 
 
-Filename: rapid_orientation-0.0.8.dist-info/WHEEL
+Filename: rapid_orientation-3.6.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_orientation-0.0.8.dist-info/entry_points.txt
+Filename: rapid_orientation-3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_orientation-0.0.8.dist-info/top_level.txt
+Filename: rapid_orientation-3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_orientation-0.0.8.dist-info/RECORD
+Filename: rapid_orientation-3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_orientation/rapid_orientation.py

```diff
@@ -24,24 +24,24 @@
 import yaml
 
 from .utils import LoadImage, OrtInferSession, create_operators
 
 root_dir = Path(__file__).resolve().parent
 
 
-class RapidOrientation:
+class RapidOrientation():
     def __init__(self, model_path: str = None):
-        config_path = str(root_dir / "config.yaml")
+        config_path = str(root_dir / 'config.yaml')
         config = self.read_yaml(config_path)
         if model_path is None:
-            model_path = str(root_dir / "models" / "rapid_orientation.onnx")
-        config["model_path"] = model_path
+            model_path = str(root_dir / 'models' / 'rapid_orientation.onnx')
+        config['model_path'] = model_path
 
         self.session = OrtInferSession(config)
-        self.labels = self.session.get_metadata()["character"].splitlines()
+        self.labels = self.session.get_metadata()['character'].splitlines()
 
         self.preprocess_ops = create_operators(config["PreProcess"])
 
         self.load_img = LoadImage()
 
     def __call__(self, img_content: Union[str, np.ndarray, bytes, Path]):
         images = self.load_img(img_content)
@@ -57,35 +57,31 @@
         pred_idx = np.argmax(pred_output)
         pred_txt = self.labels[pred_idx]
         elapse = time.time() - s
         return pred_txt, elapse
 
     @staticmethod
     def read_yaml(yaml_path):
-        with open(yaml_path, "rb") as f:
+        with open(yaml_path, 'rb') as f:
             data = yaml.load(f, Loader=yaml.Loader)
         return data
 
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-img", "--img_path", type=str, required=True, help="Path to image for layout."
-    )
-    parser.add_argument(
-        "-m",
-        "--model_path",
-        type=str,
-        default=str(root_dir / "models" / "rapid_orientation.onnx"),
-        help="The model path used for inference.",
-    )
+    parser.add_argument('-img', '--img_path', type=str, required=True,
+                        help='Path to image for layout.')
+    parser.add_argument('-m', '--model_path', type=str,
+                        default=str(root_dir / 'models' /
+                                    'rapid_orientation.onnx'),
+                        help='The model path used for inference.')
     args = parser.parse_args()
 
     orientation_engine = RapidOrientation(args.model_path)
 
     img = cv2.imread(args.img_path)
     orientaion_result, _ = orientation_engine(img)
     print(orientaion_result)
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     main()
```

## rapid_orientation/utils.py

```diff
@@ -5,111 +5,92 @@
 import warnings
 from io import BytesIO
 from pathlib import Path
 from typing import Union
 
 import cv2
 import numpy as np
-from onnxruntime import (
-    GraphOptimizationLevel,
-    InferenceSession,
-    SessionOptions,
-    get_available_providers,
-    get_device,
-)
+from onnxruntime import (GraphOptimizationLevel, InferenceSession,
+                         SessionOptions, get_available_providers, get_device)
 from PIL import Image, UnidentifiedImageError
 
 InputType = Union[str, np.ndarray, bytes, Path]
 
 
-class OrtInferSession:
+class OrtInferSession():
     def __init__(self, config):
         sess_opt = SessionOptions()
         sess_opt.log_severity_level = 4
         sess_opt.enable_cpu_mem_arena = False
         sess_opt.graph_optimization_level = GraphOptimizationLevel.ORT_ENABLE_ALL
 
-        cuda_ep = "CUDAExecutionProvider"
-        cpu_ep = "CPUExecutionProvider"
-        cpu_provider_options = {
-            "arena_extend_strategy": "kSameAsRequested",
-        }
+        cuda_ep = 'CUDAExecutionProvider'
+        cpu_ep = 'CPUExecutionProvider'
+        cpu_provider_options = {"arena_extend_strategy": "kSameAsRequested", }
 
         EP_list = []
-        if (
-            config["use_cuda"]
-            and get_device() == "GPU"
-            and cuda_ep in get_available_providers()
-        ):
+        if config['use_cuda'] and get_device() == 'GPU' \
+                and cuda_ep in get_available_providers():
             EP_list = [(cuda_ep, config[cuda_ep])]
         EP_list.append((cpu_ep, cpu_provider_options))
 
-        self._verify_model(config["model_path"])
-        self.session = InferenceSession(
-            config["model_path"], sess_options=sess_opt, providers=EP_list
-        )
+        self._verify_model(config['model_path'])
+        self.session = InferenceSession(config['model_path'],
+                                        sess_options=sess_opt,
+                                        providers=EP_list)
 
         has_cuda_ep = cuda_ep not in self.session.get_providers()
-        if config["use_cuda"] and has_cuda_ep:
-            warnings.warn(
-                f"{cuda_ep} is not avaiable for current env,"
-                f"the inference part is automatically shifted to "
-                f"be executed under {cpu_ep}. "
-                f"Please ensure the installed onnxruntime-gpu "
-                f" version matches your cuda and cudnn version, "
-                f"you can check their relations from the offical web site: "
-                f"https://onnxruntime.ai/docs/execution-providers/CUDA-ExecutionProvider.html",
-                RuntimeWarning,
-            )
+        if config['use_cuda'] and has_cuda_ep:
+            warnings.warn(f'{cuda_ep} is not avaiable for current env,'
+                          f'the inference part is automatically shifted to '
+                          f'be executed under {cpu_ep}. '
+                          f'Please ensure the installed onnxruntime-gpu '
+                          f' version matches your cuda and cudnn version, '
+                          f'you can check their relations from the offical web site: '
+                          f'https://onnxruntime.ai/docs/execution-providers/CUDA-ExecutionProvider.html',
+                          RuntimeWarning)
 
     def __call__(self, input_content: np.ndarray) -> np.ndarray:
         input_dict = dict(zip(self.get_input_names(), [input_content]))
         try:
             return self.session.run(self.get_output_names(), input_dict)
         except Exception as e:
-            raise ONNXRuntimeError("ONNXRuntime inferece failed.") from e
+            raise ONNXRuntimeError('ONNXRuntime inferece failed.') from e
 
-    def get_input_names(
-        self,
-    ):
+    def get_input_names(self, ):
         return [v.name for v in self.session.get_inputs()]
 
-    def get_output_names(
-        self,
-    ):
+    def get_output_names(self,):
         return [v.name for v in self.session.get_outputs()]
 
     def get_metadata(self):
         meta_dict = self.session.get_modelmeta().custom_metadata_map
         return meta_dict
 
     @staticmethod
     def _verify_model(model_path):
         model_path = Path(model_path)
         if not model_path.exists():
-            raise FileNotFoundError(f"{model_path} does not exists.")
+            raise FileNotFoundError(f'{model_path} does not exists.')
         if not model_path.is_file():
-            raise FileExistsError(f"{model_path} is not a file.")
+            raise FileExistsError(f'{model_path} is not a file.')
 
 
 class ONNXRuntimeError(Exception):
     pass
 
 
-class LoadImage:
-    def __init__(
-        self,
-    ):
+class LoadImage():
+    def __init__(self, ):
         pass
 
     def __call__(self, img: InputType) -> np.ndarray:
         if not isinstance(img, InputType.__args__):
             raise LoadImageError(
-                f"The img type {type(img)} does not in {InputType.__args__}"
-            )
+                f'The img type {type(img)} does not in {InputType.__args__}')
 
         img = self.load_img(img)
 
         if img.ndim == 2:
             return cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
 
         if img.ndim == 3 and img.shape[2] == 4:
@@ -120,125 +101,124 @@
     def load_img(self, img: InputType) -> np.ndarray:
         if isinstance(img, (str, Path)):
             self.verify_exist(img)
             try:
                 img = np.array(Image.open(img))
                 img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
             except UnidentifiedImageError as e:
-                raise LoadImageError(f"cannot identify image file {img}") from e
+                raise LoadImageError(
+                    f'cannot identify image file {img}') from e
             return img
 
         if isinstance(img, bytes):
             img = np.array(Image.open(BytesIO(img)))
             img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
             return img
 
         if isinstance(img, np.ndarray):
             return img
 
-        raise LoadImageError(f"{type(img)} is not supported!")
+        raise LoadImageError(f'{type(img)} is not supported!')
 
     @staticmethod
     def cvt_four_to_three(img: np.ndarray) -> np.ndarray:
-        """RGBA → RGB"""
+        '''RGBA → RGB
+        '''
         r, g, b, a = cv2.split(img)
         new_img = cv2.merge((b, g, r))
 
         not_a = cv2.bitwise_not(a)
         not_a = cv2.cvtColor(not_a, cv2.COLOR_GRAY2BGR)
 
         new_img = cv2.bitwise_and(new_img, new_img, mask=a)
         new_img = cv2.add(new_img, not_a)
         return new_img
 
     @staticmethod
     def verify_exist(file_path: Union[str, Path]):
         if not Path(file_path).exists():
-            raise LoadImageError(f"{file_path} does not exist.")
+            raise LoadImageError(f'{file_path} does not exist.')
 
 
 class LoadImageError(Exception):
     pass
 
 
 def create_operators(params):
     """
     create operators based on the config
 
     Args:
         params(list): a dict list, used to create some operators
     """
-    assert isinstance(params, list), "operator config should be a list"
+    assert isinstance(params, list), ('operator config should be a list')
     mod = importlib.import_module(__name__)
     ops = []
     for operator in params:
-        assert isinstance(operator, dict) and len(operator) == 1, "yaml format error"
+        assert isinstance(operator,
+                          dict) and len(operator) == 1, "yaml format error"
         op_name = list(operator)[0]
         param = {} if operator[op_name] is None else operator[op_name]
         op = getattr(mod, op_name)(**param)
         ops.append(op)
     return ops
 
 
-class ResizeImage:
+class ResizeImage():
     def __init__(self, size=None, resize_short=None):
         if resize_short is not None and resize_short > 0:
             self.resize_short = resize_short
             self.w, self.h = None, None
         elif size is not None:
             self.resize_short = None
             self.w = size if isinstance(size, int) else size[0]
             self.h = size if isinstance(size, int) else size[1]
         else:
-            raise ValueError(
-                "invalid params for ReisizeImage for '\
-                'both 'size' and 'resize_short' are None"
-            )
+            raise ValueError("invalid params for ReisizeImage for '\
+                'both 'size' and 'resize_short' are None")
 
     def __call__(self, img: np.ndarray):
         img_h, img_w = img.shape[:2]
 
         if self.resize_short:
             percent = float(self.resize_short) / min(img_w, img_h)
             w = int(round(img_w * percent))
             h = int(round(img_h * percent))
         else:
             w = self.w
             h = self.h
         return cv2.resize(img, (w, h))
 
 
-class NormalizeImage:
-    def __init__(
-        self,
-    ):
+class NormalizeImage():
+    def __init__(self,):
         self.scale = np.float32(1.0 / 255.0)
         mean = [0.485, 0.456, 0.406]
         std = [0.229, 0.224, 0.225]
 
         shape = 1, 1, 3
-        self.mean = np.array(mean).reshape(shape).astype("float32")
-        self.std = np.array(std).reshape(shape).astype("float32")
+        self.mean = np.array(mean).reshape(shape).astype('float32')
+        self.std = np.array(std).reshape(shape).astype('float32')
 
     def __call__(self, img):
         img = np.array(img).astype(np.float32)
         img = (img * self.scale - self.mean) / self.std
         return img.astype(np.float32)
 
 
-class ToCHWImage:
+class ToCHWImage():
     def __init__(self):
         pass
 
     def __call__(self, img):
         img = np.array(img)
         return img.transpose((2, 0, 1))
 
 
-class CropImage:
+class CropImage():
     def __init__(self, size):
         self.size = size
         if isinstance(size, int):
             self.size = (size, size)
 
     def __call__(self, img):
         w, h = self.size
```

## Comparing `rapid_orientation-0.0.8.dist-info/METADATA` & `rapid_orientation-3.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: rapid-orientation
-Version: 0.0.8
+Version: 3.6
 Summary: Tools for classifying the direction of images containing text based ONNXRuntime.
 Home-page: https://github.com/RapidAI/RapidStructure
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: ppstructure,layout,rapidocr,rapid_orientation
 Platform: Any
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6,<3.12
+Requires-Python: >=3.6,<=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: onnxruntime (>=1.7.0)
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: opencv-python (>=4.5.1.48)
 Requires-Dist: numpy (>=1.21.6)
 Requires-Dist: Pillow
 
 ## rapid-orientation
 <p align="left">
-    <a href=""><img src="https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg"></a>
+    <a href=""><img src="https://img.shields.io/badge/Python->=3.6,<=3.11-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href="https://pypi.org/project/rapid-orientation/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapid-orientation"></a>
     <a href="https://pepy.tech/project/rapid-orientation"><img src="https://static.pepy.tech/personalized-badge/rapid-orientation?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
 </p>
 
-
 ### 1. Install package by pypi.
 ```bash
 $ pip install rapid-orientation
 ```
 
 ### 2. Run by script.
 - RapidOrientation has the default `model_path` value, you can set the different value of `model_path` to use different models, e.g. `orientation_engine = RapidOrientation(model_path='rapid_orientation.onnx')`
```

### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: rapid-orientation Version: 0.0.8 Summary: Tools for
+Metadata-Version: 2.1 Name: rapid-orientation Version: 3.6 Summary: Tools for
 classifying the direction of images containing text based ONNXRuntime. Home-
 page: https://github.com/RapidAI/RapidStructure Author: SWHL Author-email:
 liekkaskono@163.com License: Apache-2.0 Keywords:
 ppstructure,layout,rapidocr,rapid_orientation Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Python: >=3.6,<3.12 Description-Content-Type: text/markdown Requires-Dist:
+Python: >=3.6,<=3.11 Description-Content-Type: text/markdown Requires-Dist:
 onnxruntime (>=1.7.0) Requires-Dist: PyYAML (>=6.0) Requires-Dist: opencv-
 python (>=4.5.1.48) Requires-Dist: numpy (>=1.21.6) Requires-Dist: Pillow ##
 rapid-orientation
-[https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg] [https://
+[https://img.shields.io/badge/Python->=3.6,<=3.11-aff.svg] [https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
 static.pepy.tech/personalized-badge/rapid-
 orientation?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
 ### 1. Install package by pypi. ```bash $ pip install rapid-orientation ``` ###
 2. Run by script. - RapidOrientation has the default `model_path` value, you
 can set the different value of `model_path` to use different models, e.g.
 `orientation_engine = RapidOrientation(model_path='rapid_orientation.onnx')` -
```

## Comparing `rapid_orientation-0.0.8.dist-info/RECORD` & `rapid_orientation-3.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 rapid_orientation/__init__.py,sha256=WYYdZeKq1BvJkoBpnM-9QZs1Nbx6RV9uagmVFrwGvxU,122
 rapid_orientation/config.yaml,sha256=6FyPLomim5pAjMZtKUO75NLV9XKGgyKihXItxFX-Wb4,350
-rapid_orientation/rapid_orientation.py,sha256=95s7Znzt0vbqi1dHRlPGWtrpT-No_1NCTHP0QZtOhfo,2755
-rapid_orientation/utils.py,sha256=MYaX3jEIxIG18aDLJdtOYvjepfu1jDZBE038yK7SOOc,7714
+rapid_orientation/rapid_orientation.py,sha256=HSuXtvqnooy2Gm0--n2md6nLNDdrODuyJ1ysAC6aJ60,2804
+rapid_orientation/utils.py,sha256=hSoDYMQL_CPmgHioRTLkJt1Wk5ZLeqPYxvcKqT2byWc,7735
 rapid_orientation/models/rapid_orientation.onnx,sha256=nIShBBuY_HQTLRHtraf1r8jJEfrjVc3n0ExijTSvHYo,6792721
-rapid_orientation-0.0.8.dist-info/METADATA,sha256=ZRGh5Fz9YJMG-5CJvH_J9ZqZbg8tjMWd2gLNoQSTo5M,2809
-rapid_orientation-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapid_orientation-0.0.8.dist-info/entry_points.txt,sha256=Yncu1HqYh7MxLxZvupD5ut3hJbU1DWxYCrtANCxbbBg,79
-rapid_orientation-0.0.8.dist-info/top_level.txt,sha256=6Xiql6N2aF4rctCG2D0W55YnVe7aS-9dSZJ6lEYejLc,18
-rapid_orientation-0.0.8.dist-info/RECORD,,
+rapid_orientation-3.6.dist-info/METADATA,sha256=xnZ8CTZs8sSZF4qiZgThX1e-2cbIONuRX4meINpvrTc,2808
+rapid_orientation-3.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapid_orientation-3.6.dist-info/entry_points.txt,sha256=Yncu1HqYh7MxLxZvupD5ut3hJbU1DWxYCrtANCxbbBg,79
+rapid_orientation-3.6.dist-info/top_level.txt,sha256=6Xiql6N2aF4rctCG2D0W55YnVe7aS-9dSZJ6lEYejLc,18
+rapid_orientation-3.6.dist-info/RECORD,,
```

