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
