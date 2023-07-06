# Comparing `tmp/neural_data_simulator-0.2.0.tar.gz` & `tmp/neural_data_simulator-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_data_simulator-0.2.0.tar", max compression
+gzip compressed data, was "neural_data_simulator-0.2.2.tar", max compression
```

## Comparing `neural_data_simulator-0.2.0.tar` & `neural_data_simulator-0.2.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    11339 2023-04-27 10:26:04.608077 neural_data_simulator-0.2.0/LICENSE
--rw-r--r--   0        0        0     1736 2023-04-27 10:26:04.608077 neural_data_simulator-0.2.0/README.md
--rw-r--r--   0        0        0     3281 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      970 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/decoder/__init__.py
--rw-r--r--   0        0        0      999 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/decoder/config/settings_decoder.yaml
--rw-r--r--   0        0        0     7657 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/decoder/decoders.py
--rw-r--r--   0        0        0     4988 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/decoder/run_decoder.py
--rw-r--r--   0        0        0     2487 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/__init__.py
--rw-r--r--   0        0        0      607 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/config/lsl.config
--rw-r--r--   0        0        0     5069 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/config/settings.yaml
--rw-r--r--   0        0        0     1297 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/config/settings_streamer.yaml
--rw-r--r--   0        0        0     3887 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/encoder.py
--rw-r--r--   0        0        0    27939 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/ephys_generator.py
--rw-r--r--   0        0        0     9464 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/filters.py
--rw-r--r--   0        0        0     2591 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/health_checker.py
--rw-r--r--   0        0        0    11823 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/inputs.py
--rw-r--r--   0        0        0     1792 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/models.py
--rw-r--r--   0        0        0    14019 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/outputs.py
--rw-r--r--   0        0        0     3129 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/runner.py
--rw-r--r--   0        0        0     4198 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/samples.py
--rw-r--r--   0        0        0       65 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/__init__.py
--rw-r--r--   0        0        0      103 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/errors.py
--rw-r--r--   0        0        0     4723 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/post_install_config.py
--rw-r--r--   0        0        0     9843 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/run_encoder.py
--rw-r--r--   0        0        0     9060 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/run_ephys_generator.py
--rw-r--r--   0        0        0    11992 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/run_streamer.py
--rw-r--r--   0        0        0     6979 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/settings.py
--rw-r--r--   0        0        0     5574 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/streamers.py
--rw-r--r--   0        0        0     2765 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/timing.py
--rw-r--r--   0        0        0       56 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/util/__init__.py
--rw-r--r--   0        0        0     3775 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/util/buffer.py
--rw-r--r--   0        0        0      961 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/util/circular_dequeue.py
--rw-r--r--   0        0        0     3046 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/util/runtime.py
--rw-r--r--   0        0        0     1291 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/util/settings_loader.py
--rw-r--r--   0        0        0       48 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/plugins/__init__.py
--rw-r--r--   0        0        0     1000 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/plugins/examples/gamepad_preprocessor.py
--rw-r--r--   0        0        0     5294 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/plugins/examples/model.py
--rw-r--r--   0        0        0      572 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/plugins/examples/postprocessor.py
--rw-r--r--   0        0        0      498 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/plugins/examples/preprocessor.py
--rw-r--r--   0        0        0     4005 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/plugins/examples/tests/test_model.py
--rw-r--r--   0        0        0      288 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/recorder/__init__.py
--rw-r--r--   0        0        0     3201 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/recorder/run_recorder.py
--rw-r--r--   0        0        0      251 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/__init__.py
--rw-r--r--   0        0        0      872 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/__init__.py
--rw-r--r--   0        0        0     2125 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/buttons.py
--rw-r--r--   0        0        0     2734 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/input_events.py
--rw-r--r--   0        0        0     1628 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/joystick.py
--rw-r--r--   0        0        0     9783 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/metrics.py
--rw-r--r--   0        0        0     4049 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/scalers.py
--rw-r--r--   0        0        0     1583 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/screen_info.py
--rw-r--r--   0        0        0     2778 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/sprites.py
--rw-r--r--   0        0        0     6472 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_runner.py
--rw-r--r--   0        0        0    11351 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_state.py
--rw-r--r--   0        0        0    13007 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_window.py
--rw-r--r--   0        0        0     1593 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/config/settings_center_out_reach.yaml
--rw-r--r--   0        0        0    11674 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/run_center_out_reach.py
--rw-r--r--   0        0        0      837 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/run_closed_loop.py
--rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 neural_data_simulator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-07-06 08:31:26.514233 neural_data_simulator-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-06 08:31:26.514233 neural_data_simulator-0.2.2/README.md
+-rw-r--r--   0        0        0     3282 2023-07-06 08:31:48.754514 neural_data_simulator-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      970 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/decoder/__init__.py
+-rw-r--r--   0        0        0      999 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/decoder/config/settings_decoder.yaml
+-rw-r--r--   0        0        0     7657 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/decoder/decoders.py
+-rw-r--r--   0        0        0     5114 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/decoder/run_decoder.py
+-rw-r--r--   0        0        0     2487 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/__init__.py
+-rw-r--r--   0        0        0      607 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/config/lsl.config
+-rw-r--r--   0        0        0     5069 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/config/settings.yaml
+-rw-r--r--   0        0        0     1297 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/config/settings_streamer.yaml
+-rw-r--r--   0        0        0     3887 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/encoder.py
+-rw-r--r--   0        0        0    27939 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/ephys_generator.py
+-rw-r--r--   0        0        0     9464 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/filters.py
+-rw-r--r--   0        0        0     2591 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/health_checker.py
+-rw-r--r--   0        0        0    11823 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/inputs.py
+-rw-r--r--   0        0        0     1792 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/models.py
+-rw-r--r--   0        0        0    14019 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/outputs.py
+-rw-r--r--   0        0        0     3129 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/runner.py
+-rw-r--r--   0        0        0     4198 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/samples.py
+-rw-r--r--   0        0        0       65 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/errors.py
+-rw-r--r--   0        0        0     4723 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/post_install_config.py
+-rw-r--r--   0        0        0     9969 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_encoder.py
+-rw-r--r--   0        0        0     9186 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_ephys_generator.py
+-rw-r--r--   0        0        0    12118 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_streamer.py
+-rw-r--r--   0        0        0     6979 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/settings.py
+-rw-r--r--   0        0        0     5574 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/streamers.py
+-rw-r--r--   0        0        0     2765 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/timing.py
+-rw-r--r--   0        0        0       56 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/util/__init__.py
+-rw-r--r--   0        0        0     3775 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/util/buffer.py
+-rw-r--r--   0        0        0      961 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/util/circular_dequeue.py
+-rw-r--r--   0        0        0     4046 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/util/runtime.py
+-rw-r--r--   0        0        0     1291 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/util/settings_loader.py
+-rw-r--r--   0        0        0       48 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/plugins/__init__.py
+-rw-r--r--   0        0        0     1000 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/plugins/examples/gamepad_preprocessor.py
+-rw-r--r--   0        0        0     5294 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/plugins/examples/model.py
+-rw-r--r--   0        0        0      572 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/plugins/examples/postprocessor.py
+-rw-r--r--   0        0        0      498 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/plugins/examples/preprocessor.py
+-rw-r--r--   0        0        0     4005 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/plugins/examples/tests/test_model.py
+-rw-r--r--   0        0        0      288 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/recorder/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/recorder/run_recorder.py
+-rw-r--r--   0        0        0      251 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/__init__.py
+-rw-r--r--   0        0        0      872 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/__init__.py
+-rw-r--r--   0        0        0     2125 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/buttons.py
+-rw-r--r--   0        0        0     2901 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/input_events.py
+-rw-r--r--   0        0        0     1628 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/joystick.py
+-rw-r--r--   0        0        0     9827 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/metrics.py
+-rw-r--r--   0        0        0     4049 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/scalers.py
+-rw-r--r--   0        0        0     1583 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/screen_info.py
+-rw-r--r--   0        0        0     2778 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/sprites.py
+-rw-r--r--   0        0        0     6563 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_runner.py
+-rw-r--r--   0        0        0    11351 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_state.py
+-rw-r--r--   0        0        0    13249 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_window.py
+-rw-r--r--   0        0        0     1593 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/config/settings_center_out_reach.yaml
+-rw-r--r--   0        0        0    12028 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/run_center_out_reach.py
+-rw-r--r--   0        0        0     2014 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/run_closed_loop.py
+-rw-r--r--   0        0        0     3672 1970-01-01 00:00:00.000000 neural_data_simulator-0.2.2/PKG-INFO
```

### Comparing `neural_data_simulator-0.2.0/LICENSE` & `neural_data_simulator-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/README.md` & `neural_data_simulator-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 The Neural Data Simulator is a real-time system for generating electrophysiology data from behavioral data (e.g. cursor movement, arm kinematics, etc) in real-time. The NDS system can be used to test and validate closed-loop brain-computer interface systems without the need for a human in the loop, generate synthetic data for algorithm optimization, and provide a platform on which to develop BCI decoders.
 
 ## Documentation
 
 See the [documentation](https://agencyenterprise.github.io/neural-data-simulator/) for a complete system overview, installation instructions, and API details.
 
+<img width="1546" alt="Architecture" src="https://user-images.githubusercontent.com/748691/235443635-a41fcc3e-b156-4be3-9820-3bcb21329556.png">
+
 ## Installation
 
 Ensure that Python `>=3.9` and `<3.12` is installed. Then, proceed to install LSL:
 
 ```
 # on Linux/WSL
 conda install -c conda-forge liblsl
```

### Comparing `neural_data_simulator-0.2.0/pyproject.toml` & `neural_data_simulator-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neural-data-simulator"
-version = "0.2.0"
+version = "v0.2.2"
 description = "Electrophysiology simulator data for developing Brain-Computer Interfaces"
 authors = ["AE Studio <bci@ae.studio>", "Chadwick Boulay <chadwick.boulay@gmail.com>"]
 maintainers = ["Chadwick Boulay <chadwick.boulay@gmail.com>", "AE Studio <bci@ae.studio>"]
 packages = [
     {include = "neural_data_simulator", from = "src"},
     {include = "decoder", from = "src"},
     {include = "recorder", from = "src"},
```

### Comparing `neural_data_simulator-0.2.0/src/decoder/__init__.py` & `neural_data_simulator-0.2.2/src/decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/decoder/config/settings_decoder.yaml` & `neural_data_simulator-0.2.2/src/decoder/config/settings_decoder.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/decoder/decoders.py` & `neural_data_simulator-0.2.2/src/decoder/decoders.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/decoder/run_decoder.py` & `neural_data_simulator-0.2.2/src/decoder/run_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 from neural_data_simulator.outputs import StreamConfig
 from neural_data_simulator.settings import LogLevel
 from neural_data_simulator.settings import LSLInputModel
 from neural_data_simulator.settings import LSLOutputModel
 from neural_data_simulator.settings import TimerModel
 from neural_data_simulator.util.runtime import configure_logger
 from neural_data_simulator.util.runtime import get_abs_path
+from neural_data_simulator.util.runtime import initialize_logger
 from neural_data_simulator.util.runtime import open_connection
 from neural_data_simulator.util.settings_loader import get_script_settings
 
+SCRIPT_NAME = "nds-decoder"
 logger = logging.getLogger(__name__)
 
 
 class _Settings(VersionedYamlModel):
     """Decoder settings."""
 
     class Decoder(BaseModel):
@@ -110,28 +112,29 @@
     )
 
     return decoder
 
 
 def run():
     """Run the decoder loop."""
+    initialize_logger(SCRIPT_NAME)
     parser = argparse.ArgumentParser(description="Run decoder.")
     parser.add_argument(
         "--settings-path",
         type=Path,
         help="Path to the settings_decoder.yaml file.",
     )
 
     settings = cast(
         _Settings,
         get_script_settings(
             parser.parse_args().settings_path, "settings_decoder.yaml", _Settings
         ),
     )
-    configure_logger("nds-decoder", settings.log_level)
+    configure_logger(SCRIPT_NAME, settings.log_level)
 
     timer_settings = settings.timer
     timer = timing.get_timer(timer_settings.loop_time, timer_settings.max_cpu_buffer)
 
     data_output = _setup_LSL_output(settings.decoder.output)
     lsl_input_settings = settings.decoder.input.lsl
     data_input = _setup_LSL_input(
```

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/__init__.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/config/lsl.config` & `neural_data_simulator-0.2.2/src/neural_data_simulator/config/lsl.config`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/config/settings.yaml` & `neural_data_simulator-0.2.2/src/neural_data_simulator/config/settings.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/config/settings_streamer.yaml` & `neural_data_simulator-0.2.2/src/neural_data_simulator/config/settings_streamer.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/encoder.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/encoder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/ephys_generator.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/ephys_generator.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/filters.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/filters.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/health_checker.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/health_checker.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/inputs.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/inputs.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/models.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/models.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/outputs.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/outputs.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/runner.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/runner.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/samples.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/samples.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/post_install_config.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/post_install_config.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/run_encoder.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,19 @@
 from neural_data_simulator.scripts.errors import InvalidPluginError
 from neural_data_simulator.settings import EncoderEndpointType
 from neural_data_simulator.settings import EncoderSettings
 from neural_data_simulator.settings import LSLOutputModel
 from neural_data_simulator.settings import Settings
 from neural_data_simulator.util.runtime import configure_logger
 from neural_data_simulator.util.runtime import get_abs_path
+from neural_data_simulator.util.runtime import initialize_logger
 from neural_data_simulator.util.runtime import unwrap
 from neural_data_simulator.util.settings_loader import get_script_settings
 
+SCRIPT_NAME = "nds-encoder"
 logger = logging.getLogger(__name__)
 
 
 def _setup_npz_input(
     behavior_file: str, timestamps_array_name: str, data_array_name: str
 ) -> inputs.SamplesInput:
     """Set up the NPZ file input.
@@ -210,27 +212,28 @@
     )
     data_output = LSLOutputDevice(stream_config)
     return data_output
 
 
 def run():
     """Load the configuration and start the encoder."""
+    initialize_logger(SCRIPT_NAME)
     parser = argparse.ArgumentParser(description="Run encoder.")
     parser.add_argument(
         "--settings-path",
         type=Path,
         help="Path to the settings.yaml file.",
     )
     settings = cast(
         Settings,
         get_script_settings(
             parser.parse_args().settings_path, "settings.yaml", Settings
         ),
     )
-    configure_logger("nds-encoder", settings.log_level)
+    configure_logger(SCRIPT_NAME, settings.log_level)
 
     if settings.encoder.input.type == EncoderEndpointType.FILE:
         input_file = unwrap(settings.encoder.input.file)
         data_input = _setup_npz_input(
             input_file.path,
             input_file.timestamps_array_name,
             input_file.data_array_name,
```

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/run_ephys_generator.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_ephys_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,19 @@
 from neural_data_simulator.ephys_generator import Waveforms
 from neural_data_simulator.health_checker import HealthChecker
 from neural_data_simulator.outputs import StreamConfig
 from neural_data_simulator.settings import EphysGeneratorEndpointType
 from neural_data_simulator.settings import EphysGeneratorSettings
 from neural_data_simulator.settings import Settings
 from neural_data_simulator.util.runtime import configure_logger
+from neural_data_simulator.util.runtime import initialize_logger
 from neural_data_simulator.util.runtime import unwrap
 from neural_data_simulator.util.settings_loader import get_script_settings
 
+SCRIPT_NAME = "nds-ephys-generator"
 logger = logging.getLogger(__name__)
 
 
 def _setup_test_input(n_channels: int, n_units_per_channel: int) -> SpikeRateInput:
     """Set up a spike rate input for testing.
 
     The testing input will result in generating spikes from constant
@@ -140,28 +142,29 @@
     if random_seed:
         logger.info(f"Using random seed '{random_seed}'")
         np.random.seed(random_seed)
 
 
 def run():
     """Load the configuration and start the ephys generator."""
+    initialize_logger(SCRIPT_NAME)
     parser = argparse.ArgumentParser(description="Run ephys generator.")
     parser.add_argument(
         "--settings-path",
         type=Path,
         help="Path to the settings.yaml file.",
     )
     settings = cast(
         Settings,
         get_script_settings(
             parser.parse_args().settings_path, "settings.yaml", Settings
         ),
     )
     _set_random_seed(settings.ephys_generator.random_seed)
-    configure_logger("nds-ephys-generator", settings.log_level)
+    configure_logger(SCRIPT_NAME, settings.log_level)
 
     if settings.ephys_generator.input.type == EphysGeneratorEndpointType.LSL:
         lsl_input_settings = unwrap(settings.ephys_generator.input.lsl)
         spike_rate_input = _setup_LSL_input(
             lsl_input_settings.stream_name, lsl_input_settings.connection_timeout
         )
         spike_rate_input.connect()
```

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/run_streamer.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_streamer.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,19 @@
 from neural_data_simulator.outputs import StreamConfig
 from neural_data_simulator.samples import Samples
 from neural_data_simulator.settings import LogLevel
 from neural_data_simulator.settings import LSLChannelFormatType
 from neural_data_simulator.settings import LSLOutputModel
 from neural_data_simulator.util.runtime import configure_logger
 from neural_data_simulator.util.runtime import get_abs_path
+from neural_data_simulator.util.runtime import initialize_logger
 from neural_data_simulator.util.runtime import unwrap
 from neural_data_simulator.util.settings_loader import get_script_settings
 
+SCRIPT_NAME = "nds-streamer"
 logger = logging.getLogger(__name__)
 
 
 class StreamerInputType(YamlStrEnum):
     """Possible types for the streamer input."""
 
     NPZ = "npz"
@@ -280,27 +282,28 @@
         channel_labels=["ch_id", "unit_id"] + wf_ch_labels,
     )
     return stream_config
 
 
 def run():
     """Load the configuration and start the streamer."""
+    initialize_logger(SCRIPT_NAME)
     parser = argparse.ArgumentParser(description="Run streamer.")
     parser.add_argument(
         "--settings-path",
         type=Path,
         help="Path to the settings_streamer.yaml file.",
     )
     settings = cast(
         _Settings,
         get_script_settings(
             parser.parse_args().settings_path, "settings_streamer.yaml", _Settings
         ),
     )
-    configure_logger("nds-streamer", settings.log_level)
+    configure_logger(SCRIPT_NAME, settings.log_level)
 
     if settings.streamer.input_type == StreamerInputType.NPZ.value:
         input_settings = unwrap(settings.streamer.npz).input
         samples = [
             Samples.load_from_npz(
                 get_abs_path(input_settings.file),
                 timestamps_array_name=input_settings.timestamps_array_name,
```

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/settings.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/settings.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/streamers.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/streamers.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/timing.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/timing.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/util/buffer.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/util/buffer.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/util/circular_dequeue.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/util/circular_dequeue.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/util/runtime.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/util/runtime.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,60 @@
 """Functions commonly used by scripts."""
 import contextlib
 import logging
+from logging.handlers import MemoryHandler
 import os
 from pathlib import Path
+import sys
 from typing import Any, Optional, Union
 
 from neural_data_simulator.inputs import Input
 from neural_data_simulator.outputs import Output
 from neural_data_simulator.settings import LogLevel
 
 logger = logging.getLogger(__name__)
 
 NDS_HOME = os.path.join(os.path.expanduser("~"), ".nds")
 
 
+def initialize_logger(script_name: str):
+    """Initialize the logger.
+
+    Store log messages in memory until the logger is configured.
+    """
+    root_logger = logging.getLogger()
+    root_logger.setLevel(logging.NOTSET)
+    handler = logging.StreamHandler(sys.stderr)
+    handler.setFormatter(logging.Formatter(_get_log_message_format(script_name)))
+    temp_handler = MemoryHandler(1000, target=handler)
+    root_logger.addHandler(temp_handler)
+
+
 def configure_logger(script_name: str, log_level: LogLevel):
     """Set up the logger."""
+    root_logger = logging.getLogger()
+    for handler in root_logger.handlers:
+        if isinstance(handler, MemoryHandler):
+            level = logging._nameToLevel[log_level.value.upper()]
+            filtered_buffer = filter(
+                lambda record: record.levelno >= level, handler.buffer
+            )
+            handler.buffer = list(filtered_buffer)
+            break
+
     logging.basicConfig(
-        format=f"%(levelname)s [{script_name}]: %(message)s", level=log_level.value
+        format=_get_log_message_format(script_name), level=log_level.value, force=True
     )
     os.environ["LSLAPICFG"] = os.path.join(NDS_HOME, "lsl.config")
 
 
+def _get_log_message_format(script_name: str):
+    return f"%(levelname)s [{script_name}]: %(message)s"
+
+
 def get_abs_path(
     abs_or_relative_path: Union[str, Path], relative_to: str = os.getcwd()
 ) -> str:
     """Return the absolute path for a resource.
 
     If an absolute path is passed as the first parameter then
     this is returned unchanged and the second parameter is ignored.
```

### Comparing `neural_data_simulator-0.2.0/src/neural_data_simulator/util/settings_loader.py` & `neural_data_simulator-0.2.2/src/neural_data_simulator/util/settings_loader.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/plugins/examples/gamepad_preprocessor.py` & `neural_data_simulator-0.2.2/src/plugins/examples/gamepad_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/plugins/examples/model.py` & `neural_data_simulator-0.2.2/src/plugins/examples/model.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/plugins/examples/postprocessor.py` & `neural_data_simulator-0.2.2/src/plugins/examples/postprocessor.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/plugins/examples/tests/test_model.py` & `neural_data_simulator-0.2.2/src/plugins/examples/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/recorder/run_recorder.py` & `neural_data_simulator-0.2.2/src/recorder/run_recorder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/tasks/center_out_reach/__init__.py` & `neural_data_simulator-0.2.2/src/tasks/center_out_reach/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/tasks/center_out_reach/buttons.py` & `neural_data_simulator-0.2.2/src/tasks/center_out_reach/buttons.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/tasks/center_out_reach/input_events.py` & `neural_data_simulator-0.2.2/src/tasks/center_out_reach/input_events.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,19 @@
     """Listeners for input event handling."""
 
     def __init__(self):
         """Create a new instance."""
         self.event_handlers = dict()
         self.joystick_input = JoystickInput()
 
+    @property
+    def input_device_name(self):
+        """Get the name of the input device."""
+        return "joystick" if self.joystick_input.joystick else "mouse"
+
     def set_handler_for_event(self, event: InputEvent, handler: Callable):
         """Set a function as a handler for a specific input event."""
         self.event_handlers[event] = handler
 
     def get_cursor_relative_position(self) -> Tuple[int, int]:
         """Get the relative position of the joystick or mouse cursor.
```

### Comparing `neural_data_simulator-0.2.0/src/tasks/center_out_reach/joystick.py` & `neural_data_simulator-0.2.2/src/tasks/center_out_reach/joystick.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/tasks/center_out_reach/metrics.py` & `neural_data_simulator-0.2.2/src/tasks/center_out_reach/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import math
 from typing import List, Tuple
 
 import matplotlib.colors as mcolors
 import matplotlib.pyplot as plt
 from numpy import ndarray
 import numpy as np
+import pygame
 from scipy import signal
 from sklearn.metrics import r2_score
 from tasks.center_out_reach.scalers import PixelsToMetersConverter
 
 
 class MetricsCollector:
     """Collect and plot velocities resulted from running the task."""
@@ -228,14 +229,15 @@
 
     def plot_metrics(self, targets):
         """Show velocities plot and R-values.
 
         Args:
             targets: List of target positions in pixels.
         """
+        pygame.display.init()
         h_lag = self._get_lag(
             self.actual_velocities[:, 0], self.decoded_velocities[:, 0]
         )
 
         actual_velocities = self.actual_velocities[:, :]
         actual_velocities_timestamps = np.array(self.actual_velocities_timestamps)[:]
         actual_velocities_timestamps = (
```

### Comparing `neural_data_simulator-0.2.0/src/tasks/center_out_reach/scalers.py` & `neural_data_simulator-0.2.2/src/tasks/center_out_reach/scalers.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/tasks/center_out_reach/screen_info.py` & `neural_data_simulator-0.2.2/src/tasks/center_out_reach/screen_info.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/tasks/center_out_reach/sprites.py` & `neural_data_simulator-0.2.2/src/tasks/center_out_reach/sprites.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_runner.py` & `neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,21 +105,21 @@
                 Samples(timestamps=timestamps, data=velocities)
             )
 
     def stop(self):
         """Signal the loop that it should stop."""
         self.should_stop_loop = True
 
-    def run(self, task_state: TaskState):
+    def run(self, task_state: TaskState, user_input: InputHandler):
         """Start the loop.
 
         Args:
             task_state: The state machine that should be updated by the loop.
+            user_input: The user input controller for actual cursor.
         """
-        user_input = InputHandler()
         task_window = task_state.task_window
 
         user_input.set_handler_for_event(InputEvent.EXIT, self.stop)
         user_input.set_handler_for_event(InputEvent.RESET, task_window.reset_cursor)
         user_input.set_handler_for_event(
             InputEvent.TOGGLE_CURSOR, task_window.toggle_actual_cursor
         )
@@ -166,7 +166,8 @@
                 else:
                     task_window.show_hint(None)
 
             # Make the GUI think that it's running at twice the frame rate.
             # The rest of the time we use our precise timer to wait so that
             # we can output at exactly sample_rate with as little jitter as possible
             task_window.tick(self.sample_rate * 2)
+        task_window.stop_task()
```

### Comparing `neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_state.py` & `neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_state.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_window.py` & `neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,23 @@
         self._grab_and_hide_cursor()
         self.show_hint(None)
 
     def _grab_and_hide_cursor(self):
         pygame.mouse.set_visible(False)
         pygame.event.set_grab(True)
 
+    def _release_and_show_cursor(self):
+        pygame.mouse.set_visible(True)
+        pygame.event.set_grab(False)
+
+    def stop_task(self):
+        """Stop the task."""
+        self._release_and_show_cursor()
+        pygame.display.quit()
+
     def _set_window_size_background_and_title(self) -> pygame.surface.Surface:
         screen = pygame.display.set_mode(self.window_size)
         screen.fill(self.params.background_color)
         pygame.display.set_caption("NDS Center-out reach")
         pygame.display.flip()
         return screen
```

### Comparing `neural_data_simulator-0.2.0/src/tasks/config/settings_center_out_reach.yaml` & `neural_data_simulator-0.2.2/src/tasks/config/settings_center_out_reach.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.0/src/tasks/run_center_out_reach.py` & `neural_data_simulator-0.2.2/src/tasks/run_center_out_reach.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 from typing import cast, Optional, Tuple
 
 import numpy as np
 from pydantic import BaseModel
 from pydantic import validator
 from pydantic_yaml import VersionedYamlModel
+from tasks.center_out_reach.input_events import InputHandler
 from tasks.center_out_reach.metrics import MetricsCollector
 from tasks.center_out_reach.scalers import PixelsToMetersConverter
 from tasks.center_out_reach.scalers import StandardVelocityScaler
 from tasks.center_out_reach.task_runner import TaskRunner
 from tasks.center_out_reach.task_state import StateParams
 from tasks.center_out_reach.task_state import TaskState
 from tasks.center_out_reach.task_window import TaskWindow
@@ -20,18 +21,20 @@
 from neural_data_simulator import inputs
 from neural_data_simulator import outputs
 from neural_data_simulator.outputs import StreamConfig
 from neural_data_simulator.settings import LogLevel
 from neural_data_simulator.settings import LSLInputModel
 from neural_data_simulator.settings import LSLOutputModel
 from neural_data_simulator.util.runtime import configure_logger
+from neural_data_simulator.util.runtime import initialize_logger
 from neural_data_simulator.util.runtime import open_connection
 from neural_data_simulator.util.runtime import unwrap
 from neural_data_simulator.util.settings_loader import get_script_settings
 
+SCRIPT_NAME = "nds-center-out-reach"
 logger = logging.getLogger(__name__)
 
 
 class _Settings(VersionedYamlModel):
     """Center-out reach settings."""
 
     class CenterOutReach(BaseModel):
@@ -196,40 +199,44 @@
             hint.append({"color": rich_text[1], "text": rich_text[0]})
         else:
             hint.append({"color": default_text_color, "text": part})
     return hint
 
 
 def _get_menu_text(
-    default_text_color, actual_cursor_color, decoded_cursor_color, target_color
+    default_text_color,
+    actual_cursor_color,
+    decoded_cursor_color,
+    target_color,
+    input_device,
 ):
     text = (
         f"\nWelcome to the Center Out Reaching Task!\n\n"
         f"Press the <Start> button to begin.\n\n"
         f"Two cursors will be presented: the [input cursor]({actual_cursor_color})"
-        f" that\n directly follows your mouse movements (and can be toggled\n"
+        f" that\n directly follows your {input_device} movements (and can be toggled\n"
         f" on and off by pressing `c` on the keyboard), and the\n"
         f" [decoded cursor]({decoded_cursor_color}) that is the decoded from the"
         f" simulated\n spikes from the [input cursor]({actual_cursor_color})"
         f" movement.\n\nYour goal is to reach and stay within the"
         f" [target]({target_color}) using the\n"
         f" [decoded cursor]({decoded_cursor_color})"
         f" until the next [target]({target_color}) is presented.\n"
         f"There is no time or target limit, you can press the\n"
         f" `Escape` key to finish the task at any time.\n"
     )
     return _parse_rich_text(text, default_text_color)
 
 
-def _get_training_text(default_text_color, target_color):
+def _get_training_text(default_text_color, target_color, input_device):
     text = (
         f"\nWelcome to the Center Out Reaching Task!\n\n"
         f"Press the <Start> button to begin.\n\n"
         f"In open loop mode, the cursor follows your\n"
-        f"mouse movements.\n\nYour goal is to reach and stay within the"
+        f"{input_device} movements.\n\nYour goal is to reach and stay within the"
         f" [target]({target_color}) using the\n"
         f" cursor"
         f" until the next [target]({target_color}) is presented.\n\n"
         f"There is no time or target limit, you can press the\n"
         f" `Escape` key to finish the task at any time.\n"
     )
     return _parse_rich_text(text, default_text_color)
@@ -240,14 +247,15 @@
         settings.center_out_reach.input.enabled
         and settings.center_out_reach.with_metrics
     )
 
 
 def run():
     """Run the center-out reach task GUI."""
+    initialize_logger(SCRIPT_NAME)
     parser = argparse.ArgumentParser(description="Run GUI.")
     parser.add_argument(
         "--settings-path",
         type=Path,
         help="Path to the settings_center_out_reach.yaml file.",
     )
 
@@ -255,15 +263,15 @@
         _Settings,
         get_script_settings(
             parser.parse_args().settings_path,
             "settings_center_out_reach.yaml",
             _Settings,
         ),
     )
-    configure_logger("nds-center-out-reach", settings.log_level)
+    configure_logger(SCRIPT_NAME, settings.log_level)
 
     if settings.center_out_reach.input.enabled:
         lsl_input_settings = unwrap(settings.center_out_reach.input.lsl)
         data_input = _setup_LSL_input(
             lsl_input_settings.stream_name, lsl_input_settings.connection_timeout
         )
     else:
@@ -309,39 +317,41 @@
             actual_cursor_color,
             decoded_cursor_color,
         )
     else:
         metrics_collector = None
 
     with_decoded_cursor = settings.center_out_reach.input.enabled
+
+    user_input = InputHandler()
     if with_decoded_cursor:
         menu_text = _get_menu_text(
             "black",
             actual_cursor_color,
             decoded_cursor_color,
             window_settings.colors.target,
+            user_input.input_device_name,
         )
     else:
         menu_text = _get_training_text(
-            "black",
-            window_settings.colors.target,
+            "black", window_settings.colors.target, user_input.input_device_name
         )
 
     with open_connection(data_output), open_connection(data_input):
         task_window = TaskWindow(window_rect, window_params, menu_text)
         task_state = TaskState(task_window, state_params)
         task_runner = TaskRunner(
             sampling_rate,
             data_input,
             data_output,
             velocity_scaler,
             with_decoded_cursor,
             metrics_collector,
         )
-        task_runner.run(task_state)
+        task_runner.run(task_state, user_input)
 
         if not task_window.show_menu_screen and _metrics_enabled(settings):
             unwrap(metrics_collector).plot_metrics(task_window.target_positions)
 
         task_window.leave()
```

### Comparing `neural_data_simulator-0.2.0/PKG-INFO` & `neural_data_simulator-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-data-simulator
-Version: 0.2.0
+Version: 0.2.2
 Summary: Electrophysiology simulator data for developing Brain-Computer Interfaces
 License: Apache-2.0
 Author: AE Studio
 Author-email: bci@ae.studio
 Maintainer: Chadwick Boulay
 Maintainer-email: chadwick.boulay@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -44,14 +44,16 @@
 
 The Neural Data Simulator is a real-time system for generating electrophysiology data from behavioral data (e.g. cursor movement, arm kinematics, etc) in real-time. The NDS system can be used to test and validate closed-loop brain-computer interface systems without the need for a human in the loop, generate synthetic data for algorithm optimization, and provide a platform on which to develop BCI decoders.
 
 ## Documentation
 
 See the [documentation](https://agencyenterprise.github.io/neural-data-simulator/) for a complete system overview, installation instructions, and API details.
 
+<img width="1546" alt="Architecture" src="https://user-images.githubusercontent.com/748691/235443635-a41fcc3e-b156-4be3-9820-3bcb21329556.png">
+
 ## Installation
 
 Ensure that Python `>=3.9` and `<3.12` is installed. Then, proceed to install LSL:
 
 ```
 # on Linux/WSL
 conda install -c conda-forge liblsl
```

