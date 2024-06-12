# CSS Selectors

# What are CSS Selectors?
CSS selectors allow us to choose specific elements and apply styles to them. Suppose we want to add a custom style to only a specific tag(s). There, We can make use of CSS selector. 

There are different types of CSS selectors, which are as follows:

- Universal Selector
- Element Selector
- Id Selector
- Class Selector
- Group Selector
- Let's look into these selectors one by one

# Universal Selector
Universal selector represented by "*" targets all the HTML elements on the page.

```html
The syntax of Universal Selector is as follows:


* {
    property : value;
}

<!-- Consider the code snippet: -->

<html>

<head>
    <style>
        * {
            color: purple;
            text-align: center;
        }
    </style>
</head>

<body>
    <p>Welcome to </p>
    <h1>CodeWithHarry</h1>
</body>

</html>

```



# Element Selector (Type Selector)

The element selector selects the target element based on the specific type. Suppose you want to underline all the <p> tags; in this case, the element selector will be the best choice.

The syntax of Element Selector is as follows:

```html
p {
    property : value;
}
A selector can be any HTML tag. Here, we have considered the p tag.

<!-- Consider the code snippet: -->

<html>

<head>
    <title>CSS</title>
    <style>
        p{
            text-decoration: underline;
        }
    </style>
</head>

<body>
    <h1>CodeWithHarry</h1>
    <h2>we offer: </h2>
    <p>Python Tutorials - 100 Days of Code</p>
    <p>Ultimate JavaScript Course</p>
    <p>React JS Tutorials For Beginners</p>
</body>

</html>

```

Note: Element selector is not recommended as the same tag can be used multiple times in the document. So, overlapping rules can occur in the stylesheet.

# ID Selector
The ID selector targets the elements based on the specific ID. It is written with the hash “#” character followed by the ID name in the style sheet.

The syntax of ID Selector is as follows:

```html

#ID {
    property : value;
}
<!-- Consider the code snippet: -->

<html>

<head>
    <style>
        #title {
            text-align: center;
            color: red;
        }
    </style>
</head>

<body>
    <h1 id="title">CodeWithHarry</h1>
    <p>I'm a Developer and the founder of CodeWithHarry.com</p>
</body>

</html>

```

In the style block, the selector  #title, will only target the HTML element having an ID of "title".


# Class Selector
The class selector does the same job as the id selector, a class selector helps group various types of elements. Suppose, we want to give a custom style to a specific group of elements. In this case, the class selector is the best option.

It is written with the period “.” character followed by the class name in the style sheet.

The syntax of Class Selector is as follows:

```html

.class {
    property : value;
}

<!-- Consider the code snippet: -->

<html>

<head>
    <title>CSS</title>
    <style>
        .red {
            color: red;
        }
    </style>
</head>

<body>
    <p>This is simple p tag</p>
    <p class="red">This p tag has class red</p>
    <p>This is simple p tag</p>
    <p class="red">This p tag has class red</p>
</body>

</html>
```

In the above code snippet, the color:red will only be applied to the element having class 'red'.


# Group Selector

The group selector is used to minimise the code. Commas "," are used to separate each selector in a grouping. This reduces the number of lines of code. The code also looks clean.

The syntax of Group Selector is as follows:

```html
div, p, a {
    property : value;
}
<!-- Consider the code snippet: -->

<html>

<head>
    <title>CSS</title>
    <style>
        h1 {
            color: red;
        }

        p,a {
            color: purple;
        }
    </style>
</head>

<body>
    <h1>CodeWithHarry</h1>
    <p>This is the p tag</p>
    <a href="#">This is the anchor (a) tag</a>
</body>

</html>
```



# More Selectors

```html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>More on CSS Selectors</title>
    <style>
        /* .box:first-child{
            background-color: red;
        } */

        /* .box::first-line{
            color: yellow;
        } */

        /* .boxes *{
            color: blue;
            border: 2px solid black;
        }

        p, a, .box, [data-color="primary"]{
            padding-top: 45px;
        } */

        /* .box:nth-child(odd){
            background-color: blue;
        } */

        /* .box:nth-last-child(2){
            background-color: red;
        } */

        /* .boxes::before {
            content: "Harry is good";
            color: blue;
        } */

        /* .boxes::after {
            content: "Sigma course is also good";
            color: red;
        } */

        /* ::selection {
            background-color: black;
            color: aqua;
        } */

        /* .box::first-letter {
            color: peru;
            font-size: 45px;
        } */

        /* input::placeholder {
            color: rgb(84, 84, 88);
        } */
    </style>
</head>

<body>
    <div class="boxes">
        <div data-color="primary" class="box">I am first box</div>
        <div class="box">Hey I am a box</div>
        <div class="box">Hey I am a box</div>
        <input type="text" placeholder="Type your name here">
    </div>
</body>

</html>
```

# Summary:
Universal Selector(*): Target the entire page.
Element Selector: Target a specific element.
ID Selector(#): Target element with a specific ID.
Class Selector(.): Target element(s) with the same class.
Group Selector: Group elements and target them.
