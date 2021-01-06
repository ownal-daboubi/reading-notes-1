# Read: 10 - JS Debugging:
# Error Handling & Debugging:
## Finding and understanding the errors:
* Know the order of the execution to find the source of the error.
* Define execution contexts:global context, function context, eval content.
* Variable scope: global scope, function-level scope.
* understanding what is the stack and how it works.
* use **exception**: a set of statements to handle the error.
* use **Error objects** to help you find where your mistakes are, like SyntaxError and ReferenceError.

## Fixing the errors:
* Debug your script:
 * What is the proplem.
 * where is the problem.
* Handle errors gracefully using try, catch, throw, and finally statements.
 * Example:
  ``` try {
      //Try to execute this code
      catch (exception) {
          //If there is an exception, run this code
          finally {
              //This always gets executed

``

* Set multiple breakpoints
* Use Console:
 * `console.table()`
 * `console.log()`
 * `console.info()`
 * `console.groupEnd ()`
 * `console.assert()`
* use debugger Keyword.
 * Example: 
 ``` if (area < 100) {
     debugger;
```
* throw errors: `throw new Error( message that you think is causing the error) ;`. 
![](https://res.cloudinary.com/practicaldev/image/fetch/s--k4xY232R--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://thepracticaldev.s3.amazonaws.com/i/ee9i03972mp4ts2qh8pd.png)

## Common Errors:
* Check your capitalization.
* Check that there are no missing closing braces } or parentheses ) .
* Check that there are no commas inside a , } or , ) by accident.
* Check if there is any missing ;
* Check the script is not missing a parameter when calling a function.
* Pay attention to the data type you are dealing with.

![](https://www.websolutions.com/Customer-Content/www/CMS/files/error_2.gif)


