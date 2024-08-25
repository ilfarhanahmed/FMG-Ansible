git --global user.email "abc@xyz.com"
git --global user.name "abc"

//Generate SSH key:
ssh-keygen -t ed25519 -C "your_email@example.com"

//Get the key and add to GitHub > Settings > SSH
cat ~/.ssh/id_ed25519

//Adding ssh key to ssh agent
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519

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
git remote add origin git@github.com:<user><repo>
git branch -M <target github branch>

//pull 
git pull origin <branch>

//push
git push -u origin <branch name>
