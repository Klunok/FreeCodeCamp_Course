# What Is CSS, and What Is Its Role on the Web?

CSS, which stands for ***Cascading Style Sheets***, is a crucial component of modern web development. It's a markup language used to apply styles for HTML. In simpler terms, if HTML is the structure of a web page, CSS is what makes it look good.
The primary role of CSS is to separate the content of a web page from its visual presentation. This separation allows web developers to create more flexible and maintainable websites.
With CSS, you can control the layout, colors, fonts, and overall visual appearance of web pages without altering the HTML structure.
Cascading means that styles can be inherited and overridden, allowing for a hierarchical structure of styling. You will learn more about how this works in future lessons.
CSS also supports the use of external stylesheets.

# What Is the Basic Anatomy of a CSS Rule?

CSS is responsible for the styles of a web page. All of these styles are made up of various CSS rules.
A CSS rule is made up of two main parts: a selector and a declaration block.

Example:
```
selector {
  property: value;
}
```

A selector is a pattern used in CSS to identify and target specific HTML elements for styling.
Examples of selectors include type selectors, class selectors, and ID selectors.
The curly braces provided in the basic syntax are known as a declaration block. A declaration block applies a set of styles for a given selector, or selectors.
Inside the declaration block, you will have a series of declarations. Each declaration consists of a property and a value.


# What Is the Meta Viewport Element Used For?

Meta Viewport is a special HTML meta element that gives the browser instructions on how to control the page's dimensions and scaling on different devices, particularly on mobile phones and tablets.

Let's take a look at the basic syntax of the meta viewport element:

```
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

This element is typically placed in the ```head``` section of your HTML document. 

The ```width=device-width``` part tells the browser to set the width of the page to match the screen width of the device. This is essential for creating responsive layouts that adapt to different screen sizes.

The ```initial-scale=1.0``` sets the initial zoom level when the page is first loaded. A value of 1.0 means that the page is displayed at 100% zoom, without any scaling.

While it's possible to disable zooming with the ```user-scalable=no attribute``` , it's generally recommended to avoid this for accessibility reasons.

Many users rely on the ability to zoom for better readability, especially those with visual impairments.

Here's an example of what not to do:

```
<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
```

Instead, it's better to design your website to be responsive and readable at different zoom levels, ensuring that all users can comfortably access your content.

# What Are Some Default Browser Styles Applied to HTML?

"Default browser styles" or "user-agent styles" are applied to your web pages even before you write any CSS

These default browser styles provide basic formatting to ensure that HTML elements are displayed in a readable way across all browsers.

# What Are Inline, Internal, and External CSS, and When Should You Use Each One?

 CSS can be applied to a webpage in three main ways: inline, internal, or external.  
 **Inline** CSS is written within an HTML using `style`. 
 Example:
```html
<p style="color: green;">This is an inline-styled paragraph.</p>
```

 **Internal** CCS is written within the `style` tags inside the `head` section of an HTML document.  
 Example:
```html
<head>
  <style> p { color: blue; } </style>
</head>
<body>
  <p>This paragraph is styled using internal CSS.</p>
</body>
```

 **External** CSS is written in a separate `.css` file and linked to the HTML documend using the `link` element in the `head` section.  
 Example:
```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <p>This paragraph is styled using external CSS.</p>
</body>
```

 Element `link` has a `rel` attribute that specifies the relationship between the current document and the linked resource, such as linking to a stylesheet or an external resource.
 The `href` attribute specifies the URL of the linked resource, indicating where tthe resource should be retrived from.

# How Do Width and Height Work?

 In CSS, the `width` and `height` properties are used to control the dimenstions of elements on a webpage.
 Properties can be defined in different units such as pixels `px`, percentages `%`, viewport units `vw`, `vh`, and more.

 The `width`. If do not specify, then the default is set to `auto`.  
 For `div` element, `width: auto` makes it exopand to fill the full width of its parent container.  
 The `height`. Similarly, the height is `auto` by default.
 Example:

```html
<head>
  <style>
    .box {
      width: 100px;
      height: 100px;
      background-color: skyblue
    }
  </style>
</head>
<body>
  <div class="box"></div>
</body>
```

 Example has a `div` element with class named `box`, This element will be occupying `100px` in height and width, whereas the background color will be `shyblue`.  
 Pixels are a fixed-size unit of measurement in CSS, providing precise control over dimensions.  
 The `min-width` property specifies the minimum width an element can be.  
 The `min-heght` property specifies the minimum height an element can be.  
 Example:

```html
<head>
  <style>
    .box {
      width: 50px;
      min-width: 100px;
      height: 50px;
      min-height: 100px;
      background-color: lightcoral;
    }
  </style>
</head>
<body>
  <div class="box"></div>
</body>
```
 The `max-width` property specifies the maximum width an element can be.  
 The `max-heght` property specifies the maximum height an element can be.  
 Example:
```html
<head>
  <style>
    .box {
      width: 200px;
      max-width: 150px;
      height: 200px;
      max-height: 150px;
      background-color: lightgreen;
    }
  </style>
</head>
<body>
  <div class="box"></div>
</body>
```

# What Are the Different Types of CSS Combinators?

 CSS combinators are used to define the relationship between selectors in CSS.  
 They help in selecting elements based on their relationship to other elements, which allows for more precise and efficient styling.
Example:
```html
<link rel="stylesheet" href="styles.css">

<figure>
  <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="Relaxing Cat">
  <figcaption>A relaxing cat with a border</figcaption>
</figure>
figure img {
  border: 4px solid red;
}
```

  The descendant combinator to select all image elements inside figure elements and apply a solid red border on all four sides.  
 The child combinator (`>`) in CSS is used to select elements that are direct children of a specified parent element.  
Example:
```html
<div class="container">
  <p>First</p>
  <div>
    <p>Second</p>
  </div>
  <div>
    <p>Third</p>
  </div>
</div>
```






