# Comparing `tmp/faster-whisper-0.6.0.tar.gz` & `tmp/faster-whisper-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster-whisper-0.6.0.tar", last modified: Wed May 24 14:17:09 2023, max compression
+gzip compressed data, was "faster-whisper-0.7.0.tar", last modified: Tue Jul 18 13:25:41 2023, max compression
```

## Comparing `faster-whisper-0.6.0.tar` & `faster-whisper-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:17:09.528253 faster-whisper-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-24 14:17:09.528253 faster-whisper-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:17:09.524253 faster-whisper-0.6.0/faster_whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:17:09.524253 faster-whisper-0.6.0/faster_whisper/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  1807524 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/assets/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    33826 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/transcribe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/vad.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:17:09.524253 faster-whisper-0.6.0/faster_whisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-24 14:17:09.000000 faster-whisper-0.6.0/faster_whisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-24 14:17:09.000000 faster-whisper-0.6.0/faster_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:17:09.000000 faster-whisper-0.6.0/faster_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-24 14:17:09.000000 faster-whisper-0.6.0/faster_whisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 14:17:09.000000 faster-whisper-0.6.0/faster_whisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/requirements.conversion.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-24 14:17:09.528253 faster-whisper-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:25:41.022580 faster-whisper-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-18 13:25:41.022580 faster-whisper-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:25:41.018580 faster-whisper-0.7.0/faster_whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:25:41.022580 faster-whisper-0.7.0/faster_whisper/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  1807524 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/assets/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36931 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/transcribe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/vad.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:25:41.022580 faster-whisper-0.7.0/faster_whisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-18 13:25:40.000000 faster-whisper-0.7.0/faster_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-18 13:25:41.000000 faster-whisper-0.7.0/faster_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:25:40.000000 faster-whisper-0.7.0/faster_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-18 13:25:40.000000 faster-whisper-0.7.0/faster_whisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 13:25:40.000000 faster-whisper-0.7.0/faster_whisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/requirements.conversion.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-18 13:25:41.022580 faster-whisper-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/setup.py
```

### Comparing `faster-whisper-0.6.0/LICENSE` & `faster-whisper-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.6.0/PKG-INFO` & `faster-whisper-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 0.6.0
+Version: 0.7.0
 Summary: Faster Whisper transcription with CTranslate2
 Home-page: https://github.com/guillaumekln/faster-whisper
 Author: Guillaume Klein
 License: MIT
 Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
@@ -112,15 +112,19 @@
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True)
         ```
         
         The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
         
         ```python
-        segments, _ = model.transcribe("audio.mp3", vad_filter=True, vad_parameters=dict(min_silence_duration_ms=500))
+        segments, _ = model.transcribe(
+            "audio.mp3",
+            vad_filter=True,
+            vad_parameters=dict(min_silence_duration_ms=500),
+        )
         ```
         
         ### Logging
         
         The library logging level can be configured like this:
         
         ```python
@@ -137,14 +141,16 @@
         ## Community integrations
         
         Here is a non exhaustive list of open-source projects using faster-whisper. Feel free to add your project to the list!
         
         * [whisper-ctranslate2](https://github.com/Softcatala/whisper-ctranslate2) is a command line client based on faster-whisper and compatible with the original client from openai/whisper.
         * [whisper-diarize](https://github.com/MahmoudAshraf97/whisper-diarization) is a speaker diarization tool that is based on faster-whisper and NVIDIA NeMo.
         * [whisper-standalone-win](https://github.com/Purfview/whisper-standalone-win) contains the portable ready to run binaries of faster-whisper for Windows.
+        * [asr-sd-pipeline](https://github.com/hedrergudene/asr-sd-pipeline) provides a scalable, modular, end to end multi-speaker speech to text solution implemented using AzureML pipelines.
+        * [Open-Lyrics](https://github.com/zh-plus/Open-Lyrics) is a Python library that transcribes voice files using faster-whisper, and translates/polishes the resulting text into `.lrc` files in the desired language using OpenAI-GPT.
         
         ## Model conversion
         
         When loading a model from its size such as `WhisperModel("large-v2")`, the correspondig CTranslate2 model is automatically downloaded from the [Hugging Face Hub](https://huggingface.co/guillaumekln).
         
         We also provide a script to convert any Whisper models compatible with the Transformers library. They could be the original OpenAI models or user fine-tuned models.
         
@@ -158,14 +164,26 @@
         ```
         
         * The option `--model` accepts a model name on the Hub or a path to a model directory.
         * If the option `--copy_files tokenizer.json` is not used, the tokenizer configuration is automatically downloaded when the model is loaded later.
         
         Models can also be converted from the code. See the [conversion API](https://opennmt.net/CTranslate2/python/ctranslate2.converters.TransformersConverter.html).
         
+        ### Load a converted model
+        
+        1. Directly load the model from a local directory:
+        ```python
+        model = faster_whisper.WhisperModel("whisper-large-v2-ct2")
+        ```
+        
+        2. [Upload your model to the Hugging Face Hub](https://huggingface.co/docs/transformers/model_sharing#upload-with-the-web-interface) and load it from its name:
+        ```python
+        model = faster_whisper.WhisperModel("username/whisper-large-v2-ct2")
+        ```
+        
         ## Comparing performance against other implementations
         
         If you are comparing the performance against other Whisper implementations, you should make sure to run the comparison with similar settings. In particular:
         
         * Verify that the same transcription options are used, especially the same beam size. For example in openai/whisper, `model.transcribe` uses a default beam size of 1 but here we use a default beam size of 5.
         * When running on CPU, make sure to set the same number of threads. Many frameworks will read the environment variable `OMP_NUM_THREADS`, which can be set when running your script:
```

### Comparing `faster-whisper-0.6.0/README.md` & `faster-whisper-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -105,15 +105,19 @@
 ```python
 segments, _ = model.transcribe("audio.mp3", vad_filter=True)
 ```
 
 The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
 
 ```python
-segments, _ = model.transcribe("audio.mp3", vad_filter=True, vad_parameters=dict(min_silence_duration_ms=500))
+segments, _ = model.transcribe(
+    "audio.mp3",
+    vad_filter=True,
+    vad_parameters=dict(min_silence_duration_ms=500),
+)
 ```
 
 ### Logging
 
 The library logging level can be configured like this:
 
 ```python
@@ -130,14 +134,16 @@
 ## Community integrations
 
 Here is a non exhaustive list of open-source projects using faster-whisper. Feel free to add your project to the list!
 
 * [whisper-ctranslate2](https://github.com/Softcatala/whisper-ctranslate2) is a command line client based on faster-whisper and compatible with the original client from openai/whisper.
 * [whisper-diarize](https://github.com/MahmoudAshraf97/whisper-diarization) is a speaker diarization tool that is based on faster-whisper and NVIDIA NeMo.
 * [whisper-standalone-win](https://github.com/Purfview/whisper-standalone-win) contains the portable ready to run binaries of faster-whisper for Windows.
+* [asr-sd-pipeline](https://github.com/hedrergudene/asr-sd-pipeline) provides a scalable, modular, end to end multi-speaker speech to text solution implemented using AzureML pipelines.
+* [Open-Lyrics](https://github.com/zh-plus/Open-Lyrics) is a Python library that transcribes voice files using faster-whisper, and translates/polishes the resulting text into `.lrc` files in the desired language using OpenAI-GPT.
 
 ## Model conversion
 
 When loading a model from its size such as `WhisperModel("large-v2")`, the correspondig CTranslate2 model is automatically downloaded from the [Hugging Face Hub](https://huggingface.co/guillaumekln).
 
 We also provide a script to convert any Whisper models compatible with the Transformers library. They could be the original OpenAI models or user fine-tuned models.
 
@@ -151,14 +157,26 @@
 ```
 
 * The option `--model` accepts a model name on the Hub or a path to a model directory.
 * If the option `--copy_files tokenizer.json` is not used, the tokenizer configuration is automatically downloaded when the model is loaded later.
 
 Models can also be converted from the code. See the [conversion API](https://opennmt.net/CTranslate2/python/ctranslate2.converters.TransformersConverter.html).
 
+### Load a converted model
+
+1. Directly load the model from a local directory:
+```python
+model = faster_whisper.WhisperModel("whisper-large-v2-ct2")
+```
+
+2. [Upload your model to the Hugging Face Hub](https://huggingface.co/docs/transformers/model_sharing#upload-with-the-web-interface) and load it from its name:
+```python
+model = faster_whisper.WhisperModel("username/whisper-large-v2-ct2")
+```
+
 ## Comparing performance against other implementations
 
 If you are comparing the performance against other Whisper implementations, you should make sure to run the comparison with similar settings. In particular:
 
 * Verify that the same transcription options are used, especially the same beam size. For example in openai/whisper, `model.transcribe` uses a default beam size of 1 but here we use a default beam size of 5.
 * When running on CPU, make sure to set the same number of threads. Many frameworks will read the environment variable `OMP_NUM_THREADS`, which can be set when running your script:
```

### Comparing `faster-whisper-0.6.0/faster_whisper/assets/silero_vad.onnx` & `faster-whisper-0.7.0/faster_whisper/assets/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.6.0/faster_whisper/audio.py` & `faster-whisper-0.7.0/faster_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.6.0/faster_whisper/feature_extractor.py` & `faster-whisper-0.7.0/faster_whisper/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.6.0/faster_whisper/tokenizer.py` & `faster-whisper-0.7.0/faster_whisper/tokenizer.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.6.0/faster_whisper/transcribe.py` & `faster-whisper-0.7.0/faster_whisper/transcribe.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     patience: float
     length_penalty: float
     log_prob_threshold: Optional[float]
     no_speech_threshold: Optional[float]
     compression_ratio_threshold: Optional[float]
     condition_on_previous_text: bool
     temperatures: List[float]
-    initial_prompt: Optional[str]
+    initial_prompt: Optional[Union[str, Iterable[int]]]
     prefix: Optional[str]
     suppress_blank: bool
     suppress_tokens: Optional[List[int]]
     without_timestamps: bool
     max_initial_timestamp: float
     word_timestamps: bool
     prepend_punctuations: str
@@ -84,16 +84,17 @@
         download_root: Optional[str] = None,
         local_files_only: bool = False,
     ):
         """Initializes the Whisper model.
 
         Args:
           model_size_or_path: Size of the model to use (tiny, tiny.en, base, base.en,
-            small, small.en, medium, medium.en, large-v1, or large-v2) or a path to a converted
-            model directory. When a size is configured, the converted model is downloaded
+            small, small.en, medium, medium.en, large-v1, or large-v2), a path to a converted
+            model directory, or a CTranslate2-converted Whisper model ID from the Hugging Face Hub.
+            When a size or a model ID is configured, the converted model is downloaded
             from the Hugging Face Hub.
           device: Device to use for computation ("cpu", "cuda", "auto").
           device_index: Device ID to use.
             The model can also be loaded on multiple GPUs by passing a list of IDs
             (e.g. [0, 1, 2, 3]). In that case, multiple transcriptions can run in parallel
             when transcribe() is called from multiple Python threads (see also num_workers).
           compute_type: Type to use for computation.
@@ -166,15 +167,15 @@
             0.8,
             1.0,
         ],
         compression_ratio_threshold: Optional[float] = 2.4,
         log_prob_threshold: Optional[float] = -1.0,
         no_speech_threshold: Optional[float] = 0.6,
         condition_on_previous_text: bool = True,
-        initial_prompt: Optional[str] = None,
+        initial_prompt: Optional[Union[str, Iterable[int]]] = None,
         prefix: Optional[str] = None,
         suppress_blank: bool = True,
         suppress_tokens: Optional[List[int]] = [-1],
         without_timestamps: bool = False,
         max_initial_timestamp: float = 1.0,
         word_timestamps: bool = False,
         prepend_punctuations: str = "\"'“¿([{-",
@@ -204,15 +205,16 @@
           no_speech_threshold: If the no_speech probability is higher than this value AND
             the average log probability over sampled tokens is below `log_prob_threshold`,
             consider the segment as silent.
           condition_on_previous_text: If True, the previous output of the model is provided
             as a prompt for the next window; disabling may make the text inconsistent across
             windows, but the model becomes less prone to getting stuck in a failure loop,
             such as repetition looping or timestamps going out of sync.
-          initial_prompt: Optional text to provide as a prompt for the first window.
+          initial_prompt: Optional text string or iterable of token ids to provide as a
+            prompt for the first window.
           prefix: Optional text to provide as a prefix for the first window.
           suppress_blank: Suppress blank outputs at the beginning of the sampling.
           suppress_tokens: List of token IDs to suppress. -1 will suppress a default set
             of symbols as defined in the model config.json file.
           without_timestamps: Only sample text tokens.
           max_initial_timestamp: The initial timestamp cannot be later than this.
           word_timestamps: Extract word-level timestamps using the cross-attention pattern
@@ -357,18 +359,22 @@
         content_frames = features.shape[-1] - self.feature_extractor.nb_max_frames
         idx = 0
         seek = 0
         all_tokens = []
         prompt_reset_since = 0
 
         if options.initial_prompt is not None:
-            initial_prompt = " " + options.initial_prompt.strip()
-            initial_prompt_tokens = tokenizer.encode(initial_prompt)
-            all_tokens.extend(initial_prompt_tokens)
+            if isinstance(options.initial_prompt, str):
+                initial_prompt = " " + options.initial_prompt.strip()
+                initial_prompt_tokens = tokenizer.encode(initial_prompt)
+                all_tokens.extend(initial_prompt_tokens)
+            else:
+                all_tokens.extend(options.initial_prompt)
 
+        last_speech_timestamp = 0.0
         while seek < content_frames:
             time_offset = seek * self.feature_extractor.time_per_frame
             segment = features[:, seek : seek + self.feature_extractor.nb_max_frames]
             segment_size = min(
                 self.feature_extractor.nb_max_frames, content_frames - seek
             )
             segment_duration = segment_size * self.feature_extractor.time_per_frame
@@ -502,20 +508,22 @@
                 self.add_word_timestamps(
                     current_segments,
                     tokenizer,
                     encoder_output,
                     segment_size,
                     options.prepend_punctuations,
                     options.append_punctuations,
+                    last_speech_timestamp=last_speech_timestamp,
                 )
 
                 word_end_timestamps = [
                     w["end"] for s in current_segments for w in s["words"]
                 ]
-
+                if len(word_end_timestamps) > 0:
+                    last_speech_timestamp = word_end_timestamps[-1]
                 if not single_timestamp_ending and len(word_end_timestamps) > 0:
                     seek_shift = round(
                         (word_end_timestamps[-1] - time_offset) * self.frames_per_second
                     )
 
                     if seek_shift > 0:
                         seek = previous_seek + seek_shift
@@ -641,14 +649,20 @@
                 self.logger.debug(
                     "Log probability threshold is not met with temperature %.1f (%f < %f)",
                     temperature,
                     avg_logprob,
                     options.log_prob_threshold,
                 )
 
+            if (
+                options.no_speech_threshold is not None
+                and result.no_speech_prob > options.no_speech_threshold
+            ):
+                needs_fallback = False  # silence
+
             if not needs_fallback:
                 break
 
         return result, avg_logprob, final_temperature, compression_ratio
 
     def get_prompt(
         self,
@@ -668,39 +682,62 @@
         if without_timestamps:
             prompt.append(tokenizer.no_timestamps)
 
         if prefix:
             prefix_tokens = tokenizer.encode(" " + prefix.strip())
             if len(prefix_tokens) >= self.max_length // 2:
                 prefix_tokens = prefix_tokens[: self.max_length // 2 - 1]
+            if not without_timestamps:
+                prompt.append(tokenizer.timestamp_begin)
             prompt.extend(prefix_tokens)
 
         return prompt
 
     def add_word_timestamps(
         self,
         segments: List[dict],
         tokenizer: Tokenizer,
         encoder_output: ctranslate2.StorageView,
         num_frames: int,
         prepend_punctuations: str,
         append_punctuations: str,
+        last_speech_timestamp: float,
     ):
         if len(segments) == 0:
             return
 
         text_tokens_per_segment = [
             [token for token in segment["tokens"] if token < tokenizer.eot]
             for segment in segments
         ]
 
         text_tokens = list(itertools.chain.from_iterable(text_tokens_per_segment))
         alignment = self.find_alignment(
             tokenizer, text_tokens, encoder_output, num_frames
         )
+        word_durations = np.array([word["end"] - word["start"] for word in alignment])
+        word_durations = word_durations[word_durations.nonzero()]
+        median_duration = np.median(word_durations) if len(word_durations) > 0 else 0.0
+        max_duration = median_duration * 2
+
+        # hack: truncate long words at sentence boundaries.
+        # a better segmentation algorithm based on VAD should be able to replace this.
+        if len(word_durations) > 0:
+            median_duration = np.median(word_durations)
+            max_duration = median_duration * 2
+            sentence_end_marks = ".。!！?？"
+            # ensure words at sentence boundaries
+            # are not longer than twice the median word duration.
+            for i in range(1, len(alignment)):
+                if alignment[i]["end"] - alignment[i]["start"] > max_duration:
+                    if alignment[i]["word"] in sentence_end_marks:
+                        alignment[i]["end"] = alignment[i]["start"] + max_duration
+                    elif alignment[i - 1]["word"] in sentence_end_marks:
+                        alignment[i]["start"] = alignment[i]["end"] - max_duration
+
         merge_punctuations(alignment, prepend_punctuations, append_punctuations)
 
         time_offset = (
             segments[0]["seek"]
             * self.feature_extractor.hop_length
             / self.feature_extractor.sampling_rate
         )
@@ -723,18 +760,59 @@
                             probability=timing["probability"],
                         )
                     )
 
                 saved_tokens += len(timing["tokens"])
                 word_index += 1
 
+            # hack: truncate long words at segment boundaries.
+            # a better segmentation algorithm based on VAD should be able to replace this.
             if len(words) > 0:
-                # adjust the segment-level timestamps based on the word-level timestamps
-                segment["start"] = words[0]["start"]
-                segment["end"] = words[-1]["end"]
+                # ensure the first and second word after a pause is not longer than
+                # twice the median word duration.
+                if words[0]["end"] - last_speech_timestamp > median_duration * 4 and (
+                    words[0]["end"] - words[0]["start"] > max_duration
+                    or (
+                        len(words) > 1
+                        and words[1]["end"] - words[0]["start"] > max_duration * 2
+                    )
+                ):
+                    if (
+                        len(words) > 1
+                        and words[1]["end"] - words[1]["start"] > max_duration
+                    ):
+                        boundary = max(
+                            words[1]["end"] / 2, words[1]["end"] - max_duration
+                        )
+                        words[0]["end"] = words[1]["start"] = boundary
+                    words[0]["start"] = max(0, words[0]["end"] - max_duration)
+
+                # prefer the segment-level start timestamp if the first word is too long.
+                if (
+                    segment["start"] < words[0]["end"]
+                    and segment["start"] - 0.5 > words[0]["start"]
+                ):
+                    words[0]["start"] = max(
+                        0, min(words[0]["end"] - median_duration, segment["start"])
+                    )
+                else:
+                    segment["start"] = words[0]["start"]
+
+                # prefer the segment-level end timestamp if the last word is too long.
+                if (
+                    segment["end"] > words[-1]["start"]
+                    and segment["end"] + 0.5 < words[-1]["end"]
+                ):
+                    words[-1]["end"] = max(
+                        words[-1]["start"] + median_duration, segment["end"]
+                    )
+                else:
+                    segment["end"] = words[-1]["end"]
+
+                last_speech_timestamp = segment["end"]
 
             segment["words"] = words
 
     def find_alignment(
         self,
         tokenizer: Tokenizer,
         text_tokens: List[int],
@@ -771,30 +849,14 @@
         start_times = jump_times[word_boundaries[:-1]]
         end_times = jump_times[word_boundaries[1:]]
         word_probabilities = [
             np.mean(text_token_probs[i:j])
             for i, j in zip(word_boundaries[:-1], word_boundaries[1:])
         ]
 
-        # hack: ensure the first and second word is not longer than twice the median word duration.
-        # a better segmentation algorithm based on VAD should be able to replace this.
-        word_durations = end_times - start_times
-        word_durations = word_durations[word_durations.nonzero()]
-        if len(word_durations) > 0:
-            median_duration = np.median(word_durations)
-            max_duration = median_duration * 2
-            if len(word_durations) >= 2 and word_durations[1] > max_duration:
-                boundary = max(end_times[2] / 2, end_times[2] - max_duration)
-                end_times[0] = start_times[1] = boundary
-            if (
-                len(word_durations) >= 1
-                and end_times[0] - start_times[0] > max_duration
-            ):
-                start_times[0] = max(0, end_times[0] - max_duration)
-
         return [
             dict(
                 word=word, tokens=tokens, start=start, end=end, probability=probability
             )
             for word, tokens, start, end, probability in zip(
                 words, word_tokens, start_times, end_times, word_probabilities
             )
```

### Comparing `faster-whisper-0.6.0/faster_whisper/utils.py` & `faster-whisper-0.7.0/faster_whisper/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import re
 
 from typing import Optional
 
 import huggingface_hub
 import requests
 
 from tqdm.auto import tqdm
@@ -29,50 +30,55 @@
 
 def get_logger():
     """Returns the module logger."""
     return logging.getLogger("faster_whisper")
 
 
 def download_model(
-    size: str,
+    size_or_id: str,
     output_dir: Optional[str] = None,
     local_files_only: bool = False,
     cache_dir: Optional[str] = None,
 ):
     """Downloads a CTranslate2 Whisper model from the Hugging Face Hub.
 
     The model is downloaded from https://huggingface.co/guillaumekln.
 
     Args:
-      size: Size of the model to download (tiny, tiny.en, base, base.en, small, small.en,
-        medium, medium.en, large-v1, or large-v2).
+      size_or_id: Size of the model to download (tiny, tiny.en, base, base.en, small, small.en,
+        medium, medium.en, large-v1, or large-v2), or a CTranslate2-converted model ID
+        from the Hugging Face Hub (e.g. guillaumekln/faster-whisper-large-v2).
       output_dir: Directory where the model should be saved. If not set, the model is saved in
         the cache directory.
       local_files_only:  If True, avoid downloading the file and return the path to the local
         cached file if it exists.
       cache_dir: Path to the folder where cached files are stored.
 
     Returns:
       The path to the downloaded model.
 
     Raises:
       ValueError: if the model size is invalid.
     """
-    if size not in _MODELS:
-        raise ValueError(
-            "Invalid model size '%s', expected one of: %s" % (size, ", ".join(_MODELS))
-        )
+    if re.match(r".*/.*", size_or_id):
+        repo_id = size_or_id
+    else:
+        if size_or_id not in _MODELS:
+            raise ValueError(
+                "Invalid model size '%s', expected one of: %s"
+                % (size_or_id, ", ".join(_MODELS))
+            )
 
-    repo_id = "guillaumekln/faster-whisper-%s" % size
+        repo_id = "guillaumekln/faster-whisper-%s" % size_or_id
 
     allow_patterns = [
         "config.json",
         "model.bin",
         "tokenizer.json",
-        "vocabulary.txt",
+        "vocabulary.*",
     ]
 
     kwargs = {
         "local_files_only": local_files_only,
         "allow_patterns": allow_patterns,
         "tqdm_class": disabled_tqdm,
     }
```

### Comparing `faster-whisper-0.6.0/faster_whisper/vad.py` & `faster-whisper-0.7.0/faster_whisper/vad.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Attributes:
       threshold: Speech threshold. Silero VAD outputs speech probabilities for each audio chunk,
         probabilities ABOVE this value are considered as SPEECH. It is better to tune this
         parameter for each dataset separately, but "lazy" 0.5 is pretty good for most datasets.
       min_speech_duration_ms: Final speech chunks shorter min_speech_duration_ms are thrown out.
       max_speech_duration_s: Maximum duration of speech chunks in seconds. Chunks longer
         than max_speech_duration_s will be split at the timestamp of the last silence that
-        lasts more than 100s (if any), to prevent aggressive cutting. Otherwise, they will be
+        lasts more than 100ms (if any), to prevent aggressive cutting. Otherwise, they will be
         split aggressively just before max_speech_duration_s.
       min_silence_duration_ms: In the end of each speech chunk wait for min_silence_duration_ms
         before separating it
       window_size_samples: Audio chunks of window_size_samples size are fed to the silero VAD model.
         WARNING! Silero VAD models were trained using 512, 1024, 1536 samples for 16000 sample rate.
         Values other than these may affect model performance!!
       speech_pad_ms: Final speech chunks are padded by speech_pad_ms each side
```

### Comparing `faster-whisper-0.6.0/faster_whisper.egg-info/PKG-INFO` & `faster-whisper-0.7.0/faster_whisper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 0.6.0
+Version: 0.7.0
 Summary: Faster Whisper transcription with CTranslate2
 Home-page: https://github.com/guillaumekln/faster-whisper
 Author: Guillaume Klein
 License: MIT
 Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
@@ -112,15 +112,19 @@
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True)
         ```
         
         The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
         
         ```python
-        segments, _ = model.transcribe("audio.mp3", vad_filter=True, vad_parameters=dict(min_silence_duration_ms=500))
+        segments, _ = model.transcribe(
+            "audio.mp3",
+            vad_filter=True,
+            vad_parameters=dict(min_silence_duration_ms=500),
+        )
         ```
         
         ### Logging
         
         The library logging level can be configured like this:
         
         ```python
@@ -137,14 +141,16 @@
         ## Community integrations
         
         Here is a non exhaustive list of open-source projects using faster-whisper. Feel free to add your project to the list!
         
         * [whisper-ctranslate2](https://github.com/Softcatala/whisper-ctranslate2) is a command line client based on faster-whisper and compatible with the original client from openai/whisper.
         * [whisper-diarize](https://github.com/MahmoudAshraf97/whisper-diarization) is a speaker diarization tool that is based on faster-whisper and NVIDIA NeMo.
         * [whisper-standalone-win](https://github.com/Purfview/whisper-standalone-win) contains the portable ready to run binaries of faster-whisper for Windows.
+        * [asr-sd-pipeline](https://github.com/hedrergudene/asr-sd-pipeline) provides a scalable, modular, end to end multi-speaker speech to text solution implemented using AzureML pipelines.
+        * [Open-Lyrics](https://github.com/zh-plus/Open-Lyrics) is a Python library that transcribes voice files using faster-whisper, and translates/polishes the resulting text into `.lrc` files in the desired language using OpenAI-GPT.
         
         ## Model conversion
         
         When loading a model from its size such as `WhisperModel("large-v2")`, the correspondig CTranslate2 model is automatically downloaded from the [Hugging Face Hub](https://huggingface.co/guillaumekln).
         
         We also provide a script to convert any Whisper models compatible with the Transformers library. They could be the original OpenAI models or user fine-tuned models.
         
@@ -158,14 +164,26 @@
         ```
         
         * The option `--model` accepts a model name on the Hub or a path to a model directory.
         * If the option `--copy_files tokenizer.json` is not used, the tokenizer configuration is automatically downloaded when the model is loaded later.
         
         Models can also be converted from the code. See the [conversion API](https://opennmt.net/CTranslate2/python/ctranslate2.converters.TransformersConverter.html).
         
+        ### Load a converted model
+        
+        1. Directly load the model from a local directory:
+        ```python
+        model = faster_whisper.WhisperModel("whisper-large-v2-ct2")
+        ```
+        
+        2. [Upload your model to the Hugging Face Hub](https://huggingface.co/docs/transformers/model_sharing#upload-with-the-web-interface) and load it from its name:
+        ```python
+        model = faster_whisper.WhisperModel("username/whisper-large-v2-ct2")
+        ```
+        
         ## Comparing performance against other implementations
         
         If you are comparing the performance against other Whisper implementations, you should make sure to run the comparison with similar settings. In particular:
         
         * Verify that the same transcription options are used, especially the same beam size. For example in openai/whisper, `model.transcribe` uses a default beam size of 1 but here we use a default beam size of 5.
         * When running on CPU, make sure to set the same number of threads. Many frameworks will read the environment variable `OMP_NUM_THREADS`, which can be set when running your script:
```

### Comparing `faster-whisper-0.6.0/faster_whisper.egg-info/SOURCES.txt` & `faster-whisper-0.7.0/faster_whisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.6.0/setup.py` & `faster-whisper-0.7.0/setup.py`

 * *Files identical despite different names*

