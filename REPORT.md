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

![task1.png](docs/task2.1.png)
+ git checkout ci
+ git rebase -i HEAD~2
  ![task1.png](docs/task2.2.png)
  ![task1.png](docs/task2.3.png)
  ![task1.png](docs/task2.4.png)
  ![task1.png](docs/task2.5.png)
+ git rebase master
  ![task1.png](docs/task2.6.png)
+ git checkout master
+ git merge ci
  ![task1.png](docs/task2.7.png)
+ git branch -D ci
  ![task1.png](docs/task2.8.png)

## Task 3

+ git log --graph --oneline --reflog
  ![task1.png](docs/task3.1.png)
+ git checkout aae7df3ec8096a0815f04212b809db7a0dbddd27
  ![task1.png](docs/task3.2.png)
+ git switch -c old-master
  ![task1.png](docs/task3.3.png)