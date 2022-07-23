**[Git and Gitbash](https://github.com/ZjeniiaSt/kottans-frontend/blob/main/README.md#git-and-gitbash)**

## Git and GitBash

**for Terminal**
```
cd ~/Desktop                   to folder
mkdir my-project               create folder
echo 'Some text' > file.txt    create file
cat file.txt                   read file
rm file.txt                    delete file
ls                             show files list
ls -la                         show hidden list

```

**Basic commands**
```
git init
git status                              staging area/index

git add <files>
git add .
git commit -m 'message'
git log                                 history

git checkout <commit hash>
git checkout -b <branch name>

git branch                             branchs list
git branch -b                          branch list all repo

git branch -m <new branch name>        rename CURRENT branch
git branch -d <branch name>            delete branch NOT CURRENT
```

**Working with branches**
```
git merge <feature branch name>
git rebase main

git checkout <branch>^                 to previosly commit
git checkout HEAD~N                    to N commit
git branch -f main HEAD~3

git reset HEAD~1                       for local
git revert HEAD                        for published

git cherry-pick <Com1> <Com2>...
git rebase -i <branch>

git commit --amend                     change last commit
```


**Connection with a repo**
```
git pull
git push

git clone <url>

git remote add origin <url>          connect - repo
git push -u origin <branch>          first connect - branch

git fetch

git remove                           check connect
```
