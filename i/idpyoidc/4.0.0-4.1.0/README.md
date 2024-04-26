# Comparing `tmp/idpyoidc-4.0.0.tar.gz` & `tmp/idpyoidc-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idpyoidc-4.0.0.tar", last modified: Tue Feb 27 11:17:37 2024, max compression
+gzip compressed data, was "idpyoidc-4.1.0.tar", last modified: Fri Apr 26 07:12:29 2024, max compression
```

## Comparing `idpyoidc-4.0.0.tar` & `idpyoidc-4.1.0.tar`

### file list

```diff
@@ -1,304 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.336333 idpyoidc-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-02-27 11:17:37.336333 idpyoidc-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 11:17:37.336333 idpyoidc-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.284333 idpyoidc-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.292333 idpyoidc-4.0.0/src/idpyoidc/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/claims.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.296333 idpyoidc-4.0.0/src/idpyoidc/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.296333 idpyoidc-4.0.0/src/idpyoidc/client/claims/
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/claims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/claims/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/claims/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/claims/transform.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24429 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/client_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4303 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/configure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12100 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/current.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/entity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1884 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.300333 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11836 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.300333 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/dpop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/jar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/par.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/pkce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/status_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/client_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/refresh_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/resource_owner_password_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/server_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    27972 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/stand_alone_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/token_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/token_revocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oauth2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.304333 idpyoidc-4.0.0/src/idpyoidc/client/oidc/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6314 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.304333 idpyoidc-4.0.0/src/idpyoidc/client/oidc/add_on/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/backchannel_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/check_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/check_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/end_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/provider_info_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/read_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/refresh_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/userinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/oidc/webfinger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.304333 idpyoidc-4.0.0/src/idpyoidc/client/provider/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/provider/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/provider/linkedin.py
--rw-r--r--   0 runner    (1001) docker     (127)    22198 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/rp_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    26812 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/service_context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9673 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/client/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.304333 idpyoidc-4.0.0/src/idpyoidc/combo/
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/combo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/encrypter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/impexp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/item.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1166 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.304333 idpyoidc-4.0.0/src/idpyoidc/message/
--rw-r--r--   0 runner    (1001) docker     (127)    33129 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.304333 idpyoidc-4.0.0/src/idpyoidc/message/oauth2/
--rw-r--r--   0 runner    (1001) docker     (127)    21256 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/message/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/message/oauth2/device_authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.304333 idpyoidc-4.0.0/src/idpyoidc/message/oidc/
--rw-r--r--   0 runner    (1001) docker     (127)    41155 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/message/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/message/oidc/backchannel_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    26129 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/message/oidc/identity_assurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/message/oidc/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.308333 idpyoidc-4.0.0/src/idpyoidc/server/
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/authn_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.308333 idpyoidc-4.0.0/src/idpyoidc/server/authz/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4169 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/authz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.308333 idpyoidc-4.0.0/src/idpyoidc/server/claims/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/claims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/claims/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/claims/oidc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19393 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/client_authn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/client_configure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21940 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/construct.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10286 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/cookie_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17331 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16013 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/endpoint_context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1902 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/login_hint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.308333 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.308333 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/add_on/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/add_on/dpop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/add_on/extra_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/add_on/pkce.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    43994 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/pushed_authorization.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1135 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/server_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7452 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.312333 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7752 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/access_token.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2810 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/client_credentials.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5220 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/refresh_token.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3614 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/resource_owner_password_credentials.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12603 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/token_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_revocation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.312333 idpyoidc-4.0.0/src/idpyoidc/server/oidc/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.312333 idpyoidc-4.0.0/src/idpyoidc/server/oidc/add_on/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/backchannel_authentication.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1181 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/discovery.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/provider_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/read_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    19075 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    15766 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/session.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1634 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.312333 idpyoidc-4.0.0/src/idpyoidc/server/oidc/token_helper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/token_helper/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7994 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/token_helper/access_token.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6398 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/token_helper/refresh_token.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/token_helper/token_exchange.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8066 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/oidc/userinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.316333 idpyoidc-4.0.0/src/idpyoidc/server/session/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/session/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10511 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/session/claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/session/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    19743 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/session/grant.py
--rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/session/grant_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/session/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/session/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/session/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/template_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.316333 idpyoidc-4.0.0/src/idpyoidc/server/token/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4168 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/token/exception.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/token/handler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10788 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/token/id_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/token/jwt_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.316333 idpyoidc-4.0.0/src/idpyoidc/server/user_authn/
--rwxr-xr-x   0 runner    (1001) docker     (127)       30 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/user_authn/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5569 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/user_authn/authn_context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11459 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/user_authn/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.316333 idpyoidc-4.0.0/src/idpyoidc/server/user_info/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2342 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/user_info/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4308 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/server/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/ssl_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.316333 idpyoidc-4.0.0/src/idpyoidc/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8958 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/storage/abfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/storage/listfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/src/idpyoidc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.336333 idpyoidc-4.0.0/src/idpyoidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-02-27 11:17:37.000000 idpyoidc-4.0.0/src/idpyoidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-02-27 11:17:37.000000 idpyoidc-4.0.0/src/idpyoidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 11:17:37.000000 idpyoidc-4.0.0/src/idpyoidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 11:17:37.000000 idpyoidc-4.0.0/src/idpyoidc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-27 11:17:37.000000 idpyoidc-4.0.0/src/idpyoidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-27 11:17:37.000000 idpyoidc-4.0.0/src/idpyoidc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:37.336333 idpyoidc-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_01_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_03_time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    15230 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_04_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    23147 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_05_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)    55382 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_06_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_07_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    17299 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_08_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_09_work_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_11_impexp.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_12_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_13_dump_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_14_read_only_list_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_20_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_21_abfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_22_backchannel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_00_current.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_01_service_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_02_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_02b_entity_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_03_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_04_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_05_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    21248 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_06_client_authn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_10_entity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20925 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_12_client_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_14_service_context_impexp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_15_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_16_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_17_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_18_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_19_webfinger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_20_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)    49595 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_21_oidc_service.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8892 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_22_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_23_pkce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_24_oic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_25_oauth2_cc_ropc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_26_read_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21072 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_27_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)    20059 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_28_stand_alone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_29_pushed_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    40091 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_30_rp_handler_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_30_rph_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_31_oauth2_persistent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5123 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_32_oidc_persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_40_dpop.py
--rw-r--r--   0 runner    (1001) docker     (127)    23182 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_41_rp_handler_persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_50_ciba.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_51_identity_assurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_client_55_token_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_00_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_00a_client_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_01_claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_01_construct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_02_session_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_03_authz_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_04_session_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_05_token_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18567 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_06_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_07_sess_mngm_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    23484 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_08_id_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_09_authn_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    26484 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_10_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_11_session_manager_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_12_session_life.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_13_user_authn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_14_userinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_15_login_hint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9153 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_16_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_16_endpoint_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    26669 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_17_client_authn.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5420 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_20a_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_20b_claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_20c_authz_handling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25253 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_20d_client_authn.py
--rw-r--r--   0 runner    (1001) docker     (127)    21883 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_20e_jwt_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    18326 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_20f_userinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11436 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_20g_cookie_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2446 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_21_oidc_discovery_endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3832 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_22_oidc_provider_config_endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14767 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_23_oidc_registration_endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29343 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_24_oauth2_authorization_endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7926 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_24_oauth2_authorization_endpoint_jar.py
--rw-r--r--   0 runner    (1001) docker     (127)    24627 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_24_oauth2_resource_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)    39072 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_24_oauth2_token_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    36213 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_24_oauth2_token_endpoint_def_conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53909 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_24_oidc_authorization_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_25_oauth2_cc_ropc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25941 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_26_oidc_userinfo_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    26767 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_30_oidc_end_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    20030 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_31_oauth2_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_32_oidc_read_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_33_oauth2_pkce.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9850 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_34_oidc_sso.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    45206 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_35_oidc_token_endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    35257 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_35_oidc_token_endpoint_def_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    61177 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_36_oauth2_token_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)    22305 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_38_oauth2_revocation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_40_oauth2_pushed_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    21544 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_50_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_60_dpop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_server_61_add_on.py
--rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_tandem_oauth2_add_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_tandem_oauth2_cc_ropc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_tandem_oauth2_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    25343 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_tandem_oauth2_token_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_tandem_oauth2_token_revocation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_tandem_oidc_code.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:17:29.000000 idpyoidc-4.0.0/tests/test_y_actor_01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.034001 idpyoidc-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-26 07:12:29.034001 idpyoidc-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 07:12:29.034001 idpyoidc-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.978001 idpyoidc-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.986001 idpyoidc-4.1.0/src/idpyoidc/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/claims.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.990001 idpyoidc-4.1.0/src/idpyoidc/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.990001 idpyoidc-4.1.0/src/idpyoidc/client/claims/
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/claims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/claims/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/claims/oauth2resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/claims/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/claims/transform.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24348 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/client_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4303 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/configure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12100 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/entity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1884 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.994001 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11836 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.994001 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/dpop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/jar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/par.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/pkce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/status_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/client_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/refresh_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/resource_owner_password_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/server_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27972 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/stand_alone_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/token_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oauth2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.998001 idpyoidc-4.1.0/src/idpyoidc/client/oidc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6273 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.998001 idpyoidc-4.1.0/src/idpyoidc/client/oidc/add_on/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/backchannel_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/check_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/check_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/end_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/provider_info_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/refresh_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/oidc/webfinger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.998001 idpyoidc-4.1.0/src/idpyoidc/client/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/provider/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/provider/linkedin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22198 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/rp_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27192 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/service_context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9673 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/client/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.998001 idpyoidc-4.1.0/src/idpyoidc/combo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/combo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/impexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/item.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1166 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.998001 idpyoidc-4.1.0/src/idpyoidc/message/
+-rw-r--r--   0 runner    (1001) docker     (127)    33129 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.998001 idpyoidc-4.1.0/src/idpyoidc/message/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/message/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/message/oauth2/device_authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:28.998001 idpyoidc-4.1.0/src/idpyoidc/message/oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)    41155 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/message/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/message/oidc/backchannel_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26129 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/message/oidc/identity_assurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/message/oidc/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.002001 idpyoidc-4.1.0/src/idpyoidc/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/authn_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.002001 idpyoidc-4.1.0/src/idpyoidc/server/authz/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4149 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/authz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.002001 idpyoidc-4.1.0/src/idpyoidc/server/claims/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/claims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/claims/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/claims/oidc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19393 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/client_authn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/client_configure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21940 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/construct.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10286 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/cookie_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17331 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15971 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/endpoint_context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1902 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/login_hint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.006001 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.006001 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/add_on/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/add_on/dpop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/add_on/extra_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/add_on/pkce.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44130 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/pushed_authorization.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1135 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/server_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7452 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.006001 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7752 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/access_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2810 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/client_credentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5220 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/refresh_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3614 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/resource_owner_password_credentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12603 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_revocation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.006001 idpyoidc-4.1.0/src/idpyoidc/server/oidc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.006001 idpyoidc-4.1.0/src/idpyoidc/server/oidc/add_on/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/backchannel_authentication.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1181 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/discovery.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/provider_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19075 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15766 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1634 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.010001 idpyoidc-4.1.0/src/idpyoidc/server/oidc/token_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/token_helper/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7994 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/token_helper/access_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6398 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/token_helper/refresh_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/token_helper/token_exchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8188 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/oidc/userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.010001 idpyoidc-4.1.0/src/idpyoidc/server/session/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/session/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10504 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/session/claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/session/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19743 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/session/grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/session/grant_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/session/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/session/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/session/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/template_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.010001 idpyoidc-4.1.0/src/idpyoidc/server/token/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4168 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/token/exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/token/handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10788 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/token/id_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/token/jwt_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.010001 idpyoidc-4.1.0/src/idpyoidc/server/user_authn/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       30 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/user_authn/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5569 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/user_authn/authn_context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11459 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/user_authn/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.010001 idpyoidc-4.1.0/src/idpyoidc/server/user_info/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2342 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/user_info/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4308 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/server/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/ssl_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.014001 idpyoidc-4.1.0/src/idpyoidc/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8958 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/storage/abfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/storage/listfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/src/idpyoidc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.034001 idpyoidc-4.1.0/src/idpyoidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-26 07:12:28.000000 idpyoidc-4.1.0/src/idpyoidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-04-26 07:12:28.000000 idpyoidc-4.1.0/src/idpyoidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:12:28.000000 idpyoidc-4.1.0/src/idpyoidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:12:28.000000 idpyoidc-4.1.0/src/idpyoidc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-26 07:12:28.000000 idpyoidc-4.1.0/src/idpyoidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 07:12:28.000000 idpyoidc-4.1.0/src/idpyoidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:29.034001 idpyoidc-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_01_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_03_time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15230 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_04_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23147 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_05_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55382 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_06_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_07_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17299 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_08_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_09_work_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_11_impexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_12_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_13_dump_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_14_read_only_list_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_20_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_21_abfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_22_backchannel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_00_current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_01_service_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_02_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_02b_entity_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_03_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_04_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_05_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21248 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_06_client_authn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_10_entity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20925 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_12_client_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_14_service_context_impexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_15_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_16_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_17_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_18_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_19_webfinger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_20_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50444 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_21_oidc_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8922 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_22_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_23_pkce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_24_oic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_25_oauth2_cc_ropc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_26_read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21072 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_27_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20059 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_28_stand_alone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_29_pushed_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40757 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_30_rp_handler_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_30_rph_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_31_oauth2_persistent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5153 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_32_oidc_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_40_dpop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23182 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_41_rp_handler_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_50_ciba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_51_identity_assurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_client_55_token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_00_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_00a_client_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_01_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_01_construct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_02_session_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_03_authz_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_04_session_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_05_token_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18567 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_06_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_07_sess_mngm_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23484 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_08_id_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_09_authn_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26484 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_10_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_11_session_manager_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_12_session_life.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_13_user_authn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_14_userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_15_login_hint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9153 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_16_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_16_endpoint_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26669 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_17_client_authn.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5420 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_20a_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_20b_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_20c_authz_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25253 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_20d_client_authn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21883 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_20e_jwt_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18326 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_20f_userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11436 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_20g_cookie_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2446 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_21_oidc_discovery_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3832 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_22_oidc_provider_config_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14767 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_23_oidc_registration_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29343 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_24_oauth2_authorization_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7926 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_24_oauth2_authorization_endpoint_jar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24627 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_24_oauth2_resource_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39072 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_24_oauth2_token_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36213 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_24_oauth2_token_endpoint_def_conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53909 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_24_oidc_authorization_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_25_oauth2_cc_ropc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25941 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_26_oidc_userinfo_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26767 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_30_oidc_end_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20030 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_31_oauth2_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_32_oidc_read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_33_oauth2_pkce.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9850 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_34_oidc_sso.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45206 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_35_oidc_token_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35257 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_35_oidc_token_endpoint_def_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61177 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_36_oauth2_token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22305 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_38_oauth2_revocation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_40_oauth2_pushed_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21794 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_50_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_60_dpop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_server_61_add_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_tandem_oauth2_add_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_tandem_oauth2_cc_ropc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_tandem_oauth2_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25343 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_tandem_oauth2_token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_tandem_oauth2_token_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_tandem_oidc_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:12:21.000000 idpyoidc-4.1.0/tests/test_y_actor_01.py
```

### Comparing `idpyoidc-4.0.0/LICENSE` & `idpyoidc-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/PKG-INFO` & `idpyoidc-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idpyoidc
-Version: 4.0.0
+Version: 4.1.0
 Summary: Python implementation of everything OAuth2 and OpenID Connect
 Home-page: https://github.com/IdentityPython/idpy-oidc/
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `idpyoidc-4.0.0/README.md` & `idpyoidc-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/pyproject.toml` & `idpyoidc-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/setup.py` & `idpyoidc-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Roland Hedberg"
-__version__ = "4.0.0"
+__version__ = "4.1.0"
 
 VERIFIED_CLAIM_PREFIX = "__verified"
 
 
 def verified_claim_name(claim):
     return "{}_{}".format(VERIFIED_CLAIM_PREFIX, claim)
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/claims.py` & `idpyoidc-4.1.0/src/idpyoidc/claims.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/claims/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/client/claims/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/claims/oauth2.py` & `idpyoidc-4.1.0/src/idpyoidc/client/claims/oauth2.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/claims/oidc.py` & `idpyoidc-4.1.0/src/idpyoidc/client/claims/oidc.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/claims/transform.py` & `idpyoidc-4.1.0/src/idpyoidc/client/claims/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,24 @@
 ):
     if info:  # The provider info
         for key, val in supported.items():
             if key in preference:
                 _pref_val = preference.get(key)  # defined in configuration
                 _info_val = info.get(key)
                 if _info_val:
-                    # Only use provider setting if less or equal to what I support
-                    if key.endswith("supported"):  # list
-                        preference[key] = [x for x in _pref_val if x in _info_val]
+                    if isinstance(_info_val, bool):
+                        if _info_val is False and _pref_val is True:
+                            # Turn off support if server doesn't support
+                            preference[key] = _info_val
                     else:
-                        pass
+                        # Only use provider setting if less or equal to what I support
+                        if key.endswith("supported"):  # list
+                            preference[key] = [x for x in _pref_val if x in _info_val]
+                        else:
+                            pass
             elif val is None:  # No default, means the RP does not have a preference
                 # if key not in ['jwks_uri', 'jwks']:
                 pass
             else:
                 # there is a default
                 _info_val = info.get(key)
                 if _info_val:  # The OP has an opinion
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/client_auth.py` & `idpyoidc-4.1.0/src/idpyoidc/client/client_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -516,17 +516,15 @@
 
         if not algorithm:
             algorithm = self.choose_algorithm(**kwargs)
         return audience, algorithm
 
     def _construct_client_assertion(self, service, **kwargs):
         _context = service.upstream_get("context")
-        _entity = service.upstream_get("entity")
-        if _entity is None:
-            _entity = service.upstream_get("unit")
+        _entity = service.upstream_get("unit")
 
         _keyjar = service.upstream_get("attribute", "keyjar")
         audience, algorithm = self._get_audience_and_algorithm(_context, _keyjar, **kwargs)
 
         if "kid" in kwargs:
             signing_key = self._get_signing_key(
                 algorithm, _keyjar, _context.kid["sig"], kid=kwargs["kid"]
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/configure.py` & `idpyoidc-4.1.0/src/idpyoidc/client/configure.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/cookie.py` & `idpyoidc-4.1.0/src/idpyoidc/client/cookie.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/current.py` & `idpyoidc-4.1.0/src/idpyoidc/client/current.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/defaults.py` & `idpyoidc-4.1.0/src/idpyoidc/client/defaults.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/entity.py` & `idpyoidc-4.1.0/src/idpyoidc/client/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,14 @@
                 keyjar=self.keyjar,
                 upstream_get=self.unit_get,
                 client_type=client_type,
                 entity_id=self.entity_id,
             )
 
         self.setup_client_authn_methods(config)
-
         self.upstream_get = upstream_get
 
     def get_services(self, *arg):
         return self._service
 
     def get_service_context(self, *arg):  # Want to get rid of this
         return self.context
@@ -166,16 +165,16 @@
     def get_service_by_endpoint_name(self, endpoint_name, *arg):
         for service in self._service.values():
             if service.endpoint_name == endpoint_name:
                 return service
 
         return None
 
-    def get_entity(self):
-        return self
+    # def get_entity(self):
+    #     return self
 
     def get_client_id(self):
         _val = self.context.claims.get_usage("client_id")
         if _val:
             return _val
         else:
             return self.context.claims.get_preference("client_id")
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/exception.py` & `idpyoidc-4.1.0/src/idpyoidc/client/exception.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/http.py` & `idpyoidc-4.1.0/src/idpyoidc/client/http.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/access_token.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/access_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/dpop.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/dpop.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
 import uuid
 from hashlib import sha256
 from typing import Optional
 
 from cryptojwt.jwk.jwk import key_from_jwk_dict
-from cryptojwt.jws.jws import JWS
 from cryptojwt.jws.jws import factory
+from cryptojwt.jws.jws import JWS
 from cryptojwt.key_bundle import key_by_alg
 
+from idpyoidc.client.client_auth import BearerHeader
+from idpyoidc.client.client_auth import find_token_info
 from idpyoidc.client.service_context import ServiceContext
+from idpyoidc.message import Message
 from idpyoidc.message import SINGLE_OPTIONAL_STRING
 from idpyoidc.message import SINGLE_REQUIRED_INT
 from idpyoidc.message import SINGLE_REQUIRED_JSON
 from idpyoidc.message import SINGLE_REQUIRED_STRING
-from idpyoidc.message import Message
 from idpyoidc.metadata import get_signing_algs
 from idpyoidc.time_util import utc_time_sans_frac
 
 logger = logging.getLogger(__name__)
 
 
 class DPoPProof(Message):
@@ -87,21 +89,21 @@
 
             return self
         else:
             return None
 
 
 def dpop_header(
-    service_context: ServiceContext,
-    service_endpoint: str,
-    http_method: str,
-    headers: Optional[dict] = None,
-    token: Optional[str] = "",
-    nonce: Optional[str] = "",
-    **kwargs
+        service_context: ServiceContext,
+        service_endpoint: str,
+        http_method: str,
+        headers: Optional[dict] = None,
+        token: Optional[str] = "",
+        nonce: Optional[str] = "",
+        **kwargs
 ) -> dict:
     """
 
     :param service_context:
     :param service_endpoint:
     :param http_method:
     :param headers: The HTTP headers to which the DPoP header should be added.
@@ -155,15 +157,15 @@
         headers = {"dpop": jws}
     else:
         headers["dpop"] = jws
 
     return headers
 
 
-def add_support(services, dpop_signing_alg_values_supported):
+def add_support(services, dpop_signing_alg_values_supported, with_dpop_header=None):
     """
     Add the necessary pieces to make pushed authorization happen.
 
     :param services: A dictionary with all the services the client has access to.
     :param signing_algorithms: Allowed signing algorithms, there is no default algorithms
     """
 
@@ -181,7 +183,57 @@
 
     _service.construct_extra_headers.append(dpop_header)
 
     # The same for userinfo requests
     _userinfo_service = services.get("userinfo")
     if _userinfo_service:
         _userinfo_service.construct_extra_headers.append(dpop_header)
+    # To be backward compatible
+    if with_dpop_header is None:
+        with_dpop_header = ["userinfo"]
+
+    # Add dpop HTTP header to these
+    for _srv in with_dpop_header:
+        if _srv == "accesstoken":
+            continue
+        _service = services.get(_srv)
+        if _service:
+            _service.construct_extra_headers.append(dpop_header)
+
+
+class DPoPClientAuth(BearerHeader):
+    tag = "dpop_client_auth"
+
+    def construct(self, request=None, service=None, http_args=None, **kwargs):
+        """
+        Constructing the Authorization header. The value of
+        the Authorization header is "Bearer <access_token>".
+
+        :param request: Request class instance
+        :param service: The service this authentication method applies to.
+        :param http_args: HTTP header arguments
+        :param kwargs: extra keyword arguments
+        :return:
+        """
+
+        _token_type = "access_token"
+
+        _token_info = find_token_info(request, _token_type, service, **kwargs)
+
+        if not _token_info:
+            raise KeyError("No bearer token available")
+
+        # The authorization value starts with the token_type
+        # if _token_info["token_type"].to_lower() != "bearer":
+        _bearer = f"DPoP {_token_info[_token_type]}"
+
+        # Add 'Authorization' to the headers
+        if http_args is None:
+            http_args = {"headers": {}}
+            http_args["headers"]["Authorization"] = _bearer
+        else:
+            try:
+                http_args["headers"]["Authorization"] = _bearer
+            except KeyError:
+                http_args["headers"] = {"Authorization": _bearer}
+
+        return http_args
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/jar.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/jar.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/par.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/par.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,17 @@
         else:
             _name = ""
             for _name, spec in authn_method.items():
                 if _name not in _context.client_authn_methods:
                     _context.client_authn_methods[_name] = execute(spec)
             authn_method = _name
 
-        _args = {}
+        _args = kwargs.copy()
         if _context.issuer:
             _args["iss"] = _context.issuer
-        if _name == "client_attestation":
-            _wia = kwargs.get("client_attestation")
-            if _wia:
-                _args["client_attestation"] = _wia
 
         _headers = service.get_headers(
             request_args, http_method=_http_method, authn_method=authn_method, **_args
         )
         _headers["Content-Type"] = "application/x-www-form-urlencoded"
 
     # construct the message body
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/pkce.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/pkce.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/add_on/status_check.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/add_on/status_check.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/authorization.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/authorization.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/client_credentials.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/client_credentials.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/introspection.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/introspection.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/refresh_access_token.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/refresh_access_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/registration.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/registration.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/resource_owner_password_credentials.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/resource_owner_password_credentials.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/server_metadata.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/server_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def get_endpoint(self):
         """
         Find the issuer ID and from it construct the service endpoint
 
         :return: Service endpoint
         """
         try:
-            _iss = self.upstream_get("context").issuer
+            _iss = self.upstream_get("attribute","issuer")
         except AttributeError:
             _iss = self.endpoint
 
         if _iss.endswith("/"):
             return self.url_pattern.format(_iss[:-1])
 
         return self.url_pattern.format(_iss)
@@ -68,21 +68,24 @@
             if issuer.endswith("/"):
                 _issuer = issuer[:-1]
             else:
                 _issuer = issuer
 
         # In some cases we can live with the two URLs not being
         # the same. But this is an excepted that has to be explicit
-        try:
-            self.upstream_get("context").allow["issuer_mismatch"]
-        except KeyError:
-            if _issuer != _pcr_issuer:
-                raise OidcServiceError(
-                    "provider info issuer mismatch '%s' != '%s'" % (_issuer, _pcr_issuer)
-                )
+        _allow = self.upstream_get("attribute", "allow")
+        if _allow:
+            _allowed = _allow.get("issuer_mismatch", None)
+            if _allowed:
+                return _issuer
+
+        if _issuer != _pcr_issuer:
+            raise OidcServiceError(
+                "provider info issuer mismatch '%s' != '%s'" % (_issuer, _pcr_issuer)
+            )
         return _issuer
 
     def _set_endpoints(self, resp):
         """
         If there are services defined set the service endpoint to be
         the URLs specified in the provider information."""
         for key, val in resp.items():
@@ -127,17 +130,18 @@
             _keyjar = KeyJar()
 
         _loaded = False
         # Load the keys. Note that this only means that the key specification
         # is loaded not necessarily that any keys are fetched.
         if "jwks_uri" in resp:
             LOGGER.debug(f"'jwks_uri' in provider info: {resp['jwks_uri']}")
-            _hp = self.upstream_get('entity').httpc_params
-            if "verify" in _hp and "verify" not in _keyjar.httpc_params:
-                _keyjar.httpc_params["verify"] = _hp["verify"]
+            _hp = self.upstream_get("attribute","httpc_params")
+            if _hp:
+                if "verify" in _hp and "verify" not in _keyjar.httpc_params:
+                    _keyjar.httpc_params["verify"] = _hp["verify"]
             _keyjar.load_keys(_pcr_issuer, jwks_uri=resp["jwks_uri"])
             _loaded = True
         elif "jwks" in resp:
             LOGGER.debug("'jwks' in provider info")
             _keyjar.load_keys(_pcr_issuer, jwks=resp["jwks"])
             _loaded = True
         else:
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/stand_alone_client.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/stand_alone_client.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/token_exchange.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/token_exchange.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/token_revocation.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/token_revocation.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oauth2/utils.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oauth2/utils.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,14 @@
         upstream_get: Optional[Callable] = None,
         key_conf: Optional[dict] = None,
         entity_id: Optional[str] = "",
         verify_ssl: Optional[bool] = True,
         jwks_uri: Optional[str] = "",
         **kwargs
     ):
-        self.upstream_get = upstream_get
         if services:
             _srvs = services
         else:
             _srvs = config.get("services", DEFAULT_OIDC_SERVICES)
 
         oauth2.Client.__init__(
             self,
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/access_token.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/access_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     ):
         """
         Need to add some information before running verify()
 
         :return: dictionary with arguments to the verify call
         """
         _context = self.upstream_get("context")
-        _entity = self.upstream_get("entity")
+        _entity = self.upstream_get("unit")
 
         kwargs = {
             "client_id": _entity.get_client_id(),
             "iss": _context.issuer,
             "keyjar": self.upstream_get("attribute", "keyjar"),
             "verify": True,
             "skew": _context.clock_skew,
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/authorization.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         _context = self.upstream_get("context")
 
         if "expires_in" in resp:
             resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
         _context.cstate.update(key, resp)
 
     def get_request_from_response(self, response):
-        _context = self.upstream_get("service_context")
+        _context = self.upstream_get("context")
         return _context.cstate.get_set(response["state"], message=oauth2.AuthorizationRequest)
 
     def post_parse_response(self, response, **kwargs):
         response = authorization.Authorization.post_parse_response(self, response, **kwargs)
 
         _idt = response.get(verified_claim_name("id_token"))
         if _idt:
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/backchannel_authentication.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/backchannel_authentication.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/check_id.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/check_id.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/check_session.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/check_session.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/end_session.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/end_session.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/provider_info_discovery.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/provider_info_discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Add redirect_uris to the request arguments.
 
     :param request_args: Incoming request arguments
     :param service: A link to the service
     :param kwargs: Possible extra keyword arguments
     :return: A possibly augmented set of request arguments.
     """
-    _work_environment = service.upstream_get("context").claims
+    _work_environment = service.upstream_get("attribute", "claims")
     if "redirect_uris" not in request_args:
         # Callbacks is a dictionary with callback type 'code', 'implicit',
         # 'form_post' as keys.
         _callback = _work_environment.get_preference("callback")
         if _callback:
             # Filter out local additions.
             _uris = [v for k, v in _callback.items() if not k.startswith("__")]
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/read_registration.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/read_registration.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/refresh_access_token.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/refresh_access_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/registration.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/registration.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/userinfo.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/userinfo.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/utils.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/utils.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/oidc/webfinger.py` & `idpyoidc-4.1.0/src/idpyoidc/client/oidc/webfinger.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/provider/github.py` & `idpyoidc-4.1.0/src/idpyoidc/client/provider/github.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/provider/linkedin.py` & `idpyoidc-4.1.0/src/idpyoidc/client/provider/linkedin.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/rp_handler.py` & `idpyoidc-4.1.0/src/idpyoidc/client/rp_handler.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/service.py` & `idpyoidc-4.1.0/src/idpyoidc/client/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,17 +258,24 @@
             if "state" not in request_args:
                 request_args["state"] = kwargs["state"]
 
         # logger.debug("request_args: %s" % sanitize(request_args))
         _args = self.gather_request_args(**request_args)
 
         # logger.debug("kwargs: %s" % sanitize(kwargs))
+
+        # we must check if claims module is idpyoidc.client.claims.oauth2recource as
+        # in that case we don't want to set_defaults like application_type etc.
+        obj = self.upstream_get("context").claims
         # initiate the request as in an instance of the self.msg_type
         # message type
-        request = self.msg_type(**_args)
+        if(obj.__class__.__module__ == "idpyoidc.client.claims.oauth2resource"):
+            request = self.msg_type(**_args, set_defaults=False)
+        else:
+            request = self.msg_type(**_args)
 
         _behaviour_args = kwargs.get("behaviour_args")
         if _behaviour_args:
             post_args.update(_behaviour_args)
 
         return self.do_post_construct(request, **post_args)
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/service_context.py` & `idpyoidc-4.1.0/src/idpyoidc/client/service_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from cryptojwt.key_jar import KeyJar
 from cryptojwt.utils import as_bytes
 
 from idpyoidc.claims import Claims
 from idpyoidc.claims import claims_dump
 from idpyoidc.claims import claims_load
 from idpyoidc.client.claims.oauth2 import Claims as OAUTH2_Specs
+from idpyoidc.client.claims.oauth2resource import Claims as OAUTH2RESOURCE_Specs
 from idpyoidc.client.claims.oidc import Claims as OIDC_Specs
 from idpyoidc.client.configure import Configuration
 from idpyoidc.util import rndstr
 
 from ..impexp import ImpExp
 from .claims.transform import preferred_to_registered
 from .claims.transform import supported_to_preferred
@@ -129,14 +130,16 @@
         self.config = config
         self.upstream_get = upstream_get
 
         if not client_type or client_type == "oidc":
             self.claims = OIDC_Specs()
         elif client_type == "oauth2":
             self.claims = OAUTH2_Specs()
+        elif client_type == "oauth2resource":
+            self.claims = OAUTH2RESOURCE_Specs()
         else:
             raise ValueError(f"Unknown client type: {client_type}")
 
         self.entity_id = kwargs.get("entity_id", kwargs.get("client_id", ""))
         if not self.entity_id:
             self.entity_id = config.conf.get("entity_id", config.conf.get("client_id"))
 
@@ -152,14 +155,15 @@
         self.args = {}
         self.add_on = {}
         self.iss_hash = ""
         self.issuer = ""
         self.httpc_params = {}
         self.client_secret_expires_at = 0
         self.registration_response = {}
+        self.client_authn_methods = {}
 
         # _def_value = copy.deepcopy(DEFAULT_VALUE)
 
         _issuer = config.get("issuer")
         if _issuer:
             self.issuer = _issuer
         else:
@@ -182,14 +186,17 @@
 
         _response_types = self.get_preference(
             "response_types_supported", self.supports().get("response_types_supported", [])
         )
 
         self.construct_uris(response_types=_response_types)
 
+        self.map_supported_to_preferred()
+        self.map_preferred_to_registered()
+
     def __setitem__(self, key, value):
         setattr(self, key, value)
 
     def filename_from_webname(self, webname):
         """
         A 1<->1 map is maintained between a URL pointing to a file and
         the name of the file in the file system.
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/client/util.py` & `idpyoidc-4.1.0/src/idpyoidc/client/util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/combo/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/combo/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/configure.py` & `idpyoidc-4.1.0/src/idpyoidc/configure.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/context.py` & `idpyoidc-4.1.0/src/idpyoidc/context.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/converter.py` & `idpyoidc-4.1.0/src/idpyoidc/converter.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/encrypter.py` & `idpyoidc-4.1.0/src/idpyoidc/encrypter.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/exception.py` & `idpyoidc-4.1.0/src/idpyoidc/exception.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/impexp.py` & `idpyoidc-4.1.0/src/idpyoidc/impexp.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/item.py` & `idpyoidc-4.1.0/src/idpyoidc/item.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/logging.py` & `idpyoidc-4.1.0/src/idpyoidc/logging.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/message/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/message/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/message/oauth2/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/message/oauth2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -632,14 +632,30 @@
     """
     Error response from the revocation endpoint
     """
 
     c_allowed_values = ResponseMessage.c_allowed_values.copy()
     c_allowed_values.update({"error": ["unsupported_token_type"]})
 
+class OAuthProtectedResourceRequest(Message):
+    c_param = {
+        "resource": SINGLE_REQUIRED_STRING,
+        "authorization_servers": OPTIONAL_LIST_OF_STRINGS,
+        "jwks_uri": SINGLE_OPTIONAL_STRING,
+        "resource_documentation": SINGLE_OPTIONAL_STRING,
+        "scopes_supported": OPTIONAL_LIST_OF_STRINGS,
+        "bearer_methods_supported": OPTIONAL_LIST_OF_STRINGS,
+        "resource_signing_alg_values_supported": OPTIONAL_LIST_OF_STRINGS,
+        "resource_encryption_alg_values_supported": OPTIONAL_LIST_OF_STRINGS,
+        "resource_encryption_enc_values_supported": OPTIONAL_LIST_OF_STRINGS,
+        "client_registration_types": OPTIONAL_LIST_OF_STRINGS,
+        "organization_name": SINGLE_OPTIONAL_STRING,
+        "resource_policy_uri": SINGLE_OPTIONAL_STRING,
+        "resource_tos_uri": SINGLE_OPTIONAL_STRING
+    }
 
 def factory(msgtype, **kwargs):
     """
     Factory method that can be used to easily instansiate a class instance
 
     :param msgtype: The name of the class
     :param kwargs: Keyword arguments
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/message/oauth2/device_authorization.py` & `idpyoidc-4.1.0/src/idpyoidc/message/oauth2/device_authorization.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/message/oidc/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/message/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/message/oidc/backchannel_authentication.py` & `idpyoidc-4.1.0/src/idpyoidc/message/oidc/backchannel_authentication.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/message/oidc/identity_assurance.py` & `idpyoidc-4.1.0/src/idpyoidc/message/oidc/identity_assurance.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/message/oidc/session.py` & `idpyoidc-4.1.0/src/idpyoidc/message/oidc/session.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/metadata.py` & `idpyoidc-4.1.0/src/idpyoidc/metadata.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/node.py` & `idpyoidc-4.1.0/src/idpyoidc/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,17 +177,17 @@
     def get_unit(self, *args):
         return self
 
 
 def topmost_unit(unit):
     if hasattr(unit, "upstream_get"):
         if unit.upstream_get:
-            next_unit = unit.upstream_get("unit")
-            if next_unit:
-                unit = topmost_unit(next_unit)
+            superior = unit.upstream_get("unit")
+            if superior:
+                unit = topmost_unit(superior)
 
     return unit
 
 
 class ClientUnit(Unit):
     name = ""
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/server/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             httpc=httpc,
             upstream_get=upstream_get,
             httpc_params=httpc_params,
             key_conf=key_conf,
             issuer_id=self.issuer,
         )
 
-        self.upstream_get = upstream_get
         if isinstance(conf, OPConfiguration) or isinstance(conf, ASConfiguration):
             self.conf = conf
         else:
             self.conf = OPConfiguration(conf)
 
         self.endpoint = do_endpoints(self.conf, self.unit_get)
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/authn_event.py` & `idpyoidc-4.1.0/src/idpyoidc/server/authn_event.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/authz/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/server/authz/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         if not scopes:
             scopes = request.get("scope", [])
         else:
             scopes = _context.scopes_handler.filter_scopes(scopes, client_id=_client_id)
         grant.scope = scopes
 
         # After this is where user consent should be handled
-        grant.claims = self.upstream_get("context").claims_interface.get_claims_all_usage(
+        grant.claims = _context.claims_interface.get_claims_all_usage(
             session_id=session_id, scopes=scopes
         )
 
         return grant
 
 
 class Implicit(AuthzHandling):
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/claims/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/server/claims/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/claims/oauth2.py` & `idpyoidc-4.1.0/src/idpyoidc/server/claims/oauth2.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/claims/oidc.py` & `idpyoidc-4.1.0/src/idpyoidc/server/claims/oidc.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/client_authn.py` & `idpyoidc-4.1.0/src/idpyoidc/server/client_authn.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/client_configure.py` & `idpyoidc-4.1.0/src/idpyoidc/server/client_configure.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/configure.py` & `idpyoidc-4.1.0/src/idpyoidc/server/configure.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/construct.py` & `idpyoidc-4.1.0/src/idpyoidc/server/construct.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/cookie_handler.py` & `idpyoidc-4.1.0/src/idpyoidc/server/cookie_handler.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/endpoint.py` & `idpyoidc-4.1.0/src/idpyoidc/server/endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/endpoint_context.py` & `idpyoidc-4.1.0/src/idpyoidc/server/endpoint_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         else:  # Backward compatibility
             self.httpc_params = {"verify": conf.get("verify_ssl", True)}
 
         self.set_scopes_handler()
         self.dev_auth_db = None
         _interface = conf.get("claims_interface")
         if _interface:
-            self.claims_interface = init_service(_interface, self.upstream_get)
+            self.claims_interface = init_service(_interface, self.unit_get)
 
         if isinstance(conf, OPConfiguration):
             conf = conf.conf
         _supports = self.supports()
         self.keyjar = self.claims.load_conf(conf, supports=_supports, keyjar=keyjar)
         self.provider_info = self.claims.provider_info(_supports)
         self.provider_info["issuer"] = self.issuer
@@ -272,17 +272,15 @@
         authz_spec = self.conf.get("authz")
         if authz_spec:
             return init_service(authz_spec, self.unit_get)
         else:
             return authz.Implicit(self.unit_get)
 
     def setup_client_authn_methods(self):
-        self.client_authn_methods = client_auth_setup(
-            self.upstream_get, self.conf.get("client_authn_methods")
-        )
+        self.client_authn_methods = client_auth_setup(self.unit_get, self.conf.get("client_authn_methods"))
 
     def setup_login_hint_lookup(self):
         _conf = self.conf.get("login_hint_lookup")
         if _conf:
             _userinfo = None
             _kwargs = _conf.get("kwargs")
             if _kwargs:
@@ -303,18 +301,18 @@
         return cookie_cont
 
     def set_scopes_handler(self):
         _spec = self.conf.get("scopes_handler")
         if _spec:
             _kwargs = _spec.get("kwargs", {})
             _cls = importer(_spec["class"])
-            self.scopes_handler = _cls(self.upstream_get, **_kwargs)
+            self.scopes_handler = _cls(self.unit_get, **_kwargs)
         else:
             self.scopes_handler = Scopes(
-                self.upstream_get,
+                self.unit_get,
                 allowed_scopes=self.conf.get("allowed_scopes"),
                 scopes_to_claims=self.conf.get("scopes_to_claims"),
             )
 
     def do_add_on(self, endpoints):
         _add_on_conf = self.conf.get("add_ons", self.conf.get("add_on"))
         if not _add_on_conf:
@@ -436,15 +434,15 @@
     def set_usage(self, claim, value):
         return self.claims.set_usage(claim, value)
 
     def setup_authentication(self):
         _conf = self.conf.get("authentication")
         if _conf:
             self.authn_broker = populate_authn_broker(
-                _conf, self.upstream_get, self.template_handler
+                _conf, self.unit_get, self.template_handler
             )
         else:
             self.authn_broker = {}
 
         self.endpoint_to_authn_method = {}
         for method in self.authn_broker:
             try:
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/exception.py` & `idpyoidc-4.1.0/src/idpyoidc/server/exception.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/login_hint.py` & `idpyoidc-4.1.0/src/idpyoidc/server/login_hint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/add_on/dpop.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/add_on/dpop.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/add_on/extra_args.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/add_on/extra_args.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/add_on/pkce.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/add_on/pkce.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/authorization.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/authorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from cryptojwt import as_unicode
 from cryptojwt import b64d
 from cryptojwt.jwe.exception import JWEException
 from cryptojwt.jws.exception import NoSuitableSigningKeys
 from cryptojwt.utils import as_bytes
 from cryptojwt.utils import b64e
 
-from idpyoidc import claims
 from idpyoidc import metadata
 from idpyoidc.exception import ImproperlyConfigured
 from idpyoidc.exception import ParameterError
 from idpyoidc.exception import URIError
 from idpyoidc.message import Message
 from idpyoidc.message import oauth2
 from idpyoidc.message.oauth2 import AuthorizationRequest
@@ -89,19 +88,19 @@
 
 def max_age(request):
     verified_request = verified_claim_name("request")
     return request.get(verified_request, {}).get("max_age") or request.get("max_age", 0)
 
 
 def verify_uri(
-    context: EndpointContext,
-    request: Union[dict, Message],
-    uri_type: str,
-    client_id: Optional[str] = None,
-    endpoint_type: Optional[str] = 'oidc'
+        context: EndpointContext,
+        request: Union[dict, Message],
+        uri_type: str,
+        client_id: Optional[str] = None,
+        endpoint_type: Optional[str] = 'oidc'
 ):
     """
     A redirect URI
     MUST NOT contain a fragment
     MAY contain query component
 
     :param context: An EndpointContext instance
@@ -206,15 +205,15 @@
     :param request: The Authorization request
     :param uri_type: 'redirect_uri' or 'post_logout_redirect_uri'
     :return: redirect_uri
     """
     uri = ""
 
     if uri_type in request:
-        verify_uri(context, request, uri_type,endpoint_type=endpoint_type)
+        verify_uri(context, request, uri_type, endpoint_type=endpoint_type)
         uri = request[uri_type]
     else:
         uris = f"{uri_type}s"
         client_id = str(request["client_id"])
         if client_id in context.cdb:
             _specs = context.cdb[client_id].get(uris)
             if not _specs:
@@ -227,18 +226,18 @@
         else:
             raise UnknownClient(client_id)
 
     return uri
 
 
 def authn_args_gather(
-    request: Union[AuthorizationRequest, dict],
-    authn_class_ref: str,
-    cinfo: dict,
-    **kwargs,
+        request: Union[AuthorizationRequest, dict],
+        authn_class_ref: str,
+        cinfo: dict,
+        **kwargs,
 ):
     """
     Gather information to be used by the authentication method
 
     :param request: The request either as a dictionary or as a Message instance
     :param authn_class_ref: Authentication class reference
     :param cinfo: Client information
@@ -294,16 +293,16 @@
     if "resource" not in request:
         return request
 
     resource_servers_per_client = kwargs["resource_servers_per_client"]
     client_id = request["client_id"]
 
     if (
-        isinstance(resource_servers_per_client, dict)
-        and client_id not in resource_servers_per_client
+            isinstance(resource_servers_per_client, dict)
+            and client_id not in resource_servers_per_client
     ):
         return oauth2.AuthorizationErrorResponse(
             error="invalid_target",
             error_description=f"Resources for client {client_id} not found",
         )
 
     if isinstance(resource_servers_per_client, dict):
@@ -371,15 +370,15 @@
         self.post_parse_request.append(self._post_parse_request)
         self.allowed_request_algorithms = AllowedAlgorithms(ALG_PARAMS)
         self.resource_indicators_config = kwargs.get("resource_indicators", None)
 
     def filter_request(self, context, req):
         return req
 
-    def extra_response_args(self, aresp):
+    def extra_response_args(self, aresp, **kwargs):
         return aresp
 
     def authentication_error_response(self, request, error, error_description, **kwargs):
         _error_msg = self.error_cls(error=error, error_description=error_description)
         _state = request.get("state")
         if _state:
             _error_msg["state"] = _state
@@ -522,16 +521,16 @@
                 error="invalid_request",
                 error_description="{}:{}".format(err.__class__.__name__, err),
             )
         else:
             request["redirect_uri"] = redirect_uri
 
         if (
-            "resource_indicators" in _cinfo
-            and "authorization_code" in _cinfo["resource_indicators"]
+                "resource_indicators" in _cinfo
+                and "authorization_code" in _cinfo["resource_indicators"]
         ):
             resource_indicators_config = _cinfo["resource_indicators"]["authorization_code"]
         else:
             resource_indicators_config = self.resource_indicators_config
 
         if resource_indicators_config is not None:
             if "policy" not in resource_indicators_config:
@@ -638,21 +637,21 @@
 
         try:
             return json.loads(as_unicode(_id))
         except UnicodeDecodeError:
             return identity
 
     def setup_auth(
-        self,
-        request: Optional[Union[Message, dict]],
-        redirect_uri: str,
-        cinfo: dict,
-        cookie: List[dict] = None,
-        acr: str = None,
-        **kwargs,
+            self,
+            request: Optional[Union[Message, dict]],
+            redirect_uri: str,
+            cinfo: dict,
+            cookie: List[dict] = None,
+            acr: str = None,
+            **kwargs,
     ) -> dict:
         """
 
         :param request: The authorization/authentication request
         :param redirect_uri:
         :param cinfo: client info
         :param cookie: List of cookies
@@ -768,20 +767,20 @@
 
         return {"session_id": _session_id, "identity": identity, "user": user}
 
     def aresp_check(self, aresp, request):
         return ""
 
     def response_mode(
-        self,
-        request: Union[dict, AuthorizationRequest],
-        response_args: Optional[Union[dict, AuthorizationResponse]] = None,
-        return_uri: Optional[str] = "",
-        fragment_enc: Optional[bool] = None,
-        **kwargs,
+            self,
+            request: Union[dict, AuthorizationRequest],
+            response_args: Optional[Union[dict, AuthorizationResponse]] = None,
+            return_uri: Optional[str] = "",
+            fragment_enc: Optional[bool] = None,
+            **kwargs,
     ) -> dict:
         resp_mode = request["response_mode"]
         if resp_mode == "form_post":
             if isinstance(response_args, AuthorizationRequest):
                 _args = response_args.to_dict()
             else:
                 _args = response_args
@@ -939,15 +938,15 @@
                 resp = self.authentication_error_response(
                     request,
                     error="invalid_request",
                     error_description="unsupported_response_type",
                 )
                 return {"response_args": resp, "fragment_enc": fragment_enc}
 
-        aresp = self.extra_response_args(aresp)
+        aresp = self.extra_response_args(aresp, client_id=request["client_id"])
 
         return {"response_args": aresp, "fragment_enc": fragment_enc}
 
     def post_authentication(self, request: Union[dict, Message], session_id: str, **kwargs) -> dict:
         """
         Things that are done after a successful authentication.
 
@@ -1083,18 +1082,18 @@
 
         return resp_info
 
     def do_request_user(self, request_info, **kwargs):
         return kwargs
 
     def process_request(
-        self,
-        request: Optional[Union[Message, dict]] = None,
-        http_info: Optional[dict] = None,
-        **kwargs,
+            self,
+            request: Optional[Union[Message, dict]] = None,
+            http_info: Optional[dict] = None,
+            **kwargs,
     ):
         """The AuthorizationRequest endpoint
 
         :param http_info: Information on the HTTP request
         :param request: The authorization request as a Message instance
         :return: dictionary
         """
@@ -1149,14 +1148,15 @@
             }
         except Exception as err:
             logger.exception(err)
             return {"http_response": "Internal error: {}".format(err)}
 
 
 class AllowedAlgorithms:
+
     def __init__(self, algorithm_parameters):
         self.algorithm_parameters = algorithm_parameters
 
     def __call__(self, client_id, context, alg, alg_type):
         _cinfo = context.cdb[client_id]
         _pinfo = context.provider_info
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/introspection.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/introspection.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/pushed_authorization.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/pushed_authorization.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/server_metadata.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/server_metadata.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/access_token.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/access_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/client_credentials.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/client_credentials.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/refresh_token.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/refresh_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/resource_owner_password_credentials.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/resource_owner_password_credentials.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_helper/token_exchange.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_helper/token_exchange.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oauth2/token_revocation.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oauth2/token_revocation.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/authorization.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/authorization.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/backchannel_authentication.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/backchannel_authentication.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/discovery.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/discovery.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/provider_config.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/provider_config.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/read_registration.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/read_registration.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/registration.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/registration.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/session.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/session.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/token.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/token_helper/access_token.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/token_helper/access_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/token_helper/refresh_token.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/token_helper/refresh_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/oidc/userinfo.py` & `idpyoidc-4.1.0/src/idpyoidc/server/oidc/userinfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,26 +147,30 @@
             )
             allowed = False
 
             # This has to be made more finegrained.
             # if "offline_access" in session["authn_req"]["scope"]:
             #     pass
 
+        _cntxt = self.upstream_get("context")
         if allowed:
-            _cntxt = self.upstream_get("context")
             _claims_restriction = _cntxt.claims_interface.get_claims(
                 _session_info["branch_id"], scopes=token.scope, claims_release_point="userinfo"
             )
             info = _cntxt.claims_interface.get_user_claims(
                 _session_info["user_id"], claims_restriction=_claims_restriction
             )
             info["sub"] = _grant.sub
             if _grant.add_acr_value("userinfo"):
                 info["acr"] = _grant.authentication_event["authn_info"]
 
+            extra_claims = kwargs.get("extra_claims")
+            if extra_claims:
+                info.update(extra_claims)
+
         if "userinfo" in _cntxt.cdb[request["client_id"]]:
             self.config["policy"] = _cntxt.cdb[request["client_id"]]["userinfo"]["policy"]
 
         if "policy" in self.config:
             info = self._enforce_policy(request, info, token, self.config)
 
         return {"response_args": info, "client_id": _session_info["client_id"]}
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/scopes.py` & `idpyoidc-4.1.0/src/idpyoidc/server/scopes.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             except KeyError:
                 continue
 
     return res
 
 
 class Scopes:
+
     def __init__(self, upstream_get, allowed_scopes=None, scopes_to_claims=None):
         self.upstream_get = upstream_get
         if not scopes_to_claims:
             scopes_to_claims = dict(SCOPE2CLAIMS)
         self._scopes_to_claims = scopes_to_claims
         self.allowed_scopes = list(scopes_to_claims.keys())
 
@@ -59,29 +60,29 @@
         Returns the set of scopes that a specific client can use.
 
         :param client_id: The client identifier
         :returns: List of scope names. Can be empty.
         """
         allowed_scopes = self.allowed_scopes
         if client_id:
-            client = self.upstream_get("context").cdb.get(client_id)
+            client = self.upstream_get("attribute", "cdb").get(client_id)
             if client is not None:
                 allowed_scopes = client.get("allowed_scopes", allowed_scopes)
         return allowed_scopes
 
     def get_scopes_mapping(self, client_id=None):
         """
-        Returns the mapping of scopes to claims fora specific client.
+        Returns the mapping of scopes to claims for a specific client.
 
         :param client_id: The client identifier
         :returns: Dict of scopes to claims. Can be empty.
         """
         scopes_to_claims = self._scopes_to_claims
         if client_id:
-            client = self.upstream_get("context").cdb.get(client_id)
+            client = self.upstream_get("attribute", "cdb").get(client_id)
             if client is not None:
                 scopes_to_claims = client.get("scopes_to_claims", scopes_to_claims)
         return scopes_to_claims
 
     def filter_scopes(self, scopes, client_id=None):
         allowed_scopes = self.get_allowed_scopes(client_id)
         return [s for s in scopes if s in allowed_scopes]
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/session/claims.py` & `idpyoidc-4.1.0/src/idpyoidc/server/session/claims.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,22 @@
             return authorization_request["claims"].get(claims_release_point, {})
 
         return {}
 
     def _get_module(self, usage, context):
         module = None
         if usage == "userinfo":
-            module = self.upstream_get("endpoint", "userinfo")
+            module = context.upstream_get("endpoint","userinfo")
         elif usage == "id_token":
             try:
                 module = context.session_manager.token_handler["id_token"]
             except KeyError:
                 raise ServiceError("No support for ID Tokens")
         elif usage == "introspection":
-            module = self.upstream_get("endpoint", "introspection")
+            module = context.upstream_get("endpoint","introspection")
         elif usage == "access_token":
             try:
                 module = context.session_manager.token_handler["access_token"]
             except KeyError:
                 raise ServiceError("No support for Access Tokens")
 
         return module
@@ -64,27 +64,27 @@
     def _client_claims(
         self,
         client_id: str,
         module: object,
         claims_release_point: str,
         secondary_identifier: Optional[str] = "",
     ):
-        _context = self.upstream_get("context")
-        add_claims_by_scope = _context.cdb[client_id].get("add_claims", {}).get("by_scope", {})
+        _cdb = self.upstream_get("attribute", "cdb")
+        add_claims_by_scope = _cdb[client_id].get("add_claims", {}).get("by_scope", {})
         if add_claims_by_scope:
             _claims_by_scope = add_claims_by_scope.get(claims_release_point)
             if _claims_by_scope is None and secondary_identifier:
                 _claims_by_scope = add_claims_by_scope.get(secondary_identifier, False)
 
             if _claims_by_scope is None:
                 _claims_by_scope = module.kwargs.get("add_claims_by_scope", {})
         else:
             _claims_by_scope = module.kwargs.get("add_claims_by_scope", {})
 
-        add_claims_always = _context.cdb[client_id].get("add_claims", {}).get("always", {})
+        add_claims_always = _cdb[client_id].get("add_claims", {}).get("always", {})
         _always_add = add_claims_always.get(claims_release_point, [])
         if secondary_identifier:
             _always_2 = add_claims_always.get(secondary_identifier, [])
             _always_add.extend(_always_2)
 
         return _claims_by_scope, _always_add
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/session/database.py` & `idpyoidc-4.1.0/src/idpyoidc/server/session/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 class Database(ImpExp):
     parameter = {"db": DLDict, "crypt_config": {}}
 
     def __init__(self, crypt_config: Optional[dict] = None, **kwargs):
         ImpExp.__init__(self)
         self.db = DLDict()
 
-        for k, v in kwargs.items():
-            setattr(self, k, v)
+        # for k, v in kwargs.items():
+        #     setattr(self, k, v)
 
         if crypt_config is None:
             crypt_config = default_crypt_config()
 
         _crypt = init_encrypter(crypt_config)
         self.crypt = _crypt["encrypter"]
         self.crypt_config = _crypt["conf"]
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/session/grant.py` & `idpyoidc-4.1.0/src/idpyoidc/server/session/grant.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/session/grant_manager.py` & `idpyoidc-4.1.0/src/idpyoidc/server/session/grant_manager.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/session/info.py` & `idpyoidc-4.1.0/src/idpyoidc/server/session/info.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/session/manager.py` & `idpyoidc-4.1.0/src/idpyoidc/server/session/manager.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/session/token.py` & `idpyoidc-4.1.0/src/idpyoidc/server/session/token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/token/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/server/token/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/token/handler.py` & `idpyoidc-4.1.0/src/idpyoidc/server/token/handler.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/token/id_token.py` & `idpyoidc-4.1.0/src/idpyoidc/server/token/id_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/token/jwt_token.py` & `idpyoidc-4.1.0/src/idpyoidc/server/token/jwt_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/user_authn/authn_context.py` & `idpyoidc-4.1.0/src/idpyoidc/server/user_authn/authn_context.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/user_authn/user.py` & `idpyoidc-4.1.0/src/idpyoidc/server/user_authn/user.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/user_info/__init__.py` & `idpyoidc-4.1.0/src/idpyoidc/server/user_info/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/server/util.py` & `idpyoidc-4.1.0/src/idpyoidc/server/util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/ssl_context.py` & `idpyoidc-4.1.0/src/idpyoidc/ssl_context.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/storage/abfile.py` & `idpyoidc-4.1.0/src/idpyoidc/storage/abfile.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/storage/listfile.py` & `idpyoidc-4.1.0/src/idpyoidc/storage/listfile.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/time_util.py` & `idpyoidc-4.1.0/src/idpyoidc/time_util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc/util.py` & `idpyoidc-4.1.0/src/idpyoidc/util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/src/idpyoidc.egg-info/PKG-INFO` & `idpyoidc-4.1.0/src/idpyoidc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idpyoidc
-Version: 4.0.0
+Version: 4.1.0
 Summary: Python implementation of everything OAuth2 and OpenID Connect
 Home-page: https://github.com/IdentityPython/idpy-oidc/
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `idpyoidc-4.0.0/src/idpyoidc.egg-info/SOURCES.txt` & `idpyoidc-4.1.0/src/idpyoidc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 src/idpyoidc/client/http.py
 src/idpyoidc/client/rp_handler.py
 src/idpyoidc/client/service.py
 src/idpyoidc/client/service_context.py
 src/idpyoidc/client/util.py
 src/idpyoidc/client/claims/__init__.py
 src/idpyoidc/client/claims/oauth2.py
+src/idpyoidc/client/claims/oauth2resource.py
 src/idpyoidc/client/claims/oidc.py
 src/idpyoidc/client/claims/transform.py
 src/idpyoidc/client/oauth2/__init__.py
 src/idpyoidc/client/oauth2/access_token.py
 src/idpyoidc/client/oauth2/authorization.py
 src/idpyoidc/client/oauth2/client_credentials.py
 src/idpyoidc/client/oauth2/introspection.py
```

### Comparing `idpyoidc-4.0.0/tests/test_01_util.py` & `idpyoidc-4.1.0/tests/test_01_util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_03_time_util.py` & `idpyoidc-4.1.0/tests/test_03_time_util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_04_message.py` & `idpyoidc-4.1.0/tests/test_04_message.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_05_oauth2.py` & `idpyoidc-4.1.0/tests/test_05_oauth2.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_06_oidc.py` & `idpyoidc-4.1.0/tests/test_06_oidc.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_07_session.py` & `idpyoidc-4.1.0/tests/test_07_session.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_08_transform.py` & `idpyoidc-4.1.0/tests/test_08_transform.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_09_work_condition.py` & `idpyoidc-4.1.0/tests/test_09_work_condition.py`

 * *Files 20% similar despite different names*

```diff
@@ -248,7 +248,145 @@
             "userinfo_encrypted_response_alg",
             "userinfo_encrypted_response_enc",
             "userinfo_signed_response_alg",
         }
 
         # Not what I asked for but something I can handle
         assert to_use["subject_type"] == "pairwise"
+
+    def test_registration_response_consistence(self):
+        client_conf = {
+            "application_type": "web",
+            "base_url": "https://client.example.org/",
+            "redirect_uris": [
+                "https://client.example.org/callback",
+                "https://client.example.org/callback2",
+            ],
+            "client_name": "My Example",
+            "client_id": "client_id",
+            "keys": {"key_defs": KEYSPEC, "read_only": True},
+            "client_secret": "a longesh password",
+            "logo_uri": "https://client.example.org/logo.png",
+            "contacts": ["ve7jtb@example.org", "mary@example.org"],
+        }
+
+        self.claims.load_conf(client_conf, self.supported)
+
+        self.claims.prefer = supported_to_preferred(
+            supported=self.supported,
+            preference=self.claims.prefer,
+            base_url="https://example.com",
+        )
+        to_use_1 = preferred_to_registered(
+            prefers=self.claims.prefer,
+            supported=self.supported,
+        )
+
+        OP_BASEURL = "https://example.com"
+        provider_info_response = {
+            "version": "3.0",
+            "token_endpoint_auth_methods_supported": [
+                "client_secret_post",
+                "client_secret_basic",
+                "client_secret_jwt",
+                "private_key_jwt",
+            ],
+            "issuer": OP_BASEURL,
+            "jwks_uri": f"{OP_BASEURL}/static/jwks_tE2iLbOAqXhe8bqh.json",
+            "authorization_endpoint": f"{OP_BASEURL}/authorization",
+            "token_endpoint": f"{OP_BASEURL}/token",
+            "userinfo_endpoint": f"{OP_BASEURL}/userinfo",
+            "registration_endpoint": f"{OP_BASEURL}/registration",
+            "end_session_endpoint": f"{OP_BASEURL}/end_session",
+            # below are a set which the RP has default values but the OP overwrites
+            "scopes_supported": ["openid", "fee", "faa", "foo", "fum"],
+            "response_types_supported": ["code", "id_token", "code id_token"],
+            "response_modes_supported": ["query", "form_post", "new_fangled"],
+            # this does not have a default value
+            "acr_values_supported": ["mfa"],
+        }
+
+        pref = self.claims.prefer = supported_to_preferred(
+            supported=self.supported,
+            preference=self.claims.prefer,
+            base_url="https://example.com",
+            info=provider_info_response,
+        )
+
+        registration_request = create_registration_request(self.claims.prefer, self.supported)
+
+        assert set(registration_request.keys()) == {
+            "application_type",
+            "client_name",
+            "contacts",
+            "default_max_age",
+            "id_token_signed_response_alg",
+            "jwks",
+            "logo_uri",
+            "redirect_uris",
+            "request_object_signing_alg",
+            "response_modes",  # non-standard
+            "response_types",
+            "subject_type",
+            "token_endpoint_auth_method",
+            "token_endpoint_auth_signing_alg",
+            "userinfo_signed_response_alg",
+        }
+
+        assert registration_request["subject_type"] == "public"
+
+        registration_response = {
+            "application_type": "web",
+            "redirect_uris": [
+                "https://client.example.org/callback",
+                "https://client.example.org/callback2",
+            ],
+            "client_name": "My Example",
+            "logo_uri": "https://client.example.org/logo.png",
+            "subject_type": "pairwise",
+            "sector_identifier_uri": "https://other.example.net/file_of_redirect_uris.json",
+            "token_endpoint_auth_method": "client_secret_basic",
+            "jwks_uri": "https://client.example.org/my_public_keys.jwks",
+            "userinfo_encrypted_response_alg": "RSA1_5",
+            "userinfo_encrypted_response_enc": "A128CBC-HS256",
+            "contacts": ["ve7jtb@example.org", "mary@example.org"],
+            "request_uris": [
+                "https://client.example.org/rf.txt#qpXaRLh_n93TTR9F252ValdatUQvQiJi5BDub2BeznA"
+            ],
+        }
+
+        to_use_2 = preferred_to_registered(
+            prefers=self.claims.prefer,
+            supported=self.supported,
+            registration_response=registration_response,
+        )
+
+        assert set(to_use_2.keys()) == {
+            "application_type",
+            "client_id",
+            "client_name",
+            "client_secret",
+            "contacts",
+            "default_max_age",
+            "encrypt_request_object_supported",
+            "encrypt_userinfo_supported",
+            "id_token_signed_response_alg",
+            "jwks",
+            "jwks_uri",
+            "logo_uri",
+            "redirect_uris",
+            "request_object_signing_alg",
+            "request_uris",
+            "response_modes",
+            "response_types",
+            "scope",
+            "sector_identifier_uri",
+            "subject_type",
+            "token_endpoint_auth_method",
+            "token_endpoint_auth_signing_alg",
+            "userinfo_encrypted_response_alg",
+            "userinfo_encrypted_response_enc",
+            "userinfo_signed_response_alg",
+        }
+
+        # Not what I asked for but something I can handle
+        assert to_use_2["subject_type"] == "pairwise"
```

### Comparing `idpyoidc-4.0.0/tests/test_11_impexp.py` & `idpyoidc-4.1.0/tests/test_11_impexp.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_13_dump_item.py` & `idpyoidc-4.1.0/tests/test_13_dump_item.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_14_read_only_list_file.py` & `idpyoidc-4.1.0/tests/test_14_read_only_list_file.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_20_config.py` & `idpyoidc-4.1.0/tests/test_20_config.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_21_abfile.py` & `idpyoidc-4.1.0/tests/test_21_abfile.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_22_backchannel.py` & `idpyoidc-4.1.0/tests/test_22_backchannel.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_00_current.py` & `idpyoidc-4.1.0/tests/test_client_00_current.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_01_service_context.py` & `idpyoidc-4.1.0/tests/test_client_01_service_context.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_02_entity.py` & `idpyoidc-4.1.0/tests/test_client_02_entity.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_02b_entity_metadata.py` & `idpyoidc-4.1.0/tests/test_client_02b_entity_metadata.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_03_config.py` & `idpyoidc-4.1.0/tests/test_client_03_config.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_04_service.py` & `idpyoidc-4.1.0/tests/test_client_04_service.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_05_util.py` & `idpyoidc-4.1.0/tests/test_client_05_util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_06_client_authn.py` & `idpyoidc-4.1.0/tests/test_client_06_client_authn.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_10_entity.py` & `idpyoidc-4.1.0/tests/test_client_10_entity.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_12_client_auth.py` & `idpyoidc-4.1.0/tests/test_client_12_client_auth.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_14_service_context_impexp.py` & `idpyoidc-4.1.0/tests/test_client_14_service_context_impexp.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_15_cookie.py` & `idpyoidc-4.1.0/tests/test_client_15_cookie.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_16_util.py` & `idpyoidc-4.1.0/tests/test_client_16_util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_17_http.py` & `idpyoidc-4.1.0/tests/test_client_17_http.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_18_service.py` & `idpyoidc-4.1.0/tests/test_client_18_service.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_19_webfinger.py` & `idpyoidc-4.1.0/tests/test_client_19_webfinger.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_20_oauth2.py` & `idpyoidc-4.1.0/tests/test_client_20_oauth2.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_21_oidc_service.py` & `idpyoidc-4.1.0/tests/test_client_21_oidc_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 
-import pytest
-import responses
 from cryptojwt.exception import UnsupportedAlgorithm
 from cryptojwt.jws import jws
 from cryptojwt.jws.utils import left_hash
 from cryptojwt.jwt import JWT
 from cryptojwt.key_jar import build_keyjar
 from cryptojwt.key_jar import init_key_jar
+import pytest
+import responses
 
 from idpyoidc.client.defaults import DEFAULT_OIDC_SERVICES
 from idpyoidc.client.entity import Entity
 from idpyoidc.client.exception import ParameterError
 from idpyoidc.client.oidc.registration import response_types_to_grant_types
 from idpyoidc.exception import MissingRequiredAttribute
 from idpyoidc.message.oidc import AccessTokenRequest
@@ -721,15 +721,15 @@
             "authorization_endpoint": "{}/authorization".format(OP_BASEURL),
             "token_endpoint": "{}/token".format(OP_BASEURL),
             "userinfo_endpoint": "{}/userinfo".format(OP_BASEURL),
             "registration_endpoint": "{}/registration".format(OP_BASEURL),
             "end_session_endpoint": "{}/end_session".format(OP_BASEURL),
         }
         _context = self.service.upstream_get("context")
-        assert _context.claims.use == {}
+        # assert _context.claims.use == {}
         resp = self.service.post_parse_response(provider_info_response)
 
         iss_jwks = ISS_KEY.export_jwks_as_json(issuer_id=ISS)
         with responses.RequestsMock() as rsps:
             rsps.add("GET", resp["jwks_uri"], body=iss_jwks, status=200)
 
             self.service.update_service_context(resp, "")
@@ -784,15 +784,39 @@
             "authorization_endpoint": "{}/authorization".format(OP_BASEURL),
             "token_endpoint": "{}/token".format(OP_BASEURL),
             "userinfo_endpoint": "{}/userinfo".format(OP_BASEURL),
             "registration_endpoint": "{}/registration".format(OP_BASEURL),
             "end_session_endpoint": "{}/end_session".format(OP_BASEURL),
         }
         _context = self.service.upstream_get("context")
-        assert _context.claims.use == {}
+        assert set(_context.claims.use.keys()) == {
+            'application_type',
+            'backchannel_logout_session_required',
+            'backchannel_logout_uri',
+            'callback_uris',
+            'client_id',
+            'client_secret',
+            'contacts',
+            'default_max_age',
+            'encrypt_id_token_supported',
+            'encrypt_request_object_supported',
+            'encrypt_userinfo_supported',
+            'grant_types',
+            'id_token_signed_response_alg',
+            'jwks',
+            'post_logout_redirect_uris',
+            'redirect_uris',
+            'request_object_signing_alg',
+            'response_modes',
+            'response_types',
+            'scope',
+            'subject_type',
+            'token_endpoint_auth_method',
+            'token_endpoint_auth_signing_alg',
+            'userinfo_signed_response_alg'}
         resp = self.service.post_parse_response(provider_info_response)
 
         iss_jwks = ISS_KEY.export_jwks_as_json(issuer_id=ISS)
         with responses.RequestsMock() as rsps:
             rsps.add("GET", resp["jwks_uri"], body=iss_jwks, status=200)
 
             self.service.update_service_context(resp, "")
```

### Comparing `idpyoidc-4.0.0/tests/test_client_22_oidc.py` & `idpyoidc-4.1.0/tests/test_client_22_oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
         )
         assert isinstance(msg, RefreshAccessTokenRequest)
         assert msg.to_dict() == {
             "client_id": "client_1",
             "client_secret": "abcdefghijklmnop",
             "grant_type": "refresh_token",
             "refresh_token": "refresh_with_me",
+            'scope': 'openid'
         }
 
     def test_do_userinfo_request_init(self):
         _context = self.client.get_context()
         _state = _context.cstate.create_key()
         _context.cstate.set(_state, {"iss": "issuer"})
```

### Comparing `idpyoidc-4.0.0/tests/test_client_23_pkce.py` & `idpyoidc-4.1.0/tests/test_client_23_pkce.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_24_oic_utils.py` & `idpyoidc-4.1.0/tests/test_client_24_oic_utils.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_25_oauth2_cc_ropc.py` & `idpyoidc-4.1.0/tests/test_client_25_oauth2_cc_ropc.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_26_read_registration.py` & `idpyoidc-4.1.0/tests/test_client_26_read_registration.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_27_conversation.py` & `idpyoidc-4.1.0/tests/test_client_27_conversation.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_28_stand_alone.py` & `idpyoidc-4.1.0/tests/test_client_28_stand_alone.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_29_pushed_auth.py` & `idpyoidc-4.1.0/tests/test_client_29_pushed_auth.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_30_rp_handler_oidc.py` & `idpyoidc-4.1.0/tests/test_client_30_rp_handler_oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 import os
 from urllib.parse import parse_qs
 from urllib.parse import urlparse
 from urllib.parse import urlsplit
 
+from cryptojwt.key_jar import init_key_jar
 import pytest
 import responses
-from cryptojwt.key_jar import init_key_jar
 
 from idpyoidc.client.entity import Entity
 from idpyoidc.client.rp_handler import RPHandler
-from idpyoidc.message.oidc import JRD
 from idpyoidc.message.oidc import AccessTokenResponse
 from idpyoidc.message.oidc import AuthorizationResponse
 from idpyoidc.message.oidc import IdToken
+from idpyoidc.message.oidc import JRD
 from idpyoidc.message.oidc import Link
 from idpyoidc.message.oidc import OpenIDSchema
 from idpyoidc.message.oidc import ProviderConfigurationResponse
 from idpyoidc.message.oidc import RegistrationResponse
 from idpyoidc.util import rndstr
 
 BASE_URL = "https://example.com/rp"
@@ -256,22 +256,29 @@
         assert set(_context.get("provider_info").keys()) == {
             "authorization_endpoint",
             "token_endpoint",
             "userinfo_endpoint",
         }
 
         _pref = [k for k, v in _context.prefers().items() if v]
-        assert set(_pref) == {
-            "client_id",
-            "client_secret",
-            "redirect_uris",
-            "response_types_supported",
-            "callback_uris",
-            "scopes_supported",
-        }
+        assert set(_pref) == {'application_type',
+                              'callback_uris',
+                              'client_id',
+                              'client_secret',
+                              'default_max_age',
+                              'grant_types_supported',
+                              'id_token_signing_alg_values_supported',
+                              'redirect_uris',
+                              'request_object_signing_alg_values_supported',
+                              'response_modes_supported',
+                              'response_types_supported',
+                              'scopes_supported',
+                              'subject_types_supported',
+                              'token_endpoint_auth_signing_alg_values_supported',
+                              'userinfo_signing_alg_values_supported'}
 
         _github_id = iss_id("github")
         _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         # The key jar should only contain a symmetric key that is the clients
         # secret. 2 because one is marked for encryption and the other signing
@@ -300,16 +307,17 @@
         issuer = self.rph.do_provider_info(client)
         self.rph.do_client_registration(client, "github")
 
         # only 2 things should have happened
 
         assert self.rph.hash2issuer["github"] == issuer
         assert (
-            client.get_context().get_preference("callback_uris").get("post_logout_redirect_uris")
-            is None
+                client.get_context().get_preference("callback_uris").get(
+                    "post_logout_redirect_uris")
+                is None
         )
 
     def test_do_client_setup(self):
         client = self.rph.client_setup("github")
         _github_id = iss_id("github")
         _context = client.get_context()
```

### Comparing `idpyoidc-4.0.0/tests/test_client_30_rph_defaults.py` & `idpyoidc-4.1.0/tests/test_client_30_rph_defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from urllib.parse import parse_qs
 from urllib.parse import urlparse
 
+from cryptojwt.key_jar import build_keyjar
 import pytest
 import responses
-from cryptojwt.key_jar import build_keyjar
 
 from idpyoidc.client.defaults import DEFAULT_KEY_DEFS
 from idpyoidc.client.rp_handler import RPHandler
 from idpyoidc.message.oidc import ProviderConfigurationResponse
 from idpyoidc.message.oidc import RegistrationResponse
 
 BASE_URL = "https://example.com"
@@ -32,26 +32,37 @@
             "userinfo",
             "refresh_token",
         }
 
         _context = client.get_context()
 
         assert set(_context.claims.prefer.keys()) == {
-            "application_type",
-            "callback_uris",
-            "id_token_encryption_alg_values_supported",
-            "id_token_encryption_enc_values_supported",
-            "jwks_uri",
-            "redirect_uris",
-            "request_object_encryption_alg_values_supported",
-            "request_object_encryption_enc_values_supported",
-            "scopes_supported",
-            "userinfo_encryption_alg_values_supported",
-            "userinfo_encryption_enc_values_supported",
-        }
+            'application_type',
+            'callback_uris',
+            'default_max_age',
+            'encrypt_request_object_supported',
+            'encrypt_userinfo_supported',
+            'grant_types_supported',
+            'id_token_encryption_alg_values_supported',
+            'id_token_encryption_enc_values_supported',
+            'id_token_signing_alg_values_supported',
+            'jwks_uri',
+            'redirect_uris',
+            'request_object_encryption_alg_values_supported',
+            'request_object_encryption_enc_values_supported',
+            'request_object_signing_alg_values_supported',
+            'response_modes_supported',
+            'response_types_supported',
+            'scopes_supported',
+            'subject_types_supported',
+            'token_endpoint_auth_methods_supported',
+            'token_endpoint_auth_signing_alg_values_supported',
+            'userinfo_encryption_alg_values_supported',
+            'userinfo_encryption_enc_values_supported',
+            'userinfo_signing_alg_values_supported'}
 
         _keyjar = client.get_attribute("keyjar")
         assert list(_keyjar.owners()) == ["", BASE_URL]
         keys = _keyjar.get_issuer_keys("")
         assert len(keys) == 2
 
         assert _context.base_url == BASE_URL
```

### Comparing `idpyoidc-4.0.0/tests/test_client_31_oauth2_persistent.py` & `idpyoidc-4.1.0/tests/test_client_31_oauth2_persistent.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_32_oidc_persistent.py` & `idpyoidc-4.1.0/tests/test_client_32_oidc_persistent.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         msg = client_1.get_service("refresh_token").construct(request_args=req_args, state=_state)
         assert isinstance(msg, RefreshAccessTokenRequest)
         assert msg.to_dict() == {
             "client_id": "client_1",
             "client_secret": "abcdefghijklmnop",
             "grant_type": "refresh_token",
             "refresh_token": "refresh_with_me",
+            'scope': 'openid'
         }
 
     def test_do_userinfo_request_init(self):
         # Client 1 starts
         client_1 = RP(config=CONF)
         _state = client_1.get_context().cstate.create_state(iss=ISSUER)
```

### Comparing `idpyoidc-4.0.0/tests/test_client_40_dpop.py` & `idpyoidc-4.1.0/tests/test_client_40_dpop.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_41_rp_handler_persistent.py` & `idpyoidc-4.1.0/tests/test_client_41_rp_handler_persistent.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_50_ciba.py` & `idpyoidc-4.1.0/tests/test_client_50_ciba.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_51_identity_assurance.py` & `idpyoidc-4.1.0/tests/test_client_51_identity_assurance.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_client_55_token_exchange.py` & `idpyoidc-4.1.0/tests/test_client_55_token_exchange.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_00_configure.py` & `idpyoidc-4.1.0/tests/test_server_00_configure.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_00a_client_configure.py` & `idpyoidc-4.1.0/tests/test_server_00a_client_configure.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_01_claims.py` & `idpyoidc-4.1.0/tests/test_server_01_claims.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_01_construct.py` & `idpyoidc-4.1.0/tests/test_server_01_construct.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_02_session_token.py` & `idpyoidc-4.1.0/tests/test_server_02_session_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_03_authz_handling.py` & `idpyoidc-4.1.0/tests/test_server_03_authz_handling.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_04_session_info.py` & `idpyoidc-4.1.0/tests/test_server_04_session_info.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_05_token_handler.py` & `idpyoidc-4.1.0/tests/test_server_05_token_handler.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_06_grant.py` & `idpyoidc-4.1.0/tests/test_server_06_grant.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_07_sess_mngm_db.py` & `idpyoidc-4.1.0/tests/test_server_07_sess_mngm_db.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_08_id_token.py` & `idpyoidc-4.1.0/tests/test_server_08_id_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_09_authn_context.py` & `idpyoidc-4.1.0/tests/test_server_09_authn_context.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_10_session_manager.py` & `idpyoidc-4.1.0/tests/test_server_10_session_manager.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_11_session_manager_pairwise.py` & `idpyoidc-4.1.0/tests/test_server_11_session_manager_pairwise.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_12_session_life.py` & `idpyoidc-4.1.0/tests/test_server_12_session_life.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_13_user_authn.py` & `idpyoidc-4.1.0/tests/test_server_13_user_authn.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_14_userinfo.py` & `idpyoidc-4.1.0/tests/test_server_14_userinfo.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_15_login_hint.py` & `idpyoidc-4.1.0/tests/test_server_15_login_hint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_16_endpoint.py` & `idpyoidc-4.1.0/tests/test_server_16_endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_16_endpoint_context.py` & `idpyoidc-4.1.0/tests/test_server_16_endpoint_context.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_17_client_authn.py` & `idpyoidc-4.1.0/tests/test_server_17_client_authn.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_20a_server.py` & `idpyoidc-4.1.0/tests/test_server_20a_server.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_20b_claims.py` & `idpyoidc-4.1.0/tests/test_server_20b_claims.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_20c_authz_handling.py` & `idpyoidc-4.1.0/tests/test_server_20c_authz_handling.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_20d_client_authn.py` & `idpyoidc-4.1.0/tests/test_server_20d_client_authn.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_20e_jwt_token.py` & `idpyoidc-4.1.0/tests/test_server_20e_jwt_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_20f_userinfo.py` & `idpyoidc-4.1.0/tests/test_server_20f_userinfo.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_20g_cookie_handler.py` & `idpyoidc-4.1.0/tests/test_server_20g_cookie_handler.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_21_oidc_discovery_endpoint.py` & `idpyoidc-4.1.0/tests/test_server_21_oidc_discovery_endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_22_oidc_provider_config_endpoint.py` & `idpyoidc-4.1.0/tests/test_server_22_oidc_provider_config_endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_23_oidc_registration_endpoint.py` & `idpyoidc-4.1.0/tests/test_server_23_oidc_registration_endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_24_oauth2_authorization_endpoint.py` & `idpyoidc-4.1.0/tests/test_server_24_oauth2_authorization_endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_24_oauth2_authorization_endpoint_jar.py` & `idpyoidc-4.1.0/tests/test_server_24_oauth2_authorization_endpoint_jar.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_24_oauth2_resource_indicators.py` & `idpyoidc-4.1.0/tests/test_server_24_oauth2_resource_indicators.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_24_oauth2_token_endpoint.py` & `idpyoidc-4.1.0/tests/test_server_24_oauth2_token_endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_24_oauth2_token_endpoint_def_conf.py` & `idpyoidc-4.1.0/tests/test_server_24_oauth2_token_endpoint_def_conf.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_24_oidc_authorization_endpoint.py` & `idpyoidc-4.1.0/tests/test_server_24_oidc_authorization_endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_26_oidc_userinfo_endpoint.py` & `idpyoidc-4.1.0/tests/test_server_26_oidc_userinfo_endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_30_oidc_end_session.py` & `idpyoidc-4.1.0/tests/test_server_30_oidc_end_session.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_31_oauth2_introspection.py` & `idpyoidc-4.1.0/tests/test_server_31_oauth2_introspection.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_32_oidc_read_registration.py` & `idpyoidc-4.1.0/tests/test_server_32_oidc_read_registration.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_33_oauth2_pkce.py` & `idpyoidc-4.1.0/tests/test_server_33_oauth2_pkce.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_34_oidc_sso.py` & `idpyoidc-4.1.0/tests/test_server_34_oidc_sso.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_35_oidc_token_endpoint.py` & `idpyoidc-4.1.0/tests/test_server_35_oidc_token_endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_35_oidc_token_endpoint_def_conf.py` & `idpyoidc-4.1.0/tests/test_server_35_oidc_token_endpoint_def_conf.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_36_oauth2_token_exchange.py` & `idpyoidc-4.1.0/tests/test_server_36_oauth2_token_exchange.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_38_oauth2_revocation_endpoint.py` & `idpyoidc-4.1.0/tests/test_server_38_oauth2_revocation_endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_40_oauth2_pushed_authorization.py` & `idpyoidc-4.1.0/tests/test_server_40_oauth2_pushed_authorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,16 +135,16 @@
                     "kwargs": {
                         "client_authn_method": [
                             "client_secret_post",
                             "client_secret_basic",
                             "client_secret_jwt",
                             "private_key_jwt",
                         ]
-                    },
-                },
+                    }
+                }
             },
             "authentication": {
                 "anon": {
                     "acr": "http://www.swamid.se/policy/assurance/al1",
                     "class": "idpyoidc.server.user_authn.user.NoAuthn",
                     "kwargs": {"user": "diana"},
                 }
```

### Comparing `idpyoidc-4.0.0/tests/test_server_50_persistence.py` & `idpyoidc-4.1.0/tests/test_server_50_persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,24 +277,29 @@
         server2.context.load(
             _store,
             init_args={
                 "upstream_get": server2.upstream_get,
                 "handler": server2.context.session_manager.token_handler,
             },
         )
+        server2.context.upstream_get = server2.unit_get
 
         self.endpoint = {
             1: server1.get_endpoint("userinfo"),
             2: server2.get_endpoint("userinfo"),
         }
 
         self.session_manager = {
             1: server1.context.session_manager,
             2: server2.context.session_manager,
         }
+        self.context_unit_get = {
+            1: server1.context.unit_get,
+            2: server2.context.unit_get
+        }
         self.user_id = "diana"
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier="", index=1):
         if sector_identifier:
             authz_req = auth_req.copy()
             authz_req["sector_identifier_uri"] = sector_identifier
         else:
@@ -335,16 +340,17 @@
 
         self.session_manager[index].set([self.user_id, _session_info["client_id"], grant.id], grant)
 
         return _token
 
     def _dump_restore(self, fro, to):
         _store = self.session_manager[fro].dump()
+        context_unit_get = self.endpoint[to].upstream_get("unit").context.unit_get
         self.session_manager[to].load(
-            _store, init_args={"upstream_get": self.endpoint[to].upstream_get}
+            _store, init_args={"upstream_get": context_unit_get}
         )
 
     def test_init(self):
         assert self.endpoint[1]
         assert set(self.endpoint[1].upstream_get("context").provider_info["scopes_supported"]) == {
             "openid"
         }
```

### Comparing `idpyoidc-4.0.0/tests/test_server_60_dpop.py` & `idpyoidc-4.1.0/tests/test_server_60_dpop.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_server_61_add_on.py` & `idpyoidc-4.1.0/tests/test_server_61_add_on.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_tandem_oauth2_add_on.py` & `idpyoidc-4.1.0/tests/test_tandem_oauth2_add_on.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_tandem_oauth2_cc_ropc.py` & `idpyoidc-4.1.0/tests/test_tandem_oauth2_cc_ropc.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_tandem_oauth2_code.py` & `idpyoidc-4.1.0/tests/test_tandem_oauth2_code.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_tandem_oauth2_token_exchange.py` & `idpyoidc-4.1.0/tests/test_tandem_oauth2_token_exchange.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_tandem_oauth2_token_revocation.py` & `idpyoidc-4.1.0/tests/test_tandem_oauth2_token_revocation.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-4.0.0/tests/test_tandem_oidc_code.py` & `idpyoidc-4.1.0/tests/test_tandem_oidc_code.py`

 * *Files identical despite different names*

