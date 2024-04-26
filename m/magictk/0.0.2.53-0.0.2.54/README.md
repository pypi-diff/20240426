# Comparing `tmp/magictk-0.0.2.53.tar.gz` & `tmp/magictk-0.0.2.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.53.tar", last modified: Thu Apr 25 14:57:36 2024, max compression
+gzip compressed data, was "magictk-0.0.2.54.tar", last modified: Fri Apr 26 01:09:12 2024, max compression
```

## Comparing `magictk-0.0.2.53.tar` & `magictk-0.0.2.54.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:36.375087 magictk-0.0.2.53/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-25 14:57:35.000000 magictk-0.0.2.53/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-25 14:57:36.371087 magictk-0.0.2.53/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-25 14:57:35.000000 magictk-0.0.2.53/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:36.371087 magictk-0.0.2.53/magictk/
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3285 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    13554 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11247 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12242 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)     3725 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/mtk.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5995 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     8106 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/scrollbar.py
--rw-r--r--   0 root         (0) root         (0)     6178 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10245 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:36.371087 magictk-0.0.2.53/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-25 14:57:36.000000 magictk-0.0.2.53/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      592 2024-04-25 14:57:36.000000 magictk-0.0.2.53/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 14:57:36.000000 magictk-0.0.2.53/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 14:57:36.000000 magictk-0.0.2.53/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 14:57:36.375087 magictk-0.0.2.53/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-25 14:57:35.000000 magictk-0.0.2.53/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 01:09:12.358843 magictk-0.0.2.54/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-26 01:09:11.000000 magictk-0.0.2.54/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-26 01:09:12.358843 magictk-0.0.2.54/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-26 01:09:11.000000 magictk-0.0.2.54/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 01:09:12.358843 magictk-0.0.2.54/magictk/
+-rw-r--r--   0 root         (0) root         (0)      442 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    17051 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11247 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12242 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/icon.py
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5995 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     8106 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/scrollbar.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10245 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 01:09:12.358843 magictk-0.0.2.54/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-26 01:09:12.000000 magictk-0.0.2.54/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      610 2024-04-26 01:09:12.000000 magictk-0.0.2.54/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 01:09:12.000000 magictk-0.0.2.54/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-26 01:09:12.000000 magictk-0.0.2.54/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 01:09:12.358843 magictk-0.0.2.54/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-26 01:09:11.000000 magictk-0.0.2.54/setup.py
```

### Comparing `magictk-0.0.2.53/PKG-INFO` & `magictk-0.0.2.54/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.53
-Summary: A tkinter weights looks like element-plus
+Version: 0.0.2.54
+Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `magictk-0.0.2.53/README.md` & `magictk-0.0.2.54/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/_window_ctl.py` & `magictk-0.0.2.54/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/_window_size.py` & `magictk-0.0.2.54/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/basicwindow.py` & `magictk-0.0.2.54/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/button.py` & `magictk-0.0.2.54/magictk/button.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,22 +64,58 @@
                 self._fill_gc.append(g_color)
                 self._fill_fc.append(f_color)
                 self._fill_hc.append(h_color)
                 self._fill_obj.append(obj)
                 x_n += 1
             y_n += 1
 
+    def _draw_icon(self, x, y, name, size, **kwargs):
+        border_info = border_info = json.loads(photoload.loadres(
+            f"icon/{name}@{size}"))
+        y_n = 0
+        for i in border_info:
+            x_n = 0
+            for j in i:
+                px = x+y_n+1
+                py = y+x_n+1
+                lcolor = j
+                g_color = color_tmpl.mix_color(
+                    self.color["regular_text"], self.color["background"], int((1-lcolor/255)*1000)/1000)
+                f_color = color_tmpl.mix_color(
+                    self.color[self._color_fg], self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
+                h_color = color_tmpl.mix_color(
+                    self.color[self._color_fg], self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
+
+                obj = self.canvas.create_rectangle(
+                    px, py, px, py, width=0, fill=g_color)
+
+                def update_color(obj, g_color, f_color, h_color):
+                    if (self._is_hover == 2):
+                        self.canvas.itemconfig(
+                            obj, fill=h_color)
+                    else:
+                        self.canvas.itemconfig(
+                            obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
+
+                self._fill_func.append(update_color)
+                self._fill_gc.append(g_color)
+                self._fill_fc.append(f_color)
+                self._fill_hc.append(h_color)
+                self._fill_obj.append(obj)
+                x_n += 1
+            y_n += 1
+
     def _update_color(self):
         n = 0
         for i in self._fill_func:
             i(self._fill_obj[n], self._fill_gc[n],
               self._fill_fc[n], self._fill_hc[n])
             n += 1
 
-    def __init__(self, master=None, root_anim=None, w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _set_defaultcolor=None):
+    def __init__(self, master=None, root_anim=None, w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _set_defaultcolor=None, iconname="", iconsize=24):
         global use_font
         use_font = fontconfig.getfont()
         self._fill_obj = []
         self._fill_func = []
         self._fill_gc = []
         self._fill_fc = []
         self._fill_hc = []
@@ -103,15 +139,21 @@
             self.root = master.root
         else:
             self.root = root_anim
 
         self.canvas = tkinter.Canvas(
             master, bg=self.color["background"], width=self.w, height=self.h, borderwidth=0, bd=0, highlightcolor=self.color["background"], highlightthickness=0)
 
+        if (iconname != ''):
+            self.text = ""
         self._draw()
+        if (iconname != ''):
+            self.size = iconsize
+            self._draw_icon(self.w//2-self.size//2, self.h //
+                            2-self.size//2, iconname, iconsize)
         self._update_color()
         self._bind_event()
         self.bind_anim()
 
         for event, eventfunc in master.p_event_list:
             self.canvas.bind(event, eventfunc)
 
@@ -248,14 +290,50 @@
             self._func(self)
             self._update_color()
         self.canvas.bind("<ButtonRelease-1>", pressrelease_v)
 
 
 class ButtonFill(Button):
 
+    def _draw_icon(self, x, y, name, size, **kwargs):
+        border_info = border_info = json.loads(photoload.loadres(
+            f"icon/{name}@{size}"))
+        y_n = 0
+        for i in border_info:
+            x_n = 0
+            for j in i:
+                px = x+y_n+1
+                py = y+x_n+1
+                lcolor = j
+                g_color = color_tmpl.mix_color(
+                    "#FFFFFF", self.color[self._color_bd], int((1-lcolor/255)*1000)/1000)
+                f_color = color_tmpl.mix_color(
+                    "#FFFFFF", self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
+                h_color = color_tmpl.mix_color(
+                    "#FFFFFF", self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
+
+                obj = self.canvas.create_rectangle(
+                    px, py, px, py, width=0, fill=g_color)
+
+                def update_color(obj, g_color, f_color, h_color):
+                    if (self._is_hover == 2):
+                        self.canvas.itemconfig(
+                            obj, fill=h_color)
+                    else:
+                        self.canvas.itemconfig(
+                            obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
+
+                self._fill_func.append(update_color)
+                self._fill_gc.append(g_color)
+                self._fill_fc.append(f_color)
+                self._fill_hc.append(h_color)
+                self._fill_obj.append(obj)
+                x_n += 1
+            y_n += 1
+
     def _draw_corner(self, r_x, r_y, x, y, **kwargs):
         border_info = json.loads(photoload.loadres("buttonborder"))
         y_n = 0
         for i in border_info:
             x_n = 0
             for j in i:
                 if (r_x == 0):
@@ -304,19 +382,19 @@
                 self._fill_gc.append(g_color)
                 self._fill_fc.append(f_color)
                 self._fill_hc.append(h_color)
                 self._fill_obj.append(obj)
                 x_n += 1
             y_n += 1
 
-    def __init__(self, master=None, root_anim=None, color_type="primary", w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _dis_color=None):
+    def __init__(self, master=None, root_anim=None, color_type="primary", w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _dis_color=None, iconname="", iconsize=24):
         if (_dis_color is None):
             self._color_bd = color_type
             self._color_bg = color_type
             self._color_bg1 = color_type
             self._color_fg1 = color_type+"_light3"
             self._color_fg = color_type+"_dark"
             self._color_fg3 = color_type+"_light3"
             self._color_fg2 = color_type+"_dark"
             self._color_text = "#FFFFFF"
         super().__init__(master=master, root_anim=root_anim, w=w, h=h,
-                         text=text, color_list=color_list, func=func, _set_defaultcolor=True)
+                         text=text, color_list=color_list, func=func, _set_defaultcolor=True, iconname=iconname, iconsize=iconsize)
```

### Comparing `magictk-0.0.2.53/magictk/checkbox.py` & `magictk-0.0.2.54/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/color_tmpl.py` & `magictk-0.0.2.54/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/entry.py` & `magictk-0.0.2.54/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/fontconfig.py` & `magictk-0.0.2.54/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/frame.py` & `magictk-0.0.2.54/magictk/frame.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/icon.ico` & `magictk-0.0.2.54/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/photoload.py` & `magictk-0.0.2.54/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/progressbar.py` & `magictk-0.0.2.54/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/res.pickle` & `magictk-0.0.2.54/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/scrollbar.py` & `magictk-0.0.2.54/magictk/scrollbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/select.py` & `magictk-0.0.2.54/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/submenu.py` & `magictk-0.0.2.54/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/window.py` & `magictk-0.0.2.54/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk/workspace.py` & `magictk-0.0.2.54/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.53/magictk.egg-info/PKG-INFO` & `magictk-0.0.2.54/magictk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.53
-Summary: A tkinter weights looks like element-plus
+Version: 0.0.2.54
+Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `magictk-0.0.2.53/magictk.egg-info/SOURCES.txt` & `magictk-0.0.2.54/magictk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 ./magictk/button.py
 ./magictk/checkbox.py
 ./magictk/color_tmpl.py
 ./magictk/entry.py
 ./magictk/fontconfig.py
 ./magictk/frame.py
 ./magictk/icon.ico
+./magictk/icon.py
 ./magictk/mtk.py
 ./magictk/photoload.py
 ./magictk/progressbar.py
 ./magictk/res.pickle
 ./magictk/scrollbar.py
 ./magictk/select.py
 ./magictk/submenu.py
```

### Comparing `magictk-0.0.2.53/setup.py` & `magictk-0.0.2.54/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "magictk": "./magictk",
     },
     python_requires='>=3.8',
     include_package_data=True,
     install_requires=[],
     author='cxykevin|git.hmtsai.cn',
     author_email='cxykevin@yeah.net',
-    description='A tkinter weights looks like element-plus',
+    description='Some tkinter weights look like element-plus',
     long_description='',
     url='http://git.hmtsai.cn/cxykevin/magictk.git',
     license='GPLv2',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

