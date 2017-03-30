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

Between the comments below, write HTML to create a basic web page (using the
format described in the instructions). The page should have a title in the head
and an unordered list (with three items) inside the body.

<!DOCTYPE html>
<html>
<header>
 <h1>Title goes here</h1>
 <link rel="stylesheet" type="text/css" href="css/style.css">
  <script src="tbd.js" type="text/javascript" charset="utf-8" defer></script>
  </header>

<body>
<div>
  <ul>
    <li> List Item 1 </li>
    <li> List Item 2 </li>
    <li> List Item 3 </li>
  </ul>
</div>
</body>

<footer>
</footer>

</html>

## Question 2

How would we reference each of the following categories of elements?

-   All elements that belong to the _class_ `big`
-   The element matching _ID_ `contentPane`
-   Only those elements belonging to both the `important` and `red` _classes_
-   All `p` elements whose parent elements are `div`s

<!-- your answer starts here -->
In CSS, to refer to all elements of the class 'big', you'd use a period. So
.big {
    float: left;

}

In CSS, to refer to contentPane, you'd use a #. So
#contentPane {
    float: left;
}

For only those belonging to important and red:

.important .red {
    float: left;

}

All P elements as follow:
p {
 font-family: "Droid Serif", serif;
 line-height: 26px;
}
<!-- your answer ends here -->

## Question 3

Consider the following HTML and CSS code. What text color and font-family values
will the div labeled 'specialDiv' have?

**index.html**

```HTML
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" type="text/css" href="assets/css/main.css">
  </head>
  <body>
    <div class="things">
      <div class="specialDiv" style="font-family: cursive">
        Blah blah blah.
      </div>
    </div>
  </body>
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

The font family for .specialDiv is cursive,sans-serif and color is yellow

## Question 4

Order the following parts of the _box model_ from **'innermost'** to
**'outermost'**.


content, padding, border, margin

## Question 5

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

divTwo, divThree on left of screen...Then on right is divOne is all the way to the right of the window since floated right.
Next Line is divFour on left followed by divFive.

<!-- your answer starts here -->

<!-- your answer ends here -->

## Question 6

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

550px would only be affected where min-width is 400px.
So it would be set to 25% which is 25px
