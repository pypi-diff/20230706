# Comparing `tmp/midjourney-py-1.0.2.tar.gz` & `tmp/midjourney-py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midjourney-py-1.0.2.tar", last modified: Thu Jul  6 08:17:54 2023, max compression
+gzip compressed data, was "midjourney-py-1.0.3.tar", last modified: Thu Jul  6 08:27:35 2023, max compression
```

## Comparing `midjourney-py-1.0.2.tar` & `midjourney-py-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 08:17:54.769018 midjourney-py-1.0.2/
--rw-rw-rw-   0        0        0     8401 2023-07-06 08:17:54.756814 midjourney-py-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7563 2023-07-06 08:17:40.000000 midjourney-py-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 08:17:54.676226 midjourney-py-1.0.2/midjourney/
--rw-rw-rw-   0        0        0       66 2023-07-05 11:33:54.000000 midjourney-py-1.0.2/midjourney/__init__.py
--rw-rw-rw-   0        0        0      137 2023-07-05 11:37:33.000000 midjourney-py-1.0.2/midjourney/decrypt.py
--rw-rw-rw-   0        0        0     2392 2023-07-05 12:17:36.000000 midjourney-py-1.0.2/midjourney/index.py
--rw-rw-rw-   0        0        0     2539 2023-07-05 12:02:44.000000 midjourney-py-1.0.2/midjourney/irequest.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:17:54.756814 midjourney-py-1.0.2/midjourney_py.egg-info/
--rw-rw-rw-   0        0        0     8401 2023-07-06 08:17:54.000000 midjourney-py-1.0.2/midjourney_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-06 08:17:54.000000 midjourney-py-1.0.2/midjourney_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 08:17:54.000000 midjourney-py-1.0.2/midjourney_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 08:17:54.000000 midjourney-py-1.0.2/midjourney_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-06 08:17:54.000000 midjourney-py-1.0.2/midjourney_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 08:17:54.769018 midjourney-py-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1485 2023-07-06 08:15:24.000000 midjourney-py-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:27:35.555539 midjourney-py-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-07-06 08:27:35.555539 midjourney-py-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:27:35.555539 midjourney-py-1.0.3/midjourney/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/midjourney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/midjourney/decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/midjourney/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/midjourney/irequest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:27:35.555539 midjourney-py-1.0.3/midjourney_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-07-06 08:27:34.000000 midjourney-py-1.0.3/midjourney_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-06 08:27:35.000000 midjourney-py-1.0.3/midjourney_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 08:27:34.000000 midjourney-py-1.0.3/midjourney_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 08:27:34.000000 midjourney-py-1.0.3/midjourney_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 08:27:34.000000 midjourney-py-1.0.3/midjourney_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 08:27:35.555539 midjourney-py-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/setup.py
```

### Comparing `midjourney-py-1.0.2/README.md` & `midjourney-py-1.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,201 +1,202 @@
-# Installation
-```installation
-pip install midjourney-py==1.0.0
-```
-
-# midjourney
-
-midjourney library provides a simplified and convenient way for developers to interact with the Midjourney API. With this library, developers can easily integrate Midjourney's powerful image processing capabilities into their applications without dealing with the complexities of manual API calls.
-
-## Key Features
-
-1. _Simplified Interface_: The APIRequest class abstracts away the complexities of API
-2. _Authentication Handling_: he library handles the authentication process, ensuring that API requests are properly authenticated with the provided API key.
-3. _Endpoint Methods_: The library provides intuitive methods for each API endpoint, making it easy to perform actions such as describing images, retrieving results, upscaling images, generating images based on prompts, and generating seeds for image generation.
-4. _Response Handling_: The library processes API responses and provides them in a structured format, simplifying the integration of API results into the application workflow.
-
-### Using the Imagine API
-
-```python
-
-from midjourney import Midjourney
-
-midjourney = Midjourney(
-    api_key="API_KEY", callback_uri="")
-
-# IMAGINE
-seed = midjourney.imagine(prompt='cute mouse with hats')
-
-result = midjourney.result(seed=seed)
-if result.get('status') == 'completed':
-    response = result
-    print(response)
-else:
-    message = result.get('message')
-    print(message)
-
-```
-
-### Imagine Response 
-
-_Note_ the _task id_ generated will be passed to the result method to generate the imageUrl
-
-```json
-{
-  "taskId": "your_task_id"
-}
-```
-
-when passed to the result method
-
-```json
-{
-  "status": "completed",
-  "imageUrl": "https://cdn.discordapp.com/attachments/1124090271676772432/1126110757319360582/olivier_A_crying_white_kid_holding_a_blue_candy_splash_around_h_5b0a4099-f398-4118-8206-33f64c1a5589.png"
-}
-```
-
-
-### Using the Describe API
-
-Describe images using the describe api from midjourney
-
-```python
-
-from midjourney import Midjourney
-
-
-midjourney = Midjourney(
-    api_key="API_KEY", callback_uri="")
-
-seed = midjourney.describe(
-    image_path=r"C:\Users\Basit Ng\Downloads\rabbit.png")
-
-result = midjourney.result(seed=seed)
-if result.get('status') == 'completed':
-    response = result
-    print(response)
-else:
-    message = result.get('message')
-    print(message)
-
-
-```
-
-#### Describe response
-
-```json
-{
-  "taskId": "task_id_generated"
-}
-```
-
-when passed to the result method
-
-```json
-{
-  "status": "completed",
-  "content": [
-    "1️⃣ four images of a lion lying in water, in the style of cinematic sets, fantasy characters, cinematic lighting, ray tracing, soggy, naturalistic bird portraits, strong facial expression ",
-    "2️⃣ four different images of a lion sitting in the water, in the style of vray tracing, realistic, emotive portraits, bokeh, [noah bradley](https://goo.gl/search?artist%20noah%20bradley), fairy tale, photorealistic compositions, 8k ",
-    "3️⃣ lion portraits in the water, in the style of [raphael lacoste](https://goo.gl/search?artist%20raphael%20lacoste), bokeh, detailed character expressions, [charles spencelayh](https://goo.gl/search?artist%20charles%20spencelayh), emotional and dramatic scenes, nature inspired, fawncore ",
-    "4️⃣ the lion  lion photo editing, lion phototutorials, lionphotography, portrait photography, animal photography, lion photo, in the style of vray tracing, wet-on-wet blending, multi-panel compositions, rendered in cinema4d, 8k 3d, fairy tale, bokeh"
-  ]
-}
-```
-### Using the RESULT API
-
-```python
-
-from midjourney import Midjourney
-
-
-midjourney = Midjourney(
-    api_key="API_KEY", callback_uri="")
-
-seed = {
-    "taskId": 'your_task_id',
-}
-result = midjourney.result(seed=seed)
-if result.get('status') == 'completed':
-    response = result
-    print(response)
-else:
-    message = result.get('message')
-    print(message)
-
-```
-
-#### Result response
-
-```json
-{
-  "imageURL": "https://cdn.discordapp.com/attachments/1124090271676772432/1125924854990917713/njho_Lion_king_8k_ultra_reality_in_a_rainy_zone___4410563673654_de36ac34-3209-4940-ab10-7178305ca75f.png"
-}
-```
-
-### Using the UPSCALE API
-
-The response will contain the imageURL of the upscaled image.
-
-```python
-from midjourney import Midjourney
-
-midjourney = Midjourney(
-    api_key="API_KEY", callback_uri="")
-
-upscale = midjourney.upscale(
-    task_id="the_task_id", position="2")
-
-print(upscale)
-
-```
-
-#### Upscale response
-
-```json
-{ "imageURL": "https://..........png" }
-```
-
-### Using the SEED API
-
-```python
-from midjourney import Midjourney
-
-midjourney = Midjourney(
-    api_key="AI_KEY", callback_uri="")
-
-seed = midjourney.seed(task_id="the_task_id")
-
-print(seed)
-```
-
-#### Seed response
-
-```json
-{ "taskId": "https://..........png" }
-```
-
-# Get a midjourney api to interact with midjourney-py
-
-[Slash Image](https://slashimagine.pro)
-
-The midjourney is created to make interacting with midjourney-py easy and more structured.
-
-# Wonderful Piece of art generated by the midjourney-py project
-
-1. [A crying white kid holding a blue candy ](https://cdn.discordapp.com/attachments/1124090271676772432/1126110757319360582/olivier_A_crying_white_kid_holding_a_blue_candy_splash_around_h_5b0a4099-f398-4118-8206-33f64c1a5589.png)
-2. [Upscaled Lion](https://cdn.midjourney.com/de36ac34-3209-4940-ab10-7178305ca75f/0_3.png)
-3. [Lion 8k Ultra reality in a rainy zone](https://cdn.discordapp.com/attachments/1124090271676772432/1126104957876187237/olivier_Lion_king_8k_ultra_reality_in_a_rainy_zone___7017353063_1d46e0b1-ae48-47d6-b362-c91415b6d500.png)
-4. [A Lion King in a doom environment](https://cdn.discordapp.com/attachments/1124090271676772432/1125927531137220638/olivier_A_lion_king_in_a_doom_environment___0825378725574918___96c19b7a-5cbe-4879-a24f-1a2941670be8.png)
-5. [Cute Lion with hats](https://cdn.discordapp.com/attachments/1124090271676772432/1125922290304041071/olivier_cute_lion_with_hats___8761618977992125___53dbddbd-63cc-45ef-86da-f16e8026ce96.png)
-6. [8k ultra reality girl](https://cdn.discordapp.com/attachments/1124109999103295560/1125782219466748015/ajaga_abdulbasit_8k_ultra_reality_girl_e4694834-d68a-4335-8713-be93c294a7d6.png)
-7. [Ajaga Abdulbasit generate a custom 8k picture of a coding ninja](https://cdn.discordapp.com/attachments/1124109999103295560/1125250412996472862/ajaga_abdulbasit_generate_a_custom_8k_picture_of_a_coding_ninja_05848b15-4e0f-4694-b0f8-358862b84e06.png)
-
-### Special Thanks
-
-I would like to extend special thanks to _John Coogan_ and the team at _midjourney_ for their invaluable contributions in making the midjourney-py package accessible to others. Their dedication and expertise have greatly enhanced the functionality and usability of the package. By leveraging their knowledge and efforts, developers can now seamlessly integrate the Mid Journey API into their Python projects. Their commitment to open-source collaboration and their willingness to share their expertise have been instrumental in fostering a vibrant and supportive developer community. We extend our heartfelt appreciation to _John Coogan_ and the entire _midjourney_ team for their outstanding contributions and for making the midjourney-py package a valuable resource for developers.
-
-### Discord Community for Code Ninjas
-
-[Join the community](https://discord.gg/U6K4gMZh)
+# Installation
+
+```installation
+pip install midjourney-py==1.0.0
+```
+
+# midjourney
+
+midjourney library provides a simplified and convenient way for developers to interact with the Midjourney API. With this library, developers can easily integrate Midjourney's powerful image processing capabilities into their applications without dealing with the complexities of manual API calls.
+
+## Key Features
+
+1. _Simplified Interface_: The APIRequest class abstracts away the complexities of API
+2. _Authentication Handling_: he library handles the authentication process, ensuring that API requests are properly authenticated with the provided API key.
+3. _Endpoint Methods_: The library provides intuitive methods for each API endpoint, making it easy to perform actions such as describing images, retrieving results, upscaling images, generating images based on prompts, and generating seeds for image generation.
+4. _Response Handling_: The library processes API responses and provides them in a structured format, simplifying the integration of API results into the application workflow.
+
+### Using the Imagine API
+
+```python
+
+from midjourney import Midjourney
+
+midjourney = Midjourney(
+    api_key="API_KEY", callback_uri="")
+
+# IMAGINE
+seed = midjourney.imagine(prompt='cute mouse with hats')
+
+result = midjourney.result(seed=seed)
+if result.get('status') == 'completed':
+    response = result
+    print(response)
+else:
+    message = result.get('message')
+    print(message)
+
+```
+
+### Imagine Response
+
+_Note_ the _task id_ generated will be passed to the result method to generate the imageUrl
+
+```json
+{
+  "taskId": "your_task_id"
+}
+```
+
+when passed to the result method
+
+```json
+{
+  "status": "completed",
+  "imageUrl": "https://cdn.discordapp.com/attachments/1124090271676772432/1126110757319360582/olivier_A_crying_white_kid_holding_a_blue_candy_splash_around_h_5b0a4099-f398-4118-8206-33f64c1a5589.png"
+}
+```
+
+### Using the Describe API
+
+Describe images using the describe api from midjourney
+
+```python
+
+from midjourney import Midjourney
+
+
+midjourney = Midjourney(
+    api_key="API_KEY", callback_uri="")
+
+seed = midjourney.describe(
+    image_path=r"C:\Users\Basit Ng\Downloads\rabbit.png")
+
+result = midjourney.result(seed=seed)
+if result.get('status') == 'completed':
+    response = result
+    print(response)
+else:
+    message = result.get('message')
+    print(message)
+
+
+```
+
+#### Describe response
+
+```json
+{
+  "taskId": "task_id_generated"
+}
+```
+
+when passed to the result method
+
+```json
+{
+  "status": "completed",
+  "content": [
+    "1️⃣ four images of a lion lying in water, in the style of cinematic sets, fantasy characters, cinematic lighting, ray tracing, soggy, naturalistic bird portraits, strong facial expression ",
+    "2️⃣ four different images of a lion sitting in the water, in the style of vray tracing, realistic, emotive portraits, bokeh, [noah bradley](https://goo.gl/search?artist%20noah%20bradley), fairy tale, photorealistic compositions, 8k ",
+    "3️⃣ lion portraits in the water, in the style of [raphael lacoste](https://goo.gl/search?artist%20raphael%20lacoste), bokeh, detailed character expressions, [charles spencelayh](https://goo.gl/search?artist%20charles%20spencelayh), emotional and dramatic scenes, nature inspired, fawncore ",
+    "4️⃣ the lion  lion photo editing, lion phototutorials, lionphotography, portrait photography, animal photography, lion photo, in the style of vray tracing, wet-on-wet blending, multi-panel compositions, rendered in cinema4d, 8k 3d, fairy tale, bokeh"
+  ]
+}
+```
+
+### Using the RESULT API
+
+```python
+
+from midjourney import Midjourney
+
+
+midjourney = Midjourney(
+    api_key="API_KEY", callback_uri="")
+
+seed = {
+    "taskId": 'your_task_id',
+}
+result = midjourney.result(seed=seed)
+if result.get('status') == 'completed':
+    response = result
+    print(response)
+else:
+    message = result.get('message')
+    print(message)
+
+```
+
+#### Result response
+
+```json
+{
+  "imageURL": "https://cdn.discordapp.com/attachments/1124090271676772432/1125924854990917713/njho_Lion_king_8k_ultra_reality_in_a_rainy_zone___4410563673654_de36ac34-3209-4940-ab10-7178305ca75f.png"
+}
+```
+
+### Using the UPSCALE API
+
+The response will contain the imageURL of the upscaled image.
+
+```python
+from midjourney import Midjourney
+
+midjourney = Midjourney(
+    api_key="API_KEY", callback_uri="")
+
+upscale = midjourney.upscale(
+    task_id="the_task_id", position="2")
+
+print(upscale)
+
+```
+
+#### Upscale response
+
+```json
+{ "imageURL": "https://..........png" }
+```
+
+### Using the SEED API
+
+```python
+from midjourney import Midjourney
+
+midjourney = Midjourney(
+    api_key="AI_KEY", callback_uri="")
+
+seed = midjourney.seed(task_id="the_task_id")
+
+print(seed)
+```
+
+#### Seed response
+
+```json
+{ "taskId": "https://..........png" }
+```
+
+# Get a midjourney api to interact with midjourney-py
+
+[Get API key](https://slashimagine.pro)
+
+The midjourney is created to make interacting with midjourney-py easy and more structured.
+
+# Wonderful Piece of art generated by the midjourney-py project
+
+1. [A crying white kid holding a blue candy ](https://cdn.discordapp.com/attachments/1124090271676772432/1126110757319360582/olivier_A_crying_white_kid_holding_a_blue_candy_splash_around_h_5b0a4099-f398-4118-8206-33f64c1a5589.png)
+2. [Upscaled Lion](https://cdn.midjourney.com/de36ac34-3209-4940-ab10-7178305ca75f/0_3.png)
+3. [Lion 8k Ultra reality in a rainy zone](https://cdn.discordapp.com/attachments/1124090271676772432/1126104957876187237/olivier_Lion_king_8k_ultra_reality_in_a_rainy_zone___7017353063_1d46e0b1-ae48-47d6-b362-c91415b6d500.png)
+4. [A Lion King in a doom environment](https://cdn.discordapp.com/attachments/1124090271676772432/1125927531137220638/olivier_A_lion_king_in_a_doom_environment___0825378725574918___96c19b7a-5cbe-4879-a24f-1a2941670be8.png)
+5. [Cute Lion with hats](https://cdn.discordapp.com/attachments/1124090271676772432/1125922290304041071/olivier_cute_lion_with_hats___8761618977992125___53dbddbd-63cc-45ef-86da-f16e8026ce96.png)
+6. [8k ultra reality girl](https://cdn.discordapp.com/attachments/1124109999103295560/1125782219466748015/ajaga_abdulbasit_8k_ultra_reality_girl_e4694834-d68a-4335-8713-be93c294a7d6.png)
+7. [Ajaga Abdulbasit generate a custom 8k picture of a coding ninja](https://cdn.discordapp.com/attachments/1124109999103295560/1125250412996472862/ajaga_abdulbasit_generate_a_custom_8k_picture_of_a_coding_ninja_05848b15-4e0f-4694-b0f8-358862b84e06.png)
+
+### Special Thanks
+
+I would like to extend special thanks to _John Coogan_ and the team at _midjourney_ for their invaluable contributions in making the midjourney-py package accessible to others. Their dedication and expertise have greatly enhanced the functionality and usability of the package. By leveraging their knowledge and efforts, developers can now seamlessly integrate the Mid Journey API into their Python projects. Their commitment to open-source collaboration and their willingness to share their expertise have been instrumental in fostering a vibrant and supportive developer community. We extend our heartfelt appreciation to _John Coogan_ and the entire _midjourney_ team for their outstanding contributions and for making the midjourney-py package a valuable resource for developers.
+
+### Discord Community for Code Ninjas
+
+[Join the community](https://discord.gg/U6K4gMZh)
```

### Comparing `midjourney-py-1.0.2/midjourney/index.py` & `midjourney-py-1.0.3/midjourney/index.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from typing import Dict
-import time
-from midjourney.irequest import APIRequest
-
-
-class Midjourney:
-    def __init__(self, api_key: str, callback_uri: str):
-        self.api_request = APIRequest(api_key, callback_uri)
-
-    def result(self, seed: Dict) -> Dict:
-        task_id = seed.get('taskId')
-
-        if not task_id:
-            return {'status': 'error', 'message': 'Invalid seed data'}
-
-        print("Running task....")
-        while True:
-            try:
-                response = self.api_request.get_result(task_id)
-            except Exception as e:
-                return {'status': 'error', 'message': str(e)}
-
-            if response and isinstance(response, dict):
-                if 'imageURL' in response:
-                    print("Completed task....")
-                    return {'status': 'completed', 'imageUrl': response['imageURL']}
-                elif 'seed' in response:
-                    print("Completed task....")
-                    return {'status': 'completed', 'seed': response['seed']}
-                elif 'content' in response:
-                    print("Completed task....")
-                    return {'status': 'completed', 'content': response['content']}
-                elif response.get('status') == 'running':
-                    percentage = response.get('percentage')
-                    print(f"Task is {percentage}% complete.")
-                elif response.get('status') in ['pending', 'waiting-to-start', 'unknown', {}, 'failed-please-resubmit']:
-                    print("Task is pending. Waiting for it to start...")
-                    time.sleep(2)
-                    continue
-            else:
-                print("Waiting for task to start...")
-                time.sleep(2)
-                continue
-
-            if response.get('status') not in ['running', 'pending', 'unknown']:
-                break
-
-    def imagine(self, prompt: str) -> Dict:
-        return self.api_request.imagine(prompt)
-
-    def upscale(self, task_id: str, position: str) -> Dict:
-        return self.api_request.upscale_image(task_id, position)
-
-    def seed(self, task_id: str) -> Dict:
-        return self.api_request.seed(task_id)
-
-    def describe(self, image_path: str, filename: str) -> Dict:
-        return self.api_request.describe_image(image_file_path=image_path, filename=filename)
+from typing import Dict
+import time
+from midjourney.irequest import APIRequest
+
+
+class Midjourney:
+    def __init__(self, api_key: str, callback_uri: str):
+        self.api_request = APIRequest(api_key, callback_uri)
+
+    def result(self, seed: Dict) -> Dict:
+        task_id = seed.get('taskId')
+
+        if not task_id:
+            return {'status': 'error', 'message': 'Invalid seed data'}
+
+        print("Running task....")
+        while True:
+            try:
+                response = self.api_request.get_result(task_id)
+            except Exception as e:
+                return {'status': 'error', 'message': str(e)}
+
+            if response and isinstance(response, dict):
+                if 'imageURL' in response:
+                    print("Completed task....")
+                    return {'status': 'completed', 'imageUrl': response['imageURL']}
+                elif 'seed' in response:
+                    print("Completed task....")
+                    return {'status': 'completed', 'seed': response['seed']}
+                elif 'content' in response:
+                    print("Completed task....")
+                    return {'status': 'completed', 'content': response['content']}
+                elif response.get('status') == 'running':
+                    percentage = response.get('percentage')
+                    print(f"Task is {percentage}% complete.")
+                elif response.get('status') in ['pending', 'waiting-to-start', 'unknown', {}, 'failed-please-resubmit']:
+                    print("Task is pending. Waiting for it to start...")
+                    time.sleep(2)
+                    continue
+            else:
+                print("Waiting for task to start...")
+                time.sleep(2)
+                continue
+
+            if response.get('status') not in ['running', 'pending', 'unknown']:
+                break
+
+    def imagine(self, prompt: str) -> Dict:
+        return self.api_request.imagine(prompt)
+
+    def upscale(self, task_id: str, position: str) -> Dict:
+        return self.api_request.upscale_image(task_id, position)
+
+    def seed(self, task_id: str) -> Dict:
+        return self.api_request.seed(task_id)
+
+    def describe(self, image_path: str, filename: str) -> Dict:
+        return self.api_request.describe_image(image_file_path=image_path, filename=filename)
```

