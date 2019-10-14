My Cheat Sheet

##**Text editor**

What features should you look for in a text editor? I would say some
of the most important features are: 1.) code completion; 2.) syntax
highlighting; 3.) a nice variety of themes (to reduce eye strain and
fatigue); and 4.) the ability to choose from a healthy selection of
extensions available when you need them. You might find some other
features that are must-have’s, but I think these features are a good
start.

Differece between text editor and IDE

An IDE (Integrated Development Environment) is really a suite of
different software all coming together. An IDE is a text editor, a file
manager, a compiler, and a debugger all in one software package.

#**Command Terminal**

A command line, or terminal, is a text based interface to the system.
command line has a shell
linus is case sensitive
there must be a space between the command line and the first 
linux is an extensionless system: the stuff that comes after a full stop
hidden files, name is preceeded with full stop (period); i.e. .filename
When you enter commands, they are actually stored in a history. You can traverse this history using the up and down arrow keys
ls -a lists all files in directory, including hidden

echo command tells you what command terminal shell in

Ok, the first thing we need to appreciate with linux is that under the hood, everything is actually a file. A text file is a file, a directory is a file, your keyboard is a file (one that the system reads from only), your monitor is a file (one that the system writes to only) etc.
absolute vs relative paths
~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents
. (dot) - This is a reference to your current directory. eg in the example above we referred to Documents on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).
.. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this would do a listing of the root directory.

ls - list [options] [location]
Line 1 - We ran ls in it's most basic form. It listed the contents of our current directory.
Line 4 - We ran ls with a single command line option ( -l ) which indicates we are going to do a long listing. A long listing has the following:
First character indicates whether it is a normal file ( - ) or directory ( d )
Next 9 characters are permissions for the file or directory (we'll learn more about them in section 6).
The next field is the number of blocks (don't worry too much about this).
The next field is the owner of the file or directory (ryan in this case).
The next field is the group the file or directory belongs to (users in this case).
Following this is the file size.
Next up is the file modification time.
Finally we have the actual name of the file or directory.
Line 10 - We ran ls with a command line argument ( /etc ). When we do this it tells ls not to list our current directory but instead to list that directories contents.
