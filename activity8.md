#



### Push to GitHub

- Local Git Repository
  - Make the project directory a Git repository by running:
    ```bash
    git init
    ```
   - Create a `.gitignore` file to exclude `node_modules`  file from version control:

    ```
    node_modules/
    ```
  - Stage all the changes:

    ```bash
    git add .
    ```
  - Commit the changes:
    ```bash
    git commit -m  "meaningful message"
    ```

- Push to GitHub
  - Create a new repository on GitHub
  - Link your local repository to the GitHub repository:
    ```bash
    git remote add origin <GitHub Repository URL>
    ```
  - Push your local repository to GitHub:
    ```bash
    git push -u origin main
    ```