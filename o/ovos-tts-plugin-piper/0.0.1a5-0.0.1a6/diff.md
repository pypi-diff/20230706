# Comparing `tmp/ovos_tts_plugin_piper-0.0.1a5-py3-none-any.whl.zip` & `tmp/ovos_tts_plugin_piper-0.0.1a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12017 bytes, number of entries: 10
--rw-r--r--  2.0 unx    14985 b- defN 23-Jul-06 00:51 ovos_tts_plugin_piper/__init__.py
--rw-r--r--  2.0 unx     4775 b- defN 23-Jul-06 00:51 ovos_tts_plugin_piper/engine.py
--rw-r--r--  2.0 unx      178 b- defN 23-Jul-06 00:51 ovos_tts_plugin_piper/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Jul-06 00:52 ovos_tts_plugin_piper-0.0.1a5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1149 b- defN 23-Jul-06 00:52 ovos_tts_plugin_piper-0.0.1a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 00:52 ovos_tts_plugin_piper-0.0.1a5.dist-info/WHEEL
--rw-r--r--  2.0 unx      186 b- defN 23-Jul-06 00:52 ovos_tts_plugin_piper-0.0.1a5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-06 00:52 ovos_tts_plugin_piper-0.0.1a5.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-06 00:52 ovos_tts_plugin_piper-0.0.1a5.dist-info/zip-safe
--rw-rw-r--  2.0 unx      948 b- defN 23-Jul-06 00:52 ovos_tts_plugin_piper-0.0.1a5.dist-info/RECORD
-10 files, 33685 bytes uncompressed, 10357 bytes compressed:  69.3%
+Zip file size: 11960 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    14821 b- defN 23-Jul-06 00:53 ovos_tts_plugin_piper/__init__.py
+-rw-r--r--  2.0 unx     4775 b- defN 23-Jul-06 00:53 ovos_tts_plugin_piper/engine.py
+-rw-r--r--  2.0 unx      178 b- defN 23-Jul-06 00:53 ovos_tts_plugin_piper/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Jul-06 00:53 ovos_tts_plugin_piper-0.0.1a6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1149 b- defN 23-Jul-06 00:53 ovos_tts_plugin_piper-0.0.1a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 00:53 ovos_tts_plugin_piper-0.0.1a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      186 b- defN 23-Jul-06 00:53 ovos_tts_plugin_piper-0.0.1a6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-06 00:53 ovos_tts_plugin_piper-0.0.1a6.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-06 00:53 ovos_tts_plugin_piper-0.0.1a6.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jul-06 00:53 ovos_tts_plugin_piper-0.0.1a6.dist-info/RECORD
+10 files, 33521 bytes uncompressed, 10300 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: ovos_tts_plugin_piper/engine.py
 Comment: 
 
 Filename: ovos_tts_plugin_piper/version.py
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a5.dist-info/LICENSE
+Filename: ovos_tts_plugin_piper-0.0.1a6.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a5.dist-info/METADATA
+Filename: ovos_tts_plugin_piper-0.0.1a6.dist-info/METADATA
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a5.dist-info/WHEEL
+Filename: ovos_tts_plugin_piper-0.0.1a6.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a5.dist-info/entry_points.txt
+Filename: ovos_tts_plugin_piper-0.0.1a6.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a5.dist-info/top_level.txt
+Filename: ovos_tts_plugin_piper-0.0.1a6.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a5.dist-info/zip-safe
+Filename: ovos_tts_plugin_piper-0.0.1a6.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a5.dist-info/RECORD
+Filename: ovos_tts_plugin_piper-0.0.1a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_tts_plugin_piper/__init__.py

```diff
@@ -223,16 +223,14 @@
         else:
             raise ValueError(f"invalid voice: {voice}")
 
     def _piper_synth(self, text: str, lang: str, voice: str, speaker: int) -> bytes:
         """Synthesize audio from text and return WAV bytes"""
 
         engine, speaker = self.get_model(lang, voice, speaker)
-        phonemes = PiperG2P(engine).utterance2arpa(text, lang, ignore_oov=True)
-        phonemes = " ".join([f"{p}:0.4" for p in phonemes])
 
         sents = re.split('(?<=[.!?]) +', text)
 
         results = [engine.synthesize(sentence,
                                      speaker_id=speaker,
                                      length_scale=self.length_scale,
                                      noise_scale=self.noise_scale,
@@ -247,15 +245,15 @@
 
             with wav_file:
                 for audio_bytes in results:
                     # Add audio to existing WAV file
                     wav_file.writeframes(audio_bytes)
             wav_bytes = wav_io.getvalue()
 
-        return wav_bytes, phonemes
+        return wav_bytes
 
     def get_tts(self, sentence, wav_file, lang=None, voice=None, speaker=None):
         """Generate WAV and phonemes.
 
         Arguments:
             sentence (str): sentence to generate audio for
             wav_file (str): output file
@@ -268,19 +266,19 @@
         """
         lang = lang or self.lang
         # HACK: bug in some neon-core versions - neon_audio.tts.neon:_get_tts:198 - INFO - Legacy Neon TTS signature found 
         if isinstance(speaker, dict):
             LOG.warning("Legacy Neon TTS signature found, pass speaker as a str")
             speaker = None
 
-        wav_bytes, phonemes = self._piper_synth(sentence, lang, voice, speaker)
+        wav_bytes = self._piper_synth(sentence, lang, voice, speaker)
         with open(wav_file, "wb") as f:
             f.write(wav_bytes)
 
-        return wav_file, phonemes
+        return wav_file, None
 
     def available_languages(self) -> set:
         return set(self.lang2voices.keys())
 
 
 PiperTTSPluginConfig = {
     lang: [{v: {"model": PiperTTSPlugin.voice2url[v], "offline": True}}
```

## ovos_tts_plugin_piper/version.py

```diff
@@ -1,8 +1,8 @@
 
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 1
-VERSION_ALPHA = 5
+VERSION_ALPHA = 6
 # END_VERSION_BLOCK
```

## Comparing `ovos_tts_plugin_piper-0.0.1a5.dist-info/LICENSE` & `ovos_tts_plugin_piper-0.0.1a6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_tts_plugin_piper-0.0.1a5.dist-info/METADATA` & `ovos_tts_plugin_piper-0.0.1a6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-piper
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: piper tts plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-plugin-piper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft plugin tts OVOS OpenVoiceOS
 Platform: UNKNOWN
```

## Comparing `ovos_tts_plugin_piper-0.0.1a5.dist-info/RECORD` & `ovos_tts_plugin_piper-0.0.1a6.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-ovos_tts_plugin_piper/__init__.py,sha256=iS5AU4wneCG0Fetalb_BKoiDfIB7gGCzcRkEgJIwA2o,14985
+ovos_tts_plugin_piper/__init__.py,sha256=r8Ss6p1-En6HHw9UhQ_rH1kP9yphqV1DndKDBCBXxOQ,14821
 ovos_tts_plugin_piper/engine.py,sha256=zCEcyQiCkqMp_JZgkLUdKniZdV_S7bAuAqbEIXLBwkw,4775
-ovos_tts_plugin_piper/version.py,sha256=DHwYRdBiDIoBbzvMhHbyzw5ef5Od5A-kbyHcVIlNYpQ,178
-ovos_tts_plugin_piper-0.0.1a5.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_tts_plugin_piper-0.0.1a5.dist-info/METADATA,sha256=vaw5am8h_2jBnkOTd4KUy_a2IfBEHZaGFR1VW8kKypg,1149
-ovos_tts_plugin_piper-0.0.1a5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_tts_plugin_piper-0.0.1a5.dist-info/entry_points.txt,sha256=eHpADEdMHzf8Y-h30EKm587TkxMsv91Xb98ph3DgRUY,186
-ovos_tts_plugin_piper-0.0.1a5.dist-info/top_level.txt,sha256=WTvxxS42UAwh0oi25ypLaxvMGD85j_wGzrux2QFoqLs,22
-ovos_tts_plugin_piper-0.0.1a5.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_tts_plugin_piper-0.0.1a5.dist-info/RECORD,,
+ovos_tts_plugin_piper/version.py,sha256=ujZhFLO_-AiuLxyMWb_XD0TJPl03Jnd8Ugqsh4nWAZY,178
+ovos_tts_plugin_piper-0.0.1a6.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_tts_plugin_piper-0.0.1a6.dist-info/METADATA,sha256=0jgRywcY7VRpp5Wa8hm_Ru1HiXUxr9gSVPFc2-S9FbY,1149
+ovos_tts_plugin_piper-0.0.1a6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_tts_plugin_piper-0.0.1a6.dist-info/entry_points.txt,sha256=eHpADEdMHzf8Y-h30EKm587TkxMsv91Xb98ph3DgRUY,186
+ovos_tts_plugin_piper-0.0.1a6.dist-info/top_level.txt,sha256=WTvxxS42UAwh0oi25ypLaxvMGD85j_wGzrux2QFoqLs,22
+ovos_tts_plugin_piper-0.0.1a6.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_tts_plugin_piper-0.0.1a6.dist-info/RECORD,,
```

