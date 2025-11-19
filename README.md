# crispy-system
Everything we have learnt about git

# Revert Reset and Restore


## Revert
```git
git revert commitiD
```
Revert finds the differences between two branches and reverts all changes, forcing you to create a new commit.

This opens up a vi editor and you must enter:
```vi
:wq
```
In order to write and quit the new commit.

## Restore
```git
git restore file.txt
```
This is the opposite of the git add function. It can move files from the staging area, back to the working directory, undoing changes.

If a file has been added accidentally with unwanted changes, you can restore previous version by adding the --stage option. e.g.

```git
git restore --stage file.txt
```

## Reset
This is a very dangerous function in git and resets the file back to a specific commit and removes all more recent commits.

```git
git reset commitID
```

After resetting file, the user must restore to apply the changes and move the file back to the working directory.

