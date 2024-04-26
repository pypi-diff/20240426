# Comparing `tmp/django_bocor_ds-2.1.0.tar.gz` & `tmp/django_bocor_ds-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_bocor_ds-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_bocor_ds-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_bocor_ds-2.1.0.tar` & `django_bocor_ds-2.2.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0     8196 2024-04-13 00:01:41.783512 django_bocor_ds-2.1.0/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-21 05:49:50.372491 django_bocor_ds-2.1.0/.gitattributes
--rw-r--r--   0        0        0        7 2024-03-29 05:46:41.713784 django_bocor_ds-2.1.0/.gitignore
--rw-r--r--   0        0        0       52 2024-03-21 06:06:29.551428 django_bocor_ds-2.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      405 2024-03-21 06:06:29.465715 django_bocor_ds-2.1.0/.idea/django-bocor-ds.iml
--rw-r--r--   0        0        0      174 2024-03-21 06:06:29.480874 django_bocor_ds-2.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      421 2024-03-21 06:08:26.611158 django_bocor_ds-2.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      282 2024-03-21 06:06:29.471790 django_bocor_ds-2.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-03-21 06:06:29.484071 django_bocor_ds-2.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_bocor_ds-2.1.0/LICENSE
--rw-r--r--   0        0        0     1760 2024-04-26 06:35:37.368209 django_bocor_ds-2.1.0/README.md
--rw-r--r--   0        0        0     6148 2024-04-13 00:02:19.172196 django_bocor_ds-2.1.0/django_bocor_ds/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-21 06:07:02.999245 django_bocor_ds-2.1.0/django_bocor_ds/__init__.py
--rw-r--r--   0        0        0      495 2024-03-26 07:24:10.511682 django_bocor_ds-2.1.0/django_bocor_ds/admin.py
--rw-r--r--   0        0        0      160 2024-03-21 06:07:03.001129 django_bocor_ds-2.1.0/django_bocor_ds/apps.py
--rw-r--r--   0        0        0      947 2024-03-24 12:14:35.423434 django_bocor_ds-2.1.0/django_bocor_ds/forms.py
--rw-r--r--   0        0        0     1915 2024-03-26 07:22:15.008801 django_bocor_ds-2.1.0/django_bocor_ds/migrations/0001_initial.py
--rw-r--r--   0        0        0      540 2024-03-26 08:05:25.492109 django_bocor_ds-2.1.0/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py
--rw-r--r--   0        0        0      502 2024-03-27 02:55:50.933146 django_bocor_ds-2.1.0/django_bocor_ds/migrations/0003_portfolio_redirect_link.py
--rw-r--r--   0        0        0      351 2024-03-27 05:19:19.375307 django_bocor_ds-2.1.0/django_bocor_ds/migrations/0004_remove_portfolio_redirect_link.py
--rw-r--r--   0        0        0        0 2024-03-21 06:07:03.001526 django_bocor_ds-2.1.0/django_bocor_ds/migrations/__init__.py
--rw-r--r--   0        0        0      948 2024-03-27 05:06:04.714022 django_bocor_ds-2.1.0/django_bocor_ds/models.py
--rw-r--r--   0        0        0     6148 2024-03-21 08:10:33.959729 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/.DS_Store
--rwxr-xr-x   0        0        0    24429 2024-04-03 08:25:58.403114 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/css/style.css
--rwxr-xr-x   0        0        0   249630 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/img/footer-bg.jpg
--rwxr-xr-x   0        0        0     5114 2024-03-17 05:37:08.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/js/main.js
--rwxr-xr-x   0        0        0     2893 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_footer.scss
--rwxr-xr-x   0        0        0     1290 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_general.scss
--rwxr-xr-x   0        0        0      709 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_header.scss
--rwxr-xr-x   0        0        0     1422 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_hero.scss
--rwxr-xr-x   0        0        0     4101 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_nav.scss
--rwxr-xr-x   0        0        0    15555 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_sections.scss
--rwxr-xr-x   0        0        0      454 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_variables.scss
--rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/style.scss
--rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js
--rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/aos/aos.css
--rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js
--rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/aos/aos.js
--rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/aos/aos.js.map
--rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css
--rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map
--rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css
--rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css
--rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css
--rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css
--rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot
--rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg
--rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf
--rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff
--rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2
--rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css
--rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css
--rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css
--rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css
--rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js
--rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js
--rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js
--rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js
--rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php
--rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js
--rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css
--rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js
--rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map
--rw-r--r--   0        0        0     6148 2024-04-03 00:07:46.476654 django_bocor_ds-2.1.0/django_bocor_ds/templates/.DS_Store
--rwxr-xr-x   0        0        0     6381 2024-03-17 05:37:08.000000 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/__inner-page.html
--rw-r--r--   0        0        0     8057 2024-03-26 07:30:05.640370 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/__portfolio-details.html
--rw-r--r--   0        0        0     1241 2024-04-26 06:23:47.737266 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_about.html
--rw-r--r--   0        0        0      735 2024-03-25 05:29:33.069856 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_clients.html
--rw-r--r--   0        0        0     2606 2024-04-26 06:35:37.365523 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_contact.html
--rw-r--r--   0        0        0      794 2024-04-26 06:35:37.358645 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_faq.html
--rw-r--r--   0        0        0     1441 2024-04-26 06:22:56.117396 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_features.html
--rw-r--r--   0        0        0      626 2024-04-26 06:25:22.029168 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_hero.html
--rw-r--r--   0        0        0     1553 2024-04-26 06:25:22.020526 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_portfolio.html
--rw-r--r--   0        0        0     1185 2024-04-26 06:35:37.370423 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_pricing.html
--rw-r--r--   0        0        0     1156 2024-04-26 06:25:22.026522 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_services.html
--rw-r--r--   0        0        0     1653 2024-04-26 06:35:37.354165 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_team.html
--rw-r--r--   0        0        0     2404 2024-04-04 04:41:10.261572 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/footer.html
--rw-r--r--   0        0        0     1452 2024-04-21 07:23:02.021277 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/header.html
--rw-r--r--   0        0        0     3561 2024-03-26 06:02:21.891761 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/index.html
--rw-r--r--   0        0        0     1914 2024-04-03 08:20:59.077335 django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/seo.html
--rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_bocor_ds-2.1.0/django_bocor_ds/templatetags/__init__.py
--rw-r--r--   0        0        0     5223 2024-03-22 23:51:55.383813 django_bocor_ds-2.1.0/django_bocor_ds/templatetags/bocords_tags.py
--rw-r--r--   0        0        0       60 2024-03-21 06:07:03.001392 django_bocor_ds-2.1.0/django_bocor_ds/tests.py
--rw-r--r--   0        0        0      265 2024-03-27 05:05:51.517275 django_bocor_ds-2.1.0/django_bocor_ds/urls.py
--rw-r--r--   0        0        0     2469 2024-04-03 06:57:03.342404 django_bocor_ds-2.1.0/django_bocor_ds/views.py
--rw-r--r--   0        0        0      784 2024-04-26 06:35:37.362605 django_bocor_ds-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 django_bocor_ds-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     8196 2024-04-13 00:01:41.783512 django_bocor_ds-2.2.0/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-21 05:49:50.372491 django_bocor_ds-2.2.0/.gitattributes
+-rw-r--r--   0        0        0        7 2024-03-29 05:46:41.713784 django_bocor_ds-2.2.0/.gitignore
+-rw-r--r--   0        0        0       52 2024-03-21 06:06:29.551428 django_bocor_ds-2.2.0/.idea/.gitignore
+-rw-r--r--   0        0        0      405 2024-03-21 06:06:29.465715 django_bocor_ds-2.2.0/.idea/django-bocor-ds.iml
+-rw-r--r--   0        0        0      174 2024-03-21 06:06:29.480874 django_bocor_ds-2.2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      421 2024-03-21 06:08:26.611158 django_bocor_ds-2.2.0/.idea/misc.xml
+-rw-r--r--   0        0        0      282 2024-03-21 06:06:29.471790 django_bocor_ds-2.2.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-21 06:06:29.484071 django_bocor_ds-2.2.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_bocor_ds-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1760 2024-04-26 06:35:37.368209 django_bocor_ds-2.2.0/README.md
+-rw-r--r--   0        0        0     6148 2024-04-13 00:02:19.172196 django_bocor_ds-2.2.0/django_bocor_ds/.DS_Store
+-rw-r--r--   0        0        0        0 2024-03-21 06:07:02.999245 django_bocor_ds-2.2.0/django_bocor_ds/__init__.py
+-rw-r--r--   0        0        0      495 2024-03-26 07:24:10.511682 django_bocor_ds-2.2.0/django_bocor_ds/admin.py
+-rw-r--r--   0        0        0      160 2024-03-21 06:07:03.001129 django_bocor_ds-2.2.0/django_bocor_ds/apps.py
+-rw-r--r--   0        0        0      947 2024-03-24 12:14:35.423434 django_bocor_ds-2.2.0/django_bocor_ds/forms.py
+-rw-r--r--   0        0        0     1915 2024-03-26 07:22:15.008801 django_bocor_ds-2.2.0/django_bocor_ds/migrations/0001_initial.py
+-rw-r--r--   0        0        0      540 2024-03-26 08:05:25.492109 django_bocor_ds-2.2.0/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py
+-rw-r--r--   0        0        0      502 2024-03-27 02:55:50.933146 django_bocor_ds-2.2.0/django_bocor_ds/migrations/0003_portfolio_redirect_link.py
+-rw-r--r--   0        0        0      351 2024-03-27 05:19:19.375307 django_bocor_ds-2.2.0/django_bocor_ds/migrations/0004_remove_portfolio_redirect_link.py
+-rw-r--r--   0        0        0        0 2024-03-21 06:07:03.001526 django_bocor_ds-2.2.0/django_bocor_ds/migrations/__init__.py
+-rw-r--r--   0        0        0      948 2024-03-27 05:06:04.714022 django_bocor_ds-2.2.0/django_bocor_ds/models.py
+-rw-r--r--   0        0        0     6148 2024-03-21 08:10:33.959729 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/.DS_Store
+-rwxr-xr-x   0        0        0    24429 2024-04-03 08:25:58.403114 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/css/style.css
+-rwxr-xr-x   0        0        0   249630 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/img/footer-bg.jpg
+-rwxr-xr-x   0        0        0     5114 2024-03-17 05:37:08.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/js/main.js
+-rwxr-xr-x   0        0        0     2893 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_footer.scss
+-rwxr-xr-x   0        0        0     1290 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_general.scss
+-rwxr-xr-x   0        0        0      709 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_header.scss
+-rwxr-xr-x   0        0        0     1422 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_hero.scss
+-rwxr-xr-x   0        0        0     4101 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_nav.scss
+-rwxr-xr-x   0        0        0    15555 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_sections.scss
+-rwxr-xr-x   0        0        0      454 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_variables.scss
+-rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/style.scss
+-rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js
+-rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/aos/aos.css
+-rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js
+-rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/aos/aos.js
+-rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/aos/aos.js.map
+-rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css
+-rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css
+-rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css
+-rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css
+-rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css
+-rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot
+-rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg
+-rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf
+-rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff
+-rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2
+-rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css
+-rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css
+-rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css
+-rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css
+-rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js
+-rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js
+-rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js
+-rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js
+-rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php
+-rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js
+-rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css
+-rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js
+-rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map
+-rw-r--r--   0        0        0     6148 2024-04-03 00:07:46.476654 django_bocor_ds-2.2.0/django_bocor_ds/templates/.DS_Store
+-rwxr-xr-x   0        0        0     6381 2024-03-17 05:37:08.000000 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/__inner-page.html
+-rw-r--r--   0        0        0     8057 2024-03-26 07:30:05.640370 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/__portfolio-details.html
+-rw-r--r--   0        0        0     1241 2024-04-26 06:23:47.737266 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_about.html
+-rw-r--r--   0        0        0      735 2024-03-25 05:29:33.069856 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_clients.html
+-rw-r--r--   0        0        0     3506 2024-04-26 08:21:58.255733 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_contact.html
+-rw-r--r--   0        0        0      794 2024-04-26 06:35:37.358645 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_faq.html
+-rw-r--r--   0        0        0     1441 2024-04-26 06:22:56.117396 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_features.html
+-rw-r--r--   0        0        0      626 2024-04-26 06:25:22.029168 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_hero.html
+-rw-r--r--   0        0        0     1553 2024-04-26 06:25:22.020526 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_portfolio.html
+-rw-r--r--   0        0        0     1185 2024-04-26 06:35:37.370423 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_pricing.html
+-rw-r--r--   0        0        0     1156 2024-04-26 06:25:22.026522 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_services.html
+-rw-r--r--   0        0        0     1653 2024-04-26 06:35:37.354165 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_team.html
+-rw-r--r--   0        0        0     2404 2024-04-04 04:41:10.261572 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/footer.html
+-rw-r--r--   0        0        0     1452 2024-04-21 07:23:02.021277 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/header.html
+-rw-r--r--   0        0        0     3561 2024-03-26 06:02:21.891761 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/index.html
+-rw-r--r--   0        0        0     1914 2024-04-03 08:20:59.077335 django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/seo.html
+-rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_bocor_ds-2.2.0/django_bocor_ds/templatetags/__init__.py
+-rw-r--r--   0        0        0     5223 2024-03-22 23:51:55.383813 django_bocor_ds-2.2.0/django_bocor_ds/templatetags/bocords_tags.py
+-rw-r--r--   0        0        0       60 2024-03-21 06:07:03.001392 django_bocor_ds-2.2.0/django_bocor_ds/tests.py
+-rw-r--r--   0        0        0      265 2024-03-27 05:05:51.517275 django_bocor_ds-2.2.0/django_bocor_ds/urls.py
+-rw-r--r--   0        0        0     2469 2024-04-03 06:57:03.342404 django_bocor_ds-2.2.0/django_bocor_ds/views.py
+-rw-r--r--   0        0        0      784 2024-04-26 08:22:51.125372 django_bocor_ds-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 django_bocor_ds-2.2.0/PKG-INFO
```

### Comparing `django_bocor_ds-2.1.0/.DS_Store` & `django_bocor_ds-2.2.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/LICENSE` & `django_bocor_ds-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/README.md` & `django_bocor_ds-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/.DS_Store` & `django_bocor_ds-2.2.0/django_bocor_ds/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/forms.py` & `django_bocor_ds-2.2.0/django_bocor_ds/forms.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/migrations/0001_initial.py` & `django_bocor_ds-2.2.0/django_bocor_ds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py` & `django_bocor_ds-2.2.0/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/models.py` & `django_bocor_ds-2.2.0/django_bocor_ds/models.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/.DS_Store` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/css/style.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/css/style.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/img/footer-bg.jpg` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/img/footer-bg.jpg`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/js/main.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/js/main.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_footer.scss` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_general.scss` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_header.scss` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_hero.scss` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_hero.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_nav.scss` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/scss/_sections.scss` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/scss/_sections.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/aos/aos.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/aos/aos.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/aos/aos.js.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/aos/aos.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map` & `django_bocor_ds-2.2.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/.DS_Store` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/__inner-page.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/__inner-page.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/__portfolio-details.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/__portfolio-details.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_about.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_about.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_clients.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_clients.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_contact.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_contact.html`

 * *Files 24% similar despite different names*

```diff
@@ -22,142 +22,199 @@
 00000150: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
 00000160: 6c61 7373 3d22 636f 6c2d 6d64 2d31 3222  lass="col-md-12"
 00000170: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
 00000180: 2020 3c64 6976 2063 6c61 7373 3d22 696e    <div class="in
 00000190: 666f 2d62 6f78 2220 6461 7461 2d61 6f73  fo-box" data-aos
 000001a0: 3d22 6661 6465 2d75 7022 3e0a 2020 2020  ="fade-up">.    
 000001b0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-000001c0: 2063 6c61 7373 3d22 6278 2062 782d 6d61   class="bx bx-ma
-000001d0: 7022 3e3c 2f69 3e0a 2020 2020 2020 2020  p"></i>.        
-000001e0: 2020 2020 2020 2020 2020 3c68 333e 7b7b            <h3>{{
-000001f0: 2063 6f6e 7461 6374 2e69 6e66 6f31 2e30   contact.info1.0
-00000200: 207d 7d3c 2f68 333e 0a20 2020 2020 2020   }}</h3>.       
-00000210: 2020 2020 2020 2020 2020 203c 703e 7b7b             <p>{{
-00000220: 2063 6f6e 7461 6374 2e69 6e66 6f31 2e31   contact.info1.1
-00000230: 207c 2073 6166 6520 7d7d 3c2f 703e 0a20   | safe }}</p>. 
-00000240: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000250: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00000260: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00000270: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00000280: 6173 733d 2263 6f6c 2d6d 642d 3622 3e0a  ass="col-md-6">.
-00000290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002a0: 3c64 6976 2063 6c61 7373 3d22 696e 666f  <div class="info
-000002b0: 2d62 6f78 206d 742d 3422 2064 6174 612d  -box mt-4" data-
-000002c0: 616f 733d 2266 6164 652d 7570 2220 6461  aos="fade-up" da
-000002d0: 7461 2d61 6f73 2d64 656c 6179 3d22 3130  ta-aos-delay="10
-000002e0: 3022 3e0a 2020 2020 2020 2020 2020 2020  0">.            
-000002f0: 2020 2020 2020 3c69 2063 6c61 7373 3d22        <i class="
-00000300: 6278 2062 782d 656e 7665 6c6f 7065 223e  bx bx-envelope">
-00000310: 3c2f 693e 0a20 2020 2020 2020 2020 2020  </i>.           
-00000320: 2020 2020 2020 203c 6833 3e7b 7b20 636f         <h3>{{ co
-00000330: 6e74 6163 742e 696e 666f 322e 3020 7d7d  ntact.info2.0 }}
-00000340: 3c2f 6833 3e0a 2020 2020 2020 2020 2020  </h3>.          
-00000350: 2020 2020 2020 2020 3c70 3e7b 7b20 636f          <p>{{ co
-00000360: 6e74 6163 742e 696e 666f 322e 3120 7c20  ntact.info2.1 | 
-00000370: 7361 6665 207d 7d3c 2f70 3e0a 2020 2020  safe }}</p>.    
-00000380: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00000390: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-000003a0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-000003b0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000003c0: 3d22 636f 6c2d 6d64 2d36 223e 0a20 2020  ="col-md-6">.   
-000003d0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-000003e0: 7620 636c 6173 733d 2269 6e66 6f2d 626f  v class="info-bo
-000003f0: 7820 6d74 2d34 2220 6461 7461 2d61 6f73  x mt-4" data-aos
-00000400: 3d22 6661 6465 2d75 7022 2064 6174 612d  ="fade-up" data-
-00000410: 616f 732d 6465 6c61 793d 2231 3030 223e  aos-delay="100">
-00000420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000430: 2020 203c 6920 636c 6173 733d 2262 7820     <i class="bx 
-00000440: 6278 2d70 686f 6e65 2d63 616c 6c22 3e3c  bx-phone-call"><
-00000450: 2f69 3e0a 2020 2020 2020 2020 2020 2020  /i>.            
-00000460: 2020 2020 2020 3c68 333e 7b7b 2063 6f6e        <h3>{{ con
-00000470: 7461 6374 2e69 6e66 6f33 2e30 207d 7d3c  tact.info3.0 }}<
-00000480: 2f68 333e 0a20 2020 2020 2020 2020 2020  /h3>.           
-00000490: 2020 2020 2020 203c 703e 7b7b 2063 6f6e         <p>{{ con
-000004a0: 7461 6374 2e69 6e66 6f33 2e31 207c 2073  tact.info3.1 | s
-000004b0: 6166 6520 7d7d 3c2f 703e 0a20 2020 2020  afe }}</p>.     
-000004c0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-000004d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000004e0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-000004f0: 2020 203c 2f64 6976 3e0a 0a20 2020 2020     </div>..     
-00000500: 2020 2020 203c 2f64 6976 3e0a 0a20 2020       </div>..   
-00000510: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00000520: 733d 2263 6f6c 2d6c 672d 3620 6d74 2d34  s="col-lg-6 mt-4
-00000530: 206d 742d 6c67 2d30 223e 0a20 2020 2020   mt-lg-0">.     
-00000540: 2020 2020 2020 203c 212d 2d20 7572 6c20         <!-- url 
-00000550: ed83 9cea b7b8 20ec 9588 ec97 9020 ec95  ...... ...... ..
-00000560: b5ec bba4 20ec 9db4 eb8f 9920 eab0 80eb  .... ...... ....
-00000570: 8aa5 ed95 98eb 8ba4 202d 2d3e 0a20 2020  ........ -->.   
-00000580: 2020 2020 2020 2020 203c 666f 726d 2061           <form a
-00000590: 6374 696f 6e3d 227b 2520 7572 6c20 2762  ction="{% url 'b
-000005a0: 6f63 6f72 6473 3a68 6f6d 6527 2025 7d23  ocords:home' %}#
-000005b0: 636f 6e74 6163 7422 206d 6574 686f 643d  contact" method=
-000005c0: 2250 4f53 5422 2072 6f6c 653d 2266 6f72  "POST" role="for
-000005d0: 6d22 2063 6c61 7373 3d22 7068 702d 656d  m" class="php-em
-000005e0: 6169 6c2d 666f 726d 2020 772d 3130 3022  ail-form  w-100"
-000005f0: 2064 6174 612d 616f 733d 2266 6164 652d   data-aos="fade-
-00000600: 7570 223e 0a20 2020 2020 2020 2020 2020  up">.           
-00000610: 2020 207b 2520 6373 7266 5f74 6f6b 656e     {% csrf_token
-00000620: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000630: 2020 3c64 6976 2063 6c61 7373 3d22 726f    <div class="ro
-00000640: 7722 3e0a 2020 2020 2020 2020 2020 2020  w">.            
-00000650: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00000660: 636f 6c2d 6d64 2d36 2066 6f72 6d2d 6772  col-md-6 form-gr
-00000670: 6f75 7022 3e0a 2020 2020 2020 2020 2020  oup">.          
-00000680: 2020 2020 2020 2020 7b7b 2066 6f72 6d2e          {{ form.
-00000690: 6e61 6d65 207d 7d0a 2020 2020 2020 2020  name }}.        
-000006a0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-000006b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000006c0: 6469 7620 636c 6173 733d 2263 6f6c 2d6d  div class="col-m
-000006d0: 642d 3620 666f 726d 2d67 726f 7570 206d  d-6 form-group m
-000006e0: 742d 3320 6d74 2d6d 642d 3022 3e0a 2020  t-3 mt-md-0">.  
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000700: 7b7b 2066 6f72 6d2e 656d 6169 6c20 7d7d  {{ form.email }}
-00000710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000720: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00000730: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00000740: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00000750: 636c 6173 733d 2266 6f72 6d2d 6772 6f75  class="form-grou
-00000760: 7020 6d74 2d33 223e 0a20 2020 2020 2020  p mt-3">.       
-00000770: 2020 2020 2020 2020 207b 7b20 666f 726d           {{ form
-00000780: 2e63 6f6d 7061 6e79 207d 7d0a 2020 2020  .company }}.    
-00000790: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-000007a0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-000007b0: 6469 7620 636c 6173 733d 2266 6f72 6d2d  div class="form-
-000007c0: 6772 6f75 7020 6d74 2d33 223e 0a20 2020  group mt-3">.   
-000007d0: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
-000007e0: 666f 726d 2e6d 6573 7361 6765 207d 7d0a  form.message }}.
-000007f0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00000800: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00000810: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
-00000820: 792d 3322 3e0a 2020 2020 2020 2020 2020  y-3">.          
-00000830: 2020 2020 2020 7b25 2069 6620 706f 7374        {% if post
-00000840: 5f6d 6573 7361 6765 2025 7d0a 2020 2020  _message %}.    
-00000850: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00000860: 2063 6c61 7373 3d22 616c 6572 7420 616c   class="alert al
-00000870: 6572 742d 7375 6363 6573 7320 616c 6572  ert-success aler
-00000880: 742d 6469 736d 6973 7369 626c 6520 6661  t-dismissible fa
-00000890: 6465 2073 686f 7720 2220 726f 6c65 3d22  de show " role="
-000008a0: 616c 6572 7422 3e0a 2020 2020 2020 2020  alert">.        
-000008b0: 2020 2020 2020 2020 2020 7b7b 2070 6f73            {{ pos
-000008c0: 745f 6d65 7373 6167 6520 7d7d 0a20 2020  t_message }}.   
-000008d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000008e0: 6275 7474 6f6e 2074 7970 653d 2262 7574  button type="but
-000008f0: 746f 6e22 2063 6c61 7373 3d22 6274 6e2d  ton" class="btn-
-00000900: 636c 6f73 6522 2064 6174 612d 6273 2d64  close" data-bs-d
-00000910: 6973 6d69 7373 3d22 616c 6572 7422 2061  ismiss="alert" a
-00000920: 7269 612d 6c61 6265 6c3d 2243 6c6f 7365  ria-label="Close
-00000930: 223e 3c2f 6275 7474 6f6e 3e0a 2020 2020  "></button>.    
-00000940: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00000950: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00000960: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-00000970: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00000980: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00000990: 2020 3c64 6976 2063 6c61 7373 3d22 7465    <div class="te
-000009a0: 7874 2d63 656e 7465 7222 3e3c 6275 7474  xt-center"><butt
-000009b0: 6f6e 2074 7970 653d 2273 7562 6d69 7422  on type="submit"
-000009c0: 3eeb acb8 ec9d 98ed 9598 eab8 b03c 2f62  >............</b
-000009d0: 7574 746f 6e3e 3c2f 6469 763e 0a20 2020  utton></div>.   
-000009e0: 2020 2020 2020 2020 203c 2f66 6f72 6d3e           </form>
-000009f0: 0a20 2020 2020 2020 2020 203c 2f64 6976  .          </div
-00000a00: 3e0a 0a20 2020 2020 2020 203c 2f64 6976  >..        </div
-00000a10: 3e0a 0a20 2020 2020 203c 2f64 6976 3e0a  >..      </div>.
-00000a20: 2020 2020 3c2f 7365 6374 696f 6e3e           </section>
+000001c0: 2063 6c61 7373 3d22 6278 2062 782d 7b7b   class="bx bx-{{
+000001d0: 2063 6f6e 7461 6374 2e69 6e66 6f31 2e62   contact.info1.b
+000001e0: 7820 7d7d 223e 3c2f 693e 0a20 2020 2020  x }}"></i>.     
+000001f0: 2020 2020 2020 2020 2020 2020 203c 6833               <h3
+00000200: 3e7b 7b20 636f 6e74 6163 742e 696e 666f  >{{ contact.info
+00000210: 312e 7469 746c 6520 7d7d 3c2f 6833 3e0a  1.title }}</h3>.
+00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000230: 2020 7b25 2069 6620 636f 6e74 6163 742e    {% if contact.
+00000240: 696e 666f 312e 6c69 6e6b 2025 7d0a 2020  info1.link %}.  
+00000250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000260: 3c61 2068 7265 663d 227b 7b20 636f 6e74  <a href="{{ cont
+00000270: 6163 742e 696e 666f 312e 636f 6e74 656e  act.info1.conten
+00000280: 7473 207d 7d22 2074 6172 6765 743d 225f  ts }}" target="_
+00000290: 626c 616e 6b22 3e7b 7b20 636f 6e74 6163  blank">{{ contac
+000002a0: 742e 696e 666f 312e 636f 6e74 656e 7473  t.info1.contents
+000002b0: 207d 7d3c 2f61 3e0a 2020 2020 2020 2020   }}</a>.        
+000002c0: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
+000002d0: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
+000002e0: 2020 2020 2020 203c 703e 7b7b 2063 6f6e         <p>{{ con
+000002f0: 7461 6374 2e69 6e66 6f31 2e63 6f6e 7465  tact.info1.conte
+00000300: 6e74 7320 7c20 7361 6665 207d 7d3c 2f70  nts | safe }}</p
+00000310: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000320: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000340: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00000350: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000360: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+00000370: 636f 6e74 6163 742e 696e 666f 3320 257d  contact.info3 %}
+00000380: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00000390: 6469 7620 636c 6173 733d 2263 6f6c 2d6d  div class="col-m
+000003a0: 642d 3622 3e0a 2020 2020 2020 2020 2020  d-6">.          
+000003b0: 2020 2020 7b25 2065 6c73 6520 257d 0a20      {% else %}. 
+000003c0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+000003d0: 7620 636c 6173 733d 2263 6f6c 2d6d 642d  v class="col-md-
+000003e0: 3132 223e 0a20 2020 2020 2020 2020 2020  12">.           
+000003f0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+00000400: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000410: 6469 7620 636c 6173 733d 2269 6e66 6f2d  div class="info-
+00000420: 626f 7820 6d74 2d34 2220 6461 7461 2d61  box mt-4" data-a
+00000430: 6f73 3d22 6661 6465 2d75 7022 2064 6174  os="fade-up" dat
+00000440: 612d 616f 732d 6465 6c61 793d 2231 3030  a-aos-delay="100
+00000450: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000460: 2020 2020 203c 6920 636c 6173 733d 2262       <i class="b
+00000470: 7820 6278 2d7b 7b20 636f 6e74 6163 742e  x bx-{{ contact.
+00000480: 696e 666f 322e 6278 207d 7d22 3e3c 2f69  info2.bx }}"></i
+00000490: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000004a0: 2020 2020 3c68 333e 7b7b 2063 6f6e 7461      <h3>{{ conta
+000004b0: 6374 2e69 6e66 6f32 2e74 6974 6c65 207d  ct.info2.title }
+000004c0: 7d3c 2f68 333e 0a20 2020 2020 2020 2020  }</h3>.         
+000004d0: 2020 2020 2020 2020 207b 2520 6966 2063           {% if c
+000004e0: 6f6e 7461 6374 2e69 6e66 6f32 2e6c 696e  ontact.info2.lin
+000004f0: 6b20 257d 0a20 2020 2020 2020 2020 2020  k %}.           
+00000500: 2020 2020 2020 203c 6120 6872 6566 3d22         <a href="
+00000510: 7b7b 2063 6f6e 7461 6374 2e69 6e66 6f32  {{ contact.info2
+00000520: 2e63 6f6e 7465 6e74 7320 7d7d 2220 7461  .contents }}" ta
+00000530: 7267 6574 3d22 5f62 6c61 6e6b 223e 7b7b  rget="_blank">{{
+00000540: 2063 6f6e 7461 6374 2e69 6e66 6f32 2e63   contact.info2.c
+00000550: 6f6e 7465 6e74 7320 7d7d 3c2f 613e 0a20  ontents }}</a>. 
+00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000570: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
+00000580: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00000590: 3e7b 7b20 636f 6e74 6163 742e 696e 666f  >{{ contact.info
+000005a0: 322e 636f 6e74 656e 7473 207c 2073 6166  2.contents | saf
+000005b0: 6520 7d7d 3c2f 703e 0a20 2020 2020 2020  e }}</p>.       
+000005c0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+000005d0: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
+000005e0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+000005f0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000600: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00000610: 207b 2520 6966 2063 6f6e 7461 6374 2e69   {% if contact.i
+00000620: 6e66 6f33 2025 7d0a 2020 2020 2020 2020  nfo3 %}.        
+00000630: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000640: 3d22 636f 6c2d 6d64 2d36 223e 0a20 2020  ="col-md-6">.   
+00000650: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00000660: 7620 636c 6173 733d 2269 6e66 6f2d 626f  v class="info-bo
+00000670: 7820 6d74 2d34 2220 6461 7461 2d61 6f73  x mt-4" data-aos
+00000680: 3d22 6661 6465 2d75 7022 2064 6174 612d  ="fade-up" data-
+00000690: 616f 732d 6465 6c61 793d 2231 3030 223e  aos-delay="100">
+000006a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000006b0: 2020 203c 6920 636c 6173 733d 2262 7820     <i class="bx 
+000006c0: 6278 2d7b 7b20 636f 6e74 6163 742e 696e  bx-{{ contact.in
+000006d0: 666f 332e 6278 207d 7d22 3e3c 2f69 3e0a  fo3.bx }}"></i>.
+000006e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006f0: 2020 3c68 333e 7b7b 2063 6f6e 7461 6374    <h3>{{ contact
+00000700: 2e69 6e66 6f33 2e74 6974 6c65 207d 7d3c  .info3.title }}<
+00000710: 2f68 333e 0a20 2020 2020 2020 2020 2020  /h3>.           
+00000720: 2020 2020 2020 207b 2520 6966 2063 6f6e         {% if con
+00000730: 7461 6374 2e69 6e66 6f33 2e6c 696e 6b20  tact.info3.link 
+00000740: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00000750: 2020 2020 203c 6120 6872 6566 3d22 7b7b       <a href="{{
+00000760: 2063 6f6e 7461 6374 2e69 6e66 6f33 2e63   contact.info3.c
+00000770: 6f6e 7465 6e74 7320 7d7d 2220 7461 7267  ontents }}" targ
+00000780: 6574 3d22 5f62 6c61 6e6b 223e 7b7b 2063  et="_blank">{{ c
+00000790: 6f6e 7461 6374 2e69 6e66 6f33 2e63 6f6e  ontact.info3.con
+000007a0: 7465 6e74 7320 7d7d 3c2f 613e 0a20 2020  tents }}</a>.   
+000007b0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000007c0: 2520 656c 7365 2025 7d0a 2020 2020 2020  % else %}.      
+000007d0: 2020 2020 2020 2020 2020 2020 3c70 3e7b              <p>{
+000007e0: 7b20 636f 6e74 6163 742e 696e 666f 332e  { contact.info3.
+000007f0: 636f 6e74 656e 7473 207c 2073 6166 6520  contents | safe 
+00000800: 7d7d 3c2f 703e 0a20 2020 2020 2020 2020  }}</p>.         
+00000810: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
+00000820: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
+00000830: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000840: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00000850: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
+00000860: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00000870: 2020 2020 2020 203c 2f64 6976 3e0a 0a20         </div>.. 
+00000880: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00000890: 0a20 2020 2020 2020 2020 203c 6469 7620  .          <div 
+000008a0: 636c 6173 733d 2263 6f6c 2d6c 672d 3620  class="col-lg-6 
+000008b0: 6d74 2d34 206d 742d 6c67 2d30 223e 0a20  mt-4 mt-lg-0">. 
+000008c0: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+000008d0: 7572 6c20 ed83 9cea b7b8 20ec 9588 ec97  url ...... .....
+000008e0: 9020 ec95 b5ec bba4 20ec 9db4 eb8f 9920  . ...... ...... 
+000008f0: eab0 80eb 8aa5 ed95 98eb 8ba4 202d 2d3e  ............ -->
+00000900: 0a20 2020 2020 2020 2020 2020 203c 666f  .            <fo
+00000910: 726d 2061 6374 696f 6e3d 227b 2520 7572  rm action="{% ur
+00000920: 6c20 2762 6f63 6f72 6473 3a68 6f6d 6527  l 'bocords:home'
+00000930: 2025 7d23 636f 6e74 6163 7422 206d 6574   %}#contact" met
+00000940: 686f 643d 2250 4f53 5422 2072 6f6c 653d  hod="POST" role=
+00000950: 2266 6f72 6d22 2063 6c61 7373 3d22 7068  "form" class="ph
+00000960: 702d 656d 6169 6c2d 666f 726d 2020 772d  p-email-form  w-
+00000970: 3130 3022 2064 6174 612d 616f 733d 2266  100" data-aos="f
+00000980: 6164 652d 7570 223e 0a20 2020 2020 2020  ade-up">.       
+00000990: 2020 2020 2020 207b 2520 6373 7266 5f74         {% csrf_t
+000009a0: 6f6b 656e 2025 7d0a 2020 2020 2020 2020  oken %}.        
+000009b0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000009c0: 3d22 726f 7722 3e0a 2020 2020 2020 2020  ="row">.        
+000009d0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000009e0: 7373 3d22 636f 6c2d 6d64 2d36 2066 6f72  ss="col-md-6 for
+000009f0: 6d2d 6772 6f75 7022 3e0a 2020 2020 2020  m-group">.      
+00000a00: 2020 2020 2020 2020 2020 2020 7b7b 2066              {{ f
+00000a10: 6f72 6d2e 6e61 6d65 207d 7d0a 2020 2020  orm.name }}.    
+00000a20: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000a30: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00000a40: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
+00000a50: 6f6c 2d6d 642d 3620 666f 726d 2d67 726f  ol-md-6 form-gro
+00000a60: 7570 206d 742d 3320 6d74 2d6d 642d 3022  up mt-3 mt-md-0"
+00000a70: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000a80: 2020 2020 7b7b 2066 6f72 6d2e 656d 6169      {{ form.emai
+00000a90: 6c20 7d7d 0a20 2020 2020 2020 2020 2020  l }}.           
+00000aa0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000ab0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00000ac0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00000ad0: 6469 7620 636c 6173 733d 2266 6f72 6d2d  div class="form-
+00000ae0: 6772 6f75 7020 6d74 2d33 223e 0a20 2020  group mt-3">.   
+00000af0: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
+00000b00: 666f 726d 2e63 6f6d 7061 6e79 207d 7d0a  form.company }}.
+00000b10: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000b20: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000b30: 2020 203c 6469 7620 636c 6173 733d 2266     <div class="f
+00000b40: 6f72 6d2d 6772 6f75 7020 6d74 2d33 223e  orm-group mt-3">
+00000b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000b60: 207b 7b20 666f 726d 2e6d 6573 7361 6765   {{ form.message
+00000b70: 207d 7d0a 2020 2020 2020 2020 2020 2020   }}.            
+00000b80: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000b90: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00000ba0: 733d 226d 792d 3322 3e0a 2020 2020 2020  s="my-3">.      
+00000bb0: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+00000bc0: 706f 7374 5f6d 6573 7361 6765 2025 7d0a  post_message %}.
+00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000be0: 3c64 6976 2063 6c61 7373 3d22 616c 6572  <div class="aler
+00000bf0: 7420 616c 6572 742d 7375 6363 6573 7320  t alert-success 
+00000c00: 616c 6572 742d 6469 736d 6973 7369 626c  alert-dismissibl
+00000c10: 6520 6661 6465 2073 686f 7720 2220 726f  e fade show " ro
+00000c20: 6c65 3d22 616c 6572 7422 3e0a 2020 2020  le="alert">.    
+00000c30: 2020 2020 2020 2020 2020 2020 2020 7b7b                {{
+00000c40: 2070 6f73 745f 6d65 7373 6167 6520 7d7d   post_message }}
+00000c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c60: 2020 203c 6275 7474 6f6e 2074 7970 653d     <button type=
+00000c70: 2262 7574 746f 6e22 2063 6c61 7373 3d22  "button" class="
+00000c80: 6274 6e2d 636c 6f73 6522 2064 6174 612d  btn-close" data-
+00000c90: 6273 2d64 6973 6d69 7373 3d22 616c 6572  bs-dismiss="aler
+00000ca0: 7422 2061 7269 612d 6c61 6265 6c3d 2243  t" aria-label="C
+00000cb0: 6c6f 7365 223e 3c2f 6275 7474 6f6e 3e0a  lose"></button>.
+00000cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cd0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00000ce0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+00000cf0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00000d00: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00000d10: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000d20: 3d22 7465 7874 2d63 656e 7465 7222 3e3c  ="text-center"><
+00000d30: 6275 7474 6f6e 2074 7970 653d 2273 7562  button type="sub
+00000d40: 6d69 7422 3eeb acb8 ec9d 98ed 9598 eab8  mit">...........
+00000d50: b03c 2f62 7574 746f 6e3e 3c2f 6469 763e  .</button></div>
+00000d60: 0a20 2020 2020 2020 2020 2020 203c 2f66  .            </f
+00000d70: 6f72 6d3e 0a20 2020 2020 2020 2020 203c  orm>.          <
+00000d80: 2f64 6976 3e0a 0a20 2020 2020 2020 203c  /div>..        <
+00000d90: 2f64 6976 3e0a 0a20 2020 2020 203c 2f64  /div>..      </d
+00000da0: 6976 3e0a 2020 2020 3c2f 7365 6374 696f  iv>.    </sectio
+00000db0: 6e3e                                     n>
```

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_faq.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_faq.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_features.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_features.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_hero.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_hero.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_portfolio.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_portfolio.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_pricing.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_pricing.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_services.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_services.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/_team.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/_team.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/footer.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/footer.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/header.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/header.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/index.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/index.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templates/bocords/seo.html` & `django_bocor_ds-2.2.0/django_bocor_ds/templates/bocords/seo.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/templatetags/bocords_tags.py` & `django_bocor_ds-2.2.0/django_bocor_ds/templatetags/bocords_tags.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/django_bocor_ds/views.py` & `django_bocor_ds-2.2.0/django_bocor_ds/views.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.1.0/pyproject.toml` & `django_bocor_ds-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django_bocor_ds"
-version = "2.1.0"
+version = "2.2.0"
 description = "my demiansoft templates"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
     "Django >= 4.2.11",
```

### Comparing `django_bocor_ds-2.1.0/PKG-INFO` & `django_bocor_ds-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_bocor_ds
-Version: 2.1.0
+Version: 2.2.0
 Summary: my demiansoft templates
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django >= 4.2.11
 Requires-Dist: libsass>=0.23.0
 Requires-Dist: django-analyticsds >= 0.3.1
```

