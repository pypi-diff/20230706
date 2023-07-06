# Comparing `tmp/biliarchiver-0.0.17.tar.gz` & `tmp/biliarchiver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biliarchiver-0.0.17.tar", max compression
+gzip compressed data, was "biliarchiver-0.0.9.tar", max compression
```

## Comparing `biliarchiver-0.0.17.tar` & `biliarchiver-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,13 @@
--rw-r--r--   0        0        0      131 2023-07-06 16:33:04.928968 biliarchiver-0.0.17/README.md
--rw-r--r--   0        0        0     7973 2023-06-11 13:55:41.732697 biliarchiver-0.0.17/biliarchiver/_biliarchiver_upload_bvid.py
--rw-r--r--   0        0        0     9224 2023-06-16 08:12:16.037415 biliarchiver-0.0.17/biliarchiver/archive_bvid.py
--rw-r--r--   0        0        0     6406 2023-07-06 15:33:53.278338 biliarchiver-0.0.17/biliarchiver/cli_tools/bili_archive_bvids.py
--rw-r--r--   0        0        0     4133 2023-06-06 19:45:06.489235 biliarchiver-0.0.17/biliarchiver/cli_tools/bili_get_bvids.py
--rw-r--r--   0        0        0     1490 2023-06-07 12:25:53.093261 biliarchiver-0.0.17/biliarchiver/cli_tools/bili_upload.py
--rw-r--r--   0        0        0      413 2023-07-06 16:29:12.824614 biliarchiver-0.0.17/biliarchiver/cli_tools/biliarchiver.py
--rw-r--r--   0        0        0     2139 2023-06-07 14:08:15.117924 biliarchiver-0.0.17/biliarchiver/config.py
--rw-r--r--   0        0        0      194 2023-06-09 04:15:33.665307 biliarchiver-0.0.17/biliarchiver/exception.py
--rw-r--r--   0        0        0     2724 2023-06-06 05:53:18.324384 biliarchiver-0.0.17/biliarchiver/utils/dirLock.py
--rw-r--r--   0        0        0      237 2023-06-07 06:29:29.311341 biliarchiver-0.0.17/biliarchiver/utils/ffmpeg.py
--rw-r--r--   0        0        0     1278 2023-06-05 16:41:54.082484 biliarchiver-0.0.17/biliarchiver/utils/string.py
--rw-r--r--   0        0        0       32 2023-07-06 16:33:34.849530 biliarchiver-0.0.17/biliarchiver/version.py
--rw-r--r--   0        0        0      637 2023-07-06 16:33:43.681695 biliarchiver-0.0.17/pyproject.toml
--rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 biliarchiver-0.0.17/setup.py
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 biliarchiver-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-06-06 20:05:41.529385 biliarchiver-0.0.9/README.md
+-rw-r--r--   0        0        0     7575 2023-06-06 19:48:46.123664 biliarchiver-0.0.9/biliarchiver/_biliarchiver_upload_bvid.py
+-rw-r--r--   0        0        0     7157 2023-06-06 19:12:07.431306 biliarchiver-0.0.9/biliarchiver/archive_bvid.py
+-rw-r--r--   0        0        0     4734 2023-06-07 04:48:33.598085 biliarchiver-0.0.9/biliarchiver/bili_archive_bvids.py
+-rw-r--r--   0        0        0     4133 2023-06-06 19:45:06.489235 biliarchiver-0.0.9/biliarchiver/bili_get_bvids.py
+-rw-r--r--   0        0        0     1490 2023-06-07 04:52:11.184454 biliarchiver-0.0.9/biliarchiver/bili_uploade.py
+-rw-r--r--   0        0        0     2018 2023-06-06 19:20:55.302758 biliarchiver-0.0.9/biliarchiver/config.py
+-rw-r--r--   0        0        0     2724 2023-06-06 05:53:18.324384 biliarchiver-0.0.9/biliarchiver/utils/dirLock.py
+-rw-r--r--   0        0        0     1278 2023-06-05 16:41:54.082484 biliarchiver-0.0.9/biliarchiver/utils/string.py
+-rw-r--r--   0        0        0       31 2023-06-06 19:35:41.648702 biliarchiver-0.0.9/biliarchiver/version.py
+-rw-r--r--   0        0        0      530 2023-06-07 04:58:02.482737 biliarchiver-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 biliarchiver-0.0.9/setup.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 biliarchiver-0.0.9/PKG-INFO
```

### Comparing `biliarchiver-0.0.17/biliarchiver/_biliarchiver_upload_bvid.py` & `biliarchiver-0.0.9/biliarchiver/_biliarchiver_upload_bvid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 import json
 import os
 from pathlib import Path
 import time
 from internetarchive import get_item
 from requests import Response
 from rich import print
-from biliarchiver.exception import VideosBasePathNotFoundError
 
 from biliarchiver.utils.string import human_readable_upper_part_map
 from biliarchiver.config import BILIBILI_IDENTIFIER_PERFIX, config
 from biliarchiver.utils.dirLock import UploadLock, AlreadyRunningError
 from biliarchiver.version import BILI_ARCHIVER_VERSION
 
 def upload_bvid(bvid):
     try:
         lock_dir = config.storage_home_dir / '.locks' / bvid
         os.makedirs(lock_dir, exist_ok=True)
         with UploadLock(lock_dir): # type: ignore
             _upload_bvid(bvid)
     except AlreadyRunningError:
         print(f'已经有一个上传 {bvid} 的进程在运行，跳过')
-    except VideosBasePathNotFoundError:
-        print(f'没有找到 {bvid} 对应的文件夹。可能是因已存在 IA item 而跳过了下载，或者你传入了错误的 bvid')
     except Exception as e:
         print(f'上传 {bvid} 时出错：')
         raise e
 
 def _upload_bvid(bvid: str):
     access_key, secret_key = read_ia_keys(config.ia_key_file)
 
     # identifier format: BiliBili-{bvid}_p{pid}-{upper_part} 
     upper_part = human_readable_upper_part_map(string=bvid, backward=True)
     OLD_videos_basepath: Path = config.storage_home_dir / 'videos' / bvid
     videos_basepath: Path = config.storage_home_dir / 'videos' / f'{bvid}-{upper_part}'
-
     if os.path.exists(OLD_videos_basepath):
         print(f'检测到旧的视频主目录 {OLD_videos_basepath}，将其重命名为 {videos_basepath}...')
         os.rename(OLD_videos_basepath, videos_basepath)
-
-    if not os.path.exists(videos_basepath):
-        raise VideosBasePathNotFoundError(f'{videos_basepath}')
     for local_identifier in os.listdir(videos_basepath):
         remote_identifier = f'{local_identifier}-{upper_part}'
         if os.path.exists(f'{videos_basepath}/{local_identifier}/_uploaded.mark'):
             print(f'{local_identifier} => {remote_identifier} 已经上传过了(_uploaded.mark)')
             continue
         if local_identifier.startswith('_') :
             print(f'跳过 {local_identifier}')
@@ -77,18 +70,17 @@
 
         for filename in os.listdir(f'{videos_basepath}/{local_identifier}'):
             file = f'{videos_basepath}/{local_identifier}/{filename}'
             if os.path.isfile(file):
                 if os.path.basename(file).startswith('_'):
                     continue
                 if not os.path.isfile(file):
-                   continue
+                    continue
                 filedict[filename] = file
-
-        assert f'{file_basename}.mp4' in filedict
+        
 
         # IA 去重
         for file_in_item in item.files:
             if file_in_item["name"] in filedict:
                 filedict.pop(file_in_item["name"])
                 print(f"File {file_in_item['name']} already exists in {remote_identifier}.")
 
@@ -143,15 +135,15 @@
                 access_key=access_key,
                 secret_key=secret_key,
                 verbose=True,
                 queue_derive=True,
                 retries=5,
             )
 
-        tries = 100
+        tries = 30
         item = get_item(remote_identifier) # refresh item
         while not item.exists and tries > 0:
             print(f"Waiting for item to be created ({tries})  ...", end='\r')
             time.sleep(30)
             item = get_item(remote_identifier)
             tries -= 1
```

### Comparing `biliarchiver-0.0.17/biliarchiver/archive_bvid.py` & `biliarchiver-0.0.9/biliarchiver/archive_bvid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 import os
 from pathlib import Path
-from typing import Union
 
 import aiofiles
 import httpx
 from bilix.download.utils import raise_api_error, req_retry
 from bilix.exception import APIError
 
 from bilix.sites.bilibili import api
@@ -70,23 +69,14 @@
         file_basename = f'{bvid}_p{pid}'
         video_basepath = videos_basepath / f'{BILIBILI_IDENTIFIER_PERFIX}-{file_basename}'
         video_extrapath = video_basepath / 'extra'
         if os.path.exists(f'{video_basepath}/_downloaded.mark'):
             print(f'{file_basename}: 已经下载过了')
             continue
 
-        def delete_cache(reason: str = ''):
-            if not os.path.exists(video_basepath):
-                return
-            _files_in_video_basepath = os.listdir(video_basepath)
-            for _file in _files_in_video_basepath:
-                if _file.startswith(file_basename):
-                    print(f'{file_basename}: {reason}，删除缓存: {_file}')
-                    os.remove(video_basepath / _file)
-        delete_cache('为防出错，清空上次未完成的下载缓存')
         video_info = await api.get_video_info(d.client, page.p_url)
         print(f'{file_basename}: {video_info.title}...')
         os.makedirs(video_basepath, exist_ok=True)
         os.makedirs(video_extrapath, exist_ok=True)
 
 
         old_p_name = video_info.pages[video_info.p].p_name
@@ -96,78 +86,51 @@
         video_info.pages[video_info.p].p_name = file_basename # 所以这里覆盖 p_name 为 file_basename
         video_info.h1_title = 'iiiiii' * 50 # 然后假装超长标题
         # 这样 bilix 保存的文件名就是我们想要的了（谁叫 bilix 不支持自定义文件名呢）
         # NOTE: p_name 似乎也不宜过长，否则还是会被 bilix 截断。
         # 但是我们以 {bvid}_p{pid} 作为文件名，这个长度是没问题的。
 
 
+        # 选择编码，优先 hevc，没有的话就 avc
+        # 不选 av0 ，毕竟目前没几个设备能拖得动
         codec = None
-        quality = None
         if video_info.dash:
-            # 选择编码 dvh->hev->avc
-            # 不选 av0 ，毕竟目前没几个设备能拖得动
-            codec_candidates = ['dvh', 'hev', 'avc']
-            for codec_candidate in codec_candidates:
+            for media in video_info.dash.videos:
+                if media.codec.startswith('hev'):
+                    codec = media.codec
+                    print(f'{file_basename}: "{codec}" "{media.quality}" ...')
+                    break
+            if codec is None:
                 for media in video_info.dash.videos:
-                    if media.codec.startswith(codec_candidate):
+                    if media.codec.startswith('avc'):
                         codec = media.codec
-                        quality = media.quality
                         print(f'{file_basename}: "{codec}" "{media.quality}" ...')
                         break
-                if codec is not None:
-                    break
-            assert codec is not None and quality is not None, f'{file_basename}: 没有 dvh、avc 或 hevc 编码的视频'
+            assert codec is not None, f'{file_basename}: 没有 avc 或 hevc 编码的视频'
         elif video_info.other:
-            print(f'{file_basename}: 未解析到 dash 资源，交给 bilix 处理 ...')
+            print(f'{file_basename}: 未解析到dash资源，交给 bilix 处理 ...')
             codec = ''
-            quality = 0
         else:
             raise APIError(f'{file_basename}: 未解析到视频资源', page.p_url)
 
         assert codec is not None
-        assert isinstance(quality, (int, str))
 
         cor1 = d.get_video(page.p_url ,video_info=video_info, path=video_basepath,
-                    quality=quality, # 选择最高画质
+                    quality=0, # 选择最高画质
                     codec=codec, # 编码
                     # 下载 ass 弹幕(bilix 会自动调用 danmukuC 将 pb 弹幕转为 ass)、封面、字幕
                     # 弹幕、封面、字幕都会被放进 extra 子目录里，所以需要 d.hierarchy is True
                     dm=True, image=True, subtitle=True
                     )
         # 下载原始的 pb 弹幕
         cor2 = d.get_dm(page.p_url, video_info=video_info, path=video_extrapath)
         # 下载视频超详细信息（BV 级别，不是分 P 级别）
         cor3 = download_bilibili_video_detail(d.client, bvid, f'{video_extrapath}/{file_basename}.info.json')
         await asyncio.gather(cor1, cor2, cor3)
 
-        if codec.startswith('hev') and not os.path.exists(video_basepath / f'{file_basename}.mp4'):
-
-            # 如果有下载缓存文件（以 file_basename 开头的文件），说明这个 hevc 的 dash 资源存在，只是可能因为网络之类的原因下载中途失败了
-            delete_cache('下载出错')
-
-            # 下载缓存文件都不存在，应该是对应的 dash 资源根本就没有，一些老视频会出现这种情况。
-            # 换 avc 编码
-            print(f'{file_basename}: 视频文件没有被下载？也许是 hevc 对应的 dash 资源不存在，尝试 avc ……')
-            for media in video_info.dash.videos:
-                if media.codec.startswith('avc'):
-                    codec = media.codec
-                    print(f'{file_basename}: "{codec}" "{media.quality}" ...')
-                    break
-            cor4 = d.get_video(page.p_url ,video_info=video_info, path=video_basepath,
-                    quality=0, # 选择最高画质
-                    codec=codec, # 编码
-                    # 下载 ass 弹幕(bilix 会自动调用 danmukuC 将 pb 弹幕转为 ass)、封面、字幕
-                    # 弹幕、封面、字幕都会被放进 extra 子目录里，所以需要 d.hierarchy is True
-                    dm=True, image=True, subtitle=True
-                    )
-            await asyncio.gather(cor4)
-
-
-        assert os.path.exists(video_basepath / f'{file_basename}.mp4')
-
         # 还原为了自定义文件名而做的覆盖
         video_info.pages[video_info.p].p_name = old_p_name
         video_info.h1_title = old_h1_title
 
         # 单 p 下好了
         async with aiofiles.open(f'{video_basepath}/_downloaded.mark', 'w', encoding='utf-8') as f:
             await f.write('')
```

### Comparing `biliarchiver-0.0.17/biliarchiver/cli_tools/bili_get_bvids.py` & `biliarchiver-0.0.9/biliarchiver/bili_get_bvids.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.17/biliarchiver/cli_tools/bili_upload.py` & `biliarchiver-0.0.9/biliarchiver/bili_uploade.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.17/biliarchiver/config.py` & `biliarchiver-0.0.9/biliarchiver/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,28 @@
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 @dataclass
-class _Config(metaclass=singleton):
+class Config(metaclass=singleton):
     video_concurrency: int = 3 
     part_concurrency: int = 10
     stream_retry: int = 20
     storage_home_dir: Path = Path('bilibili_archive_dir/').expanduser()
     ia_key_file: Path = Path('~/.bili_ia_keys.txt').expanduser()
-    cookies_file: Path = Path('~/.cookies.txt').expanduser()
 
     def __init__(self):
         self.is_right_pwd()
         if not os.path.exists(CONFIG_FILE):
             print(f'{CONFIG_FILE} 不存在，创建中...')
             self.save()
         with open(CONFIG_FILE, 'r', encoding='utf-8') as f:
-            print(f'Loading {CONFIG_FILE} ...')
+            print(f'读取 {CONFIG_FILE}...')
             config_file = json.load(f)
 
         self.video_concurrency: int = config_file['video_concurrency']
         self.part_concurrency: int = config_file['part_concurrency']
         self.stream_retry: int = config_file['stream_retry']
 
         self.storage_home_dir: Path = Path(config_file['storage_home_dir']).expanduser()
@@ -44,15 +43,14 @@
         with open(CONFIG_FILE, 'w', encoding='utf-8') as f:
             json.dump({
                 'video_concurrency': self.video_concurrency,
                 'part_concurrency': self.part_concurrency,
                 'stream_retry': self.stream_retry,
                 'storage_home_dir': str(self.storage_home_dir),
                 'ia_key_file': str(self.ia_key_file),
-                'cookies_file': str(self.cookies_file),
             }, f, ensure_ascii=False, indent=4)
 
     def is_right_pwd(self):
         if not os.path.exists('biliarchiver.home'):
             raise Exception('先在当前工作目录创建 biliarchiver.home 文件')
 
-config = _Config()
+config = Config()
```

### Comparing `biliarchiver-0.0.17/biliarchiver/utils/dirLock.py` & `biliarchiver-0.0.9/biliarchiver/utils/dirLock.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.17/biliarchiver/utils/string.py` & `biliarchiver-0.0.9/biliarchiver/utils/string.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.17/setup.py` & `biliarchiver-0.0.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['biliarchiver', 'biliarchiver.cli_tools', 'biliarchiver.utils']
+['biliarchiver', 'biliarchiver.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bilix==0.18.3', 'danmakuc>=0.3.6,<0.4.0', 'internetarchive>=3.5.0,<4.0.0']
+['bilix==0.18.3', 'internetarchive>=3.5.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['bili_archive_bvids = '
-                     'biliarchiver.cli_tools:bili_archive_bvids.main',
-                     'bili_get_bvids = '
-                     'biliarchiver.cli_tools:bili_get_bvids.main',
-                     'bili_upload = biliarchiver.cli_tools:bili_upload.main',
-                     'biliarchiver = biliarchiver.cli_tools:biliarchiver.main']}
+                     'biliarchiver:bili_archive_bvids.main',
+                     'bili_get_bvids = biliarchiver:bili_get_bvids.main',
+                     'bili_uploade = biliarchiver:bili_uploade.main']}
 
 setup_kwargs = {
     'name': 'biliarchiver',
-    'version': '0.0.17',
+    'version': '0.0.9',
     'description': '',
-    'long_description': '# biliarchiver\n\n> 基于 bilix 的 BiliBili 存档工具\n\n## Install\n\n```bash\npip install biliarchiver\n```\n\n## Usage\n\n待补充。\n',
+    'long_description': '# biliarchiver\n\n## 基于 bilix 的 BiliBili 存档工具\n\n~~ IA iteam identifier 格式兼容 tubeup ~~。  \n现在不兼容了，Tubeup 不适合存 B 站视频，它的 identifier 设计不科学，大规模存档必定会撞车。\n\n目前，我可能随时 commit 乱飞且动不动就 git push -f 这个仓库。（为了在我的 vps 和本地之间同步代码）\n\nuserscript.js 还没适配新换的 identifier 格式。\n',
     'author': 'yzqzss',
     'author_email': 'yzqzss@yandex.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

