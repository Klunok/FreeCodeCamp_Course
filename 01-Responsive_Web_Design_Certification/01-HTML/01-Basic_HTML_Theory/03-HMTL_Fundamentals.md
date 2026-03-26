# What are Div Elements and When Should You Use Them?

## Div
The div element is used as a container to group other elements.
```
<div>
  <p>Example paragraph element.</p>
</div>
```
You will mainly use the div element when you want to group HTML elements that will share a set of CSS styles.

## Section
The section element has semantic meaning over the div element which is not semantic.
```
<section>
  <h2>Mammals</h2>
  <p>
    Mammals are warm-blooded animals with fur or hair. Most give birth to live
    young.
  </p>
  <ul>
    <li>Lion</li>
    <li>Elephant</li>
    <li>Dolphin</li>
  </ul>
</section>
```

In HTML, which is a language, elements have their own semantic meaning too. 
So, this means if you use a section element, the browser will pick up its semantic meaning and understand to treat this as a section - on desktops, mobiles, you name it.

# What Are IDs and Classes, and When Should You Use Them?

The *id* attribute adds a unique identifier to an HTML element.
Below the h1 element, add an h2 element with an id set to "subtitle". You can write whatever text you like for the h2 and you will see the changes in the preview window. To interact with the example, you will need to enable the interactive editor.
```
<h1 id="title">Movie Review Page</h1>
```
NOTE: Some CSS has been provided for you in this interactive example. Don't worry about trying to understand the CSS code because you will learn more about that in future lessons. But if you wanted to change the color of the first and third boxes, enable the interactive editor and click on the styles.css tab and change the background-color: red; to background-color: black;.

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta
       name="viewport"
       content="width=device-width, initial-scale=1.0" />
    <title>Colored boxes example</title>
    <link rel="stylesheet" href="./styles.css" />
  </head>
  <body>
    <div class="box red-box"></div>
    <div class="box blue-box"></div>
    <div class="box red-box"></div>
    <div class="box blue-box"></div>
  </body>
</html>
```

```
.box {
  width: 100px;
  height: 100px;
}

.red-box {
  background-color: red;
}

.blue-box {
  background-color: blue;
}
```

# What Are HTML Entities, and What Are Some Common Examples?

An HTML entity, or character reference, is a set of characters used to represent a reserved character in HTML.

not working
```
<p>This is an <img /> element</p>
```

use the an ampersand sign (&) and end with a semicolon (;)

```
<p>This is an &lt;img /&gt; element</p>
```

# What Is the Role of the Script Element in HTML, and How Can It Be Used to Link to External JavaScript Files?

The script element is used to embed executable code. 

Example of using the script element to link to an external JavaScript file:
```
<script src="path-to-javascript-file.js"></script>
```

Example of using the script element in an HTML document:
**Remove the //**
```
<body>
  <script>
    // alert("Welcome to freeCodeCamp");
  </script>
</body>
```

