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


## Delete

1. Delete a branch  
git branch -d < branch-name > 

2. Delete a repository (you should on the parent directory):  
 rm -rf < respository >/.git    (delete the git file first)  
 rm -r < repo >   (recursively delete a non-empty directory)  

## Merge

1. Git merge -> failed -> resolve the conflicts first -> then do the merge again  

2. Merge two branches (fast-forward merge):    
Normally we need to be on the receiving branch (often master). We need to ensure the head pointer is pointing to the receiving branch.

git merge branch-1

3. 3-way merge (two branches diverged, both have new commits):  
 git merge branch-1  
 -> manually resolve the conflicts  
 git add .  
 git commit -m 'feat(title): summary'  

## Setup Remote

git remote add upstream git@github.factset.com:cmt/WorkflowManagerApi.git  
git remote add origin git@github.factset.com:yourUserName/WorkflowManagerApi.git  

### Origin vs Upstream

`upstream` generally refers to the original repo that you have forked
`origin` is your fork: your own repo on GitHub, clone of the original repo of GitHub
