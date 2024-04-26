# Comparing `tmp/djehuty-24.3.tar.gz` & `tmp/djehuty-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djehuty-24.3.tar", last modified: Thu Mar 28 16:51:33 2024, max compression
+gzip compressed data, was "djehuty-24.4.tar", last modified: Fri Apr 26 13:35:33 2024, max compression
```

## Comparing `djehuty-24.3.tar` & `djehuty-24.4.tar`

### file list

```diff
@@ -1,338 +1,347 @@
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.945133 djehuty-24.3/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      689 2024-02-01 14:42:06.000000 djehuty-24.3/LICENSE
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      390 2024-02-01 14:42:06.000000 djehuty-24.3/MANIFEST.in
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3553 2024-03-28 16:51:33.945133 djehuty-24.3/PKG-INFO
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2894 2024-02-01 14:42:06.000000 djehuty-24.3/README.md
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.905134 djehuty-24.3/doc/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6256 2024-02-01 14:42:06.000000 djehuty-24.3/doc/contributing.tex
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6289 2024-03-28 16:50:46.000000 djehuty-24.3/doc/djehuty.sty
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6146 2024-02-01 14:42:06.000000 djehuty-24.3/doc/djehuty.tex
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.906134 djehuty-24.3/doc/figures/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13201 2024-02-01 14:42:06.000000 djehuty-24.3/doc/figures/account.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14498 2024-02-01 14:42:06.000000 djehuty-24.3/doc/figures/dataset-container.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17205 2024-02-01 14:42:06.000000 djehuty-24.3/doc/figures/dataset.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13387 2024-02-01 14:42:06.000000 djehuty-24.3/doc/figures/funding.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    97787 2024-02-01 14:42:06.000000 djehuty-24.3/doc/figures/logo.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14790 2024-02-01 14:42:06.000000 djehuty-24.3/doc/figures/rdf-list-abbrev.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    28697 2024-02-01 14:42:06.000000 djehuty-24.3/doc/figures/references-graph.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9279 2024-02-01 14:42:06.000000 djehuty-24.3/doc/figures/typed-literals-notation.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8596 2024-02-01 14:42:06.000000 djehuty-24.3/doc/figures/typed-notation.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3436 2024-02-01 14:42:06.000000 djehuty-24.3/doc/introduction.tex
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4689 2024-02-01 14:42:06.000000 djehuty-24.3/doc/knowledge-graph.tex
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      719 2024-02-01 14:42:06.000000 djehuty-24.3/doc/references.bib
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.906134 djehuty-24.3/etc/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.906134 djehuty-24.3/etc/djehuty/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3195 2024-02-01 14:42:06.000000 djehuty-24.3/etc/djehuty/djehuty-example-config.xml
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      261 2024-02-01 14:42:06.000000 djehuty-24.3/etc/djehuty.service
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      834 2024-03-28 16:50:46.000000 djehuty-24.3/pyproject.toml
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.902134 djehuty-24.3/rpmbuild/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.906134 djehuty-24.3/rpmbuild/SPECS/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1366 2024-03-28 16:50:46.000000 djehuty-24.3/rpmbuild/SPECS/djehuty.spec
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       38 2024-03-28 16:51:33.945133 djehuty-24.3/setup.cfg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       92 2024-02-01 14:42:06.000000 djehuty-24.3/setup.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.902134 djehuty-24.3/src/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.906134 djehuty-24.3/src/djehuty/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/__init__.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.907134 djehuty-24.3/src/djehuty/backup/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    54348 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/backup/database.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    23959 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/backup/figshare.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.909134 djehuty-24.3/src/djehuty/backup/resources/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   947483 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/backup/resources/contributors_organizations.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4941 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/backup/resources/dois.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3073 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/backup/resources/groups.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4870 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/backup/resources/languages.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4397 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/backup/resources/licenses.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    59038 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/backup/resources/public_collections.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    31365 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/backup/resources/root_categories.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8742 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/backup/ui.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6304 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/ui.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.909134 djehuty-24.3/src/djehuty/utils/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1810 2024-03-28 14:55:38.000000 djehuty-24.3/src/djehuty/utils/constants.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8336 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/utils/convenience.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6595 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/utils/rdf.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.911134 djehuty-24.3/src/djehuty/web/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4162 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/cache.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   144409 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/database.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3011 2024-03-08 13:06:17.000000 djehuty-24.3/src/djehuty/web/email_handler.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    26324 2024-03-28 14:55:38.000000 djehuty-24.3/src/djehuty/web/formatter.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1431 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/locks.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.903134 djehuty-24.3/src/djehuty/web/resources/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.914134 djehuty-24.3/src/djehuty/web/resources/html_templates/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      100 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/400.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      117 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/403.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      122 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/404.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      137 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/410.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1041 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/activate_2fa_session.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.915134 djehuty-24.3/src/djehuty/web/resources/html_templates/admin/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      702 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/admin/dashboard.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1620 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/admin/exploratory.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2637 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/admin/maintenance.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2119 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/admin/quota_requests.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.915134 djehuty-24.3/src/djehuty/web/resources/html_templates/admin/reports/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1915 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/admin/reports/dashboard.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2249 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/admin/reports/embargoed_datasets.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2091 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/admin/reports/restricted_datasets.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1616 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/admin/sparql.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2097 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/admin/users.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5068 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/author.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1964 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/badge.svg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4651 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/categories.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2053 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/category.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      695 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/collection.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5232 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/dataset.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1176 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/dataset_access_request.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.916133 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1092 2024-02-15 12:37:40.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/collection-private-links.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4213 2024-02-20 12:24:54.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/dashboard.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1450 2024-02-15 12:37:40.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/dataset-private-links.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14014 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/edit-collection.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    30735 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/edit-dataset.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2405 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/edit-session.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8403 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/language-selector.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3316 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/my-collections.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4956 2024-02-22 12:19:50.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/my-data.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2263 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/new_private_link.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5655 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/profile.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      572 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/published-collection.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      625 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/submitted-for-review.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.917133 djehuty-24.3/src/djehuty/web/resources/html_templates/email/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      188 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/2fa_token.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      129 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/2fa_token.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      450 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/data_access_request.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      334 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/data_access_request.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      557 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/dataset_submitted.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      412 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/dataset_submitted.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      128 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/declined_dataset_notification.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       47 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/declined_dataset_notification.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      209 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/feedback.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      128 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/feedback.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      307 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/layout.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      129 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/published_dataset_notification.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       48 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/published_dataset_notification.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      317 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/quota_request.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      212 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/quota_request.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      451 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/submitted_for_review_notification.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      319 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/email/submitted_for_review_notification.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2910 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/feedback.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4473 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/institutions.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6273 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/layout.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      162 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/maintenance.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1585 2024-03-12 09:27:51.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/opendap_to_doi.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11949 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/portal.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      180 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/private_link_is_expired.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13781 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/public_metadata.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.917133 djehuty-24.3/src/djehuty/web/resources/html_templates/review/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5734 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/review/overview.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      479 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/review/published.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    15962 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/html_templates/search.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.929133 djehuty-24.3/src/djehuty/web/resources/sparql_templates/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1775 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/account_by_email.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2145 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/account_by_session_token.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      969 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/account_categories.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1074 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/account_sessions.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      700 2024-03-12 07:51:39.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/account_storage_used.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      438 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/account_uuid_by_orcid.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3493 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/accounts.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      387 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/append_to_list.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      641 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/associated_authors.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1800 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/author_profile.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1349 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/author_public_items.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2704 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/authors.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2209 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/categories.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      555 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/categories_tree.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      660 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/category_by_id.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1624 2024-02-22 12:19:50.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/collaborators.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      212 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/collection_dataset_containers.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      867 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/collection_datasets.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      301 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/collection_datasets_count.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      908 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/collection_versions.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5885 2024-03-12 07:51:39.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/collections.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      596 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/collections_by_account.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      809 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/collections_from_dataset.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      423 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/contact_info_from_container.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1534 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/container.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1906 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/container_items.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      348 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/container_uuid_by_id.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1282 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/custom_fields.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3555 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/dataset_files.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      277 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/dataset_is_under_review.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1214 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/dataset_statistics.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      781 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/dataset_statistics_timeline.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      374 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/dataset_storage_used.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      919 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/dataset_versions.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    10886 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/datasets.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      634 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/datasets_missing_dois.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1007 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/decline_draft_dataset.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      347 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_account_property.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1038 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_associations.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1101 2024-02-22 12:19:50.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_collaborator.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      870 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_collection_draft.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      826 2024-03-12 07:51:39.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_dataset_draft.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      816 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_dataset_embargo.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      382 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_inactive_session_by_uuid.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      813 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_item_categories.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      760 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_item_from_list.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      647 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_items_all_from_list.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      852 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_private_links.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      365 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_session.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      421 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_session_by_uuid.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      276 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_sessions.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      251 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/derived_from.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      249 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/explorer_properties.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      336 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/explorer_property_types.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      179 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/explorer_types.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1457 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/funding.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      547 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/group.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      490 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/group_by_name.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1000 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/item_collaborative_permissions.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      629 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/latest_datasets_portal.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      476 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/licenses.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      609 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/missing_checksummed_files_for_container.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1274 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/opendap_to_doi.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      254 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/prefixes.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1155 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/private_links.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2394 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/publish_draft_collection.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2803 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/publish_draft_dataset.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      829 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/quota_requests.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      232 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/record_uri.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1188 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/references.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3263 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/reviews.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      703 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/root_categories.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      463 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/search_tags.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      389 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/statistics.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      329 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/statistics_authors.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      485 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/statistics_collections.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      473 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/statistics_datasets.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      299 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/statistics_files.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      718 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/subcategories_by_category.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1332 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/tags.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5688 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_account.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5781 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_collection.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11656 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_dataset.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1022 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_dataset_thumb.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      422 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_doi_after_publishing.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4214 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_file.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      560 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_git_uuid.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      846 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_orcid_for_account.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1670 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_private_link.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1696 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_quota_request.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1279 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_review.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1008 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_session.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1699 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_view_and_download_counts.sparql
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.903134 djehuty-24.3/src/djehuty/web/resources/static/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.930133 djehuty-24.3/src/djehuty/web/resources/static/css/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9840 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/css/dropzone.min.css
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4997 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/css/form.css
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13823 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/css/jquery.dataTables.min.css
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17776 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/static/css/main.css
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4090 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/css/pub.css
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    24375 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/css/quill.4tu.css
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.932133 djehuty-24.3/src/djehuty/web/resources/static/fonts/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   174632 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/FiraMono-Regular.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   247784 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/SourceSansPro-Bold.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   109604 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/SourceSansPro-Italic.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   248504 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/SourceSansPro-Regular.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   208302 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-brands-400.eot
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   207972 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-brands-400.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   120496 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-brands-400.woff
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   117400 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-brands-400.woff2
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   420030 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-solid-900.eot
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   419720 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-solid-900.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   170112 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-solid-900.woff
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   156496 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-solid-900.woff2
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.935133 djehuty-24.3/src/djehuty/web/resources/static/images/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   136306 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/CoreTrustSeal.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1838 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/collection-thumb.svg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3137 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/dataset-thumb.svg
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.935133 djehuty-24.3/src/djehuty/web/resources/static/images/datatables/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      160 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/datatables/sort_asc.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      148 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/datatables/sort_asc_disabled.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      201 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/datatables/sort_both.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      158 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/datatables/sort_desc.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      146 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/datatables/sort_desc_disabled.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1817 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/ext-link.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   156038 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/favicon.ico
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3519 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/favicon.png
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.936133 djehuty-24.3/src/djehuty/web/resources/static/images/licenses/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5427 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/licenses/apache.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2672 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-0.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1773 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by-nc-nd.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1888 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by-nc-sa.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1709 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by-nc.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1562 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by-nd.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1697 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by-sa.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1468 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2666 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/licenses/gnu-gpl-v3.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3427 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/loader.svg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13671 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/logo-delft.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5737 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/logo-eindhoven.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    29080 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/logo-gray.svg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4815 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/logo-other.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     7852 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/logo-twente.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4593 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/logo-wageningen.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17172 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/logo.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      539 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/logosleft-white-tudelft.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      479 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/logosleft-white-tueindhoven.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      920 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/logosleft-white-tutwente.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      764 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/logosleft-white-wageningen.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2311 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/nikhef-black.svg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      967 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/orcid.svg
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.941133 djehuty-24.3/src/djehuty/web/resources/static/images/portal/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    45036 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/aerospace-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    56826 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/agricultural-and-veterinary-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    32670 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/atmospheric-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    64498 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/biology.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    67098 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/built-environment-and-design.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    48523 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/business-and-management.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    74133 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/chemistry.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    45270 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/civil-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    56936 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/earth-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    57174 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/electrical-and-electronic-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    46321 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/environmental-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    47125 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/geomatic-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    81026 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/information-and-computing-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    71960 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/materials-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    43103 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/mathematics.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    40696 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/mechanical-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    46816 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/medical-and-health-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    75625 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/nanotechnology.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8616 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/other-institutions.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    38216 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/physical-geography-and-environmental-geoscience.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    50449 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/physics.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13023 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/tudelft.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17442 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/tueindhoven.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9400 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/utwente.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    16609 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/images/portal/wageningen.jpg
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.943133 djehuty-24.3/src/djehuty/web/resources/static/js/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.944133 djehuty-24.3/src/djehuty/web/resources/static/js/ace/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   371331 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/ace/ace.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    39763 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/ace/ext-language_tools.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11910 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/ace/ext-searchbox.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8183 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/ace/mode-sparql.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3150 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/ace/theme-crimson_editor.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   275533 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/d3.v7.min.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2556 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/dataset_landing_page.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1427 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/depositor-dashboard.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   114702 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/dropzone.min.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    24869 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/edit-collection.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    57946 2024-02-22 12:19:50.000000 djehuty-24.3/src/djehuty/web/resources/static/js/edit-dataset.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3600 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/edit-profile.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6093 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/exploratory.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    89501 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    88377 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/jquery.dataTables.min.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3519 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/query-editor.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   327924 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/quill.min.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3027 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/resources/static/js/ranking.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4167 2024-03-08 13:06:17.000000 djehuty-24.3/src/djehuty/web/resources/static/js/review-overview.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    29712 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/resources/static/js/search.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8362 2024-02-22 12:19:50.000000 djehuty-24.3/src/djehuty/web/resources/static/js/utils.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    46697 2024-03-27 09:02:41.000000 djehuty-24.3/src/djehuty/web/ui.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    16169 2024-03-08 13:06:17.000000 djehuty-24.3/src/djehuty/web/validator.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   401480 2024-03-28 16:46:13.000000 djehuty-24.3/src/djehuty/web/wsgi.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14835 2024-02-01 14:42:06.000000 djehuty-24.3/src/djehuty/web/xml_formatter.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-03-28 16:51:33.945133 djehuty-24.3/src/djehuty.egg-info/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3553 2024-03-28 16:51:33.000000 djehuty-24.3/src/djehuty.egg-info/PKG-INFO
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17927 2024-03-28 16:51:33.000000 djehuty-24.3/src/djehuty.egg-info/SOURCES.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        1 2024-03-28 16:51:33.000000 djehuty-24.3/src/djehuty.egg-info/dependency_links.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       44 2024-03-28 16:51:33.000000 djehuty-24.3/src/djehuty.egg-info/entry_points.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        8 2024-03-28 16:51:33.000000 djehuty-24.3/src/djehuty.egg-info/top_level.txt
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.559275 djehuty-24.4/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      689 2024-02-01 14:42:06.000000 djehuty-24.4/LICENSE
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      390 2024-02-01 14:42:06.000000 djehuty-24.4/MANIFEST.in
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3553 2024-04-26 13:35:33.559275 djehuty-24.4/PKG-INFO
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2894 2024-02-01 14:42:06.000000 djehuty-24.4/README.md
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.532276 djehuty-24.4/doc/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6256 2024-02-01 14:42:06.000000 djehuty-24.4/doc/contributing.tex
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6289 2024-04-26 13:34:55.000000 djehuty-24.4/doc/djehuty.sty
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6146 2024-02-01 14:42:06.000000 djehuty-24.4/doc/djehuty.tex
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.533276 djehuty-24.4/doc/figures/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13201 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/account.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14498 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/dataset-container.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17205 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/dataset.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13387 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/funding.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    97787 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/logo.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14790 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/rdf-list-abbrev.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    28697 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/references-graph.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9279 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/typed-literals-notation.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8596 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/typed-notation.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3436 2024-02-01 14:42:06.000000 djehuty-24.4/doc/introduction.tex
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4689 2024-02-01 14:42:06.000000 djehuty-24.4/doc/knowledge-graph.tex
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      719 2024-02-01 14:42:06.000000 djehuty-24.4/doc/references.bib
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.533276 djehuty-24.4/etc/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.533276 djehuty-24.4/etc/djehuty/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3616 2024-04-24 20:01:44.000000 djehuty-24.4/etc/djehuty/djehuty-example-config.xml
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      338 2024-04-24 20:01:44.000000 djehuty-24.4/etc/djehuty.service
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      834 2024-04-26 13:34:55.000000 djehuty-24.4/pyproject.toml
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.530276 djehuty-24.4/rpmbuild/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.533276 djehuty-24.4/rpmbuild/SPECS/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1366 2024-04-26 13:34:55.000000 djehuty-24.4/rpmbuild/SPECS/djehuty.spec
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       38 2024-04-26 13:35:33.559275 djehuty-24.4/setup.cfg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       92 2024-02-01 14:42:06.000000 djehuty-24.4/setup.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.531276 djehuty-24.4/src/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.533276 djehuty-24.4/src/djehuty/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/__init__.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.534276 djehuty-24.4/src/djehuty/backup/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    54348 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/database.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    23959 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/figshare.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.535276 djehuty-24.4/src/djehuty/backup/resources/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   947483 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/contributors_organizations.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4941 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/dois.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3073 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/groups.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4870 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/languages.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4397 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/licenses.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    59038 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/public_collections.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    31365 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/root_categories.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8742 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/ui.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6304 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/ui.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.535276 djehuty-24.4/src/djehuty/utils/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2084 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/utils/constants.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8336 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/utils/convenience.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6595 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/utils/rdf.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.536276 djehuty-24.4/src/djehuty/web/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4162 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/cache.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   146479 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/database.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3011 2024-03-08 13:06:17.000000 djehuty-24.4/src/djehuty/web/email_handler.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    26886 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/formatter.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1431 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/locks.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.531276 djehuty-24.4/src/djehuty/web/resources/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.538276 djehuty-24.4/src/djehuty/web/resources/html_templates/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      100 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/400.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      117 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/403.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      122 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/404.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      137 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/410.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1041 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/activate_2fa_session.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.539276 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      702 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/dashboard.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1666 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/exploratory.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2637 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/maintenance.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2119 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/quota_requests.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.539276 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1915 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/dashboard.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2249 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/embargoed_datasets.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2091 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/restricted_datasets.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1616 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/sparql.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2778 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/users.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5068 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/author.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1966 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/badge.svg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4651 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/categories.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2053 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/category.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      695 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/collection.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2790 2024-04-26 13:32:51.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/colors.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4530 2024-04-26 13:32:51.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/dataset.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1176 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/dataset_access_request.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.540276 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1092 2024-02-15 12:37:40.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/collection-private-links.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4216 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/dashboard.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1450 2024-02-15 12:37:40.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/dataset-private-links.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13903 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-collection.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    31761 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-dataset.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2405 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-session.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8403 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/language-selector.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3319 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/my-collections.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4959 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/my-data.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2263 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/new_private_link.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5658 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/profile.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      572 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/published-collection.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      625 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/submitted-for-review.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.542276 djehuty-24.4/src/djehuty/web/resources/html_templates/email/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      188 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/2fa_token.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      129 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/2fa_token.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      450 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/data_access_request.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      334 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/data_access_request.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      887 2024-04-26 13:03:07.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_approved.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      691 2024-04-26 13:03:07.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_approved.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      401 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_declined.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      274 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_declined.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      557 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_submitted.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      412 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_submitted.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      291 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/declined_dataset_notification.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      158 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/declined_dataset_notification.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      209 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/feedback.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      128 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/feedback.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      345 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/layout.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      292 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/published_dataset_notification.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      159 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/published_dataset_notification.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      439 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/quota_approved.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      316 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/quota_approved.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      317 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/quota_request.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      212 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/quota_request.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      451 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/submitted_for_review_notification.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      319 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/submitted_for_review_notification.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2910 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/feedback.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      256 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/git_instructions.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4465 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/institutions.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6362 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/layout.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3547 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/loader.svg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      162 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/maintenance.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1585 2024-03-12 09:27:51.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/opendap_to_doi.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11949 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/portal.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      180 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/private_link_is_expired.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13781 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/public_metadata.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.542276 djehuty-24.4/src/djehuty/web/resources/html_templates/review/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5734 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/review/overview.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      479 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/review/published.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    15954 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/search.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.549276 djehuty-24.4/src/djehuty/web/resources/sparql_templates/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1775 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_by_email.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2145 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_by_session_token.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      969 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_categories.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1074 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_sessions.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      700 2024-03-12 07:51:39.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_storage_used.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      438 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_uuid_by_orcid.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3493 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/accounts.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      387 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/append_to_list.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      641 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/associated_authors.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1800 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/author_profile.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1349 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/author_public_items.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3119 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/authors.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2209 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/categories.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      555 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/categories_tree.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      660 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/category_by_id.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1624 2024-02-22 12:19:50.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collaborators.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      212 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_dataset_containers.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      867 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_datasets.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      301 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_datasets_count.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      908 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_versions.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5885 2024-03-12 07:51:39.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      596 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections_by_account.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      809 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections_from_dataset.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      423 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/contact_info_from_container.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1534 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/container.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1906 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/container_items.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      348 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/container_uuid_by_id.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1282 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/custom_fields.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3555 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_files.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      277 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_is_under_review.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1214 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_statistics.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      781 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_statistics_timeline.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      374 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_storage_used.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      919 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_versions.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    10888 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/datasets.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      634 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/datasets_missing_dois.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1007 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/decline_draft_dataset.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      347 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_account_property.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1038 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_associations.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1101 2024-02-22 12:19:50.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_collaborator.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      870 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_collection_draft.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      826 2024-03-12 07:51:39.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_dataset_draft.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      816 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_dataset_embargo.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      382 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_inactive_session_by_uuid.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      813 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_item_categories.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      760 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_item_from_list.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      647 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_items_all_from_list.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      852 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_private_links.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      365 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_session.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      421 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_session_by_uuid.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      276 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_sessions.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      251 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/derived_from.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      249 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/explorer_properties.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      336 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/explorer_property_types.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      179 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/explorer_types.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1457 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/funding.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      547 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/group.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      490 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/group_by_name.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1000 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/item_collaborative_permissions.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      629 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/latest_datasets_portal.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      476 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/licenses.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      609 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/missing_checksummed_files_for_container.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1274 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/opendap_to_doi.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      254 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/prefixes.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1155 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/private_links.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2418 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/publish_draft_collection.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2827 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/publish_draft_dataset.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      945 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/quota_requests.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      232 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/record_uri.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1188 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/references.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3263 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/reviews.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      703 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/root_categories.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      463 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/search_tags.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      389 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/statistics.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      329 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/statistics_authors.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      485 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/statistics_collections.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      473 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/statistics_datasets.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      955 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/statistics_files.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      718 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/subcategories_by_category.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1332 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/tags.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5688 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_account.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1982 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_author.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5781 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_collection.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11656 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_dataset.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1022 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_dataset_thumb.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      422 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_doi_after_publishing.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4214 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_file.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      560 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_git_uuid.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      846 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_orcid_for_account.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1670 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_private_link.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1696 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_quota_request.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1279 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_review.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1008 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_session.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1699 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_view_and_download_counts.sparql
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.531276 djehuty-24.4/src/djehuty/web/resources/static/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.549276 djehuty-24.4/src/djehuty/web/resources/static/css/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9840 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/css/dropzone.min.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5058 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/static/css/form.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13823 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/css/jquery.dataTables.min.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    16381 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/static/css/main.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3791 2024-04-26 13:32:51.000000 djehuty-24.4/src/djehuty/web/resources/static/css/pub.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    24375 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/css/quill.4tu.css
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.552276 djehuty-24.4/src/djehuty/web/resources/static/fonts/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   174632 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/FiraMono-Regular.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   247784 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Bold.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   109604 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Italic.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   248504 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Regular.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   208302 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.eot
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   207972 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   120496 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.woff
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   117400 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.woff2
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   420030 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.eot
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   419720 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   170112 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.woff
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   156496 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.woff2
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.553276 djehuty-24.4/src/djehuty/web/resources/static/images/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   136306 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/CoreTrustSeal.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1838 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/collection-thumb.svg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3137 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/dataset-thumb.svg
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.554276 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      160 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/sort_asc.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      148 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/sort_asc_disabled.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      201 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/sort_both.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      158 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/sort_desc.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      146 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/sort_desc_disabled.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1817 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/ext-link.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   156038 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/favicon.ico
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3519 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/favicon.png
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.554276 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5427 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/apache.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2672 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-0.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1773 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc-nd.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1888 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc-sa.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1709 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1562 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nd.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1697 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-sa.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1468 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2666 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/gnu-gpl-v3.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13671 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-delft.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5737 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-eindhoven.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    29080 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-gray.svg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4815 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-other.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     7852 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-twente.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4593 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-wageningen.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17172 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      539 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-tudelft.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      479 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-tueindhoven.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      920 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-tutwente.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      764 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-wageningen.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2311 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/nikhef-black.svg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      967 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/orcid.svg
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.557276 djehuty-24.4/src/djehuty/web/resources/static/images/portal/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    45036 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/aerospace-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    56826 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/agricultural-and-veterinary-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    32670 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/atmospheric-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    64498 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/biology.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    67098 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/built-environment-and-design.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    48523 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/business-and-management.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    74133 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/chemistry.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    45270 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/civil-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    56936 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/earth-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    57174 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/electrical-and-electronic-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    46321 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/environmental-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    47125 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/geomatic-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    81026 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/information-and-computing-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    71960 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/materials-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    43103 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/mathematics.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    40696 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/mechanical-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    46816 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/medical-and-health-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    75625 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/nanotechnology.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8616 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/other-institutions.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    38216 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/physical-geography-and-environmental-geoscience.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    50449 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/physics.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13023 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/tudelft.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17442 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/tueindhoven.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9400 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/utwente.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    16609 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/wageningen.jpg
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.558276 djehuty-24.4/src/djehuty/web/resources/static/js/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.559275 djehuty-24.4/src/djehuty/web/resources/static/js/ace/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   371331 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ace/ace.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    39763 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ace/ext-language_tools.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11910 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ace/ext-searchbox.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8183 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ace/mode-sparql.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3150 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ace/theme-crimson_editor.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   275533 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/d3.v7.min.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2556 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/dataset_landing_page.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1427 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/depositor-dashboard.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   114702 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/dropzone.min.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    24869 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/edit-collection.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    61653 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/static/js/edit-dataset.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3600 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/edit-profile.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6093 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/exploratory.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    89501 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    88377 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3519 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/query-editor.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   327924 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/quill.min.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3027 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ranking.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4167 2024-03-08 13:06:17.000000 djehuty-24.4/src/djehuty/web/resources/static/js/review-overview.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    29712 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/static/js/search.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8788 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/static/js/utils.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    47651 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/ui.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    16169 2024-03-08 13:06:17.000000 djehuty-24.4/src/djehuty/web/validator.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   415838 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/wsgi.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14835 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/xml_formatter.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.559275 djehuty-24.4/src/djehuty.egg-info/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3553 2024-04-26 13:35:33.000000 djehuty-24.4/src/djehuty.egg-info/PKG-INFO
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    18514 2024-04-26 13:35:33.000000 djehuty-24.4/src/djehuty.egg-info/SOURCES.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        1 2024-04-26 13:35:33.000000 djehuty-24.4/src/djehuty.egg-info/dependency_links.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       44 2024-04-26 13:35:33.000000 djehuty-24.4/src/djehuty.egg-info/entry_points.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        8 2024-04-26 13:35:33.000000 djehuty-24.4/src/djehuty.egg-info/top_level.txt
```

### Comparing `djehuty-24.3/LICENSE` & `djehuty-24.4/LICENSE`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/PKG-INFO` & `djehuty-24.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djehuty
-Version: 24.3
+Version: 24.4
 Summary: The 4TU.ResearchData repository system
 Author-email: Roel Janssen <r.r.e.janssen@tudelft.nl>
 Project-URL: Homepage, https://data.4tu.nl
 Project-URL: Source Code, https://github.com/4TUResearchData/djehuty
 Project-URL: Bug Tracker, https://github.com/4TUResearchData/djehuty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `djehuty-24.3/README.md` & `djehuty-24.4/README.md`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/contributing.tex` & `djehuty-24.4/doc/contributing.tex`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/djehuty.sty` & `djehuty-24.4/doc/djehuty.sty`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 \definecolor{DarkGray}{rgb}{0.40, 0.40, 0.40}
 
 % When highlighting text, make sure the highlighting box doesn't
 % add padding space.
 \setlength{\fboxsep}{0pt}
 
 %% Create a variable that holds the current version of djehuty.
-\def \djehutyversion {24.3}
+\def \djehutyversion {24.4}
 
 \newcommand\VRule[1][\arrayrulewidth]{\vrule width #1}
 \newcommand{\oddcell}{\cellcolor{OddRowColor}}
 \newcommand{\oddrow}{\rowcolor{OddRowColor}}
 \newcommand{\evenrow}{\rowcolor{EvenRowColor}}
 \newcommand{\headrow}{\rowcolor{Gray}}
 \newcommand{\B}{$\bullet{}$}
```

### Comparing `djehuty-24.3/doc/djehuty.tex` & `djehuty-24.4/doc/djehuty.tex`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/figures/account.pdf` & `djehuty-24.4/doc/figures/account.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/figures/dataset-container.pdf` & `djehuty-24.4/doc/figures/dataset-container.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/figures/dataset.pdf` & `djehuty-24.4/doc/figures/dataset.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/figures/funding.pdf` & `djehuty-24.4/doc/figures/funding.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/figures/logo.pdf` & `djehuty-24.4/doc/figures/logo.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/figures/rdf-list-abbrev.pdf` & `djehuty-24.4/doc/figures/rdf-list-abbrev.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/figures/references-graph.pdf` & `djehuty-24.4/doc/figures/references-graph.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/figures/typed-literals-notation.pdf` & `djehuty-24.4/doc/figures/typed-literals-notation.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/figures/typed-notation.pdf` & `djehuty-24.4/doc/figures/typed-notation.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/introduction.tex` & `djehuty-24.4/doc/introduction.tex`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/knowledge-graph.tex` & `djehuty-24.4/doc/knowledge-graph.tex`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/doc/references.bib` & `djehuty-24.4/doc/references.bib`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/etc/djehuty/djehuty-example-config.xml` & `djehuty-24.4/etc/djehuty/djehuty-example-config.xml`

 * *Files 14% similar despite different names*

#### Comparing `djehuty-24.3/etc/djehuty/djehuty-example-config.xml` & `djehuty-24.4/etc/djehuty/djehuty-example-config.xml`

```diff
@@ -1,12 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
 <djehuty>
   <maintenance-mode>0</maintenance-mode>
   <site-name>Djehuty example instance</site-name>
+  <site-shorttag>example-shorttag</site-shorttag>
   <site-description>Djehuty example instance</site-description>
+  <support-email-address>support@example.com</support-email-address>
+  <colors>
+    <primary-color>#f49120</primary-color>
+    <primary-color-hover>#d26000</primary-color-hover>
+    <primary-color-active>#9d4800</primary-color-active>
+    <privilege-button-color>#fce3bf</privilege-button-color>
+    <footer-background-color>#707070</footer-background-color>
+  </colors>
   <small-footer>
     <div id="footer-wrapper2">
       <p>
         This repository is powered by
         <a href="https://github.com/4TUResearchData/djehuty">djehuty</a>
         built for
         <a href="https://data.4tu.nl">4TU.ResearchData</a>
```

### Comparing `djehuty-24.3/pyproject.toml` & `djehuty-24.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend   = "setuptools.build_meta"
 
 [project]
 name            = "djehuty"
-version         = "24.3"
+version         = "24.4"
 authors         = [{ name="Roel Janssen", email="r.r.e.janssen@tudelft.nl" }]
 description     = "The 4TU.ResearchData repository system"
 readme          = "README.md"
 requires-python = ">=3.7"
 classifiers     = [
     "Programming Language :: Python :: 3",
     "Environment :: Web Environment",
```

### Comparing `djehuty-24.3/rpmbuild/SPECS/djehuty.spec` & `djehuty-24.4/rpmbuild/SPECS/djehuty.spec`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:        djehuty
-Version:     24.3
+Version:     24.4
 Release:     1%{?dist}
 Summary:     Repository system for 4TU.ResearchData
 Source0:     %{name}-%{version}.tar.gz
 License:     AGPLv3+
 Group:       System Environment/Daemons
 BuildRoot:   %{_tmppath}/%{name}-%{version}-%{release}-buildroot
 Prefix:      %{_prefix}
@@ -44,11 +44,11 @@
 %clean
 rm -rf $RPM_BUILD_ROOT
 
 %files
 %defattr(-,root,root)
 %doc README.md
 %{python3_sitelib}/%{name}/
-%{python3_sitelib}/%{name}-24.3*
+%{python3_sitelib}/%{name}-24.4*
 %{_unitdir}/%{name}.service
 /etc/%{name}/djehuty-example-config.xml
 /usr/bin/djehuty
```

### Comparing `djehuty-24.3/src/djehuty/backup/database.py` & `djehuty-24.4/src/djehuty/backup/database.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/backup/figshare.py` & `djehuty-24.4/src/djehuty/backup/figshare.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/backup/resources/contributors_organizations.json` & `djehuty-24.4/src/djehuty/backup/resources/contributors_organizations.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/backup/resources/dois.json` & `djehuty-24.4/src/djehuty/backup/resources/dois.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/backup/resources/groups.json` & `djehuty-24.4/src/djehuty/backup/resources/groups.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/backup/resources/languages.json` & `djehuty-24.4/src/djehuty/backup/resources/languages.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/backup/resources/licenses.json` & `djehuty-24.4/src/djehuty/backup/resources/licenses.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/backup/resources/public_collections.json` & `djehuty-24.4/src/djehuty/backup/resources/public_collections.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/backup/resources/root_categories.json` & `djehuty-24.4/src/djehuty/backup/resources/root_categories.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/backup/ui.py` & `djehuty-24.4/src/djehuty/backup/ui.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/ui.py` & `djehuty-24.4/src/djehuty/ui.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/utils/constants.py` & `djehuty-24.4/src/djehuty/utils/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,48 +13,58 @@
                      'eindhoven' : 'Eindhoven_University_of_Technology',
                      'twente'    : 'University_of_Twente',
                      'wageningen': 'Wageningen_University_and_Research',
                      'other'     : 'Other_institutions' }
 
 filetypes_by_extension = {
     "bash":       "Shell",
-    "bib":        "La(TeX)",
+    "bib":        "TeX",
     "c":          "C",
     "cc":         "C++",
     "cpp":        "C++",
     "cs":         "C#",
     "css":        "CSS",
     "cxx":        "C++",
     "d":          "D",
+    "f":          "Fortran",
+    "f77":        "Fortran",
+    "f90":        "Fortran",
+    "for":        "Fortran",
     "geojson":    "JSON",
     "go":         "Go",
     "gohtml":     "Go",
     "h":          "C",
     "hpp":        "C++",
+    "hs":         "Haskell",
+    "html":       "HTML",
+    "htm":        "HTML",
     "hxx":        "C++",
     "in":         "Automake",
     "ipynb":      "Jupyter Notebook",
     "java":       "Java",
+    "jl":         "Julia",
     "js":         "JavaScript",
     "json":       "JSON",
     "m":          "Matlab",
+    "mat":        "Matlab",
     "md":         "Markdown",
     "mts":        "TypeScript",
     "mysql":      "SQL",
     "php":        "PHP",
     "pl":         "Perl",
     "pm":         "Perl",
     "py":         "Python",
     "r":          "R",
     "rb":         "Ruby",
     "rs":         "Rust",
     "sh":         "Shell",
     "sparql":     "SPARQL",
     "sql":        "SQL",
-    "sty":        "La(TeX)",
-    "tex":        "La(TeX)",
+    "sty":        "TeX",
+    "tex":        "TeX",
     "ts":         "TypeScript",
     "tsx":        "TypeScript",
     "xml":        "XML",
+    "xyz":        "Chemical XYZ",
     "yaml":       "YAML",
     "yml":        "YAML",
 }
```

### Comparing `djehuty-24.3/src/djehuty/utils/convenience.py` & `djehuty-24.4/src/djehuty/utils/convenience.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/utils/rdf.py` & `djehuty-24.4/src/djehuty/utils/rdf.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/cache.py` & `djehuty-24.4/src/djehuty/web/cache.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/database.py` & `djehuty-24.4/src/djehuty/web/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,28 +444,38 @@
         return self.__run_query (query)
 
     def datasets_missing_dois (self):
         """Procedure to retrieve datasets where a DOI registration went wrong."""
         query = self.__query_from_template ("datasets_missing_dois")
         return self.__run_query (query)
 
+    def repository_file_statistics (self, extended_properties=False, use_cache=False):
+        """Returns files and their sizes, and optionally more properties."""
+        query = self.__query_from_template ("statistics_files", {
+            "extended_properties": extended_properties
+        })
+
+        if use_cache:
+            return self.__run_query (query, query, "repository_statistics")
+
+        return self.__run_query (query)
+
     def repository_statistics (self):
         """Procedure to retrieve repository-wide statistics."""
 
         datasets_query    = self.__query_from_template ("statistics_datasets")
         collections_query = self.__query_from_template ("statistics_collections")
         authors_query     = self.__query_from_template ("statistics_authors")
-        files_query       = self.__query_from_template ("statistics_files")
 
         row = { "datasets": 0, "authors": 0, "collections": 0, "files": 0, "bytes": 0 }
         try:
             datasets    = self.__run_query (datasets_query, datasets_query, "repository_statistics")
             authors     = self.__run_query (authors_query, authors_query, "repository_statistics")
             collections = self.__run_query (collections_query, collections_query, "repository_statistics")
-            files       = self.__run_query (files_query, files_query, "repository_statistics")
+            files       = self.repository_file_statistics (use_cache=True)
             number_of_files = 0
             number_of_bytes = 0
             for entry in files:
                 number_of_files += 1
                 number_of_bytes += int(float(entry["bytes"]))
 
             files_results = {
@@ -564,15 +574,16 @@
             return None
 
     def authors (self, first_name=None, full_name=None, group_id=None,
                  author_id=None, institution_id=None, is_active=None,
                  is_public=None, job_title=None, last_name=None,
                  orcid_id=None, url_name=None, limit=10, order="order_index",
                  order_direction="asc", item_uri=None, search_for=None,
-                 account_uuid=None, item_type="dataset", is_published=True):
+                 account_uuid=None, item_type="dataset", is_published=True,
+                 author_uuid=None):
         """Procedure to retrieve authors of a dataset."""
 
         prefix = item_type.capitalize()
 
         filters  = rdf.sparql_filter ("group_id",       group_id)
         filters += rdf.sparql_filter ("id",             author_id)
         filters += rdf.sparql_filter ("institution_id", institution_id)
@@ -594,14 +605,15 @@
 
         query = self.__query_from_template ("authors", {
             "item_type":   item_type,
             "prefix":      prefix,
             "is_published": is_published,
             "item_uri":    item_uri,
             "account_uuid": account_uuid,
+            "author_uuid": author_uuid,
             "filters":     filters
         })
         query += rdf.sparql_suffix (order, order_direction, limit, None)
 
         return self.__run_query(query)
 
     def author_profile (self, author_uri):
@@ -1317,22 +1329,25 @@
             "status": None if status_uri is None else rdf.urify_value (status_uri),
             "assign_to_account": status == "approved"
         })
 
         self.cache.invalidate_by_prefix ("accounts")
         return self.__run_logged_query (query)
 
-    def quota_requests (self, status=None):
+    def quota_requests (self, status=None, quota_request_uuid=None):
         """Procedure to return a list of quota requests."""
 
         status_uri = None
         if status is not None:
             status_uri = rdf.urify_value (rdf.DJHT[f"QuotaRequest{status.capitalize()}"])
 
-        query = self.__query_from_template ("quota_requests", { "status": status_uri })
+        query = self.__query_from_template ("quota_requests", {
+            "status": status_uri,
+            "quota_request_uuid": quota_request_uuid
+        })
         return self.__run_query (query)
 
     def update_account (self, account_uuid, active=None, email=None, job_title=None,
                         first_name=None, last_name=None, institution_user_id=None,
                         institution_id=None,
                         maximum_file_size=None, modified_date=None, created_date=None,
                         location=None, biography=None, categories=None, twitter=None,
@@ -1959,20 +1974,22 @@
                                        use_cache      = False)[0]
             new_version_number = latest["version"] + 1
         except IndexError:
             self.log.error ("No latest version for <container:%s>.", container_uuid)
 
         collection_uuid = draft["uuid"]
         blank_node   = self.wrap_in_blank_node (collection_uuid, "collection")
+        current_time = datetime.strftime (datetime.now(), "%Y-%m-%dT%H:%M:%SZ")
         query        = self.__query_from_template ("publish_draft_collection", {
             "account_uuid":      account_uuid,
             "blank_node":        blank_node,
             "version":           new_version_number,
             "container_uuid":    container_uuid,
             "collection_uuid":   collection_uuid,
+            "timestamp":         current_time,
             "first_publication": not latest
         })
 
         return bool(self.__run_logged_query (query))
 
     def create_draft_from_published_collection (self, container_uuid):
         """Procedure to copy a published collection as draft in its container."""
@@ -2077,19 +2094,21 @@
                                     use_cache      = False)[0]
             new_version_number = latest["version"] + 1
         except IndexError:
             self.log.error ("No latest version for <container:%s>.", container_uuid)
 
         dataset_uuid = draft["uuid"]
         blank_node   = self.wrap_in_blank_node (dataset_uuid, "dataset")
+        current_time = datetime.strftime (datetime.now(), "%Y-%m-%dT%H:%M:%SZ")
         query        = self.__query_from_template ("publish_draft_dataset", {
             "blank_node":        blank_node,
             "version":           new_version_number,
             "container_uuid":    container_uuid,
             "dataset_uuid":      dataset_uuid,
+            "timestamp":         current_time,
             "first_publication": not latest
         })
 
         if self.__run_logged_query (query):
             self.cache.invalidate_by_prefix ("repository_statistics")
             self.cache.invalidate_by_prefix ("reviews")
             self.cache.invalidate_by_prefix (f"datasets_{account_uuid}")
@@ -2207,14 +2226,35 @@
         rdf.add (graph, container_uri, rdf.DJHT["draft"], draft_uri, "uri")
 
         if self.add_triples_from_graph (graph):
             return draft_uuid
 
         return None
 
+    def update_author (self, author_uuid, created_by, first_name, last_name, email, orcid):
+        """Update the author record identified by AUTHOR_UUID, CREATED_BY."""
+
+        full_name = None
+        if first_name is not None and last_name is not None:
+            full_name = f"{first_name} {last_name}"
+
+        current_time = datetime.strftime (datetime.now(), "%Y-%m-%dT%H:%M:%S")
+        query = self.__query_from_template ("update_author", {
+            "author_uuid": author_uuid,
+            "created_by": created_by,
+            "full_name": rdf.escape_string_value (full_name),
+            "first_name": rdf.escape_string_value (first_name),
+            "last_name": rdf.escape_string_value (last_name),
+            "email": rdf.escape_string_value (email),
+            "orcid": rdf.escape_string_value (self.__normalize_orcid (orcid)),
+            "modified_date": rdf.escape_datetime_value (current_time)
+        })
+
+        return self.__run_query (query)
+
     def update_dataset (self, dataset_uuid, account_uuid, title=None,
                         description=None, resource_doi=None, doi=None,
                         resource_title=None, license_url=None, group_id=None,
                         time_coverage=None, publisher=None, language=None,
                         mimetype=None, contributors=None, license_remarks=None,
                         geolocation=None, longitude=None, latitude=None,
                         data_link=None, has_linked_file=None, derived_from=None,
@@ -3134,14 +3174,19 @@
         """Returns True when the session's account may impersonate other accounts."""
         return self.__may_execute_role (session_token, "impersonate", account)
 
     def may_review_quotas (self, session_token, account=None):
         """Returns True when the session's account may handle storage requests."""
         return self.__may_execute_role (session_token, "review_quotas", account)
 
+    def may_review_integrity (self, session_token, account=None):
+        """Returns True when the session's account may view data integrity information."""
+        return (self.__may_execute_role (session_token, "administer", account) and
+                self.__may_execute_role (session_token, "review_integrity", account))
+
     def is_depositor (self, session_token):
         """Returns True when the account linked to the session is a depositor, False otherwise"""
         return self.is_logged_in (session_token)
 
     def is_logged_in (self, session_token):
         """Returns True when the session_token is valid, False otherwise."""
```

### Comparing `djehuty-24.3/src/djehuty/web/email_handler.py` & `djehuty-24.4/src/djehuty/web/email_handler.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/formatter.py` & `djehuty-24.4/src/djehuty/web/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,26 @@
             "firstOnline":         conv.value_or_none(record, "timeline_first_online"),
             "revision":            conv.value_or_none(record, "timeline_revision"),
         },
         "resource_title":          conv.value_or_none(record, "resource_title"),
         "resource_doi":            conv.value_or_none(record, "resource_doi")
     }
 
+def format_author_record_v3 (record):
+    """Record formatter for the v3 authors API output."""
+    return {
+        "uuid":        conv.value_or_none (record, "uuid"),
+        "first_name":  conv.value_or_none(record, "first_name"),
+        "last_name":   conv.value_or_none(record, "last_name"),
+        "full_name":   conv.value_or_none(record, "full_name"),
+        "email":       conv.value_or_none(record, "email"),
+        "orcid":       conv.value_or (record, "orcid_id", None),
+        "is_editable": conv.value_or (record, "is_editable", False)
+    }
+
 def format_author_record (record):
     """Record formatter for authors."""
     return {
       "id":        conv.value_or_none(record, "id"),
       "uuid":      conv.value_or_none(record, "uuid"),
       "full_name": conv.value_or_none(record, "full_name"),
       "is_active": bool(conv.value_or_none(record, "is_active")),
```

### Comparing `djehuty-24.3/src/djehuty/web/locks.py` & `djehuty-24.4/src/djehuty/web/locks.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/activate_2fa_session.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/activate_2fa_session.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/admin/dashboard.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/dashboard.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/admin/exploratory.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/exploratory.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% extends "layout.html" %}
 {% block headers %}
   <script src="/static/js/jquery-3.6.0.min.js"></script>
   <script src="/static/js/d3.v7.min.js"></script>
+  <script src="/static/js/utils.js"></script>
   <script src="/static/js/exploratory.js"></script>
   <style>
 #data-model-explorer {
     width: 100%;
     height: 400pt;
     margin: 1em 0em 1em 0em;
     border: solid 2pt #333333;
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/admin/maintenance.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/maintenance.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/admin/quota_requests.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/quota_requests.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/admin/reports/dashboard.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/dashboard.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/admin/reports/embargoed_datasets.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/embargoed_datasets.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/admin/reports/restricted_datasets.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/restricted_datasets.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/admin/sparql.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/sparql.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/author.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/author.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/badge.svg` & `djehuty-24.4/src/djehuty/web/resources/html_templates/badge.svg`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     <stop offset="1" stop-opacity=".1"/>
   </linearGradient>
   <mask id="a" width="{{outer_width}}" height="20">
     <rect width="{{outer_width}}" height="20" rx="3" fill="#fff"/>
   </mask>
   <g mask="url(#a)">
     <path fill="#555" d="M0 0h{{left_width}}v20H0z" />
-    <path fill="#f49120" d="M{{left_width}} 0h{{right_width}}v20H{{left_width}}z" />
+    <path fill="{{color}}" d="M{{left_width}} 0h{{right_width}}v20H{{left_width}}z" />
     <path fill="url(#b)" d="M0 0h{{outer_width}}v20H0z" />
   </g>
   <g fill="#fff" text-anchor="middle" font-family="DejaVu Sans,Verdana,Geneva,sans-serif" font-size="11">
     <text x="16.1875" y="15" fill="#010101" fill-opacity=".3">DOI</text>
     <text x="16.1875" y="14">DOI</text>
     <text x="{{doi_text_x}}" y="15" fill="#010101" fill-opacity=".3">{{doi}}</text>
     <text x="{{doi_text_x}}" y="14">{{doi}}</text>
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/categories.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/categories.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/category.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/category.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/collection.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/collection.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/dataset.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/dataset.html`

 * *Files 17% similar despite different names*

```diff
@@ -5,42 +5,14 @@
 <script src="/static/js/quill.min.js"></script>
 <script src="/static/js/utils.js"></script>
 <link rel="stylesheet" type="text/css" href="/static/css/pub.css" />
 <link href="/static/css/quill.4tu.css" rel="stylesheet">
 <style>
 #access-request-wrapper { display: none; }
 #content-wrapper {padding: 0}
-#content-wrapper input[type="text"],
-#content-wrapper input[type="datetime-local"],
-#content-wrapper input[type="date"],
-#content-wrapper textarea, .texteditor {
-    display: block;
-    padding: .7em;
-    border: solid 1pt #aaa;
-    border-radius: 0em .5em .5em .5em;
-    width: 832pt;
-    margin-top: 0em;
-    margin-bottom: 1em;
-    font-size: 13pt;
-}
-.texteditor {
-    padding: 0em !important;
-    border-radius: 0em 0em .5em .5em !important;
-    resize: vertical;
-    font-size: 1.0em;
-    width: 852pt;
-}
-#content-wrapper label {
-    display: inline-block;
-    background: #ffeecc;
-    color: #000;
-    padding: .5em .5em .25em .5em;
-    border-radius: .5em .5em 0em 0em;
-    font-weight: bold;
-}
 </style>
 {% endblock %}
 
 {% block body %}
 {% set doi = item.doi %}
 {% set pid = item.dataset_id %}
 {% set item_type = "dataset" %}
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/dataset_access_request.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/dataset_access_request.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/collection-private-links.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/collection-private-links.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/dashboard.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/dashboard.html`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     border-radius: .5em .5em 0em 0em;
     font-weight: bold;
 }
 </style>
 {% endblock %}
 {% block submenu %}
 <ul>
-  <li class="active corporate-identity-submenu-active">Dashboard
+  <li class="active corporate-identity-submenu-active">My Dashboard
   <li class="create-button"><a href="/my/sessions/new">Create API token</a>
   <li><a href="/my/datasets">My Datasets</a>
   <li><a href="/my/collections">My Collections</a>
 </ul>
 {% endblock %}
 {% block body %}
 <h1>Dashboard</h1>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "layout.html" %} {% block headers %}
 {% endblock %} {% block submenu %}
-    * Dashboard
+    * My Dashboard
     * _C_r_e_a_t_e_ _A_P_I_ _t_o_k_e_n
     * _M_y_ _D_a_t_a_s_e_t_s
     * _M_y_ _C_o_l_l_e_c_t_i_o_n_s
 {% endblock %} {% block body %}
 ************ DDaasshhbbooaarrdd ************
 ********** QQuuiicckk aaccttiioonnss **********
 _A_d_d_ _n_e_w_ _d_a_t_a_s_e_t _C_r_e_a_t_e_ _n_e_w_ _c_o_l_l_e_c_t_i_o_n
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/dataset-private-links.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/dataset-private-links.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/edit-collection.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-collection.html`

 * *Files 1% similar despite different names*

```diff
@@ -84,26 +84,24 @@
   margin: 0em 1em .5em 0em;
   padding: .5em;
   border-radius: .5em;
   background: #eee;
 }
 #doi-wrapper p { margin: 0pt; }
 .collection-content-loader { display: none; }
-.submit-button a { background: #f49120 !important; }
-.submit-button a:hover { background: #f7ad58 !important; }
 .private-links-button a { background: #53736f !important; }
 .private-links-button a:hover { background: #7e9693 !important; }
 </style>
 {% endblock %}
 {% block submenu %}
 <ul>
   <li><a href="/my/collections">&#8592; Go back</a>
   <li class="active corporate-identity-submenu-active">Edit collection
   <li class="hide-for-javascript save-button"><a id="save" href="#">Save draft</a>
-  <li class="hide-for-javascript submit-button"><a id="publish" href="#">Publish</a>
+  <li class="hide-for-javascript publish-button"><a id="publish" href="#">Publish</a>
   <li class="hide-for-javascript delete-button"><a id="delete" href="#">Delete</a>
   <li class="hide-for-javascript private-links-button"><a id="private-links" target="_blank" href="/my/collections/{{collection["uuid"]}}/private_links?go_back=no">Private access</a>
 </ul>
 {% endblock %}
 {% block body %}
 <div class="collection-content-loader"></div>
 <div class="collection-content">
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/edit-dataset.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-dataset.html`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,16 @@
     vertical-align: middle;
     text-align: center;
     color: #333;
 }
 .upload-container:hover { cursor: pointer; }
 .upload-container p { font-size: 1.2em; }
 .file-incomplete-warning { font-style: italic; color: red; }
+table#files tbody tr td:nth-child(2) { min-width: 260px; }
+table#files tbody tr td:nth-child(3) { width: 15px; text-align: right; }
 #collaborators-form input[type="text"] {
   width: 790px;
   background: #fff;
   margin: 0px;
   border-radius: 5pt;
   border: solid 1px #ccc;
   padding: .5em;
@@ -117,19 +119,19 @@
 #access-wrapper select,
 #access-wrapper .ql-toolbar.ql-4tu,
 #access-wrapper .texteditor { width: 832pt !important; }
 #embargoed_access_form { display: none }
 #restricted_access_form { display: none; }
 #file-upload h4 { font-size: 1.5em; padding: 0em; margin: .75em 0em .75em 0em; }
 #categories-wrapper .subitem-checkbox { margin-left: 3em; }
-#new-author { text-align: center; line-height: 3.5em; height: 3.5em; }
+#new-author, #update-author { text-align: center; line-height: 3.5em; height: 3.5em; }
 #new-funding { text-align: center; line-height: 3.5em; height: 3.5em; }
-#new-author-form { padding: 1em; }
-#new-author-form label { background: #eee; }
-#new-author-form input[type="text"] { width: 800pt; }
+#new-author-form, #author-inline-edit-form td { padding: 1em; }
+#new-author-form label, #author-inline-edit-form label { background: #eee; }
+#new-author-form input[type="text"], #author-inline-edit-form input[type="text"] { width: 800pt; }
 #new-funding-form { padding: 1em; }
 #new-funding-form label { background: #eee; }
 #new-funding-form input[type="text"] { width: 800pt; }
 #geolocation-wrapper label { background: #eee; }
 #geolocation-wrapper input[type="text"] { width: 812pt; }
 #references-list { display: none; border: none; }
 #references-list thead { display: none; }
@@ -156,16 +158,14 @@
 #git-files { margin: 0em; padding: 0em; }
 #git-files li { list-style-type: none; margin: 0em; padding: .5em; }
 #git-files li:nth-child(even) { background: #fafafa; }
 #embargo_options { display: none; }
 #refresh-git-files { font-size: .75em; }
 .decline-button a { background: #aa3333 !important; }
 .decline-button a:hover { background: #cc3333 !important; }
-.publish-button a { background: #f49120 !important; }
-.publish-button a:hover { background: #f7ad58 !important; }
 .preview-button a { background: #736f53 !important; }
 .preview-button a:hover { background: #96937e !important; }
 .private-links-button a { background: #53736f !important; }
 .private-links-button a:hover { background: #7e9693 !important; }
 #doi-wrapper p { margin: 0pt; }
 .article-content-loader { display: none; }
 #files-table-actions { text-align: right; }
@@ -228,15 +228,15 @@
 <p>Fields marked with <span class="required-field">&#8727;</span> are required.</p>
 <label for="title">Title</label><div class="fas fa-question-circle help-icon"><span class="help-text">Give your research a title that is more descriptive than just a file name. This will help making your items discoverable via search engines such as Google. The title should have at least three characters.</span></div><span class="required-field">&#8727;</span>
 <input type="text" id="title" name="title" value="{{article["title"]}}" />
 <label for="authors">Authors</label><div class="fas fa-question-circle help-icon"><span class="help-text">Select authors from the list or manually add them by creating a new author record. Hit enter after adding each author and drag and drop names to arrange them in the order you wish.</span></div><span class="required-field">&#8727;</span>
 <input type="text" id="authors" name="authors" />
 <table class="inside-form-table multi-list" id="authors-list">
   <thead>
-    <tr><th>Author</th><th>Actions</th></tr>
+    <tr><th>Author</th><th colspan="2">Actions</th></tr>
   </thead>
   <tbody></tbody>
 </table>
 
 {%- if not disable_collaboration: %}
 <label>Collaborators <span class="beta-badge">Beta</span></label><div class="fas fa-question-circle help-icon"><span class="help-text">Add people who can collaborate on this dataset.  Collaborators are not visible on the publication, but instead are given access to this form to either change metadata, or upload files.</span></div>
 <div id="collaborator-wrapper" class="options-wrapper">
@@ -244,16 +244,16 @@
 <div class="expand-collaborators">
 </div>
 <div id="expanded-collaborators">
   <table id="collaborators-form" class="corporate-identity-table">
     <thead>
       <tr>
         <th colspan="1" scope="colgroup">Collaborator</th>
-        <th colspan="2" scope="colgroup">Metadata</th>
-        <th colspan="3" scope="colgroup">Files</th>
+        <th colspan="2" scope="colgroup">Metadata<div class="fas fa-question-circle help-icon"><span class="help-text">Refers to all the fields on this page</span></div></th>
+        <th colspan="3" scope="colgroup">Files<div class="fas fa-question-circle help-icon"><span class="help-text">Refers to the uploaded files</span></div></th>
         <th colspan="1" scope="colgroup"></th>
       </tr>
       <tr>
         <th scope="col"></th>
         <th scope="col"><span class="fas fa-glasses"title="Read"></span></th>
         <th scope="col"><span class="fas fa-pen"title="Edit"></span></th>
         <th scope="col"><span class="fas fa-glasses"title="Read"></span></th>
@@ -281,15 +281,15 @@
 --><input type="radio" name="access_type" id="embargoed_access" value="embargoed" /><!--
 --><label for="embargoed_access" class="no-head">Embargoed access</label><!--
 --><input type="radio" name="access_type" id="restricted_access" value="restricted" /><!--
 --><label for="restricted_access" class="no-head">Restricted access</label>
   </div>
   <div class="access_level" id="open_access_form">
     <p>
-      Open access is the default setting in 4TU.ResearchData by which your dataset will be directly accessible to others.
+      Open access is the default setting in {{site_name}} by which your dataset will be directly accessible to others.
     </p>
     <label for="license_open" class="inner-head">Licence</label><div class="fas fa-question-circle help-icon"><span class="help-text">Select the appropriate licence from the list. Need to know more? Read our <a target="_blank" rel="noopener noreferrer" href="https://data.4tu.nl/info/en/use/publish-cite/upload-your-data-in-our-data-repository/licencing">guidance</a> for more information on the licence types we offer.</span></div><span class="required-field"> &#8727;</span>
     <select id="license_open" class="license-selector" name="license">
       <option value="" disabled selected>Select a licence</option>
     </select>
   </div>
   <div class="access_level" id="embargoed_access_form">
@@ -364,15 +364,15 @@
 <input class="subitem-checkbox" type="radio" name="groups" value="{{sub.id}}" id="group_{{sub.id}}"><!--
 --><label class="subitem-label no-head" for="group_{{sub.id}}">{{sub.name}}</label><br>
 {%- endfor %}
 </div>
 {%- endfor %}
 </div>
 <label for="publisher">Publisher</label>
-<input type="text" id="publisher" name="publisher" value="{{article["publisher"] | default("4TU.ResearchData", True)}}">
+<input type="text" id="publisher" name="publisher" value="{% if article["publisher"] %}{{article["publisher"]}}{% else %}{{site_name}}{% endif %}">
 <label for="funding">Funding</label><div class="fas fa-question-circle help-icon"><span class="help-text">Select from the list by searching for funder name, grant number or grant name or manually add them by creating a new funding record.</span></div>
 <input type="text" id="funding" name="funding" />
 <table class="inside-form-table multi-list" id="funding-list">
   <thead>
     <tr><th>Name</th><th>Actions</th></tr>
   </thead>
   <tbody></tbody>
@@ -401,15 +401,15 @@
 </div>
 <h3 class="corporate-identity-h3">Findability</h3>
 <label for="language">Language</label><div class="fas fa-question-circle help-icon"><span class="help-text">Select a language from the list.</span></div><span class="required-field">&#8727;</span>
 {% set item = article %}
 {% include 'depositor/language-selector.html' %}
 <label for="time_coverage">Time coverage</label><div class="fas fa-question-circle help-icon"><span class="help-text">Indicate the dates to which the data refer. Enter the year, or the beginning and ending date.</span></div>
 <input type="text" id="time_coverage" name="time_coverage" value="{{article["time_coverage"] | default("", True)}}" />
-<label>Geolocation</label>
+<label>Geolocation</label><div class="fas fa-question-circle help-icon"><span class="help-text">When your dataset covers geographical data, fill in the following section </span></div>
 <div id="geolocation-wrapper">
   <label for="geolocation">Name</label><div class="fas fa-question-circle help-icon"><span class="help-text">The geographic area to which the data refer (e.g. municipality, town/city, region, country)</span></div>
   <input type="text" id="geolocation" name="geolocation" placeholder="Example: Dam Square, Amsterdam" value="{{article["geolocation"] | default("", True)}}" />
   <label for="longitude">Longitude</label><div class="fas fa-question-circle help-icon"><span class="help-text">Geographic longitude in decimal degrees, East is positive, West is negative. Values: -180 to 180.</span></div>
   <input type="text" id="longitude" name="longitude" placeholder="Example: 4.893" value="{{article["longitude"] | default("", True)}}" />
   <label for="latitude">Latitude</label><div class="fas fa-question-circle help-icon"><span class="help-text">Geographic latitude in decimal degrees, North is positive, South is negative. Values: -90 to 90.</span></div>
   <input type="text" id="latitude" name="latitude" placeholder="Example: 52.893" value="{{article["latitude"] | default("", True)}}" />
@@ -446,31 +446,34 @@
   <p>Only use this option when there are no files to attach.  Enter the reason
     for creating a metadata only record and why the files cannot be shared.</p>
   <label for="metadata_only_reason">Reason</label>
   <input type="text" name="metadata_only_reason" id="metadata_only_reason" value="{{article["metadata_reason"]}}"/>
 </div>
 <div id="external_link_field" class="record-type-field">
   <p>Only use when no files can be attached. Add the URL where your files can
-    be found. Note that 4TU.ResearchData is not responsible for maintaining the
+    be found. Note that {{site_name}} is not responsible for maintaining the
     link or for its validity.</p>
   <label for="external_link">External URL</label>
   <input type="text" name="external_url" id="external_url" value="{{article["url"]}}" />
   <div class="a-button">
     <a href="#" onclick="javascript:submit_external_link('{{article["container_uuid"]}}'); return false;">Save URL</a>
   </div>
 </div>
 <div id="software_upload_field" class="record-type-field">
   <h4 class="corporate-identity-h4">Publish source code through Git</h4>
-  <p>To publish from a Git repository, push a branch to the <code>4tu</code> remote.</p>
-  <p>First, add the <code>4tu</code> remote:</p>
-  <pre>git remote add 4tu {{base_url}}/v3/datasets/{{article.git_uuid}}.git</pre>
+  <p>To publish from a Git repository, push a branch to the <code>{{site_shorttag}}</code> remote.</p>
+  <p>First, add the <code>{{site_shorttag}}</code> remote:</p>
+  <pre>git remote add {{site_shorttag}} {{base_url}}/v3/datasets/{{article.git_uuid}}.git</pre>
   <p>Then, push the repository to it:</p>
   <pre>
-git push 4tu --all
-git push 4tu --tags</pre>
+git push {{site_shorttag}} --all
+git push {{site_shorttag}} --tags</pre>
+  <p>When publishing a newer version of this dataset in the future, the Git <code>remote</code> location will be reset.
+    So when your dataset has been published, remove the remote:</p>
+  <pre>git remote remove 4tu</pre>
   <h4 class="corporate-identity-h4">Git repository files and branches <span class="no-select"> &nbsp;<a id="refresh-git-files" href="#" class="fas fa-sync"></a></span></h4>
   <label>Git default branch</label><div class="fas fa-question-circle help-icon"><span class="help-text">The selected branch will be the branch a user is in after pulling the Git repository.</span></div>
   <select id="git-branches">
     <option value="" disabled="disabled">Select branch</option>
   </select>
   <label id="git-files-label">Git file list</label>
   <div id="git-files-wrapper" class="options-wrapper">
@@ -512,9 +515,12 @@
 <h3 class="corporate-identity-h3">Terms and agreement</h3>
 <input type="checkbox" name="deposit_agreement" id="deposit_agreement">
 <label class="no-head" for="deposit_agreement">I agree with the <a target="_blank" rel="noopener noreferrer" href="/s/docs/deposit-agreement.pdf">Deposit Agreement</a>.</label><span class="required-field">&#8727;</span><br />
 <input type="checkbox" name="publish_agreement" id="publish_agreement">
 <label class="no-head" for="publish_agreement">I agree that my dataset will be published once
   the review is complete.</label><span class="required-field">&#8727;</span>
 </div>
+{%- if not article.is_shared_with_me or permissions.metadata_edit %}
+<a class="hide-for-javascript save-button button"id="save_bottom" href="#">Save draft</a>
+{%- endif %}
 </div>
 {% endblock %}
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/edit-session.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-session.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/language-selector.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/language-selector.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/my-collections.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/my-collections.html`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     jQuery("#table-unpublished-collections-loader").remove();
     jQuery("#table-published-collections-loader").remove();
 });
 </script>
 {% endblock %}
 {% block submenu %}
 <ul>
-  <li><a href="/my/dashboard">Dashboard</a>
+  <li><a href="/my/dashboard">My Dashboard</a>
   <li><a href="/my/datasets">My Datasets</a>
   <li class="active corporate-identity-submenu-active">My Collections
   <li class="create-button"><a href="/my/collections/new">Create new collection</a>
 </ul>
 {% endblock %}
 {% block body %}
 <noscript>
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/my-data.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/my-data.html`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     jQuery("#table-review").show();
     jQuery("#table-review-loader").remove();
 });
 </script>
 {% endblock %}
 {% block submenu %}
 <ul>
-  <li><a href="/my/dashboard">Dashboard</a>
+  <li><a href="/my/dashboard">My Dashboard</a>
   <li class="active corporate-identity-submenu-active">My Datasets
   <li class="create-button"><a href="/my/datasets/new">Add new dataset</a>
   <li><a href="/my/collections">My Collections</a>
 </ul>
 {% endblock %}
 {% block body %}
 <noscript>
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/new_private_link.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/new_private_link.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/profile.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/profile.html`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     background-size: contain;
     background-repeat: none;
 }
 </style>
 {% endblock %}
 {% block submenu %}
 <ul>
-  <li class="hide-for-javascript"><a id="dashboard" href="/my/dashboard">Dashboard</a>
+  <li class="hide-for-javascript"><a id="dashboard" href="/my/dashboard">My Dashboard</a>
   <li class="active corporate-identity-submenu-active">Profile
   <li class="hide-for-javascript save-button"><a id="save" href="#">Save</a>
 {%- if account.author_uuid != "unknown" %}
   <li class="hide-for-javascript"><a id="show-public-profile" href="/authors/{{account.author_uuid}}">Public profile</a>
   {%- if orcid_client_id is not none: %}
     {%- if "orcid" not in account or account.orcid is none or account.orcid == "": %}
   <li class="hide-for-javascript orcid-button"><a id="connect-with-orcid" href="/my/profile/connect-with-orcid"><span class="fab fa-orcid"></span>Connect ORCID</a>
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/published-collection.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/published-collection.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/depositor/submitted-for-review.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/submitted-for-review.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/email/dataset_submitted.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_submitted.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/feedback.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/feedback.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/institutions.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/institutions.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     border-radius: .5em .5em 0em 0em;
 }
 .loader {
     display: block;
     width: 100%;
     min-height: 100px;
     background-color: rgba(255, 255, 255, 0.5);
-    background-image: url('/static/images/loader.svg');
+    background-image: url('/theme/loader.svg');
     background-position: center;
     background-repeat: no-repeat;
     z-index: 100;
 }
 #top-datasets th { text-align: left; white-space: nowrap; color: #ffffff; padding: .5em; }
 #top-datasets-wrapper table { width: 100%; max-width: 880pt; }
 #top-datasets tbody tr td { padding: .5em; z-index: 50; }
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/layout.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="UTF-8">
     <meta name="description" content="{{site_description}}">
-    <meta name="keywords" content="4tu, 4tu.researchdata">
-    <meta name="author" content="4TU.ResearchData">
+    <meta name="keywords" content="{{site_shorttag}}, {{site_name}}, data repository">
+    <meta name="author" content="{{site_name}}">
     <meta http-equiv="Content-Security-Policy" content="default-src 'self' api.figshare.com ndownloader.figshare.com s3-eu-west-1.amazonaws.com 'unsafe-inline'; frame-src https://www.youtube.com">
     <title>{% if page_title %}{{page_title|safe}}{% else %}{{site_name | default("Djehuty", True)}}{% endif %}</title>
     <link rel='shortcut icon' type='image/x-icon' href='/static/images/favicon.ico'>
+    <link rel="stylesheet" type="text/css" href="/theme/colors.css">
     <link rel="stylesheet" type="text/css" href="/static/css/main.css">
     {% block headers %}{% endblock %}
   </head>
   <body>
     <div id="wrapper" {%- if path == "/" %} class="footer1"{% else %} class="footer2"{% endif %}>
       {%- if sandbox_message %}
       <div id="sandbox-message" class="pre-header" {% if sandbox_message_css %}style="{{sandbox_message_css | safe}}"{% endif %}>
@@ -31,15 +32,15 @@
       {%- endif %}
       {%- if private_view and not is_reviewing %}
       <div id="pre-header" class="pre-header">
         <p>You are viewing a pre-publication item. It hasn't been reviewed or published.</p>
       </div>
       {%- endif %}
       <div id="header" class="corporate-identity-header">
-        <div id="header-left"><a href="/"><img id="corporate-identity-logo" src="/static/images/logo.png" alt="4TU.ResearchData portal"></a></div>
+        <div id="header-left"><a href="/"><img id="corporate-identity-logo" src="/static/images/logo.png" alt="{{site_name}} logo"></a></div>
         <div id="header-middle">
           <div id="search-box-wrapper">
             {%- if not maintenance_mode %}
             <form method="get" action="/search?search=">
               <input id="search-box" aria-label="Search" title="Search" name="search" type="text" placeholder="Search..." maxlength="255" value="{{search_for}}"><!--
               --><input type="submit" class="search-submit-btn fa-search" value="&#xf002;">
             </form>
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 {{iimmppeerrssoonnaattiinngg__aaccccoouunntt..llaasstt__nnaammee}}}}. _C_l_i_c_k_ _h_e_r_e to stop reviewing.
 {% else: %}
 Impersonating as {{{{iimmppeerrssoonnaattiinngg__aaccccoouunntt..ffiirrsstt__nnaammee}}}} {{
 {{iimmppeerrssoonnaattiinngg__aaccccoouunntt..llaasstt__nnaammee}}}}. _C_l_i_c_k_ _h_e_r_e to stop impersonating.
 {%- endif %} {%- endif %} {%- if private_view and not is_reviewing %}
 You are viewing a pre-publication item. It hasn't been reviewed or published.
 {%- endif %}
-_[_4_T_U_._R_e_s_e_a_r_c_h_D_a_t_a_ _p_o_r_t_a_l_]
+_[_{_{_s_i_t_e___n_a_m_e_}_}_ _l_o_g_o_]
 {%- if not maintenance_mode %}
 [{{search_for}}      ][&#xf002;]
 {%- endif %}
 {%- if not maintenance_mode %} {%- if not is_logged_in %} {%- if
 identity_provider == "orcid" %}
 _L_o_g_ _i_n
 {%- endif %} {%- if identity_provider == "saml" or identity_provider ==
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/opendap_to_doi.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/opendap_to_doi.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/portal.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/portal.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/public_metadata.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/public_metadata.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/review/overview.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/review/overview.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/html_templates/search.html` & `djehuty-24.4/src/djehuty/web/resources/html_templates/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     font-size: 12pt;
     padding: .5em .75em .5em .75em;
     margin: 0pt 5pt 0pt 0pt;
     user-select: none;
     border-radius: .5em .5em 0em 0em;
 }
 #search-loader {
-    background-image: url('/static/images/loader.svg');
+    background-image: url('/theme/loader.svg');
     background-position: center;
     background-repeat: no-repeat;
     color: darkgrey;
     display: inline-block;
     font-size: 2.5em;
     font-style: italic;
     padding-top: 5.0em;
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/account_by_email.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_by_email.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/account_by_session_token.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_by_session_token.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/account_categories.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_categories.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/account_sessions.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_sessions.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/account_storage_used.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_storage_used.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/accounts.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/accounts.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/associated_authors.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/associated_authors.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/author_profile.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/author_profile.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/author_public_items.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/author_public_items.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/authors.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/container_items.sparql`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,49 @@
 {% extends "prefixes.sparql" %}
 {% block query %}
-SELECT DISTINCT ?first_name      ?full_name       ?group_id
-                ?uuid ?id        ?institution_id  ?is_active
-                ?is_public       ?job_title       ?last_name
-                ?orcid_id        ?url_name        ?order_index
+SELECT DISTINCT ?account_uuid ?container_uuid ?version ?container_uri
+                (?item_uri AS ?uri) ?uuid
 WHERE {
   GRAPH <{{state_graph}}> {
-    ?author            rdf:type                 djht:Author .
-    OPTIONAL { ?author djht:id                  ?id . }
-
-    {%- if item_uri is not none %}
-    ?item_uri          rdf:type                 djht:{{prefix}} ;
-                       djht:authors             ?authors .
-    ?authors           rdf:rest*                ?rest .
-    ?rest              rdf:first                ?author ;
-                       djht:index               ?order_index .
+    ?container_uri       rdf:type/rdfs:subClassOf djht:Container .
+    ?container_uri       djht:account             ?account .
+    {%- if is_published is none and is_latest is none %}
+    ?item_uri            djht:container           ?container_uri .
+    {%- elif is_published %}
+    {%- if is_latest %}
+    ?container_uri       djht:latest_published_version ?item_uri .
+    {%- else %}
+    ?container_uri       djht:published_versions/rdf:rest*/rdf:first ?item_uri .
     {%- endif %}
-    {%- if account_uuid is not none %}
-    ?container         rdf:type                 djht:{{prefix}}Container .
-    {%- if is_published %}
-    ?container         djht:published_versions/rdf:rest*/rdf:first ?item_uri .
     {%- else %}
-    ?container         djht:draft               ?item_uri .
+    ?container_uri       djht:draft                ?item_uri .
     {%- endif %}
-    ?container         djht:account             ?account .
 
-    {%- if not disable_collaboration %}
+{%- if account_uuid is not none and not disable_collaboration: %}
     OPTIONAL {
-      ?item_uri          djht:container      ?container .
-      ?collaborator      rdf:type            djht:Collaborator .
-      ?collaborator      djht:item           ?item_uri .
-      ?collaborator      djht:account        ?collaborator_account .
-      ?collaborator      djht:metadata_read  "true"^^xsd:boolean .
+      ?collaborator       rdf:type            djht:Collaborator .
+      ?collaborator       djht:item           ?item_uri .
+      ?collaborator       djht:account        ?collaborator_account .
+      ?collaborator       djht:metadata_read  "true"^^xsd:boolean .
     }
-    {%- endif %}
-    {%- endif %}
-    OPTIONAL { ?author djht:first_name          ?first_name . }
-    OPTIONAL { ?author djht:full_name           ?full_name . }
-    OPTIONAL { ?author djht:group_id            ?group_id . }
-    OPTIONAL { ?author djht:institution_id      ?institution_id . }
-    OPTIONAL { ?author djht:is_active           ?is_active . }
-    OPTIONAL { ?author djht:is_public           ?is_public . }
-    OPTIONAL { ?author djht:job_title           ?job_title . }
-    OPTIONAL { ?author djht:last_name           ?last_name . }
-    OPTIONAL { ?author djht:orcid_id            ?orcid_id . }
-    OPTIONAL { ?author djht:url_name            ?url_name . }
-
-    BIND(STRAFTER(STR(?author), "author:") AS ?uuid)
+{%- endif %}
+    OPTIONAL { ?item_uri djht:version              ?version . }
+    BIND(STRAFTER(STR(?container_uri), "container:") AS ?container_uuid)
+    BIND(STRAFTER(STR(?account), "account:")         AS ?account_uuid)
+    BIND(STRAFTER(STR(?item_uri), ":")               AS ?uuid)
   }
-{%- if account_uuid is not none %}
+{%- if account_uuid is not none: %}
   {%- if disable_collaboration %}
 FILTER (?account = <account:{{account_uuid}}>)
   {%- else %}
 FILTER (?account = <account:{{account_uuid}}> ||
         ?collaborator_account = <account:{{account_uuid}}>)
   {%- endif %}
 {%- endif %}
-{%- if item_uri is not none %}
-  FILTER (?item_uri = <{{item_uri}}>)
-{% endif %}
-{% if filters is not none %}{{ filters | safe }}{% endif %}
+{%- if container_uri is not none: %}
+FILTER (?container_uri = <{{container_uri}}>)
+{%- endif %}
+{%- if item_uuid is not none %}
+FILTER (STRAFTER(STR(?item_uri), ":") = STR("{{item_uuid}}"))
+{%- endif %}
 }
 {% endblock %}
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/categories.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/categories.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/categories_tree.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/categories_tree.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/category_by_id.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/category_by_id.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/collaborators.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collaborators.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/collection_datasets.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_datasets.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/collection_versions.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_versions.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/collections.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/collections_by_account.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections_by_account.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/collections_from_dataset.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections_from_dataset.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/container.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/container.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/custom_fields.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/custom_fields.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/dataset_files.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_files.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/dataset_statistics.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_statistics.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/dataset_statistics_timeline.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_statistics_timeline.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/dataset_versions.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_versions.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/datasets.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/datasets.sparql`

 * *Files 0% similar despite different names*

```diff
@@ -86,16 +86,16 @@
     OPTIONAL { ?dataset djht:posted_date          ?timeline_posted . }
     OPTIONAL { ?dataset djht:revision_date        ?timeline_revision . }
 
     OPTIONAL {
       ?dataset          djht:license               ?license_url .
       ?license_url      rdf:type                   djht:License .
       ?license_url      djht:id                    ?license_id .
-      ?license_url      djht:spdx                  ?license_spdx .
       ?license_url      djht:name                  ?license_name .
+      OPTIONAL { ?license_url djht:spdx            ?license_spdx . }
     }
 
     OPTIONAL { ?dataset djht:git_uuid              ?git_uuid . }
     OPTIONAL { ?dataset djht:citation              ?citation . }
     OPTIONAL { ?dataset djht:confidential_reason   ?confidential_reason . }
     OPTIONAL { ?dataset djht:created_date          ?created_date . }
     OPTIONAL { ?dataset djht:defined_type          ?defined_type . }
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/datasets_missing_dois.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/datasets_missing_dois.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/decline_draft_dataset.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/decline_draft_dataset.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_associations.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_associations.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_collaborator.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_collaborator.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_collection_draft.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_collection_draft.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_dataset_draft.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_dataset_draft.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_dataset_embargo.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_dataset_embargo.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_item_categories.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_item_categories.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_item_from_list.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_item_from_list.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_items_all_from_list.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_items_all_from_list.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/delete_private_links.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_private_links.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/funding.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/funding.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/group.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/group.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/item_collaborative_permissions.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/item_collaborative_permissions.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/latest_datasets_portal.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/latest_datasets_portal.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/missing_checksummed_files_for_container.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/missing_checksummed_files_for_container.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/opendap_to_doi.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/opendap_to_doi.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/private_links.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/private_links.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/publish_draft_collection.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/publish_draft_collection.sparql`

 * *Files 2% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 
     OPTIONAL { ?container djht:latest_published_version ?latest_published_version . }
     OPTIONAL { ?draft_collection djht:is_latest     ?is_latest . }
     OPTIONAL { ?draft_collection djht:is_public     ?is_public . }
     OPTIONAL { ?draft_collection djht:is_editable   ?is_editable . }
     OPTIONAL { ?draft_collection djht:version       ?version . }
 
-    BIND(NOW() AS ?now)
+    BIND("{{timestamp}}"^^xsd:dateTime AS ?now)
   }
   FILTER (?container = <container:{{container_uuid}}>)
   FILTER (?account = <account:{{account_uuid}}>)
 }
 {% endblock %}
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/publish_draft_dataset.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/publish_draft_dataset.sparql`

 * *Files 2% similar despite different names*

```diff
@@ -55,12 +55,12 @@
     OPTIONAL { ?container djht:latest_published_version ?latest_published_version . }
     OPTIONAL { ?draft_dataset djht:is_latest     ?is_latest . }
     OPTIONAL { ?draft_dataset djht:is_public     ?is_public . }
     OPTIONAL { ?draft_dataset djht:is_editable   ?is_editable . }
     OPTIONAL { ?draft_dataset djht:is_under_review ?is_under_review . }
     OPTIONAL { ?draft_dataset djht:version       ?version . }
 
-    BIND(NOW() AS ?now)
+    BIND("{{timestamp}}"^^xsd:dateTime AS ?now)
   }
   FILTER (?container = <container:{{container_uuid}}>)
 }
 {% endblock %}
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/quota_requests.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/quota_requests.sparql`

 * *Files 26% similar despite different names*

```diff
@@ -14,11 +14,13 @@
     ?account djht:email          ?email .
     OPTIONAL { ?account djht:first_name     ?first_name . }
     OPTIONAL { ?account djht:last_name      ?last_name . }
   }
   BIND (STRAFTER(STR(?request), "quota-request:") AS ?uuid)
   {%- if status is not none: %}
   FILTER (?status = {{status | safe}})
+  {%- endif %}{% if quota_request_uuid is not none: %}
+  FILTER (?request = <quota-request:{{quota_request_uuid}}>)
   {%- endif %}
 }
 ORDER BY DESC(?created_date)
 {% endblock %}
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/references.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/references.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/reviews.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/reviews.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/root_categories.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/root_categories.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/subcategories_by_category.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/subcategories_by_category.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/tags.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/tags.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_account.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_account.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_collection.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_collection.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_dataset.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_dataset.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_dataset_thumb.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_dataset_thumb.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_file.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_file.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_git_uuid.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_git_uuid.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_orcid_for_account.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_orcid_for_account.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_private_link.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_private_link.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_quota_request.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_quota_request.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_review.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_review.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_session.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_session.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/sparql_templates/update_view_and_download_counts.sparql` & `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_view_and_download_counts.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/css/dropzone.min.css` & `djehuty-24.4/src/djehuty/web/resources/static/css/dropzone.min.css`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/css/form.css` & `djehuty-24.4/src/djehuty/web/resources/static/css/form.css`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
     margin-bottom: 1em;
 }
 .inside-form-table thead tr { background: #ccc; border-radius: .5em .5em 0em 0em; }
 .inside-form-table thead tr th { color: #000; text-align: left; padding: .5em; z-index: 50; border-top: none; }
 .inside-form-table thead tr th:last-child { text-align: right; }
 .inside-form-table tbody tr td { padding: .5em; z-index: 50; }
 .inside-form-table tbody tr:nth-child(even) { background: #fafafa; }
-.inside-form-table tbody tr td:last-child { text-align: right; width: 130pt; }
-.inside-form-table tbody tr td:nth-child(1) {
+.inside-form-table tbody tr td:not(:first-child) { max-width: 15px; }
+.inside-form-table tbody tr td:first-child {
     text-overflow: ellipsis;
     overflow: hidden;
     white-space: nowrap;
     width: 100%;
     max-width: 572pt;
 }
+#author-inline-edit-form { border: solid 1pt #111; background: #fff; }
 #content-wrapper input[type="text"],
 #content-wrapper input[type="datetime-local"],
 #content-wrapper input[type="date"],
 #content-wrapper textarea,
 #content-wrapper .options-wrapper, #groups-wrapper, #access-wrapper, #geolocation-wrapper, #thumbnails-wrapper {
     display: block;
     padding: .7em;
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/css/jquery.dataTables.min.css` & `djehuty-24.4/src/djehuty/web/resources/static/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/css/main.css` & `djehuty-24.4/src/djehuty/web/resources/static/css/main.css`

 * *Files 9% similar despite different names*

```diff
@@ -41,43 +41,14 @@
   src: url("/static/fonts/fa-brands-400.eot");
   src: url("/static/fonts/fa-brands-400.eot?#iefix") format("embedded-opentype"),
        url("/static/fonts/fa-brands-400.woff2") format("woff2"),
        url("/static/fonts/fa-brands-400.woff") format("woff"),
        url("/static/fonts/fa-brands-400.ttf") format("truetype");
 }
 
-.corporate-identity { color: #f49120; }
-.corporate-identity:hover { color: #d26000; }
-
-.corporate-identity-h1 { border-bottom: 4px dotted #f49120;}
-.corporate-identity-h3 { border-bottom: 4px dotted #f49120; }
-.corporate-identity-h4 { border-bottom: 2px dotted #f49120; }
-
-.corporate-identity li.active { background: #f49120; }
-.corporate-identity li.active a { color: #ffffff; text-decoration: none; }
-.corporate-identity-submenu-active { border-bottom: solid .25em #f49120; }
-
-.corporate-identity-background { background: #f49120; }
-
-.corporate-identity-border { border: solid 2pt #f49120; }
-.corporate-identity-header { border-top: 4px solid #f49120; }
-.corporate-identity-footer { color: #ffffff; background: #707070; border-bottom: 3px solid #f49120; }
-
-.corporate-identity-privilege-button { background: #fce3bf; }
-.corporate-identity-standard-button { background: #f49120; color: #fff; font-weight: bold; text-decoration: none; }
-.corporate-identity-standard-button:hover { background: #d26000; cursor: pointer; color: #fff; text-decoration: none; }
-.corporate-identity-standard-button:active { background: #9d4800; cursor: pointer; color: #fff; text-decoration: none; }
-
-.corporate-identity-table {
-    width: 100%;
-    max-width: 880pt;
-    border: solid 2pt #f49120;
-    border-radius: .5em;
-}
-.corporate-identity-table thead tr { background: #f49120; border-radius: .5em .5em 0em 0em; }
 .corporate-identity-table thead tr th {
     color: #000;
     text-align: left;
     padding: .5em;
     z-index: 50;
     border-top: none;
     white-space: nowrap;
@@ -168,17 +139,14 @@
     text-decoration: none;
 }
 .cancel-button {
     color: #fff;
     font-weight: bold;
     text-decoration: none;
 }
-#login-button { margin-right: 25px; background: #f39000; color: #ffffff; }
-#login-button:hover { background: #d26000; cursor: pointer; }
-#login-button:active { background: #9d4800; cursor: pointer; }
 #login-button a { color: #ffffff; text-decoration: none; }
 #dashboard-button { margin-left: .5em; background: #505050; color: #ffffff; }
 #dashboard-button:hover { background: #303030; cursor: pointer; }
 #dashboard-button:active { background: #000000; cursor: pointer; }
 #dashboard-button a { color: #ffffff; text-decoration: none; }
 #logout-button { color: #cc0000; }
 #logout-button:hover { color: #ff0000; cursor: pointer; }
@@ -211,22 +179,20 @@
     font-size: 12pt;
     padding: 5px 5px 5px 0px;
     margin: 0pt 5pt 0pt 0pt;
     user-select: none;
     text-transform: uppercase;
 }
 #site-navigation ul:first-child { margin-left: 5mm; }
-#primary-menu .menu-item-has-children:hover { color: #f39000; }
 #primary-menu .menu-item-has-children:hover > ul {
     background: #ffffff;
     display: block;
     min-width: 120pt;
 }
 #primary-menu li a { text-decoration: none; }
-#primary-menu li a:hover { color: #f39000; }
 .submenu {
     position: absolute;
     display: none;
     max-width: 220pt;
     background: #f1f1f1;
     box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.25);
     border-radius: .5em;
@@ -505,14 +471,22 @@
     color: #ffffff;
     background: #505050;
     padding: 2pt 6pt 2pt 6pt;
     text-decoration: none;
     line-height: 1.75em;
     border-radius: 4pt;
 }
+#save_bottom {
+    margin: 30px 0px 30px 0px;
+    text-decoration: none;
+}
+
+#save_bottom { background: #139257; color: #ffffff; }
+#save_bottom:hover { background: #18b76d; }
+#save_bottom:active { background: #107a48; }
 #submenu li.orcid-button a { background: #a6ce39; color: #ffffff; }
 #submenu li.orcid-button a:hover { background: #c6e080; color: #ffffff; }
 #submenu li.orcid-button a:active { background: #739022; color: #ffffff; }
 #submenu li.create-button a { background: #925713; color: #ffffff; }
 #submenu li.create-button a:hover { background: #b76d18; }
 #submenu li.create-button a:active { background: #7a4810; }
 #submenu li.save-button a { background: #139257; color: #ffffff; }
@@ -523,35 +497,37 @@
 #submenu li.delete-button a:active { background: #7a1048; }
 img { user-select: none; }
 .loader {
     display: block;
     width: auto;
     min-height: 100px;
     background-color: rgba(255, 255, 255, 0.5);
-    background-image: url('/static/images/loader.svg');
+    background-image: url('/theme/loader.svg');
     background-position: center;
     background-repeat: no-repeat;
     z-index: 100;
 }
 .loader-top {
     display: block;
     width: auto;
     min-height: 100px;
     background-color: rgba(255, 255, 255, 0.5);
-    background-image: url('/static/images/loader.svg');
+    background-image: url('/theme/loader.svg');
     background-position: top;
     background-repeat: no-repeat;
     z-index: 100;
 }
 .no-script { background: #cc0000; color: #ffffff; padding: 1em; }
 .hide-for-javascript { display: none !important; }
 #message { display: none; color: #ffffff; border-radius: .5em; padding: 0em; margin: 0em;  }
 #message p { padding: 1em; }
+#message a { color: #fff; }
 .success { background: #009900; padding: 0em; margin: 0em; }
 .failure { background: #990000; padding: 0em; margin: 0em; }
+.transparent { background: none; padding: 0em; margin: 0em; user-select: none; }
 .hidden { font-size: 0; user-select: none; }
 .center { text-align: center; }
 .no-select { user-select: none; }
 #pre-header {
     display: block;
     width: 100%;
     background: #aa3333;
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/css/pub.css` & `djehuty-24.4/src/djehuty/web/resources/static/css/pub.css`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,21 @@
 #wrapper #content #categories   { padding-top: 10px; clear: left }
 #wrapper #content #tags, #geo, #time_coverage, #dates, #collections, #peer, #references, #publisher, #format, #organizations,
 #wrapper #content #contributors, #funding, #usage, #derived_from, #same_as, #language, #licence, #export, #data_link
                                 { margin-top: 10px }
 #wrapper #content #funding ul   { list-style-type: square; margin-left: 20px }
 #wrapper #content #funding .funder_name { display: block; color: #999 }
 #wrapper #content #files .size  { display: inline-block; width:120px; font-size:12px; color: #999; text-align:right; margin-right:5px }
-#wrapper #content #files #total_size { font-size:12px; color: #999 }
 #wrapper #content #files .md5   { font-size: 75%;  color: #333; font-family: monospace; margin: auto 1em auto 1em; }
 #wrapper #content #metadata #left_column  { width: 65%; margin-bottom:10px }
 #wrapper #content #metadata #right_column { float: right; width: 33%; margin-bottom:10px }
 #wrapper #content .warning      { background-color: #ff0 }
 #wrapper #content .label        { text-transform: uppercase }
-#wrapper #content ul            { list-style-type: none; padding:0; margin:0 }
+#wrapper #content ul            { list-style-type: none; padding:0; margin-top:20px}
 #wrapper #content #data         { clear: right; border-top: 1px solid #000; margin-bottom: 10px }
-#wrapper #content #data ul      { margin-left: 20px }
-#wrapper #content li.zip        { padding: 2px; width: 180px; text-align: center; border: 1px solid #000; border-radius: 10px }
-#wrapper #content li.zip a      { font-weight: bold }
 #wrapper #content #collect,      #cite,      #versions      { display: none; border: 3px solid #f39000; padding: 10px; margin-bottom:10px; border-radius: 10px }
 #wrapper #content #collect_show, #cite_show                 { border: none; padding:3px; margin-bottom: 10px; border-radius: 10px; text-aligh: center; width:70px }
 #wrapper #content #collect_hide, #cite_hide, #versions_hide { border: none }
 #wrapper #content #citation     { font-weight: bold }
 #wrapper #content #type_versions { margin-bottom:10px }
 #wrapper #content #versions     { width: 220px; position:absolute; background-color: #fff }
 #wrapper #content #versions_show { padding: 2px 10px 2px 10px; border: none; background-color: #fff; font: inherit; font-size: inherit; }
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/css/quill.4tu.css` & `djehuty-24.4/src/djehuty/web/resources/static/css/quill.4tu.css`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/FiraMono-Regular.ttf` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/FiraMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/SourceSansPro-Bold.ttf` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/SourceSansPro-Italic.ttf` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/SourceSansPro-Regular.ttf` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-brands-400.eot` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-brands-400.ttf` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-brands-400.woff` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-brands-400.woff2` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-solid-900.eot` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-solid-900.ttf` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-solid-900.woff` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/fonts/fa-solid-900.woff2` & `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/CoreTrustSeal.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/CoreTrustSeal.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/collection-thumb.svg` & `djehuty-24.4/src/djehuty/web/resources/static/images/collection-thumb.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/dataset-thumb.svg` & `djehuty-24.4/src/djehuty/web/resources/static/images/dataset-thumb.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/ext-link.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/ext-link.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/favicon.ico` & `djehuty-24.4/src/djehuty/web/resources/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/favicon.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/licenses/apache.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/apache.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-0.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-0.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by-nc-nd.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc-nd.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by-nc-sa.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc-sa.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by-nc.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by-nd.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nd.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by-sa.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-sa.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/licenses/cc-by.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/licenses/gnu-gpl-v3.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/gnu-gpl-v3.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/loader.svg` & `djehuty-24.4/src/djehuty/web/resources/html_templates/loader.svg`

 * *Files 18% similar despite different names*

```diff
@@ -14,202 +14,209 @@
 000000d0: 2278 4d69 6459 4d69 6422 3e0a 3c67 2074  "xMidYMid">.<g t
 000000e0: 7261 6e73 666f 726d 3d22 726f 7461 7465  ransform="rotate
 000000f0: 2830 2035 3020 3530 2922 3e0a 2020 3c72  (0 50 50)">.  <r
 00000100: 6563 7420 783d 2234 372e 3522 2079 3d22  ect x="47.5" y="
 00000110: 3237 2e35 2220 7278 3d22 322e 3522 2072  27.5" rx="2.5" r
 00000120: 793d 2234 2e39 3522 2077 6964 7468 3d22  y="4.95" width="
 00000130: 3522 2068 6569 6768 743d 2231 3122 2066  5" height="11" f
-00000140: 696c 6c3d 2223 6634 3931 3230 223e 0a20  ill="#f49120">. 
-00000150: 2020 203c 616e 696d 6174 6520 6174 7472     <animate attr
-00000160: 6962 7574 654e 616d 653d 226f 7061 6369  ibuteName="opaci
-00000170: 7479 2220 7661 6c75 6573 3d22 313b 3022  ty" values="1;0"
-00000180: 206b 6579 5469 6d65 733d 2230 3b31 2220   keyTimes="0;1" 
-00000190: 6475 723d 2230 2e38 7322 2062 6567 696e  dur="0.8s" begin
-000001a0: 3d22 2d30 2e37 3333 3333 3333 3333 3333  ="-0.73333333333
-000001b0: 3333 3333 3373 2220 7265 7065 6174 436f  33333s" repeatCo
-000001c0: 756e 743d 2269 6e64 6566 696e 6974 6522  unt="indefinite"
-000001d0: 3e3c 2f61 6e69 6d61 7465 3e0a 2020 3c2f  ></animate>.  </
-000001e0: 7265 6374 3e0a 3c2f 673e 3c67 2074 7261  rect>.</g><g tra
-000001f0: 6e73 666f 726d 3d22 726f 7461 7465 2833  nsform="rotate(3
-00000200: 3020 3530 2035 3029 223e 0a20 203c 7265  0 50 50)">.  <re
-00000210: 6374 2078 3d22 3437 2e35 2220 793d 2232  ct x="47.5" y="2
-00000220: 372e 3522 2072 783d 2232 2e35 2220 7279  7.5" rx="2.5" ry
-00000230: 3d22 342e 3935 2220 7769 6474 683d 2235  ="4.95" width="5
-00000240: 2220 6865 6967 6874 3d22 3131 2220 6669  " height="11" fi
-00000250: 6c6c 3d22 2366 3439 3132 3022 3e0a 2020  ll="#f49120">.  
-00000260: 2020 3c61 6e69 6d61 7465 2061 7474 7269    <animate attri
-00000270: 6275 7465 4e61 6d65 3d22 6f70 6163 6974  buteName="opacit
-00000280: 7922 2076 616c 7565 733d 2231 3b30 2220  y" values="1;0" 
-00000290: 6b65 7954 696d 6573 3d22 303b 3122 2064  keyTimes="0;1" d
-000002a0: 7572 3d22 302e 3873 2220 6265 6769 6e3d  ur="0.8s" begin=
-000002b0: 222d 302e 3636 3636 3636 3636 3636 3636  "-0.666666666666
-000002c0: 3636 3636 7322 2072 6570 6561 7443 6f75  6666s" repeatCou
-000002d0: 6e74 3d22 696e 6465 6669 6e69 7465 223e  nt="indefinite">
-000002e0: 3c2f 616e 696d 6174 653e 0a20 203c 2f72  </animate>.  </r
-000002f0: 6563 743e 0a3c 2f67 3e3c 6720 7472 616e  ect>.</g><g tran
-00000300: 7366 6f72 6d3d 2272 6f74 6174 6528 3630  sform="rotate(60
-00000310: 2035 3020 3530 2922 3e0a 2020 3c72 6563   50 50)">.  <rec
-00000320: 7420 783d 2234 372e 3522 2079 3d22 3237  t x="47.5" y="27
-00000330: 2e35 2220 7278 3d22 322e 3522 2072 793d  .5" rx="2.5" ry=
-00000340: 2234 2e39 3522 2077 6964 7468 3d22 3522  "4.95" width="5"
-00000350: 2068 6569 6768 743d 2231 3122 2066 696c   height="11" fil
-00000360: 6c3d 2223 6634 3931 3230 223e 0a20 2020  l="#f49120">.   
-00000370: 203c 616e 696d 6174 6520 6174 7472 6962   <animate attrib
-00000380: 7574 654e 616d 653d 226f 7061 6369 7479  uteName="opacity
-00000390: 2220 7661 6c75 6573 3d22 313b 3022 206b  " values="1;0" k
-000003a0: 6579 5469 6d65 733d 2230 3b31 2220 6475  eyTimes="0;1" du
-000003b0: 723d 2230 2e38 7322 2062 6567 696e 3d22  r="0.8s" begin="
-000003c0: 2d30 2e36 7322 2072 6570 6561 7443 6f75  -0.6s" repeatCou
-000003d0: 6e74 3d22 696e 6465 6669 6e69 7465 223e  nt="indefinite">
-000003e0: 3c2f 616e 696d 6174 653e 0a20 203c 2f72  </animate>.  </r
-000003f0: 6563 743e 0a3c 2f67 3e3c 6720 7472 616e  ect>.</g><g tran
-00000400: 7366 6f72 6d3d 2272 6f74 6174 6528 3930  sform="rotate(90
-00000410: 2035 3020 3530 2922 3e0a 2020 3c72 6563   50 50)">.  <rec
-00000420: 7420 783d 2234 372e 3522 2079 3d22 3237  t x="47.5" y="27
-00000430: 2e35 2220 7278 3d22 322e 3522 2072 793d  .5" rx="2.5" ry=
-00000440: 2234 2e39 3522 2077 6964 7468 3d22 3522  "4.95" width="5"
-00000450: 2068 6569 6768 743d 2231 3122 2066 696c   height="11" fil
-00000460: 6c3d 2223 6634 3931 3230 223e 0a20 2020  l="#f49120">.   
-00000470: 203c 616e 696d 6174 6520 6174 7472 6962   <animate attrib
-00000480: 7574 654e 616d 653d 226f 7061 6369 7479  uteName="opacity
-00000490: 2220 7661 6c75 6573 3d22 313b 3022 206b  " values="1;0" k
-000004a0: 6579 5469 6d65 733d 2230 3b31 2220 6475  eyTimes="0;1" du
-000004b0: 723d 2230 2e38 7322 2062 6567 696e 3d22  r="0.8s" begin="
-000004c0: 2d30 2e35 3333 3333 3333 3333 3333 3333  -0.5333333333333
-000004d0: 3333 3373 2220 7265 7065 6174 436f 756e  333s" repeatCoun
-000004e0: 743d 2269 6e64 6566 696e 6974 6522 3e3c  t="indefinite"><
-000004f0: 2f61 6e69 6d61 7465 3e0a 2020 3c2f 7265  /animate>.  </re
-00000500: 6374 3e0a 3c2f 673e 3c67 2074 7261 6e73  ct>.</g><g trans
-00000510: 666f 726d 3d22 726f 7461 7465 2831 3230  form="rotate(120
-00000520: 2035 3020 3530 2922 3e0a 2020 3c72 6563   50 50)">.  <rec
-00000530: 7420 783d 2234 372e 3522 2079 3d22 3237  t x="47.5" y="27
-00000540: 2e35 2220 7278 3d22 322e 3522 2072 793d  .5" rx="2.5" ry=
-00000550: 2234 2e39 3522 2077 6964 7468 3d22 3522  "4.95" width="5"
-00000560: 2068 6569 6768 743d 2231 3122 2066 696c   height="11" fil
-00000570: 6c3d 2223 6634 3931 3230 223e 0a20 2020  l="#f49120">.   
-00000580: 203c 616e 696d 6174 6520 6174 7472 6962   <animate attrib
-00000590: 7574 654e 616d 653d 226f 7061 6369 7479  uteName="opacity
-000005a0: 2220 7661 6c75 6573 3d22 313b 3022 206b  " values="1;0" k
-000005b0: 6579 5469 6d65 733d 2230 3b31 2220 6475  eyTimes="0;1" du
-000005c0: 723d 2230 2e38 7322 2062 6567 696e 3d22  r="0.8s" begin="
-000005d0: 2d30 2e34 3636 3636 3636 3636 3636 3636  -0.4666666666666
-000005e0: 3636 3773 2220 7265 7065 6174 436f 756e  667s" repeatCoun
-000005f0: 743d 2269 6e64 6566 696e 6974 6522 3e3c  t="indefinite"><
-00000600: 2f61 6e69 6d61 7465 3e0a 2020 3c2f 7265  /animate>.  </re
-00000610: 6374 3e0a 3c2f 673e 3c67 2074 7261 6e73  ct>.</g><g trans
-00000620: 666f 726d 3d22 726f 7461 7465 2831 3530  form="rotate(150
-00000630: 2035 3020 3530 2922 3e0a 2020 3c72 6563   50 50)">.  <rec
-00000640: 7420 783d 2234 372e 3522 2079 3d22 3237  t x="47.5" y="27
-00000650: 2e35 2220 7278 3d22 322e 3522 2072 793d  .5" rx="2.5" ry=
-00000660: 2234 2e39 3522 2077 6964 7468 3d22 3522  "4.95" width="5"
-00000670: 2068 6569 6768 743d 2231 3122 2066 696c   height="11" fil
-00000680: 6c3d 2223 6634 3931 3230 223e 0a20 2020  l="#f49120">.   
-00000690: 203c 616e 696d 6174 6520 6174 7472 6962   <animate attrib
-000006a0: 7574 654e 616d 653d 226f 7061 6369 7479  uteName="opacity
-000006b0: 2220 7661 6c75 6573 3d22 313b 3022 206b  " values="1;0" k
-000006c0: 6579 5469 6d65 733d 2230 3b31 2220 6475  eyTimes="0;1" du
-000006d0: 723d 2230 2e38 7322 2062 6567 696e 3d22  r="0.8s" begin="
-000006e0: 2d30 2e34 7322 2072 6570 6561 7443 6f75  -0.4s" repeatCou
-000006f0: 6e74 3d22 696e 6465 6669 6e69 7465 223e  nt="indefinite">
-00000700: 3c2f 616e 696d 6174 653e 0a20 203c 2f72  </animate>.  </r
-00000710: 6563 743e 0a3c 2f67 3e3c 6720 7472 616e  ect>.</g><g tran
-00000720: 7366 6f72 6d3d 2272 6f74 6174 6528 3138  sform="rotate(18
-00000730: 3020 3530 2035 3029 223e 0a20 203c 7265  0 50 50)">.  <re
-00000740: 6374 2078 3d22 3437 2e35 2220 793d 2232  ct x="47.5" y="2
-00000750: 372e 3522 2072 783d 2232 2e35 2220 7279  7.5" rx="2.5" ry
-00000760: 3d22 342e 3935 2220 7769 6474 683d 2235  ="4.95" width="5
-00000770: 2220 6865 6967 6874 3d22 3131 2220 6669  " height="11" fi
-00000780: 6c6c 3d22 2366 3439 3132 3022 3e0a 2020  ll="#f49120">.  
-00000790: 2020 3c61 6e69 6d61 7465 2061 7474 7269    <animate attri
-000007a0: 6275 7465 4e61 6d65 3d22 6f70 6163 6974  buteName="opacit
-000007b0: 7922 2076 616c 7565 733d 2231 3b30 2220  y" values="1;0" 
-000007c0: 6b65 7954 696d 6573 3d22 303b 3122 2064  keyTimes="0;1" d
-000007d0: 7572 3d22 302e 3873 2220 6265 6769 6e3d  ur="0.8s" begin=
-000007e0: 222d 302e 3333 3333 3333 3333 3333 3333  "-0.333333333333
-000007f0: 3333 3333 7322 2072 6570 6561 7443 6f75  3333s" repeatCou
-00000800: 6e74 3d22 696e 6465 6669 6e69 7465 223e  nt="indefinite">
-00000810: 3c2f 616e 696d 6174 653e 0a20 203c 2f72  </animate>.  </r
-00000820: 6563 743e 0a3c 2f67 3e3c 6720 7472 616e  ect>.</g><g tran
-00000830: 7366 6f72 6d3d 2272 6f74 6174 6528 3231  sform="rotate(21
-00000840: 3020 3530 2035 3029 223e 0a20 203c 7265  0 50 50)">.  <re
-00000850: 6374 2078 3d22 3437 2e35 2220 793d 2232  ct x="47.5" y="2
-00000860: 372e 3522 2072 783d 2232 2e35 2220 7279  7.5" rx="2.5" ry
-00000870: 3d22 342e 3935 2220 7769 6474 683d 2235  ="4.95" width="5
-00000880: 2220 6865 6967 6874 3d22 3131 2220 6669  " height="11" fi
-00000890: 6c6c 3d22 2366 3439 3132 3022 3e0a 2020  ll="#f49120">.  
-000008a0: 2020 3c61 6e69 6d61 7465 2061 7474 7269    <animate attri
-000008b0: 6275 7465 4e61 6d65 3d22 6f70 6163 6974  buteName="opacit
-000008c0: 7922 2076 616c 7565 733d 2231 3b30 2220  y" values="1;0" 
-000008d0: 6b65 7954 696d 6573 3d22 303b 3122 2064  keyTimes="0;1" d
-000008e0: 7572 3d22 302e 3873 2220 6265 6769 6e3d  ur="0.8s" begin=
-000008f0: 222d 302e 3236 3636 3636 3636 3636 3636  "-0.266666666666
-00000900: 3636 3636 3673 2220 7265 7065 6174 436f  66666s" repeatCo
-00000910: 756e 743d 2269 6e64 6566 696e 6974 6522  unt="indefinite"
-00000920: 3e3c 2f61 6e69 6d61 7465 3e0a 2020 3c2f  ></animate>.  </
-00000930: 7265 6374 3e0a 3c2f 673e 3c67 2074 7261  rect>.</g><g tra
-00000940: 6e73 666f 726d 3d22 726f 7461 7465 2832  nsform="rotate(2
-00000950: 3430 2035 3020 3530 2922 3e0a 2020 3c72  40 50 50)">.  <r
-00000960: 6563 7420 783d 2234 372e 3522 2079 3d22  ect x="47.5" y="
-00000970: 3237 2e35 2220 7278 3d22 322e 3522 2072  27.5" rx="2.5" r
-00000980: 793d 2234 2e39 3522 2077 6964 7468 3d22  y="4.95" width="
-00000990: 3522 2068 6569 6768 743d 2231 3122 2066  5" height="11" f
-000009a0: 696c 6c3d 2223 6634 3931 3230 223e 0a20  ill="#f49120">. 
-000009b0: 2020 203c 616e 696d 6174 6520 6174 7472     <animate attr
-000009c0: 6962 7574 654e 616d 653d 226f 7061 6369  ibuteName="opaci
-000009d0: 7479 2220 7661 6c75 6573 3d22 313b 3022  ty" values="1;0"
-000009e0: 206b 6579 5469 6d65 733d 2230 3b31 2220   keyTimes="0;1" 
-000009f0: 6475 723d 2230 2e38 7322 2062 6567 696e  dur="0.8s" begin
-00000a00: 3d22 2d30 2e32 7322 2072 6570 6561 7443  ="-0.2s" repeatC
-00000a10: 6f75 6e74 3d22 696e 6465 6669 6e69 7465  ount="indefinite
-00000a20: 223e 3c2f 616e 696d 6174 653e 0a20 203c  "></animate>.  <
-00000a30: 2f72 6563 743e 0a3c 2f67 3e3c 6720 7472  /rect>.</g><g tr
-00000a40: 616e 7366 6f72 6d3d 2272 6f74 6174 6528  ansform="rotate(
-00000a50: 3237 3020 3530 2035 3029 223e 0a20 203c  270 50 50)">.  <
-00000a60: 7265 6374 2078 3d22 3437 2e35 2220 793d  rect x="47.5" y=
-00000a70: 2232 372e 3522 2072 783d 2232 2e35 2220  "27.5" rx="2.5" 
-00000a80: 7279 3d22 342e 3935 2220 7769 6474 683d  ry="4.95" width=
-00000a90: 2235 2220 6865 6967 6874 3d22 3131 2220  "5" height="11" 
-00000aa0: 6669 6c6c 3d22 2366 3439 3132 3022 3e0a  fill="#f49120">.
-00000ab0: 2020 2020 3c61 6e69 6d61 7465 2061 7474      <animate att
-00000ac0: 7269 6275 7465 4e61 6d65 3d22 6f70 6163  ributeName="opac
-00000ad0: 6974 7922 2076 616c 7565 733d 2231 3b30  ity" values="1;0
-00000ae0: 2220 6b65 7954 696d 6573 3d22 303b 3122  " keyTimes="0;1"
-00000af0: 2064 7572 3d22 302e 3873 2220 6265 6769   dur="0.8s" begi
-00000b00: 6e3d 222d 302e 3133 3333 3333 3333 3333  n="-0.1333333333
-00000b10: 3333 3333 3333 3373 2220 7265 7065 6174  3333333s" repeat
-00000b20: 436f 756e 743d 2269 6e64 6566 696e 6974  Count="indefinit
-00000b30: 6522 3e3c 2f61 6e69 6d61 7465 3e0a 2020  e"></animate>.  
-00000b40: 3c2f 7265 6374 3e0a 3c2f 673e 3c67 2074  </rect>.</g><g t
-00000b50: 7261 6e73 666f 726d 3d22 726f 7461 7465  ransform="rotate
-00000b60: 2833 3030 2035 3020 3530 2922 3e0a 2020  (300 50 50)">.  
-00000b70: 3c72 6563 7420 783d 2234 372e 3522 2079  <rect x="47.5" y
-00000b80: 3d22 3237 2e35 2220 7278 3d22 322e 3522  ="27.5" rx="2.5"
-00000b90: 2072 793d 2234 2e39 3522 2077 6964 7468   ry="4.95" width
-00000ba0: 3d22 3522 2068 6569 6768 743d 2231 3122  ="5" height="11"
-00000bb0: 2066 696c 6c3d 2223 6634 3931 3230 223e   fill="#f49120">
-00000bc0: 0a20 2020 203c 616e 696d 6174 6520 6174  .    <animate at
-00000bd0: 7472 6962 7574 654e 616d 653d 226f 7061  tributeName="opa
-00000be0: 6369 7479 2220 7661 6c75 6573 3d22 313b  city" values="1;
-00000bf0: 3022 206b 6579 5469 6d65 733d 2230 3b31  0" keyTimes="0;1
-00000c00: 2220 6475 723d 2230 2e38 7322 2062 6567  " dur="0.8s" beg
-00000c10: 696e 3d22 2d30 2e30 3636 3636 3636 3636  in="-0.066666666
-00000c20: 3636 3636 3636 3637 7322 2072 6570 6561  66666667s" repea
-00000c30: 7443 6f75 6e74 3d22 696e 6465 6669 6e69  tCount="indefini
-00000c40: 7465 223e 3c2f 616e 696d 6174 653e 0a20  te"></animate>. 
-00000c50: 203c 2f72 6563 743e 0a3c 2f67 3e3c 6720   </rect>.</g><g 
-00000c60: 7472 616e 7366 6f72 6d3d 2272 6f74 6174  transform="rotat
-00000c70: 6528 3333 3020 3530 2035 3029 223e 0a20  e(330 50 50)">. 
-00000c80: 203c 7265 6374 2078 3d22 3437 2e35 2220   <rect x="47.5" 
-00000c90: 793d 2232 372e 3522 2072 783d 2232 2e35  y="27.5" rx="2.5
-00000ca0: 2220 7279 3d22 342e 3935 2220 7769 6474  " ry="4.95" widt
-00000cb0: 683d 2235 2220 6865 6967 6874 3d22 3131  h="5" height="11
-00000cc0: 2220 6669 6c6c 3d22 2366 3439 3132 3022  " fill="#f49120"
-00000cd0: 3e0a 2020 2020 3c61 6e69 6d61 7465 2061  >.    <animate a
-00000ce0: 7474 7269 6275 7465 4e61 6d65 3d22 6f70  ttributeName="op
-00000cf0: 6163 6974 7922 2076 616c 7565 733d 2231  acity" values="1
-00000d00: 3b30 2220 6b65 7954 696d 6573 3d22 303b  ;0" keyTimes="0;
-00000d10: 3122 2064 7572 3d22 302e 3873 2220 6265  1" dur="0.8s" be
-00000d20: 6769 6e3d 2230 7322 2072 6570 6561 7443  gin="0s" repeatC
-00000d30: 6f75 6e74 3d22 696e 6465 6669 6e69 7465  ount="indefinite
-00000d40: 223e 3c2f 616e 696d 6174 653e 0a20 203c  "></animate>.  <
-00000d50: 2f72 6563 743e 0a3c 2f67 3e0a 3c2f 7376  /rect>.</g>.</sv
-00000d60: 673e 0a                                  g>.
+00000140: 696c 6c3d 227b 7b70 7269 6d61 7279 5f63  ill="{{primary_c
+00000150: 6f6c 6f72 7d7d 223e 0a20 2020 203c 616e  olor}}">.    <an
+00000160: 696d 6174 6520 6174 7472 6962 7574 654e  imate attributeN
+00000170: 616d 653d 226f 7061 6369 7479 2220 7661  ame="opacity" va
+00000180: 6c75 6573 3d22 313b 3022 206b 6579 5469  lues="1;0" keyTi
+00000190: 6d65 733d 2230 3b31 2220 6475 723d 2230  mes="0;1" dur="0
+000001a0: 2e38 7322 2062 6567 696e 3d22 2d30 2e37  .8s" begin="-0.7
+000001b0: 3333 3333 3333 3333 3333 3333 3333 3373  333333333333333s
+000001c0: 2220 7265 7065 6174 436f 756e 743d 2269  " repeatCount="i
+000001d0: 6e64 6566 696e 6974 6522 3e3c 2f61 6e69  ndefinite"></ani
+000001e0: 6d61 7465 3e0a 2020 3c2f 7265 6374 3e0a  mate>.  </rect>.
+000001f0: 3c2f 673e 3c67 2074 7261 6e73 666f 726d  </g><g transform
+00000200: 3d22 726f 7461 7465 2833 3020 3530 2035  ="rotate(30 50 5
+00000210: 3029 223e 0a20 203c 7265 6374 2078 3d22  0)">.  <rect x="
+00000220: 3437 2e35 2220 793d 2232 372e 3522 2072  47.5" y="27.5" r
+00000230: 783d 2232 2e35 2220 7279 3d22 342e 3935  x="2.5" ry="4.95
+00000240: 2220 7769 6474 683d 2235 2220 6865 6967  " width="5" heig
+00000250: 6874 3d22 3131 2220 6669 6c6c 3d22 7b7b  ht="11" fill="{{
+00000260: 7072 696d 6172 795f 636f 6c6f 727d 7d22  primary_color}}"
+00000270: 3e0a 2020 2020 3c61 6e69 6d61 7465 2061  >.    <animate a
+00000280: 7474 7269 6275 7465 4e61 6d65 3d22 6f70  ttributeName="op
+00000290: 6163 6974 7922 2076 616c 7565 733d 2231  acity" values="1
+000002a0: 3b30 2220 6b65 7954 696d 6573 3d22 303b  ;0" keyTimes="0;
+000002b0: 3122 2064 7572 3d22 302e 3873 2220 6265  1" dur="0.8s" be
+000002c0: 6769 6e3d 222d 302e 3636 3636 3636 3636  gin="-0.66666666
+000002d0: 3636 3636 3636 3636 7322 2072 6570 6561  66666666s" repea
+000002e0: 7443 6f75 6e74 3d22 696e 6465 6669 6e69  tCount="indefini
+000002f0: 7465 223e 3c2f 616e 696d 6174 653e 0a20  te"></animate>. 
+00000300: 203c 2f72 6563 743e 0a3c 2f67 3e3c 6720   </rect>.</g><g 
+00000310: 7472 616e 7366 6f72 6d3d 2272 6f74 6174  transform="rotat
+00000320: 6528 3630 2035 3020 3530 2922 3e0a 2020  e(60 50 50)">.  
+00000330: 3c72 6563 7420 783d 2234 372e 3522 2079  <rect x="47.5" y
+00000340: 3d22 3237 2e35 2220 7278 3d22 322e 3522  ="27.5" rx="2.5"
+00000350: 2072 793d 2234 2e39 3522 2077 6964 7468   ry="4.95" width
+00000360: 3d22 3522 2068 6569 6768 743d 2231 3122  ="5" height="11"
+00000370: 2066 696c 6c3d 227b 7b70 7269 6d61 7279   fill="{{primary
+00000380: 5f63 6f6c 6f72 7d7d 223e 0a20 2020 203c  _color}}">.    <
+00000390: 616e 696d 6174 6520 6174 7472 6962 7574  animate attribut
+000003a0: 654e 616d 653d 226f 7061 6369 7479 2220  eName="opacity" 
+000003b0: 7661 6c75 6573 3d22 313b 3022 206b 6579  values="1;0" key
+000003c0: 5469 6d65 733d 2230 3b31 2220 6475 723d  Times="0;1" dur=
+000003d0: 2230 2e38 7322 2062 6567 696e 3d22 2d30  "0.8s" begin="-0
+000003e0: 2e36 7322 2072 6570 6561 7443 6f75 6e74  .6s" repeatCount
+000003f0: 3d22 696e 6465 6669 6e69 7465 223e 3c2f  ="indefinite"></
+00000400: 616e 696d 6174 653e 0a20 203c 2f72 6563  animate>.  </rec
+00000410: 743e 0a3c 2f67 3e3c 6720 7472 616e 7366  t>.</g><g transf
+00000420: 6f72 6d3d 2272 6f74 6174 6528 3930 2035  orm="rotate(90 5
+00000430: 3020 3530 2922 3e0a 2020 3c72 6563 7420  0 50)">.  <rect 
+00000440: 783d 2234 372e 3522 2079 3d22 3237 2e35  x="47.5" y="27.5
+00000450: 2220 7278 3d22 322e 3522 2072 793d 2234  " rx="2.5" ry="4
+00000460: 2e39 3522 2077 6964 7468 3d22 3522 2068  .95" width="5" h
+00000470: 6569 6768 743d 2231 3122 2066 696c 6c3d  eight="11" fill=
+00000480: 227b 7b70 7269 6d61 7279 5f63 6f6c 6f72  "{{primary_color
+00000490: 7d7d 223e 0a20 2020 203c 616e 696d 6174  }}">.    <animat
+000004a0: 6520 6174 7472 6962 7574 654e 616d 653d  e attributeName=
+000004b0: 226f 7061 6369 7479 2220 7661 6c75 6573  "opacity" values
+000004c0: 3d22 313b 3022 206b 6579 5469 6d65 733d  ="1;0" keyTimes=
+000004d0: 2230 3b31 2220 6475 723d 2230 2e38 7322  "0;1" dur="0.8s"
+000004e0: 2062 6567 696e 3d22 2d30 2e35 3333 3333   begin="-0.53333
+000004f0: 3333 3333 3333 3333 3333 3373 2220 7265  33333333333s" re
+00000500: 7065 6174 436f 756e 743d 2269 6e64 6566  peatCount="indef
+00000510: 696e 6974 6522 3e3c 2f61 6e69 6d61 7465  inite"></animate
+00000520: 3e0a 2020 3c2f 7265 6374 3e0a 3c2f 673e  >.  </rect>.</g>
+00000530: 3c67 2074 7261 6e73 666f 726d 3d22 726f  <g transform="ro
+00000540: 7461 7465 2831 3230 2035 3020 3530 2922  tate(120 50 50)"
+00000550: 3e0a 2020 3c72 6563 7420 783d 2234 372e  >.  <rect x="47.
+00000560: 3522 2079 3d22 3237 2e35 2220 7278 3d22  5" y="27.5" rx="
+00000570: 322e 3522 2072 793d 2234 2e39 3522 2077  2.5" ry="4.95" w
+00000580: 6964 7468 3d22 3522 2068 6569 6768 743d  idth="5" height=
+00000590: 2231 3122 2066 696c 6c3d 227b 7b70 7269  "11" fill="{{pri
+000005a0: 6d61 7279 5f63 6f6c 6f72 7d7d 223e 0a20  mary_color}}">. 
+000005b0: 2020 203c 616e 696d 6174 6520 6174 7472     <animate attr
+000005c0: 6962 7574 654e 616d 653d 226f 7061 6369  ibuteName="opaci
+000005d0: 7479 2220 7661 6c75 6573 3d22 313b 3022  ty" values="1;0"
+000005e0: 206b 6579 5469 6d65 733d 2230 3b31 2220   keyTimes="0;1" 
+000005f0: 6475 723d 2230 2e38 7322 2062 6567 696e  dur="0.8s" begin
+00000600: 3d22 2d30 2e34 3636 3636 3636 3636 3636  ="-0.46666666666
+00000610: 3636 3636 3773 2220 7265 7065 6174 436f  66667s" repeatCo
+00000620: 756e 743d 2269 6e64 6566 696e 6974 6522  unt="indefinite"
+00000630: 3e3c 2f61 6e69 6d61 7465 3e0a 2020 3c2f  ></animate>.  </
+00000640: 7265 6374 3e0a 3c2f 673e 3c67 2074 7261  rect>.</g><g tra
+00000650: 6e73 666f 726d 3d22 726f 7461 7465 2831  nsform="rotate(1
+00000660: 3530 2035 3020 3530 2922 3e0a 2020 3c72  50 50 50)">.  <r
+00000670: 6563 7420 783d 2234 372e 3522 2079 3d22  ect x="47.5" y="
+00000680: 3237 2e35 2220 7278 3d22 322e 3522 2072  27.5" rx="2.5" r
+00000690: 793d 2234 2e39 3522 2077 6964 7468 3d22  y="4.95" width="
+000006a0: 3522 2068 6569 6768 743d 2231 3122 2066  5" height="11" f
+000006b0: 696c 6c3d 227b 7b70 7269 6d61 7279 5f63  ill="{{primary_c
+000006c0: 6f6c 6f72 7d7d 223e 0a20 2020 203c 616e  olor}}">.    <an
+000006d0: 696d 6174 6520 6174 7472 6962 7574 654e  imate attributeN
+000006e0: 616d 653d 226f 7061 6369 7479 2220 7661  ame="opacity" va
+000006f0: 6c75 6573 3d22 313b 3022 206b 6579 5469  lues="1;0" keyTi
+00000700: 6d65 733d 2230 3b31 2220 6475 723d 2230  mes="0;1" dur="0
+00000710: 2e38 7322 2062 6567 696e 3d22 2d30 2e34  .8s" begin="-0.4
+00000720: 7322 2072 6570 6561 7443 6f75 6e74 3d22  s" repeatCount="
+00000730: 696e 6465 6669 6e69 7465 223e 3c2f 616e  indefinite"></an
+00000740: 696d 6174 653e 0a20 203c 2f72 6563 743e  imate>.  </rect>
+00000750: 0a3c 2f67 3e3c 6720 7472 616e 7366 6f72  .</g><g transfor
+00000760: 6d3d 2272 6f74 6174 6528 3138 3020 3530  m="rotate(180 50
+00000770: 2035 3029 223e 0a20 203c 7265 6374 2078   50)">.  <rect x
+00000780: 3d22 3437 2e35 2220 793d 2232 372e 3522  ="47.5" y="27.5"
+00000790: 2072 783d 2232 2e35 2220 7279 3d22 342e   rx="2.5" ry="4.
+000007a0: 3935 2220 7769 6474 683d 2235 2220 6865  95" width="5" he
+000007b0: 6967 6874 3d22 3131 2220 6669 6c6c 3d22  ight="11" fill="
+000007c0: 7b7b 7072 696d 6172 795f 636f 6c6f 727d  {{primary_color}
+000007d0: 7d22 3e0a 2020 2020 3c61 6e69 6d61 7465  }">.    <animate
+000007e0: 2061 7474 7269 6275 7465 4e61 6d65 3d22   attributeName="
+000007f0: 6f70 6163 6974 7922 2076 616c 7565 733d  opacity" values=
+00000800: 2231 3b30 2220 6b65 7954 696d 6573 3d22  "1;0" keyTimes="
+00000810: 303b 3122 2064 7572 3d22 302e 3873 2220  0;1" dur="0.8s" 
+00000820: 6265 6769 6e3d 222d 302e 3333 3333 3333  begin="-0.333333
+00000830: 3333 3333 3333 3333 3333 7322 2072 6570  3333333333s" rep
+00000840: 6561 7443 6f75 6e74 3d22 696e 6465 6669  eatCount="indefi
+00000850: 6e69 7465 223e 3c2f 616e 696d 6174 653e  nite"></animate>
+00000860: 0a20 203c 2f72 6563 743e 0a3c 2f67 3e3c  .  </rect>.</g><
+00000870: 6720 7472 616e 7366 6f72 6d3d 2272 6f74  g transform="rot
+00000880: 6174 6528 3231 3020 3530 2035 3029 223e  ate(210 50 50)">
+00000890: 0a20 203c 7265 6374 2078 3d22 3437 2e35  .  <rect x="47.5
+000008a0: 2220 793d 2232 372e 3522 2072 783d 2232  " y="27.5" rx="2
+000008b0: 2e35 2220 7279 3d22 342e 3935 2220 7769  .5" ry="4.95" wi
+000008c0: 6474 683d 2235 2220 6865 6967 6874 3d22  dth="5" height="
+000008d0: 3131 2220 6669 6c6c 3d22 7b7b 7072 696d  11" fill="{{prim
+000008e0: 6172 795f 636f 6c6f 727d 7d22 3e0a 2020  ary_color}}">.  
+000008f0: 2020 3c61 6e69 6d61 7465 2061 7474 7269    <animate attri
+00000900: 6275 7465 4e61 6d65 3d22 6f70 6163 6974  buteName="opacit
+00000910: 7922 2076 616c 7565 733d 2231 3b30 2220  y" values="1;0" 
+00000920: 6b65 7954 696d 6573 3d22 303b 3122 2064  keyTimes="0;1" d
+00000930: 7572 3d22 302e 3873 2220 6265 6769 6e3d  ur="0.8s" begin=
+00000940: 222d 302e 3236 3636 3636 3636 3636 3636  "-0.266666666666
+00000950: 3636 3636 3673 2220 7265 7065 6174 436f  66666s" repeatCo
+00000960: 756e 743d 2269 6e64 6566 696e 6974 6522  unt="indefinite"
+00000970: 3e3c 2f61 6e69 6d61 7465 3e0a 2020 3c2f  ></animate>.  </
+00000980: 7265 6374 3e0a 3c2f 673e 3c67 2074 7261  rect>.</g><g tra
+00000990: 6e73 666f 726d 3d22 726f 7461 7465 2832  nsform="rotate(2
+000009a0: 3430 2035 3020 3530 2922 3e0a 2020 3c72  40 50 50)">.  <r
+000009b0: 6563 7420 783d 2234 372e 3522 2079 3d22  ect x="47.5" y="
+000009c0: 3237 2e35 2220 7278 3d22 322e 3522 2072  27.5" rx="2.5" r
+000009d0: 793d 2234 2e39 3522 2077 6964 7468 3d22  y="4.95" width="
+000009e0: 3522 2068 6569 6768 743d 2231 3122 2066  5" height="11" f
+000009f0: 696c 6c3d 227b 7b70 7269 6d61 7279 5f63  ill="{{primary_c
+00000a00: 6f6c 6f72 7d7d 223e 0a20 2020 203c 616e  olor}}">.    <an
+00000a10: 696d 6174 6520 6174 7472 6962 7574 654e  imate attributeN
+00000a20: 616d 653d 226f 7061 6369 7479 2220 7661  ame="opacity" va
+00000a30: 6c75 6573 3d22 313b 3022 206b 6579 5469  lues="1;0" keyTi
+00000a40: 6d65 733d 2230 3b31 2220 6475 723d 2230  mes="0;1" dur="0
+00000a50: 2e38 7322 2062 6567 696e 3d22 2d30 2e32  .8s" begin="-0.2
+00000a60: 7322 2072 6570 6561 7443 6f75 6e74 3d22  s" repeatCount="
+00000a70: 696e 6465 6669 6e69 7465 223e 3c2f 616e  indefinite"></an
+00000a80: 696d 6174 653e 0a20 203c 2f72 6563 743e  imate>.  </rect>
+00000a90: 0a3c 2f67 3e3c 6720 7472 616e 7366 6f72  .</g><g transfor
+00000aa0: 6d3d 2272 6f74 6174 6528 3237 3020 3530  m="rotate(270 50
+00000ab0: 2035 3029 223e 0a20 203c 7265 6374 2078   50)">.  <rect x
+00000ac0: 3d22 3437 2e35 2220 793d 2232 372e 3522  ="47.5" y="27.5"
+00000ad0: 2072 783d 2232 2e35 2220 7279 3d22 342e   rx="2.5" ry="4.
+00000ae0: 3935 2220 7769 6474 683d 2235 2220 6865  95" width="5" he
+00000af0: 6967 6874 3d22 3131 2220 6669 6c6c 3d22  ight="11" fill="
+00000b00: 7b7b 7072 696d 6172 795f 636f 6c6f 727d  {{primary_color}
+00000b10: 7d22 3e0a 2020 2020 3c61 6e69 6d61 7465  }">.    <animate
+00000b20: 2061 7474 7269 6275 7465 4e61 6d65 3d22   attributeName="
+00000b30: 6f70 6163 6974 7922 2076 616c 7565 733d  opacity" values=
+00000b40: 2231 3b30 2220 6b65 7954 696d 6573 3d22  "1;0" keyTimes="
+00000b50: 303b 3122 2064 7572 3d22 302e 3873 2220  0;1" dur="0.8s" 
+00000b60: 6265 6769 6e3d 222d 302e 3133 3333 3333  begin="-0.133333
+00000b70: 3333 3333 3333 3333 3333 3373 2220 7265  33333333333s" re
+00000b80: 7065 6174 436f 756e 743d 2269 6e64 6566  peatCount="indef
+00000b90: 696e 6974 6522 3e3c 2f61 6e69 6d61 7465  inite"></animate
+00000ba0: 3e0a 2020 3c2f 7265 6374 3e0a 3c2f 673e  >.  </rect>.</g>
+00000bb0: 3c67 2074 7261 6e73 666f 726d 3d22 726f  <g transform="ro
+00000bc0: 7461 7465 2833 3030 2035 3020 3530 2922  tate(300 50 50)"
+00000bd0: 3e0a 2020 3c72 6563 7420 783d 2234 372e  >.  <rect x="47.
+00000be0: 3522 2079 3d22 3237 2e35 2220 7278 3d22  5" y="27.5" rx="
+00000bf0: 322e 3522 2072 793d 2234 2e39 3522 2077  2.5" ry="4.95" w
+00000c00: 6964 7468 3d22 3522 2068 6569 6768 743d  idth="5" height=
+00000c10: 2231 3122 2066 696c 6c3d 227b 7b70 7269  "11" fill="{{pri
+00000c20: 6d61 7279 5f63 6f6c 6f72 7d7d 223e 0a20  mary_color}}">. 
+00000c30: 2020 203c 616e 696d 6174 6520 6174 7472     <animate attr
+00000c40: 6962 7574 654e 616d 653d 226f 7061 6369  ibuteName="opaci
+00000c50: 7479 2220 7661 6c75 6573 3d22 313b 3022  ty" values="1;0"
+00000c60: 206b 6579 5469 6d65 733d 2230 3b31 2220   keyTimes="0;1" 
+00000c70: 6475 723d 2230 2e38 7322 2062 6567 696e  dur="0.8s" begin
+00000c80: 3d22 2d30 2e30 3636 3636 3636 3636 3636  ="-0.06666666666
+00000c90: 3636 3636 3637 7322 2072 6570 6561 7443  666667s" repeatC
+00000ca0: 6f75 6e74 3d22 696e 6465 6669 6e69 7465  ount="indefinite
+00000cb0: 223e 3c2f 616e 696d 6174 653e 0a20 203c  "></animate>.  <
+00000cc0: 2f72 6563 743e 0a3c 2f67 3e3c 6720 7472  /rect>.</g><g tr
+00000cd0: 616e 7366 6f72 6d3d 2272 6f74 6174 6528  ansform="rotate(
+00000ce0: 3333 3020 3530 2035 3029 223e 0a20 203c  330 50 50)">.  <
+00000cf0: 7265 6374 2078 3d22 3437 2e35 2220 793d  rect x="47.5" y=
+00000d00: 2232 372e 3522 2072 783d 2232 2e35 2220  "27.5" rx="2.5" 
+00000d10: 7279 3d22 342e 3935 2220 7769 6474 683d  ry="4.95" width=
+00000d20: 2235 2220 6865 6967 6874 3d22 3131 2220  "5" height="11" 
+00000d30: 6669 6c6c 3d22 7b7b 7072 696d 6172 795f  fill="{{primary_
+00000d40: 636f 6c6f 727d 7d22 3e0a 2020 2020 3c61  color}}">.    <a
+00000d50: 6e69 6d61 7465 2061 7474 7269 6275 7465  nimate attribute
+00000d60: 4e61 6d65 3d22 6f70 6163 6974 7922 2076  Name="opacity" v
+00000d70: 616c 7565 733d 2231 3b30 2220 6b65 7954  alues="1;0" keyT
+00000d80: 696d 6573 3d22 303b 3122 2064 7572 3d22  imes="0;1" dur="
+00000d90: 302e 3873 2220 6265 6769 6e3d 2230 7322  0.8s" begin="0s"
+00000da0: 2072 6570 6561 7443 6f75 6e74 3d22 696e   repeatCount="in
+00000db0: 6465 6669 6e69 7465 223e 3c2f 616e 696d  definite"></anim
+00000dc0: 6174 653e 0a20 203c 2f72 6563 743e 0a3c  ate>.  </rect>.<
+00000dd0: 2f67 3e0a 3c2f 7376 673e 0a              /g>.</svg>.
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/logo-delft.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/logo-delft.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/logo-eindhoven.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/logo-eindhoven.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/logo-gray.svg` & `djehuty-24.4/src/djehuty/web/resources/static/images/logo-gray.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/logo-other.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/logo-other.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/logo-twente.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/logo-twente.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/logo-wageningen.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/logo-wageningen.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/logo.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/logosleft-white-tudelft.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-tudelft.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/logosleft-white-tutwente.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-tutwente.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/logosleft-white-wageningen.png` & `djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-wageningen.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/nikhef-black.svg` & `djehuty-24.4/src/djehuty/web/resources/static/images/nikhef-black.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/orcid.svg` & `djehuty-24.4/src/djehuty/web/resources/static/images/orcid.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/aerospace-engineering.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/aerospace-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/agricultural-and-veterinary-sciences.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/agricultural-and-veterinary-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/atmospheric-sciences.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/atmospheric-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/biology.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/biology.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/built-environment-and-design.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/built-environment-and-design.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/business-and-management.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/business-and-management.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/chemistry.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/chemistry.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/civil-engineering.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/civil-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/earth-sciences.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/earth-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/electrical-and-electronic-engineering.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/electrical-and-electronic-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/environmental-sciences.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/environmental-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/geomatic-engineering.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/geomatic-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/information-and-computing-sciences.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/information-and-computing-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/materials-engineering.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/materials-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/mathematics.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/mathematics.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/mechanical-engineering.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/mechanical-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/medical-and-health-sciences.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/medical-and-health-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/nanotechnology.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/nanotechnology.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/other-institutions.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/other-institutions.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/physical-geography-and-environmental-geoscience.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/physical-geography-and-environmental-geoscience.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/physics.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/physics.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/tudelft.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/tudelft.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/tueindhoven.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/tueindhoven.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/utwente.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/utwente.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/images/portal/wageningen.jpg` & `djehuty-24.4/src/djehuty/web/resources/static/images/portal/wageningen.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/ace/ace.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/ace/ace.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/ace/ext-language_tools.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/ace/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/ace/ext-searchbox.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/ace/ext-searchbox.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/ace/mode-sparql.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/ace/mode-sparql.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/ace/theme-crimson_editor.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/ace/theme-crimson_editor.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/d3.v7.min.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/d3.v7.min.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/dataset_landing_page.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/dataset_landing_page.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/depositor-dashboard.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/depositor-dashboard.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/dropzone.min.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/edit-collection.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/edit-collection.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/edit-dataset.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/edit-dataset.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -438,33 +438,109 @@
         }
         jQuery("#tags-list").show();
     }).fail(function() {
         show_message("failure", "<p>Failed to retrieve tags.</p>");
     });
 }
 
+function cancel_edit_author(author_uuid, dataset_uuid) {
+    jQuery("#author-inline-edit-form").remove();
+    jQuery(`#edit-author-${author_uuid}`).attr("onclick",
+            `javascript:edit_author('${author_uuid}', ` +
+            `'${dataset_uuid}'); return false`)
+        .removeClass("fa-times")
+        .removeClass("fa-lg")
+        .addClass("fa-pen");
+}
+
+function update_author(author_uuid, dataset_uuid) {
+    let record = {
+        "first_name": jQuery("#edit_author_first_name").val(),
+        "last_name": jQuery("#edit_author_last_name").val(),
+        "email": jQuery("#edit_author_email").val(),
+        "orcid": jQuery("#edit_author_orcid").val()
+    }
+    jQuery.ajax({
+        url: `/v3/authors/${author_uuid}`,
+        data: JSON.stringify(record),
+        type: "PUT",
+        contentType: "application/json",
+        accept: "application/json",
+    }).done(function() {
+        cancel_edit_author(author_uuid, dataset_uuid);
+        render_authors_for_dataset(dataset_uuid);
+    }).fail(function() {
+        show_message("failure", "<p>Failed to update author details.</p>");
+    })
+}
+
+function edit_author(author_uuid, dataset_uuid) {
+    jQuery.ajax({
+        url: `/v3/datasets/${dataset_uuid}/authors/${author_uuid}`,
+        type: "GET",
+        accept: "application/json",
+    }).done(function(author) {
+        let html = `<tr id="author-inline-edit-form"><td colspan="3">`;
+        html += `<label for="author_first_name">First name</label>`;
+        html += `<input type="text" id="edit_author_first_name" name="author_first_name" value="${or_empty (author.first_name)}">`;
+        html += `<label for="author_last_name">Last name</label>`;
+        html += `<input type="text" id="edit_author_last_name" name="author_last_name" value="${or_empty (author.last_name)}">`;
+        html += `<label for="author_email">E-mail address</label>`;
+        html += `<input type="text" id="edit_author_email" name="author_email" value="${or_empty (author.email)}">`;
+        html += `<label for="author_orcid">ORCID</label>`;
+        html += `<input type="text" id="edit_author_orcid" name="author_orcid" value="${or_empty (author.orcid)}">`;
+        html += `<div id="update-author" class="a-button">`;
+        html += `<a href="#" onclick="javascript:update_author(`;
+        html += `'${author_uuid}', '${dataset_uuid}'); `;
+        html += `return false;">Update author</a></div>`;
+        html += `</td></tr>`;
+
+        jQuery(`#author-${author_uuid}`).after(html);
+        jQuery(`#edit-author-${author_uuid}`)
+            .removeClass("fa-pen")
+            .addClass("fa-times")
+            .addClass("fa-lg")
+            .attr("onclick",
+                `javascript:cancel_edit_author('${author_uuid}', ` +
+                `'${dataset_uuid}'); return false;`);
+    });
+}
+
 function render_authors_for_dataset(dataset_uuid) {
     jQuery.ajax({
-        url: `/v2/account/articles/${dataset_uuid}/authors`,
+        url: `/v3/datasets/${dataset_uuid}/authors`,
         data: {
-            "limit": 10000,
-            "order": "asc",
-            "order_direction": "id"
+            "limit": 10000
         },
         type: "GET",
         accept: "application/json",
     }).done(function(authors) {
         jQuery("#authors-list tbody").empty();
         for (let author of authors) {
-            let row = `<tr><td>${author.full_name}`;
-            if (author.orcid_id != null && author.orcid_id != "") {
-                row += ` (${author.orcid_id})`;
+            let row = `<tr id="author-${author.uuid}"><td>${author.full_name}`;
+            let orcid = null;
+            if (author.orcid_id && author.orcid_id != "") {
+                orcid = author.orcid_id;
+            } else
+            if (author.orcid && author.orcid != "") {
+                orcid = author.orcid;
+            }
+            if (orcid !== null) {
+                row += ` <a href="https://orcid.org/${orcid}" `;
+                row += `target="_blank" rel="noopener noreferrer"><img `;
+                row += `src="/static/images/orcid.svg" style="height: 15px" `;
+                row += `alt="ORCID" title="ORCID profile (new window)" /></a>`;
+            }
+            if (author.is_editable) {
+                row += `</td><td><a id="edit-author-${author.uuid}" href="#" onclick="javascript:edit_author('${author.uuid}', `;
+                row += `'${dataset_uuid}'); return false" class="fas fa-pen" title="Edit"></a>`;
+            } else {
+                row += "</td><td>";
             }
-            row += `</td><td><a href="#" `;
-            row += `onclick="javascript:remove_author('${author.uuid}', `;
+            row += `</td><td><a href="#" onclick="javascript:remove_author('${author.uuid}', `;
             row += `'${dataset_uuid}'); return false;" class="fas fa-trash-can" `;
             row += `title="Remove"></a></td></tr>`;
             jQuery("#authors-list tbody").append(row);
         }
         jQuery("#authors-list").show();
     }).fail(function() {
         show_message("failure", "<p>Failed to retrieve author details.</p>");
@@ -1191,14 +1267,17 @@
 
         jQuery("#delete").on("click", function(event) {
             delete_dataset(dataset_uuid, event);
         });
         jQuery("#save").on("click", function(event) {
             save_dataset(dataset_uuid, event);
         });
+        jQuery("#save_bottom").on("click", function(event) {
+            save_dataset(dataset_uuid, event);
+        });
         jQuery("#submit").on("click", function(event) {
             submit_dataset(dataset_uuid, event);
         });
         jQuery("#publish").on("click", function(event) {
             publish_dataset(dataset_uuid, event);
         });
         jQuery("#decline").on("click", function(event) {
```

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/edit-profile.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/edit-profile.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/exploratory.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/exploratory.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/jquery-3.6.0.min.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/jquery.dataTables.min.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/query-editor.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/query-editor.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/quill.min.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/quill.min.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/ranking.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/ranking.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/review-overview.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/review-overview.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/search.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/search.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/resources/static/js/utils.js` & `djehuty-24.4/src/djehuty/web/resources/static/js/utils.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -2,24 +2,31 @@
     return [text].join('');
 }
 
 function or_null(value) {
     return (value == "" || value == "<p><br></p>") ? null : value;
 }
 
+function or_empty(value) {
+    return (value === undefined || value == null || value == "") ? "" : value;
+}
+
 function show_message(type, message) {
+    if (jQuery("#message.transparent").length > 0) {
+        jQuery("#message").removeClass("transparent").empty();
+    }
     jQuery("#message")
         .addClass(type)
         .append(message)
         .fadeIn(250);
     setTimeout(function() {
         jQuery("#message").fadeOut(500, function() {
-            jQuery("#message").removeClass(type).empty();
+            jQuery("#message").removeClass(type).addClass("transparent").html("<p>&nbsp;</p>").show();
         });
-    }, 5000);
+    }, 20000);
 }
 
 function install_sticky_header() {
     var submenu_offset = jQuery("#submenu").offset().top;
     jQuery(window).on('resize scroll', function() {
         let scroll_offset = jQuery(window).scrollTop();
         if (submenu_offset <= scroll_offset) {
@@ -27,14 +34,17 @@
             jQuery("#message").addClass("sticky-message");
             jQuery("h1").addClass("sticky-margin");
             jQuery("#message").width(jQuery("#content-wrapper").width());
         } else {
             jQuery("#submenu").removeClass("sticky");
             jQuery("#message").removeClass("sticky-message");
             jQuery("h1").removeClass("sticky-margin");
+            if (jQuery("#message.transparent").length > 0) {
+                jQuery("#message").removeClass("transparent").empty().hide();
+            }
         }
     });
 }
 
 function install_touchable_help_icons() {
     jQuery(".help-icon").on("click", function() {
         let selector = jQuery(this).find(".help-text");
```

### Comparing `djehuty-24.3/src/djehuty/web/ui.py` & `djehuty-24.4/src/djehuty/web/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,14 +352,15 @@
             lowercase_email = email.lower()
             server.db.privileges[lowercase_email] = {
                 "may_administer":  bool(int(config_value (account, "may-administer", None, False))),
                 "may_query":       bool(int(config_value (account, "may-run-sparql-queries", None, False))),
                 "may_impersonate": bool(int(config_value (account, "may-impersonate", None, False))),
                 "may_review":      bool(int(config_value (account, "may-review", None, False))),
                 "may_review_quotas": bool(int(config_value (account, "may-review-quotas", None, False))),
+                "may_review_integrity": bool(int(config_value (account, "may-review-integrity", None, False))),
                 "may_process_feedback": bool(int(config_value (account, "may-process-feedback", None, False))),
                 "may_receive_email_notifications": bool(int(config_value (account, "may-receive-email-notifications", None, True))),
                 "orcid":           orcid
             }
 
             ## The "needs_2fa" property is set to True when the user has any
             ## extra privilege.
@@ -447,14 +448,23 @@
             code = 302
             if "code" in redirect_to.attrib:
                 code = int(redirect_to.attrib["code"])
             server.static_pages[uri_path] = {"redirect-to": redirect_to.text, "code": code}
             if not inside_reload:
                 logger.info ("Loaded redirect (%i): %s -> %s", code, uri_path, redirect_to.text)
 
+def read_colors_configuration (server, xml_root):
+    """Procedure to parse and set the color scheme configuration."""
+    colors = xml_root.find("colors")
+    if colors:
+        for color in ["primary-color", "primary-color-hover",
+                      "primary-color-active", "privilege-button-color",
+                      "footer-background-color"]:
+            server.colors[color] = config_value (colors, color, fallback=server.colors[color])
+
 def read_datacite_configuration (server, xml_root):
     """Procedure to parse and set the DataCite API configuration."""
     datacite = xml_root.find("datacite")
     if datacite:
         server.datacite_url      = config_value (datacite, "api-url")
         server.datacite_id       = config_value (datacite, "repository-id")
         server.datacite_password = config_value (datacite, "password")
@@ -667,21 +677,30 @@
         if site_name is not None:
             server.site_name = site_name.text
 
         site_description = xml_root.find ("site-description")
         if site_description is not None:
             server.site_description = site_description.text
 
+        site_shorttag = xml_root.find ("site-shorttag")
+        if site_shorttag is not None:
+            server.site_shorttag = site_shorttag.text
+
+        support_email_address = xml_root.find ("support-email-address")
+        if support_email_address is not None:
+            server.support_email_address = support_email_address.text
+
         read_orcid_configuration (server, xml_root)
         read_datacite_configuration (server, xml_root)
         read_email_configuration (server, xml_root, logger)
         read_saml_configuration (server, xml_root, logger)
         read_automatic_login_configuration (server, xml_root)
         read_privilege_configuration (server, xml_root, logger)
         read_quotas_configuration (server, xml_root)
+        read_colors_configuration (server, xml_root)
 
         for include_element in xml_root.iter('include'):
             include    = include_element.text
 
             if include is None:
                 continue
```

### Comparing `djehuty-24.3/src/djehuty/web/validator.py` & `djehuty-24.4/src/djehuty/web/validator.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty/web/wsgi.py` & `djehuty-24.4/src/djehuty/web/wsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
 class ApiServer:
     """This class implements the HTTP interface for users."""
 
     def __init__ (self, address="127.0.0.1", port=8080):
         self.base_url         = f"http://{address}:{port}"
         self.site_name        = ""
         self.site_description = ""
+        self.site_shorttag    = ""
+        self.support_email_address = ""
         self.db               = database.SparqlInterface()  # pylint: disable=invalid-name
         self.email            = email_handler.EmailInterface()
         self.cookie_key       = "djehuty_session"
         self.impersonator_cookie_key = f"impersonator_{self.cookie_key}"
         self.allow_crawlers   = False
         self.in_production    = False
         self.in_preproduction = False
@@ -106,27 +108,36 @@
         self.datacite_password   = None
         self.datacite_prefix     = None
         self.ssi_psk             = None
         self.log_access          = self.log_access_directly
         self.log                 = logging.getLogger(__name__)
         self.locks               = locks.Locks()
         self.menu = []
+        self.colors = {
+            "primary-color":           "#f49120",
+            "primary-color-hover":     "#d26000",
+            "primary-color-active":    "#9d4800",
+            "privilege-button-color":  "#fce3bf",
+            "footer-background-color": "#707070"
+        }
         self.static_pages = {}
 
         ## Routes to all reachable pages and API calls.
         ## --------------------------------------------------------------------
 
         self.url_map = Map([
             ## ----------------------------------------------------------------
             ## UI
             ## ----------------------------------------------------------------
             R("/",                                                               self.ui_home),
             R("/portal",                                                         self.ui_redirect_to_home),
             R("/browse",                                                         self.ui_redirect_to_home),
             R("/robots.txt",                                                     self.robots_txt),
+            R("/theme/colors.css",                                               self.colors_css),
+            R("/theme/loader.svg",                                               self.loader_svg),
             R("/login",                                                          self.ui_login),
             R("/account/home",                                                   self.ui_account_home),
             R("/logout",                                                         self.ui_logout),
             R("/my/dashboard",                                                   self.ui_dashboard),
             R("/my/datasets",                                                    self.ui_my_data),
             R("/my/datasets/<dataset_id>/edit",                                  self.ui_edit_dataset),
             R("/my/datasets/<dataset_id>/delete",                                self.ui_delete_dataset),
@@ -322,43 +333,52 @@
             R("/v3/datasets/<dataset_id>/upload",                                self.api_v3_dataset_upload_file),
             R("/v3/datasets/<dataset_id>/image-files",                           self.api_v3_dataset_image_files),
             R("/v3/datasets/<dataset_id>/update-thumbnail",                      self.api_v3_datasets_update_thumbnail),
             R("/v3/datasets/<dataset_id>.git/files",                             self.api_v3_dataset_git_files),
             R("/v3/datasets/<dataset_id>.git/branches",                          self.api_v3_dataset_git_branches),
             R("/v3/datasets/<dataset_id>.git/set-default-branch",                self.api_v3_datasets_git_set_default_branch),
             R("/v3/file/<file_id>",                                              self.api_v3_file),
+            R("/v3/datasets/<container_uuid>/authors",                           self.api_v3_dataset_authors),
+            R("/v3/datasets/<container_uuid>/authors/<author_uuid>",             self.api_v3_dataset_authors),
             R("/v3/datasets/<dataset_id>/references",                            self.api_v3_dataset_references),
             R("/v3/collections/<collection_id>/references",                      self.api_v3_collection_references),
             R("/v3/datasets/<dataset_id>/tags",                                  self.api_v3_dataset_tags),
             R("/v3/collections/<collection_id>/tags",                            self.api_v3_collection_tags),
             R("/v3/groups",                                                      self.api_v3_groups),
             R("/v3/profile",                                                     self.api_v3_profile),
             R("/v3/profile/categories",                                          self.api_v3_profile_categories),
             R("/v3/profile/quota-request",                                       self.api_v3_profile_quota_request),
             R("/v3/profile/picture",                                             self.api_v3_profile_picture),
             R("/v3/profile/picture/<account_uuid>",                              self.api_v3_profile_picture_for_account),
             R("/v3/tags/search",                                                 self.api_v3_tags_search),
             R("/v3/datasets/<dataset_uuid>/collaborators",                       self.api_v3_dataset_collaborators),
             R("/v3/datasets/<dataset_uuid>/collaborators/<collaborator_uuid>",   self.api_v3_dataset_remove_collaborator),
             R("/v3/accounts/search",                                             self.api_v3_accounts_search),
+            R("/v3/authors/<author_uuid>",                                       self.api_v3_author_details),
 
             ## Data model exploratory
             ## ----------------------------------------------------------------
             R("/v3/explore/types",                                               self.api_v3_explore_types),
             R("/v3/explore/properties",                                          self.api_v3_explore_properties),
             R("/v3/explore/property_value_types",                                self.api_v3_explore_property_types),
             R("/v3/explore/clear-cache",                                         self.api_v3_explore_clear_cache),
 
             ## Reviewer
             ## ----------------------------------------------------------------
             R("/v3/datasets/<dataset_uuid>/assign-reviewer/<reviewer_uuid>",     self.api_v3_datasets_assign_reviewer),
 
+            ## Administrative
+            ## ----------------------------------------------------------------
+            R("/v3/admin/files-integrity-statistics",                            self.api_v3_admin_files_integrity_statistics),
+            R("/v3/admin/accounts/clear-cache",                                  self.api_v3_admin_accounts_clear_cache),
+
             ## ----------------------------------------------------------------
             ## GIT HTTP API
             ## ----------------------------------------------------------------
+            R("/v3/datasets/<git_uuid>.git",                                     self.api_v3_private_dataset_git_instructions),
             R("/v3/datasets/<git_uuid>.git/info/refs",                           self.api_v3_private_dataset_git_refs),
             R("/v3/datasets/<git_uuid>.git/git-upload-pack",                     self.api_v3_private_dataset_git_upload_pack),
             R("/v3/datasets/<git_uuid>.git/git-receive-pack",                    self.api_v3_private_dataset_git_receive_pack),
             R("/v3/datasets/<git_uuid>.git/languages",                           self.api_v3_dataset_git_languages),
             R("/v3/datasets/<git_uuid>.git/contributors",                        self.api_v3_dataset_git_contributors),
 
             ## ----------------------------------------------------------------
@@ -478,37 +498,43 @@
 
         return None
 
     def __render_svg_template (self, template_name, **context):
         template = self.jinja.get_template (template_name)
         return self.response (template.render (context), mimetype="image/svg+xml")
 
+    def __render_css_template (self, template_name, **context):
+        template = self.jinja.get_template (template_name)
+        return self.response (template.render (context), mimetype="text/css")
+
     def __render_template (self, request, template_name, **context):
         template      = self.jinja.get_template (template_name)
         token         = self.token_from_cookie (request)
         account       = self.db.account_by_session_token (token)
         impersonator_token = self.__impersonator_token (request)
         parameters    = {
             "base_url":        self.base_url,
             "site_name":       self.site_name,
             "site_description": self.site_description,
+            "site_shorttag":   self.site_shorttag,
             "small_footer":    self.small_footer,
             "large_footer":    self.large_footer,
             "path":            request.path,
             "in_production":   self.in_production,
             "maintenance_mode": self.maintenance_mode,
             "sandbox_message": self.sandbox_message,
             "sandbox_message_css": self.sandbox_message_css,
             "identity_provider": self.identity_provider,
             "orcid_client_id": self.orcid_client_id,
             "orcid_endpoint":  self.orcid_endpoint,
             "session_token":   self.token_from_request (request),
             "is_logged_in":    account is not None,
             "is_reviewing":    self.db.may_review (impersonator_token),
             "may_review":      self.db.may_review (token, account),
+            "may_review_integrity": self.db.may_review_integrity (token, account),
             "may_review_quotas": self.db.may_review_quotas (token, account),
             "may_administer":  self.db.may_administer (token, account),
             "may_query":       self.db.may_query (token, account),
             "may_impersonate":  self.db.may_impersonate (token, account),
             "impersonating_account": self.__impersonating_account (request),
             "menu":            self.menu,
         }
@@ -697,26 +723,23 @@
         else:
             response = self.response (json.dumps({
                 "message": "This resource is gone."
             }))
         response.status_code = 410
         return response
 
-    def error_413 (self, request, quota_available=0, quota_total=None, quota_used=None, uploading_size=None):
+    def error_413 (self, request):
         """Procedure to respond with HTTP 413."""
         response = None
-        message = "Your storage space is insufficient. Please check your storage usage and quota on the dashboard. "
-        message += f"(quota={quota_total}, used={quota_used}, available={quota_available}, your file={uploading_size})."
+        message  = "You've reached your storage quota. "
+        message += "<a href=\"/my/dashboard\">Request more storage here</a>."
         if self.accepts_json (request):
-            response = self.response (json.dumps({
-                "message": message
-            }))
+            response = self.response (json.dumps({ "message": message }))
         else:
-            response = self.response (message,
-                                      mimetype="text/plain")
+            response = self.response (message, mimetype="text/plain")
         response.status_code = 413
         return response
 
     def error_415 (self, allowed_types):
         """Procedure to respond with HTTP 415."""
         response = self.response (f"Supported Content-Types: {allowed_types}",
                                   mimetype="text/plain")
@@ -1421,14 +1444,37 @@
         if self.allow_crawlers:
             output += "Allow: /\n"
         else:
             output += "Disallow: /\n"
 
         return self.response (output, mimetype="text/plain")
 
+    def colors_css (self, request):
+        """Implements /theme/colors.css."""
+
+        if not self.accepts_content_type (request, "text/css", strict=False):
+            return self.error_406 ("text/css")
+
+        return self.__render_css_template (
+            "colors.css",
+            primary_color           = self.colors['primary-color'],
+            primary_color_hover     = self.colors['primary-color-hover'],
+            primary_color_active    = self.colors['primary-color-active'],
+            footer_background_color = self.colors['footer-background-color'],
+            privilege_button_color  = self.colors['privilege-button-color'])
+
+    def loader_svg (self, request):
+        """Implements /theme/loader.svg."""
+
+        if not self.accepts_content_type (request, "image/svg+xml", strict=False):
+            return self.error_406 ("image/svg+xml")
+
+        return self.__render_svg_template ("loader.svg",
+            primary_color = self.colors["primary-color"])
+
     def ui_maintenance (self, request):
         """Implements a maintenance page."""
         if not self.maintenance_mode:
             self.error_404 (request)
 
         if self.accepts_html (request):
             return self.__render_template (request, "maintenance.html")
@@ -2696,14 +2742,31 @@
             return self.error_403 (request)
 
         if not validator.is_valid_uuid (quota_request_uuid):
             return self.error_400 (request, "Invalid quota request UUID.",
                                    "InvalidQuotaRequestUUIError")
 
         if self.db.update_quota_request (quota_request_uuid, status = status):
+            if status == "approved":
+                try:
+                    record = self.db.quota_requests (quota_request_uuid=quota_request_uuid)[0]
+                    subject = "Quota request approved"
+                    requested_size = int(record["requested_size"] / 1000000000)
+                    self.__send_templated_email ([record["email"]],
+                                                 subject,
+                                                 "quota_approved",
+                                                 title          = subject,
+                                                 email_address  = record["email"],
+                                                 first_name     = record["first_name"],
+                                                 requested_size = requested_size,
+                                                 base_url       = self.base_url,
+                                                 support_email  = self.support_email_address)
+                except (IndexError, KeyError):
+                    self.log.error ("Unable to send e-mail for quota request %s.",
+                                    quota_request_uuid)
             return redirect ("/admin/quota-requests", code=302)
 
         return self.error_500 ()
 
     def ui_admin_approve_quota_request (self, request, quota_request_uuid):
         """Implements /admin/approve-quota-request/<id>."""
         return self.__process_quota_request (request, quota_request_uuid, "approved")
@@ -4280,23 +4343,28 @@
                                                        is_published=False)
 
                 _, error_response = self.__needs_collaborative_permissions (
                     account_uuid, request, "dataset", dataset, "metadata_read")
                 if error_response is not None:
                     return error_response
 
-                authors = self.db.authors (item_uri   = dataset["uri"],
-                                           account_uuid = account_uuid,
-                                           is_published = False,
-                                           item_type  = "dataset",
-                                           limit      = 10000)
+                authors = self.db.authors (
+                    item_uri     = dataset["uri"],
+                    account_uuid = account_uuid,
+                    is_published = False,
+                    item_type    = "dataset",
+                    limit        = validator.integer_value (request.args, "limit"),
+                    order        = validator.string_value (request.args, "order", 0, 32),
+                    order_direction = validator.order_direction (request.args, "order_direction"))
 
                 return self.default_list_response (authors, formatter.format_author_record)
-            except (IndexError, KeyError, TypeError):
-                pass
+            except (IndexError, KeyError, TypeError) as error:
+                self.log.error ("Unable to retrieve authors: %s", error)
+            except validator.ValidationException as error:
+                return self.error_400 (request, error.message, error.code)
 
             return self.error_500 ()
 
         if request.method in ('POST', 'PUT'):
             ## The 'parameters' will be a dictionary containing a key "authors",
             ## which can contain multiple dictionaries of author records.
             parameters = request.get_json()
@@ -6067,14 +6135,100 @@
                                     return_count    = record["return_count"])
         if record["return_count"]:
             return self.response (json.dumps(records[0]))
 
         return self.default_list_response (records, formatter.format_dataset_record,
                                            base_url = self.base_url)
 
+    def api_v3_dataset_authors (self, request, container_uuid, author_uuid=None):
+        """Implements /v3/datasets/<uuid>/authors[/<author_uuid>]."""
+
+        if not validator.is_valid_uuid (container_uuid):
+            return self.error_404 (request)
+
+        if author_uuid is not None and not validator.is_valid_uuid (container_uuid):
+            return self.error_404 (request)
+
+        account_uuid = self.default_authenticated_error_handling (request, "GET",
+                                                                  "application/json")
+        if isinstance (account_uuid, Response):
+            return account_uuid
+
+        try:
+            dataset = self.db.datasets (container_uuid = container_uuid,
+                                        account_uuid   = account_uuid,
+                                        is_published   = False,
+                                        is_latest      = False,
+                                        limit          = 1)[0]
+
+            _, error_response = self.__needs_collaborative_permissions (
+                account_uuid, request, "dataset", dataset, "metadata_read")
+            if error_response is not None:
+                return error_response
+
+            authors = self.db.authors (
+                item_uri     = dataset["uri"],
+                account_uuid = account_uuid,
+                author_uuid  = author_uuid,
+                is_published = False,
+                item_type    = "dataset",
+                limit        = validator.integer_value (request.args, "limit"),
+                order        = validator.string_value (request.args, "order", 0, 32),
+                order_direction = validator.order_direction (request.args, "order_direction"))
+
+            if author_uuid is not None:
+                return self.response (json.dumps(formatter.format_author_record_v3 (authors[0])))
+
+            return self.default_list_response (authors, formatter.format_author_record_v3)
+        except (IndexError, KeyError, TypeError) as error:
+            self.log.error ("Unable to retrieve authors: %s", error)
+
+        return self.error_500 ()
+
+    def api_v3_author_details (self, request, author_uuid):
+        """Implements /v3/authors/<author_uuid>."""
+
+        if not validator.is_valid_uuid (author_uuid):
+            return self.error_404 (request)
+
+        account_uuid = self.default_authenticated_error_handling (request,
+                                                                  ["GET", "PUT"],
+                                                                  "application/json")
+        if isinstance (account_uuid, Response):
+            return account_uuid
+
+        if request.method in  ("GET", "HEAD"):
+            try:
+                author = self.db.authors (author_uuid = author_uuid)[0]
+                if author is None:
+                    return self.error_404 (request)
+                return self.response (json.dumps(formatter.format_author_record_v3 (author)))
+            except IndexError:
+                return self.error_404 (request)
+
+        if request.method == "PUT":
+            record = request.get_json()
+            try:
+                parameters = {
+                    "first_name": validator.string_value (record, "first_name", 0, 255),
+                    "last_name":  validator.string_value (record, "last_name", 0, 255),
+                    "email":      validator.string_value (record, "email", 0, 255),
+                    "orcid":      validator.string_value (record, "orcid", 0, 255)
+                }
+
+                if not self.db.update_author (author_uuid, account_uuid, **parameters):
+                    return self.error_500 ()
+
+                return self.respond_204 ()
+
+            except validator.ValidationException as error:
+                return self.error_400 (request, error.message, error.code)
+
+        return self.error_405 (["GET", "PUT"])
+
     def api_v3_datasets_codemeta (self, request):
         """Implements /v3/datasets/codemeta."""
 
         try:
             errors          = []
             offset, limit   = self.__paging_offset_and_limit (request, error_list=errors)
             modified_since  = validator.string_value (request.args, "modified_since", 0, 32, False, error_list=errors)
@@ -6385,17 +6539,38 @@
                                                is_published = False)
 
         if dataset is None:
             return self.error_403 (request)
 
         container_uuid = dataset["container_uuid"]
         if self.db.decline_dataset (container_uuid, account_uuid):
-            subject = f"Dataset declined: {container_uuid}"
-            self.__send_email_to_reviewers (subject, "declined_dataset_notification",
-                                            dataset=dataset)
+            try:
+                # E-mail the datase owner.
+                account = self.db.account_by_uuid (dataset["account_uuid"])
+
+                # Retrieve the dataset again to get the DOIs.
+                dataset = self.db.datasets (dataset_uuid=dataset["uuid"],
+                                            is_published=None,
+                                            is_latest=None,
+                                            use_cache=False)[0]
+                subject = f"Declined: {dataset['title']}"
+                parameters = {
+                    "base_url": self.base_url,
+                    "support_email": self.support_email_address,
+                    "title": dataset["title"]
+                }
+                self.__send_templated_email ([account["email"]], subject,
+                                             "dataset_declined", **parameters)
+
+                self.__send_email_to_reviewers (subject, "declined_dataset_notification",
+                                                dataset=dataset, account_email = account["email"],
+                                                **parameters)
+            except (TypeError, IndexError, KeyError):
+                self.log.error ("Unable to send decline e-mail for dataset: %s.", dataset["uuid"])
+
             return self.respond_201 ({
                 "location": f"{self.base_url}/review/overview"
             })
 
         return self.error_500 ()
 
     def api_v3_dataset_publish (self, request, dataset_id):
@@ -6443,17 +6618,40 @@
                                                item_type="dataset",
                                                version=version):
                     logging.error ("Updating DOI %s for publication of %s failed.",
                                    reserved_doi, container_uuid)
                     return self.error_500 ()
 
         if self.db.publish_dataset (container_uuid, account_uuid):
-            subject = f"Dataset published: {container_uuid}"
-            self.__send_email_to_reviewers (subject, "published_dataset_notification",
-                                            dataset=dataset)
+            try:
+                # E-mail the datase owner.
+                account = self.db.account_by_uuid (dataset["account_uuid"])
+
+                # Retrieve the dataset again to get the DOIs.
+                dataset = self.db.datasets (dataset_uuid=dataset["uuid"], use_cache=False)[0]
+                subject = f"Approved: {dataset['title']}"
+                parameters = {
+                    "base_url": self.base_url,
+                    "support_email": self.support_email_address,
+                    "title": dataset["title"],
+                    "container_uuid": dataset["container_uuid"],
+                    "versioned_doi": value_or_none (dataset, "doi"),
+                    "container_doi": dataset["container_doi"]
+                }
+                self.__send_templated_email ([account["email"]], subject,
+                                             "dataset_approved", **parameters)
+
+                self.__send_email_to_reviewers (subject, "published_dataset_notification",
+                                                dataset=dataset, account_email = account["email"],
+                                                **parameters)
+
+            except (TypeError, IndexError, KeyError) as error:
+                self.log.error ("Unable to send approval e-mail for dataset %s: %s.",
+                                dataset["uuid"], error)
+
             return self.respond_201 ({
                 "location": f"{self.base_url}/review/published/{dataset_id}"
             })
 
         return self.error_500 ()
 
     def api_v3_collection_publish (self, request, collection_id):
@@ -6850,15 +7048,15 @@
         if account is None or "quota" not in account:
             self.log.error ("Account %s does not have an assigmed quota.", account_uuid)
             return self.error_403 (request)
 
         storage_used      = self.db.account_storage_used (account_uuid)
         storage_available = account["quota"] - storage_used
         if storage_available < 1:
-            return self.error_413 (request, 0)
+            return self.error_413 (request)
 
         try:
             dataset   = self.__dataset_by_id_or_uri (dataset_id,
                                                      account_uuid=account_uuid,
                                                      is_published=False)
             if dataset is None:
                 return self.error_403 (request)
@@ -6891,15 +7089,15 @@
                     "Missing Content-Length header.",
                     "MissingContentLength")
 
             # Note that the bytes_to_read contain some overhead of the
             # multipart headings (~220 bytes per chunk).
             if storage_available < bytes_to_read:
                 self.log.error ("File upload failed because user's quota limit: quota(%d), used(%d), available(%s), filesize(%d)", account["quota"], storage_used, storage_available, bytes_to_read)
-                return self.error_413 (request, storage_available, account["quota"], storage_used, bytes_to_read)
+                return self.error_413 (request)
 
             input_stream = request.stream
 
             # Read the boundary, plus '--', plus CR/LF.
             read_ahead_bytes = len(boundary) + 4
             boundary_scan  = input_stream.read (read_ahead_bytes)
             expected_begin = f"--{boundary}\r\n".encode("utf-8")
@@ -7341,14 +7539,66 @@
                 order_direction = validator.order_direction (request.args, "order_direction"))
 
             return self.default_list_response (records, formatter.format_group_record)
 
         except validator.ValidationException as error:
             return self.error_400 (request, error.message, error.code)
 
+    def api_v3_admin_files_integrity_statistics (self, request):
+        """Implements /v3/admin/files-integrity-statistics."""
+
+        if not self.accepts_json (request):
+            return self.error_406 ("application/json")
+
+        token = self.token_from_cookie (request)
+        if not self.db.may_review_integrity (token):
+            return self.error_403 (request)
+
+        files = self.db.repository_file_statistics (extended_properties=True)
+        number_of_files = 0
+        number_of_inaccessible_files = 0
+        number_of_incomplete_metadata = 0
+        number_of_bytes = 0
+        number_of_links = 0
+        incomplete_metadata = []
+        missing_files = []
+
+        for entry in files:
+            if value_or (entry, "is_link_only", False):
+                number_of_links += 1
+                continue
+
+            number_of_files += 1
+            number_of_bytes += int(float(entry["bytes"]))
+
+            filesystem_location = self.__filesystem_location (entry)
+            if not filesystem_location:
+                number_of_incomplete_metadata += 1
+                incomplete_metadata.append (value_or (entry, "uuid", "unknown"))
+                continue
+
+            if not os.path.isfile (filesystem_location):
+                number_of_inaccessible_files += 1
+                missing_files.append (filesystem_location)
+
+        output = {
+            "number_of_links":              number_of_links,
+            "number_of_files":              number_of_files,
+            "number_of_bytes":              number_of_bytes,
+            "number_of_accessible_files":   number_of_files - number_of_inaccessible_files,
+            "number_of_inaccessible_files": number_of_inaccessible_files,
+            "number_of_incomplete_metadata": number_of_incomplete_metadata,
+            "percentage_accessible":        (1.0 - (number_of_inaccessible_files / number_of_files)) * 100,
+            "percentage_inaccessible":      number_of_inaccessible_files / number_of_files * 100,
+            "inaccessible_files":           missing_files,
+            "incomplete_metadata":          incomplete_metadata,
+        }
+
+        return self.response (json.dumps(output))
+
     def __git_create_repository (self, git_uuid):
         git_directory = f"{self.db.storage}/{git_uuid}.git"
         if not os.path.exists (git_directory):
             initial_repository = pygit2.init_repository (git_directory, True)
             if initial_repository:
                 try:
                     with open (f"{git_directory}/config", "a",
@@ -7428,14 +7678,37 @@
             return output
 
         except subprocess.CalledProcessError as error:
             self.log.error ("Proxying to Git failed with exit code %d", error.returncode)
             self.log.error ("The command was:\n---\n%s\n---", error.cmd)
             return self.error_500()
 
+    def api_v3_private_dataset_git_instructions (self, request, git_uuid):
+        """Implements an instruction page for /v3/datasets/<id>.git."""
+        handler = self.default_error_handling (request, "GET", "text/html")
+        if handler is not None:
+            return handler
+
+        if not validator.is_valid_uuid (git_uuid):
+            return self.error_404 (request)
+
+        try:
+            # Only consider published datasets to not reveal whether a UUID
+            # is reserved for a Git repository.
+            dataset = self.db.datasets (git_uuid     = git_uuid,
+                                        is_published = True,
+                                        is_latest    = None)[0]
+            git_repository_url = self.__git_repository_url_for_dataset (dataset)
+            return self.__render_template (request, "git_instructions.html",
+                                           git_repository_url = git_repository_url)
+        except IndexError:
+            pass
+
+        return self.error_404 (request)
+
     def api_v3_private_dataset_git_refs (self, request, git_uuid):
         """Implements /v3/datasets/<id>.git/<suffix>."""
 
         service = validator.string_value (request.args, "service", 0, 16)
         self.__git_create_repository (git_uuid)
 
         ## Used for clone and pull.
@@ -7608,18 +7881,25 @@
 
         # Drop the binary count from the statistics, because we only
         # generate a summary with line counts below.
         statistics.pop("binary", None)
 
         summary = {}
         for _, extension in enumerate (statistics):
-            lines = 0
+            num_bytes_for_extension = 0
             for entry in statistics[extension]:
-                lines += value_or (entry, "lines", 0)
-            summary[extension] = lines
+                num_lines = value_or (entry, "lines", 0)
+                num_bytes = value_or (entry, "size", 0)
+                # Remove minified sources by the heuristic that the average
+                # line length must be smaller than 300 bytes long.  This seems
+                # to come close to how Github reports the statistics.
+                if num_lines > 0 and num_bytes / num_lines < 300:
+                    num_bytes_for_extension += num_bytes
+
+            summary[extension] = num_bytes_for_extension
 
         sorted_summary = dict(sorted(summary.items(),
                                      key=lambda item: item[1],
                                      reverse=True))
         return self.response (json.dumps (sorted_summary))
 
     def api_v3_dataset_git_contributors (self, request, git_uuid):
@@ -7820,14 +8100,30 @@
         self.log.info ("Invalidating explorer caches.")
         self.db.cache.invalidate_by_prefix ("explorer_properties")
         self.db.cache.invalidate_by_prefix ("explorer_types")
         self.db.cache.invalidate_by_prefix ("explorer_property_types")
 
         return self.respond_204 ()
 
+    def api_v3_admin_accounts_clear_cache (self, request):
+        """Implements /v3/admin/accounts/clear-cache."""
+
+        handler = self.default_error_handling (request, "GET", "application/json")
+        if handler is not None:
+            return handler
+
+        token = self.token_from_cookie (request)
+        if not self.db.may_administer (token):
+            return self.error_403 (request)
+
+        self.log.info ("Invalidating accounts caches.")
+        self.db.cache.invalidate_by_prefix ("accounts")
+
+        return self.respond_204 ()
+
     def api_v3_datasets_assign_reviewer (self, request, dataset_uuid, reviewer_uuid):
         """Implements /v3/datasets/<id>/assign-reviewer/<rid>."""
 
         if request.method != "PUT":
             return self.error_405 ("PUT")
 
         account_uuid = self.account_uuid_from_request (request)
@@ -7889,15 +8185,16 @@
         return self.respond_201 ({ "message": "The MD5 sums have been regenerated."})
 
     def api_v3_doi_badge (self, request, dataset_id, version=None):
         """Implements /v3/datasets/<id>/doi-badge-v<version>.svg."""
         try:
             dataset = self.__dataset_by_id_or_uri (dataset_id, version=version)
             doi = dataset["container_doi"] if version is None else dataset["doi"]
-            return self.__render_svg_template ("badge.svg", doi=doi, version=version)
+            return self.__render_svg_template ("badge.svg", doi=doi, version=version,
+                                               color=self.colors["primary-color"])
         except KeyError:
             pass
 
         return self.error_404 (request)
 
     def api_v3_receive_from_ssi (self, request):
         """Implements /v3/receive-from-ssi."""
```

### Comparing `djehuty-24.3/src/djehuty/web/xml_formatter.py` & `djehuty-24.4/src/djehuty/web/xml_formatter.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.3/src/djehuty.egg-info/PKG-INFO` & `djehuty-24.4/src/djehuty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djehuty
-Version: 24.3
+Version: 24.4
 Summary: The 4TU.ResearchData repository system
 Author-email: Roel Janssen <r.r.e.janssen@tudelft.nl>
 Project-URL: Homepage, https://data.4tu.nl
 Project-URL: Source Code, https://github.com/4TUResearchData/djehuty
 Project-URL: Bug Tracker, https://github.com/4TUResearchData/djehuty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `djehuty-24.3/src/djehuty.egg-info/SOURCES.txt` & `djehuty-24.4/src/djehuty.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,19 +56,22 @@
 src/djehuty/web/resources/html_templates/410.html
 src/djehuty/web/resources/html_templates/activate_2fa_session.html
 src/djehuty/web/resources/html_templates/author.html
 src/djehuty/web/resources/html_templates/badge.svg
 src/djehuty/web/resources/html_templates/categories.html
 src/djehuty/web/resources/html_templates/category.html
 src/djehuty/web/resources/html_templates/collection.html
+src/djehuty/web/resources/html_templates/colors.css
 src/djehuty/web/resources/html_templates/dataset.html
 src/djehuty/web/resources/html_templates/dataset_access_request.html
 src/djehuty/web/resources/html_templates/feedback.html
+src/djehuty/web/resources/html_templates/git_instructions.html
 src/djehuty/web/resources/html_templates/institutions.html
 src/djehuty/web/resources/html_templates/layout.html
+src/djehuty/web/resources/html_templates/loader.svg
 src/djehuty/web/resources/html_templates/maintenance.html
 src/djehuty/web/resources/html_templates/opendap_to_doi.html
 src/djehuty/web/resources/html_templates/portal.html
 src/djehuty/web/resources/html_templates/private_link_is_expired.html
 src/djehuty/web/resources/html_templates/public_metadata.html
 src/djehuty/web/resources/html_templates/search.html
 src/djehuty/web/resources/html_templates/admin/dashboard.html
@@ -93,23 +96,29 @@
 src/djehuty/web/resources/html_templates/depositor/profile.html
 src/djehuty/web/resources/html_templates/depositor/published-collection.html
 src/djehuty/web/resources/html_templates/depositor/submitted-for-review.html
 src/djehuty/web/resources/html_templates/email/2fa_token.html
 src/djehuty/web/resources/html_templates/email/2fa_token.txt
 src/djehuty/web/resources/html_templates/email/data_access_request.html
 src/djehuty/web/resources/html_templates/email/data_access_request.txt
+src/djehuty/web/resources/html_templates/email/dataset_approved.html
+src/djehuty/web/resources/html_templates/email/dataset_approved.txt
+src/djehuty/web/resources/html_templates/email/dataset_declined.html
+src/djehuty/web/resources/html_templates/email/dataset_declined.txt
 src/djehuty/web/resources/html_templates/email/dataset_submitted.html
 src/djehuty/web/resources/html_templates/email/dataset_submitted.txt
 src/djehuty/web/resources/html_templates/email/declined_dataset_notification.html
 src/djehuty/web/resources/html_templates/email/declined_dataset_notification.txt
 src/djehuty/web/resources/html_templates/email/feedback.html
 src/djehuty/web/resources/html_templates/email/feedback.txt
 src/djehuty/web/resources/html_templates/email/layout.html
 src/djehuty/web/resources/html_templates/email/published_dataset_notification.html
 src/djehuty/web/resources/html_templates/email/published_dataset_notification.txt
+src/djehuty/web/resources/html_templates/email/quota_approved.html
+src/djehuty/web/resources/html_templates/email/quota_approved.txt
 src/djehuty/web/resources/html_templates/email/quota_request.html
 src/djehuty/web/resources/html_templates/email/quota_request.txt
 src/djehuty/web/resources/html_templates/email/submitted_for_review_notification.html
 src/djehuty/web/resources/html_templates/email/submitted_for_review_notification.txt
 src/djehuty/web/resources/html_templates/review/overview.html
 src/djehuty/web/resources/html_templates/review/published.html
 src/djehuty/web/resources/sparql_templates/account_by_email.sparql
@@ -189,14 +198,15 @@
 src/djehuty/web/resources/sparql_templates/statistics_authors.sparql
 src/djehuty/web/resources/sparql_templates/statistics_collections.sparql
 src/djehuty/web/resources/sparql_templates/statistics_datasets.sparql
 src/djehuty/web/resources/sparql_templates/statistics_files.sparql
 src/djehuty/web/resources/sparql_templates/subcategories_by_category.sparql
 src/djehuty/web/resources/sparql_templates/tags.sparql
 src/djehuty/web/resources/sparql_templates/update_account.sparql
+src/djehuty/web/resources/sparql_templates/update_author.sparql
 src/djehuty/web/resources/sparql_templates/update_collection.sparql
 src/djehuty/web/resources/sparql_templates/update_dataset.sparql
 src/djehuty/web/resources/sparql_templates/update_dataset_thumb.sparql
 src/djehuty/web/resources/sparql_templates/update_doi_after_publishing.sparql
 src/djehuty/web/resources/sparql_templates/update_file.sparql
 src/djehuty/web/resources/sparql_templates/update_git_uuid.sparql
 src/djehuty/web/resources/sparql_templates/update_orcid_for_account.sparql
@@ -225,15 +235,14 @@
 src/djehuty/web/resources/static/fonts/fa-solid-900.woff2
 src/djehuty/web/resources/static/images/CoreTrustSeal.png
 src/djehuty/web/resources/static/images/collection-thumb.svg
 src/djehuty/web/resources/static/images/dataset-thumb.svg
 src/djehuty/web/resources/static/images/ext-link.png
 src/djehuty/web/resources/static/images/favicon.ico
 src/djehuty/web/resources/static/images/favicon.png
-src/djehuty/web/resources/static/images/loader.svg
 src/djehuty/web/resources/static/images/logo-delft.png
 src/djehuty/web/resources/static/images/logo-eindhoven.png
 src/djehuty/web/resources/static/images/logo-gray.svg
 src/djehuty/web/resources/static/images/logo-other.png
 src/djehuty/web/resources/static/images/logo-twente.png
 src/djehuty/web/resources/static/images/logo-wageningen.png
 src/djehuty/web/resources/static/images/logo.png
```

