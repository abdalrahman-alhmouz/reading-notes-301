# The Call Stack and Debugging

* A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

* The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

* At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

* Types of errors in JS:
1-Reference errors
2-Syntax errors
3-Range errors
4-Type errors

* Best way to debug your code in javascript is to use console.log();

* Also to use call stack.

* We can use eslint to avoid runtime errors
