# Comparing `tmp/pygame_ui_controls-1.0.3-py3-none-any.whl.zip` & `tmp/pygame_ui_controls-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17995 bytes, number of entries: 7
+Zip file size: 19327 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-14 20:26 __init__.py
--rw-rw-r--  2.0 unx    24038 b- defN 23-Jul-17 18:58 pygame_ui_controls.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Jul-17 19:03 pygame_ui_controls-1.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx      681 b- defN 23-Jul-17 19:03 pygame_ui_controls-1.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-17 19:03 pygame_ui_controls-1.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-17 19:03 pygame_ui_controls-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      584 b- defN 23-Jul-17 19:03 pygame_ui_controls-1.0.3.dist-info/RECORD
-7 files, 60545 bytes uncompressed, 16949 bytes compressed:  72.0%
+-rw-rw-r--  2.0 unx    31046 b- defN 23-Jul-18 19:30 pygame_ui_controls.py
+-rw-rw-r--  2.0 unx    35149 b- defN 23-Jul-18 19:33 pygame_ui_controls-1.1.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      681 b- defN 23-Jul-18 19:33 pygame_ui_controls-1.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-18 19:33 pygame_ui_controls-1.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-18 19:33 pygame_ui_controls-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      584 b- defN 23-Jul-18 19:33 pygame_ui_controls-1.1.0.dist-info/RECORD
+7 files, 67553 bytes uncompressed, 18281 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: __init__.py
 Comment: 
 
 Filename: pygame_ui_controls.py
 Comment: 
 
-Filename: pygame_ui_controls-1.0.3.dist-info/LICENSE
+Filename: pygame_ui_controls-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: pygame_ui_controls-1.0.3.dist-info/METADATA
+Filename: pygame_ui_controls-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pygame_ui_controls-1.0.3.dist-info/WHEEL
+Filename: pygame_ui_controls-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pygame_ui_controls-1.0.3.dist-info/top_level.txt
+Filename: pygame_ui_controls-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pygame_ui_controls-1.0.3.dist-info/RECORD
+Filename: pygame_ui_controls-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pygame_ui_controls.py

```diff
@@ -17,25 +17,24 @@
 class UI:
 
     dict = {}
 
     new_rects = []
     last_rects = []
 
-    focused = None
-
     COLOR_LOCKED = (60, 60, 60), (10, 14, 17), (0, 0, 0)
     COLOR_DOWN = (0, 93, 67), (0, 66, 47), (0, 50, 27)
     COLOR_HOVERED = (93, 67, 0), (66, 47, 0), (50, 27, 0)
     COLOR_CLASSIC = (90, 90, 90), (60, 60, 60), (30, 30, 30)
 
     FONT = None
 
-    pressed = True
+    focused = None
 
+    pressed = True
     clicked_up = False
     clicked_down = False
 
     def __init__(self, name, pos, size, hoverable, locked, on_click=None):
         UI.dict[self.__class__.__name__][name] = self
 
         self.pos = pos
@@ -46,23 +45,26 @@
 
         self.hovered = False
         self.down = False
         self.clicked_up = False
         self.hoverable = hoverable
 
         if on_click:
-            self.on_click = on_click     
+            self.on_click = on_click
 
     def init():
         for subcls in UI.__subclasses__():
             UI.dict[subcls.__name__] = {}
 
     def updated_rects():
         return UI.last_rects + UI.new_rects
 
+    ##########################
+    #  UI ELEMENTS DELETION  #
+    ##########################
     @classmethod
     def delete(cls, *names):
         keys =  UI.dict[cls.__name__].keys()
         for name in names:
             if name in keys:
                 if UI.dict[cls.__name__][name] == UI.focused:
                     UI.focused = None
@@ -74,81 +76,108 @@
             UI.focused = None
         UI.dict[cls.__name__] = {}
 
     def delete_all():
         for cls in UI.__subclasses__():
             UI.dict[cls.__name__] = {}
 
+    #############
+    #  GETTERS  #
+    #############
     @classmethod
     def exists(cls, name):
         return (name in UI.dict[cls.__name__].keys())
 
+    @classmethod
+    def clicked(cls, name):
+        return UI.dict[cls.__name__][name].clicked_up
 
     @classmethod
+    def confirmed(cls, name):
+        return UI.dict[cls.__name__][name].confirmed
+
+    #############
+    #  SETTERS  #
+    #############
+    @classmethod
     def lock(cls, name):
         UI.dict[cls.__name__][name].locked = True
 
     @classmethod
     def unlock(cls, name):
         UI.dict[cls.__name__][name].locked = False
 
     @classmethod
     def set_lock(cls, name, val):
         UI.dict[cls.__name__][name].locked = val
-    
-    @classmethod
-    def clicked(cls, name):
-        return UI.dict[cls.__name__][name].clicked_up
-    
-    @classmethod
-    def confirmed(cls, name):
-        return UI.dict[cls.__name__][name].confirmed
 
     @classmethod
     def set_on_click(cls, name, function):
         UI.dict[cls.__name__][name].on_click = function
 
     @classmethod
     def set_on_confirm(cls, name, function):
         UI.dict[cls.__name__][name].on_click = function
-    
+
     @classmethod
     def set_pos(cls, name, pos):
         UI.dict[cls.__name__][name].pos = pos
         UI.dict[cls.__name__][name].rect = pygame.Rect((pos[0], pos[1]), (UI.dict[cls.__name__][name].size[0], UI.dict[cls.__name__][name].size[1]))
-    
+
     @classmethod
     def set_size(cls, name, size):
         UI.dict[cls.__name__][name].size = size
         UI.dict[cls.__name__][name].rect = pygame.Rect(UI.dict[cls.__name__][name].pos, size)
         UI.dict[cls.__name__][name].appearence = UI.dict[cls.__name__][name].appearences()
 
+    ##############################
+    #  UPDATE AND DRAW ELEMENTS  #
+    ##############################
     def update(surface, x, y, pressed):
         UI.last_rects = UI.new_rects.copy()
         UI.new_rects = []
 
         # Update mouse state
         UI.clicked_down = (pressed and not UI.pressed)
         UI.clicked_up = (not pressed and UI.pressed)
         UI.pressed = pressed
 
         # Update for every item
         for cls in UI.dict:
-            # Avoid removing button while overriding on_click...
+            # Avoid removing button while overriding on_click
             for self in UI.dict[cls].values():
                 self.logic_update(x, y)
                 if self.clicked_up and hasattr(self, 'on_click'):
                     self.on_click()
                 if hasattr(self, 'on_logic_update'):
                     self.on_logic_update(x, y)
                 self.on_update(surface)
-        
+
+        # Remove focus if mouse not pressed
         if not UI.pressed:
             UI.focused = None
 
+    def logic_update(self, x, y):
+        self.clicked_up = False
+        self.hovered = self.rect.collidepoint(x, y)
+
+        if UI.clicked_down and self.hovered:
+            UI.focused = self
+
+        self.down = ((UI.pressed and self.hovered) or (UI.focused == self)) and not self.locked
+
+        self.clicked_up = UI.clicked_up and UI.focused == self and self.hovered and not self.locked
+
+        if UI.focused != None and UI.focused != self:
+            self.hovered = False
+            self.down = False
+
+    ###########
+    #  UTILS  #
+    ###########
     def get_color_from_code(self, val, is_down=False):
         if self.locked:
             return UI.COLOR_LOCKED[val]
         elif self.down or is_down:
             return UI.COLOR_DOWN[val]
         elif self.hovered:
             return UI.COLOR_HOVERED[val]
@@ -160,85 +189,92 @@
 
     def get_second_color(self, is_down=False):
         return self.get_color_from_code(1, is_down)
 
     def get_first_color(self, is_down=False):
         return self.get_color_from_code(0, is_down)
 
-    def logic_update(self, x, y):
-        self.clicked_up = False
-        self.hovered = self.rect.collidepoint(x, y)
-
-        if UI.clicked_down and self.hovered:
-            UI.focused = self
-
-        self.down = ((UI.pressed and self.hovered) or (UI.focused == self)) and not self.locked
-        
-        self.clicked_up = UI.clicked_up and UI.focused == self and self.hovered and not self.locked
-
-        if UI.focused != None and UI.focused != self:
-            self.hovered = False
-            self.down = False
-
 class Button(UI):
+    """
+    ## Parameters
+    - `name`: name of the button
+    - `pos`: position of the button
+    - `size`: size of the button
+    - `text`: text on the button
+    - `hoverable`: if the button is hoverable or not
+    - `locked`: if the button is locked or not
+    - `on_click`: function called when the button is clicked
+
+    ## Setters
+    - `Button.set_text(name, text)`: set the text of the button
+    - `Button.set_hoverable(name, hoverable)`: set if the button is hoverable or not
+
+    ## Example
+    Simple button which prints "Clicked !" when clicked
+    ```python
+    def on_click():
+        print("Clicked !")
+
+    Button("button", (0, 0), (100, 100), "Click me !", on_click=on_click)
+    ```
+    """
 
     thickness = 3
 
     TEXT_COLOR_CLASSIC = (255, 255, 255)
     TEXT_COLOR_LOCKED = (70, 70, 70)
 
     def __init__(self, name, pos, size=(300, 40), text="Button", hoverable=True, locked=False, on_click=None):
         UI.__init__(self, name, pos, size, hoverable, locked, on_click)
         self.appearence = self.appearences()
         self.text = text
 
+    #############
+    #  SETTERS  #
+    #############
+    def set_text(name, text):
+        UI.dict[Button.__name__][name].text = text
+
+    def set_hoverable(name, hoverable):
+        UI.dict[Button.__name__][name].hoverable = hoverable
+
+    ################
+    #  APPEARENCE  #
+    ################
     def appearences(self):
         outer_rect = (0, 0, self.size[0], self.size[1])
         inner_rect = (Button.thickness, Button.thickness, self.size[0] - 2 * Button.thickness, self.size[1] - 2 * Button.thickness)
 
         locked = pygame.Surface(self.size, pygame.SRCALPHA)
         down = pygame.Surface(self.size, pygame.SRCALPHA)
         hovered = pygame.Surface(self.size, pygame.SRCALPHA)
         classic = pygame.Surface(self.size, pygame.SRCALPHA)
 
         pygame.draw.rect(locked, UI.COLOR_LOCKED[0], outer_rect, border_radius=10)
         pygame.draw.rect(locked, UI.COLOR_LOCKED[1], inner_rect, border_radius=8)
-        
+
         pygame.draw.rect(down, UI.COLOR_DOWN[0], outer_rect, border_radius=10)
         pygame.draw.rect(down, UI.COLOR_DOWN[1], inner_rect, border_radius=8)
-        
+
         pygame.draw.rect(hovered, UI.COLOR_HOVERED[0], outer_rect, border_radius=10)
         pygame.draw.rect(hovered, UI.COLOR_HOVERED[1], inner_rect, border_radius=8)
-        
+
         pygame.draw.rect(classic, UI.COLOR_CLASSIC[0], outer_rect, border_radius=10)
         pygame.draw.rect(classic, UI.COLOR_CLASSIC[1], inner_rect, border_radius=8)
 
         locked = locked.convert_alpha()
         down = down.convert_alpha()
         hovered = hovered.convert_alpha()
         classic = classic.convert_alpha()
 
         return {'locked': locked, 'down': down, 'hovered': hovered, 'classic': classic}
 
-    def set_text(name, text):
-        UI.dict[Button.__name__][name].text = text
-    
-    def set_hoverable(name, hoverable):
-        UI.dict[Button.__name__][name].hoverable = hoverable
-    
-    def text_color(self):
-        if self.locked:
-            return Button.TEXT_COLOR_LOCKED
-        return Button.TEXT_COLOR_CLASSIC
-
-    def text_pos(self, text):
-        x, y = self.pos
-        width, height = self.size
-        return (x + width // 2 - text[1].width // 2, y + height // 2 - text[1].height // 2)
-
+    ############
+    #  UPDATE  #
+    ############
     def on_update(self, surface):
         UI.new_rects.append((*self.pos, *self.size))
 
         if self.locked:
             surface.blit(self.appearence['locked'], self.pos)
         elif self.down:
             surface.blit(self.appearence['down'], self.pos)
@@ -246,27 +282,77 @@
             surface.blit(self.appearence['hovered'], self.pos)
         else:
             surface.blit(self.appearence['classic'], self.pos)
 
         text = UI.FONT.render(self.text, self.text_color())
         surface.blit(text[0], self.text_pos(text))
 
+    ###########
+    #  UTILS  #
+    ###########
+    def text_color(self):
+        if self.locked:
+            return Button.TEXT_COLOR_LOCKED
+        return Button.TEXT_COLOR_CLASSIC
+
+    def text_pos(self, text):
+        x, y = self.pos
+        width, height = self.size
+        return (x + width // 2 - text[1].width // 2, y + height // 2 - text[1].height // 2)
+
 
 class ImageButton(UI):
+    """
+    ## Parameters
+    - `name`: name of the button
+    - `path`: path to the image
+    - `pos`: position of the button
+    - `size` (optional): size of the button
+    - `hoverable` (optional): if the button is hoverable or not
+    - `locked` (optional): if the button is locked or not
+    - `on_click` (optional): function to call when the button is clicked
+
+    ## Setters
+    - `Image_Button.set_image(name, path)`: change the image of the button from the path
+    - `Image_Button.set_hoverable(name, hoverable)`: set the hoverable state of the button
+
+    ## Example
+    Simple image button which prints "Button clicked" when clicked
+    ```python
+    def on_click():
+        print("Button clicked")
+
+    ImageButton("button_id", "path/to/image.png", (0, 0), size=(50, 50), hoverable=True, locked=False, on_click=on_click)
+    ```
+    """
 
     thickness = 3
     extern_thickness = 2
     intern_thickness = 2
 
     def __init__(self, name, path, pos, size=(50, 50), hoverable=True, locked=False, on_click=None):
         UI.__init__(self, name, pos, size, hoverable, locked, on_click=on_click)
 
         self.path = path
         self.appearence = self.appearences()
 
+    #############
+    #  SETTERS  #
+    #############
+    def set_image(name, path):
+        self = UI.dict[ImageButton.__name__][name]
+        self.path = path
+        self.appearence = self.appearences()
+
+    def set_hoverable(name, hoverable):
+        UI.dict[ImageButton.__name__][name].hoverable = hoverable
+
+    ################
+    #  APPEARENCE  #
+    ################
     def appearences(self):
         self.set_image_data()
 
         outer_rect = (0, 0, self.size[0], self.size[1])
         inner_rect = (ImageButton.thickness, ImageButton.thickness, self.size[0] - 2 * ImageButton.thickness, self.size[1] - 2 * ImageButton.thickness)
 
         locked = pygame.Surface(self.size, pygame.SRCALPHA)
@@ -276,40 +362,58 @@
 
         pygame.draw.rect(locked, UI.COLOR_LOCKED[0], outer_rect, border_radius=10)
         pygame.draw.rect(locked, UI.COLOR_LOCKED[1], inner_rect, border_radius=8)
         locked.blit(self.image, self.im_pos)
         mask = pygame.Surface(self.mask_size, pygame.SRCALPHA)
         pygame.draw.rect(mask, (10, 14, 17, 120), self.mask_rect, border_radius=8)
         locked.blit(mask, self.mask_pos)
-        
+
         pygame.draw.rect(down, UI.COLOR_DOWN[0], outer_rect, border_radius=10)
         pygame.draw.rect(down, UI.COLOR_DOWN[1], inner_rect, border_radius=8)
         down.blit(self.image, self.im_pos)
         mask = pygame.Surface(self.mask_size, pygame.SRCALPHA)
         pygame.draw.rect(mask, (255, 255, 255, 40), self.mask_rect, border_radius=8)
         down.blit(mask, self.mask_pos)
-        
+
         pygame.draw.rect(hovered, UI.COLOR_HOVERED[0], outer_rect, border_radius=10)
         pygame.draw.rect(hovered, UI.COLOR_HOVERED[1], inner_rect, border_radius=8)
         hovered.blit(self.image, self.im_pos)
         mask = pygame.Surface(self.mask_size, pygame.SRCALPHA)
         pygame.draw.rect(mask, (255, 255, 255, 20), self.mask_rect, border_radius=8)
         hovered.blit(mask, self.mask_pos)
-        
+
         pygame.draw.rect(classic, UI.COLOR_CLASSIC[0], outer_rect, border_radius=10)
         pygame.draw.rect(classic, UI.COLOR_CLASSIC[1], inner_rect, border_radius=8)
         classic.blit(self.image, self.im_pos)
 
         locked = locked.convert_alpha()
         down = down.convert_alpha()
         hovered = hovered.convert_alpha()
         classic = classic.convert_alpha()
 
         return {'locked': locked, 'down': down, 'hovered': hovered, 'classic': classic}
 
+    ############
+    #  UPDATE  #
+    ############
+    def on_update(self, surface):
+        UI.new_rects.append((*self.pos, *self.size))
+
+        if self.locked:
+            surface.blit(self.appearence['locked'], self.pos)
+        elif self.down:
+            surface.blit(self.appearence['down'], self.pos)
+        elif self.hovered and self.hoverable:
+            surface.blit(self.appearence['hovered'], self.pos)
+        else:
+            surface.blit(self.appearence['classic'], self.pos)
+
+    ###########
+    #  UTILS  #
+    ###########
     def set_image_data(self):
         thickness, intern_thickness, extern_thickness = ImageButton.thickness, ImageButton.intern_thickness, ImageButton.extern_thickness
 
         max_width = self.size[0] - 2 * thickness - 2 * intern_thickness - 2 * extern_thickness
         max_height = self.size[1] - 2 * thickness - 2 * intern_thickness - 2 * extern_thickness
 
         default_width, default_height = get_image_size(self.path)
@@ -317,44 +421,55 @@
 
         if default_width / max_width > default_height / max_height:
             width = max_width
             height = default_height * width / default_width
         else:
             height = max_height
             width = default_width * height / default_height
-        
+
         self.image = get_image((width, height), self.path)
         self.im_pos = (self.size[0] // 2 - width // 2, self.size[1] // 2 - height // 2)
 
-        self.mask_size = (self.size[0] - 2 * thickness - 2 * extern_thickness, self.size[1] - 2 * thickness - 2 * extern_thickness)   
-        self.mask_rect = (0, 0, *self.mask_size)     
+        self.mask_size = (self.size[0] - 2 * thickness - 2 * extern_thickness, self.size[1] - 2 * thickness - 2 * extern_thickness)
+        self.mask_rect = (0, 0, *self.mask_size)
         self.mask_pos = (thickness + extern_thickness, thickness + extern_thickness)
-        
-    def set_image(name, path):
-        self = UI.dict[ImageButton.__name__][name]
-        self.path = path
-        self.appearence = self.appearences()
-    
-    def set_hoverable(name, hoverable):
-        UI.dict[ImageButton.__name__][name].hoverable = hoverable
-
-    def on_update(self, surface):
-        UI.new_rects.append((*self.pos, *self.size))
-
-        if self.locked:
-            surface.blit(self.appearence['locked'], self.pos)
-        elif self.down:
-            surface.blit(self.appearence['down'], self.pos)
-        elif self.hovered and self.hoverable:
-            surface.blit(self.appearence['hovered'], self.pos)
-        else:
-            surface.blit(self.appearence['classic'], self.pos)
 
 
 class Slider(UI):
+    """
+    ## Parameters
+    - `name`: name of the slider
+    - `pos`: position of the slider
+    - `size`: size of the slider
+    - `hoverable` (optional): whether the slider is hoverable or not
+    - `locked` (optional): whether the slider is locked or not
+    - `value` (optional): initial value of the slider
+    - `range` (optional): range of the slider (min, max)
+    - `ticks` (optional): number of ticks of the slider, default is continuous
+    - `step` (optional): step of the slider, default is continuous
+    - `on_value_changed` (optional): function called when the value of the slider changes
+
+    ## Setters
+    - `Slider.set_lock(locked)`: sets whether the slider is locked or not
+    - `Slider.set_hoverable(hoverable)`: sets whether the slider is hoverable or not
+    - `Slider.set_value(value)`: sets the current value of the slider
+    - `Slider.set_min(value)`: sets the minimum value of the slider
+    - `Slider.set_max(value)`: sets the maximum value of the slider
+    - `Slider.set_step(value)`: sets the step of the slider
+    - `Slider.set_ticks(value)`: sets the number of ticks of the slider
+
+    ## Example
+    Simple slider which prints its value when it changes:
+    ```python
+    def on_value_changed(value):
+        print(value)
+
+    Slider("slider_id", (100, 100), (200, 50), value=5, range=(0, 10), ticks=10, on_value_changed=on_value_changed)
+    ```
+    """
 
     thickness = 3
 
     tick_width = 1
 
     COLOR_TICK = (200, 200, 200)
     COLOR_LOCKED_TICK = (20, 28, 36)
@@ -369,94 +484,96 @@
         # Either specify number of ticks, or a step, or nothing for continuous
         self.ticks = ticks
         self.step = 0
         if ticks > 0:
             self.step = (self.max - self.min) / ticks
         elif step > 0:
             self.step = step
-        
+
         self.radius = (size[1] - 2 * Slider.thickness) / 2
         self.center_width = self.size[0] - 2 * self.radius - 2 * Slider.thickness
 
         if range[0] > value or range[1] < value:
             value = range[1]
         self.value = value
-        
+
         self.appearence = self.appearences()
 
+    ###############
+    #   SETTERS   #
+    ###############
+    def set_lock(name, locked):
+        UI.dict[Slider.__name__][name].locked = locked
+
+    def set_hoverable(name, hoverable):
+        UI.dict[Slider.__name__][name].hoverable = hoverable
+
+    def set_step(name, value):
+        UI.dict[Slider.__name__][name].step = value
+
+    def set_ticks(name, value):
+        UI.dict[Slider.__name__][name].ticks = value
+
+    def set_value(name, value):
+        for key in UI.dict[Slider.__name__]:
+            if key != name:
+                continue
+            self = UI.dict[Slider.__name__][name]
+            current_val = self.value
+            if current_val == value:
+                break
+            self.value = value
+            if hasattr(self, 'on_value_changed'):
+                self.on_value_changed(value)
+
+    def set_min(name, value):
+        UI.dict[Slider.__name__][name].min = value
+
+    def set_max(name, value):
+        UI.dict[Slider.__name__][name].max = value
+
+    ##################
+    #   APPEARENCE   #
+    ##################
     def appearences(self):
         radius = int(self.radius)
 
         outer_rect = (0, 0, *self.size)
         inner_rect = (Slider.thickness, Slider.thickness, self.size[0] - 2 * Slider.thickness, self.size[1] - 2 * Slider.thickness)
 
         locked = pygame.Surface(self.size, pygame.SRCALPHA)
         down = pygame.Surface(self.size, pygame.SRCALPHA)
         hovered = pygame.Surface(self.size, pygame.SRCALPHA)
         classic = pygame.Surface(self.size, pygame.SRCALPHA)
 
         pygame.draw.rect(locked, UI.COLOR_LOCKED[0], outer_rect, border_radius=radius)
         pygame.draw.rect(locked, UI.COLOR_LOCKED[1], inner_rect, border_radius=radius)
-        
+
         pygame.draw.rect(down, UI.COLOR_DOWN[0], outer_rect, border_radius=radius)
         pygame.draw.rect(down, UI.COLOR_DOWN[1], inner_rect, border_radius=radius)
-        
+
         pygame.draw.rect(hovered, UI.COLOR_HOVERED[0], outer_rect, border_radius=radius)
         pygame.draw.rect(hovered, UI.COLOR_HOVERED[1], inner_rect, border_radius=radius)
-        
+
         pygame.draw.rect(classic, UI.COLOR_CLASSIC[0], outer_rect, border_radius=radius)
         pygame.draw.rect(classic, UI.COLOR_CLASSIC[1], inner_rect, border_radius=radius)
 
         locked = locked.convert_alpha()
         down = down.convert_alpha()
         hovered = hovered.convert_alpha()
         classic = classic.convert_alpha()
 
         return {'locked': locked, 'down': down, 'hovered': hovered, 'classic': classic}
 
-    def update_value(self, x):
-        x = x - self.pos[0] - self.radius - Slider.thickness
-        val = self.min + x * (self.max - self.min) / self.center_width
-
-        previous = self.value
-        if self.ticks or self.step:
-            self.value = min(self.max, max(self.min, self.nearest_value(val)))
-        else:
-            self.value = min(self.max, max(self.min, val))
-        
-        if self.value != previous and hasattr(self, 'on_value_changed'):
-            self.on_value_changed(self.value)
-
-    def set_value(name, value):
-        for key in UI.dict[Slider.__name__]:
-            if key != name:
-                continue
-            self = UI.dict[Slider.__name__][name]
-            current_val = self.value
-            if current_val == value:
-                break
-            self.value = value
-            if hasattr(self, 'on_value_changed'):
-                self.on_value_changed(value)
-
-    def nearest_value(self, val):
-        k = round((val - self.min) / self.step)
-        return self.min + k * self.step
-
-    def get_button_pos(self):
-        val = (self.value - self.min) * self.center_width / (self.max - self.min)
-        return self.pos[0] + Slider.thickness + self.radius + val
-
-    def get_tick_color(self, tick_value):
-        if tick_value > self.value:
-            if self.locked:
-                return Slider.COLOR_LOCKED_TICK
-            return Slider.COLOR_TICK
-        else:
-            return self.get_second_color()
+    ##############
+    #   UPDATE   #
+    ##############
+    def on_logic_update(self, x, y):
+        if self == UI.focused and not self.locked:
+            self.update_value(x)
 
     def display(self, surface):
         x = self.get_button_pos()
 
         if self.value != self.min:
             pygame.draw.rect(surface, self.get_third_color(), (self.pos[0] + Slider.thickness, self.pos[1] + Slider.thickness, x - self.pos[0] - Slider.thickness, self.size[1] - 2 * Slider.thickness),
                              border_bottom_left_radius=int(self.radius), border_top_left_radius=int(self.radius))
@@ -470,18 +587,14 @@
                     self.pos[0] + pos, self.pos[1] + self.size[1] - Slider.thickness-1), width=Slider.tick_width)
 
         pygame.draw.circle(surface, Slider.COLOR_BUTTON_SIDE,
                            (x, self.pos[1] + self.size[1] / 2), self.radius)
         pygame.draw.circle(surface, self.get_first_color(),
                            (x, self.pos[1] + self.size[1] / 2), self.radius - 2)
 
-    def on_logic_update(self, x, y):
-        if self == UI.focused and not self.locked:
-            self.update_value(x)
-
     def on_update(self, surface):
         rect = (*self.pos, *self.size)
         UI.new_rects.append(rect)
 
         if self.locked:
             surface.blit(self.appearence['locked'], (rect[0], rect[1]))
         elif self.down:
@@ -489,16 +602,85 @@
         elif self.hovered and self.hoverable:
             surface.blit(self.appearence['hovered'], (rect[0], rect[1]))
         else:
             surface.blit(self.appearence['classic'], (rect[0], rect[1]))
 
         self.display(surface)
 
+    ###########
+    #  UTILS  #
+    ###########
+    def update_value(self, x):
+        x = x - self.pos[0] - self.radius - Slider.thickness
+        val = self.min + x * (self.max - self.min) / self.center_width
+
+        previous = self.value
+        if self.ticks or self.step:
+            self.value = min(self.max, max(self.min, self.nearest_value(val)))
+        else:
+            self.value = min(self.max, max(self.min, val))
+
+        if self.value != previous and hasattr(self, 'on_value_changed'):
+            self.on_value_changed(self.value)
+
+    def nearest_value(self, val):
+        k = round((val - self.min) / self.step)
+        return self.min + k * self.step
+
+    def get_button_pos(self):
+        val = (self.value - self.min) * self.center_width / (self.max - self.min)
+        return self.pos[0] + Slider.thickness + self.radius + val
+
+    def get_tick_color(self, tick_value):
+        if tick_value > self.value:
+            if self.locked:
+                return Slider.COLOR_LOCKED_TICK
+            return Slider.COLOR_TICK
+        else:
+            return self.get_second_color()
+
 
 class CheckBox(UI):
+    """
+    ## Parameters
+    - `name`: name of the checkbox
+    - `pos`: position of the checkbox
+    - `size` (optional): size of the checkbox
+    - `checked` (optional): whether the checkbox is checked or not
+    - `hoverable` (optional): whether the checkbox is hoverable or not
+    - `locked` (optional): whether the checkbox is locked or not
+    - `linked` (optional): list of the names of the checkboxes linked to this one (itself included)
+    - `on_check` (optional): function called when the checkbox is checked
+    - `on_uncheck` (optional): function called when the checkbox is unchecked
+    - `on_action` (optional): function called when the checkbox state is changed
+
+    ## Getters
+    - `CheckBox.checked()`: returns the current state of the checkbox
+
+    ## Setters
+    - `CheckBox.uncheck()`: unchecks the checkbox
+    - `CheckBox.check()`: checks the checkbox
+    - `CheckBox.set_check(checked)`: sets the checkbox state to `checked`
+
+    ## Example
+    Simple checkbox which prints "checked" when checked, "unchecked" when unchecked
+    and "action" when the state is changed
+    ```python
+    def on_check():
+        print("checked")
+
+    def on_uncheck():
+        print("unchecked")
+
+    def on_action():
+        print("action")
+
+    CheckBox("checkbox_id", (100, 100), checked=True, on_check=on_check, on_uncheck=on_uncheck, on_action=on_action)
+    print(CheckBox.checked("checkbox_id")) # True
+    """
 
     thickness = 3
     border_radius = 4
 
     COLOR_BUTTON_SIDE = (10, 14, 18)
 
     def __init__(self, name, pos, size=30, checked=False, hoverable=True, locked=False, linked=None, on_check=None, on_uncheck=None, on_action=None):
@@ -518,59 +700,106 @@
             self.linked = tmp
         self.is_linked = (linked != None)
 
         self.setup_pos()
 
         self.appearence = self.appearences()
 
+    #############
+    #  GETTERS  #
+    #############
+    def checked(name):
+        return UI.dict[CheckBox.__name__][name].checked
+
+    #############
+    #  SETTERS  #
+    #############
+    def uncheck(name):
+        UI.dict[CheckBox.__name__][name].checked = False
+
+    def check(name):
+        UI.dict[CheckBox.__name__][name].checked = True
+
+    def set_checked(self, checked):
+        if checked:
+            self.check()
+        else:
+            self.uncheck()
+
+    ################
+    #  APPEARENCE  #
+    ################
     def appearences(self):
         radius = CheckBox.border_radius
 
         outer_rect = (0, 0, *self.size)
         inner_rect = (CheckBox.thickness, CheckBox.thickness, self.size[0] - 2 * CheckBox.thickness, self.size[1] - 2 * CheckBox.thickness)
 
         locked = pygame.Surface(self.size, pygame.SRCALPHA)
         down = pygame.Surface(self.size, pygame.SRCALPHA)
         hovered = pygame.Surface(self.size, pygame.SRCALPHA)
         classic = pygame.Surface(self.size, pygame.SRCALPHA)
 
         pygame.draw.rect(locked, UI.COLOR_LOCKED[0], outer_rect, border_radius=radius)
         pygame.draw.rect(locked, UI.COLOR_LOCKED[1], inner_rect, border_radius=radius)
-        
+
         pygame.draw.rect(down, UI.COLOR_DOWN[0], outer_rect, border_radius=radius)
         pygame.draw.rect(down, UI.COLOR_DOWN[1], inner_rect, border_radius=radius)
-        
+
         pygame.draw.rect(hovered, UI.COLOR_HOVERED[0], outer_rect, border_radius=radius)
         pygame.draw.rect(hovered, UI.COLOR_HOVERED[1], inner_rect, border_radius=radius)
-        
+
         pygame.draw.rect(classic, UI.COLOR_CLASSIC[0], outer_rect, border_radius=radius)
         pygame.draw.rect(classic, UI.COLOR_CLASSIC[1], inner_rect, border_radius=radius)
 
         locked = locked.convert_alpha()
         down = down.convert_alpha()
         hovered = hovered.convert_alpha()
         classic = classic.convert_alpha()
 
         return {'locked': locked, 'down': down, 'hovered': hovered, 'classic': classic}
 
-    def setup_pos(self):
-        self.tick_center = (self.pos[0] + self.size[0] / 2, self.pos[1] + self.size[0] / 2)
+    ############
+    #  UPDATE  #
+    ############
+    def on_update(self, surface):
+        rect = (*self.pos, *self.size)
+        UI.new_rects.append(rect)
+
+        if self.locked:
+            surface.blit(self.appearence['locked'], self.pos)
+        elif self.down or self.checked:
+            surface.blit(self.appearence['down'], self.pos)
+        elif self.hovered and self.hoverable:
+            surface.blit(self.appearence['hovered'], self.pos)
+        else:
+            surface.blit(self.appearence['classic'], self.pos)
+
+        if self.checked:
+            pygame.draw.circle(surface, CheckBox.COLOR_BUTTON_SIDE, self.tick_center, (self.size[0] - 2 * CheckBox.thickness - 4) / 2)
+            pygame.draw.circle(surface, self.get_first_color(is_down=self.checked), self.tick_center, (self.size[0] - 2 * CheckBox.thickness - 4) / 2 - 2)
 
     def on_logic_update(self, x, y):
         if self.clicked_up:
             self.checked = not self.checked
             if self.is_linked:
                 self.update_linked()
             if self.checked and hasattr(self, 'on_check'):
                 self.on_check()
             if not self.checked and hasattr(self, 'on_uncheck'):
                 self.on_uncheck()
             if hasattr(self, 'on_action'):
                 self.on_action(self.checked)
-    
+
+    ###########
+    #  UTILS  #
+    ###########
+    def setup_pos(self):
+        self.tick_center = (self.pos[0] + self.size[0] / 2, self.pos[1] + self.size[0] / 2)
+
     def uncheck_others(self):
         for name in self.linked:
             UI.dict[CheckBox.__name__][name].checked = False
 
     def checkable(self):
         for name in self.linked:
             if UI.dict[CheckBox.__name__][name].checked:
@@ -580,76 +809,79 @@
     # Cannot be unchecked if it's the only one checked, and checking it uncheck the others
     def update_linked(self):
         if self.checked:
             self.uncheck_others()
         elif self.checkable():
             self.checked = True
 
-    def uncheck(name):
-        UI.dict[CheckBox.__name__][name].checked = False
-
-    def check(name):
-        UI.dict[CheckBox.__name__][name].checked = True
-
-    def checked(name):
-        return UI.dict[CheckBox.__name__][name].checked
-
     def link(name, others):
         UI.dict[CheckBox.__name__][name].links = others
 
-    def on_update(self, surface):
-        rect = (*self.pos, *self.size)
-        UI.new_rects.append(rect)
-
-        if self.locked:
-            surface.blit(self.appearence['locked'], self.pos)
-        elif self.down or self.checked:
-            surface.blit(self.appearence['down'], self.pos)
-        elif self.hovered and self.hoverable:
-            surface.blit(self.appearence['hovered'], self.pos)
-        else:
-            surface.blit(self.appearence['classic'], self.pos)
-
-        if self.checked:
-            pygame.draw.circle(surface, CheckBox.COLOR_BUTTON_SIDE, self.tick_center, (self.size[0] - 2 * CheckBox.thickness - 4) / 2)
-            pygame.draw.circle(surface, self.get_first_color(is_down=self.checked), self.tick_center, (self.size[0] - 2 * CheckBox.thickness - 4) / 2 - 2)
-
 
 class Text(UI):
+    """
+    ## Parameters
+        - `name`: name of the UI element
+        - `pos`: position of the UI element
+        - `text` (optional): text to display
+        - `color` (optional): text color, any RGB format
+        - `centered` (optional): text alignment, (horizontal, vertical)
+
+    ## Setters
+    - `Text.set_text(name, text)`: changes the text displayed
+    - `Text.set_text_color(name, color)`: changes the color of the text
+
+    ## Example
+    Centered blue text at (0, 0):
+    ```python
+    Text("text_id", (0, 0), "Hello World !", color=(255, 0, 0), centered=(True, True))
+    Text.set_text("text_id", "Hello World !")
+    Text.set_text_color("text_id", "#0000ff")
+    ```
+    """
 
-    def __init__(self, name, pos, text="Text", color=None, centered=(False, False)):
+    def __init__(self, name:str, pos, text="Text", color=None, centered=(False, False)):
         UI.__init__(self, name, pos, size=(0, 0), hoverable=False, locked=False)
-        
+
         self.color = color
         if color == None:
             self.color = (255, 255, 255)
 
         self.text = text
         self.centered = centered
         self.appearence = self.appearences()
 
-    def appearences(self):
-        rendered = UI.FONT.render(self.text, self.color)
-        self.size = rendered[0].get_size()
-        return rendered[0]
-
+    #############
+    #  SETTERS  #
+    #############
     def set_text(name, text):
         self = UI.dict[Text.__name__][name]
         self.text = text
         self.appearence = self.appearences()
-    
+
     def set_text_color(name, color):
         self = UI.dict[Text.__name__][name]
         self.color = color
         self.appearence = self.appearences()
 
+    ################
+    #  APPEARENCE  #
+    ################
+    def appearences(self):
+        rendered = UI.FONT.render(self.text, self.color)
+        self.size = rendered[0].get_size()
+        return rendered[0]
+
+    ############
+    #  UPDATE  #
+    ############
     def on_update(self, surface):
         rect = (*self.pos, *self.size)
         UI.new_rects.append(rect)
-        
+
         x, y = self.pos
 
         if self.centered[0]:
             x -= self.size[0] / 2
         if self.centered[1]:
             y -= self.size[1] / 2
```

## Comparing `pygame_ui_controls-1.0.3.dist-info/LICENSE` & `pygame_ui_controls-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pygame_ui_controls-1.0.3.dist-info/METADATA` & `pygame_ui_controls-1.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-ui-controls
-Version: 1.0.3
+Version: 1.1.0
 Summary: Pygame UI controls
 Home-page: https://github.com/ArthurLeFloch/PygameUI
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

