# Activity 1: Git Basics

## Part 1/3: Introduction to Git Basics: Local Repository

In this task, you will install Git, configure it with your name and email. Please follow these [instructions](./git.md)


### Objective: 

To familiarize beginners with the fundamental Git commands and workflow including `git init`, `git add`, `git commit`, and `git status`.

### Steps:

1. **Setting Up Your Workspace in Visual Studio Code:**
   - Open Visual Studio Code (VSCode).
   - Navigate to the directory where you want to create your Git repository in the VSCode file explorer.
   - Right-click on the desired directory to open the context menu.
   - Select "Open in Terminal" from the context menu to launch the integrated terminal within VSCode.
   - The terminal will open with the current directory set to the selected directory, allowing you to proceed with initializing your Git repository.

2. **Initializing a Git Repository:**
   - Once you're in the desired directory, initialize a new Git repository using the `git init` command:
     ```
     git init
     ```
   - This command creates a new Git repository in the current directory.

3. **Creating a Sample File:**
   - Create a new text file named `sample.txt`.
   - Add some content to the file.

4. **Checking the Status:**
   - Use the `git status` command to see the current status of your repository:
     ```
     git status
     ```
   - This command shows you which files are tracked, untracked, modified, or staged for commit.

5. **Staging Changes:**
   - To stage changes for commit, use the `git add` command followed by the filename. For example, to stage `sample.txt`:
     ```
     git add sample.txt
     ```
   - Alternatively, you can use `git add .` to stage all changes in the directory:
     ```
     git add .
     ```

6. **Committing Changes:**
   - Once you've staged your changes, commit them to the repository using the `git commit` command:
     ```
     git commit -m "Initial commit"
     ```
   - The `-m` flag allows you to include a commit message. Make sure your commit message is descriptive and concise.

7. **Viewing the Status Again:**
   - After committing your changes, use `git status` once more to verify that your working directory is clean:
     ```
     git status
     ```

8. **Conclusion:**
   - You've successfully initialized a Git repository, staged changes, and committed them. You're now ready to continue working with Git and managing your project's version control.

Additional Notes:
- Remember that Git tracks changes to files, not the files themselves. This means you need to explicitly add files to the staging area using `git add` before committing them.
- Regularly using `git status` helps you keep track of the state of your repository and what changes still need to be staged or committed.


## Part 2/3: Adding Multiple Files to Your Git Repository

### Objective:

To understand how to add multiple files to a Git repository using the `git add .` command.

### Steps:

1. **Open Visual Studio Code and Integrated Terminal:**
   - Launch Visual Studio Code (VSCode).
   - Open the directory where your Git repository is located using the VSCode file explorer.
   - Right-click on the directory to open the context menu.
   - Select "Open in Terminal" from the context menu to open the integrated terminal within VSCode.
   - Once you're in the desired directory, initialize a new Git repository using the `git init` command:
     ```
     git init
     ```
   - This command creates a new Git repository in the current directory.   

2. **Create Three Sample Files:**
   - Inside the directory, create three new text files using any text editor available in VSCode.
   - Name the files `file1.txt`, `file2.txt`, and `file3.txt`.
   - Add some content to each file.

3. **Check Repository Status:**
   - In the integrated terminal, use the `git status` command to check the status of your repository:
     ```
     git status
     ```
   - This command will display the current status of your repository, showing which files are untracked.

4. **Stage Changes:**
   - To stage all changes in the directory for commit, use the `git add .` command:
     ```
     git add .
     ```
   - This command stages all new and modified files in the current directory and its subdirectories.

5. **Verify Staging:**
   - Use the `git status` command again to verify that all changes have been staged successfully:
     ```
     git status
     ```
   - The output should indicate that the files you created (`file1.txt`, `file2.txt`, and `file3.txt`) are now staged for commit.

6. **Commit Changes:**
   - Commit the staged changes to the repository with a descriptive commit message:
     ```
     git commit -m "Added three sample files"
     ```
   - Ensure that your commit message is informative and describes the changes you've made.

7. **View Repository Status Again:**
   - Once the changes are committed, use `git status` to verify that your working directory is clean:
     ```
     git status
     ```
   - The output should indicate that there are no uncommitted changes in your repository.

8. **Conclusion:**
   - You've successfully added multiple files to your Git repository using the `git add .` command. You can now continue working on your project with version control enabled.

Additional Notes:
- Utilizing `git add .` allows you to efficiently stage multiple files for commit without having to specify each file individually.
- Remember to regularly use `git status` to keep track of the state of your repository and ensure that your changes are being managed effectively.

## Part 3/3: Exploring Git Workflow 

### Objective:

To understand the roles of `git add` and `git commit` commands in the Git workflow using an `index.html` file as an example.

### Steps:

1. **Open Visual Studio Code and Integrated Terminal:**
   - Launch Visual Studio Code (VSCode).
   - Open the directory where your Git repository is located using the VSCode file explorer.
   - Right-click on the directory to open the context menu.
   - Select "Open in Terminal" from the context menu to open the integrated terminal within VSCode.
   - Once you're in the desired directory, initialize a new Git repository using the `git init` command:
     ```
     git init
     ```
   - This command creates a new Git repository in the current directory.
   
2. **Create index.html File:**
   - Inside the directory, create a new file named `index.html` using any text editor available in VSCode.
   - Add some HTML content to the file, such as `<html><head><title>Hello World</title></head><body><h1>Hello, Git!</h1></body></html>`.

3. **Check Repository Status:**
   - In the integrated terminal, use the `git status` command to check the status of your repository:
     ```
     git status
     ```
   - This command will display the current status of your repository, showing that `index.html` is an untracked file.

4. **Explain the Need for "git add":**
   - Discuss why we need `git add`:
     - Git tracks changes made to files in the repository.
     - However, it doesn't automatically detect new files or changes to existing files.
     - We use `git add` to stage changes or new files for inclusion in the next commit.

5. **Stage Changes with "git add":**
   - Stage the changes made to `index.html` for commit using the `git add` command:
     ```
     git add index.html
     ```
   - This command adds the changes made to `index.html` to the staging area, preparing them for commit.

6. **Explain the Need for "git commit":**
   - Discuss why we need `git commit`:
     - Once changes are staged using `git add`, they are ready to be permanently saved to the repository.
     - `git commit` creates a snapshot of the changes staged in the staging area and adds a commit message to describe the changes.

7. **Commit Staged Changes with "git commit":**
   - Commit the staged changes to the repository with a descriptive commit message using the `git commit` command:
     ```
     git commit -m "Added index.html file"
     ```
   - This command saves the staged changes as a new commit in the repository, along with the provided commit message.

8. **Review the Repository Status:**
   - Use `git status` to verify that the changes have been committed successfully:
     ```
     git status
     ```
   - The output should indicate that there are no uncommitted changes in your repository.

9. **Conclusion:**
   - Reflect on the roles of `git add` and `git commit`:
     - `git add`: Stages changes or new files for inclusion in the next commit.
     - `git commit`: Saves staged changes as a new commit in the repository, creating a snapshot of the project's state.
   - Understanding these commands and their differences is essential for effective version control management in Git.

Additional Notes:
- Emphasize the importance of committing changes regularly to track project progress and maintain a reliable version history.
- Encourage students to experiment with the Git commands in their own projects to reinforce their understanding of the workflow.