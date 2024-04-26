# Comparing `tmp/ofnodes-1.7.1.tar.gz` & `tmp/ofnodes-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.7.1.tar", max compression
+gzip compressed data, was "ofnodes-1.8.0.tar", max compression
```

## Comparing `ofnodes-1.7.1.tar` & `ofnodes-1.8.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.7.1/LICENSE
--rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.7.1/README.md
--rw-r--r--   0        0        0      590 2024-04-25 04:49:09.706501 ofnodes-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     1488 2024-04-25 04:48:44.846592 ofnodes-1.7.1/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 02:55:30.992047 ofnodes-1.7.1/src/ofnodes/components/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.7.1/src/ofnodes/components/nodes/__init__ copy.py
--rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.7.1/src/ofnodes/components/nodes/__init__.py
--rw-r--r--   0        0        0     2676 2024-04-23 17:49:14.794379 ofnodes-1.7.1/src/ofnodes/components/nodes/descriptors.py
--rw-r--r--   0        0        0      817 2024-04-23 19:26:45.294035 ofnodes-1.7.1/src/ofnodes/components/nodes/mixins.py
--rw-r--r--   0        0        0        0 2024-04-23 17:49:14.794379 ofnodes-1.7.1/src/ofnodes/components/structures/__init__.py
--rw-r--r--   0        0        0     9082 2024-04-23 17:49:14.794379 ofnodes-1.7.1/src/ofnodes/components/structures/descriptors.py
--rw-r--r--   0        0        0    20313 2024-04-23 17:49:14.794379 ofnodes-1.7.1/src/ofnodes/components/structures/mixins.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.7.1/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     1520 2024-04-23 18:51:28.074288 ofnodes-1.7.1/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.7.1/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.7.1/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0     2749 2024-04-25 04:48:44.850592 ofnodes-1.7.1/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.8.0/LICENSE
+-rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.8.0/README.md
+-rw-r--r--   0        0        0      590 2024-04-26 14:35:49.613667 ofnodes-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1488 2024-04-25 04:48:44.846592 ofnodes-1.8.0/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:55:30.992047 ofnodes-1.8.0/src/ofnodes/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.8.0/src/ofnodes/components/nodes/__init__ copy.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.8.0/src/ofnodes/components/nodes/__init__.py
+-rw-r--r--   0        0        0     2676 2024-04-23 17:49:14.794379 ofnodes-1.8.0/src/ofnodes/components/nodes/descriptors.py
+-rw-r--r--   0        0        0      817 2024-04-23 19:26:45.294035 ofnodes-1.8.0/src/ofnodes/components/nodes/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:49:14.794379 ofnodes-1.8.0/src/ofnodes/components/structures/__init__.py
+-rw-r--r--   0        0        0     9082 2024-04-23 17:49:14.794379 ofnodes-1.8.0/src/ofnodes/components/structures/descriptors.py
+-rw-r--r--   0        0        0    20486 2024-04-26 14:35:49.613667 ofnodes-1.8.0/src/ofnodes/components/structures/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.8.0/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     1520 2024-04-23 18:51:28.074288 ofnodes-1.8.0/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.8.0/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.8.0/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0     2737 2024-04-26 14:35:49.613667 ofnodes-1.8.0/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     2139 2024-04-26 14:35:49.613667 ofnodes-1.8.0/src/ofnodes/structures/stack.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.8.0/PKG-INFO
```

### Comparing `ofnodes-1.7.1/LICENSE` & `ofnodes-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.1/README.md` & `ofnodes-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.1/pyproject.toml` & `ofnodes-1.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.7.1"
+version = "1.8.0"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.7.1/src/ofnodes/__init__.py` & `ofnodes-1.8.0/src/ofnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.1/src/ofnodes/components/nodes/descriptors.py` & `ofnodes-1.8.0/src/ofnodes/components/nodes/descriptors.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.1/src/ofnodes/components/nodes/mixins.py` & `ofnodes-1.8.0/src/ofnodes/components/nodes/mixins.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.1/src/ofnodes/components/structures/descriptors.py` & `ofnodes-1.8.0/src/ofnodes/components/structures/descriptors.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.1/src/ofnodes/components/structures/mixins.py` & `ofnodes-1.8.0/src/ofnodes/components/structures/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,27 +100,25 @@
             >>> linked_structure.head.next
             >>> linked_structure.head, linked_structure.head.next, linked_structure.tail
             (Node(data='2 node'), None, Node(data='2 node'))
         """
         self.target = target_data  # trigger the setter
 
         if getattr(self._head, 'data') == self._target:
-            self.remove_head()
-            return
+            return self.remove_head()
 
         current_node = self._head
         while current_node.next is not self._tail:
             if current_node.next.data == self._target:
                 setattr(current_node, '_next', current_node.next.next)
                 return
             current_node = current_node.next
 
         if getattr(self._tail, 'data') == self._target:
-            self.remove_tail()
-            return
+            return self.remove_tail()
 
     def remove_head(self) -> None:
         """Removes the head node from the linked structure.
 
             Raises:
                 ValueError: If the linked structure is empty.
 
@@ -145,21 +143,23 @@
                 >>> linked_structure.head.data[42]
                 'a string'
                 >>> linked_structure.remove_head()
                 >>> linked_structure
                 LinkedStructure(head=None, tail=None)
         """
         if self._head and self._head is self._tail:
+            node = self._head
             self._head = None
             self._tail = None
-            return
+            return  node
         if self._head and self._head is not self._tail:
+            node = self._head
             self._head = self._head.next
-            return
-        raise ValueError("Cannot remove head from empty list")
+            return node
+        raise ValueError("Cannot remove head from empty linked structure")
 
     def remove_tail(self) -> None:
         """Removes the tail node from the linked structure.
 
         Raises:
             ValueError: If the linked structure is empty.
 
@@ -191,32 +191,35 @@
             """
         match self._head:
             case None:
                 raise ValueError("Cannot remove tail from empty list")
             case self._head:
                 if not getattr(self._head, "_next"):
                     # it's a one node list
+                    node = self._tail
                     setattr(self, "_head", None)
                     setattr(self, "_tail", None)
-                    return
+                    return node
                 if getattr(self._head, "next") is self._tail:
                     # there are two nodes
+                    node = self._tail
                     setattr(self, "_tail", self._head)
                     setattr(self._tail, "_next", None)
-                    return
+                    return node
                 # there are more than two nodes
                 node = self._head
                 # find second to last node
                 while getattr(node, "_next") and getattr(node._next, "_next"):
                     if getattr(node._next, "_next") is self._tail:
                         node = getattr(node, "_next")  # target found
                         break
                     node = getattr(node, "_next")  # keep looking
                 setattr(node, "_next", None)  # point the second to last node to None
                 setattr(self, "_tail", node)  # assign tail to the node
+                return node
 
 class PrintMixin:
     """Mixin class providing node data print functionality"""
     def print_node_data(self) -> None:
         """Traverse the linked data structure and print the data attribute of each node.
 
         Returns:
```

### Comparing `ofnodes-1.7.1/src/ofnodes/nodes/singlynode.py` & `ofnodes-1.8.0/src/ofnodes/nodes/singlynode.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.1/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-1.8.0/src/ofnodes/structures/singlylinkedlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             return "Empty Singly Linked List"
         node = self._head
         nodes = []
         while node:
             nodes.append(str(node.data))
             node = node.next
         return ' -> '.join(nodes)
-            
+
     def __dir__(self) -> list[str]:
         # Get the list of attributes and methods from the parent classes
         parent_dir = set(super().__dir__())
         # Filter out private attributes and methods
         parent_dir = {attr for attr in parent_dir if attr not in {'_head', '_tail', '_target'}}
         # Return a sorted list of all attributes and methods
         return sorted(parent_dir)
```

### Comparing `ofnodes-1.7.1/PKG-INFO` & `ofnodes-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 1.7.1
+Version: 1.8.0
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

