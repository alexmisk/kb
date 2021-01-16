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

### Remove all tags
```
#Delete local tags.
git tag -l | xargs git tag -d

#Fetch remote tags.
git fetch

#Delete remote tags.
git tag -l | xargs -n 1 git push --delete origin

#Delete local ta
git tag -l | xargs git tag -d
```