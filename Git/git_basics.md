# Git Basics CheatSheet
The cheatsheet is broken down into sections of code, followed by their output.

## SETUP

``` bash
git config --global user.name “[firstname lastname]”
```

``` bash
git config --global user.email “[valid-email]”
```

``` bash
git config --global color.ui auto
```

``` bash
git init
```

``` bash 
git clone [url]
```

## Staging

``` bash
git status
```

``` bash
git add [file]
```

``` bash
git reset [file]
```

``` bash
git diff
```

``` bash
git diff --staged
```

``` bash
git commit -m 'Commit message'
```

## Branches

``` bash
git branch
```

``` bash
git branch [branch_name]
```

``` bash
git checkout
```

``` bash
git merge [branch_name]
```

``` bash
git log
```

## Insepction

``` bash
git log
```

``` bash 
git log branch_2..branch_1
```

``` bash
git log --follow [file]
```

``` bash
git diff branch_2...branch_1
```

``` bash
git show [SHA]
```

## Sharing/Updating

``` bash
git remote add [alias] [url]
```

``` bash
git fetch [alias]
```

``` bash
git merge [alias]/[branch]
```

``` bash
git push [alias] [branch]
```

``` bash
git pull
```

```
git pull [remote_name] [branch_name]
```

## Path Changes

``` bash
git rm [file]
```

``` bash
git mv [existing-path] [new-path]
```

``` bash
git log --stat -M
```

## Rewrite History

``` bash
git rebase [branch]
```

``` bash
git reset --hard [commit]
```

## Temporary Commits

``` bash
git stash
```

``` bash
git stash list
```

``` bash
git stash pop
```

``` bash
git stash drop
```

## Git Ignore Patterns

``` bash
logs/
*.notes
pattern*/
```

``` bash
git config --global core.excludesfile [file]
```