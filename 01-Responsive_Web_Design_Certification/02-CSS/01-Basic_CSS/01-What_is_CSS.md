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




