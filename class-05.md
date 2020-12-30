# Read: 05 - HTML Images; CSS Color & Text:
# HTML Images:
## Adding Images:
* To add an image into the page you need to use an `<img>`element. It is a self-closing tag.
* It carry the following attributes:
 * `src`: This tells the browser where it can find the image file.
 * `alt`: This provides a text description of the image which describes the image if you cannot see it.
 * `title`: This provides additional information about the image.
 * `height`: This specifies the height of the image in pixels.
 * `width`: This specifies the width of the image in pixels.
 * `align`: It has been removed from HTML5.
* Example:
``` <img src="images/quokka.jpg" alt="A family of
quokka" width="600" height="450" />
```
## Image Placement:
Where you place the image in the code is important because browsers show HTML elements in one of two ways:
1. Block elements always appear on a new line. Examples of block elements include the `<h1>` and `<p>` elements. If the `<img>` is followed by a block level element then the block level element will sit on a new line after the imageas shown in the first example on this page.
2. Inline elements sit within a block level element and do not start on a new line. Examples of inline elements include the `<b>`,
`<em>`, and `<img>` elements. If the `<img>` element is inside a block level element, any text or other inline elements will flow around the image as shown in the second and third examples on this page.

## Three rules to remember when you are creating images for your website:
1. Save an image in the right formate:
 * **JPEG**: Whenever you have many different colors in a picture you should use a JPEG.
 * **GIF**, **PNG**: Use GIF or PNG format when saving images with few colors or large areas of the same color.
2. Save an image at the right size:
* The images you use on your website should be saved at the same *width* and *height* that you want them to appear on the page.
* When cropping images it is important not to lose valuable information. It is best to source images that are the correct shape if possible.
3. Use the correct resolution:
* Images created for the web should be saved at a resolution of **72 ppi**. The higher the resolution of the image, the larger the size of the file.

> Note: If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses.

## Tools to edit and save the image:
1. Adobe Photoshop.
2. Adobe Fireworks
3. Pixelmator
4. PaintShop Pro
5. Paint.net 

## HTML 5: Figure and Figure Caption:
* `<figure>`: used to contain images and their caption so that the two are associated.
* `<figcaption>`: allows web page authors to add a caption to an image.
* Example: 
```<figure>
<img src="images/otters.jpg" alt="Photograph of two sea otters floating in water">
<br />
<figcaption>Sea otters hold hands when they sleep so they don't drift away from each other.</figcaption>
</figure>
```
# CSS Colors:
## Color Property:
* This property allows you to specify the color of text inside an element.
* You can specify any color in CSS in one of three ways:
 1. RBG Values
 2. Hex Codes
 3. Color Names

## background-color Property:
* CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.
* An Example: 
``` body {
background-color: rgb(200,200,200);
background-color: hsl(0,0%,78%);
opacity: 0.5;
}
```
## Other features you can use:
* Contrast: When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.
* Opacity property: allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0.
* HSL Colors ( Hue, Saturation,Lightness):
 * hue: expressed as an angle (between 0 and 360 degrees).
 * saturation: expressed as a percentage.
 * lightness: expressed as a percentage with 0% being white, 50% being normal, and 100% being black.

# Text in CSS:
## The font-family property:
* The value of this property is the name of the typeface you want to use.
* Designers suggest pages usually look better if they use no more than *three* typefaces on a page.

## The Font-size property:
* enables you to specify a size for the font.
* Units of type size: Pixels, Percentages, Ems.
## @font-face:
allows you to use a font, even if it is not installed on the computer of the person browsing.
* Example:
``` @font-face {
font-family: 'ChunkFiveRegular';
src: url('fonts/chunkfive.eot');
}
```

## The Font-weight property:
allows you to create bold text. There are two values that this property commonly takes:
* `normal`: This causes text to appear at a normal weight.
* `bold`: This causes text to appear bold.

## The Font-style property:
There are three values this property can take:
* `normal`: This causes text to appear in a normal style.
* `italic`: This causes text to appear italic.
* `oblique`: This causes text to appear oblique.

## The text-transform property:
This is used to change the case of text:
* `uppercase`: This causes the text to appear uppercase.
* `lowercase`: This causes the text to appear lowercase.
* `capitalize`: This causes the first letter of each word to appear capitalized.

## The text-decoration property:
It allows you to specify the following values:
* `none`: This removes any decoration already applied to the text.
* `underline`: This adds a line underneath the text.
* `overline`: This adds a line over the top of the text.
* `line-through`: This adds a line through words.
* `blink`: This animates the text to make it flash on and off.

## The line-height property:
The line-height property sets the height of an entire line of text, so the difference between the fontsize and the line-height is equivalent to the leading.

## The letter-spacing, word-spacing properties:
When you specify a value for these properties, it should be given in ems, and it will be added on top of the default value specified by the font.

## The text-align property:
It allows you to control the alignment of text. The property can take one of four values: `left`, `right`, `center`, `justify`. 

## The vertical-align property:
It is more commonly used with inline elements such as `<img>`, `<em>`, or `<strong>` elements.

## The text-indent property:
It allows you to indent the first line of text within an element.

## The text-shadow property:
It is used to create a drop shadow.

## :first-letter, :first-line pseudo-elements:
Used to specify different values for the first letter or first line of text inside an element.

## :link, :visited pseudo classes:
They allow you to set different styles for links that have and have not yet been visited.

## :hover, :active, :focus pseudo-classes:
There are three pseudo-classes that allow you to change the appearance of elements when a user is interacting with them.

### Applying Text Example:
``` <style type="text/css">
body {
font-family: Georgia, Times, serif;
font-size: 12px;
font-weight: bold;
font-style: italic;
text-transform: uppercase;
text-decoration: underline;
line-height: 1.4em;
letter-spacing: 0.2em;
word-spacing: 1em;
text-align: left;
vertical-align: text-top;
text-indent: 20px;
text-shadow: -1px -1px #666666;
}
```
