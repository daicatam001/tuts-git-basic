# GIT BASIC


## Concept

#### Detached HEAD

When checkout specific commit

#### Reset Command

Reset HEAD of the branch (undo commit)

## Config

### Global config

```
git config --global user.email "you@example.com"
git config --global user.name "You"
```

## Basic

### Check specific commit

```
git checkout [hash]
git checkout [branch_name] // back to latest commit on brach
```

### Quit log

```
q
```

### Merge

```
git merge [other_branch]
```

### Create branch

```
git branch [branch_name]
git checkout [branch_name] / git switch [branch_name]
// Or
git checkout -b [branch_name]
// Or
git switch -c [branch_name]

```

### Delete branch

```
git branch -D [branch_name] [branch_name2]
```


### Show branchs

```
git branch
```


### Show list track files

```
git ls-files
```

### Remove file

```
git rm [file_name]
```


### Revert unstage file

```
git checkout [filename]
git checkout . // revert all
// Or
git restore [filename]
git restore . // revert all
```

### Delete untrack file

```
git clean -dn // would remove all
git clean -dn [filename] // would remove file

git clean -df  // remove all without asking
git clean -df [filename] // remove file without asking
```

### Undo stage changes

```
git restore --staged // unstage all
git restore --staged [filename] // unstage file
```

### Reset HEAD

```
git reset --soft HEAD~[number_of_commit] // undo commit to staged area
git reset HEAD~[number_of_commit] // undo commit to unstaged area
git reset --hard HEAD~[number_of_commit] // undo commit and remove all changed
```