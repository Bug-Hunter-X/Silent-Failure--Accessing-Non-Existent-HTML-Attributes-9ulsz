# Silent Failure: Accessing Non-Existent HTML Attributes

This repository demonstrates a subtle error in JavaScript when interacting with HTML elements.  Attempting to access a non-existent attribute on an HTML element using JavaScript does not throw an error. Instead, it silently returns `undefined`, which can lead to unexpected behavior and difficult-to-debug issues in your application.

The `bug.html` file showcases this issue. The JavaScript code attempts to access a non-existent attribute (`nonExistentAttribute`) on a div element.  While this does not cause a runtime error, it leads to `undefined` being assigned to `myVar`.

The solution, in `bugSolution.html`, demonstrates safe attribute access using optional chaining or checking for the attribute's existence before attempting to access it.