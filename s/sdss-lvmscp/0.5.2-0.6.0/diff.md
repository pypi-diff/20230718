# Comparing `tmp/sdss_lvmscp-0.5.2.tar.gz` & `tmp/sdss_lvmscp-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmscp-0.5.2.tar", max compression
+gzip compressed data, was "sdss_lvmscp-0.6.0.tar", max compression
```

## Comparing `sdss_lvmscp-0.5.2.tar` & `sdss_lvmscp-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1504 2023-07-17 21:19:01.855097 sdss_lvmscp-0.5.2/LICENSE.md
--rw-r--r--   0        0        0     1578 2023-07-17 21:19:01.855381 sdss_lvmscp-0.5.2/README.md
--rw-r--r--   0        0        0     2715 2023-07-17 21:19:03.919656 sdss_lvmscp-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      369 2023-07-17 21:19:03.920422 sdss_lvmscp-0.5.2/python/lvmscp/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-17 21:19:03.920800 sdss_lvmscp-0.5.2/python/lvmscp/__main__.py
--rw-r--r--   0        0        0      258 2023-07-17 21:19:03.921295 sdss_lvmscp-0.5.2/python/lvmscp/actor/__init__.py
--rw-r--r--   0        0        0     8321 2023-07-17 21:19:03.921704 sdss_lvmscp-0.5.2/python/lvmscp/actor/actor.py
--rw-r--r--   0        0        0      859 2023-07-17 21:19:03.922201 sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/__init__.py
--rw-r--r--   0        0        0     1515 2023-07-17 21:19:03.922558 sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/expose.py
--rw-r--r--   0        0        0     3827 2023-07-17 21:19:03.922963 sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/focus.py
--rw-r--r--   0        0        0     1272 2023-07-17 21:19:03.923301 sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/hardware_status.py
--rw-r--r--   0        0        0      758 2023-07-17 21:19:03.923644 sdss_lvmscp-0.5.2/python/lvmscp/controller.py
--rw-r--r--   0        0        0    13727 2023-07-17 21:19:03.924065 sdss_lvmscp-0.5.2/python/lvmscp/delegate.py
--rw-r--r--   0        0        0    40775 2023-07-17 21:19:03.924729 sdss_lvmscp-0.5.2/python/lvmscp/etc/LVM_100kHz.acf
--rw-r--r--   0        0        0     5736 2023-07-17 21:19:03.925225 sdss_lvmscp-0.5.2/python/lvmscp/etc/lvmscp.yml
--rw-r--r--   0        0        0      161 2023-07-17 21:19:03.925605 sdss_lvmscp-0.5.2/python/lvmscp/etc/schema.json
--rw-r--r--   0        0        0    18807 2023-07-17 21:19:03.926089 sdss_lvmscp-0.5.2/python/lvmscp/ln2.py
--rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 sdss_lvmscp-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-18 16:46:38.763487 sdss_lvmscp-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0     1578 2023-07-18 16:46:38.763707 sdss_lvmscp-0.6.0/README.md
+-rw-r--r--   0        0        0     2715 2023-07-18 16:46:38.805588 sdss_lvmscp-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-07-18 16:46:38.805984 sdss_lvmscp-0.6.0/python/lvmscp/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-18 16:46:38.806198 sdss_lvmscp-0.6.0/python/lvmscp/__main__.py
+-rw-r--r--   0        0        0      258 2023-07-18 16:46:38.806462 sdss_lvmscp-0.6.0/python/lvmscp/actor/__init__.py
+-rw-r--r--   0        0        0     8321 2023-07-18 16:46:38.806778 sdss_lvmscp-0.6.0/python/lvmscp/actor/actor.py
+-rw-r--r--   0        0        0      859 2023-07-18 16:46:38.807452 sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1515 2023-07-18 16:46:38.807710 sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/expose.py
+-rw-r--r--   0        0        0     3827 2023-07-18 16:46:38.808061 sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/focus.py
+-rw-r--r--   0        0        0     1272 2023-07-18 16:46:38.808328 sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/hardware_status.py
+-rw-r--r--   0        0        0      758 2023-07-18 16:46:38.808603 sdss_lvmscp-0.6.0/python/lvmscp/controller.py
+-rw-r--r--   0        0        0    13727 2023-07-18 16:46:38.808877 sdss_lvmscp-0.6.0/python/lvmscp/delegate.py
+-rw-r--r--   0        0        0    40889 2023-07-18 16:46:38.809375 sdss_lvmscp-0.6.0/python/lvmscp/etc/LVM_100kHz.acf
+-rw-r--r--   0        0        0     5736 2023-07-18 16:46:38.809690 sdss_lvmscp-0.6.0/python/lvmscp/etc/lvmscp.yml
+-rw-r--r--   0        0        0      161 2023-07-18 16:46:38.809975 sdss_lvmscp-0.6.0/python/lvmscp/etc/schema.json
+-rw-r--r--   0        0        0    18807 2023-07-18 16:46:38.810293 sdss_lvmscp-0.6.0/python/lvmscp/ln2.py
+-rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 sdss_lvmscp-0.6.0/PKG-INFO
```

### Comparing `sdss_lvmscp-0.5.2/LICENSE.md` & `sdss_lvmscp-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/README.md` & `sdss_lvmscp-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/pyproject.toml` & `sdss_lvmscp-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmscp"
-version = "0.5.2"
+version = "0.6.0"
 description = "LVM spectrograph control package."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "Changgon Kim <changgonkim@khu.ac.kr>"]
 maintainers = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmscp"
 repository = "https://github.com/sdss/lvmscp"
@@ -28,15 +28,15 @@
 [tool.poetry.scripts]
 lvmscp = "lvmscp.__main__:main"
 ln2fill = "lvmscp.ln2:ln2fill"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 click-default-group = "^1.2.2"
-sdss-archon = "^0.10.0"
+sdss-archon = "^0.11.0"
 httpx = ">=0.18.1"
 Authlib = ">=1.0.0rc1"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=7.11.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
```

### Comparing `sdss_lvmscp-0.5.2/python/lvmscp/__main__.py` & `sdss_lvmscp-0.6.0/python/lvmscp/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/python/lvmscp/actor/actor.py` & `sdss_lvmscp-0.6.0/python/lvmscp/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/__init__.py` & `sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/expose.py` & `sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/focus.py` & `sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/focus.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/hardware_status.py` & `sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/hardware_status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/python/lvmscp/controller.py` & `sdss_lvmscp-0.6.0/python/lvmscp/controller.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/python/lvmscp/delegate.py` & `sdss_lvmscp-0.6.0/python/lvmscp/delegate.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/python/lvmscp/etc/LVM_100kHz.acf` & `sdss_lvmscp-0.6.0/python/lvmscp/etc/LVM_100kHz.acf`

 * *Files 1% similar despite different names*

```diff
@@ -25,184 +25,189 @@
 CONSTANT9="A_HIGH=4"
 CONSTANTS=20
 FANDISABLE=0
 FRAMEMODE=2
 IP=10.0.0.2
 LINE0=Main:
 LINE1="RESET; IF ContinuousExposures GOTO Continuous"
-LINE10="X; GOTO EndInt"
-LINE100="S2LOW; X(ST)"
-LINE101="X; CALL HorizontalSWShift(2200)"
-LINE102="RGLOW; CLAMP(10000)"
-LINE103=NOCLAMP
-LINE104="S1HIGH; X(ST)"
-LINE105="S3LOW; X(ST)"
-LINE106="S2HIGH; X(ST)"
-LINE107="X; RETURN SkipLine"
-LINE108=
-LINE109=SkipLineBin:
-LINE11=
-LINE110="RGHIGH; CALL VerticalShift(SkipLineBinVShift)"
-LINE111="X; TSHIFT1(AT)"
-LINE112="X; TSHIFT2(AT)"
-LINE113="S1LOW; X(ST)"
-LINE114="S3HIGH; X(ST)"
-LINE115="S2LOW; X(ST)"
-LINE116="X; CALL HorizontalSWShift(2200)"
-LINE117="RGLOW; CLAMP(10000)"
-LINE118=NOCLAMP
-LINE119="S1HIGH; X(ST)"
-LINE12=Exposure:
-LINE120="S3LOW; X(ST)"
-LINE121="S2HIGH; X(ST)"
-LINE122="X; RETURN SkipLineBin"
-LINE123=
-LINE124=Pixel:
-LINE125="RGHIGH; X(24)"
-LINE126=RGLOW
-LINE127="X; CALL HorizontalShift(HorizontalBinning)"
-LINE128=PCLK
-LINE129="NOPCLK; X(PIXEL_CLOCK)"
-LINE13="X; CALL IntUnit(IntMS)"
-LINE130="SWLOW; X(10)"
-LINE131="SWHIGH; X(PIXEL_CLOCK)"
-LINE132="X; RETURN Pixel"
-LINE133=
-LINE134=SkipPixel:
-LINE135="RGHIGH; X(24)"
-LINE136=RGLOW
-LINE137="X; CALL HorizontalShift"
-LINE138=X
-LINE139="X; X(PIXEL_CLOCK)"
-LINE14="X; Exposures--"
-LINE140="SWLOW; X(10)"
-LINE141="SWHIGH; X(PIXEL_CLOCK)"
-LINE142="X; RETURN SkipPixel"
-LINE143=
-LINE144=HorizontalShift:
-LINE145="S1HIGH; X(ST)"
-LINE146="S3LOW; X(ST)"
-LINE147="S2HIGH; X(ST)"
-LINE148="S1LOW; X(ST)"
-LINE149="S3HIGH; X(ST)"
-LINE15="X; GOTO Main"
-LINE150="S2LOW; X(STM1)"
-LINE151="X; RETURN HorizontalShift"
-LINE152=
-LINE153=HorizontalSWShift:
-LINE154="S1HIGH; X(ST)"
-LINE155="S3SWLOW; X(ST)"
-LINE156="S2HIGH; X(ST)"
-LINE157="S1LOW; X(ST)"
-LINE158="S3SWHIGH; X(ST)"
-LINE159="S2LOW; X(STM1)"
-LINE16=
-LINE160="X; RETURN HorizontalSWShift"
-LINE161=
-LINE162=VerticalShift:
-LINE163="IMAGE1; X(AT)"
-LINE164="IMAGE2; X(AT)"
-LINE165="IMAGE3; X(AT)"
-LINE166="IMAGE4; X(AT)"
-LINE167="IMAGE5; X(AT)"
-LINE168="IMAGE6; X(AT)"
-LINE169="X; RETURN VerticalShift"
-LINE17=EndInt:
-LINE18="NOINT; ReadOut--"
-LINE19="NOINT; CALL NoIntUnit(NoIntMS)"
+LINE10="X; CALL IntUnitCS(IntCS)"
+LINE100="RGHIGH; CALL VerticalShift"
+LINE101="X; TSHIFT1(AT)"
+LINE102="X; TSHIFT2(AT)"
+LINE103="S1LOW; X(ST)"
+LINE104="S3HIGH; X(ST)"
+LINE105="S2LOW; X(ST)"
+LINE106="X; CALL HorizontalSWShift(2200)"
+LINE107="RGLOW; CLAMP(10000)"
+LINE108=NOCLAMP
+LINE109="S1HIGH; X(ST)"
+LINE11="X; GOTO EndInt"
+LINE110="S3LOW; X(ST)"
+LINE111="S2HIGH; X(ST)"
+LINE112="X; RETURN SkipLine"
+LINE113=
+LINE114=SkipLineBin:
+LINE115="RGHIGH; CALL VerticalShift(SkipLineBinVShift)"
+LINE116="X; TSHIFT1(AT)"
+LINE117="X; TSHIFT2(AT)"
+LINE118="S1LOW; X(ST)"
+LINE119="S3HIGH; X(ST)"
+LINE12=
+LINE120="S2LOW; X(ST)"
+LINE121="X; CALL HorizontalSWShift(2200)"
+LINE122="RGLOW; CLAMP(10000)"
+LINE123=NOCLAMP
+LINE124="S1HIGH; X(ST)"
+LINE125="S3LOW; X(ST)"
+LINE126="S2HIGH; X(ST)"
+LINE127="X; RETURN SkipLineBin"
+LINE128=
+LINE129=Pixel:
+LINE13=Exposure:
+LINE130="RGHIGH; X(24)"
+LINE131=RGLOW
+LINE132="X; CALL HorizontalShift(HorizontalBinning)"
+LINE133=PCLK
+LINE134="NOPCLK; X(PIXEL_CLOCK)"
+LINE135="SWLOW; X(10)"
+LINE136="SWHIGH; X(PIXEL_CLOCK)"
+LINE137="X; RETURN Pixel"
+LINE138=
+LINE139=SkipPixel:
+LINE14="X; CALL IntUnitCS(IntCS)"
+LINE140="RGHIGH; X(24)"
+LINE141=RGLOW
+LINE142="X; CALL HorizontalShift"
+LINE143=X
+LINE144="X; X(PIXEL_CLOCK)"
+LINE145="SWLOW; X(10)"
+LINE146="SWHIGH; X(PIXEL_CLOCK)"
+LINE147="X; RETURN SkipPixel"
+LINE148=
+LINE149=HorizontalShift:
+LINE15="X; Exposures--"
+LINE150="S1HIGH; X(ST)"
+LINE151="S3LOW; X(ST)"
+LINE152="S2HIGH; X(ST)"
+LINE153="S1LOW; X(ST)"
+LINE154="S3HIGH; X(ST)"
+LINE155="S2LOW; X(STM1)"
+LINE156="X; RETURN HorizontalShift"
+LINE157=
+LINE158=HorizontalSWShift:
+LINE159="S1HIGH; X(ST)"
+LINE16="X; GOTO Main"
+LINE160="S3SWLOW; X(ST)"
+LINE161="S2HIGH; X(ST)"
+LINE162="S1LOW; X(ST)"
+LINE163="S3SWHIGH; X(ST)"
+LINE164="S2LOW; X(STM1)"
+LINE165="X; RETURN HorizontalSWShift"
+LINE166=
+LINE167=VerticalShift:
+LINE168="IMAGE1; X(AT)"
+LINE169="IMAGE2; X(AT)"
+LINE17=
+LINE170="IMAGE3; X(AT)"
+LINE171="IMAGE4; X(AT)"
+LINE172="IMAGE5; X(AT)"
+LINE173="IMAGE6; X(AT)"
+LINE174="X; RETURN VerticalShift"
+LINE18=EndInt:
+LINE19="NOINT; ReadOut--"
 LINE2="X; IF Exposures GOTO Exposure"
-LINE20=NOCLAMP
-LINE21="RGHIGH; CALL HorizontalSWShift(2200)"
-LINE22="RGLOW; CLAMP(10000)"
-LINE23="S1HIGH; X(ST)"
-LINE24="S3LOW; X(ST)"
-LINE25="S2HIGH; X(ST)"
-LINE26="NOCLAMP; CALL SkipLine(PreSkipLines)"
-LINE27="FCLK; CALL Line(Lines)"
-LINE28="X; CALL SkipLine(PostSkipLines)"
-LINE29="X; CALL Line(OverscanLines)"
+LINE20="NOINT; CALL NoIntUnit(NoIntMS)"
+LINE21=NOCLAMP
+LINE22="RGHIGH; CALL HorizontalSWShift(2200)"
+LINE23="RGLOW; CLAMP(10000)"
+LINE24="S1HIGH; X(ST)"
+LINE25="S3LOW; X(ST)"
+LINE26="S2HIGH; X(ST)"
+LINE27="NOCLAMP; CALL SkipLine(PreSkipLines)"
+LINE28="FCLK; CALL Line(Lines)"
+LINE29="X; CALL SkipLine(PostSkipLines)"
 LINE3="X; IF ReadOut GOTO EndInt"
-LINE30="X; GOTO Main"
-LINE31=
-LINE32=Flush:
-LINE33="X; DoFlush--"
-LINE34="X; CALL FlushOne(FlushCount)"
-LINE35="X; GOTO Main"
-LINE36=
-LINE37=FlushOne:
-LINE38="X; CALL SkipLineBin(FlushBin)"
-LINE39="X; RETURN FlushOne"
+LINE30="X; CALL Line(OverscanLines)"
+LINE31="X; GOTO Main"
+LINE32=
+LINE33=Flush:
+LINE34="X; DoFlush--"
+LINE35="X; CALL FlushOne(FlushCount)"
+LINE36="X; GOTO Main"
+LINE37=
+LINE38=FlushOne:
+LINE39="X; CALL SkipLineBin(FlushBin)"
 LINE4="X; IF DoFlush GOTO Flush"
-LINE40=
-LINE41=IntUnit:
-LINE42="INT; IF AbortExposure GOTO Abort"
-LINE43="INT; CALL SmallIntUnit(502)"
-LINE44="X; X(99)"
-LINE45="X; RETURN IntUnit"
-LINE46=
-LINE47=Abort:
-LINE48="X; Exposures--"
-LINE49="X; AbortExposure--"
+LINE40="X; RETURN FlushOne"
+LINE41=
+LINE42=IntUnitCS:
+LINE43="X; CALL IntUnit(10)"
+LINE44="X; RETURN IntUnitCS"
+LINE45=
+LINE46=IntUnit:
+LINE47="INT; IF AbortExposure GOTO Abort"
+LINE48="INT; CALL SmallIntUnit(502)"
+LINE49="X; X(99)"
 LINE5="X; IF AutoFlush GOTO FlushOne"
-LINE50="X; GOTO Main"
+LINE50="X; RETURN IntUnit"
 LINE51=
-LINE52=NoIntUnit:
-LINE53="NOINT; CALL SmallIntUnit(502)"
-LINE54="X; NOINT(99)"
-LINE55="X; RETURN NoIntUnit"
+LINE52=Abort:
+LINE53="X; Exposures--"
+LINE54="X; AbortExposure--"
+LINE55="X; GOTO Main"
 LINE56=
-LINE57=SmallIntUnit:
-LINE58="RGHIGH; X(21)"
-LINE59="RGLOW; X(15)"
+LINE57=NoIntUnit:
+LINE58="NOINT; CALL SmallIntUnit(502)"
+LINE59="X; NOINT(99)"
 LINE6="X; GOTO Main"
-LINE60="S1HIGH; X(20)"
-LINE61="S3LOW; X(20)"
-LINE62="S2HIGH; X(20)"
-LINE63="S1LOW; X(20)"
-LINE64="S3HIGH; X(20)"
-LINE65="S2LOW; X(20)"
-LINE66="SWLOW; X(16)"
-LINE67="SWHIGH; X(16)"
-LINE68="SWHIGH; RETURN SmallIntUnit"
-LINE69=
+LINE60="X; RETURN NoIntUnit"
+LINE61=
+LINE62=SmallIntUnit:
+LINE63="RGHIGH; X(21)"
+LINE64="RGLOW; X(15)"
+LINE65="S1HIGH; X(20)"
+LINE66="S3LOW; X(20)"
+LINE67="S2HIGH; X(20)"
+LINE68="S1LOW; X(20)"
+LINE69="S3HIGH; X(20)"
 LINE7=
-LINE70=Line:
-LINE71="X; CALL VerticalShift(VerticalBinning)"
-LINE72="X; TSHIFT1(AT)"
-LINE73="X; TSHIFT2(AT)"
-LINE74="S1LOW; X(ST)"
-LINE75="S3HIGH; X(ST)"
-LINE76="S2LOW; X(ST)"
-LINE77="LCLK; CALL SkipPixel(PreSkipPixels)"
-LINE78="X; CALL Pixel(Pixels)"
-LINE79="X; CALL SkipPixel(PostSkipPixels)"
+LINE70="S2LOW; X(20)"
+LINE71="SWLOW; X(16)"
+LINE72="SWHIGH; X(16)"
+LINE73="SWHIGH; RETURN SmallIntUnit"
+LINE74=
+LINE75=Line:
+LINE76="X; CALL VerticalShift(VerticalBinning)"
+LINE77="X; TSHIFT1(AT)"
+LINE78="X; TSHIFT2(AT)"
+LINE79="S1LOW; X(ST)"
 LINE8=Continuous:
-LINE80="X; CALL Pixel(OverscanPixels)"
-LINE81="X; CALL Pixel"
-LINE82="CLAMP; X(10000)"
-LINE83=NOCLAMP
-LINE84="S1HIGH; X(ST)"
-LINE85="S3LOW; X(ST)"
-LINE86="S2HIGH; X(ST)"
-LINE87="X; CALL WaitOne(WaitCount)"
-LINE88="X; RETURN Line"
-LINE89=
-LINE9="X; CALL IntUnit(IntMS)"
-LINE90=WaitOne:
-LINE91="X; X(50000)"
-LINE92="X; RETURN WaitOne"
-LINE93=
-LINE94=SkipLine:
-LINE95="RGHIGH; CALL VerticalShift"
-LINE96="X; TSHIFT1(AT)"
-LINE97="X; TSHIFT2(AT)"
-LINE98="S1LOW; X(ST)"
-LINE99="S3HIGH; X(ST)"
+LINE80="S3HIGH; X(ST)"
+LINE81="S2LOW; X(ST)"
+LINE82="LCLK; CALL SkipPixel(PreSkipPixels)"
+LINE83="X; CALL Pixel(Pixels)"
+LINE84="X; CALL SkipPixel(PostSkipPixels)"
+LINE85="X; CALL Pixel(OverscanPixels)"
+LINE86="X; CALL Pixel"
+LINE87="CLAMP; X(10000)"
+LINE88=NOCLAMP
+LINE89="S1HIGH; X(ST)"
+LINE9="X; CALL IntUnit"
+LINE90="S3LOW; X(ST)"
+LINE91="S2HIGH; X(ST)"
+LINE92="X; CALL WaitOne(WaitCount)"
+LINE93="X; RETURN Line"
+LINE94=
+LINE95=WaitOne:
+LINE96="X; X(50000)"
+LINE97="X; RETURN WaitOne"
+LINE98=
+LINE99=SkipLine:
 LINECOUNT=2040
-LINES=170
+LINES=175
 LINESCAN=0
 MOD1\XVN_ENABLE1=1
 MOD1\XVN_ENABLE2=1
 MOD1\XVN_ENABLE3=1
 MOD1\XVN_ENABLE4=0
 MOD1\XVN_LABEL1=BB_C
 MOD1\XVN_LABEL2=BB_B
@@ -376,28 +381,28 @@
 MOD12\HEATERAD=0
 MOD12\HEATERAENABLE=1
 MOD12\HEATERAFORCE=0
 MOD12\HEATERAFORCELEVEL=0
 MOD12\HEATERAI=1
 MOD12\HEATERAIL=1000
 MOD12\HEATERALABEL=HEATER_B
-MOD12\HEATERALIMIT=25.0
+MOD12\HEATERALIMIT=8.0
 MOD12\HEATERAP=30
 MOD12\HEATERARAMP=0
 MOD12\HEATERARAMPRATE=1
 MOD12\HEATERASENSOR=2
 MOD12\HEATERATARGET=-105
 MOD12\HEATERBD=0
 MOD12\HEATERBENABLE=1
 MOD12\HEATERBFORCE=0
 MOD12\HEATERBFORCELEVEL=0
 MOD12\HEATERBI=1
 MOD12\HEATERBIL=1000
 MOD12\HEATERBLABEL=HEATER_C
-MOD12\HEATERBLIMIT=25.0
+MOD12\HEATERBLIMIT=8.0
 MOD12\HEATERBP=30
 MOD12\HEATERBRAMP=0
 MOD12\HEATERBRAMPRATE=1
 MOD12\HEATERBSENSOR=0
 MOD12\HEATERBTARGET=-124
 MOD12\HEATERUPDATETIME=1000
 MOD12\SENSORACURRENT=100000
@@ -460,28 +465,28 @@
 MOD2\HEATERAD=0
 MOD2\HEATERAENABLE=1
 MOD2\HEATERAFORCE=0
 MOD2\HEATERAFORCELEVEL=0
 MOD2\HEATERAI=1
 MOD2\HEATERAIL=1000
 MOD2\HEATERALABEL=HEATER_A
-MOD2\HEATERALIMIT=25.0
+MOD2\HEATERALIMIT=8.0
 MOD2\HEATERAP=30
 MOD2\HEATERARAMP=0
 MOD2\HEATERARAMPRATE=1
 MOD2\HEATERASENSOR=0
-MOD2\HEATERATARGET=-109.5
+MOD2\HEATERATARGET=-107.6
 MOD2\HEATERBD=0
 MOD2\HEATERBENABLE=0
 MOD2\HEATERBFORCE=0
 MOD2\HEATERBFORCELEVEL=0
 MOD2\HEATERBI=0
 MOD2\HEATERBIL=1000
 MOD2\HEATERBLABEL=
-MOD2\HEATERBLIMIT=25.0
+MOD2\HEATERBLIMIT=8.0
 MOD2\HEATERBP=0
 MOD2\HEATERBRAMP=0
 MOD2\HEATERBRAMPRATE=1
 MOD2\HEATERBSENSOR=0
 MOD2\HEATERBTARGET=0
 MOD2\HEATERUPDATETIME=1000
 MOD2\SENSORACURRENT=100000
@@ -906,15 +911,15 @@
 PARAMETER13="VerticalBinning=1"
 PARAMETER14="ST=12"
 PARAMETER15="STM1=11"
 PARAMETER16="AT=9000"
 PARAMETER17="WaitCount=0"
 PARAMETER18="PIXEL_CLOCK=440"
 PARAMETER19=
-PARAMETER2="IntMS=0"
+PARAMETER2="IntCS=0"
 PARAMETER20=# Switches
 PARAMETER21="AbortExposure=0"
 PARAMETER22="ReadOut=0"
 PARAMETER23="DoFlush=0"
 PARAMETER24="AutoFlush=1"
 PARAMETER25=
 PARAMETER26=# Flushing
```

### Comparing `sdss_lvmscp-0.5.2/python/lvmscp/etc/lvmscp.yml` & `sdss_lvmscp-0.6.0/python/lvmscp/etc/lvmscp.yml`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/python/lvmscp/ln2.py` & `sdss_lvmscp-0.6.0/python/lvmscp/ln2.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.2/PKG-INFO` & `sdss_lvmscp-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmscp
-Version: 0.5.2
+Version: 0.6.0
 Summary: LVM spectrograph control package.
 Home-page: https://github.com/sdss/lvmscp
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Maintainer: José Sánchez-Gallego
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Authlib (>=1.0.0rc1)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: httpx (>=0.18.1)
-Requires-Dist: sdss-archon (>=0.10.0,<0.11.0)
+Requires-Dist: sdss-archon (>=0.11.0,<0.12.0)
 Project-URL: Documentation, https://sdss-lvmscp.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/lvmscp
 Description-Content-Type: text/markdown
 
 # lvmscp
 
 ![Versions](https://img.shields.io/badge/python->3.8-blue)
```

