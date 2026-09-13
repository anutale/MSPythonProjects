Linux Commands :

Linux Command # 1 

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
