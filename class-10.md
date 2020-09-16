# Error Handling & Debugging
- ORDER OF EXECUTION 
To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run.
- EXECUT.ION CONTEXTS 
The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope. 

## EXECUTION CONTEXT & HOISTING
1: PREPARE
• The new scope is created
• Variables, functions, and arguments are created
• The value of the this keyword is determined

2: EXECUTE
• Now it can assign values to variables
• Reference functions and run their code
• Execute statements 
## ERROR OBJECTS

 > HOW TO DEAL WITH ERRORS
 
 you should:
 1: DEBUG THE SCRIPT TO FIX ERRORS
 2: HANDLE ERRORS GRACEFULLY 
 
 ## BROWSER DEV TOOLS & JAVASCRIPT CONSOLE 
 The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be. 
 
 ### LOOK AT ERRORS IN CHROME 
 The console will show you when there is an error in your JavaScript. It also displays the line where it became a problem for the interpreter.
 
 ### LOOK AT ERRORS IN FIREFOX 
 
1. The Console option is selected.
2. Only the JavaScript and Logging options need to be turned on. The Net, CSS, and Security options show other information. 
3. The type of error and the error message are shown on the left.
4. On the right-hand side of the console, you can see the name of the JavaScript file and the line number of the error. 

## DEBUGGING TIPS 
Here are a selection of practical tips that you can try to use when debugging your scripts. 
- ANOTHER BROWSER
Some problems are browserspecific. Try the code in another browser to see which ones are
causing a problem.
- ADD NUMBERS
Write numbers to the console so you can see which the items get logged. It shows how far your
code runs before errors stop it. 
- STRIP IT BACK
Remove parts of code, and strip it down to the minimum you need. You can do this either by
removing the code altogether, or by just commenting it out using multi-line comments:
/* Anything between these characters is a cofllllent */
- EXPLAINING THE CODE
Programmers often report finding a solution to a problem while explaining the code to someone else
- SEARCH
Stack Overflow is a Q+A site for programmers. 
- CODE PLAYGROUNDS
If you want to ask about problematic code on a forum, in addition to pasting the code into a post, you could add it to a code
playground site (such as JSBin.com, JSFiddle. com, or Dabbl et. corn) and then post a link to it from the forum. 

> If you understand execution contexts (which have two stages) and stacks, you are more likely to find the error in your code.
Debugging is the process of finding errors. It involves a process of deduction.

>The console helps narrow down the area in which the error is located, so you can try to find the exact error.

>JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.
If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedbackز
