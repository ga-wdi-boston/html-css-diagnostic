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

<!-- your answer ends here -->

## Question 2
Below, write some HTML to create a basic web page. It should have a title in the head and an unordered list (with three items) inside the body.
<!-- your answer starts here -->

<!-- your answer ends here -->

## Question 3
What are the three ways we can add CSS to an HTML document? Which will we use most often?
<!-- your answer starts here -->

<!-- your answer ends here -->

## Question 4
What selectors could we write to select each of the following categories of elements?
* All elements that belong to the class `big`
* The element matching ID `contentPane`
* Any elements that belong both to the `important` and `red` classes
* Any `p` elements whose parent elements are `div`s

<!-- your answer starts here -->

<!-- your answer ends here -->


## Question 5
Consider the following HTML and CSS code. What color and font-family values will the div 'specialDiv' have?
**index.html**
```HTML
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" type="text/css" href="assets/css/main.css">
</head>
  <div class="things">
    <div id="specialDiv" style="font-family: cursive">
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
#specialDiv {
  color: yellow;
  font-family: sans-serif;
}
.things {
  font-family: arial;
}
.things div {
  color: red;
  font-size: 16px;
}
```

<!-- your answer starts here -->

<!-- your answer ends here -->

## Question 6
Order the following spaces from innermost to outermost, according to the box model:
* content
* border
* margin
* padding

<!-- your answer starts here -->

<!-- your answer ends here -->

## Question 7
Of `em`, `px`, and `%`, which would we probably use for elements of fixed size? Which would we probably use to appropriately scale div dimensions? Which would we probably use to appropriately scale font size and text?

<!-- your answer starts here -->

<!-- your answer ends here -->

## Question 8
Consider the following HTML and CSS. Assuming that the window is much larger than the dimensions of any of the `divs` given below, how will they be arranged on the page?
**index.html**
```HTML
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" type="text/css" href="assets/css/style.css">
</head>
<body>
  <div id="divOne"></div>
  <div id="divTwo"></div>
  <div id="divThree"></div>
  <div id="divFour"></div>
  <div id="divFive"></div>
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

#divOne {
  float: right;
}

#divFour {
  clear: left;
}
```

<!-- your answer starts here -->

<!-- your answer ends here -->
