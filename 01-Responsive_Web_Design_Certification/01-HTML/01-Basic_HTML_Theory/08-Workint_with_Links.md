# What Are the Different Target Attribute Types, and How Do They Work?

You may have seen the target attribute on anchor elements, or links. This important attribute tells the browser where to open the URL for the anchor element.
Enable the interactive editor, click on the link and you will be directed to the freeCodeCamp homepage in a new browser tab.
```
<a href="https://freecodecamp.org" target="_blank">Visit freeCodeCamp</a>
```
# What Is the Difference Between Absolute and Relative Paths?

If you are linking to a resource on your local machine, use an absolute path, which includes the full directory location of the file. Here's how to link to the about.html file with an absolute path:
```
<p>
  Read more on the
  <a
    href="/Users/user/Desktop/fCC/script-code/absolute-vs-relative-paths/pages/about.html"
    >About Page</a
    >
</p>
```
Here's an example of an absolute URL that links to the freeCodeCamp logo:
```
<a href="https://design-style-guide.freecodecamp.org/img/fcc_secondary_small.svg">
  View fCC Logo
</a>
```
Here's what the absolute URL looks like in the browser address bar:
```
file:///Users/user/Desktop/fCC/script-code/absolute-vs-relative-paths/pages/about.html
```

Here's the relative URL, an example of linking to the about.html page from the contact.html page, both of which are in the same folder:
```
<p>
  Read more on the
  <a href="about.html">About Page</a>
</p>
```
So, which should you use and when: an absolute path, an absolute URL, or a relative path? Here are the rules you should follow:

- Use absolute paths when you want to reference a resource from a fixed location, such as from the root of your site or a known directory on your local machine;
- Use absolute URL when linking to a resource hosted on an external website.
- Use relative paths when linking to resources within the same website;
- Use relative paths if you want to keep your code cleaner and easier to maintain during development;
- Use relative paths during local testing to ensure links work without an internet connection.

# What Is the Difference Between Slashes, a Single Dot, and Double Dot in Path Syntax?

You may have seen links like /public/logo.png, ./script.js, or ../styles.css before. But what do these special types of links mean? These are called file paths. There are three key syntaxes to know. First is the slash, which can be a backslash (\) or forward slash (/) depending on your operating system. The second is the single dot (.). And finally, we have the double dot (..).

The slash is known as the "path separator". It is used to indicate a break in the text between folder or file names. This is how your computer knows that naomis-files/ points to a directory of that same name, while naomis/files/ points to a files directory in the naomis directory.

# What Are the Different Link States, and Why Are They Important?

The first is the default state, which is ```:link```. This state represents a link which the user has not visited, clicked, or interacted with yet. 
The second state is ```:visited```, which applies when a user has already visited the page being linked to. 
The third state is ```:hover```. This state applies when a user is hovering their cursor over a link.
And finally, we have ```:active```. This state applies to links that are being activated by the user.
