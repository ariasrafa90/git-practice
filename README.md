# Practice repository to start learning Git

- git init: Create a new repository
- git status: Compare working directory, staging area, and current branch
- git add: Add changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: Set or get configuration
- git log: Show history (aka "log") of project commits
- git stash: Stash changes from working directory
- git stash list: List stashes
- git stash pop: Apply stashed changed to working directory
- git checkout: Check out the branch (update HEAD and apply changes to working directory)
- git branch -c: Create a branch
- git checkout -b: Create a branch, then check it out.
- git branch: List branches
- git merge: Merge changes from different branches
- git remote add <remote> <url>: Add a new <remote> at <url>
- git remote -v: List remote repositories
- git push -u <remote> <branch>: Push <branch> to <remote>, and set default upstream for a branch.
- git fetch: Fetch changes from remote repository
- git pull: Fetch, and then merge


## Commit messages

Default editor is vim (this can be changed)
- `i` to enter *insert* mode
- Type commit message
- `Escape` -> `:wq` -> `Enter` to write message and quit Or use `git commit -m "<message>"`

- First line should be clear, accurate and concise
- Use proper spelling, grammar and punctuation
- Don't end with `.`


## Merging

Merging means to bring the changes from one branch to another.

- A fast-forward merge happens when the target branch was branched from the current one, and there are no new changes to the current branch since then.
- An Automatic merge happens when the two histories have diverged, but git is able to reconcile them into one set of changes. This creates a new commit on the current branch.


## Whats a remote?

A remote repo is one hosted somewhere other than our local machine. We can add remotes with `git remote add`, and set up *tracking branches* to track difference between local and remote repositories.

We push to remote with `git push`, and fetch from them with `git fetch`. We can also fetch and then merge with `git pull`.
