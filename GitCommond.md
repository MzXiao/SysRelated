###Preset---git config
git config --list
git config --global user.name YOURNAME
git config --global user.email YOUREMAIL


###Local Work---into your project file
git init
git add -A
git commit -m "commit message"
git log 

git status --hard COMMIT_ID
git reflog 


###Linking Github---save your work on github

1.Github SSH
ssh-keygen -t rsa -C "Github account email address"
cat ~/.ssh/id_rsa.pub
[github]
Click Settings-->SSH and GPG keys -->New SSH key-->save

ssh -T git@github.com




2.link github
[github]
login your github:--->creat a repo
[local]
git remote add origin git@github.com:YOUR_REPO_ADDR

git push -u origin master //first time push
git push origin master



###Working With Others---
