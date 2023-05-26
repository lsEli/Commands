# Commands

Related repository at <https://github.com/lsEli/GitTest>

## Git help

```bash
git help config
```

## Git config help

```bash
git config -h
```

## Git version

```bash
git --version
```

## Global name and email

```bash
git config --global user.name "Your Name"
git config --global user.email "Your Email"
```

## Default branch name

```bash
git config --global init.defaultBranch main
```

## Move to a directory

Root directory.

```bash
cd /path/to/directory
```

## Initialize a repository

```bash
git init
```

## Git status

```bash
git status
```

## Track files

```bash
git add file1 file2 file3
```

## Track all files

```bash
git add .
```

## Untrack files

```bash
git rm --cached file1 file2 file3
```

## Untrack all files

```bash
git rm --cached -r .
```

## Commit changes

```bash
git commit -m "Message"
```

## Files differences

```bash
git diff
```

## Unstage a file

```bash
git restore --staged file
```

## Skip staging area

```bash
git commit -am "Message"
```

## Remove a file

```bash
git rm file
```

## Restore a file

```bash
git restore file
```

## Rename a file

```bash
git mv old_file new_file
```

## Git log

```bash
git log
```

## One line git log

```bash
git log --oneline
```

## Git log details

```bash
git log -p
q
```

## Amend a commit

```bash
git commit --amend -m "Message"
```

## Reset previous commit

```bash
git reset commit_id
```

## See git branches

```bash
git branch
```

## Create a branch

```bash
git branch branch_name
```

## Switch to a branch

```bash
git switch branch_name
```

## Git merge

```bash
git merge -m "Message" branch_name
```

## Delete a branch

```bash
git branch -d branch_name
```

## Switch with branch creation

```bash
git switch -c branch_name
```

## Git remote

```bash
git remote add origin url_to_repository
```

## Push to origin

```bash
git push -u origin branch_name
```

## Push all branches to origin

```bash
git push --all
```

## Pull from origin

```bash
git pull
```

or

### Fetch from origin

```bash
git fetch
```

### Git merge from origin

```bash
git merge
```
