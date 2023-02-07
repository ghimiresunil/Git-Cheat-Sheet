# Git Cheatsheet By Sunil Ghimire

##### 1. For Config:
=> git config --global user.name "Sunil Ghimire" <br>
=> git config --global user.email "info@sunilghimire.com.np" <br>

##### 2. To View  user.name and email
=> git config --list 

##### 3. To Get Help:
=> git help <br>
=> git help `<topic>`

##### 4. Initialize a Repository
=> git init

##### 5. To Add File To Staging Area
=> git add filename <br>
=> git add filename1 filename2 <br>
=> git add . `To Add All Files In Directory` 

##### 6. To Commit Change
=> git commit -m 'Short and Sweet Message' <br>
=> git commit -am 'Staging and Comit Directly' 
  
##### 7. The seven rules of a great Git commit message
* Separate subject from body with a blank line <br>
* Limit the subject line to 50 characters <br>
* Capitalize the subject line <br>
* Do not end the subject line with a period <br>
* Use the imperative mood in the subject line <br>
* Wrap the body at 72 characters <br>
* Use the body to explain what and why vs. how
  
##### 8. Clone Existing Repository
=> git clone <project_url>

##### 9. Checking the Status Files
=> git status <br>
=> git status -s [Short Status]

##### 10. View Difference
=> git diff  [ Find difference between commited and unstaged files] <br>
=> git diff --staged [difference in staged files]

##### 11. To Remove File From git
=> git rm filename

##### 12. To Move File
=> git mv file_from file_to [If we rename the file]

##### 13. To Move staged file to not staged
=> git reset HEAD <br>
=> git reset HEAD file1.txt

##### 14. To Unmodifying a Modified File
=> git checkout filename

##### 15. To View Commit History
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

##### 16. To ignore files:
=> create .gitignore file <br>
=> then add filename/foldername line by line <br>
=> *.c => ignore al .c files <br>
=> !main.c => not ignore main.c file <br>
=> node_modules/ => Directory node_modules and all files inside it.

##### 17. To Unstaging a Staged File with git restore
=> git restore <br>
=> git restore --staged file1.txt

##### 18. To Work With Remote Repository
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

##### 19. Git Tag
=> git tag -l <br>
=> git tag --list  <br>
=> git tag -a v1.4 -m "my version 1.4"  <br>
=> git show v1.4 <br>
=> git tag v1.4-lw  [Lightweigt] <br>
=> git tag -d v1.4-lw <br>
=> git checkout v2.0.0 <br>

##### 20. To Transfer Tag to Remote
=> git push origin <tagname>.

##### 21. Working With Branch
=> git branch testing [To Creating Testing Branch] <br>
=> git checkout testing [Switch Branch] <br>
=> git commit -am 'made a change' <br>
=> git checkout master [To Move to Master Branch] <br>
=> git checkout -b <newbranchname>.[Creating branch and switching to it] <br>
=> git branch --merged <br>
=> git branch --no-merged <br>
=> git branch --move bad-branch-name corrected-branch-name <br>

##### 22. Redo Commit
=> git reset <br>
=> git reset SHA1 <br>
=> git reset -hard SHA1 

##### 23.  Git Stash
=> git stash save <br>
=> git stash list <br>
=> git stash pop <br>
=> git stash apply stash{0} <br>
=> git stash clear <br>
=> git stash grop stash <br>

##### 24. Merge
=> git merge branchname <br>
=> git merge --no-ff branch name

#### 25. Rebase
=> git rebase branchname

#### 26. Git Explained to a 6 years old

=> Imagine you get some paper and crayons for your birthday. <br>
=> You use them to yourself a nice beach scene. Then you go have a nice sandwish for lunch. <br>
=> When you come back, you start to draw some seagulls - but shit, the food coma hits and thet look terrible! <br>
=> So, you crumple up the paper in anger, throw it on the floor for mommy to clean up, and you start over from scratch, re-drawing the beach scene, then trying the seagulls once more, after you finish crying, of course. <br>
=> Wouldn't it be nice if instead, mommy could reach into the closet and pull out an exact copy of the beach scence before you want to lunch? <br>
That way, you just get right back to the seagulls and not have to re-do all the work before that print. <br>
=> **That's essentially Git** <br>
(except that YOU can go into the closet yourself and mommy can continue to lay on the counch enjoying her coffee- that's how everyone's childhood was, right?!)<br>
=> With Git though, it's code.. `You create a file` ,  `You edit it a bit`, `Then, you **"Commit"** it to Git` <br>
=> Without getting into the inner workings, there is essentially from your perspective anyway, a copy of the file exactly as it was at the time you commit it. <br>
Make Some changes commit it again, now there's two couples (**two "versions"**) that look like the file at the same time of each commit. <br>
=> These copies are the file's "history". You can compare two different versions to see what changed, and you can "revert" you own copy to a previous change, just like our bratty own artist.

# Awesome notes on git commands [IMAGES]

![git_01](https://user-images.githubusercontent.com/40186859/130892497-b7887735-528b-49c1-8bac-04f4f6b8c50a.jpeg) 
*Figure 01: Awesome notes on git commands*<br> 
![git_02](https://user-images.githubusercontent.com/40186859/130892587-defe34d2-b593-40e2-8dbd-3f0bcbe8602e.jpeg)
*Figure 02: Awesome notes on git commands*<br>
![git_03](https://user-images.githubusercontent.com/40186859/130892695-f7b4ed2b-e09d-438d-bc65-5ce910699ea8.jpeg)
*Figure 03: Awesome notes on git commands*<br>
![git_04](https://user-images.githubusercontent.com/40186859/130892758-fc517a04-9520-48b5-a5ff-847f1bdf1f93.jpeg)
*Figure 04: Awesome notes on git commands*<br>
