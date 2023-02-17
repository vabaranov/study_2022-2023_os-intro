---
## Front matter
title: "Лабараторная работа 2."
subtitle: "Первоначальная настройка Git."
author: "Владимир Андреевич Баранов"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы
Целью данной лабораторной работы является изучить идеологию и применение средств контроля версий, а также освоить умения по работе с git.

# Задание

Создать базовую конфигурацию для работы с git.
Создать ключ SSH.
Создать ключ PGP.
Настроить подписи git.
Зарегистрироваться на Github.
Создать локальный каталог для выполнения заданий по предмету

# Выполнение лабораторной работы

1. Задам имя и email владельца репозитория, настрою utf-8 в выводе сообщений git

![Базовая настройка.](image/01.png){#fig:001 width=90%}

2. Задам имя начальной ветки и параметров 

![Базовая настройка.](image/02.png){#fig:002 width=90%}

3. Создаю ключ pgp 

![Генерация ключа.](image/03.png){#fig:003 width=90%}
![Создание ключа.](image/04.png){#fig:004 width=90%}

4. Добавляю PGP ключ в GitHub 

![Список ключей и копирование отпечатка.](image/05.png){#fig:005 width=90%}
![Добавление ключа.](image/06.png){#fig:006 width=90%}
![Полученный ключ добавляю  в GitHub.](image/07.png){#fig:007 width=90%}

5. Настрою автоматические подписи коммитов git 

![Авторизация.](image/08.png){#fig:008 width=90%}

6. Настрою GitHub 

![Авторизация.](image/09.png){#fig:009 width=90%}
![Авторизация.](image/10.png){#fig:010 width=90%}
![Авторизация.](image/11.png){#fig:011 width=90%}

7. Создаю репозиторий курса на основе шаблона 

![Создание репозитория.](image/12.png){#fig:012 width=90%}
![Создание репозитория.](image/13.png){#fig:013 width=90%}

8. Настрою каталог курса 

![Настройка каталога.](image/14.png){#fig:014 width=90%}
![Отправка файлов на сервер.](image/15.png){#fig:015 width=90%}
![Отправка файлов на сервер.](image/16.png){#fig:016 width=90%}

# Выводы

Мы изучили идеологию и применение средсв контроля версий, а также освоили умения по работе с Git.

# Контрольные вопросы

    1. Что такое системы контроля версий (VCS) и для решения каких задач они предназначаются?
    
    Ответ: Система, позволяющая работать нескольким людям над одним проектом.
    
    2. Объясните следующие понятия VCS и их отношения: хранилище, commit, история, рабочая копия.
   
    Ответ: хранилище-директория, хранящая конкретный проект; коммит-текущее состояние рабочей копии;истрия-последовательность коммитов;рабочая копия-текщее состояние репозитория, которое находится в состоянии изменения.
    
    3. Что представляют собой и чем отличаются централизованные и децентрализованные VCS? Приведите примеры VCS каждого вида.
    
    Ответ: в централизованнных все пользователи подключены к единому серверу, в децентрализованных пользователи подключены к нескольким владельцам.
    
    4. Опишите действия с VCS при единоличной работе с хранилищем.
    
    Ответ: при единоличной работе с хранилищем все изменения, созданные пользователем, не влияют на общий репозиторий.
    
    5. Опишите порядок работы с общим хранилищем VCS.
    
    Ответ: из общего хранилища можно получить изменения проекта.
    
    6. Каковы основные задачи, решаемые инструментальным средством git?
    
    Ответ: git позволяет нескольким людям работать над одним проектом.
    
    7. Назовите и дайте краткую характеристику командам git.
    
    Ответ: add-добавить файлы в коммит; push-отправить коммит на удаленный репозиторий;pull-импортировать проект с удаленного репозитория.
    
    8. Приведите примеры использования при работе с локальным и удалённым репозиториями.
    
    Ответ: 
    9. Что такое и зачем могут быть нужны ветви (branches)?
    
    Ответ: создав новую ветвь, можно, не вредя проекту, работать над конкретной частью проекта.
    
    10. Как и зачем можно игнорировать некоторые файлы при commit?
    
    Ответ: some files may well be user specific.


