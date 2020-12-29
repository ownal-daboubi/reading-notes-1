# Links in HTML:
* Writing a link using `<a>` element:
Links are created using the `<a>` element which has an attribute called **href**. The value of the href attribute is the page that you want people to go to when they click on the link.
Ex: `<a href="http://www.empireonline.com">Empire</a>`.
* Linking to Other Pages on the Same Site:
When you are linking to other pages within the same site, you can use a relative URL.
Ex: `<a href="index.html">`

### Directory Structure:
* On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder.
* root folder: The top-level folder, contains all of the other files and folders for a website.
* The relationship between files and folders on a website is described using the same terminology as a family tree.
* The main homepage of a site written in HTML (and the homepages of each section in a child folder) is called *index.html*.
* Relative URLs can be used when linking to pages within your own website.

### Email links:
The href attribute starts with **mailto**: and is followed by the email address you want the email to be sent to.
Ex: `<a href="mailto:jon@example.org">Email Jon</a>`

### open in a new window:
you can use the target attribute on the opening `<a>` tag. The value of this attribute should be _blank.
Ex: `<a href="http://www.imdb.com" target="_blank">`

### Linking to a Specific Part of the Same Page:
* Before you can link to a specific part of a page, you need to identify the points in the page that the link will go to using the *id attribute*.
* you use the `<a>` element again, but the value of the href attribute starts with the `#` symbol, followed by the value of the id attribute of the element you want to link to.

# Layout:
## position property:
1. `position: static;` : for normal flow.this is the default way in which browsers treat HTML elements.
2. `position: relative;` : for Relative positioning, moves an element in relation to where it would have been in normal flow.
Ex:
``` p.example {
position: relative;
top: 10px;
left: 100px;
}

```
3. `position:absolute;`: for absolute positioning, the box is taken out of normal flow and no longer affects the
position of other elements on the page.
Ex: 
```
h1 {
position: absolute;
top: 0px;
left: 500px;
width: 250px;}
```
4. `position:fixed;`: Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed.

# Functions in JavaScript:
## What is functions:
* Functions let you group a series of statements together to perform a specific task. 
* If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements.
## Declaring a function:
`**function** Function-Name() {Code Block;}`
## Calling a function:
`Function_Name();`
## Declarings function that needs information:
`**function** Function-Name(parameters) {Code Block; **return** parameters;}`

![](https://res.cloudinary.com/practicaldev/image/fetch/s--pClJgvrv--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/mt2jlra7jd5gdgl8up8y.png)

## Calling a function that needs information:
`Function-Name(parameters value);`

## Functions Expressions:
* Expressions produce a value. They can be used where values are expected.
* If a function is placed where a browser expects to see an expression, then it gets treated as an expression.
* An Example:
``` var ar ea = f unction(width, height) {
r eturn width * height;
} ;
var size = area(3, 4) ;
```
## Variable Scope in JavaScript:
1. local scope: When a variable is created inside a function using the var keyword, it can only be used in that function. It is called a local variable or function-level variable. It is said to have local scope.
2. global scope: If you create a variable outside of a function, then it can be used anywhere within the script. It is called a global variable and has global scope.

## Variables and Memory:
* Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded.
* Local variables are only remembered during the period of time that a function is being executed.

![](https://i.imgur.com/iZ9I8lV.png)

# 6 Reasons for Pair Programming:
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness
![](https://stackify.com/wp-content/uploads/2017/05/Pair_Programming-e1496165906922-1280x720.png)