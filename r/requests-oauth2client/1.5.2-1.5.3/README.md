# Comparing `tmp/requests_oauth2client-1.5.2.tar.gz` & `tmp/requests_oauth2client-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_oauth2client-1.5.2.tar", max compression
+gzip compressed data, was "requests_oauth2client-1.5.3.tar", max compression
```

## Comparing `requests_oauth2client-1.5.2.tar` & `requests_oauth2client-1.5.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      126 2024-04-15 12:48:08.410838 requests_oauth2client-1.5.2/AUTHORS.md
--rw-r--r--   0        0        0      586 2024-04-15 12:48:08.410838 requests_oauth2client-1.5.2/LICENSE
--rw-r--r--   0        0        0    42324 2024-04-15 12:48:08.410838 requests_oauth2client-1.5.2/README.md
--rw-r--r--   0        0        0     3405 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     4915 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/__init__.py
--rw-r--r--   0        0        0    20663 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/api_client.py
--rw-r--r--   0        0        0    15250 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/auth.py
--rw-r--r--   0        0        0    30628 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/authorization_request.py
--rw-r--r--   0        0        0     5230 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/backchannel_authentication.py
--rw-r--r--   0        0        0    65234 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/client.py
--rw-r--r--   0        0        0    15640 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/client_authentication.py
--rw-r--r--   0        0        0     4348 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/device_authorization.py
--rw-r--r--   0        0        0     2775 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/discovery.py
--rw-r--r--   0        0        0     8319 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/exceptions.py
--rw-r--r--   0        0        0      228 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/flask/__init__.py
--rw-r--r--   0        0        0     2552 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/flask/auth.py
--rw-r--r--   0        0        0     3491 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/pooling.py
--rw-r--r--   0        0        0        0 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/py.typed
--rw-r--r--   0        0        0    17344 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/tokens.py
--rw-r--r--   0        0        0     3588 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/utils.py
--rw-r--r--   0        0        0      293 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/vendor_specific/__init__.py
--rw-r--r--   0        0        0     5104 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/vendor_specific/auth0.py
--rw-r--r--   0        0        0     2379 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/vendor_specific/ping.py
--rw-r--r--   0        0        0      550 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/.coveragerc
--rw-r--r--   0        0        0        0 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/__init__.py
--rw-r--r--   0        0        0    20551 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/conftest.py
--rw-r--r--   0        0        0     7304 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_authorization_code.py
--rw-r--r--   0        0        0     2068 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_client_credentials.py
--rw-r--r--   0        0        0     4888 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_device_authorization.py
--rw-r--r--   0        0        0     3358 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_oidc.py
--rw-r--r--   0        0        0     2006 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_refresh_token.py
--rw-r--r--   0        0        0     5675 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_token_exchange.py
--rw-r--r--   0        0        0        0 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/__init__.py
--rw-r--r--   0        0        0    16685 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/conftest.py
--rw-r--r--   0        0        0    11645 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/test_api_client.py
--rw-r--r--   0        0        0     8702 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/test_auth.py
--rw-r--r--   0        0        0    10541 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/test_authorization_request.py
--rw-r--r--   0        0        0    10149 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/test_backchannel_authentication.py
--rw-r--r--   0        0        0    57347 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/test_client.py
--rw-r--r--   0        0        0     6095 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_client_authentication.py
--rw-r--r--   0        0        0     7773 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_device_authorization.py
--rw-r--r--   0        0        0     1909 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_discovery.py
--rw-r--r--   0        0        0     3392 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_flask.py
--rw-r--r--   0        0        0    21063 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_oidc.py
--rw-r--r--   0        0        0     1460 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_pkce.py
--rw-r--r--   0        0        0    11502 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_tokens.py
--rw-r--r--   0        0        0     1248 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_utils.py
--rw-r--r--   0        0        0        0 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/vendor_specific/__init__.py
--rw-r--r--   0        0        0     1828 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/vendor_specific/test_auth0.py
--rw-r--r--   0        0        0     1752 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/vendor_specific/test_ping.py
--rw-r--r--   0        0        0    43327 1970-01-01 00:00:00.000000 requests_oauth2client-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0      126 2024-04-26 11:18:13.841716 requests_oauth2client-1.5.3/AUTHORS.md
+-rw-r--r--   0        0        0      586 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/LICENSE
+-rw-r--r--   0        0        0    42460 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/README.md
+-rw-r--r--   0        0        0     3405 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4915 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/__init__.py
+-rw-r--r--   0        0        0    20663 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/api_client.py
+-rw-r--r--   0        0        0    15250 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/auth.py
+-rw-r--r--   0        0        0    30628 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/authorization_request.py
+-rw-r--r--   0        0        0     5230 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/backchannel_authentication.py
+-rw-r--r--   0        0        0    65234 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/client.py
+-rw-r--r--   0        0        0    15640 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/client_authentication.py
+-rw-r--r--   0        0        0     4348 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/device_authorization.py
+-rw-r--r--   0        0        0     2775 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/discovery.py
+-rw-r--r--   0        0        0     8319 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/exceptions.py
+-rw-r--r--   0        0        0      228 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/flask/__init__.py
+-rw-r--r--   0        0        0     2552 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/flask/auth.py
+-rw-r--r--   0        0        0     3491 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/pooling.py
+-rw-r--r--   0        0        0        0 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/py.typed
+-rw-r--r--   0        0        0    17344 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/tokens.py
+-rw-r--r--   0        0        0     3593 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/utils.py
+-rw-r--r--   0        0        0      293 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/vendor_specific/__init__.py
+-rw-r--r--   0        0        0     5104 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/vendor_specific/auth0.py
+-rw-r--r--   0        0        0     2379 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/requests_oauth2client/vendor_specific/ping.py
+-rw-r--r--   0        0        0      550 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/tests/.coveragerc
+-rw-r--r--   0        0        0        0 2024-04-26 11:18:13.845716 requests_oauth2client-1.5.3/tests/__init__.py
+-rw-r--r--   0        0        0    20551 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/conftest.py
+-rw-r--r--   0        0        0     7304 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/test_authorization_code.py
+-rw-r--r--   0        0        0     2068 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/test_client_credentials.py
+-rw-r--r--   0        0        0     4888 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/test_device_authorization.py
+-rw-r--r--   0        0        0     3358 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/test_oidc.py
+-rw-r--r--   0        0        0     2006 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/test_refresh_token.py
+-rw-r--r--   0        0        0     5675 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/test_token_exchange.py
+-rw-r--r--   0        0        0        0 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/__init__.py
+-rw-r--r--   0        0        0    16685 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/conftest.py
+-rw-r--r--   0        0        0    11645 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_api_client.py
+-rw-r--r--   0        0        0     8702 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_auth.py
+-rw-r--r--   0        0        0    10541 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_authorization_request.py
+-rw-r--r--   0        0        0    10149 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_backchannel_authentication.py
+-rw-r--r--   0        0        0    57347 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_client.py
+-rw-r--r--   0        0        0     6095 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_client_authentication.py
+-rw-r--r--   0        0        0     7773 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_device_authorization.py
+-rw-r--r--   0        0        0     1909 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_discovery.py
+-rw-r--r--   0        0        0     3392 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_flask.py
+-rw-r--r--   0        0        0    21063 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_oidc.py
+-rw-r--r--   0        0        0     1460 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_pkce.py
+-rw-r--r--   0        0        0    12121 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_tokens.py
+-rw-r--r--   0        0        0     1248 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/vendor_specific/__init__.py
+-rw-r--r--   0        0        0     1828 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/vendor_specific/test_auth0.py
+-rw-r--r--   0        0        0     1752 2024-04-26 11:18:13.849717 requests_oauth2client-1.5.3/tests/unit_tests/vendor_specific/test_ping.py
+-rw-r--r--   0        0        0    43463 1970-01-01 00:00:00.000000 requests_oauth2client-1.5.3/PKG-INFO
```

### Comparing `requests_oauth2client-1.5.2/LICENSE` & `requests_oauth2client-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/README.md` & `requests_oauth2client-1.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,28 +74,28 @@
 import requests
 from requests_oauth2client import BearerAuth
 
 token = "an_access_token"
 resp = requests.get("https://my.protected.api/endpoint", auth=BearerAuth(token))
 ```
 
-This authentication handler will add a `Authorization: Bearer <access_token>` header in the request,
-with your access token, properly formatted according to [RFC6750](https://datatracker.ietf.org/doc/html/rfc6750#section-2.1).
+This authentication handler will add a `Authorization: Bearer <access_token>` header in the request, with your access
+token, properly formatted according to [RFC6750](https://datatracker.ietf.org/doc/html/rfc6750#section-2.1).
 
 ## Using an OAuth2Client
 
 [OAuth2Client] offers several methods that implement the communication to the various endpoints that are standardised by
 OAuth 2.0 and its extensions. Those endpoints include the Token Endpoint, the Revocation, Introspection, UserInfo,
 BackChannel Authentication and Device Authorization Endpoints.
 
 You have to provide the URLs for those endpoints if you intend to use them. Otherwise, only the Token Endpoint is
 mandatory to initialize an `OAuth2Client`.
 
-To initialize an instance of `OAuth2Client`, you only need a Token Endpoint URI from your AS, and the credentials for your
-application, which are typically a `client_id` and a `client_secret`, usually also provided by the AS:
+To initialize an instance of `OAuth2Client`, you only need a Token Endpoint URI from your AS, and the credentials for
+your application, which are typically a `client_id` and a `client_secret`, usually also provided by the AS:
 
 ```python
 from requests_oauth2client import OAuth2Client
 
 oauth2client = OAuth2Client(
     token_endpoint="https://url.to.the/token_endpoint",
     client_id="my_client_id",
@@ -106,15 +106,17 @@
 The Token Endpoint is the only endpoint that is mandatory to obtain tokens. Credentials are used to authenticate the
 client everytime it sends a request to its Authorization Server. Usually, those are a static Client ID and Secret, which
 are the direct equivalent of a username and a password, but meant for an application instead of for a human user. The
 default authentication method used by `OAuth2Client` is *Client Secret Post*, but other standardised methods such as
 *Client Secret Basic*, *Client Secret JWT* or *Private Key JWT* are supported as well. See
 [more about client authentication methods below](#supported-client-authentication-methods).
 
-Instead of providing each endpoint URL yourself, you may also [use the AS metadata endpoint URI](#initializing-an-oauth2client-from-a-discovery-document), or the document data itself, to initialize your OAuth 2.0 client with the appropriate endpoints.
+Instead of providing each endpoint URL yourself, you may also
+[use the AS metadata endpoint URI](#initializing-an-oauth2client-from-a-discovery-document), or the document data
+itself, to initialize your OAuth 2.0 client with the appropriate endpoints.
 
 ## Obtaining tokens
 
 [OAuth2Client] has dedicated methods to send requests to the Token Endpoint using the different standardised (and/or
 custom) grants. Since the Token Endpoint URL and Client Authentication Method to use are already declared for the client
 at init time, the only required parameters for those methods are those that will be sent in the request to the Token
 Endpoint.
@@ -228,17 +230,20 @@
 When you send your first request,
 [OAuth2ClientCredentialsAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2ClientCredentialsAuth)
 will automatically retrieve an access token from the AS using the Client Credentials grant, then will include it in the
 request. Next requests will use the same token, as long as it is valid. A new token will be automatically retrieved once
 the previous one is expired.
 
 You can configure a leeway, which is a period of time before the actual expiration, in seconds, when a new token will be
-obtained. This may help getting continuous access to the API when the client and API clocks are slightly out of sync. Use the parameter `leeway` to `OAuth2ClientCredentialsAuth`:
+obtained. This may help getting continuous access to the API when the client and API clocks are slightly out of sync.
+Use the parameter `leeway` to `OAuth2ClientCredentialsAuth`:
 
 ```python
+from requests_oauth2client import OAuth2ClientCredentialsAuth
+
 auth = OAuth2ClientCredentialsAuth(
     oauth2client,
     scope="myscope",
     leeway=30,
 )
 ```
 
@@ -261,18 +266,21 @@
 #### Generating Authorization Requests
 
 To be able to use the Authorization Code grant, you need 2 (optionally 3) URIs:
 
 - the URL for Authorization Endpoint, which is the url where you must send your Authorization Requests
 - the Redirect URI, which is the url pointing to your application, where the Authorization Server will reply with
   Authorization Response
-- optionally, the issuer identifier, if your AS uses [Issuer Identification](RFC9207).
+- optionally, the issuer identifier, if your AS uses
+  [Issuer Identification](https://www.rfc-editor.org/rfc/rfc9207.html).
 
-You can declare those URIs when initializing your `OAuth2Client` instance, or you can [use the AS discovery endpoint](#initializing-an-oauth2client-from-a-discovery-document) to initialize those URLs automatically.
-Then you can generate valid Authorization Requests by calling the method `.authorization_request()`, with the request specific parameters, such as `scope`, `state`, `nonce` as parameter:
+You can declare those URIs when initializing your `OAuth2Client` instance, or you can
+[use the AS discovery endpoint](#initializing-an-oauth2client-from-a-discovery-document) to initialize those URLs
+automatically. Then you can generate valid Authorization Requests by calling the method `.authorization_request()`, with
+the request specific parameters, such as `scope`, `state`, `nonce` as parameter:
 
 ```python
 from requests_oauth2client import OAuth2Client
 
 client = OAuth2Client(
     token_endpoint="https://url.to.the/token_endoint",
     authorization_endpoint="https://url.to.the/authorization_endpoint",
@@ -308,28 +316,29 @@
 
 #### Validating the Authorization Response
 
 Once you have redirected the user browser to the Authorization Request URI, and after the user is successfully
 authenticated and authorized, plus any other extra interactive step is complete, the AS will respond with a redirection
 to your redirect_uri. That is the *Authorization Response*. It contains several parameters that must be retrieved by
 your client. The *Authorization Code* is one of those parameters, but you must also validate that the *state* matches
-your request; if using [AS Issuer Identification](RFC9207), you must also validate that the issuer matches what is expected. You can do this with:
+your request; if using [AS Issuer Identification](https://www.rfc-editor.org/rfc/rfc9207.html), you must also validate
+that the issuer matches what is expected. You can do this with:
 
 ```python
 # using the `az_request` as defined above
 
 response_uri = input(
     "Please enter the full url and/or params obtained on the redirect_uri: "
 )
 # say the callback url is https://url.to.my.application/redirect_uri?code=an_az_code&state=FBx9mWeLwoKGgG76vhi6v61-4mgxmgZhtWIa7aTffdY&issuer=https://url.to.the.as
 az_response = az_request.validate_callback(response_uri)
 ```
 
-This `auth_response` is an `AuthorizationResponse` instance and contains everything that is needed for your application to
-complete the authentication and get its tokens from the AS.
+This `auth_response` is an `AuthorizationResponse` instance and contains everything that is needed for your application
+to complete the authentication and get its tokens from the AS.
 
 #### Exchanging code for tokens
 
 Once you have obtained the AS response, containing an authorization code, your application must exchange it for actual
 Token(s).
 
 To exchange a code for Access and/or ID tokens, use the
@@ -817,16 +826,16 @@
     auth=ClientSecretJwt("client_id", "client_secret"),
 )
 ```
 
 This will fetch the document from the specified URI, then will decode it and initialize an [OAuth2Client] pointing to
 the appropriate endpoint URIs.
 
-If using the `issuer` keyword arg, the URI to the discovery endpoint will be deduced from that identifier, and a check will
-be made that the `issuer` from the retrieved metadata document matches that value.
+If using the `issuer` keyword arg, the URI to the discovery endpoint will be deduced from that identifier, and a check
+will be made that the `issuer` from the retrieved metadata document matches that value.
 
 ## Specialized API Client
 
 Using APIs usually involves multiple endpoints under the same root url, with a common authentication method. To make it
 easier, `requests_oauth2client` includes a [requests.Session] wrapper called [ApiClient], which takes the root API url
 as parameter on initialization. You can then send requests to different endpoints by passing their relative path instead
 of the full url. [ApiClient] also accepts an `auth` parameter with an AuthHandler. You can pass any of the OAuth2 Auth
@@ -923,17 +932,17 @@
 
 ## Vendor-Specific clients
 
 `requests_oauth2client` is flexible enough to handle most use cases, so you should be able to use any AS by any vendor
 as long as it supports OAuth 2.0.
 
 You can however create a subclass of [OAuth2Client] or [ApiClient] to make it easier to use with specific Authorization
-Servers or APIs. [OAuth2Client] has several extensibility points in the form of methods like `OAuth2Client.parse_token_response()`,
-`OAuth2Client.on_token_error()` that implement response parsing, error handling, etc.
-
+Servers or APIs. [OAuth2Client] has several extensibility points in the form of methods like
+`OAuth2Client.parse_token_response()`, `OAuth2Client.on_token_error()` that implement response parsing, error handling,
+etc.
 
 ```python
 from requests_oauth2client.vendor_specific import Auth0
 
 a0client = Auth0.client(
     "mytenant.eu", client_id="client_id", client_secret="client_secret"
 )
```

### Comparing `requests_oauth2client-1.5.2/pyproject.toml` & `requests_oauth2client-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "requests_oauth2client"
-version = "1.5.2"
+version = "1.5.3"
 homepage = "https://github.com/guillp/requests_oauth2client"
 description = "An OAuth2.x client based on `requests`."
 authors = ["Guillaume Pujol <guill.p.linux@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
     'Development Status :: 4 - Beta',
```

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/__init__.py` & `requests_oauth2client-1.5.3/requests_oauth2client/__init__.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/api_client.py` & `requests_oauth2client-1.5.3/requests_oauth2client/api_client.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/auth.py` & `requests_oauth2client-1.5.3/requests_oauth2client/auth.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/authorization_request.py` & `requests_oauth2client-1.5.3/requests_oauth2client/authorization_request.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/backchannel_authentication.py` & `requests_oauth2client-1.5.3/requests_oauth2client/backchannel_authentication.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/client.py` & `requests_oauth2client-1.5.3/requests_oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/client_authentication.py` & `requests_oauth2client-1.5.3/requests_oauth2client/client_authentication.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/device_authorization.py` & `requests_oauth2client-1.5.3/requests_oauth2client/device_authorization.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/discovery.py` & `requests_oauth2client-1.5.3/requests_oauth2client/discovery.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/exceptions.py` & `requests_oauth2client-1.5.3/requests_oauth2client/exceptions.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/flask/auth.py` & `requests_oauth2client-1.5.3/requests_oauth2client/flask/auth.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/pooling.py` & `requests_oauth2client-1.5.3/requests_oauth2client/pooling.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/tokens.py` & `requests_oauth2client-1.5.3/requests_oauth2client/tokens.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/utils.py` & `requests_oauth2client-1.5.3/requests_oauth2client/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 This module contains helper methods that are used in multiple places.
 
 """
 
 from __future__ import annotations
 
+from contextlib import suppress
 from datetime import datetime, timedelta, timezone
 from functools import wraps
 from typing import Any, Callable
 
 from furl import furl  # type: ignore[import-untyped]
 
 
@@ -103,14 +104,15 @@
         *args: Any,
         expires_in: int | str | None = None,
         expires_at: datetime | None = None,
         **kwargs: Any,
     ) -> Any:
         if expires_in is None and expires_at is None:
             return f(*args, **kwargs)
-        if expires_in and isinstance(expires_in, str) and expires_in.isdigit() and int(expires_in) >= 1:
-            expires_at = datetime.now(tz=timezone.utc) + timedelta(seconds=int(expires_in))
-        elif expires_in and isinstance(expires_in, int) and expires_in >= 1:
+        if expires_in and isinstance(expires_in, str):
+            with suppress(ValueError):
+                expires_at = datetime.now(tz=timezone.utc) + timedelta(seconds=int(expires_in))
+        elif expires_in and isinstance(expires_in, int):
             expires_at = datetime.now(tz=timezone.utc) + timedelta(seconds=expires_in)
         return f(*args, expires_at=expires_at, **kwargs)
 
     return decorator
```

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/vendor_specific/auth0.py` & `requests_oauth2client-1.5.3/requests_oauth2client/vendor_specific/auth0.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/requests_oauth2client/vendor_specific/ping.py` & `requests_oauth2client-1.5.3/requests_oauth2client/vendor_specific/ping.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/.coveragerc` & `requests_oauth2client-1.5.3/tests/.coveragerc`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/conftest.py` & `requests_oauth2client-1.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/test_authorization_code.py` & `requests_oauth2client-1.5.3/tests/test_authorization_code.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/test_client_credentials.py` & `requests_oauth2client-1.5.3/tests/test_client_credentials.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/test_device_authorization.py` & `requests_oauth2client-1.5.3/tests/test_device_authorization.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/test_oidc.py` & `requests_oauth2client-1.5.3/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/test_refresh_token.py` & `requests_oauth2client-1.5.3/tests/test_refresh_token.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/test_token_exchange.py` & `requests_oauth2client-1.5.3/tests/test_token_exchange.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/conftest.py` & `requests_oauth2client-1.5.3/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_api_client.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_auth.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_authorization_request.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_authorization_request.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_backchannel_authentication.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_backchannel_authentication.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_client.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_client_authentication.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_client_authentication.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_device_authorization.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_device_authorization.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_discovery.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_flask.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_flask.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_oidc.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_pkce.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_pkce.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_tokens.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -196,15 +196,14 @@
     )
 
     with pytest.raises(ExpiredJwt):
         id_token.validate(public_jwk, issuer=issuer, audience=audience, nonce=nonce, check_exp=True)
 
     assert id_token.alg == "RS256"
     assert id_token.kid == "my_key"
-    assert id_token == id_token
     assert id_token.aud == audience
     assert id_token.is_expired()
     assert id_token.is_expired(1000)
     assert id_token.expires_at == datetime(2021, 8, 17, 12, 50, 20, tzinfo=timezone.utc)
     assert id_token.issued_at == datetime(2021, 8, 17, 12, 49, 20, tzinfo=timezone.utc)
 
 
@@ -280,9 +279,20 @@
 
 
 @freeze_time()
 def test_token_serializer() -> None:
     serializer = BearerTokenSerializer()
     assert serializer.dumps(BearerToken("access_token")) == "q1ZKTE5OLS6OL8nPTs1TskLl6iiB6fiSyoJUoJxTamJRapFSLQA"
     assert serializer.loads("q1ZKTE5OLS6OL8nPTs1TskLl6iiB6fiSyoJUoJxTamJRapFSLQA") == BearerToken("access_token")
+
     assert serializer.dumps(BearerToken("access_token", expires_in=60)) == "q1ZKTE5OLS6OL8nPTs1TskLl6iiB6fiSyoJUoJxTamJRahFQNLWiILMotTg-E6jDzKAWAA"
     assert serializer.loads("q1ZKTE5OLS6OL8nPTs1TskLl6iiB6fiSyoJUoJxTamJRahFQNLWiILMotTg-E6jDzKAWAA") == BearerToken("access_token", expires_in=60)
+
+    assert serializer.dumps(BearerToken("access_token", expires_in=-60)) == "q1ZKTE5OLS6OL8nPTs1TskLl6iiB6fiSyoJUoJxTamJRahFQNLWiILMotTg-E6hD18ygFgA"
+    assert serializer.loads("q1ZKTE5OLS6OL8nPTs1TskLl6iiB6fiSyoJUoJxTamJRahFQNLWiILMotTg-E6hD18ygFgA") == BearerToken("access_token", expires_in=-60)
+
+
+@freeze_time()
+def test_expires_in_as_str() -> None:
+    assert BearerToken("access_token", expires_in=60) == BearerToken("access_token", expires_in="60")
+    assert BearerToken("access_token", expires_in=-60) == BearerToken("access_token", expires_in="-60")
+    assert BearerToken("access_token", expires_in="foo") == BearerToken("access_token")
```

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/test_utils.py` & `requests_oauth2client-1.5.3/tests/unit_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/vendor_specific/test_auth0.py` & `requests_oauth2client-1.5.3/tests/unit_tests/vendor_specific/test_auth0.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/tests/unit_tests/vendor_specific/test_ping.py` & `requests_oauth2client-1.5.3/tests/unit_tests/vendor_specific/test_ping.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.2/PKG-INFO` & `requests_oauth2client-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests_oauth2client
-Version: 1.5.2
+Version: 1.5.3
 Summary: An OAuth2.x client based on `requests`.
 Home-page: https://github.com/guillp/requests_oauth2client
 License: Apache-2.0
 Author: Guillaume Pujol
 Author-email: guill.p.linux@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
@@ -102,28 +102,28 @@
 import requests
 from requests_oauth2client import BearerAuth
 
 token = "an_access_token"
 resp = requests.get("https://my.protected.api/endpoint", auth=BearerAuth(token))
 ```
 
-This authentication handler will add a `Authorization: Bearer <access_token>` header in the request,
-with your access token, properly formatted according to [RFC6750](https://datatracker.ietf.org/doc/html/rfc6750#section-2.1).
+This authentication handler will add a `Authorization: Bearer <access_token>` header in the request, with your access
+token, properly formatted according to [RFC6750](https://datatracker.ietf.org/doc/html/rfc6750#section-2.1).
 
 ## Using an OAuth2Client
 
 [OAuth2Client] offers several methods that implement the communication to the various endpoints that are standardised by
 OAuth 2.0 and its extensions. Those endpoints include the Token Endpoint, the Revocation, Introspection, UserInfo,
 BackChannel Authentication and Device Authorization Endpoints.
 
 You have to provide the URLs for those endpoints if you intend to use them. Otherwise, only the Token Endpoint is
 mandatory to initialize an `OAuth2Client`.
 
-To initialize an instance of `OAuth2Client`, you only need a Token Endpoint URI from your AS, and the credentials for your
-application, which are typically a `client_id` and a `client_secret`, usually also provided by the AS:
+To initialize an instance of `OAuth2Client`, you only need a Token Endpoint URI from your AS, and the credentials for
+your application, which are typically a `client_id` and a `client_secret`, usually also provided by the AS:
 
 ```python
 from requests_oauth2client import OAuth2Client
 
 oauth2client = OAuth2Client(
     token_endpoint="https://url.to.the/token_endpoint",
     client_id="my_client_id",
@@ -134,15 +134,17 @@
 The Token Endpoint is the only endpoint that is mandatory to obtain tokens. Credentials are used to authenticate the
 client everytime it sends a request to its Authorization Server. Usually, those are a static Client ID and Secret, which
 are the direct equivalent of a username and a password, but meant for an application instead of for a human user. The
 default authentication method used by `OAuth2Client` is *Client Secret Post*, but other standardised methods such as
 *Client Secret Basic*, *Client Secret JWT* or *Private Key JWT* are supported as well. See
 [more about client authentication methods below](#supported-client-authentication-methods).
 
-Instead of providing each endpoint URL yourself, you may also [use the AS metadata endpoint URI](#initializing-an-oauth2client-from-a-discovery-document), or the document data itself, to initialize your OAuth 2.0 client with the appropriate endpoints.
+Instead of providing each endpoint URL yourself, you may also
+[use the AS metadata endpoint URI](#initializing-an-oauth2client-from-a-discovery-document), or the document data
+itself, to initialize your OAuth 2.0 client with the appropriate endpoints.
 
 ## Obtaining tokens
 
 [OAuth2Client] has dedicated methods to send requests to the Token Endpoint using the different standardised (and/or
 custom) grants. Since the Token Endpoint URL and Client Authentication Method to use are already declared for the client
 at init time, the only required parameters for those methods are those that will be sent in the request to the Token
 Endpoint.
@@ -256,17 +258,20 @@
 When you send your first request,
 [OAuth2ClientCredentialsAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2ClientCredentialsAuth)
 will automatically retrieve an access token from the AS using the Client Credentials grant, then will include it in the
 request. Next requests will use the same token, as long as it is valid. A new token will be automatically retrieved once
 the previous one is expired.
 
 You can configure a leeway, which is a period of time before the actual expiration, in seconds, when a new token will be
-obtained. This may help getting continuous access to the API when the client and API clocks are slightly out of sync. Use the parameter `leeway` to `OAuth2ClientCredentialsAuth`:
+obtained. This may help getting continuous access to the API when the client and API clocks are slightly out of sync.
+Use the parameter `leeway` to `OAuth2ClientCredentialsAuth`:
 
 ```python
+from requests_oauth2client import OAuth2ClientCredentialsAuth
+
 auth = OAuth2ClientCredentialsAuth(
     oauth2client,
     scope="myscope",
     leeway=30,
 )
 ```
 
@@ -289,18 +294,21 @@
 #### Generating Authorization Requests
 
 To be able to use the Authorization Code grant, you need 2 (optionally 3) URIs:
 
 - the URL for Authorization Endpoint, which is the url where you must send your Authorization Requests
 - the Redirect URI, which is the url pointing to your application, where the Authorization Server will reply with
   Authorization Response
-- optionally, the issuer identifier, if your AS uses [Issuer Identification](RFC9207).
+- optionally, the issuer identifier, if your AS uses
+  [Issuer Identification](https://www.rfc-editor.org/rfc/rfc9207.html).
 
-You can declare those URIs when initializing your `OAuth2Client` instance, or you can [use the AS discovery endpoint](#initializing-an-oauth2client-from-a-discovery-document) to initialize those URLs automatically.
-Then you can generate valid Authorization Requests by calling the method `.authorization_request()`, with the request specific parameters, such as `scope`, `state`, `nonce` as parameter:
+You can declare those URIs when initializing your `OAuth2Client` instance, or you can
+[use the AS discovery endpoint](#initializing-an-oauth2client-from-a-discovery-document) to initialize those URLs
+automatically. Then you can generate valid Authorization Requests by calling the method `.authorization_request()`, with
+the request specific parameters, such as `scope`, `state`, `nonce` as parameter:
 
 ```python
 from requests_oauth2client import OAuth2Client
 
 client = OAuth2Client(
     token_endpoint="https://url.to.the/token_endoint",
     authorization_endpoint="https://url.to.the/authorization_endpoint",
@@ -336,28 +344,29 @@
 
 #### Validating the Authorization Response
 
 Once you have redirected the user browser to the Authorization Request URI, and after the user is successfully
 authenticated and authorized, plus any other extra interactive step is complete, the AS will respond with a redirection
 to your redirect_uri. That is the *Authorization Response*. It contains several parameters that must be retrieved by
 your client. The *Authorization Code* is one of those parameters, but you must also validate that the *state* matches
-your request; if using [AS Issuer Identification](RFC9207), you must also validate that the issuer matches what is expected. You can do this with:
+your request; if using [AS Issuer Identification](https://www.rfc-editor.org/rfc/rfc9207.html), you must also validate
+that the issuer matches what is expected. You can do this with:
 
 ```python
 # using the `az_request` as defined above
 
 response_uri = input(
     "Please enter the full url and/or params obtained on the redirect_uri: "
 )
 # say the callback url is https://url.to.my.application/redirect_uri?code=an_az_code&state=FBx9mWeLwoKGgG76vhi6v61-4mgxmgZhtWIa7aTffdY&issuer=https://url.to.the.as
 az_response = az_request.validate_callback(response_uri)
 ```
 
-This `auth_response` is an `AuthorizationResponse` instance and contains everything that is needed for your application to
-complete the authentication and get its tokens from the AS.
+This `auth_response` is an `AuthorizationResponse` instance and contains everything that is needed for your application
+to complete the authentication and get its tokens from the AS.
 
 #### Exchanging code for tokens
 
 Once you have obtained the AS response, containing an authorization code, your application must exchange it for actual
 Token(s).
 
 To exchange a code for Access and/or ID tokens, use the
@@ -845,16 +854,16 @@
     auth=ClientSecretJwt("client_id", "client_secret"),
 )
 ```
 
 This will fetch the document from the specified URI, then will decode it and initialize an [OAuth2Client] pointing to
 the appropriate endpoint URIs.
 
-If using the `issuer` keyword arg, the URI to the discovery endpoint will be deduced from that identifier, and a check will
-be made that the `issuer` from the retrieved metadata document matches that value.
+If using the `issuer` keyword arg, the URI to the discovery endpoint will be deduced from that identifier, and a check
+will be made that the `issuer` from the retrieved metadata document matches that value.
 
 ## Specialized API Client
 
 Using APIs usually involves multiple endpoints under the same root url, with a common authentication method. To make it
 easier, `requests_oauth2client` includes a [requests.Session] wrapper called [ApiClient], which takes the root API url
 as parameter on initialization. You can then send requests to different endpoints by passing their relative path instead
 of the full url. [ApiClient] also accepts an `auth` parameter with an AuthHandler. You can pass any of the OAuth2 Auth
@@ -951,17 +960,17 @@
 
 ## Vendor-Specific clients
 
 `requests_oauth2client` is flexible enough to handle most use cases, so you should be able to use any AS by any vendor
 as long as it supports OAuth 2.0.
 
 You can however create a subclass of [OAuth2Client] or [ApiClient] to make it easier to use with specific Authorization
-Servers or APIs. [OAuth2Client] has several extensibility points in the form of methods like `OAuth2Client.parse_token_response()`,
-`OAuth2Client.on_token_error()` that implement response parsing, error handling, etc.
-
+Servers or APIs. [OAuth2Client] has several extensibility points in the form of methods like
+`OAuth2Client.parse_token_response()`, `OAuth2Client.on_token_error()` that implement response parsing, error handling,
+etc.
 
 ```python
 from requests_oauth2client.vendor_specific import Auth0
 
 a0client = Auth0.client(
     "mytenant.eu", client_id="client_id", client_secret="client_secret"
 )
```

