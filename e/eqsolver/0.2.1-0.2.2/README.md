# Comparing `tmp/eqsolver-0.2.1-py3-none-any.whl.zip` & `tmp/eqsolver-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,11 @@
-Zip file size: 4255 bytes, number of entries: 4
--rw-rw-rw-  2.0 fat     8985 b- defN 24-Apr-25 21:59 eqsolver-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 21:59 eqsolver-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-25 21:59 eqsolver-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      301 b- defN 24-Apr-25 21:59 eqsolver-0.2.1.dist-info/RECORD
-4 files, 9379 bytes uncompressed, 3665 bytes compressed:  60.9%
+Zip file size: 11334 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     1057 b- defN 24-Apr-24 10:36 eqsolver/ISLM.py
+-rw-rw-rw-  2.0 fat       30 b- defN 24-Apr-25 00:44 eqsolver/__init__.py
+-rw-rw-rw-  2.0 fat     2385 b- defN 24-Apr-25 01:16 eqsolver/gasConsts.py
+-rw-rw-rw-  2.0 fat     3347 b- defN 24-Apr-25 01:48 eqsolver/gasEquations.py
+-rw-rw-rw-  2.0 fat    16403 b- defN 24-Apr-25 00:42 eqsolver/solver.py
+-rw-rw-rw-  2.0 fat     8970 b- defN 24-Apr-25 22:25 eqsolver-0.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 22:25 eqsolver-0.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-25 22:25 eqsolver-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      684 b- defN 24-Apr-25 22:25 eqsolver-0.2.2.dist-info/RECORD
+9 files, 32977 bytes uncompressed, 10166 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1,13 +1,28 @@
-Filename: eqsolver-0.2.1.dist-info/METADATA
+Filename: eqsolver/ISLM.py
 Comment: 
 
-Filename: eqsolver-0.2.1.dist-info/WHEEL
+Filename: eqsolver/__init__.py
 Comment: 
 
-Filename: eqsolver-0.2.1.dist-info/top_level.txt
+Filename: eqsolver/gasConsts.py
 Comment: 
 
-Filename: eqsolver-0.2.1.dist-info/RECORD
+Filename: eqsolver/gasEquations.py
+Comment: 
+
+Filename: eqsolver/solver.py
+Comment: 
+
+Filename: eqsolver-0.2.2.dist-info/METADATA
+Comment: 
+
+Filename: eqsolver-0.2.2.dist-info/WHEEL
+Comment: 
+
+Filename: eqsolver-0.2.2.dist-info/top_level.txt
+Comment: 
+
+Filename: eqsolver-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `eqsolver-0.2.1.dist-info/METADATA` & `eqsolver-0.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 Metadata-Version: 2.1
 Name: eqsolver
-Version: 0.2.1
+Version: 0.2.2
 Summary: Define model from system of equations, algebraically solve for variables, calculate boiling point, latent heat, other physics gas concepts
 Author: Brigham Turner
 Author-email: brighamturner12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 
-<h1>Equation System Solver: </h1>
+<h1>Equation System Solver </h1>
 
-<h3>Purpose:</h3>
+<h3>Purpose</h3>
 1) define your own model of equations, and use the solver to solve them.
 2) solve physics problems relating to gas: the energy to compress gas, final pressure/temperature after gas compression, boiling points and latent heat of water. 3) this solver can solve the ISLM economics model.
 
-<h3>Solver Overview:</h3>
+<h3>Solver Overview</h3>
 To use the tool, one instantiates the solver class with as input a class of equations. One then can call this class with a method name equal to one of these equations, or several (separated by underscores), using the names of known variables as arguments. The output is a dictionary showing the values of unknown variables.
 
-<h3>Equation Class:</h3>
+<h3>Equation Class</h3>
 Each variable in this class is an equation - as described earlier, to use the equation, the solver class is called with method name equal to the name of the variable storing the equations. The solver won't use all of the equations in the equation class, only the ones referenced in a function call (again, each equation name separated by an underscore).
 Warning: don't use "I" as a variable name because this will be counted as a complex number.
 
-<h3>Equation Class Optional Inner Classes:</h3>
+<h3>Equation Class Optional Inner Classes</h3>
 
 If the equation class has inner classes, then instead of using the variable name of an equation as a method name, one can instead use the name of the inner class, and the solver will know to use every single equation in said inner class. Unless accessed through the name of the inner class, the solver won't be able to access equations defined in inner classes so using them as a method name won't work (this is deliberate, to potentially allow equation names to be similar). This is particularly useful, because to define a constant, one just uses the constant name as the variable name and sets it equal to an integer or float (so not a string as would be the case for an equation), so constant names that are equal which are defined in inner classes won't conflict with each other.
 
 To allow the user to expose variables inside of an inner class to method calling, just add the key word "GROUP_" to the name of the inner class. This still allows all equations to be called simultaneously by using the inner class name (including the prefix "GROUP_").
 
 Inner classes can also import equations from other inner classes. To do this, rather than defining a variable inside of the inner class to be equal to an equation, define it to be equal to the name of a different already defined equation or inner class (if inner class, it imports all equations contained by that class). Just be sure to include the prefix "get:" in the string before the following equation / inner class name. This works successively: if inner class B has "x = 'get:A'", and inner class C has "x = 'get:B'" and inner class D has "x = 'get:C'" then inncer class D will ultimately be referencing equations all the way back to inner class A.
 
-<h3>Function Call Arguments:</h3>
+<h3>Function Call Arguments</h3>
 
 The the arguments to each method must be all of the known variables in the equations: there must always be at least as many equations as there are unknown variables. Thus, if you don't give the method enough known variables so that the unknown variables outnumber the equations it will throw an error. The name of each argument must be the same as the name of the variable. You may also provide a class with variable names in it, and it will decipher this class. Alternatively, you can simultaneously provide a class and keyword arguments.
 
-<h3>Getting Algebraic Solution:</h3>
+<h3>Getting Algebraic Solution</h3>
 Normally, the functions will return a dictionary where each key is an unknown variable and the value (float) of that key is the variable. All calculations are computed algebraically, not numerically, but unless you provide the keyword argument "algebraic" separated by underscores from the equation names in the name of the method, it will only give you the numbers for each solution, rather than the equation used to get these numbers.
 
 If instead you use the "algebraic" keyword, no numbers will be provided, rather it will provide a dictionary where each key is a variable name and the value is the equation that would give the variable name's value given known variables. This dictionary is actually the first value in a list that is returned, the second value in the list is simply a repetition of all the known variables.
 
-<h3>Multiple Solutions:</h3>
+<h3>Multiple Solutions</h3>
 If a system of equations has 2 solutions, you made also provide "solutionIndex" as an argument to the function and set this equal to either 0 - to get the first solution - 1 - to get the second solution, and so on. If there are multiple solutions but solutionIndex was never provided as a keyword, it will throw an error.
 
-<h3>Updating Class of Inputs with Solutions:</h3>
+<h3>Updating Class of Inputs with Solutions</h3>
 If you provide the solver with a class containing known variables and want the solver to variables to this class equal to the solutions, add "setVal = True" to the function arguments. If class already has these variables, it will throw an error unless you add "redefine = True" to the function arguments as well.
 
-<h3>Instances Where It Gets Stuck Loading:</h3>
+<h3>Instances Where It Gets Stuck Loading</h3>
 At its core, the equation solver uses sympy. This solver should be better than sympy because sympy has a difficult with long sequences of equations, where the first can be easily solved, and once it is, each next equation can easily be solved. In cases like these, sympy usually gets stuck endlessly loading, whereas this solver will be able to solve them. In my experience, this equation solver or sympy have never been wrong, however, sometimes they can't find solutions (meaning they get stuck infinitely loading) to systems that do in fact have solutions. Particularly in cases where u substitution is required or dividing one equation by another equation is required to solve algebraically.
 
-<h3>Numerical Solutions:</h3>
+<h3>Numerical Solutions</h3>
 One may get a numerical solution by including the keyword "numerical", separated by underscores, in a method call function name. Unfortunately, if there are multiple solutions, this may return the wrong one.
 
-<h3>Using Derivatives, Integrals, and Solve Function in Equations:</h3>
+<h3>Using Derivatives, Integrals, and Solve Function in Equations</h3>
 This solver can do a lot of interesting things with its equations - as seen in my examples with physics gas equations, an equation can use "integral", "derivative", or "solve" as functions - in the case of solve, it can solve an inner equation and put the output of that in the equation. See sympy for more details. It is also worth noting that sympy is coded to not use equations, but rather expressions that equal zero, so to use the solve function, the input is an expression that should resolve to zero, rather than an equation.
-<h3>When You Should Use This Tool:</h3>
+<h3>When You Should Use This Tool</h3>
 Ultimately, if your goal is to solve just one equation, then this tool may be a little overcomplicated and it would be better to just directly use sympy. Rather, the scope of this tool is to solve long and complicated equations in a simple way: All one does is define the equations in a class, give them to the solver, and then tell the solver the known variables and it provides a solution. This allows the user to focus on perfecting their model and making sure the equations are correct, rather than focusing on checking if algebra was performed correctly. 
 
 This solver also solves one of the bugs of sympy - as described before - sympy has a difficult time with systems with too many equations. Also, as an edge use, the solver class will store the algebraic solution to a problem once it is found. Thus, any algebra computed internally is never repeated, thus speeding up loops that may repeatedly ask for the same solution to an equation but with different inputs.
 
-<h3>Project Inspiration:</h3>
+<h3>Project Inspiration</h3>
 The original purpose of this tool was to simplify solving long systems of physics equations that were cumbersome to solve by hand and annoying to program into sympy. 
-<h3>Solving Physics Gas Problems, and ISLM model:</h3>
+<h3>Solving Physics Gas Problems, and ISLM model</h3>
 This solver already has stored in it a class containing the essential equations relating to gas compression and water evaporation. It can be used to solve for the boiling points of water and latent heat of water given pressure and temperature - computations that would be very difficult to perform by hand, and for which I haven't found python libraries that are coded to do.
 In addition, to the solver also has stored in it the equations for the ISLM model, though these equations often vary.
```

