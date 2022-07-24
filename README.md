**[Git and Gitbash](https://github.com/ZjeniiaSt/kottans-frontend/blob/main/README.md#git-and-gitbash)**

**[Linux CLI, and HTTP](https://github.com/ZjeniiaSt/kottans-frontend/blob/main/README.md#linux-cli-and-http)**

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
git fetch
git merge 

git pull
git push

git pull --rebase

git clone <url>

git remote add origin <url>          connect - repo
git push -u origin <branch>          first connect - branch

git remove                           check connect
```


## Linux CLI, and HTTP

**HTTP** - Hypertext Transfer Protocol (* протокол прикладного рівня для "переговорів" про доставлення Web-сервером документа Web-браузеру)

**URL-адрес** - (Uniform Resource Locator – уніфікований покажчик [місцезнаходження інформаційного] ресурсу)

**Methods**
```
GET: для запиту ресурсу. В URL-адресі міститься вся необхідна інформація для визначення місцезнаходження та повернення ресурсу сервером.
POST: для створення нового ресурсу. Запити POST звичайно містять дані для створення нового ресурсу.
PUT: для оновлення існуючого ресурсу. У вмісті можуть знаходитися оновлені дані для ресурсу.
DELETE: для видалення існуючого ресурсу.
```

**Status codes**

200 OK
```
202 Accepted (* Прийнято).
204 No Content (* Нема вмісту): тіло повідомлення не передається.
205 Reset Content (* Скинути вміст).
206 Partial Content (* Частковий вміст).
```

3xx: Переадресація
```
301 Moved Permanently (*  Постійно переміщений): запитуваний об'єкт було остаточно перенесено на новий URL.
303 See Other (* Дивитися інший): запитуваний об'єкт було тимчасово перенесено на нову URL-адресу. 
304 Not Modified (* Не модифікований): сервер виявив, що ресурс не було змінено і клієнту варто використовувати копію з кеш-пам'яті. 
```

4xx: Request error 
```
404 Not Found (*  Не знайдено).
400 Bad Request ( Зіпсований запит).
401 Unauthorized (*  Несанкціонований доступ).
403 Forbidden (* Заборонено).
405 Method Not Allowed (* Метод не допустимий).
409 Conflict (* Конфлікт).
```

5xx: Server error
```
500 Internal Server Error 
501 Not Implemented (* Не реалізовано).
503 Service Unavailable (* Сервіс недоступний).
```
