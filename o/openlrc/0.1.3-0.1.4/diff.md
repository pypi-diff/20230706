# Comparing `tmp/openlrc-0.1.3.tar.gz` & `tmp/openlrc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlrc-0.1.3.tar", max compression
+gzip compressed data, was "openlrc-0.1.4.tar", max compression
```

## Comparing `openlrc-0.1.3.tar` & `openlrc-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.1.3/LICENSE
--rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.1.3/openlrc/__init__.py
--rw-r--r--   0        0        0     6642 2023-06-24 22:32:18.752179 openlrc-0.1.3/openlrc/chatbot.py
--rw-r--r--   0        0        0     2273 2023-06-26 16:59:34.458995 openlrc-0.1.3/openlrc/context.py
--rw-r--r--   0        0        0      701 2023-06-25 03:24:03.534882 openlrc-0.1.3/openlrc/exceptions.py
--rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.1.3/openlrc/logger.py
--rw-r--r--   0        0        0    11568 2023-06-27 02:37:19.204604 openlrc-0.1.3/openlrc/openlrc.py
--rw-r--r--   0        0        0     5160 2023-06-27 03:39:14.631067 openlrc-0.1.3/openlrc/opt.py
--rw-r--r--   0        0        0     7768 2023-06-26 19:29:42.139607 openlrc-0.1.3/openlrc/prompter.py
--rw-r--r--   0        0        0     3608 2023-06-27 02:39:59.839257 openlrc-0.1.3/openlrc/subtitle.py
--rw-r--r--   0        0        0     5905 2023-06-26 02:59:37.362684 openlrc-0.1.3/openlrc/transcribe.py
--rw-r--r--   0        0        0     5788 2023-06-26 19:30:54.045688 openlrc-0.1.3/openlrc/translate.py
--rw-r--r--   0        0        0     5744 2023-06-25 13:45:28.650508 openlrc-0.1.3/openlrc/utils.py
--rw-r--r--   0        0        0     1305 2023-06-27 04:24:27.572507 openlrc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3909 2023-06-27 02:28:07.921266 openlrc-0.1.3/README.md
--rw-r--r--   0        0        0     5271 1970-01-01 00:00:00.000000 openlrc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.1.4/LICENSE
+-rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.1.4/openlrc/__init__.py
+-rw-r--r--   0        0        0     6642 2023-07-01 13:36:53.572387 openlrc-0.1.4/openlrc/chatbot.py
+-rw-r--r--   0        0        0     2704 2023-06-27 13:49:50.307093 openlrc-0.1.4/openlrc/context.py
+-rw-r--r--   0        0        0      966 2023-07-05 20:31:15.832362 openlrc-0.1.4/openlrc/exceptions.py
+-rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.1.4/openlrc/logger.py
+-rw-r--r--   0        0        0    13866 2023-07-06 14:20:07.448891 openlrc-0.1.4/openlrc/openlrc.py
+-rw-r--r--   0        0        0     5204 2023-07-03 18:14:57.916841 openlrc-0.1.4/openlrc/opt.py
+-rw-r--r--   0        0        0     7664 2023-06-27 08:09:12.518292 openlrc-0.1.4/openlrc/prompter.py
+-rw-r--r--   0        0        0     6372 2023-06-29 05:51:12.383562 openlrc-0.1.4/openlrc/subtitle.py
+-rw-r--r--   0        0        0    15382 2023-07-06 13:45:34.304340 openlrc-0.1.4/openlrc/transcribe.py
+-rw-r--r--   0        0        0     5726 2023-06-27 18:43:39.771392 openlrc-0.1.4/openlrc/translate.py
+-rw-r--r--   0        0        0     6552 2023-07-06 13:45:34.300323 openlrc-0.1.4/openlrc/utils.py
+-rw-r--r--   0        0        0     1718 2023-07-06 14:29:59.404295 openlrc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5508 2023-07-06 14:34:39.772560 openlrc-0.1.4/README.md
+-rw-r--r--   0        0        0     6960 1970-01-01 00:00:00.000000 openlrc-0.1.4/PKG-INFO
```

### Comparing `openlrc-0.1.3/LICENSE` & `openlrc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.3/openlrc/chatbot.py` & `openlrc-0.1.4/openlrc/chatbot.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.3/openlrc/context.py` & `openlrc-0.1.4/openlrc/context.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #  Copyright (C) 2023. Hao Zheng
 #  All rights reserved.
-
-import os
+from difflib import get_close_matches
+from pathlib import Path
+from typing import Union
 
 import yaml
 
 from openlrc.logger import logger
 
 
 class Context:
@@ -14,51 +15,62 @@
         Context(optional) for translation.
 
         :param background: Providing background information for establishing context for the translation.
         :param synopsis_map: {"name(without extension)": "synopsis", ...}
         :param audio_type: Audio type, default to Anime.
         :param config_path: Path to config file.
         """
-        self.config_path = config_path
+        self.config_path = None
         self.background = background
         self.audio_type = audio_type
         self.synopsis_map = synopsis_map if synopsis_map else dict()
 
-        # if config_path exist, load yaml file, else create a new one
-        if config_path and os.path.exists(config_path):
-            self.load_config(self.config_path)
-
-    def load_config(self, config_path):
-        if not os.path.exists(config_path):
+        # if config_path exist, load yaml file
+        if config_path:
+            config_path = Path(config_path)
+            if config_path.exists():
+                self.load_config(config_path)
+            else:
+                raise FileNotFoundError(f'Config file {config_path} not found.')
+
+    def load_config(self, config_path: Union[str, Path]):
+        config_path = Path(config_path)
+        if not config_path.exists():
             raise FileNotFoundError(f'Config file {config_path} not found.')
 
         with open(config_path, 'r', encoding='utf-8') as f:
-            config = yaml.load(f, yaml.CLoader)
+            config: dict = yaml.safe_load(f)
 
-        if config['background']:
+        if config.get('background'):
             self.background = config['background']
 
-        if config['audio_type']:
+        if config.get('audio_type'):
             self.audio_type = config['audio_type']
 
-        if config['synopsis_map']:
+        if config.get('synopsis_map'):
             self.synopsis_map = config['synopsis_map']
 
+        self.config_path = config_path
+
     def save_config(self):
         with open(self.config_path, 'w') as f:
             yaml.dump({
                 'background': self.background,
                 'audio_type': self.audio_type,
                 'synopsis_map': self.synopsis_map,
             }, f)
 
     def get_synopsis(self, audio_name):
-        if self.synopsis_map and any(k in audio_name for k in self.synopsis_map.keys()):
-            for k, v in self.synopsis_map.items():
-                if k in audio_name:
-                    logger.info(f'Found synopsis map: {k} -> {v}')
-                    return v
+        value = ''
+        if self.synopsis_map:
+            matches = get_close_matches(audio_name, self.synopsis_map.keys())
+            if matches:
+                key = matches[0]
+                value = self.synopsis_map.get(key)
+                logger.info(f'Found synopsis map: {key} -> {value}')
+            else:
+                logger.info(f'No synopsis map for {audio_name} found.')
 
-        return ''
+        return value
 
     def __str__(self):
         return f'Context(background={self.background}, audio_type={self.audio_type}, synopsis_map={self.synopsis_map})'
```

### Comparing `openlrc-0.1.3/openlrc/exceptions.py` & `openlrc-0.1.4/openlrc/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,7 +21,17 @@
     def __init__(self, message):
         super().__init__(message)
 
 
 class FfmpegException(Exception):
     def __init__(self, message):
         super().__init__(message)
+
+
+class TranscribeException(Exception):
+    def __init__(self, message):
+        super().__init__(message)
+
+
+class DependencyException(Exception):
+    def __init__(self, message):
+        super().__init__(f'Dependency not correctly installed: {message}')
```

### Comparing `openlrc-0.1.3/openlrc/logger.py` & `openlrc-0.1.4/openlrc/logger.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.3/openlrc/openlrc.py` & `openlrc-0.1.4/openlrc/openlrc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,250 +1,305 @@
 #  Copyright (C) 2023. Hao Zheng
 #  All rights reserved.
 
+import concurrent.futures
 import json
-import os
-import traceback
-from multiprocessing.pool import ThreadPool
+from concurrent.futures import Future
+from pathlib import Path
 from pprint import pformat
 from queue import Queue
-from threading import Thread, Lock
+from threading import Lock
+from typing import List
 
 from openlrc.context import Context
 from openlrc.logger import logger
 from openlrc.opt import SubtitleOptimizer
 from openlrc.subtitle import Subtitle
 from openlrc.transcribe import Transcriber
 from openlrc.translate import GPTTranslator
-from openlrc.utils import Timer, change_ext, extend_filename, get_audio_duration, format_timestamp, extract_audio, \
-    get_file_type, get_filename
+from openlrc.utils import Timer, extend_filename, get_audio_duration, format_timestamp, extract_audio, \
+    get_file_type
 
 
 class LRCer:
-    def __init__(self, model_name='large-v2', compute_type='float16', fee_limit=0.1, consumer_thread=11):
+    def __init__(self, model_name='large-v2', compute_type='float16', fee_limit=0.1, consumer_thread=11,
+                 asr_options=None, vad_options=None):
         """
         :param model_name: Name of whisper model (tiny, tiny.en, base, base.en, small, small.en, medium,
                         medium.en, large-v1, or large-v2) When a size is configured, the converted model is downloaded
                         from the Hugging Face Hub.
                         Default: ``large-v2``
         :param compute_type: The type of computation to use. Can be ``int8``, ``int8_float16``, ``int16``,
                         ``float16`` or ``float32``.
                         Default: ``float16``
         :param fee_limit: The maximum fee you are willing to pay for one translation call. Default: ``0.1``
         :param consumer_thread: To prevent exceeding the RPM and TPM limits set by OpenAI, the default is TPM/MAX_TOKEN.
+        :param asr_options: parameters for whisper model.
+        :param vad_options: parameters for VAD model.
         """
 
         self.transcriber = Transcriber(model_name=model_name, compute_type=compute_type)
         self.fee_limit = fee_limit
         self.api_fee = 0  # Can be updated in different thread, operation should be thread-safe
         self.from_video = set()
         self.context: Context = Context()
 
         self._lock = Lock()
         self.exception = None
         self.consumer_thread = consumer_thread
 
-    def transcription_producer(self, transcription_queue, audio_paths):
+        # Default Automatic Speech Recognition (ASR) options
+        self.asr_options = {
+            "beam_size": 5,
+            "best_of": 5,
+            "patience": 1,
+            "length_penalty": 1,
+            "temperatures": [0.0, 0.2, 0.4, 0.6, 0.8, 1.0],
+            "compression_ratio_threshold": 2.4,
+            "log_prob_threshold": -1.0,
+            "no_speech_threshold": 0.6,
+            "condition_on_previous_text": True,
+            "initial_prompt": None,
+            "prefix": None,
+            "suppress_blank": True,
+            "suppress_tokens": [-1],
+            "without_timestamps": True,
+            "max_initial_timestamp": 0.0,
+            "word_timestamps": False,
+            "prepend_punctuations": "\"'“¿([{-",
+            "append_punctuations": "\"'.。,，!！?？:：”)]}、",
+            "suppress_numerals": False,
+        }
+
+        # Parameters for VAD (see pyannote.audio), reduce them if speech is not being detected
+        self.vad_options = {
+            "vad_onset": 0.500,
+            "vad_offset": 0.363
+        }
+
+        if asr_options:
+            self.asr_options.update(asr_options)
+
+        if vad_options:
+            self.vad_options.update(vad_options)
+
+    def transcription_producer(self, transcription_queue, audio_paths, src_lang):
         """
         Sequential Producer.
         """
         for audio_path in audio_paths:
-            transcribed_path = change_ext(extend_filename(audio_path, '_transcribed'), 'json')
-            if not os.path.exists(transcribed_path):
+            transcribed_path = extend_filename(audio_path, '_transcribed').with_suffix('.json')
+            if not transcribed_path.exists():
                 with Timer('Transcription process'):
                     logger.info(
                         f'Audio length: {audio_path}: {format_timestamp(get_audio_duration(audio_path), fmt="srt")}')
-                    segments, info = self.transcriber.transcribe(audio_path, batch_size=4)
+                    segments, info = self.transcriber.transcribe(audio_path, batch_size=4, language=src_lang,
+                                                                 asr_options=self.asr_options,
+                                                                 vad_options=self.vad_options)
                     logger.info(f'Detected language: {info.language}')
 
                     # From generator to list with progress bar shown
-                    seg_list = segments['sentences']  # [{'text': ..., 'start_word': ..., 'end_word':...}, ...]
+                    seg_list = segments['sentences']  # [{'text': ..., 'start': ..., 'end':...}, ...]
                     logger.debug(f'Transcribed fast-whisper Segments: {seg_list}')
 
                 # Save the transcribed json
                 self.to_json(seg_list, name=transcribed_path, lang=info.language)  # xxx_transcribed.json
             else:
                 logger.info(f'Found transcribed json file: {transcribed_path}')
             transcription_queue.put(transcribed_path)
             logger.info(f'Put transcription: {transcribed_path}')
 
         transcription_queue.put(None)
         logger.info('Transcription producer finished.')
 
-    def transcription_consumer(self, transcription_queue, target_lang, prompter):
+    def transcription_consumer(self, transcription_queue, target_lang, prompter, skip_trans):
         """
         Parallel Consumer.
         """
-        with ThreadPool() as pool:
-            _ = [pool.apply_async(self.translation_worker,
-                                  args=(transcription_queue, target_lang, prompter))
-                 for _ in range(self.consumer_thread)]
-            pool.close()
-            pool.join()
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            futures = [executor.submit(self.consumer_worker, transcription_queue, target_lang, prompter, skip_trans)
+                       for _ in range(self.consumer_thread)]
+            concurrent.futures.wait(futures)
         logger.info('Transcription consumer finished.')
 
-    def translation_worker(self, transcription_queue, target_lang, prompter):
+    def consumer_worker(self, transcription_queue, target_lang, prompter, skip_trans):
         """
         Parallel translation.
         """
         while True:
             logger.debug(f'Translation worker waiting transcription...')
             transcribed_path = transcription_queue.get()
 
             if transcribed_path is None:
                 transcription_queue.put(None)
                 logger.debug('Translation worker finished.')
                 return
 
             logger.info(f'Got transcription: {transcribed_path}')
-            transcribed_sub = Subtitle(transcribed_path)
+            transcribed_sub = Subtitle.from_json(transcribed_path)
             transcribed_opt_sub = self.post_process(transcribed_sub, update_name=True)
-            audio_name = get_filename(transcribed_path.replace('_transcribed', ''), without_dir=True)
+            audio_name = transcribed_path.stem.replace('_transcribed', '')
 
             # xxx_transcribed_optimized_translated.json
             translated_path = extend_filename(transcribed_opt_sub.filename, '_translated')
-            compare_path = transcribed_path.replace('_transcribed.json', '_compare.json')
-            if not os.path.exists(translated_path):
-                if not os.path.exists(compare_path):
-                    # Translate the transcribed json
-                    translator = GPTTranslator(prompter=prompter, fee_limit=self.fee_limit)
-                    context = self.context
-                    with Timer('Translation process'):
-                        try:
-                            target_texts = translator.translate(
-                                transcribed_opt_sub.get_texts(),
-                                src_lang=transcribed_opt_sub.lang,
-                                target_lang=target_lang,
-                                title=audio_name,
-                                audio_type=context.audio_type,
-                                background=context.background,
-                                synopsis=context.get_synopsis(audio_name),
-                                compare_path=compare_path
-                            )
-                        except Exception as e:
-                            self.exception = e
-
-                    with self._lock:
-                        self.api_fee += translator.api_fee  # Ensure thread-safe
-                else:
-                    logger.info(f'Found compare json file: {compare_path}')
-                    with open(compare_path, 'r', encoding='utf-8') as f:
-                        target_texts = [item['output'] for item in json.load(f)['compare']]
-                    if len(target_texts) != len(transcribed_opt_sub):
-                        logger.error(f'Compare json file {compare_path} is not valid.')
-                        raise ValueError(f'Compare json file {compare_path} is not valid.')
-                transcribed_opt_sub.set_texts(target_texts, lang=target_lang)
-
-                # xxx_transcribed_optimized_translated.json
-                transcribed_opt_sub.save(translated_path, update_name=True)
+            if skip_trans:
+                final_subtitle = transcribed_opt_sub
             else:
-                logger.info(f'Found translated json file: {translated_path}')
-
-            translated_sub = Subtitle(translated_path)
-            output_filename = transcribed_path.replace('_transcribed.json', '.json')
-
-            final_subtitle = self.post_process(translated_sub, output_name=output_filename, t2m=target_lang == 'zh-cn',
-                                               update_name=True)  # xxx.json
+                with Timer('Translation process'):
+                    try:
+                        final_subtitle = self._translate(audio_name, prompter, target_lang, transcribed_opt_sub,
+                                                         translated_path)
+                    except Exception as e:
+                        self.exception = e
 
             final_subtitle.to_lrc()
-            if get_filename(output_filename) in self.from_video:
+            if audio_name in self.from_video:
                 final_subtitle.to_srt()
             logger.info(f'Translation fee til now: {self.api_fee:.4f} USD')
 
-    def run(self, paths, target_lang='zh-cn', prompter='base_trans', context_path=None):
+    def _translate(self, audio_name, prompter, target_lang, transcribed_opt_sub, translated_path):
+        json_filename = Path(audio_name).with_suffix('.json')
+        compare_path = Path(translated_path.parent, f'{audio_name}_compare.json')
+        if not translated_path.exists():
+            if not compare_path.exists():
+                # Translate the transcribed json
+                translator = GPTTranslator(prompter=prompter, fee_limit=self.fee_limit)
+                context = self.context
+
+                target_texts = translator.translate(
+                    transcribed_opt_sub.texts,
+                    src_lang=transcribed_opt_sub.lang,
+                    target_lang=target_lang,
+                    title=audio_name,
+                    audio_type=context.audio_type,
+                    background=context.background,
+                    synopsis=context.get_synopsis(audio_name),
+                    compare_path=compare_path
+                )
+
+                with self._lock:
+                    self.api_fee += translator.api_fee  # Ensure thread-safe
+            else:
+                logger.info(f'Found compare json file: {compare_path}')
+                with open(compare_path, 'r', encoding='utf-8') as f:
+                    target_texts = [item['output'] for item in json.load(f)['compare']]
+                if len(target_texts) != len(transcribed_opt_sub):
+                    logger.error(f'Compare json file {compare_path} is not valid.')
+                    raise ValueError(f'Compare json file {compare_path} is not valid.')
+            transcribed_opt_sub.set_texts(target_texts, lang=target_lang)
+
+            # xxx_transcribed_optimized_translated.json
+            transcribed_opt_sub.save(translated_path, update_name=True)
+        else:
+            logger.info(f'Found translated json file: {translated_path}')
+        translated_sub = Subtitle.from_json(translated_path)
+
+        final_subtitle = self.post_process(translated_sub, output_name=json_filename, t2m=target_lang == 'zh-cn',
+                                           update_name=True)  # xxx.json
+        return final_subtitle
+
+    def run(self, paths, src_lang=None, target_lang='zh-cn', prompter='base_trans', context_path=None,
+            skip_trans=False):
         """
         Split the translation into 2 phases: transcription and translation. They're running in parallel.
         Firstly, transcribe the audios one-by-one. At the same time, translation threads are created and waiting for
         the transcription results. After all the transcriptions are done, the translation threads will start to
         translate the transcribed texts.
 
         :param paths: Audio/Video paths, can be a list or a single path.
+        :param src_lang: Language of the audio, default to auto detect.
         :param target_lang: Target language, default to Mandarin Chinese.
         :param prompter: Currently, only `base_trans` is supported.
         :param context_path: path to context config file. (Default to use `context.yaml` in the first audio's directory)
+        :param skip_trans: Skip the translation process if True.
         """
-        if isinstance(paths, str):
+        if not paths:
+            logger.warning('No audio/video file given. Skip LRCer.run()')
+            return
+
+        if isinstance(paths, str) or isinstance(paths, Path):
             paths = [paths]
 
         audio_paths = self.pre_process(paths)
 
         logger.info(f'Working on {len(audio_paths)} audio files: {pformat(audio_paths)}')
 
         if context_path:
+            context_path = Path(context_path)
             self.context.load_config(context_path)
             logger.info(f'Found context config: {context_path}')
             logger.debug(f'Context: {self.context}')
         else:
             # Try to find the default `context.yaml` in the first audio's directory
             try:
-                context_path = os.path.join(os.path.dirname(paths[0]), 'context.yaml')
+                context_path = audio_paths[0].parent / 'context.yaml'
                 self.context.load_config(context_path)
                 logger.info(f'Found context config file: {context_path}')
             except FileNotFoundError:
                 logger.info(f'Default context config not found: {self.context}, using default context.')
 
         transcription_queue = Queue()
 
         with Timer('Transcription (Producer) and Translation (Consumer) process'):
-            consumer = Thread(target=self.transcription_consumer,
-                              args=(transcription_queue, target_lang, prompter))
-            producer = Thread(target=self.transcription_producer,
-                              args=(transcription_queue, audio_paths))
+            consumer = concurrent.futures.ThreadPoolExecutor(thread_name_prefix='Consumer') \
+                .submit(self.transcription_consumer, transcription_queue, target_lang, prompter, skip_trans)
+            producer: Future = concurrent.futures.ThreadPoolExecutor(thread_name_prefix='Producer') \
+                .submit(self.transcription_producer, transcription_queue, audio_paths, src_lang)
 
-            consumer.start()
-            producer.start()
-
-            producer.join()
-            consumer.join()
+            producer.result()
+            consumer.result()
 
             if self.exception:
-                traceback.print_exception(type(self.exception), self.exception, self.exception.__traceback__)
+                # traceback.print_exception(type(self.exception), self.exception, self.exception.__traceback__)
+                raise self.exception
 
         logger.info(f'Totally used API fee: {self.api_fee:.4f} USD')
 
     @staticmethod
     def to_json(segments, name, lang):
         result = {
             'generator': 'LRC generated by https://github.com/zh-plus/Open-Lyrics',
             'language': lang,
             'segments': []
         }
 
         for segment in segments:
             result['segments'].append({
-                'start': segment["start_word"]["start"],
-                'end': segment["end_word"]["end"],
+                'start': segment["start"],
+                'end': segment["end"],
                 'text': segment["text"]
             })
 
         with open(name, 'w', encoding='utf-8') as f:
             json.dump(result, f, ensure_ascii=False, indent=4)
 
         logger.info(f'File saved to {name}')
 
         return result
 
     def pre_process(self, paths):
+        paths = [Path(path) for path in paths]
+
         # Check if path is audio or video
         for i, path in enumerate(paths):
-            if not os.path.exists(path) or not os.path.isfile(path):
+            if not path.exists() or not path.is_file():
                 raise FileNotFoundError(f'File not found: {path}')
 
             paths[i] = extract_audio(path)
 
             if get_file_type(path) == 'video':
-                self.from_video.add(get_filename(path))
+                self.from_video.add(path.name)
 
         return paths
 
     @staticmethod
-    def post_process(transcribed_sub, output_name=None, remove_files=None, t2m=False, update_name=False):
+    def post_process(transcribed_sub: Path, output_name: Path = None, remove_files: List[Path] = None, t2m=False,
+                     update_name=False):
         optimizer = SubtitleOptimizer(transcribed_sub)
         optimizer.perform_all(t2m=t2m)
         optimizer.save(output_name, update_name=update_name)
 
         # Remove intermediate files
         if remove_files:
-            for file in remove_files:
-                os.remove(file)
+            _ = [file.unlink() for file in remove_files if file.is_file()]
 
         return optimizer.subtitle
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openlrc-0.1.3/openlrc/opt.py` & `openlrc-0.1.4/openlrc/opt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 #  Copyright (C) 2023. Hao Zheng
 #  All rights reserved.
 
 import re
+from pathlib import Path
 from typing import Union
 
 import zhconv
 
 from openlrc.logger import logger
 from openlrc.subtitle import Subtitle
 from openlrc.utils import extend_filename
 
+# Different language may need different threshold
+cut_long_threshold = {
+    350: 'en',
+    125: 'cn, ja'
+}
+
 
 class SubtitleOptimizer:
-    def __init__(self, subtitle: Union[str, Subtitle]):
-        if isinstance(subtitle, str):
-            subtitle = Subtitle(subtitle)
+    def __init__(self, subtitle: Union[Path, Subtitle]):
+        if isinstance(subtitle, Path):
+            subtitle = Subtitle.from_json(subtitle)
 
         self.subtitle = subtitle
+        self.lang = self.subtitle.lang
 
     @property
     def filename(self):
         return self.subtitle.filename
 
     def merge_same(self):
         """
@@ -30,16 +38,14 @@
 
         for i, element in enumerate(self.subtitle.segments):
             if i == 0 or element.text != new_elements[-1].text:
                 new_elements.append(element)
             else:
                 new_elements[-1].end = element.end
 
-        logger.debug(f'Merge same text: {len(self.subtitle.segments)} -> {len(new_elements)}')
-
         self.subtitle.segments = new_elements
 
     def merge_short(self, threshold=1.5):
         """
         Merge the short duration subtitle.
         """
         new_elements = []
@@ -67,16 +73,14 @@
             else:
                 if not merged_element:
                     merged_element = element
                 else:
                     merged_element.text += ' ' + element.text
                     merged_element.end = element.end
 
-        logger.debug(f'Merge the short duration subtitle: {len(self.subtitle.segments)} -> {len(new_elements)}')
-
         self.subtitle.segments = new_elements
 
     def merge_repeat(self):
         """
         Merge the same pattern in one lyric.
         :return:
         """
@@ -84,55 +88,52 @@
 
         for i, element in enumerate(new_elements):
             text = element.text
             text = re.sub(r'(.)\1{4,}', r'\1\1...', text)
             text = re.sub(r'(.+)\1{4,}', r'\1\1...', text)
             new_elements[i].text = text
 
-        logger.debug('Merge same words done.')
-
         self.subtitle.segments = new_elements
 
-    def cut_long(self, threshold=125, keep=20):
+    def cut_long(self, keep=20):
+        threshold = 150
+        for threshold, lang in cut_long_threshold.items():
+            if self.lang.lower() in lang:
+                threshold = threshold
+                break
+
         new_elements = self.subtitle.segments
 
         for i, element in enumerate(new_elements):
-            if len(element.text) > threshold:
+            if len(element.text) > threshold and len(element.text) / len(set(element.text)) > 3.0:
+                # text length larger than threshold and text density is larger than 3.0
                 logger.warning(f'Cut long text: {element.text}\nInto: {element.text[:keep]}...')
                 new_elements[i].text = element.text[:keep] + f'(Cut to {keep})'
 
-        logger.debug('Cut long text done.')
-
         self.subtitle.segments = new_elements
 
     def traditional2mandarin(self):
         new_elements = self.subtitle.segments
 
         for i, element in enumerate(new_elements):
             new_elements[i].text = zhconv.convert(element.text, locale='zh-cn')
 
-        logger.debug('Traditional Chinese to Mandarin done.')
-
         self.subtitle.segments = new_elements
 
     def remove_unk(self):
         new_elements = self.subtitle.segments
 
         for i, element in enumerate(new_elements):
             new_elements[i].text = element.text.replace('<unk>', '')
 
-        logger.debug('Remove <unk> done.')
-
         self.subtitle.segments = new_elements
 
     def remove_empty(self):
         self.subtitle.segments = [element for element in self.subtitle.segments if element.text]
 
-        logger.debug('Remove empty done.')
-
     def perform_all(self, t2m=False):
         for _ in range(2):
             self.merge_same()
             self.merge_short()
             self.merge_repeat()
             self.cut_long()
             self.remove_unk()
```

### Comparing `openlrc-0.1.3/openlrc/prompter.py` & `openlrc-0.1.4/openlrc/prompter.py`

 * *Files 5% similar despite different names*

```diff
@@ -175,18 +175,16 @@
         if translated_lang != target_lang:
             logger.warning(f'Translated language is {translated_lang}, not {target_lang}.')
             return False
 
         # It's ok to keep going without summary and scene
         if not summary or not summary.group(1):
             logger.warning(f'Fail to extract summary.')
-            logger.debug(f'output_str: {content}')
         if not scene or not scene.group(1):
             logger.warning(f'Fail to extract scene.')
-            logger.debug(f'output_str: {content}')
 
         return True
 
 
 prompter_map = {
     'base_trans': BaseTranslatePrompter,
 }
```

### Comparing `openlrc-0.1.3/openlrc/translate.py` & `openlrc-0.1.4/openlrc/translate.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,33 +10,30 @@
 
 from openlrc.chatbot import GPTBot
 from openlrc.logger import logger
 from openlrc.prompter import prompter_map, BaseTranslatePrompter
 
 
 class GPTTranslator:
-    def __init__(self, prompter: str = 'base_trans', fee_limit=0.1, chunk_size=30, intercept_line=None,
-                 force_translate=False):
+    def __init__(self, prompter: str = 'base_trans', fee_limit=0.1, chunk_size=30, intercept_line=None):
         """
         :param prompter: Translate prompter, choices can be found in `prompter_map` from prompter.py.
         :param fee_limit: Fee limit (USD) for OpenAI API.
         :param chunk_size: Use small (<20) chunk size for speed (more async call), and enhance translation
                     stability (keep audio timeline consistency).
         :param intercept_line: Intercepted text line number.
-        :param force_translate: Force translation even if the source language is the same as the target language.
         """
         if prompter not in prompter_map:
             raise ValueError(f'Prompter {prompter} not found.')
 
         self.prompter = prompter
         self.fee_limit = fee_limit
         self.chunk_size = chunk_size
         self.api_fee = 0
         self.intercept_line = intercept_line
-        self.force_translate = force_translate
 
     @staticmethod
     def make_chunks(texts, chunk_size=30):
         """
         Split the subtitle into chunks, each chunk has a line number of chunk_size.
         :return: List of chunks, each chunk is a list of (line_number, text) tuples
         """
@@ -134,11 +131,14 @@
             'api-version': '3.0',
             'from': src_lang,
             'to': target_lang
         }
 
         body = [{'text': text} for text in texts]
 
-        request = requests.post(self.constructed_url, params=params, headers=self.headers, json=body)
+        try:
+            request = requests.post(self.constructed_url, params=params, headers=self.headers, json=body, timeout=20)
+        except TimeoutError:
+            raise RuntimeError('Failed to connect to Microsoft Translator API.')
         response = request.json()
 
         return json.dumps(response, sort_keys=True, ensure_ascii=False, indent=4, separators=(',', ': '))
```

### Comparing `openlrc-0.1.3/pyproject.toml` & `openlrc-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "openlrc"
-version = "0.1.3"
+version = "0.1.4"
 description = "Transcribe (whisper) and translate (gpt) voice into LRC file."
 license = "MIT"
 authors = [
     "Hao Zheng <zhenghaosustc@gmail.com>"
 ]
 readme = "README.md"
 homepage = "https://github.com/zh-plus/Open-Lyrics"
@@ -32,28 +32,40 @@
 include = [
     { path = 'openlrc' },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 openai = "^0.27.6"
-faster-whisper = "^0.6.0"
 tiktoken = "^0.3.1"
 langcodes = "^3.3.0"
 language-data = "^1.1"
-rich = "^12.6.0"
 tqdm = "^4.65.0"
 audioread = "^3.0.0"
 zhconv = "^1.4.3"
 punctuators = "^0.0.5"
 colorlog = "^6.7.0"
-pytest = "^7.4.0"
 ffmpeg-python = "^0.2.0"
 lingua-language-detector = "^1.3.2"
+pandas = "^2.0.2"
+filetype = "^1.2.0"
+jaconvV2 = "^0.4"
+spacy = "^3.5.4"
+pysbd = "^0.3.4"
+faster-whisper = "^0.6.0"
+#whisperx = { git = "https://github.com/m-bain/whisperx.git" }
+#torch = { version = "2.0.1", source = "torch" }
+#torchaudio = { version = "2.0.2", source = "torch" }
+#torchvision = { version = "0.15.2", source = "torch" }
 
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
+#[[tool.poetry.source]]
+#name = "torch"
+#url = "https://download.pytorch.org/whl/nightly/cu117"
+#priority = "supplemental"
+
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/zh-plus/Open-Lyrics/issues"
```

### Comparing `openlrc-0.1.3/README.md` & `openlrc-0.1.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 # Open-Lyrics
 
+[![PyPI](https://img.shields.io/pypi/v/openlrc)](https://pypi.org/project/openlrc/)
+[![PyPI - License](https://img.shields.io/pypi/l/openlrc)](https://pypi.org/project/openlrc/)
+[![Downloads](https://static.pepy.tech/badge/openlrc)](https://pepy.tech/project/openlrc)
+![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/zh-plus/Open-Lyrics/ci.yml)
+
 Open-Lyrics is a Python library that transcribes voice files using
 [faster-whisper](https://github.com/guillaumekln/faster-whisper), and translates/polishes the resulting text
 into `.lrc` files in the desired language using [OpenAI-GPT](https://github.com/openai/openai-python).
 
 ## Installation
 
 1. Please install CUDA and cuDNN first according to https://opennmt.net/CTranslate2/installation.html to
    enable `faster-whisper`.
 
 2. Add your [OpenAI API key](https://platform.openai.com/account/api-keys) to environment variable `OPENAI_API_KEY`.
 
 3. Install [PyTorch](https://pytorch.org/get-started/locally/):
-    ```shell
+   ```shell
    pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
    ```
 
-4. Install [whisperx](https://github.com/m-bain/whisperX)
+4. Install [whisperx](https://github.com/m-bain/whisperX) and (Recommended) the
+   latest [fast-whisper](https://github.com/guillaumekln/faster-whisper)
+   ```shell
+   pip install git+https://github.com/guillaumekln/faster-whisper
+   pip install git+https://github.com/m-bain/whisperx.git
+   ```
 
-    ```shell
-    pip install git+https://github.com/m-bain/whisperx.git
-    ```
+5. (Optional) If you want to process videos, install [ffmpeg](https://ffmpeg.org/download.html) and add `bin` directory
+   to your `PATH`.
 
-5. This project can be installed from PyPI:
+6. This project can be installed from PyPI:
 
     ```shell
     pip install openlrc
     ```
 
    or install directly from GitHub:
 
     ```shell
     pip install git+https://github.com/zh-plus/Open-Lyrics
     ```
 
+7. Go to [Spacy](https://spacy.io/usage) to install the required package using `spacy download xxx`.
+   For example, you need `spacy download ja_core_news_sm` if the source language is japanese.
+
 ## Usage
 
 ```python
 from openlrc import LRCer
 
 lrcer = LRCer()
 
@@ -46,14 +58,15 @@
 
 # Multiple files
 lrcer.run(['./data/test1.mp3', './data/test2.mp3'], target_lang='zh-cn')
 # Note we run the transcription sequentially, but run the translation concurrently for each file.
 
 # Path can contain video
 lrcer.run(['./data/test_audio.mp3', './data/test_video.mp4'], target_lang='zh-cn')
+# Generate translated ./data/test_audio.lrc and ./data/test_video.srt
 
 # Use context.yaml to improve translation
 lrcer.run('./data/test.mp3', target_lang='zh-cn', context_path='./data/context.yaml')
 ```
 
 ### Context
 
@@ -75,33 +88,44 @@
 
 ## Todo
 
 - [x] [Efficiency] Batched translate/polish for GPT request (enable contextual ability).
 - [x] [Efficiency] Concurrent support for GPT request.
 - [x] [Efficiency & Transcription Quality] Use [whisperx](https://github.com/m-bain/whisperX) for transcription.
 - [x] [Translation Quality] Make translate prompt more robust according to https://github.com/openai/openai-cookbook.
-- [x] [Usability] Automatically fix json encoder error using GPT.
+- [x] [Feature] Automatically fix json encoder error using GPT.
 - [x] [Efficiency] Asynchronously perform transcription and translation for multiple audio inputs.
 - [x] [Quality] Improve batched translation/polish prompt according
   to [gpt-subtrans](https://github.com/machinewrapped/gpt-subtrans).
-- [x] [Usability] Input video support.
-- [ ] [Usability] Multiple output format support.
+- [x] [Feature] Input video support.
+- [X] [Feature] Multiple output format support.
+- [ ] [Feature] Align ground-truth transcription with audio.
 - [ ] [Quality]
   Use [multilingual language model](https://www.sbert.net/docs/pretrained_models.html#multi-lingual-models) to assess
   translation quality.
 - [ ] [Quality] Speech enhancement for input audio.
 - [ ] [Efficiency] Add Azure OpenAI Service support.
-- [ ] [Usability] Add local LLM support.
-- [ ] [Usability] Multiple translate engine (Microsoft, DeepL, Google, etc.) support.
+- [ ] [Quality] Use [claude](https://www.anthropic.com/index/introducing-claude) for translation.
+- [ ] [Feature] Add local LLM support.
+- [ ] [Feature] Multiple translate engine (Microsoft, DeepL, Google, etc.) support.
+- [ ] [**Feature**] Build
+  a [electron + fastapi](https://ivanyu2021.hashnode.dev/electron-django-desktop-app-integrate-javascript-and-python)
+  GUI for cross-platform application.
+- [ ] Add [fine-tuned whisper-large-v2](https://huggingface.co/models?search=whisper-large-v2) models for common
+  languages.
 - [ ] [Others] Add transcribed examples.
     - [ ] Song
     - [ ] Podcast
     - [ ] Audiobook
 
 ## Credits
 
 - https://github.com/guillaumekln/faster-whisper
 - https://github.com/m-bain/whisperX
 - https://github.com/openai/openai-python
 - https://github.com/openai/whisper
 - https://github.com/machinewrapped/gpt-subtrans
-- https://github.com/MicrosoftTranslator/Text-Translation-API-V3-Python
+- https://github.com/MicrosoftTranslator/Text-Translation-API-V3-Python
+
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=zh-plus/Open-Lyrics&type=Date)](https://star-history.com/#zh-plus/Open-Lyrics&Date)
```

### Comparing `openlrc-0.1.3/PKG-INFO` & `openlrc-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlrc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Transcribe (whisper) and translate (gpt) voice into LRC file.
 Home-page: https://github.com/zh-plus/Open-Lyrics
 License: MIT
 Keywords: openai-gpt3,whisper,voice transcribe,lrc
 Author: Hao Zheng
 Author-email: zhenghaosustc@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -17,63 +17,78 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: audioread (>=3.0.0,<4.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: faster-whisper (>=0.6.0,<0.7.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
+Requires-Dist: filetype (>=1.2.0,<2.0.0)
+Requires-Dist: jaconvV2 (>=0.4,<0.5)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: lingua-language-detector (>=1.3.2,<2.0.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
+Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: punctuators (>=0.0.5,<0.0.6)
-Requires-Dist: pytest (>=7.4.0,<8.0.0)
-Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: pysbd (>=0.3.4,<0.4.0)
+Requires-Dist: spacy (>=3.5.4,<4.0.0)
 Requires-Dist: tiktoken (>=0.3.1,<0.4.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: zhconv (>=1.4.3,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/zh-plus/Open-Lyrics/issues
 Description-Content-Type: text/markdown
 
 # Open-Lyrics
 
+[![PyPI](https://img.shields.io/pypi/v/openlrc)](https://pypi.org/project/openlrc/)
+[![PyPI - License](https://img.shields.io/pypi/l/openlrc)](https://pypi.org/project/openlrc/)
+[![Downloads](https://static.pepy.tech/badge/openlrc)](https://pepy.tech/project/openlrc)
+![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/zh-plus/Open-Lyrics/ci.yml)
+
 Open-Lyrics is a Python library that transcribes voice files using
 [faster-whisper](https://github.com/guillaumekln/faster-whisper), and translates/polishes the resulting text
 into `.lrc` files in the desired language using [OpenAI-GPT](https://github.com/openai/openai-python).
 
 ## Installation
 
 1. Please install CUDA and cuDNN first according to https://opennmt.net/CTranslate2/installation.html to
    enable `faster-whisper`.
 
 2. Add your [OpenAI API key](https://platform.openai.com/account/api-keys) to environment variable `OPENAI_API_KEY`.
 
 3. Install [PyTorch](https://pytorch.org/get-started/locally/):
-    ```shell
+   ```shell
    pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
    ```
 
-4. Install [whisperx](https://github.com/m-bain/whisperX)
+4. Install [whisperx](https://github.com/m-bain/whisperX) and (Recommended) the
+   latest [fast-whisper](https://github.com/guillaumekln/faster-whisper)
+   ```shell
+   pip install git+https://github.com/guillaumekln/faster-whisper
+   pip install git+https://github.com/m-bain/whisperx.git
+   ```
 
-    ```shell
-    pip install git+https://github.com/m-bain/whisperx.git
-    ```
+5. (Optional) If you want to process videos, install [ffmpeg](https://ffmpeg.org/download.html) and add `bin` directory
+   to your `PATH`.
 
-5. This project can be installed from PyPI:
+6. This project can be installed from PyPI:
 
     ```shell
     pip install openlrc
     ```
 
    or install directly from GitHub:
 
     ```shell
     pip install git+https://github.com/zh-plus/Open-Lyrics
     ```
 
+7. Go to [Spacy](https://spacy.io/usage) to install the required package using `spacy download xxx`.
+   For example, you need `spacy download ja_core_news_sm` if the source language is japanese.
+
 ## Usage
 
 ```python
 from openlrc import LRCer
 
 lrcer = LRCer()
 
@@ -82,14 +97,15 @@
 
 # Multiple files
 lrcer.run(['./data/test1.mp3', './data/test2.mp3'], target_lang='zh-cn')
 # Note we run the transcription sequentially, but run the translation concurrently for each file.
 
 # Path can contain video
 lrcer.run(['./data/test_audio.mp3', './data/test_video.mp4'], target_lang='zh-cn')
+# Generate translated ./data/test_audio.lrc and ./data/test_video.srt
 
 # Use context.yaml to improve translation
 lrcer.run('./data/test.mp3', target_lang='zh-cn', context_path='./data/context.yaml')
 ```
 
 ### Context
 
@@ -111,33 +127,45 @@
 
 ## Todo
 
 - [x] [Efficiency] Batched translate/polish for GPT request (enable contextual ability).
 - [x] [Efficiency] Concurrent support for GPT request.
 - [x] [Efficiency & Transcription Quality] Use [whisperx](https://github.com/m-bain/whisperX) for transcription.
 - [x] [Translation Quality] Make translate prompt more robust according to https://github.com/openai/openai-cookbook.
-- [x] [Usability] Automatically fix json encoder error using GPT.
+- [x] [Feature] Automatically fix json encoder error using GPT.
 - [x] [Efficiency] Asynchronously perform transcription and translation for multiple audio inputs.
 - [x] [Quality] Improve batched translation/polish prompt according
   to [gpt-subtrans](https://github.com/machinewrapped/gpt-subtrans).
-- [x] [Usability] Input video support.
-- [ ] [Usability] Multiple output format support.
+- [x] [Feature] Input video support.
+- [X] [Feature] Multiple output format support.
+- [ ] [Feature] Align ground-truth transcription with audio.
 - [ ] [Quality]
   Use [multilingual language model](https://www.sbert.net/docs/pretrained_models.html#multi-lingual-models) to assess
   translation quality.
 - [ ] [Quality] Speech enhancement for input audio.
 - [ ] [Efficiency] Add Azure OpenAI Service support.
-- [ ] [Usability] Add local LLM support.
-- [ ] [Usability] Multiple translate engine (Microsoft, DeepL, Google, etc.) support.
+- [ ] [Quality] Use [claude](https://www.anthropic.com/index/introducing-claude) for translation.
+- [ ] [Feature] Add local LLM support.
+- [ ] [Feature] Multiple translate engine (Microsoft, DeepL, Google, etc.) support.
+- [ ] [**Feature**] Build
+  a [electron + fastapi](https://ivanyu2021.hashnode.dev/electron-django-desktop-app-integrate-javascript-and-python)
+  GUI for cross-platform application.
+- [ ] Add [fine-tuned whisper-large-v2](https://huggingface.co/models?search=whisper-large-v2) models for common
+  languages.
 - [ ] [Others] Add transcribed examples.
     - [ ] Song
     - [ ] Podcast
     - [ ] Audiobook
 
 ## Credits
 
 - https://github.com/guillaumekln/faster-whisper
 - https://github.com/m-bain/whisperX
 - https://github.com/openai/openai-python
 - https://github.com/openai/whisper
 - https://github.com/machinewrapped/gpt-subtrans
 - https://github.com/MicrosoftTranslator/Text-Translation-API-V3-Python
+
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=zh-plus/Open-Lyrics&type=Date)](https://star-history.com/#zh-plus/Open-Lyrics&Date)
+
```

