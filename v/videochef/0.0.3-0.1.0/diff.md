# Comparing `tmp/videochef-0.0.3.tar.gz` & `tmp/videochef-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "videochef-0.0.3.tar", last modified: Wed Nov 16 23:09:39 2022, max compression
+gzip compressed data, was "/Users/jonahpearl/Documents/PiN/Datta lab/Local_code/videochef/dist/.tmp-umltyml8/videochef-0.1.0.tar", last modified: Wed Jul  5 19:26:29 2023, max compression
```

## Comparing `videochef-0.0.3.tar` & `videochef-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxrwxr-x   0 jop9552  (176288) jop9552  (2176288)        0 2022-11-16 23:09:39.691529 videochef-0.0.3/
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)     1067 2022-11-16 16:17:26.000000 videochef-0.0.3/LICENSE.txt
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)      757 2022-11-16 23:09:39.692775 videochef-0.0.3/PKG-INFO
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)      222 2022-11-16 21:10:58.000000 videochef-0.0.3/README.md
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)      227 2022-11-16 16:17:26.000000 videochef-0.0.3/pyproject.toml
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)       78 2022-11-16 23:09:39.695786 videochef-0.0.3/setup.cfg
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)     1380 2022-11-16 23:08:37.000000 videochef-0.0.3/setup.py
-drwxrwxr-x   0 jop9552  (176288) jop9552  (2176288)        0 2022-11-16 23:09:39.620012 videochef-0.0.3/src/
-drwxrwxr-x   0 jop9552  (176288) jop9552  (2176288)        0 2022-11-16 23:09:39.659389 videochef-0.0.3/src/videochef/
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)       54 2022-11-16 18:01:08.000000 videochef-0.0.3/src/videochef/__init__.py
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)     2117 2022-11-16 21:06:28.000000 videochef-0.0.3/src/videochef/chef.py
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)     8034 2022-11-16 23:05:46.000000 videochef-0.0.3/src/videochef/io.py
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)      978 2022-11-16 21:06:23.000000 videochef-0.0.3/src/videochef/util.py
-drwxrwxr-x   0 jop9552  (176288) jop9552  (2176288)        0 2022-11-16 23:09:39.687501 videochef-0.0.3/src/videochef.egg-info/
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)      757 2022-11-16 23:09:39.000000 videochef-0.0.3/src/videochef.egg-info/PKG-INFO
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)      365 2022-11-16 23:09:39.000000 videochef-0.0.3/src/videochef.egg-info/SOURCES.txt
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)        1 2022-11-16 23:09:39.000000 videochef-0.0.3/src/videochef.egg-info/dependency_links.txt
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)        1 2022-11-16 16:18:01.000000 videochef-0.0.3/src/videochef.egg-info/not-zip-safe
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)       20 2022-11-16 23:09:39.000000 videochef-0.0.3/src/videochef.egg-info/requires.txt
--rw-rw-r--   0 jop9552  (176288) jop9552  (2176288)       10 2022-11-16 23:09:39.000000 videochef-0.0.3/src/videochef.egg-info/top_level.txt
+drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-05 19:26:29.000000 videochef-0.1.0/
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     1067 2022-11-14 03:17:49.000000 videochef-0.1.0/LICENSE.txt
+-rw-r--r--   0 jonahpearl   (501) staff       (20)      757 2023-07-05 19:26:29.000000 videochef-0.1.0/PKG-INFO
+-rw-r--r--   0 jonahpearl   (501) staff       (20)      247 2023-07-05 19:23:51.000000 videochef-0.1.0/README.md
+-rw-r--r--   0 jonahpearl   (501) staff       (20)      227 2022-11-14 03:39:07.000000 videochef-0.1.0/pyproject.toml
+-rw-r--r--   0 jonahpearl   (501) staff       (20)       78 2023-07-05 19:26:29.000000 videochef-0.1.0/setup.cfg
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     1381 2023-07-05 19:25:53.000000 videochef-0.1.0/setup.py
+drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-05 19:26:29.000000 videochef-0.1.0/src/
+drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef/
+-rw-r--r--   0 jonahpearl   (501) staff       (20)       54 2023-07-05 19:23:51.000000 videochef-0.1.0/src/videochef/__init__.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)    13178 2023-07-05 19:23:51.000000 videochef-0.1.0/src/videochef/chef.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)    10109 2023-07-05 19:23:51.000000 videochef-0.1.0/src/videochef/io.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     3187 2023-07-05 19:23:51.000000 videochef-0.1.0/src/videochef/util.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     6850 2023-07-05 19:23:51.000000 videochef-0.1.0/src/videochef/viz.py
+drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/
+-rw-r--r--   0 jonahpearl   (501) staff       (20)      757 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/PKG-INFO
+-rw-r--r--   0 jonahpearl   (501) staff       (20)      442 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/SOURCES.txt
+-rw-r--r--   0 jonahpearl   (501) staff       (20)        1 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/dependency_links.txt
+-rw-r--r--   0 jonahpearl   (501) staff       (20)        1 2022-11-14 03:40:09.000000 videochef-0.1.0/src/videochef.egg-info/not-zip-safe
+-rw-r--r--   0 jonahpearl   (501) staff       (20)       20 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/requires.txt
+-rw-r--r--   0 jonahpearl   (501) staff       (20)       10 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/top_level.txt
+drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-05 19:26:29.000000 videochef-0.1.0/tests/
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     3837 2023-07-05 19:23:51.000000 videochef-0.1.0/tests/test_chef.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     2965 2023-07-05 19:23:51.000000 videochef-0.1.0/tests/test_util.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     1445 2023-07-05 19:23:51.000000 videochef-0.1.0/tests/test_viz.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `videochef-0.0.3/LICENSE.txt` & `videochef-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `videochef-0.0.3/PKG-INFO` & `videochef-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videochef
-Version: 0.0.3
+Version: 0.1.0
 Summary: Whip up some fast, embarrassingly parallel video processing
 Home-page: https://github.com/jonahpearl/videochef
 Author: Jonah Pearl
 Author-email: jonahpearl@g.harvard.edu
 License: MIT
 Project-URL: Issue Tracker, https://github.com/jonahpearl/videochef/issues
 Classifier: Development Status :: 1 - Planning
```

### Comparing `videochef-0.0.3/setup.py` & `videochef-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name='videochef',
-    version='0.0.3',
+    version='0.1.0',
     license='MIT',
     description='Whip up some fast, embarrassingly parallel video processing',
     author='Jonah Pearl',
     author_email='jonahpearl@g.harvard.edu',
     url='https://github.com/jonahpearl/videochef',
     packages=find_packages('src'),
     package_dir={'': 'src'},
@@ -38,8 +38,8 @@
 
         'Issue Tracker': 'https://github.com/jonahpearl/videochef/issues',
     },
     python_requires='>=3.6',
     install_requires=[
         'numpy', 'click', 'av', 'tqdm',
     ],
-)
+)
```

### Comparing `videochef-0.0.3/src/videochef/io.py` & `videochef-0.1.0/src/videochef/io.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,32 +2,75 @@
 import av
 import subprocess
 import datetime
 import os
 
 import pdb
 
-class videoWriter():
+class VideoWriter():
+    """A simple, ffmpeg-based video writer. Will try to infer grayscale vs. color (use RGB!), and act accordingly.
+    Inputs should be (nframes) x (w) x (h) x (RGB).
+
+    """
     def __init__(self, file_name, **ffmpeg_options):
         self.pipe = None
         self.file_name = file_name
         self.ffmpeg_options = ffmpeg_options
         
     def __enter__(self):
         return self
     
     def __exit__(self, type, value, traceback):
         if self.pipe is not None:
             self.pipe.stdin.close()
+            self.pipe.wait()  # wait for ffmpeg to finish so the video is ready to go on the next line of code; otherwise run into weird conditions where video isn't saved to disk yet
         
     def append(self, frames):
-        if len(frames.shape)==2: frames = frames[None]
-        self.pipe = write_frames(self.file_name, frames, pipe=self.pipe, **self.ffmpeg_options)
+        """Convert frames into an array (nframes) x (w) x (h) x color.
+        Frames should have color as final dimension, if at all.
+
+        Arguments:
+            frames {[type]} -- [description]
+        """
+
+        # Infer whether or not the frames have color
+        # Will fail if the video is 3 px tall...seems unlikely.
+        is_color = (len(frames.shape) >= 3) and (frames.shape[-1] == 3)
+
+        # Re-shape the array accordingly
+        if is_color and (len(frames.shape) == 3):
+            # If color but only one frame, add a singleton dim in front
+            frames = frames[None]
+        elif is_color and (len(frames.shape) == 4):
+            pass
+        elif len(frames.shape) == 2:
+            # If not color and only one frame, add a singleton dimension in front
+            frames = frames[None]
+
+        # Set default options if video is in color or gray.
+        if is_color:
+            pixel_format = self.ffmpeg_options.pop('pixel_format', 'rgb24')
+            codec = self.ffmpeg_options.pop('codec', 'h264')
+        else:
+            pixel_format = self.ffmpeg_options.pop('pixel_format', 'gray8')
+            codec = self.ffmpeg_options.pop('codec', 'ffv1')
+
+        if type(frames) ==  np.ndarray and len(frames.shape)==2:
+             frames = frames[None]
+
+        self.pipe = write_frames(
+            self.file_name, 
+            frames, 
+            pipe=self.pipe, 
+            pixel_format=pixel_format,
+            codec=codec,
+            **self.ffmpeg_options
+        )
 
-class videoReader():
+class VideoReader():
     def __init__(self, file_name, frame_ixs=None, reporter_val=None, mp4_to_gray=False):
         self.file_name = file_name
         self.file_ext = os.path.splitext(self.file_name)[1]
         self.frame_ixs = frame_ixs
         self.reporter_val = reporter_val
         self.mp4_to_gray = mp4_to_gray
 
@@ -99,18 +142,21 @@
             if self.reporter_val: print(f'read frame {ix} from reader {self.reporter_val}')
             if self.final_frame_ix is not None and (ix > self.final_frame_ix): break  # short circuit to speed up multiprocessing
             if frame_mask[ix]:
                 yield self.convert_frame_to_np(frame)
     
     
     def convert_frame_to_np(self, frame):
-        if self.file_ext == '.avi' and self.codec == 'ffv1' and self.pix_fmt == 'gray':
+        if self.file_ext == '.avi' and self.codec == 'ffv1' and 'gray' in self.pix_fmt:
             return frame.to_ndarray()
-        elif (self.file_ext == '.mp4' and self.codec == 'h264' and self.pix_fmt == 'yuvj420p') or \
-             (self.file_ext == '.mp4' and self.codec == 'mpeg4' and self.pix_fmt == 'yuv420p')  :
+        elif self.file_ext == '.avi' and self.codec == 'h264' and 'yuv' in self.pix_fmt:
+            return np.array(frame.to_image())
+        elif (self.file_ext == '.mp4' and self.codec == 'h264' and (self.pix_fmt == 'yuvj420p' or self.pix_fmt == 'yuv420p' or self.pix_fmt == 'yuv444p')) or \
+             (self.file_ext == '.mp4' and (self.codec == 'h265' or self.codec == 'hevc') and (self.pix_fmt == 'yuvj420p' or self.pix_fmt == 'yuv420p')) or \
+             (self.file_ext == '.mp4' and self.codec == 'mpeg4' and self.pix_fmt == 'yuv420p'):
             if self.mp4_to_gray:
                 return np.array(frame.to_image())[:,:,0]
             else:
                 return np.array(frame.to_image())
         else:
             raise NotImplementedError(f'Video format {self.file_ext} with codec {self.codec} and px fmt {self.pix_fmt} is not supported yet.')
     def __exit__(self, exc_type, exc_value, exc_traceback):
@@ -138,15 +184,15 @@
                '-slices', str(slices),
                '-slicecrc', str(slicecrc),
                '-r', str(fps),
                filename]
 
     if not pipe: pipe = subprocess.Popen(command, stdin=subprocess.PIPE, stderr=subprocess.PIPE)
     dtype = np.uint16 if pixel_format.startswith('gray16') else np.uint8
-    for i in range(frames.shape[0]): pipe.stdin.write(frames[i,:,:].astype(dtype).tobytes())
+    for i in range(frames.shape[0]): pipe.stdin.write(frames[i,...].astype(dtype).tobytes())
     return pipe
 
 
 def read_frames(filename, frames, threads=6, fps=30, frames_is_timestamp=False,
                 pixel_format='gray16', frame_size=(640,576),
                 slices=24, slicecrc=1, get_cmd=False):
     """
@@ -192,8 +238,8 @@
     out, err = pipe.communicate()
     if(err):
         print('error', err)
         return None
     
     dtype = ('uint16' if '16' in pixel_format else 'uint8')
     video = np.frombuffer(out, dtype=dtype).reshape((len(frames), frame_size[1], frame_size[0]))
-    return video
+    return video
```

### Comparing `videochef-0.0.3/src/videochef.egg-info/PKG-INFO` & `videochef-0.1.0/src/videochef.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videochef
-Version: 0.0.3
+Version: 0.1.0
 Summary: Whip up some fast, embarrassingly parallel video processing
 Home-page: https://github.com/jonahpearl/videochef
 Author: Jonah Pearl
 Author-email: jonahpearl@g.harvard.edu
 License: MIT
 Project-URL: Issue Tracker, https://github.com/jonahpearl/videochef/issues
 Classifier: Development Status :: 1 - Planning
```

