# Squash and Merge to Stage
-  git checkout stage  OR  git checkout -t origin/stage
-  git fetch origin -> git pull origin
-  git push origin head (after your implementation done)
-  Squash and Merge (after approved)
	
# Merge Back to Dev
-  git checkout stage
-  git fetch origin/git pull origin
-  git branch -vv (double check the upstream branch and current head is correct)
-  git checkout -b merge-back-to-dev
-  git push origin head
-  create PR and copy paste the title and description
  
 ensure you Merge Commit the PR
