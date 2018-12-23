# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > REPLACE THIS TEXT WITH YOUR RESPONSE
- Show current working directory path: `ls`
- Create a directory: `mkdir`
- Delete a directory: `rm -r <directory>`
- Create a file using a `touch` command: `touch <file name>`
- Delete a file: `rm <file name>`
- Rename a file: `mv <file A to rename> <renamed version of file A>`
- List a hidden file: `ls -a`
- Copy a file from one directory to another: `cp <file name> <directory>/`
- Bonus command: Print working directory: `pwd`
- Bonus command: Go up 3 directory levels: `cd ../../../`
- Bonus command: Copy all files of a certain format in to another directory: `cp star*.txt <directory>`
- Bonus command: Assign something (text, file , directory, command) to a variable: `<variable name>=<text/file/directory/command>` 
---

### Q2.  List Files in Unix   

What do the following commands do:  
* `ls` - Lists out the contents of the current working directory.  
* `ls -a`  - Lists out the contents of the current working directory, including hidden files.
* `ls -l`  - Lists out a table of the files in the current working directory with various attributes of that file (hard links, commands that can be run, creator, group, etc.)
* `ls -lh`  - Lists out all contents in the long form above with sizes in 'human-readable' format: 87621 -> 86K
* `ls -lah`  - Lists out all files, including hidden files,  in long form with human readable sizes.
* `ls -t`  - List out directory contents, sorted by modification time. 
* `ls -Glp`  - List out directory contents in long form, with different colors for files and folders, and with indicators appended to the end of the different file types. 

> > REPLACE THIS TEXT WITH YOUR RESPONSE

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > REPLACE THIS TEXT WITH YOUR RESPONSE

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > REPLACE THIS TEXT WITH YOUR RESPONSE

 

