TASK 1

~$ ls
# I see a list of directorie and files. These are the contents of the recruit or home directory

~$ pwd
# I see a path /home/recruit given. This is where I am currently. It is the present working directory.

~$ mkdir workspace
~$ cd ~/workspace/
~/workspace$ ls
# workspace directory is empty. No directories and files

~/workspace$ touch README.md
~/workspace$ ls
# README.md appears in the workspace directory

~/workspace$ cp README.md CHANGELOG.md
~/workspace$ ls
# CHANGELOG.md and README.md appear in workspace directory


TASK 2

~$ touch exercise.md
~$ ls
# exercise.md appears together with Desktop, Pictures, Downloads, etc.


TASK 5

~$ cd ~/Documents
~/Documents$ touch pad.md
# creates a file named pad.md in Documents directory
~/Documents$ cd ..
# navigates back to the previous folder
~$ cd ~/Desktop
~/Desktop$ mkdir work
# creates a directory named work
~/Desktop$ cd work
~/Desktop/work$ cp /home/recruit/Documents/pad.md pad_copy.md
# copies pad.md from Documents to work directory and renames it to pad_copy
~/Desktop/work$ sudo updatedb
#updates database with administrator's credentials
~/Desktop/work$ cd ..
# Navigates back to Desktop
~/Desktop$ locate pad_copy.md
# path of pad_copy is provided

TASK 6

~$ find ~/ -name *.pdf
# Displays all pdf files on the computer
~$ find ~/ -name *.pdf > pdfresults.md
# writes output to output to pdfresults
~$ find . -type f -newermt 2020-01-16
# Populates a list of files that were modified today
