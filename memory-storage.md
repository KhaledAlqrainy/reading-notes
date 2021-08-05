# Memory Storage

### What is a ‘call’?

*  A call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation 

### How many ‘calls’ can happen at once?

* Only one.

### What does LIFO mean?

* Last In First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
 
* function greeting() {

    // [1] Some code here sayHi();
     
    // [2] Some code here } 
    
    function sayHi() { return “Hi!”; }


// Invoke the greeting function greeting();


// [3] Some code here

### What causes a Stack Overflow?

* when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

### What is a ‘refrence error’?

* It happens when you try to use a variable that is not yet declared 

### What is a ‘syntax error’?

* It happens  when you have something that cannot be parsed in terms of syntax

### What is a ‘range error’?

* It happens when you try to manipulate an object with some kind of length and give it an invalid length

### What is a ‘type error’?

* It happens when the types you are trying to use or access are incompatible

### What is a breakpoint?

* it can be achieved by putting a debugger statement in your code in the line you want to break.

### What does the word ‘debugger’ do in your code?

* when I want to put a breakpoint or console.log my code for example.