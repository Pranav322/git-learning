# Learning git and github 
-------git funamental--------
# Git init 
Git init - to initialize a repository

# recommended but not necessary -  remove .git from excluded file in vs code in settings m this will show .git folder in vs code

# git status - 
git status - tells the current status
# u shows untracked files in vscode 
# M shows modified file in vscode 
# A shows added file in vscode


# .gitignore 
.gitignore - if you dont want your private info to be exposed or unnecessary modules like node_modules, create a .gitignroe file and put all such files or folder there
# repository 
repository is just some snapshots of some changes

# git add 
git add -  add file for next commit

# git add .
git add . -  - all file in current directory will be added
# git reset . 
git reset . - undo git add

# commit - every commit has a unique id by which git can tell the difference between commits

 git commit -m "Initial commit" - will create a commit and after commiting we get back to normal and we have no untracked file

# git log
git log - information about last commit

# head is most currrent commit on a branch


# git commit -am -- remove the necessity of using git add 

-------------fundamentals complete ------------

---------git remote---------

# a way to work on remote repositories
# remote means github version and local means vs code version
# git remote 
git remote add origin <url> - will link our code to remote repository

# git remote -v
# git remote show origin

# next step - sync our code with that repository
# git push 
git push - kinda like upload
git push origin master -u -- origin is our name of remote repo and master is branch name and u will allow us to use command git pull 



# next -git merge
# if we are changing directly in remote repository our remote repository will be one commit ahead so how to sync our remote repository with local repository , lets see

# now we have master branch in remote and in loca and we both are unsynced
# there are two ways - fetch and merge

#git fetch - fetch change from remote and then merge
git merge origin/master


# git pull - 
git pull - dont fetch and merge , just pull

# but if you have uncommited change in local repository and try to pull there might be conflict  , so aither commit or use stash - we will look at it later
# there migh tbe merge conflict even when your loca code is modifying the smae code that you are pulling

# git clone - clone a repository from remote
git clone <repository url>

# github codespaces

when you are on your repo , hit . --it will open a cloud based version of your version on vs code , but you dont have terminal access


---------start git branch now------------------
# git branch 
git branch - this command will give list of all current branch

git branch -M main - this will change our master branch name to main which is common thing nowadays

git branch <branch name> - will create a new branch
git branch -d <branch name> - will delete
d and D differ - D will delete no matter what but d will delete safely

# git -checkout

git checkout <branch name> - switch to brannch 

git checkout -b <branch name> - will create and switch to branch in one single command 

git checkout - --this will take yout o previous branch
# merge conflicts - kinda scary

when same line of code gets modified

# how to solve - git diff will tell the differnce

git merge --abort will take you to previous version

now git add . and git commit -m "merged conflict"

# fork -- more of a github thing 
when you want to work on open source code , fork will make a copy of code on your own account but will have linked with main repo , you can send pull request after making changes


# how to fork - lets see
