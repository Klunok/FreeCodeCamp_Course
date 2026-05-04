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
```html
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
 In above HTML structure, the `container` class is applied to a `div` element.  
 Inside this container, there is a direct child `p` element ("First"), followed by two additional `div` elements, each containing a `p` element ("Second" and "Third").  
 The first `p` element is a direct child of the `.container` element, while the other two `p` elements are nested inside other div elements, making them deeper descendants.  
 To apply styles to just the direct child of the `container` class, you can use the child combinator like this:
```html
<link rel="stylesheet" href="styles.css">

<div class="container">
  <p>First</p>
  <div>
    <p>Second</p>
  </div>
  <div>
    <p>Third</p>
  </div>
</div>

.container > p {
  color: blue;
}
```
 In the above example, only targeting the direct child of `container` class. This will give the direct child the text color of `blue`.
 Because the other two paragraph elements are nested inside `div` elements, they are not considered direct children of the `container` class and will not get the text color of blue.
 The next-sibling combinator (`+`) in CSS selects an element that immediately follows a specified sibling element.  
 This combinator is useful when to apply styles to an element that directly follows another element, allowing for targeted styling based on the element's position relative to its siblings.
Example:
```html
<figure>
  <img
    src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg"
    alt="A cute orange cat lying on its back."
  />
  <figcaption>A cute orange cat lying on its back.</figcaption>
</figure>
```

 Here, we have a figure element containing an `img` element followed by a `figcaption` element.  
 The `figcaption` element is the immediate sibling of the `img` element.

 If you wanted to apply a black border around the `figcaption` element, you can use the next-sibling combinator like this:
```html
<link rel="stylesheet" href="styles.css">

<figure>
  <img
    src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg"
    alt="A cute orange cat lying on its back."
  />
  <figcaption>A cute orange cat lying on its back.</figcaption>
</figure>
img + figcaption {
  border: 4px solid black;
}
```
 In this example, the next-sibling combinator (`+`) selects the `figcaption` element that immediately follows the `img` element. The applied CSS rule adds a `4px solid black border` around the `figcaption`.

## What Is the Difference Between Inline and Block-Level Elements in CSS?

In HTML and CSS, elements are classified as either **inline elements** or **block-level elements**, and this classification dictates how they behave in the document layout.

Understanding this difference is crucial for controlling how your content is displayed on a webpage.

Block-level elements are elements that take up the full width available to them by default, stretching across the width of their container.

These elements always start on a new line and push other content to the next line, creating a "block" of content.

Block-level elements have the CSS property `display: block;` applied by default. This property ensures that the element stretches to fill the container's width and appears on a new line.

Some common block-level elements are `div` elements, paragraphs, headings, ordered lists, unordered lists, and section elements.

Here is a code example of a block-level element:

```html
<p style="border: 2px solid red;">
  First paragraph
</p>
<p>Second paragraph</p>
```

In this example, we have two paragraph elements where the first one has a red border around it.

The two paragraph elements do not share the same line because they are block level elements by default.

So, both paragraph elements will take up the full width of its container, which in this case is the `body` element.

Block-level elements are ideal when you want content to stack vertically, such as paragraphs, sections, or larger blocks of content. They're commonly used to define the layout and structure of a webpage.

Inline elements, unlike block-level elements, only take up as much width as they need and do not start on a new line. These elements flow within the content, allowing text and other inline elements to appear alongside them.

Inline elements have the CSS property `display: inline;` applied by default. This property ensures that the element remains within the flow of the content and does not break onto a new line.

Common inline elements are `span`, `anchor`, and `img` elements.

Here's an example to better understand inline elements:

```html
<p>This is a
  <span style="color: red; border: 2px solid green;">red</span>
  word inside a paragraph.
</p>
```

In this example, we have a `span` element nested inside of a paragraph element. The `span` element has a `red` text color with a `green` border around it so you can see the highlighted word better.

As you can see, the `span` element only takes up as much space as the word "red" and does not push the following content to a new line.

Inline elements are best used for styling smaller portions of text or content within a line, such as emphasizing a word, creating hyperlinks, or applying specific styles to parts of a paragraph.

## How Does Inline-Block Work, and How Does It Differ from Inline and Block Elements?

When working with CSS, you often encounter three different types of display behaviors for elements: `inline`, `block`, and `inline-block`.

Each of these properties affects how elements are positioned and how they interact with other elements on the page.

In this lesson, we will focus on how the `inline-block` property works and how it differs from both inline and block-level elements.

Block-level elements behave like large containers or "blocks" that take up the full width of their parent container. They always start on a new line, and their height and width can be adjusted.

Inline elements only take up as much space as they need. They flow within the surrounding content and do not break onto a new line.

The `inline-block` property is a hybrid of these two behaviors. Like inline elements, `inline-block` elements remain in the text flow without starting on a new line.

However, unlike inline elements, you can adjust the width and height of an `inline-block` element, just as you would with block-level elements.

In short, the key difference between `inline` and `inline-block` is that `inline` elements cannot have their size controlled, whereas `inline-block` elements allow for full control over dimensions while still staying inline with other content.

Let's take a look at an example.

```html
<link href="styles.css" rel="stylesheet">

<div class="container">
  <span class="inline-block-element element1">Inline-Block</span>
  <span class="inline-block-element element2">Inline-Block</span>
</div>
```

```css
.inline-block-element {
  display: inline-block;
  width: 150px;
  height: 100px;
}

.element1 {
  background-color: lightblue;
}

.element2 {
  background-color: lightgreen;
}
```

In the above example, we have a `div` with a class of `container`. Inside that `div` element, we have two `span` elements.

Each of the span elements is set to `display:inline-block` and has a width and height set as well.

The inline-block elements will appear side by side because they behave like inline elements, but they also have a specified width and height, which gives them block-like properties.

But, if you remove the `display: inline-block` property, neither the `height` nor the `width` will be applied even though you defined it clearly.

Here is the revised CSS:

```html
<link href="styles.css" rel="stylesheet">

<div class="container">
  <span class="inline-block-element element1">Span element</span>
  <span class="inline-block-element element2">Span element</span>
</div>
```

```css
.inline-block-element {
  width: 150px;
  height: 100px;
}

.element1 {
  background-color: lightblue;
}

.element2 {
  background-color: lightgreen;
}
```

In this code, we removed the `display: inline-block;` property but kept everything else intact. Here, the `span` elements revert to their default behavior as inline elements.

As a result, the specified width and height are ignored, and the elements only take up the space needed for their content.

Understanding how `inline-block` works is useful because you can use it for creating layouts that require both alignment and dimension control within a continuous text flow.

## What Are Margins and Padding, and How Do They Work?

Margin and padding are essential properties in CSS for creating well-structured, readable, and visually appealing web pages.

Margins control the space outside an element, helping to separate it from other elements and define the layout structure, while padding controls the space inside an element, improving content readability and aesthetic appeal.

To better understand the differences between `margin` and `padding`, let's take a look at some examples.

Here is an HTML example of three paragraph elements on the page:

```html
<p>Paragraph one</p>
<p>Paragraph two</p>
<p>Paragraph three</p>
```

To apply spacing to the top of each paragraph element, you can use the `margin-top` property like this:

```html
<link rel="stylesheet" href="styles.css">

<p>Paragraph one</p>
<p>Paragraph two</p>
<p>Paragraph three</p>
```

```
p {
  margin-top: 20px;
  border: 2px solid black;
}
```

In this example, we are applying `20px` of margin only to the top of each paragraph element.

We also have a solid black border on all four sides so you can see the margin better.

The four different `margin` properties are `margin-top`, `margin-right`, `margin-bottom` and `margin-left`.

Here is an example of using all four properties:

```html
<link rel="stylesheet" href="styles.css">

<span>Paragraph one</span>
<p>Paragraph two</p>
<span>Paragraph three</span>
```

```
p {
  margin-top: 10px;
  margin-right: 20px;
  margin-bottom: 30px;
  margin-left: 40px;
  border: 2px solid black;
}
```

In this example, we are assigning spacing values on all four sides of the paragraph element. A solid black border has also been added so you can see the margins better.

Another way to use the `margin` property is with shorthand notation. You can specify one, two, three, or four values at once. Let’s explore these options together.

When using a singular value on the `margin` shorthand, that exact value will be applied to all four sides of the target element.

Here is an example of using a single value on `margin` shorthand:

```html
<link rel="stylesheet" href="styles.css">

<span>Paragraph one</span>
<p>Paragraph two</p>
<span>Paragraph three</span>
```

```
p {
  margin: 10px;
}
```

This code example will apply `10px` of `margin` equally to all four sides of the paragraph element.

When using two values, the first value applies to the `top` and `bottom`, while the second value applies to the `left` and `right` sides of the element.

Here is an example of using of two values for the `margin` shorthand:

```html
<link rel="stylesheet" href="styles.css">

<span>Paragraph one</span>
<p>Paragraph two</p>
<span>Paragraph three</span>
```

```
p {
  margin: 10px 20px;
}
```

This sets the `top` and `bottom` margins to `10px`, and `20px` for the `left` and `right` margins for the paragraph element.

If three values are provided, the first value applies to the `top` margin, the second value to the `left` and `right` margin, and the third value to the `bottom` margin.

Here is an example to better understand:

```html
<link rel="stylesheet" href="styles.css">

<span>Paragraph one</span>
<p>Paragraph two</p>
<span>Paragraph three</span>
```

```
p {
  margin: 10px 20px 30px;
}
```

This sets the margin to `10px` for the `top`, `20px` for the `left` and `right`, and `30px` for the `bottom`.

When using four values, this gives you more control, as you can independently specify each margin value for each side of the target element.

The first value targets the `top`, the second value targets the `right`, the third value targets the `bottom`, and the fourth value targets the `left`.

Here is an example of using the margin shorthand with four values:

```html
<link rel="stylesheet" href="styles.css">

<span>Paragraph one</span>
<p>Paragraph two</p>
<span>Paragraph three</span>
```

```
p {
  margin: 10px 20px 30px 40px;
}
```

This sets the margin to `10px` for the `top`, `20px` for the `right`, `30px` for the `bottom`, and `40px` for the `left`.

The `padding` property is used to apply space inside the element, between the content and its border.

Like the `margin` property, the four `padding` properties are `padding-top`, `padding-right`, `padding-bottom` and `padding-left`.

Here's an example on how to set the `padding` for a paragraph element:

```html
<link rel="stylesheet" href="styles.css">

<span>Paragraph one</span>
<p>Paragraph two</p>
<span>Paragraph three</span>
```

```
p {
  padding-top: 10px;
  padding-right: 20px;
  padding-bottom: 30px;
  padding-left: 40px;
  border: 2px solid black;
}
```

This sets the padding to `10px` for the `top`, `20px` for the `right`, `30px` for the `bottom`, and `40px` for the `left`.

As you can see that, `padding` is applied to the content which is inside the border, unlike `margin` which applies to outside the border.

Just like the `margin` property, you can also choose to use the shorthand for the `padding` property.

You can either specify one, two, three, or four values on the `padding` shorthand property as well.

Here is an example of using the `padding` shorthand for paragraph element from earlier:

```html
<link rel="stylesheet" href="styles.css">

<span>Paragraph one</span>
<p>Paragraph two</p>
<span>Paragraph three</span>
```

```
p {
  padding: 10px 20px 30px 40px;
  border: 2px solid black;
}
```

In the example, using the shorthand the code will set the padding to `10px` for the `top`, `20px` for the `right`, `30px` for the `bottom`, and `40px` for the `left` of the paragraph element.


