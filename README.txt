1. `git init` - powers your folder to be managed by git, and initializes a new empty repository.it also creates a .git folder that has all the relevant logics to manage versions of your project. 


2. `working area` -> There can be a bunch of files that are not currently handled by git. It means that changes done or to be done in those files are not managed by git yet. A file which is in working area is considered to be not in staging area. when we do `git status` we see a bunch of untracked files  then these are actually called to be in working area.

3. `staging area` -> what all files are going to be part of next version that we will create. This staging area is the place where git knows what changes will be done from the last version to the next version.

4. `respository area` -> This area actually contains the details of all your previous registered versions. And the files in this area, git already manages them and knows their version history.

5. `git add <file> -> moves file from working area to staging area.

6. `git rm --cached <file>` moves file back from staging area to wokring area.

7. `commit` -> commit is a particular version if the project. It captures a snapshot of the project's staged changes and created a version out of it.

8. `git commot` -> registers staging changes to a commit.

9 `git log` -> list downs all the commits of all the repository.

10. `git restore <file>` -> it removes all files changes from the staging area to be commited . This can be useful, if we did some dirty piece of code and now no more want it . Instead of deleting every change line by line, we can restore it or you can say restore last clean version of file.

11. `git restore --staged <file>` -> it removes file from changes from staging area to the working area. this only works if your changes are in your staging area.

12. Diff between git rm and git restore?
ans: if you want to move the whole file back to untracked state, then we do git rm, otherwise if we just want the changes to be moved in working area or staging area then we git restore.

13. `git commit -m "<your commit message>"` -> if we want to avoid opening a text editor vim to add commit msg we can use this following command