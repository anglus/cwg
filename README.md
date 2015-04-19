# cwg
ABOUT THE CONSTRUCTED WORD GENERATOR

The Constructed Word Generator is a KornShell script that takes a set of rules from STDIN or a file and constructs one or more random words based on those rules. It can be used to generate words for an invented language or names for science fiction or fantasy stories. It was inspired by Curt Snyder's "romulan.c" (a C port of Star Trek author Diane Duane's BASIC program) and Jeffrey Henning's "LangMaker". The former program was written in C and had the Rihannsu phonemes hard-coded in. The latter program was written in Visual Basic for Windows, and could generate words using rules provided by the user. I wanted a program that did the same thing as LangMaker, but functioned more like a proper Unix program.

I wrote the Constructed Word Generator mostly in February and March of 2006. I wanted it to be portable to as many Unix-like systems as possible, so I originally attempted to write it in the Bourne shell, but due to various deficiencies of the Bourne shell, and also due to the fact that not many people were using 7th Edition Unix or 4.2BSD in 2006, I rewrote it in the KornShell, implementations of which are available for all modern Unix-like systems.

INSTALLATION

Download, copy, or move the file "cwg.ksh" to a directory that is in your PATH. Make the script executable. I prefer to rename my executable script to simply "cwg". The follwing example assumes you have a "$HOME/bin" directory that is in your PATH:

$ mv cwg.ksh ~/bin/cwg

$ chmod +x ~/bin/cwg

The Constructed Word Generator operates on data provided by the user, either in the form of a rules file or entered directly from the keyboard. If you wish to test the script with some example files, download some of the sample "*.rules" files to a directory of your choice.
