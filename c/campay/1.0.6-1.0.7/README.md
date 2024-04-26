# Comparing `tmp/campay-1.0.6.tar.gz` & `tmp/campay-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "campay-1.0.6.tar", last modified: Sun Sep  4 19:12:40 2022, max compression
+gzip compressed data, was "campay-1.0.7.tar", last modified: Fri Apr 26 13:50:47 2024, max compression
```

## Comparing `campay-1.0.6.tar` & `campay-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 endur     (1000) endur     (1000)        0 2022-09-04 19:12:40.669658 campay-1.0.6/
--rw-rw-r--   0 endur     (1000) endur     (1000)    35149 2021-04-22 02:37:58.000000 campay-1.0.6/LICENSE
--rw-rw-r--   0 endur     (1000) endur     (1000)     5466 2022-09-04 19:12:40.669658 campay-1.0.6/PKG-INFO
--rw-rw-r--   0 endur     (1000) endur     (1000)     4983 2022-09-04 19:11:42.000000 campay-1.0.6/README.md
--rw-rw-r--   0 endur     (1000) endur     (1000)      119 2021-04-23 02:58:18.000000 campay-1.0.6/pyproject.toml
--rw-rw-r--   0 endur     (1000) endur     (1000)      607 2022-09-04 19:12:40.669658 campay-1.0.6/setup.cfg
-drwxrwxr-x   0 endur     (1000) endur     (1000)        0 2022-09-04 19:12:40.669658 campay-1.0.6/src/
-drwxrwxr-x   0 endur     (1000) endur     (1000)        0 2022-09-04 19:12:40.669658 campay-1.0.6/src/campay/
--rw-rw-r--   0 endur     (1000) endur     (1000)        0 2021-04-22 02:39:13.000000 campay-1.0.6/src/campay/__init__.py
--rw-rw-r--   0 endur     (1000) endur     (1000)    12408 2022-09-02 07:47:56.000000 campay-1.0.6/src/campay/sdk.py
-drwxrwxr-x   0 endur     (1000) endur     (1000)        0 2022-09-04 19:12:40.669658 campay-1.0.6/src/campay.egg-info/
--rw-rw-r--   0 endur     (1000) endur     (1000)     5466 2022-09-04 19:12:40.000000 campay-1.0.6/src/campay.egg-info/PKG-INFO
--rw-rw-r--   0 endur     (1000) endur     (1000)      219 2022-09-04 19:12:40.000000 campay-1.0.6/src/campay.egg-info/SOURCES.txt
--rw-rw-r--   0 endur     (1000) endur     (1000)        1 2022-09-04 19:12:40.000000 campay-1.0.6/src/campay.egg-info/dependency_links.txt
--rw-rw-r--   0 endur     (1000) endur     (1000)        7 2022-09-04 19:12:40.000000 campay-1.0.6/src/campay.egg-info/top_level.txt
+drwxrwxr-x   0 endur     (1000) endur     (1000)        0 2024-04-26 13:50:47.551823 campay-1.0.7/
+-rw-rw-r--   0 endur     (1000) endur     (1000)    35149 2021-04-22 02:37:58.000000 campay-1.0.7/LICENSE
+-rw-r--r--   0 endur     (1000) endur     (1000)     7061 2024-04-26 13:50:47.551823 campay-1.0.7/PKG-INFO
+-rw-rw-r--   0 endur     (1000) endur     (1000)     6578 2024-04-26 13:39:06.000000 campay-1.0.7/README.md
+-rw-rw-r--   0 endur     (1000) endur     (1000)      119 2021-04-23 02:58:18.000000 campay-1.0.7/pyproject.toml
+-rw-rw-r--   0 endur     (1000) endur     (1000)      607 2024-04-26 13:50:47.551823 campay-1.0.7/setup.cfg
+drwxrwxr-x   0 endur     (1000) endur     (1000)        0 2024-04-26 13:50:47.551823 campay-1.0.7/src/
+drwxrwxr-x   0 endur     (1000) endur     (1000)        0 2024-04-26 13:50:47.551823 campay-1.0.7/src/campay/
+-rw-rw-r--   0 endur     (1000) endur     (1000)        0 2021-04-22 02:39:13.000000 campay-1.0.7/src/campay/__init__.py
+-rw-rw-r--   0 endur     (1000) endur     (1000)    15256 2024-04-26 13:16:38.000000 campay-1.0.7/src/campay/sdk.py
+drwxrwxr-x   0 endur     (1000) endur     (1000)        0 2024-04-26 13:50:47.551823 campay-1.0.7/src/campay.egg-info/
+-rw-r--r--   0 endur     (1000) endur     (1000)     7061 2024-04-26 13:50:47.000000 campay-1.0.7/src/campay.egg-info/PKG-INFO
+-rw-rw-r--   0 endur     (1000) endur     (1000)      219 2024-04-26 13:50:47.000000 campay-1.0.7/src/campay.egg-info/SOURCES.txt
+-rw-rw-r--   0 endur     (1000) endur     (1000)        1 2024-04-26 13:50:47.000000 campay-1.0.7/src/campay.egg-info/dependency_links.txt
+-rw-rw-r--   0 endur     (1000) endur     (1000)        7 2024-04-26 13:50:47.000000 campay-1.0.7/src/campay.egg-info/top_level.txt
```

### Comparing `campay-1.0.6/LICENSE` & `campay-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `campay-1.0.6/PKG-INFO` & `campay-1.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: campay
-Version: 1.0.6
+Version: 1.0.7
 Summary: Payment Gateway
 Home-page: https://github.com/CamPay/campay-python-sdk
 Author: CamPay
 Author-email: info@campay.net
 Project-URL: Bug Tracker, https://github.com/CamPay/campay-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -65,14 +65,16 @@
             "app_password" : "PASTE YOUR APP_PASSWORD HERE",
             "environment" : "DEV" #use "DEV" for demo mode or "PROD" for live mode
         })
     ```
 
 ### To collect payments from your client - DIRECTLY
 
+   **OPTION 1**: This option initiates a transaction and waits( or block the running code) for the transaction to complete before returning a response. 
+
    ```python
          collect = campay.collect({
             "amount": "5", #The amount you want to collect
             "currency": "XAF",
             "from": "2376xxxxxxxx", #Phone number to request amount from. Must include country code
             "description": "some description",
             "external_reference": "", #Reference from the system initiating the transaction.
@@ -80,14 +82,46 @@
 
          print(collect)
          #{"reference": "bcedde9b-62a7-4421-96ac-2e6179552a1a", "external_reference":"12345678", "status": "SUCCESSFUL", "amount": 5, "currency": "XAF", "operator": "MTN", "code": "CP201027T00005", "operator_reference":  "1880106956" }
          
    ```
    > status can be SUCCESSFUL or FAILED
 
+   **OPTION 2**: This option initiates a transaction and immediately returns the initiated transaction reference for you to use to check the status of the transaction.
+
+   ```python
+         collect = campay.initCollect({
+            "amount": "5", #The amount you want to collect
+            "currency": "XAF",
+            "from": "2376xxxxxxxx", #Phone number to request amount from. Must include country code
+            "description": "some description",
+            "external_reference": "", #Reference from the system initiating the transaction.
+         })
+
+         print(collect)
+         #{"reference": "bcedde9b-62a7-4421-96ac-2e6179552a1a", "ussd_code": "*126# for MTN or #150*50# for ORANGE", "operator": "mtn or orange" }
+         
+   ```
+   > The default status for initiated transactions is PENDING
+
+### To check a transaction status.
+
+   You need the initiated transaction **reference** to use this function.
+
+   ```python
+         campay_status = campay.get_transaction_status({
+            "reference": "bcedde9b-62a7-1234-96ac-2e6179552a1a", #The amount you want to collect
+         })
+
+         print(campay_status)
+         #{"reference": "bcedde9b-62a7-4421-96ac-2e6179552a1a", "external_reference":"12345678", "status": "SUCCESSFUL", "amount": 5, "currency": "XAF", "operator": "MTN", "code": "CP201027T00005", "operator_reference":  "1880106956" }
+         
+   ```
+   > status can be PENDING, SUCCESSFUL or FAILED
+
 ### To collect payments from your client - using PAYMENT LINKS
 
    ```python
          payment_link = campay.get_payment_link({
             "amount": "5",
             "currency": "XAF",
             "description": "some description",
@@ -100,14 +134,15 @@
          '''
          Redirect your customer to the returned payment link 
          '''
          
    ```
    > status can be SUCCESSFUL or FAILED
 
+
 ### To disburse
    > Please enable API withdrawal under app settings before trying this request
    
    ```python
         disburse = campay.disburse({
             "amount": "5", #The amount you want to disburse
             "currency": "XAF",
```

### Comparing `campay-1.0.6/README.md` & `campay-1.0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -50,14 +50,16 @@
             "app_password" : "PASTE YOUR APP_PASSWORD HERE",
             "environment" : "DEV" #use "DEV" for demo mode or "PROD" for live mode
         })
     ```
 
 ### To collect payments from your client - DIRECTLY
 
+   **OPTION 1**: This option initiates a transaction and waits( or block the running code) for the transaction to complete before returning a response. 
+
    ```python
          collect = campay.collect({
             "amount": "5", #The amount you want to collect
             "currency": "XAF",
             "from": "2376xxxxxxxx", #Phone number to request amount from. Must include country code
             "description": "some description",
             "external_reference": "", #Reference from the system initiating the transaction.
@@ -65,14 +67,46 @@
 
          print(collect)
          #{"reference": "bcedde9b-62a7-4421-96ac-2e6179552a1a", "external_reference":"12345678", "status": "SUCCESSFUL", "amount": 5, "currency": "XAF", "operator": "MTN", "code": "CP201027T00005", "operator_reference":  "1880106956" }
          
    ```
    > status can be SUCCESSFUL or FAILED
 
+   **OPTION 2**: This option initiates a transaction and immediately returns the initiated transaction reference for you to use to check the status of the transaction.
+
+   ```python
+         collect = campay.initCollect({
+            "amount": "5", #The amount you want to collect
+            "currency": "XAF",
+            "from": "2376xxxxxxxx", #Phone number to request amount from. Must include country code
+            "description": "some description",
+            "external_reference": "", #Reference from the system initiating the transaction.
+         })
+
+         print(collect)
+         #{"reference": "bcedde9b-62a7-4421-96ac-2e6179552a1a", "ussd_code": "*126# for MTN or #150*50# for ORANGE", "operator": "mtn or orange" }
+         
+   ```
+   > The default status for initiated transactions is PENDING
+
+### To check a transaction status.
+
+   You need the initiated transaction **reference** to use this function.
+
+   ```python
+         campay_status = campay.get_transaction_status({
+            "reference": "bcedde9b-62a7-1234-96ac-2e6179552a1a", #The amount you want to collect
+         })
+
+         print(campay_status)
+         #{"reference": "bcedde9b-62a7-4421-96ac-2e6179552a1a", "external_reference":"12345678", "status": "SUCCESSFUL", "amount": 5, "currency": "XAF", "operator": "MTN", "code": "CP201027T00005", "operator_reference":  "1880106956" }
+         
+   ```
+   > status can be PENDING, SUCCESSFUL or FAILED
+
 ### To collect payments from your client - using PAYMENT LINKS
 
    ```python
          payment_link = campay.get_payment_link({
             "amount": "5",
             "currency": "XAF",
             "description": "some description",
@@ -85,14 +119,15 @@
          '''
          Redirect your customer to the returned payment link 
          '''
          
    ```
    > status can be SUCCESSFUL or FAILED
 
+
 ### To disburse
    > Please enable API withdrawal under app settings before trying this request
    
    ```python
         disburse = campay.disburse({
             "amount": "5", #The amount you want to disburse
             "currency": "XAF",
```

### Comparing `campay-1.0.6/setup.cfg` & `campay-1.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = campay
-version = 1.0.6
+version = 1.0.7
 author = CamPay
 author_email = info@campay.net
 description = Payment Gateway
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CamPay/campay-python-sdk
 project_urls =
```

### Comparing `campay-1.0.6/src/campay/sdk.py` & `campay-1.0.7/src/campay/sdk.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 			
 			return {"token":token, "is_successful":is_successful}
 
 		else:
 			return {"token":None, "is_successful":False}
 
 	
+
 	def collect(self, values):
 		if self.debug:
 			print(">>>>>>>>>>>>>>>>>>: ", "Collecting...")
 
 		token = self.get_token()["token"]
 		
 		if token:
@@ -148,14 +149,77 @@
 		else:
 			message = "Token error. Please check your App Username and Pass password. Also check your environment"
 			if self.debug:
 				print(">>>>>>>>>>>>>>>>>>: ", message)
 			return {"status":"FAILED", "message":message}
 
 
+
+	def initCollect(self, values):
+		if self.debug:
+			print(">>>>>>>>>>>>>>>>>>: ", "Collecting...")
+
+		token = self.get_token()["token"]
+		
+		if token:
+
+			#### Request collect
+			collect_data = {
+				"amount":str(values["amount"]),
+				"currency": str(values["currency"]),
+				"from":str(values["from"]),
+				"description":str(values["description"]),
+				"external_reference":str(values["external_reference"])
+			}
+			collect_payload = json.dumps(collect_data)
+			collect_headers = {
+				'Authorization': 'Token '+token,
+				'Content-Type': 'application/json'
+			}
+			
+			got_json_response = False
+			try:
+				collect_response = requests.post(self.host+'/api/collect/', data=collect_payload, headers=collect_headers, verify=False)
+				collect_response_json = collect_response.json()
+				got_json_response = True
+			except:
+				pass
+			
+			if got_json_response:
+				if self.debug:
+					print(">>>>>>>>>>>>>>>>>>: ", collect_response_json)
+					
+				collect_response_status_code = int(collect_response.status_code)
+				if collect_response_status_code == 200:
+					print(">>>>>>>>>>>>>>>>>>: Confirm on phone...")
+					return collect_response_json
+				else:
+
+					message = collect_response_json["message"]
+					if self.debug:
+						print(">>>>>>>>>>>>>>>>>>: ", message)
+
+					return {"status":"FAILED", "message": message}
+
+			else:
+				message = "Collect error"
+				if self.debug:
+					print(">>>>>>>>>>>>>>>>>>: ", message)
+				return {"status":"FAILED", "message":message}
+
+		else:
+			message = "Token error. Please check your App Username and Pass password. Also check your environment"
+			if self.debug:
+				print(">>>>>>>>>>>>>>>>>>: ", message)
+			return {"status":"FAILED", "message":message}
+
+
+
+
+
 	def disburse(self, values):
 		if self.debug:
 			print(">>>>>>>>>>>>>>>>>>: ", "Disbursing...")
 		token = self.get_token()["token"]
 		if token:
 
 			#### Request withdraw
@@ -238,14 +302,15 @@
 		else:
 			message = "Token error. Please check your App Username and Pass password. Also check your environment"
 			if self.debug:
 				print(">>>>>>>>>>>>>>>>>>: ", message)
 			return {"status":"FAILED", "message":message}
 
 
+
 	def get_balance(self):
 		if self.debug:
 			print(">>>>>>>>>>>>>>>>>>: ", "Getting balance...")
 		token = self.get_token()["token"]
 		if token:
 			status_headers = {
 				'Authorization': 'Token '+token,
@@ -430,7 +495,48 @@
 
 		else:
 			message = "Token error. Please check your App Username and Pass password. Also check your environment"
 			if self.debug:
 				print(">>>>>>>>>>>>>>>>>>: ", message)
 			return {"status":"FAILED", "message":message}
 
+
+
+	def get_transaction_status(self, values):
+		if self.debug:
+			print(">>>>>>>>>>>>>>>>>>: ", "Getting Transaction status...")
+		token = self.get_token()["token"]
+		if token:
+			try:
+				reference = values["reference"]
+			except:
+				return {"status":"", "message":"Transaction Reference is required"}
+			
+			status_headers = {
+				'Authorization': 'Token '+token,
+				'Content-Type': 'application/json',
+			}
+							
+			got_json_response = False
+			try:
+				response = requests.get(self.host+f"/api/transaction/{reference}/", headers=status_headers, verify=False)
+				response_json = response.json()
+				got_json_response = True
+			except:
+				pass
+
+			if got_json_response:
+				if self.debug:
+					print(">>>>>>>>>>>>>>>>>>: ", response_json)
+				return response_json
+				
+			else:
+				message = "Request error"
+				if self.debug:
+					print(">>>>>>>>>>>>>>>>>>: ", message)
+				return {"status":"", "message":message}
+
+		else:
+			message = "Token error. Please check your App Username and Pass password. Also check your environment"
+			if self.debug:
+				print(">>>>>>>>>>>>>>>>>>: ", message)
+			return {"status":"", "message":message}
```

### Comparing `campay-1.0.6/src/campay.egg-info/PKG-INFO` & `campay-1.0.7/src/campay.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: campay
-Version: 1.0.6
+Version: 1.0.7
 Summary: Payment Gateway
 Home-page: https://github.com/CamPay/campay-python-sdk
 Author: CamPay
 Author-email: info@campay.net
 Project-URL: Bug Tracker, https://github.com/CamPay/campay-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -65,14 +65,16 @@
             "app_password" : "PASTE YOUR APP_PASSWORD HERE",
             "environment" : "DEV" #use "DEV" for demo mode or "PROD" for live mode
         })
     ```
 
 ### To collect payments from your client - DIRECTLY
 
+   **OPTION 1**: This option initiates a transaction and waits( or block the running code) for the transaction to complete before returning a response. 
+
    ```python
          collect = campay.collect({
             "amount": "5", #The amount you want to collect
             "currency": "XAF",
             "from": "2376xxxxxxxx", #Phone number to request amount from. Must include country code
             "description": "some description",
             "external_reference": "", #Reference from the system initiating the transaction.
@@ -80,14 +82,46 @@
 
          print(collect)
          #{"reference": "bcedde9b-62a7-4421-96ac-2e6179552a1a", "external_reference":"12345678", "status": "SUCCESSFUL", "amount": 5, "currency": "XAF", "operator": "MTN", "code": "CP201027T00005", "operator_reference":  "1880106956" }
          
    ```
    > status can be SUCCESSFUL or FAILED
 
+   **OPTION 2**: This option initiates a transaction and immediately returns the initiated transaction reference for you to use to check the status of the transaction.
+
+   ```python
+         collect = campay.initCollect({
+            "amount": "5", #The amount you want to collect
+            "currency": "XAF",
+            "from": "2376xxxxxxxx", #Phone number to request amount from. Must include country code
+            "description": "some description",
+            "external_reference": "", #Reference from the system initiating the transaction.
+         })
+
+         print(collect)
+         #{"reference": "bcedde9b-62a7-4421-96ac-2e6179552a1a", "ussd_code": "*126# for MTN or #150*50# for ORANGE", "operator": "mtn or orange" }
+         
+   ```
+   > The default status for initiated transactions is PENDING
+
+### To check a transaction status.
+
+   You need the initiated transaction **reference** to use this function.
+
+   ```python
+         campay_status = campay.get_transaction_status({
+            "reference": "bcedde9b-62a7-1234-96ac-2e6179552a1a", #The amount you want to collect
+         })
+
+         print(campay_status)
+         #{"reference": "bcedde9b-62a7-4421-96ac-2e6179552a1a", "external_reference":"12345678", "status": "SUCCESSFUL", "amount": 5, "currency": "XAF", "operator": "MTN", "code": "CP201027T00005", "operator_reference":  "1880106956" }
+         
+   ```
+   > status can be PENDING, SUCCESSFUL or FAILED
+
 ### To collect payments from your client - using PAYMENT LINKS
 
    ```python
          payment_link = campay.get_payment_link({
             "amount": "5",
             "currency": "XAF",
             "description": "some description",
@@ -100,14 +134,15 @@
          '''
          Redirect your customer to the returned payment link 
          '''
          
    ```
    > status can be SUCCESSFUL or FAILED
 
+
 ### To disburse
    > Please enable API withdrawal under app settings before trying this request
    
    ```python
         disburse = campay.disburse({
             "amount": "5", #The amount you want to disburse
             "currency": "XAF",
```

