# Comparing `tmp/videochef-0.1.0.tar.gz` & `tmp/videochef-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jonahpearl/Documents/PiN/Datta lab/Local_code/videochef/dist/.tmp-umltyml8/videochef-0.1.0.tar", last modified: Wed Jul  5 19:26:29 2023, max compression
+gzip compressed data, was "/Users/jonahpearl/Documents/PiN/Datta lab/Local_code/videochef/dist/.tmp-kcmuckrz/videochef-0.1.1.tar", last modified: Thu Jul  6 04:29:09 2023, max compression
```

## Comparing `videochef-0.1.0.tar` & `videochef-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-05 19:26:29.000000 videochef-0.1.0/
--rw-r--r--   0 jonahpearl   (501) staff       (20)     1067 2022-11-14 03:17:49.000000 videochef-0.1.0/LICENSE.txt
--rw-r--r--   0 jonahpearl   (501) staff       (20)      757 2023-07-05 19:26:29.000000 videochef-0.1.0/PKG-INFO
--rw-r--r--   0 jonahpearl   (501) staff       (20)      247 2023-07-05 19:23:51.000000 videochef-0.1.0/README.md
--rw-r--r--   0 jonahpearl   (501) staff       (20)      227 2022-11-14 03:39:07.000000 videochef-0.1.0/pyproject.toml
--rw-r--r--   0 jonahpearl   (501) staff       (20)       78 2023-07-05 19:26:29.000000 videochef-0.1.0/setup.cfg
--rw-r--r--   0 jonahpearl   (501) staff       (20)     1381 2023-07-05 19:25:53.000000 videochef-0.1.0/setup.py
-drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-05 19:26:29.000000 videochef-0.1.0/src/
-drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef/
--rw-r--r--   0 jonahpearl   (501) staff       (20)       54 2023-07-05 19:23:51.000000 videochef-0.1.0/src/videochef/__init__.py
--rw-r--r--   0 jonahpearl   (501) staff       (20)    13178 2023-07-05 19:23:51.000000 videochef-0.1.0/src/videochef/chef.py
--rw-r--r--   0 jonahpearl   (501) staff       (20)    10109 2023-07-05 19:23:51.000000 videochef-0.1.0/src/videochef/io.py
--rw-r--r--   0 jonahpearl   (501) staff       (20)     3187 2023-07-05 19:23:51.000000 videochef-0.1.0/src/videochef/util.py
--rw-r--r--   0 jonahpearl   (501) staff       (20)     6850 2023-07-05 19:23:51.000000 videochef-0.1.0/src/videochef/viz.py
-drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/
--rw-r--r--   0 jonahpearl   (501) staff       (20)      757 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/PKG-INFO
--rw-r--r--   0 jonahpearl   (501) staff       (20)      442 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/SOURCES.txt
--rw-r--r--   0 jonahpearl   (501) staff       (20)        1 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/dependency_links.txt
--rw-r--r--   0 jonahpearl   (501) staff       (20)        1 2022-11-14 03:40:09.000000 videochef-0.1.0/src/videochef.egg-info/not-zip-safe
--rw-r--r--   0 jonahpearl   (501) staff       (20)       20 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/requires.txt
--rw-r--r--   0 jonahpearl   (501) staff       (20)       10 2023-07-05 19:26:29.000000 videochef-0.1.0/src/videochef.egg-info/top_level.txt
-drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-05 19:26:29.000000 videochef-0.1.0/tests/
--rw-r--r--   0 jonahpearl   (501) staff       (20)     3837 2023-07-05 19:23:51.000000 videochef-0.1.0/tests/test_chef.py
--rw-r--r--   0 jonahpearl   (501) staff       (20)     2965 2023-07-05 19:23:51.000000 videochef-0.1.0/tests/test_util.py
--rw-r--r--   0 jonahpearl   (501) staff       (20)     1445 2023-07-05 19:23:51.000000 videochef-0.1.0/tests/test_viz.py
+drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-06 04:29:09.703139 videochef-0.1.1/
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     1067 2022-11-14 03:17:49.000000 videochef-0.1.1/LICENSE.txt
+-rw-r--r--   0 jonahpearl   (501) staff       (20)      757 2023-07-06 04:29:09.703235 videochef-0.1.1/PKG-INFO
+-rw-r--r--   0 jonahpearl   (501) staff       (20)      247 2023-07-05 19:23:51.000000 videochef-0.1.1/README.md
+-rw-r--r--   0 jonahpearl   (501) staff       (20)      227 2022-11-14 03:39:07.000000 videochef-0.1.1/pyproject.toml
+-rw-r--r--   0 jonahpearl   (501) staff       (20)       78 2023-07-06 04:29:09.703582 videochef-0.1.1/setup.cfg
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     1381 2023-07-06 04:28:55.000000 videochef-0.1.1/setup.py
+drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-06 04:29:09.698501 videochef-0.1.1/src/
+drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-06 04:29:09.700936 videochef-0.1.1/src/videochef/
+-rw-r--r--   0 jonahpearl   (501) staff       (20)       73 2023-07-06 04:26:21.000000 videochef-0.1.1/src/videochef/__init__.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)    13178 2023-07-05 19:23:51.000000 videochef-0.1.1/src/videochef/chef.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)    12098 2023-07-06 04:26:21.000000 videochef-0.1.1/src/videochef/io.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     3187 2023-07-05 19:23:51.000000 videochef-0.1.1/src/videochef/util.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     8221 2023-07-06 04:26:21.000000 videochef-0.1.1/src/videochef/viz.py
+drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-06 04:29:09.702037 videochef-0.1.1/src/videochef.egg-info/
+-rw-r--r--   0 jonahpearl   (501) staff       (20)      757 2023-07-06 04:29:09.000000 videochef-0.1.1/src/videochef.egg-info/PKG-INFO
+-rw-r--r--   0 jonahpearl   (501) staff       (20)      442 2023-07-06 04:29:09.000000 videochef-0.1.1/src/videochef.egg-info/SOURCES.txt
+-rw-r--r--   0 jonahpearl   (501) staff       (20)        1 2023-07-06 04:29:09.000000 videochef-0.1.1/src/videochef.egg-info/dependency_links.txt
+-rw-r--r--   0 jonahpearl   (501) staff       (20)        1 2022-11-14 03:40:09.000000 videochef-0.1.1/src/videochef.egg-info/not-zip-safe
+-rw-r--r--   0 jonahpearl   (501) staff       (20)       20 2023-07-06 04:29:09.000000 videochef-0.1.1/src/videochef.egg-info/requires.txt
+-rw-r--r--   0 jonahpearl   (501) staff       (20)       10 2023-07-06 04:29:09.000000 videochef-0.1.1/src/videochef.egg-info/top_level.txt
+drwxr-xr-x   0 jonahpearl   (501) staff       (20)        0 2023-07-06 04:29:09.702939 videochef-0.1.1/tests/
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     3837 2023-07-05 19:23:51.000000 videochef-0.1.1/tests/test_chef.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     2965 2023-07-05 19:23:51.000000 videochef-0.1.1/tests/test_util.py
+-rw-r--r--   0 jonahpearl   (501) staff       (20)     1445 2023-07-05 19:23:51.000000 videochef-0.1.1/tests/test_viz.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `videochef-0.1.0/LICENSE.txt` & `videochef-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `videochef-0.1.0/PKG-INFO` & `videochef-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videochef
-Version: 0.1.0
+Version: 0.1.1
 Summary: Whip up some fast, embarrassingly parallel video processing
 Home-page: https://github.com/jonahpearl/videochef
 Author: Jonah Pearl
 Author-email: jonahpearl@g.harvard.edu
 License: MIT
 Project-URL: Issue Tracker, https://github.com/jonahpearl/videochef/issues
 Classifier: Development Status :: 1 - Planning
```

### Comparing `videochef-0.1.0/setup.py` & `videochef-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name='videochef',
-    version='0.1.0',
+    version='0.1.1',
     license='MIT',
     description='Whip up some fast, embarrassingly parallel video processing',
     author='Jonah Pearl',
     author_email='jonahpearl@g.harvard.edu',
     url='https://github.com/jonahpearl/videochef',
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `videochef-0.1.0/src/videochef/chef.py` & `videochef-0.1.1/src/videochef/chef.py`

 * *Files identical despite different names*

### Comparing `videochef-0.1.0/src/videochef/io.py` & `videochef-0.1.1/src/videochef/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 import pdb
 
 class VideoWriter():
     """A simple, ffmpeg-based video writer. Will try to infer grayscale vs. color (use RGB!), and act accordingly.
     Inputs should be (nframes) x (w) x (h) x (RGB).
 
     """
-    def __init__(self, file_name, **ffmpeg_options):
+    def __init__(self, file_name, **write_frames_options):
         self.pipe = None
         self.file_name = file_name
-        self.ffmpeg_options = ffmpeg_options
+        self.write_frame_options = write_frames_options
         
     def __enter__(self):
         return self
     
     def __exit__(self, type, value, traceback):
         if self.pipe is not None:
             self.pipe.stdin.close()
             self.pipe.wait()  # wait for ffmpeg to finish so the video is ready to go on the next line of code; otherwise run into weird conditions where video isn't saved to disk yet
         
     def append(self, frames):
-        """Convert frames into an array (nframes) x (w) x (h) x color.
+        """Write frames to the file.
+        Will convert frames into an array (nframes) x (w) x (h) x color, by inference.
         Frames should have color as final dimension, if at all.
 
         Arguments:
             frames {[type]} -- [description]
         """
 
         # Infer whether or not the frames have color
@@ -44,30 +45,30 @@
             pass
         elif len(frames.shape) == 2:
             # If not color and only one frame, add a singleton dimension in front
             frames = frames[None]
 
         # Set default options if video is in color or gray.
         if is_color:
-            pixel_format = self.ffmpeg_options.pop('pixel_format', 'rgb24')
-            codec = self.ffmpeg_options.pop('codec', 'h264')
+            pixel_format = self.write_frame_options.pop('pixel_format', 'yuv420p')  # output pixel format
+            codec = self.write_frame_options.pop('codec', 'libx264')
         else:
-            pixel_format = self.ffmpeg_options.pop('pixel_format', 'gray8')
-            codec = self.ffmpeg_options.pop('codec', 'ffv1')
+            pixel_format = self.write_frame_options.pop('pixel_format', 'gray8')
+            codec = self.write_frame_options.pop('codec', 'ffv1')
 
-        if type(frames) ==  np.ndarray and len(frames.shape)==2:
-             frames = frames[None]
+        # if type(frames) ==  np.ndarray and len(frames.shape) == 2:
+        #      frames = frames[None]
 
         self.pipe = write_frames(
             self.file_name, 
             frames, 
             pipe=self.pipe, 
             pixel_format=pixel_format,
             codec=codec,
-            **self.ffmpeg_options
+            **self.write_frame_options
         )
 
 class VideoReader():
     def __init__(self, file_name, frame_ixs=None, reporter_val=None, mp4_to_gray=False):
         self.file_name = file_name
         self.file_ext = os.path.splitext(self.file_name)[1]
         self.frame_ixs = frame_ixs
@@ -161,34 +162,77 @@
             raise NotImplementedError(f'Video format {self.file_ext} with codec {self.codec} and px fmt {self.pix_fmt} is not supported yet.')
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.reader.close()            
                 
 def write_frames(filename, frames, 
                  threads=6, fps=30, crf=10,
                  pixel_format='gray8', codec='ffv1',
-                 pipe=None, slices=24, slicecrc=1):
+                 pipe=None, slices=24, slicecrc=1,
+                 preset='veryfast'):
+    """Use ffmpeg to write frames into a movie
+
+    Arguments:
+        filename {str} -- full filename of video to write
+        frames {iterable of arrays} -- the frames to write. Should be numpy arrays (probably uint8's)
+
+    Keyword Arguments:
+        threads {int} -- n threads for ffmpeg (default: {6})
+        fps {int} -- desired output fps (default: {30})
+        crf {int} -- quality factor. Normal default is 23, here we boost it a bit (lower is better), because science. (default: {10})
+        pixel_format {str} -- output pixel format. For quicktime playable movies, use "yuv420p" and pass 3D frames (). (default: {'gray8'})
+        codec {str} -- video codec to use. For color, prefer "libx264" (default: {'ffv1'})
+        pipe {[type]} -- internal use (default: {None})
+        slices {int} -- number of ffmpeg slices (default: {24})
+        slicecrc {int} -- ? (default: {1})
+
+    Returns:
+        [type] -- [description]
+    """
     
     frame_size = '{0:d}x{1:d}'.format(frames.shape[2], frames.shape[1])
-    command = ['ffmpeg',
-               '-y',
-               '-loglevel', 'fatal',
-               '-framerate', str(fps),
-               '-f', 'rawvideo',
-               '-s', frame_size,
-               '-pix_fmt', pixel_format,
-               '-i', '-',
-               '-an',
-               '-crf',str(crf),
-               '-vcodec', codec,
-               '-preset', 'ultrafast',
-               '-threads', str(threads),
-               '-slices', str(slices),
-               '-slicecrc', str(slicecrc),
-               '-r', str(fps),
-               filename]
+
+    if pixel_format == 'gray8' or 'rgb' in pixel_format:
+        command = ['ffmpeg',
+                '-y',
+                '-loglevel', 'fatal',
+                '-framerate', str(fps),
+                '-f', 'rawvideo',
+                '-s', frame_size,
+                '-pix_fmt', pixel_format,
+                '-i', '-',
+                '-an',
+                '-crf',str(crf),
+                '-vcodec', codec,
+                '-preset', preset,
+                '-threads', str(threads),
+                '-slices', str(slices),
+                '-slicecrc', str(slicecrc),
+                '-r', str(fps),
+                filename]
+    elif 'yuv' in pixel_format:
+        # assume user is passing rgb (unlikely to be passing yuv formatted arrays)
+        command = ['ffmpeg',
+                '-y',
+                '-loglevel', 'fatal',
+                '-framerate', str(fps),
+                '-f', 'rawvideo',
+                '-s', frame_size,
+                '-pix_fmt', 'rgb24',  # user will pass input as rgb...
+                '-i', '-',
+                '-an',
+                '-crf',str(crf),
+                '-c:v', 'libx264',
+                '-pix_fmt', pixel_format,  # ...but output will be converted to yuv
+                '-preset', preset,
+                '-threads', str(threads),
+                '-slices', str(slices),
+                '-slicecrc', str(slicecrc),
+                '-r', str(fps),
+                filename]
+
 
     if not pipe: pipe = subprocess.Popen(command, stdin=subprocess.PIPE, stderr=subprocess.PIPE)
     dtype = np.uint16 if pixel_format.startswith('gray16') else np.uint8
     for i in range(frames.shape[0]): pipe.stdin.write(frames[i,...].astype(dtype).tobytes())
     return pipe
```

### Comparing `videochef-0.1.0/src/videochef/util.py` & `videochef-0.1.1/src/videochef/util.py`

 * *Files identical despite different names*

### Comparing `videochef-0.1.0/src/videochef/viz.py` & `videochef-0.1.1/src/videochef/viz.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     in_vid_name,
     out_vid_name,
     peri_evt_frames_list,
     event_frame_num_in_vid=None,
     traces=None,
     trace_to_vid_fs_ratio=None,
     out_fps=12,
-    overwrite=False
+    overwrite=False,
+    **write_frame_kwargs,
 ):
     """Create a tiled gallery of peri-event videos
 
     Arguments:
         in_vid_name {path} -- video to read
         out_vid_name {path} -- video to write
         peri_evt_frames_list {list of iterables} -- peri-event frame lists for each event
@@ -66,30 +67,55 @@
     Keyword Arguments:
         traces {array} -- TODO: allow user to display sync'd traces (default: {None})
         trace_to_vid_fs_ratio {[type]} -- TODO: ^^ (default: {None})
         out_fps {int} -- desired fps of written video. Often nice to slow it down. (default: {12})
         overwrite {bool} -- if True, overwrites any existing video at out_vid_name (default: {False})
 
     Returns: n/a
+
+    Dummy example:
+        # makes peri-event vids from 0.5 sec before to 1.5 sec after the event's frame
+        movie_path = '/path/to/your/movie.mp4'  # at least ~ 1100 frames long for this example
+        fps = 30
+        overwrite = False
+        window = (-0.5, 1.5)
+        event_idx_in_vid = np.arange(0,1000,100)
+        peristim_frames_list = [np.arange(idx+window[0]*vid_fps, idx+window[1]*vid_fps) for idx in event_idx_in_vid]
+        out_vid_name = movie_path.replace('movie', 'perievent_movie')
+        try:
+            videochef.viz.peri_event_vid(
+                movie_path,
+                out_vid_name,
+                peri_evt_frames_list=peristim_frames_list,
+                event_frame_num_in_vid=(0 - window[0])*vid_fps,
+                out_fps=fps/5,  # slow down the output
+                overwrite=overwrite,
+            )
+        except BrokenPipeError:
+            warnings.warn('Encountered broken pipe, skipping...')
+        
     """
 
     # Plan layout to be as close to square as possible
     num_stims = len(peri_evt_frames_list)
     nrows = np.ceil(np.sqrt(num_stims)).astype('int')
 
-    # Skip already existing vids?
+    # Skip already existing vids
     if exists(out_vid_name) and not overwrite: 
         return None
 
-    # One video per odor/session pair.
+    # libx264 is a better verison of h264.
+    # yuv420 is open-able by quicktime and most video players.
+    # NB, user should still pass in RGB frames -- it will be converted by ffmpeg into yuv (see videochef.io.write_frames()).
     waiting_writer = VideoWriter(
         out_vid_name, 
         fps=out_fps, 
-        codec='h264', 
-        pixel_format='rgb24'  # 8 bit, 3 colors
+        codec='libx264', 
+        pixel_format='yuv420p',  
+        **write_frame_kwargs,
     )
     with ExitStack() as stack:
 
         # Get video readers (and they seek to exactly the right place on this line!)
         print('Getting readers...')
         peristim_readers = [
             stack.enter_context(
@@ -112,15 +138,18 @@
             # Add each mini-frame to the big frame
             panels,titles = [],[]  # empty lists for frame
 
             ii = 0  # counter for layout
             for iReader, frame in enumerate(frames):
 
                 # Convert frame to RGB if it isn't already
-                frame = np.stack(3 * (frame,), axis=-1)
+                if frame.ndim == 2:
+                    frame = np.stack(3 * (frame,), axis=-1)
+                elif frame.ndim != 3:
+                    raise ValueError('Expected 3D frames but got frames of shape {frame.shape}')
 
                 # Append a mark for whether event fr has passed or not
                 if event_frame_num_in_vid is not None:
                     if (ix < event_frame_num_in_vid):
                         fill = 1
                     else:
                         fill = -1  # for some reason, -1 fills it
```

### Comparing `videochef-0.1.0/src/videochef.egg-info/PKG-INFO` & `videochef-0.1.1/src/videochef.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videochef
-Version: 0.1.0
+Version: 0.1.1
 Summary: Whip up some fast, embarrassingly parallel video processing
 Home-page: https://github.com/jonahpearl/videochef
 Author: Jonah Pearl
 Author-email: jonahpearl@g.harvard.edu
 License: MIT
 Project-URL: Issue Tracker, https://github.com/jonahpearl/videochef/issues
 Classifier: Development Status :: 1 - Planning
```

### Comparing `videochef-0.1.0/tests/test_chef.py` & `videochef-0.1.1/tests/test_chef.py`

 * *Files identical despite different names*

### Comparing `videochef-0.1.0/tests/test_util.py` & `videochef-0.1.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `videochef-0.1.0/tests/test_viz.py` & `videochef-0.1.1/tests/test_viz.py`

 * *Files identical despite different names*

