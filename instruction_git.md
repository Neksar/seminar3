# Инструкция по работе с программой GIT

[logo git](git.jpg)

Git это программа для управления контролями версий

## Создание репозитория

Для того, чтобы создать (инициализировать новый репозиторий в текущей папке используется команда:

    git init

## Проверка состония репозитория

Для того, чтобы проверить в каком состоянии находится репозиторийнужно выполнить команду:

    git status

## Добавление изменений отслеживания

Для того, чтобы добавить изменение отслеживания нужно выполнить команду:

    git add <filename>

## Сохранение внесенных изменений

Для того, чтобы сохранить внесенные изменения в контроле версий нужно выполнить команду:

    git commit

Для того, чтобы добавить к внесенным изменения в контроле версий краткое описание, нужно выполнить команду:

    git commit -m "message"

Для того, чтобы добавить в commit изменения, необходимо выполнить команду:

    git commit -a

Для того, чтобы сразу выполнить добавление изменения в репозиторий с добавлением краткого описания изменения, нужно выполнить команду:

    git commit -am "message"

## Открытие логов внесенных изменений в репозиторий

Для того, чтобы открыть список внесенных изменений в репозиторий нужно выполнить команду:

    git log

Для того, чтобы открыть полный список всех внесенных в репозиторий изменений, нужно выполнить команду:

    git log --all

Для того, чтобы открыть список внесенных изменений в репозиторий с кратким номером commit одним списком, нужно выполнить команду:

    git log --oneline

## Перемещение между commit внутри репозитория

Для того, чтобы перейти к какому-либо из commit необходимо выполнить команду, где под hash понимается номер необходимого commit, допускается использования первых 6 значений номера:

    git checkout <hash>

## Отображение внесенного изменения в commit

Для того, чтобы вывести, что какое именно изменение было внесено в commit, необходимо выполнить команду:

    git diff

Для того, чтобы вывести разницу между интересующимися hash в commit, необходимо выполнить команду:

    git diff <hash1> <hash2>

где hash1 и hash2 - это номер commit в репозитории.

# Второй семинар

## Игнорирование файлов

Для того, чтобы заигнорировать файл необходимо создать в репозитории файл с названием .gitignore и поместить в него название необходимых файлов.

# Ветвление

Ветвление в Git нужны для корректной работы по нескольким направлениям одновременно над одним и тем же проектом.

## Просмотр всех веток

Для того, чтобы посмотреть полный список веток, необходимо выполнить команду git branch

## Создание новой ветки

Для создания новой ветки, необходимо выполнить команду git branch <name_branch>

## Перемещение между ветками

Для того, чтобы переместиться на другую ветку, необходимо выполнить команду:

    git checkout <name_branch>
    

## Удаление веток

Для того, чтобы удалить ветку, необходимо перейти в ветку master и выполнить команду:

    git branch -d <name_branch>

## Слияние веток

Для того, чтобы выполнить слияние веток, необходимо перейти в ветку в которую будет происходить слияние и выполнить команду:

    git merge <name_branch>
## Решение конфликтов

Для решения конфлитка при слиянии веток, выдается 3 варианта решения:
* Принять первый вариант
* Принять оба варианта
* Сравнить варианты

## Удаленные репозитории

Удаленные репозитории нужна для ...

## Создание нового репозитория

Чтобы создать новый репозиторий ...
