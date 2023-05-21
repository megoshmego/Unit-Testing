Important terms and ideas:

1. Jasmine: A JavaScript testing framework that allows you to write and run tests for your code.
2. CDN (Content Distribution Network): A network of servers that delivers web content, such as scripts and CSS files, to users based on their geographic location, providing faster and more efficient access to resources.
3. Jasmine Standalone: A standalone version of the Jasmine framework that includes the necessary JavaScript files and CSS for testing.
4. CSS (Cascading Style Sheets): A style sheet language used for describing the look and formatting of a document written in HTML.
5. Spec: A term used in Jasmine to refer to a test case or a unit of code being tested.
6. Test Interface: The user interface provided by Jasmine that displays the status and results of your tests.
7. Best Practice: A recommended approach or methodology that is considered the most effective or efficient in a given context.

Code snippets:

1. Including Jasmine CSS:
```html
<head>
  <link rel="stylesheet" href="path/to/jasmine.css">
</head>
```

2. Including Jasmine Scripts:
```html
<body>
  <!-- Include Jasmine scripts -->
  <script src="path/to/jasmine.js"></script>
  <script src="path/to/jasmine-html.js"></script>
  <script src="path/to/boot.js"></script>
</body>
```

3. Writing Tests in Separate File:
```javascript
// taxes.js
function calculateTaxes(income) {
  // Function implementation
}

// taxes.test.js
// Include the taxes.js script first

// Write your tests here
describe('calculateTaxes', function() {
  it('should calculate taxes correctly', function() {
    // Test case code
  });
});
```

These code snippets demonstrate how to include Jasmine CSS and scripts in your HTML file, as well as how to write tests in a separate file using Jasmine's `describe` and `it` functions.