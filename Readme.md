# Инструкция по работе с git

## Что такое система контроля версий  
Система управления версиями (также используется определение «система контроля версий», от англ. Version Control System, **VCS** или Revision Control System) — программное обеспечение для облегчения работы с изменяющейся информацией.  
Система управления версиями позволяет хранить несколько версий одного и того же документа, при необходимости возвращаться к более ранним версиям, определять, кто и когда сделал то или иное изменение, и многое другое.

## Что такое git?
Git - это одна из реализаций распределенных систем конроля версий. Git позволяет управлять нашими изменениями, создавать фиксации и т.п...  
*(Тут, типа, делал конфликт. И вроде бы разрулил его.)*

## Подготовка репозитория
Репозиторий это хранилище файлов поддерживающее версионность. 
Создать репозиторий можно с помощью применения в папке команды  

**git init** - Создаёт новый локальный репозиторий с заданным именем

**git clone [url-адрес]** - Скачивает репозиторий вместе со всей его историей изменений

## Внесение изменений. Просмотр изменений и создание коммитов (фиксация изменений).

**git status** - Перечисляет все новые или изменённые файлы, которые нуждаются в фиксации.

**git diff** - Показывает различия по внесённым изменениям в ещё не проиндексированных файлах.

**git add [файл]** - Индексирует указанный файл для последующего коммита.

**git diff --staged** - Показывает различия между проиндексированной и последней зафиксированной версиями файлов.

**git reset [файл]** - Отменяет индексацию указанного файла, при этом сохраняет его содержимое.

**git commit -m "[сообщение с описанием]"** - Фиксирует проиндексированные изменения и сохраняет их в историю версий.

## Перемещение между сохранениями
Перемещаться между нашими сохранениями можно с помощью команды *git checkout*. Для этого достаточно применить команду *git checkout <номер коммита>*.
Можно отменить изменения с помощью команд *git revert* и *git reset*.  
*git revert <номер коммита>* отменяет изменения до указанной версии и создаст новый коммит.  
*git reset --hard <номер коммита>* отменяет изменения до указанного коммита и затрет всю историю изменений после этого коммита.

## Журнал изменений

## Ветки в git

## Слияние веток и решение конфликтов

## Удаление веток

## Скачивание удаленного репозитория

## Примечание

> **Скопировать нахрен все отсюда https://training.github.com/downloads/ru/github-git-cheat-sheet/ , откорректировать, и если останется смысл, дозаполнить что-то из оставшихс подзаголовков!**