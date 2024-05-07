# The Command Line:

## So what are they exactly?
the command line/terminal is way to interact with the computer throught a text command instead of using the screen and mouse. it is faster and more efficient compare to the GUI.
 
### The Command Line Parts :
- the prompt
- the command line
- command line arguments ( Options )
- output from running the command.

### Basic Shortcuts:
#### - echo $SHELL:
 display the shell that is avalible on you device (mine is bash) 
#### - echo $HISTSIZE 
 recent commands history number

### Basic Navigation!

- pwd : shows our present working directory that we are in, it stands for (Print Working Directory)
- ls : shows the contents of our working directory, it stand for list
- ls -l : shows the contents of our working directory as along list

Paths in Linux: In linux we have two types of path absolute and relative.
Absolute paths specify a location (file or directory) in relation to the root directory i.e (/home/ryan). 
Relative paths determine the file  location of the file or directory in relation to where we are in the system. They will not begin with a slash. (file1.txt file2.txt file3.txt)

Move Around: In order to move around in the system we use a command called cd which stands for change directory. It works as follows:

cd [location]

More About Files!

- Everything is a File: linux under the hood treat everything as a file (i.e text file, directory,  keyboard. etc...)
- Linux is an Extensionless System :  Under Linux the system actually ignores the extension and looks inside the file to determine what type of file it is.
- Linux is Case Sensitive : that mean you can savw to direcoties with the same name but one with uppercase lettter and the other with samll letter.


file
    obtain information about what type of file a file or directory is.
ls -a
    List the contents of a directory, including hidden files.

### Manual Pages!

- The manual pages is a page where you can see each command line details, like how to use it and what are the SYNOPSIS, DESCRIPTION, and so on.

to display the manual page for specific command type the following :

- man > then the command to look up

you can also Do a keyword search for all manual pages containing the given search term. 
   man -k 'search term'

After performing a search within a manual page, select the next found item.
   n

### File Manipulation!

Making a Directory : If you want to make a directory you can type the following command in the terminal :

mkdir [options] 'Directory'

Removing a Directory : to remove a directory (empty directory) use the following command :

rmdir [options] 'Directory'

Creating a Blank File : touch [options] 'filename'

Copying a File or Directory : cp [options] 'source' 'destination'

Moving a File or Directory : mv [options] 'source' 'destination'

Removing a File (and non empty Directories) : rm [options] 'file'

Removing non empty Directories : rm -r 'Directory'