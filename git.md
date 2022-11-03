# GIT
## VCS - version control system
## GitHub GitLab
## [https://git-scm.com/](https://git-scm.com/ "Сайт git") сайт 

```bash
git --versuin # Текущая версия git
```

```bash
git --help # обзор базовых возможностей
```
```bash
git init # Инициализация репозитория
```

```bash
git log # Просмотр истории изменений (коммитов)
git log -p
```
```bash
git status # Статус файлов
```
untracked files - файлы не отслеживаются
```bash
git add <file> # Добавляем текущий файл для отслеживания изменений
git add . # Добавить все файлы для отслеживания изменений
```
```bash
git rm --cached <file> # Отменить отслеживание
```

```bash
git commit -m 'First Commit' # Коммитим в локальный репозиторий
```
> -m - message

```bash
git commit -am 'Anoter commit' # Взять все файлы под версионный контроль и закоммитить
```

```bash
git branch # Смотрим ветки
git branch <branch> # Создаем ветку
git branch -D <branch> # Удалить ветку
git branch -m <new branch name> # Переименовать текущую ветку
git branch -a # Отображает все ветки, включая те, которые находятся в удаленных репозиториях.
git branch -vv
```
```bash
git checkout <branch> # Переключиться на другую ветку
git checkout -b <new_branch> # Создать новую ветку и переключиться на нее.
```

## Слияние веток
```bash
git merge test # Мержим файлы из test в master
```

## Настройки конфига git
```bash
git config --global user.name # Текущее имя пользователь
git config --global user.name 'Anatoliy' # Поменять текущее имя на имя Anatoliy
git config --list # Получаем список всех настроек.
```

## Работа с удаленным репозиторием
```bash
git remote add origin <url> # Связываем удаленный репозиторий с удаленным.
git remote add origin https://github.com/talisman/new.git

git remote # проверяем списки удаленных репозиториев
git remote -v # ссылка на удаленный репозиторий.
```
```bash
git push -u origin master # Заливаем в удаленный репозиторий
```
> origin - источник
```bash
git push # Так как привязка уже сделана, то просто заливаем изменения из локального в удаленный репозиторий.
```

```bash
git pull # Получаем изменения из удаленного репозитория
```
```bash
git clone https://github.com/talisman/new.git # Клонируем репозиторий
```

## Создаем файлы для игнорирования
.gitignore
