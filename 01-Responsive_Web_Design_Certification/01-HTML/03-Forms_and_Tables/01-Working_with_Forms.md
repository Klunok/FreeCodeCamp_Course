# How Do Forms, Labels, and Inputs Work in HTML?

 Example:
```html
<form action="url-goes-here">
  <!-- input elements go here -->
</form>
```

 The `action` attribute specifies where the form data will be sent upon submission.  
 To collect specific informaiotn, like names and email addreses, the `input` element.  
 Example:
```html
<form action="">
  <input type="text" />
</form>
```
 The `input` elements are void elements and do not have closing tags.  
 The `type` attribute defines the data type expected from the user.  
To add a `label` for the input.
 Example:
```html
<form action="">
  <label>
    Full Name:
    <input type="text" />
  </label>
</form>
```

 By nesting an `input` inside a `label` element, created an implicit association between the `label` and the `input` field. 

 ```html
 <form action="">
  <label for="email"> Email Address: </label>
  <input type="email" id="email" />
</form>
```

if wanted to show additional hints to the users about the expected input, you can use the `placeholder` attribute.  
Example:  
```html
<form action="">
  <label for="email"> Email Address: </label>
  <input type="email" id="email" placeholder="example@email.com" />
</form>
```

# What Are the Different Types of Buttons, and When Should You Use Them?

 The `button` element is used to perform a particular action.  
 Example:
```html
<button>Start Game</button>
```

 The `button` element has a `type` attribute which controls the behavior of the button when it is activated.  
 Example:
```html
<button type="button">Show Alert</button>
```

 Another possible value for the `type` attribute is the `submit` value.  
 Example:
```html
<form action="">
  <label for="email">Email address:</label>
  <input type="email" id="email" name="email" />
  <button type="submit">Submit form</button>
</form>
```

 The `value` attribute is used to show the button text.  
 The `input` element are void, which means they cannot have child nodes, such as text, and can only have a start tag.  

# What Is Client-Side Form Validation in HTML Forms, and What Are Some Examples?

 One common example of build-in form validation is to use the `required` attribute in inputs.  
 The `required` attribute specifies that the user needs to fill out that portion of the form befire it gets submitted. 
 Exapmle:
```html
 <form action="">
  <label for="email">Email Address (Required field):</label>
  <input required type="email" name="email" id="email" />
  <button type="submit">Submit Form</button>
</form>
```

 The `minlength` and `maxlength` attributes are used to set the minimum and maximum length.  
 Example:
```html
<form action="">
  <label for="email">Email Address (Required field):</label>
  <input
    required
    type="email"
    name="email"
    id="email"
    minlength="4"
    maxlength="64"
  />
  <button type="submit">Submit Form</button>
</form>
```

# What Are the Different Form States, and Why Are They Important?

 In HTML, form controls, like inputs, can be in different stages or conditions like a `focused` state, `readonly` state, or `disabled` state.  
 
