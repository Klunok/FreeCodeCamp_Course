# Why Should You Care About Semantic HTML?

Using correct semantic elements can improve your development experience. Rather than having to sift through a bunch of developments to find your navigation bar, you can edit the nav element directly and know what you're changing. Throughout this section, you will learn more about these topics, how to use semantic elements, and why semantic HTML is so important.

# Why is it Important to Have Good Structural Hierarchy?

The most important aspect of creating a structural hierarchy is the proper use of heading elements. Heading elements are numbered as ```h1```, ```h2```, ```h3```, and so on. These numbers represent the heading level for that element.

```html
<section>
  <h1>freeCodeCamp</h1>
  <h2>Learn Front-End Development</h2>
  <h2>Learn Back-End Development</h2>
</section>
```
# What Is the Difference Between Presentational and Semantic HTML?

Many presentational HTML elements are deprecated, which means that they are outdated and no longer recommended. There are better ways to get the same results. However, it is helpful to know that they exist, so we'll take a look at some examples.

Enable the interactive editor and add center tags around the <p>Another example text.</p> to see it centered on the page.

```html
<center>
  This text is centered.
  <p>HTML is awesome.</p>
</center>
<p>Another example text.</p>
```

Enable the interactive editor and add big tags around the Some other text and see the changes in the preview window.

```html
<p>
  This text has a normal font size.
  <big>This text is larger.</big>
  Some other text.
</p>
```

Remember that font size should always be set with CSS, so you should not use this element in modern HTML.

Examples of semantic HTML elements include:
- The header element for defining the header of the document, or section.
- The navigation section element, nav, for sections with navigation links.
- The section element for grouping related information.
- The figure element for illustrations and diagrams.

The semantic elements clearly show their purpose within the HTML structure. There are many different semantic HTML elements. You will definitely find one that fits the needs of your project.

