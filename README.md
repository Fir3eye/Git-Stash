# Git Stash Command Guide

The `git stash` command allows you to temporarily save your uncommitted changes without committing them to the repository. It helps in situations where you want to switch branches or work on something else without committing incomplete work.

## Table of Contents
1. [Basic Usage](#basic-usage)
2. [Listing Stashes](#listing-stashes)
3. [Showing Stash Data](#showing-stash-data)
4. [Applying Stashes](#applying-stashes)
5. [Dropping Stashes](#dropping-stashes)
6. [Creating Named Stashes](#creating-named-stashes)
7. [Restoring Untracked Files](#restoring-untracked-files)

---

## Basic Usage

To stash your current changes (both staged and unstaged):

```bash
git stash
```
- Listing Stashes
```
git stash list
```
- Showing Stash Data
```bash 
git stash show
```
- Full Diff (Detailed View):
```
git stash show -p
```
- Full Diff (Detailed View): specific stash
```
git stash show -p stash@{1}
```
- Applying Stashes
```
git stash apply
```


- To apply a specific stash:
```
git stash apply stash@{n}
```


- Dropping Stashes
```
git stash drop stash@{n}
```


- To drop the most recent stash:
```
git stash drop
```


- Creating Named Stashes
```
git stash push -m "WIP: Refactor login module"
```

- Restoring Untracked Files
```
git stash push -u
```

- Applies the last stash 
```
git stash pop
```
- Clearing All Stashes:
```
git stash clear
```
