## Lets-pracitce-collaboration

###### **Deleting a remote branch**
```
git push --delete <remote name(main)><branchName>
git branch -D <branchname> Since the branch still exists in the working repo

```
###### **To seee the current changes made but not yet staged**
```
git diff
git diff --cached [If you want to see what changes had been already staged, use this version:]

```
###### **I have some changes that I’d like to add to the previous commit!**
```
git commit -a --amend

```

###### ** Let’s commit these changed files!

```
alias gca = git commit -a

This commits all changed files, so you don’t need to add them manually. However, if there are some new files, that had not been committed yet, obviously you need to point to them explicitly:

alias ga = git add**

```

######   Moving the mistakenly committed files back to the staging area from the previous commit, without cancelling the changes done to them. This can be done like

```
git reset --soft HEAD^ OR
git reset --soft HEAD~1 
```
Remember the reset always works locally but not remote
######