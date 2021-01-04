# Readings: CSS Layout
# Layout:
we use Layout to control where each HTML element sits on a page and how to make this layout eye-catching

![](https://devdocs.magento.com/common/images/layouts_block_containers_defn21.png)


## position property:
List of properties used to control the elements of the page:
1. position: static; : for normal flow.this is the default way in which browsers treat HTML elements.
2. position: relative; : for Relative positioning, moves an element in relation to where it would have been in normal flow.
Ex:
``` p.example {
position: relative;
top: 10px;
left: 100px;
}

```
3. position:absolute;: for absolute positioning, the box is taken out of normal flow and no longer affects the
position of other elements on the page.
Ex: 
```
h1 {
position: absolute;
top: 0px;
left: 500px;
width: 250px;}
```
4. position:fixed; : is a type of absolute positioning that requires the position property to have a value of fixed.
5. `z-index` :to control which element sits on top.
Ex:
``` h1 {
position: fixed;
z-index: 10;}
}
```
6. The float property: allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible. 
Ex: `float: right;`
7. The clear property: allows you to say that no element should touch the left or right sides of a box.
Ex: `clear: left;`
8. `@import` rule: to import other style sheets. 
9. `<link>` element: rule to import other style sheets. 

![](https://fiverr-res.cloudinary.com/videos/so_27.964941,t_main1,q_auto,f_auto/d3zphhlsg0xkvqphqbn7/design-a-user-centered-and-modern-ecommerce-website-design.png)

for more Information: [w3school](https://www.w3schools.com/html/html_layout.asp).
