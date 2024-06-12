# Flex-Box

FlexBox aka Flexible Box Layout makes it easier to layout, align and style items in the container while maintaining the responsiveness of the website.

To create a flexbox you need to set the display of the container as flex

Eg: {display: flex;}

This element is called the flex container, and stores the sub-elements which are known as flex items


# Flex Container Properties
The flex container properties are:

1. Flex Direction
It defines in which direction the flex elements would be displayed. It takes values like row, column or “reverse” too.


2. Flex Wrap
By using this property we can make our elements responsive for different screen sizes. 

3. Justify Content
This property is used to set the position of content or rather align content along the main axis.

4. Align Items
Just like the justify-content property, align-items define the alignment of the flex container but along the cross-axis.

5. Align Content
This property is very similar to align item but here rather than the flex items, the content present in the item is selected for the property.



# Flex Items Properties
The flex item properties are:

1. Order:
As the name suggests, this property sets the order in which the flex items are shown.

2. Flex Grow & Shrink
Decides the relative size of flex items. By default, this property is zero and thus items have the same size.

3. Align Self
This property allows default alignment to be overridden for the individual flex items. Try adding inline CSS to see how this property is used.

 



```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Flexbox</title>
    <style>
        .container {
            border: 2px solid red;
            display: flex;
            height: 80vh;
            /* justify-content: center; */
            align-items: center;
            /* flex-direction: column; */
            flex-wrap: wrap;
            /* align-content: flex-start; */
            /* there is no justify-items  in flexbox; */
            /* gap: 30px; 
            row-gap: 40px;
            column-gap: 10px; */
            gap: 40px 10px;

        }

        .item {  
            /* flex-grow: 1; */
            height: 92px;
            width: 92px;
            border: 2px solid black;
            /* margin: 4px; */
            background-color: blueviolet;
        }

        .order-1{
            order: 1;
        }
        .order-2{
            order: 2;
        }
        .order-3{
            order: 3;
        }

        .item1{  
            /* flex-grow: 2; */
            /* flex-shrink: 2; */
            align-self: flex-end;
        }
    </style>
</head>

<body>

    <main>
        <div class="container">
            <div class="item item1">1</div>
            <div class="item">2</div>
            <div class="item">3</div>
            <div class="item order-1">4</div>
            <div class="item"></div>
            <div class="item"></div>
            <div class="item"></div>
            <div class="item"></div>
            <div class="item"></div>
            <div class="item"></div>
            <div class="item"></div>
            
         
        </div>
    </main>

</body>

</html>
```