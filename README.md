# Git-Cheat-Sheet

# Git Cheatsheet By Bishworaj Poudel

##### 1. For Config:
=> git config --global user.name "Sunil Ghimire" <br>
=> git config --global user.email "sunilghimire64@gmail.com" <br>

##### 2. To View  user.name and email
git config --list 

##### 3. To Get Help:
=> git help
=> git help <topic>

##### 4. Initialize a Repository
=> git init

##### 5. To Add File To Staging Area
=> git add filename
=> git add filename1 filename2
=> git add . [To Add All Files In Directory]

##### 6. To Commit Change
=> git commit -m 'Short and Sweet Message'
=> git commit -am 'Staging and Comit Directly' 

##### 7. Clone Existing Repository
=> git clone <project_url>

##### 8. Checking the Status Files
=> git status
=> git status -s [Short Status]

##### 9. View Difference
=> git diff  [ Find difference between commited and unstaged files ]
=> git diff --staged [difference in staged files]

##### 10. To Remove File From git
=> git rm filename

##### 11. To Move File
=> git mv file_from file_to [If we rename the file]

##### 12. To Move staged file to not staged
=> git reset HEAD
=> git reset HEAD file1.txt

##### 13. To Unmodifying a Modified File
=> git checkout filename

##### 14. To View Commit History
=> git log
=> git log --oneline [Oneline Easy and Fast]
=> git log --stat [More History]
=> git log --pretty=oneline [Show SHA1 Value]
=> git log --pretty=format:"%h %s" --graph 
=> git log --pretty=format:"%h - %an, %ar : %s" 
=> git log --since=2.weeks
=> git log --after=2.weeks
=> git log --author "Bishworaj Poudel"
=> git log --oneline --decorate --graph --all 

##### 15. To ignore files:
=> create .gitignore file
=> then add filename/foldername line by line
=> *.c => ignore al .c files
=> !main.c => not ignore main.c file
=> node_modules/ => Directory node_modules and all files inside it.

##### 16. To Unstaging a Staged File with git restore
=> git restore
=> git restore --staged file1.txt

##### 17. To Work With Remote Repository
=> git remote show origin [To View Remote Origin Details]
=> git remote -v
=> git remote add origin <url>:
=> git push origin master
=> git pull => pull data with current head
=> git fetch => only download the data to local repository
=> git fetch origin mod => To retrive remote branch
=> git remote rename pb paul 
=> git remote remove paul
=> git push origin --delete bad-branch-name

##### 18. Git Tag
=> git tag -l
=> git tag --list 
=> git tag -a v1.4 -m "my version 1.4" 
=> git show v1.4
=> git tag v1.4-lw  [Lightweigt]
=> git tag -d v1.4-lw 
=> git checkout v2.0.0 

##### 19. To Transfer Tag to Remote
=> git push origin <tagname>.


##### 20. Working With Branch
=> git branch testing [To Creating Testing Branch]
=> git checkout testing [Switch Branch]
=> git commit -am 'made a change'
=> git checkout master [To Move to Master Branch]
=> git checkout -b <newbranchname>.[Creating branch and switching to it] 
=> git branch --merged
=> git branch --no-merged 
=> git branch --move bad-branch-name corrected-branch-name

##### 21. Redo Commit
=> git reset
=> git reset SHA1
=> git reset -hard SHA1 

##### 22.  Git Stash
=> git stash save 
=> git stash list
=> git stash pop
=> git stash apply stash{0}
=> git stash clear
=> git stash grop stash

##### 22. Merge
=> git merge branchname
=> git merge --no-ff branch name

#### 23. Rebase
=> git rebase branchname
