# Comparing `tmp/neapolitan-24.3.tar.gz` & `tmp/neapolitan-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neapolitan-24.3.tar", last modified: Sun Mar 24 15:17:11 2024, max compression
+gzip compressed data, was "neapolitan-24.4.tar", last modified: Fri Apr 26 15:36:10 2024, max compression
```

## Comparing `neapolitan-24.3.tar` & `neapolitan-24.4.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      830 2024-02-25 11:40:41.743801 neapolitan-24.3/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2201 2024-02-25 10:14:00.232888 neapolitan-24.3/.github/workflows/test.yml
--rw-r--r--   0        0        0       71 2024-02-25 11:35:47.954340 neapolitan-24.3/.gitignore
--rw-r--r--   0        0        0     2453 2024-03-24 14:08:41.467554 neapolitan-24.3/CHANGELOG.rst
--rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-24.3/LICENSE
--rw-r--r--   0        0        0     2059 2024-01-10 19:10:13.295500 neapolitan-24.3/README.rst
--rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-24.3/docs/Makefile
--rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-24.3/docs/make.bat
--rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-24.3/docs/source/conf.py
--rw-r--r--   0        0        0     3710 2024-03-24 13:35:56.709747 neapolitan-24.3/docs/source/crud-view.rst
--rw-r--r--   0        0        0     2757 2023-06-20 05:53:36.043680 neapolitan-24.3/docs/source/index.rst
--rw-r--r--   0        0        0     3234 2024-02-02 14:37:37.025010 neapolitan-24.3/docs/source/templates.rst
--rw-r--r--   0        0        0     4304 2023-06-20 05:53:36.044167 neapolitan-24.3/docs/source/tutorial.rst
--rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-24.3/justfile
--rw-r--r--   0        0        0      659 2024-02-25 10:14:00.234693 neapolitan-24.3/pyproject.toml
--rw-r--r--   0        0        0      978 2024-03-24 14:09:06.768947 neapolitan-24.3/src/neapolitan/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 14:37:37.025055 neapolitan-24.3/src/neapolitan/management/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 14:37:37.025123 neapolitan-24.3/src/neapolitan/management/commands/__init__.py
--rw-r--r--   0        0        0     3682 2024-02-02 14:37:37.025247 neapolitan-24.3/src/neapolitan/management/commands/mktemplate.py
--rw-r--r--   0        0        0      595 2023-06-24 08:45:27.680357 neapolitan-24.3/src/neapolitan/templates/neapolitan/object_confirm_delete.html
--rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-24.3/src/neapolitan/templates/neapolitan/object_detail.html
--rw-r--r--   0        0        0      713 2023-06-20 05:53:36.045153 neapolitan-24.3/src/neapolitan/templates/neapolitan/object_form.html
--rw-r--r--   0        0        0      828 2023-06-20 05:31:31.333102 neapolitan-24.3/src/neapolitan/templates/neapolitan/object_list.html
--rw-r--r--   0        0        0      337 2023-06-20 05:31:31.333306 neapolitan-24.3/src/neapolitan/templates/neapolitan/partial/detail.html
--rw-r--r--   0        0        0     1137 2024-01-10 19:10:13.295755 neapolitan-24.3/src/neapolitan/templates/neapolitan/partial/list.html
--rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-24.3/src/neapolitan/templatetags/__init__.py
--rw-r--r--   0        0        0     1899 2023-04-24 09:52:53.326834 neapolitan-24.3/src/neapolitan/templatetags/neapolitan.py
--rw-r--r--   0        0        0    16883 2024-03-24 13:55:44.181755 neapolitan-24.3/src/neapolitan/views.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-24.3/tests/__init__.py
--rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-24.3/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-24.3/tests/migrations/__init__.py
--rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-24.3/tests/models.py
--rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-24.3/tests/settings.py
--rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-24.3/tests/templates/base.html
--rw-r--r--   0        0        0       14 2024-02-02 14:37:37.025535 neapolitan-24.3/tests/templates/tests/.gitignore
--rw-r--r--   0        0        0     4798 2024-03-24 13:55:04.994763 neapolitan-24.3/tests/tests.py
--rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 neapolitan-24.3/PKG-INFO
+-rw-r--r--   0        0        0      830 2024-02-25 11:40:41.743801 neapolitan-24.4/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2201 2024-02-25 10:14:00.232888 neapolitan-24.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0       71 2024-02-25 11:35:47.954340 neapolitan-24.4/.gitignore
+-rw-r--r--   0        0        0     4743 2024-04-26 14:48:47.547457 neapolitan-24.4/CHANGELOG.rst
+-rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-24.4/LICENSE
+-rw-r--r--   0        0        0     2100 2024-04-26 14:47:52.809372 neapolitan-24.4/README.rst
+-rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-24.4/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-24.4/docs/make.bat
+-rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-24.4/docs/source/conf.py
+-rw-r--r--   0        0        0     4647 2024-04-26 14:47:52.815015 neapolitan-24.4/docs/source/crud-view.rst
+-rw-r--r--   0        0        0     2757 2023-06-20 05:53:36.043680 neapolitan-24.4/docs/source/index.rst
+-rw-r--r--   0        0        0     3234 2024-02-02 14:37:37.025010 neapolitan-24.4/docs/source/templates.rst
+-rw-r--r--   0        0        0     4304 2023-06-20 05:53:36.044167 neapolitan-24.4/docs/source/tutorial.rst
+-rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-24.4/justfile
+-rw-r--r--   0        0        0      659 2024-02-25 10:14:00.234693 neapolitan-24.4/pyproject.toml
+-rw-r--r--   0        0        0      978 2024-04-26 14:55:57.141655 neapolitan-24.4/src/neapolitan/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 14:37:37.025055 neapolitan-24.4/src/neapolitan/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 14:37:37.025123 neapolitan-24.4/src/neapolitan/management/commands/__init__.py
+-rw-r--r--   0        0        0     3773 2024-04-26 14:47:52.797077 neapolitan-24.4/src/neapolitan/management/commands/mktemplate.py
+-rw-r--r--   0        0        0      595 2023-06-24 08:45:27.680357 neapolitan-24.4/src/neapolitan/templates/neapolitan/object_confirm_delete.html
+-rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-24.4/src/neapolitan/templates/neapolitan/object_detail.html
+-rw-r--r--   0        0        0      713 2023-06-20 05:53:36.045153 neapolitan-24.4/src/neapolitan/templates/neapolitan/object_form.html
+-rw-r--r--   0        0        0      821 2024-04-26 14:47:52.809606 neapolitan-24.4/src/neapolitan/templates/neapolitan/object_list.html
+-rw-r--r--   0        0        0      337 2023-06-20 05:31:31.333306 neapolitan-24.4/src/neapolitan/templates/neapolitan/partial/detail.html
+-rw-r--r--   0        0        0     1137 2024-01-10 19:10:13.295755 neapolitan-24.4/src/neapolitan/templates/neapolitan/partial/list.html
+-rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-24.4/src/neapolitan/templatetags/__init__.py
+-rw-r--r--   0        0        0     1822 2024-04-26 14:47:52.809804 neapolitan-24.4/src/neapolitan/templatetags/neapolitan.py
+-rw-r--r--   0        0        0    17529 2024-04-26 14:47:52.810058 neapolitan-24.4/src/neapolitan/views.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-24.4/tests/__init__.py
+-rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-24.4/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0      789 2024-04-26 14:47:52.810216 neapolitan-24.4/tests/migrations/0002_namedcollection.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-24.4/tests/migrations/__init__.py
+-rw-r--r--   0        0        0      438 2024-04-26 14:47:52.810385 neapolitan-24.4/tests/models.py
+-rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-24.4/tests/settings.py
+-rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-24.4/tests/templates/base.html
+-rw-r--r--   0        0        0       14 2024-02-02 14:37:37.025535 neapolitan-24.4/tests/templates/tests/.gitignore
+-rw-r--r--   0        0        0     8489 2024-04-26 14:47:52.810608 neapolitan-24.4/tests/tests.py
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 neapolitan-24.4/PKG-INFO
```

### Comparing `neapolitan-24.3/.github/workflows/docs.yml` & `neapolitan-24.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/.github/workflows/test.yml` & `neapolitan-24.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/LICENSE` & `neapolitan-24.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/README.rst` & `neapolitan-24.4/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -20,23 +20,26 @@
 
 I want easy CRUD views for it, without it taking all day:
 
 .. code:: python
 
     # urls.py
     from neapolitan.views import CRUDView
+    from .models import Bookmark
 
     class BookmarkView(CRUDView):
         model = Bookmark
         fields = ["url", "title", "note"]
         filterset_fields = [
             "favourite",
         ]
 
-    urlpatterns = [ ... ] + BookmarkView.get_urls()
+    urlpatterns = [
+        *BookmarkView.get_urls(),
+    ]
 
 Neapolitan's ``CRUDView`` provides the standard list, detail,
 create, edit, and delete views for a model, as well as the hooks you need to
 be able to customise any part of that.
 
 Neapolitan provides base templates and re-usable template tags to make getting
 your model on the page as easy as possible.
```

### Comparing `neapolitan-24.3/docs/Makefile` & `neapolitan-24.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/docs/make.bat` & `neapolitan-24.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/docs/source/conf.py` & `neapolitan-24.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/docs/source/index.rst` & `neapolitan-24.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/docs/source/templates.rst` & `neapolitan-24.4/docs/source/templates.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/docs/source/tutorial.rst` & `neapolitan-24.4/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/pyproject.toml` & `neapolitan-24.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/src/neapolitan/__init__.py` & `neapolitan-24.4/src/neapolitan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
 """
 
-__version__ = "24.3"
+__version__ = "24.4"
```

### Comparing `neapolitan-24.3/src/neapolitan/management/commands/mktemplate.py` & `neapolitan-24.4/src/neapolitan/management/commands/mktemplate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import shutil
 from pathlib import Path
 
 from django.core.exceptions import ImproperlyConfigured
 from django.core.management.base import BaseCommand, CommandError
 from django.template.loader import TemplateDoesNotExist, get_template
 from django.template.engine import Engine
+from django.apps import apps
 
 class Command(BaseCommand):
     help = "Bootstrap a CRUD template for a model, copying from the active neapolitan default templates."
 
     def add_arguments(self, parser):
         parser.add_argument(
             "model",
@@ -88,15 +89,16 @@
             # Get the filesystem path of neapolitan's object template.
             neapolitan_template = get_template(neapolitan_template_name)
             neapolitan_template_path = neapolitan_template.origin.name
 
             # Find target directory.
             # 1. If  f"{app_name}/templates" exists, use that.
             # 2. Otherwise, use first project level template dir.
-            target_dir = f"{app_name}/templates"
+            app_config = apps.get_app_config(app_name)
+            target_dir = f"{app_config.path}/templates"
             if not Path(target_dir).exists():
                 try:
                     target_dir = Engine.get_default().template_dirs[0]
                 except (ImproperlyConfigured, IndexError):
                     raise CommandError(
                         "No app or project level template dir found."
                     )
```

### Comparing `neapolitan-24.3/src/neapolitan/templates/neapolitan/object_confirm_delete.html` & `neapolitan-24.4/src/neapolitan/templates/neapolitan/object_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/src/neapolitan/templates/neapolitan/object_form.html` & `neapolitan-24.4/src/neapolitan/templates/neapolitan/object_form.html`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/src/neapolitan/templates/neapolitan/object_list.html` & `neapolitan-24.4/src/neapolitan/templates/neapolitan/object_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <div class="mt-4 sm:ml-16 sm:mt-0 sm:flex-none">
         <a class="block rounded-md bg-indigo-600 px-3 py-2 text-center text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
            href="{{ create_view_url }}">Add a new {{ object_verbose_name }}</a>
     </div>
 </div>
 
 {% if object_list %}
-    {% object_list object_list view.fields %}
+    {% object_list object_list view %}
 {% else %}
     <p class="mt-8">There are no {{ object_verbose_name_plural }}. Create one now?</p>
 {% endif %}
 
 <hr>
 
 {% endblock %}
```

### Comparing `neapolitan-24.3/src/neapolitan/templates/neapolitan/partial/list.html` & `neapolitan-24.4/src/neapolitan/templates/neapolitan/partial/list.html`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/src/neapolitan/templatetags/neapolitan.py` & `neapolitan-24.4/src/neapolitan/templatetags/neapolitan.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from django import template
-from django.urls import reverse
 from django.utils.safestring import mark_safe
 
+from neapolitan.views import Role
+
 register = template.Library()
 
 
-def action_links(object):
-    model_name = object._meta.model_name
+def action_links(view, object):
     actions = [
-        (reverse(f"{model_name}-detail", kwargs={"pk": object.pk}), "View"),
-        (reverse(f"{model_name}-update", kwargs={"pk": object.pk}), "Edit"),
-        (reverse(f"{model_name}-delete", kwargs={"pk": object.pk}), "Delete"),
+        (Role.DETAIL.reverse(view, object), "View"),
+        (Role.UPDATE.reverse(view, object), "Edit"),
+        (Role.DELETE.reverse(view, object), "Delete"),
     ]
     links = [f"<a href='{url}'>{anchor_text}</a>" for url, anchor_text in actions]
     return mark_safe(" | ".join(links))
 
 
 @register.inclusion_tag("neapolitan/partial/detail.html")
 def object_detail(object, fields):
@@ -34,34 +34,35 @@
             mf = object._meta.get_field(f)
             yield (mf.verbose_name, mf.value_to_string(object))
 
     return {"object": iter()}
 
 
 @register.inclusion_tag("neapolitan/partial/list.html")
-def object_list(objects, fields):
+def object_list(objects, view):
     """
     Renders a list of objects with the given fields.
 
     Inclusion tag usage::
 
-        {% object_list objects fields %}
+        {% object_list objects view %}
 
     Template: ``neapolitan/partial/list.html`` — Will render a table of objects
     with links to view, edit, and delete views.
     """
 
+    fields = view.fields
     headers = [objects[0]._meta.get_field(f).verbose_name for f in fields]
     object_list = [
         {
             "object": object,
             "fields": [
                 object._meta.get_field(f).value_to_string(object) for f in fields
             ],
-            "actions": action_links(object),
+            "actions": action_links(view, object),
         }
         for object in objects
     ]
     return {
         "headers": headers,
         "object_list": object_list,
     }
```

### Comparing `neapolitan-24.3/src/neapolitan/views.py` & `neapolitan-24.4/src/neapolitan/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import enum
 
 from django.core.exceptions import ImproperlyConfigured
 from django.core.paginator import InvalidPage, Paginator
-from django.db import models
 from django.forms import models as model_forms
 from django.http import Http404, HttpResponseRedirect
 from django.shortcuts import get_object_or_404
 from django.template.response import TemplateResponse
 from django.urls import path, reverse
 from django.utils.decorators import classonlymethod
+from django.utils.functional import classproperty
 from django.utils.translation import gettext as _
 from django.views.generic import View
 from django_filters.filterset import filterset_factory
 
 
 # A CRUDView is a view that can perform all the CRUD operations on a model. The
 # `role` attribute determines which operations are available for a given
@@ -54,14 +54,54 @@
             case Role.DETAIL:
                 return {"template_name_suffix": "_detail"}
             case Role.CREATE | Role.UPDATE:
                 return {"template_name_suffix": "_form"}
             case Role.DELETE:
                 return {"template_name_suffix": "_confirm_delete"}
 
+    @property
+    def url_name_component(self):
+        return self.value
+
+    def url_pattern(self, view_cls):
+        url_base = view_cls.url_base
+        url_kwarg = view_cls.lookup_url_kwarg or view_cls.lookup_field
+        path_converter = view_cls.path_converter
+        match self:
+            case Role.LIST:
+                return f"{url_base}/"
+            case Role.DETAIL:
+                return f"{url_base}/<{path_converter}:{url_kwarg}>/"
+            case Role.CREATE:
+                return f"{url_base}/new/"
+            case Role.UPDATE:
+                return f"{url_base}/<{path_converter}:{url_kwarg}>/edit/"
+            case Role.DELETE:
+                return f"{url_base}/<{path_converter}:{url_kwarg}>/delete/"
+
+    def get_url(self, view_cls):
+        return path(
+            self.url_pattern(view_cls),
+            view_cls.as_view(role=self),
+            name=f"{view_cls.url_base}-{self.url_name_component}"
+        )
+
+    def reverse(self, view, object=None):
+        url_name = f"{view.url_base}-{self.url_name_component}"
+        url_kwarg = view.lookup_url_kwarg or view.lookup_field
+        match self:
+            case Role.LIST | Role.CREATE:
+                return reverse(url_name)
+            case _:
+                return reverse(
+                    url_name,
+                    kwargs={url_kwarg: getattr(object, view.lookup_field)},
+                )
+
+
 
 class CRUDView(View):
     """
     CRUDView is Neapolitan's core. It provides the standard list, detail,
     create, edit, and delete views for a model, as well as the hooks you need to
     be able to customise any part of that.
     """
@@ -72,14 +112,15 @@
 
     # Object lookup parameters. These are used in the URL kwargs, and when
     # performing the model instance lookup.
     # Note that if unset then `lookup_url_kwarg` defaults to using the same
     # value as `lookup_field`.
     lookup_field = "pk"
     lookup_url_kwarg = None
+    path_converter = "int"
     object = None
 
     # All the following are optional, and fall back to default values
     # based on the 'model' shortcut.
     # Each of these has a corresponding `.get_<attribute>()` method.
     queryset = None
     form_class = None
@@ -246,18 +287,18 @@
 
     def get_success_url(self):
         assert self.model is not None, (
             "'%s' must define 'model' or override 'get_success_url()'"
             % self.__class__.__name__
         )
         if self.role is Role.DELETE:
-            success_url = reverse(f"{self.model._meta.model_name}-list")
+            success_url = reverse(f"{self.url_base}-list")
         else:
             success_url = reverse(
-                f"{self.model._meta.model_name}-detail", kwargs={"pk": self.object.pk}
+                f"{self.url_base}-detail", kwargs={"pk": self.object.pk}
             )
         return success_url
 
     # Pagination and filtering
 
     def get_paginate_by(self):
         """
@@ -326,15 +367,15 @@
 
         return None
 
     def get_context_data(self, **kwargs):
         kwargs["view"] = self
         kwargs["object_verbose_name"] = self.model._meta.verbose_name
         kwargs["object_verbose_name_plural"] = self.model._meta.verbose_name_plural
-        kwargs["create_view_url"] = reverse(f"{self.model._meta.model_name}-create")
+        kwargs["create_view_url"] = reverse(f"{self.url_base}-create")
 
         if getattr(self, "object", None) is not None:
             kwargs["object"] = self.object
             context_object_name = self.get_context_object_name()
             if context_object_name:
                 kwargs[context_object_name] = self.object
 
@@ -440,45 +481,27 @@
 
         # Mark the callback if the view class is async.
         # if cls.view_is_async:
         #     markcoroutinefunction(view)
 
         return view
 
+    @classproperty
+    def url_base(cls):
+        """
+        The base component of generated URLs.
+
+        Defaults to the model's name, but may be overridden by setting
+        `url_base` directly on the class, overriding this property::
+
+            class AlternateCRUDView(CRUDView):
+                model = Bookmark
+                url_base = "something-else"
+        """
+        return cls.model._meta.model_name
+
     @classonlymethod
-    def get_urls(cls):
+    def get_urls(cls, roles=None):
         """Classmethod to generate URL patterns for the view."""
-
-        verbose_name = cls.model._meta.model_name
-        urlpatterns = [
-            path(
-                f"{verbose_name}/",
-                cls.as_view(role=Role.LIST),
-                name=f"{verbose_name}-list",
-            ),
-            path(
-                f"{verbose_name}/new/",
-                cls.as_view(role=Role.CREATE),
-                name=f"{verbose_name}-create",
-            ),
-            # TODO: make the lookup field configurable. Determined by
-            # lookup_field and lookup_url_kwarg. ???: how to handle the type of
-            # the converter? (int, slug, etc.)
-            # It's just a string that gets passed to path(). SO an extra view
-            # field with the name of a registered converter.
-            path(
-                f"{verbose_name}/<int:pk>/",
-                cls.as_view(role=Role.DETAIL),
-                name=f"{verbose_name}-detail",
-            ),
-            path(
-                f"{verbose_name}/<int:pk>/edit/",
-                cls.as_view(role=Role.UPDATE),
-                name=f"{verbose_name}-update",
-            ),
-            path(
-                f"{verbose_name}/<int:pk>/delete/",
-                cls.as_view(role=Role.DELETE),
-                name=f"{verbose_name}-delete",
-            ),
-        ]
-        return urlpatterns
+        if roles is None:
+            roles = iter(Role)
+        return [role.get_url(cls) for role in roles]
```

### Comparing `neapolitan-24.3/tests/migrations/0001_initial.py` & `neapolitan-24.4/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/tests/settings.py` & `neapolitan-24.4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `neapolitan-24.3/PKG-INFO` & `neapolitan-24.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neapolitan
-Version: 24.3
+Version: 24.4
 Summary: Neapolitan: quick CRUD views for Django.
 Author-email: Carlton Gibson <carlton.gibson@noumenal.es>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django
 Requires-Dist: django-filter
 Requires-Dist: Sphinx ; extra == "docs"
@@ -37,23 +37,26 @@
 
 I want easy CRUD views for it, without it taking all day:
 
 .. code:: python
 
     # urls.py
     from neapolitan.views import CRUDView
+    from .models import Bookmark
 
     class BookmarkView(CRUDView):
         model = Bookmark
         fields = ["url", "title", "note"]
         filterset_fields = [
             "favourite",
         ]
 
-    urlpatterns = [ ... ] + BookmarkView.get_urls()
+    urlpatterns = [
+        *BookmarkView.get_urls(),
+    ]
 
 Neapolitan's ``CRUDView`` provides the standard list, detail,
 create, edit, and delete views for a model, as well as the hooks you need to
 be able to customise any part of that.
 
 Neapolitan provides base templates and re-usable template tags to make getting
 your model on the page as easy as possible.
```

