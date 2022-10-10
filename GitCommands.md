# Git Commands

---

### Basics:

`ls` list all files/directories

`cd <directory>` move into specified directory

`cd ..` move out of current directory to one before

`tab` autofill the rest of the file name

### Git:

`git status` returns status of current branch, use often

`git log` shows entire history of repo

`git diff` shows all changes to a code file

`git reset HEAD` unstage changes to previous version

`git reset HEAD~1`unstage changes to version before the previous

### Repositories:

`git init <repo name>` Creates a new repository locally

`git remote -v` checks the remote origin repo connected 

`git remote add origin <url>` sets a repo as origin

### Config:

`git config --global user.name "<Full name>"` attaches github name onto local

`git config --global user.email <email>` attaches github email onto local

`git config --list` shows name and email attached to local

---

### Clone:

`git clone <repo url>` clones entire repo onto local

`git clone <repo url> -b <branch name>` clones only the specified branch onto local

### Fetch:

`git fetch <url> <remote branch>:<local branch>` downloads remote banch onto local machine, creating local branch simultaneously 

### Pull:

`git pull` download changes from remote repo to local machine

---

### Add:

`git add <file name>` adds specified file

`git add .` adds all files in the directory

### Commit:

`git commit -m "<list changes>"` commits files, must add a descirption of why 

`git commit -am "<list changes>"` shortcut for files already added

`esc` `:wq!` `enter` escape from popup if you forget to add description

### Push:

`git push <url> <branch>` push changes on local up to remote repo

`git push origin <branch>` if origin repo is already set

`git push --set-upstream <url name> <branch name>` connect a local branch to a specific remote branch

`git push -u <url name> <branch name>` shorthand

`git push -u origin <branch>` shorthand if origin already set

---

### Branch:

`git branch` lists all branches in the repo

`git branch -d <branch name>` deletes named branch, cannot be on that branch at the time

### Checkout:

`git checkout <branch name>` switches to specified branch 

### Merge:

`git merge <branch>` combines all updated changes from branch specified to one currently on

---
