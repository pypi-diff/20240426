# Comparing `tmp/ynab_transaction_adjuster-1.0.0.tar.gz` & `tmp/ynab_transaction_adjuster-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_transaction_adjuster-1.0.0.tar", max compression
+gzip compressed data, was "ynab_transaction_adjuster-1.1.0.tar", max compression
```

## Comparing `ynab_transaction_adjuster-1.0.0.tar` & `ynab_transaction_adjuster-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35148 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/LICENSE
--rw-r--r--   0        0        0     3588 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/README.md
--rw-r--r--   0        0        0      673 2024-04-23 05:43:58.176581 ynab_transaction_adjuster-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      291 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/__init__.py
--rw-r--r--   0        0        0     5018 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/adjuster.py
--rw-r--r--   0        0        0     2686 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/client.py
--rw-r--r--   0        0        0     1003 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/exceptions.py
--rw-r--r--   0        0        0      357 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/__init__.py
--rw-r--r--   0        0        0      246 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/category.py
--rw-r--r--   0        0        0      621 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/categorygroup.py
--rw-r--r--   0        0        0      263 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/credentials.py
--rw-r--r--   0        0        0     2920 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/modifiedtransaction.py
--rw-r--r--   0        0        0     1718 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/modifier.py
--rw-r--r--   0        0        0     1252 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/modifiersubtransaction.py
--rw-r--r--   0        0        0      586 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/payee.py
--rw-r--r--   0        0        0      594 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/subtransaction.py
--rw-r--r--   0        0        0     2905 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/transaction.py
--rw-r--r--   0        0        0       72 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/repos/__init__.py
--rw-r--r--   0        0        0     1980 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/repos/categoryrepo.py
--rw-r--r--   0        0        0     1771 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/repos/payeerepo.py
--rw-r--r--   0        0        0     2848 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/serializer.py
--rw-r--r--   0        0        0     1283 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/signaturechecker.py
--rw-r--r--   0        0        0     4385 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3566 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/README.md
+-rw-r--r--   0        0        0      673 2024-04-26 07:48:01.514400 ynab_transaction_adjuster-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      291 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/__init__.py
+-rw-r--r--   0        0        0     5359 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/adjuster.py
+-rw-r--r--   0        0        0     2954 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/client.py
+-rw-r--r--   0        0        0     1003 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/exceptions.py
+-rw-r--r--   0        0        0      357 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/category.py
+-rw-r--r--   0        0        0      621 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/categorygroup.py
+-rw-r--r--   0        0        0      263 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/credentials.py
+-rw-r--r--   0        0        0     2920 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifiedtransaction.py
+-rw-r--r--   0        0        0     1718 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifier.py
+-rw-r--r--   0        0        0     1252 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifiersubtransaction.py
+-rw-r--r--   0        0        0      586 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/payee.py
+-rw-r--r--   0        0        0      594 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/subtransaction.py
+-rw-r--r--   0        0        0     3106 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/transaction.py
+-rw-r--r--   0        0        0       72 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/repos/__init__.py
+-rw-r--r--   0        0        0     1980 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/repos/categoryrepo.py
+-rw-r--r--   0        0        0     1771 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/repos/payeerepo.py
+-rw-r--r--   0        0        0     2848 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/serializer.py
+-rw-r--r--   0        0        0     1283 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/signaturechecker.py
+-rw-r--r--   0        0        0     4363 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-1.1.0/PKG-INFO
```

### Comparing `ynab_transaction_adjuster-1.0.0/LICENSE` & `ynab_transaction_adjuster-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/README.md` & `ynab_transaction_adjuster-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 		# your implementation
 
 		# return the altered modifier
 		return modifier
 ```
 
 ### Initialize
-Create a [`Credentials`][models.Credentials] object and initialize Adjuster class with it
+Create a `Credentials` object and initialize Adjuster class with it
 ```py
 from ynabtransactionadjuster import Credentials
 
 my_credentials = Credentials(token='<token>', budget='<budget>', account='<account>')
 my_adjuster = MyAdjuster.from_credentials(credentials=my_credentials)
 ```
```

### Comparing `ynab_transaction_adjuster-1.0.0/pyproject.toml` & `ynab_transaction_adjuster-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ynab-transaction-adjuster"
-version = "1.0.0"
+version = "1.1.0"
 description = "Library to adjust transactions in YNAB based on custom patterns"
 authors = ["Daniel Basta <ynab@basta.info>"]
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabtransactionadjuster'}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/adjuster.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/adjuster.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 		:param pretty_print: if set to True will print modified transactions as strings in console
 
 		:return: List of modified transactions
 		:raises SignatureError: if signature of implemented adjuster functions is not compatible
 		:raises AdjustError: if there is any error during the adjust process
 		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
 		"""
-		self.check_signatures()
+		self._check_signatures()
 		filtered_transactions = self.filter(self.transactions)
 		s = Serializer(transactions=filtered_transactions, adjust_func=self.adjust, categories=self.categories)
 		modified_transactions = s.run()
 		if pretty_print:
 			print('\n'.join(map(str, modified_transactions)))
 		return modified_transactions
 
@@ -88,20 +88,28 @@
 		implementation of the two methods and push the updated transactions back to YNAB
 
 		:return: count of adjusted transactions which have been updated in YNAB
 		:raises SignatureError: if signature of implemented adjuster functions is not compatible
 		:raises AdjustError: if there is any error during the adjust process
 		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
 		"""
-		self.check_signatures()
+		self._check_signatures()
 		filtered_transactions = self.filter(self.transactions)
 		s = Serializer(transactions=filtered_transactions, adjust_func=self.adjust, categories=self.categories)
 		modified_transactions = s.run()
 		if modified_transactions:
 			client = Client.from_credentials(credentials=self.credentials)
 			updated = client.update_transactions(modified_transactions)
 			return updated
 		return 0
 
-	def check_signatures(self):
+	def _check_signatures(self):
 		SignatureChecker(func=self.filter, parent_func=Adjuster.filter).check()
 		SignatureChecker(func=self.adjust, parent_func=Adjuster.adjust).check()
+
+	def fetch_transaction(self, transaction_id: str) -> Transaction:
+		"""Fetches an individual transaction from the YNAB account
+
+		:param transaction_id: Transaction ID of the transaction to be fetched
+		"""
+		client = Client.from_credentials(credentials=self.credentials)
+		return client.fetch_transaction(transaction_id=transaction_id)
```

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/client.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 		r.raise_for_status()
 
 		data = r.json()['data']['transactions']
 		transaction_dicts = [t for t in data if t['deleted'] is False]
 		transactions = [Transaction.from_dict(t) for t in transaction_dicts]
 		return transactions
 
+	def fetch_transaction(self, transaction_id: str) -> Transaction:
+		r = requests.get(f'{YNAB_BASE_URL}/budgets/{self._budget}/transactions/{transaction_id}', headers=self._header)
+		r.raise_for_status()
+		return Transaction.from_dict(r.json()['data']['transaction'])
+
 	def update_transactions(self, transactions: List[ModifiedTransaction]) -> int:
 		"""Updates transactions in YNAB. The updates are done in bulk.
 
 		:param transactions: list of modified transactions to be updated
 		:raises HTTPError: if bulk update call is not successful. Error can be related to any item in the passed list
 		of transactions
 		"""
```

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/exceptions.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/exceptions.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/categorygroup.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/categorygroup.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/modifiedtransaction.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifiedtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/modifier.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifier.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/modifiersubtransaction.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifiersubtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/payee.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/payee.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/subtransaction.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/subtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/transaction.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/transaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,29 @@
 	:ivar memo: The memo of the original transaction
 	:ivar payee: The payee of the original transaction
 	:ivar flag_color: The flag color of the original transaction
 	:ivar import_payee_name: The payee as recorded by YNAB on import
 	:ivar import_payee_name_original: The original payee or memo as recorded by the bank
 	:ivar approved: approval status of the original transaction
 	:ivar cleared: clearance state of the original transaction
+	:ivar transfer_transaction_id: id of the originating transaction if transaction is transfer
 	"""
 	id: str
 	transaction_date: date
 	category: Optional[Category]
 	amount: int
 	memo: Optional[str]
 	payee: Payee
 	flag_color: Optional[Literal['red', 'green', 'blue', 'orange', 'purple', 'yellow']]
 	import_payee_name_original: Optional[str]
 	import_payee_name: Optional[str]
 	subtransactions: Tuple[SubTransaction, ...]
 	cleared: Literal['uncleared', 'cleared', 'reconciled']
 	approved: bool
+	transfer_transaction_id: Optional[str]
 
 	@classmethod
 	def from_dict(cls, t_dict: dict) -> 'Transaction':
 
 		def build_category(t_dict: dict) -> Optional[Category]:
 			if not t_dict['category_name'] in ('Uncategorized', 'Split'):
 				return Category(id=t_dict['category_id'], name=t_dict['category_name'])
@@ -60,14 +62,15 @@
 						   import_payee_name_original=t_dict['import_payee_name_original'],
 						   import_payee_name=t_dict['import_payee_name'],
 						   flag_color=t_dict['flag_color'],
 						   payee=build_payee(t_dict),
 						   subtransactions=tuple([build_subtransaction(st) for st in t_dict['subtransactions']]),
 						   amount=t_dict['amount'],
 						   approved=t_dict['approved'],
-						   cleared=t_dict['cleared'])
+						   cleared=t_dict['cleared'],
+						   transfer_transaction_id=t_dict['transfer_transaction_id'])
 
 	def as_dict(self) -> dict:
 		return asdict(self)
 
 	def __str__(self) -> str:
 		return f"{self.transaction_date} | {self.payee.name} | {float(self.amount) / 1000:.2f} | {self.memo}"
```

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/repos/categoryrepo.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/repos/categoryrepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/repos/payeerepo.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/repos/payeerepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/serializer.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/serializer.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/signaturechecker.py` & `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/signaturechecker.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.0.0/PKG-INFO` & `ynab_transaction_adjuster-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynab-transaction-adjuster
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library to adjust transactions in YNAB based on custom patterns
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,15 +72,15 @@
 		# your implementation
 
 		# return the altered modifier
 		return modifier
 ```
 
 ### Initialize
-Create a [`Credentials`][models.Credentials] object and initialize Adjuster class with it
+Create a `Credentials` object and initialize Adjuster class with it
 ```py
 from ynabtransactionadjuster import Credentials
 
 my_credentials = Credentials(token='<token>', budget='<budget>', account='<account>')
 my_adjuster = MyAdjuster.from_credentials(credentials=my_credentials)
 ```
```

