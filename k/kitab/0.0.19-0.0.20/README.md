# Comparing `tmp/kitab-0.0.19.tar.gz` & `tmp/kitab-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitab-0.0.19.tar", last modified: Thu Apr 25 20:49:15 2024, max compression
+gzip compressed data, was "kitab-0.0.20.tar", last modified: Fri Apr 26 08:28:47 2024, max compression
```

## Comparing `kitab-0.0.19.tar` & `kitab-0.0.20.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 20:49:15.958520 kitab-0.0.19/
--rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.19/LICENSE
--rw-rw-rw-   0        0        0     4353 2024-04-25 20:49:15.951517 kitab-0.0.19/PKG-INFO
--rw-rw-rw-   0        0        0     4375 2024-04-25 19:49:09.000000 kitab-0.0.19/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 20:49:15.831916 kitab-0.0.19/kitab/
--rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.19/kitab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 20:49:15.860764 kitab-0.0.19/kitab/api/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.19/kitab/api/__init__.py
--rw-rw-rw-   0        0        0     7400 2024-04-25 20:23:48.000000 kitab-0.0.19/kitab/api/app.py
-drwxrwxrwx   0        0        0        0 2024-04-25 20:49:15.876956 kitab-0.0.19/kitab/db/
--rw-rw-rw-   0        0        0      415 2024-04-25 20:35:38.000000 kitab-0.0.19/kitab/db/__init__.py
--rw-rw-rw-   0        0        0      232 2024-04-25 20:34:57.000000 kitab-0.0.19/kitab/db/db_credentials.py
--rw-rw-rw-   0        0        0     1836 2024-04-25 20:34:46.000000 kitab-0.0.19/kitab/db/db_info.py
--rw-rw-rw-   0        0        0    17442 2024-04-25 20:35:46.000000 kitab-0.0.19/kitab/db/functions.py
--rw-rw-rw-   0        0        0     6541 2024-04-25 20:35:58.000000 kitab-0.0.19/kitab/db/get_data.py
--rw-rw-rw-   0        0        0    12190 2024-04-25 20:36:06.000000 kitab-0.0.19/kitab/db/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-04-25 20:49:15.881983 kitab-0.0.19/kitab/logger/
--rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.19/kitab/logger/__init__.py
--rw-rw-rw-   0        0        0     1812 2024-04-25 18:53:05.000000 kitab-0.0.19/kitab/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-25 20:49:15.889754 kitab-0.0.19/kitab/recommendation_model/
--rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.19/kitab/recommendation_model/__init__.py
--rw-rw-rw-   0        0        0     4216 2024-04-25 14:23:05.000000 kitab-0.0.19/kitab/recommendation_model/models.py
--rw-rw-rw-   0        0        0     5612 2024-04-25 20:23:27.000000 kitab-0.0.19/kitab/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 20:49:15.946518 kitab-0.0.19/kitab.egg-info/
--rw-rw-rw-   0        0        0     4353 2024-04-25 20:49:15.000000 kitab-0.0.19/kitab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2024-04-25 20:49:15.000000 kitab-0.0.19/kitab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 20:49:15.000000 kitab-0.0.19/kitab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-04-25 20:49:15.000000 kitab-0.0.19/kitab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-25 20:49:15.000000 kitab-0.0.19/kitab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 20:49:15.958520 kitab-0.0.19/setup.cfg
--rw-rw-rw-   0        0        0      991 2024-04-25 20:49:10.000000 kitab-0.0.19/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 20:49:15.941517 kitab-0.0.19/tests/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.19/tests/test_module1.py
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.19/tests/test_module2.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:28:47.140948 kitab-0.0.20/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.20/LICENSE
+-rw-rw-rw-   0        0        0     4353 2024-04-26 08:28:47.136948 kitab-0.0.20/PKG-INFO
+-rw-rw-rw-   0        0        0     4375 2024-04-25 19:49:09.000000 kitab-0.0.20/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 08:28:47.033183 kitab-0.0.20/kitab/
+-rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.20/kitab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:28:47.090696 kitab-0.0.20/kitab/api/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.20/kitab/api/__init__.py
+-rw-rw-rw-   0        0        0     7848 2024-04-26 08:09:51.000000 kitab-0.0.20/kitab/api/app.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:28:47.108817 kitab-0.0.20/kitab/db/
+-rw-rw-rw-   0        0        0      416 2024-04-26 08:05:03.000000 kitab-0.0.20/kitab/db/__init__.py
+-rw-rw-rw-   0        0        0      232 2024-04-25 20:34:57.000000 kitab-0.0.20/kitab/db/db_credentials.py
+-rw-rw-rw-   0        0        0     1836 2024-04-25 20:34:46.000000 kitab-0.0.20/kitab/db/db_info.py
+-rw-rw-rw-   0        0        0    20351 2024-04-26 08:21:42.000000 kitab-0.0.20/kitab/db/functions.py
+-rw-rw-rw-   0        0        0     6765 2024-04-26 08:23:42.000000 kitab-0.0.20/kitab/db/get_data.py
+-rw-rw-rw-   0        0        0    13657 2024-04-26 08:27:29.000000 kitab-0.0.20/kitab/db/sql_interactions.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:28:47.117368 kitab-0.0.20/kitab/logger/
+-rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.20/kitab/logger/__init__.py
+-rw-rw-rw-   0        0        0     1812 2024-04-25 18:53:05.000000 kitab-0.0.20/kitab/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:28:47.122870 kitab-0.0.20/kitab/recommendation_model/
+-rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.20/kitab/recommendation_model/__init__.py
+-rw-rw-rw-   0        0        0     4216 2024-04-25 14:23:05.000000 kitab-0.0.20/kitab/recommendation_model/models.py
+-rw-rw-rw-   0        0        0     6250 2024-04-26 08:26:41.000000 kitab-0.0.20/kitab/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:28:47.134923 kitab-0.0.20/kitab.egg-info/
+-rw-rw-rw-   0        0        0     4353 2024-04-26 08:28:46.000000 kitab-0.0.20/kitab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2024-04-26 08:28:46.000000 kitab-0.0.20/kitab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 08:28:46.000000 kitab-0.0.20/kitab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-04-26 08:28:46.000000 kitab-0.0.20/kitab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 08:28:46.000000 kitab-0.0.20/kitab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 08:28:47.141951 kitab-0.0.20/setup.cfg
+-rw-rw-rw-   0        0        0      991 2024-04-26 08:27:45.000000 kitab-0.0.20/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:28:47.130416 kitab-0.0.20/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.20/tests/test_module1.py
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.20/tests/test_module2.py
```

### Comparing `kitab-0.0.19/LICENSE` & `kitab-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `kitab-0.0.19/PKG-INFO` & `kitab-0.0.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitab
-Version: 0.0.19
+Version: 0.0.20
 Summary: A package for book recommendation.
 Author: Alexander Shahramanyan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `kitab-0.0.19/README.md` & `kitab-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `kitab-0.0.19/kitab/api/app.py` & `kitab-0.0.20/kitab/api/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,34 +38,55 @@
     authors: list[str] | None = None
     genres: list[str] | None = None
     
     class Config:
         extra = "forbid"
 
 
-@app.get("/get_book")
-def get_book(isbn: str):
+@app.get("/get_book_by_isbn")
+def get_book_isbn(isbn: str):
     """
     Get the book by ISBN.
     
     Parameters:
-    ISBNs (str): The ISBN of the book.
+    ISBN (str): The ISBN of the book.
 
     Returns:
     dict: The book information.
     """
     # Get the book by ISBN
     book = get_book_by_ISBN(isbn)
     
     # If it doesn't exist, return a message
     if book is None:
         return {"message": "Book not found."}
     
     return book
 
+
+@app.get("/get_book_by_title")
+def get_book_title(title: str):
+    """
+    Get the book by title.
+    
+    Parameters:
+    title (str): The title of the book.
+
+    Returns:
+    dict: The book information.
+    """
+    # Get the book by ISBN
+    book = get_book_by_title(title)
+    
+    # If it doesn't exist, return a message
+    if book is None:
+        return {"message": "Book not found."}
+    
+    return book
+
 
 @app.post("/add_book")
 def add_book(book: Book):
     """
     Add a book to the database.
     
     Parameters:
```

### Comparing `kitab-0.0.19/kitab/db/db_info.py` & `kitab-0.0.20/kitab/db/db_info.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.19/kitab/db/functions.py` & `kitab-0.0.20/kitab/db/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 ch.setLevel(logging.DEBUG)
 ch.setFormatter(CustomFormatter())
 logger.addHandler(ch)
 
 def get_book_by_ISBN(ISBN: str, verbose: bool = False):
     """
     Retrieves a book from the database based on its ISBN.
+    
+    Example:
+    >>> from kitab.db.functions import get_book_by_ISBN
+    >>> get_book_by_ISBN("1442942355")
 
     Parameters:
     ISBN (str): The ISBN of the book to retrieve.
     verbose (bool): Whether to print verbose output. Defaults to False.
 
     Returns:
     dict or None: A dictionary containing the book information if found, or None if no book is found.
@@ -80,14 +84,18 @@
     # Return the book
     return book
 
 
 def get_book_by_title(title: str, verbose: bool = False):
     """
     Retrieves a book from the database based on its title.
+    
+    Example:
+    >>> from kitab.db.functions import get_book_by_title
+    >>> get_book_by_title("The Ghostly Rental")
 
     Parameters:
     title (str): The title of the book to retrieve.
     verbose (bool): Whether to print verbose output. Defaults to False.
 
     Returns:
     dict or None: A dictionary containing the book information if found, or None if no book is found.
@@ -112,14 +120,31 @@
     # Return the book
     return get_book_by_ISBN(ISBN)
 
 
 def add_book_db(book: dict, verbose: bool = False) -> bool:
     """
     Adds a book to the database.
+    
+    Example:
+    >>> from kitab.db.functions import add_book_db
+    >>> add_book_db({
+            "isbn": "1442942355",
+            "title": "The Ghostly Rental",
+            "description": "Employing the subtle methods of presenting mysterious ghost stories in the backdrop of psychological troubles, the novel presents the life of James. The troubles that he faces, combined with the baffling events around him give an aura to the novel that is almost unsurpassable.",
+            "available": False,
+            "authors": [
+                "Henry James"
+            ],
+            "genres": [
+                "Horror",
+                "Short Stories",
+                "The United States Of America"
+            ]
+        })
 
     Parameters:
     book (dict): A dictionary containing the book information.
     
     Returns:
     bool: True if the book was successfully added, False otherwise.
     """
@@ -172,14 +197,25 @@
     except:
         return False    
     
 def update_book_db(ISBN: str, new_book: dict, verbose: bool = True) -> bool:
     """
     Updates a book in the database.
     
+    Example:
+    >>> from kitab.db.functions import update_book_db
+    >>> update_book_db({
+            "available": True,
+            "genres": [
+                "Horror",
+                "Short Stories",
+                "Mystery"
+            ]
+        })
+    
     Parameters:
     ISBN (str): The ISBN of the book to update.
     new_book (dict): A dictionary containing the updated book information.
     verbose (bool): Whether to print verbose output. Defaults to False.
     
     Returns:
     bool: True if the book was successfully updated, False otherwise.
@@ -258,14 +294,18 @@
         return True
     except:
         return False
 
 def get_table_from_db(table_name: str, conditions: dict = None, verbose: bool = False) -> pd.DataFrame:
     """
     Retrieves a table from the database.
+    
+    Example:
+    >>> from kitab.db.functions import get_table_from_db
+    >>> get_table_from_db("book", conditions={"available": True})
 
     Parameters:
     table_name (str): The name of the table to retrieve.
     conditions (dict): A dictionary of conditions to filter the table.
     verbose (bool): Whether to print verbose output. Defaults to False.
 
     Returns:
@@ -287,14 +327,18 @@
     
     # Return the table
     return table
 
 def _get_or_add_genres(db: SqlHandler, genres: list[str], verbose: bool = False) -> list[int]:
     """
     Get the genre IDs for the given list of genres. If the genres do not exist in the database, add them to the genre table.
+    
+    Example:
+    >>> from kitab.db.functions import _get_or_add_genres
+    >>> _get_or_add_genres(db, genres=["Horror", "Short Stories"])
 
     Parameters:
     db (SqlHandler): The database handler.
     genres (list[str]): A list of genres.
     verbose (bool): Whether to print verbose output. Defaults to False.
 
     Returns:
@@ -321,15 +365,22 @@
         logger.info("New genres added.")
     
     return genre_ids
 
 def _get_or_add_authors(db: SqlHandler, authors: list[str], verbose: bool = False) -> list[int]:
     """
     Get the author IDs for the given list of authors. If the authors do not exist in the database, add them to the author table.
-
+    
+    Example:
+    >>> from kitab.db.functions import _get_or_add_authors
+    >>> from kitab.db.db_credentials import DB_USER, DB_PASSWORD, DB_HOST, DB_PORT, DB_NAME
+    >>> from kitab.db.sql_interactions import SqlHandler
+    >>> db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
+    >>> _get_or_add_authors(db, authors=["Henry James"])
+    
     Parameters:
     db (SqlHandler): The database handler.
     authors (list[str]): A list of authors.
     verbose (bool): Whether to print verbose output. Defaults to False.
 
     Returns:
     list[int]: A list of author IDs.
@@ -356,14 +407,18 @@
     
     return author_ids
 
 def get_authors(ISBNs: list[str], verbose: bool = False) -> dict[str:list]:
     """
     Get the authors for the given list of ISBNs.
     
+    Example:
+    >>> from kitab.db.functions import get_authors
+    >>> get_authors(ISBNs=["1442942355", "1613720211"])
+    
     Parameters:
     ISBNs (list[str]): A list of ISBNs.
     verbose (bool): Whether to print verbose output. Defaults to False.
 
     Returns:
     dict[str:list]: A dictionary containing the authors for each ISBN.
     """
@@ -391,14 +446,18 @@
     # Return the dictionary of lists
     return isbn_authors
 
 def get_genres(ISBNs: list[str], verbose: bool = False) -> dict[list]:
     """
     Get the genres for the given list of ISBNs.
     
+    Example:
+    >>> from kitab.db.functions import get_genres
+    >>> get_genres(ISBNs=["1442942355", "1613720211"])
+    
     Parameters:
     ISBNs (list[str]): A list of ISBNs.
     verbose (bool): Whether to print verbose output. Defaults to False.
 
     Returns:
     dict[str:list]: A dictionary containing the genres for each ISBN.
     """
@@ -427,14 +486,18 @@
     return isbn_genres
 
 
 def get_history_by_recommendation_isbn(recommendation_isbn: str, verbose: bool = False) -> dict:
     """
     Get the history of recommendations for a book with the given ISBN.
     
+    Example:
+    >>> from kitab.db.functions import get_history_by_recommendation_isbn
+    >>> get_history_by_recommendation_isbn(recommendation_isbn="1442942355")
+    
     Parameters:
     recommendation_ISBN (str): The ISBN of the recommended book.
 
     Returns:
     dict: A dictionary containing the history of recommendations for the book.
     """
     # Open connection to the database
@@ -449,14 +512,18 @@
     return history.drop(columns="log_id").to_dict(orient='records')
 
 
 def add_recommendation_log(description: str, recommendation_ISBN: str, successful: bool, verbose: bool = False) -> bool:
     """
     Adds a recommendation log to the history table.
     
+    Example:
+    >>> from kitab.db.functions import add_recommendation_log
+    >>> add_recommendation_log(description="In a masterful blend of psychological intrigue and spectral disturbances, this novel unfurls the complex life of Clara. Her internal struggles are mirrored by eerie, inexplicable occurrences, weaving a tale that is both deeply personal and chillingly atmospheric, offering an unparalleled exploration of the human psyche shadowed by the paranormal.", recommendation_isbn="1442942355", successful=True)
+    
     Parameters:
     description (str): The description of the recommendation.
     recommendation_ISBN (str): The ISBN of the recommended book.
     successful (bool): Whether the recommendation was successful or not.
     verbose (bool): Whether to print verbose output. Defaults to False.
 
     Returns:
```

### Comparing `kitab-0.0.19/kitab/db/get_data.py` & `kitab-0.0.20/kitab/db/get_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 
 
 
 def get_full_data(folder_path: str = "data", verbose: bool = False):
     """
     Retrieves and combines data from multiple CSV files and corresponding pickle files.
     
+    Example:
+    >>> from kitab.db.get_data import get_full_data
+    >>> get_full_data(folder_path="data")
+    
     Parameters:
     folder_path (str): The path to the directory containing the CSV and pickle files.
     verbose (bool): Whether to display logs. Default is False.
     
     Returns:
     pandas.DataFrame: A DataFrame containing the combined data with an additional 'embedding' column.
     """
@@ -58,14 +62,18 @@
  
     return df
 
 
 def load_data(folder_path: str = "data", verbose: bool = False):
     """
     Load data from a specified folder path and insert it into the database.
+    
+    Example:
+    >>> from kitab.db.get_data import load_data
+    >>> load_data(folder_path="data")
 
     Parameters:
     folder_path (str): The path to the folder containing the data files. Default is "data".
     verbose (bool): Whether to display logs. Default is False.
 
     Returns:
     None
```

### Comparing `kitab-0.0.19/kitab/db/sql_interactions.py` & `kitab-0.0.20/kitab/db/sql_interactions.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,14 +48,18 @@
             logger.info('The connection has been closed.')
 
 
     def get_table_columns(self, table_name: str, verbose: bool = False) -> list:
         """
         Retrieves the columns of a table in the database.
         
+        Example:
+        >>> from kitab.db.sql_interactions import get_table_columns
+        >>> db.get_table_columns("Book")
+
         Parameters:
         table_name (str): The name of the table whose columns are to be retrieved.
         verbose (bool): Whether to print verbose output. Defaults to False.
         
         Returns:
         list: A list of column names in the table.
         """
@@ -72,14 +76,18 @@
             return []
     
     
     def execute_commands(self, commands: list, verbose: bool = False) -> None:
         """
         Executes a list of commands in the database.
         
+        Example:
+        >>> from kitab.db.sql_interactions import execute_commands
+        >>> db.execute_commands(commands)
+
         Parameters:
         commands (list): A list of SQL commands to be executed.
         verbose (bool): Whether to print verbose output. Defaults to False.
         
         Returns:
         None
         """
@@ -92,14 +100,19 @@
             logger.info('Commands executed successfully.')
 
 
     def insert_many(self, df: pd.DataFrame, table_name: str, verbose: bool = False) -> None:
         """
         Inserts data from a DataFrame into a table in the database.
 
+        Example:
+        >>> from kitab.db.sql_interactions import insert_many
+        >>> df = pd.DataFrame(...)
+        >>> db.insert_many(df, "Book")
+
         Parameters:
         df (pd.DataFrame): The DataFrame containing the data to be inserted.
         table_name (str): The name of the table to be dropped.
         verbose (bool): Whether to print verbose output. Defaults to False.
 
         Returns:
         None
@@ -152,14 +165,18 @@
             logger.error(f'Error occurred while inserting data into {table_name}: {e}')
 
 
     def truncate_table(self, table_name: str, verbose: bool = False) -> None:
         """
         Truncates a table from the database.
 
+        Example:
+        >>> from kitab.db.sql_interactions import truncate_table
+        >>> db.trucate_table("Book")
+
         Parameters:
         table_name (str): The name of the table to be truncated.
         verbose (bool): Whether to print verbose output. Defaults to False.
 
         Returns:
         None
         """
@@ -172,14 +189,18 @@
         # self.cursor.close()
 
 
     def drop_table(self, table_name: str, verbose: bool = False) -> None:
         """
         Drops a table from the database if it exists.
 
+        Example:
+        >>> from kitab.db.sql_interactions import drop_table
+        >>> db.drop_table("Book")
+
         Parameters:
         table_name (str): The name of the table to be dropped.
         verbose (bool): Whether to print verbose output. Defaults to False.
 
         Returns:
         None
         """
@@ -195,14 +216,19 @@
             logger.info(f"Table '{table_name}' deleted.")
 
         
     def insert_records(self, table_name: str, values_list: list[dict], verbose: bool = False) -> None:
         """
         Insert one or more records into the database table.
 
+        Example:
+        >>> from kitab.db.sql_interactions import insert_records
+        >>> list_of_books = [...]
+        >>> db.insert_records("Book", list_of_books)
+
         Parameters:
         values_list (List[Dict]): A list of dictionaries containing column names as keys and their values as values.
         verbose (bool): Whether to print verbose output. Defaults to False.
 
         Returns:
         None
         """
@@ -218,50 +244,61 @@
         self.cursor.executemany(query, values)
         self.connection.commit()
 
         if verbose:
             logger.info(f"{len(values_list)} records inserted successfully.")
 
 
-    def update_records(self, table_name: str, update_values: dict, condition: dict, verbose: bool = False) -> None:
+    def update_records(self, table_name: str, updated_values: dict, condition: dict, verbose: bool = False) -> None:
         """
         Update records in the database table based on a given condition.
 
+        Example:
+        >>> from kitab.db.sql_interactions import update_records
+        >>> updated_values = {...}
+        >>> conditions = {...}
+        >>> db.update_records("Book", updated_values, conditions)        
+
         Parameters:
         table_name (str): The name of the table to update records in.
         condition (dict): A dictionary representing the condition for selecting records to update.
-        update_values (dict): A dictionary containing column names as keys and their updated values as values.
+        updated_values (dict): A dictionary containing column names as keys and their updated values as values.
         verbose (bool): Whether to print verbose output. Defaults to False.
 
         Returns:
         None
         """
         if not condition:
             logger.warning("No condition provided for updating records.")
             return
 
-        if not update_values:
+        if not updated_values:
             logger.warning("No values provided for update.")
             return
 
-        set_clause = ', '.join([f"{column} = %s" for column in update_values.keys()])
+        set_clause = ', '.join([f"{column} = %s" for column in updated_values.keys()])
         condition_clause = ' AND '.join([f"{column} = %s" for column in condition.keys()])
 
         query = f"UPDATE {table_name} SET {set_clause} WHERE {condition_clause};"
-        values = list(update_values.values()) + list(condition.values())
+        values = list(updated_values.values()) + list(condition.values())
 
         self.cursor.execute(query, tuple(values))
         self.connection.commit()
 
         if verbose:
             logger.info("Records updated successfully.")
         
     def remove_records(self, table_name: str, conditions_list: list[dict], verbose: bool = False) -> None:
         """
         Remove records from the database table based on multiple conditions.
+        
+        Example:
+        >>> from kitab.db.sql_interactions import remove_records
+        >>> list_of_conditions = [...]
+        >>> db.remove_records("Book", list_of_conditions)          
 
         Parameters:
         table_name (str): The name of the table to remove records from.
         conditions_list (list[dict]): A list of dictionaries representing conditions for selecting records to remove.
             The conditions inside each dictionary are concatenated using AND, and the dictionaries inside the list are concatenated using OR.
         verbose (bool): Whether to print verbose output. Defaults to False.
 
@@ -289,14 +326,19 @@
         if verbose:
             logger.info("Records removed successfully.")
 
     def get_table(self, table_name: str, conditions: dict = None, verbose: bool = False) -> pd.DataFrame:
         """
         Retrieve data from the database table.
 
+        Example:
+        >>> from kitab.db.sql_interactions import get_table
+        >>> list_of_conditions = [...]
+        >>> db.get_table("Book", list_of_conditions)          
+        
         Parameters:
         table_name (str): The name of the table to retrieve data from.
         conditions (dict, optional): A dictionary representing the conditions to filter records. Defaults to None.
         verbose (bool): Whether to print verbose output. Defaults to False.
 
         Returns:
         pd.DataFrame: A DataFrame containing the retrieved data.
```

### Comparing `kitab-0.0.19/kitab/logger/logger.py` & `kitab-0.0.20/kitab/logger/logger.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.19/kitab/recommendation_model/models.py` & `kitab-0.0.20/kitab/recommendation_model/models.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.19/kitab/utils.py` & `kitab-0.0.20/kitab/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,59 +21,81 @@
 
 model = SentenceTransformer('sentence-transformers/all-MiniLM-L6-v2')
 
 def cos_vec_vec(vector1: np.ndarray, vector2: np.ndarray) -> float:
     """
     Compute the cosine similarity between two vectors.
     
+    Example:
+    >>> from kitab.utils import cos_mat_vec
+    >>> import numpy as np
+    >>> vector1 = np.array([1, 2, 3])
+    >>> vector2 = np.array([1, 2, 3])
+    >>> cos_mat_vec(vector1, vector2)
+    
     Parameters:
     vector1 (np.ndarray): The first vector.
     vector2 (np.ndarray): The second vector.
     
     Returns:
     float: The cosine similarity between the two vectors.
     """
     dot_product = np.dot(vector1, vector2)
     norm_vector1 = np.linalg.norm(vector1)
     norm_vector2 = np.linalg.norm(vector2)
     return dot_product / (norm_vector1 * norm_vector2)
 
-def cos_mat_vec(vector1: np.ndarray, vector2: np.ndarray) -> np.ndarray:
+def cos_mat_vec(matr: np.ndarray, vect: np.ndarray) -> np.ndarray:
     """
     Compute the cosine similarity between a matrix (consisting of vectors) and a vector.
     
+    Example:
+    >>> from kitab.utils import cos_mat_vec
+    >>> import numpy as np
+    >>> matrix = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
+    >>> vector = np.array([1, 2, 3])
+    >>> cos_mat_vec(matrix, vector)
+    
     Parameters:
-    vector1 (np.ndarray): The matrix (containing individual vectors).
-    vector2 (np.ndarray): The vector.
+    matr (np.ndarray): The matrix (containing individual vectors).
+    vect (np.ndarray): The vector.
     
     Returns:
     np.ndarray: The cosine similarity between the matrix and the vector.
     """
-    dot_product = np.dot(vector1, vector2)
-    norm_vector1 = np.linalg.norm(vector1, axis=1)
-    norm_vector2 = np.linalg.norm(vector2)
+    dot_product = np.dot(matr, vect)
+    norm_vector1 = np.linalg.norm(matr, axis=1)
+    norm_vector2 = np.linalg.norm(vect)
     return dot_product / (norm_vector1 * norm_vector2)
 
 def get_embedding(text: str) -> np.ndarray:
     """
     Returns the embedding of the text.
     
+    Example:
+    >>> from kitab.utils import get_embedding
+    >>> get_embedding(text="Hello, world!")
+    
     Parameters:
     text (str): The text to be embedded.
     
     Returns:
     np.ndarray: The embedding of the text.
     """
     return model.encode(text)    
             
 
 # To add in the future: function gets embedding_func: function = None, or gets the embeddings from the user
 def process_data(data_file: str, destination_folder: str = "data", column_names: dict[str:str] = None, random_availability: bool = False, chunk_size: int = 20000, verbose: bool = False) -> None:
     """
     Process the given data file, perform data cleaning, and save the processed data and embeddings.
+    
+    Example:
+    >>> from kitab.utils import process_data
+    >>> process_data(data_file="data.csv")
 
     Parameters:
     data_file (str): The path to the data file.
     destination_folder (str): The path to the destination folder where the processed data and embeddings will be saved.
     column_names (dict[str:str], optional): A dictionary mapping required column names to the corresponding column names in the data file. Defaults to None.
     random_availability (bool, optional): If True, add random book availability to the data. If False, the data must contain an 'availability' column. Defaults to False.
     chunk_size (int, optional): The size of the chunks to split the data into. Defaults to 20000.
```

### Comparing `kitab-0.0.19/kitab.egg-info/PKG-INFO` & `kitab-0.0.20/kitab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitab
-Version: 0.0.19
+Version: 0.0.20
 Summary: A package for book recommendation.
 Author: Alexander Shahramanyan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `kitab-0.0.19/kitab.egg-info/SOURCES.txt` & `kitab-0.0.20/kitab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kitab-0.0.19/setup.py` & `kitab-0.0.20/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Add install requirements
 setup(
     author="Alexander Shahramanyan",
     description="A package for book recommendation.",
     name="kitab",
     packages=find_packages(include=["kitab", "kitab.*"]),
-    version="0.0.19",
+    version="0.0.20",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector', 'python-dotenv', 'tqdm'],
     python_requires=">=3.9",
```

