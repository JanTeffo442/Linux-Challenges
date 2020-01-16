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
~$ mv exercise.md /tmp
# moves exercise.md to tmp directory
~$ cd /tmp
/tmp$ ls
# exercise.md appears in tmp directory
/tmp$ rm exercise.md
/tmp$ ls
# exercise.md removed form tmp

TASK 3

~$ touch umuzi.md recruit.md cohort.md
# Creates three files with the associated names
~$ cat umuzi.md
# Write the text "This is the best place to be" to umuzi.md then press Enter to save and CTRL+Z to exit

~$ cat recruit.md
# Write the text "Making Umuzi Better" to recruit.md then press Enter to save and CTRL+Z to exit

~$ cat cohort.md
# Write the text "Best cohort ever.2020" to cohort.md then press Enter to save and CTRL+Z to exit

~$ cat umuzi.md recruit.md cohort.md > summary.md
# Creates the file summamry.md and copies the content of umuzi.md, recruit.md, cohort.md respectively
~$ cat summary.md
# Displays 
# This is the best place to be
# Making Umuzi Better
# Best cohort ever.2020
# respectively

~$ cat umuzi.md recruit.md cohort.md -> summary
# Enter the text "The end" and press ENTER to save and CTRL+Z to exit

~$ cat summary.md
# Displays 
# This is the best place to be
# Making Umuzi Better
# Best cohort ever.2020
# Withiut overwriting the contents of summary.md


TASK 4
~$ locate umuzi
# Populates locations of all files and directories with name umuzi
~$ locate umuzi > search_result.md
# Copies output of locate umuzi into saerch_result.md
~$ cat search_result.md
# Displays locations of all files and directories with name umuzi

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
~$ find . -type f -newermt 2020-01-16 -ls
# Populates a list of files that were modified today

TASK 7
~$ nano my_bio.md
# opens nano editor to creates a file named my_bio.md
# Press CTRL+O to edit the name of the file and Press # Enter to save, the Press CTRL+X to exit editor
~$ mkdir my_files
# Creates a directory named my_files
~$ mv my_bio ~/my_files
# moves my_bio.md to my_files directory
~$ cd ~/my_files
~/my_files$ ls
# Displays my_bio.md

