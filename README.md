# git_commands
A list of useful git commands

## Basic commands

### Clone a remote repository
git clone <repository_URL>

### Add changes to the staging area
git add <file>

## Commit changes
git commit -m "Commit message"

## View the current status of the repository
git status
git status -s

## View the commit history
git log
git log --stat
git log --oneline

## Commands for working with branches 

### Create a new branch
git branch <branch_name>

### Switch to a specific branch
git checkout <branch_name>

## Push changes to the remote repository
git push origin <branch>

## Update the local repository with remote changes
git pull origin <branch>

## Merge changes from one branch to another
git merge <branch_name>
