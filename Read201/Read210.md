# ERROR HANDLING & DEBUGGING


**ORDER OF EXECUTION**

To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run

**EXECUTION CONTEXTS**

The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope.


## UNDERSTANDING ERRORS

If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code.

**ERROR OBJECTS**

Error objects can help you find where your mistakes are
and browsers have tools to help you read them.

> Ref in book - 459-461 all type of error

**HOW TO DEAL WITH ERRORS**

there are two things we can do with the errors.

1- DEBUG THE SCRIPT TO FIX ERRORS

If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.

2- HANDLE ERRORS GRACEFULLY

You can handle errors gracefully using try, catch,
throw, and finally statements.

Sometimes, an error may occur in the script for a
reason beyond your control. For example, you might
request data from a third party, and their server
may not respond. In such cases, it is particularly
important to write error-handling code.

**A DEBUGGING WORKFLOW**

1. Look at the error message, it tells you:

• The relevant script that caused the problem.

• The line number where it became a problem for
the interpreter. (As you will see, the cause of
the error may be earlier in a script; but this is the
point at which the script could not continue.)

• The type of error (although the underlying cause
of the error may be different).

2. Check how far the script is running.
Use tools to write messages to the console to tell
how far your script has executed.

3. Use breakpoints where things are going wrong.
They let you pause execution and inspect the va lues
that are stored in variables.

**BROWSER DEV TOOLS & JAVASCRIPT CONSOLE**

The JavaScript console will tell you when there is a problem with a script,
where to look for the problem, and what kind of issue it seems to be.

The JavaScript console is just one of severa l developer tools that are
found in all modern browsers.

**BREAKPOINTS**

You can pause the execution of a script on any
line using breakpoints. Then you can check the
va lues stored in variables at that point in time.

**THROWING ERRORS**

If you know something might cause a problem for your script, you can
generate your own errors before the interpreter creates them.

To create your own error, you use the following line:
throw new Error('message');