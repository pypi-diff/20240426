# Comparing `tmp/pdftext-0.1.1.tar.gz` & `tmp/pdftext-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftext-0.1.1.tar", max compression
+gzip compressed data, was "pdftext-0.1.2.tar", max compression
```

## Comparing `pdftext-0.1.1.tar` & `pdftext-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11269 2024-04-25 22:26:10.211937 pdftext-0.1.1/LICENSE
--rw-r--r--   0        0        0     6065 2024-04-25 22:26:10.211937 pdftext-0.1.1/README.md
--rw-r--r--   0        0        0     1198 2024-04-25 22:26:10.211937 pdftext-0.1.1/extract_text.py
--rw-r--r--   0        0        0    11225 2024-04-25 22:26:10.211937 pdftext-0.1.1/models/dt.joblib
--rw-r--r--   0        0        0     2225 2024-04-25 22:26:10.211937 pdftext-0.1.1/pdftext/extraction.py
--rw-r--r--   0        0        0     5701 2024-04-25 22:26:10.211937 pdftext-0.1.1/pdftext/inference.py
--rw-r--r--   0        0        0      153 2024-04-25 22:26:10.211937 pdftext-0.1.1/pdftext/model.py
--rw-r--r--   0        0        0     3078 2024-04-25 22:26:10.211937 pdftext-0.1.1/pdftext/pdf/chars.py
--rw-r--r--   0        0        0     3082 2024-04-25 22:26:10.211937 pdftext-0.1.1/pdftext/pdf/utils.py
--rw-r--r--   0        0        0     2202 2024-04-25 22:26:10.211937 pdftext-0.1.1/pdftext/postprocessing.py
--rw-r--r--   0        0        0      478 2024-04-25 22:26:10.211937 pdftext-0.1.1/pdftext/settings.py
--rw-r--r--   0        0        0      856 2024-04-25 22:26:10.211937 pdftext-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7041 1970-01-01 00:00:00.000000 pdftext-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11269 2024-04-26 05:34:48.558207 pdftext-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6486 2024-04-26 05:34:48.558207 pdftext-0.1.2/README.md
+-rw-r--r--   0        0        0     1198 2024-04-26 05:34:48.558207 pdftext-0.1.2/extract_text.py
+-rw-r--r--   0        0        0    18905 2024-04-26 05:34:48.562207 pdftext-0.1.2/models/dt.joblib
+-rw-r--r--   0        0        0     2225 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/extraction.py
+-rw-r--r--   0        0        0     5786 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/inference.py
+-rw-r--r--   0        0        0      153 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/model.py
+-rw-r--r--   0        0        0     3186 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/pdf/chars.py
+-rw-r--r--   0        0        0     3353 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/pdf/utils.py
+-rw-r--r--   0        0        0     2129 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/postprocessing.py
+-rw-r--r--   0        0        0      478 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/settings.py
+-rw-r--r--   0        0        0      856 2024-04-26 05:34:48.562207 pdftext-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7462 1970-01-01 00:00:00.000000 pdftext-0.1.2/PKG-INFO
```

### Comparing `pdftext-0.1.1/LICENSE` & `pdftext-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftext-0.1.1/README.md` & `pdftext-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # PDFText
 
 Text extraction like [PyMuPDF](https://github.com/pymupdf/PyMuPDF), but without the AGPL license.  PDFText extracts plain text or structured blocks and lines.  It's built on [pypdfium2](https://github.com/pypdfium2-team/pypdfium2), so it's [fast, accurate](#benchmarks), and Apache licensed.
 
+## Community
+
+[Discord](https://discord.gg//KuZwXNGnfH) is where we discuss future development.
+
 # Installation
 
 You'll need python 3.9+ first.  Then run `pip install pdftext`.
 
 # Usage
 
 - Inspect the settings in `pdftext/settings.py`.  You can override any settings with environment variables.
@@ -73,33 +77,33 @@
 text = dictionary_output(PDF_PATH)
 ```
 
 If you want more customization, check out the `pdftext.extraction._get_pages` function for a starting point to dig deeper.  pdftext is a pretty thin wrapper around [pypdfium2](https://pypdfium2.readthedocs.io/en/stable/), so you might want to look at the documentation for that as well.
 
 # Benchmarks
 
-I benchmarked extraction speed and accuracy of [pymupdf](https://pymupdf.readthedocs.io/en/latest/), [pdfplumber](https://github.com/jsvine/pdfplumber), and pdftext.  I chose pymupdf because it extracts blocks and lines.  Pdfplumber extracts words and bboxes.  I did not benchmark pypdf, even though it is a great library, because it doesn't provide individual words/lines and bbox information.
+I benchmarked extraction speed and accuracy of [pymupdf](https://pymupdf.readthedocs.io/en/latest/), [pdfplumber](https://github.com/jsvine/pdfplumber), and pdftext.  I chose pymupdf because it extracts blocks and lines.  Pdfplumber extracts words and bboxes.  I did not benchmark pypdf, even though it is a great library, because it doesn't provide individual character/line/block and bbox information.
 
-Here are the scores:
+Here are the scores, run on an M1 Macbook, without multiprocessing:
 
 | Library    | Time (s per page) | Alignment Score (% accuracy vs pymupdf) |
 |------------|-------------------|-----------------------------------------|
 | pymupdf    | 0.32              | --                                      |
-| pdftext    | 1.79              | 96.22                                   |
-| pdfplumber | 3.0               | 89.88                                   |
+| pdftext    | 1.4               | 97.76                                   |
+| pdfplumber | 3.0               | 90.3                                    |
 
-pdftext is approximately 2x slower than using pypdfium2 alone (if you were to extract all the same information).
+pdftext is approximately 2x slower than using pypdfium2 alone (if you were to extract all the same character information).
 
 There are additional benchmarks for pypdfium2 and other tools [here](https://github.com/py-pdf/benchmarks).
 
 ## Methodology
 
 I used a benchmark set of 200 pdfs extracted from [common crawl](https://huggingface.co/datasets/pixparse/pdfa-eng-wds), then processed by a team at HuggingFace.
 
-For each library, I used a detailed extraction method, to pull out font information, as well as just the words.  This ensured we were comparing similar performance numbers.
+For each library, I used a detailed extraction method, to pull out font information, as well as just the words.  This ensured we were comparing similar performance numbers.  I formatted the text similarly when extracting - newlines after lines, and double newlines after blocks.  For pdfplumber, I could only do the newlines after lines, since it doesn't recognize blocks.
 
 For the alignment score, I extracted the text, then used the rapidfuzz library to find the alignment percentage.  I used the text extracted by pymupdf as the pseudo-ground truth.
 
 ## Running benchmarks
 
 You can run the benchmarks yourself.  To do so, you have to first install pdftext manually.  The install assumes you have poetry and Python 3.9+ installed.
 
@@ -110,18 +114,19 @@
 python benchmark.py # Will download the benchmark pdfs automatically
 ```
 
 The benchmark script has a few options:
 
 - `--max` this controls the maximum number of pdfs to benchmark
 - `--result_path` a folder to save the results.  A file called `results.json` will be created in the folder.
+- `--pdftext_only` skip running pdfplumber, which can be slow.
 
 # How it works
 
-PDFText is a very light wrapper around pypdfium2.  It first uses pypdfium2 to extract characters in order, along with font and other information.  Then it uses a simple decision tree algorithm to group characters into lines and blocks.  It then done some simple postprocessing to clean up the text.
+PDFText is a very light wrapper around pypdfium2.  It first uses pypdfium2 to extract characters in order, along with font and other information.  Then it uses a simple decision tree algorithm to group characters into lines and blocks.  It does some simple postprocessing to clean up the text.
 
 # Credits
 
 This is built on some amazing open source work, including:
 
 - [pypdfium2](https://github.com/pypdfium2-team/pypdfium2)
 - [scikit-learn](https://scikit-learn.org/stable/index.html)
```

### Comparing `pdftext-0.1.1/extract_text.py` & `pdftext-0.1.2/extract_text.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.1.1/pdftext/extraction.py` & `pdftext-0.1.2/pdftext/extraction.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.1.1/pdftext/pdf/chars.py` & `pdftext-0.1.2/pdftext/pdf/chars.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 def get_pdfium_chars(pdf_path, fontname_sample_freq=settings.FONTNAME_SAMPLE_FREQ):
     pdf = pdfium.PdfDocument(pdf_path)
     blocks = []
 
     for page_idx in range(len(pdf)):
         page = pdf.get_page(page_idx)
         text_page = page.get_textpage()
+        mediabox = page.get_mediabox()
+        bl_origin = mediabox[0] == 0 and mediabox[1] == 0
 
         bbox = page.get_bbox()
         page_width = math.ceil(bbox[2] - bbox[0])
         page_height = math.ceil(abs(bbox[1] - bbox[3]))
 
         text_chars = {
             "chars": [],
@@ -54,15 +56,15 @@
                 prev_fontname = fontname
                 fontname, fontflags = get_fontname(text_page, i)
                 update_previous_fonts(text_chars, i, fontname, fontflags, prev_fontname, text_page, fontname_sample_freq)
 
             rotation = pdfium_c.FPDFText_GetCharAngle(text_page, i)
             rotation = rotation * 180 / math.pi # convert from radians to degrees
             coords = text_page.get_charbox(i, loose=True)
-            device_coords = page_bbox_to_device_bbox(page, coords, page_width, page_height, normalize=True)
+            device_coords = page_bbox_to_device_bbox(page, coords, page_width, page_height, bl_origin, normalize=True)
 
             char_info = {
                 "font": {
                     "size": fontsize,
                     "weight": fontweight,
                     "name": fontname,
                     "flags": fontflags
```

### Comparing `pdftext-0.1.1/pdftext/postprocessing.py` & `pdftext-0.1.2/pdftext/postprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,15 +58,13 @@
     for block in page["blocks"]:
         block_text = ""
         for line in block["lines"]:
             line_text = ""
             for char in line["chars"]:
                 line_text += char["char"]
             line_text = postprocess_text(line_text)
-            if line_text.endswith("\n"):
-                line_text = line_text[:-1].strip() + " "
+            line_text = line_text.rstrip() + "\n"
 
             block_text += line_text
-        if not block_text.endswith("\n"):
-            block_text += "\n\n"
+        block_text = block_text.rstrip() + "\n\n"
         text += block_text
     return text
```

### Comparing `pdftext-0.1.1/pyproject.toml` & `pdftext-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdftext"
-version = "0.1.1"
+version = "0.1.2"
 description = "Extract structured text from pdfs quickly"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/VikParuchuri/pdftext"
 keywords = ["pdf", "text", "extraction"]
 packages = [
```

### Comparing `pdftext-0.1.1/PKG-INFO` & `pdftext-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftext
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extract structured text from pdfs quickly
 Home-page: https://github.com/VikParuchuri/pdftext
 License: Apache-2.0
 Keywords: pdf,text,extraction
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -21,14 +21,18 @@
 Project-URL: Repository, https://github.com/VikParuchuri/pdftext
 Description-Content-Type: text/markdown
 
 # PDFText
 
 Text extraction like [PyMuPDF](https://github.com/pymupdf/PyMuPDF), but without the AGPL license.  PDFText extracts plain text or structured blocks and lines.  It's built on [pypdfium2](https://github.com/pypdfium2-team/pypdfium2), so it's [fast, accurate](#benchmarks), and Apache licensed.
 
+## Community
+
+[Discord](https://discord.gg//KuZwXNGnfH) is where we discuss future development.
+
 # Installation
 
 You'll need python 3.9+ first.  Then run `pip install pdftext`.
 
 # Usage
 
 - Inspect the settings in `pdftext/settings.py`.  You can override any settings with environment variables.
@@ -96,33 +100,33 @@
 text = dictionary_output(PDF_PATH)
 ```
 
 If you want more customization, check out the `pdftext.extraction._get_pages` function for a starting point to dig deeper.  pdftext is a pretty thin wrapper around [pypdfium2](https://pypdfium2.readthedocs.io/en/stable/), so you might want to look at the documentation for that as well.
 
 # Benchmarks
 
-I benchmarked extraction speed and accuracy of [pymupdf](https://pymupdf.readthedocs.io/en/latest/), [pdfplumber](https://github.com/jsvine/pdfplumber), and pdftext.  I chose pymupdf because it extracts blocks and lines.  Pdfplumber extracts words and bboxes.  I did not benchmark pypdf, even though it is a great library, because it doesn't provide individual words/lines and bbox information.
+I benchmarked extraction speed and accuracy of [pymupdf](https://pymupdf.readthedocs.io/en/latest/), [pdfplumber](https://github.com/jsvine/pdfplumber), and pdftext.  I chose pymupdf because it extracts blocks and lines.  Pdfplumber extracts words and bboxes.  I did not benchmark pypdf, even though it is a great library, because it doesn't provide individual character/line/block and bbox information.
 
-Here are the scores:
+Here are the scores, run on an M1 Macbook, without multiprocessing:
 
 | Library    | Time (s per page) | Alignment Score (% accuracy vs pymupdf) |
 |------------|-------------------|-----------------------------------------|
 | pymupdf    | 0.32              | --                                      |
-| pdftext    | 1.79              | 96.22                                   |
-| pdfplumber | 3.0               | 89.88                                   |
+| pdftext    | 1.4               | 97.76                                   |
+| pdfplumber | 3.0               | 90.3                                    |
 
-pdftext is approximately 2x slower than using pypdfium2 alone (if you were to extract all the same information).
+pdftext is approximately 2x slower than using pypdfium2 alone (if you were to extract all the same character information).
 
 There are additional benchmarks for pypdfium2 and other tools [here](https://github.com/py-pdf/benchmarks).
 
 ## Methodology
 
 I used a benchmark set of 200 pdfs extracted from [common crawl](https://huggingface.co/datasets/pixparse/pdfa-eng-wds), then processed by a team at HuggingFace.
 
-For each library, I used a detailed extraction method, to pull out font information, as well as just the words.  This ensured we were comparing similar performance numbers.
+For each library, I used a detailed extraction method, to pull out font information, as well as just the words.  This ensured we were comparing similar performance numbers.  I formatted the text similarly when extracting - newlines after lines, and double newlines after blocks.  For pdfplumber, I could only do the newlines after lines, since it doesn't recognize blocks.
 
 For the alignment score, I extracted the text, then used the rapidfuzz library to find the alignment percentage.  I used the text extracted by pymupdf as the pseudo-ground truth.
 
 ## Running benchmarks
 
 You can run the benchmarks yourself.  To do so, you have to first install pdftext manually.  The install assumes you have poetry and Python 3.9+ installed.
 
@@ -133,18 +137,19 @@
 python benchmark.py # Will download the benchmark pdfs automatically
 ```
 
 The benchmark script has a few options:
 
 - `--max` this controls the maximum number of pdfs to benchmark
 - `--result_path` a folder to save the results.  A file called `results.json` will be created in the folder.
+- `--pdftext_only` skip running pdfplumber, which can be slow.
 
 # How it works
 
-PDFText is a very light wrapper around pypdfium2.  It first uses pypdfium2 to extract characters in order, along with font and other information.  Then it uses a simple decision tree algorithm to group characters into lines and blocks.  It then done some simple postprocessing to clean up the text.
+PDFText is a very light wrapper around pypdfium2.  It first uses pypdfium2 to extract characters in order, along with font and other information.  Then it uses a simple decision tree algorithm to group characters into lines and blocks.  It does some simple postprocessing to clean up the text.
 
 # Credits
 
 This is built on some amazing open source work, including:
 
 - [pypdfium2](https://github.com/pypdfium2-team/pypdfium2)
 - [scikit-learn](https://scikit-learn.org/stable/index.html)
```

