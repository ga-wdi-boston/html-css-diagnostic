# HTML & CSS Diagnostic

This file is a **markdown** file. Markdown is a special way of formatting text,
and one that's used by GitHub in its README files.

In responding to some of these questions, you may be asked to write HTML or CSS
code. Please do so using the following Markdown formatting.

## For HTML

    ```HTML
    <html>
    ...
    </html>
    ```

## For CSS

    ```CSS
    ul {
      ...
    }
    ```

Using this format will make it easier for us to grade you, so that we can get
everyone their feedback faster. Thanks for your help!

## Question 1

When we say that the web is a service, what does that mean? Explain the
interaction in terms of clients and servers.

The web provides online accessibility to users, and this is done through the interaction
between clients and servers. Clients can be defined as web browsers or smartphone
apps that send out requests to the servers, and the servers are able to identify the
type of resource requested, what it will be used for, and it delivers it to the client.
The client, then, receives and displays the resource in its appropriate format whether
that is in the form of pdf files, a web page or images. 


## Question 2

Between the comments below, write HTML to create a basic web page (using the
format described in the instructions). The page should have a title in the head
and an unordered list (with three items) inside the body.

<!DOCTYPE html>
<html>
  <head>
    <title>Diagnostic</title>
  </head>
  <body>
    <ul>
      <li>A</li>
      <li>B</li>
      <li>C</li>
    </ul>
  </body>
</html>


## Question 3

How would we reference each of the following categories of elements?

-   All elements that belong to the _class_ `big`
-   The element matching _ID_ `contentPane`
-   Only those elements belonging to both the `important` and `red` _classes_
-   All `p` elements whose parent elements are `div`s

1. .big
2. #contentPane
3. .important, .red
4. div p


## Question 4

Consider the following HTML and CSS code. What text color and font-family values
will the div labeled 'specialDiv' have?

**index.html**

```HTML
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" type="text/css" href="assets/css/main.css">
</head>
  <div class="things">
    <div class="specialDiv" style="font-family: cursive">
      Blah blah blah.
    </div>
  </div>
</html>
```

**main.css**

```CSS
* {
  color: black;
}
div {
  color: blue;
}
.specialDiv {
  color: yellow;
  font-family: sans-serif;
}
.things {
  font-family: arial;
  color: red;
  font-size: 16px;
}
```

specialDiv will have the color yellow and it will first display the font-family
cursive, and if that is not available it will choose a generic sans-serif font.


## Question 5

Order the following parts of the _box model_ from **'innermost'** to
**'outermost'**.

content, border, margin, padding

Content --> Padding --> Border --> Margin


## Question 6

Consider the following HTML and CSS. Assuming that the window is much larger
than the dimensions of any of the `div`s given below, how will each `div` be
arranged on the page?

**index.html**

```HTML
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" type="text/css" href="assets/css/style.css">
</head>
<body>
  <div class="divOne"></div>
  <div class="divTwo"></div>
  <div class="divThree"></div>
  <div class="divFour"></div>
  <div class="divFive"></div>
</body>
</html>
```

**style.css**

```CSS
div {
  /* ... */
  /* Some other specifications, e.g. dimensions. */
  /* ... */
  float: left;
}

.divOne {
  float: right;
}

.divFour {
  clear: left;
}
```

divTwo, divThree, and divFive will be arranged on the same horizontal plane on
the left side, while divOne will be floated to the right of the other divs (also on the same line).
divFour will appear right after the line break, underneath the div's.   


## Question 7

Consider the following media queries. How wide, in `px`, would an element
with the class `.stretch` be at a _screen width_ of 550px?

```CSS
.stretch {
  width: 100px;
}

@media (min-width: 400px) {
  .stretch {
    width: 25%;
  }
}

@media (min-width: 800px) {
  .stretch {
    width: 30%;
  }
}
```

The media query (min-width: 400px) kicks in, assigning .stretch to 25% of the width
the pixels available on the screen.

550px * .25 = 137.5px
