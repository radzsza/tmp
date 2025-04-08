Aleksandra Radziukiewicz  
08-04-2025  
# Short git(hub) tutorial  

<details>

<summary> What is git(hub)? </summary>  
### Git  
Version control system.
### github
A platform allowing developers to:  
* create  
* store  
* manage  
* share  

their code. It is often used for collaboration in programming projects or to share open access code.  

</details>

<details>

<summary> Getting started with a new repo </summary>

I am going to skip steps like "log in" or "click here"

### github
1. Create a repo  
2. Copy https or ssh url (depends on what you use - I used https and PAT)
### terminal  
1. `git config --global user.name "username"`, `git config --global user.email [emai]`  
2. In the designated directory - `git init`  
Linking with the github repo:  
3. `git remote add origin [repo-url]`
Commiting the changes:  
4. `git add [a specific file or .]` to track newly created files (not tracked before)  
5. `git commit -m "message"` to commit changes in already tracked files  
Push:  
6. `git push origin [master/main]`  
7. enter username and access token

</details>

<details>

<summary> Access tokens </summary>

### Private access token

TODO

### Fine-grained tokens

TODO

</details>

