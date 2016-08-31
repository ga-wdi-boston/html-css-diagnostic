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

<!-- your answer starts here -->
The web allows the exchange of information between users and providers. The user
accesses information on the web through a program called a client, and the
provider processes requests from users and sends the requested information
through a program called a server. The web is a service in the sense that it is
the network and system by which providers fulfill requests from users.
<!-- your answer ends here -->

## Question 2

Between the comments below, write HTML to create a basic web page (using the
format described in the instructions). The page should have a title in the head
and an unordered list (with three items) inside the body.

<!-- your answer starts here -->
```HTML
<html>
  <head>
    <title>
      My Awesome Web Page
    </title>
  </head>
  <body>
    <ul>
      <li>Super</li>
      <li>Exciting</li>
      <li>Content!!!</li>
    </ul>
  </body>
</html>
```

<!-- your answer ends here -->

## Question 3

How would we reference each of the following categories of elements?

-   All elements that belong to the _class_ `big`
-   The element matching _ID_ `contentPane`
-   Only those elements belonging to both the `important` and `red` _classes_
-   All `p` elements whose parent elements are `div`s

<!-- your answer starts here -->
.big

#contentPane

.important.red

div p

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

<!-- your answer starts here -->
The div labled "specialDiv" will have yellow text from the cursive font family.
<!-- your answer ends here -->

## Question 5

Order the following parts of the _box model_ from **'innermost'** to
**'outermost'**.

content, border, margin, padding

<!-- your answer starts here -->
content
padding
border
margin
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
divOne and divFour will appear on the first line, with divFour at the far left
and divOne at the far right. The other divs will appear on subsequent lines,
individually and in this order: divTwo, divThree, divFive. Like this:

|divFour                divOne|
|divTwo                       |
|divThree                     |
|divFive                      |

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
At a screen width of 550px, .stretch will be as wide as 25% of the screen, so:

(550 * 0.25) = 137.5px

An element with the class .stretch will be 137.5px wide.

<!-- your answer ends here -->
