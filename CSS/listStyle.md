# CSS List Styles
Lists are a common element in web design used to prevent content from being un-organized. CSS allows you to style lists to match the design aesthetic and improve the readability of the web page.

Following are the various techniques for styling HTML lists.

- Unordered list styling
To style unordered lists (bulleted lists), we can change the list item marker.
```html
<!-- Syntax: -->

ul {
    list-style-type: value;
}
```

The value can be

- disc: (default) - Filled circle marker
- circle: hollow circle marker
- square: a filled square marker
- None: No marker (remove bullets)

# Example:
```html
<head>
    <style>
        .ul1 {
            list-style-type: disc;
        }
        .ul2 {
            list-style-type: circle;
        }
        .ul3 {
            list-style-type: square;
        }
        .ul4 {
            list-style-type: none;
        }
    </style>
</head>
<body>
    <ul class="ul1">
        <li>Hello world</li>
        <li>This is ul1</li>
    </ul>
    <ul class="ul2">
        <li>Hello world</li>
        <li>This is ul2</li>
    </ul>
    <ul class="ul3">
        <li>Hello world</li>
        <li>This is ul3</li>
    </ul>
    <ul class="ul4">
        <li>Hello world</li>
        <li>This is ul4</li>
    </ul>
</body>
</html>
```

# Ordered Lists Styling
For ordered lists (numbered lists), we can cusromize the list item numbering.

```html
<!-- Syntax: -->

ol {
    list-style-type: value;
}
```
The value can be any of the following:

- decimal: (default) - Decimal numbers (1, 2, 3, etc.)
- decimal-leading-zero: Decimal numbers with leading zeros (01, 02, 03, etc.)
- lower-roman: lowercase Roman numbers (i, ii, iii,...)
- upper-roman: uppercase Roman numbers (I, II, III,...)
- lower-alpha: lowercase alphabetical letters (a, b, c, etc.)
- upper-alpha: uppercase alphabetical letters (A, B, C, etc.)

# Example:
```html
<html lang="en">
<head>
    <title>CWH</title>
    <style>
        .ul1 {
            list-style-type: decimal;
        }
        .ul2 {
            list-style-type: decimal-leading-zero;
        }
        .ul3 {
            list-style-type: lower-roman;
        }
        .ul4 {
            list-style-type: upper-roman;
        }
        .ul5 {
            list-style-type: lower-alpha;
        }
        .ul6 {
            list-style-type: upper-alpha;
        }
    </style>
</head>
<body>
    <ul class="ul1">
        <li>hello, world</li>
        <li>This is style decimal</li>
    </ul>
    <ul class="ul2">
        <li>hello, world</li>
        <li>This is style list-style-type</li>
    </ul>
    <ul class="ul3">
        <li>hello, world</li>
        <li>This is lstyle lower-roman</li>
    </ul>
    <ul class="ul4">
        <li>hello, world</li>
        <li>This is style upper-roman</li>
    </ul>
    <ul class="ul5">
        <li>hello, world</li>
        <li>This is lower-alpha</li>
    </ul>
    <ul class="ul6">
        <li>hello, world</li>
        <li>This is upper-alpha</li>
    </ul>
</body>
</html>
```

# List-style position
The 'list-style-position' property determines where the list markers (bullets or numbers) are placed in relation to the content.

It has two values:

- inside: (default) List markers are inside the content's box. This is the default behaviour.
- outside: List markers are outside the content's box, typically to the left of the content, creating a hanging indent effect.
# Example:
```html
<html lang="en">
<head>
    <style>
        .ul1 {
            list-style-position: inside;
        }
        .ul2 {
            list-style-position: outside;
        }
    </style>
</head>
<body>
    <ul class="ul1">
        <li>hello, world</li>
        <li>list style position : inside</li>
    </ul>
    <ul class="ul2">
        <li>hello, world</li>
        <li>list style position : outside</li>
    </ul>
</body>
</html>
```

# Removing the default list styles
To remove default list styles (bullets or numbers), set the 'list-style' property to 'none'.

# Example:
```html
<html lang="en">
<head>
    <style>
        .ul1 {
            list-style: circle;
        }
        .ul2 {
            list-style: none;
        }
    </style>
</head>
<body>
    <ul class="ul1">
        <li>hello, world</li>
        <li>Developer</li>
    </ul>
    <ul class="ul2">
        <li>hello, world</li>
        <li>list style :none</li>
    </ul>
</body>
</html>
```

# Custom List Style
To set a custom list style, set the 'list-style-type' to your new required custom style.

# Example:
```html
<html lang="en">
<head>
    <style>
        .ul1 {
            list-style-type: "😍";
        }
    </style>
</head>
<body>
    <ul class="ul1">
        <li>name</li>
        <li>class</li>
    </ul>
</body>
```