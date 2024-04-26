# Comparing `tmp/python-automation-framework-0.1.6.tar.gz` & `tmp/python-automation-framework-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-automation-framework-0.1.6.tar", last modified: Thu Dec 14 12:05:42 2023, max compression
+gzip compressed data, was "python-automation-framework-0.1.7.tar", last modified: Fri Apr 26 09:25:56 2024, max compression
```

## Comparing `python-automation-framework-0.1.6.tar` & `python-automation-framework-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-12-14 12:05:42.546690 python-automation-framework-0.1.6/
--rw-r--r--   0 mikereiche   (502) staff       (20)     5722 2023-12-14 12:05:42.542172 python-automation-framework-0.1.6/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     5472 2023-09-05 19:24:39.000000 python-automation-framework-0.1.6/README.md
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-12-14 12:05:42.487856 python-automation-framework-0.1.6/paf/
--rw-r--r--   0 mikereiche   (502) staff       (20)     6923 2023-09-05 19:24:59.000000 python-automation-framework-0.1.6/paf/assertion.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3585 2023-12-14 11:49:24.000000 python-automation-framework-0.1.6/paf/common.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2163 2023-12-14 12:05:07.000000 python-automation-framework-0.1.6/paf/component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      451 2023-06-05 10:36:16.000000 python-automation-framework-0.1.6/paf/config.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2509 2023-09-05 19:52:42.000000 python-automation-framework-0.1.6/paf/control.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.1.6/paf/dom.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.1.6/paf/javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2639 2023-12-14 11:48:42.000000 python-automation-framework-0.1.6/paf/listener.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2649 2023-05-09 19:33:48.000000 python-automation-framework-0.1.6/paf/locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     4353 2023-10-28 07:19:12.000000 python-automation-framework-0.1.6/paf/manager.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3183 2023-12-14 11:49:17.000000 python-automation-framework-0.1.6/paf/page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2349 2023-09-05 19:24:39.000000 python-automation-framework-0.1.6/paf/request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      302 2023-05-09 19:33:48.000000 python-automation-framework-0.1.6/paf/types.py
--rw-r--r--   0 mikereiche   (502) staff       (20)    16429 2023-12-14 12:05:07.000000 python-automation-framework-0.1.6/paf/uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     6689 2023-05-02 17:26:39.000000 python-automation-framework-0.1.6/paf/xpath.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-12-14 12:05:42.499205 python-automation-framework-0.1.6/python_automation_framework.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     5722 2023-12-14 12:05:42.000000 python-automation-framework-0.1.6/python_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      689 2023-12-14 12:05:42.000000 python-automation-framework-0.1.6/python_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-12-14 12:05:42.000000 python-automation-framework-0.1.6/python_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-12-14 12:05:42.000000 python-automation-framework-0.1.6/python_automation_framework.egg-info/requires.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-12-14 12:05:42.000000 python-automation-framework-0.1.6/python_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-12-14 12:05:42.546822 python-automation-framework-0.1.6/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-12-14 12:05:23.000000 python-automation-framework-0.1.6/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-12-14 12:05:42.539248 python-automation-framework-0.1.6/test/
--rw-r--r--   0 mikereiche   (502) staff       (20)     2021 2023-05-09 19:15:59.000000 python-automation-framework-0.1.6/test/test_component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1434 2023-09-05 19:52:42.000000 python-automation-framework-0.1.6/test/test_control.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2443 2023-12-14 11:48:42.000000 python-automation-framework-0.1.6/test/test_demo_mode.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      524 2023-05-09 19:33:48.000000 python-automation-framework-0.1.6/test/test_javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3291 2023-05-09 19:33:48.000000 python-automation-framework-0.1.6/test/test_locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3984 2023-10-08 14:27:12.000000 python-automation-framework-0.1.6/test/test_manager.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1937 2023-10-08 14:27:12.000000 python-automation-framework-0.1.6/test/test_page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1124 2023-05-09 19:33:48.000000 python-automation-framework-0.1.6/test/test_request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)    10987 2023-12-14 12:05:07.000000 python-automation-framework-0.1.6/test/test_uielement.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2024-04-26 09:25:56.584310 python-automation-framework-0.1.7/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5722 2024-04-26 09:25:56.584015 python-automation-framework-0.1.7/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5472 2023-09-05 19:24:39.000000 python-automation-framework-0.1.7/README.md
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2024-04-26 09:25:56.542499 python-automation-framework-0.1.7/paf/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6923 2023-09-05 19:24:59.000000 python-automation-framework-0.1.7/paf/assertion.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3585 2024-02-04 15:14:02.000000 python-automation-framework-0.1.7/paf/common.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2163 2023-12-14 12:05:07.000000 python-automation-framework-0.1.7/paf/component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      451 2023-06-05 10:36:16.000000 python-automation-framework-0.1.7/paf/config.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2509 2023-09-05 19:52:42.000000 python-automation-framework-0.1.7/paf/control.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.1.7/paf/dom.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.1.7/paf/javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2639 2023-12-14 11:48:42.000000 python-automation-framework-0.1.7/paf/listener.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2649 2023-05-09 19:33:48.000000 python-automation-framework-0.1.7/paf/locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4447 2024-04-26 09:25:26.000000 python-automation-framework-0.1.7/paf/manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3176 2024-02-05 07:00:46.000000 python-automation-framework-0.1.7/paf/page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2349 2023-09-05 19:24:39.000000 python-automation-framework-0.1.7/paf/request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      302 2023-05-09 19:33:48.000000 python-automation-framework-0.1.7/paf/types.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)    16841 2024-04-26 09:25:26.000000 python-automation-framework-0.1.7/paf/uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6689 2023-05-02 17:26:39.000000 python-automation-framework-0.1.7/paf/xpath.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2024-04-26 09:25:56.552664 python-automation-framework-0.1.7/python_automation_framework.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5722 2024-04-26 09:25:56.000000 python-automation-framework-0.1.7/python_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      689 2024-04-26 09:25:56.000000 python-automation-framework-0.1.7/python_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2024-04-26 09:25:56.000000 python-automation-framework-0.1.7/python_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       46 2024-04-26 09:25:56.000000 python-automation-framework-0.1.7/python_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        4 2024-04-26 09:25:56.000000 python-automation-framework-0.1.7/python_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2024-04-26 09:25:56.584374 python-automation-framework-0.1.7/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      587 2024-04-26 09:25:31.000000 python-automation-framework-0.1.7/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2024-04-26 09:25:56.583355 python-automation-framework-0.1.7/test/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2021 2023-05-09 19:15:59.000000 python-automation-framework-0.1.7/test/test_component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1253 2023-12-14 12:19:42.000000 python-automation-framework-0.1.7/test/test_control.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2443 2023-12-14 11:48:42.000000 python-automation-framework-0.1.7/test/test_demo_mode.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      524 2023-05-09 19:33:48.000000 python-automation-framework-0.1.7/test/test_javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3291 2023-05-09 19:33:48.000000 python-automation-framework-0.1.7/test/test_locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4209 2024-04-26 09:25:26.000000 python-automation-framework-0.1.7/test/test_manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1937 2023-10-08 14:27:12.000000 python-automation-framework-0.1.7/test/test_page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1124 2023-05-09 19:33:48.000000 python-automation-framework-0.1.7/test/test_request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)    12139 2024-04-26 09:25:26.000000 python-automation-framework-0.1.7/test/test_uielement.py
```

### Comparing `python-automation-framework-0.1.6/PKG-INFO` & `python-automation-framework-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.1.6
+Version: 0.1.7
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 [![Pypi](https://img.shields.io/pypi/v/python-automation-framework.svg)](https://pypi.org/project/python-automation-framework)
 ![Tests Status](https://github.com/mreiche/python-automation-framework/actions/workflows/tests.yml/badge.svg)
```

### Comparing `python-automation-framework-0.1.6/README.md` & `python-automation-framework-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/paf/assertion.py` & `python-automation-framework-0.1.7/paf/assertion.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/paf/common.py` & `python-automation-framework-0.1.7/paf/common.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/paf/component.py` & `python-automation-framework-0.1.7/paf/component.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/paf/control.py` & `python-automation-framework-0.1.7/paf/control.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/paf/javascript.py` & `python-automation-framework-0.1.7/paf/javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/paf/listener.py` & `python-automation-framework-0.1.7/paf/listener.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/paf/locator.py` & `python-automation-framework-0.1.7/paf/locator.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/paf/manager.py` & `python-automation-framework-0.1.7/paf/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,23 +89,23 @@
         key = session_keys[index]
         self._session_driver_map.pop(key)
 
     def shutdown_all(self):
         for webdriver in list(self._session_driver_map.values()):
             self.shutdown(webdriver)
 
-    def take_screenshot(self, webdriver: WebDriver) -> Path | None:
+    def take_screenshot(self, webdriver: WebDriver, file_name: str = None) -> Path | None:
         dir = Path(Property.env(Property.PAF_SCREENSHOTS_DIR))
-        title = webdriver.title
-        if empty(title):
-            title = webdriver.current_url
+        if empty(file_name):
+            title = webdriver.title
+            if empty(title):
+                title = webdriver.current_url
+            formatter = inject.instance(Formatter)
+            file_name = f"{webdriver.session_id}-{title}-{formatter.datetime(datetime.now())}.png"
 
-        formatter = inject.instance(Formatter)
-
-        file_name = f"{title}-{formatter.datetime(datetime.now())}.png"
         dir.mkdir(parents=True, exist_ok=True)
         path = dir / file_name
         if webdriver.save_screenshot(dir / file_name):
             return path
         else:
             return None
```

### Comparing `python-automation-framework-0.1.6/paf/page.py` & `python-automation-framework-0.1.7/paf/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from paf.assertion import StringAssertion, Format
 from paf.common import HasName, Locator
 from paf.manager import WebDriverManager
 from paf.request import WebDriverRequest
 from paf.types import PAGE, COMPONENT
-from paf.uielement import DefaultUiElement
+from paf.uielement import DefaultUiElement, UiElement
 
 
 class PageFactory:
     def create_page(self, page_class: Type[PAGE], webdriver: WebDriver = None) -> PAGE:
         if not webdriver:
             webdriver = inject.instance(WebDriverManager).get_webdriver(WebDriverRequest())
 
@@ -27,16 +27,15 @@
     def open(self, url: str):
         self._webdriver.get(url)
         return self
 
     def __str__(self):
         return self.name
 
-    def _find(self, by: Locator, name: str = None):
-        from paf.uielement import UiElement
+    def _find(self, by: Locator, name: str = None) -> UiElement:
         return DefaultUiElement(
             by=by,
             webdriver=self._webdriver,
             parent=self,
             name=name,
         )
 
@@ -58,15 +57,15 @@
 
     def scroll_by(self, x: int = 0, y: int = 0):
         actions = ActionChains(self._webdriver)
         actions.scroll_by_amount(x, y).perform()
 
 
 class FinderPage(BasePage):
-    def find(self, by: Locator, name: str = None):
+    def find(self, by: Locator, name: str = None) -> UiElement:
         ui_element = self._find(by, name)
         ui_element._parent = None
         return ui_element
 
 
 class Page(BasePage):
     def __init__(self, webdriver: WebDriver):
```

### Comparing `python-automation-framework-0.1.6/paf/request.py` & `python-automation-framework-0.1.7/paf/request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/paf/uielement.py` & `python-automation-framework-0.1.7/paf/uielement.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from abc import abstractmethod, ABC
 from contextlib import contextmanager
 from datetime import datetime
 from pathlib import Path
 from typing import Type, TypeVar, List, Generic, Iterable, Iterator, Callable, ContextManager
 
 import inject
+from is_empty import empty
 from selenium.webdriver import ActionChains
 from selenium.webdriver.common.by import By as SeleniumBy
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.color import Color
 
 import paf.javascript as script
@@ -23,15 +24,15 @@
 from paf.types import Mapper, R, Consumer
 from paf.xpath import XPath
 
 
 class UiElementActions(ABC):
 
     @abstractmethod
-    def click(self):   # pragma: no cover
+    def click(self):  # pragma: no cover
         pass
 
     @abstractmethod
     def hover(self):  # pragma: no cover
         pass
 
     @abstractmethod
@@ -99,15 +100,15 @@
         pass
 
     @abstractmethod
     def highlight(self, color: Color = Color.from_string("#0f0"), seconds: float = 2):  # pragma: no cover
         pass
 
     @abstractmethod
-    def take_screenshot(self) -> Path | None:  # pragma: no cover
+    def take_screenshot(self, file_name: str = None) -> Path | None:  # pragma: no cover
         pass
 
 
 class UiElementTests:
     @property
     @abstractmethod
     def expect(self) -> "UiElementAssertion":  # pragma: no cover
@@ -115,27 +116,35 @@
 
     @property
     @abstractmethod
     def wait_for(self) -> "UiElementAssertion":  # pragma: no cover
         pass
 
 
-class UiElement(WebdriverRetainer, UiElementTests, UiElementActions, HasParent, PageObjectList["UiElement"], ABC):
+class UiElement(
+    WebdriverRetainer,
+    PageObject["UiElement"],
+    UiElementTests,
+    UiElementActions,
+    HasParent,
+    PageObjectList["UiElement"],
+    ABC
+):
     def __str__(self):
         return self.name
 
     @property
     def name(self):
         if self._name:
             return self._name
         else:
             return f"UiElement({self._by.__str__()})[{self._index}]"
 
     @abstractmethod
-    def find(self, by: Locator, name: str = None):  # pragma: no cover
+    def find(self, by: Locator, name: str = None) -> "UiElement":  # pragma: no cover
         pass
 
     @property
     def expect(self):
         return UiElementAssertion(self)
 
     @property
@@ -224,34 +233,34 @@
     def submit(self):
         pass
 
     def __getitem__(self, index: int) -> T:
         return self
 
     def __iter__(self) -> Iterator[T]:
-        pass
+        return [].__iter__()
 
     def find(self, by: Locator, name: str = None):
         return InexistentUiElement(name, self)
 
     @contextmanager
     def _find_web_elements(self) -> ContextManager[List[WebElement]]:
         yield []
 
 
 class DefaultUiElement(UiElement):
 
     def __init__(
-        self,
-        by: Locator,
-        ui_element: UiElement = None,
-        webdriver: WebDriver = None,
-        parent: object = None,
-        index: int = 0,
-        name: str = None,
+            self,
+            by: Locator,
+            ui_element: UiElement = None,
+            webdriver: WebDriver = None,
+            parent: object = None,
+            index: int = 0,
+            name: str = None,
     ):
 
         if isinstance(by, XPath):
             by = By.xpath(str(by))
         elif isinstance(by, str):
             by = By.css_selector(by)
 
@@ -302,24 +311,25 @@
         elif self._webdriver:
             self._webdriver.switch_to.default_content()
             web_elements = self._webdriver.find_elements(self._by.by, self._by.value)
             yield self._filter_web_elements(web_elements)
         else:
             raise Exception(f"{self.name_path} initialized without WebDriver nor UiElement")
 
-    @contextmanager
-    def find_web_element(self) -> ContextManager[WebElement]:
-        with self._find_web_elements() as web_elements:
-            count = len(web_elements)
-            if self._by.is_unique and count != 1:
-                raise NotUniqueException()
-            elif count > self._index:
-                yield web_elements[self._index]
-            else:
-                raise NotFoundException()
+    # @contextmanager
+    # def find_web_element(self) -> ContextManager[WebElement]:
+    #     pass
+    #     with self._find_web_elements() as web_elements:
+    #         count = len(web_elements)
+    #         if self._by.is_unique and count != 1:
+    #             raise NotUniqueException()
+    #         elif count > self._index:
+    #             yield web_elements[self._index]
+    #         else:
+    #             raise NotFoundException()
 
     def _web_element_action_sequence(self, action: Consumer[WebElement], action_name: str):
         listener = inject.instance(Listener)
 
         def _sequence():
             with self.find_web_element() as web_element:
                 action(web_element)
@@ -335,19 +345,21 @@
         self._web_element_action_sequence(lambda x: x.click(), "click")
         return self
 
     def send_keys(self, value: str):
         self._web_element_action_sequence(lambda x: x.send_keys(value), "send_keys")
         return self
 
-    def take_screenshot(self) -> Path | None:
+    def take_screenshot(self, file_name: str = None) -> Path | None:
         with self.find_web_element() as web_element:
             dir = Path(Property.env(Property.PAF_SCREENSHOTS_DIR))
-            formatter = inject.instance(Formatter)
-            file_name = f"{self.name}-{formatter.datetime(datetime.now())}.png"
+            if empty(file_name):
+                formatter = inject.instance(Formatter)
+                file_name = f"{self.webdriver.session_id}-{self.name}-{formatter.datetime(datetime.now())}.png"
+
             dir.mkdir(parents=True, exist_ok=True)
             path = dir / file_name
             if web_element.screenshot(str(path)):
                 return path
             else:
                 return None
 
@@ -403,14 +415,15 @@
     def submit(self):
         self._web_element_action_sequence(lambda x: x.submit(), "submit")
         return self
 
     def scroll_into_view(self, x: int = 0, y: int = 0):
         def _action(web_element: WebElement):
             script.scroll_to_center(self._webdriver, web_element, Point(x, y))
+
         self._web_element_action_sequence(_action, "scroll_into_view")
 
     def scroll_to_top(self, x: int = 0, y: int = 0):
         def _action(web_element: WebElement):
             script.scroll_to_top(self._webdriver, web_element, Point(x, y))
 
         self._web_element_action_sequence(_action, "scroll_to_top")
@@ -434,26 +447,26 @@
             index=index
         )
 
 
 class UiElementAssertion:
 
     def __init__(
-        self,
-        ui_element: UiElement,
-        raise_exception: bool = True,
+            self,
+            ui_element: UiElement,
+            raise_exception: bool = True,
     ):
         self._ui_element = ui_element
         self._raise = raise_exception
 
     def _map_web_element_property(
-        self,
-        assertion_class: Type[ASSERTION],
-        mapper: Mapper[WebElement, any],
-        property_name: str
+            self,
+            assertion_class: Type[ASSERTION],
+            mapper: Mapper[WebElement, any],
+            property_name: str
     ) -> ASSERTION:
 
         def _map_failsafe():
             try:
                 with self._ui_element.find_web_element() as web_element:
                     return mapper(web_element)
             except Exception:
@@ -487,18 +500,20 @@
     def tag_name(self):
         return self._map_web_element_property(StringAssertion, lambda x: x.tag_name, "tag name")
 
     def attribute(self, attribute: str | Attribute):
         if isinstance(attribute, Attribute):
             attribute = attribute.value
 
-        return self._map_web_element_property(StringAssertion, lambda x: x.get_attribute(attribute), f"attribute({attribute})")
+        return self._map_web_element_property(StringAssertion, lambda x: x.get_attribute(attribute),
+                                              f"attribute({attribute})")
 
     def css(self, property_name: str):
-        return self._map_web_element_property(StringAssertion, lambda x: x.value_of_css_property(property_name), f"css({property_name}")
+        return self._map_web_element_property(StringAssertion, lambda x: x.value_of_css_property(property_name),
+                                              f"css({property_name}")
 
     def classes(self, *classes):
         return self.attribute(Attribute.CLASS).has_words(*classes)
 
     def visible(self, expected: bool):
         return self._visible(expected, False)
```

### Comparing `python-automation-framework-0.1.6/paf/xpath.py` & `python-automation-framework-0.1.7/paf/xpath.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/python_automation_framework.egg-info/PKG-INFO` & `python-automation-framework-0.1.7/python_automation_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.1.6
+Version: 0.1.7
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 [![Pypi](https://img.shields.io/pypi/v/python-automation-framework.svg)](https://pypi.org/project/python-automation-framework)
 ![Tests Status](https://github.com/mreiche/python-automation-framework/actions/workflows/tests.yml/badge.svg)
```

### Comparing `python-automation-framework-0.1.6/python_automation_framework.egg-info/SOURCES.txt` & `python-automation-framework-0.1.7/python_automation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/setup.py` & `python-automation-framework-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="python-automation-framework",
     description="Automation framework for the WebDriver API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.1.6",
+    version="0.1.7",
     url="https://github.com/mreiche/python-automation-framework",
     author="Mike Reiche",
     packages=["paf"],
     install_requires=["inject>=4.3.1", "selenium>=4.8.3", "is-empty>=1.0.1"],
 )
```

### Comparing `python-automation-framework-0.1.6/test/test_component.py` & `python-automation-framework-0.1.7/test/test_component.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/test/test_control.py` & `python-automation-framework-0.1.7/test/test_control.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,35 +21,25 @@
         retry(lambda: None)
 
     global_config = get_config()
     assert global_config.retry_count == backup_config.retry_count
     assert global_config.wait_after_fail == backup_config.wait_after_fail
 
 
-def change_first():
+def test_change_first():
     global_config = get_config()
     assert global_config.retry_count == Property.env(Property.PAF_SEQUENCE_RETRY_COUNT)
 
     with change(retry_count=0):
         sleep(0.3)
         config = get_config()
         assert config.retry_count == 0
 
 
-def change_second():
+def test_change_second():
     global_config = get_config()
     assert global_config.retry_count == Property.env(Property.PAF_SEQUENCE_RETRY_COUNT)
 
     with change(retry_count=99):
         sleep(0.1)
         config = get_config()
         assert config.retry_count == 99
-
-
-@pytest.mark.asyncio
-async def test_thread_safety():
-    tasks = [
-        asyncio.to_thread(change_first),
-        asyncio.to_thread(change_second)
-    ]
-
-    await asyncio.gather(*tasks)
```

### Comparing `python-automation-framework-0.1.6/test/test_demo_mode.py` & `python-automation-framework-0.1.7/test/test_demo_mode.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/test/test_javascript.py` & `python-automation-framework-0.1.7/test/test_javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/test/test_locator.py` & `python-automation-framework-0.1.7/test/test_locator.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/test/test_manager.py` & `python-automation-framework-0.1.7/test/test_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,20 @@
 def test_take_screenshot(manager: WebDriverManager):
     create_webdriver()
     webdrivers = manager.webdrivers
     assert isinstance(webdrivers, list)
 
     for webdriver in webdrivers:
         path = manager.take_screenshot(webdriver)
+        assert webdriver.session_id in path.name
+        assert path.exists()
+
+        path = manager.take_screenshot(webdriver, "test")
+        assert webdriver.session_id not in path.name
+        assert path.name == "test"
         assert path.exists()
 
 
 def test_shutdown_by_session_key(manager: WebDriverManager):
     request = WebDriverRequest("test")
     create_webdriver(request)
     manager.shutdown_session(request.session_name)
```

### Comparing `python-automation-framework-0.1.6/test/test_page.py` & `python-automation-framework-0.1.7/test/test_page.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/test/test_request.py` & `python-automation-framework-0.1.7/test/test_request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.6/test/test_uielement.py` & `python-automation-framework-0.1.7/test/test_uielement.py`

 * *Files 10% similar despite different names*

```diff
@@ -149,14 +149,23 @@
     p.last.expect.attribute("name").be("pName41")
 
     for item in p:
         item.expect.attribute("name").be("pName1")
         break
 
 
+def test_inexistent_sub_element(finder: FinderPage):
+    finder.open("https://testpages.herokuapp.com/styled/find-by-playground-test.html")
+
+    # Sub elements
+    div = finder.find("#div1")
+    inexistent = div.find("#inexistent")
+    inexistent.expect.count.be(0)
+
+
 def test_form(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/basic-html-form-test.html")
 
     checkbox = finder.find(XPath.at("input").name("checkboxes[]").attribute("value").be("cb3"))
     checkbox.expect.selected(True)
 
     textarea = finder.find(By.name("comments"))
@@ -177,16 +186,23 @@
     # From Textarea
     finder.find("#_valuecomments").expect.text.be("Hello World")
 
 
 def test_screenshot(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/find-by-playground-test.html")
     p = finder.find(By.id("pre1").unique)
+
     path = p.take_screenshot()
-    assert path
+    assert finder.webdriver.session_id in path.name
+    assert path.exists()
+
+    path = p.take_screenshot("test")
+    assert finder.webdriver.session_id not in path.name
+    assert "test" in path.name
+    assert path.exists()
 
 
 def test_retry(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/key-click-display-test.html")
     btn = finder.find(By.id("button").unique)
     clicks = finder.find(XPath.at("div").id("events").select("p"))
     btn.click()
@@ -312,14 +328,31 @@
 
     with pytest.raises(Exception, match=re.escape("Expected UiElement(By.css selector(#unkown))[0] count [0] to be [1] after 0 retries")):
         with change(retry_count=0):
             unknown = finder.find("#unkown")
             unknown.expect.count.be(1)
 
 
-def test_empty_ui_element():
+def test_inexistent_ui_element_wrapper():
     empty_ui_element = InexistentUiElement()
     empty_ui_element.expect.count.be(0)
+    assert empty_ui_element.webdriver is None
+    empty_ui_element.scroll_to_top()
+    empty_ui_element.scroll_into_view()
+    empty_ui_element.highlight()
+    empty_ui_element.click()
+    empty_ui_element.hover()
+    empty_ui_element.long_click()
+    empty_ui_element.double_click()
+    empty_ui_element.drag_and_drop_to(empty_ui_element)
+    empty_ui_element.send_keys("test")
+    empty_ui_element.type("test")
+    empty_ui_element.clear()
+    empty_ui_element.submit()
+    assert empty_ui_element.take_screenshot() is None
+    assert isinstance(empty_ui_element.find("#inexistent"), InexistentUiElement)
+    for e in empty_ui_element:
+        assert False
 
 
 def teardown_module():
     inject.instance(WebDriverManager).shutdown_all()
```

