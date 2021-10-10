# Unit Test and TDD

**Unit test :** are pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

**AAA: Arrange, Act and Assert.** 

* Arrange: you need to organize the data needed to execute that piece of code (input);

* Act: here you will execute the code being tested (exercise the behaviour);

* Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

**TDD :** can grow our software design consciously and well, just building what is needed to make the test pass, craft the software design first and the code will be more reliable.


### If name equals main

> If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 

**it can be helpful for many reason such as :**
* Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.

* If you import this script as a module in another script, the __name__ is set to the name of the script/module.

* Python files can act as either reusable modules, or as standalone programs.

* if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.

### Recursion

> The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function.

* we have two types of Recursion, **Direct** and **indirect**.
* A function fun is called direct recursive if it calls the same function fun. A function fun is called indirect recursive if it calls another function say fun_new and fun_new calls fun directly or indirectly.
