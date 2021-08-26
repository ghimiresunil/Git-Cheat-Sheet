# Git Cheatsheet By Sunil Ghimire

##### 1. For Config:
=> git config --global user.name "Sunil Ghimire" <br>
=> git config --global user.email "sunilghimire64@gmail.com" <br>

##### 2. To View  user.name and email
=> git config --list 

##### 3. To Get Help:
=> git help <br>
=> git help <topic>

##### 4. Initialize a Repository
=> git init

##### 5. To Add File To Staging Area
=> git add filename <br>
=> git add filename1 filename2 <br>
=> git add . [To Add All Files In Directory] 

##### 6. To Commit Change
=> git commit -m 'Short and Sweet Message' <br>
=> git commit -am 'Staging and Comit Directly' 

##### 7. Clone Existing Repository
=> git clone <project_url>

##### 8. Checking the Status Files
=> git status <br>
=> git status -s [Short Status]

##### 9. View Difference
=> git diff  [ Find difference between commited and unstaged files] <br>
=> git diff --staged [difference in staged files]

##### 10. To Remove File From git
=> git rm filename

##### 11. To Move File
=> git mv file_from file_to [If we rename the file]

##### 12. To Move staged file to not staged
=> git reset HEAD <br>
=> git reset HEAD file1.txt

##### 13. To Unmodifying a Modified File
=> git checkout filename

##### 14. To View Commit History
=> git log <br>
=> git log --oneline [Oneline Easy and Fast] <br>
=> git log --stat [More History] <br>
=> git log --pretty=oneline [Show SHA1 Value] <br>
=> git log --pretty=format:"%h %s" --graph <br>
=> git log --pretty=format:"%h - %an, %ar : %s" <br>
=> git log --since=2.weeks <br>
=> git log --after=2.weeks <br>
=> git log --author "Sunil Ghimire" <br>
=> git log --oneline --decorate --graph --all 

##### 15. To ignore files:
=> create .gitignore file <br>
=> then add filename/foldername line by line <br>
=> *.c => ignore al .c files <br>
=> !main.c => not ignore main.c file <br>
=> node_modules/ => Directory node_modules and all files inside it.

##### 16. To Unstaging a Staged File with git restore
=> git restore <br>
=> git restore --staged file1.txt

##### 17. To Work With Remote Repository
=> git remote show origin [To View Remote Origin Details] <br>
=> git remote -v <br>
=> git remote add origin <url>: <br>
=> git push origin master <br>
=> git pull => pull data with current head <br>
=> git fetch => only download the data to local repository <br>
=> git fetch origin mod => To retrive remote branch <br>
=> git remote rename pb paul <br>
=> git remote remove paul <br>
=> git push origin --delete bad-branch-name <br>

##### 18. Git Tag
=> git tag -l <br>
=> git tag --list  <br>
=> git tag -a v1.4 -m "my version 1.4"  <br>
=> git show v1.4 <br>
=> git tag v1.4-lw  [Lightweigt] <br>
=> git tag -d v1.4-lw <br>
=> git checkout v2.0.0 <br>

##### 19. To Transfer Tag to Remote
=> git push origin <tagname>.


##### 20. Working With Branch
=> git branch testing [To Creating Testing Branch] <br>
=> git checkout testing [Switch Branch] <br>
=> git commit -am 'made a change' <br>
=> git checkout master [To Move to Master Branch] <br>
=> git checkout -b <newbranchname>.[Creating branch and switching to it] <br>
=> git branch --merged <br>
=> git branch --no-merged <br>
=> git branch --move bad-branch-name corrected-branch-name <br>

##### 21. Redo Commit
=> git reset <br>
=> git reset SHA1 <br>
=> git reset -hard SHA1 

##### 22.  Git Stash
=> git stash save <br>
=> git stash list <br>
=> git stash pop <br>
=> git stash apply stash{0} <br>
=> git stash clear <br>
=> git stash grop stash <br>

##### 22. Merge
=> git merge branchname <br>
=> git merge --no-ff branch name

#### 23. Rebase
=> git rebase branchname
  
# Awesome notes on #git commands [IMAGES]

![Figure 01: Awesome notes on git commands](https://user-images.githubusercontent.com/40186859/130892497-b7887735-528b-49c1-8bac-04f4f6b8c50a.jpeg) 
|*Figure 01: Awesome notes on git commands*|
![git_02](https://user-images.githubusercontent.com/40186859/130892587-defe34d2-b593-40e2-8dbd-3f0bcbe8602e.jpeg)
|*Figure 02: Awesome notes on git commands*|
![git_03](https://user-images.githubusercontent.com/40186859/130892695-f7b4ed2b-e09d-438d-bc65-5ce910699ea8.jpeg)
|*Figure 03: Awesome notes on git commands*|
![git_04](https://user-images.githubusercontent.com/40186859/130892758-fc517a04-9520-48b5-a5ff-847f1bdf1f93.jpeg)
|*Figure 04: Awesome notes on git commands*|
