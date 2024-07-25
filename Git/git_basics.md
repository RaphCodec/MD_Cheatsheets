# Git Basics CheatSheet
The cheatsheet is broken down into sections of code, followed by their output.

## SETUP

Set the username to be associated with each history marker

``` bash
git config --global user.name “[firstname lastname]”
```

Set the email to be associated with each history marker
``` bash
git config --global user.email “[valid-email]”
```

Set automatic command line coloring
``` bash
git config --global color.ui auto
```

Initilize a Repository
``` bash
git init
```

Clone a Repository into the current directory via a url
``` bash 
git clone [url]
```

## Staging

Show modified files in the working directory, both staged and unstaged for the next commit
``` bash
git status
```

Add a file to the stage in it's current state for the next commit
``` bash
git add [file]
```

Add all current directory changes to stage.
``` bash
git add .
```

Add all current directory changes to stage, excluding new files and hidden directories
``` bash
git add *
```

Unstage a file while keeping the current changes
``` bash
git reset [file]
```

See the changes of files that have changed but are not staged
``` bash
git diff
```

See the chnages of files that have changed and are staged
``` bash
git diff --staged
```

Commit your staged files as a new commit snapshot
``` bash
git commit -m 'Commit message'
```

## Branches

Show a list of your branches. A * will appear next to the branch that is currently active
``` bash
git branch
```

Create a new branch at the current commit
``` bash
git branch [branch_name]
```

Switch to another branch
``` bash
git checkout [branch_name]
```

Create a new brancher and switch to it
``` bash
git checkout -b [branch_name]
```

Merge a branch into the branch that is currently checked out
``` bash
git merge [branch_name]
```

See branch history
``` bash
git log
```

## Insepction

See commit history on current branch
``` bash
git log
```

See the commits that are on on branch_1 but not branch_2
``` bash 
git log branch_2..branch_1
```

Show the commits for a specific file. including file renames
``` bash
git log --follow [file]
```

See the diff of what is in branch_1 but not in brnach_2
``` bash
git diff branch_2...branch_1
```

Show any Git object in a human-readable format
``` bash
git show [SHA]
```

## Sharing/Updating

Add a url with an alias
``` bash
git remote add [alias] [url]
```

get all the branches down from a remote
``` bash
git fetch [alias]
```

Merge a remote branch into the current local branch to bring it up to date
``` bash
git merge [alias]/[branch]
```

Send local branch commits to a remote branch
``` bash
git push [alias] [branch]
```

Fetch and merge remote branch commits into a local tracking branch
``` bash
git pull
```

Git pull from a specific remote branch
```
git pull [remote_name] [branch_name]
```

## Path Changes

Delete a file and stage the deletion for a commit
``` bash
git rm [file]
```

Move a file to a new directory and stage the change
``` bash
git mv [existing-path] [new-path]
```

Show logs of paths that have moved
``` bash
git log --stat -M
```

## Rewrite History

Apply commits of the current branch ahead of a specififed branch
``` bash
git rebase [branch]
```

Clear staging area and re-write working-tre history from a specified commit
``` bash
git reset --hard [commit]
```

## Temporary Commits

Save modified and staged changes
``` bash
git stash
```

List stack-order of stashed file changes
``` bash
git stash list
```

Get files out of stash and back into working area
``` bash
git stash pop
```

delete files in stash
``` bash
git stash drop
```

## Git Ignore Patterns

Prevent files and direcotries with certain patterns from being saved by Git.

`logs/` ingores all files and sub-folders in the logs folder

`*.notes` ignores all files with the extension .notes

`pattern*/` ignores all folders whore name starts with pattern
``` bash
logs/
*.notes
pattern*/
```

System wide ignore patern for all local repositories
``` bash
git config --global core.excludesfile [file]
```