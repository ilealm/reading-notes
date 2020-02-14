# Read 10 Error Handling & Debugging

### February 14th, 2020


### _FError Handling & Debugging_
* Execution context:
  * Global execution context. 
    * Code that is in the script, but not in functions.
    * There is only one global context in page.
    * Creates its own variable objects.
  * Function context functions: 
    * Code that is run un a function.
    * Each function has its own function context.
    * Creates its own variable objects. 
  * Eval context.
    * Code is executed like code in an internal function called eval().
  * Each execution context can also access it parents variable object.
    * If a variable is not found in the variable object or the current execution context, it can look to
    the variable object of the parent execution context. (which can affect performance). 
  * We can't access to the object variable. 
* Each context have its own _**variable object**_ :
    * Details of all of the variables, functions and parameters for that execution context.
* Variable scope:
  * Global.
  * Funtion level. Each time a fuction is called, the variables can have different value.
* The way the js interpreter execute commands, is by a stak line.
  * Each time a new item is addes to the list,  its creates a new execution context.
* Each time a script enters a new execution context, exist two phases of activity:
  1. Prepare:
    * The new scope is created.
    * Variables. funtions and arguments are created.
    * This is taking all the variables and functions and hoisting them to the top of the execution context.
  1. Execute:
    * Now it can be assign values to variables.
    * Reference functions and run their code.
    * Execute statemensts.
  * This two phases are called _**hoisting**_.
  * hoisting allows to call functions aor assign values to a variable that have not been declared yet.
  * When js finds an error, it throws an _**exeption**_.
    * When an error ocurrs, js will try to find the exeption-handing code. If there is none in the current context, will search in the parent context and so on.
