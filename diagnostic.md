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
  It means that it works through a combination of clients making requests and
  servers receiving and responding to said requests.

  A client sends and HTTP request to an HTTP server. The server processes the
  request, which creates the HTTP response. The response is sent to the client,
  and the client processes the response.
<!-- your answer ends here -->

## Question 2

Between the comments below, write HTML to create a basic web page (using the
format described in the instructions). The page should have a title in the head
and an unordered list (with three items) inside the body.

<!-- your answer starts here -->
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My Page of Cat Fails!</title>
  </head>
  <body>
    <ul>
      <li>Cat Fail</li>
      <li>Cat Fail 2</li>
      <li>And yet another Cat Fail!</li>
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
```CSS
.big
#contentPane
.important.red
div > p
```
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
  .specialDiv will be yellow and have the cursive font family
<!-- your answer ends here -->

## Question 5

Order the following parts of the _box model_ from **'innermost'** to
**'outermost'**.

content, border, margin, padding

<!-- your answer starts here -->
content, padding, border, margin
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
Taken together, all five divs will be floated to the left. Within that, .divFour
 will be at the top. Below it, divOne will be on the right.
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
100px.
<!-- your answer ends here -->
