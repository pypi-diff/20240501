# Comparing `tmp/librus_apix-0.7.4.tar.gz` & `tmp/librus_apix-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.7.4.tar", last modified: Tue Apr 30 10:49:02 2024, max compression
+gzip compressed data, was "librus_apix-0.7.5.tar", last modified: Tue Apr 30 15:40:25 2024, max compression
```

## Comparing `librus_apix-0.7.4.tar` & `librus_apix-0.7.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:49:02.389091 librus_apix-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 10:48:59.000000 librus_apix-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-30 10:49:02.389091 librus_apix-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-30 10:48:59.000000 librus_apix-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:49:02.389091 librus_apix-0.7.4/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/get_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:49:02.389091 librus_apix-0.7.4/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-30 10:49:02.000000 librus_apix-0.7.4/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-30 10:49:02.000000 librus_apix-0.7.4/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:49:02.000000 librus_apix-0.7.4/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 10:49:02.000000 librus_apix-0.7.4/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 10:49:02.000000 librus_apix-0.7.4/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 10:48:59.000000 librus_apix-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 10:49:02.389091 librus_apix-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 10:48:59.000000 librus_apix-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:40:25.684041 librus_apix-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 15:40:23.000000 librus_apix-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-30 15:40:25.684041 librus_apix-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-30 15:40:23.000000 librus_apix-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:40:25.680041 librus_apix-0.7.5/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/get_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-30 15:40:23.000000 librus_apix-0.7.5/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:40:25.684041 librus_apix-0.7.5/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-30 15:40:25.000000 librus_apix-0.7.5/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-30 15:40:25.000000 librus_apix-0.7.5/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:40:25.000000 librus_apix-0.7.5/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 15:40:25.000000 librus_apix-0.7.5/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 15:40:25.000000 librus_apix-0.7.5/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 15:40:23.000000 librus_apix-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 15:40:25.684041 librus_apix-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:40:23.000000 librus_apix-0.7.5/setup.py
```

### Comparing `librus_apix-0.7.4/LICENSE` & `librus_apix-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/README.md` & `librus_apix-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/librus_apix/announcements.py` & `librus_apix-0.7.5/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/librus_apix/attendance.py` & `librus_apix-0.7.5/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/librus_apix/completed_lessons.py` & `librus_apix-0.7.5/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/librus_apix/get_token.py` & `librus_apix-0.7.5/librus_apix/get_token.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/librus_apix/grades.py` & `librus_apix-0.7.5/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/librus_apix/homework.py` & `librus_apix-0.7.5/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/librus_apix/messages.py` & `librus_apix-0.7.5/librus_apix/messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,27 +12,29 @@
     author: str
     title: str
     date: str
     href: str
     unread: bool
     has_attachment: bool
 
+
 def recipient_groups(token) -> List[str]:
     soup = no_access_check(
         BeautifulSoup(token.get(token.RECIPIENT_GROUPS_URL).text, "lxml")
     )
     groups = []
     trs = soup.select("table.message-recipients > tbody > tr")
     for tr in trs:
         radio = tr.select_one("input.recipiantTypeRadio")
         if radio is None:
             raise ParseError("Error getting groups (radio)")
         groups.append(radio.attrs.get("value", ""))
     return groups
 
+
 def get_recipients(token: Token, group: str):
     payload = {
         "typAdresata": group,
         "poprzednia": 5,
         "tabZaznaczonych": "",
         "czyWirtualneKlasy": False,
         "idGrupy": 0,
@@ -62,19 +64,26 @@
         "Rodzaj": 0,
         "temat": title,
         "tresc": content,
         "poprzednia": 5,
         "fileStorageIdentifier": "",
         "wyslij": "Wyślij",
     }
-    sent_message = token.post(token.SEND_MESSAGE_URL, data=payload)
+    sent_message = no_access_check(
+        BeautifulSoup(token.post(token.SEND_MESSAGE_URL, data=payload).text, "lxml")
+    )
+    result = sent_message.select_one("div.container-background > p")
+    if result is None:
+        raise ParseError("Error getting the result of the message!")
+    result = result.text
+    if "nie zostala" in result.text:
+        return {False, result}
     if sent_message.status_code == 200:
-        return True
-
-    return False
+        return {True, result}
+    return {False, result}
 
 
 def message_content(token: Token, content_url: str) -> str:
     soup = no_access_check(
         BeautifulSoup(token.get(token.MESSAGE_URL + "/" + content_url).text, "lxml")
     )
     content = soup.find("div", attrs={"class": "container-message-content"})
```

### Comparing `librus_apix-0.7.4/librus_apix/schedule.py` & `librus_apix-0.7.5/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/librus_apix/student_information.py` & `librus_apix-0.7.5/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/librus_apix/timetable.py` & `librus_apix-0.7.5/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/librus_apix/urls.py` & `librus_apix-0.7.5/librus_apix/urls.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.7.5/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.4/setup.cfg` & `librus_apix-0.7.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = 0.7.4
+version = 0.7.5
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

