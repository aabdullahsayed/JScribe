
**Exercise 1: Inline Script (For small, single-page scripts)**
The first exercise involves placing your JavaScript directly into your HTML file. To ensure the HTML content loads before the script runs, you should **place the `<script>` tags right at the bottom of your content, just before the closing `</body>` tag**. 

```html
<!DOCTYPE html>
<html>
<head>
    <title>My Web Page</title>
</head>
<body>
    <!-- Your web page content loads here first -->
    <h1>Welcome to my page</h1>

    <!-- The script is placed at the bottom -->
    <script>
        alert("Hello!"); // The alert pops up after the page content loads
    </script>
</body>
</html>
```

**Exercise 2: External Script (For larger scripts or multiple pages)**
If you have a larger script (10+ lines) or want to use the same script across multiple pages, the tutorial demonstrates **moving the code into an external file**. 

**Step 1:** Create a new file called `test.js`.
**Step 2:** Paste your JavaScript code directly into this file **without** any `<script>` tags, because the browser already knows it is a JavaScript file due to the `.js` extension.

`test.js`:
```javascript
alert("Hello!");
```

**Step 3:** Link to this external file in your HTML document. Similar to the first exercise, you **put this link down at the bottom of the body tag** using the `src` attribute.

`index.html`:
```html
<!DOCTYPE html>
<html>
<head>
    <title>My Web Page</title>
</head>
<body>
    <!-- Your web page content -->
    <h1>Welcome to my page</h1>

    <!-- Linking the external test.js file at the bottom -->
    <script src="test.js"></script>
</body>
</html>
```

*(Note: The exact text inside the `alert()` function is not specified in the source transcript, so a placeholder like `"Hello!"` is used to complete the exercise structure.)*


## Exercise 2: External Script (For larger scripts or multiple pages)

If you have a larger script (10+ lines) or want to use the same script across multiple pages, the tutorial demonstrates moving the code into an external file.

**Step 1:** Create a new file called `test.js`.

**Step 2:** Paste your JavaScript code directly into this file without any `<script>` tags, because the browser already knows it is a JavaScript file due to the `.js` extension.

**`test.js`**:
```javascript
alert("Hello!");
```

**Step 3:** Link to this external file in your HTML document. Similar to the first exercise, you put this link down at the bottom of the body tag using the src attribute.

`index.html`:
```html
<!DOCTYPE html>
<html>
<head>
    <title>My Web Page</title>
</head>
<body>
    <h1>Welcome to my page</h1>

    <script src="test.js"></script>
</body>
</html>
```

