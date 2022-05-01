# How do fetch, pull, and push differ?

- `git fetch` - download all changes from a remote repo into your local repo.
- `git pull` - download all changes from a remote repo into your local repo and merge them into a tracked local branch.
- `git push` - upload all changes from a local repo to a remote repo.

## Git fetch
`git fetch` looks all changes made in the **remote repo** and downloads them into your **local repo**. The code in your tracked **local branch** does not change. 
Note: Use ‘git merge’ to make changes to a tracked **local branch** after reviewing & confirming the details fetched. 


## Git pull
`git pull` performs a `git fetch` followed by a `git merge` into a tracked **local branch**. The code is updated immediately.
Note: Confirm that you understand the changes being made prior to using `git pull`. You cannot review the changes locally beforehand.


## Git push
`git push` uploads all changes made in your **local repo** to the **remote repo**. Code is shared with a remote repository to replicate the changes made locally. 
Note: Pushing will fail if commits in the **remote branch** are not in your **local branch**. Resolve this by synchronizing the **local branch** with the **remote branch** with either `git pull` or `git fetch` and `git merge`.
