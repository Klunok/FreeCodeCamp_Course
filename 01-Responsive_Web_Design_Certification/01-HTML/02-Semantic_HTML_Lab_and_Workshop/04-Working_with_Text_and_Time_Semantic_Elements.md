# How Do Block and Inline Quotes Work in HTML?
In HTML, quoted elements are used to distinguish quoted text from the surrounding content. This gives the quoted text a format that is easy to identify.

If the source of the quote has an address, you can ```cite``` it with the cite attribute. The value of this attribute should be a valid URL.
Example:
```html
<blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
  "Can you imagine what it would be like to be a successful developer? To have built software systems that people rely upon?"
</blockquote>
```

Blockquote element.
Example:
```html
<blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
  <p>Build your projects. Show them to your friends. Build projects for your friends.</p>
  <p>Build your network. Help the people you meet along the way. What goes around comes around. You'll get what's coming to you.</p>   
  <p>It is not too late. Life is long.</p>
  <p>You will look back on this moment years from now and be glad you made a move.</p>
</blockquote>
```

# How Do You Display Abbreviations in HTML?

There are two common forms of abbreviations: acronyms and initialisms.

An acronym is a word formed from the initial letters of a phrase, with each letter representing the first letter of a word in that phrase.

GUI is an example of an acronym. It stands for Graphical User Interface. By taking the first letters of each word G, U, and I, you get the acronym GUI.

An initialism is formed from the initial letters of a phrase, with each letter representing the first letter of a word in that phrase.

Here's an example where you can see a paragraph with the sentence ```HTML is the foundation of the web```:

```
<p><abbr>HTML</abbr> is the foundation of the web.</p>
```
# How Do You Display Addresses in HTML?

Example of the ```address``` element for a company contact page:

```html
<address>
  <h2>Company Name</h2>
  <p>
    1234 Elm Street<br />
    Springfield, IL 62701<br />
    United States
  </p>
  <p>Phone: <a href="tel:+15555555555">+1 (555) 555-5555</a></p>
  <p>Email: <a href="mailto:contact@company.com">contact@company.com</a></p>
</address>
```
# How Do You Display Times and Dates in HTML?

The ```time``` element is used to represent a specific moment in time.

The ```datetime``` attribute is used to translate dates and times into a machine-readable format.

The value for the ```datetime``` attribute is in the ISO 8601 format. ISO 8601 is an international standard to represent dates and times.



