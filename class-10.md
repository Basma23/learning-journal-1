# JS Debugging
## ORDER OF EXECUTION 
To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.[1]

## EXECUTION CONTEXTS 
The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope.[1] 

## THE STACK
The JavaScribt interpreter processes one line of code at a tim. When a statementneeds datafrom another function, it stacks the new function on top of the the current task.[1]

## Error Handling & Debugging
- When we understand the execution contexts and stacks, we will be able to find the error in our code.
- The process of finding errors we called it **Debugging**.
- Console is helping us to find the location of the error.
- There are 7 different types of errors of JavaScript. Each one of them creates its own error object, that can tell us about its error line number and gives a description of that error. 
-  We can handle our errors gracefully by using the try, catch, and statements. We use them to give our users helpful feedback. 

###### Resources
###### From Duckett JS book

[Main Page](https://basma23.github.io/reading-notes/)
