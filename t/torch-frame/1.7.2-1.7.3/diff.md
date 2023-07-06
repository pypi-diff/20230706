# Comparing `tmp/torch-frame-1.7.2.tar.gz` & `tmp/torch-frame-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\torch-frame-1.7.2.tar", last modified: Tue Jul  4 13:01:07 2023, max compression
+gzip compressed data, was "dist\torch-frame-1.7.3.tar", last modified: Thu Jul  6 15:26:22 2023, max compression
```

## Comparing `torch-frame-1.7.2.tar` & `torch-frame-1.7.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 13:01:07.000000 torch-frame-1.7.2/
--rw-rw-rw-   0        0        0      516 2023-07-04 13:01:07.000000 torch-frame-1.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     4619 2023-07-04 13:00:55.000000 torch-frame-1.7.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 13:01:07.000000 torch-frame-1.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1662 2023-07-04 00:59:45.000000 torch-frame-1.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame/
--rw-rw-rw-   0        0        0      345 2023-06-22 03:49:09.000000 torch-frame-1.7.2/torch_frame/__init__.py
--rw-rw-rw-   0        0        0      104 2022-10-29 16:33:51.000000 torch-frame-1.7.2/torch_frame/_get_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame/datasets/
--rw-rw-rw-   0        0        0       69 2023-06-22 03:27:40.000000 torch-frame-1.7.2/torch_frame/datasets/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-06-22 03:27:40.000000 torch-frame-1.7.2/torch_frame/datasets/dataloader_wrappers.py
--rw-rw-rw-   0        0        0     1690 2023-06-22 03:27:40.000000 torch-frame-1.7.2/torch_frame/datasets/dataset_wrappers.py
--rw-rw-rw-   0        0        0     6280 2022-08-20 06:57:53.000000 torch-frame-1.7.2/torch_frame/ddp_trainer.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame/hooks/
--rw-rw-rw-   0        0        0      164 2022-08-21 08:37:48.000000 torch-frame-1.7.2/torch_frame/hooks/__init__.py
--rw-rw-rw-   0        0        0     3678 2023-07-04 12:44:20.000000 torch-frame-1.7.2/torch_frame/hooks/checkpoint_hook.py
--rw-rw-rw-   0        0        0     5506 2022-10-17 14:31:24.000000 torch-frame-1.7.2/torch_frame/hooks/eval_hook.py
--rw-rw-rw-   0        0        0     2897 2022-01-05 16:01:30.000000 torch-frame-1.7.2/torch_frame/hooks/hookbase.py
--rw-rw-rw-   0        0        0     5181 2022-05-29 11:46:20.000000 torch-frame-1.7.2/torch_frame/hooks/logger_hook.py
--rw-rw-rw-   0        0        0     4526 2022-01-04 14:56:31.000000 torch-frame-1.7.2/torch_frame/lr_scheduler.py
--rw-rw-rw-   0        0        0    24466 2023-07-04 12:50:51.000000 torch-frame-1.7.2/torch_frame/trainer.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame/utils/
--rw-rw-rw-   0        0        0      197 2022-07-23 16:05:47.000000 torch-frame-1.7.2/torch_frame/utils/__init__.py
--rw-rw-rw-   0        0        0     2877 2021-12-28 15:17:35.000000 torch-frame-1.7.2/torch_frame/utils/config_parser.py
--rw-rw-rw-   0        0        0      474 2022-07-10 14:07:55.000000 torch-frame-1.7.2/torch_frame/utils/dist_utils.py
--rw-rw-rw-   0        0        0     1534 2022-01-09 15:26:45.000000 torch-frame-1.7.2/torch_frame/utils/history_buffer.py
--rw-rw-rw-   0        0        0     4762 2022-08-20 06:57:53.000000 torch-frame-1.7.2/torch_frame/utils/logger.py
--rw-rw-rw-   0        0        0     5926 2022-08-26 15:29:40.000000 torch-frame-1.7.2/torch_frame/utils/metric.py
--rw-rw-rw-   0        0        0     5089 2022-07-10 14:17:20.000000 torch-frame-1.7.2/torch_frame/utils/misc.py
--rw-rw-rw-   0        0        0     1153 2022-07-23 16:09:27.000000 torch-frame-1.7.2/torch_frame/utils/progress_bar.py
--rw-rw-rw-   0        0        0     2422 2022-11-08 15:26:22.000000 torch-frame-1.7.2/torch_frame/utils/test_speed.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame/vision/
--rw-rw-rw-   0        0        0       52 2022-03-13 15:20:23.000000 torch-frame-1.7.2/torch_frame/vision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame/vision/augmentations/
--rw-rw-rw-   0        0        0       43 2022-02-20 14:36:40.000000 torch-frame-1.7.2/torch_frame/vision/augmentations/__init__.py
--rw-rw-rw-   0        0        0      756 2022-08-20 08:01:58.000000 torch-frame-1.7.2/torch_frame/vision/augmentations/base.py
--rw-rw-rw-   0        0        0    10161 2022-03-15 06:49:07.000000 torch-frame-1.7.2/torch_frame/vision/augmentations/boxes.py
--rw-rw-rw-   0        0        0     2779 2023-03-23 15:45:03.000000 torch-frame-1.7.2/torch_frame/vision/augmentations/colors.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame/vision/tools/
--rw-rw-rw-   0        0        0       31 2022-03-13 15:20:39.000000 torch-frame-1.7.2/torch_frame/vision/tools/__init__.py
--rw-rw-rw-   0        0        0    14776 2022-08-26 15:29:40.000000 torch-frame-1.7.2/torch_frame/vision/tools/object_detection.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame.egg-info/
--rw-rw-rw-   0        0        0      516 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-04 13:01:07.000000 torch-frame-1.7.2/torch_frame.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 15:26:22.000000 torch-frame-1.7.3/
+-rw-rw-rw-   0        0        0      516 2023-07-06 15:26:22.000000 torch-frame-1.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4619 2023-07-04 13:00:55.000000 torch-frame-1.7.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:26:22.000000 torch-frame-1.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1662 2023-07-06 15:08:07.000000 torch-frame-1.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:26:22.000000 torch-frame-1.7.3/torch_frame/
+-rw-rw-rw-   0        0        0      345 2023-06-22 03:49:09.000000 torch-frame-1.7.3/torch_frame/__init__.py
+-rw-rw-rw-   0        0        0      104 2022-10-29 16:33:51.000000 torch-frame-1.7.3/torch_frame/_get_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:26:22.000000 torch-frame-1.7.3/torch_frame/datasets/
+-rw-rw-rw-   0        0        0       69 2023-06-22 03:27:40.000000 torch-frame-1.7.3/torch_frame/datasets/__init__.py
+-rw-rw-rw-   0        0        0     1004 2023-06-22 03:27:40.000000 torch-frame-1.7.3/torch_frame/datasets/dataloader_wrappers.py
+-rw-rw-rw-   0        0        0     1690 2023-06-22 03:27:40.000000 torch-frame-1.7.3/torch_frame/datasets/dataset_wrappers.py
+-rw-rw-rw-   0        0        0     6315 2023-07-06 15:17:41.000000 torch-frame-1.7.3/torch_frame/ddp_trainer.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:26:22.000000 torch-frame-1.7.3/torch_frame/hooks/
+-rw-rw-rw-   0        0        0      164 2022-08-21 08:37:48.000000 torch-frame-1.7.3/torch_frame/hooks/__init__.py
+-rw-rw-rw-   0        0        0     3678 2023-07-04 12:44:20.000000 torch-frame-1.7.3/torch_frame/hooks/checkpoint_hook.py
+-rw-rw-rw-   0        0        0     5698 2023-07-06 15:24:32.000000 torch-frame-1.7.3/torch_frame/hooks/eval_hook.py
+-rw-rw-rw-   0        0        0     2897 2022-01-05 16:01:30.000000 torch-frame-1.7.3/torch_frame/hooks/hookbase.py
+-rw-rw-rw-   0        0        0     5181 2022-05-29 11:46:20.000000 torch-frame-1.7.3/torch_frame/hooks/logger_hook.py
+-rw-rw-rw-   0        0        0     4526 2022-01-04 14:56:31.000000 torch-frame-1.7.3/torch_frame/lr_scheduler.py
+-rw-rw-rw-   0        0        0    25112 2023-07-06 15:23:15.000000 torch-frame-1.7.3/torch_frame/trainer.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:26:22.000000 torch-frame-1.7.3/torch_frame/utils/
+-rw-rw-rw-   0        0        0      219 2023-07-06 14:55:59.000000 torch-frame-1.7.3/torch_frame/utils/__init__.py
+-rw-rw-rw-   0        0        0     2877 2021-12-28 15:17:35.000000 torch-frame-1.7.3/torch_frame/utils/config_parser.py
+-rw-rw-rw-   0        0        0      474 2022-07-10 14:07:55.000000 torch-frame-1.7.3/torch_frame/utils/dist_utils.py
+-rw-rw-rw-   0        0        0     1612 2023-07-06 15:26:13.000000 torch-frame-1.7.3/torch_frame/utils/ema.py
+-rw-rw-rw-   0        0        0     1534 2022-01-09 15:26:45.000000 torch-frame-1.7.3/torch_frame/utils/history_buffer.py
+-rw-rw-rw-   0        0        0     4762 2022-08-20 06:57:53.000000 torch-frame-1.7.3/torch_frame/utils/logger.py
+-rw-rw-rw-   0        0        0     5926 2022-08-26 15:29:40.000000 torch-frame-1.7.3/torch_frame/utils/metric.py
+-rw-rw-rw-   0        0        0     5089 2022-07-10 14:17:20.000000 torch-frame-1.7.3/torch_frame/utils/misc.py
+-rw-rw-rw-   0        0        0     1153 2022-07-23 16:09:27.000000 torch-frame-1.7.3/torch_frame/utils/progress_bar.py
+-rw-rw-rw-   0        0        0     2422 2022-11-08 15:26:22.000000 torch-frame-1.7.3/torch_frame/utils/test_speed.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:26:22.000000 torch-frame-1.7.3/torch_frame/vision/
+-rw-rw-rw-   0        0        0       52 2022-03-13 15:20:23.000000 torch-frame-1.7.3/torch_frame/vision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:26:22.000000 torch-frame-1.7.3/torch_frame/vision/augmentations/
+-rw-rw-rw-   0        0        0       43 2022-02-20 14:36:40.000000 torch-frame-1.7.3/torch_frame/vision/augmentations/__init__.py
+-rw-rw-rw-   0        0        0      756 2022-08-20 08:01:58.000000 torch-frame-1.7.3/torch_frame/vision/augmentations/base.py
+-rw-rw-rw-   0        0        0    10161 2022-03-15 06:49:07.000000 torch-frame-1.7.3/torch_frame/vision/augmentations/boxes.py
+-rw-rw-rw-   0        0        0     2779 2023-03-23 15:45:03.000000 torch-frame-1.7.3/torch_frame/vision/augmentations/colors.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:26:22.000000 torch-frame-1.7.3/torch_frame/vision/tools/
+-rw-rw-rw-   0        0        0       31 2022-03-13 15:20:39.000000 torch-frame-1.7.3/torch_frame/vision/tools/__init__.py
+-rw-rw-rw-   0        0        0    14776 2022-08-26 15:29:40.000000 torch-frame-1.7.3/torch_frame/vision/tools/object_detection.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:26:22.000000 torch-frame-1.7.3/torch_frame.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-06 15:26:21.000000 torch-frame-1.7.3/torch_frame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1190 2023-07-06 15:26:21.000000 torch-frame-1.7.3/torch_frame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:26:21.000000 torch-frame-1.7.3/torch_frame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-06 15:26:21.000000 torch-frame-1.7.3/torch_frame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-06 15:26:21.000000 torch-frame-1.7.3/torch_frame.egg-info/top_level.txt
```

### Comparing `torch-frame-1.7.2/PKG-INFO` & `torch-frame-1.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-frame
-Version: 1.7.2
+Version: 1.7.3
 Summary: 用于深度学习快速实现代码的框架
 Home-page: https://github.com/darknli/Pytorch-Frame/tree/main/torch_frame
 Author: Darkn Lxs
 Author-email: 1187220556@qq.com
 License: UNKNOWN
 Description: 见readme
 Platform: UNKNOWN
```

### Comparing `torch-frame-1.7.2/README.md` & `torch-frame-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/setup.py` & `torch-frame-1.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # 允许setup.py在任何路径下执行
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="torch-frame",  # 库名, 需要在pypi中唯一
-    version="1.7.2",  # 版本号
+    version="1.7.3",  # 版本号
     author="Darkn Lxs",  # 作者
     author_email="1187220556@qq.com",  # 作看都将（方便使用索类现问图后成我我们）
     description="用于深度学习快速实现代码的框架",  # 简介
     long_description="见readme",  # 详细描述（一般会写在README.md中）
     long_description_content_type="text/markdown",  # README.md中描述的语法（一般为markdown)
     url="https://github.com/darknli/Pytorch-Frame/tree/main/torch_frame",  # 库/项目主页，放该项目的远程库地址即可
     packages=setuptools.find_packages(),  # 默认值即可，这个是方便以后我们给库拓展新功能的
```

### Comparing `torch-frame-1.7.2/torch_frame/datasets/dataloader_wrappers.py` & `torch-frame-1.7.3/torch_frame/datasets/dataloader_wrappers.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/datasets/dataset_wrappers.py` & `torch-frame-1.7.3/torch_frame/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/ddp_trainer.py` & `torch-frame-1.7.3/torch_frame/ddp_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,53 @@
 from .utils.dist_utils import *
 
 
 class DDPTrainer(Trainer):
     """
     Trainer的DDP版本。需要注意的是，在调用该类前依然要执行init_process_group，为了避免重复打印或保存数据，应该在外部选择性
     的根据gpu_id调用hooker, 在创建DDPTrainer对象时会自动根据环境判断是否使用ddp，无需手动设置
+
+
+    Parameters
+    ---------
+    model : torch.nn.Module, 训练模型, 训练时的输出只能是以下三种:
+        * torch.Tensor, 对于这种输出是模型backward用的loss, 在torch-frame框架中被称为total_loss
+        * dict, 里面是模型的各路分支的loss，需要是标量, Trainer会自动将其求和得到total_loss, 再做backward
+        * Tuple[Union[dict, torch.Tensor], dict]. 前两种的混合体, 元组第一个输出是前面两种的任意一种;
+          第二个输出是非需要backward类的, Trainer不会把这个dict汇总到total_loss上
+    optimizer : torch.optim.Optimizer, 优化器
+    lr_scheduler : optim.lr_scheduler._LRScheduler, 学习率调节器
+    dataset : torch.utils.data.Dataset, 训练集数据生成器, 不需要创建dataloader, 由DDPTrainer内部创建
+    dataset_params : dict, dataset的参数, key是诸如batch_size的参数
+    max_epochs : int, 训练的总轮数
+    work_dir : str, 保存模型和日志的根目录地址
+    clip_grad_norm : float, default 0.0
+        梯度裁剪的设置, 如果置为小于等于0, 则不作梯度裁剪
+    enable_amp : bool, 使用混合精度
+    warmup_method : str, default None
+        warmup的类型, 包含以下四种取值
+        * constant
+        * linear
+        * exp
+        * None : 不使用warmup
+    warmup_iters : int, default 1000, warmup最后的iter数
+    warmup_factor : float, default 0.001
+        warmup初始学习率 = warmup_factor * initial_lr
+    hooks : List[HookBase], default None.
+        hooks, 保存模型、输出评估指标、loss等用
+    use_ema : bool, default False. 是否使用EMA技术
+    ema_decay: float = 0.9999. EMA模型衰减系数
+    create_new_dir : Optional[str], default time
+        存在同名目录时以何种策略创建目录
+        * None, 直接使用同名目录
+        * `time_s`, 如果已经存在同名目录, 则以时间(精确到秒)为后缀创建新目录
+        * `time_m`, 如果已经存在同名目录, 则以时间(精确到分)为后缀创建新目录
+        * `time_h`, 如果已经存在同名目录, 则以时间(精确到小时)为后缀创建新目录
+        * `time_d`, 如果已经存在同名目录, 则以时间(精确到日)为后缀创建新目录
+        * `count`, 如果已经存在同名目录, 则以序号为后缀创建新目录
     """
 
     def __init__(self,
                  model: nn.Module,
                  optimizer: optim.Optimizer,
                  lr_scheduler: optim.lr_scheduler._LRScheduler,
                  dataset: Dataset,
@@ -20,66 +59,29 @@
                  work_dir: str = "work_dir",
                  clip_grad_norm: float = 0.0,
                  enable_amp=False,
                  warmup_method: Optional[str] = None,
                  warmup_iters: int = 1000,
                  warmup_factor: float = 0.001,
                  hooks: Optional[List[HookBase]] = None,
+                 use_ema: bool = False,
+                 ema_decay: float = 0.9999,
                  create_new_dir: Optional[str] = "time_s"
                  ):
-        """
-        初始化
-
-        Parameters
-        ---------
-        model : torch.nn.Module, 训练模型, 训练时的输出只能是以下三种:
-            * torch.Tensor, 对于这种输出是模型backward用的loss, 在torch-frame框架中被称为total_loss
-            * dict, 里面是模型的各路分支的loss，需要是标量, Trainer会自动将其求和得到total_loss, 再做backward
-            * Tuple[Union[dict, torch.Tensor], dict]. 前两种的混合体, 元组第一个输出是前面两种的任意一种;
-              第二个输出是非需要backward类的, Trainer不会把这个dict汇总到total_loss上
-        optimizer : torch.optim.Optimizer, 优化器
-        lr_scheduler : optim.lr_scheduler._LRScheduler, 学习率调节器
-        dataset : torch.utils.data.Dataset, 训练集数据生成器, 不需要创建dataloader, 由DDPTrainer内部创建
-        dataset_params : dict, dataset的参数, key是诸如batch_size的参数
-        max_epochs : int, 训练的总轮数
-        work_dir : str, 保存模型和日志的根目录地址
-        clip_grad_norm : float, default 0.0
-            梯度裁剪的设置, 如果置为小于等于0, 则不作梯度裁剪
-        enable_amp : bool, 使用混合精度
-        warmup_method : str, default None
-            warmup的类型, 包含以下四种取值
-            * constant
-            * linear
-            * exp
-            * None : 不使用warmup
-        warmup_iters : int, default 1000, warmup最后的iter数
-        warmup_factor : float, default 0.001
-            warmup初始学习率 = warmup_factor * initial_lr
-        hooks : List[HookBase], default None.
-            hooks, 保存模型、输出评估指标、loss等用
-        create_new_dir : Optional[str], default time
-            存在同名目录时以何种策略创建目录
-            * None, 直接使用同名目录
-            * `time_s`, 如果已经存在同名目录, 则以时间(精确到秒)为后缀创建新目录
-            * `time_m`, 如果已经存在同名目录, 则以时间(精确到分)为后缀创建新目录
-            * `time_h`, 如果已经存在同名目录, 则以时间(精确到小时)为后缀创建新目录
-            * `time_d`, 如果已经存在同名目录, 则以时间(精确到日)为后缀创建新目录
-            * `count`, 如果已经存在同名目录, 则以序号为后缀创建新目录
-        """
         self.use_dist = is_dist_avail_and_initialized()
         if self.use_dist:
             num_tasks = get_world_size()
             global_rank = get_rank()
             sampler_trainer = DistributedSampler(dataset, num_replicas=num_tasks, rank=global_rank)
         else:
             sampler_trainer = RandomSampler(dataset)
         data_loader = DataLoader(dataset, sampler=sampler_trainer, **dataset_params)
         super(DDPTrainer, self).__init__(model, optimizer, lr_scheduler, data_loader, max_epochs, work_dir,
                                          clip_grad_norm, enable_amp,  warmup_method, warmup_iters, warmup_factor,
-                                         hooks, create_new_dir)
+                                         hooks, use_ema, ema_decay, create_new_dir)
 
     def _train_one_epoch(self) -> None:
         """执行模型一个epoch的全部操作"""
         if self.use_dist:
             # dist.barrier()  这里可能会造成阻塞
             self.data_loader.sampler.set_epoch(self.epoch)
         super(DDPTrainer, self)._train_one_epoch()
```

### Comparing `torch-frame-1.7.2/torch_frame/hooks/checkpoint_hook.py` & `torch-frame-1.7.3/torch_frame/hooks/checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/hooks/eval_hook.py` & `torch-frame-1.7.3/torch_frame/hooks/eval_hook.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,21 +41,22 @@
         super(EvalHook, self).__init__(period, max_to_keep, self.prefix + save_metric, max_first, save_last)
         self._eval_func = eval_func
         self.dataloader = dataloader
 
     @torch.no_grad()
     def _do_eval(self):
         tot_res = {}
-        self.trainer.model.eval()
+        mode_model = self.trainer.model_evaluate.training
+        self.trainer.model_evaluate.eval()
         with tqdm(self.dataloader, desc="eval") as pbar:
             for batch in pbar:
-                res = self._eval_func(self.trainer.model, batch)
+                res = self._eval_func(self.trainer.model_evaluate, batch)
                 for k, v in res.items():
                     tot_res.setdefault(k, []).extend(v)
-        self.trainer.model.train()
+        self.trainer.model_evaluate.train(mode_model)
         if tot_res:
             rename_res = {self.prefix + k: np.mean(v) for k, v in tot_res.items()}
             self.log(self.trainer.epoch, **rename_res, smooth=False, window_size=1)
 
     def after_epoch(self):
         if self.every_n_epochs(self._period) or self.is_last_epoch():
             self._do_eval()
@@ -103,19 +104,20 @@
         assert hasattr(eval_metric, "update") and isinstance(getattr(eval_metric, "update"), Callable)
         assert hasattr(eval_metric, "evaluate") and isinstance(getattr(eval_metric, "evaluate"), Callable)
         self._eval_metric = eval_metric
         self.dataloader = dataloader
 
     @torch.no_grad()
     def _do_eval(self):
-        self.trainer.model.eval()
+        mode_model = self.trainer.model_evaluate.training
+        self.trainer.model_evaluate.eval()
         with tqdm(self.dataloader, desc="eval") as pbar:
             for batch in pbar:
-                self._eval_metric.update(self.trainer.model, batch)
-        self.trainer.model.train()
+                self._eval_metric.update(self.trainer.model_evaluate, batch)
+        self.trainer.model_evaluate.train(mode_model)
         tot_res = self._eval_metric.evaluate()
         self._eval_metric.reset()
         if tot_res:
             rename_res = {self.prefix + k: np.mean(v) for k, v in tot_res.items()}
             self.log(self.trainer.epoch, **rename_res, smooth=False, window_size=1)
 
     def after_epoch(self):
```

### Comparing `torch-frame-1.7.2/torch_frame/hooks/hookbase.py` & `torch-frame-1.7.3/torch_frame/hooks/hookbase.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/hooks/logger_hook.py` & `torch-frame-1.7.3/torch_frame/hooks/logger_hook.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/lr_scheduler.py` & `torch-frame-1.7.3/torch_frame/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/trainer.py` & `torch-frame-1.7.3/torch_frame/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 import torch.nn as nn
 import torch.optim as optim
 from torch.cuda.amp import GradScaler, autocast
 from torch.nn.parallel import DataParallel, DistributedDataParallel
 from torch.nn.utils import clip_grad_norm_
 from torch.utils.data import DataLoader
 from .hooks import CheckpointerHook, HookBase, LoggerHook
-from .utils import setup_logger, ProgressBar
+from .utils import setup_logger, ProgressBar, HistoryBuffer, EMA
 from .utils.misc import get_workspace
 from .utils.dist_utils import get_rank
 from .lr_scheduler import LRWarmupScheduler
-from .utils import HistoryBuffer
 from ._get_logger import logger
 
 
 class Trainer:
     """
     一个基于epoch的通用训练框架（目前只支持单gpu运行）, 包含：
     1. 计算从dataloader中计算loss
@@ -34,14 +33,51 @@
         model = ...          # 初始化你的模型
         optimizer = ...      # 你的优化器
         lr_scheduler = ...   # 初始化你的调节器
         data_loader = ...    # 初始化你的数据生成器
         # 训练100轮
         trainer = Trainer(model, optimizer, lr_scheduler, data_loader, max_epochs=100)
         trainer.train()
+
+    Parameters
+    ---------
+    model : torch.nn.Module, 训练模型, 训练时的输出只能是以下三种:
+        * torch.Tensor, 对于这种输出是模型backward用的loss, 在torch-frame框架中被称为total_loss
+        * dict, 里面是模型的各路分支的loss，需要是标量, Trainer会自动将其求和得到total_loss, 再做backward
+        * Tuple[Union[dict, torch.Tensor], dict]. 前两种的混合体, 元组第一个输出是前面两种的任意一种;
+          第二个输出是非需要backward类的, Trainer不会把这个dict汇总到total_loss上
+    optimizer : torch.optim.Optimizer, 优化器
+    lr_scheduler : optim.lr_scheduler._LRScheduler, 学习率调节器
+    data_loader : torch.utils.data.DataLoader, 数据生成器
+    max_epochs : int, 训练的总轮数
+    work_dir : str, 保存模型和日志的根目录地址
+    clip_grad_norm : float, default 0.0
+        梯度裁剪的设置, 如果置为小于等于0, 则不作梯度裁剪
+    enable_amp : bool, 使用混合精度
+    warmup_method : str, default None
+        warmup的类型, 包含以下四种取值
+        * constant
+        * linear
+        * exp
+        * None : 不使用warmup
+    warmup_iters : int, default 1000, warmup最后的iter数
+    warmup_factor : float, default 0.001
+        warmup初始学习率 = warmup_factor * initial_lr
+    hooks : List[HookBase], default None.
+        hooks, 保存模型、输出评估指标、loss等用
+    use_ema : bool, default False. 是否使用EMA技术
+    ema_decay: float = 0.9999. EMA模型衰减系数
+    create_new_dir : Optional[str], default time
+        存在同名目录时以何种策略创建目录
+        * None, 直接使用同名目录
+        * `time_s`, 如果已经存在同名目录, 则以时间(精确到秒)为后缀创建新目录
+        * `time_m`, 如果已经存在同名目录, 则以时间(精确到分)为后缀创建新目录
+        * `time_h`, 如果已经存在同名目录, 则以时间(精确到小时)为后缀创建新目录
+        * `time_d`, 如果已经存在同名目录, 则以时间(精确到日)为后缀创建新目录
+        * `count`, 如果已经存在同名目录, 则以序号为后缀创建新目录
     """
 
     def __init__(
             self,
             model: nn.Module,
             optimizer: optim.Optimizer,
             lr_scheduler: optim.lr_scheduler._LRScheduler,
@@ -50,59 +86,27 @@
             work_dir: str = "work_dir",
             clip_grad_norm: float = 0.0,
             enable_amp=False,
             warmup_method: Optional[str] = None,
             warmup_iters: int = 1000,
             warmup_factor: float = 0.001,
             hooks: Optional[List[HookBase]] = None,
+            use_ema: bool = False,
+            ema_decay: float = 0.9999,
             create_new_dir: Optional[str] = "time_s"
     ):
-        """
-        初始化
-
-        Parameters
-        ---------
-        model : torch.nn.Module, 训练模型, 训练时的输出只能是以下三种:
-            * torch.Tensor, 对于这种输出是模型backward用的loss, 在torch-frame框架中被称为total_loss
-            * dict, 里面是模型的各路分支的loss，需要是标量, Trainer会自动将其求和得到total_loss, 再做backward
-            * Tuple[Union[dict, torch.Tensor], dict]. 前两种的混合体, 元组第一个输出是前面两种的任意一种;
-              第二个输出是非需要backward类的, Trainer不会把这个dict汇总到total_loss上
-        optimizer : torch.optim.Optimizer, 优化器
-        lr_scheduler : optim.lr_scheduler._LRScheduler, 学习率调节器
-        data_loader : torch.utils.data.DataLoader, 数据生成器
-        max_epochs : int, 训练的总轮数
-        work_dir : str, 保存模型和日志的根目录地址
-        clip_grad_norm : float, default 0.0
-            梯度裁剪的设置, 如果置为小于等于0, 则不作梯度裁剪
-        enable_amp : bool, 使用混合精度
-        warmup_method : str, default None
-            warmup的类型, 包含以下四种取值
-            * constant
-            * linear
-            * exp
-            * None : 不使用warmup
-        warmup_iters : int, default 1000, warmup最后的iter数
-        warmup_factor : float, default 0.001
-            warmup初始学习率 = warmup_factor * initial_lr
-        hooks : List[HookBase], default None.
-            hooks, 保存模型、输出评估指标、loss等用
-        create_new_dir : Optional[str], default time
-            存在同名目录时以何种策略创建目录
-            * None, 直接使用同名目录
-            * `time_s`, 如果已经存在同名目录, 则以时间(精确到秒)为后缀创建新目录
-            * `time_m`, 如果已经存在同名目录, 则以时间(精确到分)为后缀创建新目录
-            * `time_h`, 如果已经存在同名目录, 则以时间(精确到小时)为后缀创建新目录
-            * `time_d`, 如果已经存在同名目录, 则以时间(精确到日)为后缀创建新目录
-            * `count`, 如果已经存在同名目录, 则以序号为后缀创建新目录
-        """
         logger.setLevel(logging.INFO)
 
         self.work_dir = get_workspace(work_dir, create_new_dir)
 
         self.model = model
+        if use_ema:
+            self.model_ema = EMA(self.model_or_module, ema_decay)
+        else:
+            self.model_ema = None
         self.optimizer = optimizer
         # convert epoch-based scheduler to iteration-based scheduler
         self.lr_scheduler = LRWarmupScheduler(
             lr_scheduler, len(data_loader), warmup_method, warmup_iters, warmup_factor
         )
         self.data_loader = data_loader
         self.metric_storage = MetricStorage()
@@ -169,14 +173,21 @@
     @property
     def model_or_module(self) -> nn.Module:
         if isinstance(self.model, (DistributedDataParallel, DataParallel)):
             return self.model.module
         return self.model
 
     @property
+    def model_evaluate(self) -> nn.Module:
+        """评估用的模型"""
+        if self.model_ema:
+            return self.model_ema.model
+        return self.model_or_module
+
+    @property
     def registered_hook_names(self) -> List[str]:
         """注册的所有hook名字"""
         return [h.__class__.__name__ for h in self._hooks]
 
     def log(self, *args, **kwargs) -> None:
         """更新评估指标"""
         self.metric_storage.update(*args, **kwargs)
@@ -206,15 +217,14 @@
         console_log_level *= 10
         file_log_level *= 10
         setup_logger("torch_frame", output=self.log_file,
                      console_log_level=console_log_level, file_log_level=file_log_level)
 
         os.makedirs(self.ckpt_dir, exist_ok=True)
         if self.start_epoch == 0:
-            logger.info(f"Registered default hooks: {self.registered_hook_names}")
             split_line = "-" * 50
             logger.info(
                 f"\n{split_line}\n"
                 f"Work directory: {self.work_dir}\n"
                 f"{split_line}"
             )
 
@@ -236,27 +246,28 @@
             h.trainer = weakref.proxy(self)
             # We always keep :class:`LoggerHook` as the last hook to avoid losing any records
             # that should have been logged. The order of other hooks remains the same.
             if self._hooks and isinstance(self._hooks[-1], LoggerHook):
                 self._hooks.insert(len(self._hooks) - 1, h)
             else:
                 self._hooks.append(h)
+        logger.warning(f"Registered default hooks: {self.registered_hook_names}")
 
     def _call_hooks(self, stage: str) -> None:
         for h in self._hooks:
             getattr(h, stage)()
 
     def _build_default_hooks(self) -> List[HookBase]:
         return [
             CheckpointerHook(),
             LoggerHook(tb_log_dir=self.tb_log_dir),
         ]
 
     def _update_iter_metrics(self, loss_dict: Dict[str, torch.Tensor], data_time: float,
-                          iter_time: float, lr: float) -> None:
+                             iter_time: float, lr: float) -> None:
         """
         每个iter评估的log
         Parameters
         ----------
         loss_dict : dict, losses的标量字典
         data_time : float, dataloader的一个iter耗时
         iter_time : float, 一个iter全部耗时
@@ -332,14 +343,16 @@
         # 4. 更新模型参数 #
         ##############################
         if self._enable_amp:
             self._grad_scaler.step(self.optimizer)
             self._grad_scaler.update()
         else:
             self.optimizer.step()
+        if self.model_ema:
+            self.model_ema.update(self.model)
 
         ###########################
         # 5. 调整学习率 #
         ###########################
         self.lr_scheduler.step()
 
         show_info = {k: v.detach().cpu().item() if isinstance(v, torch.Tensor) else v for k, v in loss_info.items()}
@@ -429,15 +442,15 @@
         if self._enable_amp:
             data["grad_scaler"] = self._grad_scaler.state_dict()
 
         file_path = osp.join(self.ckpt_dir, file_name)
         if print_info:
             logger.info(f"Saving checkpoint to {file_path}")
         if save_single_model:
-            torch.save(self.model_or_module.state_dict(), file_path)
+            torch.save(self.model_evaluate.state_dict(), file_path)
         else:
             torch.save(data, file_path)
 
     def load_checkpoint(self, path: str = None, checkpoint: Dict[str, Any] = None):
         """
         加载参数
 
@@ -504,14 +517,20 @@
                 if h.class_name == key and h.checkpointable:
                     h.load_state_dict(value)
                     break
 
         # 8. 加载保存目录
         self.work_dir = checkpoint["work_dir"]
 
+        # 9. 加载ema 模型
+        if self.model_ema:
+            lambda_decay = self.model_ema.decay
+            self.model_ema = EMA(self.model_or_module, updates=self.cur_iter)
+            self.model_ema.decay = lambda_decay
+
         if path:
             logger.info(f"加载模型{path}成功")
 
 
 class MetricStorage(dict):
     """The class stores the values of multiple metrics (some of them may be noisy, e.g., loss,
     batch time) in training process, and provides access to the smoothed values for better logging.
```

### Comparing `torch-frame-1.7.2/torch_frame/utils/config_parser.py` & `torch-frame-1.7.3/torch_frame/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/utils/history_buffer.py` & `torch-frame-1.7.3/torch_frame/utils/history_buffer.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/utils/logger.py` & `torch-frame-1.7.3/torch_frame/utils/logger.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/utils/metric.py` & `torch-frame-1.7.3/torch_frame/utils/metric.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/utils/misc.py` & `torch-frame-1.7.3/torch_frame/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/utils/progress_bar.py` & `torch-frame-1.7.3/torch_frame/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/utils/test_speed.py` & `torch-frame-1.7.3/torch_frame/utils/test_speed.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/vision/augmentations/base.py` & `torch-frame-1.7.3/torch_frame/vision/augmentations/base.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/vision/augmentations/boxes.py` & `torch-frame-1.7.3/torch_frame/vision/augmentations/boxes.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/vision/augmentations/colors.py` & `torch-frame-1.7.3/torch_frame/vision/augmentations/colors.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame/vision/tools/object_detection.py` & `torch-frame-1.7.3/torch_frame/vision/tools/object_detection.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.7.2/torch_frame.egg-info/PKG-INFO` & `torch-frame-1.7.3/torch_frame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-frame
-Version: 1.7.2
+Version: 1.7.3
 Summary: 用于深度学习快速实现代码的框架
 Home-page: https://github.com/darknli/Pytorch-Frame/tree/main/torch_frame
 Author: Darkn Lxs
 Author-email: 1187220556@qq.com
 License: UNKNOWN
 Description: 见readme
 Platform: UNKNOWN
```

### Comparing `torch-frame-1.7.2/torch_frame.egg-info/SOURCES.txt` & `torch-frame-1.7.3/torch_frame.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 torch_frame/hooks/checkpoint_hook.py
 torch_frame/hooks/eval_hook.py
 torch_frame/hooks/hookbase.py
 torch_frame/hooks/logger_hook.py
 torch_frame/utils/__init__.py
 torch_frame/utils/config_parser.py
 torch_frame/utils/dist_utils.py
+torch_frame/utils/ema.py
 torch_frame/utils/history_buffer.py
 torch_frame/utils/logger.py
 torch_frame/utils/metric.py
 torch_frame/utils/misc.py
 torch_frame/utils/progress_bar.py
 torch_frame/utils/test_speed.py
 torch_frame/vision/__init__.py
```

