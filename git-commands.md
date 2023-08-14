### Create new branch and switch to it

```
git branch <new-branch> # `git branch` lists all branches
git checkout <new-branch>
```

### Include files in commit

```
git add <file1> <file2>
```

### Sync local repo with remote

```
git pull
```

### Unstage changes (so they're not included in commit)

```
git restore --staged <file1> <file2>
```

### Push branch and set remote as upstream

```
git push --set-upstream origin <branch-name>
```