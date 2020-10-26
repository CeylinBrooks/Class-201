# From the Duckett JS book:

## Ch. 10, “Error Handling & Debugging”

- The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope.
- EXECUTION CONTEXT
JavaScript
Hello Molly
Every statement in a script lives in one of three
execution contexts:
- Q GLOBAL CONTEXT
Code that is in the script, but not in a function.
There is only one global context in any page.
- FUNCTION CONTEXT
Code that is being run within a function.
Each function has its own function context.
Each time a script enters a new execution context, there are two phases
of activity:
1: PREPARE
• The new scope is created
• Variables, functions, and arguments are created
• The value of the this keyword is determined
Understanding that these two phases happen helps
with understanding a concept called hoisting. You
may have seen that you can:
• Call functions before they have been declared
(if they were created using function declarations

• Assign a value to a va ria ble that has not yet been
declared
This is because any variables and functions within
each execution context are created before they are
executed.
The preparation phase is often described as taking
all of the variables and functions and hoisting them
to the top of the execution context. Or you can think
of them as having been prepared.
Each execution context also creates its own
vari ab 1 es object. This object contains details of all
of the variables, functions, and parameters for that
execution context.
8 ERROR HANDLING & DEBUGGING
2: EXECUTE
• Now it can assign values to variables
• Reference functions and r
