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
