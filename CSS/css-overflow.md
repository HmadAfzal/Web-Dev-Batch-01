# CSS Overflow
Sometimes the content shown is too large to be visible in a single line or division of the website. So, to avoid loss of that information we can use overflow property.


# Overflow Hidden
It hides the content which doesn’t fit the box.
```html
<!-- Eg: -->

div {
            background-color: rebeccapurple;
            width: 200px;
            height: 60px;
            border: 2px solid;
            overflow: hidden;
        }
 
```

# Overflow Scroll
It adds an automatic scroller in the container so for the seeing the content it can be scrolled without affecting the container dimensions.

 
```html
<!-- Eg: -->

div {
            background-color: rebeccapurple;
            width: 200px;
            height: 60px;
            border: 2px solid;
            overflow: scroll;
        }
 ```



# Overflow Auto
It is quite similar to scroll but the scroller is only added when the content starts getting out of the container. Mostly this option is used to avoid unnecessary scroll bars if the content already is within the content dimensions.