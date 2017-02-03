# git_cheatsheet
A list of commonly used git commands

## Branches

### Listing

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

### Getting stuff

Retrieve a specific file (or files) from another branch:
```
git checkout <branch_name> -- <file_paths>
```

### Deleting

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

Show diff between a local file and a remote file that may be on different paths (files are in different folders):
```
git diff remotename/branchname:path/to/file.txt other/path/to/file.txt
```
OR
```
git diff HEAD:other/path/to/file.txt remotename/branchname:path/to/file.txt
```

Show a summary of files changed between two branches
```
git diff --name-status branch1..branch2
```
... or to compare against the current branch:
```
git diff --name-status ..otherBranch
```

## Remotes
Add a remote:
```
git remote add remoteName git://github.com/user/repo.git
git fetch remoteName
```

## Commits
Change the commit message (amend) the most recent commit on the current branch:
```
git commit --amend
```

## Undoing things
Revert changes to a file by pulling that file from another branch:
```
git checkout branchname -- path/to/file.js
```
