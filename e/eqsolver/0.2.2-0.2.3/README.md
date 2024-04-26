# Comparing `tmp/eqsolver-0.2.2-py3-none-any.whl.zip` & `tmp/eqsolver-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11334 bytes, number of entries: 9
+Zip file size: 11586 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat     1057 b- defN 24-Apr-24 10:36 eqsolver/ISLM.py
 -rw-rw-rw-  2.0 fat       30 b- defN 24-Apr-25 00:44 eqsolver/__init__.py
 -rw-rw-rw-  2.0 fat     2385 b- defN 24-Apr-25 01:16 eqsolver/gasConsts.py
 -rw-rw-rw-  2.0 fat     3347 b- defN 24-Apr-25 01:48 eqsolver/gasEquations.py
 -rw-rw-rw-  2.0 fat    16403 b- defN 24-Apr-25 00:42 eqsolver/solver.py
--rw-rw-rw-  2.0 fat     8970 b- defN 24-Apr-25 22:25 eqsolver-0.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 22:25 eqsolver-0.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-25 22:25 eqsolver-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      684 b- defN 24-Apr-25 22:25 eqsolver-0.2.2.dist-info/RECORD
-9 files, 32977 bytes uncompressed, 10166 bytes compressed:  69.2%
+-rw-rw-rw-  2.0 fat     9897 b- defN 24-Apr-26 01:56 eqsolver-0.2.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-26 01:56 eqsolver-0.2.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-26 01:56 eqsolver-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      684 b- defN 24-Apr-26 01:56 eqsolver-0.2.3.dist-info/RECORD
+9 files, 33904 bytes uncompressed, 10418 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: eqsolver/gasEquations.py
 Comment: 
 
 Filename: eqsolver/solver.py
 Comment: 
 
-Filename: eqsolver-0.2.2.dist-info/METADATA
+Filename: eqsolver-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: eqsolver-0.2.2.dist-info/WHEEL
+Filename: eqsolver-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: eqsolver-0.2.2.dist-info/top_level.txt
+Filename: eqsolver-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: eqsolver-0.2.2.dist-info/RECORD
+Filename: eqsolver-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `eqsolver-0.2.2.dist-info/METADATA` & `eqsolver-0.2.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 Metadata-Version: 2.1
 Name: eqsolver
-Version: 0.2.2
+Version: 0.2.3
 Summary: Define model from system of equations, algebraically solve for variables, calculate boiling point, latent heat, other physics gas concepts
 Author: Brigham Turner
 Author-email: brighamturner12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: sympy
 
 
 <h1>Equation System Solver </h1>
 
 <h3>Purpose</h3>
 1) define your own model of equations, and use the solver to solve them.
 2) solve physics problems relating to gas: the energy to compress gas, final pressure/temperature after gas compression, boiling points and latent heat of water. 3) this solver can solve the ISLM economics model.
 
+Finaly, this solver also solves a bug in sympy allowing larger systems of equations to be solved.
+
 <h3>Solver Overview</h3>
 To use the tool, one instantiates the solver class with as input a class of equations. One then can call this class with a method name equal to one of these equations, or several (separated by underscores), using the names of known variables as arguments. The output is a dictionary showing the values of unknown variables.
 
+<h3>Examples</h3>
+
+[Here is an example for making a class containing equations - here for the equations defining the ISLM economics model.](https://github.com/brighamturner12/eqsolver/blob/main/gas/eqsolver/eqsolver/ISLM.py)
+
+[Here is the code that uses this class to find solutions to problems involivng the ISLM.](https://github.com/brighamturner12/eqsolver/blob/main/economicsExamples.py)
+
+[Here is an example containing a class for the physics gas equations.](https://github.com/brighamturner12/eqsolver/blob/main/gas/eqsolver/eqsolver/gasEquations.py)
+
+[And here these equations are used to solve physics problems.](https://github.com/brighamturner12/eqsolver/blob/main/gasExamples.py)
+
+One must note that in these examples, the entire file containing the model is imported as a class.
+
 <h3>Equation Class</h3>
 Each variable in this class is an equation - as described earlier, to use the equation, the solver class is called with method name equal to the name of the variable storing the equations. The solver won't use all of the equations in the equation class, only the ones referenced in a function call (again, each equation name separated by an underscore).
 Warning: don't use "I" as a variable name because this will be counted as a complex number.
 
 <h3>Equation Class Optional Inner Classes</h3>
 
 If the equation class has inner classes, then instead of using the variable name of an equation as a method name, one can instead use the name of the inner class, and the solver will know to use every single equation in said inner class. Unless accessed through the name of the inner class, the solver won't be able to access equations defined in inner classes so using them as a method name won't work (this is deliberate, to potentially allow equation names to be similar). This is particularly useful, because to define a constant, one just uses the constant name as the variable name and sets it equal to an integer or float (so not a string as would be the case for an equation), so constant names that are equal which are defined in inner classes won't conflict with each other.
```

