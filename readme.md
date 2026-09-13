Linux Commands :

Linux Command # 1 : cat command 

Cat Command in Linux

The cat (concatenate) command in Linux is used to view, create, and combine file contents directly from the terminal. It allows users to quickly work with file content without opening a text editor.

Primarily used to display the contents of files on the terminal.
Can concatenate multiple files and display them as a single continuous output.
Helps in creating new files or appending data to existing ones.
Useful for quick file inspection, debugging, and scripting tasks without opening a text editor.
Examples
Below are some basic and commonly used examples of the cat command in Linux.

1: View the Content of a Single File in Linux
To display the content of a single file in the terminal.

Syntax: 

cat file_name
Example:

cat jayesh.txt


Linux Command # 2 : cd

Changing the Directory in Linux | cd Command

The cd (Change Directory) command in Linux is used to navigate between directories in the file system.

It allows users to move from the current working directory to another specified directory by providing either an absolute path or a relative path.
This command is essential for exploring different locations within the Linux environment and managing files efficiently.
Examples:
Here are some commonly used examples of the cd command in Linux.

1. Move Inside a Subdirectory
To move inside a subdirectory in Linux use the CD Linux Command. Here, replace [directory_name] with the desired directory you want to move in.

Syntax:

cd [directory_name]
Example:

cd Documents


Linux Command # 3 : cp command

cp Command in Linux

The cp (copy) command in Linux is used to duplicate files or directories from one location to another within the file system. It supports copying single files, multiple files, and entire directories, with options to control overwriting and attribute preservation.

Copy data from one file to another
Copy multiple files into a directory
Recursively copy directories and subdirectories
Overwrite existing files by default
It offers three principal modes of operation, each serving different purposes.

1. Copying Between Two Files in Linux
When the cp command is provided with two file names, it copies the contents of the source file to the destination file.

If the destination file does not exist, it is created.
If the destination file already exists, it is overwritten without warning.
cp Sorce_file Destination_file
Example 1: Copy to a New File

Create a new file by copying the contents of an existing file.

cp a.txt b.txt
a.txt exists in the directory
b.txt does not exist, so it is created
Contents of a.txt are copied into b.txt

Example 2: Overwrite an Existing File

Replace the contents of an existing file with another file’s contents.

cp a.txt c.txt
c.txt already exists
Its contents are replaced with the contents of a.txt


Syntax
The cp command has a flexible syntax depending on whether you are copying a single file, multiple files, or directories.

cp [options] <source> <destination>
cp [options] <source1> <source2> ... <destination_directory>
cp: invokes the copy command
[options]: optional flags that modify the behavior (e.g., -i, -f, -r, -p)
<source>: the file or directory to be copied
<source1> <source2> ...: allows specifying multiple source files
<destination>: target file or directory
<destination_directory>: if copying multiple files, the destination must be a directory
...: indicates that multiple sources can be specified


2. Copy files to a Directory in Linux
When the cp command is given one or more source files followed by a destination directory, it copies each source file into the destination directory using the same file names.

f the destination directory does not exist, it is created.
If files with the same name already exist in the destination, they are overwritten without warning.
cp Src_file1 Src_file2 ... Dest_directory
Src_file1 Src_file2 ...: one or more source files
Dest_directory: directory where files are copied
...: indicates that multiple source files can be specified
Example: Copy Multiple Files to a Directory

Copy several files into a single directory in one command.

cp a.txt b.txt c.txt new/
a.txt, b.txt, and c.txt are source files
new/ is the destination directory
All files are copied into new/ with their original names


Linux Command # 4 : mkdir (create directory command)

How to Create Directory in Linux | mkdir Command

The mkdir command in Linux stands for “make directory” and is used to create new folders quickly and efficiently from the terminal.

It helps users organize their files by creating one or multiple directories at once, with options to set permissions and create nested folders easily.
Used to create new directories within the Linux file system.
Allows the creation of multiple directories simultaneously in a single command.

Examples
1) How to create a directory in Linux using the `mkdir` command?
To create a single directory, use the following syntax:

For Example: 

If we want to create a directory name "jayesh_gfg".

Syntax:

mkdir jayesh_gfg
This command creates a directory named "jayesh_gfg" in the current location. You can replace "jayesh_gfg" with any name you prefer.


Linux command # 5 : rmdir to (to remove directories)

rmdir Command in Linux With Examples

The rmdir command in Linux is used to safely remove empty directories from the filesystem.

Specifically designed to delete only empty directories.
Unlike the rm command, it cannot delete files or non-empty directories.
Ensures data safety by verifying that the directory is empty before deletion.
Helps maintain a clean and organized directory structure.
Commonly used for system cleanup and managing temporary or unused folders.

Example 1: Remove a single empty directory:
rmdir test

Example 2: Remove multiple empty directories:
rmdir dir1 dir2 dir3

Linux Command # 6 : pwd

Displaying the Current Working Directory in Linux | pwd Command

Displaying the Current Working Directory
To print the current working directory, simply enter:

pwd

Linux Command # 7 : CHMOD

chmod Command in Linux

The chmod (change mode) command in Linux/UNIX is used to modify file and directory permissions. It controls who can read, write, or execute a file by setting access rights for the owner, group, and others. Let’s use the chmod command to set the permission to 745.

Command:

chmod 745 newfile.txt

Linux Command # 8 : more

more command in Linux with Examples

The more command in Linux is used to view the contents of a text file one screen (or page) at a time in the terminal, allowing users to scroll through long files easily.

Forward navigation only - you can move ahead line by line (Enter) or page by page (Space).
Cannot scroll backward, unlike the less command.
Useful for reading logs, configuration files, or command outputs (cat file.txt | more or more file.txt).
You can search text within a file by typing /pattern.
Example
The command used to display the contents of a file one page at a time.

more sample.txt

Linux Command # 9 : find

Find Command in Linux

The find command in Linux is used to search for files and directories based on name, type, size, date, or other conditions. It scans the specified directory and its sub directories to locate files matching the given criteria.

Search based on modification time (e.g., files edited last week).
Locate files with specific permissions or content.
Automate tasks like deleting or executing commands on found files.
Example : To find a file named "example.txt" in the home directory, you would use:

find ./gfg -name "sample.txt"

Linux Command # 10 : kill

kill Command in Linux

The kill command in Linux is used to send signals to processes in order to control their execution. It is commonly used to terminate processes, but it can also pause, resume, or perform other actions depending on the signal sent. The kill command sends signals to processes using their Process ID (PID).

Located in /bin/kill , it’s a built-in Linux command.
Sends specific signals to processes using their Process ID (PID).
By default, it sends the SIGTERM (15) signal to terminate a process.
Can use other signals like SIGKILL (9) or SIGSTOP (19) for different actions.
Example: Killing the Mozilla Firefox Process
Terminate the Mozilla Firefox browser process when it becomes unresponsive or needs to be closed from the terminal.

Step 1: Identify the Firefox PID
Check the running Firefox processes and their PIDs.

Command:

ps aux | grep firefox

Linux Command # 11 : ps

ps Command in Linux

The ps command in Linux is used to display information about currently running processes. It provides a snapshot of processes at the time the command is executed. System administrators commonly use it to monitor processes, troubleshoot issues, and identify resource usage.

Display currently running processes on a Linux system
Identify process IDs (PIDs) for management tasks like stopping processes
View process ownership, CPU usage, and memory consumption
Inspect background processes and system services
Filter processes based on users, IDs, terminals, or command names
Example: Display Processes in the Current Terminal
This command displays the processes running in the current shell session. When executed without options, the ps command only shows processes associated with the current terminal.

Command:

ps

Linux Command # 12 : finger

Finger command in Linux with Examples

The 'finger' command is a powerful utility in Linux used to display information about users logged into the system. This command is commonly used by system administrators to retrieve detailed user information, including login name, full name, idle time, login time, and sometimes the user's email address. The 'finger' command offers more comprehensive details compared to the 'pinky' command, which is a lighter version with limited output.


Working with finger User Information Lookup Tool
Once installed, the 'finger' command can be used to fetch detailed information about users on your Linux system. Here are some common ways to use this command:

1. Retrieving User Information
To get detailed information about a specific user, simply use the 'finger' command followed by the username.

$finger manav

Linux Command # 13 : df 

df Command in Linux

The df command in Linux is used to display disk space usage of mounted file systems. It provides information about total space, used space, available space, and the percentage of usage for each file system.

Can display output in human-readable format.
Useful for system monitoring and storage management.
Example 1: Display Disk Usage of All Mounted File Systems
Command:

df

Linux Command # 14 : grep

grep command in Unix/Linux

The grep command is one of the most useful tools in Linux and Unix systems. It is used to search for specific words, phrases, or patterns inside text files, and shows the matching lines on your screen.

grep Command is useful when you need to quickly find certain keywords or phrases in logs or documents. Let’s consider an example:

Search for a word in a file
If you have a file called notes.txt and you want to find all lines containing the word Python, you can use:

grep "python" notes.txt

Syntax of grep Command in Unix/Linux
The basic syntax of the `grep` command is as follows:

grep [options] pattern [files]
[options]: These are command-line flags that modify the behavior of grep. 
[pattern]: This is the regular expression you want to search for.
[file]: This is the name of the file(s) you want to search within. You can specify multiple files for simultaneous searching.

Linux Command # 15 : man

How to Read Manual Pages in Linux | man Command

The "man" command, short for manual, is a powerful tool in the Linux operating system that allows users to access detailed information about various commands, utilities, and system calls. The "man" command provides comprehensive documentation, helping users understand how to use and configure different elements of the Linux environment. This article will explore the "man" command in detail, covering its syntax, and options, and providing practical examples.

The basic syntax of the "man" command is as follows:

man [option] [command]
Here,

"option" refers to additional flags that modify the behavior of the "man" command,

"command" is the Linux command or utility for which you want to access the manua





####################################################################

~~~~~~~~~~~~~~~~~~~~~~~~~~~~Git Commands~~~~~~~~~~~~~~~~~~~~~~~~~~

###################################################################


INSTALLATION & GUIS
With platform specific installers for Git, GitHub also provides the 
ease of staying up-to-date with the latest releases of the command
line tool while providing a graphical user interface for day-to-day
interaction, review, and repository synchronization.

GitHub for Windows
https://windows.github.com

GitHub for Mac
https://mac.github.com

For Linux and Solaris platforms, the latest release is available on the oﬃcial Git web site.

Git for All Platforms
http://git-scm.com

SETUP
Configuring user information used across all local repositories

git config --global user.name “[firstname lastname]”
set a name that is identifiable for credit when review version history

git config --global user.email “[valid-email]”
set an email address that will be associated with each history marker

git config --global color.ui auto
set automatic command line coloring for Git for easy reviewing

SETUP & INIT
Configuring user information, initializing and cloning repositories

git init
initialize an existing directory as a Git repository

git clone [url]
retrieve an entire repository from a hosted location via URL

STAGE & SNAPSHOT
Working with snapshots and the Git staging area

git status
show modified files in working directory, staged for your next commit

git add [file]
add a file as it looks now to your next commit (stage)

git reset [file]
unstage a file while retaining the changes in working directory

git diff
diﬀ of what is changed but not staged

git diff --staged
diﬀ of what is staged but not yet committed

git commit -m “[descriptive message]”
commit your staged content as a new commit snapshot

BRANCH & MERGE
Isolating work in branches, changing context, and integrating changes

git branch
list your branches. a * will appear next to the currently active branch

git branch [branch-name]
create a new branch at the current commit

git checkout
switch to another branch and check it out into your working directory

git merge [branch]
merge the specified branch’s history into the current one

git log
show all commits in the current branch’s history

INSPECT & COMPARE
Examining logs, diﬀs and object information

git log
show the commit history for the currently active branch

git log branchB..branchA
show the commits on branchA that are not on branchB

git log --follow [file]
show the commits that changed file, even across renames

git diff branchB...branchA
show the diﬀ of what is in branchA that is not in branchB

git show [SHA]
show any object in Git in human-readable format

SHARE & UPDATE
Retrieving updates from another repository and updating local repos

git remote add [alias] [url]
add a git URL as an alias

git fetch [alias]
fetch down all the branches from that Git remote

git merge [alias]/[branch]
merge a remote branch into your current branch to bring it up to date

git push [alias] [branch]
Transmit local branch commits to the remote repository branch

git pull
fetch and merge any commits from the tracking remote branch
