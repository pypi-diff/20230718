# Comparing `tmp/RangeSlider-2021.7.4.tar.gz` & `tmp/RangeSlider-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RangeSlider-2021.7.4.tar", last modified: Wed Jul  7 12:14:35 2021, max compression
+gzip compressed data, was "RangeSlider-2023.7.1.tar", last modified: Tue Jul 18 13:24:27 2023, max compression
```

## Comparing `RangeSlider-2021.7.4.tar` & `RangeSlider-2023.7.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2021-07-07 12:14:35.000000 RangeSlider-2021.7.4/
--rw-rw-rw-   0        0        0     9750 2021-07-07 12:14:35.000000 RangeSlider-2021.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     7567 2021-07-07 12:14:16.000000 RangeSlider-2021.7.4/README.md
-drwxrwxrwx   0        0        0        0 2021-07-07 12:14:35.000000 RangeSlider-2021.7.4/RangeSlider/
--rw-rw-rw-   0        0        0    28969 2021-07-07 10:07:14.000000 RangeSlider-2021.7.4/RangeSlider/RangeSlider.py
--rw-rw-rw-   0        0        0       64 2021-07-07 06:42:58.000000 RangeSlider-2021.7.4/RangeSlider/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-07 12:14:35.000000 RangeSlider-2021.7.4/RangeSlider.egg-info/
--rw-rw-rw-   0        0        0     9750 2021-07-07 12:14:35.000000 RangeSlider-2021.7.4/RangeSlider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2021-07-07 12:14:35.000000 RangeSlider-2021.7.4/RangeSlider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-07 12:14:35.000000 RangeSlider-2021.7.4/RangeSlider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2021-07-07 12:14:35.000000 RangeSlider-2021.7.4/RangeSlider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-07-07 12:14:35.000000 RangeSlider-2021.7.4/setup.cfg
--rw-rw-rw-   0        0        0     1851 2021-07-07 12:13:45.000000 RangeSlider-2021.7.4/setup.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-18 13:24:27.690401 RangeSlider-2023.7.1/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)    12625 2023-07-18 13:24:27.690401 RangeSlider-2023.7.1/PKG-INFO
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)    11734 2023-07-17 18:35:22.000000 RangeSlider-2023.7.1/README.md
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-18 13:24:27.690401 RangeSlider-2023.7.1/RangeSlider/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)    36567 2023-07-17 18:40:49.000000 RangeSlider-2023.7.1/RangeSlider/RangeSlider.py
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       64 2022-12-25 11:45:33.000000 RangeSlider-2023.7.1/RangeSlider/__init__.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-18 13:24:27.690401 RangeSlider-2023.7.1/RangeSlider.egg-info/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)    12625 2023-07-18 13:24:27.000000 RangeSlider-2023.7.1/RangeSlider.egg-info/PKG-INFO
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      209 2023-07-18 13:24:27.000000 RangeSlider-2023.7.1/RangeSlider.egg-info/SOURCES.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-07-18 13:24:27.000000 RangeSlider-2023.7.1/RangeSlider.egg-info/dependency_links.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       12 2023-07-18 13:24:27.000000 RangeSlider-2023.7.1/RangeSlider.egg-info/top_level.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       38 2023-07-18 13:24:27.690401 RangeSlider-2023.7.1/setup.cfg
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     2034 2023-07-18 13:23:43.000000 RangeSlider-2023.7.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `RangeSlider-2021.7.4/RangeSlider/RangeSlider.py` & `RangeSlider-2023.7.1/RangeSlider/RangeSlider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,127 @@
 from tkinter import *
 from tkinter.ttk import *
 
-
+# v2023.07.1
 
 class RangeSliderH(Frame):
     LINE_COLOR = "#476b6b"
     LINE_S_COLOR="#0a50ff"
     LINE_WIDTH = 3
     BAR_COLOR_INNER = "#5c8a8a"
     BAR_COLOR_OUTTER = "#c2d6d6"
     BAR_RADIUS = 10
     BAR_RADIUS_INNER = 5
     DIGIT_PRECISION = '.1f' # for showing in the canvas
     FONT_SIZE=16
     FONT_FAMILY='Times'
+    TEXT_COLOR='#000000'
     IMAGE_ANCHOR_L=CENTER
     IMAGE_ANCHOR_R=CENTER
+    STEP_MARKER_COLOR='#ffffff'
     def __init__(self, master, variables, Width = 400, Height = 80, min_val = 0, max_val = 1, padX=3,
                     image_anchorR=CENTER, image_anchorL=CENTER, imageL=None, imageR=None,
                     auto=True, line_width=3, bar_radius=10,
-                    bar_color_inner='#5c8a8a', line_s_color="#0a50ff", bar_color_outer='#c2d6d6', line_color = '#476b6b', bgColor= '#ffffff',
-                    show_value = True, digit_precision='.1f', valueSide='TOP', font_family='Times', font_size=16, suffix=""):
+                    bar_color_inner='#5c8a8a', line_s_color="#0a50ff", bar_color_outer='#c2d6d6', line_color = '#476b6b', bgColor= '#ffffff', step_marker_color = "#ffffff", font_color = '#000000',
+                    show_value = True, digit_precision='.1f', valueSide='TOP', font_family='Times', font_size=16, suffix="",
+                    step_size = 0,step_marker=False, cross_each_other = False):
         RangeSliderH.LINE_COLOR=line_color
         RangeSliderH.LINE_WIDTH=line_width
         RangeSliderH.BAR_COLOR_INNER=bar_color_inner
         RangeSliderH.BAR_COLOR_OUTTER=bar_color_outer
         RangeSliderH.BAR_RADIUS=bar_radius
         RangeSliderH.BAR_RADIUS_INNER=bar_radius-5
         RangeSliderH.DIGIT_PRECISION=digit_precision
         RangeSliderH.FONT_SIZE=font_size
         RangeSliderH.FONT_FAMILY=font_family
         RangeSliderH.IMAGE_ANCHOR_L=image_anchorL
         RangeSliderH.IMAGE_ANCHOR_R=image_anchorR
         RangeSliderH.LINE_S_COLOR=line_s_color
+        RangeSliderH.STEP_MARKER_COLOR=step_marker_color
+        RangeSliderH.TEXT_COLOR=font_color
         if auto:
             if imageL!=None or imageR!=None:
                 raise Exception("Can't decide if to use auto shape or images!")
             else:
                 critical1=max(max(len(str(min_val)+suffix),len(str(max_val)+suffix))*RangeSliderH.FONT_SIZE*1.33/4,RangeSliderH.BAR_RADIUS)
                 critical2=2*(padX+RangeSliderH.BAR_RADIUS)
                 critical3=2*(1.33*RangeSliderH.FONT_SIZE+RangeSliderH.BAR_RADIUS)
                 if show_value and padX<critical1:
-                    raise Exception("padX too small, value won't be visible completely, expected padX to be atleast "+ str(critical1+1)+"px.")
+                    raise Exception("[padX] too small, value won't be visible completely, expected [padX] to be atleast "+ str(critical1+1)+"px.")
                 if Width<critical2:
-                    raise Exception("Dimensions incompatible, consider decreasing padX or bar_radius or consider increasing widget width, as per given configuration width should be atleast ."+str(critical2+1)+"px.")
+                    raise Exception("Dimensions incompatible, consider decreasing [padX] or [bar_radius] or consider increasing widget [Width], as per given configuration [Width] should be atleast ."+str(critical2+1)+"px.")
                 if Height<critical3:
-                    raise Exception("Dimensions incompatible, consider decreasing bar_radius or consider increasing widget height, as per given configuration height should be atleast ."+str(critical3+1)+"px.")
+                    raise Exception("Dimensions incompatible, consider decreasing [bar_radius] or consider increasing widget [Height], as per given configuration [Height] should be atleast ."+str(critical3+1)+"px.")
                 if RangeSliderH.BAR_RADIUS<=line_width:
-                    raise Exception("bar_radius too small, should be atleast equal to line_width(default=10)")
+                    raise Exception("[bar_radius] too small, should be atleast equal to [line_width] (default=10)")
                 self.draw='auto'
         else:
             if imageL==None or imageR==None:
                 raise Exception("Handle for one image missing.")
             else:
                 critical1=imageL.height()+2*1.33*RangeSliderH.FONT_SIZE
                 critical2=imageR.width()*2+2*padX
                 critical3=max(len(str(min_val)+suffix),len(str(max_val)+suffix))*RangeSliderH.FONT_SIZE*1.33/4
                 if imageL.height()==imageR.height() and imageL.width()==imageR.width():
                     if critical1<Height and critical2< Width:
                         if show_value and padX<critical3:
-                            raise Exception("padX too small, value won't be visible completely, expected padX to be atleast "+str(critical3+1)+"px.")
+                            raise Exception("[padX] too small, value won't be visible completely, expected [padX] to be atleast "+str(critical3+1)+"px.")
                         self.draw='image'
                     else:
-                        raise Exception("Image dimensions not suited with widget Height and width, as per given configuration height should be atleast "+str(critical1+1)+"px and width should be atleast "+str(critical2+1)+"px.")
+                        raise Exception("Image dimensions not suited with widget height and width, as per given configuration [Height] should be atleast "+str(critical1+1)+"px and [Width] should be atleast "+str(critical2+1)+"px.")
                 else:
                     raise Exception("Image dimensions incompatible, both handles should have same height and width respectively.")
         Frame.__init__(self, master, height = Height, width = Width)
+        self.cross_each_other = cross_each_other
         self.padx=padX
         self.ImageL=imageL
         self.ImageR=imageR
         self.master = master
-        self.init_lis = [min_val,max_val]
+        if self.cross_each_other == False:
+            assert variables[0].get() <= variables[1].get(), "Left Handle value is more than the Right Handle Value, which is not possible."
         self.max_val = max_val
         self.min_val = min_val
         self.show_value = show_value
         self.valueSide=valueSide
         self.H = Height
         self.W = Width
         self.canv_H = self.H
         self.canv_W = self.W
         self.suffix=suffix
         self.variables=variables
+        self.step_marker = step_marker
+        if self.step_marker:
+            assert step_size > 0, "[step_size] must be provided if [step_marker] set to True."
+        if step_size > 0:
+            self.init_lis = [(variables[0].get()//step_size)*step_size,
+                            (variables[1].get()//step_size)*step_size]
+        else:
+            self.init_lis = [variables[0].get(),
+                            variables[1].get()]
+        self.step_size= step_size / (self.max_val-self.min_val)
         if not show_value:
             self.slider_y = self.canv_H/2 # y pos of the slider
         else:
             if self.valueSide=='BOTTOM':
                 if self.draw=='auto':
                     self.slider_y = RangeSliderH.BAR_RADIUS+2
                 else:
                     self.slider_y = imageL.height()/2 + 2
             elif self.valueSide=='TOP':
                 if self.draw=='auto':
                     self.slider_y = self.canv_H - RangeSliderH.BAR_RADIUS - 2
                 else:
                     self.slider_y = self.canv_H - imageL.height()/2 - 2
             else:
-                raise Exception("valueSide can either be TOP or BOTTOM.")
+                raise Exception("[valueSide] can either be TOP or BOTTOM.")
         if self.draw=='auto':
             self.slider_x = RangeSliderH.BAR_RADIUS+self.padx # x pos of the slider (left side)
         else:
             self.slider_x = self.ImageL.width()/2+self.padx
-
+        self.L = self.canv_W - 2*self.slider_x
         self.bars = []
         self.selected_idx = None # current selection bar index
         for value in self.init_lis:
             pos = (value-min_val)/(max_val-min_val)
             ids = []
             bar = {"Pos":pos, "Ids":ids, "Value":value}
             self.bars.append(bar)
@@ -124,23 +141,43 @@
         self.__setValues()
 
 
     def getValues(self):
         values = [bar["Value"] for bar in self.bars]
         return values
 
+    def forceValues(self, values):
+        """values needs to be a list of the following format:
+           [first_handle_value, second_handle_value], where first and second are in reference
+           to the variables given, depending on cross_each_other, if cross_each_other is left
+           to default value of False, first refers to left and second refers to right. Both the
+           values should be between min_val and max_val."""
+        assert all([pos >= self.min_val and pos <= self.max_val for pos in values])
+        for idx in range(len(self.bars)):
+            self.__moveBar(idx, (values[idx] - self.min_val)/(self.max_val - self.min_val)) # value = pos*(self.max_val - self.min_val)+self.min_val => pos = (value - self.min_val)/(self.max_val - self.min_val)
+
     def __setValues(self):
         values=self.getValues()
         self.variables[0].set(values[0])
         self.variables[1].set(values[1])
 
     def getPos(self):
         poss = [bar["Pos"] for bar in self.bars]
         return poss
 
+    def forcePos(self, pos):
+        """pos needs to be a list of the following format:
+           [first_handle_value, second_handle_value], where first and second are in reference
+           to the variables given, depending on cross_each_other, if cross_each_other is left
+           to default value of False, first refers to left and second refers to right. Both the
+           values should be between 0 and 1."""
+        assert all([pos >= 0 and pos <= 1 for pos in pos])
+        for idx in range(len(self.bars)):
+            self.__moveBar(idx, pos[idx])
+
     def _mouseMotion(self, event):
         x = event.x; y = event.y
         selection = self.__checkSelection(x,y)
         if selection[0]:
             self.canv.config(cursor = "hand2")
             self.selected_idx = selection[1]
         else:
@@ -151,31 +188,47 @@
         x = event.x; y = event.y
         if self.selected_idx == None:
             return False
         pos = self.__calcPos(x)
         idx = self.selected_idx
         self.__moveBar(idx,pos)
 
+    def __addStepMarker(self):
+        numberOfMarkers = int((1 // self.step_size)) + 1
+        markerXs = [self.slider_x + i*(self.step_size * self.L) for i in range(numberOfMarkers)]
+        R = self.LINE_WIDTH/2
+        markerIDs = [self.canv.create_line(mX,self.slider_y-R,mX,self.slider_y+R, fill = RangeSliderV.STEP_MARKER_COLOR) for mX in markerXs]
+        return (markerIDs)
+
     def __addTrack(self, startx, starty, endx, endy, posL, posR):
         rangeOutL = self.canv.create_line(startx, starty, startx+posL*(endx-startx), endy, fill = RangeSliderH.LINE_COLOR, width = RangeSliderH.LINE_WIDTH)
         rangeS = self.canv.create_line(startx+posL*(endx-startx), starty, endx-(1-posR)*(endx-startx), endy, fill = RangeSliderH.LINE_S_COLOR, width = RangeSliderH.LINE_WIDTH)
         rangeOutR = self.canv.create_line(endx-(1-posR)*(endx-startx), starty, endx, endy, fill = RangeSliderH.LINE_COLOR, width = RangeSliderH.LINE_WIDTH)
-        return [rangeOutL, rangeS, rangeOutR]
+        if self.step_marker:
+            markerIDs = self.__addStepMarker()
+            return [rangeOutL, rangeS, rangeOutR, markerIDs]
+        return [rangeOutL, rangeS, rangeOutR, []]
 
     def __addTrackL(self, startx, starty, endx, endy, posL, posR):
         rangeOutL = self.canv.create_line(startx, starty, startx+posL*(endx-startx), endy, fill = RangeSliderH.LINE_COLOR, width = RangeSliderH.LINE_WIDTH)
         rangeS = self.canv.create_line(startx+posL*(endx-startx), starty, endx-(1-posR)*(endx-startx), endy, fill = RangeSliderH.LINE_S_COLOR, width = RangeSliderH.LINE_WIDTH)
         # rangeOutR = self.canv.create_line(endx-(1-posR)*(endx-startx), starty, endx, endy, fill = RangeSliderH.LINE_COLOR, width = RangeSliderH.LINE_WIDTH)
-        return [rangeOutL, rangeS]
+        if self.step_marker:
+            markerIDs = self.__addStepMarker()
+            return [rangeOutL, rangeS, markerIDs]
+        return [rangeOutL, rangeS, []]
 
     def __addTrackR(self, startx, starty, endx, endy, posL, posR):
         # rangeOutL = self.canv.create_line(startx, starty, startx+posL*(endx-startx), endy, fill = RangeSliderH.LINE_COLOR, width = RangeSliderH.LINE_WIDTH)
         rangeS = self.canv.create_line(startx+posL*(endx-startx), starty, endx-(1-posR)*(endx-startx), endy, fill = RangeSliderH.LINE_S_COLOR, width = RangeSliderH.LINE_WIDTH)
         rangeOutR = self.canv.create_line(endx-(1-posR)*(endx-startx), starty, endx, endy, fill = RangeSliderH.LINE_COLOR, width = RangeSliderH.LINE_WIDTH)
-        return [rangeS, rangeOutR]
+        if self.step_marker:
+            markerIDs = self.__addStepMarker()
+            return [rangeS, rangeOutR, markerIDs]
+        return [rangeS, rangeOutR, []]
 
     def __addBar(self, pos, tempIdx=None):
         """@ pos: position of the bar, ranged from (0,1)"""
         if pos <0 or pos >1:
             raise Exception("Pos error - Pos: "+str(pos))
         if self.draw=='auto':
             R = RangeSliderH.BAR_RADIUS
@@ -185,19 +238,19 @@
             x = self.slider_x+pos*L
             id_outer = self.canv.create_oval(x-R,y-R,x+R,y+R, fill = RangeSliderH.BAR_COLOR_OUTTER, width = 2, outline = "")
             id_inner = self.canv.create_oval(x-r,y-r,x+r,y+r, fill = RangeSliderH.BAR_COLOR_INNER, outline = "")
             if self.show_value:
                 if self.valueSide=='TOP':
                     y_value = y-RangeSliderH.BAR_RADIUS-RangeSliderH.FONT_SIZE/2
                     value = pos*(self.max_val - self.min_val)+self.min_val
-                    id_value = self.canv.create_text(x,y_value,anchor=S, text = format(value, RangeSliderH.DIGIT_PRECISION)+self.suffix,font=(RangeSliderH.FONT_FAMILY,RangeSliderH.FONT_SIZE))
+                    id_value = self.canv.create_text(x,y_value,anchor=S, text = format(value, RangeSliderH.DIGIT_PRECISION)+self.suffix,font=(RangeSliderH.FONT_FAMILY,RangeSliderH.FONT_SIZE), fill = RangeSliderH.TEXT_COLOR)
                 elif self.valueSide=='BOTTOM':
                     y_value = y+RangeSliderH.BAR_RADIUS+RangeSliderH.FONT_SIZE/2
                     value = pos*(self.max_val - self.min_val)+self.min_val
-                    id_value = self.canv.create_text(x,y_value,anchor=N, text = format(value, RangeSliderH.DIGIT_PRECISION)+self.suffix,font=(RangeSliderH.FONT_FAMILY,RangeSliderH.FONT_SIZE))
+                    id_value = self.canv.create_text(x,y_value,anchor=N, text = format(value, RangeSliderH.DIGIT_PRECISION)+self.suffix,font=(RangeSliderH.FONT_FAMILY,RangeSliderH.FONT_SIZE), fill = RangeSliderH.TEXT_COLOR)
                 else:
                     raise Exception("valueSide can either be TOP or BOTTOM")
                 return [id_outer, id_inner, id_value]
             else:
                 return [id_outer, id_inner]
         elif self.draw=='image':
             L=self.canv_W - 2*self.slider_x
@@ -207,19 +260,19 @@
                 imageH=self.canv.create_image(x,y,anchor=RangeSliderH.IMAGE_ANCHOR_L,image=self.ImageL)
             elif tempIdx==1:
                 imageH=self.canv.create_image(x,y,anchor=RangeSliderH.IMAGE_ANCHOR_R,image=self.ImageR)
             if self.show_value:
                 if self.valueSide=='TOP':
                     y_value = y-self.ImageL.height()/2-RangeSliderH.FONT_SIZE/2
                     value = pos*(self.max_val - self.min_val)+self.min_val
-                    id_value = self.canv.create_text(x,y_value,anchor=S, text = format(value, RangeSliderH.DIGIT_PRECISION)+self.suffix,font=(RangeSliderH.FONT_FAMILY,RangeSliderH.FONT_SIZE))
+                    id_value = self.canv.create_text(x,y_value,anchor=S, text = format(value, RangeSliderH.DIGIT_PRECISION)+self.suffix,font=(RangeSliderH.FONT_FAMILY,RangeSliderH.FONT_SIZE), fill = RangeSliderH.TEXT_COLOR)
                 elif self.valueSide=='BOTTOM':
                     y_value = y+self.ImageL.height()/2+RangeSliderH.FONT_SIZE/2
                     value = pos*(self.max_val - self.min_val)+self.min_val
-                    id_value = self.canv.create_text(x,y_value,anchor=N, text = format(value, RangeSliderH.DIGIT_PRECISION)+self.suffix,font=(RangeSliderH.FONT_FAMILY,RangeSliderH.FONT_SIZE))
+                    id_value = self.canv.create_text(x,y_value,anchor=N, text = format(value, RangeSliderH.DIGIT_PRECISION)+self.suffix,font=(RangeSliderH.FONT_FAMILY,RangeSliderH.FONT_SIZE), fill = RangeSliderH.TEXT_COLOR)
                 else:
                     raise Exception("valueSide can either be TOP or BOTTOM")
                 return [imageH, id_value]
             else:
                 return [imageH]
 
 
@@ -228,44 +281,51 @@
         current_pos=self.bars[idx]["Pos"]
         for i in range(0,2):
             ids=self.bars[i]["Ids"]
             for id in ids:
                 self.canv.delete(id)
         for trackComponentsId in self.track[idx:idx+2]:
             self.canv.delete(trackComponentsId)
+        for trackComponentsId in self.track[-1]:
+            self.canv.delete(trackComponentsId)
         if idx==0:
             otherIdx=1
             otherPos=positions[1]
-            if pos<=otherPos:
-                pos=pos
-            else:
-                pos=current_pos
-            self.track[0:2] = self.__addTrackL(self.slider_x, self.slider_y, self.canv_W-self.slider_x, self.slider_y, pos, otherPos)
+            if self.cross_each_other == False:
+                if pos<=otherPos:
+                    pos=pos
+                else:
+                    pos=current_pos
+            self.track[0], self.track[1], self.track[-1] = self.__addTrackL(self.slider_x, self.slider_y, self.canv_W-self.slider_x, self.slider_y, pos, otherPos)
         else:
             otherIdx=0
             otherPos=positions[0]
-            if pos>=otherPos:
-                pos=pos
-            else:
-                pos=current_pos
-            self.track[1:3] = self.__addTrackR(self.slider_x, self.slider_y, self.canv_W-self.slider_x, self.slider_y, otherPos, pos)
+            if self.cross_each_other == False:
+                if pos>=otherPos:
+                    pos=pos
+                else:
+                    pos=current_pos
+            self.track[1], self.track[2], self.track[-1] = self.__addTrackR(self.slider_x, self.slider_y, self.canv_W-self.slider_x, self.slider_y, otherPos, pos)
         
         self.bars[idx]["Ids"] = self.__addBar(pos, idx)
         self.bars[idx]["Pos"] = pos
         self.bars[idx]["Value"] = pos*(self.max_val - self.min_val)+self.min_val
 
         self.bars[otherIdx]["Ids"] = self.__addBar(otherPos, otherIdx)
         self.bars[otherIdx]["Pos"] = otherPos
         self.bars[otherIdx]["Value"] = otherPos*(self.max_val - self.min_val)+self.min_val
 
         self.__setValues()
 
     def __calcPos(self, x):
         """calculate position from x coordinate"""
-        pos = (x - self.slider_x)/(self.canv_W-2*self.slider_x)
+        pos = (x - self.slider_x)/self.L
+        if self.step_size != 0:
+            css = (pos // self.step_size)
+            pos = (css + 1 * (pos % self.step_size > 0.5)) * self.step_size
         if pos<0:
             return 0
         elif pos>1:
             return 1
         else:
             return pos
 
@@ -297,81 +357,99 @@
     BAR_COLOR_INNER = "#5c8a8a"
     BAR_COLOR_OUTTER = "#c2d6d6"
     BAR_RADIUS = 10
     BAR_RADIUS_INNER = 5
     DIGIT_PRECISION = '.1f' # for showing in the canvas
     FONT_SIZE=16
     FONT_FAMILY='Times'
+    TEXT_COLOR='#000000'
     IMAGE_ANCHOR_L=CENTER
     IMAGE_ANCHOR_U=CENTER
+    STEP_MARKER_COLOR='#ffffff'
     def __init__(self, master, variables, Width = 80, Height = 400, min_val = 0, max_val = 1, padY=3,
                     image_anchorU=CENTER, image_anchorL=CENTER, imageL=None, imageU=None,
                     auto=True, line_width=3, bar_radius=10,
-                    bar_color_inner='#5c8a8a', line_s_color="#0a50ff", bar_color_outer='#c2d6d6', line_color = '#476b6b', bgColor='#ffffff',
-                    show_value = True, digit_precision='.1f', valueSide='LEFT', font_family='Times', font_size=16, suffix=""):
+                    bar_color_inner='#5c8a8a', line_s_color="#0a50ff", bar_color_outer='#c2d6d6', line_color = '#476b6b', bgColor='#ffffff', step_marker_color = "#ffffff", font_color = '#000000',
+                    show_value = True, digit_precision='.1f', valueSide='LEFT', font_family='Times', font_size=16, suffix="",
+                    step_size = 0, step_marker=False ,cross_each_other = False):
+
         RangeSliderV.LINE_COLOR=line_color
         RangeSliderV.LINE_WIDTH=line_width
         RangeSliderV.BAR_COLOR_INNER=bar_color_inner
         RangeSliderV.BAR_COLOR_OUTTER=bar_color_outer
         RangeSliderV.BAR_RADIUS=bar_radius
         RangeSliderV.BAR_RADIUS_INNER=bar_radius-5
         RangeSliderV.DIGIT_PRECISION=digit_precision
         RangeSliderV.FONT_SIZE=font_size
         RangeSliderV.FONT_FAMILY=font_family
         RangeSliderV.IMAGE_ANCHOR_L=image_anchorL
         RangeSliderV.IMAGE_ANCHOR_U=image_anchorU
         RangeSliderV.LINE_S_COLOR=line_s_color
+        RangeSliderV.STEP_MARKER_COLOR=step_marker_color
+        RangeSliderV.TEXT_COLOR=font_color
         if auto:
             if imageL!=None or imageU!=None:
                 raise Exception("Can't decide if to use auto shape or images!")
             else:
                 critical1=max(RangeSliderV.BAR_RADIUS, RangeSliderV.FONT_SIZE*1.33/2)
                 critical2=2*(RangeSliderV.BAR_RADIUS+max(len(str(min_val)),len(str(max_val)))*RangeSliderV.FONT_SIZE/1.2)
                 critical3=2*(padY+RangeSliderV.BAR_RADIUS)
                 if show_value and padY<critical1:
-                    raise Exception("padY too small, handle won't be visible completely, as per given condition padY should be atleast "+str(critical1+1)+"px.")
+                    raise Exception("[padY] too small, handle won't be visible completely, as per given condition [padY] should be atleast "+str(critical1+1)+"px.")
                 if Width<critical2:
-                    raise Exception("Dimensions incompatible, consider decreasing bar_radius or FONT_SIZE or consider increasing widget width, as per given conditios width should be atleast "+str(critical2+1)+"px.")
+                    raise Exception("Dimensions incompatible, consider decreasing [bar_radius] or [FONT_SIZE] or consider increasing widget [Width], as per given conditios [Width] should be atleast "+str(critical2+1)+"px.")
                 if Height<critical3:
-                    raise Exception("Dimensions incompatible, consider decreasing bar_radius or consider increasing widget height, as per given conditios height should be atleast "+str(critical3+1)+"px.")
+                    raise Exception("Dimensions incompatible, consider decreasing [bar_radius] or consider increasing widget [Height], as per given conditios [Height] should be atleast "+str(critical3+1)+"px.")
                 if RangeSliderV.BAR_RADIUS<=line_width:
-                    raise Exception("bar_radius too small, should be minimum equal to line_width(default=3).")
+                    raise Exception("[bar_radius] too small, should be minimum equal to [line_width] (default=3).")
                 self.draw='auto'
         else:
             if imageL==None or imageU==None:
                 raise Exception("Handle for one image missing.")
             else:
                 critical1=(imageL.height()+padY)*2
                 critical2=imageL.width()+max(len(str(min_val)),len(str(max_val)))*RangeSliderV.FONT_SIZE/1.2
                 critical3=max(imageU.height()/2, RangeSliderV.FONT_SIZE*1.33/2)
                 if imageL.height()==imageU.height() and imageL.width()==imageU.width():
                     if critical1<Height and critical2< Width:
                         if show_value and padY<critical3:
-                            raise Exception("padY too small, value won't be visible completely, padY mimumum expected is "+str(critical3)+"px.")
+                            raise Exception("[padY] too small, value won't be visible completely, [padY] mimumum expected is "+str(critical3)+"px.")
                         self.draw='image'
                     else:
-                        raise Exception("Image dimensions not suited with widget Height and width, minimum height expected is "+str(critical1)+"px and minimum width expected is "+str(critical2)+"px.")
+                        raise Exception("Image dimensions not suited with widget height and width, minimum [Height] expected is "+str(critical1)+"px and minimum [Width] expected is "+str(critical2)+"px.")
                 else:
                     raise Exception("Image dimensions incompatible, width and height of both handles should be same respectively.")
         Frame.__init__(self, master, height = Height, width = Width)
+        self.cross_each_other = cross_each_other
         self.pady=padY
         self.ImageL=imageL
         self.ImageU=imageU
         self.master = master
-        self.init_lis = [min_val,max_val]
+        if self.cross_each_other == False:
+            assert variables[0].get() <= variables[1].get(), "Top Handle value is less than the Bottom Handle Value, which is not possible."
+        self.step_marker = step_marker
+        if self.step_marker:
+            assert step_size > 0, "[step_size] must be provided if [step_marker] set to True."
+        if step_size != 0:
+            self.init_lis = [(variables[0].get()//step_size)*step_size,
+                            (variables[1].get()//step_size)*step_size]
+        else:
+            self.init_lis = [variables[0].get(),
+                            variables[1].get()]
         self.max_val = max_val
         self.min_val = min_val
         self.show_value = show_value
         self.valueSide=valueSide
         self.H = Height
         self.W = Width
         self.canv_H = self.H
         self.canv_W = self.W
         self.suffix=suffix
         self.variables=variables
+        self.step_size= step_size / (self.max_val-self.min_val)
         if not show_value:
             self.slider_x = self.canv_W/2 # y pos of the slider
         else:
             if self.valueSide=='LEFT':
                 if self.draw=='auto':
                     self.slider_x = self.canv_W-RangeSliderV.BAR_RADIUS-2
                 elif self.draw=='image':
@@ -380,15 +458,15 @@
                 if self.draw=='auto':
                     self.slider_x = RangeSliderV.BAR_RADIUS+2
                 else:
                     self.slider_x = self.ImageL.width()/2+2
             else:
                 raise Exception("valueSide can either be LEFT or RIGHT")
         self.slider_y=self.pady
-
+        self.L = self.canv_H - 2*self.slider_y
         self.bars = []
         self.selected_idx = None # current selection bar index
         for value in self.init_lis:
             pos = (value-min_val)/(max_val-min_val)
             ids = []
             bar = {"Pos":pos, "Ids":ids, "Value":value}
             self.bars.append(bar)
@@ -407,23 +485,43 @@
         self.__setValues()
 
 
     def getValues(self):
         values = [bar["Value"] for bar in self.bars]
         return values
 
+    def forceValues(self, values):
+        """values needs to be a list of the following format:
+           [first_handle_value, second_handle_value], where first and second are in reference
+           to the variables given, depending on cross_each_other, if cross_each_other is left
+           to default value of False, first refers to top and second refers to bottom. Both the
+           values should be between min_val and max_val."""
+        assert all([pos >= self.min_val and pos <= self.max_val for pos in values])
+        for idx in range(len(self.bars)):
+            self.__moveBar(idx, (values[idx] - self.min_val)/(self.max_val - self.min_val)) # value = pos*(self.max_val - self.min_val)+self.min_val => pos = (value - self.min_val)/(self.max_val - self.min_val)
+
     def __setValues(self):
         values=self.getValues()
         self.variables[0].set(values[0])
         self.variables[1].set(values[1])
 
     def getPos(self):
         poss = [bar["Pos"] for bar in self.bars]
         return poss
 
+    def forcePos(self, pos):
+        """pos needs to be a list of the following format:
+           [first_handle_value, second_handle_value], where first and second are in reference
+           to the variables given, depending on cross_each_other, if cross_each_other is left
+           to default value of False, first refers to top and second refers to bottom. Both the
+           values should be between 0 and 1."""
+        assert all([pos >= 0 and pos <= 1 for pos in pos])
+        for idx in range(len(self.bars)):
+            self.__moveBar(idx, pos[idx])
+
     def _mouseMotion(self, event):
         x = event.x; y = event.y
         selection = self.__checkSelection(x,y)
         if selection[0]:
             self.canv.config(cursor = "hand2")
             self.selected_idx = selection[1]
         else:
@@ -434,31 +532,47 @@
         x = event.x; y = event.y
         if self.selected_idx == None:
             return False
         pos = self.__calcPos(y)
         idx = self.selected_idx
         self.__moveBar(idx,pos)
 
+    def __addStepMarker(self):
+        numberOfMarkers = int((1 // self.step_size)) + 1
+        markerYs = [self.slider_y + i*(self.step_size * self.L) for i in range(numberOfMarkers)]
+        R = self.LINE_WIDTH/2
+        markerIDs = [self.canv.create_line(self.slider_x-R,mY,self.slider_x+R,mY, fill = RangeSliderV.STEP_MARKER_COLOR) for mY in markerYs]
+        return (markerIDs)
+
     def __addTrack(self, startx, starty, endx, endy, posL, posU):
         rangeOutL = self.canv.create_line(startx, starty+(1-posL)*(endy-starty), startx, endy, fill = RangeSliderV.LINE_COLOR, width = RangeSliderV.LINE_WIDTH)
         rangeS = self.canv.create_line(startx, starty+(1-posU)*(endy-starty), startx, starty+(1-posL)*(endy-starty), fill = RangeSliderV.LINE_S_COLOR, width = RangeSliderV.LINE_WIDTH)
         rangeOutU = self.canv.create_line(startx, starty, endx, starty+(1-posU)*(endy-starty), fill = RangeSliderV.LINE_COLOR, width = RangeSliderV.LINE_WIDTH)
-        return [rangeOutL, rangeS, rangeOutU]
+        if self.step_marker:
+            markerIDs = self.__addStepMarker()
+            return [rangeOutL, rangeS, rangeOutU, markerIDs]
+        return [rangeOutL, rangeS, rangeOutU, []]
 
     def __addTrackL(self, startx, starty, endx, endy, posL, posU):
         rangeOutL = self.canv.create_line(startx, starty+(1-posL)*(endy-starty), startx, endy, fill = RangeSliderV.LINE_COLOR, width = RangeSliderV.LINE_WIDTH)
         rangeS = self.canv.create_line(startx, starty+(1-posU)*(endy-starty), startx, starty+(1-posL)*(endy-starty), fill = RangeSliderV.LINE_S_COLOR, width = RangeSliderV.LINE_WIDTH)
         # rangeOutU = self.canv.create_line(startx, starty, endx, starty+(1-posU)*(endy-starty), fill = RangeSliderV.LINE_COLOR, width = RangeSliderV.LINE_WIDTH)
-        return [rangeOutL, rangeS]
+        if self.step_marker:
+            markerIDs = self.__addStepMarker()
+            return [rangeOutL, rangeS, markerIDs]
+        return [rangeOutL, rangeS, []]
 
     def __addTrackR(self, startx, starty, endx, endy, posL, posU):
         # rangeOutL = self.canv.create_line(startx, starty+(1-posL)*(endy-starty), startx, endy, fill = RangeSliderV.LINE_COLOR, width = RangeSliderV.LINE_WIDTH)
         rangeS = self.canv.create_line(startx, starty+(1-posU)*(endy-starty), startx, starty+(1-posL)*(endy-starty), fill = RangeSliderV.LINE_S_COLOR, width = RangeSliderV.LINE_WIDTH)
         rangeOutU = self.canv.create_line(startx, starty, endx, starty+(1-posU)*(endy-starty), fill = RangeSliderV.LINE_COLOR, width = RangeSliderV.LINE_WIDTH)
-        return [rangeS, rangeOutU]
+        if self.step_marker:
+            markerIDs = self.__addStepMarker()
+            return [rangeS, rangeOutU, markerIDs]
+        return [rangeS, rangeOutU, []]
 
     def __addBar(self, pos, tempIdx=None):
         """@ pos: position of the bar, ranged from (0,1)"""
         if pos <0 or pos >1:
             raise Exception("Pos error - Pos: "+str(pos))
         if self.draw=='auto':
             R = RangeSliderV.BAR_RADIUS
@@ -468,19 +582,19 @@
             x = self.slider_x
             id_outer = self.canv.create_oval(x-R,y-R,x+R,y+R, fill = RangeSliderV.BAR_COLOR_OUTTER, width = 2, outline = "")
             id_inner = self.canv.create_oval(x-r,y-r,x+r,y+r, fill = RangeSliderV.BAR_COLOR_INNER, outline = "")
             if self.show_value:
                 if self.valueSide=='LEFT':
                     x_value = x-RangeSliderV.BAR_RADIUS-RangeSliderV.FONT_SIZE/2
                     value = pos*(self.max_val - self.min_val)+self.min_val
-                    id_value = self.canv.create_text(x_value,y,anchor=E, text = format(value, RangeSliderV.DIGIT_PRECISION)+self.suffix,font=(RangeSliderV.FONT_FAMILY,RangeSliderV.FONT_SIZE))
+                    id_value = self.canv.create_text(x_value,y,anchor=E, text = format(value, RangeSliderV.DIGIT_PRECISION)+self.suffix,font=(RangeSliderV.FONT_FAMILY,RangeSliderV.FONT_SIZE), fill = RangeSliderV.TEXT_COLOR)
                 elif self.valueSide=='RIGHT':
                     x_value = x+RangeSliderV.BAR_RADIUS+RangeSliderV.FONT_SIZE/2
                     value = pos*(self.max_val - self.min_val)+self.min_val
-                    id_value = self.canv.create_text(x_value,y,anchor=W, text = format(value, RangeSliderV.DIGIT_PRECISION)+self.suffix,font=(RangeSliderV.FONT_FAMILY,RangeSliderV.FONT_SIZE))
+                    id_value = self.canv.create_text(x_value,y,anchor=W, text = format(value, RangeSliderV.DIGIT_PRECISION)+self.suffix,font=(RangeSliderV.FONT_FAMILY,RangeSliderV.FONT_SIZE), fill = RangeSliderV.TEXT_COLOR)
                 else:
                     raise Exception("valueSide can either be LEFT or RIGHT.")
                 return [id_outer, id_inner, id_value]
             else:
                 return [id_outer, id_inner]
         elif self.draw=='image':
             L=self.canv_H - 2*self.slider_y
@@ -490,19 +604,19 @@
                 imageH=self.canv.create_image(x,y,anchor=RangeSliderV.IMAGE_ANCHOR_L,image=self.ImageL)
             elif tempIdx==1:
                 imageH=self.canv.create_image(x,y,anchor=RangeSliderV.IMAGE_ANCHOR_U,image=self.ImageU)
             if self.show_value:
                 if self.valueSide=='LEFT':
                     x_value = x-self.ImageL.width()/2-RangeSliderV.FONT_SIZE/2
                     value = pos*(self.max_val - self.min_val)+self.min_val
-                    id_value = self.canv.create_text(x_value,y, anchor=E, text = format(value, RangeSliderV.DIGIT_PRECISION)+self.suffix,font=(RangeSliderV.FONT_FAMILY,RangeSliderV.FONT_SIZE))
+                    id_value = self.canv.create_text(x_value,y, anchor=E, text = format(value, RangeSliderV.DIGIT_PRECISION)+self.suffix,font=(RangeSliderV.FONT_FAMILY,RangeSliderV.FONT_SIZE), fill = RangeSliderV.TEXT_COLOR)
                 elif self.valueSide=='RIGHT':
                     x_value = x+self.ImageL.width()/2+RangeSliderV.FONT_SIZE/2
                     value = pos*(self.max_val - self.min_val)+self.min_val
-                    id_value = self.canv.create_text(x_value,y, anchor=W, text = format(value, RangeSliderV.DIGIT_PRECISION)+self.suffix,font=(RangeSliderV.FONT_FAMILY,RangeSliderV.FONT_SIZE))
+                    id_value = self.canv.create_text(x_value,y, anchor=W, text = format(value, RangeSliderV.DIGIT_PRECISION)+self.suffix,font=(RangeSliderV.FONT_FAMILY,RangeSliderV.FONT_SIZE), fill = RangeSliderV.TEXT_COLOR)
                 else:
                     raise Exception("valueSide can either be LEFT or RIGHT")  
                 return [imageH, id_value]
             else:
                 return [imageH]
 
 
@@ -511,45 +625,52 @@
         current_pos=self.bars[idx]["Pos"]
         for i in range(0,2):
             ids=self.bars[i]["Ids"]
             for id in ids:
                 self.canv.delete(id)
         for trackComponentsId in self.track[idx:idx+2]:
             self.canv.delete(trackComponentsId)
+        for trackComponentsId in self.track[-1]:
+            self.canv.delete(trackComponentsId)
         if idx==0:
             otherIdx=1
             otherPos=positions[1]
-            if pos<=otherPos:
-                pos=pos
-            else:
-                pos=current_pos
-            self.track[0:2] = self.__addTrackL(self.slider_x, self.slider_y, self.slider_x, self.canv_H-self.slider_y, pos, otherPos)
+            if self.cross_each_other == False:
+                if pos<=otherPos:
+                    pos=pos
+                else:
+                    pos=current_pos
+            self.track[0], self.track[1], self.track[-1] = self.__addTrackL(self.slider_x, self.slider_y, self.slider_x, self.canv_H-self.slider_y, pos, otherPos)
         else:
             otherIdx=0
             otherPos=positions[0]
-            if pos>=otherPos:
-                pos=pos
-            else:
-                pos=current_pos
-            self.track[1:3] = self.__addTrackR(self.slider_x, self.slider_y, self.slider_x, self.canv_H-self.slider_y, otherPos, pos)
+            if self.cross_each_other == False:
+                if pos>=otherPos:
+                    pos=pos
+                else:
+                    pos=current_pos
+            self.track[1], self.track[2], self.track[-1] = self.__addTrackR(self.slider_x, self.slider_y, self.slider_x, self.canv_H-self.slider_y, otherPos, pos)
         
         self.bars[idx]["Ids"] = self.__addBar(pos, idx)
         self.bars[idx]["Pos"] = pos
         self.bars[idx]["Value"] = pos*(self.max_val - self.min_val)+self.min_val
 
         self.bars[otherIdx]["Ids"] = self.__addBar(otherPos, otherIdx)
         self.bars[otherIdx]["Pos"] = otherPos
         self.bars[otherIdx]["Value"] = otherPos*(self.max_val - self.min_val)+self.min_val
 
         self.__setValues()
 
     def __calcPos(self, y):
         """calculate position from x coordinate"""
-        pos = (y - self.slider_y)/(self.canv_H-2*self.slider_y)
+        pos = (y - self.slider_y)/self.L
         pos = 1-pos
+        if self.step_size != 0:
+            css = (pos // self.step_size)
+            pos = (css + 1 * (pos % self.step_size > 0.5)) * self.step_size
         if pos<0:
             return 0
         elif pos>1:
             return 1
         else:
             return pos
```

### Comparing `RangeSlider-2021.7.4/setup.py` & `RangeSlider-2023.7.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,29 +2,33 @@
 
 with open("README.md",'r') as fh:
     long_description=fh.read()
 
 setup(
   name = 'RangeSlider',         # How you named your package folder (MyLib)
   packages = ['RangeSlider'],   # Chose the same as "name"
-  version = '2021.7.4',      # Start with a small number and increase it with every change you make
+  version = '2023.07.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Python tkinter widget for range selection in slider widget structure with two handles',   # Give a short description about your library
   author = 'Harsh Agarwal',                   # Type in your name
   author_email = 'harshvinay752@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/harshvinay752/RangeSlider',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/harshvinay752/RangeSlider/archive/refs/tags/2021.7.4.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/harshvinay752/RangeSlider/archive/refs/tags/2023.07.1.tar.gz',    # I explain this later on
   keywords = ['Python','tkinter','range','slider','two handle','selector','widget'],   # Keywords that define your package best
   install_requires=[],
   long_description=long_description,
   long_description_content_type="text/markdown",
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
   ],
 )
```

