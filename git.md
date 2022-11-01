# GIT
# VCS - version control system
# GitHub GitLab
# git-scm.com сайт 

git --versuin # Текущая версия git
git --help # обзор базовых возможностей

git init # Инициализация репозитория
git log # Просмотр истории изменений (коммитов)
git log -p

git status # Статус файлов
# untracked files - файлы не отслеживаются

git add <file> # Добавляем текущий файл для отслеживания изменений
git add . # Добавить все файлы для отслеживания изменений

git rm --cached <file> # Отменить отслеживание

git commit -m 'First Commit' # Коммитим в локальный репозиторий
# -m - message

git commit -am 'Anoter commit' # Взять все файлы под версионный контроль и закоммитить

git branch # Смотрим ветки
git branch <branch> # Создаем ветку
git branch -D <branch> # Удалить ветку
git branch -m <new branch name> # Переименовать текущую ветку
git branch -a # Отображает все ветки, включая те, которые находятся в удаленных репозиториях.
git branch -vv

git checkout <branch> # Переключиться на другую ветку
git checkout -b <new_branch> # Создать новую ветку и переключиться на нее.

# Слияние веток
git merge test # Мержим файлы из test в master

# Настройки конфига git
git config --global user.name # Текущее имя пользователь
git config --global user.name 'Anatoliy' # Поменять текущее имя на имя Anatoliy
git config --list # Получаем список всех настроек.

# Работа с удаленным репозиторием
git remote add origin <url> # Связываем удаленный репозиторий с удаленным.
git remote add origin https://github.com/talisman/new.git

git remote # проверяем списки удаленных репозиториев
git remote -v # ссылка на удаленный репозиторий.

git push -u origin master # Заливаем в удаленный репозиторий
# origin - источник
git push # Так как привязка уже сделана, то просто заливаем изменения из локального в удаленный репозиторий.

git pull # Получаем изменения из удаленного репозитория

git clone https://github.com/talisman/new.git # Клонируем репозиторий

# Создаем файлы для игнорирования
.gitignore