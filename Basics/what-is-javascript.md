# What is JavaScript?


## Javascript

JavaScript is a high-level, dynamic, interpreted programming language that is commonly used on web pages to create a responsive, interactive experience for users. JavaScript can be used to add functionality to a website, produce visually appealing animations, and validate forms. It is an essential building block for creating modern web applications and is supported by all modern web browsers.

JavaScript code can be written directly in an HTML document using a script tag, or it can be contained in a separate file and linked to the HTML document. JavaScript code can be executed on both the client side (in the user's web browser) and the server side (on the web server).

Here's an example of how JavaScript can be used to change the text color of a website:

```html
<head> 
<script>
  function changeColor() { 
    var x = document.getElementById("myText"); 
    x.style.color = "red"; 
  } 
</script> 
</head> 
<body>
  <h1 id="myText" onclick="changeColor()">Hello World!</h1> 
</body>
```

In this example, the JavaScript code creates a function that changes the color of the h1 element to red when it is clicked. The onclick attribute in the HTML calls the changeColor() function when the h1 element is clicked.

## Key Takeaways

- JavaScript is a high-level, dynamic, interpreted programming language used to create responsive, interactive web pages.
    
- JavaScript can be executed on both the client side and server side.
    
- JavaScript is essential for creating modern web applications and is supported by all modern web browsers.

[Next](where-is-javascript-used.md)