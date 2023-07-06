# Comparing `tmp/Abg-2.1.tar.gz` & `tmp/Abg-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-2.1.tar", last modified: Sat Jul  1 13:41:32 2023, max compression
+gzip compressed data, was "Abg-2.2.tar", last modified: Thu Jul  6 10:34:07 2023, max compression
```

## Comparing `Abg-2.1.tar` & `Abg-2.2.tar`

### file list

```diff
@@ -1,45 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.001030 Abg-2.1/Abg/
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-01 13:41:05.000000 Abg-2.1/Abg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.001030 Abg-2.1/Abg/chat_status/
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-01 13:41:05.000000 Abg-2.1/Abg/chat_status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-07-01 13:41:05.000000 Abg-2.1/Abg/chat_status/chat_status.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-07-01 13:41:05.000000 Abg-2.1/Abg/chat_status/custom_filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/helpers/
--rw-r--r--   0 root         (0) root         (0)      831 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3179 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/human_read.py
--rw-r--r--   0 root         (0) root         (0)     7350 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/msg_types.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/parser.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/pyro_progress.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/ratelimit.py
--rw-r--r--   0 root         (0) root         (0)     5357 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/inline/
--rw-r--r--   0 root         (0) root         (0)      274 2023-07-01 13:41:05.000000 Abg-2.1/Abg/inline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6105 2023-07-01 13:41:05.000000 Abg-2.1/Abg/inline/inline_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     4267 2023-07-01 13:41:05.000000 Abg-2.1/Abg/inline/inline_pagination_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-07-01 13:41:05.000000 Abg-2.1/Abg/inline/reply_keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/patch/
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/patch/bound/
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/bound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11979 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/bound/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/patch/listen/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12016 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/listen/listen.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/listen/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/patch/methods/
--rw-r--r--   0 root         (0) root         (0)      127 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/methods/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/methods/send_as_file.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/methods/send_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.001030 Abg-2.1/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4948 2023-07-01 13:41:31.000000 Abg-2.1/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      877 2023-07-01 13:41:31.000000 Abg-2.1/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 13:41:31.000000 Abg-2.1/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-01 13:41:31.000000 Abg-2.1/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4948 2023-07-01 13:41:32.005030 Abg-2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2420 2023-07-01 13:41:05.000000 Abg-2.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-01 13:41:32.005030 Abg-2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2994 2023-07-01 13:41:05.000000 Abg-2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:07.428015 Abg-2.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:07.420015 Abg-2.2/Abg/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-07-06 10:29:41.000000 Abg-2.2/Abg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:07.420015 Abg-2.2/Abg/chat_status/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-06 10:29:41.000000 Abg-2.2/Abg/chat_status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-07-06 10:29:41.000000 Abg-2.2/Abg/chat_status/chat_status.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-07-06 10:29:41.000000 Abg-2.2/Abg/chat_status/custom_filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:07.420015 Abg-2.2/Abg/helpers/
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-06 10:29:41.000000 Abg-2.2/Abg/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-07-06 10:29:41.000000 Abg-2.2/Abg/helpers/get_user.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2023-07-06 10:29:41.000000 Abg-2.2/Abg/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-07-06 10:29:41.000000 Abg-2.2/Abg/helpers/http_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-07-06 10:29:41.000000 Abg-2.2/Abg/helpers/human_read.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-06 10:29:41.000000 Abg-2.2/Abg/helpers/msg_types.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-07-06 10:29:41.000000 Abg-2.2/Abg/helpers/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-07-06 10:29:41.000000 Abg-2.2/Abg/helpers/pyro_progress.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-07-06 10:29:41.000000 Abg-2.2/Abg/helpers/ratelimit.py
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-07-06 10:29:41.000000 Abg-2.2/Abg/helpers/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:07.424015 Abg-2.2/Abg/inline/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-06 10:29:41.000000 Abg-2.2/Abg/inline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6105 2023-07-06 10:29:41.000000 Abg-2.2/Abg/inline/inline_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-07-06 10:29:41.000000 Abg-2.2/Abg/inline/inline_pagination_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-07-06 10:29:41.000000 Abg-2.2/Abg/inline/reply_keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:07.424015 Abg-2.2/Abg/patch/
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:07.424015 Abg-2.2/Abg/patch/bound/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/bound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11979 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/bound/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:07.424015 Abg-2.2/Abg/patch/decorators/
+-rw-r--r--   0 root         (0) root         (0)       95 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/decorators/callback.py
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/decorators/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:07.424015 Abg-2.2/Abg/patch/listen/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12016 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/listen/listen.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/listen/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:07.424015 Abg-2.2/Abg/patch/methods/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/methods/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/methods/send_as_file.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-06 10:29:41.000000 Abg-2.2/Abg/patch/methods/send_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:07.420015 Abg-2.2/Abg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-07-06 10:34:07.000000 Abg-2.2/Abg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-07-06 10:34:07.000000 Abg-2.2/Abg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 10:34:07.000000 Abg-2.2/Abg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 10:34:07.000000 Abg-2.2/Abg.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 10:34:07.000000 Abg-2.2/Abg.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-06 10:34:07.000000 Abg-2.2/Abg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-07-06 10:34:07.428015 Abg-2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2336 2023-07-06 10:29:41.000000 Abg-2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 10:34:07.428015 Abg-2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3073 2023-07-06 10:29:41.000000 Abg-2.2/setup.py
```

### Comparing `Abg-2.1/Abg/chat_status/chat_status.py` & `Abg-2.2/Abg/chat_status/chat_status.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/chat_status/custom_filters.py` & `Abg-2.2/Abg/chat_status/custom_filters.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/helpers/__init__.py` & `Abg-2.2/Abg/helpers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 You should have received a copy of the GNU General Public License.
 
 along with Abg.  If not, see <https://www.gnu.org/licenses/>.
 """
+from .get_user import *
 from .helpers import *
 from .human_read import *
+from .msg_types import *
 from .parser import *
 from .pyro_progress import *
-from .msg_types import *
 from .string import *
```

### Comparing `Abg-2.1/Abg/helpers/helpers.py` & `Abg-2.2/Abg/helpers/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,27 +16,28 @@
                 btn(button, button) if type(button) == str else btn(*button)
             )  # InlineKeyboardButton
             line.append(button)
         lines.append(line)
     return InlineKeyboardMarkup(inline_keyboard=lines)
     # return {'inline_keyboard': lines}
 
+
 def ikb2(rows=None, back=False, todo="start_back"):
     # rows = pass the rows
     # back - if want to make back button
     # todo - callback data of back button
 
     if rows is None:
         rows = []
     lines = []
     try:
         for row in rows:
             line = []
             for button in row:
-                btn_text = button.split(".")[1].upper()
+                btn_text = button.split(".")[1].capitalize()
                 button = btn(btn_text, button)  # InlineKeyboardButton
                 line.append(button)
             lines.append(line)
     except AttributeError:
         for row in rows:
             line = []
             for button in row:
@@ -51,14 +52,15 @@
             line.append(button)
         lines.append(line)
     if back:
         back_btn = [(btn("« ʙᴀᴄᴋ", todo))]
         lines.append(back_btn)
     return InlineKeyboardMarkup(inline_keyboard=lines)
 
+
 def btn(text, value, type="callback_data"):
     return InlineKeyboardButton(text, **{type: value})
     # return {'text': text, type: value}
 
 
 # The inverse of above
 def bki(keyboard):
@@ -112,9 +114,7 @@
 
 def force_reply(selective=True):
     return ForceReply(selective=selective)
 
 
 def array_chunk(input, size):
     return [input[i : i + size] for i in range(0, len(input), size)]
-
-
```

### Comparing `Abg-2.1/Abg/helpers/http_helper.py` & `Abg-2.2/Abg/helpers/http_helper.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/helpers/human_read.py` & `Abg-2.2/Abg/helpers/human_read.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/helpers/msg_types.py` & `Abg-2.2/Abg/helpers/msg_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,448 +13,448 @@
 000000c0: 5449 434b 4552 203d 2035 0a20 2020 2041  TICKER = 5.    A
 000000d0: 5544 494f 203d 2036 0a20 2020 2056 4f49  UDIO = 6.    VOI
 000000e0: 4345 203d 2037 0a20 2020 2056 4944 454f  CE = 7.    VIDEO
 000000f0: 5f4e 4f54 4520 3d20 380a 2020 2020 414e  _NOTE = 8.    AN
 00000100: 494d 4154 494f 4e20 3d20 390a 2020 2020  IMATION = 9.    
 00000110: 414e 494d 4154 4544 5f53 5449 434b 4552  ANIMATED_STICKER
 00000120: 203d 2031 300a 2020 2020 434f 4e54 4143   = 10.    CONTAC
-00000130: 5420 3d20 3131 0a0a 6173 796e 6320 6465  T = 11..async de
-00000140: 6620 7365 6e64 5f63 6d64 2863 3a20 436c  f send_cmd(c: Cl
-00000150: 6965 6e74 2c20 6d73 6774 7970 653a 2069  ient, msgtype: i
-00000160: 6e74 293a 0a20 2020 2047 4554 5f46 4f52  nt):.    GET_FOR
-00000170: 4d41 5420 3d20 7b0a 2020 2020 2020 2020  MAT = {.        
-00000180: 5479 7065 732e 5445 5854 2e76 616c 7565  Types.TEXT.value
-00000190: 3a20 632e 7365 6e64 5f6d 6573 7361 6765  : c.send_message
-000001a0: 2c0a 2020 2020 2020 2020 5479 7065 732e  ,.        Types.
-000001b0: 444f 4355 4d45 4e54 2e76 616c 7565 3a20  DOCUMENT.value: 
-000001c0: 632e 7365 6e64 5f64 6f63 756d 656e 742c  c.send_document,
-000001d0: 0a20 2020 2020 2020 2054 7970 6573 2e50  .        Types.P
-000001e0: 484f 544f 2e76 616c 7565 3a20 632e 7365  HOTO.value: c.se
-000001f0: 6e64 5f70 686f 746f 2c0a 2020 2020 2020  nd_photo,.      
-00000200: 2020 5479 7065 732e 5649 4445 4f2e 7661    Types.VIDEO.va
-00000210: 6c75 653a 2063 2e73 656e 645f 7669 6465  lue: c.send_vide
-00000220: 6f2c 0a20 2020 2020 2020 2054 7970 6573  o,.        Types
-00000230: 2e53 5449 434b 4552 2e76 616c 7565 3a20  .STICKER.value: 
-00000240: 632e 7365 6e64 5f73 7469 636b 6572 2c0a  c.send_sticker,.
-00000250: 2020 2020 2020 2020 5479 7065 732e 4155          Types.AU
-00000260: 4449 4f2e 7661 6c75 653a 2063 2e73 656e  DIO.value: c.sen
-00000270: 645f 6175 6469 6f2c 0a20 2020 2020 2020  d_audio,.       
-00000280: 2054 7970 6573 2e56 4f49 4345 2e76 616c   Types.VOICE.val
-00000290: 7565 3a20 632e 7365 6e64 5f76 6f69 6365  ue: c.send_voice
-000002a0: 2c0a 2020 2020 2020 2020 5479 7065 732e  ,.        Types.
-000002b0: 5649 4445 4f5f 4e4f 5445 2e76 616c 7565  VIDEO_NOTE.value
-000002c0: 3a20 632e 7365 6e64 5f76 6964 656f 5f6e  : c.send_video_n
-000002d0: 6f74 652c 0a20 2020 2020 2020 2054 7970  ote,.        Typ
-000002e0: 6573 2e41 4e49 4d41 5449 4f4e 2e76 616c  es.ANIMATION.val
-000002f0: 7565 3a20 632e 7365 6e64 5f61 6e69 6d61  ue: c.send_anima
-00000300: 7469 6f6e 2c0a 2020 2020 2020 2020 5479  tion,.        Ty
-00000310: 7065 732e 414e 494d 4154 4544 5f53 5449  pes.ANIMATED_STI
-00000320: 434b 4552 2e76 616c 7565 3a20 632e 7365  CKER.value: c.se
-00000330: 6e64 5f73 7469 636b 6572 2c0a 2020 2020  nd_sticker,.    
-00000340: 2020 2020 5479 7065 732e 434f 4e54 4143      Types.CONTAC
-00000350: 543a 2063 2e73 656e 645f 636f 6e74 6163  T: c.send_contac
-00000360: 742c 0a20 2020 207d 0a20 2020 2072 6574  t,.    }.    ret
-00000370: 7572 6e20 4745 545f 464f 524d 4154 5b6d  urn GET_FORMAT[m
-00000380: 7367 7479 7065 5d0a 0a0a 6173 796e 6320  sgtype]...async 
-00000390: 6465 6620 6765 745f 6e6f 7465 5f74 7970  def get_note_typ
-000003a0: 6528 6d3a 204d 6573 7361 6765 293a 0a20  e(m: Message):. 
-000003b0: 2020 2022 2222 4765 7420 7479 7065 206f     """Get type o
-000003c0: 6620 6e6f 7465 2e22 2222 0a20 2020 2069  f note.""".    i
-000003d0: 6620 6c65 6e28 6d2e 7465 7874 2e73 706c  f len(m.text.spl
-000003e0: 6974 2829 2920 3c3d 2031 3a0a 2020 2020  it()) <= 1:.    
-000003f0: 2020 2020 7265 7475 726e 204e 6f6e 652c      return None,
-00000400: 204e 6f6e 652c 204e 6f6e 652c 204e 6f6e   None, None, Non
-00000410: 650a 0a20 2020 2064 6174 615f 7479 7065  e..    data_type
-00000420: 203d 204e 6f6e 650a 2020 2020 636f 6e74   = None.    cont
-00000430: 656e 7420 3d20 4e6f 6e65 0a20 2020 2072  ent = None.    r
-00000440: 6177 5f74 6578 7420 3d20 6d2e 7465 7874  aw_text = m.text
-00000450: 2e6d 6172 6b64 6f77 6e20 6966 206d 2e74  .markdown if m.t
-00000460: 6578 7420 656c 7365 206d 2e63 6170 7469  ext else m.capti
-00000470: 6f6e 2e6d 6172 6b64 6f77 6e0a 2020 2020  on.markdown.    
-00000480: 6172 6773 203d 2072 6177 5f74 6578 742e  args = raw_text.
-00000490: 7370 6c69 7428 4e6f 6e65 2c20 3229 0a20  split(None, 2). 
-000004a0: 2020 206e 6f74 655f 6e61 6d65 203d 2061     note_name = a
-000004b0: 7267 735b 315d 0a0a 2020 2020 6966 206c  rgs[1]..    if l
-000004c0: 656e 2861 7267 7329 203e 3d20 333a 0a20  en(args) >= 3:. 
-000004d0: 2020 2020 2020 2074 6578 7420 3d20 6172         text = ar
-000004e0: 6773 5b32 5d0a 2020 2020 2020 2020 6461  gs[2].        da
-000004f0: 7461 5f74 7970 6520 3d20 5479 7065 732e  ta_type = Types.
-00000500: 5445 5854 0a0a 2020 2020 656c 6966 206d  TEXT..    elif m
-00000510: 2e72 6570 6c79 5f74 6f5f 6d65 7373 6167  .reply_to_messag
-00000520: 653a 0a20 2020 2020 2020 2069 6620 6d2e  e:.        if m.
-00000530: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-00000540: 2e74 6578 743a 0a20 2020 2020 2020 2020  .text:.         
-00000550: 2020 2074 6578 7420 3d20 6d2e 7265 706c     text = m.repl
-00000560: 795f 746f 5f6d 6573 7361 6765 2e74 6578  y_to_message.tex
-00000570: 742e 6d61 726b 646f 776e 0a20 2020 2020  t.markdown.     
-00000580: 2020 2065 6c69 6620 6d2e 7265 706c 795f     elif m.reply_
-00000590: 746f 5f6d 6573 7361 6765 2e63 6170 7469  to_message.capti
-000005a0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-000005b0: 7465 7874 203d 206d 2e72 6570 6c79 5f74  text = m.reply_t
-000005c0: 6f5f 6d65 7373 6167 652e 6361 7074 696f  o_message.captio
-000005d0: 6e2e 6d61 726b 646f 776e 0a20 2020 2020  n.markdown.     
-000005e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000005f0: 2020 2020 2074 6578 7420 3d20 2222 0a0a       text = ""..
-00000600: 2020 2020 2020 2020 6966 206c 656e 2861          if len(a
-00000610: 7267 7329 203e 3d20 3220 616e 6420 6d2e  rgs) >= 2 and m.
-00000620: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-00000630: 2e74 6578 743a 2020 2320 6e6f 7420 6361  .text:  # not ca
-00000640: 7074 696f 6e2c 2074 6578 740a 2020 2020  ption, text.    
-00000650: 2020 2020 2020 2020 6461 7461 5f74 7970          data_typ
-00000660: 6520 3d20 5479 7065 732e 5445 5854 0a0a  e = Types.TEXT..
-00000670: 2020 2020 2020 2020 656c 6966 206d 2e72          elif m.r
-00000680: 6570 6c79 5f74 6f5f 6d65 7373 6167 652e  eply_to_message.
-00000690: 7374 6963 6b65 723a 0a20 2020 2020 2020  sticker:.       
-000006a0: 2020 2020 2063 6f6e 7465 6e74 203d 206d       content = m
-000006b0: 2e72 6570 6c79 5f74 6f5f 6d65 7373 6167  .reply_to_messag
-000006c0: 652e 7374 6963 6b65 722e 6669 6c65 5f69  e.sticker.file_i
-000006d0: 640a 2020 2020 2020 2020 2020 2020 6461  d.            da
-000006e0: 7461 5f74 7970 6520 3d20 5479 7065 732e  ta_type = Types.
-000006f0: 5354 4943 4b45 520a 0a20 2020 2020 2020  STICKER..       
-00000700: 2065 6c69 6620 6d2e 7265 706c 795f 746f   elif m.reply_to
-00000710: 5f6d 6573 7361 6765 2e64 6f63 756d 656e  _message.documen
-00000720: 743a 0a20 2020 2020 2020 2020 2020 2069  t:.            i
-00000730: 6620 6d2e 7265 706c 795f 746f 5f6d 6573  f m.reply_to_mes
-00000740: 7361 6765 2e64 6f63 756d 656e 742e 6d69  sage.document.mi
-00000750: 6d65 5f74 7970 6520 3d3d 2022 6170 706c  me_type == "appl
-00000760: 6963 6174 696f 6e2f 782d 6261 642d 7467  ication/x-bad-tg
-00000770: 7374 6963 6b65 7222 3a0a 2020 2020 2020  sticker":.      
-00000780: 2020 2020 2020 2020 2020 6461 7461 5f74            data_t
-00000790: 7970 6520 3d20 5479 7065 732e 414e 494d  ype = Types.ANIM
-000007a0: 4154 4544 5f53 5449 434b 4552 0a20 2020  ATED_STICKER.   
-000007b0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000007c0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000007d0: 6174 615f 7479 7065 203d 2054 7970 6573  ata_type = Types
-000007e0: 2e44 4f43 554d 454e 540a 2020 2020 2020  .DOCUMENT.      
-000007f0: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
-00000800: 6d2e 7265 706c 795f 746f 5f6d 6573 7361  m.reply_to_messa
-00000810: 6765 2e64 6f63 756d 656e 742e 6669 6c65  ge.document.file
-00000820: 5f69 640a 0a20 2020 2020 2020 2065 6c69  _id..        eli
-00000830: 6620 6d2e 7265 706c 795f 746f 5f6d 6573  f m.reply_to_mes
-00000840: 7361 6765 2e70 686f 746f 3a0a 2020 2020  sage.photo:.    
-00000850: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
-00000860: 3d20 6d2e 7265 706c 795f 746f 5f6d 6573  = m.reply_to_mes
-00000870: 7361 6765 2e70 686f 746f 2e66 696c 655f  sage.photo.file_
-00000880: 6964 2020 2320 6c61 7374 2065 6c65 6d20  id  # last elem 
-00000890: 3d20 6265 7374 2071 7561 6c69 7479 0a20  = best quality. 
-000008a0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-000008b0: 7479 7065 203d 2054 7970 6573 2e50 484f  type = Types.PHO
-000008c0: 544f 0a0a 2020 2020 2020 2020 656c 6966  TO..        elif
-000008d0: 206d 2e72 6570 6c79 5f74 6f5f 6d65 7373   m.reply_to_mess
-000008e0: 6167 652e 6175 6469 6f3a 0a20 2020 2020  age.audio:.     
-000008f0: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
-00000900: 206d 2e72 6570 6c79 5f74 6f5f 6d65 7373   m.reply_to_mess
-00000910: 6167 652e 6175 6469 6f2e 6669 6c65 5f69  age.audio.file_i
-00000920: 640a 2020 2020 2020 2020 2020 2020 6461  d.            da
-00000930: 7461 5f74 7970 6520 3d20 5479 7065 732e  ta_type = Types.
-00000940: 4155 4449 4f0a 0a20 2020 2020 2020 2065  AUDIO..        e
-00000950: 6c69 6620 6d2e 7265 706c 795f 746f 5f6d  lif m.reply_to_m
-00000960: 6573 7361 6765 2e76 6f69 6365 3a0a 2020  essage.voice:.  
-00000970: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
-00000980: 7420 3d20 6d2e 7265 706c 795f 746f 5f6d  t = m.reply_to_m
-00000990: 6573 7361 6765 2e76 6f69 6365 2e66 696c  essage.voice.fil
-000009a0: 655f 6964 0a20 2020 2020 2020 2020 2020  e_id.           
-000009b0: 2064 6174 615f 7479 7065 203d 2054 7970   data_type = Typ
-000009c0: 6573 2e56 4f49 4345 0a0a 2020 2020 2020  es.VOICE..      
-000009d0: 2020 656c 6966 206d 2e72 6570 6c79 5f74    elif m.reply_t
-000009e0: 6f5f 6d65 7373 6167 652e 7669 6465 6f3a  o_message.video:
-000009f0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00000a00: 7465 6e74 203d 206d 2e72 6570 6c79 5f74  tent = m.reply_t
-00000a10: 6f5f 6d65 7373 6167 652e 7669 6465 6f2e  o_message.video.
-00000a20: 6669 6c65 5f69 640a 2020 2020 2020 2020  file_id.        
-00000a30: 2020 2020 6461 7461 5f74 7970 6520 3d20      data_type = 
-00000a40: 5479 7065 732e 5649 4445 4f0a 0a20 2020  Types.VIDEO..   
-00000a50: 2020 2020 2065 6c69 6620 6d2e 7265 706c       elif m.repl
-00000a60: 795f 746f 5f6d 6573 7361 6765 2e76 6964  y_to_message.vid
-00000a70: 656f 5f6e 6f74 653a 0a20 2020 2020 2020  eo_note:.       
-00000a80: 2020 2020 2063 6f6e 7465 6e74 203d 206d       content = m
-00000a90: 2e72 6570 6c79 5f74 6f5f 6d65 7373 6167  .reply_to_messag
-00000aa0: 652e 7669 6465 6f5f 6e6f 7465 2e66 696c  e.video_note.fil
-00000ab0: 655f 6964 0a20 2020 2020 2020 2020 2020  e_id.           
-00000ac0: 2064 6174 615f 7479 7065 203d 2054 7970   data_type = Typ
-00000ad0: 6573 2e56 4944 454f 5f4e 4f54 450a 0a20  es.VIDEO_NOTE.. 
-00000ae0: 2020 2020 2020 2065 6c69 6620 6d2e 7265         elif m.re
-00000af0: 706c 795f 746f 5f6d 6573 7361 6765 2e61  ply_to_message.a
-00000b00: 6e69 6d61 7469 6f6e 3a0a 2020 2020 2020  nimation:.      
-00000b10: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
-00000b20: 6d2e 7265 706c 795f 746f 5f6d 6573 7361  m.reply_to_messa
-00000b30: 6765 2e61 6e69 6d61 7469 6f6e 2e66 696c  ge.animation.fil
-00000b40: 655f 6964 0a20 2020 2020 2020 2020 2020  e_id.           
-00000b50: 2064 6174 615f 7479 7065 203d 2054 7970   data_type = Typ
-00000b60: 6573 2e41 4e49 4d41 5449 4f4e 0a0a 2020  es.ANIMATION..  
-00000b70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00000b80: 7265 7475 726e 204e 6f6e 652c 204e 6f6e  return None, Non
-00000b90: 652c 204e 6f6e 652c 204e 6f6e 650a 0a20  e, None, None.. 
-00000ba0: 2020 2072 6574 7572 6e20 6e6f 7465 5f6e     return note_n
-00000bb0: 616d 652c 2074 6578 742c 2064 6174 615f  ame, text, data_
-00000bc0: 7479 7065 2c20 636f 6e74 656e 740a 0a0a  type, content...
-00000bd0: 6173 796e 6320 6465 6620 6765 745f 6669  async def get_fi
-00000be0: 6c74 6572 5f74 7970 6528 6d3a 204d 6573  lter_type(m: Mes
-00000bf0: 7361 6765 293a 0a20 2020 2022 2222 4765  sage):.    """Ge
-00000c00: 7420 6669 6c74 6572 2074 7970 652e 2222  t filter type.""
-00000c10: 220a 2020 2020 6966 206c 656e 286d 2e74  ".    if len(m.t
-00000c20: 6578 742e 7370 6c69 7428 2929 203c 3d20  ext.split()) <= 
-00000c30: 313a 0a20 2020 2020 2020 2072 6574 7572  1:.        retur
-00000c40: 6e20 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  n None, None, No
-00000c50: 6e65 2c20 4e6f 6e65 0a0a 2020 2020 6461  ne, None..    da
-00000c60: 7461 5f74 7970 6520 3d20 4e6f 6e65 0a20  ta_type = None. 
-00000c70: 2020 2063 6f6e 7465 6e74 203d 204e 6f6e     content = Non
-00000c80: 650a 2020 2020 7261 775f 7465 7874 203d  e.    raw_text =
-00000c90: 206d 2e74 6578 742e 6d61 726b 646f 776e   m.text.markdown
-00000ca0: 2069 6620 6d2e 7465 7874 2065 6c73 6520   if m.text else 
-00000cb0: 6d2e 6361 7074 696f 6e2e 6d61 726b 646f  m.caption.markdo
-00000cc0: 776e 0a20 2020 2061 7267 7320 3d20 7261  wn.    args = ra
-00000cd0: 775f 7465 7874 2e73 706c 6974 284e 6f6e  w_text.split(Non
-00000ce0: 652c 2032 290a 0a20 2020 2069 6620 6e6f  e, 2)..    if no
-00000cf0: 7420 6d2e 7265 706c 795f 746f 5f6d 6573  t m.reply_to_mes
-00000d00: 7361 6765 2061 6e64 206d 2e74 6578 7420  sage and m.text 
-00000d10: 616e 6420 6c65 6e28 6d2e 7465 7874 2e73  and len(m.text.s
-00000d20: 706c 6974 2829 2920 3e3d 2033 3a0a 2020  plit()) >= 3:.  
-00000d30: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
-00000d40: 4e6f 6e65 0a20 2020 2020 2020 2074 6578  None.        tex
-00000d50: 7420 3d20 6d2e 7465 7874 2e73 706c 6974  t = m.text.split
-00000d60: 284e 6f6e 652c 2032 295b 325d 0a20 2020  (None, 2)[2].   
-00000d70: 2020 2020 2064 6174 615f 7479 7065 203d       data_type =
-00000d80: 2054 7970 6573 2e54 4558 540a 0a20 2020   Types.TEXT..   
-00000d90: 2065 6c69 6620 6d2e 7265 706c 795f 746f   elif m.reply_to
-00000da0: 5f6d 6573 7361 6765 3a0a 2020 2020 2020  _message:.      
-00000db0: 2020 6966 206d 2e72 6570 6c79 5f74 6f5f    if m.reply_to_
-00000dc0: 6d65 7373 6167 652e 7465 7874 3a0a 2020  message.text:.  
-00000dd0: 2020 2020 2020 2020 2020 7465 7874 203d            text =
-00000de0: 206d 2e72 6570 6c79 5f74 6f5f 6d65 7373   m.reply_to_mess
-00000df0: 6167 652e 7465 7874 2e6d 6172 6b64 6f77  age.text.markdow
-00000e00: 6e0a 2020 2020 2020 2020 656c 6966 206d  n.        elif m
-00000e10: 2e72 6570 6c79 5f74 6f5f 6d65 7373 6167  .reply_to_messag
-00000e20: 652e 6361 7074 696f 6e3a 0a20 2020 2020  e.caption:.     
-00000e30: 2020 2020 2020 2074 6578 7420 3d20 6d2e         text = m.
-00000e40: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-00000e50: 2e63 6170 7469 6f6e 2e6d 6172 6b64 6f77  .caption.markdow
-00000e60: 6e0a 2020 2020 2020 2020 656c 7365 3a0a  n.        else:.
-00000e70: 2020 2020 2020 2020 2020 2020 7465 7874              text
-00000e80: 203d 2022 220a 0a20 2020 2020 2020 2069   = ""..        i
-00000e90: 6620 6c65 6e28 6172 6773 2920 3e3d 2032  f len(args) >= 2
-00000ea0: 2061 6e64 206d 2e72 6570 6c79 5f74 6f5f   and m.reply_to_
-00000eb0: 6d65 7373 6167 652e 7465 7874 3a20 2023  message.text:  #
-00000ec0: 206e 6f74 2063 6170 7469 6f6e 2c20 7465   not caption, te
-00000ed0: 7874 0a20 2020 2020 2020 2020 2020 2064  xt.            d
-00000ee0: 6174 615f 7479 7065 203d 2054 7970 6573  ata_type = Types
-00000ef0: 2e54 4558 540a 0a20 2020 2020 2020 2065  .TEXT..        e
-00000f00: 6c69 6620 6d2e 7265 706c 795f 746f 5f6d  lif m.reply_to_m
-00000f10: 6573 7361 6765 2e73 7469 636b 6572 3a0a  essage.sticker:.
-00000f20: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00000f30: 656e 7420 3d20 6d2e 7265 706c 795f 746f  ent = m.reply_to
-00000f40: 5f6d 6573 7361 6765 2e73 7469 636b 6572  _message.sticker
-00000f50: 2e66 696c 655f 6964 0a20 2020 2020 2020  .file_id.       
-00000f60: 2020 2020 2064 6174 615f 7479 7065 203d       data_type =
-00000f70: 2054 7970 6573 2e53 5449 434b 4552 0a0a   Types.STICKER..
-00000f80: 2020 2020 2020 2020 656c 6966 206d 2e72          elif m.r
-00000f90: 6570 6c79 5f74 6f5f 6d65 7373 6167 652e  eply_to_message.
-00000fa0: 646f 6375 6d65 6e74 3a0a 2020 2020 2020  document:.      
-00000fb0: 2020 2020 2020 6966 206d 2e72 6570 6c79        if m.reply
-00000fc0: 5f74 6f5f 6d65 7373 6167 652e 646f 6375  _to_message.docu
-00000fd0: 6d65 6e74 2e6d 696d 655f 7479 7065 203d  ment.mime_type =
-00000fe0: 3d20 2261 7070 6c69 6361 7469 6f6e 2f78  = "application/x
-00000ff0: 2d62 6164 2d74 6773 7469 636b 6572 223a  -bad-tgsticker":
-00001000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001010: 2064 6174 615f 7479 7065 203d 2054 7970   data_type = Typ
-00001020: 6573 2e41 4e49 4d41 5445 445f 5354 4943  es.ANIMATED_STIC
-00001030: 4b45 520a 2020 2020 2020 2020 2020 2020  KER.            
-00001040: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00001050: 2020 2020 2020 6461 7461 5f74 7970 6520        data_type 
-00001060: 3d20 5479 7065 732e 444f 4355 4d45 4e54  = Types.DOCUMENT
-00001070: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00001080: 7465 6e74 203d 206d 2e72 6570 6c79 5f74  tent = m.reply_t
-00001090: 6f5f 6d65 7373 6167 652e 646f 6375 6d65  o_message.docume
-000010a0: 6e74 2e66 696c 655f 6964 0a0a 2020 2020  nt.file_id..    
-000010b0: 2020 2020 656c 6966 206d 2e72 6570 6c79      elif m.reply
-000010c0: 5f74 6f5f 6d65 7373 6167 652e 7068 6f74  _to_message.phot
-000010d0: 6f3a 0a20 2020 2020 2020 2020 2020 2063  o:.            c
-000010e0: 6f6e 7465 6e74 203d 206d 2e72 6570 6c79  ontent = m.reply
-000010f0: 5f74 6f5f 6d65 7373 6167 652e 7068 6f74  _to_message.phot
-00001100: 6f2e 6669 6c65 5f69 6420 2023 206c 6173  o.file_id  # las
-00001110: 7420 656c 656d 203d 2062 6573 7420 7175  t elem = best qu
-00001120: 616c 6974 790a 2020 2020 2020 2020 2020  ality.          
-00001130: 2020 6461 7461 5f74 7970 6520 3d20 5479    data_type = Ty
-00001140: 7065 732e 5048 4f54 4f0a 0a20 2020 2020  pes.PHOTO..     
-00001150: 2020 2065 6c69 6620 6d2e 7265 706c 795f     elif m.reply_
-00001160: 746f 5f6d 6573 7361 6765 2e61 7564 696f  to_message.audio
-00001170: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00001180: 6e74 656e 7420 3d20 6d2e 7265 706c 795f  ntent = m.reply_
-00001190: 746f 5f6d 6573 7361 6765 2e61 7564 696f  to_message.audio
-000011a0: 2e66 696c 655f 6964 0a20 2020 2020 2020  .file_id.       
-000011b0: 2020 2020 2064 6174 615f 7479 7065 203d       data_type =
-000011c0: 2054 7970 6573 2e41 5544 494f 0a0a 2020   Types.AUDIO..  
-000011d0: 2020 2020 2020 656c 6966 206d 2e72 6570        elif m.rep
-000011e0: 6c79 5f74 6f5f 6d65 7373 6167 652e 766f  ly_to_message.vo
-000011f0: 6963 653a 0a20 2020 2020 2020 2020 2020  ice:.           
-00001200: 2063 6f6e 7465 6e74 203d 206d 2e72 6570   content = m.rep
-00001210: 6c79 5f74 6f5f 6d65 7373 6167 652e 766f  ly_to_message.vo
-00001220: 6963 652e 6669 6c65 5f69 640a 2020 2020  ice.file_id.    
-00001230: 2020 2020 2020 2020 6461 7461 5f74 7970          data_typ
-00001240: 6520 3d20 5479 7065 732e 564f 4943 450a  e = Types.VOICE.
-00001250: 0a20 2020 2020 2020 2065 6c69 6620 6d2e  .        elif m.
-00001260: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-00001270: 2e76 6964 656f 3a0a 2020 2020 2020 2020  .video:.        
-00001280: 2020 2020 636f 6e74 656e 7420 3d20 6d2e      content = m.
-00001290: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-000012a0: 2e76 6964 656f 2e66 696c 655f 6964 0a20  .video.file_id. 
-000012b0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-000012c0: 7479 7065 203d 2054 7970 6573 2e56 4944  type = Types.VID
-000012d0: 454f 0a0a 2020 2020 2020 2020 656c 6966  EO..        elif
-000012e0: 206d 2e72 6570 6c79 5f74 6f5f 6d65 7373   m.reply_to_mess
-000012f0: 6167 652e 7669 6465 6f5f 6e6f 7465 3a0a  age.video_note:.
-00001300: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00001310: 656e 7420 3d20 6d2e 7265 706c 795f 746f  ent = m.reply_to
-00001320: 5f6d 6573 7361 6765 2e76 6964 656f 5f6e  _message.video_n
-00001330: 6f74 652e 6669 6c65 5f69 640a 2020 2020  ote.file_id.    
-00001340: 2020 2020 2020 2020 6461 7461 5f74 7970          data_typ
-00001350: 6520 3d20 5479 7065 732e 5649 4445 4f5f  e = Types.VIDEO_
-00001360: 4e4f 5445 0a0a 2020 2020 2020 2020 656c  NOTE..        el
-00001370: 6966 206d 2e72 6570 6c79 5f74 6f5f 6d65  if m.reply_to_me
-00001380: 7373 6167 652e 616e 696d 6174 696f 6e3a  ssage.animation:
-00001390: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-000013a0: 7465 6e74 203d 206d 2e72 6570 6c79 5f74  tent = m.reply_t
-000013b0: 6f5f 6d65 7373 6167 652e 616e 696d 6174  o_message.animat
-000013c0: 696f 6e2e 6669 6c65 5f69 640a 2020 2020  ion.file_id.    
-000013d0: 2020 2020 2020 2020 6461 7461 5f74 7970          data_typ
-000013e0: 6520 3d20 5479 7065 732e 414e 494d 4154  e = Types.ANIMAT
-000013f0: 494f 4e0a 0a20 2020 2065 6c73 653a 0a20  ION..    else:. 
-00001400: 2020 2020 2020 2074 6578 7420 3d20 4e6f         text = No
-00001410: 6e65 0a20 2020 2020 2020 2064 6174 615f  ne.        data_
-00001420: 7479 7065 203d 204e 6f6e 650a 2020 2020  type = None.    
-00001430: 2020 2020 636f 6e74 656e 7420 3d20 4e6f      content = No
-00001440: 6e65 0a0a 2020 2020 7265 7475 726e 2074  ne..    return t
-00001450: 6578 742c 2064 6174 615f 7479 7065 2c20  ext, data_type, 
-00001460: 636f 6e74 656e 740a 0a0a 6173 796e 6320  content...async 
-00001470: 6465 6620 6765 745f 776c 636d 5f74 7970  def get_wlcm_typ
-00001480: 6528 6d3a 204d 6573 7361 6765 293a 0a20  e(m: Message):. 
-00001490: 2020 2022 2222 4765 7420 776c 636d 2074     """Get wlcm t
-000014a0: 7970 652e 2222 220a 2020 2020 6461 7461  ype.""".    data
-000014b0: 5f74 7970 6520 3d20 4e6f 6e65 0a20 2020  _type = None.   
-000014c0: 2063 6f6e 7465 6e74 203d 204e 6f6e 650a   content = None.
-000014d0: 2020 2020 7261 775f 7465 7874 203d 206d      raw_text = m
-000014e0: 2e74 6578 742e 6d61 726b 646f 776e 2069  .text.markdown i
-000014f0: 6620 6d2e 7465 7874 2065 6c73 6520 6d2e  f m.text else m.
-00001500: 6361 7074 696f 6e2e 6d61 726b 646f 776e  caption.markdown
-00001510: 0a20 2020 2061 7267 7320 3d20 7261 775f  .    args = raw_
-00001520: 7465 7874 2e73 706c 6974 284e 6f6e 652c  text.split(None,
-00001530: 2031 290a 0a20 2020 2069 6620 6e6f 7420   1)..    if not 
-00001540: 6d2e 7265 706c 795f 746f 5f6d 6573 7361  m.reply_to_messa
-00001550: 6765 2061 6e64 206d 2e74 6578 7420 616e  ge and m.text an
-00001560: 6420 6c65 6e28 6d2e 7465 7874 2e73 706c  d len(m.text.spl
-00001570: 6974 2829 2920 3e3d 2032 3a0a 2020 2020  it()) >= 2:.    
-00001580: 2020 2020 636f 6e74 656e 7420 3d20 4e6f      content = No
-00001590: 6e65 0a20 2020 2020 2020 2074 6578 7420  ne.        text 
-000015a0: 3d20 6d2e 7465 7874 2e73 706c 6974 284e  = m.text.split(N
-000015b0: 6f6e 652c 2031 295b 315d 0a20 2020 2020  one, 1)[1].     
-000015c0: 2020 2064 6174 615f 7479 7065 203d 2054     data_type = T
-000015d0: 7970 6573 2e54 4558 540a 0a20 2020 2065  ypes.TEXT..    e
-000015e0: 6c69 6620 6d2e 7265 706c 795f 746f 5f6d  lif m.reply_to_m
-000015f0: 6573 7361 6765 3a0a 2020 2020 2020 2020  essage:.        
-00001600: 6966 206d 2e72 6570 6c79 5f74 6f5f 6d65  if m.reply_to_me
-00001610: 7373 6167 652e 7465 7874 3a0a 2020 2020  ssage.text:.    
-00001620: 2020 2020 2020 2020 7465 7874 203d 206d          text = m
-00001630: 2e72 6570 6c79 5f74 6f5f 6d65 7373 6167  .reply_to_messag
-00001640: 652e 7465 7874 2e6d 6172 6b64 6f77 6e0a  e.text.markdown.
-00001650: 2020 2020 2020 2020 656c 6966 206d 2e72          elif m.r
-00001660: 6570 6c79 5f74 6f5f 6d65 7373 6167 652e  eply_to_message.
-00001670: 6361 7074 696f 6e3a 0a20 2020 2020 2020  caption:.       
-00001680: 2020 2020 2074 6578 7420 3d20 6d2e 7265       text = m.re
-00001690: 706c 795f 746f 5f6d 6573 7361 6765 2e63  ply_to_message.c
-000016a0: 6170 7469 6f6e 2e6d 6172 6b64 6f77 6e0a  aption.markdown.
-000016b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000016c0: 2020 2020 2020 2020 2020 7465 7874 203d            text =
-000016d0: 2022 220a 0a20 2020 2020 2020 2069 6620   ""..        if 
-000016e0: 6c65 6e28 6172 6773 2920 3e3d 2031 2061  len(args) >= 1 a
-000016f0: 6e64 206d 2e72 6570 6c79 5f74 6f5f 6d65  nd m.reply_to_me
-00001700: 7373 6167 652e 7465 7874 3a20 2023 206e  ssage.text:  # n
-00001710: 6f74 2063 6170 7469 6f6e 2c20 7465 7874  ot caption, text
-00001720: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00001730: 615f 7479 7065 203d 2054 7970 6573 2e54  a_type = Types.T
-00001740: 4558 540a 0a20 2020 2020 2020 2065 6c69  EXT..        eli
-00001750: 6620 6d2e 7265 706c 795f 746f 5f6d 6573  f m.reply_to_mes
-00001760: 7361 6765 2e73 7469 636b 6572 3a0a 2020  sage.sticker:.  
-00001770: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
-00001780: 7420 3d20 6d2e 7265 706c 795f 746f 5f6d  t = m.reply_to_m
-00001790: 6573 7361 6765 2e73 7469 636b 6572 2e66  essage.sticker.f
-000017a0: 696c 655f 6964 0a20 2020 2020 2020 2020  ile_id.         
-000017b0: 2020 2064 6174 615f 7479 7065 203d 2054     data_type = T
-000017c0: 7970 6573 2e53 5449 434b 4552 0a0a 2020  ypes.STICKER..  
-000017d0: 2020 2020 2020 656c 6966 206d 2e72 6570        elif m.rep
-000017e0: 6c79 5f74 6f5f 6d65 7373 6167 652e 646f  ly_to_message.do
-000017f0: 6375 6d65 6e74 3a0a 2020 2020 2020 2020  cument:.        
-00001800: 2020 2020 6966 206d 2e72 6570 6c79 5f74      if m.reply_t
-00001810: 6f5f 6d65 7373 6167 652e 646f 6375 6d65  o_message.docume
-00001820: 6e74 2e6d 696d 655f 7479 7065 203d 3d20  nt.mime_type == 
-00001830: 2261 7070 6c69 6361 7469 6f6e 2f78 2d62  "application/x-b
-00001840: 6164 2d74 6773 7469 636b 6572 223a 0a20  ad-tgsticker":. 
-00001850: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00001860: 6174 615f 7479 7065 203d 2054 7970 6573  ata_type = Types
-00001870: 2e41 4e49 4d41 5445 445f 5354 4943 4b45  .ANIMATED_STICKE
-00001880: 520a 2020 2020 2020 2020 2020 2020 656c  R.            el
-00001890: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000018a0: 2020 2020 6461 7461 5f74 7970 6520 3d20      data_type = 
-000018b0: 5479 7065 732e 444f 4355 4d45 4e54 0a20  Types.DOCUMENT. 
-000018c0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-000018d0: 6e74 203d 206d 2e72 6570 6c79 5f74 6f5f  nt = m.reply_to_
-000018e0: 6d65 7373 6167 652e 646f 6375 6d65 6e74  message.document
-000018f0: 2e66 696c 655f 6964 0a0a 2020 2020 2020  .file_id..      
-00001900: 2020 656c 6966 206d 2e72 6570 6c79 5f74    elif m.reply_t
-00001910: 6f5f 6d65 7373 6167 652e 7068 6f74 6f3a  o_message.photo:
-00001920: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00001930: 7465 6e74 203d 206d 2e72 6570 6c79 5f74  tent = m.reply_t
-00001940: 6f5f 6d65 7373 6167 652e 7068 6f74 6f2e  o_message.photo.
-00001950: 6669 6c65 5f69 6420 2023 206c 6173 7420  file_id  # last 
-00001960: 656c 656d 203d 2062 6573 7420 7175 616c  elem = best qual
-00001970: 6974 790a 2020 2020 2020 2020 2020 2020  ity.            
-00001980: 6461 7461 5f74 7970 6520 3d20 5479 7065  data_type = Type
-00001990: 732e 5048 4f54 4f0a 0a20 2020 2020 2020  s.PHOTO..       
-000019a0: 2065 6c69 6620 6d2e 7265 706c 795f 746f   elif m.reply_to
-000019b0: 5f6d 6573 7361 6765 2e61 7564 696f 3a0a  _message.audio:.
-000019c0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-000019d0: 656e 7420 3d20 6d2e 7265 706c 795f 746f  ent = m.reply_to
-000019e0: 5f6d 6573 7361 6765 2e61 7564 696f 2e66  _message.audio.f
-000019f0: 696c 655f 6964 0a20 2020 2020 2020 2020  ile_id.         
-00001a00: 2020 2064 6174 615f 7479 7065 203d 2054     data_type = T
-00001a10: 7970 6573 2e41 5544 494f 0a0a 2020 2020  ypes.AUDIO..    
-00001a20: 2020 2020 656c 6966 206d 2e72 6570 6c79      elif m.reply
-00001a30: 5f74 6f5f 6d65 7373 6167 652e 766f 6963  _to_message.voic
-00001a40: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
-00001a50: 6f6e 7465 6e74 203d 206d 2e72 6570 6c79  ontent = m.reply
-00001a60: 5f74 6f5f 6d65 7373 6167 652e 766f 6963  _to_message.voic
-00001a70: 652e 6669 6c65 5f69 640a 2020 2020 2020  e.file_id.      
-00001a80: 2020 2020 2020 6461 7461 5f74 7970 6520        data_type 
-00001a90: 3d20 5479 7065 732e 564f 4943 450a 0a20  = Types.VOICE.. 
-00001aa0: 2020 2020 2020 2065 6c69 6620 6d2e 7265         elif m.re
-00001ab0: 706c 795f 746f 5f6d 6573 7361 6765 2e76  ply_to_message.v
-00001ac0: 6964 656f 3a0a 2020 2020 2020 2020 2020  ideo:.          
-00001ad0: 2020 636f 6e74 656e 7420 3d20 6d2e 7265    content = m.re
-00001ae0: 706c 795f 746f 5f6d 6573 7361 6765 2e76  ply_to_message.v
-00001af0: 6964 656f 2e66 696c 655f 6964 0a20 2020  ideo.file_id.   
-00001b00: 2020 2020 2020 2020 2064 6174 615f 7479           data_ty
-00001b10: 7065 203d 2054 7970 6573 2e56 4944 454f  pe = Types.VIDEO
-00001b20: 0a0a 2020 2020 2020 2020 656c 6966 206d  ..        elif m
-00001b30: 2e72 6570 6c79 5f74 6f5f 6d65 7373 6167  .reply_to_messag
-00001b40: 652e 7669 6465 6f5f 6e6f 7465 3a0a 2020  e.video_note:.  
-00001b50: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
-00001b60: 7420 3d20 6d2e 7265 706c 795f 746f 5f6d  t = m.reply_to_m
-00001b70: 6573 7361 6765 2e76 6964 656f 5f6e 6f74  essage.video_not
-00001b80: 652e 6669 6c65 5f69 640a 2020 2020 2020  e.file_id.      
-00001b90: 2020 2020 2020 6461 7461 5f74 7970 6520        data_type 
-00001ba0: 3d20 5479 7065 732e 5649 4445 4f5f 4e4f  = Types.VIDEO_NO
-00001bb0: 5445 0a0a 2020 2020 2020 2020 656c 6966  TE..        elif
-00001bc0: 206d 2e72 6570 6c79 5f74 6f5f 6d65 7373   m.reply_to_mess
-00001bd0: 6167 652e 616e 696d 6174 696f 6e3a 0a20  age.animation:. 
-00001be0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-00001bf0: 6e74 203d 206d 2e72 6570 6c79 5f74 6f5f  nt = m.reply_to_
-00001c00: 6d65 7373 6167 652e 616e 696d 6174 696f  message.animatio
-00001c10: 6e2e 6669 6c65 5f69 640a 2020 2020 2020  n.file_id.      
-00001c20: 2020 2020 2020 6461 7461 5f74 7970 6520        data_type 
-00001c30: 3d20 5479 7065 732e 414e 494d 4154 494f  = Types.ANIMATIO
-00001c40: 4e0a 0a20 2020 2065 6c73 653a 0a20 2020  N..    else:.   
-00001c50: 2020 2020 2074 6578 7420 3d20 4e6f 6e65       text = None
-00001c60: 0a20 2020 2020 2020 2064 6174 615f 7479  .        data_ty
-00001c70: 7065 203d 204e 6f6e 650a 2020 2020 2020  pe = None.      
-00001c80: 2020 636f 6e74 656e 7420 3d20 4e6f 6e65    content = None
-00001c90: 0a0a 2020 2020 7265 7475 726e 2074 6578  ..    return tex
-00001ca0: 742c 2064 6174 615f 7479 7065 2c20 636f  t, data_type, co
-00001cb0: 6e74 656e 740a                           ntent.
+00000130: 5420 3d20 3131 0a0a 0a61 7379 6e63 2064  T = 11...async d
+00000140: 6566 2073 656e 645f 636d 6428 633a 2043  ef send_cmd(c: C
+00000150: 6c69 656e 742c 206d 7367 7479 7065 3a20  lient, msgtype: 
+00000160: 696e 7429 3a0a 2020 2020 4745 545f 464f  int):.    GET_FO
+00000170: 524d 4154 203d 207b 0a20 2020 2020 2020  RMAT = {.       
+00000180: 2054 7970 6573 2e54 4558 542e 7661 6c75   Types.TEXT.valu
+00000190: 653a 2063 2e73 656e 645f 6d65 7373 6167  e: c.send_messag
+000001a0: 652c 0a20 2020 2020 2020 2054 7970 6573  e,.        Types
+000001b0: 2e44 4f43 554d 454e 542e 7661 6c75 653a  .DOCUMENT.value:
+000001c0: 2063 2e73 656e 645f 646f 6375 6d65 6e74   c.send_document
+000001d0: 2c0a 2020 2020 2020 2020 5479 7065 732e  ,.        Types.
+000001e0: 5048 4f54 4f2e 7661 6c75 653a 2063 2e73  PHOTO.value: c.s
+000001f0: 656e 645f 7068 6f74 6f2c 0a20 2020 2020  end_photo,.     
+00000200: 2020 2054 7970 6573 2e56 4944 454f 2e76     Types.VIDEO.v
+00000210: 616c 7565 3a20 632e 7365 6e64 5f76 6964  alue: c.send_vid
+00000220: 656f 2c0a 2020 2020 2020 2020 5479 7065  eo,.        Type
+00000230: 732e 5354 4943 4b45 522e 7661 6c75 653a  s.STICKER.value:
+00000240: 2063 2e73 656e 645f 7374 6963 6b65 722c   c.send_sticker,
+00000250: 0a20 2020 2020 2020 2054 7970 6573 2e41  .        Types.A
+00000260: 5544 494f 2e76 616c 7565 3a20 632e 7365  UDIO.value: c.se
+00000270: 6e64 5f61 7564 696f 2c0a 2020 2020 2020  nd_audio,.      
+00000280: 2020 5479 7065 732e 564f 4943 452e 7661    Types.VOICE.va
+00000290: 6c75 653a 2063 2e73 656e 645f 766f 6963  lue: c.send_voic
+000002a0: 652c 0a20 2020 2020 2020 2054 7970 6573  e,.        Types
+000002b0: 2e56 4944 454f 5f4e 4f54 452e 7661 6c75  .VIDEO_NOTE.valu
+000002c0: 653a 2063 2e73 656e 645f 7669 6465 6f5f  e: c.send_video_
+000002d0: 6e6f 7465 2c0a 2020 2020 2020 2020 5479  note,.        Ty
+000002e0: 7065 732e 414e 494d 4154 494f 4e2e 7661  pes.ANIMATION.va
+000002f0: 6c75 653a 2063 2e73 656e 645f 616e 696d  lue: c.send_anim
+00000300: 6174 696f 6e2c 0a20 2020 2020 2020 2054  ation,.        T
+00000310: 7970 6573 2e41 4e49 4d41 5445 445f 5354  ypes.ANIMATED_ST
+00000320: 4943 4b45 522e 7661 6c75 653a 2063 2e73  ICKER.value: c.s
+00000330: 656e 645f 7374 6963 6b65 722c 0a20 2020  end_sticker,.   
+00000340: 2020 2020 2054 7970 6573 2e43 4f4e 5441       Types.CONTA
+00000350: 4354 3a20 632e 7365 6e64 5f63 6f6e 7461  CT: c.send_conta
+00000360: 6374 2c0a 2020 2020 7d0a 2020 2020 7265  ct,.    }.    re
+00000370: 7475 726e 2047 4554 5f46 4f52 4d41 545b  turn GET_FORMAT[
+00000380: 6d73 6774 7970 655d 0a0a 0a61 7379 6e63  msgtype]...async
+00000390: 2064 6566 2067 6574 5f6e 6f74 655f 7479   def get_note_ty
+000003a0: 7065 286d 3a20 4d65 7373 6167 6529 3a0a  pe(m: Message):.
+000003b0: 2020 2020 2222 2247 6574 2074 7970 6520      """Get type 
+000003c0: 6f66 206e 6f74 652e 2222 220a 2020 2020  of note.""".    
+000003d0: 6966 206c 656e 286d 2e74 6578 742e 7370  if len(m.text.sp
+000003e0: 6c69 7428 2929 203c 3d20 313a 0a20 2020  lit()) <= 1:.   
+000003f0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00000400: 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  , None, None, No
+00000410: 6e65 0a0a 2020 2020 6461 7461 5f74 7970  ne..    data_typ
+00000420: 6520 3d20 4e6f 6e65 0a20 2020 2063 6f6e  e = None.    con
+00000430: 7465 6e74 203d 204e 6f6e 650a 2020 2020  tent = None.    
+00000440: 7261 775f 7465 7874 203d 206d 2e74 6578  raw_text = m.tex
+00000450: 742e 6d61 726b 646f 776e 2069 6620 6d2e  t.markdown if m.
+00000460: 7465 7874 2065 6c73 6520 6d2e 6361 7074  text else m.capt
+00000470: 696f 6e2e 6d61 726b 646f 776e 0a20 2020  ion.markdown.   
+00000480: 2061 7267 7320 3d20 7261 775f 7465 7874   args = raw_text
+00000490: 2e73 706c 6974 284e 6f6e 652c 2032 290a  .split(None, 2).
+000004a0: 2020 2020 6e6f 7465 5f6e 616d 6520 3d20      note_name = 
+000004b0: 6172 6773 5b31 5d0a 0a20 2020 2069 6620  args[1]..    if 
+000004c0: 6c65 6e28 6172 6773 2920 3e3d 2033 3a0a  len(args) >= 3:.
+000004d0: 2020 2020 2020 2020 7465 7874 203d 2061          text = a
+000004e0: 7267 735b 325d 0a20 2020 2020 2020 2064  rgs[2].        d
+000004f0: 6174 615f 7479 7065 203d 2054 7970 6573  ata_type = Types
+00000500: 2e54 4558 540a 0a20 2020 2065 6c69 6620  .TEXT..    elif 
+00000510: 6d2e 7265 706c 795f 746f 5f6d 6573 7361  m.reply_to_messa
+00000520: 6765 3a0a 2020 2020 2020 2020 6966 206d  ge:.        if m
+00000530: 2e72 6570 6c79 5f74 6f5f 6d65 7373 6167  .reply_to_messag
+00000540: 652e 7465 7874 3a0a 2020 2020 2020 2020  e.text:.        
+00000550: 2020 2020 7465 7874 203d 206d 2e72 6570      text = m.rep
+00000560: 6c79 5f74 6f5f 6d65 7373 6167 652e 7465  ly_to_message.te
+00000570: 7874 2e6d 6172 6b64 6f77 6e0a 2020 2020  xt.markdown.    
+00000580: 2020 2020 656c 6966 206d 2e72 6570 6c79      elif m.reply
+00000590: 5f74 6f5f 6d65 7373 6167 652e 6361 7074  _to_message.capt
+000005a0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+000005b0: 2074 6578 7420 3d20 6d2e 7265 706c 795f   text = m.reply_
+000005c0: 746f 5f6d 6573 7361 6765 2e63 6170 7469  to_message.capti
+000005d0: 6f6e 2e6d 6172 6b64 6f77 6e0a 2020 2020  on.markdown.    
+000005e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000005f0: 2020 2020 2020 7465 7874 203d 2022 220a        text = "".
+00000600: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00000610: 6172 6773 2920 3e3d 2032 2061 6e64 206d  args) >= 2 and m
+00000620: 2e72 6570 6c79 5f74 6f5f 6d65 7373 6167  .reply_to_messag
+00000630: 652e 7465 7874 3a20 2023 206e 6f74 2063  e.text:  # not c
+00000640: 6170 7469 6f6e 2c20 7465 7874 0a20 2020  aption, text.   
+00000650: 2020 2020 2020 2020 2064 6174 615f 7479           data_ty
+00000660: 7065 203d 2054 7970 6573 2e54 4558 540a  pe = Types.TEXT.
+00000670: 0a20 2020 2020 2020 2065 6c69 6620 6d2e  .        elif m.
+00000680: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00000690: 2e73 7469 636b 6572 3a0a 2020 2020 2020  .sticker:.      
+000006a0: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
+000006b0: 6d2e 7265 706c 795f 746f 5f6d 6573 7361  m.reply_to_messa
+000006c0: 6765 2e73 7469 636b 6572 2e66 696c 655f  ge.sticker.file_
+000006d0: 6964 0a20 2020 2020 2020 2020 2020 2064  id.            d
+000006e0: 6174 615f 7479 7065 203d 2054 7970 6573  ata_type = Types
+000006f0: 2e53 5449 434b 4552 0a0a 2020 2020 2020  .STICKER..      
+00000700: 2020 656c 6966 206d 2e72 6570 6c79 5f74    elif m.reply_t
+00000710: 6f5f 6d65 7373 6167 652e 646f 6375 6d65  o_message.docume
+00000720: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
+00000730: 6966 206d 2e72 6570 6c79 5f74 6f5f 6d65  if m.reply_to_me
+00000740: 7373 6167 652e 646f 6375 6d65 6e74 2e6d  ssage.document.m
+00000750: 696d 655f 7479 7065 203d 3d20 2261 7070  ime_type == "app
+00000760: 6c69 6361 7469 6f6e 2f78 2d62 6164 2d74  lication/x-bad-t
+00000770: 6773 7469 636b 6572 223a 0a20 2020 2020  gsticker":.     
+00000780: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+00000790: 7479 7065 203d 2054 7970 6573 2e41 4e49  type = Types.ANI
+000007a0: 4d41 5445 445f 5354 4943 4b45 520a 2020  MATED_STICKER.  
+000007b0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007d0: 6461 7461 5f74 7970 6520 3d20 5479 7065  data_type = Type
+000007e0: 732e 444f 4355 4d45 4e54 0a20 2020 2020  s.DOCUMENT.     
+000007f0: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
+00000800: 206d 2e72 6570 6c79 5f74 6f5f 6d65 7373   m.reply_to_mess
+00000810: 6167 652e 646f 6375 6d65 6e74 2e66 696c  age.document.fil
+00000820: 655f 6964 0a0a 2020 2020 2020 2020 656c  e_id..        el
+00000830: 6966 206d 2e72 6570 6c79 5f74 6f5f 6d65  if m.reply_to_me
+00000840: 7373 6167 652e 7068 6f74 6f3a 0a20 2020  ssage.photo:.   
+00000850: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
+00000860: 203d 206d 2e72 6570 6c79 5f74 6f5f 6d65   = m.reply_to_me
+00000870: 7373 6167 652e 7068 6f74 6f2e 6669 6c65  ssage.photo.file
+00000880: 5f69 6420 2023 206c 6173 7420 656c 656d  _id  # last elem
+00000890: 203d 2062 6573 7420 7175 616c 6974 790a   = best quality.
+000008a0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+000008b0: 5f74 7970 6520 3d20 5479 7065 732e 5048  _type = Types.PH
+000008c0: 4f54 4f0a 0a20 2020 2020 2020 2065 6c69  OTO..        eli
+000008d0: 6620 6d2e 7265 706c 795f 746f 5f6d 6573  f m.reply_to_mes
+000008e0: 7361 6765 2e61 7564 696f 3a0a 2020 2020  sage.audio:.    
+000008f0: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
+00000900: 3d20 6d2e 7265 706c 795f 746f 5f6d 6573  = m.reply_to_mes
+00000910: 7361 6765 2e61 7564 696f 2e66 696c 655f  sage.audio.file_
+00000920: 6964 0a20 2020 2020 2020 2020 2020 2064  id.            d
+00000930: 6174 615f 7479 7065 203d 2054 7970 6573  ata_type = Types
+00000940: 2e41 5544 494f 0a0a 2020 2020 2020 2020  .AUDIO..        
+00000950: 656c 6966 206d 2e72 6570 6c79 5f74 6f5f  elif m.reply_to_
+00000960: 6d65 7373 6167 652e 766f 6963 653a 0a20  message.voice:. 
+00000970: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00000980: 6e74 203d 206d 2e72 6570 6c79 5f74 6f5f  nt = m.reply_to_
+00000990: 6d65 7373 6167 652e 766f 6963 652e 6669  message.voice.fi
+000009a0: 6c65 5f69 640a 2020 2020 2020 2020 2020  le_id.          
+000009b0: 2020 6461 7461 5f74 7970 6520 3d20 5479    data_type = Ty
+000009c0: 7065 732e 564f 4943 450a 0a20 2020 2020  pes.VOICE..     
+000009d0: 2020 2065 6c69 6620 6d2e 7265 706c 795f     elif m.reply_
+000009e0: 746f 5f6d 6573 7361 6765 2e76 6964 656f  to_message.video
+000009f0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+00000a00: 6e74 656e 7420 3d20 6d2e 7265 706c 795f  ntent = m.reply_
+00000a10: 746f 5f6d 6573 7361 6765 2e76 6964 656f  to_message.video
+00000a20: 2e66 696c 655f 6964 0a20 2020 2020 2020  .file_id.       
+00000a30: 2020 2020 2064 6174 615f 7479 7065 203d       data_type =
+00000a40: 2054 7970 6573 2e56 4944 454f 0a0a 2020   Types.VIDEO..  
+00000a50: 2020 2020 2020 656c 6966 206d 2e72 6570        elif m.rep
+00000a60: 6c79 5f74 6f5f 6d65 7373 6167 652e 7669  ly_to_message.vi
+00000a70: 6465 6f5f 6e6f 7465 3a0a 2020 2020 2020  deo_note:.      
+00000a80: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
+00000a90: 6d2e 7265 706c 795f 746f 5f6d 6573 7361  m.reply_to_messa
+00000aa0: 6765 2e76 6964 656f 5f6e 6f74 652e 6669  ge.video_note.fi
+00000ab0: 6c65 5f69 640a 2020 2020 2020 2020 2020  le_id.          
+00000ac0: 2020 6461 7461 5f74 7970 6520 3d20 5479    data_type = Ty
+00000ad0: 7065 732e 5649 4445 4f5f 4e4f 5445 0a0a  pes.VIDEO_NOTE..
+00000ae0: 2020 2020 2020 2020 656c 6966 206d 2e72          elif m.r
+00000af0: 6570 6c79 5f74 6f5f 6d65 7373 6167 652e  eply_to_message.
+00000b00: 616e 696d 6174 696f 6e3a 0a20 2020 2020  animation:.     
+00000b10: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
+00000b20: 206d 2e72 6570 6c79 5f74 6f5f 6d65 7373   m.reply_to_mess
+00000b30: 6167 652e 616e 696d 6174 696f 6e2e 6669  age.animation.fi
+00000b40: 6c65 5f69 640a 2020 2020 2020 2020 2020  le_id.          
+00000b50: 2020 6461 7461 5f74 7970 6520 3d20 5479    data_type = Ty
+00000b60: 7065 732e 414e 494d 4154 494f 4e0a 0a20  pes.ANIMATION.. 
+00000b70: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00000b80: 2072 6574 7572 6e20 4e6f 6e65 2c20 4e6f   return None, No
+00000b90: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 0a0a  ne, None, None..
+00000ba0: 2020 2020 7265 7475 726e 206e 6f74 655f      return note_
+00000bb0: 6e61 6d65 2c20 7465 7874 2c20 6461 7461  name, text, data
+00000bc0: 5f74 7970 652c 2063 6f6e 7465 6e74 0a0a  _type, content..
+00000bd0: 0a61 7379 6e63 2064 6566 2067 6574 5f66  .async def get_f
+00000be0: 696c 7465 725f 7479 7065 286d 3a20 4d65  ilter_type(m: Me
+00000bf0: 7373 6167 6529 3a0a 2020 2020 2222 2247  ssage):.    """G
+00000c00: 6574 2066 696c 7465 7220 7479 7065 2e22  et filter type."
+00000c10: 2222 0a20 2020 2069 6620 6c65 6e28 6d2e  "".    if len(m.
+00000c20: 7465 7874 2e73 706c 6974 2829 2920 3c3d  text.split()) <=
+00000c30: 2031 3a0a 2020 2020 2020 2020 7265 7475   1:.        retu
+00000c40: 726e 204e 6f6e 652c 204e 6f6e 652c 204e  rn None, None, N
+00000c50: 6f6e 652c 204e 6f6e 650a 0a20 2020 2064  one, None..    d
+00000c60: 6174 615f 7479 7065 203d 204e 6f6e 650a  ata_type = None.
+00000c70: 2020 2020 636f 6e74 656e 7420 3d20 4e6f      content = No
+00000c80: 6e65 0a20 2020 2072 6177 5f74 6578 7420  ne.    raw_text 
+00000c90: 3d20 6d2e 7465 7874 2e6d 6172 6b64 6f77  = m.text.markdow
+00000ca0: 6e20 6966 206d 2e74 6578 7420 656c 7365  n if m.text else
+00000cb0: 206d 2e63 6170 7469 6f6e 2e6d 6172 6b64   m.caption.markd
+00000cc0: 6f77 6e0a 2020 2020 6172 6773 203d 2072  own.    args = r
+00000cd0: 6177 5f74 6578 742e 7370 6c69 7428 4e6f  aw_text.split(No
+00000ce0: 6e65 2c20 3229 0a0a 2020 2020 6966 206e  ne, 2)..    if n
+00000cf0: 6f74 206d 2e72 6570 6c79 5f74 6f5f 6d65  ot m.reply_to_me
+00000d00: 7373 6167 6520 616e 6420 6d2e 7465 7874  ssage and m.text
+00000d10: 2061 6e64 206c 656e 286d 2e74 6578 742e   and len(m.text.
+00000d20: 7370 6c69 7428 2929 203e 3d20 333a 0a20  split()) >= 3:. 
+00000d30: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
+00000d40: 204e 6f6e 650a 2020 2020 2020 2020 7465   None.        te
+00000d50: 7874 203d 206d 2e74 6578 742e 7370 6c69  xt = m.text.spli
+00000d60: 7428 4e6f 6e65 2c20 3229 5b32 5d0a 2020  t(None, 2)[2].  
+00000d70: 2020 2020 2020 6461 7461 5f74 7970 6520        data_type 
+00000d80: 3d20 5479 7065 732e 5445 5854 0a0a 2020  = Types.TEXT..  
+00000d90: 2020 656c 6966 206d 2e72 6570 6c79 5f74    elif m.reply_t
+00000da0: 6f5f 6d65 7373 6167 653a 0a20 2020 2020  o_message:.     
+00000db0: 2020 2069 6620 6d2e 7265 706c 795f 746f     if m.reply_to
+00000dc0: 5f6d 6573 7361 6765 2e74 6578 743a 0a20  _message.text:. 
+00000dd0: 2020 2020 2020 2020 2020 2074 6578 7420             text 
+00000de0: 3d20 6d2e 7265 706c 795f 746f 5f6d 6573  = m.reply_to_mes
+00000df0: 7361 6765 2e74 6578 742e 6d61 726b 646f  sage.text.markdo
+00000e00: 776e 0a20 2020 2020 2020 2065 6c69 6620  wn.        elif 
+00000e10: 6d2e 7265 706c 795f 746f 5f6d 6573 7361  m.reply_to_messa
+00000e20: 6765 2e63 6170 7469 6f6e 3a0a 2020 2020  ge.caption:.    
+00000e30: 2020 2020 2020 2020 7465 7874 203d 206d          text = m
+00000e40: 2e72 6570 6c79 5f74 6f5f 6d65 7373 6167  .reply_to_messag
+00000e50: 652e 6361 7074 696f 6e2e 6d61 726b 646f  e.caption.markdo
+00000e60: 776e 0a20 2020 2020 2020 2065 6c73 653a  wn.        else:
+00000e70: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
+00000e80: 7420 3d20 2222 0a0a 2020 2020 2020 2020  t = ""..        
+00000e90: 6966 206c 656e 2861 7267 7329 203e 3d20  if len(args) >= 
+00000ea0: 3220 616e 6420 6d2e 7265 706c 795f 746f  2 and m.reply_to
+00000eb0: 5f6d 6573 7361 6765 2e74 6578 743a 2020  _message.text:  
+00000ec0: 2320 6e6f 7420 6361 7074 696f 6e2c 2074  # not caption, t
+00000ed0: 6578 740a 2020 2020 2020 2020 2020 2020  ext.            
+00000ee0: 6461 7461 5f74 7970 6520 3d20 5479 7065  data_type = Type
+00000ef0: 732e 5445 5854 0a0a 2020 2020 2020 2020  s.TEXT..        
+00000f00: 656c 6966 206d 2e72 6570 6c79 5f74 6f5f  elif m.reply_to_
+00000f10: 6d65 7373 6167 652e 7374 6963 6b65 723a  message.sticker:
+00000f20: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00000f30: 7465 6e74 203d 206d 2e72 6570 6c79 5f74  tent = m.reply_t
+00000f40: 6f5f 6d65 7373 6167 652e 7374 6963 6b65  o_message.sticke
+00000f50: 722e 6669 6c65 5f69 640a 2020 2020 2020  r.file_id.      
+00000f60: 2020 2020 2020 6461 7461 5f74 7970 6520        data_type 
+00000f70: 3d20 5479 7065 732e 5354 4943 4b45 520a  = Types.STICKER.
+00000f80: 0a20 2020 2020 2020 2065 6c69 6620 6d2e  .        elif m.
+00000f90: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00000fa0: 2e64 6f63 756d 656e 743a 0a20 2020 2020  .document:.     
+00000fb0: 2020 2020 2020 2069 6620 6d2e 7265 706c         if m.repl
+00000fc0: 795f 746f 5f6d 6573 7361 6765 2e64 6f63  y_to_message.doc
+00000fd0: 756d 656e 742e 6d69 6d65 5f74 7970 6520  ument.mime_type 
+00000fe0: 3d3d 2022 6170 706c 6963 6174 696f 6e2f  == "application/
+00000ff0: 782d 6261 642d 7467 7374 6963 6b65 7222  x-bad-tgsticker"
+00001000: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001010: 2020 6461 7461 5f74 7970 6520 3d20 5479    data_type = Ty
+00001020: 7065 732e 414e 494d 4154 4544 5f53 5449  pes.ANIMATED_STI
+00001030: 434b 4552 0a20 2020 2020 2020 2020 2020  CKER.           
+00001040: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00001050: 2020 2020 2020 2064 6174 615f 7479 7065         data_type
+00001060: 203d 2054 7970 6573 2e44 4f43 554d 454e   = Types.DOCUMEN
+00001070: 540a 2020 2020 2020 2020 2020 2020 636f  T.            co
+00001080: 6e74 656e 7420 3d20 6d2e 7265 706c 795f  ntent = m.reply_
+00001090: 746f 5f6d 6573 7361 6765 2e64 6f63 756d  to_message.docum
+000010a0: 656e 742e 6669 6c65 5f69 640a 0a20 2020  ent.file_id..   
+000010b0: 2020 2020 2065 6c69 6620 6d2e 7265 706c       elif m.repl
+000010c0: 795f 746f 5f6d 6573 7361 6765 2e70 686f  y_to_message.pho
+000010d0: 746f 3a0a 2020 2020 2020 2020 2020 2020  to:.            
+000010e0: 636f 6e74 656e 7420 3d20 6d2e 7265 706c  content = m.repl
+000010f0: 795f 746f 5f6d 6573 7361 6765 2e70 686f  y_to_message.pho
+00001100: 746f 2e66 696c 655f 6964 2020 2320 6c61  to.file_id  # la
+00001110: 7374 2065 6c65 6d20 3d20 6265 7374 2071  st elem = best q
+00001120: 7561 6c69 7479 0a20 2020 2020 2020 2020  uality.         
+00001130: 2020 2064 6174 615f 7479 7065 203d 2054     data_type = T
+00001140: 7970 6573 2e50 484f 544f 0a0a 2020 2020  ypes.PHOTO..    
+00001150: 2020 2020 656c 6966 206d 2e72 6570 6c79      elif m.reply
+00001160: 5f74 6f5f 6d65 7373 6167 652e 6175 6469  _to_message.audi
+00001170: 6f3a 0a20 2020 2020 2020 2020 2020 2063  o:.            c
+00001180: 6f6e 7465 6e74 203d 206d 2e72 6570 6c79  ontent = m.reply
+00001190: 5f74 6f5f 6d65 7373 6167 652e 6175 6469  _to_message.audi
+000011a0: 6f2e 6669 6c65 5f69 640a 2020 2020 2020  o.file_id.      
+000011b0: 2020 2020 2020 6461 7461 5f74 7970 6520        data_type 
+000011c0: 3d20 5479 7065 732e 4155 4449 4f0a 0a20  = Types.AUDIO.. 
+000011d0: 2020 2020 2020 2065 6c69 6620 6d2e 7265         elif m.re
+000011e0: 706c 795f 746f 5f6d 6573 7361 6765 2e76  ply_to_message.v
+000011f0: 6f69 6365 3a0a 2020 2020 2020 2020 2020  oice:.          
+00001200: 2020 636f 6e74 656e 7420 3d20 6d2e 7265    content = m.re
+00001210: 706c 795f 746f 5f6d 6573 7361 6765 2e76  ply_to_message.v
+00001220: 6f69 6365 2e66 696c 655f 6964 0a20 2020  oice.file_id.   
+00001230: 2020 2020 2020 2020 2064 6174 615f 7479           data_ty
+00001240: 7065 203d 2054 7970 6573 2e56 4f49 4345  pe = Types.VOICE
+00001250: 0a0a 2020 2020 2020 2020 656c 6966 206d  ..        elif m
+00001260: 2e72 6570 6c79 5f74 6f5f 6d65 7373 6167  .reply_to_messag
+00001270: 652e 7669 6465 6f3a 0a20 2020 2020 2020  e.video:.       
+00001280: 2020 2020 2063 6f6e 7465 6e74 203d 206d       content = m
+00001290: 2e72 6570 6c79 5f74 6f5f 6d65 7373 6167  .reply_to_messag
+000012a0: 652e 7669 6465 6f2e 6669 6c65 5f69 640a  e.video.file_id.
+000012b0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+000012c0: 5f74 7970 6520 3d20 5479 7065 732e 5649  _type = Types.VI
+000012d0: 4445 4f0a 0a20 2020 2020 2020 2065 6c69  DEO..        eli
+000012e0: 6620 6d2e 7265 706c 795f 746f 5f6d 6573  f m.reply_to_mes
+000012f0: 7361 6765 2e76 6964 656f 5f6e 6f74 653a  sage.video_note:
+00001300: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00001310: 7465 6e74 203d 206d 2e72 6570 6c79 5f74  tent = m.reply_t
+00001320: 6f5f 6d65 7373 6167 652e 7669 6465 6f5f  o_message.video_
+00001330: 6e6f 7465 2e66 696c 655f 6964 0a20 2020  note.file_id.   
+00001340: 2020 2020 2020 2020 2064 6174 615f 7479           data_ty
+00001350: 7065 203d 2054 7970 6573 2e56 4944 454f  pe = Types.VIDEO
+00001360: 5f4e 4f54 450a 0a20 2020 2020 2020 2065  _NOTE..        e
+00001370: 6c69 6620 6d2e 7265 706c 795f 746f 5f6d  lif m.reply_to_m
+00001380: 6573 7361 6765 2e61 6e69 6d61 7469 6f6e  essage.animation
+00001390: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+000013a0: 6e74 656e 7420 3d20 6d2e 7265 706c 795f  ntent = m.reply_
+000013b0: 746f 5f6d 6573 7361 6765 2e61 6e69 6d61  to_message.anima
+000013c0: 7469 6f6e 2e66 696c 655f 6964 0a20 2020  tion.file_id.   
+000013d0: 2020 2020 2020 2020 2064 6174 615f 7479           data_ty
+000013e0: 7065 203d 2054 7970 6573 2e41 4e49 4d41  pe = Types.ANIMA
+000013f0: 5449 4f4e 0a0a 2020 2020 656c 7365 3a0a  TION..    else:.
+00001400: 2020 2020 2020 2020 7465 7874 203d 204e          text = N
+00001410: 6f6e 650a 2020 2020 2020 2020 6461 7461  one.        data
+00001420: 5f74 7970 6520 3d20 4e6f 6e65 0a20 2020  _type = None.   
+00001430: 2020 2020 2063 6f6e 7465 6e74 203d 204e       content = N
+00001440: 6f6e 650a 0a20 2020 2072 6574 7572 6e20  one..    return 
+00001450: 7465 7874 2c20 6461 7461 5f74 7970 652c  text, data_type,
+00001460: 2063 6f6e 7465 6e74 0a0a 0a61 7379 6e63   content...async
+00001470: 2064 6566 2067 6574 5f77 6c63 6d5f 7479   def get_wlcm_ty
+00001480: 7065 286d 3a20 4d65 7373 6167 6529 3a0a  pe(m: Message):.
+00001490: 2020 2020 2222 2247 6574 2077 6c63 6d20      """Get wlcm 
+000014a0: 7479 7065 2e22 2222 0a20 2020 2064 6174  type.""".    dat
+000014b0: 615f 7479 7065 203d 204e 6f6e 650a 2020  a_type = None.  
+000014c0: 2020 636f 6e74 656e 7420 3d20 4e6f 6e65    content = None
+000014d0: 0a20 2020 2072 6177 5f74 6578 7420 3d20  .    raw_text = 
+000014e0: 6d2e 7465 7874 2e6d 6172 6b64 6f77 6e20  m.text.markdown 
+000014f0: 6966 206d 2e74 6578 7420 656c 7365 206d  if m.text else m
+00001500: 2e63 6170 7469 6f6e 2e6d 6172 6b64 6f77  .caption.markdow
+00001510: 6e0a 2020 2020 6172 6773 203d 2072 6177  n.    args = raw
+00001520: 5f74 6578 742e 7370 6c69 7428 4e6f 6e65  _text.split(None
+00001530: 2c20 3129 0a0a 2020 2020 6966 206e 6f74  , 1)..    if not
+00001540: 206d 2e72 6570 6c79 5f74 6f5f 6d65 7373   m.reply_to_mess
+00001550: 6167 6520 616e 6420 6d2e 7465 7874 2061  age and m.text a
+00001560: 6e64 206c 656e 286d 2e74 6578 742e 7370  nd len(m.text.sp
+00001570: 6c69 7428 2929 203e 3d20 323a 0a20 2020  lit()) >= 2:.   
+00001580: 2020 2020 2063 6f6e 7465 6e74 203d 204e       content = N
+00001590: 6f6e 650a 2020 2020 2020 2020 7465 7874  one.        text
+000015a0: 203d 206d 2e74 6578 742e 7370 6c69 7428   = m.text.split(
+000015b0: 4e6f 6e65 2c20 3129 5b31 5d0a 2020 2020  None, 1)[1].    
+000015c0: 2020 2020 6461 7461 5f74 7970 6520 3d20      data_type = 
+000015d0: 5479 7065 732e 5445 5854 0a0a 2020 2020  Types.TEXT..    
+000015e0: 656c 6966 206d 2e72 6570 6c79 5f74 6f5f  elif m.reply_to_
+000015f0: 6d65 7373 6167 653a 0a20 2020 2020 2020  message:.       
+00001600: 2069 6620 6d2e 7265 706c 795f 746f 5f6d   if m.reply_to_m
+00001610: 6573 7361 6765 2e74 6578 743a 0a20 2020  essage.text:.   
+00001620: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
+00001630: 6d2e 7265 706c 795f 746f 5f6d 6573 7361  m.reply_to_messa
+00001640: 6765 2e74 6578 742e 6d61 726b 646f 776e  ge.text.markdown
+00001650: 0a20 2020 2020 2020 2065 6c69 6620 6d2e  .        elif m.
+00001660: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00001670: 2e63 6170 7469 6f6e 3a0a 2020 2020 2020  .caption:.      
+00001680: 2020 2020 2020 7465 7874 203d 206d 2e72        text = m.r
+00001690: 6570 6c79 5f74 6f5f 6d65 7373 6167 652e  eply_to_message.
+000016a0: 6361 7074 696f 6e2e 6d61 726b 646f 776e  caption.markdown
+000016b0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000016c0: 2020 2020 2020 2020 2020 2074 6578 7420             text 
+000016d0: 3d20 2222 0a0a 2020 2020 2020 2020 6966  = ""..        if
+000016e0: 206c 656e 2861 7267 7329 203e 3d20 3120   len(args) >= 1 
+000016f0: 616e 6420 6d2e 7265 706c 795f 746f 5f6d  and m.reply_to_m
+00001700: 6573 7361 6765 2e74 6578 743a 2020 2320  essage.text:  # 
+00001710: 6e6f 7420 6361 7074 696f 6e2c 2074 6578  not caption, tex
+00001720: 740a 2020 2020 2020 2020 2020 2020 6461  t.            da
+00001730: 7461 5f74 7970 6520 3d20 5479 7065 732e  ta_type = Types.
+00001740: 5445 5854 0a0a 2020 2020 2020 2020 656c  TEXT..        el
+00001750: 6966 206d 2e72 6570 6c79 5f74 6f5f 6d65  if m.reply_to_me
+00001760: 7373 6167 652e 7374 6963 6b65 723a 0a20  ssage.sticker:. 
+00001770: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00001780: 6e74 203d 206d 2e72 6570 6c79 5f74 6f5f  nt = m.reply_to_
+00001790: 6d65 7373 6167 652e 7374 6963 6b65 722e  message.sticker.
+000017a0: 6669 6c65 5f69 640a 2020 2020 2020 2020  file_id.        
+000017b0: 2020 2020 6461 7461 5f74 7970 6520 3d20      data_type = 
+000017c0: 5479 7065 732e 5354 4943 4b45 520a 0a20  Types.STICKER.. 
+000017d0: 2020 2020 2020 2065 6c69 6620 6d2e 7265         elif m.re
+000017e0: 706c 795f 746f 5f6d 6573 7361 6765 2e64  ply_to_message.d
+000017f0: 6f63 756d 656e 743a 0a20 2020 2020 2020  ocument:.       
+00001800: 2020 2020 2069 6620 6d2e 7265 706c 795f       if m.reply_
+00001810: 746f 5f6d 6573 7361 6765 2e64 6f63 756d  to_message.docum
+00001820: 656e 742e 6d69 6d65 5f74 7970 6520 3d3d  ent.mime_type ==
+00001830: 2022 6170 706c 6963 6174 696f 6e2f 782d   "application/x-
+00001840: 6261 642d 7467 7374 6963 6b65 7222 3a0a  bad-tgsticker":.
+00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001860: 6461 7461 5f74 7970 6520 3d20 5479 7065  data_type = Type
+00001870: 732e 414e 494d 4154 4544 5f53 5449 434b  s.ANIMATED_STICK
+00001880: 4552 0a20 2020 2020 2020 2020 2020 2065  ER.            e
+00001890: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000018a0: 2020 2020 2064 6174 615f 7479 7065 203d       data_type =
+000018b0: 2054 7970 6573 2e44 4f43 554d 454e 540a   Types.DOCUMENT.
+000018c0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+000018d0: 656e 7420 3d20 6d2e 7265 706c 795f 746f  ent = m.reply_to
+000018e0: 5f6d 6573 7361 6765 2e64 6f63 756d 656e  _message.documen
+000018f0: 742e 6669 6c65 5f69 640a 0a20 2020 2020  t.file_id..     
+00001900: 2020 2065 6c69 6620 6d2e 7265 706c 795f     elif m.reply_
+00001910: 746f 5f6d 6573 7361 6765 2e70 686f 746f  to_message.photo
+00001920: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+00001930: 6e74 656e 7420 3d20 6d2e 7265 706c 795f  ntent = m.reply_
+00001940: 746f 5f6d 6573 7361 6765 2e70 686f 746f  to_message.photo
+00001950: 2e66 696c 655f 6964 2020 2320 6c61 7374  .file_id  # last
+00001960: 2065 6c65 6d20 3d20 6265 7374 2071 7561   elem = best qua
+00001970: 6c69 7479 0a20 2020 2020 2020 2020 2020  lity.           
+00001980: 2064 6174 615f 7479 7065 203d 2054 7970   data_type = Typ
+00001990: 6573 2e50 484f 544f 0a0a 2020 2020 2020  es.PHOTO..      
+000019a0: 2020 656c 6966 206d 2e72 6570 6c79 5f74    elif m.reply_t
+000019b0: 6f5f 6d65 7373 6167 652e 6175 6469 6f3a  o_message.audio:
+000019c0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+000019d0: 7465 6e74 203d 206d 2e72 6570 6c79 5f74  tent = m.reply_t
+000019e0: 6f5f 6d65 7373 6167 652e 6175 6469 6f2e  o_message.audio.
+000019f0: 6669 6c65 5f69 640a 2020 2020 2020 2020  file_id.        
+00001a00: 2020 2020 6461 7461 5f74 7970 6520 3d20      data_type = 
+00001a10: 5479 7065 732e 4155 4449 4f0a 0a20 2020  Types.AUDIO..   
+00001a20: 2020 2020 2065 6c69 6620 6d2e 7265 706c       elif m.repl
+00001a30: 795f 746f 5f6d 6573 7361 6765 2e76 6f69  y_to_message.voi
+00001a40: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
+00001a50: 636f 6e74 656e 7420 3d20 6d2e 7265 706c  content = m.repl
+00001a60: 795f 746f 5f6d 6573 7361 6765 2e76 6f69  y_to_message.voi
+00001a70: 6365 2e66 696c 655f 6964 0a20 2020 2020  ce.file_id.     
+00001a80: 2020 2020 2020 2064 6174 615f 7479 7065         data_type
+00001a90: 203d 2054 7970 6573 2e56 4f49 4345 0a0a   = Types.VOICE..
+00001aa0: 2020 2020 2020 2020 656c 6966 206d 2e72          elif m.r
+00001ab0: 6570 6c79 5f74 6f5f 6d65 7373 6167 652e  eply_to_message.
+00001ac0: 7669 6465 6f3a 0a20 2020 2020 2020 2020  video:.         
+00001ad0: 2020 2063 6f6e 7465 6e74 203d 206d 2e72     content = m.r
+00001ae0: 6570 6c79 5f74 6f5f 6d65 7373 6167 652e  eply_to_message.
+00001af0: 7669 6465 6f2e 6669 6c65 5f69 640a 2020  video.file_id.  
+00001b00: 2020 2020 2020 2020 2020 6461 7461 5f74            data_t
+00001b10: 7970 6520 3d20 5479 7065 732e 5649 4445  ype = Types.VIDE
+00001b20: 4f0a 0a20 2020 2020 2020 2065 6c69 6620  O..        elif 
+00001b30: 6d2e 7265 706c 795f 746f 5f6d 6573 7361  m.reply_to_messa
+00001b40: 6765 2e76 6964 656f 5f6e 6f74 653a 0a20  ge.video_note:. 
+00001b50: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00001b60: 6e74 203d 206d 2e72 6570 6c79 5f74 6f5f  nt = m.reply_to_
+00001b70: 6d65 7373 6167 652e 7669 6465 6f5f 6e6f  message.video_no
+00001b80: 7465 2e66 696c 655f 6964 0a20 2020 2020  te.file_id.     
+00001b90: 2020 2020 2020 2064 6174 615f 7479 7065         data_type
+00001ba0: 203d 2054 7970 6573 2e56 4944 454f 5f4e   = Types.VIDEO_N
+00001bb0: 4f54 450a 0a20 2020 2020 2020 2065 6c69  OTE..        eli
+00001bc0: 6620 6d2e 7265 706c 795f 746f 5f6d 6573  f m.reply_to_mes
+00001bd0: 7361 6765 2e61 6e69 6d61 7469 6f6e 3a0a  sage.animation:.
+00001be0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00001bf0: 656e 7420 3d20 6d2e 7265 706c 795f 746f  ent = m.reply_to
+00001c00: 5f6d 6573 7361 6765 2e61 6e69 6d61 7469  _message.animati
+00001c10: 6f6e 2e66 696c 655f 6964 0a20 2020 2020  on.file_id.     
+00001c20: 2020 2020 2020 2064 6174 615f 7479 7065         data_type
+00001c30: 203d 2054 7970 6573 2e41 4e49 4d41 5449   = Types.ANIMATI
+00001c40: 4f4e 0a0a 2020 2020 656c 7365 3a0a 2020  ON..    else:.  
+00001c50: 2020 2020 2020 7465 7874 203d 204e 6f6e        text = Non
+00001c60: 650a 2020 2020 2020 2020 6461 7461 5f74  e.        data_t
+00001c70: 7970 6520 3d20 4e6f 6e65 0a20 2020 2020  ype = None.     
+00001c80: 2020 2063 6f6e 7465 6e74 203d 204e 6f6e     content = Non
+00001c90: 650a 0a20 2020 2072 6574 7572 6e20 7465  e..    return te
+00001ca0: 7874 2c20 6461 7461 5f74 7970 652c 2063  xt, data_type, c
+00001cb0: 6f6e 7465 6e74 0a                        ontent.
```

### Comparing `Abg-2.1/Abg/helpers/parser.py` & `Abg-2.2/Abg/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/helpers/pyro_progress.py` & `Abg-2.2/Abg/helpers/pyro_progress.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/helpers/ratelimit.py` & `Abg-2.2/Abg/helpers/ratelimit.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/helpers/string.py` & `Abg-2.2/Abg/helpers/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from html import escape
 from re import compile as compile_re
-from time import time
 from typing import List
 
-from Abg.helpers.parser import escape_markdown
 from pyrogram.enums import ChatType
 from pyrogram.types import InlineKeyboardButton, Message
 
+from Abg.helpers.parser import escape_markdown
+
 BTN_URL_REGEX = compile_re(r"(\[([^\[]+?)\]\(buttonurl:(?:/{0,2})(.+?)(:same)?\))")
 
+
 async def parse_button(text: str):
     """Parse button from text."""
     markdown_note = text
     prev = 0
     note_data = ""
     buttons = []
     for match in BTN_URL_REGEX.finditer(markdown_note):
@@ -120,14 +121,15 @@
             id=m.from_user.id,
         )
     else:
         teks = ""
 
     return teks
 
+
 def split_limits(text):
     if len(text) < 2048:
         return [text]
 
     lines = text.splitlines(True)
     small_msg = ""
     result = []
@@ -136,15 +138,16 @@
             small_msg += line
         else:
             result.append(small_msg)
             small_msg = line
 
     result.append(small_msg)
     return result
-    
+
+
 async def split_quotes(text: str):
     """Split quotes in text."""
     if not any(text.startswith(char) for char in START_CHAR):
         return text.split(None, 1)
     counter = 1  # ignore first char -> is some kind of quote
     while counter < len(text):
         if text[counter] == "\\":
```

### Comparing `Abg-2.1/Abg/inline/inline_keyboard.py` & `Abg-2.2/Abg/inline/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/inline/inline_pagination_keyboard.py` & `Abg-2.2/Abg/inline/inline_pagination_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/inline/reply_keyboard.py` & `Abg-2.2/Abg/inline/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/patch/bound/message.py` & `Abg-2.2/Abg/patch/bound/message.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/patch/listen/listen.py` & `Abg-2.2/Abg/patch/listen/listen.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/patch/listen/utils.py` & `Abg-2.2/Abg/patch/listen/utils.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/patch/methods/edit_message_text.py` & `Abg-2.2/Abg/patch/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/patch/methods/send_as_file.py` & `Abg-2.2/Abg/patch/methods/send_as_file.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg/patch/methods/send_message.py` & `Abg-2.2/Abg/patch/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `Abg-2.1/Abg.egg-info/PKG-INFO` & `Abg-2.2/Abg.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.1
-Summary: Telegram bot helpers
-Home-page: https://github.com/Abishnoi69
-Author: Abishnoi1M
+Version: 2.2
+Summary: Telegram bot helpers, A add-on for Pyrogram
+Home-page: https://github.com/Abishnoi69/Abg
+Author: Abishnoi 
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
-Project-URL: Community, https://t.me/Abgpy
+Project-URL: Community, https://telegram.me/AbgPy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
 Description: # ᴀʙɢ :->
         > 
         ### • Conversation
         
         ```python
         from pyrogram import filters, Client
         from pyrogram.types import Message
         from Abg import patch  # type : ignore
         
         app = Client("my_account")
         
-        @app.on_message(filters.command(["myinfo"]))
+        @app.on_cmd("myinfo")
         async def my_info(self: Client, ctx: Message):
             if not ctx.from_user:
                 return
             name = await ctx.chat.ask("Type Your Name")
             age = await ctx.chat.ask("Type your age")
             add = await ctx.chat.ask("Type your address")
             # you can also use : ctx.reply_text(...)
@@ -36,28 +36,25 @@
             )
         
           app.run()
         ```
         >
         ### • User Rights 
         
-        ```python 
-        from Abg.chat_status import adminsOnly, command
-        from pyrogram.enums import ChatType
+        ```python
+        from Abg import patch  # type : ignore
+        from Abg.chat_status import adminsOnly
         from pyrogram.types import Message
         from pyrogram import Client
         
         app = Client("my_account")
         
-        @app.on_message(command("del"))
+        @app.on_cmd("del"], group_only=True)
         @adminsOnly("can_delete_messages")
         async def del_msg(c: Client, m: Message):
-            if m.chat.type != ChatType.SUPERGROUP:
-                return
-        
             if m.reply_to_message:
                 await m.delete()
                 await c.delete_messages(
                     chat_id=m.chat.id,
                     message_ids=m.reply_to_message.id,
                 )
             else:
@@ -113,23 +110,23 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: ~=3.7
+Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
```

### Comparing `Abg-2.1/Abg.egg-info/SOURCES.txt` & `Abg-2.2/Abg.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 README.md
 setup.py
 Abg/__init__.py
 Abg.egg-info/PKG-INFO
 Abg.egg-info/SOURCES.txt
 Abg.egg-info/dependency_links.txt
+Abg.egg-info/not-zip-safe
+Abg.egg-info/requires.txt
 Abg.egg-info/top_level.txt
 Abg/chat_status/__init__.py
 Abg/chat_status/chat_status.py
 Abg/chat_status/custom_filters.py
 Abg/helpers/__init__.py
+Abg/helpers/get_user.py
 Abg/helpers/helpers.py
 Abg/helpers/http_helper.py
 Abg/helpers/human_read.py
 Abg/helpers/msg_types.py
 Abg/helpers/parser.py
 Abg/helpers/pyro_progress.py
 Abg/helpers/ratelimit.py
@@ -20,14 +23,17 @@
 Abg/inline/__init__.py
 Abg/inline/inline_keyboard.py
 Abg/inline/inline_pagination_keyboard.py
 Abg/inline/reply_keyboard.py
 Abg/patch/__init__.py
 Abg/patch/bound/__init__.py
 Abg/patch/bound/message.py
+Abg/patch/decorators/__init__.py
+Abg/patch/decorators/callback.py
+Abg/patch/decorators/command.py
 Abg/patch/listen/__init__.py
 Abg/patch/listen/listen.py
 Abg/patch/listen/utils.py
 Abg/patch/methods/__init__.py
 Abg/patch/methods/edit_message_text.py
 Abg/patch/methods/send_as_file.py
 Abg/patch/methods/send_message.py
```

### Comparing `Abg-2.1/PKG-INFO` & `Abg-2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.1
-Summary: Telegram bot helpers
-Home-page: https://github.com/Abishnoi69
-Author: Abishnoi1M
+Version: 2.2
+Summary: Telegram bot helpers, A add-on for Pyrogram
+Home-page: https://github.com/Abishnoi69/Abg
+Author: Abishnoi 
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
-Project-URL: Community, https://t.me/Abgpy
+Project-URL: Community, https://telegram.me/AbgPy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
 Description: # ᴀʙɢ :->
         > 
         ### • Conversation
         
         ```python
         from pyrogram import filters, Client
         from pyrogram.types import Message
         from Abg import patch  # type : ignore
         
         app = Client("my_account")
         
-        @app.on_message(filters.command(["myinfo"]))
+        @app.on_cmd("myinfo")
         async def my_info(self: Client, ctx: Message):
             if not ctx.from_user:
                 return
             name = await ctx.chat.ask("Type Your Name")
             age = await ctx.chat.ask("Type your age")
             add = await ctx.chat.ask("Type your address")
             # you can also use : ctx.reply_text(...)
@@ -36,28 +36,25 @@
             )
         
           app.run()
         ```
         >
         ### • User Rights 
         
-        ```python 
-        from Abg.chat_status import adminsOnly, command
-        from pyrogram.enums import ChatType
+        ```python
+        from Abg import patch  # type : ignore
+        from Abg.chat_status import adminsOnly
         from pyrogram.types import Message
         from pyrogram import Client
         
         app = Client("my_account")
         
-        @app.on_message(command("del"))
+        @app.on_cmd("del"], group_only=True)
         @adminsOnly("can_delete_messages")
         async def del_msg(c: Client, m: Message):
-            if m.chat.type != ChatType.SUPERGROUP:
-                return
-        
             if m.reply_to_message:
                 await m.delete()
                 await c.delete_messages(
                     chat_id=m.chat.id,
                     message_ids=m.reply_to_message.id,
                 )
             else:
@@ -113,23 +110,23 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: ~=3.7
+Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
```

### Comparing `Abg-2.1/README.md` & `Abg-2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ```python
 from pyrogram import filters, Client
 from pyrogram.types import Message
 from Abg import patch  # type : ignore
 
 app = Client("my_account")
 
-@app.on_message(filters.command(["myinfo"]))
+@app.on_cmd("myinfo")
 async def my_info(self: Client, ctx: Message):
     if not ctx.from_user:
         return
     name = await ctx.chat.ask("Type Your Name")
     age = await ctx.chat.ask("Type your age")
     add = await ctx.chat.ask("Type your address")
     # you can also use : ctx.reply_text(...)
@@ -23,28 +23,25 @@
     )
 
   app.run()
 ```
 >
 ### • User Rights 
 
-```python 
-from Abg.chat_status import adminsOnly, command
-from pyrogram.enums import ChatType
+```python
+from Abg import patch  # type : ignore
+from Abg.chat_status import adminsOnly
 from pyrogram.types import Message
 from pyrogram import Client
 
 app = Client("my_account")
 
-@app.on_message(command("del"))
+@app.on_cmd("del"], group_only=True)
 @adminsOnly("can_delete_messages")
 async def del_msg(c: Client, m: Message):
-    if m.chat.type != ChatType.SUPERGROUP:
-        return
-
     if m.reply_to_message:
         await m.delete()
         await c.delete_messages(
             chat_id=m.chat.id,
             message_ids=m.reply_to_message.id,
         )
     else:
```

### Comparing `Abg-2.1/setup.py` & `Abg-2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 #  Copyright (C) 2023-present Abishnoi6 <https://github.com/Abishnoi69>
 #
 #  This file is part of Abg.
 #
 #  Abg is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
@@ -14,62 +13,65 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Abg.  If not, see <http://www.gnu.org/licenses/>.
 
 # ===================================================================
 
-import setuptools
+import re
+
+from setuptools import find_packages, setup
+
+with open("Abg/__init__.py", encoding="utf-8") as f:
+    version = re.findall(r"__version__ = \"(.+)\"", f.read())[0]
 
-with open("README.md", encoding="utf8") as readme:
-    long_description = readme.read()
+with open("README.md", encoding="utf-8") as f:
+    readme = f.read()
 
-"""    
-def read(file: str) -> list:
-    with open(file, encoding="utf-8") as r:
-        return [i.strip() for i in r]
-"""
+with open("requirements.txt", encoding="utf-8") as f:
+    requires = f.read().splitlines()
 
-setuptools.setup(
+setup(
     name="Abg",
-    packages=setuptools.find_packages(),
-    version="2.1",
-    description="Telegram bot helpers",
-    long_description=long_description,
+    version=version,
+    description="Telegram bot helpers, A add-on for Pyrogram",
+    long_description=readme,
     long_description_content_type="text/markdown",
-    url="https://github.com/Abishnoi69",
+    url="https://github.com/Abishnoi69/Abg",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
-    author="Abishnoi1M",
+    author="Abishnoi ",
     author_email="Abishnoi69@Abg.org",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Internet",
         "Topic :: Communications",
         "Topic :: Communications :: Chat",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Software Development :: Libraries :: Application Frameworks",
     ],
     keywords="telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch botapi https",
     project_urls={
         "Tracker": "https://github.com/Abishnoi69/Abg/issues",
-        "Community": "https://t.me/Abgpy",
+        "Community": "https://telegram.me/AbgPy",
         "Source": "https://github.com/Abishnoi69/Abg",
         "Documentation": "https://github.com/Abishnoi69/Abg/tree/master/doce",
     },
-    python_requires="~=3.7",
-    # install_requires=read("requirements.txt")
+    python_requires="~=3.6",
+    packages=find_packages(),
+    zip_safe=False,
+    install_requires=requires,
 )
```

