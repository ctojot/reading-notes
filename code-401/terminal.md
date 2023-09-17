# Practice in the Terminal

This file includes an outline of the reading. I did this just in case there's someting I don't remember and have something to look back to. I included my thoughts after each section.

## The Command Line

### What are they exactly?

- The command line is a text based interface to a system
- You can type commands via keyboard and you will receive feedback by text as well
- Here's a breakdown of what you'll see on a commnad line:

  - First thing you will see is a prompt
  - Anything you type will appear after the prompt
  - Once you type a command and hit enter, you will be given an output
  - Outputs can either produce text feedback, an error notice, or nothing at all

### Opening a Terminal

- Getting to a terminal depends on the type of system you have:

  - For mac users, you would go into **Applications** -> **Utilities** and look for a program called **Terminal** (You can also use **command + space** to bring up Spotlight and search for **Terminal**)
  - For Linux users, you either go to **Applications** -> **Utilities** or **Applications** -> **System** depending on your linux distribution (You can also right-click the desktop and find a **Open in Terminal** option)
  - For windows, you will need an **SSH Client** to remotely log into another machine

### The Shell, BASH

- The shell is part of the operatin system that defines how the terminal will behave and looks after running commands
- The most common shell is ***Bash***

### Shortcuts

- Linux is full of shortcuts to make our lives easier
- One example is the up and down keys, the system stores your history so instead of typing something mulitples you can probably hit the up or down key a couples times to reuse that same command

### Thoughts of The Command Line

- This section is very valuable to me. I feel like when we started coding, we were told to use terminals but we never really went into depth with it. I like know what I'm using and why I'm using it to understand things better. This sections explains all the questions I had previously. The only thing I wish to understand now is why you have to do use a terminal remotely with Windows.

## Basic Navigation

### Introduction

- Learning about the basics of moving around the system

### So where are we?

- **pwd** stands for ***Print Working Directory***
- pwd tells you the current directory that you are in
- Most Linux commands are abbreviations

### What's in our current location?

- **ls** is short for ***List***
- When run with no arguments, it will create a listing of the current location
- ls ***[options] [location]*** (Brackets indicate that ls can be run with our without these)
- **-l** is a command line option to indicate long listing
- **/etc** is command argument that lists the current directories contents

### Paths

- A **path** is a means get to a particular file or directory on the system

#### Absoulte and Relative Paths

- **Root** directory is denoted with a single forward slash '/'
- **Absolute** paths specify a location (file or directory) in relation to the root directory (easliy identified with the forward slash '/')
- **Relative** paths specify a location (file or directory) in relation to where you currently are in the system (Does not include a slash)
- Example of absolute path: ls /home/user/Documents
- Example of relative path: ls Documents

#### More on paths

- Most things on Linux can be acheived in different ways, paths or no different
- Ways to help build paths:

  - (~) tilde: a shortcut for the home directory
  - (.) dot: a reference to your current directory
  - (..) dotdot: a reference to the parent directory

### Let's move around a bit

- **cd** stands for ***Change Directory***
- cd ***[location]***
- If you run this command without arguments it will take you back to your home directory
- Location can be specified as an absolute or relative path

### Thoughts on Basic Navigation

- As far as it goes I didn't want to to deep with the activity. I've ruined files on PC's by accident. This does help me with finding ways to do things much easier. The Tab shortcut is very useful one that I discovered on my own but didn't really know its purpose so I never utilized it. Also knowing theres muliple ways to do things is very helpful as well. Whenever i am learning something, I always try to find the correct way to do things. So it's nice to know that there's multiple ways to do something. The way I usually navigate through the terminal is using ls, seeing what's inside, and then using cd to go where I need to. I feel more comfortable doing it this way.

## More About Files

### Everything is a file

- Everything from a file, a directory, a keyboard, even a monitor are all files

### Linux is a Extensionless System

- A file extension is usually a set of 2-4 characters after a full stop at the end of a file
- Common extensions:

  - file.exe - an exectuable file or program
  - file.txt - a plain text file
  - file.png, file.gif, file.jpg - image files

- Some systems use the file extensions to determine that type of file that it is
- Linus ignores the extension and looks inside the file itself to determine what type of file it is	
- **file** ***[path]***

### Linux is Case Sensitive

- Other systems like Windows are case insestive when it comes to referring to files
- Linux is case sensitive, so it is possible to have files with the same name but letters are different case
- This also means commands are case sensitive as well
- With the command ***ls*** there are two options ***s*** and ***S*** both of which do different things

### Spaces in Names

- Spaces in files and directories are valid but require caution
- For example, the command ***cd Holiday Photos*** would return ***cd: Holiday: No such files or directory***, becuase of the space its only reading Holiday and Photos is not taken in account

### Quotes

- One way to work around this would be adding quotes around ***Holiday Photos***
- You can use either single or double quotes
- Anything inside quotes is considered a single item

### Escape Characters

- Another method is using escape characters like backslash "\"
- Backslash escapes (or nullifies) the meaning of the next character
- For example, the correct command would be ***cd Holiday"\"Photos***

### Hidden Files and Directories

