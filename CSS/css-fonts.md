# CSS Fonts
Fonts play a crucial role in making your page visually appealing. Fonts decide how texts will look on the screen; depending on the website, different kinds of fonts are used.

- Let’s look at the major font attributes.

# Font Color
Font color defines the colour of the text or typography.

Syntax:
```html
selector{
    color: red;
}
```


# Font size
The font size property sets the size of the fonts.

It has some predefined sizes, such as small, medium, large, larger, etc.

The most commonly used units for font size are px (pixels), em (ems), rem (root ems), and percentage (%).

# Quick notes:

- px: px is the absolute unit. This is useful for setting precise sizes.
- em: em is the relative unit, based on the font size of the parent element. If the element's font size is 1.5 em, that means the element will be 1.5 times the size of the parent.
- rem: rem is the relative unit, based on the font size of the root element, i.e., <html>.
Example:
```html
<html lang="en">
<head>
    <style>
        #p1 {
            font-size: small;
        }
        #p2 {
            font-size: medium;
        }
        #p3 {
            font-size: large;
        }
        #p4 {
            font-size: larger;
        }
        #p5 {
            font-size: 25px;
        }
        #p6 {
            font-size: 2em;
        }
        #p7 {
            font-size: 2rem;
        }
        #p8 {
            font-size: 50%;
        }
    </style>
</head>
<body>
    <p id="p1">font-size: small</p>
    <p id="p2">font-size: medium</p>
    <p id="p3">font-size: largr</p>
    <p id="p4">font-size: larger</p>
    <p id="p5">font-size: 25px</p>
    <p id="p6">font-size: 2em</p>
    <p id="p7">font-size: 2rem</p>
    <p id="p8">font-size: 50%</p>
</body>
</html>

```

# CSS Font Style
The font style property sets the style of the font.

There are three types of font styles: italic, normal, and oblique.

- Quick notes:

italic: Italic texts are slightly to the right.
normal: Default text style.
Oblique: Oblique is similar to italic but has less bend
Example:
```html
<html lang="en">

<head>
    <style>
        #p1 {
            font-style: italic;
        }
        #p2 {
            font-style: normal;
        }
        #p3 {
            font-style: oblique;
        }
    </style>
</head>
<body>
    <p id="p1">font-style: italic</p>
    <p id="p2">font-style: normal</p>
    <p id="p3">font-style: oblique</p>
</body>
</html>
cwh tutorial image

CSS Font Variant
The CSS font variant property helps to toggle with the variations of the text.

There are two common values for the font-variant property.

normal: The default value.
small-caps: This value renders the text in small capital letters.
Example:
<html lang="en">
<head>
    <style>
        #p1 {
            font-variant: normal;
        }
        #p2 {
            font-variant: small-caps;
        }
    </style>
</head>
<body>
    <p id="p1">font-variant: normal;</p>
    <p id="p2">font-variant: small-caps;</p>
</body>
</html>
```

# CSS Font Weight
The font-weight property controls the thickness or boldness of the text.

The values range from 100 (thin) to 900 (ultra-bold) and also have some predefined values such as lighter, bold, and bolder.

Example:
```html
<html lang="en">
<head>
    <style>
        #p1 {
            font-weight: 100;
        }
        #p2 {
            font-weight: 200;
        }
        #p3 {
            font-weight: 300;
        }
        #p4 {
            font-weight: 400;
        }
        #p5 {
            font-weight: 500;
        }
        #p6 {
            font-weight: 600;
        }
        #p7 {
            font-weight: 700;
        }
        #p8 {
            font-weight: 800;
        }
        #p9 {
            font-weight: 900;
        }
        #p10 {
            font-weight: lighter;
        }
        #p11 {
            font-weight: bold;
        }
        #p12 {
            font-weight: bolder;
        }
    </style>
</head>
<body>
    <p id="p1">font-weight: 100</p>
    <p id="p2">font-weight: 200</p>
    <p id="p3">font-weight: 300</p>
    <p id="p4">font-weight: 400</p>
    <p id="p5">font-weight: 500</p>
    <p id="p6">font-weight: 600</p>
    <p id="p7">font-weight: 700</p>
    <p id="p8">font-weight: 800</p>
    <p id="p9">font-weight: 900</p>
    <p id="p10">font-size: lighter</p>
    <p id="p11">font-size: bold</p>
    <p id="p12">font-size: bolder</p>
</body>
</html>
```

# Font Family 
The font family property specifies the font stack. This is used to set the preferred font for the text content.

We can define multiple font family names separated by commas based on priority.

Syntax:
```html
selector{
      font-family: font1, font2, font3;
}
```
Example:
```html
<html lang="en">
<head>
    <style>
        h1{
            font-family: 'Courier New', Courier, monospace;
        }
        h2{
            font-family: 'Times New Roman', Times, serif;
        }
    </style>
</head>
<body>
    <h1>hello world</h1>
    <h2>Hello World</h2>
</body>
</html>
```


# Custom fonts
We can also use custom fonts for our websites; here, we will be using Google Fonts.

Follow the steps:

- Go to https://fonts.google.com/
- Select your preferred font.
- Choose the fonts based on font weight.
- Copy the import link and paste it on the top of the stylesheet.
- Copy the font family and paste it wherever you want to use it.
