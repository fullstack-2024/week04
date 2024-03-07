# Activity 7: 

### Part 1:

This part illustrates the usage of `getElementById`, `querySelectorAll`, and `querySelector` methods for DOM manipulation.

0. **Setup**

- **Create the Folder**:
   - Launch Visual Studio Code on your computer.
   - Click on "File" in the top menu.
   - Select "Open Folder...".
   - Choose the directory where you want to create the `week4-lab7` folder.
   - Click on "New Folder" icon in the Explorer pane.
   - Name the folder `week4-lab7`.

- **Create Files**:
   - Right-click on the `week4-lab7` folder in the Explorer pane.
   - Select "New File".
   - Name the file `index.html`.
   - Repeat the same steps to create another file named `script.js`.

- **Add Content**:
   - Open `index.html` file by double-clicking on it in the Explorer pane.
   - Paste the following content into `index.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Week 4 Lab 7</title>
</head>
<body>
    <h1>Hello from Week 4 Lab 7!</h1>
    <script src="script.js"></script>
</body>
</html>
```

   - Open `script.js` file by double-clicking on it in the Explorer pane.
   - Paste the following content into `script.js`:

```javascript
// JavaScript code for Week 4 Lab 7
console.log("Hello from script.js!");
```


1. Replace the content of `index.html` with the following:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DOM Manipulation Lab</title>
    <style>
        /* CSS styles for demonstration */
        .highlight {
            background-color: yellow;
        }
    </style>
</head>
<body>
    <h1>DOM Manipulation Lab</h1>
    <div id="content">
        <p id="paragraph1">This is paragraph 1.</p>
        <p class="paragraph">This is paragraph 2.</p>
        <span>This is a span element.</span>
    </div>
    <ul>
        <li class="list-item">List item 1</li>
        <li>List item 2</li>
        <li class="list-item">List item 3</li>
    </ul>
    <script src="script.js"></script>
</body>
</html>
```

2. Replace the content of `script.js` with the following:

```javascript
// Selecting elements using getElementById
const paragraph1 = document.getElementById('paragraph1');
paragraph1.textContent = 'This paragraph is selected using getElementById.';
paragraph1.style.color = 'blue';

// Selecting elements using querySelectorAll
const listItems = document.querySelectorAll('.list-item');
listItems.forEach(item => {
    item.textContent += ' (Selected using querySelectorAll)';
    item.classList.add('highlight');
});

// Selecting the first paragraph element using querySelector
const firstParagraph = document.querySelector('p');
firstParagraph.textContent += ' (Selected using querySelector)';
```   

3. **Running the Lab**:
   - Open `index.html` in a web browser.
   - Inspect the web page to see the changes made by JavaScript.
   - Verify that elements are selected and manipulated as expected.

### Explanation:

- In the HTML file, we have a simple structure with paragraphs, spans, and list items. Some elements have `id` or `class` attributes for selection.
- In the JavaScript file, we demonstrate the usage of `getElementById`, `querySelectorAll`, and `querySelector` methods.
- We select an element with the `id` of `paragraph1` using `getElementById` and modify its text content and style properties.
- We select all list items with the class `list-item` using `querySelectorAll`, iterate through them, and modify their text content and apply a CSS class for highlighting.
- We select the first paragraph element using `querySelector` and modify its text content.


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

