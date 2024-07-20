# Git Basics CheatSheet
The cheatsheet is broken down into sections of code, followed by their output.

## SETUP

``` git
git config --global user.name “[firstname lastname]”
```

``` git
git config --global user.email “[valid-email]”
```

``` git
git config --global color.ui auto
```

```git
git init
```

```git 
git clone [url]
```

## Staging

``` git
git status
```

``` git
git add [file]
```

``` git
git reset [file]
```

``` git
git diff
```

``` git
git diff --staged
```

``` git
git commit -m 'Commit message'
```

## Branches

```git
git branch
```

``` git
git branch [branch_name]
```

```git
git checkout
```

```git
git merge [branch_name]
```

``` git
git log
```

## Insepction

``` git
git log
```

```git 
git log branch_2..branch_1
```

```git
git log --follow [file]
```

```git
git diff branch_2...branch_1
```

```git
git show [SHA]
```

