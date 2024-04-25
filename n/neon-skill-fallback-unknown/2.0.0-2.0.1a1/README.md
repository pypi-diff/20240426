# Comparing `tmp/neon-skill-fallback_unknown-2.0.0.tar.gz` & `tmp/neon-skill-fallback_unknown-2.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-fallback_unknown-2.0.0.tar", last modified: Wed Mar 27 20:58:26 2024, max compression
+gzip compressed data, was "neon-skill-fallback_unknown-2.0.1a1.tar", last modified: Thu Apr 25 22:53:08 2024, max compression
```

## Comparing `neon-skill-fallback_unknown-2.0.0.tar` & `neon-skill-fallback_unknown-2.0.1a1.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.835497 neon-skill-fallback_unknown-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-27 20:58:26.835497 neon-skill-fallback_unknown-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.807497 neon-skill-fallback_unknown-2.0.0/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.811498 neon-skill-fallback_unknown-2.0.0/dialog/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ca-es/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ca-es/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ca-es/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ca-es/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.811498 neon-skill-fallback_unknown-2.0.0/dialog/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/cs-cz/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/cs-cz/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/cs-cz/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/cs-cz/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.811498 neon-skill-fallback_unknown-2.0.0/dialog/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/da-dk/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/da-dk/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/da-dk/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/da-dk/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.811498 neon-skill-fallback_unknown-2.0.0/dialog/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/de-de/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/de-de/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/de-de/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/de-de/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.815497 neon-skill-fallback_unknown-2.0.0/dialog/en-us/
--rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/en-us/question.dialog
--rwxr-xr-x   0 runner    (1001) docker     (127)      299 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/en-us/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/en-us/websearch.dialog
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/en-us/who.is.dialog
--rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/en-us/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.815497 neon-skill-fallback_unknown-2.0.0/dialog/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/es-es/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/es-es/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/es-es/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/es-es/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.815497 neon-skill-fallback_unknown-2.0.0/dialog/es-lm/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/es-lm/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/es-lm/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/es-lm/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/es-lm/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.815497 neon-skill-fallback_unknown-2.0.0/dialog/eu-eu/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/eu-eu/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/eu-eu/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/eu-eu/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/eu-eu/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.815497 neon-skill-fallback_unknown-2.0.0/dialog/fa-fa/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fa-fa/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fa-fa/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fa-fa/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fa-fa/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.815497 neon-skill-fallback_unknown-2.0.0/dialog/fa-ir/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fa-ir/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fa-ir/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fa-ir/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fa-ir/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.819497 neon-skill-fallback_unknown-2.0.0/dialog/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fr-fr/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fr-fr/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fr-fr/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/fr-fr/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.819497 neon-skill-fallback_unknown-2.0.0/dialog/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/gl-es/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/gl-es/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/gl-es/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/gl-es/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.819497 neon-skill-fallback_unknown-2.0.0/dialog/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/hu-hu/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/hu-hu/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/hu-hu/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/hu-hu/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.819497 neon-skill-fallback_unknown-2.0.0/dialog/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/it-it/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/it-it/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/it-it/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/it-it/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.819497 neon-skill-fallback_unknown-2.0.0/dialog/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/nl-nl/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/nl-nl/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/nl-nl/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/nl-nl/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.819497 neon-skill-fallback_unknown-2.0.0/dialog/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/pl-pl/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/pl-pl/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/pl-pl/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/pl-pl/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.819497 neon-skill-fallback_unknown-2.0.0/dialog/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/pt-br/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/pt-br/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/pt-br/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/pt-br/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.823497 neon-skill-fallback_unknown-2.0.0/dialog/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ro-ro/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ro-ro/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ro-ro/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ro-ro/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.823497 neon-skill-fallback_unknown-2.0.0/dialog/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ru-ru/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ru-ru/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ru-ru/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/ru-ru/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.823497 neon-skill-fallback_unknown-2.0.0/dialog/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/sv-se/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/sv-se/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/sv-se/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/sv-se/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.823497 neon-skill-fallback_unknown-2.0.0/dialog/uk-ua/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/uk-ua/question.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/uk-ua/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/uk-ua/websearch.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/uk-ua/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/dialog/uk-ua/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.823497 neon-skill-fallback_unknown-2.0.0/neon_skill_fallback_unknown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-27 20:58:26.000000 neon-skill-fallback_unknown-2.0.0/neon_skill_fallback_unknown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-03-27 20:58:26.000000 neon-skill-fallback_unknown-2.0.0/neon_skill_fallback_unknown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 20:58:26.000000 neon-skill-fallback_unknown-2.0.0/neon_skill_fallback_unknown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-27 20:58:26.000000 neon-skill-fallback_unknown-2.0.0/neon_skill_fallback_unknown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-27 20:58:26.000000 neon-skill-fallback_unknown-2.0.0/neon_skill_fallback_unknown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 20:58:26.000000 neon-skill-fallback_unknown-2.0.0/neon_skill_fallback_unknown.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 20:58:26.835497 neon-skill-fallback_unknown-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.823497 neon-skill-fallback_unknown-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.823497 neon-skill-fallback_unknown-2.0.0/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/ui/UnknownIntent.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.811498 neon-skill-fallback_unknown-2.0.0/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.827498 neon-skill-fallback_unknown-2.0.0/vocab/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/ca-es/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/ca-es/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/ca-es/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.827498 neon-skill-fallback_unknown-2.0.0/vocab/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/cs-cz/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/cs-cz/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/cs-cz/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.827498 neon-skill-fallback_unknown-2.0.0/vocab/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/da-dk/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/da-dk/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/da-dk/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.827498 neon-skill-fallback_unknown-2.0.0/vocab/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/de-de/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/de-de/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/de-de/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.827498 neon-skill-fallback_unknown-2.0.0/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/en-us/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/en-us/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/en-us/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.827498 neon-skill-fallback_unknown-2.0.0/vocab/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/es-es/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/es-es/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/es-es/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.827498 neon-skill-fallback_unknown-2.0.0/vocab/es-lm/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/es-lm/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/es-lm/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/es-lm/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.827498 neon-skill-fallback_unknown-2.0.0/vocab/eu-eu/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/eu-eu/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/eu-eu/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/eu-eu/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.827498 neon-skill-fallback_unknown-2.0.0/vocab/fa-fa/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/fa-fa/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/fa-fa/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/fa-fa/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.831498 neon-skill-fallback_unknown-2.0.0/vocab/fa-ir/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/fa-ir/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/fa-ir/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/fa-ir/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.831498 neon-skill-fallback_unknown-2.0.0/vocab/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/fr-fr/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/fr-fr/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/fr-fr/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.831498 neon-skill-fallback_unknown-2.0.0/vocab/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/gl-es/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/gl-es/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/gl-es/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.831498 neon-skill-fallback_unknown-2.0.0/vocab/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/hu-hu/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/hu-hu/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/hu-hu/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.831498 neon-skill-fallback_unknown-2.0.0/vocab/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/it-it/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/it-it/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/it-it/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.831498 neon-skill-fallback_unknown-2.0.0/vocab/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/nl-nl/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/nl-nl/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/nl-nl/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.831498 neon-skill-fallback_unknown-2.0.0/vocab/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/pl-pl/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/pl-pl/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/pl-pl/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.831498 neon-skill-fallback_unknown-2.0.0/vocab/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/pt-br/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/pt-br/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/pt-br/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.831498 neon-skill-fallback_unknown-2.0.0/vocab/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/ro-ro/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/ro-ro/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/ro-ro/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.835497 neon-skill-fallback_unknown-2.0.0/vocab/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/ru-ru/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/ru-ru/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/ru-ru/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.835497 neon-skill-fallback_unknown-2.0.0/vocab/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/sv-se/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/sv-se/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/sv-se/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:58:26.835497 neon-skill-fallback_unknown-2.0.0/vocab/uk-ua/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/uk-ua/question.voc
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/uk-ua/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-27 20:58:24.000000 neon-skill-fallback_unknown-2.0.0/vocab/uk-ua/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.650665 neon-skill-fallback_unknown-2.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-25 22:53:08.650665 neon-skill-fallback_unknown-2.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.626665 neon-skill-fallback_unknown-2.0.1a1/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.630665 neon-skill-fallback_unknown-2.0.1a1/dialog/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ca-es/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ca-es/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ca-es/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ca-es/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.630665 neon-skill-fallback_unknown-2.0.1a1/dialog/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/cs-cz/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/cs-cz/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/cs-cz/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/cs-cz/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.630665 neon-skill-fallback_unknown-2.0.1a1/dialog/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/da-dk/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/da-dk/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/da-dk/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/da-dk/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.630665 neon-skill-fallback_unknown-2.0.1a1/dialog/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/de-de/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/de-de/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/de-de/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/de-de/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.630665 neon-skill-fallback_unknown-2.0.1a1/dialog/en-us/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/en-us/question.dialog
+-rwxr-xr-x   0 runner    (1001) docker     (127)      299 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/en-us/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/en-us/websearch.dialog
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/en-us/who.is.dialog
+-rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/en-us/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.630665 neon-skill-fallback_unknown-2.0.1a1/dialog/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/es-es/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/es-es/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/es-es/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/es-es/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.634666 neon-skill-fallback_unknown-2.0.1a1/dialog/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/es-lm/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/es-lm/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/es-lm/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/es-lm/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.634666 neon-skill-fallback_unknown-2.0.1a1/dialog/eu-eu/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/eu-eu/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/eu-eu/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/eu-eu/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/eu-eu/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.634666 neon-skill-fallback_unknown-2.0.1a1/dialog/fa-fa/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fa-fa/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fa-fa/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fa-fa/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fa-fa/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.634666 neon-skill-fallback_unknown-2.0.1a1/dialog/fa-ir/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fa-ir/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fa-ir/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fa-ir/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fa-ir/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.634666 neon-skill-fallback_unknown-2.0.1a1/dialog/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fr-fr/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fr-fr/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fr-fr/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/fr-fr/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.634666 neon-skill-fallback_unknown-2.0.1a1/dialog/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/gl-es/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/gl-es/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/gl-es/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/gl-es/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.638666 neon-skill-fallback_unknown-2.0.1a1/dialog/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/hu-hu/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/hu-hu/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/hu-hu/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/hu-hu/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.638666 neon-skill-fallback_unknown-2.0.1a1/dialog/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/it-it/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/it-it/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/it-it/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/it-it/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.638666 neon-skill-fallback_unknown-2.0.1a1/dialog/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/nl-nl/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/nl-nl/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/nl-nl/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/nl-nl/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.638666 neon-skill-fallback_unknown-2.0.1a1/dialog/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/pl-pl/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/pl-pl/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/pl-pl/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/pl-pl/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.638666 neon-skill-fallback_unknown-2.0.1a1/dialog/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/pt-br/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/pt-br/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/pt-br/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/pt-br/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.638666 neon-skill-fallback_unknown-2.0.1a1/dialog/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ro-ro/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ro-ro/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ro-ro/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ro-ro/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.638666 neon-skill-fallback_unknown-2.0.1a1/dialog/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ru-ru/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ru-ru/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ru-ru/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/ru-ru/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.642665 neon-skill-fallback_unknown-2.0.1a1/dialog/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/sv-se/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/sv-se/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/sv-se/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/sv-se/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.642665 neon-skill-fallback_unknown-2.0.1a1/dialog/uk-ua/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/uk-ua/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/uk-ua/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/uk-ua/websearch.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/uk-ua/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/dialog/uk-ua/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.642665 neon-skill-fallback_unknown-2.0.1a1/neon_skill_fallback_unknown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-25 22:53:08.000000 neon-skill-fallback_unknown-2.0.1a1/neon_skill_fallback_unknown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-25 22:53:08.000000 neon-skill-fallback_unknown-2.0.1a1/neon_skill_fallback_unknown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 22:53:08.000000 neon-skill-fallback_unknown-2.0.1a1/neon_skill_fallback_unknown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-25 22:53:08.000000 neon-skill-fallback_unknown-2.0.1a1/neon_skill_fallback_unknown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-25 22:53:08.000000 neon-skill-fallback_unknown-2.0.1a1/neon_skill_fallback_unknown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 22:53:08.000000 neon-skill-fallback_unknown-2.0.1a1/neon_skill_fallback_unknown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 22:53:08.650665 neon-skill-fallback_unknown-2.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.642665 neon-skill-fallback_unknown-2.0.1a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.642665 neon-skill-fallback_unknown-2.0.1a1/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/ui/UnknownIntent.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.626665 neon-skill-fallback_unknown-2.0.1a1/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.642665 neon-skill-fallback_unknown-2.0.1a1/vocab/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/ca-es/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/ca-es/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/ca-es/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.642665 neon-skill-fallback_unknown-2.0.1a1/vocab/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/cs-cz/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/cs-cz/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/cs-cz/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.642665 neon-skill-fallback_unknown-2.0.1a1/vocab/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/da-dk/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/da-dk/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/da-dk/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.642665 neon-skill-fallback_unknown-2.0.1a1/vocab/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/de-de/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/de-de/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/de-de/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.646665 neon-skill-fallback_unknown-2.0.1a1/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/en-us/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/en-us/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/en-us/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.646665 neon-skill-fallback_unknown-2.0.1a1/vocab/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/es-es/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/es-es/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/es-es/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.646665 neon-skill-fallback_unknown-2.0.1a1/vocab/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/es-lm/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/es-lm/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/es-lm/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.646665 neon-skill-fallback_unknown-2.0.1a1/vocab/eu-eu/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/eu-eu/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/eu-eu/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/eu-eu/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.646665 neon-skill-fallback_unknown-2.0.1a1/vocab/fa-fa/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/fa-fa/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/fa-fa/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/fa-fa/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.646665 neon-skill-fallback_unknown-2.0.1a1/vocab/fa-ir/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/fa-ir/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/fa-ir/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/fa-ir/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.646665 neon-skill-fallback_unknown-2.0.1a1/vocab/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/fr-fr/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/fr-fr/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/fr-fr/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.646665 neon-skill-fallback_unknown-2.0.1a1/vocab/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/gl-es/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/gl-es/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/gl-es/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.646665 neon-skill-fallback_unknown-2.0.1a1/vocab/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/hu-hu/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/hu-hu/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/hu-hu/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.650665 neon-skill-fallback_unknown-2.0.1a1/vocab/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/it-it/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/it-it/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/it-it/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.650665 neon-skill-fallback_unknown-2.0.1a1/vocab/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/nl-nl/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/nl-nl/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/nl-nl/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.650665 neon-skill-fallback_unknown-2.0.1a1/vocab/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/pl-pl/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/pl-pl/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/pl-pl/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.650665 neon-skill-fallback_unknown-2.0.1a1/vocab/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/pt-br/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/pt-br/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/pt-br/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.650665 neon-skill-fallback_unknown-2.0.1a1/vocab/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/ro-ro/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/ro-ro/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/ro-ro/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.650665 neon-skill-fallback_unknown-2.0.1a1/vocab/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/ru-ru/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/ru-ru/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/ru-ru/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.650665 neon-skill-fallback_unknown-2.0.1a1/vocab/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/sv-se/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/sv-se/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/sv-se/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:08.650665 neon-skill-fallback_unknown-2.0.1a1/vocab/uk-ua/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/uk-ua/question.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/uk-ua/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 22:53:05.000000 neon-skill-fallback_unknown-2.0.1a1/vocab/uk-ua/why.is.voc
```

### Comparing `neon-skill-fallback_unknown-2.0.0/LICENSE` & `neon-skill-fallback_unknown-2.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-2.0.0/LICENSE.md` & `neon-skill-fallback_unknown-2.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-2.0.0/PKG-INFO` & `neon-skill-fallback_unknown-2.0.1a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-fallback_unknown
-Version: 2.0.0
+Version: 2.0.1a1
 Summary: Neon Unknown Fallback Skill
 Home-page: https://github.com/NeonGeckoCom/skill-fallback_unknown
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `neon-skill-fallback_unknown-2.0.0/README.md` & `neon-skill-fallback_unknown-2.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-2.0.0/__init__.py` & `neon-skill-fallback_unknown-2.0.1a1/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-2.0.0/neon_skill_fallback_unknown.egg-info/PKG-INFO` & `neon-skill-fallback_unknown-2.0.1a1/neon_skill_fallback_unknown.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-fallback-unknown
-Version: 2.0.0
+Version: 2.0.1a1
 Summary: Neon Unknown Fallback Skill
 Home-page: https://github.com/NeonGeckoCom/skill-fallback_unknown
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `neon-skill-fallback_unknown-2.0.0/neon_skill_fallback_unknown.egg-info/SOURCES.txt` & `neon-skill-fallback_unknown-2.0.1a1/neon_skill_fallback_unknown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-2.0.0/setup.py` & `neon-skill-fallback_unknown-2.0.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-2.0.0/skill.json` & `neon-skill-fallback_unknown-2.0.1a1/skill.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981884057971016%*

 * *Differences: {"'requirements'": "{'python': {insert: [(2, 'ovos_utils~=0.0,>=0.0.28')], delete: [2]}}"}*

```diff
@@ -22,15 +22,15 @@
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
             "neon-utils~=1.5",
             "ovos-workshop~=0.0.15",
-            "ovos_utils~=0.0.28"
+            "ovos_utils~=0.0,>=0.0.28"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Unknown request fallback handler. Executes if every other step failed to answer the question.",
     "skillname": "skill-fallback_unknown",
     "summary": "Unknown request fallback handler. Executes if every other step failed to answer the question.",
```

### Comparing `neon-skill-fallback_unknown-2.0.0/test/test_skill.py` & `neon-skill-fallback_unknown-2.0.1a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-2.0.0/ui/UnknownIntent.qml` & `neon-skill-fallback_unknown-2.0.1a1/ui/UnknownIntent.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-2.0.0/version.py` & `neon-skill-fallback_unknown-2.0.1a1/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.0"
+__version__ = "2.0.1a1"
```
