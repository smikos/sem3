# **Инструкция по работе с Git**
![emblem](t.jpg)

Система контроля версии Git нужна для сохранений разных версий программы. Для отслеживаний всех изменений и удобства отката версий.

## Создание локального репозитория

Чтобы создать (иницилизировать) новый локальный репозиторий нужно в терминале (находясь в нужной папку) ввести команду:

    git init

## Проверка состояния репозитория

Чтобы посмотреть состояние проекта, изменные и добавленные файл. Нужно ввести команду:

    git status
## Добавление файлов
Для такого чтоб добавить новые или измененные файлы из вашего рабочего каталога нужна команда:

    git add "filename"
Можно добавить все изменения , командой

    git add .

## Создание коммитов

Чтоб создать сохранение (коммит) нужно использовать команду:

    git commit 
  чтоб сразу был комент использовать можно:

    git commit –m “Комментарий к коммиту”
    
 комбинация параметров создает коммит всех проиндексированных изменений и добавляет к коммиту подставленный комментарий

    git commit -am"комментарий"

## Просмотр

Просмотреть коммиты можно при помощи команды:

    git log

чтоб были только коммиты и сокр коды нужна команда:

    git log --oneline

чтоб смотреть все ( в случае если в старой версии ты)

    git log --all

чтоб смотреть все и сокр было

    git log --oneline --all

## Переключение 

Чтоб сменить директорию и откатить состояние назад используй команду :

    git checkout <hash коммита>
чтоб вернуться на главную ( на последнию , где остановился)

    git checkout master

## Изменение 

Чтоб показать изменения между фиксациями, фиксацией и рабочим деревом и т. д.

    git diff

Чтоб посмотреть изменения между определенными коммитами надо :

    git diff (hash1) (hash2)

   ## Ветвление в Git

   Ветвления нужны для указываения других коммитов

      

### Просмотр существующих веток

Для просмотра имеющихся веток используется команда

    git branch

## Создание новой ветки

Для создания нвой ветки используется команда :

    git branch "branch_name"
    
### Переключение между ветками

Для того чтобы переключиться на другую ветку используется команда:

    git checkout <branch_name>

## Удаление ветки

Чтоб удалить ветку нужна команда:

     git branch -d "branch_name"

## Соединение 

Чтоб соединить ветки надо использовать команду:

     git merge "branch_name"

## Конфликты 

Конфликты возникают в связи с разной информацией в ветке и мастере при их соединение .

Решение конфликтов бывает автоматическое и ручное. В ручном нужно выбрать , вносим мы изменения из ветки но удаляем из мастера, оставляем из мастера и не вносим из ветки , и можно объединить их.

### Полный просмотр

Чтоб смотреть все коммиты в коротком ввиде плюс ветки branch нужно использовать команду

    git log --oneline --all --graph

## Удаленные репозитории
Удаленные репозитори используется, для возможности работы с файлом из любой точки и с любого пк у которого есть доступ к сети.
