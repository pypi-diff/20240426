# Comparing `tmp/fastapi_nextauth_jwt-1.1.2.tar.gz` & `tmp/fastapi_nextauth_jwt-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_nextauth_jwt-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fastapi_nextauth_jwt-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_nextauth_jwt-1.1.2.tar` & `fastapi_nextauth_jwt-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,40 @@
--rw-r--r--   0        0        0     1069 2023-07-19 15:09:11.148761 fastapi_nextauth_jwt-1.1.2/LICENSE
--rw-r--r--   0        0        0     2143 2023-07-19 15:09:11.148761 fastapi_nextauth_jwt-1.1.2/README.md
--rw-r--r--   0        0        0      732 2023-07-19 15:09:11.148761 fastapi_nextauth_jwt-1.1.2/examples/simple/README.md
--rw-r--r--   0        0        0        6 2023-07-19 15:09:11.148761 fastapi_nextauth_jwt-1.1.2/examples/simple/fastapi/.gitignore
--rw-r--r--   0        0        0      504 2023-07-19 15:09:11.148761 fastapi_nextauth_jwt-1.1.2/examples/simple/fastapi/main.py
--rw-r--r--   0        0        0       53 2023-07-19 15:09:11.148761 fastapi_nextauth_jwt-1.1.2/examples/simple/fastapi/requirements.txt
--rw-r--r--   0        0        0       40 2023-07-19 15:09:11.148761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/.eslintrc.json
--rw-r--r--   0        0        0      375 2023-07-19 15:09:11.148761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/.gitignore
--rw-r--r--   0        0        0     1751 2023-07-19 15:09:11.148761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/README.md
--rw-r--r--   0        0        0      201 2023-07-19 15:09:11.148761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/next-env.d.ts
--rw-r--r--   0        0        0      254 2023-07-19 15:09:11.148761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/next.config.js
--rw-r--r--   0        0        0   288145 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/package-lock.json
--rw-r--r--   0        0        0      628 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/package.json
--rw-r--r--   0        0        0       82 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/postcss.config.js
--rw-r--r--   0        0        0    25931 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/public/favicon.ico
--rw-r--r--   0        0        0     1375 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/public/next.svg
--rw-r--r--   0        0        0      629 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/public/vercel.svg
--rw-r--r--   0        0        0      119 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/src/middleware.ts
--rw-r--r--   0        0        0      386 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/src/pages/_app.tsx
--rw-r--r--   0        0        0      264 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/src/pages/_document.tsx
--rw-r--r--   0        0        0     1356 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/src/pages/api/auth/[...nextauth].js
--rw-r--r--   0        0        0      311 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/src/pages/api/hello.ts
--rw-r--r--   0        0        0     1662 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/src/pages/index.tsx
--rw-r--r--   0        0        0      578 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/src/styles/globals.css
--rw-r--r--   0        0        0      480 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/tailwind.config.js
--rw-r--r--   0        0        0      556 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/tsconfig.json
--rw-r--r--   0        0        0      661 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      222 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/src/fastapi_nextauth_jwt/__init__.py
--rw-r--r--   0        0        0      974 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/src/fastapi_nextauth_jwt/cookies.py
--rw-r--r--   0        0        0      938 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/src/fastapi_nextauth_jwt/csrf.py
--rw-r--r--   0        0        0      873 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/src/fastapi_nextauth_jwt/exceptions.py
--rw-r--r--   0        0        0     6322 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py
--rw-r--r--   0        0        0      580 2023-07-19 15:09:11.152761 fastapi_nextauth_jwt-1.1.2/src/fastapi_nextauth_jwt/operations.py
--rw-r--r--   0        0        0     2713 1970-01-01 00:00:00.000000 fastapi_nextauth_jwt-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2328 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/README.md
+-rw-r--r--   0        0        0      812 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/README.md
+-rw-r--r--   0        0        0      324 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/docker-compose.yml
+-rw-r--r--   0        0        0       12 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/fastapi/.dockerignore
+-rw-r--r--   0        0        0        6 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/fastapi/.gitignore
+-rw-r--r--   0        0        0      303 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/fastapi/Dockerfile
+-rw-r--r--   0        0        0      504 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/fastapi/main.py
+-rw-r--r--   0        0        0       33 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/fastapi/requirements.txt
+-rw-r--r--   0        0        0       27 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/.dockerignore
+-rw-r--r--   0        0        0       40 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/.eslintrc.json
+-rw-r--r--   0        0        0      375 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/.gitignore
+-rw-r--r--   0        0        0      264 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/Dockerfile
+-rw-r--r--   0        0        0     1751 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/README.md
+-rw-r--r--   0        0        0      267 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/next-env.d.ts
+-rw-r--r--   0        0        0      254 2024-04-26 16:50:43.421717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/next.config.js
+-rw-r--r--   0        0        0   175146 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/package-lock.json
+-rw-r--r--   0        0        0      646 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/package.json
+-rw-r--r--   0        0        0       82 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/postcss.config.js
+-rw-r--r--   0        0        0    25931 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/public/favicon.ico
+-rw-r--r--   0        0        0     1375 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/public/next.svg
+-rw-r--r--   0        0        0      629 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/public/vercel.svg
+-rw-r--r--   0        0        0       71 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/src/app/api/auth/[...nextauth]/route.ts
+-rw-r--r--   0        0        0      791 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/src/auth.ts
+-rw-r--r--   0        0        0       80 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/src/middleware.ts
+-rw-r--r--   0        0        0      386 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/src/pages/_app.tsx
+-rw-r--r--   0        0        0      264 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/src/pages/_document.tsx
+-rw-r--r--   0        0        0      311 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/src/pages/api/hello.ts
+-rw-r--r--   0        0        0     1662 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/src/pages/index.tsx
+-rw-r--r--   0        0        0      578 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/src/styles/globals.css
+-rw-r--r--   0        0        0      480 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/tailwind.config.js
+-rw-r--r--   0        0        0      710 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/tsconfig.json
+-rw-r--r--   0        0        0      661 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      237 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/src/fastapi_nextauth_jwt/__init__.py
+-rw-r--r--   0        0        0      974 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/src/fastapi_nextauth_jwt/cookies.py
+-rw-r--r--   0        0        0      938 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/src/fastapi_nextauth_jwt/csrf.py
+-rw-r--r--   0        0        0     1070 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/src/fastapi_nextauth_jwt/exceptions.py
+-rw-r--r--   0        0        0     7588 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py
+-rw-r--r--   0        0        0      580 2024-04-26 16:50:43.425717 fastapi_nextauth_jwt-2.0.0/src/fastapi_nextauth_jwt/operations.py
+-rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 fastapi_nextauth_jwt-2.0.0/PKG-INFO
```

### Comparing `fastapi_nextauth_jwt-1.1.2/LICENSE` & `fastapi_nextauth_jwt-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.2/README.md` & `fastapi_nextauth_jwt-2.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 # fastapi-nextauth-jwt
 [![PyPI version](https://badge.fury.io/py/fastapi-nextauth-jwt.svg)](https://badge.fury.io/py/fastapi-nextauth-jwt)
 
-This project contains a FastAPI dependency that can be used to decrypt and validate JWTs generated by NextAuth.
-The purpose of this project is to make it easy to use a FastAPI backend in projects that use Next.js and NextAuth 
-in the frontend. 
+This project contains a FastAPI dependency that can be used to decrypt and validate JWTs generated by Auth.js.
+The purpose of this project is to make it easy to use a FastAPI backend in projects that use Next.js and NextAuth / Auth.js 
+in the frontend. It might work with other frameworks using Auth.js too! (But I haven't tested that, feel free to contribute if you do)
 
-Besides JWT decryption and validation, NextAuth compatible cross-site request forgery (CSRF) protection is also implemented.
+Besides JWT decryption and validation, Auth.js compatible cross-site request forgery (CSRF) protection is also implemented.
 
 # Installation
-General usage:
 ```shell
 pip install fastapi-nextauth-jwt
 ```
-Development:
-```shell
-pip install "fastapi-nextauth-jwt[test]"
-```
-
 # Usage
 
 ```python
 from typing import Annotated
 from fastapi import FastAPI, Depends
 from fastapi_nextauth_jwt import NextAuthJWT
 
@@ -32,22 +26,25 @@
 
 @app.get("/")
 async def return_jwt(jwt: Annotated[dict, Depends(JWT)]):
     return jwt
 ```
 
 There are a few configuration options available in the NextAuthJWT constructor, but the most important one is `secret`,
-which should be equivalent to `NEXTAUTH_SECRET` on the Next.js side. A real application would obviously not hardcode the secret like this,
-but rely on the `NEXTAUTH_SECRET` env var.
+which should be equivalent to `NEXTAUTH_SECRET` on the Next.js side. Please don't hardcode the secret like this in a real application,
+but rely on the `NEXTAUTH_SECRET` env var :)
 
 It is also possible to enable or disable CSRF protection using `csrf_prevention_enabled`. 
 If this is not set, this will looks at the ENV environment variable. If this is `dev` then CSRF protection will be disabled.
 It is also possible to customize the HTTP verbs to which CSRF protection is applied.
 
 You should also set the `NEXTAUTH_URL` environment variable, as it is used to determine
-whether or not secure cookies are being used. Or you can set the cookie names manually.
+whether secure cookies are being used. Or you can set the cookie names manually.
+
+## NextAuth / Auth.js v4 compatibility
+A compatibility shim is included if you're still on NextAuth v4, just replace `NexAuthJWT` with `NextAuthJWTv4`
 
 ## Examples
 A [simple example](https://github.com/TCatshoek/fastapi-nextauth-jwt/tree/main/examples/simple) is available in the examples folder. It uses Next.js URL rewrites to direct
 requests to FastAPI. This is just one way to do it, putting both the backend and frontend
 behind something like nginx would also be a good strategy. As long as the cookies can make it to FastAPI
 you should be good to go!
```

### Comparing `fastapi_nextauth_jwt-1.1.2/examples/simple/README.md` & `fastapi_nextauth_jwt-2.0.0/examples/simple/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,24 +4,31 @@
 and a FastAPI backend.
 
 It uses [Next.js url rewriting](https://nextjs.org/docs/pages/api-reference/next-config-js/rewrites)
 to direct requests starting with `/fastapi` to the FastAPI backend.
 
 ## Setup
 
-### FastAPI
+### With docker compose:
+```shell
+docker-compose up
+```
+
+### Without docker:
+
+#### FastAPI
 ```shell
 cd fastapi
 python -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
 uvicorn main:app --reload
 ```
 
-### Next.js
+#### Next.js
 ```shell
 cd nextjs
 npm install
 npm run dev
 ```
 
 ## Usage
```

### Comparing `fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/README.md` & `fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/package.json` & `fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'dependencies'": "{'@types/node': '^20.12.7', '@types/react': '^18.3.0', '@types/react-dom': "*

 * *                   "'^18.3.0', 'autoprefixer': '^10.4.19', 'eslint': '^8.57.0', "*

 * *                   "'eslint-config-next': '^14.2.3', 'next': '^14.2.3', 'next-auth': "*

 * *                   "'^5.0.0-beta.17', 'postcss': '^8.4.38', 'react': '^18.3.0', 'react-dom': "*

 * *                   "'^18.3.0', 'tailwindcss': '^3.4.3', 'typescript': '^5.4.5'}",*

 * * "'devDependencies'": "{'prettier': '^3.2.5'}"}*

```diff
@@ -1,25 +1,25 @@
 {
     "dependencies": {
-        "@types/node": "20.4.2",
-        "@types/react": "18.2.15",
-        "@types/react-dom": "18.2.7",
-        "autoprefixer": "10.4.14",
-        "eslint": "8.45.0",
-        "eslint-config-next": "13.4.10",
-        "next": "13.4.10",
-        "next-auth": "^4.22.1",
-        "postcss": "8.4.26",
-        "react": "18.2.0",
-        "react-dom": "18.2.0",
-        "tailwindcss": "3.3.3",
-        "typescript": "5.1.6"
+        "@types/node": "^20.12.7",
+        "@types/react": "^18.3.0",
+        "@types/react-dom": "^18.3.0",
+        "autoprefixer": "^10.4.19",
+        "eslint": "^8.57.0",
+        "eslint-config-next": "^14.2.3",
+        "next": "^14.2.3",
+        "next-auth": "^5.0.0-beta.17",
+        "postcss": "^8.4.38",
+        "react": "^18.3.0",
+        "react-dom": "^18.3.0",
+        "tailwindcss": "^3.4.3",
+        "typescript": "^5.4.5"
     },
     "devDependencies": {
-        "prettier": "3.0.0"
+        "prettier": "^3.2.5"
     },
     "name": "nextjs",
     "private": true,
     "scripts": {
         "build": "next build",
         "dev": "next dev",
         "lint": "next lint",
```

### Comparing `fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/public/favicon.ico` & `fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/public/next.svg` & `fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/public/next.svg`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/public/vercel.svg` & `fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/public/vercel.svg`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/src/pages/index.tsx` & `fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/src/pages/index.tsx`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/src/styles/globals.css` & `fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/src/styles/globals.css`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.2/examples/simple/nextjs/tsconfig.json` & `fastapi_nextauth_jwt-2.0.0/examples/simple/nextjs/tsconfig.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9479166666666666%*

 * *Differences: {"'compilerOptions'": "{'plugins': [OrderedDict([('name', 'next')])]}",*

 * * "'include'": "{insert: [(3, '.next/types/**/*.ts')]}"}*

```diff
@@ -15,21 +15,27 @@
         "moduleResolution": "node",
         "noEmit": true,
         "paths": {
             "@/*": [
                 "./src/*"
             ]
         },
+        "plugins": [
+            {
+                "name": "next"
+            }
+        ],
         "resolveJsonModule": true,
         "skipLibCheck": true,
         "strict": true,
         "target": "es5"
     },
     "exclude": [
         "node_modules"
     ],
     "include": [
         "next-env.d.ts",
         "**/*.ts",
-        "**/*.tsx"
+        "**/*.tsx",
+        ".next/types/**/*.ts"
     ]
 }
```

### Comparing `fastapi_nextauth_jwt-1.1.2/pyproject.toml` & `fastapi_nextauth_jwt-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.2/src/fastapi_nextauth_jwt/cookies.py` & `fastapi_nextauth_jwt-2.0.0/src/fastapi_nextauth_jwt/cookies.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.2/src/fastapi_nextauth_jwt/csrf.py` & `fastapi_nextauth_jwt-2.0.0/src/fastapi_nextauth_jwt/csrf.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.2/src/fastapi_nextauth_jwt/exceptions.py` & `fastapi_nextauth_jwt-2.0.0/src/fastapi_nextauth_jwt/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 class NextAuthJWTException(Exception):
     def __init__(self, *args: object):
         super().__init__(args)
         self.message = None
         self.status_code = None
 
 
@@ -23,8 +22,14 @@
         self.status_code = status_code
         self.message = message
 
 
 class TokenExpiredException(NextAuthJWTException):
     def __init__(self, status_code: int, message: str):
         self.status_code = status_code
-        self.message = message
+        self.message = message
+
+
+class UnsupportedEncryptionAlgorithmException(NextAuthJWTException):
+    def __init__(self, status_code: int, message: str):
+        self.status_code = status_code
+        self.message = message
```

### Comparing `fastapi_nextauth_jwt-1.1.2/src/fastapi_nextauth_jwt/operations.py` & `fastapi_nextauth_jwt-2.0.0/src/fastapi_nextauth_jwt/operations.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.2/PKG-INFO` & `fastapi_nextauth_jwt-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_nextauth_jwt
-Version: 1.1.2
+Version: 2.0.0
 Summary: A fastapi dependency used to decode jwt tokens generated by nextauth,
 Author: Tom Catshoek
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: fastapi
 Requires-Dist: cryptography
 Requires-Dist: python-jose[cryptography]
@@ -13,30 +13,24 @@
 Requires-Dist: httpx ; extra == "test"
 Project-URL: Home, https://github.com/TCatshoek/fastapi-nextauth-jwt
 Provides-Extra: test
 
 # fastapi-nextauth-jwt
 [![PyPI version](https://badge.fury.io/py/fastapi-nextauth-jwt.svg)](https://badge.fury.io/py/fastapi-nextauth-jwt)
 
-This project contains a FastAPI dependency that can be used to decrypt and validate JWTs generated by NextAuth.
-The purpose of this project is to make it easy to use a FastAPI backend in projects that use Next.js and NextAuth 
-in the frontend. 
+This project contains a FastAPI dependency that can be used to decrypt and validate JWTs generated by Auth.js.
+The purpose of this project is to make it easy to use a FastAPI backend in projects that use Next.js and NextAuth / Auth.js 
+in the frontend. It might work with other frameworks using Auth.js too! (But I haven't tested that, feel free to contribute if you do)
 
-Besides JWT decryption and validation, NextAuth compatible cross-site request forgery (CSRF) protection is also implemented.
+Besides JWT decryption and validation, Auth.js compatible cross-site request forgery (CSRF) protection is also implemented.
 
 # Installation
-General usage:
 ```shell
 pip install fastapi-nextauth-jwt
 ```
-Development:
-```shell
-pip install "fastapi-nextauth-jwt[test]"
-```
-
 # Usage
 
 ```python
 from typing import Annotated
 from fastapi import FastAPI, Depends
 from fastapi_nextauth_jwt import NextAuthJWT
 
@@ -48,22 +42,25 @@
 
 @app.get("/")
 async def return_jwt(jwt: Annotated[dict, Depends(JWT)]):
     return jwt
 ```
 
 There are a few configuration options available in the NextAuthJWT constructor, but the most important one is `secret`,
-which should be equivalent to `NEXTAUTH_SECRET` on the Next.js side. A real application would obviously not hardcode the secret like this,
-but rely on the `NEXTAUTH_SECRET` env var.
+which should be equivalent to `NEXTAUTH_SECRET` on the Next.js side. Please don't hardcode the secret like this in a real application,
+but rely on the `NEXTAUTH_SECRET` env var :)
 
 It is also possible to enable or disable CSRF protection using `csrf_prevention_enabled`. 
 If this is not set, this will looks at the ENV environment variable. If this is `dev` then CSRF protection will be disabled.
 It is also possible to customize the HTTP verbs to which CSRF protection is applied.
 
 You should also set the `NEXTAUTH_URL` environment variable, as it is used to determine
-whether or not secure cookies are being used. Or you can set the cookie names manually.
+whether secure cookies are being used. Or you can set the cookie names manually.
+
+## NextAuth / Auth.js v4 compatibility
+A compatibility shim is included if you're still on NextAuth v4, just replace `NexAuthJWT` with `NextAuthJWTv4`
 
 ## Examples
 A [simple example](https://github.com/TCatshoek/fastapi-nextauth-jwt/tree/main/examples/simple) is available in the examples folder. It uses Next.js URL rewrites to direct
 requests to FastAPI. This is just one way to do it, putting both the backend and frontend
 behind something like nginx would also be a good strategy. As long as the cookies can make it to FastAPI
 you should be good to go!
```

