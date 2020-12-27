# Text in HTML:
Let`s start with some HTML tags and see how can we use them:

| Tag Name | Meaning | Tag Name | Meaning |
|----------|---------|----------|---------|
|  `<h1>`  |  used for main headings | `<h2> ... <h6>`  | used for subheadings |
| `<p>` |  create a paragraph |`<b> ` |  make characters appear bold |
| `<sup>` | used to contain characters that should be superscript |  `<i> `        |    make characters appear italic     |
| `<sub> ` | used to contain characters that should be subscript | <br/>  | add a line break inside the middle of a paragraph |
| `<hr />` | create a break between themes |`<blockquote> ` | used for longer quotes |
|`<strong> `|indicates that its content has strong importance| `<q> `|used for shorter quotes |
| `<em> ` | indicates emphasis that subtly changes the meaning of a sentence |`<abbr> `|used for an abbreviation or an acronym|
|`<cite>`| used to indicate where the citation is from|`<dfn> `| used to indicate the defining instance of a new term |
|`<address> `| contain contact details for the author of the page | `<ins> ` |used to show content that has been inserted into a document|
|`<s>`|indicates something that is no longer accurate or relevant |`<del> `|show text that has been deleted from it|

# Introducing CSS

CSS consists of rules that help you with controling how the content of an element should appear.

### Understanding CSS: Thinking Inside the Box
The key to understanding how CSS works is to imagine that there is an invisible **box** around every **HTML element**.
This will help us see the page that we want to create inside of our head before starting to write the code!
CSS rules help us control the box and its content!

### Blocks & Inline elements
* Block level elements look like they start on a new line..
* Inline elements flow within the text and do not start on a new line. 

### CSS Associates Style rues with HTML elements
In other words, we can add CSS rules to our HTML elements in order to customize them the way we desire!
 Here is an example of a CSS rule applied to a HTML element:
![A example CSS rule](https://puzzleweb.ru/en/images/css/1_1.png)

And Here is a practical example:
![html element](https://www.tutorialchip.com/wp-content/uploads/2011/01/Re-Defining-HTML-Tags.jpg)

### Linking CSS with HTML:
To do so:
1. Go to your HTML code
2. Between the **head** opening and closing tag
3. Write the following line:

![an example](https://help.globalscape.com/help/cuteftp9/images/DB_NewDocumentTemplate_link.gif)

### Using Internal CSS:
In case you don't to create a new CSS file, you can still apply CSS rules inside your HTML code, and here is how:
![an example](https://csharpcorner-mindcrackerinc.netdna-ssl.com/UploadFile/219d4d/basics-of-css-part-1/Images/paragraph%20color.png)

### CSS Selectors:
Remember: *Rules* are made of *selectors*
[Here is a link that can give you a good idea of the most common selectors in CSS](https://www.w3schools.com/cssref/css_selectors.asp) 

# Basic JavaScript Instructions:
Let`s start by defining some key vocabulary in JavaScript:
| Vocabulary | Meaning |
|----------|---------|
| Statement |Each individual instruction or step that a computer can follow one-by-one, ends with a ";" |
| Comments | To explain what your code does |
| Variables | Used to to temporarily store the bits of information |
| Array | a special type of variable. It doesn't just store one value; it stores a list of values |
| Expression | An expression evaluates into (results in) a single value |
| Operator | Allow programmers to create a single value from one or more values |
| Concatenation | The process of joining together two or more strings to create one new string |


### Variables Declaration: 
For that we use the variable keyword **var** followed by a **space** then **the name of the variable** then **;**
Ex: `var price;`

### Assign a value to a variable:
Variable name= variable value;
Ex: `price = 5;`

### Data Types: 
* Booleans
* Numbers
* Strings
> Note: we assign all of the data types to variables.

### Naming a variable:
Here are six rules you must always follow when giving a variable a name:
1. The name must begin with a letter, dollar sign ($), or an underscore. It must not start with a number.
2. The name can contain letters, numbers, dollar sign ($), or an underscore. Note that you must not use a dash or a period in a variable name.
3. You cannot use keywords or reserved words.
4. All variables are case sensitive.
5. Use a name that describes the kind of information that the variable stores.
6. If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word.

### Creating an array:
we use the **var** keyword followed by **the name of the array**, The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma.
Ex: `var colors;`
`colors ['white', 'black', ' custom '];`

### Values in an array:
Values can be accessed as if they are in a numbered list, counting starts from zero.
Ex: `var itemThree = colors [ 2] ;`

## Mathematical operators: 
Mathematical operators and their order of execution:

![d](https://i.stack.imgur.com/foy5H.png)

## String operators:
* There is just one string operator: **the+ symbol**. It is used to join the strings on either side of it.

## Comparison and Logical Operators:

| The Operator        | Its symbol |
|---------------------|------------|
| Equal to            | ==         |
| Not Equal to        | !=         |
| Strict equal to     | ===        |
| Strict not equal to | !==        |
| Greater than        | >          |
| Less than           | <          |
| Greater or equal to | =>         |
| Less or equal to    | <=         |
| Logical and         | &&         |
| Logical or          | \|\|       |
| Not                 | !          |

## Conditions and Loops:
### If Statement: 
Ex: `if (true) { console.log(Do this!); }`
### If else Statement:
Ex: `if (true) {console.log(In case it is true);} `
`else { console.log(In case it is false);}`

# Writing a Git Commit Message
*  Git commit message is the best way to communicate context about a change to fellow developers.
* Understanding why something happened months or years ago becomes not only possible but efficient.
* Teams should first agree on a commit message convention that defines at least the style, content, and metadata.

## The seven rules of a great Git commit message:
1. Separate subject from body with a blank line
2. Limit the subject line to 50 characters
3. Capitalize the subject line
4. Do not end the subject line with a period
5. Use the imperative mood in the subject line
6. Wrap the body at 72 characters
7. Use the body to explain what and why vs. how