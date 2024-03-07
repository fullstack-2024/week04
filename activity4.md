# Activity 4: Introduction to Linux Command Line

## Part 1/3: Commands Covered:

- `whoami`: Display current user name
- `man`: Access the manual pages for commands
- `clear`: Clear the terminal screen
- Introduction to Options: Basic understanding of command options
- `pwd`: Print working directory
- `ls`: List directory contents
- `cd`: Change directory
- `mkdir`: Make directories


### 1. Getting Started:
- Open your terminal application.

### 2. `whoami`:
- Type `whoami` and press Enter.
- Note down the username displayed, which represents the current user.

### 3. `man`:
- Type `man` followed by any command name (e.g., `man ls`) and press Enter.
- Explore the manual pages for the specified command using the arrow keys to navigate and press `q` to exit.

### 4. `clear`:
- Type `clear` and press Enter to clear the terminal screen.

### 5. Introduction to Options:
- Learn about options by accessing the manual pages for a command with options.
- For example, type `man ls` to explore the options available for the `ls` command.

> The `ls` command is used to list directory contents in Linux. It comes with various options that can modify its behavior. Some common options for the `ls` command include:

1. `-a`: Lists all files, including hidden files (those starting with a dot `.`).
2. `-l`: Displays detailed information about each file, including permissions, owner, group, size, and modification date.
3. `-h`: Displays file sizes in a human-readable format (e.g., kilobytes, megabytes).
4. `-t`: Sorts files by modification time, with the newest files first.
5. `-r`: Reverses the order of sorting.
6. `-R`: Recursively lists subdirectories.
7. `-S`: Sorts files by size, with the largest files first.
8. `-d`: Lists directories themselves, rather than their contents.


### 6. `pwd`:
- Type `pwd` and press Enter to display the current working directory.
- Take note of the directory path.

### 7. `ls`:
- Type `ls` and press Enter to list the contents of the current directory.
- Experiment with different options, such as `ls -l` to list in long format or `ls -a` to show hidden files.

### 8. `cd`:
- Use `cd` followed by a directory name to navigate to that directory.
- For example, type `cd Desktop` and press Enter to change to the Desktop directory.
- Use `cd ..` to move up one directory level.

### 9. `mkdir`:
- Type `mkdir myfolder` and press Enter to create a new directory named "myfolder" in the current directory.
- Use `ls` to confirm that the directory has been created.

-----------
## Part 2/3: Commands Covered:

- `touch`: Create empty files or update file timestamps
- `rmdir`: Remove empty directories
- `rm`: Remove files or directories
- `open`: Open files or directories with default applications
- `mv`: Move or rename files or directories
- `cp`: Copy files or directories

## Instructions:

### 1. Getting Started:
- Open your terminal application.

### 2. `touch`:
- Use the `touch` command followed by a file name to create a new empty file.
- For example, type `touch myfile.txt` and press Enter to create a file named "myfile.txt".

### 3. `rmdir`:
- Create an empty directory using the `mkdir` command (e.g., `mkdir mydir`).
- Use the `rmdir` command followed by the directory name to remove the empty directory.
- For example, type `rmdir mydir` and press Enter to remove the directory named "mydir".

### 4. `rm`:
- Use the `rm` command followed by a file name to remove a file.
- For example, type `rm myfile.txt` and press Enter to delete the file "myfile.txt".
- Use the `-r` option to recursively remove directories and their contents.
- For example, type `rm -r mydir` to delete the directory "mydir" and all its contents.

### 5. `open`:
- Use the `open` command followed by a file name to open the file with the default application.
- For example, type `open ~/.profile` and press Enter to open the file "myfile.txt" with the default text editor.

### 6. `mv`:
- Use the `mv` command followed by the source and destination file or directory names to move or rename files or directories.
- For example, type `mv myfile.txt newfile.txt` to rename the file "myfile.txt" to "newfile.txt".
- To move a file or directory to a different location, specify the destination directory.
- For example, type `mv myfile.txt Documents/` to move the file "myfile.txt" to the "Documents" directory.

### 7. `cp`:
- Use the `cp` command followed by the source and destination file or directory names to copy files or directories.
- For example, type `cp myfile.txt mycopy.txt` to create a copy of the file "myfile.txt" named "mycopy.txt".
- To copy a directory and its contents, use the `-r` option.
- For example, type `cp -r mydir mydir_copy` to copy the directory "mydir" and all its contents to a new directory named "mydir_copy".


-----------
## Part 3/3: Commands Covered:

## Commands Covered:

- `head`: Display the beginning of a file.
- `tail`: Display the end of a file.
- `date`: Display the current date and time.
- Redirecting Standard Output: Learn to redirect command output to files.
- `cat`: Concatenate and display file contents.
- `less`: View file contents interactively.
- `echo`: Display a line of text.
- `wc`: Count lines, words, and characters in a file.
- Piping: Combine multiple commands to perform complex tasks.



### 1. Getting Started:
- Open your terminal application.

### 2. `head` Command:
- Type `head  ~/.profile` and press Enter.
- Note the first few lines of the file displayed on the screen.

### 3. `tail` Command:
- Type `tail  ~/.profile` and press Enter.
- Note the last few lines of the file displayed on the screen.

### 4. `date` Command:
- Type `date` and press Enter.
- Note the current date and time displayed on the screen.

### 5. Redirecting Standard Output:
- Use `>` to redirect command output to a file.
- For example, type `date > current_date.txt` and press Enter.
- Open the `current_date.txt` file to view the date written to it.

### 6. `cat` Command:
- Type `cat filename.txt` and press Enter.
- Note the entire contents of the file displayed on the screen.

### 7. `less` Command:
- Type `less filename.txt` and press Enter.
- Use the arrow keys to navigate through the file contents.
- Press `q` to exit the `less` command.

### 8. `echo` Command:
- Type `echo "Hello, World!"` and press Enter.
- Note the text "Hello, World!" displayed on the screen.

### 9. `wc` Command:
- Type `wc filename.txt` and press Enter.
- Note the number of lines, words, and characters in the file displayed on the screen.

### 10. Piping:
- Use the `|` operator to pipe the output of one command as input to another command.
- For example, type `cat  ~/.profile | head -n 5` and press Enter.
- Note that only the first 5 lines of the file are displayed.

