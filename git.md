### Undo last commit without losing changes
```
git reset --soft HEAD~1
```

---

### Change branch name
```
git branch -m new-branch-name
```

---

### Reject changes in current directory
```
git checkout -- .
```

---

### Revert to specific commit
```
git reset --hard commit-hash
git stash -u
git push -f origin/current-branch-name
```
