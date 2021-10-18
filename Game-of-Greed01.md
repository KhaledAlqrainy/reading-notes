# Scopes :

> Is the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on, A name will only be visible to and accessible by the code in its scope. 

* **Global scope:** The names that you define in this scope are available to all your code.

* **Local scope:** The names that you define in this scope are only available or visible to the code within the scope.


* In Global names any part of the code can modify it and causes a lot of errors, you need to keep up with code to know which value to assign.

* Using scopes will avoid this problem and let each variable in it own place were it can't be access in any part of the code. 

### Names and Scopes in Python

* Python uses the location of the name assignment or definition to associate it with a particular scope. In other words, where you assign or define a name in your code determines the scope or visibility of that name.

### Python Scope vs Namespace

* Python scope determines where in your program a name is visible and implemented as dictionaries that map names to objects.

* When you use a name Python searches through different scope levels (or namespaces) to determine whether the name exists or not.

### Using the LEGB Rule for Python Scope

> LEGB named after the Python scope for names. The letters in LEGB stand for Local, Enclosing, Global, and Built-in.

it stands for :


* **Local (or function) scope** is the code block or body of any Python function or lambda expression. 

* **Enclosing (or nonlocal) scope** is a special scope that only exists for nested functions.

* **Global (or module) scope** contains all of the names that you define at the top level of a program or a module. 

* **Built-in scope** contains names such as keywords, functions, exceptions, and other attributes that are built into Python. 

### Functions: The Local Scope

> Every time you call a function, you’re also creating a new local scope. On the other hand, you can think of each def statement and lambda expression as a blueprint for new local scopes. These local scopes will come into existence whenever you call the function at hand.


### Modules: The Global Scope

> Whenever you run a Python program or an interactive session like in the above code, the interpreter executes the code in the module or script that serves as an entry point to your program. This module or script is loaded with the special name, __main__. From this point on, you can say that your main global scope is the scope of __main__.


### builtins: The Built-In Scope

> is a special Python scope that’s implemented as a standard library module named built-ins in Python 3.x. All of Python’s built-in objects live in this module. They’re automatically loaded to the built-in scope when you run the Python interpreter. Python searches built-ins last in its LEGB lookup, so you get all the names it defines for free.


### The non-local Statement

* It consists of the nonlocal keyword followed by one or more names separated by commas. These names will refer to the same names in the enclosing Python scope 


### Discovering Unusual Python Scopes

* **Comprehension Variables Scope** is a compact way to process all or part of the elements in a collection or sequence. You can use comprehensions to create lists, dictionaries, and sets.

* **Exception Variables Scope** The exception variable is a variable that holds a reference to the exception raised by a try statement. In Python 3.x, such variables are local to the except block and are forgotten when the block ends.

* **Class and Instance Attributes Scope** The names that you assigned inside a class statement don’t clash with names elsewhere. You can say that these names follow the LEGB rule, where the class block represents the L level.


### Using Scope Related Built-In Functions

* **globals()** is a built-in function that returns a reference to the current global scope or namespace dictionary. This dictionary always stores the names of the current module. 

* **locals()** This updates and returns a dictionary that holds a copy of the current state of the local Python scope or namespace.

* **vars()** is a Python built-in function that returns the .**__dict__** attribute of a module, class, instance, or any other object which has a dictionary attribute. Remember that .**__dict__** is a special dictionary that Python uses to implement namespaces. 

* **dir()** using it without arguments to get the list of names in the current Python scope. If you call dir() with an argument, then the function attempts to return a list of valid attributes for that object