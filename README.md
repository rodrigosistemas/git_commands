# git_commands
<img src="https://github.com/rodrigosistemas/git_commands/blob/main/images/Git-logo.png" alt="Git Logo" widht="300" height="200">

## Basic commands

#### List configuration
```bash
git config -l
```
#### Config username
```bash
git config --global user.name ""
```
#### Config email
```bash
git config --global user.email 
```
#### Check the current editor
```bash
git config --get core.editor
```
#### Set vscode as default editor
```bash
git config --global core.editor "code --wait"
```
#### Set nano as default editor
```bash
git config --global core.editor nano
```
#### Open default editor
```bash
git config --global -e
```
#### Autocrlf configuration Windows
```bash
git config --global core.autocrlf true
```
#### Aurocrlf configuration Linux/Mac
```bash
git config --global core.autocrlf input
```

<br>

### SSH local keys configuration

#### Generate a new SSH key: (Any operating system)
```bash
ssh-keygen -t rsa -b 4096 -C "youremail@example.com"
```

#### Check process and add it (Windows/Linux)
```bash
eval $(ssh-agent -s)
```
```bash
ssh-add ~/.ssh/id_rsa
```

<br>

#### Clone a remote repository
```bash
git clone <repository_URL>
```

#### Add changes to the staging area
```bash
git add <file>
```

#### Commit changes
```bash
git commit -m "Commit message"
```

#### Modify commit
```bash
git commit --amend -m "Change version"
```

#### View the current status of the repository
```bash
git status
```
```bash
git status -s
```

#### View the commit history
```bash
git log
```
```bash
git log --stat
```
```bash
git log --oneline 
```
```bash
git log --oneline --all --graph
```

#### Return to a specific deleted commit
```bash
git reset --hard <commit_hash>
```
```bash
git reset --soft <commit_hash>
```

#### Deleting a file from the repository and the file system
```bash
git git rm <file_name>
```
```bash
git rm --force <file_name>
```

#### Remove a file from the repository but keep it in the file system
```bash
git rm --cached <file_name>
```

<br>

### See the difference between one version and another

#### View changes made in the last two commits
```bash
git show <ccommit_hash>
```

#### View changes from one commit version to another
```bash
git diff <commit1> <commit2>
```

<br>

### Commands for working with branches 

#### Create a new branch
```bash
git branch <branch_name>
```

#### Create a new branch
```bash
git checkout -b <branch_name>
```

#### All remote branches are displayed
```bash
git branch -r
```
#### All branches both local and remote are shown
```bash
git branch -a
```

#### Delete a branch
```bash
git branch -d <branch_name>
```
#### Force branch deletion
```bash
git branch -D <branch_name>
```

#### Switch to a specific branch
```bash
git checkout <branch_name>
```
```bash
git switch <branch_name>
```

#### Push changes to the remote repository
```bash
git push origin <branch>
```

#### Update the local repository with remote changes
```bash
git pull origin <branch>
```

#### Merge changes from one branch to another
```bash
git merge <branch_name>
```

#### Attatch new branch
```bash
git rebase <branch_name>
```
#### Reset changes (private branches)
```bash
git reset
```

#### Undo current changes and roll back one commit
```bash
git reset --hard HEAD~1
```

#### Keeps current changes and roll back one commit
```bash
git reset --soft HEAD~1
```

#### Restore git commmit
```bash
git reset --hard <commit_hash>
```

#### Revert changes (public branches)
#### Push a new commit which reverts the pushed commit
```bash
git revert <commit_hash>
```

#### Header pointer history
```bash
git reflog
```

<br>

### Uplodad project to Github

#### Add the remote repository
```bash
git remote add origin <Repository_URL>
```

#### View the current remote repository
```bash
git remote -v
```

#### Upload your changes to Github
```bash
git push -u origin main
```

<br>

### Tags

#### Creation of a tag
```bash
git tag <tag_name>
```

#### Creation of a tag with message
```bash
git tag -a <tag_name> -m "Message"
```

#### List of all tags
```bash
git tag
```

#### View detailed information of a tag
```bash
git show <tag_name>
```

#### Sharing tags with a remote repository:
```bash
git push origin <tag_name>
```

#### Delete a tag
```bash
git tag -d <tag_name>
```

#### Delete a tag in the remote repository
```bash
git push --delete origin <tag_name>
```

<br>

### Solving common erros

#### Solve conflict Git Error | Github Error: failed to push some refs to '[REPO URL]'
```bash
git pull --rebase origin main
```
```bash
git log
```
```bash
git push -u origin main
```

<br>

### Temporarily save local changes

#### Save changes in the stash
```bash
git stash
```
```bash
git stash -m "Stash message"
```

#### View a list of stashes
```bash
git stash list
```

#### Apply stash changes
```bash
git stash apply
```

#### Delete a stash
```bash
git stash drop <identifier_stash>
```

#### Apply and remove stash in a single step
```bash
git stash pop
```

<br>

### Cherry pick
```bash
git cherry-pick <commit_hash>
```

<br>

### Teamwork
#### Shows how many commits each team member has made
```bash
git shortlog
```
#### Shows how many commits have been made by each team member up to those that have been eliminated
```bash
git shortlog -sn -all
```
#### Shows how many commits each member has made by removing the deleted ones without the merges
```bash
git shortlog -sn -all --no-merges 
```
#### Shows who did what line by line
```bash
git blame <file_name>
```
```bash
git blame <file_name> -<Lxx><xx>
```
