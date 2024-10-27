## Mastering Git

### Add files and commit them to git

```
git add .
git commit -m "Added files"
```

### See which files are not staged

```
git status
```

Command shows the differences between your working directory and the staging area (index). It’s useful to review changes that are not yet staged for commit.

```
git diff
```

### To see staged changes

```
git diff --cached
or
git dif --staged
```

This command shows the differences between the staged changes and the last commit.

Alternatively, if you just want to see a list of staged files without their content.

```
git diff --name-only --cached
```

### To unstage a file

```
git restore --staged filename
```

### Remove a file from tracking and from git

```
git rm --cached filename
git commit -m "Remove filename"
git push
```

### To see logs of previous commits

This will show the informaiton about the author, time and commit message along with the commit hash or ID

```

git log
or
git log --oneline
or
git log --oneline --graph --all --decorate

```

### To see changes or state of another commit

Now the head will point to this branch

```

git checkout <commit_hash>

```

### If any changes you made in the deacthed head and you don't want them in the main head

```

git checkout -f main

```

### To list global configuration

```

git config --global --list

```

### Add a Remote URL (if there isn’t already one)

```

git remote add origin git@github.com-account1:username/repo.git

```

### Set the Remote URL for an Existing Repository:

```

git remote set-url origin git@github.com-account1:username/repo.git

```

### Push your local changes to remote

```

git push -u origin

```

### Check connection

```

ssh -T git@github.com

```

### Verify the Remote URL

```

git remote -v

```

### List SSH Keys

```

ls -l ~/.ssh

```

### Create new branch

```

git branch feat/branch

```

### Create and checkout to new branch

```

git checkout -b feat/branch

```

### To create a new banch from a specific branch which you want to make the source of new branch

```

git branh new-branch source-branch

```

### To show all branches

```

git branch

```

### Prune Deleted Remote Branches

Use the --prune option with git fetch to remove any references to branches that no longer exist on the remote

```

git fetch --prune

```

Verify the Branch is Gone

```

git branch -r

```

Optional Cleanup (if still showing locally)

```

git branch -d branch-name

```

### To merge a branch into current branch

```

git merge branch-name

```

### To fix a code or to go to a specific commit where code was working fine

```

git reset <commit_hash>

```

This is a mix-reset and changes made after that commit become unstaged for you to either keep them or discard them.
After that we can push our changes to that branch and for that there are two ways:

- Force push and update remote

```

git push -f origin branch_name

```

- Or first pull and resolve confict and then push

```

git pull

```

### To save the current satged or unstaged changes before doing another pull or fix

```

git stash

```

And to view the stash list and go back to specifix stash

```

git stash list
git stash apply stash_name

```

```

```
