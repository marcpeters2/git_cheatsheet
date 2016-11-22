# git_cheatsheet
A list of commonly used git commands

## Branches
List local branches:
```
git branch
```

List remote branches:
```
git branch -r
```

List all local and remote branches:
```
git branch -a
```

Delete local branch:
```
git branch -d <branch_name>
```

Delete remote branch:
```
git push origin --delete <branch_name>
```

## Diffs
Show diff between the current branch and another branch:
```
git diff other_branch..
```
