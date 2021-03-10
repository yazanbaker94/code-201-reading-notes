# ERROR HANDLING AND DEBUGGING



The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope. 



Each time a script enters a new execution context, there are two phases
of activity:
1: PREPARE
2: EXECUTE 



In the interpreter, each execution context has its own va ri ables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's v a ri ables object. 




If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handl ing code. 




Error objects can help you find where your mistakes are
and browsers have tools to help you read them.




Now that you know what an error is and how the browser treats them,
there are two things you can do with the errors. 


1: DEBUG THE SCRIPT TO FIX ERRORS 

2: HANDLE ERRORS GRACEFULLY 


Debugging is about deduction: eliminating potential causes of an error.
Here is a workflow for techniques you will meet over the next 20 pages.
Try to narrow down where the problem might be, then look for clues. 

The JavaScript console will tell you when there is a problem with a script,
where to look for the problem, and what kind of issue it seems to be. 

The JavaScript console is just one of several developer tools that are
found in all modern browsers. 




The console will show you when there is an
error in your JavaScript. It also displays the line
where it became a problem for the interpreter. 



Browsers that have a console have a console object, which has several
methods that your script can use to display data in the console.
The object is documented in the Console API. 


You can pause the execution of a script on any
line using breakpoints. Then you can check the
values stored in variables at that point in time.


If you set multiple breakpoints, you can step
through them one-by-one to see where values
change and a problem might occur. 




You can indicate that a breakpoint should be
triggered only if a condition that you specify is
met. The condition can use existing variables. 



If you know your code might fail, use try, catch, and finally.
Each one is given its own code block.


* TRY
* CATCH
* FINALLY 


If you know something might cause a problem for your script, you can
generate your own errors before the interpreter creates them. 




If you understand execution contexts (which have two
stages) and stacks, you are more likely to find the error
in your code.

Debugging is the process of finding errors. It involves a
process of deduction.

The console helps narrow down the area in which the
error is located, so you can try to find the exact error.

JavaScript has 7 different types of errors. Each creates
its own error object, which can tell you its line number
and gives a description of the error.

If you know that you may get an error, you can handle
it gracefully using the try, catch, finally statements.
Use them to give your users helpful feedback. 


![jscript](https://i.ibb.co/Tm0X31Z/Capture.png)




BOOKS USED:

1. javascript and jquery interactive jon du


