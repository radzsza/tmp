Aleksandra Radziukiewicz  
08-04-2025  
# Short git(hub) tutorial

## What is git(hub)?

### Git

Version control system.

### github

A platform allowing developers to:  
* create  
* store  
* manage  
* share  

their code. It is often used for collaboration in programming projects or to share open access code.  

## Getting started with a new repo

I am going to skip steps like "log in" or "click here"  

### github
1. Create a repo  
2. Copy https or ssh url (depends on what you use - I used https and PAT)
### terminal  
1. `git config --global user.name "username"`, `git config --global user.email <emai>`  
2. In the designated directory - `git init`  
Linking with the github repo:  
3. `git remote add origin <repo-url>`  
Commiting the changes:  
4. `git add <filename/.>`  
5. `git commit -m "message"`  
Push:  
6. `git push origin <branch-name>`  
7. enter username and access token

## Access tokens

Github disabled password authentication - you have to use either SSH 
or Personal Access Token. You just put it instead of the password in 
step 7.  

## Restoring

1. `git log` to see all the commits  
2. make a new branch `git branch <name>`  
3. `git checkout <ID>` where ID is commit ID we want to restore  
4. make changes  
5. commit and push changes  
6. merge

## Conflicts

In case of conflict between 2 branches (ie the same file has 
differences and git doesn't know which one is correct) - the merge 
conflict already occurred  

1. `git log --merge`  
2. find the section with `<<<<<<<` and `>>>>>>>`  
3. decide between the differentiated parts  
4. add, commit, push  

## Pull and fetch

In most cases `git pull <repo-url>` works fine. If there are 
conflicts, ie file was edited on 2 separate machines and git blocks 
`pull`:  
1. `git fetch <name>` to download the changes  
2. `git merge <branch-name>` - current branch is the deafult to merge the second branch with  
Pull is fetch and merge combined.

## Basic commands

* `git init` - starts a local repo  
* `git clone` - clones a remote repo locally (I also used `git remote add origin <url>`)  
* `git status` - shows modified files  
* `git add <name/.>` - add a file/all files in a directory to next commit  
* `git commit -m "message"` - new commit snapshot of added files  
* `git branch <optional-name>` - creates a new branch  
* `git checkout <name>` - switch to another branch  
* `git merge <branch>` - merge specified branch with current  
* `git log` - all commits in the current branch (commit history)  
* `git fetch` - downloads a repo to local  
* `git pull` - download a repo and merge with local  

