This file is a **markdown** file. Markdown is a special way of formatting text, and one that's used by GitHub in its README files.

In responding to some of these questions, you may be asked to write HTML or CSS code. Please do so using the following Markdown formatting.

##### For HTML
    ```HTML
    <html>
    ...
    </html>
    ```

##### For CSS
    ```CSS
    ul {
      ...
    }
    ```

Using this format will make it easier for us to grade you, so that we can get everyone their feedback faster. Thanks for your help!

## Question 1

When we say that the web is a service, what does that mean? Explain the interaction in terms of clients and servers.
<!-- your answer starts here -->
That mean that the web is a service between the client and a server. They both need each other to be a service. The client asks for information from the server and the server provide the data the client needs.
<!-- your answer ends here -->

## Question 2

Between the comments below, write HTML to create a basic web page (using the format described in the instructions). The page should have a title in the head and an unordered list (with three items) inside the body.
<!-- your answer starts here -->
<!DOCTYPE html>
<html>
  <head>
    <title>Test Webpage!!!</title>
  </head>
  <body>
    <ul>
      <li>One</li>
      <li>Two</li>
      <li>Three</li>
    </ul>
   </body>
   <footer>
    <p>Something smells like feet down here...</p>
  </footer>
</html>
<!-- your answer ends here -->

## Question 3

What selectors could we write to reference each of the following categories of elements?
* All elements that belong to the class `big`
* The element matching ID `contentPane`
* Any elements that belong both to the `important` and `red` classes
* Any `p` elements whose parent elements are `div`s

<!-- your answer starts here -->
.big {}
#contentPane {}
.important.red {}
p {} //Unless the div has a class name then its ".div p {}"
<!-- your answer ends here -->

## Question 4

Consider the following HTML and CSS code. What text color and font-family values will the div labelled 'specialDiv' have?

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
color: yellow;
font-family: sans-serif;
<!-- your answer ends here -->

## Question 5

Order the following parts of the box model from 'innermost' to 'outermost'.
* content
* border
* margin
* padding

<!-- your answer starts here -->
content
padding
border
margin
<!-- your answer ends here -->

## Question 6

Consider the following HTML and CSS. Assuming that the window is much larger than the dimensions of any of the `divs` given below, how will they be arranged on the page?

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
divTwo divThree divOne
divFour divFive
<!-- your answer ends here -->

## Question 7

Consider the following media queries. How wide would the screen need to be for elements with the class `stretch` to have a width of 150 pixels?
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
600px
<!-- your answer ends here -->
