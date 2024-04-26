# Comparing `tmp/mypy-boto3-cognito-idp-1.34.59.tar.gz` & `tmp/mypy_boto3_cognito_idp-1.34.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-idp-1.34.59.tar", last modified: Fri Mar  8 20:21:20 2024, max compression
+gzip compressed data, was "mypy_boto3_cognito_idp-1.34.91.tar", last modified: Thu Apr 25 00:48:23 2024, max compression
```

## Comparing `mypy-boto3-cognito-idp-1.34.59.tar` & `mypy_boto3_cognito_idp-1.34.91.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:21:20.598137 mypy-boto3-cognito-idp-1.34.59/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-08 20:21:01.000000 mypy-boto3-cognito-idp-1.34.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14243 2024-03-08 20:21:20.598137 mypy-boto3-cognito-idp-1.34.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-03-08 20:21:01.000000 mypy-boto3-cognito-idp-1.34.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:21:20.598137 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-03-08 20:21:01.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-03-08 20:21:01.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-08 20:21:01.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    80779 2024-03-08 20:21:02.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    80776 2024-03-08 20:21:02.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-03-08 20:21:02.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-03-08 20:21:02.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-03-08 20:21:02.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-03-08 20:21:02.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:21:01.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    81400 2024-03-08 20:21:04.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    81400 2024-03-08 20:21:03.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-08 20:21:01.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:21:20.598137 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14243 2024-03-08 20:21:20.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-08 20:21:20.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:21:20.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:21:20.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-08 20:21:20.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-08 20:21:20.000000 mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 20:21:20.598137 mypy-boto3-cognito-idp-1.34.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-08 20:21:01.000000 mypy-boto3-cognito-idp-1.34.59/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:23.058523 mypy_boto3_cognito_idp-1.34.91/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14243 2024-04-25 00:48:23.058523 mypy_boto3_cognito_idp-1.34.91/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12660 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:23.058523 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2396 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2396 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    80829 2024-04-24 23:43:40.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    80826 2024-04-24 23:43:39.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14776 2024-04-24 23:43:42.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14776 2024-04-24 23:43:41.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11049 2024-04-24 23:43:41.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11039 2024-04-24 23:43:41.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    83482 2024-04-24 23:43:47.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    83482 2024-04-24 23:43:45.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       62 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:23.058523 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14243 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      756 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       53 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       23 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2024-04-25 00:48:23.058523 mypy_boto3_cognito_idp-1.34.91/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2014 2024-04-24 23:43:36.000000 mypy_boto3_cognito_idp-1.34.91/setup.py
```

### Comparing `mypy-boto3-cognito-idp-1.34.59/LICENSE` & `mypy_boto3_cognito_idp-1.34.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.34.59/PKG-INFO` & `mypy_boto3_cognito_idp-1.34.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.34.59
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.34.59 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.34.91 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-idp)](https://pepy.tech/project/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.34.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cognito-idp-1.34.59/README.md` & `mypy_boto3_cognito_idp-1.34.91/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-idp)](https://pepy.tech/project/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.34.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/__init__.py` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/__init__.pyi` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/__main__.py` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoIdentityProvider 1.34.59\n"
-        "Version:         1.34.59\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.CognitoIdentityProvider 1.34.91\n"
+        "Version:         1.34.91\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.59")
+    print("1.34.91")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/client.py` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     ListResourceServersPaginator,
     ListUserPoolClientsPaginator,
     ListUserPoolsPaginator,
     ListUsersInGroupPaginator,
     ListUsersPaginator,
 )
 from .type_defs import (
-    AccountRecoverySettingTypeTypeDef,
+    AccountRecoverySettingTypeUnionTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserResponseTypeDef,
     AdminGetDeviceResponseTypeDef,
     AdminGetUserResponseTypeDef,
     AdminInitiateAuthResponseTypeDef,
     AdminListDevicesResponseTypeDef,
@@ -60,15 +60,15 @@
     AdminListUserAuthEventsResponseTypeDef,
     AdminRespondToAuthChallengeResponseTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AssociateSoftwareTokenResponseTypeDef,
     AttributeTypeTypeDef,
     BlobTypeDef,
-    CompromisedCredentialsRiskConfigurationTypeTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeUnionTypeDef,
     ConfirmDeviceResponseTypeDef,
     ContextDataTypeTypeDef,
     CreateGroupResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
     CreateResourceServerResponseTypeDef,
     CreateUserImportJobResponseTypeDef,
     CreateUserPoolClientResponseTypeDef,
@@ -111,15 +111,15 @@
     ListUsersResponseTypeDef,
     LogConfigurationTypeTypeDef,
     MFAOptionTypeTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     ResendConfirmationCodeResponseTypeDef,
     ResourceServerScopeTypeTypeDef,
     RespondToAuthChallengeResponseTypeDef,
-    RiskExceptionConfigurationTypeTypeDef,
+    RiskExceptionConfigurationTypeUnionTypeDef,
     SchemaAttributeTypeTypeDef,
     SetLogDeliveryConfigurationResponseTypeDef,
     SetRiskConfigurationResponseTypeDef,
     SetUICustomizationResponseTypeDef,
     SetUserPoolMfaConfigResponseTypeDef,
     SignUpResponseTypeDef,
     SmsConfigurationTypeTypeDef,
@@ -132,15 +132,15 @@
     TokenValidityUnitsTypeTypeDef,
     UpdateGroupResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     UpdateResourceServerResponseTypeDef,
     UpdateUserAttributesResponseTypeDef,
     UpdateUserPoolClientResponseTypeDef,
     UpdateUserPoolDomainResponseTypeDef,
-    UserAttributeUpdateSettingsTypeTypeDef,
+    UserAttributeUpdateSettingsTypeUnionTypeDef,
     UserContextDataTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
     VerifySoftwareTokenResponseTypeDef,
 )
@@ -714,24 +714,24 @@
         UsernameAttributes: Sequence[UsernameAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...,
+        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...,
     ) -> CreateUserPoolResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool)
         """
@@ -1251,17 +1251,17 @@
         """
 
     def set_risk_configuration(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
-        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
+        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
-        RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...,
+        RiskExceptionConfiguration: RiskExceptionConfigurationTypeUnionTypeDef = ...,
     ) -> SetRiskConfigurationResponseTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_risk_configuration)
         """
@@ -1481,23 +1481,23 @@
         LambdaConfig: LambdaConfigTypeTypeDef = ...,
         AutoVerifiedAttributes: Sequence[VerifiedAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...,
+        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_pool)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/client.pyi` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     ListResourceServersPaginator,
     ListUserPoolClientsPaginator,
     ListUserPoolsPaginator,
     ListUsersInGroupPaginator,
     ListUsersPaginator,
 )
 from .type_defs import (
-    AccountRecoverySettingTypeTypeDef,
+    AccountRecoverySettingTypeUnionTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserResponseTypeDef,
     AdminGetDeviceResponseTypeDef,
     AdminGetUserResponseTypeDef,
     AdminInitiateAuthResponseTypeDef,
     AdminListDevicesResponseTypeDef,
@@ -60,15 +60,15 @@
     AdminListUserAuthEventsResponseTypeDef,
     AdminRespondToAuthChallengeResponseTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AssociateSoftwareTokenResponseTypeDef,
     AttributeTypeTypeDef,
     BlobTypeDef,
-    CompromisedCredentialsRiskConfigurationTypeTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeUnionTypeDef,
     ConfirmDeviceResponseTypeDef,
     ContextDataTypeTypeDef,
     CreateGroupResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
     CreateResourceServerResponseTypeDef,
     CreateUserImportJobResponseTypeDef,
     CreateUserPoolClientResponseTypeDef,
@@ -111,15 +111,15 @@
     ListUsersResponseTypeDef,
     LogConfigurationTypeTypeDef,
     MFAOptionTypeTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     ResendConfirmationCodeResponseTypeDef,
     ResourceServerScopeTypeTypeDef,
     RespondToAuthChallengeResponseTypeDef,
-    RiskExceptionConfigurationTypeTypeDef,
+    RiskExceptionConfigurationTypeUnionTypeDef,
     SchemaAttributeTypeTypeDef,
     SetLogDeliveryConfigurationResponseTypeDef,
     SetRiskConfigurationResponseTypeDef,
     SetUICustomizationResponseTypeDef,
     SetUserPoolMfaConfigResponseTypeDef,
     SignUpResponseTypeDef,
     SmsConfigurationTypeTypeDef,
@@ -132,15 +132,15 @@
     TokenValidityUnitsTypeTypeDef,
     UpdateGroupResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     UpdateResourceServerResponseTypeDef,
     UpdateUserAttributesResponseTypeDef,
     UpdateUserPoolClientResponseTypeDef,
     UpdateUserPoolDomainResponseTypeDef,
-    UserAttributeUpdateSettingsTypeTypeDef,
+    UserAttributeUpdateSettingsTypeUnionTypeDef,
     UserContextDataTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
     VerifySoftwareTokenResponseTypeDef,
 )
@@ -711,24 +711,24 @@
         UsernameAttributes: Sequence[UsernameAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...,
+        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...,
     ) -> CreateUserPoolResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool)
         """
@@ -1248,17 +1248,17 @@
         """
 
     def set_risk_configuration(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
-        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
+        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
-        RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...,
+        RiskExceptionConfiguration: RiskExceptionConfigurationTypeUnionTypeDef = ...,
     ) -> SetRiskConfigurationResponseTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_risk_configuration)
         """
@@ -1478,23 +1478,23 @@
         LambdaConfig: LambdaConfigTypeTypeDef = ...,
         AutoVerifiedAttributes: Sequence[VerifiedAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...,
+        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_pool)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/literals.py` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -255,24 +256,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -333,15 +336,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -470,14 +472,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -521,14 +524,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -574,25 +578,30 @@
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "il-central-1",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/literals.pyi` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -255,24 +256,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -333,15 +336,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -470,14 +472,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -521,14 +524,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -574,25 +578,30 @@
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "il-central-1",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/paginator.py` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/paginator.pyi` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/type_defs.py` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,26 +175,29 @@
     "ListUserPoolsRequestRequestTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
     "PasswordPolicyTypeTypeDef",
     "RevokeTokenRequestRequestTypeDef",
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
+    "AccountRecoverySettingTypeOutputTypeDef",
     "AccountRecoverySettingTypeTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
@@ -235,14 +238,15 @@
     "SetUICustomizationRequestRequestTypeDef",
     "LogConfigurationTypeTypeDef",
     "ForgotPasswordResponseTypeDef",
     "GetUserAttributeVerificationCodeResponseTypeDef",
     "ResendConfirmationCodeResponseTypeDef",
     "SignUpResponseTypeDef",
     "UpdateUserAttributesResponseTypeDef",
+    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     "ConfirmDeviceRequestRequestTypeDef",
     "ConfirmForgotPasswordRequestRequestTypeDef",
     "ConfirmSignUpRequestRequestTypeDef",
     "ForgotPasswordRequestRequestTypeDef",
     "InitiateAuthRequestRequestTypeDef",
     "ResendConfirmationCodeRequestRequestTypeDef",
@@ -271,29 +275,33 @@
     "GetUICustomizationResponseTypeDef",
     "SetUICustomizationResponseTypeDef",
     "LambdaConfigTypeTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "ListUserPoolClientsResponseTypeDef",
     "NotifyConfigurationTypeTypeDef",
     "UserPoolPolicyTypeTypeDef",
+    "RiskExceptionConfigurationTypeUnionTypeDef",
     "SchemaAttributeTypeTypeDef",
+    "UserAttributeUpdateSettingsTypeUnionTypeDef",
+    "AccountRecoverySettingTypeUnionTypeDef",
     "AdminGetDeviceResponseTypeDef",
     "AdminListDevicesResponseTypeDef",
     "GetDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "AdminCreateUserResponseTypeDef",
     "ListUsersInGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "AdminListUserAuthEventsResponseTypeDef",
     "AdminInitiateAuthResponseTypeDef",
     "AdminRespondToAuthChallengeResponseTypeDef",
     "InitiateAuthResponseTypeDef",
     "RespondToAuthChallengeResponseTypeDef",
     "LogDeliveryConfigurationTypeTypeDef",
     "SetLogDeliveryConfigurationRequestRequestTypeDef",
+    "CompromisedCredentialsRiskConfigurationTypeUnionTypeDef",
     "AdminInitiateAuthRequestRequestTypeDef",
     "AdminRespondToAuthChallengeRequestRequestTypeDef",
     "CreateResourceServerResponseTypeDef",
     "DescribeResourceServerResponseTypeDef",
     "ListResourceServersResponseTypeDef",
     "UpdateResourceServerResponseTypeDef",
     "CreateUserPoolClientResponseTypeDef",
@@ -1149,21 +1157,28 @@
     "RevokeTokenRequestRequestTypeDef",
     {
         "Token": str,
         "ClientId": str,
         "ClientSecret": NotRequired[str],
     },
 )
-RiskExceptionConfigurationTypeTypeDef = TypedDict(
-    "RiskExceptionConfigurationTypeTypeDef",
+RiskExceptionConfigurationTypeOutputTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     {
         "BlockedIPRangeList": NotRequired[List[str]],
         "SkippedIPRangeList": NotRequired[List[str]],
     },
 )
+RiskExceptionConfigurationTypeTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeTypeDef",
+    {
+        "BlockedIPRangeList": NotRequired[Sequence[str]],
+        "SkippedIPRangeList": NotRequired[Sequence[str]],
+    },
+)
 StringAttributeConstraintsTypeTypeDef = TypedDict(
     "StringAttributeConstraintsTypeTypeDef",
     {
         "MinLength": NotRequired[str],
         "MaxLength": NotRequired[str],
     },
 )
@@ -1229,14 +1244,20 @@
         "UserPoolId": str,
         "ProviderName": str,
         "ProviderDetails": NotRequired[Mapping[str, str]],
         "AttributeMapping": NotRequired[Mapping[str, str]],
         "IdpIdentifiers": NotRequired[Sequence[str]],
     },
 )
+UserAttributeUpdateSettingsTypeOutputTypeDef = TypedDict(
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
+    {
+        "AttributesRequireVerificationBeforeUpdate": NotRequired[List[VerifiedAttributeTypeType]],
+    },
+)
 VerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "VerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
         "AccessToken": NotRequired[str],
         "Session": NotRequired[str],
         "FriendlyDeviceName": NotRequired[str],
@@ -1246,14 +1267,20 @@
     "VerifyUserAttributeRequestRequestTypeDef",
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
     },
 )
+AccountRecoverySettingTypeOutputTypeDef = TypedDict(
+    "AccountRecoverySettingTypeOutputTypeDef",
+    {
+        "RecoveryMechanisms": NotRequired[List[RecoveryOptionTypeTypeDef]],
+    },
+)
 AccountRecoverySettingTypeTypeDef = TypedDict(
     "AccountRecoverySettingTypeTypeDef",
     {
         "RecoveryMechanisms": NotRequired[Sequence[RecoveryOptionTypeTypeDef]],
     },
 )
 AccountTakeoverActionsTypeTypeDef = TypedDict(
@@ -1513,16 +1540,16 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 AdminListGroupsForUserResponseTypeDef = TypedDict(
     "AdminListGroupsForUserResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1535,16 +1562,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateGroupResponseTypeDef = TypedDict(
     "UpdateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1641,19 +1668,26 @@
 UpdateUserAttributesResponseTypeDef = TypedDict(
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
+    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
+    {
+        "Actions": CompromisedCredentialsActionsTypeTypeDef,
+        "EventFilter": NotRequired[List[EventFilterTypeType]],
+    },
+)
 CompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
-        "EventFilter": NotRequired[List[EventFilterTypeType]],
+        "EventFilter": NotRequired[Sequence[EventFilterTypeType]],
     },
 )
 ConfirmDeviceRequestRequestTypeDef = TypedDict(
     "ConfirmDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
         "DeviceKey": str,
@@ -2000,24 +2034,24 @@
         "KMSKeyID": NotRequired[str],
     },
 )
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "Providers": List[ProviderDescriptionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUserPoolClientsResponseTypeDef = TypedDict(
     "ListUserPoolClientsResponseTypeDef",
     {
         "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 NotifyConfigurationTypeTypeDef = TypedDict(
     "NotifyConfigurationTypeTypeDef",
     {
         "SourceArn": str,
         "From": NotRequired[str],
@@ -2029,26 +2063,35 @@
 )
 UserPoolPolicyTypeTypeDef = TypedDict(
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": NotRequired[PasswordPolicyTypeTypeDef],
     },
 )
+RiskExceptionConfigurationTypeUnionTypeDef = Union[
+    RiskExceptionConfigurationTypeTypeDef, RiskExceptionConfigurationTypeOutputTypeDef
+]
 SchemaAttributeTypeTypeDef = TypedDict(
     "SchemaAttributeTypeTypeDef",
     {
         "Name": NotRequired[str],
         "AttributeDataType": NotRequired[AttributeDataTypeType],
         "DeveloperOnlyAttribute": NotRequired[bool],
         "Mutable": NotRequired[bool],
         "Required": NotRequired[bool],
         "NumberAttributeConstraints": NotRequired[NumberAttributeConstraintsTypeTypeDef],
         "StringAttributeConstraints": NotRequired[StringAttributeConstraintsTypeTypeDef],
     },
 )
+UserAttributeUpdateSettingsTypeUnionTypeDef = Union[
+    UserAttributeUpdateSettingsTypeTypeDef, UserAttributeUpdateSettingsTypeOutputTypeDef
+]
+AccountRecoverySettingTypeUnionTypeDef = Union[
+    AccountRecoverySettingTypeTypeDef, AccountRecoverySettingTypeOutputTypeDef
+]
 AdminGetDeviceResponseTypeDef = TypedDict(
     "AdminGetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2082,32 +2125,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListUsersInGroupResponseTypeDef = TypedDict(
     "ListUsersInGroupResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 AdminListUserAuthEventsResponseTypeDef = TypedDict(
     "AdminListUserAuthEventsResponseTypeDef",
     {
         "AuthEvents": List[AuthEventTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AdminInitiateAuthResponseTypeDef = TypedDict(
     "AdminInitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
@@ -2156,14 +2199,18 @@
 SetLogDeliveryConfigurationRequestRequestTypeDef = TypedDict(
     "SetLogDeliveryConfigurationRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "LogConfigurations": Sequence[LogConfigurationTypeTypeDef],
     },
 )
+CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = Union[
+    CompromisedCredentialsRiskConfigurationTypeTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
+]
 AdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "AdminInitiateAuthRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "AuthFlow": AuthFlowTypeType,
         "AuthParameters": NotRequired[Mapping[str, str]],
@@ -2199,16 +2246,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResourceServersResponseTypeDef = TypedDict(
     "ListResourceServersResponseTypeDef",
     {
         "ResourceServers": List[ResourceServerTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateResourceServerResponseTypeDef = TypedDict(
     "UpdateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2362,30 +2409,30 @@
         "AliasAttributes": NotRequired[List[AliasAttributeTypeType]],
         "UsernameAttributes": NotRequired[List[UsernameAttributeTypeType]],
         "SmsVerificationMessage": NotRequired[str],
         "EmailVerificationMessage": NotRequired[str],
         "EmailVerificationSubject": NotRequired[str],
         "VerificationMessageTemplate": NotRequired[VerificationMessageTemplateTypeTypeDef],
         "SmsAuthenticationMessage": NotRequired[str],
-        "UserAttributeUpdateSettings": NotRequired[UserAttributeUpdateSettingsTypeTypeDef],
+        "UserAttributeUpdateSettings": NotRequired[UserAttributeUpdateSettingsTypeOutputTypeDef],
         "MfaConfiguration": NotRequired[UserPoolMfaTypeType],
         "DeviceConfiguration": NotRequired[DeviceConfigurationTypeTypeDef],
         "EstimatedNumberOfUsers": NotRequired[int],
         "EmailConfiguration": NotRequired[EmailConfigurationTypeTypeDef],
         "SmsConfiguration": NotRequired[SmsConfigurationTypeTypeDef],
         "UserPoolTags": NotRequired[Dict[str, str]],
         "SmsConfigurationFailure": NotRequired[str],
         "EmailConfigurationFailure": NotRequired[str],
         "Domain": NotRequired[str],
         "CustomDomain": NotRequired[str],
         "AdminCreateUserConfig": NotRequired[AdminCreateUserConfigTypeTypeDef],
         "UserPoolAddOns": NotRequired[UserPoolAddOnsTypeTypeDef],
         "UsernameConfiguration": NotRequired[UsernameConfigurationTypeTypeDef],
         "Arn": NotRequired[str],
-        "AccountRecoverySetting": NotRequired[AccountRecoverySettingTypeTypeDef],
+        "AccountRecoverySetting": NotRequired[AccountRecoverySettingTypeOutputTypeDef],
     },
 )
 GetLogDeliveryConfigurationResponseTypeDef = TypedDict(
     "GetLogDeliveryConfigurationResponseTypeDef",
     {
         "LogDeliveryConfiguration": LogDeliveryConfigurationTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2398,30 +2445,30 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
         "UserPools": List[UserPoolDescriptionTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RiskConfigurationTypeTypeDef = TypedDict(
     "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": NotRequired[str],
         "ClientId": NotRequired[str],
         "CompromisedCredentialsRiskConfiguration": NotRequired[
-            CompromisedCredentialsRiskConfigurationTypeTypeDef
+            CompromisedCredentialsRiskConfigurationTypeOutputTypeDef
         ],
         "AccountTakeoverRiskConfiguration": NotRequired[
             AccountTakeoverRiskConfigurationTypeTypeDef
         ],
-        "RiskExceptionConfiguration": NotRequired[RiskExceptionConfigurationTypeTypeDef],
+        "RiskExceptionConfiguration": NotRequired[RiskExceptionConfigurationTypeOutputTypeDef],
         "LastModifiedDate": NotRequired[datetime],
     },
 )
 SetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "SetRiskConfigurationRequestRequestTypeDef",
     {
         "UserPoolId": str,
```

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp/type_defs.pyi` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -175,26 +175,29 @@
     "ListUserPoolsRequestRequestTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
     "PasswordPolicyTypeTypeDef",
     "RevokeTokenRequestRequestTypeDef",
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
+    "AccountRecoverySettingTypeOutputTypeDef",
     "AccountRecoverySettingTypeTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
@@ -235,14 +238,15 @@
     "SetUICustomizationRequestRequestTypeDef",
     "LogConfigurationTypeTypeDef",
     "ForgotPasswordResponseTypeDef",
     "GetUserAttributeVerificationCodeResponseTypeDef",
     "ResendConfirmationCodeResponseTypeDef",
     "SignUpResponseTypeDef",
     "UpdateUserAttributesResponseTypeDef",
+    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     "ConfirmDeviceRequestRequestTypeDef",
     "ConfirmForgotPasswordRequestRequestTypeDef",
     "ConfirmSignUpRequestRequestTypeDef",
     "ForgotPasswordRequestRequestTypeDef",
     "InitiateAuthRequestRequestTypeDef",
     "ResendConfirmationCodeRequestRequestTypeDef",
@@ -271,29 +275,33 @@
     "GetUICustomizationResponseTypeDef",
     "SetUICustomizationResponseTypeDef",
     "LambdaConfigTypeTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "ListUserPoolClientsResponseTypeDef",
     "NotifyConfigurationTypeTypeDef",
     "UserPoolPolicyTypeTypeDef",
+    "RiskExceptionConfigurationTypeUnionTypeDef",
     "SchemaAttributeTypeTypeDef",
+    "UserAttributeUpdateSettingsTypeUnionTypeDef",
+    "AccountRecoverySettingTypeUnionTypeDef",
     "AdminGetDeviceResponseTypeDef",
     "AdminListDevicesResponseTypeDef",
     "GetDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "AdminCreateUserResponseTypeDef",
     "ListUsersInGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "AdminListUserAuthEventsResponseTypeDef",
     "AdminInitiateAuthResponseTypeDef",
     "AdminRespondToAuthChallengeResponseTypeDef",
     "InitiateAuthResponseTypeDef",
     "RespondToAuthChallengeResponseTypeDef",
     "LogDeliveryConfigurationTypeTypeDef",
     "SetLogDeliveryConfigurationRequestRequestTypeDef",
+    "CompromisedCredentialsRiskConfigurationTypeUnionTypeDef",
     "AdminInitiateAuthRequestRequestTypeDef",
     "AdminRespondToAuthChallengeRequestRequestTypeDef",
     "CreateResourceServerResponseTypeDef",
     "DescribeResourceServerResponseTypeDef",
     "ListResourceServersResponseTypeDef",
     "UpdateResourceServerResponseTypeDef",
     "CreateUserPoolClientResponseTypeDef",
@@ -1149,21 +1157,28 @@
     "RevokeTokenRequestRequestTypeDef",
     {
         "Token": str,
         "ClientId": str,
         "ClientSecret": NotRequired[str],
     },
 )
-RiskExceptionConfigurationTypeTypeDef = TypedDict(
-    "RiskExceptionConfigurationTypeTypeDef",
+RiskExceptionConfigurationTypeOutputTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     {
         "BlockedIPRangeList": NotRequired[List[str]],
         "SkippedIPRangeList": NotRequired[List[str]],
     },
 )
+RiskExceptionConfigurationTypeTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeTypeDef",
+    {
+        "BlockedIPRangeList": NotRequired[Sequence[str]],
+        "SkippedIPRangeList": NotRequired[Sequence[str]],
+    },
+)
 StringAttributeConstraintsTypeTypeDef = TypedDict(
     "StringAttributeConstraintsTypeTypeDef",
     {
         "MinLength": NotRequired[str],
         "MaxLength": NotRequired[str],
     },
 )
@@ -1229,14 +1244,20 @@
         "UserPoolId": str,
         "ProviderName": str,
         "ProviderDetails": NotRequired[Mapping[str, str]],
         "AttributeMapping": NotRequired[Mapping[str, str]],
         "IdpIdentifiers": NotRequired[Sequence[str]],
     },
 )
+UserAttributeUpdateSettingsTypeOutputTypeDef = TypedDict(
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
+    {
+        "AttributesRequireVerificationBeforeUpdate": NotRequired[List[VerifiedAttributeTypeType]],
+    },
+)
 VerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "VerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
         "AccessToken": NotRequired[str],
         "Session": NotRequired[str],
         "FriendlyDeviceName": NotRequired[str],
@@ -1246,14 +1267,20 @@
     "VerifyUserAttributeRequestRequestTypeDef",
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
     },
 )
+AccountRecoverySettingTypeOutputTypeDef = TypedDict(
+    "AccountRecoverySettingTypeOutputTypeDef",
+    {
+        "RecoveryMechanisms": NotRequired[List[RecoveryOptionTypeTypeDef]],
+    },
+)
 AccountRecoverySettingTypeTypeDef = TypedDict(
     "AccountRecoverySettingTypeTypeDef",
     {
         "RecoveryMechanisms": NotRequired[Sequence[RecoveryOptionTypeTypeDef]],
     },
 )
 AccountTakeoverActionsTypeTypeDef = TypedDict(
@@ -1513,16 +1540,16 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 AdminListGroupsForUserResponseTypeDef = TypedDict(
     "AdminListGroupsForUserResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1535,16 +1562,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateGroupResponseTypeDef = TypedDict(
     "UpdateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1641,19 +1668,26 @@
 UpdateUserAttributesResponseTypeDef = TypedDict(
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
+    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
+    {
+        "Actions": CompromisedCredentialsActionsTypeTypeDef,
+        "EventFilter": NotRequired[List[EventFilterTypeType]],
+    },
+)
 CompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
-        "EventFilter": NotRequired[List[EventFilterTypeType]],
+        "EventFilter": NotRequired[Sequence[EventFilterTypeType]],
     },
 )
 ConfirmDeviceRequestRequestTypeDef = TypedDict(
     "ConfirmDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
         "DeviceKey": str,
@@ -2000,24 +2034,24 @@
         "KMSKeyID": NotRequired[str],
     },
 )
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "Providers": List[ProviderDescriptionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUserPoolClientsResponseTypeDef = TypedDict(
     "ListUserPoolClientsResponseTypeDef",
     {
         "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 NotifyConfigurationTypeTypeDef = TypedDict(
     "NotifyConfigurationTypeTypeDef",
     {
         "SourceArn": str,
         "From": NotRequired[str],
@@ -2029,26 +2063,35 @@
 )
 UserPoolPolicyTypeTypeDef = TypedDict(
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": NotRequired[PasswordPolicyTypeTypeDef],
     },
 )
+RiskExceptionConfigurationTypeUnionTypeDef = Union[
+    RiskExceptionConfigurationTypeTypeDef, RiskExceptionConfigurationTypeOutputTypeDef
+]
 SchemaAttributeTypeTypeDef = TypedDict(
     "SchemaAttributeTypeTypeDef",
     {
         "Name": NotRequired[str],
         "AttributeDataType": NotRequired[AttributeDataTypeType],
         "DeveloperOnlyAttribute": NotRequired[bool],
         "Mutable": NotRequired[bool],
         "Required": NotRequired[bool],
         "NumberAttributeConstraints": NotRequired[NumberAttributeConstraintsTypeTypeDef],
         "StringAttributeConstraints": NotRequired[StringAttributeConstraintsTypeTypeDef],
     },
 )
+UserAttributeUpdateSettingsTypeUnionTypeDef = Union[
+    UserAttributeUpdateSettingsTypeTypeDef, UserAttributeUpdateSettingsTypeOutputTypeDef
+]
+AccountRecoverySettingTypeUnionTypeDef = Union[
+    AccountRecoverySettingTypeTypeDef, AccountRecoverySettingTypeOutputTypeDef
+]
 AdminGetDeviceResponseTypeDef = TypedDict(
     "AdminGetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2082,32 +2125,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListUsersInGroupResponseTypeDef = TypedDict(
     "ListUsersInGroupResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 AdminListUserAuthEventsResponseTypeDef = TypedDict(
     "AdminListUserAuthEventsResponseTypeDef",
     {
         "AuthEvents": List[AuthEventTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AdminInitiateAuthResponseTypeDef = TypedDict(
     "AdminInitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
@@ -2156,14 +2199,18 @@
 SetLogDeliveryConfigurationRequestRequestTypeDef = TypedDict(
     "SetLogDeliveryConfigurationRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "LogConfigurations": Sequence[LogConfigurationTypeTypeDef],
     },
 )
+CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = Union[
+    CompromisedCredentialsRiskConfigurationTypeTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
+]
 AdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "AdminInitiateAuthRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "AuthFlow": AuthFlowTypeType,
         "AuthParameters": NotRequired[Mapping[str, str]],
@@ -2199,16 +2246,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResourceServersResponseTypeDef = TypedDict(
     "ListResourceServersResponseTypeDef",
     {
         "ResourceServers": List[ResourceServerTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateResourceServerResponseTypeDef = TypedDict(
     "UpdateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2362,30 +2409,30 @@
         "AliasAttributes": NotRequired[List[AliasAttributeTypeType]],
         "UsernameAttributes": NotRequired[List[UsernameAttributeTypeType]],
         "SmsVerificationMessage": NotRequired[str],
         "EmailVerificationMessage": NotRequired[str],
         "EmailVerificationSubject": NotRequired[str],
         "VerificationMessageTemplate": NotRequired[VerificationMessageTemplateTypeTypeDef],
         "SmsAuthenticationMessage": NotRequired[str],
-        "UserAttributeUpdateSettings": NotRequired[UserAttributeUpdateSettingsTypeTypeDef],
+        "UserAttributeUpdateSettings": NotRequired[UserAttributeUpdateSettingsTypeOutputTypeDef],
         "MfaConfiguration": NotRequired[UserPoolMfaTypeType],
         "DeviceConfiguration": NotRequired[DeviceConfigurationTypeTypeDef],
         "EstimatedNumberOfUsers": NotRequired[int],
         "EmailConfiguration": NotRequired[EmailConfigurationTypeTypeDef],
         "SmsConfiguration": NotRequired[SmsConfigurationTypeTypeDef],
         "UserPoolTags": NotRequired[Dict[str, str]],
         "SmsConfigurationFailure": NotRequired[str],
         "EmailConfigurationFailure": NotRequired[str],
         "Domain": NotRequired[str],
         "CustomDomain": NotRequired[str],
         "AdminCreateUserConfig": NotRequired[AdminCreateUserConfigTypeTypeDef],
         "UserPoolAddOns": NotRequired[UserPoolAddOnsTypeTypeDef],
         "UsernameConfiguration": NotRequired[UsernameConfigurationTypeTypeDef],
         "Arn": NotRequired[str],
-        "AccountRecoverySetting": NotRequired[AccountRecoverySettingTypeTypeDef],
+        "AccountRecoverySetting": NotRequired[AccountRecoverySettingTypeOutputTypeDef],
     },
 )
 GetLogDeliveryConfigurationResponseTypeDef = TypedDict(
     "GetLogDeliveryConfigurationResponseTypeDef",
     {
         "LogDeliveryConfiguration": LogDeliveryConfigurationTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2398,30 +2445,30 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
         "UserPools": List[UserPoolDescriptionTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RiskConfigurationTypeTypeDef = TypedDict(
     "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": NotRequired[str],
         "ClientId": NotRequired[str],
         "CompromisedCredentialsRiskConfiguration": NotRequired[
-            CompromisedCredentialsRiskConfigurationTypeTypeDef
+            CompromisedCredentialsRiskConfigurationTypeOutputTypeDef
         ],
         "AccountTakeoverRiskConfiguration": NotRequired[
             AccountTakeoverRiskConfigurationTypeTypeDef
         ],
-        "RiskExceptionConfiguration": NotRequired[RiskExceptionConfigurationTypeTypeDef],
+        "RiskExceptionConfiguration": NotRequired[RiskExceptionConfigurationTypeOutputTypeDef],
         "LastModifiedDate": NotRequired[datetime],
     },
 )
 SetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "SetRiskConfigurationRequestRequestTypeDef",
     {
         "UserPoolId": str,
```

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp.egg-info/PKG-INFO` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.34.59
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.34.59 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.34.91 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-idp)](https://pepy.tech/project/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.34.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cognito-idp-1.34.59/mypy_boto3_cognito_idp.egg-info/SOURCES.txt` & `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.34.59/setup.py` & `mypy_boto3_cognito_idp-1.34.91/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-idp",
-    version="1.34.59",
+    version="1.34.91",
     packages=["mypy_boto3_cognito_idp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CognitoIdentityProvider 1.34.59 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.CognitoIdentityProvider 1.34.91 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

