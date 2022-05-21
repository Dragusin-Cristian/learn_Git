# Git Cheat sheet:

## Rename a branch:
### Change the name in the local repo:
* go to old_name branch: $ git branch -m new_name
* or outside that branch: $ git branch -m old_name new_name
### Then change the name to the remote repo:
* $ git push origin :old_name new_name

## Delete a branch:
### Delete locally:
* $ git branch -d branch_name
### Delete remote:
* $ git push origin --delete branch_name

## Add a new branch and populate to a remote repo:
* $ git init
* $ git remote add origin [REPO_LINK]
* $ git config --global user.email "you@example.com"
* $ git push --set-upstream origin main // continue even if you get an error
* $ git add .
* $ git commit -m "message"
* $ git branch new_branch_name
* $ git checkout new_branch_name
* $ git add .
* $ git commit -m "real message"
* $ git push

## Copy the main branch to new_branch
* $ git checkout new_branch
* $ git checkout main . // With period
* $ git add --all
* $ git commit -m "Copy from main to new_branch"
* $ git push -u origin new_branch
