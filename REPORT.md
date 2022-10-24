# Команды, используемые в лабораторной  работе
## Task 1

+ wsl --install
+ wsl --list --online

  ![task1.png](docs/task1.png)

+ wsl --install -d Ubuntu-20.04
+ cd /mnt/c/Users/wolka/Downloads/mobile-dev-backend/mobile-dev-backend
+ sudo apt update
+ sudo apt install lighttpd
+ sudo apt upgrade
+ git config --global --add safe.directory /mnt/c/Users/wolka/Downloads/mobile-dev-backend/mobile-dev-backend
+ sudo apt install gitweb
+ git instaweb

## Task 2

![task2.1.png](docs/task2.1.png)
+ git checkout ci
+ git rebase -i HEAD~2

  ![task2.2.png](docs/task2.2.png)

  ![task2.3.png](docs/task2.3.png)

  ![task2.4.png](docs/task2.4.png)

  ![task2.5.png](docs/task2.5.png)
+ git rebase master

  ![task2.6.png](docs/task2.6.png)
+ git checkout master
+ git merge ci

  ![task2.7.png](docs/task2.7.png)
+ git branch -D ci

  ![task2.8.png](docs/task2.8.png)

## Task 3

+ git log --graph --oneline --reflog

  ![task3.1.png](docs/task3.1.png)
+ git checkout aae7df3ec8096a0815f04212b809db7a0dbddd27

  ![task3.2.png](docs/task3.2.png)
+ git switch -c old-master

  ![task3.3.png](docs/task3.3.png)

## Task 4

+ git blame -L 32,+1 prisma/seed.ts

  ![task4.png](docs/task4.png)

## Task 5

+ git bisect start
+ git bisect bad 12c17ba458a0d83b4eb5218aceff147b92a2aa2b
+ git bisect good 8673a61216986f4401c85c1b8448488911c2c678
+ npm run test
+ git bisect bad
+ npm run test 
+ git bisect good
+ npm run test 
+ git bisect bad 
+ npm run test
+ git bisect bad

  ![task5.1.png](docs/task5.1.png)

  ![task5.2.png](docs/task5.2.png)
+ git bisect reset

## Task 6

+ git filter-branch --force --prune-empty --index-filter "git rm -rf --cached --ignore-unmatch .env" --tag-name-filter cat -- --all
+ echo '.env' >> .gitignore

## Task 7

  ![task7.1.png](docs/task7.1.png)
+ git filter-branch -f --env-filter "GIT_AUTHOR_NAME='Sidortsov Vladimir Sergeevich'; GIT_AUTHOR_EMAIL='TungFram@yandex.ru'; GIT_COMMITTER_NAME='Sidortsov Vladimir Sergeevich'; GIT_COMMITTER_EMAIL='TungFram@yandex.ru';" HEAD~3..HEAD

  ![task7.2.png](docs/task7.2.png)

## Task 8

+ git config rerere.enabled true
+ git merge feature
+ git add .
+ git commit
+ git reset
+ git merge feature
+ git add .
+ git commit

  ![task8.png](docs/task8.png)

## Task 9

+ git fsck

  ![task9.png](docs/task9.png)

## Task 10

+ git fsck
+ git count-objects -vH
+ git gc --prune=now --aggressive
+ git count-objects -vH
+ git fsck

  ![task10.png](docs/task10.png)

**Итоговая версия репозитория:**
![task10-final-version.png](docs/task10-final-version.png)

## Task 11

  ![task11.1.png](docs/task11.1.png)
+ git add docs/task(1-10).*
+ git add REPORT.md
+ git commit -a -m "feat: task(1-10) at REPORT.md"

  ![task11.2.png](docs/task11.2.png)
