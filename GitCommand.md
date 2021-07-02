### Preset---git config
```
git config --list
git config --global user.name YOURNAME
git config --global user.email YOUREMAIL
git config --global http.proxy http://127.0.0.1/1081
```

### Local Work---into your project file
```
git init
git add -A
git commit -m "commit message"
git log 
git log --graph --pretty=oneline --abbrev-commit

git remove --cached //stage file to workspace
git remote set-url origin git@github.com:User/project-new.git

git reset --hard COMMIT_ID
git reflog 

(Branching)
git checkout -b New_Branch
[git branch New_Branch]
[git checkout New_Branch]

git branch -d New_Branch

git merge [--no-ff -m "msg"]  New_Branch // no fast forward


git push origin --delete origin_branch //delete remote branch, origin must have

//detached head
git checkout abcd // to position abcd, detached head
git commit ... git branch temp efgh// commit some code,create temp branch
git checkout master , git merge temp // save change to master

(tag)
git checkout tag1

```




### Linking Github---save your work on github
```
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

-- delete remote branch
git push origin --delete feature_20210325_appclass

git pull
[git clone only set orign/master to your local master]
git branch -a 
git branch -d dev origin/dev
git branch --set-upstream-to=origin/dev dev
```



### Working With Others---
```
git clone 
fork 
git pull
git rebase
```

### Best Pratice
```
remote:
git branch -vv
git remote -v
git remote show origin
1.本地新建分支    推送到origin
git checkout -b feature_new 
git push origin feature_new:feature_new
git branch -u orgin/feature_new
2.删除远程分支
git push origin :remote_branch_delete
3.
```
