# Read: 07 - HTML Tables; JS Constructor Functions:
# Domain Modeling:
* Domain modeling is the process of creating a conceptual model in code for a specific problem.
* A model describes the various entities, their attributes,behaviors, and the constraints that govern the problem domain.
* Object-oriented model:An entity that stores data in properties and encapsulates behaviors in methods.
* Tips for building domain models:
 1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
 2. Model its attributes with a constructor function that defines and initializes properties.
 3. Model its behaviors with small methods that focus on doing one job well.
 4. Create instances using the `new` keyword followed by a call to a constructor function.
 5. Store the newly created object in a variable so you can access its properties and methods from outside.
 6. Use the `this` variable within methods so you can access the object's properties and methods from inside.


## HTML Tables:
* `<table>` element: used to create a table.
* `<tr>` element: indicate the start of each row.
* `<td>` element: represent each cell of a table.
 * `colspan` attribute: indicates how many columns that cell should run across.
 * `rowspan` attribute: indicate how many rows a cell should span down the table.
* `<th>` element: represent the heading for either a column or a row.
 * `colspan` attribute: indicates how many columns that cell should run across.
 * `rowspan` attribute: indicate how many rows a cell should span down the table.
* `<thead>` element: the headings of the table should sit inside it.
* `<tbody>` element: The body should sit inside it.
* `<tfoot>` element: The footer should sit inside it.
* An Example:
``` <table>
<thead>
<tr>
<th></th>
<th scope="col">Home starter hosting</th>
<th scope="col">Premium business hosting</th>
</tr>
</thead>
<tbody>
<tr>
<th scope="row">Disk space</th>
<td>250mb</td>
<td>1gb</td>
</tr>
<tr>
<th scope="row">Bandwidth</th>
<td>5gb per month</td>
<td>50gb per month</td>
</tr>
</tbody>
<tfoot>
<tr>
<td></td>
<td colspan="2">Sign up now and save 10%!</td>
</tr>
</tfoot>
</table>
``` 
# Objects in JavaScript:
* Create an object: `var objectName = new object(){methods and properties};`
* Update a property: ` objectName.propertyName = propertyValue;`
* Delete a property: `delete objectName.propertyName`
* Creating many objects:
 1. Create the template with the object's properties and methods.
 ``` function Hotel (name, rooms, booked) {
     this . booked = booked;
     this . checkAvailability = function() {
         return this.rooms - this . booked;
         };
 ```
 2. create new object: new keyword, followed by a call to the function.
 `var newHotel = new Hotel ('new', 4,2)`
* The keyword `this`: It always refers to one object, usually the object in which the function operates.
* Array can be considered a type of object.

![](https://i.ytimg.com/vi/8iXoWC9XcU8/maxresdefault.jpg)

## Build-in Objects:
1. The Browser Object Model:
2. The global JavaScript objects
3. The Document Object Model
