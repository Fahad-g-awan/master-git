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
