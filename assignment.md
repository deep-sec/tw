# How do fetch, pull, and push differ?

- `git fetch` - download all changes from a remote repo into your local repo.
- `git pull` - download all changes from a remote repo into your local repo and merge them into a tracked local branch.
- `git push` - upload all changes from a local repo to a remote repo.

## Git fetch
`git fetch` looks at all changes made in the **remote repo** and downloads them into your **local repo**. The code in your tracked **local branch** does not change. 

Note: Review & confirm the details fetched. Then use `git merge` to make changes to a tracked **local branch**. 


## Git pull
`git pull` performs a `git fetch` followed by a `git merge` into a tracked **local branch**. The code will update immediately without review.

Note: Confirm the changes before using `git pull` since there is no local review available.


## Git push
`git push` uploads all changes made in your **local repo** to the **remote repo**. This command shares code with a remote repository to replicate the local changes.

Note: Pushing will produce an error if commits in the **remote branch** are not in your **local branch**. Resolve the issue:
1. Synchronize the **local branch** with the **remote branch**.
2. Use either `git pull` or `git fetch` and `git merge`.
3. Enter `git push` to complete the process.
