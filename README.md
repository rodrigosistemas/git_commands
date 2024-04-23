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
