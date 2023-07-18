# Comparing `tmp/faster-whisper-0.5.1.tar.gz` & `tmp/faster-whisper-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster-whisper-0.5.1.tar", last modified: Wed Apr 26 15:40:24 2023, max compression
+gzip compressed data, was "faster-whisper-0.6.0.tar", last modified: Wed May 24 14:17:09 2023, max compression
```

## Comparing `faster-whisper-0.5.1.tar` & `faster-whisper-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:40:24.684096 faster-whisper-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-26 15:40:24.684096 faster-whisper-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:40:24.680096 faster-whisper-0.5.1/faster_whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:40:24.680096 faster-whisper-0.5.1/faster_whisper/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  1807524 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/assets/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    33120 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/transcribe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/vad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:40:24.680096 faster-whisper-0.5.1/faster_whisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-26 15:40:23.000000 faster-whisper-0.5.1/faster_whisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:40:24.000000 faster-whisper-0.5.1/faster_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:40:23.000000 faster-whisper-0.5.1/faster_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-26 15:40:23.000000 faster-whisper-0.5.1/faster_whisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 15:40:23.000000 faster-whisper-0.5.1/faster_whisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 15:40:24.684096 faster-whisper-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:17:09.528253 faster-whisper-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-24 14:17:09.528253 faster-whisper-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:17:09.524253 faster-whisper-0.6.0/faster_whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:17:09.524253 faster-whisper-0.6.0/faster_whisper/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  1807524 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/assets/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33826 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/transcribe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/vad.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/faster_whisper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:17:09.524253 faster-whisper-0.6.0/faster_whisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-24 14:17:09.000000 faster-whisper-0.6.0/faster_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-24 14:17:09.000000 faster-whisper-0.6.0/faster_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:17:09.000000 faster-whisper-0.6.0/faster_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-24 14:17:09.000000 faster-whisper-0.6.0/faster_whisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 14:17:09.000000 faster-whisper-0.6.0/faster_whisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/requirements.conversion.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-24 14:17:09.528253 faster-whisper-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-24 14:17:06.000000 faster-whisper-0.6.0/setup.py
```

### Comparing `faster-whisper-0.5.1/LICENSE` & `faster-whisper-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.1/PKG-INFO` & `faster-whisper-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 0.5.1
+Version: 0.6.0
 Summary: Faster Whisper transcription with CTranslate2
 Home-page: https://github.com/guillaumekln/faster-whisper
 Author: Guillaume Klein
 License: MIT
 Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
@@ -55,18 +55,14 @@
         
         ```bash
         # Install the master branch:
         pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/refs/heads/master.tar.gz"
         
         # Install a specific commit:
         pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/a4f1cc8f11433e454c3934442b5e1a4ed5e865c3.tar.gz"
-        
-        # Install for development:
-        git clone https://github.com/guillaumekln/faster-whisper.git
-        pip install -e faster-whisper/
         ```
         
         ### GPU support
         
         GPU execution requires the NVIDIA libraries cuBLAS 11.x and cuDNN 8.x to be installed on the system. Please refer to the [CTranslate2 documentation](https://opennmt.net/CTranslate2/installation.html).
         
         ## Usage
@@ -113,15 +109,15 @@
         
         The library integrates the [Silero VAD](https://github.com/snakers4/silero-vad) model to filter out parts of the audio without speech:
         
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True)
         ```
         
-        The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the function [`get_speech_timestamps`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
+        The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
         
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True, vad_parameters=dict(min_silence_duration_ms=500))
         ```
         
         ### Logging
         
@@ -136,17 +132,19 @@
         
         ### Going further
         
         See more model and transcription options in the [`WhisperModel`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
         
         ## Community integrations
         
-        Here is a non exhaustive list of open-source projects using *faster-whisper*. Feel free to add your project to the list!
+        Here is a non exhaustive list of open-source projects using faster-whisper. Feel free to add your project to the list!
         
-        * [whisper-ctranslate2](https://github.com/jordimas/whisper-ctranslate2) is a command line client based on `faster-whisper` and compatible with the original client from openai/whisper.
+        * [whisper-ctranslate2](https://github.com/Softcatala/whisper-ctranslate2) is a command line client based on faster-whisper and compatible with the original client from openai/whisper.
+        * [whisper-diarize](https://github.com/MahmoudAshraf97/whisper-diarization) is a speaker diarization tool that is based on faster-whisper and NVIDIA NeMo.
+        * [whisper-standalone-win](https://github.com/Purfview/whisper-standalone-win) contains the portable ready to run binaries of faster-whisper for Windows.
         
         ## Model conversion
         
         When loading a model from its size such as `WhisperModel("large-v2")`, the correspondig CTranslate2 model is automatically downloaded from the [Hugging Face Hub](https://huggingface.co/guillaumekln).
         
         We also provide a script to convert any Whisper models compatible with the Transformers library. They could be the original OpenAI models or user fine-tuned models.
```

### Comparing `faster-whisper-0.5.1/README.md` & `faster-whisper-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,18 +48,14 @@
 
 ```bash
 # Install the master branch:
 pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/refs/heads/master.tar.gz"
 
 # Install a specific commit:
 pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/a4f1cc8f11433e454c3934442b5e1a4ed5e865c3.tar.gz"
-
-# Install for development:
-git clone https://github.com/guillaumekln/faster-whisper.git
-pip install -e faster-whisper/
 ```
 
 ### GPU support
 
 GPU execution requires the NVIDIA libraries cuBLAS 11.x and cuDNN 8.x to be installed on the system. Please refer to the [CTranslate2 documentation](https://opennmt.net/CTranslate2/installation.html).
 
 ## Usage
@@ -106,15 +102,15 @@
 
 The library integrates the [Silero VAD](https://github.com/snakers4/silero-vad) model to filter out parts of the audio without speech:
 
 ```python
 segments, _ = model.transcribe("audio.mp3", vad_filter=True)
 ```
 
-The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the function [`get_speech_timestamps`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
+The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
 
 ```python
 segments, _ = model.transcribe("audio.mp3", vad_filter=True, vad_parameters=dict(min_silence_duration_ms=500))
 ```
 
 ### Logging
 
@@ -129,17 +125,19 @@
 
 ### Going further
 
 See more model and transcription options in the [`WhisperModel`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
 
 ## Community integrations
 
-Here is a non exhaustive list of open-source projects using *faster-whisper*. Feel free to add your project to the list!
+Here is a non exhaustive list of open-source projects using faster-whisper. Feel free to add your project to the list!
 
-* [whisper-ctranslate2](https://github.com/jordimas/whisper-ctranslate2) is a command line client based on `faster-whisper` and compatible with the original client from openai/whisper.
+* [whisper-ctranslate2](https://github.com/Softcatala/whisper-ctranslate2) is a command line client based on faster-whisper and compatible with the original client from openai/whisper.
+* [whisper-diarize](https://github.com/MahmoudAshraf97/whisper-diarization) is a speaker diarization tool that is based on faster-whisper and NVIDIA NeMo.
+* [whisper-standalone-win](https://github.com/Purfview/whisper-standalone-win) contains the portable ready to run binaries of faster-whisper for Windows.
 
 ## Model conversion
 
 When loading a model from its size such as `WhisperModel("large-v2")`, the correspondig CTranslate2 model is automatically downloaded from the [Hugging Face Hub](https://huggingface.co/guillaumekln).
 
 We also provide a script to convert any Whisper models compatible with the Transformers library. They could be the original OpenAI models or user fine-tuned models.
```

### Comparing `faster-whisper-0.5.1/faster_whisper/assets/silero_vad.onnx` & `faster-whisper-0.6.0/faster_whisper/assets/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.1/faster_whisper/audio.py` & `faster-whisper-0.6.0/faster_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.1/faster_whisper/feature_extractor.py` & `faster-whisper-0.6.0/faster_whisper/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.1/faster_whisper/tokenizer.py` & `faster-whisper-0.6.0/faster_whisper/tokenizer.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.1/faster_whisper/transcribe.py` & `faster-whisper-0.6.0/faster_whisper/transcribe.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from faster_whisper.audio import decode_audio
 from faster_whisper.feature_extractor import FeatureExtractor
 from faster_whisper.tokenizer import Tokenizer
 from faster_whisper.utils import download_model, format_timestamp, get_logger
 from faster_whisper.vad import (
     SpeechTimestampsMap,
+    VadOptions,
     collect_chunks,
     get_speech_timestamps,
 )
 
 
 class Word(NamedTuple):
     start: float
@@ -62,15 +63,17 @@
     append_punctuations: str
 
 
 class TranscriptionInfo(NamedTuple):
     language: str
     language_probability: float
     duration: float
+    all_language_probs: Optional[List[Tuple[str, float]]]
     transcription_options: TranscriptionOptions
+    vad_options: VadOptions
 
 
 class WhisperModel:
     def __init__(
         self,
         model_size_or_path: str,
         device: str = "auto",
@@ -173,15 +176,15 @@
         suppress_tokens: Optional[List[int]] = [-1],
         without_timestamps: bool = False,
         max_initial_timestamp: float = 1.0,
         word_timestamps: bool = False,
         prepend_punctuations: str = "\"'“¿([{-",
         append_punctuations: str = "\"'.。,，!！?？:：”)]}、",
         vad_filter: bool = False,
-        vad_parameters: Optional[dict] = None,
+        vad_parameters: Optional[Union[dict, VadOptions]] = None,
     ) -> Tuple[Iterable[Segment], TranscriptionInfo]:
         """Transcribes an input file.
 
         Arguments:
           audio: Path to the input file (or a file-like object), or the audio waveform.
           language: The language spoken in the audio. It should be a language code such
             as "en" or "fr". If not set, the language will be detected in the first 30 seconds
@@ -217,16 +220,16 @@
           prepend_punctuations: If word_timestamps is True, merge these punctuation symbols
             with the next word
           append_punctuations: If word_timestamps is True, merge these punctuation symbols
             with the previous word
           vad_filter: Enable the voice activity detection (VAD) to filter out parts of the audio
             without speech. This step is using the Silero VAD model
             https://github.com/snakers4/silero-vad.
-          vad_parameters: Dictionary of Silero VAD parameters (see available parameters and
-            default values in the function `get_speech_timestamps`).
+          vad_parameters: Dictionary of Silero VAD parameters or VadOptions class (see available
+            parameters and default values in the class `VadOptions`).
 
         Returns:
           A tuple with:
 
             - a generator over transcribed segments
             - an instance of TranscriptionInfo
         """
@@ -238,16 +241,19 @@
         duration = audio.shape[0] / sampling_rate
 
         self.logger.info(
             "Processing audio with duration %s", format_timestamp(duration)
         )
 
         if vad_filter:
-            vad_parameters = {} if vad_parameters is None else vad_parameters
-            speech_chunks = get_speech_timestamps(audio, **vad_parameters)
+            if vad_parameters is None:
+                vad_parameters = VadOptions()
+            elif isinstance(vad_parameters, dict):
+                vad_parameters = VadOptions(**vad_parameters)
+            speech_chunks = get_speech_timestamps(audio, vad_parameters)
             audio = collect_chunks(audio, speech_chunks)
 
             self.logger.info(
                 "VAD filter removed %s of audio",
                 format_timestamp(duration - (audio.shape[0] / sampling_rate)),
             )
 
@@ -266,25 +272,30 @@
 
         else:
             speech_chunks = None
 
         features = self.feature_extractor(audio)
 
         encoder_output = None
+        all_language_probs = None
 
         if language is None:
             if not self.model.is_multilingual:
                 language = "en"
                 language_probability = 1
             else:
                 segment = features[:, : self.feature_extractor.nb_max_frames]
                 encoder_output = self.encode(segment)
-                results = self.model.detect_language(encoder_output)
-                language_token, language_probability = results[0][0]
-                language = language_token[2:-2]
+                # results is a list of tuple[str, float] with language names and
+                # probabilities.
+                results = self.model.detect_language(encoder_output)[0]
+                # Parse language names to strip out markers
+                all_language_probs = [(token[2:-2], prob) for (token, prob) in results]
+                # Get top language token and probability
+                language, language_probability = all_language_probs[0]
 
                 self.logger.info(
                     "Detected language '%s' with probability %.2f",
                     language,
                     language_probability,
                 )
         else:
@@ -326,14 +337,16 @@
             segments = restore_speech_timestamps(segments, speech_chunks, sampling_rate)
 
         info = TranscriptionInfo(
             language=language,
             language_probability=language_probability,
             duration=duration,
             transcription_options=options,
+            vad_options=vad_parameters,
+            all_language_probs=all_language_probs,
         )
 
         return segments, info
 
     def generate_segments(
         self,
         features: np.ndarray,
@@ -746,14 +759,16 @@
         text_indices = np.array([pair[0] for pair in alignments])
         time_indices = np.array([pair[1] for pair in alignments])
 
         words, word_tokens = tokenizer.split_to_word_tokens(
             text_tokens + [tokenizer.eot]
         )
         word_boundaries = np.pad(np.cumsum([len(t) for t in word_tokens[:-1]]), (1, 0))
+        if len(word_boundaries) <= 1:
+            return []
 
         jumps = np.pad(np.diff(text_indices), (1, 0), constant_values=1).astype(bool)
         jump_times = time_indices[jumps] / self.tokens_per_second
         start_times = jump_times[word_boundaries[:-1]]
         end_times = jump_times[word_boundaries[1:]]
         word_probabilities = [
             np.mean(text_token_probs[i:j])
```

### Comparing `faster-whisper-0.5.1/faster_whisper/vad.py` & `faster-whisper-0.6.0/faster_whisper/vad.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,73 @@
 import bisect
 import functools
 import os
 import warnings
 
-from typing import List, Optional
+from typing import List, NamedTuple, Optional
 
 import numpy as np
 
 from faster_whisper.utils import get_assets_path
 
-# The code below is adapted from https://github.com/snakers4/silero-vad.
-
 
-def get_speech_timestamps(
-    audio: np.ndarray,
-    *,
-    threshold: float = 0.5,
-    min_speech_duration_ms: int = 250,
-    max_speech_duration_s: float = float("inf"),
-    min_silence_duration_ms: int = 2000,
-    window_size_samples: int = 1024,
-    speech_pad_ms: int = 400,
-) -> List[dict]:
-    """This method is used for splitting long audios into speech chunks using silero VAD.
+# The code below is adapted from https://github.com/snakers4/silero-vad.
+class VadOptions(NamedTuple):
+    """VAD options.
 
-    Args:
-      audio: One dimensional float array.
+    Attributes:
       threshold: Speech threshold. Silero VAD outputs speech probabilities for each audio chunk,
         probabilities ABOVE this value are considered as SPEECH. It is better to tune this
         parameter for each dataset separately, but "lazy" 0.5 is pretty good for most datasets.
       min_speech_duration_ms: Final speech chunks shorter min_speech_duration_ms are thrown out.
       max_speech_duration_s: Maximum duration of speech chunks in seconds. Chunks longer
         than max_speech_duration_s will be split at the timestamp of the last silence that
-        lasts more than 100s (if any), to prevent agressive cutting. Otherwise, they will be
+        lasts more than 100s (if any), to prevent aggressive cutting. Otherwise, they will be
         split aggressively just before max_speech_duration_s.
       min_silence_duration_ms: In the end of each speech chunk wait for min_silence_duration_ms
         before separating it
       window_size_samples: Audio chunks of window_size_samples size are fed to the silero VAD model.
         WARNING! Silero VAD models were trained using 512, 1024, 1536 samples for 16000 sample rate.
-        Values other than these may affect model perfomance!!
+        Values other than these may affect model performance!!
       speech_pad_ms: Final speech chunks are padded by speech_pad_ms each side
+    """
+
+    threshold: float = 0.5
+    min_speech_duration_ms: int = 250
+    max_speech_duration_s: float = float("inf")
+    min_silence_duration_ms: int = 2000
+    window_size_samples: int = 1024
+    speech_pad_ms: int = 400
+
+
+def get_speech_timestamps(
+    audio: np.ndarray,
+    vad_options: Optional[VadOptions] = None,
+    **kwargs,
+) -> List[dict]:
+    """This method is used for splitting long audios into speech chunks using silero VAD.
+
+    Args:
+      audio: One dimensional float array.
+      vad_options: Options for VAD processing.
+      kwargs: VAD options passed as keyword arguments for backward compatibility.
 
     Returns:
       List of dicts containing begin and end samples of each speech chunk.
     """
+    if vad_options is None:
+        vad_options = VadOptions(**kwargs)
+
+    threshold = vad_options.threshold
+    min_speech_duration_ms = vad_options.min_speech_duration_ms
+    max_speech_duration_s = vad_options.max_speech_duration_s
+    min_silence_duration_ms = vad_options.min_silence_duration_ms
+    window_size_samples = vad_options.window_size_samples
+    speech_pad_ms = vad_options.speech_pad_ms
+
     if window_size_samples not in [512, 1024, 1536]:
         warnings.warn(
             "Unusual window_size_samples! Supported window_size_samples:\n"
             " - [512, 1024, 1536] for 16000 sampling_rate"
         )
 
     sampling_rate = 16000
```

### Comparing `faster-whisper-0.5.1/faster_whisper.egg-info/PKG-INFO` & `faster-whisper-0.6.0/faster_whisper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 0.5.1
+Version: 0.6.0
 Summary: Faster Whisper transcription with CTranslate2
 Home-page: https://github.com/guillaumekln/faster-whisper
 Author: Guillaume Klein
 License: MIT
 Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
@@ -55,18 +55,14 @@
         
         ```bash
         # Install the master branch:
         pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/refs/heads/master.tar.gz"
         
         # Install a specific commit:
         pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/a4f1cc8f11433e454c3934442b5e1a4ed5e865c3.tar.gz"
-        
-        # Install for development:
-        git clone https://github.com/guillaumekln/faster-whisper.git
-        pip install -e faster-whisper/
         ```
         
         ### GPU support
         
         GPU execution requires the NVIDIA libraries cuBLAS 11.x and cuDNN 8.x to be installed on the system. Please refer to the [CTranslate2 documentation](https://opennmt.net/CTranslate2/installation.html).
         
         ## Usage
@@ -113,15 +109,15 @@
         
         The library integrates the [Silero VAD](https://github.com/snakers4/silero-vad) model to filter out parts of the audio without speech:
         
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True)
         ```
         
-        The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the function [`get_speech_timestamps`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
+        The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
         
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True, vad_parameters=dict(min_silence_duration_ms=500))
         ```
         
         ### Logging
         
@@ -136,17 +132,19 @@
         
         ### Going further
         
         See more model and transcription options in the [`WhisperModel`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
         
         ## Community integrations
         
-        Here is a non exhaustive list of open-source projects using *faster-whisper*. Feel free to add your project to the list!
+        Here is a non exhaustive list of open-source projects using faster-whisper. Feel free to add your project to the list!
         
-        * [whisper-ctranslate2](https://github.com/jordimas/whisper-ctranslate2) is a command line client based on `faster-whisper` and compatible with the original client from openai/whisper.
+        * [whisper-ctranslate2](https://github.com/Softcatala/whisper-ctranslate2) is a command line client based on faster-whisper and compatible with the original client from openai/whisper.
+        * [whisper-diarize](https://github.com/MahmoudAshraf97/whisper-diarization) is a speaker diarization tool that is based on faster-whisper and NVIDIA NeMo.
+        * [whisper-standalone-win](https://github.com/Purfview/whisper-standalone-win) contains the portable ready to run binaries of faster-whisper for Windows.
         
         ## Model conversion
         
         When loading a model from its size such as `WhisperModel("large-v2")`, the correspondig CTranslate2 model is automatically downloaded from the [Hugging Face Hub](https://huggingface.co/guillaumekln).
         
         We also provide a script to convert any Whisper models compatible with the Transformers library. They could be the original OpenAI models or user fine-tuned models.
```

### Comparing `faster-whisper-0.5.1/setup.py` & `faster-whisper-0.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,27 +7,35 @@
 
 def get_long_description():
     readme_path = os.path.join(base_dir, "README.md")
     with open(readme_path, encoding="utf-8") as readme_file:
         return readme_file.read()
 
 
+def get_project_version():
+    version_path = os.path.join(base_dir, "faster_whisper", "version.py")
+    version = {}
+    with open(version_path, encoding="utf-8") as fp:
+        exec(fp.read(), version)
+    return version["__version__"]
+
+
 def get_requirements(path):
     with open(path, encoding="utf-8") as requirements:
         return [requirement.strip() for requirement in requirements]
 
 
 install_requires = get_requirements(os.path.join(base_dir, "requirements.txt"))
 conversion_requires = get_requirements(
     os.path.join(base_dir, "requirements.conversion.txt")
 )
 
 setup(
     name="faster-whisper",
-    version="0.5.1",
+    version=get_project_version(),
     license="MIT",
     description="Faster Whisper transcription with CTranslate2",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="Guillaume Klein",
     url="https://github.com/guillaumekln/faster-whisper",
     classifiers=[
```

