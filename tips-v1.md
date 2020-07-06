# Remove all local branches
git branch --merged | grep -v \* | xargs git branch -D 
git branch --merged master --no-color | grep -v master | grep -v stable | xargs git branch -d
https://stackoverflow.com/questions/10610327/delete-all-local-git-branches

# Remove deleted branch names from terminal autocomplete
git fetch --prune --all
https://stackoverflow.com/questions/17933401/how-do-i-remove-deleted-branch-names-from-autocomplete