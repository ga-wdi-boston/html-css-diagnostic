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

<!-- We say it is a service because it has clients that are requesting information from servers
which the respond with what the client was asking or looking for-->

<!-- clarity 5
      comfort 5
      knowledge-->

## Question 2

Between the comments below, write HTML to create a basic web page (using the
format described in the instructions). The page should have a title in the head
and an unordered list (with three items) inside the body.

<!-- your answer starts here -->
<!DOCTYPE html>
<html>
<head>
<title>This Webstie</title>
</head>
<body>
<ul>
<li></li>
<li></li>
<li></li>
</ul>
</body>
</html>

comfort 5
clarity 5
knowledge
<!-- your answer ends here -->

## Question 3

How would we reference each of the following categories of elements?

-   All elements that belong to the _class_ `big`
-   The element matching _ID_ `contentPane`
-   Only those elements belonging to both the `important` and `red` _classes_
-   All `p` elements whose parent elements are `div`s

<!-- your answer starts here -->
.big {}
.contentPane {}
.important,red {}
.div>p {}

clarity 5
comfort 5
used google to look up 3rd and 4th response
<!-- your answer ends here -->

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

<!-- your answer starts here -->
it will have san-serif and yellow text

comfort 5
clarity 5
knowledge
<!-- your answer ends here -->

## Question 5

Order the following parts of the _box model_ from **'innermost'** to
**'outermost'**.

content, border, margin, padding

<!-- your answer starts here -->
Padding, Border, Margin

comfort 5
clarity 5
knowledge
<!-- your answer ends here -->

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

<!-- your answer starts here -->
div will be floated on the left side of the page
divOne will be floated on the right side of the page
divTwo will be under div with a gap but not floated
DivThree will be right next to divTwo on the right side
divFour will be on the left side but not floated
divFive will be right under divFour connected and touching it

comfort 3
clarity 3
knowledge
<!-- your answer ends here -->

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

<!-- your answer starts here -->
i believe it would be 25% because the min width for 25 is 400px and the min width for 30% is 800px

clarity 4
comfort 4
knowledge

<!-- your answer ends here -->
