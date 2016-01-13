---
layout: page
title: 'Assignment Directory Structure'
permalink: /assignments/dir_structure/
---

When you clone the Github branch for each assignment, you will have a top-level 
assignment directory that will contain any starter code. You may make 
subdirectories if you feel it is necessary to organize your code, but there are 
some files we require to be in the top-level assignment directory, as outlined 
below. Following these practices will ensure you pass the sanity check.

### Makefile

In early assignments, the assignment directory 
will contain a Makefile, which runs 
the commands necessary to build the binary file that may then be loaded on your 
Pi. Once you learn about Makefiles and the build process, we will stop 
providing these for you. At that point, we will expect you to create your own 
Makefile in the top-level assignment directory. This Makefile should compile 
your code into a binary file using the single command 'make', and the binary 
output should also end up in the top-level directory. 
An example Makefile with explanations can 
be found in the [make guide](/guides/make).

### .gitignore

A .gitignore file is a hidden file that Git uses to determine what files or 
types of files should not be saved and tracked. Generally, developers only 
wish to track changes to source files, so they include 
any automatically-generated files in .gitignore. 

In our case, you should not 
add any binary files (such as the output generated by 'make') to your Github 
repository. We will regenerate these binary files from your source code (using 
your Makefile) when we grade your assignment. So that you do not need to 
manually avoid including these binary files, your assignment repository 
includes a .gitignore that will skip over binary file types. Do not 
delete this .gitignore file or remove the lines in it. You may add to it if 
there are other files you would not like Git to track.