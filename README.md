# Learning git and github 
-------git funamental--------
Git init - to initialize a repository
# remove .git from excluded file in vs code in settings
git status - tells the current status
# u - untracked
.gitignore - if you dont want your private info to be exposed or unnecessary modules like node_modules
# repository is just some snapshots of some changes
git add - add file for next commit
# git add . - all file in current directory will be added
# git reset . - undo git add

# commit - every commit has a unique id by which git can tell the difference between commits

git commit - git commit -m "Initial commit"
# afte commiting we get back to normal and we have no untracked file

git log - information about last commit
# head is most currrent commit on a branch

# m - yellow - modified
# git commit -a -m -- remove the necessity of using git add 

-------------fundamentals complete ------------

---------git remote---------
# a way to work on remote repositories
git remote add origin <url> - will link our code to remote repository

# git remote -v
# git remote show origin

# next step - sync our code with that repository
git push - kinda like upload
git push origin master -u -- origin is our name of remote repo and master is branch name and u will allow us to use command git pull 




