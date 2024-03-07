# Activity 5: Creating Directories, Subdirectories, and Files using Linux CLI & Initializing Git

## Part 1/3

In this part, we will learn how to create directories, subdirectories, and files using the Linux command line interface (CLI). Additionally, we will explore how to initialize a Git repository, add files, and commit changes.


### 1. Creating Directories and Files:
- Open your terminal application.
- Navigate to the location where you want to create the directory `dev-2024-03-07`.
- Use the following command to create the directory:
  ```
  mkdir dev-2024-03-07
  ```
- Navigate into the `dev-2024-03-07` directory:
  ```
  cd dev-2024-03-07
  ```
- Create subdirectories and files as needed using commands like `mkdir` (for directories) and `touch` (for files). For example:
  ```
  mkdir subdirectory1 subdirectory2 subdirectory3
  touch file1.txt file2.txt file3.txt
  ```

### 2. Initializing Git:
- Ensure you are inside the `dev-2024-03-07` directory.
- Use the following command to initialize a Git repository:
  ```
  git init
  ```

### 3. Adding Files to Git:
- Add all files and directories to the staging area using the following command:
  ```
  git add .
  ```

### 4. Committing Changes:
- Commit the added files to the Git repository with a meaningful commit message:
  ```
  git commit -m "Initial commit: Created dev-2024-03-07 directory and added subdirectories and files"
  ```

-----
## Part 2/3

In this lab, we will expand on the previous exercise by creating multiple directories, each containing some files, using the Linux command line interface (CLI). Additionally, we will initialize a Git repository, add files, and commit changes.

### 1. Creating Multiple Directories and Files:
- Open your terminal application.
- Navigate to the location where you want to create the main directory.
- Use the following command to create the main directory (e.g., `projects`):
  ```
  mkdir projects
  ```
- Navigate into the `projects` directory:
  ```
  cd projects
  ```
- Create multiple directories (e.g., `project1`, `project2`, `project3`) using the `mkdir` command:
  ```
  mkdir project1 project2 project3
  ```
- Navigate into each directory (e.g., `project1`) using `cd` and create files as needed using the `touch` command. For example:
  ```
  cd project1
  touch file1.txt file2.txt
  ```
  Repeat this step for each directory (`project2`, `project3`) and create files as desired.

### 2. Initializing Git:
- Ensure you are inside the `projects` directory.
- Use the following command to initialize a Git repository:
  ```
  git init
  ```

### 3. Adding Files to Git:
- Add all files and directories to the staging area using the following command:
  ```
  git add .
  ```

### 4. Committing Changes:
- Commit the added files to the Git repository with a meaningful commit message:
  ```
  git commit -m "Initial commit: Created multiple directories and added files"
  ```

-----
## Part 3/3

In this part, we will enhance the previous exercise by not only creating multiple directories with files but also using additional commands such as `echo`, `cat`, and `ls` to generate content for files. We will accomplish this using the Linux command line interface (CLI) and initialize a Git repository to track our changes.

### 1. Creating Multiple Directories and Files:
- Open your terminal application.
- Navigate to the location where you want to create the main directory.
- Use the following command to create the main directory (e.g., `projects`):
  ```
  mkdir projects
  ```
- Navigate into the `projects` directory:
  ```
  cd projects
  ```
- Create multiple directories (e.g., `project1`, `project2`, `project3`) using the `mkdir` command:
  ```
  mkdir project1 project2 project3
  ```
- Navigate into each directory (e.g., `project1`) using `cd` and create files as needed. You can use commands such as `echo`, `cat`, and `ls` to generate content for files. For example:
  ```
  cd project1
  echo "This is file1 content" > file1.txt
  cat /etc/passwd > file2.txt
  ls -l > file3.txt
  date > file4.txt
  ```
  Repeat this step for each directory (`project2`, `project3`) and create files as desired.

### 2. Initializing Git:
- Ensure you are inside the `projects` directory.
- Use the following command to initialize a Git repository:
  ```
  git init
  ```

### 3. Adding Files to Git:
- Add all files and directories to the staging area using the following command:
  ```
  git add .
  ```

### 4. Committing Changes:
- Commit the added files to the Git repository with a meaningful commit message:
  ```
  git commit -m "Initial commit: Created multiple directories and added files with content generated using various commands"
  ```


