# Basics

## Basic Commands

1. Clone a repo from github  
git clone < url copied from github repo >

2. Checkout to a branch  
git checkout < branch-name >

3. Checkout to a new branch  
git checkout -b < new branch name >

4. Fetch all the updates from the remote repo (but your local branches will not be udpated)  
git fetch 

5. Fetch and merge remote udpates (will change your local files)  
git pull = git fetch + git merge  
git pull (pull all branches from remote)  
git pull origin head (pull head branch from remote)  

6. Add local changes to stage  
git add .

7. Commit local changes  
git commit -m "first commit"

8. Push local commits to remote/upstream repo
git push origin head

9. Rebase the current branch with master branch
git rebase master (master branch as a base, and all your local changes on top of that)

If 
