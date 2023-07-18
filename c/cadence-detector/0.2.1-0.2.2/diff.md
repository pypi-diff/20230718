# Comparing `tmp/cadence_detector-0.2.1.tar.gz` & `tmp/cadence_detector-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadence_detector-0.2.1.tar", last modified: Thu Jun 29 08:29:44 2023, max compression
+gzip compressed data, was "cadence_detector-0.2.2.tar", last modified: Tue Jul 18 05:27:49 2023, max compression
```

## Comparing `cadence_detector-0.2.1.tar` & `cadence_detector-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-06-29 08:29:44.255334 cadence_detector-0.2.1/
--rw-r--r--   0 matanba  (223682273) 418804322     1058 2023-04-18 10:24:48.000000 cadence_detector-0.2.1/LICENSE
--rw-r--r--   0 matanba  (223682273) 418804322     1233 2023-06-29 08:29:44.254787 cadence_detector-0.2.1/PKG-INFO
--rw-r--r--   0 matanba  (223682273) 418804322      672 2023-04-22 15:45:43.000000 cadence_detector-0.2.1/README.md
--rw-r--r--   0 matanba  (223682273) 418804322      704 2023-06-29 08:29:30.000000 cadence_detector-0.2.1/pyproject.toml
--rw-r--r--   0 matanba  (223682273) 418804322       38 2023-06-29 08:29:44.255497 cadence_detector-0.2.1/setup.cfg
-drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-06-29 08:29:44.211459 cadence_detector-0.2.1/src/
--rw-r--r--   0 matanba  (223682273) 418804322        0 2023-04-22 08:05:31.000000 cadence_detector-0.2.1/src/__init__.py
-drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-06-29 08:29:44.250486 cadence_detector-0.2.1/src/cadence_detector/
--rw-r--r--   0 matanba  (223682273) 418804322     1624 2023-05-26 12:12:19.000000 cadence_detector-0.2.1/src/cadence_detector/CadenceDetectData.py
--rw-r--r--   0 matanba  (223682273) 418804322    57953 2023-06-29 08:23:15.000000 cadence_detector-0.2.1/src/cadence_detector/CadenceDetectStateMachine.py
--rw-r--r--   0 matanba  (223682273) 418804322    63776 2023-06-29 08:16:27.000000 cadence_detector-0.2.1/src/cadence_detector/CadenceDetector.py
--rw-r--r--   0 matanba  (223682273) 418804322        1 2023-04-22 08:31:36.000000 cadence_detector-0.2.1/src/cadence_detector/__init__.py
--rw-r--r--   0 matanba  (223682273) 418804322     2277 2023-04-22 14:52:32.000000 cadence_detector-0.2.1/src/cadence_detector/cadence_detector.py
-drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-06-29 08:29:44.254082 cadence_detector-0.2.1/src/cadence_detector.egg-info/
--rw-r--r--   0 matanba  (223682273) 418804322     1233 2023-06-29 08:29:44.000000 cadence_detector-0.2.1/src/cadence_detector.egg-info/PKG-INFO
--rw-r--r--   0 matanba  (223682273) 418804322      473 2023-06-29 08:29:44.000000 cadence_detector-0.2.1/src/cadence_detector.egg-info/SOURCES.txt
--rw-r--r--   0 matanba  (223682273) 418804322        1 2023-06-29 08:29:44.000000 cadence_detector-0.2.1/src/cadence_detector.egg-info/dependency_links.txt
--rw-r--r--   0 matanba  (223682273) 418804322       26 2023-06-29 08:29:44.000000 cadence_detector-0.2.1/src/cadence_detector.egg-info/requires.txt
--rw-r--r--   0 matanba  (223682273) 418804322       26 2023-06-29 08:29:44.000000 cadence_detector-0.2.1/src/cadence_detector.egg-info/top_level.txt
+drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-07-18 05:27:49.269268 cadence_detector-0.2.2/
+-rw-r--r--   0 matanba  (223682273) 418804322     1058 2023-04-18 10:24:48.000000 cadence_detector-0.2.2/LICENSE
+-rw-r--r--   0 matanba  (223682273) 418804322     1233 2023-07-18 05:27:49.268772 cadence_detector-0.2.2/PKG-INFO
+-rw-r--r--   0 matanba  (223682273) 418804322      672 2023-04-22 15:45:43.000000 cadence_detector-0.2.2/README.md
+-rw-r--r--   0 matanba  (223682273) 418804322      704 2023-07-18 05:27:25.000000 cadence_detector-0.2.2/pyproject.toml
+-rw-r--r--   0 matanba  (223682273) 418804322       38 2023-07-18 05:27:49.269394 cadence_detector-0.2.2/setup.cfg
+drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-07-18 05:27:49.220396 cadence_detector-0.2.2/src/
+-rw-r--r--   0 matanba  (223682273) 418804322        0 2023-04-22 08:05:31.000000 cadence_detector-0.2.2/src/__init__.py
+drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-07-18 05:27:49.225490 cadence_detector-0.2.2/src/cadence_detector/
+-rw-r--r--   0 matanba  (223682273) 418804322     1654 2023-07-10 18:21:33.000000 cadence_detector-0.2.2/src/cadence_detector/CadenceDetectData.py
+-rw-r--r--   0 matanba  (223682273) 418804322    61394 2023-07-17 14:52:20.000000 cadence_detector-0.2.2/src/cadence_detector/CadenceDetectStateMachine.py
+-rw-r--r--   0 matanba  (223682273) 418804322    64926 2023-07-18 05:25:02.000000 cadence_detector-0.2.2/src/cadence_detector/CadenceDetector.py
+-rw-r--r--   0 matanba  (223682273) 418804322        1 2023-04-22 08:31:36.000000 cadence_detector-0.2.2/src/cadence_detector/__init__.py
+-rw-r--r--   0 matanba  (223682273) 418804322     2277 2023-04-22 14:52:32.000000 cadence_detector-0.2.2/src/cadence_detector/cadence_detector.py
+drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-07-18 05:27:49.268166 cadence_detector-0.2.2/src/cadence_detector.egg-info/
+-rw-r--r--   0 matanba  (223682273) 418804322     1233 2023-07-18 05:27:49.000000 cadence_detector-0.2.2/src/cadence_detector.egg-info/PKG-INFO
+-rw-r--r--   0 matanba  (223682273) 418804322      473 2023-07-18 05:27:49.000000 cadence_detector-0.2.2/src/cadence_detector.egg-info/SOURCES.txt
+-rw-r--r--   0 matanba  (223682273) 418804322        1 2023-07-18 05:27:49.000000 cadence_detector-0.2.2/src/cadence_detector.egg-info/dependency_links.txt
+-rw-r--r--   0 matanba  (223682273) 418804322       26 2023-07-18 05:27:49.000000 cadence_detector-0.2.2/src/cadence_detector.egg-info/requires.txt
+-rw-r--r--   0 matanba  (223682273) 418804322       26 2023-07-18 05:27:49.000000 cadence_detector-0.2.2/src/cadence_detector.egg-info/top_level.txt
```

### Comparing `cadence_detector-0.2.1/LICENSE` & `cadence_detector-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cadence_detector-0.2.1/PKG-INFO` & `cadence_detector-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadence_detector
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package for cadence detection
 Author-email: Matan Ben-Asher <mbenasher@yahoo.com>
 Project-URL: Homepage, https://github.com/MusicalStateMachines/CadenceDetector
 Project-URL: Bug Tracker, https://github.com/MusicalStateMachines/CadenceDetector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadence_detector-0.2.1/README.md` & `cadence_detector-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cadence_detector-0.2.1/pyproject.toml` & `cadence_detector-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cadence_detector"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Matan Ben-Asher", email="mbenasher@yahoo.com" },
 ]
 description = "A python package for cadence detection"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cadence_detector-0.2.1/src/cadence_detector/CadenceDetectData.py` & `cadence_detector-0.2.2/src/cadence_detector/CadenceDetectData.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     PCCArrival = 9
     PACAppoggExpected = 10
     IACAppoggExpected = 11
     IACArrivalExpected = 12
     HCAppoggExpected = 13
     BassAppoggExpected = 14
     PCHArrival = 15
+    HCBassAppoggExpected = 16
 
 class CDHarmonicChordDegrees(Enum):
     I = 1
     II = 2
     III = 3
     IV = 4
     V = 5
```

### Comparing `cadence_detector-0.2.1/src/cadence_detector/CadenceDetectStateMachine.py` & `cadence_detector-0.2.2/src/cadence_detector/CadenceDetectStateMachine.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class CDStateMachine(object):
     def __init__(self, isChallenger=False, minInitialMeasures=0, minPostCadenceMeasures=0):
         self.NumParts = 0
         self.MeasureCounter = 0 # measure counter is for the entire movement and not included in reset
         self.MinInitialMeasures = {CDCadentialStates.PACArrival: minInitialMeasures, CDCadentialStates.IACArrival: minInitialMeasures, CDCadentialStates.HCArrival: round(minInitialMeasures/2)}
         self.MinPostCadenceMeasures = minPostCadenceMeasures
-        self.MinPostCadenceMeasuresHC = minPostCadenceMeasures+1
+        self.MinPostCadenceMeasuresHC = max(1, minPostCadenceMeasures)
         self.IsChallenger = isChallenger
         self.reset()
 
     def reset(self):
         # initiliaze with invalid states
         self.PrevCadentialState = CDCadentialStates.Idle
         self.CurrCadentialState = CDCadentialStates.Idle
@@ -35,14 +35,15 @@
         self.RevertLastHC = False
         self.RevertLastIAC = False
         self.HarmonicStateOfLastCadence = 0
         self.SopranoOfLastCadence = 0
         self.WeightOfLastCadence = 0
         self.PrevMeasureAlberti = False
         self.PrevMeasureArpeggio = False
+        self.IsPickupMeasure = False
 
     def resetPostCadentialCounters(self):
         self.PostPACMeasureCounter = self.MinPostCadenceMeasures
         self.PostHCMeasureCounter = self.MinPostCadenceMeasuresHC
 
     def updateHarmonicState(self, Key, Chord, ChordWithRests, ChordDegree, ChordInversion, ChordFigure, Alberti, Arpeggio, RomamNumeral, RealNotes):
 
@@ -58,15 +59,16 @@
         self.CurrHarmonicState.ChordDegree = ChordDegree
         self.CurrHarmonicState.ChordInversion = ChordInversion
         self.CurrHarmonicState.ChordFigure = ChordFigure
         self.CurrHarmonicState.Alberti = Alberti
         self.CurrHarmonicState.Arpeggio = Arpeggio
         self.CurrHarmonicState.RomanNumeral = RomamNumeral
         self.CurrHarmonicState.RealNotes = RealNotes
-        self.updateCounters()
+        if not self.IsPickupMeasure:
+            self.updateCounters()
         self.updateCadentialState()
 
     def checkStateChanged(self):
         self.ChangeFlagOneShot = 0
         if self.PrevCadentialState != self.CurrCadentialState:
             self.ChangeFlagOneShot = 1
             self.TriggerString = str("T") + str(self.PrevCadentialState.value) + str(u'\u208B') + str(self.CurrCadentialState.value)
@@ -112,30 +114,31 @@
                 bassPitch = self.getBassFromChord(HarmonicState.ChordWithBassRests, favor_by_part=favor_by_part)
                 if bassPitch:
                     retVal = bassPitch.pitchClass==pitchClass
         return retVal
 
     def isSopranoOnDegree(self, deg):
         retVal = 0
-        if not isinstance(deg, list):
-            deg = [deg]
-        for curr_deg in deg:
-            target_pitch_class = self.CurrHarmonicState.Key.pitchFromDegree(curr_deg).pitchClass
-            if self.CurrHarmonicState.Chord.pitches[-1].pitchClass == target_pitch_class:
-                retVal = 1
-                #check for voice crossing of other voices
-            elif self.CurrHarmonicState.Chord.sortFrequencyAscending().pitches[-1].pitchClass == target_pitch_class:
-                retVal = 1
-                #in multipart scores, check for explicit soprano
-            elif self.NumParts > 2:
-                sopranoPartPitch = self.getSopranoPartPitch(self.CurrHarmonicState)
-                if sopranoPartPitch and sopranoPartPitch.pitchClass == target_pitch_class:
+        if not self.CurrHarmonicState.Chord.isRest:
+            if not isinstance(deg, list):
+                deg = [deg]
+            for curr_deg in deg:
+                target_pitch_class = self.CurrHarmonicState.Key.pitchFromDegree(curr_deg).pitchClass
+                if self.CurrHarmonicState.Chord.pitches[-1].pitchClass == target_pitch_class:
                     retVal = 1
-            if retVal:
-                break
+                    #check for voice crossing of other voices
+                elif self.CurrHarmonicState.Chord.sortFrequencyAscending().pitches[-1].pitchClass == target_pitch_class:
+                    retVal = 1
+                    #in multipart scores, check for explicit soprano
+                elif self.NumParts > 2:
+                    sopranoPartPitch = self.getSopranoPartPitch(self.CurrHarmonicState)
+                    if sopranoPartPitch and sopranoPartPitch.pitchClass == target_pitch_class:
+                        retVal = 1
+                if retVal:
+                    break
         return retVal
 
     def getSopranoPartPitch(self, HarmonicState):
         retVal  = 0
         if not HarmonicState.Chord.isRest:
             for p in HarmonicState.Chord.pitches:
                 if 'MySoprano' in p.groups:
@@ -211,35 +214,24 @@
         return retVal
 
     def isTonicBass(self):
         tonicPitchClass = self.CurrHarmonicState.Key.pitchFromDegree(1).pitchClass
         retVal = self.compareBassWithPitch(tonicPitchClass, mode='any', favor_by_part=True)
         return retVal
 
-    def harmonyHasThird(self):
-        return not (self.CurrHarmonicState.Chord.third is None)
-
-    def isMatchingQuality(self):
-        return not self.harmonyHasThird() or\
-               (self.CurrHarmonicState.RomanNumeral.quality == self.CurrHarmonicState.Key.mode)
-
     def harmonyHasSeventh(self, HarmonicState):
         return self.harmonyContainsPitchDegree(HarmonicState=HarmonicState, degree=4)
         #return not (HarmonicState.Chord.seventh is None)
 
     def harmonyHasTonic(self,  HarmonicState):
         return self.harmonyContainsPitchDegree(HarmonicState=HarmonicState, degree=1)
 
     def harmonyHasMediant(self, HarmonicState):
         return self.harmonyContainsPitchDegree(HarmonicState=HarmonicState, degree=3)
 
-    # TBD - should obsolete this function
-    def verifyNotI64(self, HarmonicState):
-        return not (self.harmonyHasTonic(HarmonicState) or self.harmonyHasMediant(HarmonicState)) or self.harmonyHasSeventh(HarmonicState)
-
     def isI64(self, HarmonicState):
         return self.harmonyContainsOnlyPitchDegrees(HarmonicState=HarmonicState, degrees=[1, 3, 5]) and\
                (self.harmonyHasTonic(HarmonicState) or self.harmonyHasMediant(HarmonicState)) and\
                self.isDominantBass(HarmonicState=HarmonicState)
 
     def harmonyContainsOnlyPitchDegrees(self, HarmonicState, degrees):
         pitch_classes = [HarmonicState.Key.pitchFromDegree(degree).pitchClass for degree in degrees]
@@ -378,23 +370,26 @@
     def verifyPACGrouping(self, HarmonicState):
         return self.verifyGrouping(HarmonicState=HarmonicState, start_stop='any') or self.tryGetBeatStrength()==1.0
 
     def verifyIACGrouping(self, HarmonicState):
         return self.verifyGrouping(HarmonicState=HarmonicState, start_stop='stop')
 
     def verifyHCGrouping(self, HarmonicState, start_stop='stop'):
-        return self.verifyGrouping(HarmonicState=HarmonicState, start_stop=start_stop) and self.tryGetBeatStrength()>=0.5
+        beatStrength = self.tryGetBeatStrength()
+        return beatStrength == 1.0 or\
+               (beatStrength >= 0.5 and self.verifyGrouping(HarmonicState=HarmonicState, start_stop='any')) or\
+               (beatStrength >= 0.25 and self.verifyGrouping(HarmonicState=HarmonicState, start_stop='stop'))
 
     def verifyCadenceVoiceLeading(self, prev_soprano_pitch, curr_soprano_pitch, cadence_type='PAC'):
         retVal = True
         if curr_soprano_pitch and prev_soprano_pitch:
             midi_diff = curr_soprano_pitch.midi - prev_soprano_pitch.midi
             allowed_interval_table = {'PAC': np.array([0, 1, -2, -3, -4, 5, -7]), # anticipated tonic, minor second up, major second down, major/minor third down, fourth up, fifth down
                                       'IAC': np.array([0, 1, 2, 3, 4, -1, -2, -3, -4, 5]),  # anticipated third or fifth, major/minor second up, major/minor second down, major/minor third up and down, fourth up
-                                      'HC': np.array([0, 1, 2, -1, -2, -5, -7])}
+                                      'HC': np.array([0, 1, 2, -1, -2, -3, -5, -7])}
             allowed_intervals = allowed_interval_table[cadence_type]
             allowed_intervals_full = np.concatenate((allowed_intervals, allowed_intervals-12, allowed_intervals+12)) # check also an octave down and up, Mozart K533-1, Haydn17_3_4
             retVal = midi_diff in allowed_intervals_full
         return retVal
 
     def verifySopranoVoiceLeading(self, cadence_type='PAC'):
         curr_soprano_pitch = self.getSopranoPitch(self.CurrHarmonicState)
@@ -456,25 +451,25 @@
         # ===============================================
         # ====idle state, wait for IV or II6 or I6=======
         # ===============================================
         if curr_state == CDCadentialStates.Idle:
             if (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
                 # do nothing
                 curr_state = curr_state
-            elif self.CurrHarmonicState.ChordWithBassRests.isRest and not self.PrevHarmonicState.Chord.isRest:
+            elif self.CurrHarmonicState.ChordWithBassRests.isRest and not self.PrevHarmonicState.Chord.isRest and not self.IsChallenger:
                 if self.tryGetBeatStrength() < 1.0:
-                    #if sudden rest and not on strongest beat, check if previous harmony was dominant
+                    #if sudden rest and not on strongest beat, check if previous harmony could have been HC
                     if isinstance(self.PrevHarmonicState.Key, key.Key):
-                        dominantPitchClass = self.PrevHarmonicState.Key.pitchFromDegree(5).pitchClass
-                        bassPitch = self.getBassFromChord(self.PrevHarmonicState.Chord)
-                        if bassPitch and bassPitch.pitchClass == dominantPitchClass and not self.isI64(HarmonicState=self.PrevHarmonicState) and self.verifySopranoVoiceLeading(cadence_type='HC'):
+                        if self.verifyHCGrouping(HarmonicState=self.PrevHarmonicState) and self.verifyHCHarmony(HarmonicState=self.PrevHarmonicState):
                             curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
+                        else:
+                            curr_state = curr_state
                 else:
                     curr_state = curr_state
-            elif self.isDominantEmbellishment():# this can create false HCs, need to consider non-cadential chromatic situations
+            elif self.isDominantEmbellishment() and not self.IsChallenger:# this can create false HCs, need to consider non-cadential chromatic situations
                 curr_state = CDCadentialStates.HCArrivalExpected
             elif self.CurrHarmonicState.ChordWithBassRests.isRest:
                 curr_state = curr_state
             elif self.compareBassWithPitch(self.CurrHarmonicState.Key.pitchFromDegree(4).pitchClass, mode='any'):
                 #== bass in 4th degree - IV or II6 go to expecting cadence
                 curr_state = CDCadentialStates.CadExpected
             elif self.compareBassWithPitch(self.CurrHarmonicState.Key.pitchFromDegree(6).pitchClass, mode='any'):
@@ -492,49 +487,60 @@
             if curr_state == CDCadentialStates.CadAvoided:
                 curr_state = CDCadentialStates.CadExpected
             elif curr_state == CDCadentialStates.IACArrival and not (self.isTonicBass() and self.isSopranoOnDegree(1)):
                 curr_state = CDCadentialStates.CadExpected
             elif curr_state == CDCadentialStates.IACArrival and self.tryGetBeatStrength() == 1:
                 curr_state = CDCadentialStates.CadExpected
             # now start the real state logic
-            if curr_state == CDCadentialStates.IACArrival and (self.isTonicBass() and self.isSopranoOnDegree(1)):
-                self.RevertLastIAC = True
-                curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state, verify_beat_strength=False)
-            elif self.isDominantEmbellishment():
+            # === Revert IAC to PAC  - this catches some debatable PACs and also False Positives
+            #if curr_state == CDCadentialStates.IACArrival and (self.isTonicBass() and self.isSopranoOnDegree(1)):
+            #    self.RevertLastIAC = True
+            #    curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state, verify_beat_strength=False)
+            if self.isDominantEmbellishment():
                 curr_state = CDCadentialStates.HCArrivalExpected
-            elif self.CurrHarmonicState.ChordWithBassRests.isRest:
-                curr_state = curr_state
+            elif self.CurrHarmonicState.ChordWithBassRests.isRest and not self.PrevHarmonicState.Chord.isRest and not self.IsChallenger:
+                if self.tryGetBeatStrength() < 1.0:
+                    # if sudden rest and not on strongest beat, check if previous harmony could have been HC
+                    if isinstance(self.PrevHarmonicState.Key, key.Key):
+                        if self.verifyHCGrouping(HarmonicState=self.PrevHarmonicState) and self.verifyHCHarmony(HarmonicState=self.PrevHarmonicState):
+                            curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
+                        else:
+                            curr_state = curr_state
+                else:
+                    curr_state = curr_state
             #ignoring arppegios
             elif (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
                 #if alberti or arpeggio bass unless explicit V chord
                 if self.isDominantBass(HarmonicState=self.LastNonAlbertiHarmonicState) and self.harmonyHasSeventh(self.CurrHarmonicState):
                     curr_state = CDCadentialStates.CadInevitable
                 else:
                     curr_state = curr_state
             elif self.isDominantBass() and self.harmonyHasSeventh(self.CurrHarmonicState):
                 curr_state = CDCadentialStates.CadInevitable
             elif self.isTonicBass():
                 curr_state = CDCadentialStates.HCArrivalExpected
             elif self.isDominantBass(favor_by_part=True):
-                if not self.isI64(self.CurrHarmonicState):
-                    if self.verifySopranoVoiceLeading(cadence_type='HC') and \
-                        ((self.tryGetBeatStrength()==1 and self.verifyHCGrouping(HarmonicState=self.CurrHarmonicState)) or
-                         self.verifyHCGrouping(HarmonicState=self.CurrHarmonicState, start_stop='stop')) and\
-                            self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState):
+                if self.verifySopranoVoiceLeading(cadence_type='HC') and \
+                    ((self.tryGetBeatStrength()==1 and self.verifyHCGrouping(HarmonicState=self.CurrHarmonicState)) or
+                     self.verifyHCGrouping(HarmonicState=self.CurrHarmonicState, start_stop='stop')):
+                    if self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState):
                         curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
+                    elif self.harmonyHasTonic(self.CurrHarmonicState) or self.harmonyHasMediant(self.CurrHarmonicState):
+                        curr_state = CDCadentialStates.HCAppoggExpected
                     else:
                         curr_state = CDCadentialStates.CadInevitable
                 else:
-                    curr_state = CDCadentialStates.HCAppoggExpected
+                    curr_state = CDCadentialStates.CadInevitable
+
 
         # ========================================================
         # ====inevitable cadence (PAC or IAC), wait for Is========
         # ========================================================
         elif curr_state==CDCadentialStates.CadInevitable or curr_state==CDCadentialStates.IACArrivalExpected:
-            #on dominant and then a complete rest --> HC with constraints
+            # on dominant and then a complete rest --> HC with constraints
             if self.CurrHarmonicState.ChordWithBassRests.isRest:
                 if self.verifySopranoVoiceLeading(cadence_type='HC') and\
                         self.verifyHCGrouping(HarmonicState=self.PrevHarmonicState) and\
                         self.verifyHCHarmony(HarmonicState=self.PrevHarmonicState):
                     curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
                 else:
                     curr_state = curr_state
@@ -543,15 +549,15 @@
                     self.isDominantBass(favor_by_part=True) and\
                     self.verifyHCGrouping(HarmonicState=self.CurrHarmonicState) and\
                     self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState):
                 curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
             elif self.isDominantEmbellishment():
                 curr_state = CDCadentialStates.HCArrivalExpected
             elif (self.isI64(HarmonicState=self.CurrHarmonicState) and not self.isBassPartRest()):
-                curr_state = CDCadentialStates.HCAppoggExpected
+                curr_state = CDCadentialStates.HCArrivalExpected
             elif (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
                 #if alberti and weak beat do nothing
                 curr_state = curr_state
             else:
                 # for the case where in IAC expected and dominant appears again, back to Cad inevitable
                 if curr_state==CDCadentialStates.IACArrivalExpected and self.isDominantBass(favor_by_part=True) and not self.isBassPartRest():
                     curr_state = CDCadentialStates.CadInevitable
@@ -612,54 +618,71 @@
             elif self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio:
                 if self.isDominantBass(favor_by_part=True, HarmonicState=self.LastNonAlbertiHarmonicState) and\
                         self.harmonyHasSeventh(self.CurrHarmonicState) and\
                         not self.isDominantEmbellishment():
                     curr_state = CDCadentialStates.CadInevitable
                 else:
                     curr_state = curr_state
-            elif self.tryGetBeatStrength() < 0.5 and\
-                    self.isDominantBass(favor_by_part=True) and\
+            elif self.tryGetBeatStrength() < 0.25 and\
+                    self.isDominantBass(favor_by_part=True) and \
+                    self.harmonyHasSeventh(self.CurrHarmonicState) and \
                     self.isDominantHarmony(HarmonicState=self.CurrHarmonicState):#weak beat returning to dominant, return to cad inevitable
                 curr_state = CDCadentialStates.CadInevitable
             elif self.CurrHarmonicState.ChordWithBassRests.isRest:
-                curr_state = CDCadentialStates.CadExpected
-            elif self.tryGetBeatStrength() >= 0.5: #strong beats
+                if self.verifyHCGrouping(HarmonicState=self.PrevHarmonicState) and self.verifyHCHarmony(HarmonicState=self.PrevHarmonicState):
+                    curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
+                else:
+                    curr_state = curr_state
+            elif self.tryGetBeatStrength() >= 0.25: #strong beats
                 if self.isDominantBass(favor_by_part=True) and\
                         (self.verifyHCGrouping(self.CurrHarmonicState, start_stop='any') or self.tryGetBeatStrength()==1) and\
                         not self.isI64(HarmonicState=self.CurrHarmonicState) and\
                         self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState) and\
                         self.verifySopranoVoiceLeading(cadence_type='HC'):
                     curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
                 # appoggiatura on strongest beat, or if V64
                 elif self.isDominantBass(favor_by_part=True) and\
                         (self.isI64(HarmonicState=self.CurrHarmonicState) and not self.isBassPartRest()) and\
                         self.verifyHCGrouping(self.CurrHarmonicState, start_stop='any'):
                     curr_state = CDCadentialStates.HCAppoggExpected
-                elif self.isDominantBass(favor_by_part=True) and\
+                elif self.isTonicBass() and self.tryGetBeatStrength() >= 0.5 and \
+                        self.verifyPACGrouping(HarmonicState=self.CurrHarmonicState) and \
+                        self.isDominantBass(HarmonicState=self.LastNonAlbertiHarmonicState) and\
+                        self.isDominantHarmony(HarmonicState=self.PrevHarmonicState):
+                    if self.isSopranoOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC'):
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state)
+                    elif self.isSopranoOnDegree([3, 5]) and self.verifySopranoVoiceLeading(cadence_type='IAC'):
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
+                    else:
+                        curr_state = self.checkAppoggiaturaOrAvoidance('PAC')
+                elif self.isDominantBass(favor_by_part=False) and\
                         ((self.harmonyHasSeventh(self.CurrHarmonicState) and not self.isDominantEmbellishment()) or\
                          not (self.verifyHCGrouping(self.CurrHarmonicState, start_stop='any') or self.tryGetBeatStrength()==1)): #V7 or V without grouping return to cad inevitable
                     curr_state = CDCadentialStates.CadInevitable
                 elif self.isDominantBass(favor_by_part=True) and self.tryGetBeatStrength() == 1.0:#appoggiatura on strongest beat, or if V64
                     curr_state = CDCadentialStates.HCAppoggExpected
-                elif not (self.isDominantBass() or self.isDominantEmbellishment()): #strong beat and not dominant or embellishment, cadence avoided
+                    # HC bass appoggiatura
+                elif self.tryGetBeatStrength() == 1 and self.isSopranoOnDegree([5]) and self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState) and not self.harmonyHasSeventh(self.CurrHarmonicState):
+                    curr_state = CDCadentialStates.HCBassAppoggExpected
+                elif not (self.isDominantBass() or self.isTonicBass() or self.isDominantEmbellishment()): #strong beat and not dominant or embellishment, cadence avoided
                     curr_state = CDCadentialStates.CadAvoided
                 elif self.isDominantBass(favor_by_part=True) and self.verifyHCGrouping(HarmonicState=self.CurrHarmonicState, start_stop='any') and not self.harmonyHasSeventh(self.CurrHarmonicState):
                     curr_state = CDCadentialStates.HCAppoggExpected
 
 
         elif curr_state == CDCadentialStates.PACAppoggExpected or curr_state == CDCadentialStates.BassAppoggExpected:
 
             if self.CurrHarmonicState.ChordWithBassRests.isRest or (self.tryGetBeatStrength() == 1): # and not self.isTonicBass()): # rest or new measure not on tonic, exit appoggiatura:
                 if self.isDominantBass():
                     if (self.verifyHCGrouping(self.CurrHarmonicState, start_stop='any') or self.tryGetBeatStrength()==1) and\
                             self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState) and\
                             self.verifySopranoVoiceLeading(cadence_type='HC'):
                         curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
                     elif self.isI64(self.CurrHarmonicState):  # I64 can be HC appoggiaturra on dominant bass
-                        curr_state = CDCadentialStates.HCAppoggExpected
+                        curr_state = CDCadentialStates.HCArrivalExpected
                     else:
                         curr_state = CDCadentialStates.CadInevitable
                 elif self.isTonicBass() and\
                         self.CurrHarmonicState.Chord.isConsonant() and\
                         not self.harmonyContainsPitchDegree(HarmonicState=self.CurrHarmonicState, degree=6):
                     if self.isSopranoOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC') and\
                             (not self.IsChallenger or self.verifyPACGrouping(self.CurrHarmonicState)):
@@ -672,26 +695,26 @@
                 else:
                     curr_state = CDCadentialStates.CadExpected
             else:
             # ==appoggiatura, check bass still on key and if soprano is root then PAC otherwise IAC
             # ==for bass appoggiatura check  that soprano is still on tonic and that bass is also.
             # ==grouping is not required becuase it was verified on the appoggiatura entrance
             # ==in case of alberti or arppeggio the original bass on entrance remains, so tonic bass verification is not required.
-                if curr_state == CDCadentialStates.BassAppoggExpected and (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
+                if curr_state == CDCadentialStates.BassAppoggExpected and not self.isTonicBass() and (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
                     curr_state = curr_state
                 elif self.isTonicBass() or\
                         (curr_state == CDCadentialStates.PACAppoggExpected and (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio)) and\
                         self.CurrHarmonicState.Chord.isConsonant() and\
                         not self.harmonyContainsPitchDegree(HarmonicState=self.CurrHarmonicState, degree=6):
                     if self.isSopranoOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC') and\
                             (not self.IsChallenger or self.verifyPACGrouping(self.CurrHarmonicState)):
-                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state)
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state, verify_beat_strength=False)
                     elif self.isSopranoOnDegree(3) and self.verifySopranoVoiceLeading(cadence_type='IAC') and \
                             self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
-                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state, verify_beat_strength=False)
                 elif self.isDominantBass(favor_by_part=True) and\
                         (self.verifyHCGrouping(self.CurrHarmonicState, start_stop='any') or self.tryGetBeatStrength()==1) and\
                         self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState) and\
                         self.verifySopranoVoiceLeading(cadence_type='HC'):
                     curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
                 elif not (self.isSopranoOnDegree(1) or self.isDominantBass() or self.isMediantBass()):#continue the appogiattura if dominant or mediant bass
                     curr_state = CDCadentialStates.CadAvoided
@@ -714,18 +737,23 @@
                             curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
                 elif self.isDominantBass(): # dominant bass, go to PAC appogiatura
                     curr_state = self.checkAppoggiaturaOrAvoidance('PAC')
                 elif not (self.isSopranoOnDegree(1) or self.isMediantBass()):#continue the appogiattura if dominant or mediant bass
                     curr_state = CDCadentialStates.CadAvoided
 
 
-        elif curr_state == CDCadentialStates.HCAppoggExpected:
+        elif curr_state == CDCadentialStates.HCAppoggExpected or curr_state == CDCadentialStates.HCBassAppoggExpected:
             # ==HC with appoggiatura, don't exit as long as bass is dominant
             if self.CurrHarmonicState.ChordWithBassRests.isRest:
-                curr_state = CDCadentialStates.CadExpected
+                if self.verifySopranoVoiceLeading(cadence_type='HC') and\
+                        self.verifyHCHarmony(HarmonicState=self.PrevHarmonicState) and\
+                        self.isDominantBass(HarmonicState=self.LastNonAlbertiHarmonicState):
+                    curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
+                elif not self.isDominantBass(HarmonicState=self.LastNonAlbertiHarmonicState):
+                    curr_state = CDCadentialStates.CadExpected
             else:
                 if (self.isI64(HarmonicState=self.CurrHarmonicState) and not self.isBassPartRest()) or self.isDominantEmbellishment(): # stay in HC appogg as long as I64 or dominant embellishment
                     curr_state = curr_state
                 elif self.isDominantBass(favor_by_part=True) and\
                         self.verifyHCHarmony(self.CurrHarmonicState) and\
                         self.verifySopranoVoiceLeading(cadence_type='HC'):
                     curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
@@ -740,24 +768,30 @@
                             self.harmonyHasSeventh(self.CurrHarmonicState) and\
                             not self.isDominantEmbellishment():
                         curr_state = CDCadentialStates.CadInevitable
                     else:
                         curr_state = curr_state
                 elif self.isTonicBass() and self.tryGetBeatStrength() >= 0.5 and\
                         self.verifyPACGrouping(HarmonicState=self.CurrHarmonicState) and\
+                        self.isDominantBass(HarmonicState=self.LastNonAlbertiHarmonicState) and\
                         self.isDominantHarmony(HarmonicState=self.PrevHarmonicState):
                     if self.isSopranoOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC'):
                         curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state)
                     elif self.isSopranoOnDegree([3, 5]) and self.verifySopranoVoiceLeading(cadence_type='IAC'):
                         curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
                     else:
                         curr_state = self.checkAppoggiaturaOrAvoidance('PAC')
+                elif self.isDominantBass(favor_by_part=True) and self.isDominantHarmony(HarmonicState=self.CurrHarmonicState):
+                    curr_state = CDCadentialStates.CadInevitable
+                # Mozart does use V7 in his HC appoggiatura - see K331-1
                 elif self.tryGetBeatStrength() >= 0.25 and self.isDominantBass(favor_by_part=True) and (self.harmonyHasSeventh(self.CurrHarmonicState) or self.tryGetBeatStrength() >= 0.5): #V7 or strong beat, return to cad inevitable
                     curr_state = CDCadentialStates.CadInevitable
-                elif not self.isDominantBass():
+                elif curr_state == CDCadentialStates.HCAppoggExpected and not self.isDominantBass():
+                    curr_state = CDCadentialStates.CadAvoided
+                elif curr_state == CDCadentialStates.HCBassAppoggExpected and not self.isSopranoOnDegree([5]):
                     curr_state = CDCadentialStates.CadAvoided
 
         elif curr_state == CDCadentialStates.PACArrival or curr_state == CDCadentialStates.PCCArrival:
             #conditions for exiting PAC state:
             #1. complete rest
             #2. new measure
             #3. bass not on tonic
@@ -850,15 +884,15 @@
         self.checkStateChanged()
 
     def checkAppoggiaturaOrAvoidance(self, app_type='PAC'):
         if app_type == 'PAC' and \
                 ((self.CurrHarmonicState.Key.mode == 'major' and self.isSopranoOnSemitonesFromTonic([11, 2, 4])) or
                  (self.CurrHarmonicState.Key.mode == 'minor' and self.isSopranoOnSemitonesFromTonic([10, 11, 2, 3]))):
             curr_state = CDCadentialStates.PACAppoggExpected
-        elif app_type == 'IAC' and self.isSopranoOnSemitonesFromTonic([3, 5]) and self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
+        elif app_type in ['IAC', 'PAC'] and self.isSopranoOnSemitonesFromTonic([3, 5]) and self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
             curr_state = CDCadentialStates.IACAppoggExpected
         elif app_type == 'HC' and \
                 ((self.CurrHarmonicState.Key.mode == 'major' and self.isSopranoOnSemitonesFromTonic([0, 1, 4, 6, 9])) or
                  (self.CurrHarmonicState.Key.mode == 'minor' and self.isSopranoOnSemitonesFromTonic([0, 1, 3, 6, 8]))):
             curr_state = CDCadentialStates.HCAppoggExpected
         else:
             curr_state = CDCadentialStates.CadAvoided
```

### Comparing `cadence_detector-0.2.1/src/cadence_detector/CadenceDetector.py` & `cadence_detector-0.2.2/src/cadence_detector/CadenceDetector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import numpy as np
+
 from .CadenceDetectStateMachine import *
 import music21 as m21
 import math
 import os
 import pickle
-import pickle
 import enum
 import copy
 import sys
+import itertools
 
 class CadenceDetector:
     def __init__(self,
                  maxNumMeasures=500,
                  minInitialMeasures=0,
                  minPostCadenceMeasures=0,
                  keyDetectionMode = CDKeyDetectionModes.KSWithSmoothingCadenceSensitive,
@@ -60,14 +62,16 @@
         self.EmptyMeasures = []
         self.FinalBarlines = []
         self.analysis_full = []
         self.analysis_filtered = []
         self.analysis_transition_strings = []
         self.PrevMeasureAlberti = False
         self.PrevMeasureArpeggio = False
+        self.CadentialKeyChange = False
+        self.AnchorRange = range(4,17)
 
 
     def loadMusic21Corpus(self,fileString):
         self.NoteStream = m21.corpus.parse(fileString)
         self.analyze()
 
     def loadFileAndGetMeasures(self, fileString):
@@ -516,43 +520,33 @@
         Music21StringMode = SearStringMode.replace("M","m")
         return m21.key.Key(Music21StringKey,Music21StringMode)
 
     def isArpeggioPattern(self, pitches, lengths, arp_len, up_down=None):
         if len(pitches) < arp_len or not all(lengths[0] == l for l in lengths[1:-1]): # the final note in an arpeggio can be longer
             retVal = False
         else:
-            retVal = True
+            intervals = np.diff([x.midi for x in pitches])
             if up_down == 'up':
-                if all(x.midi > pitches[0].midi for x in pitches[1:]):
-                    prev_pitch = []
-                    for p in pitches:
-                        if prev_pitch and (p.midi - prev_pitch.midi) < 3: #minor and major second disqualifies the arpeggio
-                            retVal = False
-                            break
-                        prev_pitch = p
-                else:
-                    retVal = False
+                monotonic_rising = np.all(intervals > 0)
+                num_seconds = np.count_nonzero(intervals < 3)
+                retVal = monotonic_rising and num_seconds <= 1 # allow one major or minor second
             elif up_down == 'down':
-                if all(x.midi < pitches[0].midi for x in pitches[1:]):
-                    prev_pitch = []
-                    for p in pitches:
-                        if prev_pitch and (prev_pitch.midi - p.midi) < 3: #minor and major second disqualifies the arpeggio
-                            retVal = False
-                            break
-                        prev_pitch = p
-                else:
-                    retVal = False
+                monotonic_falling = np.all(intervals < 0)
+                num_seconds = np.count_nonzero(intervals > -3)
+                retVal = monotonic_falling and num_seconds <= 1 # allow one major or minor second
+            else:
+                retVal = False
         return retVal
 
     def isAlbertiPattern(self, pitches, lengths, pattern_len):
         equal_durations = all(lengths[0] == l for l in lengths[1:4])
         lowest_pitch_first = all(x.midi >= pitches[0].midi for x in pitches[1:4])
         lowest_pitch_third = all(x.midi >= pitches[2].midi for x in pitches[1:4])
         repetitve_pitch = (pitches[1].midi == pitches[3].midi or pitches[0].midi == pitches[2].midi)
-        consecutive_pitch = np.any(np.diff([x.midi for x in pitches]) == 0)
+        consecutive_pitch = (lowest_pitch_first and pitches[0].midi == pitches[1].midi) or (lowest_pitch_third and pitches[2].midi == pitches[1].midi)
         # for pattern length 6 (3/4,3/8,6/8) verify last two as well, either continuing the same pattern or repeating the bass
         if pattern_len == 6:
             equal_durations = all(lengths[0] == l for l in lengths)
             repetitve_pitch = repetitve_pitch and (pitches[3].midi == pitches[5].midi or pitches[0] == pitches[4])
         is_alberti = equal_durations and repetitve_pitch and (lowest_pitch_first or lowest_pitch_third) and not consecutive_pitch
         bass_pitch_index = None
         if lowest_pitch_first:
@@ -669,29 +663,37 @@
 
         # check first timesig
         measure_zero = self.ChordStream.measure(0)
         curr_time_sig = self.check_and_update_timesig(measure_zero, [])
 
         # loop on measures:
         try:
+            # for debugging a measure range
+            # range_with_holes = itertools.chain(range(0, 4), range(70, 84))
+            # for currMeasureIndex in range_with_holes:
             for currMeasureIndex in range(0,self.NumMeasures):
                 # debug per measure
-                if currMeasureIndex == 18:
+                if currMeasureIndex == 79:
                     bla = 0
                 # true measures start with 1, pickups will start from zero, but not all corpora will abide to this
                 # for example, data that originates from midi cannot contain this info
                 # to overcome this, we attempt to find the pickup via initial rests and discard it
                 # also, we count the empty measures and index them out while writing the label
                 measure_number = currMeasureIndex + 1
                 # print(f"measure number {measure_number}")
                 CurrMeasuresRestless = self.ChordStreamRestless.measure(measure_number)
                 CurrMeasures = self.ChordStream.measure(measure_number)
                 CurrMeasuresNotes = self.NoteStream.measure(measure_number)
                 CurrMeasureBass = self.BassChords.measure(measure_number)
 
+                # state machines need this for their first counters
+                isPickupMeasure = measure_number == 1 and self.hasPickupMeasure
+                self.HarmonicStateMachine.IsPickupMeasure = isPickupMeasure
+                self.HarmonicStateMachineChallenger.IsPickupMeasure = isPickupMeasure
+
                 # check and update timesig
                 curr_time_sig = self.check_and_update_timesig(CurrMeasures, curr_time_sig)
 
                 # reset state machines after repeat brackets, unless cadence inevitable (TBD  - add double barlines to this)
                 if currMeasureIndex > 0 and self.FinalBarlines[currMeasureIndex-1] and not (self.HarmonicStateMachine.getCadentialOutput() == CDCadentialStates.CadInevitable):
                     self.HarmonicStateMachine.reset()
                     self.HarmonicStateMachineChallenger.reset()
@@ -785,14 +787,15 @@
                     LyricChallenger = self.HarmonicStateMachineChallenger.getCadentialOutputString()
                     # Cadence Sensitive Key Detection Mode
                     if self.KeyDetectionMode == CDKeyDetectionModes.KSWithSmoothingCadenceSensitive:
                         # and self.HarmonicStateMachineChallenger.CurrHarmonicState.Key.tonic != self.HarmonicStateMachine.CurrHarmonicState.Key.tonic: #don't be sensitive to candece in parallel key:
                         # Cadence check in main key (for key re-enforcement)
 
                         resort = False
+                        self.CadentialKeyChange = False
                         for cad in self.ReinforcementFactors:
                             if cad in Lyric:
                                 # avoid reinforcement of HC if challenger is on dominant
                                 reenforce = not (currKey.getDominant().pitchClass == challengerKey.tonic.pitchClass and challengerKey.mode=='major' and (cad == 'HC'))
                                 if reenforce:
                                     self.reenforceKeyByFactor(currKeyString, self.ReinforcementFactors[cad])
                             # Challenger Check (for key switching, but ignore HCs in subdominant key (becuase they are more likely PACs in main key))
@@ -802,19 +805,23 @@
                                     self.reenforceKeyByFactor(challengerKeyString, self.ReinforcementFactors[cad])
                                     resort = True
                         if resort:
                             # re-sort and return Top2Keys
                             self.Top2Keys = self.getTopNKeyInterpretations(2)
                             if challengerKeyString == self.Top2Keys[0][0]:
                                 Lyric = LyricChallenger
+                                self.CadentialKeyChange = True
                                 print('Cadential Key Change!')
 
                     # debugging
                     # print(self.HarmonicStateMachine.getCadentialOutput().value)
                     # thisChord.lyric = str(rn.figure)
+                    # for debugging albertis and arppeggios
+                    # if alberti or arpeggio:
+                    #    Lyric = Lyric + 'Al'
 
                     if Lyric:   # only work on non-empty lyrics
                         thisChord.lyric = Lyric
                         LyricPerBeat.append([thisChord.beat,Lyric])
                         #TBD - do we still need to print this?
                         self.analysis_transition_strings.append(f"{measuresSecondsMap[currMeasureIndex]['offsetSeconds'] + measuresSecondsMap[currMeasureIndex]['durationSeconds']*(thisChord.beat-1)/CurrMeasuresRestless.duration.quarterLength:.1f} {self.HarmonicStateMachine.getCadentialOutput().value}")
 
@@ -920,15 +927,16 @@
                 empty_measure_counter = empty_measure_counter + 1
                 continue
             measure_number = currMeasureIndex + 1
             CurrMeasureNotes = self.NoteStream.measure(measure_number)
             CurrParts = CurrMeasureNotes.recurse().getElementsByClass(m21.stream.Part)
 
             measure_number_for_score = measure_number - self.hasPickupMeasure - empty_measure_counter
-            even_meas_since_anchor = (measure_number_for_score - AnchorCadenceMeasureNumber) % 2 == 0
+            measures_since_anchor  = measure_number_for_score - AnchorCadenceMeasureNumber
+            even_meas_since_anchor = measures_since_anchor % 2 == 0
 
             CurrMeasureLyrics = []
             for part in CurrParts:
                 for thisNote in part.flat.notesAndRests:
                     CurrMeasureLyrics.append(thisNote.lyric)
 
             def remove_lyric_from_parts(lyric_list, parts):
@@ -936,42 +944,44 @@
                     for thisNote in part.flat.notesAndRests:
                         for lyric in lyric_list:
                             thisNote.lyric = thisNote.lyric.replace(lyric, '')
 
             if PrevMeasureNotes and PrevMeasureLyrics:
                 # HC --> PAC
                 if (self.isilos('HC', PrevMeasureLyrics) or self.isilos('PCH', PrevMeasureLyrics)) and (self.isilos('PAC', CurrMeasureLyrics) or self.isilos('PCC', CurrMeasureLyrics)):
-                    if even_meas_since_anchor:
+                    remove_lyric_from_parts(['PCH'], PrevParts)
+                    if even_meas_since_anchor or measures_since_anchor not in self.AnchorRange:
                         print(f'Filtering HC in measure {measure_number_for_score-1}')
-                        remove_lyric_from_parts(['HC', 'PCH'], PrevParts)
+                        remove_lyric_from_parts(['HC'], PrevParts)
+                    #elif self.isilos('HC', PrevMeasureLyrics):
+                    #    print(f'Filtering PAC in measure {measure_number_for_score}')
+                    #    remove_lyric_from_parts(['PAC'], CurrParts)
                 # PAC --> HC
                 if self.isilos('PAC', PrevMeasureLyrics) and (self.isilos('HC', CurrMeasureLyrics) or self.isilos('PCH', CurrMeasureLyrics)):
-                    if not even_meas_since_anchor:
+                    remove_lyric_from_parts(['PCH'], CurrParts)
+                    if not even_meas_since_anchor or measures_since_anchor not in self.AnchorRange:
                         print(f'Filtering HC in measure {measure_number_for_score}')
-                        remove_lyric_from_parts(['HC', 'PCH'], CurrParts)
+                        remove_lyric_from_parts(['HC'], CurrParts)
                 # PAC + HC
                 if (self.isilos('HC', CurrMeasureLyrics) or self.isilos('PCH', CurrMeasureLyrics)) and (self.isilos('PAC', CurrMeasureLyrics) or self.isilos('PCC', CurrMeasureLyrics)):
                     print(f'Filtering HC in measure {measure_number_for_score}')
                     remove_lyric_from_parts(['HC', 'PCH'], CurrParts)
                 # HC --> IAC
                 if (self.isilos('HC', PrevMeasureLyrics) or self.isilos('PCH', PrevMeasureLyrics)) and (self.isilos('IAC', CurrMeasureLyrics)):
-                    if even_meas_since_anchor:
+                    remove_lyric_from_parts(['PCH'], PrevParts)
+                    if even_meas_since_anchor or measures_since_anchor not in self.AnchorRange:
                         print(f'Filtering HC in measure {measure_number_for_score - 1}')
-                        remove_lyric_from_parts(['HC','PCH'], PrevParts)
+                        remove_lyric_from_parts(['HC'], PrevParts)
                     else:
                         print(f'Filtering IAC in measure {measure_number_for_score}')
                         remove_lyric_from_parts(['IAC'], CurrParts)
                 # IAC --> HC
                 if self.isilos('IAC', PrevMeasureLyrics) and (self.isilos('HC', CurrMeasureLyrics) or self.isilos('PCH', CurrMeasureLyrics)):
-                    if even_meas_since_anchor:
-                        print(f'Filtering IAC in measure {measure_number_for_score - 1}')
-                        remove_lyric_from_parts(['IAC'], PrevParts)
-                    else:
-                        print(f'Filtering HC in measure {measure_number_for_score}')
-                        remove_lyric_from_parts(['HC', 'PCH'], CurrParts)
+                    print(f'Filtering IAC in measure {measure_number_for_score - 1}')
+                    remove_lyric_from_parts(['IAC'], PrevParts)
                 # HC+IAC
                 if (self.isilos('HC', CurrMeasureLyrics) or self.isilos('PCH', CurrMeasureLyrics)) and self.isilos('IAC', CurrMeasureLyrics):
                     print(f'Filtering IAC in measure {measure_number_for_score}')
                     remove_lyric_from_parts(['IAC'], CurrParts)
                 # PAC+IAC
                 if (self.isilos('PAC', CurrMeasureLyrics) or self.isilos('PCC', CurrMeasureLyrics)) and self.isilos('IAC', CurrMeasureLyrics):
                     print(f'Filtering IAC in measure {measure_number_for_score}')
@@ -1009,48 +1019,48 @@
         anchor_cad = {'Measure':0, 'Lyric':[]}
         for item in self.analysis_full_filtered:
             curr_cad = item
             # check if cadence in analysis line
             cad_strings = ['PAC', 'PCC', 'HC', 'PCH', 'IAC']
             if not any(s in curr_cad['Lyric'] for s in cad_strings):
                 continue
-            even_meas_since_anchor = (curr_cad['Measure'] - anchor_cad['Measure']) % 2 == 0
+            measures_since_anchor = curr_cad['Measure'] - anchor_cad['Measure']
+            even_meas_since_anchor = measures_since_anchor % 2 == 0
             if curr_cad['Measure'] - prev_cad['Measure'] <= 1:
                 # HC --> PAC and HC+PAC
                 if ('HC' in prev_cad['Lyric'] or 'PCH' in prev_cad['Lyric']) and ('PAC' in curr_cad['Lyric'] or 'PCC' in curr_cad['Lyric']):
-                    if even_meas_since_anchor:
+                    if even_meas_since_anchor or measures_since_anchor not in self.AnchorRange or curr_cad['Measure'] == prev_cad['Measure']:
                         if prev_cad not in items_to_remove:
                             print(f"Filtering HC in measure {prev_cad['Measure']}")
                             items_to_remove.append(prev_cad)
+                    #elif 'HC' in prev_cad['Lyric']:
+                    #    if curr_cad not in items_to_remove:
+                    #        print(f"Filtering PAC in measure {curr_cad['Measure']}")
+                    #        items_to_remove.append(curr_cad)
                 # PAC --> HC and PAC+HC
                 if ('PAC' in prev_cad['Lyric'] or 'PCC' in prev_cad['Lyric']) and ('HC' in curr_cad['Lyric'] or 'PCH' in curr_cad['Lyric']):
-                    if not even_meas_since_anchor or curr_cad['Measure'] == prev_cad['Measure']:
+                    if not even_meas_since_anchor or measures_since_anchor not in self.AnchorRange or curr_cad['Measure'] == prev_cad['Measure']:
                         if curr_cad not in items_to_remove:
                             print(f"Filtering HC in measure {curr_cad['Measure']}")
                             items_to_remove.append(curr_cad)
                 # HC --> IAC
                 if ('HC' in prev_cad['Lyric'] or 'PCH' in prev_cad['Lyric']) and 'IAC' in curr_cad['Lyric']:
-                    if even_meas_since_anchor and curr_cad['Measure'] > prev_cad['Measure']:
+                    if (even_meas_since_anchor or measures_since_anchor not in self.AnchorRange) and curr_cad['Measure'] > prev_cad['Measure']:
                         if prev_cad not in items_to_remove:
                             print(f"Filtering HC in measure {prev_cad['Measure']}")
                             items_to_remove.append(prev_cad)
                     else:
                         if curr_cad not in items_to_remove:
                             print(f"Filtering IAC in measure {curr_cad['Measure']}")
                             items_to_remove.append(curr_cad)
                 # IAC --> HC
                 if 'IAC' in prev_cad['Lyric'] and ('HC' in curr_cad['Lyric'] or 'PCH' in curr_cad['Lyric']):
-                    if even_meas_since_anchor or curr_cad['Measure'] == prev_cad['Measure']:
-                        if prev_cad not in items_to_remove:
-                            print(f"Filtering IAC in measure {prev_cad['Measure']}")
-                            items_to_remove.append(prev_cad)
-                    else:
-                        if curr_cad not in items_to_remove:
-                            print(f"Filtering HC in measure {curr_cad['Measure']}")
-                            items_to_remove.append(curr_cad)
+                    if prev_cad not in items_to_remove:
+                        print(f"Filtering IAC in measure {prev_cad['Measure']}")
+                        items_to_remove.append(prev_cad)
                 # IAC --> PAC
                 if 'IAC' in prev_cad['Lyric'] and ('PAC' in curr_cad['Lyric'] or 'PCC' in curr_cad['Lyric']):
                     if prev_cad not in items_to_remove:
                         print(f"Filtering IAC in measure {prev_cad['Measure']}")
                         items_to_remove.append(prev_cad)
                 # PAC --> IAC
                 if 'IAC' in curr_cad['Lyric'] and ('PAC' in prev_cad['Lyric'] or 'PCC' in prev_cad['Lyric']):
@@ -1123,15 +1133,16 @@
             tempStateMachine = copy.deepcopy(self.HarmonicStateMachine)
             if currKeyString == self.PrevChallengerKeyString:
                 self.HarmonicStateMachine = copy.deepcopy(self.HarmonicStateMachineChallenger)
                 self.HarmonicStateMachine.CadentialKeyChange = 1
             if challengerKeyString == self.PrevKeyString:
                 self.HarmonicStateMachineChallenger = copy.deepcopy(tempStateMachine)
             # reset post cadential counters
-            self.HarmonicStateMachine.resetPostCadentialCounters()
+            if not self.CadentialKeyChange:
+                self.HarmonicStateMachine.resetPostCadentialCounters()
             self.HarmonicStateMachineChallenger.resetPostCadentialCounters()
         self.PrevKeyString = currKeyString
         self.PrevChallengerKeyString = challengerKeyString
         self.HarmonicStateMachine.IsChallenger = False
         self.HarmonicStateMachineChallenger.IsChallenger = True
 
     def setFileName(self,fileName):
```

### Comparing `cadence_detector-0.2.1/src/cadence_detector/cadence_detector.py` & `cadence_detector-0.2.2/src/cadence_detector/cadence_detector.py`

 * *Files identical despite different names*

### Comparing `cadence_detector-0.2.1/src/cadence_detector.egg-info/PKG-INFO` & `cadence_detector-0.2.2/src/cadence_detector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadence-detector
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package for cadence detection
 Author-email: Matan Ben-Asher <mbenasher@yahoo.com>
 Project-URL: Homepage, https://github.com/MusicalStateMachines/CadenceDetector
 Project-URL: Bug Tracker, https://github.com/MusicalStateMachines/CadenceDetector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

