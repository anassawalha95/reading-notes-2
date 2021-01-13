> # Class 10 *Jan 14 2021:*

> ## Topics

  * Error Handling & Debugging

---

#### **Order of Exectution**

**Order of execution:** in JavaScript is dependent on the following components working together to pass and order information.

   1. The Callstack
  
   2. The Event Loop
   
   3. The Task Queue
   
   4. WebAPIs/External Resources
   
   
----

#### **Execution Context:**

* **The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates new execution context. They correspond to variable scope.**


   1. **Execution Context:**
     
     1. Global Context: Code that is in the script, but not in a function. There is only one global context in any page.
     
     2. Function Context: Code that is being run within a function. Each function has its own function context.
     
     3. Eval Context (NOT SHOWN) Text is executed like code in an internal function called eval {) (which is not covered in this book).
   
   2. Variable Scope:
   
     1. Global Scope: a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope.
     
     2. Function-Level Scope: When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope
     

![Order of execution](https://miro.medium.com/max/3600/1*ACtBy8CIepVTOSYcVwZ34Q.png)

#### **The Stack:**

**The JavaScript interperter processe one line of code at a time. When a statement needs data from another function, it stacks(or piles) the new function on top of the current task**


![Stack](https://miro.medium.com/max/1600/0*6T6KIVRkN9nWb3QU.gif)

----

#### **Execution Context & Hosting:**
 
**Each time a script enters a new execution context, there are two phases
of activity:**

  1. Prepare:
    
   1. The new scope is created
   
   2. Variables, functions, and arguments are created
   
   3. The value of the this keyword is determined
  
  2. Execution
  
   1. Now it can assign values to variables
   
   2. Reference functions and run their code
   
   3. Execute statements
   
----

#### **Understanding Errors:**

* **If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code.**

![Types of Error](https://static.javatpoint.com/cpages/images/programming-errors-in-c.png)

----

#### **Errors Object:**

* **JavaScript provide errors object can help you find code mistakes throw a perdifind object.**

   1. When an Error object is created, it will contain the following properties:
    
     |  PROPERTY  |         DESCRIPTION         |
     |:----------:|:---------------------------:|
     |    name    | Type of execution           |
     |   message  | Description                 |
     | fileNumber | Name of the JavaScript file |
     | lineNumber | Line number of error        |
     
   2. There are seven types of built-in error objects in JavaScript:
   
     |     OBJECT     |                           DESCRIPTION                           |
     |:--------------:|:---------------------------------------------------------------:|
     |      Error     | Generic error - the other errors are all based upon this error  |
     |  Syntax Error  | Syntax has not been followed                                    |
     | ReferenceError | Tried to reference a variable that is not declared/within scope |
     |    TypeError   | An unexpected data type that cannot be coerced                  |
     |   Range Error  | Numbers not in acceptable range                                 |
     |    URIError    | encodeURI ().decodeURI(),and similar methods used incorrectly   |
     |    EvalError   | eval() function used incorrectly                                |

----

#### **How to Deal with Errors:**

   1. Debug the script to fix errors: If you come across an error while writing a script (or when someone reports a bug), you will need to debug the code, track down the source of the error, and fix it.

   2. Handle errors Gracefully: You can handle errors gracefully using try, catch, throw, and fina1ly statements.
   
![HANDLING EXCEPTIONS](https://miro.medium.com/max/2440/1*dtzEohMaIfnKkB4luQGdEg.png) 

----

#### **Debugging Workflow:**

* **Debugging is about deduction: eliminating potential causes of an error.**

* **Where is the problem ?** First, should try to can narrow down the area where the problem seems to be.

   1. Look at the error message, it tells you:
  
      * The relevant script that caused the problem.
    
      * The line number where it became a problem for the interpreter
    
      * The type of error (although the underlying cause of the error may be different).

   2. Check how far the script is running. Use tools to write messages to the console to tell how far your script has executed.

   3. Use breakpoints where things are going wrong.

* **What is Exactly is the problem ?**     

   1. When you have set breakpoints, you can see if the variables around them have the values you would expect them to.
   
   2. Break down / break out parts of the code to test smaller pieces of the functionality
   
   3. Check the number of parameters for a function, or the number of items in an array.
   
----

#### **Browser DEV Tools & Javascript Console:**

* **The JavaScript console will tell you when there is a problem with a script,where to look for the problem, and what kind of issue it seems to be.**

   CHROME/ OPERA:
   
    On a PC, press the F12 key or:
    
    1. Go to the options menu (or three line menu icon)
    
    2. Select Toots or More tools.
    
    3. Select JavaScript Console or Developer Tools
    
    On a Mac press Alt + Cmd + J. Or:
    
    4. Go to the View menu.
    
    5. Select Developer.
    
    6. Open the JavaScript Console or Developer Tools option and select Console.
    
GitHub Repo: [View](https://github.com/anassawalha95/reading-notes-2/blob/main/Class%2010.md)

GitHub Live: [View](https://anassawalha95.github.io/reading-notes-2/Class%2010)
