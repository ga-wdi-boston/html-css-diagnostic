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
The Web provides a service to access information over the Internet. It is built on top of the Internet.

## Question 2

Between the comments below, write HTML to create a basic web page (using the format described in the instructions). The page should have a title in the head and an unordered list (with three items) inside the body.
<!DOCTYPE html>
  <html>
    <head>
    <!-- Meta-data goes here. -->
    <title>html Diagnostic</title>
    </head>
    <body>
    <ul>
    <li>One</li>
    <li>Two</li>
    <li>Three</li>
    </ul>
      <!-- Page content goes here. -->
    </body>
  </html>

## Question 3

What selectors could we write to reference each of the following categories of elements?
* All elements that belong to the class `big`
  .big{
  }
* The element matching ID `contentPane`
  #contentPane{

  }
* Any elements that belong both to the `important` and `red` classes
  .important, .red{

  }
* Any `p` elements whose parent elements are `div`s
  div > p{

  }


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

specialDiv will have red color text in cursive font-family.

## Question 5

Order the following parts of the box model from 'innermost' to 'outermost'.
* content - 1
* padding - 2
* border -3
* margin - 4


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

It would look like below:
[divTwo][divThree][divFive][divOne]
[divFour]

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
Screen needs to be 1200px
