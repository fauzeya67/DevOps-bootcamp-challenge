# Linux Basic Commands and Permission Management - Practical Questions

## 1. Basic Commands
- List all files (including hidden files) in your current directory along with detailed information (permissions, owner, size, date).
- Create a new directory named `test_dir` inside your home directory and verify its creation.
- Use `grep` to search for the word "error" (case-insensitive) inside a log file named `system.log` and display the matching lines.

## 2. Redirection
- Using output redirection, save the list of all running processes to a file named `process_list.txt`.
- Append the current date and time to the end of the `process_list.txt` file.

## 3. Text Editor (vim/nano)
- Open or create a file named `notes.txt` using `vim` or `nano`. Add the text "This is a sample note." Save and exit the editor.
- Using `vim`, undo the last change you made and then redo it.

## 4. Permission Management
- Change the permissions of `notes.txt` to allow the owner to read and write, the group to read only, and others no permissions.
- Change the ownership of `notes.txt` to a different user and group (use existing users/groups on your system).
- Check your current `umask` value. Then, change the `umask` value to `027` and create a new file. Verify the permissions of this file.
