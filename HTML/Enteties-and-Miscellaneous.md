# Code Tag `<code>`

    The HTML `<code>` tag is a powerful element for displaying code snippets within a webpage. It preserves both spaces and line breaks, making it ideal for showcasing code.

## What is the `<code>` Tag?

    The HTML `<code>` tag is a simple yet powerful way to include code snippets in your webpage.

### Why Use the `<code>` Tag?

    - **Semantic Meaning**: Provides semantic value to the enclosed code.
    - **Readability**: This makes it easier for both browsers and developers to understand that the text is code.
    - **Styling**: Easier to style and highlight with CSS or JavaScript libraries like Prism.

## Basic Usage

    The most straightforward way to use the `<code>` tag is inline for short code snippets:

    ```html
    <code>Your code here</code>
    ```

# preTag `<pre>`

    The `<pre>` tag is used for displaying preformatted text, such as code snippets in various programming languages. The `<pre>` tag preserves the original formatting of text, making it an excellent choice for displaying code where spacing and indentation are key.

## Difference

    - The `<pre>` tag preserves formatting, including spaces and line breaks, while the `<code>` tag does not.
    - `<pre>` is generally used for displaying blocks of preformatted text, while `<code>` is used for inline code snippets within text.

# HTML Entities

    HTML entities are a crucial part of HTML markup language. They enable you to display characters that are reserved in HTML or that aren't readily available on the keyboard.

## What Are HTML Entities?

    HTML entities are used to represent special characters in a format that the browser can understand. They start with an ampersand (`&`) and end with a semicolon (`;`).

## Why Use HTML Entities?

    - Here are some reasons:
      - **Reserved Characters**: Characters like `<`, `>`, and `&` are reserved in HTML.
      - **Special Symbols**: For symbols like ©, ®, or mathematical symbols.
      - **Non-Breaking Spaces**: To create white spaces that won't break into a new line.

## Common HTML Entities

    - `&lt;` for `<`
    - `&gt;` for `>`
    - `&amp;` for `&`
    - `&nbsp;` for a non-breaking space
    - `&copy;` for ©

## How to Use HTML Entities

    Entities can be implemented easily within HTML code. Here are some examples:

### Using Reserved Characters

    ```html
    <p>The price is 10 &lt; 20.</p>
    ```

### Displaying Special Symbols

    ```html
    <p>Copyright &copy; 2023.</p>
    ```

### Creating Non-Breaking Spaces

    ```html
    <p>This is an example&nbsp;text.</p>
    ```

## Conclusion

    HTML entities are essential for rendering special or reserved characters on a web page. Understanding how to use them effectively is key to creating web pages that display content as intended.
