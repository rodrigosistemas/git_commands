# git_commands
<img src="https://github.com/rodrigosistemas/git_commands/blob/main/images/Git-logo.png" alt="Git Logo" widht="300" height="200">

## Basic commands

### Clone a remote repository
```bash
git clone <repository_URL>
```

### Add changes to the staging area
```bash
git add <file>
```

### Commit changes
```bash
git commit -m "Commit message"
```

### View the current status of the repository
```bash
git status
```
```bash
git status -s
```

### View the commit history
```bash
git log
```
```bash
git log --stat
```
```bash
git log --oneline
```

### Deleting a file from the repository and the file system
```bash
git git rm <nombre_del_archivo>
```
```bash
git rm --force <nombre_del_archivo>
```

### Remove a file from the repository but keep it in the file system
```bash
git rm --cached <nombre_del_archivo>
```

<br>

## See the difference between one version and another

### View changes made in the last two commits
```bash
git show <hash_del_commit>
```

### View changes from one commit version to another
```bash
git diff <commit1> <commit2>
```

<br>

## Commands for working with branches 

### Create a new branch
```bash
git branch <branch_name>
```

### Switch to a specific branch
```bash
git checkout <branch_name>
```

### Push changes to the remote repository
```bash
git push origin <branch>
```

### Update the local repository with remote changes
```bash
git pull origin <branch>
```

### Merge changes from one branch to another
```bash
git merge <branch_name>
```

### Undo all changes in staging area
```bash
git reset
```

### Undo last commit and keep changes
```bash
git reset HEAD~
```

### Undo last commit and delete changes
```bash
git reset --hard HEAD~
```

<br>

## Uplodad project to Github

### Add the remote repository
```bash
git remote add origin <URL_del_repositorio>
```

### Upload your changes to Github
```bash
git push -u origin main
```

<br>

## Tags

### Creation of a tag
```bash
git tag v1.0
```
```bash
git tag v1.0
```

### List of all tags
```bash
git tag
```

### Delete a tag
```bash
git tag -d v1.0
```

<br>

## Solving common erros

### Solve conflict Git Error | Github Error: failed to push some refs to '[REPO URL]'
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

## Temporarily save local changes

### Save changes in the stash
```bash
git stash
```
```bash
git stash -m "Stash message"
```

### View a list of stashes
```bash
git stash list
```

### Apply stash changes
```bash
git stash apply
```

### Delete a stash
```bash
git stash drop <identificador_del_stash>
```

### Apply and remove stash in a single step
```bash
git stash pop
```
