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
That the internet is composed of clients making requests using http verbs of servers using a defined protocol (http) and the servers process the requests, do something with the request, and then respond to the client request with a predefined
response number and any data requested (if everything goes OK)

## Question 2

Between the comments below, write HTML to create a basic web page (using the format described in the instructions). The page should have a title in the head and an unordered list (with three items) inside the body.

```HTML
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Diagnostic Page</title>
  </head>
  <body>
    <ul>
      <li>Diag</li>
      <li>Nos</li>
      <li>Tic</li>
    </ul>
  </body>
</html>
```

## Question 3

What selectors could we write to reference each of the following categories of elements?
* All elements that belong to the class `big`
* The element matching ID `contentPane`
* Only those elements belonging to both the `important` and `red` classes
* All `p` elements whose parent elements are `div`s

```CSS
.big {}
#contentPane {}
.important.red {}
div > p {}
```

## Question 4

Consider the following HTML and CSS code. What text color and font-family values will the div labeled 'specialDiv' have?

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

Yellow cursive that is unreadable on a white background.

## Question 5

Order the following parts of the box model from 'innermost' to 'outermost'.
* content
* border
* margin
* padding

1. content
2. padding
3. border
4. margin

## Question 6

Consider the following HTML and CSS. Assuming that the window is much larger than the dimensions of any of the `div`s given below, how will each `div` be arranged on the page?

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

divTwo divThree                       divOne
divFour divFive

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

600px
