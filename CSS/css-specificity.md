# CSS Specificity
CSS Specificity helps determine what style will be applied to the HTML element(s) when there are overlapping or multiple CSS rules.

It is a value or weight assigned to a CSS selector. The higher the specificity, the more precedence the selector has.

Let's consider the following code
```html
<html>
<head>
    <style>
        *{
            color: gray;
        }
        #title{
            color: red;
        }
        .h1{
            color: blue;
        }
        h1{
            color: pink;
        }
    </style>

</head>
<body>
    <h1 id="title" class="h1" style="color:purple">CodeWithHarry</h1>
</body>
</html>
 
```
Here the question is, what color will h1 be assigned to? This is calculated based on the selector's components which we will discussed in this tutorial.

# The Cascade Algorithm
CSS stands for Cascading Stylesheets. The cascade is the algorithm for solving conflicts where multiple CSS rules apply to an HTML element. It's the reason that the text of the button styled with the above CSS will be purple.

Understanding the cascade algorithm helps you understand how the browser resolves conflicts like this. The cascade algorithm has 4 distinct stages.

- Position and order of appearance: the order in which your CSS rules appear
- Specificity: an algorithm that determines which CSS selector has the strongest match
- Origin: the order in which CSS appears and where it comes from, whether that is a browser style, CSS from a browser extension, or your authored CSS
- Importance: some CSS rules are weighted more heavily than others, especially with the !important rule type
- 
Lets look into all these one by one

# Effect of Position
If there are two rules that have selectors of identical specificity, the last one to be declared won. In an HTML page, you can add styles in different ways: through a <link> tag, a <style> tag, or directly in the element's style attribute. If you have one <link> tag at the top of your page and another at the bottom, the styles from the bottom one will be used. The same goes for <style> tags; the ones lower down on the page take priority.

An inline style attribute with CSS declared in it will override all other CSS, regardless of its position, unless a declaration has !important defined.

If the browser doesn't support a property, it is ignored!

# Specificity
CSS specificity determines which style rules get applied to an element when there are conflicts. Higher specificity means the style will be used. It's calculated based on a point system involving inline styles, IDs, classes, and tag names.

# Inline Styles
Inline styles have the highest specificity and will always override styles if other selector(s) are also defined.
```html
<html>
<head>
    <style>
        *{
            color: gray;
        }
        #title{
            color: red;
        }
        .h1{
            color: blue;
        }
        h1{
            color: pink;
        }
    </style>

</head>
<body>
    <h1 id="title" class="h1" style="color:purple">CodeWithHarry</h1>
</body>
</html>
```

Here, you can see that the color: purple is applied to the h1 tag.

# ID Selector
The ID selector also has high specificity but comes after the inline Style specificity. So, if we have an ID and other selectors except the inline style, then the element will take the ID selector properties and values.
```html
<head>
    <style>
        *{
            color: gray;
        }
        #title{
            color: red;
        }
        .h1{
            color: blue;
        }
        h1{
            color: pink;
        }
    </style>
</head>
<body>
    <h1 id="title" class="h1">CodeWithHarry</h1>
</body>
</html>
```


# Class and Attribute Selectors
Class selectors and attribute selectors have moderate specificity. Suppose the element has a class or attribute selector and not an inline style or ID selector, then the element will take properties and values from the class or attribute selector.

```html
<head>
    <style>
        *{
            color: gray;
        
        .h1{
            color: pink;
        }
    </style>

</head>
<body>
    <h1 class="h1">CodeWithHarry</h1>
</body>
</html>
```

# Element Selector:
Element selectors like <p>, <div>, <a>, etc. have low specificity.
```html
<head>
    <style>
        *{
            color: gray;
        }
        h1{
            color: tomato;
        }
    </style>

</head>
<body>
    <h1 class="h1">CodeWithHarry</h1>
</body>
</html>
```

# Universal Selector:
Universal selectors (*) and combining selectors like not, first-child, and last-child have the lowest specificity.
```html
<head>
    <style>
        *{
            color: gray;
        }
    </style>

</head>
<body>
    <h1 class="h1">CodeWithHarry</h1>
</body>
</html>
```

So, the order of specificity is:

Inline Style > ID Selector > Class or Attribute Selector > Element Selector > Universal Selector

# Specificity Calculation
To calculate specificity, assign a value to each part of the selector:

- Universal Selector: 0
- Element selectors and pseudo-elements: 1
- Class selectors, attribute selectors, and pseudo-classes: 10
- ID selectors: 100
- Inline styles: 1000
Then, add up the values of all the parts in the selector.
