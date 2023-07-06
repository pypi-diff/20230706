# Comparing `tmp/Zeraora-0.3.2.tar.gz` & `tmp/Zeraora-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.3.2.tar", last modified: Thu Jun 29 01:45:57 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.3.3.tar", last modified: Thu Jul  6 06:36:38 2023, max compression
```

## Comparing `Zeraora-0.3.2.tar` & `Zeraora-0.3.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:45:57.000000 Zeraora-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-29 01:45:57.000000 Zeraora-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-29 01:45:42.000000 Zeraora-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:45:57.000000 Zeraora-0.3.2/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-29 01:45:57.000000 Zeraora-0.3.2/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-29 01:45:57.000000 Zeraora-0.3.2/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 01:45:57.000000 Zeraora-0.3.2/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 01:45:57.000000 Zeraora-0.3.2/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 01:45:57.000000 Zeraora-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-29 01:45:43.000000 Zeraora-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:45:57.000000 Zeraora-0.3.2/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:45:57.000000 Zeraora-0.3.2/zeraora/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/constants/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/constants/chores.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/constants/division.py
--rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:45:57.000000 Zeraora-0.3.2/zeraora/dj/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/dj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/dj/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/dj/lookups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/dj/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:45:57.000000 Zeraora-0.3.2/zeraora/drf/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/drf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/drf/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/drf/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/gvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/typeclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-06-29 01:45:43.000000 Zeraora-0.3.2/zeraora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-06 06:36:38.000000 Zeraora-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-06 06:36:21.000000 Zeraora-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-06 06:36:38.000000 Zeraora-0.3.3/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-06 06:36:38.000000 Zeraora-0.3.3/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:36:38.000000 Zeraora-0.3.3/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 06:36:38.000000 Zeraora-0.3.3/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 06:36:38.000000 Zeraora-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-06 06:36:21.000000 Zeraora-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/zeraora/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/constants/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/constants/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/constants/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/zeraora/dj/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/dj/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/dj/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/dj/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/zeraora/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/drf/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/gvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/throwables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26295 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/typeclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/utils.py
```

### Comparing `Zeraora-0.3.2/PKG-INFO` & `Zeraora-0.3.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.3.2
-Summary: 实际应用积累的长期维护的实用开源工具库。A utility Python package for our personal and corporate projects, with long time support.
+Version: 0.3.3
+Summary: 为了跨平台跨项目复用代码而开发的工具库。A utility Python package for our personal and corporate projects, with long time support.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
 Description: <h1 align="center" style="padding-top: 32px">Zeraora</h1>
@@ -15,32 +15,32 @@
             <a href="https://en.wikipedia.org/wiki/MIT_License"><img src="https://img.shields.io/pypi/l/Zeraora?color=purple"></a>
             <a href="https://pypi.org/project/Zeraora/"><img src="https://img.shields.io/pypi/v/zeraora?color=darkgreen"></a>
             <a href=""><img src="https://img.shields.io/pypi/dm/zeraora?color=C72777"></a>
             <a href=""><img src="https://img.shields.io/pypi/status/Zeraora"></a>
             <!--a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a-->
         </div>
         <div align="center">
-            <i>实际应用积累的长期维护的实用开源工具库</i>
+            <i>为了跨平台跨项目复用代码而开发的工具库</i>
             <br>
             <i>A utility Python package for our personal and corporate projects, with long time support</i>
         </div>
         
         
         ## 特性
         
         - 支持with、注解和实例化三种方式调用的计时器 `BearTimer` ；
         - 生成通用representation方便调试时查看对象内部信息的 `ReprMixin` ；
         - 将字典的任意层级递归转化为对象，以便支持点分法访问数据的 `OnionObject` ；
-        - 受 Django 的 `Choices` 和 Java 原生枚举语法启发的、可为枚举添加任意属性的 `Items` ；
+        - 受 Django 的 `Choices` 启发和 Java 原生枚举影响的、可为枚举添加任意属性的 `Items` ；
         - 用以简化 `.as_view()` 传参的 `EasyViewSetMixin` ；
         - 仿照 `DestroyModelMixin` 实现的 `SoftDeleteModelMixin` ；
         - 自动为Django模型生成下划线小写（即蛇形）数据表名的 `SnakeModel` ；
         - 包含34个省级行政区名称、区划代码、字母码、大区、简称、缩写的枚举 `Province` ；
         - 不强制依赖任何非[标准库](https://docs.python.org/zh-cn/3/library/index.html)；
-        - 更多……
+        - 更多符号见[Zeraora全局符号索引](./docs/README.md)。
         
         ## 安装
         
         使用 pip 直接安装：
         
         ```shell
         pip install zeraora
@@ -54,38 +54,53 @@
         
         使用 pip 时临时指定安装源来安装：
         
         ```shell
         pip install zeraora -i http://pypi.mirrors.ustc.edu.cn/simple/
         ```
         
-        ## 文档
-        
-        见[全局符号索引](./docs/README.md)。
+        因为没有需求，所以还没有创建 conda 版本。
         
         ## 版本
         
-        |       | 状态[^1] | 维护时间 | 依赖[^2]          | 备注                                                         |
-        | ----- | -------- | -------- | ----------------- | ------------------------------------------------------------ |
-        | 0.3.x | 🆕feature | 长期     | Python 3.7 或更新 | **分支**：main<br/>趋于稳定，但改了包结构，没办法向下兼容。  |
-        | 0.2.x | ✅bugfix  | 长期     | Python 3.7 或更新 | **分支**：0.2.x<br/>探索包结构，完善核心特性，补充非核心特性。 |
-        | 0.1.x | ❌EOL     | 不再维护 | Python 3.7 或更新 | **分支**：release/*<br/>试验自动部署，只有核心特性。         |
+        |       | 状态      | 维护结束时间 | 首版时间   | 安全版本 | 分支  | 依赖 |
+        | ----- | --------- | ------------ | ---------- | -------- | ----- | ---- |
+        | 0.3.x | 🆕feature  | ~ 0.5.x      | 2023.06.09 | -        | main  | 3.7+ |
+        | 0.2.x | ✅security | ~ 0.4.x      | 2023.04.12 | 0.2.14   | 0.2.x | 3.7+ |
+        | 0.1.x | ❌EOL      | 2023.06.09   | 2023.03.27 | -        | 0.1.x | 3.7+ |
+        
+        - 状态
+          - feature 指功能还在开发或测试，回退子版本可能会出现兼容性问题。
+          - security 指功能已经稳定，回退不会出现兼容性问题；会为问题修复发布新的子版本，但不会迁移新版功能。
+          - EOL 指已经停止维护，不会处理与之相关的任何问题，也不会发布新的子版本。
+          - 没有 prerelease 状态，因为这个状态通常不会发布包，进而难以测试。
         
-        [^1]: 概念参见[Python版本状态](https://devguide.python.org/versions/#status-key)。
-        [^2]: 仅在最低依赖版本中进行(过)单元测试。
+        - 维护结束时间
+          - 一般是到下下一个版本的安全版本发布为止。
         
-        ## 分支
+        - 安全版本
+          - 指的是 security 状态开始的那一个版本，这个版本往后的那些版本可以安全回退。
         
-        主分支将从名为 `master` 的分支切换为 `main` 并且于2023年6月12日删除前者（自动同步不好做所以躺平了），原因是 `main` 听起来确实比前者要舒服一点点，若要深究的话参见[这里](https://stackoverflow.com/a/65021103)。两条分支是完全一致的，换句话说，后续的更新**就是**在 `master` 基础上进行的。
+        - 依赖
+          - 对于 Python 版本的依赖，例如 3.7+ 指的是需要 3.7 或更新的 Python。
         
-        ## 帮助
         
-        这个包偏向于抽象及封装一些实际在用的实用功能，目前整体趋于稳定，如需部署生产环境，请优先考虑 0.3.x 或后续更新的版本。
+        ## 文档
+        
+        详见[全局符号索引](./docs/README.md)。
+        
+        ## 开发
+        
+        这个库只是为了跨平台、跨项目复用代码而已。有些是直接封装实际在用的功能，有些是在库里开发然后通过pip依赖传递给各个项目，有些可能真的只是奇思妙想灵光乍现。如果你有同样的需求，也认可这份努力，那么欢迎加入。
+        
+        详见[开发指南](./CONTRIBUTING.md)。
+        
+        ## 帮助
         
-        欢迎通过 Issue 或 Pull Request 来提出功能创意、命名建议，亦或反馈问题、修复漏洞、编写测试等等等等；如有需要，可以进入QQ群 699090940 获取帮助。
+        可以通过 Issue 反馈，或通过 Pull Request 添加你的工具；如有需要，可以进入QQ群 699090940 获取非即时性的帮助。
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,63 +1,68 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.3.2 Summary:
-å®éåºç¨ç§¯ç´¯çé¿æç»´æ¤çå®ç¨å¼æºå·¥å·åºãA utility Python
+Metadata-Version: 2.1 Name: Zeraora Version: 0.3.3 Summary:
+ä¸ºäºè·¨å¹³å°è·¨é¡¹ç®å¤ç¨ä»£ç èå¼åçå·¥å·åºãA utility Python
 package for our personal and corporate projects, with long time support. Home-
 page: https://github.com/aixcyi/zeraora Author: aixcyi Author-email:
 75880483+aixcyi@users.noreply.github.com License: MIT Project-URL: Source,
 https://github.com/aixcyi/zeraora Project-URL: Tracker, https://github.com/
 aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
 [https://img.shields.io/pypi/pyversions/zeraora?logo=python&logoColor=yellow]
  [https://img.shields.io/pypi/l/Zeraora?color=purple] [https://img.shields.io/
        pypi/v/zeraora?color=darkgreen] [https://img.shields.io/pypi/dm/
       zeraora?color=C72777] [https://img.shields.io/pypi/status/Zeraora]
-          å®éåºç¨ç§¯ç´¯çé¿æç»´æ¤çå®ç¨å¼æºå·¥å·åº
+          ä¸ºäºè·¨å¹³å°è·¨é¡¹ç®å¤ç¨ä»£ç èå¼åçå·¥å·åº
   A utility Python package for our personal and corporate projects, with long
                                  time support
 ## ç¹æ§ - æ¯æwithãæ³¨è§£åå®ä¾åä¸ç§æ¹å¼è°ç¨çè®¡æ¶å¨
 `BearTimer` ï¼ -
 çæéç¨representationæ¹ä¾¿è°è¯æ¶æ¥çå¯¹è±¡åé¨ä¿¡æ¯ç
 `ReprMixin` ï¼ -
 å°å­å¸çä»»æå±çº§éå½è½¬åä¸ºå¯¹è±¡ï¼ä»¥ä¾¿æ¯æç¹åæ³è®¿é®æ°æ®ç
-`OnionObject` ï¼ - å Django ç `Choices` å Java
-åçæä¸¾è¯­æ³å¯åçãå¯ä¸ºæä¸¾æ·»å ä»»æå±æ§ç `Items` ï¼ -
+`OnionObject` ï¼ - å Django ç `Choices` å¯åå Java
+åçæä¸¾å½±åçãå¯ä¸ºæä¸¾æ·»å ä»»æå±æ§ç `Items` ï¼ -
 ç¨ä»¥ç®å `.as_view()` ä¼ åç `EasyViewSetMixin` ï¼ - ä»¿ç§
 `DestroyModelMixin` å®ç°ç `SoftDeleteModelMixin` ï¼ -
 èªå¨ä¸ºDjangoæ¨¡åçæä¸åçº¿å°åï¼å³èå½¢ï¼æ°æ®è¡¨åç
 `SnakeModel` ï¼ -
 åå«34ä¸ªççº§è¡æ¿åºåç§°ãåºåä»£ç ãå­æ¯ç ãå¤§åºãç®ç§°ãç¼©åçæä¸¾
 `Province` ï¼ - ä¸å¼ºå¶ä¾èµä»»ä½é[æ ååº](https://docs.python.org/
-zh-cn/3/library/index.html)ï¼ - æ´å¤â¦â¦ ## å®è£ ä½¿ç¨ pip
-ç´æ¥å®è£ï¼ ```shell pip install zeraora ``` ä¸´æ¶éè¿æ¬å°ä»£çä½¿ç¨
-pip å®è£ï¼ ```shell pip install zeraora --proxy=127.0.0.1:6666 ``` ä½¿ç¨
-pip æ¶ä¸´æ¶æå®å®è£æºæ¥å®è£ï¼ ```shell pip install zeraora -i http:/
-/pypi.mirrors.ustc.edu.cn/simple/ ``` ## ææ¡£ è§[å¨å±ç¬¦å·ç´¢å¼](./docs/
-README.md)ã ## çæ¬ | | ç¶æ[^1] | ç»´æ¤æ¶é´ | ä¾èµ[^2] | å¤æ³¨ | |
------ | -------- | -------- | ----------------- | -----------------------------
-------------------------------- | | 0.3.x | ðfeature | é¿æ | Python 3.7
-ææ´æ° | **åæ¯**ï¼main
-è¶äºç¨³å®ï¼ä½æ¹äºåç»æï¼æ²¡åæ³åä¸å¼å®¹ã | | 0.2.x |
-âbugfix | é¿æ | Python 3.7 ææ´æ° | **åæ¯**ï¼0.2.x
-æ¢ç´¢åç»æï¼å®åæ ¸å¿ç¹æ§ï¼è¡¥åéæ ¸å¿ç¹æ§ã | | 0.1.x |
-âEOL | ä¸åç»´æ¤ | Python 3.7 ææ´æ° | **åæ¯**ï¼release/*
-è¯éªèªå¨é¨ç½²ï¼åªææ ¸å¿ç¹æ§ã | [^1]: æ¦å¿µåè§
-[Pythonçæ¬ç¶æ](https://devguide.python.org/versions/#status-key)ã [^2]:
-ä»å¨æä½ä¾èµçæ¬ä¸­è¿è¡(è¿)ååæµè¯ã ## åæ¯
-ä¸»åæ¯å°ä»åä¸º `master` çåæ¯åæ¢ä¸º `main`
-å¹¶ä¸äº2023å¹´6æ12æ¥å é¤åèï¼èªå¨åæ­¥ä¸å¥½åæä»¥èººå¹³äºï¼ï¼åå æ¯
-`main` å¬èµ·æ¥ç¡®å®æ¯åèè¦èæä¸ç¹ç¹ï¼è¥è¦æ·±ç©¶çè¯åè§
-[è¿é](https://stackoverflow.com/a/
-65021103)ãä¸¤æ¡åæ¯æ¯å®å¨ä¸è´çï¼æ¢å¥è¯è¯´ï¼åç»­çæ´æ°**å°±æ¯**å¨
-`master` åºç¡ä¸è¿è¡çã ## å¸®å©
-è¿ä¸ªåååäºæ½è±¡åå°è£ä¸äºå®éå¨ç¨çå®ç¨åè½ï¼ç®åæ´ä½è¶äºç¨³å®ï¼å¦éé¨ç½²çäº§ç¯å¢ï¼è¯·ä¼åèè
-0.3.x æåç»­æ´æ°ççæ¬ã æ¬¢è¿éè¿ Issue æ Pull Request
-æ¥æåºåè½åæãå½åå»ºè®®ï¼äº¦æåé¦é®é¢ãä¿®å¤æ¼æ´ãç¼åæµè¯ç­ç­ç­ç­ï¼å¦æéè¦ï¼å¯ä»¥è¿å¥QQç¾¤
-699090940 è·åå¸®å©ã Platform: UNKNOWN Classifier: Development Status :: 4
-- Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: Intended
-Audience :: Developers Classifier: Operating System :: OS Independent
+zh-cn/3/library/index.html)ï¼ - æ´å¤ç¬¦å·è§[Zeraoraå¨å±ç¬¦å·ç´¢å¼](./
+docs/README.md)ã ## å®è£ ä½¿ç¨ pip ç´æ¥å®è£ï¼ ```shell pip install
+zeraora ``` ä¸´æ¶éè¿æ¬å°ä»£çä½¿ç¨ pip å®è£ï¼ ```shell pip install
+zeraora --proxy=127.0.0.1:6666 ``` ä½¿ç¨ pip
+æ¶ä¸´æ¶æå®å®è£æºæ¥å®è£ï¼ ```shell pip install zeraora -i http://
+pypi.mirrors.ustc.edu.cn/simple/ ``` å ä¸ºæ²¡æéæ±ï¼æä»¥è¿æ²¡æåå»º
+conda çæ¬ã ## çæ¬ | | ç¶æ | ç»´æ¤ç»ææ¶é´ | é¦çæ¶é´ |
+å®å¨çæ¬ | åæ¯ | ä¾èµ | | ----- | --------- | ------------ | ---------
+- | -------- | ----- | ---- | | 0.3.x | ðfeature | ~ 0.5.x | 2023.06.09 | -
+| main | 3.7+ | | 0.2.x | âsecurity | ~ 0.4.x | 2023.04.12 | 0.2.14 | 0.2.x |
+3.7+ | | 0.1.x | âEOL | 2023.06.09 | 2023.03.27 | - | 0.1.x | 3.7+ | - ç¶æ
+- feature
+æåè½è¿å¨å¼åææµè¯ï¼åéå­çæ¬å¯è½ä¼åºç°å¼å®¹æ§é®é¢ã
+- security
+æåè½å·²ç»ç¨³å®ï¼åéä¸ä¼åºç°å¼å®¹æ§é®é¢ï¼ä¼ä¸ºé®é¢ä¿®å¤åå¸æ°çå­çæ¬ï¼ä½ä¸ä¼è¿ç§»æ°çåè½ã
+- EOL
+æå·²ç»åæ­¢ç»´æ¤ï¼ä¸ä¼å¤çä¸ä¹ç¸å³çä»»ä½é®é¢ï¼ä¹ä¸ä¼åå¸æ°çå­çæ¬ã
+- æ²¡æ prerelease
+ç¶æï¼å ä¸ºè¿ä¸ªç¶æéå¸¸ä¸ä¼åå¸åï¼è¿èé¾ä»¥æµè¯ã -
+ç»´æ¤ç»ææ¶é´ -
+ä¸è¬æ¯å°ä¸ä¸ä¸ä¸ªçæ¬çå®å¨çæ¬åå¸ä¸ºæ­¢ã - å®å¨çæ¬ -
+æçæ¯ security
+ç¶æå¼å§çé£ä¸ä¸ªçæ¬ï¼è¿ä¸ªçæ¬å¾åçé£äºçæ¬å¯ä»¥å®å¨åéã
+- ä¾èµ - å¯¹äº Python çæ¬çä¾èµï¼ä¾å¦ 3.7+ æçæ¯éè¦ 3.7
+ææ´æ°ç Pythonã ## ææ¡£ è¯¦è§[å¨å±ç¬¦å·ç´¢å¼](./docs/
+README.md)ã ## å¼å
+è¿ä¸ªåºåªæ¯ä¸ºäºè·¨å¹³å°ãè·¨é¡¹ç®å¤ç¨ä»£ç èå·²ãæäºæ¯ç´æ¥å°è£å®éå¨ç¨çåè½ï¼æäºæ¯å¨åºéå¼åç¶åéè¿pipä¾èµä¼ éç»åä¸ªé¡¹ç®ï¼æäºå¯è½ççåªæ¯å¥æå¦æ³çµåä¹ç°ãå¦æä½ æåæ ·çéæ±ï¼ä¹è®¤å¯è¿ä»½åªåï¼é£ä¹æ¬¢è¿å å¥ã
+è¯¦è§[å¼åæå](./CONTRIBUTING.md)ã ## å¸®å© å¯ä»¥éè¿ Issue
+åé¦ï¼æéè¿ Pull Request
+æ·»å ä½ çå·¥å·ï¼å¦æéè¦ï¼å¯ä»¥è¿å¥QQç¾¤ 699090940
+è·åéå³æ¶æ§çå¸®å©ã Platform: UNKNOWN Classifier: Development Status
+:: 4 - Beta Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified) Classifier: License :: OSI
 Approved :: MIT License Classifier: Topic :: Utilities Classifier: Typing ::
 Typed Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `Zeraora-0.3.2/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.3.3/Zeraora.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.3.2
-Summary: 实际应用积累的长期维护的实用开源工具库。A utility Python package for our personal and corporate projects, with long time support.
+Version: 0.3.3
+Summary: 为了跨平台跨项目复用代码而开发的工具库。A utility Python package for our personal and corporate projects, with long time support.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
 Description: <h1 align="center" style="padding-top: 32px">Zeraora</h1>
@@ -15,32 +15,32 @@
             <a href="https://en.wikipedia.org/wiki/MIT_License"><img src="https://img.shields.io/pypi/l/Zeraora?color=purple"></a>
             <a href="https://pypi.org/project/Zeraora/"><img src="https://img.shields.io/pypi/v/zeraora?color=darkgreen"></a>
             <a href=""><img src="https://img.shields.io/pypi/dm/zeraora?color=C72777"></a>
             <a href=""><img src="https://img.shields.io/pypi/status/Zeraora"></a>
             <!--a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a-->
         </div>
         <div align="center">
-            <i>实际应用积累的长期维护的实用开源工具库</i>
+            <i>为了跨平台跨项目复用代码而开发的工具库</i>
             <br>
             <i>A utility Python package for our personal and corporate projects, with long time support</i>
         </div>
         
         
         ## 特性
         
         - 支持with、注解和实例化三种方式调用的计时器 `BearTimer` ；
         - 生成通用representation方便调试时查看对象内部信息的 `ReprMixin` ；
         - 将字典的任意层级递归转化为对象，以便支持点分法访问数据的 `OnionObject` ；
-        - 受 Django 的 `Choices` 和 Java 原生枚举语法启发的、可为枚举添加任意属性的 `Items` ；
+        - 受 Django 的 `Choices` 启发和 Java 原生枚举影响的、可为枚举添加任意属性的 `Items` ；
         - 用以简化 `.as_view()` 传参的 `EasyViewSetMixin` ；
         - 仿照 `DestroyModelMixin` 实现的 `SoftDeleteModelMixin` ；
         - 自动为Django模型生成下划线小写（即蛇形）数据表名的 `SnakeModel` ；
         - 包含34个省级行政区名称、区划代码、字母码、大区、简称、缩写的枚举 `Province` ；
         - 不强制依赖任何非[标准库](https://docs.python.org/zh-cn/3/library/index.html)；
-        - 更多……
+        - 更多符号见[Zeraora全局符号索引](./docs/README.md)。
         
         ## 安装
         
         使用 pip 直接安装：
         
         ```shell
         pip install zeraora
@@ -54,38 +54,53 @@
         
         使用 pip 时临时指定安装源来安装：
         
         ```shell
         pip install zeraora -i http://pypi.mirrors.ustc.edu.cn/simple/
         ```
         
-        ## 文档
-        
-        见[全局符号索引](./docs/README.md)。
+        因为没有需求，所以还没有创建 conda 版本。
         
         ## 版本
         
-        |       | 状态[^1] | 维护时间 | 依赖[^2]          | 备注                                                         |
-        | ----- | -------- | -------- | ----------------- | ------------------------------------------------------------ |
-        | 0.3.x | 🆕feature | 长期     | Python 3.7 或更新 | **分支**：main<br/>趋于稳定，但改了包结构，没办法向下兼容。  |
-        | 0.2.x | ✅bugfix  | 长期     | Python 3.7 或更新 | **分支**：0.2.x<br/>探索包结构，完善核心特性，补充非核心特性。 |
-        | 0.1.x | ❌EOL     | 不再维护 | Python 3.7 或更新 | **分支**：release/*<br/>试验自动部署，只有核心特性。         |
+        |       | 状态      | 维护结束时间 | 首版时间   | 安全版本 | 分支  | 依赖 |
+        | ----- | --------- | ------------ | ---------- | -------- | ----- | ---- |
+        | 0.3.x | 🆕feature  | ~ 0.5.x      | 2023.06.09 | -        | main  | 3.7+ |
+        | 0.2.x | ✅security | ~ 0.4.x      | 2023.04.12 | 0.2.14   | 0.2.x | 3.7+ |
+        | 0.1.x | ❌EOL      | 2023.06.09   | 2023.03.27 | -        | 0.1.x | 3.7+ |
+        
+        - 状态
+          - feature 指功能还在开发或测试，回退子版本可能会出现兼容性问题。
+          - security 指功能已经稳定，回退不会出现兼容性问题；会为问题修复发布新的子版本，但不会迁移新版功能。
+          - EOL 指已经停止维护，不会处理与之相关的任何问题，也不会发布新的子版本。
+          - 没有 prerelease 状态，因为这个状态通常不会发布包，进而难以测试。
         
-        [^1]: 概念参见[Python版本状态](https://devguide.python.org/versions/#status-key)。
-        [^2]: 仅在最低依赖版本中进行(过)单元测试。
+        - 维护结束时间
+          - 一般是到下下一个版本的安全版本发布为止。
         
-        ## 分支
+        - 安全版本
+          - 指的是 security 状态开始的那一个版本，这个版本往后的那些版本可以安全回退。
         
-        主分支将从名为 `master` 的分支切换为 `main` 并且于2023年6月12日删除前者（自动同步不好做所以躺平了），原因是 `main` 听起来确实比前者要舒服一点点，若要深究的话参见[这里](https://stackoverflow.com/a/65021103)。两条分支是完全一致的，换句话说，后续的更新**就是**在 `master` 基础上进行的。
+        - 依赖
+          - 对于 Python 版本的依赖，例如 3.7+ 指的是需要 3.7 或更新的 Python。
         
-        ## 帮助
         
-        这个包偏向于抽象及封装一些实际在用的实用功能，目前整体趋于稳定，如需部署生产环境，请优先考虑 0.3.x 或后续更新的版本。
+        ## 文档
+        
+        详见[全局符号索引](./docs/README.md)。
+        
+        ## 开发
+        
+        这个库只是为了跨平台、跨项目复用代码而已。有些是直接封装实际在用的功能，有些是在库里开发然后通过pip依赖传递给各个项目，有些可能真的只是奇思妙想灵光乍现。如果你有同样的需求，也认可这份努力，那么欢迎加入。
+        
+        详见[开发指南](./CONTRIBUTING.md)。
+        
+        ## 帮助
         
-        欢迎通过 Issue 或 Pull Request 来提出功能创意、命名建议，亦或反馈问题、修复漏洞、编写测试等等等等；如有需要，可以进入QQ群 699090940 获取帮助。
+        可以通过 Issue 反馈，或通过 Pull Request 添加你的工具；如有需要，可以进入QQ群 699090940 获取非即时性的帮助。
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,63 +1,68 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.3.2 Summary:
-å®éåºç¨ç§¯ç´¯çé¿æç»´æ¤çå®ç¨å¼æºå·¥å·åºãA utility Python
+Metadata-Version: 2.1 Name: Zeraora Version: 0.3.3 Summary:
+ä¸ºäºè·¨å¹³å°è·¨é¡¹ç®å¤ç¨ä»£ç èå¼åçå·¥å·åºãA utility Python
 package for our personal and corporate projects, with long time support. Home-
 page: https://github.com/aixcyi/zeraora Author: aixcyi Author-email:
 75880483+aixcyi@users.noreply.github.com License: MIT Project-URL: Source,
 https://github.com/aixcyi/zeraora Project-URL: Tracker, https://github.com/
 aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
 [https://img.shields.io/pypi/pyversions/zeraora?logo=python&logoColor=yellow]
  [https://img.shields.io/pypi/l/Zeraora?color=purple] [https://img.shields.io/
        pypi/v/zeraora?color=darkgreen] [https://img.shields.io/pypi/dm/
       zeraora?color=C72777] [https://img.shields.io/pypi/status/Zeraora]
-          å®éåºç¨ç§¯ç´¯çé¿æç»´æ¤çå®ç¨å¼æºå·¥å·åº
+          ä¸ºäºè·¨å¹³å°è·¨é¡¹ç®å¤ç¨ä»£ç èå¼åçå·¥å·åº
   A utility Python package for our personal and corporate projects, with long
                                  time support
 ## ç¹æ§ - æ¯æwithãæ³¨è§£åå®ä¾åä¸ç§æ¹å¼è°ç¨çè®¡æ¶å¨
 `BearTimer` ï¼ -
 çæéç¨representationæ¹ä¾¿è°è¯æ¶æ¥çå¯¹è±¡åé¨ä¿¡æ¯ç
 `ReprMixin` ï¼ -
 å°å­å¸çä»»æå±çº§éå½è½¬åä¸ºå¯¹è±¡ï¼ä»¥ä¾¿æ¯æç¹åæ³è®¿é®æ°æ®ç
-`OnionObject` ï¼ - å Django ç `Choices` å Java
-åçæä¸¾è¯­æ³å¯åçãå¯ä¸ºæä¸¾æ·»å ä»»æå±æ§ç `Items` ï¼ -
+`OnionObject` ï¼ - å Django ç `Choices` å¯åå Java
+åçæä¸¾å½±åçãå¯ä¸ºæä¸¾æ·»å ä»»æå±æ§ç `Items` ï¼ -
 ç¨ä»¥ç®å `.as_view()` ä¼ åç `EasyViewSetMixin` ï¼ - ä»¿ç§
 `DestroyModelMixin` å®ç°ç `SoftDeleteModelMixin` ï¼ -
 èªå¨ä¸ºDjangoæ¨¡åçæä¸åçº¿å°åï¼å³èå½¢ï¼æ°æ®è¡¨åç
 `SnakeModel` ï¼ -
 åå«34ä¸ªççº§è¡æ¿åºåç§°ãåºåä»£ç ãå­æ¯ç ãå¤§åºãç®ç§°ãç¼©åçæä¸¾
 `Province` ï¼ - ä¸å¼ºå¶ä¾èµä»»ä½é[æ ååº](https://docs.python.org/
-zh-cn/3/library/index.html)ï¼ - æ´å¤â¦â¦ ## å®è£ ä½¿ç¨ pip
-ç´æ¥å®è£ï¼ ```shell pip install zeraora ``` ä¸´æ¶éè¿æ¬å°ä»£çä½¿ç¨
-pip å®è£ï¼ ```shell pip install zeraora --proxy=127.0.0.1:6666 ``` ä½¿ç¨
-pip æ¶ä¸´æ¶æå®å®è£æºæ¥å®è£ï¼ ```shell pip install zeraora -i http:/
-/pypi.mirrors.ustc.edu.cn/simple/ ``` ## ææ¡£ è§[å¨å±ç¬¦å·ç´¢å¼](./docs/
-README.md)ã ## çæ¬ | | ç¶æ[^1] | ç»´æ¤æ¶é´ | ä¾èµ[^2] | å¤æ³¨ | |
------ | -------- | -------- | ----------------- | -----------------------------
-------------------------------- | | 0.3.x | ðfeature | é¿æ | Python 3.7
-ææ´æ° | **åæ¯**ï¼main
-è¶äºç¨³å®ï¼ä½æ¹äºåç»æï¼æ²¡åæ³åä¸å¼å®¹ã | | 0.2.x |
-âbugfix | é¿æ | Python 3.7 ææ´æ° | **åæ¯**ï¼0.2.x
-æ¢ç´¢åç»æï¼å®åæ ¸å¿ç¹æ§ï¼è¡¥åéæ ¸å¿ç¹æ§ã | | 0.1.x |
-âEOL | ä¸åç»´æ¤ | Python 3.7 ææ´æ° | **åæ¯**ï¼release/*
-è¯éªèªå¨é¨ç½²ï¼åªææ ¸å¿ç¹æ§ã | [^1]: æ¦å¿µåè§
-[Pythonçæ¬ç¶æ](https://devguide.python.org/versions/#status-key)ã [^2]:
-ä»å¨æä½ä¾èµçæ¬ä¸­è¿è¡(è¿)ååæµè¯ã ## åæ¯
-ä¸»åæ¯å°ä»åä¸º `master` çåæ¯åæ¢ä¸º `main`
-å¹¶ä¸äº2023å¹´6æ12æ¥å é¤åèï¼èªå¨åæ­¥ä¸å¥½åæä»¥èººå¹³äºï¼ï¼åå æ¯
-`main` å¬èµ·æ¥ç¡®å®æ¯åèè¦èæä¸ç¹ç¹ï¼è¥è¦æ·±ç©¶çè¯åè§
-[è¿é](https://stackoverflow.com/a/
-65021103)ãä¸¤æ¡åæ¯æ¯å®å¨ä¸è´çï¼æ¢å¥è¯è¯´ï¼åç»­çæ´æ°**å°±æ¯**å¨
-`master` åºç¡ä¸è¿è¡çã ## å¸®å©
-è¿ä¸ªåååäºæ½è±¡åå°è£ä¸äºå®éå¨ç¨çå®ç¨åè½ï¼ç®åæ´ä½è¶äºç¨³å®ï¼å¦éé¨ç½²çäº§ç¯å¢ï¼è¯·ä¼åèè
-0.3.x æåç»­æ´æ°ççæ¬ã æ¬¢è¿éè¿ Issue æ Pull Request
-æ¥æåºåè½åæãå½åå»ºè®®ï¼äº¦æåé¦é®é¢ãä¿®å¤æ¼æ´ãç¼åæµè¯ç­ç­ç­ç­ï¼å¦æéè¦ï¼å¯ä»¥è¿å¥QQç¾¤
-699090940 è·åå¸®å©ã Platform: UNKNOWN Classifier: Development Status :: 4
-- Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: Intended
-Audience :: Developers Classifier: Operating System :: OS Independent
+zh-cn/3/library/index.html)ï¼ - æ´å¤ç¬¦å·è§[Zeraoraå¨å±ç¬¦å·ç´¢å¼](./
+docs/README.md)ã ## å®è£ ä½¿ç¨ pip ç´æ¥å®è£ï¼ ```shell pip install
+zeraora ``` ä¸´æ¶éè¿æ¬å°ä»£çä½¿ç¨ pip å®è£ï¼ ```shell pip install
+zeraora --proxy=127.0.0.1:6666 ``` ä½¿ç¨ pip
+æ¶ä¸´æ¶æå®å®è£æºæ¥å®è£ï¼ ```shell pip install zeraora -i http://
+pypi.mirrors.ustc.edu.cn/simple/ ``` å ä¸ºæ²¡æéæ±ï¼æä»¥è¿æ²¡æåå»º
+conda çæ¬ã ## çæ¬ | | ç¶æ | ç»´æ¤ç»ææ¶é´ | é¦çæ¶é´ |
+å®å¨çæ¬ | åæ¯ | ä¾èµ | | ----- | --------- | ------------ | ---------
+- | -------- | ----- | ---- | | 0.3.x | ðfeature | ~ 0.5.x | 2023.06.09 | -
+| main | 3.7+ | | 0.2.x | âsecurity | ~ 0.4.x | 2023.04.12 | 0.2.14 | 0.2.x |
+3.7+ | | 0.1.x | âEOL | 2023.06.09 | 2023.03.27 | - | 0.1.x | 3.7+ | - ç¶æ
+- feature
+æåè½è¿å¨å¼åææµè¯ï¼åéå­çæ¬å¯è½ä¼åºç°å¼å®¹æ§é®é¢ã
+- security
+æåè½å·²ç»ç¨³å®ï¼åéä¸ä¼åºç°å¼å®¹æ§é®é¢ï¼ä¼ä¸ºé®é¢ä¿®å¤åå¸æ°çå­çæ¬ï¼ä½ä¸ä¼è¿ç§»æ°çåè½ã
+- EOL
+æå·²ç»åæ­¢ç»´æ¤ï¼ä¸ä¼å¤çä¸ä¹ç¸å³çä»»ä½é®é¢ï¼ä¹ä¸ä¼åå¸æ°çå­çæ¬ã
+- æ²¡æ prerelease
+ç¶æï¼å ä¸ºè¿ä¸ªç¶æéå¸¸ä¸ä¼åå¸åï¼è¿èé¾ä»¥æµè¯ã -
+ç»´æ¤ç»ææ¶é´ -
+ä¸è¬æ¯å°ä¸ä¸ä¸ä¸ªçæ¬çå®å¨çæ¬åå¸ä¸ºæ­¢ã - å®å¨çæ¬ -
+æçæ¯ security
+ç¶æå¼å§çé£ä¸ä¸ªçæ¬ï¼è¿ä¸ªçæ¬å¾åçé£äºçæ¬å¯ä»¥å®å¨åéã
+- ä¾èµ - å¯¹äº Python çæ¬çä¾èµï¼ä¾å¦ 3.7+ æçæ¯éè¦ 3.7
+ææ´æ°ç Pythonã ## ææ¡£ è¯¦è§[å¨å±ç¬¦å·ç´¢å¼](./docs/
+README.md)ã ## å¼å
+è¿ä¸ªåºåªæ¯ä¸ºäºè·¨å¹³å°ãè·¨é¡¹ç®å¤ç¨ä»£ç èå·²ãæäºæ¯ç´æ¥å°è£å®éå¨ç¨çåè½ï¼æäºæ¯å¨åºéå¼åç¶åéè¿pipä¾èµä¼ éç»åä¸ªé¡¹ç®ï¼æäºå¯è½ççåªæ¯å¥æå¦æ³çµåä¹ç°ãå¦æä½ æåæ ·çéæ±ï¼ä¹è®¤å¯è¿ä»½åªåï¼é£ä¹æ¬¢è¿å å¥ã
+è¯¦è§[å¼åæå](./CONTRIBUTING.md)ã ## å¸®å© å¯ä»¥éè¿ Issue
+åé¦ï¼æéè¿ Pull Request
+æ·»å ä½ çå·¥å·ï¼å¦æéè¦ï¼å¯ä»¥è¿å¥QQç¾¤ 699090940
+è·åéå³æ¶æ§çå¸®å©ã Platform: UNKNOWN Classifier: Development Status
+:: 4 - Beta Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified) Classifier: License :: OSI
 Approved :: MIT License Classifier: Topic :: Utilities Classifier: Typing ::
 Typed Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `Zeraora-0.3.2/Zeraora.egg-info/SOURCES.txt` & `Zeraora-0.3.3/Zeraora.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 Zeraora.egg-info/dependency_links.txt
 Zeraora.egg-info/top_level.txt
 zeraora/__init__.py
 zeraora/converters.py
 zeraora/generators.py
 zeraora/gvs.py
 zeraora/structures.py
+zeraora/throwables.py
 zeraora/typeclasses.py
 zeraora/utils.py
 zeraora/constants/__init__.py
 zeraora/constants/charsets.py
-zeraora/constants/chores.py
-zeraora/constants/division.py
+zeraora/constants/configs.py
+zeraora/constants/enumerations.py
 zeraora/dj/__init__.py
 zeraora/dj/fields.py
 zeraora/dj/lookups.py
 zeraora/dj/models.py
 zeraora/drf/__init__.py
 zeraora/drf/filters.py
 zeraora/drf/viewsets.py
```

### Comparing `Zeraora-0.3.2/setup.py` & `Zeraora-0.3.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 setup(
     name='Zeraora',
     version=version,
     url='https://github.com/aixcyi/zeraora',
     license='MIT',
     author='aixcyi',
     author_email='75880483+aixcyi@users.noreply.github.com',
-    description="实际应用积累的长期维护的实用开源工具库。"
+    description="为了跨平台跨项目复用代码而开发的工具库。"
                 "A utility Python package for our personal and corporate projects, with long time support.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

### Comparing `Zeraora-0.3.2/zeraora/constants/charsets.py` & `Zeraora-0.3.3/zeraora/constants/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.2/zeraora/constants/division.py` & `Zeraora-0.3.3/zeraora/constants/enumerations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 """
-省级行政区划相关。
+常用枚举。
 """
-
-__all__ = [
-    'Region', 'Province', 'DivisionLevel',
-]
-
 from enum import Enum
 
 from ..typeclasses import Items
 
 
 class Region(int, Items):
     """
@@ -135,7 +130,24 @@
     """市级。自顶向下的第二个层级，包括地级市、地级县、自治州、盟等。"""
     COUNTY = 3
     """县级。自顶向下的第三个层级，包括县、自治县、县级市、旗、自治旗、市辖区等。"""
     TOWNSHIP = 4
     """乡级。自顶向下的第四个层级，包括县辖区、乡、镇、街道等。"""
     VILLAGE = 5
     """村级。自顶向下的第五个层级。"""
+
+
+class Degree(int, Items):
+    """
+    描述程度的五个档位。
+    """
+    HIGHEST = 100, '最高'
+    HIGH = 50, '高'
+    NORMAL = 0, '正常'
+    LOW = -50, '低'
+    LOWEST = -100, '最低'
+
+    __properties__ = 'label',
+
+    @property
+    def label(self):
+        return self._label_
```

### Comparing `Zeraora-0.3.2/zeraora/converters.py` & `Zeraora-0.3.3/zeraora/converters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 用于将一种值转换为另一种值的转换器。
 """
+from __future__ import annotations
 
 __all__ = [
     'delta2hms', 'delta2ms', 'delta2s',
     'wdate', 'get_week_range', 'get_week_side',
     'get_week_in_year',
     'represent', 'datasize', 'dsz', 'true',
     'SafeCaster', 'safecast', 'safecasts',
     'remove_exponent',
 ]
 
 import re
 from datetime import timedelta, datetime, date
 from decimal import Decimal
-from typing import Callable, Any, Tuple, Union
+from typing import Callable, Any
 from uuid import UUID
 
 from .typeclasses import Throwable, UNSET
 
 
 def remove_exponent(d: Decimal):
     """
@@ -26,28 +27,28 @@
 
     非原创代码，出自：
     https://docs.python.org/zh-cn/3/library/decimal.html#decimal-faq
     """
     return d.quantize(Decimal(1)) if d == d.to_integral() else d.normalize()
 
 
-def delta2hms(delta: timedelta) -> Tuple[int, int, float]:
+def delta2hms(delta: timedelta) -> tuple[int, int, float]:
     """
     将时间增量转换为时分秒格式，其中秒钟以小数形式包含毫秒和微秒。
 
     :param delta: 时间增量。
     :return: 一个三元元组。
     """
     h = delta.seconds // 3600
     m = delta.seconds % 3600 // 60
     s = delta.seconds % 60 + delta.microseconds / 1000000
     return h, m, s
 
 
-def delta2ms(delta: timedelta) -> Tuple[int, float]:
+def delta2ms(delta: timedelta) -> tuple[int, float]:
     """
     将时间增量转换为分秒格式，其中秒钟以小数形式包含毫秒和微秒。
 
     :param delta: 时间增量。
     :return: 二元元组。前者用一个整数表示分钟数，
              后者用一个小数表示秒钟数和纳秒数。
     """
@@ -81,15 +82,15 @@
     fmt = '%Y-%U-%w' if sunday_first else '%Y-%W-%w'
     return datetime.strptime(day, fmt).date()
 
 
 def get_week_range(year: int,
                    week_in_year: int,
                    month: int = UNSET,
-                   sunday_first=False) -> Tuple[date, ...]:
+                   sunday_first=False) -> tuple[date, ...]:
     """
     计算一年中某一周对应的所有日期。
 
     :param year: 具体年份。比如 2012、2023 等。
     :param week_in_year: 一年中的第几周。从 0 开始。
     :param month: 具体月份。若指定了这个参数，则只计算这个月的那一部分日期。
     :param sunday_first: 是否以周日为一周的开始。
@@ -107,15 +108,15 @@
         )
     return days
 
 
 def get_week_side(year: int,
                   week_in_year: int,
                   month: int = UNSET,
-                  sunday_first=False) -> Tuple[date, date]:
+                  sunday_first=False) -> tuple[date, date]:
     """
     计算一年中某一周对应的第一天和最后一天。
 
     :param year: 具体年份。比如 2012、2023 等。
     :param week_in_year: 一年中的第几周。从 0 开始。
     :param month: 具体月份。若指定了这个参数，则只计算这个月的那一部分日期。
     :param sunday_first: 是否以周日为一周的开始。
@@ -174,15 +175,15 @@
         return f'[{value:%Y-%m-%d}]'
     elif isinstance(value, UUID):
         return value.hex
     else:
         return repr(value)
 
 
-def datasize(literal: str) -> Union[int, float]:
+def datasize(literal: str) -> int | float:
     """
     将一个字面量转换为字节数目。
 
     支持的单位包括：
       - B、b
       - KB、KiB、Kb、Kib
       - MB、MiB、Mb、Mib
@@ -263,31 +264,31 @@
         """
         创建一个安全转换器，用于转换某个值而不发生特定异常。若不提供初值，则第一个转换器也必须允许无参调用。
         """
         self._value = raw
         self._default = None
         self._converters = tuple()
 
-    def __call__(self, raw: Any = UNSET) -> 'SafeCaster':
+    def __call__(self, raw: Any = UNSET) -> SafeCaster:
         self._value = raw
         return self
 
-    def catch(self, *exceptions: Throwable) -> 'SafeCaster':
+    def catch(self, *exceptions: Throwable) -> SafeCaster:
         """
         置入需要捕获的异常。应当提供可被 except 语句接受的值。
         """
         self._exceptions = tuple(
             exc for exc in exceptions
             if exc.__class__ is type
             and issubclass(exc, BaseException)
             or isinstance(exc, BaseException)
         )
         return self
 
-    def by(self, *mappers: Callable) -> 'SafeCaster':
+    def by(self, *mappers: Callable) -> SafeCaster:
         """
         置入转换器。若未提供初值，则第一个转换器也必须允许无参调用。
         """
         self._converters = tuple(
             mapper for mapper in mappers
             if callable(mapper)
         )
```

### Comparing `Zeraora-0.3.2/zeraora/dj/fields.py` & `Zeraora-0.3.3/zeraora/dj/fields.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.2/zeraora/dj/lookups.py` & `Zeraora-0.3.3/zeraora/dj/lookups.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.2/zeraora/dj/models.py` & `Zeraora-0.3.3/zeraora/dj/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 对 Django ORM模型 的增强。
 """
+from __future__ import annotations
 
 __all__ = [
     'SnakeModel', 'CreateTimeMixin',
     'TimeMixin', 'ActiveStatusMixin', 'DeletionMixin',
     'IndexMixin', 'ShortIndexMixin',
     'UrgencyMixin', 'ImportanceMixin',
     'AddressMixin', 'GlobalAddressMixin', 'BizMixin',
 ]
 
 import re
 import uuid
-from typing import Union
 
 from .. import gvs
 from ..constants import Degree, Province
 from ..structures import DivisionCode
 from ..utils import warn_empty_ads
 
 try:
@@ -276,15 +276,15 @@
 
         返回一个 ``DivisionCode`` 元组。
         写入时提供一个 ``DivisionCode`` 元组，或者一个至少有六位数字的字符串。
         """
         return DivisionCode(self.province, self.prefecture, self.county, self.township)
 
     @ad_code.setter
-    def ad_code(self, _code: Union[str, DivisionCode]):
+    def ad_code(self, _code: str | DivisionCode):
         adc = _code if isinstance(_code, DivisionCode) else DivisionCode.fromcode(_code)
         self.province = adc.province
         self.prefecture = adc.prefecture
         self.county = adc.county
         self.township = adc.township
 
     def check_area_exist(self) -> bool:
```

### Comparing `Zeraora-0.3.2/zeraora/drf/filters.py` & `Zeraora-0.3.3/zeraora/drf/filters.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.2/zeraora/drf/viewsets.py` & `Zeraora-0.3.3/zeraora/drf/viewsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 对 Django REST Framework 视图集（viewset）的增强。
 """
+from __future__ import annotations
 
 __all__ = [
     'EasyViewSetMixin',
     'SoftDeleteModelMixin',
 ]
 
-from typing import Any, Dict
+from typing import Any
 
 try:
     from django.utils.decorators import classonlymethod
     from rest_framework import status
     from rest_framework.response import Response
     from rest_framework.viewsets import ViewSetMixin
 except ImportError as e:
@@ -25,15 +26,15 @@
     适用于：
       - ``rest_framework.viewsets.ViewSet`` 的子类
       - ``rest_framework.viewsets.GenericViewSet`` 的子类
       - 需要 ``rest_framework.viewsets.ViewSetMixin`` 的类
     """
 
     @classonlymethod
-    def to_view(cls, initkwargs: Dict[str, Any] = None, **actions: str):
+    def to_view(cls, initkwargs: dict[str, Any] = None, **actions: str):
         """
         将视图类存储在一个视图函数上，方便URL反向查找。
 
         之所以调转 ``initkwargs`` 和 ``actions`` 的传参方式，是因为后者往往用得更频繁。
 
         :param initkwargs: 视图类的初始化参数。
         :param actions: HTTP方法及其在视图类中的方法函数名称。
```

### Comparing `Zeraora-0.3.2/zeraora/generators.py` & `Zeraora-0.3.3/zeraora/generators.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 
 __all__ = [
     'randbytes', 'SnowflakeWorker',
     'randb62', 'SnowflakeMultiWorker',
     'randb64', 'SnowflakeSingleWorker',
 ]
 
+import logging
 import os
 from random import getrandbits
 from time import time
 
 from .constants.charsets import BASE62, BASE64
 
+snow_logger = logging.getLogger('zeraora.snowflake')
+
 
 def randbytes(n: int) -> bytes:
     """
     生成 n 个随机字节。
 
     此函数用于在 Python 3.9 以前代替 random.randbytes(n) 方法。
     """
@@ -82,19 +85,23 @@
         if sequence & self.SEQUENCE != sequence:
             self.overflow()  # 序号上溢
 
         self._stamp = curr
         self._sequence = sequence
         return (self._stamp << 22) | (self._worker << 12) | sequence
 
-    def redirect(self) -> int:
-        raise self.TimeRedirected(self)
+    def redirect(self):
+        exc = self.TimeRedirected(self)
+        snow_logger.exception(type(self).__name__, exc_info=exc)
+        raise exc
 
     def overflow(self):
-        raise self.SequenceOverflow(self)
+        exc = self.SequenceOverflow(self)
+        snow_logger.exception(type(self).__name__, exc_info=exc)
+        raise exc
 
     def dump(self) -> dict:
         return {
             "stamp": self._stamp,
             "worker": self._worker,
             "sequence": self._sequence,
         }
@@ -134,17 +141,17 @@
         雪花ID是一个64位整数，包含1位符号+41位时间戳+10位设备编号+12位毫秒内序号。
 
         :param worker: 设备编号。取值范围 0-1023。
         :param epoch: 时间戳起点（计算用的时间戳与标准时间戳的差，单位为毫秒）。
         :raise RuntimeError: 试图创建相同worker的类实例。
         """
         if worker in cls._objects_:
-            raise RuntimeError(
-                f'存在相同的 SnowflakeMultiWorker(worker={worker})'
-            )
+            exc = RuntimeError(f'存在相同的 SnowflakeMultiWorker(worker={worker})')
+            snow_logger.exception(cls.__name__, exc_info=exc)
+            raise exc
         cls._objects_.append(worker)
         return SnowflakeWorker.__new__(cls)
 
 
 class SnowflakeSingleWorker(SnowflakeWorker):
     _instanced_ = False
 
@@ -155,20 +162,22 @@
         雪花ID是一个64位整数，包含1位符号+41位时间戳+10位设备编号+12位毫秒内序号。
         其中设备编号从0开始，当发生时钟回拨时自动递增，因此总计容许 1023 次时钟回拨。
 
         :param epoch: 时间戳起点（计算用的时间戳与标准时间戳的差，单位为毫秒）。
         :raise RuntimeError: 试图创建第二个类实例。
         """
         if cls._instanced_ is True:
-            raise RuntimeError('已实例化过 SnowflakeSingleWorker 。')
+            exc = RuntimeError('已实例化过 SnowflakeSingleWorker 。')
+            snow_logger.exception(cls.__name__, exc_info=exc)
+            raise exc
         cls._instanced_ = True
         return SnowflakeWorker.__new__(cls)
 
     def __init__(self, *, epoch: int = 0):
         super().__init__(0, epoch=epoch)
 
     def redirect(self) -> int:
         worker = self._worker + 1
         if worker & self.WORKER != worker:
-            raise self.TimeRedirected(self)
+            super().redirect()
         self._worker = worker
         return self._sequence
```

### Comparing `Zeraora-0.3.2/zeraora/structures.py` & `Zeraora-0.3.3/zeraora/structures.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 数据结构包。
 """
+from __future__ import annotations
 
 __all__ = [
     'DivisionCode',
     'Division',
 ]
 
 from typing import NamedTuple, Tuple
 
-from .constants.division import DivisionLevel
+from .constants import DivisionLevel
 
 
 class DivisionCode(NamedTuple):
     """
     统计用行政区划代码。
     """
     province: str
@@ -22,15 +23,15 @@
     township: str = '000'
     village: str = '000'
 
     def __str__(self):
         return ''.join(self)
 
     @classmethod
-    def fromcode(cls, code: str) -> "DivisionCode":
+    def fromcode(cls, code: str) -> DivisionCode:
         adc = code.ljust(12, '0')
         return cls(adc[:2], adc[2:4], adc[4:6], adc[6:9], adc[9:12])
 
 
 class Division(NamedTuple):
     """
     行政区划。
```

### Comparing `Zeraora-0.3.2/zeraora/utils.py` & `Zeraora-0.3.3/zeraora/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 偏工具属性的类与函数。
 """
+from __future__ import annotations
 
 __all__ = [
     'bear_config', 'BearTimer', 'ReprMixin', 'start', 'deprecate',
     'load_ads4', 'warn_empty_ads',
 ]
 
 import json
@@ -12,69 +13,41 @@
 import sys
 import warnings
 from decimal import Decimal
 from functools import wraps
 from itertools import groupby
 from pathlib import Path
 from time import time_ns
-from typing import Tuple, NoReturn, Union
+from typing import NoReturn
 
 from . import gvs
+from .constants import LOG_CONF_BEAR
 from .converters import represent
 from .structures import DivisionCode
 
-logger_bear = logging.getLogger('zeraora.bear')
+bear_logger = logging.getLogger('zeraora.bear')
 
-bear_config = {
-    'version': 1,
-    'formatters': {
-        'bear': {
-            'format': '[%(asctime)s] [%(levelname)s] %(message)s',
-        },
-        'bear_plus': {
-            'format': (
-                '[%(asctime)s] [%(levelname)s] '
-                '[%(module)s.%(funcName)s:%(lineno)d] '
-                '%(message)s'
-            )
-        },
-    },
-    'filters': {},
-    'handlers': {
-        'Console': {
-            'level': 'DEBUG',
-            'class': 'logging.StreamHandler',
-            'filters': [],
-            'formatter': 'bear',
-        },
-    },
-    'loggers': {
-        'zeraora.bear': {
-            'level': 'DEBUG',
-            'handlers': ['Console'],
-            'propagate': False,
-        },
-    },
-}
+bear_config = LOG_CONF_BEAR
 
 
 class BearTimer(object):
 
     def __init__(self, label: str = None, *_, **__):
         """
         熊牌计时器。对代码运行进行计时，并向名为 "zeraora.bear" 的Logger发送DEBUG等级的日志。
 
         ----
 
         使用前，需要先启用日志输出：
 
         >>> import logging.config
-        >>> from zeraora.utils import BearTimer, bear_config
+        >>> from zeraora.constants import LOG_CONF_BEAR
+        >>> from zeraora.utils import BearTimer
         >>>
-        >>> logging.config.dictConfig(bear_config)
+        >>> logging.config.dictConfig(LOG_CONF_BEAR)
         >>> bear = BearTimer()
 
         对于使用 Django 的项目可以改为在 settings.py 中进行如下设置：
 
         >>> LOGGING = {
         >>>     'version': 1,
         >>>     'formatters': {...},
@@ -164,15 +137,15 @@
 
         :param msg: 要附加的消息。默认为空文本。
         :return: 自纪元以来的当前时间（以纳秒为单位）。
         """
         now = time_ns()
         total = Decimal((now - self._start) if self._start else 0) / 1000000000
         delta = Decimal((now - self._point) if self._point else 0) / 1000000000
-        logger_bear.debug(f'[{self._label}] [{total:.9f} +{delta:.9f}]: {msg}')
+        bear_logger.debug(f'[{self._label}] [{total:.9f} +{delta:.9f}]: {msg}')
         self._point = now
         return now
 
     def start(self, msg='Starting...'):
         """
         开始计时。
 
@@ -182,15 +155,15 @@
         :return: 计时器对象自身。
         """
         self._point = 0
         self._start = time_ns()
         self._record(msg)
         return self
 
-    def step(self, msg='') -> Tuple[int, int]:
+    def step(self, msg='') -> tuple[int, int]:
         """
         中途标记。
 
         用此方法可以计算出距离上一次标记/开始计时过去了多久。
 
         如果计时器尚未开始计时，那么过去的时间始终是 0 秒。
 
@@ -318,24 +291,24 @@
 
         AttributeMeta 的变量允许接收一个返回值为字符串的函数作为类型注解，
         用于转换你的类对象的属性值，并直接作为 representation 里这个属性的值。
         """
 
     def _obtain_attrs(self) -> str:
         def obtain():
-            for attr, name in attributes.items():
+            for attr, name in attrs.items():
                 if attr.startswith('_'):
                     continue
-                mapper = annotations.get(attr, represent)
+                mapper = annots.get(attr, represent)
                 value = getattr(self, attr)
                 value = mapper(value) if callable(mapper) else value
                 yield f'{name}={value}'
 
-        attributes = self.AttributeMeta.__dict__
-        annotations = attributes.get('__annotations__', {})
+        attrs = self.AttributeMeta.__dict__
+        annots = attrs.get('__annotations__', {})
         return ' '.join(filter(None, obtain()))
 
     class TagMeta:
         """
         用于控制生成 representation 时需要带上哪些标签。
 
         注意：这个内部类不会被实例化！
@@ -350,31 +323,31 @@
 
         TagMeta 的变量允许接收一个返回值为字符串的函数作为类型注解，
         用于进一步转换你的类对象的属性值，若未提供，默认使用 bool() 来转换。
         """
 
     def _obtain_tags(self) -> str:
         def obtain():
-            for attr, option in attributes.items():
+            for attr, option in attrs.items():
                 if attr.startswith('_'):
                     continue
-                mapper = annotations.get(attr, None)
+                mapper = annots.get(attr, None)
                 value = getattr(self, attr)
                 value = mapper(value) if callable(mapper) else value
                 if isinstance(option, str) and value:
                     yield option
                 elif isinstance(option, tuple):
                     yield option[bool(value)]
                 elif isinstance(option, (list, dict)):
                     yield option[value]
                 else:
                     pass  # pragma: no cover
 
-        attributes = self.TagMeta.__dict__
-        annotations = attributes.get('__annotations__', {})
+        attrs = self.TagMeta.__dict__
+        annots = attrs.get('__annotations__', {})
         return ' '.join(filter(None, obtain()))
 
     def _obtain_pk(self) -> str:
         if hasattr(self, 'pk'):
             pk = self.pk
         elif hasattr(self, 'id'):
             pk = self.id
@@ -448,15 +421,15 @@
     """
     在未载入行政区划映射表时发出警告。（您不应该使用此方法，它只在包内使用）
     """
     if not gvs.ad_map or not gvs.ad_tree:
         warnings.warn('未载入行政区划映射表，该方法可能会失效或返回非期望值。', category=UserWarning)
 
 
-def load_ads4(fp: Union[str, Path], encoding='UTF-8', **kwargs) -> NoReturn:
+def load_ads4(fp: str | Path, encoding='UTF-8', **kwargs) -> NoReturn:
     """
     读取并过滤前四级行政区划，然后赋值给全局变量 ``zeraora.gvs.ad_map`` 和 ``zeraora.gvs.ad_tree`` 。
 
     测试数据可以在 `GitHub <https://github.com/aixcyi/zeraora/tree/main/dataset>`_
     或 `码云 <https://github.com/aixcyi/zeraora/tree/main/dataset>`_ 中找到。
 
     ----
```

