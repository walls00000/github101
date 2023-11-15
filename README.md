# github101

Repository to learn git

## Clone a repository

`git clone <repo-url>`

## Add to a change list

`git add <file> [<file>]`

## Commit changes

`git commit -m"<message>"`

## Obtain the status of your local repository

`git status`

## Push changes to a remote (origin)

`git push <remote> <branchname>`

### Push changes to the main branch to origin

`git push origin main`

## Fetch all changes from origin to your repository (including other branches)

`git fetch origin`

## Pull upstream changes from origin

`git pull`

## Checkout a local branch

`git checkout -b <branchname>`

## Show local branches

`git branch`

## Show all branches (local and remote)

`git branch -a`

## Push a branch to origin

`git push -u origin <branchname>`

## Checkout a local branch and set the upstream branch to remote (main)

`git chekout -b <branchname> --track origin/main`

## Show a diff between local changes and committed changes

`git diff <filename>`

## Merge changes from origin/<branch> into your local branch

`git merge origin/<branch>`

## Rewrite local history using origin/<branch> to compare

**_WARNING_** data loss: rewriting history can lose data

**_Note:_** to push changes after a rebase the `--force` argument to the `git push` command is required

`git rebase -i origin/<branch>`

## Reset a branch to the head at origin/<branch>

**_WARNING_** data loss: This command will _forget_ all local changes

`git reset --hard origin/<branch>`
`git reset --hard origin/HEAD`
