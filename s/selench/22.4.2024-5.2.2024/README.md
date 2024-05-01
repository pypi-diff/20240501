# Comparing `tmp/selench-22.4.2024.tar.gz` & `tmp/selench-5.2.2024.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selench-22.4.2024.tar", last modified: Sun Apr 21 21:07:35 2024, max compression
+gzip compressed data, was "selench-5.2.2024.tar", last modified: Wed May  1 21:19:43 2024, max compression
```

## Comparing `selench-22.4.2024.tar` & `selench-5.2.2024.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:07:35.549898 selench-22.4.2024/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-21 21:07:31.000000 selench-22.4.2024/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-21 21:07:35.549898 selench-22.4.2024/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-21 21:07:31.000000 selench-22.4.2024/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:07:35.549898 selench-22.4.2024/selench/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-21 21:07:31.000000 selench-22.4.2024/selench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29917 2024-04-21 21:07:31.000000 selench-22.4.2024/selench/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15900 2024-04-21 21:07:31.000000 selench-22.4.2024/selench/wait_for.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:07:35.549898 selench-22.4.2024/selench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-21 21:07:35.000000 selench-22.4.2024/selench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-21 21:07:35.000000 selench-22.4.2024/selench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 21:07:35.000000 selench-22.4.2024/selench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-21 21:07:35.000000 selench-22.4.2024/selench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 21:07:35.000000 selench-22.4.2024/selench.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 21:07:35.549898 selench-22.4.2024/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-21 21:07:31.000000 selench-22.4.2024/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:07:35.549898 selench-22.4.2024/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-21 21:07:31.000000 selench-22.4.2024/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-21 21:07:31.000000 selench-22.4.2024/tests/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-21 21:07:31.000000 selench-22.4.2024/tests/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-21 21:07:31.000000 selench-22.4.2024/tests/test_switch_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-21 21:07:31.000000 selench-22.4.2024/tests/test_wait_for.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:19:43.932385 selench-5.2.2024/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-01 21:19:37.000000 selench-5.2.2024/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-01 21:19:43.932385 selench-5.2.2024/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-01 21:19:37.000000 selench-5.2.2024/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:19:43.932385 selench-5.2.2024/selench/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-01 21:19:37.000000 selench-5.2.2024/selench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-05-01 21:19:37.000000 selench-5.2.2024/selench/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-01 21:19:37.000000 selench-5.2.2024/selench/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-05-01 21:19:37.000000 selench-5.2.2024/selench/expect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:19:43.932385 selench-5.2.2024/selench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-01 21:19:43.000000 selench-5.2.2024/selench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 21:19:43.000000 selench-5.2.2024/selench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:19:43.000000 selench-5.2.2024/selench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 21:19:43.000000 selench-5.2.2024/selench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 21:19:43.000000 selench-5.2.2024/selench.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:19:43.932385 selench-5.2.2024/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-01 21:19:37.000000 selench-5.2.2024/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:19:43.932385 selench-5.2.2024/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-01 21:19:37.000000 selench-5.2.2024/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-01 21:19:37.000000 selench-5.2.2024/tests/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-01 21:19:37.000000 selench-5.2.2024/tests/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-01 21:19:37.000000 selench-5.2.2024/tests/test_expect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-01 21:19:37.000000 selench-5.2.2024/tests/test_switch_to.py
```

### Comparing `selench-22.4.2024/LICENSE` & `selench-5.2.2024/LICENSE`

 * *Files identical despite different names*

### Comparing `selench-22.4.2024/PKG-INFO` & `selench-5.2.2024/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selench
-Version: 22.4.2024
+Version: 5.2.2024
 Summary: Selenium wrapper for Python
 Home-page: https://github.com/dsymbol/selench
 Author: dsymbol
 License: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -15,15 +15,18 @@
 # Selench
 
 Selench is a wrapper that simplifies the use of the Selenium library. 
 It provides a more concise syntax that makes the code more readable and easier to understand.
 
 ### Key Features
 
+- Concise syntax
+- Less imports
 - Elements have an explicit wait time by default
+- Simple expected_conditions implementation as expect
 - Element type detection ( CSS & XPATH )
 
 ## Installation
 
 To install the library, use pip:
 
 ```bash
@@ -60,13 +63,13 @@
     yield driver
     driver.quit()
 
 def test_ddg_search_query(driver):
     keyword = 'github'
     driver.get('https://duckduckgo.com/')
     driver.element('[name=q]').send_keys(keyword, Keys.ENTER)
-    driver.wait_for.title_to_contain(keyword)
+    driver.expect.title_to_contain(keyword)
     titles = driver.elements('a[data-testid=result-title-a] span')
 
     for title in titles:
         assert keyword in title.text.lower()
 ```
```

### Comparing `selench-22.4.2024/README.md` & `selench-5.2.2024/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Selench
 
 Selench is a wrapper that simplifies the use of the Selenium library. 
 It provides a more concise syntax that makes the code more readable and easier to understand.
 
 ### Key Features
 
+- Concise syntax
+- Less imports
 - Elements have an explicit wait time by default
+- Simple expected_conditions implementation as expect
 - Element type detection ( CSS & XPATH )
 
 ## Installation
 
 To install the library, use pip:
 
 ```bash
@@ -46,13 +49,13 @@
     yield driver
     driver.quit()
 
 def test_ddg_search_query(driver):
     keyword = 'github'
     driver.get('https://duckduckgo.com/')
     driver.element('[name=q]').send_keys(keyword, Keys.ENTER)
-    driver.wait_for.title_to_contain(keyword)
+    driver.expect.title_to_contain(keyword)
     titles = driver.elements('a[data-testid=result-title-a] span')
 
     for title in titles:
         assert keyword in title.text.lower()
 ```
```

### Comparing `selench-22.4.2024/selench/wait_for.py` & `selench-5.2.2024/selench/expect.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,377 +1,309 @@
-from typing import List
-
 from selenium.common import StaleElementReferenceException
-from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as ec
-from selenium.webdriver.support.wait import WebDriverWait
+
+from .element import Element
 
 
-class WaitFor:
+class Expect:
     """
     This class provides methods for waiting for certain conditions to be met in a web page
     using Selenium's WebDriverWait and ExpectedConditions.
     """
 
     def __init__(self, driver):
         self._driver = driver
 
-    def element_clickable(self, selector: str, timeout: int = None) -> WebElement:
+    def element_to_be_clickable(self, mark: Element | str) -> None:
         """
         An Expectation for checking an element is visible and enabled such that you can click it.
 
         Args:
-            selector: The selector of the element to wait for.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            The clickable element.
+            mark: Either a selector or an Element.
 
         Raises:
-            Exception: If the element is not clickable.
+            TimeoutException: If the element is not clickable.
         """
-        if not timeout: timeout = self._driver.wait
-        locator = self._driver._detect_locator_type(selector)
-        element = WebDriverWait(self._driver.webdriver, timeout).until(ec.element_to_be_clickable(locator),
-                                                                       "Element is not clickable")
-        return element
+        locator = (
+            mark.webelement
+            if isinstance(mark, Element)
+            else self._driver._detect_selector(mark)
+        )
+        self._driver.wait.until(
+            ec.element_to_be_clickable(locator), "Element is not clickable"
+        )
 
-    def element_visibility(self, selector: str, timeout: int = None) -> WebElement:
+    def element_to_be_visible(self, selector: str) -> None:
         """
         An expectation for checking that an element is present on the DOM of a page and visible.
         Visibility means that the element is not only displayed but also has a height and width
         that is greater than 0.
 
         Args:
-            selector: The selector of the element to wait for.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            The located and visible element.
+            selector: The selector of the element.
 
         Raises:
-            Exception: If the element is not visible within the given timeout.
+            TimeoutException: If the element is not visible within the given timeout.
         """
-        if not timeout: timeout = self._driver.wait
-        locator = self._driver._detect_locator_type(selector)
-        element = WebDriverWait(self._driver.webdriver, timeout).until(ec.visibility_of_element_located(locator),
-                                                                       "Element is not visible")
-        return element
+        locator = self._driver._detect_selector(selector)
+        self._driver.wait.until(
+            ec.visibility_of_element_located(locator), "Element is not visible"
+        )
 
-    def elements_visibility(self, selector: str, timeout: int = None) -> List[WebElement]:
+    def elements_to_be_visible(self, selector: str) -> None:
         """
         An expectation for checking that all elements are present on the DOM of a page and visible.
         Visibility means that the elements are not only displayed but also has a height and width
         that is greater than 0.
 
         Args:
             selector: The selector of the elements to wait for.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            A list of located and visible elements.
 
         Raises:
-            Exception: If the element are not visible within the given timeout.
+            TimeoutException: If the element are not visible within the given timeout.
         """
-        if not timeout: timeout = self._driver.wait
-        locator = self._driver._detect_locator_type(selector)
-        elements = WebDriverWait(self._driver.webdriver, timeout).until(ec.visibility_of_all_elements_located(locator),
-                                                                        "Not all elements are visible")
-        return elements
+        locator = self._driver._detect_selector(selector)
+        self._driver.wait.until(
+            ec.visibility_of_all_elements_located(locator),
+            "Not all elements are visible",
+        )
 
-    def element_invisibility(self, selector: str, timeout: int = None) -> WebElement:
+    def element_to_be_invisible(self, mark: Element | str) -> None:
         """
         An Expectation for checking that an element is either invisible or not present on the DOM.
 
         Args:
-            selector: The selector of the element to wait for.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            The invisible element.
+            mark: Either a selector or an Element.
 
         Raises:
-            Exception: If the element is not invisible within the given timeout.
+            TimeoutException: If the element is not invisible within the given timeout.
         """
-        if not timeout: timeout = self._driver.wait
-        locator = self._driver._detect_locator_type(selector)
-        element = WebDriverWait(self._driver.webdriver, timeout).until(ec.invisibility_of_element_located(locator),
-                                                                       "Element is not invisible")
-        return element
+        locator = (
+            mark.webelement
+            if isinstance(mark, Element)
+            else self._driver._detect_selector(mark)
+        )
+        self._driver.wait.until(
+            ec.invisibility_of_element_located(locator), "Element is not invisible"
+        )
 
-    def elements_invisibility(self, selector: str, timeout: int = None) -> List[WebElement]:
+    def elements_to_be_invisible(self, selector: str) -> None:
         """
-        An Expectation for checking that elements are either invisible or not present on the DOM.
+        An Expectation for checking that all elements are either invisible or not present on the DOM.
 
         Args:
             selector: The selector of the elements to wait for.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            A list of invisible elements.
 
         Raises:
-            Exception: If the elements are not invisible within the given timeout.
+            TimeoutException: If the elements are not invisible within the given timeout.
         """
-        if not timeout: timeout = self._driver.wait
-        locator = self._driver._detect_locator_type(selector)
-        elements = WebDriverWait(self._driver.webdriver, timeout).until(
-            self._visibility_of_all_elements_located(locator), "Elements are not invisible")
-        return elements
 
-    def element_staleness(self, element: WebElement, timeout: int = None) -> bool:
+        def invisibility_of_all_elements_located(locator):
+
+            def _predicate(driver):
+                try:
+                    elements = driver.find_elements(*locator)
+                    for element in elements:
+                        if element.is_displayed():
+                            return False
+                    return elements
+                except StaleElementReferenceException:
+                    return False
+
+            return _predicate
+
+        locator = self._driver._detect_selector(selector)
+        self._driver.wait.until(
+            invisibility_of_all_elements_located(locator), "Elements are not invisible"
+        )
+
+    def element_to_be_stale(self, element: Element) -> None:
         """
         Wait until an element is no longer attached to the DOM. element is the element to wait for.
 
         Args:
-            element: The WebElement to wait for.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            True if the element is no longer attached to the DOM.
+            element: The Element to wait for.
 
         Raises:
-            Exception: If the element is not stale.
+            TimeoutException: If the element is not stale.
         """
-        if not timeout: timeout = self._driver.wait
-        element = WebDriverWait(self._driver.webdriver, timeout).until(ec.staleness_of(element),
-                                                                       "Element did not go stale")
-        return element
+        self._driver.wait.until(
+            ec.staleness_of(element.webelement), "Element did not go stale"
+        )
 
-    def element_text(self, selector: str, timeout: int = None) -> bool:
+    def element_to_have_text(self, selector: str) -> None:
         """
         An expectation for checking if text is present in the specified element.
 
         Args:
-            selector: The selector of the element to wait for.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            True if text is present in the element.
+            selector: The selector of the element.
 
         Raises:
-            Exception: If the element does not contain text.
+            TimeoutException: If the element does not contain text.
         """
-        if not timeout: timeout = self._driver.wait
-        locator = self._driver._detect_locator_type(selector)
-        element = WebDriverWait(self._driver.webdriver, timeout).until(lambda d: bool(d.find_element(*locator).text),
-                                                                       "No text in element")
-        return element
+        locator = self._driver._detect_selector(selector)
+        self._driver.wait.until(
+            lambda d: bool(d.find_element(*locator).text), "No text in element"
+        )
 
-    def element_text_to_include(self, selector: str, text: str, timeout: int = None) -> bool:
+    def element_text_to_contain(self, selector: str, text: str) -> None:
         """
         An expectation for checking if the given text is present in the specified element.
 
         Args:
             selector: The selector of the element.
             text: The text to search for in the selected element's text.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            True if text is present in the element.
 
         Raises:
-            Exception: If the element does not contain text.
+            TimeoutException: If the element does not contain text.
 
         Example::
 
-            driver.wait_for.element_text_to_include('//div[@id="msg"]', 'welcome')
+            driver.expect.element_text_to_contain('//div[@id="msg"]', 'welcome')
         """
-        if not timeout: timeout = self._driver.wait
-        locator = self._driver._detect_locator_type(selector)
-        element = WebDriverWait(self._driver.webdriver, timeout).until(ec.text_to_be_present_in_element(locator, text),
-                                                                       f"Element text is not `{text}`")
-        return element
+        locator = self._driver._detect_selector(selector)
+        self._driver.wait.until(
+            ec.text_to_be_present_in_element(locator, text),
+            f"Element text is not `{text}`",
+        )
 
-    def element_text_to_be(self, selector: str, text: str, timeout: int = None) -> bool:
+    def element_text_to_be(self, selector: str, text: str) -> None:
         """
         An expectation for checking if the given text exactly matches the text within the specified element.
 
         Args:
             selector: The selector of the element.
             text: The expected text to be present within the element.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            True if the text exactly matches the element's text.
 
         Example::
 
-            driver.wait_for.element_text_to_be('#my-element', 'Hello')
+            driver.expect.element_text_to_be('#my-element', 'Hello')
         """
-
-        if not timeout: timeout = self._driver.wait
-        locator = self._driver._detect_locator_type(selector)
-        element = WebDriverWait(self._driver.webdriver, timeout).until(
+        locator = self._driver._detect_selector(selector)
+        self._driver.wait.until(
             lambda d: bool(d.find_element(*locator).text == text),
-            message=f"Element text doesn't match {text}"
+            f"Element text doesn't match {text}",
         )
-        return element
 
-    def element_attribute_text_to_include(self, selector: str, attribute: str, text: str, timeout: int = None) -> bool:
+    def element_attribute_text_to_contain(
+        self, selector: str, attribute: str, text: str
+    ) -> None:
         """
         An expectation for checking if the given text is present in the element’s attribute.
 
         Args:
             selector: The selector of the element.
             attribute: The name of the attribute to check for the presence of the given text.
             text: The text to search for in the selected element's attribute.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            True if text is present in the attribute.
 
         Raises:
-            Exception: If the element's attribute does not contain text.
+            TimeoutException: If the element's attribute does not contain text.
 
         Example::
 
-            driver.wait_for.element_attribute_text_to_include('//div[@id="msg"]', 'value', 'new message')
+            driver.expect.element_attribute_text_to_contain('//div[@id="msg"]', 'value', 'new message')
         """
-        if not timeout: timeout = self._driver.wait
-        locator = self._driver._detect_locator_type(selector)
-        element = WebDriverWait(self._driver.webdriver, timeout).until(ec.text_to_be_present_in_element_attribute(
-            locator, attribute, text), "Text is not present in attribute"
+        locator = self._driver._detect_selector(selector)
+        self._driver.wait.until(
+            ec.text_to_be_present_in_element_attribute(locator, attribute, text),
+            "Text is not present in attribute",
         )
-        return element
 
-    def element_selection_state(self, selector: str, is_selected: bool, timeout: int = None) -> bool:
+    def element_to_be_checked(self, selector: str) -> None:
         """
-        An expectation to locate an element and check if the selection state specified is in that state.
+        An expectation to locate an element and check if it's checked.
 
         Args:
-            selector: The selector of the element to wait for.
-            is_selected: True for checked False otherwise.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            True if the selection state specified is in that state.
+            selector: The selector of the element.
 
         Raises:
-            Exception: if the selection state specified is not in that state.
+            TimeoutException: if the selection state specified is not in that state.
+        """
+        locator = self._driver._detect_selector(selector)
+        self._driver.wait.until(
+            ec.element_located_selection_state_to_be(locator, True),
+            "Element is not checked",
+        )
 
-        Example::
+    def element_to_not_be_checked(self, selector: str) -> None:
+        """
+        An expectation to locate an element and check if it's not checked.
 
-            driver.wait_for.element_selection_state('input[type="checkbox"]', False)
+        Args:
+            selector: The selector of the element.
+
+        Raises:
+            TimeoutException: if the selection state specified is not in that state.
         """
-        if not timeout: timeout = self._driver.wait
-        locator = self._driver._detect_locator_type(selector)
-        element = WebDriverWait(self._driver.webdriver, timeout).until(
-            ec.element_located_selection_state_to_be(locator, is_selected),
-            "Element is not selected" if is_selected else "Element is selected")
-        return element
+        locator = self._driver._detect_selector(selector)
+        self._driver.wait.until(
+            ec.element_located_selection_state_to_be(locator, False),
+            "Element is checked",
+        )
 
-    def element_presence(self, selector: str, timeout: int = None) -> WebElement:
+    def element_to_be_present(self, selector: str) -> None:
         """
         An expectation for checking that an element is present on the DOM of a page.
 
         Args:
-            selector: The selector of the element to wait for.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            The DOM present element.
+            selector: The selector of the element.
 
         Raises:
-            Exception: If the element is not present on the DOM.
+            TimeoutException: If the element is not present on the DOM.
         """
-        if not timeout: timeout = self._driver.wait
-        locator = self._driver._detect_locator_type(selector)
-        element = WebDriverWait(self._driver.webdriver, timeout).until(ec.presence_of_element_located(locator),
-                                                                       "Element is not present on the DOM")
-        return element
+        locator = self._driver._detect_selector(selector)
+        self._driver.wait.until(
+            ec.presence_of_element_located(locator), "Element is not present on the DOM"
+        )
 
-    def url_to_be(self, url: str, timeout: int = None) -> bool:
+    def url_to_be(self, url: str) -> None:
         """
         An expectation for checking the current url is the expected url, which must be an exact match.
 
         Args:
             url: The expected url.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            True if the current url is the expected url.
 
         Raises:
-            Exception: if current url is not the expected url.
+            TimeoutException: if current url is not the expected url.
         """
-        if not timeout: timeout = self._driver.wait
-        element = WebDriverWait(self._driver.webdriver, timeout).until(ec.url_to_be(url),
-                                                                       f"{url} != {self._driver.url}")
-        return element
+        self._driver.wait.until(ec.url_to_be(url), f"{url} != {self._driver.url}")
 
-    def url_to_include(self, string: str, timeout: int = None) -> bool:
+    def url_to_contain(self, string: str) -> None:
         """
         An expectation for checking that the current url contains a case-sensitive substring.
 
         Args:
             string: The expected case-sensitive substring.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            True if the current url contains the string.
 
         Raises:
-            Exception: if the current url does not contain the string.
+            TimeoutException: if the current url does not contain the string.
         """
-        if not timeout: timeout = self._driver.wait
-        element = WebDriverWait(self._driver.webdriver, timeout).until(ec.url_contains(string),
-                                                                       f"`{self._driver.url}` does not contain `{string}`")
-        return element
+        self._driver.wait.until(
+            ec.url_contains(string), f"`{self._driver.url}` does not contain `{string}`"
+        )
 
-    def title_to_be(self, title: str, timeout: int = None) -> bool:
+    def title_to_be(self, title: str) -> None:
         """
         An expectation for checking the title of a page. title is the expected title, which must be an exact match.
 
         Args:
             title: The expected title.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            True if the title matches.
 
         Raises:
-            Exception: if the title doesn't match.
+            TimeoutException: if the title doesn't match.
         """
-        if not timeout: timeout = self._driver.wait
-        element = WebDriverWait(self._driver.webdriver, timeout).until(ec.title_is(title),
-                                                                       f"`{title} != {self._driver.title}")
-        return element
+        self._driver.wait.until(ec.title_is(title), f"`{title} != {self._driver.title}")
 
-    def title_to_contain(self, string: str, timeout: int = None) -> bool:
+    def title_to_contain(self, string: str) -> None:
         """
         An expectation for checking that the title contains a case-sensitive substring.
 
         Args:
             string: The expected case-sensitive substring.
-            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
-
-        Returns:
-            True if the current title contains the string.
 
         Raises:
-            Exception: if the current title does not contain the string.
+            TimeoutException: if the current title does not contain the string.
         """
-        if not timeout: timeout = self._driver.wait
-        element = WebDriverWait(self._driver.webdriver, timeout).until(ec.title_contains(string),
-                                                                       f"`{self._driver.title}` does not contain `{string}`")
-        return element
-
-    """
-     * Custom "Expected Conditions" *
-    """
-
-    @staticmethod
-    def _visibility_of_all_elements_located(locator):
-
-        def _predicate(driver):
-            try:
-                elements = driver.find_elements(*locator)
-                for element in elements:
-                    if element.is_displayed():
-                        return False
-                return elements
-            except StaleElementReferenceException:
-                return False
-
-        return _predicate
+        self._driver.wait.until(
+            ec.title_contains(string),
+            f"`{self._driver.title}` does not contain `{string}`",
+        )
```

### Comparing `selench-22.4.2024/selench.egg-info/PKG-INFO` & `selench-5.2.2024/selench.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selench
-Version: 22.4.2024
+Version: 5.2.2024
 Summary: Selenium wrapper for Python
 Home-page: https://github.com/dsymbol/selench
 Author: dsymbol
 License: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -15,15 +15,18 @@
 # Selench
 
 Selench is a wrapper that simplifies the use of the Selenium library. 
 It provides a more concise syntax that makes the code more readable and easier to understand.
 
 ### Key Features
 
+- Concise syntax
+- Less imports
 - Elements have an explicit wait time by default
+- Simple expected_conditions implementation as expect
 - Element type detection ( CSS & XPATH )
 
 ## Installation
 
 To install the library, use pip:
 
 ```bash
@@ -60,13 +63,13 @@
     yield driver
     driver.quit()
 
 def test_ddg_search_query(driver):
     keyword = 'github'
     driver.get('https://duckduckgo.com/')
     driver.element('[name=q]').send_keys(keyword, Keys.ENTER)
-    driver.wait_for.title_to_contain(keyword)
+    driver.expect.title_to_contain(keyword)
     titles = driver.elements('a[data-testid=result-title-a] span')
 
     for title in titles:
         assert keyword in title.text.lower()
 ```
```

### Comparing `selench-22.4.2024/setup.py` & `selench-5.2.2024/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selench',
-    version='22.04.2024',
+    version='5.2.2024',
     packages=find_packages(),
     url='https://github.com/dsymbol/selench',
     license='OSI Approved :: MIT License',
     author='dsymbol',
     description='Selenium wrapper for Python',
     include_package_data=True,
     long_description=open("README.md", encoding='utf-8').read(),
```

### Comparing `selench-22.4.2024/tests/test_action.py` & `selench-5.2.2024/tests/test_action.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 import shared
 
 
 def test_hover(driver):
     driver.get(f'{shared.CBT}/hover-menu.html')
-    dd_element = driver.xpath_element('//li[@class="dropdown"] /a')
-    driver.hover(dd_element)
-    new_visible_elements = driver.xpath_elements('//ul[@class="dropdown-menu"] //li /a[not(@onclick)]')
+    driver.element('//li[@class="dropdown"] /a').hover()
+    new_visible_elements = driver.elements('//ul[@class="dropdown-menu"] //li /a[not(@onclick)]')
     assert all([i.is_displayed for i in new_visible_elements])
 
 
 def test_double_click(driver):
     driver.get('https://www.javatpoint.com/oprweb/test.jsp?filename=javascript-dblclick-event1')
     driver.switch_frame('//iframe[@id="iframewrapper"]')
-    dbl_element = driver.xpath_element('//*[@id="heading"]')
-    driver.double_click(dbl_element)
-    dbl_element = driver.xpath_element('//*[@id="heading"]')
-    assert "javatpoint.com" in dbl_element.text.lower()
+    driver.element('//*[@id="heading"]').double_click()
+    assert "javatpoint.com" in driver.element('//*[@id="heading"]').text.lower()
 
 
 def test_right_click(driver):
     driver.get(f'{shared.INTERNET}/context_menu')
-    rclick_element = driver.css_element('div[id=hot-spot]')
-    driver.right_click(rclick_element)
+    driver.element('div[id=hot-spot]').right_click()
     alert = driver.alert()
     assert alert.text.lower() == 'you selected a context menu'
 
 
 def test_drag_and_drop(driver):
     expected = 'Dropped!'
     driver.get(f'{shared.CBT}/drag-and-drop.html')
-    drag = driver.css_element('#draggable')
-    drop = driver.css_element('#droppable')
-    driver.drag_and_drop(drag, drop)
-    driver.wait_for.element_text_to_be('div[id=droppable] p', expected)
-    assert driver.css_element('div[id=droppable] p').text == expected
+    drag = driver.element('#draggable')
+    drop = driver.element('#droppable')
+    drag.drag_to(drop)
+    driver.expect.element_text_to_be('div[id=droppable] p', expected)
+    assert driver.element('div[id=droppable] p').text == expected
 
     driver.get(f'{shared.INTERNET}/drag_and_drop')
-    drag = driver.css_element('div[id=column-a]')
-    drop = driver.css_element('div[id=column-b]')
-    driver.drag_and_drop(drag, drop)
-    assert driver.css_element('div[id=column-a] header').text.lower() == 'b'
+    drag = driver.element('div[id=column-a]')
+    drop = driver.element('div[id=column-b]')
+    drag.drag_to(drop)
+    assert driver.element('div[id=column-a] header').text.lower() == 'b'
 
     driver.get(f'https://dineshvelhal.github.io/testautomation-playground/mouse_events.html')
-    drag = driver.css_element('#drag_source')
-    drop = driver.css_element('#drop_target')
-    driver.drag_and_drop(drag, drop)
+    drag = driver.element('#drag_source')
+    drop = driver.element('#drop_target')
+    drag.drag_to(drop)
     assert "success" in drop.text.lower()
```

### Comparing `selench-22.4.2024/tests/test_custom.py` & `selench-5.2.2024/tests/test_custom.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 from selench import Keys
 
 import shared
 
 
 def test_basic_auth(driver):
     driver.basic_auth(f'{shared.INTERNET}/basic_auth', 'admin', 'admin')
-    assert 'congratulations' in driver.css_element('div[class=example] p').text.lower()
+    assert 'congratulations' in driver.element('div[class=example] p').text.lower()
     driver.basic_auth(f'{shared.INTERNET}/digest_auth', 'admin', 'admin')
-    assert 'congratulations' in driver.css_element('div[class=example] p').text.lower()
+    assert 'congratulations' in driver.element('div[class=example] p').text.lower()
 
 
 def test_detect_elements(driver):
     keyword = "husky"
     driver.get(shared.DUCK)
     driver.element('input[placeholder]').send_keys(keyword, Keys.ENTER)
     results = driver.elements('article h2 span')
     for i in results:
         assert keyword in i.text.lower()
 
 
 def test_locator_type(driver):
     css_examples = ['.foo:empty', '#foo', '#foo p', '.foo[bar^="fum"]', 'a:visited', 'h2', '.foo[bar*="fum"]']
     xpath_examples = ['//hr[@class="edge" and position()=1]', './div/b', '//a/@href', '//*[count(*)=3]', '//E/*[1]']
-    css_test = [driver._detect_locator_type(i) for i in css_examples]
-    xpath_test = [driver._detect_locator_type(i) for i in xpath_examples]
+    css_test = [driver._detect_selector(i) for i in css_examples]
+    xpath_test = [driver._detect_selector(i) for i in xpath_examples]
     assert all(["css" in i[0] for i in css_test])
     assert all(["xpath" in i[0] for i in xpath_test])
-
-
-def test_element_exist_visible(driver):
-    driver.get("https://github.com")
-    selector = '.text-right [aria-label="Toggle navigation"]'
-    assert driver.elements_exist(selector)
-    assert driver.elements_visible(selector)
-    driver.maximize()
-    assert not driver.elements_visible(selector)
```

### Comparing `selench-22.4.2024/tests/test_switch_to.py` & `selench-5.2.2024/tests/test_switch_to.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     driver.switch_window(name=first_window)
     assert driver.current_window_handle == first_window
 
 
 def test_switch_frame(driver):
     driver.get(f"{shared.INTERNET}/iframe")
     driver.switch_frame('iframe[id=mce_0_ifr]')
-    textarea = driver.css_element('body')
+    textarea = driver.element('body')
     textarea.clear()
     textarea.send_keys('tests')
     assert textarea.text == 'tests'
     driver.leave_frame()
-    assert driver.css_element('iframe[id=mce_0_ifr]')
+    assert driver.element('iframe[id=mce_0_ifr]')
 
 
 def test_alert(driver):
     driver.get(f"{shared.INTERNET}/javascript_alerts")
-    result = driver.css_element('#result')
-    driver.css_element('button[onclick*=Alert]').click()
+    result = driver.element('#result')
+    driver.element('button[onclick*=Alert]').click()
     driver.alert().dismiss()
     assert result.text.lower() == "you successfully clicked an alert"
-    driver.css_element('button[onclick*=Confirm]').click()
+    driver.element('button[onclick*=Confirm]').click()
     driver.alert().accept()
     assert result.text.lower() == "you clicked: ok"
-    driver.css_element('button[onclick*=Prompt]').click()
+    driver.element('button[onclick*=Prompt]').click()
     driver.alert().send_keys('tests')
     driver.alert().accept()
     assert result.text.lower() == "you entered: tests"
```

