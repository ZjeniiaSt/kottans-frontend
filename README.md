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

git merge <feature branch name>
```

**Connection with a repo**
```
git pull
git push

git clone <url>

git remote add origin <url>          connect - repo
git push -u origin <branch>          first connect - branch

git remone -v                        check connect
```
