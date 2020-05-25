# Dice-Game
## What is it?
It is a simple dice game using DOM manipulation.
It is a project of The Complete Web Dev Course
## What did I learn?
** 05/25/2020 **
### I/What is DOM?

**DOM** stands for Document Object Model

- Browser converts an HTML file into DOM. That is, it turns each element of HTML file and their associated elements into **a tree structure** which you can select and manipulate.
- **Document** is an object that contain everything in the HTML file such as **html, head, body**
- An Object have **properties** , something describes the object, and **methods** , things that the object can do.
  - There are setting and getting properties such a **s .innerHTML, .style.color.**
  - Methods are **click(), etc.**

### II/ Script Tags

**There are 3 kinds of scrip tags**

- Inline Script Tag
- Internal Script Tag
- External Script Tag
  - \&lt;script src=&quot;index.js&quot; charset=&quot;utf-8&quot;\&gt;\&lt;/script\&gt;
  - The script tag should be placed at the end of the body element. By doing that, the website looks loading faster to the users, as it is taking more time to run the JS code.

### III/ Selector

1. **Return an array**
  - getElementsByTagName(TagName)
  - getElementsByClassName(className)
  - querySelectorAll(a selector/ a combination of selectors)
2. **Return an item**
  - getElementById(id)
  - querySelector(a selector/ a combination of selectors)

### IV/ Manipulation

1. **Changing Styles**

Selecting the element and Changing the property

Note:

- In CSS, all properties are kabob casing
- In JS, all properties are camel casing
- General syntax

**Element.style.property = newProperty**

**HOWEVER,** for the purpose of separation of concerns, we keep styling for css, content for html, and behavior for js

- Using **classList** property to change the style of elements using JS
- All HTML element has the **classList** property
- We can **add, remove, or toggle class** for **classList** property

Example: Document.querySelector(&quot;h1&quot;).classList.remove(&quot;bigFont&quot;);

1. **Changing HTML Content**

- **InnerHTML** property **get all HTML content, including text and element,** inside the parent element. By using the property, you not only can manipulate the text but also the html code inside the parent HTML element.
- TextContent property **only get text, NOT the HTML code** inside the parent HTML element.

1. **Changing HTML attributes**

- **attributes** property give you an object containing all the attributes of the HTML element.
- **setAttribute(attributeName)** property give you one attribute that matches the attributeName
- **setAttribute(attributeName, newContent)** property allows you to change the content of the attribute that matches the attributeName
