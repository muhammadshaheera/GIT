# Git on CentOS7

`cd /path/of/git`
`git init` #To initializes a new Git repo

########################### SSH Cloning ###########################
https://docs.github.com/en/authentication/connecting-to-github-with-ssh
https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository?platform=linux&tool=cli

`ssh-keygen -t ed25519 -C "emailaddress@mail.com"`
Goto /root/.ssh, open file id_ed25519.pub(public key) and add it in Github setting>SSH and GPG keys as SSH key
`git clone git@github.com:username/test.git`

########################### HTTPS Cloning ###########################
https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository?platform=linux&tool=webui

Goto Github setting>Developer settings>Personal access tokens>Tokens (classic)>Generate new token (classic)
`git clone https://github.com/username/test.git`
After entering username, enter generated token as password

########################### General Configuration and Administration ###########################
`git config --global user.name "username"`
`git config --global user.email "emailaddress@mail.com"`
`git config --list #To check your git configurations`


`git add/rm file1.html file2.html`
`git commit -m "file1 and file2 addition"`

`git push`
`git push origin <branch_name>`

`git pull`
`git pull origin <branch_name>`

`git branch #To view all branches and your current branch`
`git branch <branch_name> #To create new branch`
`git checkout <branch_name> #To switch branch`
`git checkout -b <branch_name> #To create new branch and switch to it`
`git branch -d <branch_name> #To delete branch`
`git branch -D <branch_name> #To delete branch forcefully`
`git merge <branch_name> #To merge a new branch with head branch but you should have to be on head branch for this merger`
