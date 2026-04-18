
# How Do You Display Mathematical Equations and Chemical Formulas in HTML?

A superscript is a symbol or letter printed above the normal line of text.

Example:  
```html
<p>2<sup>2</sup> (2 squared) is 4.</p>
2² (2 squared) is 4.
```
# How Do You Represent Computer Code in HTML?

Common use cases for the **code** element would be for technical articles and documentation pages
Example:
```html
<p>
  To set the text color to blue in CSS, use the following code:
  <code>color: blue;</code>
</p>
```

The preformatted text element is used to represent preformatted text.
Example:
```
<pre>
  <code>
    body {
      color: red;
    }
  </code>
</pre>
```

# What Are the U, S, and Ruby Elements Used For, and How Do They Work?

Inline text: ```U```

In HTML4, the u element was used for styling purposes.  
But in HTML5, the u element should only be used to indicate that text has non-textual annotation applied.

Strikethrough element: ```S```

The ```s``` element should never be used just to show changes to a document.  
More appropriate elements in that case would be the deleted text element and the inserted text element.

Small text shown above or below the main text: ```ruby```
Fallback element: ```rb```
