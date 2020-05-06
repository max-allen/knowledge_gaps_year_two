
resources  
[bholts notes from FEM course](https://btholt.github.io/intro-to-web-dev-v2/dom)  
[browsers link from dev roadmap](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/)  
[Using the W3C DOM Level 1 Core](https://developer.mozilla.org/en-US/docs/Web/API/Document_object_model/Using_the_W3C_DOM_Level_1_Core)  
[DOM Level 1 Core specification from W3C](https://developer.mozilla.org/en-US/docs/Web/API/Document_object_model/Using_the_W3C_DOM_Level_1_Core)  
[Whitespace in the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Whitespace)

Definitions (both MDN Web Docs)
* Object model for changing content tree of documents.
* Programming interface for HTML and XML documents.
  It represents the page so programs can change the document structure,
  style, and content.
* Object-oriented representation of the web page, which can be modified
  with a scripting language like JavaScript.

Any HTML / XML document is a tree structure.  
Representing the structure of a document in memory.  
Each branch ends in a node and each node contains objects.  
DOM methods allow programmatic access to the tree.

```html
<html>
<head>
  <title>My Document</title>
</head>
<body>
  <h1>Header</h1>
  <p>Paragraph</p>
</body>
</html>
```

![the tree](https://developer.mozilla.org/@api/deki/files/415/=Using_the_W3C_DOM_Level_1_Core-doctree.jpg)

### What does DOM Level 1 Core allow me to do?

Change the content tree any way you want, programmatically! In JavaScript, this is accessible via the `document`
property on the global object. The `document` object is the implementation of the `Document interface` from the spec.