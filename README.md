**[Git and Gitbash](https://github.com/ZjeniiaSt/kottans-frontend/blob/main/README.md#git-and-gitbash)**

**[Linux CLI, and HTTP](https://github.com/ZjeniiaSt/kottans-frontend/blob/main/README.md#linux-cli-and-http)**

**[HTML and CSS](https://github.com/ZjeniiaSt/kottans-frontend/blob/main/README.md#html-and-css)**

**[Responsive Web Design](https://github.com/ZjeniiaSt/kottans-frontend/blob/main/README.md#responsive-web-design)**

**[## JS Basics]()**

## Git and GitBash

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

**for Terminal**
```
~                              home directory
.                              current directory
>                              send to a new file

cd ~/Desktop                   to folder
mkdir my-project               create folder
rmdir                          remove EMPTY folder
rmdir -r                       remove folder and files 

echo 'Some text' > file.txt    create file
mv                             move/rename
cp                             copy
cat file.txt                   read file
rm file.txt                    delete file
ls                             show files list
ls -la                         show hidden list
chmod                          change permissions
groups                         show my group
*                              wildcart - all files
0                              

man                            view manual pages
find                           locate files
finger                         show user information


lpr                            send to printer
lpq                            display print queue
lprm                           remove from print queue

df                             shows free disk space
ps aux                         list of all processes
kill                           process to die gracefully
grep                           finds words in text

```

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

## HTML and CSS

**[Validator](https://validator.w3.org/)**

**Combining selectors**
```
Element with class selector     selector.class
Child (direct) selector         selector > selector
Descendent selectot             selector selector
```
**Specification**
```
style=''  ''              ID                       class, pseudoclass, attribute,                       # of Elements
```

## Responsive Web Design

**Avoid scroll**
```
img {
  max-width: 100%;                         
  display: block;
}                              
```

**Flexbox**
```
.items {
  display: flex;
  justify-content: space-between;
}
```
**Grid**
```
.container {
  display: grid;
  grid-template-columns: 1fr 3fr;
}
```

**Multicol**
```
.container {
  column-count: 3;
  OR
  column-width: 200px;
}
```

## JS Basics
