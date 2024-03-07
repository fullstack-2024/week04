# Activity 9: 

### Part 1:

1. **Setting Up the Lab**:
   - Open Visual Studio Code on your computer.
   - Create a new folder named `week4-lab9a`.
   - Inside the `week4-lab9a` folder, create a file named `index.html`.

2. **DOM Events Example**:
   - Open `index.html` in Visual Studio Code.
   - Paste the following code to demonstrate DOM events:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Week 4 Lab 9a: DOM Events</title>
</head>
<body>
    <h2>DOM Events</h2>
    <button id="btn">Click me</button>
    <p id="output"></p>

    <script>
        // Get the button and output element
        const btn = document.getElementById('btn');
        const output = document.getElementById('output');

        // Add event listener for 'click' event
        btn.addEventListener('click', function() {
            output.textContent = 'Button clicked!';
        });
    </script>
</body>
</html>
```

3. **Running the Lab**:
   - Save the `index.html` file.
   - Open the file in a web browser by right-clicking on the file and selecting "Open with Live Server" if you have the Live Server extension installed in Visual Studio Code.
   - Alternatively, you can simply open the HTML file in any web browser by double-clicking on it.

4. **Observation**:
   - Click the button labeled "Click me".
   - Observe the text displayed below the button.
   - Notice how the text changes to "Button clicked!" when the button is clicked due to the event listener attached to the button.

### Part 2:

1. **Setting Up the Lab**:
   - Open Visual Studio Code on your computer.
   - Create a new folder named `week4-lab9b`.
   - Inside the `week4-lab9b` folder, create two files named `index.html` and `script.js`.

2. **DOM Events Example**:
   - Open `index.html` in Visual Studio Code.
   - Paste the following code to link the external JavaScript file:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Week 4 Lab 9b: DOM Events (External JavaScript)</title>
</head>
<body>
    <h2>DOM Events (External JavaScript)</h2>
    <button id="btn">Click me</button>
    <p id="output"></p>

    <!-- Link the external JavaScript file -->
    <script src="script.js"></script>
</body>
</html>
```

   - Create a file named `script.js` in the same directory.
   - Paste the following JavaScript code into `script.js` to handle the DOM event:

```javascript
// Get the button and output element
const btn = document.getElementById('btn');
const output = document.getElementById('output');

// Add event listener for 'click' event
btn.addEventListener('click', function() {
    output.textContent = 'Button clicked!';
});
```

3. **Running the Lab**:
   - Save both `index.html` and `script.js` files.
   - Open the `index.html` file in a web browser by right-clicking on the file and selecting "Open with Live Server" if you have the Live Server extension installed in Visual Studio Code.
   - Alternatively, you can simply open the HTML file in any web browser by double-clicking on it.

4. **Observation**:
   - Click the button labeled "Click me".
   - Observe the text displayed below the button.
   - Notice how the text changes to "Button clicked!" when the button is clicked due to the event listener attached to the button.

**Conclusion**:
Through this part, you have learned how to use external JavaScript files to handle DOM events in web development. By linking an external JavaScript file to an HTML document, you can keep your code organized and modular, making it easier to maintain and update. DOM events allow you to add interactivity to web pages, enhancing the user experience and creating dynamic content.

### Part 3: Local Git Repository

1. Make the project directory a Git repository by running:

```bash
git init
```

<!-- 2. Make sure that you have the `.gitignore` file and exclude the `node_modules` directory from version control:

```
node_modules/
``` -->

2. Stage all the changes:

```bash
git add .
```

3. Commit the changes:

```bash
git commit -m  "Add message here"

```

### Part 4: Push to GitHub

1. Create a new repository on GitHub:

- Go to the GitHub website .
- Click on the plus sign icon in the top right corner of the page, and then select "New repository."
- Fill in the details for your new repository:
   - Repository name: Choose a name for your new repository.
   - Description (optional): Add a short description to explain the repository's purpose.
   - Visibility: Choose between "Public" or "Private," depending on who should have access.
   - Do not initialize the repository with a `README` file or a `.gitignore` file.
- Click the "Create repository" button to create your new repository.


2. Link your local repository to the GitHub repository:

```bash
git remote add origin <GitHub Repository URL>
```

3. Push your local repository to GitHub:

```bash
git push -u origin main
```

4. Refresh the GitHub repository page to see your changes.

