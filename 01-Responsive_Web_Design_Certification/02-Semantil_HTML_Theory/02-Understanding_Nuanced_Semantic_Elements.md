# When Should You Use the Emphasis Element Over the Idiomatic Text Element?

These elements are very closely related to the concepts of presentational and semantic HTML. The idiomatic text element, ```i```, was originally used for presentational purposes to display the text in italics. But now, it is frequently used for highlighting alternative voice or mood, idiomatic terms from another language, technical terms, and thoughts.
The ```lang``` attribute inside the open ```<i>``` tag is used to specify the language of the content. In this case, the language would be French. 
This is an example of the emphasis element within a paragraph.

```
<p>
  Never give up on <em>your</em> dreams.
</p>
```
# When Should You Use the Strong Element Over the Bring Attention To Element?

The "bring attention to" element, ```b```, is commonly used to highlight keywords in summaries, or product names in reviews. Usually, browsers display this text in boldface. Here's an example using the ```b``` element to highlight product names in this review:

```
<p>
  We tested several products, including the <b>SuperSound 3000</b> for audio
  quality, the <b>QuickCharge Pro</b> for fast charging, and the
  <b>EcoClean Vacuum</b> for cleaning. The first two performed well, but the
  <b>EcoClean Vacuum</b> did not meet expectations.
</p>
```

If you need to emphasize the importance of the text, you should use the ```strong``` element instead of the ```b``` element.

strong is a semantic HTML element that emphasizes text that is crucial, or urgent. This is an example where the strong element is used to label a very important warning about the potential allergic reactions that customers may have to a product:

```
<p>
  <strong>Warning:</strong> This product may cause allergic reactions.
</p>
```
# What Are Description Lists, and When Should You Use Them?
Description lists are perfect for presenting terms and definitions in an organized and easy-to-read format, like in a glossary, or real dictionary, where you can find words with their corresponding definitions.

```
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
  <!-- <dt>JS</dt>
  <dd>JavaScript</dd> -->
</dl>
```



