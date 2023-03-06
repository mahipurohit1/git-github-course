# dummy practice repo

this is just a demo repo for just practice some git command !!!


Basics git Command 

git  init 
git status 
git commit -m "message"
git commit --amend  -> last commit mein change karne k liye 
git log 
git log --oneline
.gitignore  file 
git clone url

-------------------------------------------------------

Branch command 

git branch : show all branch 
git branch -v :  show all branch with last commit 
git branch mahipal : create a new branch 
git switch mahipal  :  switch to mahipal branch 
git switch -c mahi : create a new branch and switch to it 
git checkout mahipal : just like switch 
git checkout  -b mahi : just like switch -c 
git branch -m mahipurohit  :  rename the branch in which u present
git branch -d mahipalpurohit : delete the branch u must not present in the mahipalpurohit branch
git checkout -b mahipalpurohit 9020c44 : to recover deleted branch !

git branch -r :  show all remote branch 

-------------------------------------------------------------

Branch Merge command: 

steps :  
git switch master
git merge mahipal   
// it will merge mahipal branch into matser branch 

--------------------------------------------------------------


Git diff command 

git diff  : show diff between  staging area and working directory
git diff Head :  show diff between last commit and working directory
git diff --staged : show diff in stagged file 
git diff branch1 branch2 :diff between two branch
git diff Head [filename]
git diff commit1 commmit2

----------------------------------------------------------

Git stash command

git stash : to temporary save  uncommited work  
git stash pop : to restore the work and remove from stash
git stash apply : to restore the work but not remove from stash
git stash -u : to save untrack files 
git stash list : to show all the save file 
git stash clear :  to clear all the stash 


-------------------------------------------------------

other command 

git checkout d8194d6  :- to see specific  d8194d6 commit 
git restore filename  :- to undo changes 
git restore --staged filename : to unstagged the file 
git restore --source f2609a3 filename : to undo changes  to the specific commit 
git reset 0026739 :- to  undo commit untill 0026739 commit hash 
git  reset --hard 0026739 :-  to  undo commit untill 0026739 commit hash and your work also gone 
git revert <commit-hash> :- to ceates a brand new commit which reverses/undos the changes from a commit


------------------------------------------------------------


git push command 

git push origin main : push to main branch 
git  push origin master : push to master branch 
git push -u origin main :  it will remember upstream  

-----------------------------------------------------------------

Github Command 

git remote : to see remote name 
git remote add origin url : add remote repo to local repo
git push <remote> <local-branch>:<remote-branch>  :  to push  from mahipal branch to main branch 
git fetch origin main : fetch all commit but not include in  working directory 
git pull origin main : fetch all commit and include in  working directory 



--------------------------------------------------------------------

git Rebase : rewriting hitstory of  commit 

steps 1)
git switch featurebranch
git rebase master


Interactive Rebase
git rebase -i 4545sdd :- which allows us to edit commits, add files, drop commits, etc. 

-----------------------------------------------------------------------

Git Tags




