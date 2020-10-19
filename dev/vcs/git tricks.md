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