# Comparing `tmp/azubiheftApi-0.0.93.tar.gz` & `tmp/azubiheftapi-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azubiheftApi-0.0.93.tar", last modified: Wed Mar 20 08:42:30 2024, max compression
+gzip compressed data, was "azubiheftapi-0.0.94.tar", last modified: Fri Apr 26 19:18:53 2024, max compression
```

## Comparing `azubiheftApi-0.0.93.tar` & `azubiheftapi-0.0.94.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:42:30.078007 azubiheftApi-0.0.93/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-20 08:42:23.000000 azubiheftApi-0.0.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-20 08:42:30.078007 azubiheftApi-0.0.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-20 08:42:23.000000 azubiheftApi-0.0.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:42:30.074007 azubiheftApi-0.0.93/azubiheftApi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 08:42:23.000000 azubiheftApi-0.0.93/azubiheftApi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-03-20 08:42:23.000000 azubiheftApi-0.0.93/azubiheftApi/azubiheftApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-20 08:42:23.000000 azubiheftApi-0.0.93/azubiheftApi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:42:30.074007 azubiheftApi-0.0.93/azubiheftApi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-20 08:42:30.000000 azubiheftApi-0.0.93/azubiheftApi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-20 08:42:30.000000 azubiheftApi-0.0.93/azubiheftApi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 08:42:30.000000 azubiheftApi-0.0.93/azubiheftApi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-20 08:42:30.000000 azubiheftApi-0.0.93/azubiheftApi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-20 08:42:30.000000 azubiheftApi-0.0.93/azubiheftApi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 08:42:30.078007 azubiheftApi-0.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-20 08:42:23.000000 azubiheftApi-0.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:18:53.308330 azubiheftapi-0.0.94/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-26 19:18:53.308330 azubiheftapi-0.0.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:18:53.308330 azubiheftapi-0.0.94/azubiheftApi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/azubiheftApi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17838 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/azubiheftApi/azubiheftApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/azubiheftApi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:18:53.308330 azubiheftapi-0.0.94/azubiheftApi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-26 19:18:53.000000 azubiheftapi-0.0.94/azubiheftApi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-26 19:18:53.000000 azubiheftapi-0.0.94/azubiheftApi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:18:53.000000 azubiheftapi-0.0.94/azubiheftApi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 19:18:53.000000 azubiheftapi-0.0.94/azubiheftApi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 19:18:53.000000 azubiheftapi-0.0.94/azubiheftApi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:18:53.308330 azubiheftapi-0.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/setup.py
```

### Comparing `azubiheftApi-0.0.93/LICENSE` & `azubiheftapi-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `azubiheftApi-0.0.93/PKG-INFO` & `azubiheftapi-0.0.94/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azubiheftApi
-Version: 0.0.93
+Version: 0.0.94
 Summary: Azubiheft.de custom api
 Home-page: https://github.com/leonkohli/azubiheft-api
 Author: Leon Kohlhaussen
 Author-email: kohli.leon@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -20,16 +20,14 @@
 
 [![Downloads](https://static.pepy.tech/badge/azubiheftapi)](https://pepy.tech/project/azubiheftapi)
 [![Downloads](https://static.pepy.tech/badge/azubiheftapi/month)](https://pepy.tech/project/azubiheftapi)
 [![Downloads](https://static.pepy.tech/badge/azubiheftapi/week)](https://pepy.tech/project/azubiheftapi)
 
 This library provides a Python wrapper for azubiheft.com. With this library, developers can easily manage their Ausbildung (training) reports through a script, allowing for enhanced automation and better control over their Ausbildung documentation.
 
-> 🚀 **Note**: This API wrapper is unofficial and independent of the official Azubiheft platform. This repository stands as a tribute to [joshmuente/azubiheft-api](https://github.com/joshmuente/azubiheft-api). Heartfelt thanks to the original creator.
-
 ## 📖 About Azubiheft
 
 Azubiheft brings a streamlined online approach to training documentation. Designed for businesses, instructors, and apprentices, it offers an effortless way to manage every training entry online. With Azubiheft, you're always one step ahead with all your training data right at your fingertips.
 
 ## 🛠 Installation
 
 ```bash
```

### Comparing `azubiheftApi-0.0.93/README.md` & `azubiheftapi-0.0.94/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 [![Downloads](https://static.pepy.tech/badge/azubiheftapi)](https://pepy.tech/project/azubiheftapi)
 [![Downloads](https://static.pepy.tech/badge/azubiheftapi/month)](https://pepy.tech/project/azubiheftapi)
 [![Downloads](https://static.pepy.tech/badge/azubiheftapi/week)](https://pepy.tech/project/azubiheftapi)
 
 This library provides a Python wrapper for azubiheft.com. With this library, developers can easily manage their Ausbildung (training) reports through a script, allowing for enhanced automation and better control over their Ausbildung documentation.
 
-> 🚀 **Note**: This API wrapper is unofficial and independent of the official Azubiheft platform. This repository stands as a tribute to [joshmuente/azubiheft-api](https://github.com/joshmuente/azubiheft-api). Heartfelt thanks to the original creator.
-
 ## 📖 About Azubiheft
 
 Azubiheft brings a streamlined online approach to training documentation. Designed for businesses, instructors, and apprentices, it offers an effortless way to manage every training entry online. With Azubiheft, you're always one step ahead with all your training data right at your fingertips.
 
 ## 🛠 Installation
 
 ```bash
```

### Comparing `azubiheftApi-0.0.93/azubiheftApi/azubiheftApi.py` & `azubiheftapi-0.0.94/azubiheftApi/azubiheftApi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/python3
 # azubiheft.com web-api
 
 import requests
-from bs4 import BeautifulSoup
+from bs4 import BeautifulSoup, NavigableString
 from datetime import datetime, timedelta
 from .errors import AuthError, ValueTooLargeError, NotLoggedInError
 import time
 from typing import List
 import urllib.parse
+import re
 
 
 class Entry:
     def __init__(self, date: datetime, message: str, time_spent: str, entry_type: int):
         self.date = date
         self.message = message
         self.time_spent = time_spent
@@ -252,14 +253,21 @@
                 }
                 subjects.append(subject)
 
             return staticSubjects + subjects
 
         else:
             raise NotLoggedInError("not logged in. Login first")
+        
+    def get_art_id_from_text(self, subject_name: str) -> str:
+        subjects = self.getSubjects()  # Retrieve all subjects
+        for subject in subjects:
+            if subject_name in subject['name']:
+                return subject['id']
+        return None  # Return None if no match found
 
     def writeReports(self, entries: List[Entry]) -> None:
         """Writes a list of reports to the Azubiheft.
         - Parameters:
             entries: List of reports to be written.
         """
         if not self.isLoggedIn():
@@ -310,17 +318,18 @@
         """Writes a report to the Azubiheft.
         - Parameters:
             date: Date of the report.
             message: Message of the report.
             time_spent: Time spent on the report.
             entry_type: Type of the report.
         """
-        entry = Entry(date, message, time_spent, entry_type)
-        self.writeReports([entry])
-
+        if time_spent.strip() != "00:00":
+            entry = Entry(date, message, time_spent, entry_type)
+            self.writeReports([entry])
+            
     def getReport(self, date: datetime, include_formatting: bool = False):
         if not self.isLoggedIn():
             raise NotLoggedInError("not logged in. Login first")
 
         url = (
             "https://www.azubiheft.de/Azubi/Tagesbericht.aspx?Datum="
             + TimeHelper.dateTimeToString(date)
@@ -331,48 +340,127 @@
         reports = []
 
         # Find all report entries
         entries = soup.find_all("div", class_="d0 mo")
         for entry in entries:
             # Extract the duration and type of activity
             duration = entry.find("div", class_="row2 d4").get_text(strip=True)
+            if duration.strip() == "00:00":
+                continue
             activity_type = (
                 entry.find("div", class_="row1 d3")
                 .get_text(strip=True)
                 .replace("Art: ", "")
             )
+            seq = entry.get("data-seq")  # Extract the sequence number
 
             # Extract and format the report text
             report_text_div = entry.find("div", class_="row7 d5")
             if include_formatting:
                 # Replace <br> tags with newline characters
                 for br in report_text_div.find_all("br"):
                     br.replace_with("\n")
-                # Convert <div> tags to newline characters
-                report_text = "\n".join(
-                    [
-                        div.get_text(strip=True)
-                        for div in report_text_div.find_all("div", recursive=False)
-                    ]
-                )
-                # If there are no <div> tags, get the whole text directly
-                if not report_text:
-                    report_text = report_text_div.get_text("\n", strip=True)
+
+                # Convert <div> tags to newline characters while preserving whitespace
+                report_text_parts = []
+                for element in report_text_div.contents:
+                    if isinstance(element, NavigableString):
+                        report_text_parts.append(str(element))
+                    elif element.name == "div":
+                        report_text_parts.append("\n" + element.get_text(strip=False))
+
+                report_text = "".join(report_text_parts)
+                report_text = re.sub(r"\n+", "\n", report_text.strip())
             else:
                 # Concatenate all text without formatting
                 report_text = " ".join(report_text_div.stripped_strings)
 
             reports.append(
-                {"type": activity_type, "duration": duration, "text": report_text}
+                {
+                    "seq": seq,
+                    "type": activity_type,
+                    "duration": duration,
+                    "text": report_text,
+                }
             )
 
         if len(reports) == 0:
             print("No Reports")
         else:
             return reports
+        
+    def deleteReport(self, date: datetime, entry_number: int = None) -> None:
+        if not self.isLoggedIn():
+            raise NotLoggedInError("not logged in. Login first")
+
+        # Retrieve the report for the specified date
+        report_entries = self.getReport(date)
+        if not report_entries:
+            print("No report entries found for this date.")
+            return
+
+        if entry_number is None:
+            # Display report entries and ask user which to delete
+            for i, entry in enumerate(report_entries, 1):
+                print(
+                    f"{i}. {entry['type']} - {entry['text']} - {entry['duration']}")
+            print("all. Delete all entries")
+            choice = input(
+                "Select the number of the entry to delete (or 'all' to delete everything): ")
+        else:
+            choice = str(entry_number)
+
+        if choice.isdigit():
+            choice = int(choice) - 1
+            if choice < 0 or choice >= len(report_entries):
+                print("Invalid entry number.")
+                return
+            entries_to_delete = [report_entries[choice]]
+        elif choice == "all":
+            entries_to_delete = report_entries
+        else:
+            print("Invalid choice.")
+            return
+
+        # Retrieve the week number for the specified date
+        week_number = self.getReportWeekId(date)
+
+        headers = {
+            'x-my-ajax-request': 'ajax',
+            'Origin': 'https://www.azubiheft.de',
+            'Referer': 'https://www.azubiheft.de/',
+            'Sec-Fetch-Dest': 'empty',
+            'Sec-Fetch-Mode': 'cors',
+            'Sec-Fetch-Site': 'same-origin',
+            'Pragma': 'no-cache',
+            'Cache-Control': 'no-cache',
+        }
+
+        # Loop through and delete each selected entry
+        for entry in entries_to_delete:
+            formData = {
+                'disablePaste': '0',
+                'Seq': f"-{entry['seq']}",
+                'Art_ID': self.get_art_id_from_text(entry['type']),
+                'Abt_ID': '0',
+                'Dauer': entry['duration'],
+                'Inhalt': entry['text'],
+                'jsVer': '12'
+            }
+
+            url = f"https://www.azubiheft.de/Azubi/XMLHttpRequest.ashx?Datum={TimeHelper.dateTimeToString(
+                date)}&BrNr={week_number}&BrSt=1&BrVorh=Yes&T={TimeHelper.getActualTimestamp()}"
+
+            response = self.session.post(url, headers=headers, data=formData)
+            if response.status_code != 200:
+                print(f"Failed to delete entry: {
+                      entry['text']}. Response code: {response.status_code}")
+            else:
+                print(f"Entry deleted successfully: {entry['text']}")
+
 
 
 class TimeHelper:
     @staticmethod
     def dateTimeToString(date: datetime) -> str:
         return date.strftime("%Y%m%d")
```

### Comparing `azubiheftApi-0.0.93/azubiheftApi.egg-info/PKG-INFO` & `azubiheftapi-0.0.94/azubiheftApi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azubiheftApi
-Version: 0.0.93
+Version: 0.0.94
 Summary: Azubiheft.de custom api
 Home-page: https://github.com/leonkohli/azubiheft-api
 Author: Leon Kohlhaussen
 Author-email: kohli.leon@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -20,16 +20,14 @@
 
 [![Downloads](https://static.pepy.tech/badge/azubiheftapi)](https://pepy.tech/project/azubiheftapi)
 [![Downloads](https://static.pepy.tech/badge/azubiheftapi/month)](https://pepy.tech/project/azubiheftapi)
 [![Downloads](https://static.pepy.tech/badge/azubiheftapi/week)](https://pepy.tech/project/azubiheftapi)
 
 This library provides a Python wrapper for azubiheft.com. With this library, developers can easily manage their Ausbildung (training) reports through a script, allowing for enhanced automation and better control over their Ausbildung documentation.
 
-> 🚀 **Note**: This API wrapper is unofficial and independent of the official Azubiheft platform. This repository stands as a tribute to [joshmuente/azubiheft-api](https://github.com/joshmuente/azubiheft-api). Heartfelt thanks to the original creator.
-
 ## 📖 About Azubiheft
 
 Azubiheft brings a streamlined online approach to training documentation. Designed for businesses, instructors, and apprentices, it offers an effortless way to manage every training entry online. With Azubiheft, you're always one step ahead with all your training data right at your fingertips.
 
 ## 🛠 Installation
 
 ```bash
```

### Comparing `azubiheftApi-0.0.93/setup.py` & `azubiheftapi-0.0.94/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="azubiheftApi",
-    version="0.0.93",
+    version="0.0.94",
     author="Leon Kohlhaussen",
     author_email="kohli.leon@gmail.com",
     description="Azubiheft.de custom api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/leonkohli/azubiheft-api",
     packages=setuptools.find_packages(),
```

