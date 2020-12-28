# HTML Lists, Control Flow with JS, and the CSS Box Model

## HTML Lists:

### Numbered lists
Lists where each item in the list is numbered.
Ex: 
`<ol>`
`<li>Number 1</li>`
`<li> Number 2</li>`
`</ol>`

### Bullet lists
Lists that begin with a bullet point.
Ex:
`<ul>`
`<li>a list</li>`
`<li>another list</li>`
`</ul>`

### Definition lists
Lists are made up of a set of terms along with the definitions for each of those terms.
Ex:
``` <dl>
<dt>the definition term</dt>
<dd>This is used to contain the definition.</dd>
</dl>
```
> NOTE: we can add a sub-list inside a list, it is called ** Nested list**.

## CSS Box Model:
### Controlling size of boxes
#### width, height properties:
Used to set your own dimensions for a box. 
Ex:
``` p {
height: 300px;
width: 300px;
}
```
#### min-width, max-width, min-height, max-height properties:
Some page designs expand and shrink to fit the size of the user's screen.
Ex:
```td.description {
min-width: 450px;
max-width: 650px;
}
```
#### overflow propertiy:
Tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:
1. hidden
2. scroll
Ex:
``` p.one {
overflow: hidden;}
p.two {
overflow: scroll;}
```
### Box model for borders, margin and padding:
Every box has three available properties that can be adjusted to control its appearance:
* The border separates the edge of one box from another.
 * border-width
 * border-style
 * border-color
* Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.
* Padding is the space between the border of a box and any content contained within it.
Here is an image for further explaination: 
![meaning](https://i.pinimg.com/originals/f6/f6/c9/f6f6c946356774ddb886956cd94df4c9.png)

#### display property:
Allows you to turn an inline element into a block-level element or vice versa.
The values this property can take are:
* inline: This causes a block-level element to act like an inline element.
* block: This causes an inline element to act like a block-level element.
* inline-block: This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.
* none: This hides an element from the page.
#### visibility property:
Allows you to hide boxes from users but It leaves a space where the element would have been.
The values this property can take are:
* hidden: This hides the element.
* visible: This shows the element.
#### border-image property:
The border-image property applies an image to the border of any box. It takes a background image and slices it into nine pieces.

#### box-shadow property:
Allows you to add a drop shadow around a box.

#### border-radius property:
To create rounded corners on any box.
Ex:
``` p {
border: 5px solid #cccccc;
padding: 20px;
width: 275px;
text-align: center;
border-radius: 10px;
-moz-border-radius: 10px;
-webkit-border-radius: 10px;}
```
# Arrays in JavaScript:
### Creating an array:
we use the **var** keyword followed by **the name of the array**, The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma.
Ex: 
``` var colors;
colors ['white', 'black', ' custom '];
```
### Values in an array:
Values can be accessed as if they are in a numbered list, counting starts from zero.
Ex: `var itemThree = colors [ 2] ;`

# Decisions and Loops:
## If-else statement:
Ex:
``` if (score >= pass) {
msg = 'Congratulations, you passed!';
} else {
msg = 'Have another go!';
}
```

## Switch statement:
Ex:
``` switch (level) {
case 1:
msg = 'Good luck on the first test ' ;
break;
case 2:
msg = 'Second of three - keep going!';
break;
default :
msg = 'Good l uck!';
break
}
```
## for loop:
Ex:
``` for (i = O; i < arraylength; i++) {
roundNumber = (i + l);
}
```
## while loop:
Ex:
``` while (i < 10) {
msg += i + ' x 5 = ' + (i * 5) + '<br I>';
i++;
}
```
## Do while loop:
Ex: 
``` do {
msg += i + ' x 5 = ' + (i * 5) + '<br I>' ;s
i++;
} wh il e ( i < 1) ;
```