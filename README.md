# ce01 Unix Commands

This exercise is designed to get you acquainted with basic Unix commands.
You will create regular files and directory files and learn how to navigate 
a Unix system from the command line.

## Prerequisite Knowledge

* An introduction to Unix: http://www.ee.surrey.ac.uk/Teaching/Unix/unixintro.html
* Unix Tutorial One, Two, Three, and Four: http://www.ee.surrey.ac.uk/Teaching/Unix

## Course-Specific Learning Outcomes

* **LO1.a:** Navigate and modify files, directories, and permissions in a multi-user Unix-like environment.
* **LO1.b:** (Partial) Execute, redirect, pipe, and manage programs/processes in a multi-user Unix-like environment.

## Before You Begin

You should complete one of the setup instructions provided below before you begin.

* MacOS Setup Instructions: https://github.com/cs1302uga/cs1302-exercises/blob/master/misc/MacOS.md
* Windows 10 Setup Instructions: https://github.com/cs1302uga/cs1302-exercises/blob/master/misc/Windows10.md

If you have access to your Nike account, then you may login and perform the exercise there.
Otherwise, you may perform the exercise on your local machine. To login to Nike, open up a local
terminal in your terminal emulator and type the following command, replacing `user` with the
Nike username provided to you by System Support:

```
$ ssh user@nike.cs.uga.edu
```

**NOTE:** The `ssh` program does not display your password as you type it when logging in.

## Creating Directories

By the end of this exercise, you will have a directory hierarchy similar to 
the one seen below. You will use a variety of Unix commands to create this 
heirarchy step-by-step.

```
exercise1
 |--- README.txt
 |--- photos
 |      |--- 2017
 |      |--- 2018
 |      |--- 2019
 |--- school
 |      |--- 1302
 |            |---notes
 |                  |---day1.txt
 |                  |---names.txt
 |--- lit_works
 |      |--- 48320-0.txt

8 directories, 4 files
```

## Questions

In your notes, clearly answer the following questions. These instructions assume that you have setup
your local machine following the instructions linked to on eLC and the syllabus.

**NOTE:** For each step, please provide in your notes the full command that you typed to make the related 
action happen along with an explanation of why that command worked. Some commands require multiple options. 
It is important to not only recall what you typed but also why you typed each of them. If done properly, your 
class notes will serve as a helpful study guide for the exam. 

1. When you launch your terminal emulator, what is the absolute path of the directory it places you 
   in? What command can you use to figure it out?

1. What series of commands can be used to create the `exercise1`, `photos`, and yearly 
   subdirectories under `photos` in the example provided above? No need to create `school` or `lit_works`
   at this time. Assume that you change into each directory, as needed, after making it. Write all commands
   used in your notes.

1. Change into the `2019` directory. From within `2019`, what single command can be used to change into the `photos`
   directory? Go ahead and execute the command to navigate to `photos`.
 
1. Change into the `2019` directory. From within `2019`, what single command can be used to change into the `exercise1`
   directory? Go ahead and execute the command to navigate to `exercise1`.

1. Your present working directory (pwd) should be `exercise1`. From this directory, without changing into other
   directories, what series of commands can be used to create the `school`, `1302`, and `notes` directories? 

**CHECKPOINT**

1. Your present working directory (pwd) should be `exercise1`. What series of commands can be used to
   verify that the directories in the previous question were successfully created? Assume that
   you never change directories for this question.

1. If you are elsewhere, change into the `exercise1` directory. Use the `rmdir` command to remove (delete)
   the `school`, `1302`, and `notes` directories. Write and describe all commands used in your notes.
   
1. **[TRICKY]** If you are elsewhere, change into the `exercise1` directory. What _single command_ 
   can be used to create the `school`, `1302`, and `notes` directories? You will need to first remove 
   these directories to verify that your command works correctly.

1. The `echo` command is a pretty popular Unix command. What command can be used to learn more
   about it?

1. Change into the `notes` directory. What command(s) can be used to add your group's first and 
   last names to a regular file called `day.txt` in the present working directory?

1. Assume you are still in the `notes` directory. There are a couple different commands that can 
   be used to display the contents of a file. Give two commands that can be used to verify that 
   your group's first and last names are actually in `day.txt'. 

**CHECKPOINT**

1. Assume you are still in the `notes` directory. What command can be used to rename `day.txt`
   to `day1.txt`.

1. Change into the `exercise1` directory. What command can be used to copy `day1.txt` to
   `names.txt` into the `notes` directory?

1. Assume you are still in the `exercise1` directory. What command(s) can be used to verify that
   you actually copied the file in the previous question to the desired location?

1. Change to the `1302` directory. What command can be used to copy the entire contents of the 
   `notes` directory directly into the `exercise1` directory?

1. Now that you have two `.txt` files inside of the `exercise1` directory. What single command
   can be used to delete both of them?

**CHECKPOINT**

1. In your web browser of choice, visit
   [Project Gutenberg](https://www.gutenberg.org/) and find the `Plain Text UTF-8` version of the 
   _Adventures of Sherlock Holmes_ by Sir Arthur Conan Doyle. Use the `wget` command to download 
   this file into the `lit_works` directory. How many lines, words, and bytes are in this file?

1. As you might suspect, the name "Sherlock" (case sensitive) appears on many lines in this file. 
   What command can be used to display only these lines to standard output? 

1. What command can be used to output the number of lines containing the name "Sherlock" 
   (case sensitive)?

1. Consider your response to the previous two questions. What commands can be used to output
   the number of lines containing both the word "Sherlock" (case sensitive) and "Watson"
   (case sensitive)?

1. **[TRICKY]** What command can be used to count the number of lines in this file that
   contain the name "Sherlock" with any capitalization other than "Sherlock"? For example, 
   "sHerlock", "sherlock", "sherLOCK", etc. are examples of capitalizations that are not
   literally "Sherlock".

**CHECKPOINT**

<hr/>

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by-nc-nd/4.0/)

<small>
Copyright &copy; Michael E. Cotterell, Brad Barnes, and the University of Georgia.
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a> to students and the public.
The content and opinions expressed on this Web page do not necessarily reflect the views of nor are they endorsed by the University of Georgia or the University System of Georgia.
</small>

