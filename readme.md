## Mastering Git

### Add files and commit them to git

```
git add .
git commit -m "Added files"
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

Now the head will poin to this branch

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
