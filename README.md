## Basic Commands
> git init

Starts a local working directory

> git add file_name

Adds modified and untracked files to the staging area

> git commit -m "Commit message"

Commits your changes

## Cloning Repositry

> git clone https://github.com/libgit2/libgit2

Creates a directory named libgit2, initializes a **.git** directory inside it, pulls down all the data for that repository

## Reseting Files

> git checkout HEAD file_name | git checkout -- file_name

Restores the file in your working directory to look exactly as it did when you last made a commit. Discards changes in the working directory

> git reset HEAD file_name

Resets the file in the staging area to be the same as the HEAD commit. It does not discard file changes from the working directory, it just removes them from the staging area

> git reset commit_SHA

Resets to a previous commit, using the first 7 characters of one of the past commit *SHAs* in your Git log. The **HEAD** commit has been reassigned. You just changed history! HEAD goes to a previously made commit of your choice. Commits after that are no longer part of your project

## Git Branching

> git branch

Lists all a Git project’s branches. In the output, notice the * over the current branch

> git branch branch_name

Creates a new branch

> git checkout branch_name

Switches from one branch to another

> git merge branch_name

Merges *branch_name* into master. *(We must be on the reciever branch)*

> git branch -d branch_name | git branch -D branch_name *if branch_name was never merged*

Deletes the branch specified. After the branch has been integrated into master, it has served its purpose and can be deleted

## More Commands

> git diff file_name

Shows the differences between the file on your working directory and the staging area

> git show HEAD

Shows the most recently made commit

> git add file_name1 file_name2

Adds the files to the staging area together using a single git command. (Shortcut: *git add .*)