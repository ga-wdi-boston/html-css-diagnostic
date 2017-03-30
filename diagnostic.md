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

<!-- your answer starts here -->
```HTML
<html>
  <head>
    <meta charset="utf-8">
    <title>Restaurant Website</title>
  </head>
  <body>
    <ul>
      <li>Breakfast Menu
      <li>Lunch Menu
      <li>Dinner Menu
    </ul>
  </body>
</html>
```
<!-- your answer ends here -->

## Question 2

How would we reference each of the following categories of elements?

-   All elements that belong to the _class_ `big`
-   The element matching _ID_ `contentPane`
-   Only those elements belonging to both the `important` and `red` _classes_
-   All `p` elements whose parent elements are `div`s

<!-- your answer starts here -->
-   All elements that belong to the _class_ `big`
```CSS
.big {

}
```
-   The element matching _ID_ `contentPane`
```CSS
#contentPane {

}
```

-   Only those elements belonging to both the `important` and `red` _classes_
```CSS
.important.red {

}
```

-   All `p` elements whose parent elements are `div`s
We would need to assign a class to all of those p elements whose parent elements are divs. Let's say that class is called '.pdivs'. Then, we would reference those elements using the following code:
```CSS
.pdivs {

}
```
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

<!-- your answer starts here -->
The div labeled 'specialDiv' will have a text color of yellow and a font family of sans-serif.
<!-- your answer ends here -->

## Question 4

Order the following parts of the _box model_ from **'innermost'** to
**'outermost'**.

content, border, margin, padding

<!-- your answer starts here -->
1. Content (innermost)
2. Padding
3. Border
4. Margin (outermost)
<!-- your answer ends here -->

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

<!-- your answer starts here -->
First, I placed values into the divs so that I could run this code and see what rendered on the page. I placed in dummy values "div1", "div2", "div3", "div4", and "div5".

Then, I ran the HTML and CSS code. The output looked like this:
|div2div3                            div1|
|div4div5                                |

div2 and div3 are in the top left hand corner of the page. div1 is in the top right hand corner of the page. div 4 and div5 are directly below div2 and div3.
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

<!-- your answer starts here -->
At 550px, an element with the class '.stretch' will be 30%. Any width less than 800px and creater than 400px will trigger the media query for a width of 30%. 550px * 30% = 165px.
<!-- your answer ends here -->
