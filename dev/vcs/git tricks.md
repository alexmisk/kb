### Force “git pull” to overwrite local files

```
git fetch --all && git reset --hard origin/master
```

### Add only modified files
```
git add -u
```

### Open all modified files in vim
```
vim $(git status --porcelain | awk '{print $2}')
```

### Checkout and work in a remote branch
```
git checkout --track origin/daves_branch
```

### Add a fixup commit
```
git commit -a --fixup <commit hash>
git rebase --autosquash -i <base>
```