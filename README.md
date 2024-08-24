git --global user.email "abc@xyz.com"
git --global user.name "abc"

local directory

//git start
git init

//status
git status

//Track files
git add <file name>
git add --all

//create file to ignore files
touch .gitignore

//untrack
git rm --cached <file>

//difference
git diff

//commit changes
git commit -a -m "comment"

//list branches
git branch

//create branch
git branch <branch_name>

//switch branch
git switch <branch_name>

//merge branch to main
1. Go to main branch
2. git merge -m "comment" <branch_name>

//delete branch
git branch -d <branch_name>

//rename branch
git branch -m <old name> <new name>

//push to github
git remote add origin https://github.com/username/repo
git branch -M <target github branch>
