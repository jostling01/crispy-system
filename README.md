
# crispy-system
Everything we have learnt about git


# ***An Introduction to GitHub***

![github icon](githubicons.png)


#### GitHub is a powerful tool used to manage version control 
```
Heres a breakdown of the main features GitHub offers

- Update and create new versions of files

- Revert back to old versions of files

- Project collaboration (Super fun!)

- Development on top of an existing file
```
*This article will cover*
- Revert, Reset, Restore
- How to navigate files/folders in terminal


## States files can exist in


Working Directory
- file sitting in folder but git doesn't know what it is
- the command git add takes the file to the staging area

Staging Area
- content can be or has been added to the file but has not yet been comitted

Commit
- use the command git commit -m "*message*" to commit (save) changes to the file

Repository
- Where you and your collaborators' work is stored on GitHub


# Revert Reset and Restore Functions


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













[GitHub](https://www.github.com)

