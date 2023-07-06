# Comparing `tmp/dslclib-0.1.3.tar.gz` & `tmp/dslclib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dslclib-0.1.3.tar", max compression
+gzip compressed data, was "dslclib-0.2.0.tar", max compression
```

## Comparing `dslclib-0.1.3.tar` & `dslclib-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      702 2023-06-30 14:41:31.326866 dslclib-0.1.3/README.md
--rw-r--r--   0        0        0      334 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/__init__.py
--rw-r--r--   0        0        0      382 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/__init__.py
--rw-r--r--   0        0        0     3206 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/base.py
--rw-r--r--   0        0        0    11535 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/body_controller.py
--rw-r--r--   0        0        0     5700 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/expression_controller.py
--rw-r--r--   0        0        0     9049 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/face_recognition.py
--rw-r--r--   0        0        0     3652 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/speech_recognition.py
--rw-r--r--   0        0        0     4489 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/tts.py
--rw-r--r--   0        0        0      635 2023-06-30 14:42:02.515082 dslclib-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 dslclib-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1244 2023-07-06 12:12:13.644362 dslclib-0.2.0/README.md
+-rw-r--r--   0        0        0      376 2023-07-06 12:12:13.644362 dslclib-0.2.0/dslclib/__init__.py
+-rw-r--r--   0        0        0      433 2023-07-06 12:12:13.644362 dslclib-0.2.0/dslclib/src/__init__.py
+-rw-r--r--   0        0        0     3206 2023-07-06 12:12:13.644362 dslclib-0.2.0/dslclib/src/base.py
+-rw-r--r--   0        0        0    11759 2023-07-06 12:12:13.644362 dslclib-0.2.0/dslclib/src/body_controller.py
+-rw-r--r--   0        0        0     5915 2023-07-06 12:12:13.644362 dslclib-0.2.0/dslclib/src/expression_controller.py
+-rw-r--r--   0        0        0    12453 2023-07-06 12:12:13.644362 dslclib-0.2.0/dslclib/src/face_recognition.py
+-rw-r--r--   0        0        0     4336 2023-07-06 12:12:13.644362 dslclib-0.2.0/dslclib/src/speech_recognition.py
+-rw-r--r--   0        0        0     4489 2023-07-06 12:12:13.644362 dslclib-0.2.0/dslclib/src/tts.py
+-rw-r--r--   0        0        0      680 2023-07-06 12:12:38.740375 dslclib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 dslclib-0.2.0/PKG-INFO
```

### Comparing `dslclib-0.1.3/dslclib/src/base.py` & `dslclib-0.2.0/dslclib/src/base.py`

 * *Files identical despite different names*

### Comparing `dslclib-0.1.3/dslclib/src/body_controller.py` & `dslclib-0.2.0/dslclib/src/body_controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from dataclasses import dataclass
-from typing import Optional
+from typing import Literal, Optional
 
 from dslclib.src.base import BaseClient
 
 
 @dataclass
 class MotionType:
     """MotinonType
@@ -22,21 +22,21 @@
     DefaultMotion
     >>> MotionType.Nod
     nod
     >>> MotionType.RightHandBasePosition
     righthandbaseposition
     """
 
-    Default: str = "DefaultMotion"
-    Greeting: str = "greeting"
-    Nono: str = "nono"
-    NodDeep: str = "nod_deep"
-    Nod: str = "nod"
-    RightHandBasePosition: str = "righthandbaseposition"
-    LeftHandBasePositin: str = "lefthandbaseposition"
+    Default: Literal["DefaultMotion"] = "DefaultMotion"
+    Greeting: Literal["greeting"] = "greeting"
+    Nono: Literal["nono"] = "nono"
+    NodDeep: Literal["nod_deep"] = "nod_deep"
+    Nod: Literal["nod"] = "nod"
+    RightHandBasePosition: Literal["righthandbaseposition"] = "righthandbaseposition"
+    LeftHandBasePositin: Literal["lefthandbaseposition"] = "lefthandbaseposition"
 
 
 """
 Default: str, default = "DefaultMotion"
     デフォルトの姿勢にする
 Greeting: str, default = "greeting"
     挨拶をする．軽い会釈をする．
@@ -92,17 +92,17 @@
     monitor
     >>> GazeObject.Desk
     desk
     >>> GazeObject.Sofa
     Sofa
     """
 
-    Monitor: str = "monitor"
-    Desk: str = "desk"
-    Sofa: str = "Sofa"
+    Monitor: Literal["monitor"] = "monitor"
+    Desk: Literal["desk"] = "desk"
+    Sofa: Literal["Sofa"] = "Sofa"
 
 
 """
 Monitor: str, default = "monitor"
     Ericaの目線をモニターに向ける
 Desk: str, default = "desk"
     Ericaの目線をデスクに向ける
@@ -125,16 +125,16 @@
     --------
     >>> ControllerType.Eye
     EyeController
     >>> ControllerType.Head
     HeadController
     """
 
-    Eye: str = "EyeController"
-    Head: str = "HeadController"
+    Eye: Literal["EyeController"] = "EyeController"
+    Head: Literal["HeadController"] = "HeadController"
 
 
 """
 Eye: str, default = "EyeController"
     目線を動かすことを指示
 Head: str, default = "HeadController"
     顔の向きを動かすことを指示
```

### Comparing `dslclib-0.1.3/dslclib/src/expression_controller.py` & `dslclib-0.2.0/dslclib/src/expression_controller.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from dataclasses import dataclass
-from typing import Optional
+from typing import Literal, Optional
 
 from dslclib.src.base import BaseClient
 
 
 @dataclass
 class ExpressionType:
     """Expression
 
     Ericaの表情を事前定義したデータクラス．
     ExpressionType()とインスタンス化する必要はない．
     """
 
-    MouthA: str = "mouth-a"
-    MouthI: str = "mouth-i"
-    MouthU: str = "mouth-u"
-    MouthE: str = "mouth-e"
-    MouthO: str = "mouth-o"
-    Normal: str = "normal"
-    FullSmile: str = "fullsmile"
-    Smile: str = "smile"
-    Bad: str = "bad"
-    Angry: str = "angry"
-    EyeClose: str = "eye-close"
-    EyeOpen: str = "eye-open"
-    EyeUp: str = "eye-up"
-    EyeDown: str = "eye-down"
+    MouthA: Literal["mouth-a"] = "mouth-a"
+    MouthI: Literal["mouth-i"] = "mouth-i"
+    MouthU: Literal["mouth-u"] = "mouth-u"
+    MouthE: Literal["mouth-e"] = "mouth-e"
+    MouthO: Literal["mouth-o"] = "mouth-o"
+    Normal: Literal["normal"] = "normal"
+    FullSmile: Literal["fullsmile"] = "fullsmile"
+    Smile: Literal["smile"] = "smile"
+    Bad: Literal["bad"] = "bad"
+    Angry: Literal["angry"] = "angry"
+    EyeClose: Literal["eye-close"] = "eye-close"
+    EyeOpen: Literal["eye-open"] = "eye-open"
+    EyeUp: Literal["eye-up"] = "eye-up"
+    EyeDown: Literal["eye-down"] = "eye-down"
 
 
 """
 MouthA: str, default = 'mouth-a'
     「あ」の口
 MouthI: str, default = 'mouth-i'
     「い」の口
```

### Comparing `dslclib-0.1.3/dslclib/src/speech_recognition.py` & `dslclib-0.2.0/dslclib/src/speech_recognition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import re
 from dataclasses import dataclass
-from typing import Optional
+from typing import Literal, Optional
 
 from dslclib.src.base import BaseClient
 
 
 @dataclass
 class STTRecognitionType:
-    InterimResult = "interimresult"
-    Result = "result"
+    InterimResult: Literal["interimresult"] = "interimresult"
+    Result: Literal["result"] = "result"
+
+
+@dataclass
+class OutputForSTTRecognition:
+    type: Literal["interimresult", "result"]
+    result: str
+
+    def __getitem__(self, key):
+        return getattr(self, key)
 
 
 class SpeechRecognitionClient(BaseClient):
     """SpeechRecognitionClient
 
     Google Speech Recognition APIによる音声認識の結果をソケットから受け取るクライアント
     """
@@ -63,15 +72,15 @@
         -------
         received: str
             ソケット通信によって受け取った値を文字列に変換したもの
         """
         received = str(self.sock.recv(4096).decode())
         return received
 
-    def listen(self, interim: bool = True) -> tuple[str, str]:
+    def listen(self, interim: bool = True) -> OutputForSTTRecognition:
         """
         データがたまってからデータを出力するメソッド．
 
         interimをTrueにすると、発話中でもその時点の認識結果を出力する．
 
         interimをFalseにすると、発話終了の上での認識結果のみを出力する．
 
@@ -86,25 +95,40 @@
         interim: bool, default = True
             Trueのときは、発話中でもその時点でたまった認識結果を出力する
 
         Returns
         -------
         tuple[Literal["interimresult", "result"], str]
             (状態, 認識結果)
+
+        Examples
+        --------
+        >>> client = SpeechRecognitionClient()
+        >>> output = client.listen()
+        >>> output.result
+        こんにちは
+        >>> output["result"]
+        こんにちは
         """
         while True:
             received = self.receive_line()
             if interim:  # 発話中でも出力するかどうか
                 matching_result = re.search(r"^interimresult:([^\n]+)\n", received)
                 if matching_result is not None:
-                    return STTRecognitionType.InterimResult, matching_result.group(1)
+                    return OutputForSTTRecognition(
+                        type=STTRecognitionType.InterimResult,
+                        result=matching_result.group(1),
+                    )
 
             matching_result = re.search(r"^result:([^\n]+)\n", received)
             if matching_result is not None:
-                return STTRecognitionType.Result, matching_result.group(1)
+                return OutputForSTTRecognition(
+                    type=STTRecognitionType.Result,
+                    result=matching_result.group(1),
+                )
 
 
 if __name__ == "__main__":
     client = SpeechRecognitionClient()
     for _ in range(20):
         print(client.listen())
```

### Comparing `dslclib-0.1.3/dslclib/src/tts.py` & `dslclib-0.2.0/dslclib/src/tts.py`

 * *Files identical despite different names*

### Comparing `dslclib-0.1.3/pyproject.toml` & `dslclib-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dslclib"
-version = "0.1.3"
+version = "0.2.0"
 description = "対話システムライブコンペティションに使用できるPythonライブラリ"
 authors = ["Yuta SASAKI <yubo1336@lr.pi.titech.ac.jp>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 sphinx = "^7.0.1"
@@ -12,14 +12,16 @@
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 mypy = "^1.4.0"
 isort = "^5.12.0"
 black = "^23.3.0"
+pytest = "^7.4.0"
+pytest-asyncio = "^0.21.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [build-system]
```

### Comparing `dslclib-0.1.3/PKG-INFO` & `dslclib-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dslclib
-Version: 0.1.3
+Version: 0.2.0
 Summary: 対話システムライブコンペティションに使用できるPythonライブラリ
 Author: Yuta SASAKI
 Author-email: yubo1336@lr.pi.titech.ac.jp
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -28,7 +28,16 @@
 - `FaceRecognitinClient`→`FaceRecognitionClient`とタイポを修正しました．
 
 ### 2023/06/30
 
 - `v0.1.3`をリリースしました．
 - タイポを修正しました。
 
+### 2023/07/06
+
+- `v0.2.0`をリリースしました。
+- EmotionType.fearをEmotionType.Fearに修正しました。
+- FaceRecognitionServerの更新に伴い、face_recognition.pyにおけるモジュールをアップデートしました。
+- OutputFor...とクライアントの出力をデータクラスで定義しました。
+    - `OutputForFaceRecognition.emotion`と`OutputForFaceRecognition["emotion"]`の二つのアクセス方法を可能にしました。
+- 型ヒントの一部をstrからLiteralに変更しました。
+
```

