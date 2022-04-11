# Stash

Stash - save the current changes and back to clean working directory

**Save the staged changes:**  
 git stash  
Then you can easily checkout to other branch without committing the changes  

**See your stashed list:**  
 git stash list

**Restore the saved changes:**  
 git stash apply  
The staged changes will be back

**Change the base branch of the PR (E.g. develop -> stage)**  
(First, on GitHub -> PR Edit -> change base branch to stage)  
 git rebase origin/stage  
 git fetch origin  
 git push origin head --force  

**Difference between "git pull" and "git fetch"**  
 git fetch is similar to git pull but doesn't merge.   
Fetch gets the latest updates from origin but doesn't update your local working copy with the changes

**Checkout Remote Branch (will create a local branch with the same name)**  
 git checkout -t origin/< remote-branch-name >

**Check Upstream Branch (the remote branch that your current local branch is tracking)**  
 git branch -vv


**If we init a repo locally and want to push it remotely. Then we need to create remote origin using:**  

git remote add origin git@github.com:< user >/< repository >.git

**Push commits to the remote branch, origin means remote:**  
 git push origin master

**Clone a repo will automatically set up the origin remote.**  


**If two branches diverged (another way to do it):**  
 git checkout feature-branch
 git rebase master     -> (让feature-branch先实现master branch的changes)
 git merge master?    -> (再将master并进feature branch)


## Difference between Fork & Clone:
### Fork: 
you copy a repo from others' work remotely  
 a pull request is required to make changes to the origin master  
 the author will need to review and approve your pull request to reflect the changes  
### Clone: 
you copy a repo locally  
you just need to pull the changes to the origin master  

