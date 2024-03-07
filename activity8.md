# Activity 8: 

### Part 1:

1. **Setting Up the Lab**:
   - Open Visual Studio Code on your computer.
   - Create a new folder named `week4-lab8`.
   - Inside the `week4-lab8` folder, create a file named `index.html`.

2. **HTML Attribute Example**:
   - Open `index.html` in Visual Studio Code.
   - Paste the following code to demonstrate the HTML attribute approach:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Week 4 Lab 8: HTML Attribute vs DOM Property</title>
</head>
<body>
    <h2>HTML Attribute</h2>
    <input value="Click me" onclick="alert('Click!')" type="button">
</body>
</html>
```

3. **DOM Property Example**:
   - Below the HTML code, add a `<script>` tag to include JavaScript code.
   - Paste the following JavaScript code to demonstrate the DOM property approach:

```javascript
<script>
    const elem = document.createElement('input');
    elem.type = 'button';
    elem.value = 'Click me';
    elem.onclick = function() {
        alert('Thank you');
    };
    document.body.appendChild(elem);
</script>
```

4. **Running the Lab**:
   - Save the `index.html` file.
   - Open the file in a web browser by right-clicking on the file and selecting "Open with Live Server" if you have the Live Server extension installed in Visual Studio Code.
   - Alternatively, you can simply open the HTML file in any web browser by double-clicking on it.

5. **Observation**:
   - Compare the behavior of the button created using HTML attribute (`onclick` attribute) with the one created using DOM property (`elem.onclick` assignment).
   - Notice how the button behaves differently despite having the same visual appearance.

### Part 2: Local Git Repository

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

### Part 3: Push to GitHub

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

