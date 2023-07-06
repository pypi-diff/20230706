# Comparing `tmp/tkintertools-2.6.7.dev0.tar.gz` & `tmp/tkintertools-2.6.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.7.dev0.tar", last modified: Mon Jul  3 07:32:36 2023, max compression
+gzip compressed data, was "tkintertools-2.6.7.dev1.tar", last modified: Wed Jul  5 07:42:55 2023, max compression
```

## Comparing `tkintertools-2.6.7.dev0.tar` & `tkintertools-2.6.7.dev1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 07:32:36.042061 tkintertools-2.6.7.dev0/
--rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.7.dev0/LICENSE.txt
--rw-rw-rw-   0        0        0     9269 2023-07-03 07:32:36.041061 tkintertools-2.6.7.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     8635 2023-07-03 07:30:27.000000 tkintertools-2.6.7.dev0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 07:32:36.042061 tkintertools-2.6.7.dev0/setup.cfg
--rw-rw-rw-   0        0        0     1630 2023-07-03 07:26:30.000000 tkintertools-2.6.7.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 07:32:36.034789 tkintertools-2.6.7.dev0/tkintertools/
--rw-rw-rw-   0        0        0     2335 2023-07-03 06:46:57.000000 tkintertools-2.6.7.dev0/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    63639 2023-07-03 07:09:55.000000 tkintertools-2.6.7.dev0/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     2514 2023-07-03 06:06:54.000000 tkintertools-2.6.7.dev0/tkintertools/constants.py
--rw-rw-rw-   0        0        0    23455 2023-07-03 06:38:55.000000 tkintertools-2.6.7.dev0/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-07-03 07:32:36.040063 tkintertools-2.6.7.dev0/tkintertools.egg-info/
--rw-rw-rw-   0        0        0     9269 2023-07-03 07:32:35.000000 tkintertools-2.6.7.dev0/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-03 07:32:35.000000 tkintertools-2.6.7.dev0/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 07:32:35.000000 tkintertools-2.6.7.dev0/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 07:32:35.000000 tkintertools-2.6.7.dev0/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 07:42:55.428696 tkintertools-2.6.7.dev1/
+-rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.7.dev1/LICENSE.txt
+-rw-rw-rw-   0        0        0     9152 2023-07-05 07:42:55.428696 tkintertools-2.6.7.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     8518 2023-07-05 07:41:33.000000 tkintertools-2.6.7.dev1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-05 07:42:55.429698 tkintertools-2.6.7.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2023-07-05 07:10:06.000000 tkintertools-2.6.7.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:42:55.417320 tkintertools-2.6.7.dev1/tkintertools/
+-rw-rw-rw-   0        0        0     2335 2023-07-05 07:09:46.000000 tkintertools-2.6.7.dev1/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    63634 2023-07-04 05:00:55.000000 tkintertools-2.6.7.dev1/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     2514 2023-07-03 06:06:54.000000 tkintertools-2.6.7.dev1/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    24194 2023-07-05 07:07:35.000000 tkintertools-2.6.7.dev1/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:42:55.426697 tkintertools-2.6.7.dev1/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0     9152 2023-07-05 07:42:55.000000 tkintertools-2.6.7.dev1/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-05 07:42:55.000000 tkintertools-2.6.7.dev1/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 07:42:55.000000 tkintertools-2.6.7.dev1/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-05 07:42:55.000000 tkintertools-2.6.7.dev1/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.7.dev0/LICENSE.txt` & `tkintertools-2.6.7.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.7.dev0/PKG-INFO` & `tkintertools-2.6.7.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.7.dev0
+Version: 2.6.7.dev1
 Summary: An auxiliary module of the tkinter module.
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 Maintainer: Xiaokang2022
 Maintainer-email: 2951256653@qq.com
 License: MulanPSL-2.0
@@ -23,15 +23,15 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/03-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/05-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white?logo=about.me)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
@@ -55,25 +55,25 @@
 
 ```
 pip install tkintertools==2.6.6
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.7.dev0`
-* Release/发布日期 : 2023/07/03 (UTC+08)
+* Version/最新版本 : `2.6.7.dev1` (第 2 个预发布版本)
+* Release/发布日期 : 2023/07/05 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。  
 开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
 大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.7.dev0
+pip install tkintertools==2.6.7.dev1
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -94,28 +94,28 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.7.dev0`**
+**最新版本: `tkintertools-v2.6.7.dev1`**
 
 > **Note**  
 > 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev*`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！  
 > tkintertools 的介绍和使用教程均在 Wiki 中，[点我传送](https://github.com/Xiaokang2022/tkintertools/wiki)
 
 下面是本次版本更新内容条目：
 
-- [X] 新增常量 `ROTATE_CENTER`、`ORIGIN_COORDINATE`、`ORIGIN_SIZE`、`ORIGIN_WIDTH`、`ORIGIN_FILL` 和 `ORIGIN_OUTLINE`；
-- [X] 类 `Tk` 和 `Toplevel` 新增关键字参数 `alpha`、`toolwindow`、`topmost` 和 `transparentcolor`；
-- [X] 修复了类 `Text` 在使用鼠标滚轮滚动时会报错的 bug；
-- [X] 优化函数 `translate`、`rotate` 和 `scale` 内部的实现，提高了性能；
-- [X] 修改和完善了大量的不完整的文档注释；
-- [X] 将部分类的部分方法更改为保护方法；
+- [X] The function `rotate` of the 3D submodule adds the keyword `axis` to provide the function of rotating around the axis  
+3D 子模块的函数 `rotate` 新增关键字参数 `axis` 来提供绕轴旋转的功能
+- [X] Optimized some code and type hints  
+优化了部分代码和类型提示
+- [X] Removed abstract classes and abstract methods  
+移除了抽象类和抽象方法
 
 ### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
```

### Comparing `tkintertools-2.6.7.dev0/README.md` & `tkintertools-2.6.7.dev1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/03-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/05-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white?logo=about.me)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
@@ -37,25 +37,25 @@
 
 ```
 pip install tkintertools==2.6.6
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.7.dev0`
-* Release/发布日期 : 2023/07/03 (UTC+08)
+* Version/最新版本 : `2.6.7.dev1` (第 2 个预发布版本)
+* Release/发布日期 : 2023/07/05 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。  
 开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
 大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.7.dev0
+pip install tkintertools==2.6.7.dev1
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -76,28 +76,28 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.7.dev0`**
+**最新版本: `tkintertools-v2.6.7.dev1`**
 
 > **Note**  
 > 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev*`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！  
 > tkintertools 的介绍和使用教程均在 Wiki 中，[点我传送](https://github.com/Xiaokang2022/tkintertools/wiki)
 
 下面是本次版本更新内容条目：
 
-- [X] 新增常量 `ROTATE_CENTER`、`ORIGIN_COORDINATE`、`ORIGIN_SIZE`、`ORIGIN_WIDTH`、`ORIGIN_FILL` 和 `ORIGIN_OUTLINE`；
-- [X] 类 `Tk` 和 `Toplevel` 新增关键字参数 `alpha`、`toolwindow`、`topmost` 和 `transparentcolor`；
-- [X] 修复了类 `Text` 在使用鼠标滚轮滚动时会报错的 bug；
-- [X] 优化函数 `translate`、`rotate` 和 `scale` 内部的实现，提高了性能；
-- [X] 修改和完善了大量的不完整的文档注释；
-- [X] 将部分类的部分方法更改为保护方法；
+- [X] The function `rotate` of the 3D submodule adds the keyword `axis` to provide the function of rotating around the axis  
+3D 子模块的函数 `rotate` 新增关键字参数 `axis` 来提供绕轴旋转的功能
+- [X] Optimized some code and type hints  
+优化了部分代码和类型提示
+- [X] Removed abstract classes and abstract methods  
+移除了抽象类和抽象方法
 
 ### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
```

### Comparing `tkintertools-2.6.7.dev0/setup.py` & `tkintertools-2.6.7.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 9. 删除多余文件
 """
 
 import setuptools
 
 setuptools.setup(
     name='tkintertools',
-    version='2.6.7.dev0',
+    version='2.6.7.dev1',
     description='An auxiliary module of the tkinter module.',
     long_description=open('README.md', encoding='utf-8').read(),
     author='Xiaokang2022',
     author_email='2951256653@qq.com',
     maintainer='Xiaokang2022',
     maintainer_email='2951256653@qq.com',
     url='https://github.com/Xiaokang2022/tkintertools',
```

### Comparing `tkintertools-2.6.7.dev0/tkintertools/__init__.py` & `tkintertools-2.6.7.dev1/tkintertools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     error_info = '\n\033[31mOperation Requirements: \033[32m\nPython version shall not be less than\033[33m 3.8 !\033[0m'
     raise RuntimeError(error_info)
 
 from .__main__ import *
 from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
-__version__ = '2.6.7.dev0'
+__version__ = '2.6.7.dev1'
 __all__ = [
     # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
     # Virtual Canvas Widgets
     'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
     # Tool Classes
     'PhotoImage', 'Singleton',
```

### Comparing `tkintertools-2.6.7.dev0/tkintertools/__main__.py` & `tkintertools-2.6.7.dev1/tkintertools/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1581,21 +1581,20 @@
             initfont = ' '.join(str(i) for i in initfont)
         args += ['-font', initfont]
     if args:
         root.tk.call('tk', 'fontchooser', 'configure', *args)
     root.tk.call('tk', 'fontchooser', 'show')
 
 
-def SetProcessDpiAwareness(
-    awareness=PROCESS_SYSTEM_DPI_AWARE  # type: Literal[0, 1, 2]
-):  # type: (...) -> None
+def SetProcessDpiAwareness(awareness=PROCESS_SYSTEM_DPI_AWARE):
+    # type: (Literal[0, 1, 2]) -> None
     """
     ### 设定程序 DPI 级别
     设定窗口程序的 DPI 级别，让系统知道该如何对程序进行缩放，以提升高缩放倍数情况下的清晰度 \ 
     注意: 
     * 此函数仅在 Windows 平台上生效！
     * tkintertools 程序已内置该功能，该函数不应在 tkintertools 程序中使用，而应该在 tkinter 程序中使用！
     ---
     `awareness`: DPI 级别，值可以为 0、1 和 2，本来默认为 0，此处更改默认值为 1
     """
-    if WinDLL:
+    if WinDLL is not None:
         WinDLL('shcore').SetProcessDpiAwareness(awareness)
```

### Comparing `tkintertools-2.6.7.dev0/tkintertools/constants.py` & `tkintertools-2.6.7.dev1/tkintertools/constants.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.7.dev0/tkintertools/tools_3d.py` & `tkintertools-2.6.7.dev1/tkintertools/tools_3d.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,18 @@
 """ 3D support """
 
 import math  # 数学支持
 import statistics  # 数据统计
-from abc import ABCMeta, abstractmethod  # 抽象类
 from tkinter import Event  # 类型提示
-from typing import Iterable  # 类型提示
+from typing import Iterable, overload  # 类型提示
 
 from .__main__ import Canvas, Tk, Toplevel  # 继承和类型提示
 from .constants import *  # 常量
 
 
-def translate(coordinate, dx=0, dy=0, dz=0):
-    # type: (list[float], float, float, float) -> None
-    """
-    ### 平移
-    将一个三维空间中的点进行平移 \n
-    ---
-    `coordinate`: 点的空间坐标 \ 
-    `dx`: x 方向位移长度 \ 
-    `dy`: y 方向位移长度 \ 
-    `dz`: z 方向位移长度
-    """
-    for i, delta in enumerate((dx, dy, dz)):
-        coordinate[i] += delta
-
-
-def rotate(coordinate, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
-    # type: (list[float], float, float, float, ..., Iterable[float]) -> None
-    """
-    ### 旋转
-    将一个三维空间中的点以另一个点为旋转中心进行旋转 \n
-    ---
-    `coordinate`: 点的空间坐标 \ 
-    `dx`: x 方向旋转弧度 \ 
-    `dy`: y 方向旋转弧度 \ 
-    `dz`: z 方向旋转弧度 \ 
-    `center`: 旋转中心的空间坐标，默认值为元组 (0, 0, 0)
-    """
-    sx, sy, sz = math.sin(dx), math.sin(dy), math.sin(dz)
-    cx, cy, cz = math.cos(dx), math.cos(dy), math.cos(dz)
-
-    matrix = [[cz * cy, cz * sy * sx - sz * cx, cz * sy * cx + sz * sx],
-              [sz * cy, sz * sy * sx + cz * cx, sz * sy * cx - cz * sx],
-              [-sy,     cy * sx,                cy * cx]]
-
-    for i, c_i in enumerate(center):
-        matrix[0][i] = c_i + sum(
-            matrix[i][j] * (coordinate[j] - c_j) for j, c_j in enumerate(center))
-
-    coordinate[:] = matrix[0]
-
-
-def scale(coordinate, kx=1, ky=1, kz=1, *, center):
-    # type: (list[float], float, float, float, ..., Iterable[float]) -> None
-    """
-    ### 缩放
-    将一个三维空间中的点以另一个点为缩放中心进行缩放 \n
-    ---
-    `coordinate`: 点的空间坐标 \ 
-    `kx`: x 方向缩放比例 \ 
-    `ky`: y 方向缩放比例 \ 
-    `kz`: z 方向缩放比例 \ 
-    `center`: 缩放中心的空间坐标
-    """
-    if kx <= 0 or ky <= 0 or kz <= 0:  # 限制缩放比例的范围
-        raise ValueError('invalid scaling factor')
-    for i, k in enumerate((kx, ky, kz)):
-        coordinate[i] += (coordinate[i] - center[i]) * (k - 1)
-
-
 class Canvas_3D(Canvas):
     """ 3D 画布基类 """
 
     def __init__(
         self,
         master,  # type: Tk | Toplevel
         width,  # type: int
@@ -206,163 +146,228 @@
             return self.configure(cursor='fleur')
         elif flag is False:
             return self.configure(cursor='arrow')
         dx, dy = event.x-_cache[0], event.y-_cache[1]
         _cache[:] = [event.x, event.y]
         for item in self._items_3d:
             item.rotate(0, -2*dy/self.width[1]*math.tau, 2*dx /
-                        self.height[1]*math.tau, center=self._origin.coords)
+                        self.height[1]*math.tau, center=self._origin.coordinates[0])
             item.update()
         self.space_sort()
 
     def _scale(self, event, flag=None):  # type: (Event, bool | None) -> None
         """ 缩放事件 """
         if flag is not None:
             event.delta = flag
         k = 1.1 if event.delta > 0 else 0.9
         for item in self._items_3d:
-            item.scale(k, k, k, center=self._origin.coords)
+            item.scale(k, k, k, center=self._origin.coordinates[0])
             item.update()
         self.space_sort()
 
 
-class _3D_Object(metaclass=ABCMeta):
-    """ 3D 对象抽象元类 """
+def translate(coordinate, dx=0, dy=0, dz=0):
+    # type: (list[float], float, float, float) -> None
+    """
+    ### 平移
+    将一个三维空间中的点进行平移 \n
+    ---
+    `coordinate`: 点的空间坐标 \ 
+    `dx`: x 方向位移长度 \ 
+    `dy`: y 方向位移长度 \ 
+    `dz`: z 方向位移长度
+    """
+    for i, delta in enumerate((dx, dy, dz)):
+        coordinate[i] += delta
+
+
+@overload
+def rotate(coordinate, dx=0, dy=0, dz=0, *, center):
+    # type: (list[float], float, float, float, ..., Iterable[float]) -> None
+    ...
+
+
+@overload
+def rotate(coordinate, dx=0, *, axis):
+    # type: (list[float], float,  ..., Iterable[Iterable[float]]) -> None
+    ...
+
+
+def rotate(coordinate, dx=0, dy=0, dz=0, *, center, axis):
+    # type: (list[float], float, float, float, ..., Iterable[float], Iterable[Iterable[float]] | None) -> None
+    """
+    ### 旋转
+    将一个三维空间中的点以一个点或线为参照进行旋转 \n
+    ---
+    `coordinate`: 点的空间坐标 \ 
+    `dx`: x 方向旋转弧度，或者绕旋转轴线的旋转弧度 \ 
+    `dy`: y 方向旋转弧度 \ 
+    `dz`: z 方向旋转弧度 \ 
+    `center`: 旋转中心的空间坐标 \ 
+    `axis`: 旋转轴线的空间坐标
+    """
+    if axis is not None:  # 参照为线（定轴转动）
+        center = _Line(*axis).center()
+        n = list(axis[0])
+        for i in range(3):
+            n[i] -= axis[1][i]
+            coordinate[i] -= center[i]
+        n_m = math.hypot(*n)
+        for i in range(3):
+            n[i] /= n_m
+        x_2, y_2, z_2 = (i**2 for i in n)
+        xy, yz, zx = n[0]*n[1], n[1]*n[2], n[2]*n[0]
+        s_θ, c_θ = math.sin(dx), math.cos(dx)
+        _c_θ = 1 - c_θ
+
+        matrix = [[x_2*_c_θ + c_θ, xy*_c_θ + n[2]*s_θ, zx*_c_θ - n[1]*s_θ],
+                  [xy*_c_θ - n[2]*s_θ, y_2*_c_θ + c_θ, yz*_c_θ + n[0]*s_θ],
+                  [zx*_c_θ + n[1]*s_θ, yz*_c_θ - n[0]*s_θ, z_2*_c_θ + c_θ]]
+
+        for i, δ in enumerate(center):
+            matrix[i] = δ + sum(matrix[i][j]*coordinate[j] for j in range(3))
+
+    else:  # 参照为点（定点转动）
+        sx, sy, sz = math.sin(dx), math.sin(dy), math.sin(dz)
+        cx, cy, cz = math.cos(dx), math.cos(dy), math.cos(dz)
+
+        matrix = [[cz * cy, cz * sy * sx - sz * cx, cz * sy * cx + sz * sx],
+                  [sz * cy, sz * sy * sx + cz * cx, sz * sy * cx - cz * sx],
+                  [-sy,     cy * sx,                cy * cx]]
+
+        for i, δ in enumerate(center):
+            matrix[i] = δ + sum(
+                matrix[i][j] * (coordinate[j] - center[j]) for j in range(3))
+
+    coordinate[:] = matrix
+
 
-    @abstractmethod
-    def translate(self, dx=0, dy=0, dz=0):
+def scale(coordinate, kx=1, ky=1, kz=1, *, center):
+    # type: (list[float], float, float, float, ..., Iterable[float]) -> None
+    """
+    ### 缩放
+    将一个三维空间中的点以另一个点为缩放中心进行缩放 \n
+    ---
+    `coordinate`: 点的空间坐标 \ 
+    `kx`: x 方向缩放比例 \ 
+    `ky`: y 方向缩放比例 \ 
+    `kz`: z 方向缩放比例 \ 
+    `center`: 缩放中心的空间坐标
+    """
+    if kx <= 0 or ky <= 0 or kz <= 0:  # 限制缩放比例的范围
+        raise ValueError('invalid scaling factor')
+    for i, k in enumerate((kx, ky, kz)):
+        coordinate[i] += (coordinate[i] - center[i]) * (k - 1)
+
+
+class _3D_Object:
+    """ 3D 对象基类 """
+
+    def __init__(self, *coordinates):  # type: (list[float]) -> None
+        self.coordinates = list(coordinates)  # 所有点的坐标
+
+    def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """
         ### 平移
         `dx`: x 方向位移长度 \ 
         `dy`: y 方向位移长度 \ 
         `dz`: z 方向位移长度
         """
+        for coordinate in self.coordinates:
+            translate(coordinate, dx, dy, dz)
 
-    @abstractmethod
+    @overload
     def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
+        # type: (float, float, float, ..., Iterable[float]) -> None
+        ...
+
+    @overload
+    def rotate(self, dx=0, *, axis):
+        # type: (float, ..., Iterable[Iterable[float]]) -> None
+        ...
+
+    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER, axis=None):
+        # type: (float, float, float, ..., Iterable[float], Iterable[Iterable[float]] | None) -> None
         """
         ### 旋转
-        `dx`: x 方向旋转弧度 \ 
+        `dx`: x 方向旋转弧度，或者绕旋转轴线的旋转弧度 \ 
         `dy`: y 方向旋转弧度 \ 
         `dz`: z 方向旋转弧度 \ 
-        `center`: 旋转中心，默认为原点
+        `center`: 旋转中心，默认为原点 \ 
+        `axis`: 旋转轴线，无默认值
         """
+        for coordinate in self.coordinates:
+            rotate(coordinate, dx, dy, dz, center=center, axis=axis)
 
-    @abstractmethod
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
+        # type: (float, float, float, ..., Iterable[float] | None) -> None
         """
         ### 缩放
         `kx`: x 方向缩放比例 \ 
         `ky`: y 方向缩放比例 \ 
         `kz`: z 方向缩放比例 \ 
         `center`: 缩放中心，默认为几何中心
         """
+        if center is None:
+            center = self.center()
+        for coordinate in self.coordinates:
+            scale(coordinate, kx, ky, kz, center=center)
 
-    @abstractmethod
-    def center(self):
+    def center(self):  # type: () -> tuple[float, float, float]
         """ 几何中心 """
+        return tuple(statistics.mean(xyz) for xyz in zip(*self.coordinates))
 
-    @abstractmethod
     def _project(self, distance):
         """
         ### 投影
         `distance`: 对象与观察者的距离
         """
 
 
 class _Point(_3D_Object):
     """ 点（基类） """
 
-    def __init__(self, coords):  # type: (list[float]) -> None
-        self.coords = coords  # 利用列表引用
-
-    def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        translate(self.coords, dx, dy, dz)
-
-    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
-        # type: (float, float, float, ..., Iterable[float]) -> None
-        rotate(self.coords, dx, dy, dz, center=center)
-
-    def scale(self, kx=1, ky=1, kz=1, *, center=None):
-        # type: (float, float, float, ..., Iterable[float] | None) -> None
-        scale(self.coords, kx, ky, kz, center=center)
-
-    def center(self):  # type: () -> tuple[float, float, float]
-        return tuple(self.coords)
+    def __init__(self, coordinate):  # type: (list[float]) -> None
+        _3D_Object.__init__(self, coordinate)
 
     def _project(self, distance):  # type: (float) -> list[float]
-        relative_dis = distance - self.coords[0]
+        # override: 具体的实现
+        relative_dis = distance - self.coordinates[0][0]
         if relative_dis <= 1e-16:
             return [float('inf')]*2  # BUG: 目前超出范围只能让其消失
         k = distance/relative_dis
-        return [self.coords[1]*k, self.coords[2]*k]
+        return [self.coordinates[0][1]*k, self.coordinates[0][2]*k]
 
 
 class _Line(_3D_Object):
     """ 线（基类） """
 
     def __init__(
         self,
-        point_start,  # type: list[float]
-        point_end,  # type: list[float]
+        start,  # type: list[float]
+        end,  # type: list[float]
     ):  # type: (...) -> None
-        self.coords = [point_start, point_end]
-        self.points = [_Point(point) for point in self.coords]
-
-    def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        for coord in self.coords:
-            translate(coord, dx, dy, dz)
-
-    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
-        # type: (float, float, float, ..., Iterable[float]) -> None
-        for coord in self.coords:
-            rotate(coord, dx, dy, dz, center=center)
-
-    def scale(self, kx=1, ky=1, kz=1, *, center=None):
-        # type: (float, float, float, ..., Iterable[float] | None) -> None
-        if center is None:
-            center = self.center()
-        for coord in self.coords:
-            scale(coord, kx, ky, kz, center=center)
-
-    def center(self):  # type: () -> tuple[float, float, float]
-        return tuple(statistics.mean(coords) for coords in zip(*self.coords))
+        _3D_Object.__init__(self, start, end)
+        self.points = [_Point(start), _Point(end)]
 
     def _project(self, distance):  # type: (float) -> list[list[float]]
+        # override: 具体的实现
         return [point._project(distance) for point in self.points]
 
 
 class _Side(_3D_Object):
     """ 面（基类） """
 
-    def __init__(self, *points):  # type: (list[float]) -> None
-        self.coords = list(points)
-        self.lines = [_Line(points[ind-1], points[ind])
-                      for ind in range(len(points))]
-
-    def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        for coord in self.coords:
-            translate(coord, dx, dy, dz)
-
-    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
-        # type: (float, float, float, ..., Iterable[float]) -> None
-        for coord in self.coords:
-            rotate(coord, dx, dy, dz, center=center)
-
-    def scale(self, kx=1, ky=1, kz=1, *, center=None):
-        # type: (float, float, float, ..., Iterable[float] | None) -> None
-        if center is None:
-            center = self.center()
-        for coord in self.coords:
-            scale(coord, kx, ky, kz, center=center)
-
-    def center(self):  # type: () -> tuple[float, float, float]
-        return tuple(statistics.mean(coords) for coords in zip(*self.coords))
+    def __init__(self, *coordinates):  # type: (list[float]) -> None
+        _3D_Object.__init__(self, *coordinates)
+        self.lines = [_Line(coordinates[index-1], coordinate)
+                      for index, coordinate in enumerate(coordinates)]
 
     def _project(self, distance):  # type: (float) -> list[list[list[float]]]
+        # override: 具体的实现
         return [line._project(distance) for line in self.lines]
 
 
 class Point(_Point):
     """ 点 """
 
     def __init__(
@@ -397,16 +402,16 @@
         """ 更新对象的显示 """
         x, y = self._project(self.canvas.distance)
         self.canvas.coords(self.item, (x-self.size)*self.canvas.rx, (y-self.size) *
                            self.canvas.ry, (x+self.size)*self.canvas.rx, (y+self.size)*self.canvas.ry)
 
     def _camera_distance(self):  # type: () -> float
         """ 与相机距离 """
-        sign = math.copysign(1, self.canvas.distance - self.coords[0])
-        return sign*math.dist([self.canvas.distance, 0, 0], self.coords)
+        sign = math.copysign(1, self.canvas.distance - self.coordinates[0][0])
+        return sign*math.dist([self.canvas.distance, 0, 0], self.coordinates[0])
 
 
 class Line(_Line):
     """ 线 """
 
     def __init__(
         self,
@@ -506,25 +511,36 @@
         `dx`: x 方向位移长度 \ 
         `dy`: y 方向位移长度 \ 
         `dz`: z 方向位移长度
         """
         for side in self.sides:
             side.translate(dx, dy, dz)
 
+    @overload
     def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
         # type: (float, float, float, ..., Iterable[float]) -> None
+        ...
+
+    @overload
+    def rotate(self, dx=0, *, axis):
+        # type: (float, ..., Iterable[Iterable[float]]) -> None
+        ...
+
+    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER, axis=None):
+        # type: (float, float, float, ..., Iterable[float], Iterable[Iterable[float]] | None) -> None
         """
         ### 旋转
-        `dx`: x 方向旋转弧度 \ 
+        `dx`: x 方向旋转弧度，或者绕旋转轴线的旋转弧度 \ 
         `dy`: y 方向旋转弧度 \ 
         `dz`: z 方向旋转弧度 \ 
-        `center`: 旋转中心，默认为原点
+        `center`: 旋转中心，默认为原点 \ 
+        `axis`: 旋转轴线，无默认值
         """
         for side in self.sides:
-            side.rotate(dx, dy, dz, center=center)
+            side.rotate(dx, dy, dz, center=center, axis=axis)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         """
         ### 缩放
         `kx`: x 方向缩放比例 \ 
         `ky`: y 方向缩放比例 \ 
@@ -535,15 +551,15 @@
             center = self.center()
         for side in self.sides:
             side.scale(kx, ky, kz, center=center)
 
     def center(self):  # type: () -> tuple[float, float, float]
         """ 几何中心 """
         # BUG: 公式对凹面几何体不成立
-        return tuple(statistics.mean(axis) for axis in zip(*set(tuple(coord) for side in self.sides for coord in side.coords)))
+        return tuple(statistics.mean(axis) for axis in zip(*set(tuple(coord) for side in self.sides for coord in side.coordinates)))
 
     def update(self):  # type: () -> None
         """ 更新几何体 """
         for side in self.sides:
             side.update()
 
     def append(self, *sides):  # type: (Side) -> None
```

### Comparing `tkintertools-2.6.7.dev0/tkintertools.egg-info/PKG-INFO` & `tkintertools-2.6.7.dev1/tkintertools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.7.dev0
+Version: 2.6.7.dev1
 Summary: An auxiliary module of the tkinter module.
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 Maintainer: Xiaokang2022
 Maintainer-email: 2951256653@qq.com
 License: MulanPSL-2.0
@@ -23,15 +23,15 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/03-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/05-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white?logo=about.me)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
@@ -55,25 +55,25 @@
 
 ```
 pip install tkintertools==2.6.6
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.7.dev0`
-* Release/发布日期 : 2023/07/03 (UTC+08)
+* Version/最新版本 : `2.6.7.dev1` (第 2 个预发布版本)
+* Release/发布日期 : 2023/07/05 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。  
 开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
 大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.7.dev0
+pip install tkintertools==2.6.7.dev1
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -94,28 +94,28 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.7.dev0`**
+**最新版本: `tkintertools-v2.6.7.dev1`**
 
 > **Note**  
 > 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev*`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！  
 > tkintertools 的介绍和使用教程均在 Wiki 中，[点我传送](https://github.com/Xiaokang2022/tkintertools/wiki)
 
 下面是本次版本更新内容条目：
 
-- [X] 新增常量 `ROTATE_CENTER`、`ORIGIN_COORDINATE`、`ORIGIN_SIZE`、`ORIGIN_WIDTH`、`ORIGIN_FILL` 和 `ORIGIN_OUTLINE`；
-- [X] 类 `Tk` 和 `Toplevel` 新增关键字参数 `alpha`、`toolwindow`、`topmost` 和 `transparentcolor`；
-- [X] 修复了类 `Text` 在使用鼠标滚轮滚动时会报错的 bug；
-- [X] 优化函数 `translate`、`rotate` 和 `scale` 内部的实现，提高了性能；
-- [X] 修改和完善了大量的不完整的文档注释；
-- [X] 将部分类的部分方法更改为保护方法；
+- [X] The function `rotate` of the 3D submodule adds the keyword `axis` to provide the function of rotating around the axis  
+3D 子模块的函数 `rotate` 新增关键字参数 `axis` 来提供绕轴旋转的功能
+- [X] Optimized some code and type hints  
+优化了部分代码和类型提示
+- [X] Removed abstract classes and abstract methods  
+移除了抽象类和抽象方法
 
 ### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
```

