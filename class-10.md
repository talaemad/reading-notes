# JS Book 
# Chapter 10
* To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.
* The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope.
* EXECUTION CONTEXT Every statement in a script lives in one of three execution contexts.
* VARIABLE SCOPE The first two execution contexts correspond with the notion of scope.
* Each time a script enters a new execution context, there are two phases of activity:
1. PREPARE
* The new scope is created
* Variables, functions, and arguments are created
* The value of the this keyword is determined
2. EXECUTE
* Now it can assign values to variables
* Reference functions and run their code
* Execute statements

* In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's v a ri ables object.
* If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code.
* Error objects can help you find where your mistakes are and browsers have tools to help you read them.

1. DEBUG THE SCRIPT TO FIX ERRORS
If you come across an error while writing a script (or when someone reports a bug), you will need to debug the code, track down the source of the error, and fix it.
2. HANDLE ERRORS GRACEFULLY
You can handle errors gracefully using try, catch, throw, and finally statements.

* Debugging is about deduction: eliminating potential causes of an error. 

* WHERE IS THE PROBLEM?
First, should try to can narrow down the area where the problem seems to be. In a long script, this is especially important.
* WHAT EXACTLY IS THE PROBLEM?
Once you think that you might know the rough area in which your problem is located, you can then try to find the actual line of code that is causing the error.
* The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.
* The console will show you when there is an error in your JavaScript. It also displays the line where it became a problem for the interpreter.

* BREAKPOINTS You can pause the execution of a script on any line using breakpoints. Then you can check the va lues stored in variables at that point in time.
* If you set multiple breakpoints, you can step through them one-by-one to see where values change and a problem might occur.
* You can indicate that a breakpoint should be triggered only if a condition that you specify is met. The condition can use existing variables.
* If you know your code might fail, use try, catch, and finally. Each one is given its own code block.

1. `TRY` First, you specify the code that you t hink might throw an exception within the try block.
2. `CATCH` If the try code block throws an exception, catch steps in with an alternative set of code.
3. `FINALLY` The contents of the fi na 11 y code block will run either way - whether the try block succeeded or failed.

* If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.

* If you understand execution contexts (which have two stages) and stacks, you are more likely to find the error in your code.
* Debugging is the process of finding errors. It involves a process of deduction.
* The console helps narrow down the area in which the error is located, so you can try to find the exact error.
* JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.
* If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.