Git Basic Commands

Basic Git configuration
git config --global user.name <username>
  
git config --global user.email <email>

Initialize a empty Git Repository
  
git init 

Displays all hidden folders within repository  
ls -lart 

Display status of the tracked/untracked files  
git status 

Add file in the staging area  
git add <FILE> 

Git converts tracked to untrack mark  
git rm --cached <FILE> 
  
Add all files present in current directory to staging area  
git add . 

Taking snapshot of the files in staging area 
git commit -m msg 
  
match files with the last commit  
git checkout <FILE> 

all files matched with the last commit  
git checkout -f 

history of commits  
git log 
  
Displays desired number of last commits
git log -p -<number> 
  
Compares working tree to staging area  
git diff
  
Compares Last commit to staging area  
git diff --staged 
  
without adding files to staging area..direct commit  
git commit -a -m <msg> 

.gitignore : add files here that we dont want Git to commit
  
Create a branch  
git branch <branch_name>

Know number of branches
git branch
  
merge branch with main branch  
git merge <branchname> 
  
create a new branch and chekouts to that branch directly 
git checkout -b <newbranchname> 

Add remote repository named as origin  
git remote add origin <url> 

Rebase with the master branch  
git rebase master  
  
 Basic Difference between The merge and rebase
  
    Rebase “reapplies commits on top of another base branch”, whereas merge “joins two or more development histories together”. 
    In other words, the key difference between merge and rebase is that while merge preserves history as it happened, rebase rewrites it.
