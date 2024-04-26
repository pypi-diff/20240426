# Comparing `tmp/glpic-99.0.202404252200.tar.gz` & `tmp/glpic-99.0.202404260848.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202404252200.tar", last modified: Thu Apr 25 22:00:46 2024, max compression
+gzip compressed data, was "glpic-99.0.202404260848.tar", last modified: Fri Apr 26 08:48:45 2024, max compression
```

## Comparing `glpic-99.0.202404252200.tar` & `glpic-99.0.202404260848.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:00:46.385367 glpic-99.0.202404252200/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 22:00:46.385367 glpic-99.0.202404252200/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 22:00:33.000000 glpic-99.0.202404252200/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:00:46.385367 glpic-99.0.202404252200/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-25 22:00:33.000000 glpic-99.0.202404252200/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-25 22:00:33.000000 glpic-99.0.202404252200/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:00:46.385367 glpic-99.0.202404252200/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 22:00:46.385367 glpic-99.0.202404252200/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 22:00:45.000000 glpic-99.0.202404252200/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:48:45.346756 glpic-99.0.202404260848/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-26 08:48:45.346756 glpic-99.0.202404260848/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-26 08:48:30.000000 glpic-99.0.202404260848/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:48:45.346756 glpic-99.0.202404260848/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-04-26 08:48:30.000000 glpic-99.0.202404260848/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-04-26 08:48:30.000000 glpic-99.0.202404260848/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:48:45.346756 glpic-99.0.202404260848/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:48:45.346756 glpic-99.0.202404260848/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-26 08:48:44.000000 glpic-99.0.202404260848/setup.py
```

### Comparing `glpic-99.0.202404252200/README.md` & `glpic-99.0.202404260848/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404252200/glpic/__init__.py` & `glpic-99.0.202404260848/glpic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,17 +170,18 @@
                 # reservation = _get(link['href'], headers=self.headers)[0]
                 info['reserved'] = True
         return info
 
     def info_reservation(self, reservation):
         return _get(f'{self.base_url}/ReservationItem/{reservation}', headers=self.headers)
 
-    def list_reservations(self):
+    def list_reservations(self, overrides={}):
+        user = overrides.get('user') or self.user
         response = _get(f'{self.base_url}/Reservation', headers=self.headers)
-        user_id = self.get_user(self.user)['id']
+        user_id = self.get_user(user)['id']
         return [r for r in response if r['users_id'] == user_id]
 
     def list_computers(self, user=None, overrides={}):
         computers = _get(f'{self.base_url}/Computer?with_devices', headers=self.headers)
         if not overrides:
             return computers
         results = []
```

### Comparing `glpic-99.0.202404252200/glpic/cli.py` & `glpic-99.0.202404260848/glpic/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         computerstable.add_row(entry)
     print(computerstable)
 
 
 def list_reservations(args):
     glpic = Glpic(args.url, args.user, args.token, args.debug)
     reservationstable = PrettyTable(["Id", "Item", "Begin", "End", "Comment"])
-    for reservation in glpic.list_reservations():
+    for reservation in glpic.list_reservations(overrides=handle_parameters(args.param)):
         _id, begin, end, comment = reservation['id'], reservation['begin'], reservation['end'], reservation['comment']
         reservation_id = reservation['reservationitems_id']
         computer_id = glpic.info_reservation(reservation_id)['items_id']
         reservation_name = glpic.info_computer(computer_id, full=True)['name']
         entry = [_id, reservation_name, begin, end, comment]
         reservationstable.add_row(entry)
     print(reservationstable)
@@ -168,14 +168,15 @@
     computerlist_parser.add_argument('-P', '--param', action='append', help=PARAMHELP, metavar='PARAM')
     list_subparsers.add_parser('computer', parents=[computerlist_parser], description=computerlist_desc,
                                help=computerlist_desc, aliases=['computers'])
 
     reservationlist_desc = 'List Reservations'
     reservationlist_parser = argparse.ArgumentParser(add_help=False)
     reservationlist_parser.set_defaults(func=list_reservations)
+    reservationlist_parser.add_argument('-P', '--param', action='append', help=PARAMHELP, metavar='PARAM')
     list_subparsers.add_parser('reservation', parents=[reservationlist_parser], description=reservationlist_desc,
                                help=reservationlist_desc, aliases=['reservations'])
 
     update_desc = 'Update Object'
     update_parser = subparsers.add_parser('update', description=update_desc, help=update_desc)
     update_subparsers = update_parser.add_subparsers(metavar='', dest='subcommand_update')
```

### Comparing `glpic-99.0.202404252200/setup.py` & `glpic-99.0.202404260848/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202404252200',
+    version='99.0.202404260848',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

