---
## Front matter
title: "Индивидуальный проект"
subtitle: "Этап 3"
author: "Владимир Баранов"

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

Добавить к сайту информацию о навыках, опыте и достижениях, а также разместить несколько постов.

# Выполнение лабораторной работы

1.  Введя команду ~/bin/hugo server, получаю ссылку на локальный сайт, на котором буду промежуточно отслеживать все изменения. Изменяю информацию о навыках, меняю навыки из шаблона на свои (рис. @fig:001).

![Навыки](image/01.png){#fig:001 width=90%}

2. Изменяю информацию об опыте, меняю опыт из шаблона на свой (рис. @fig:001).

![Опыт](image/02.png){#fig:001 width=90%}


3. Изменяю информацию о достижениях, меняю достижения из шаблона на свои (рис. @fig:001).

![Достижения](image/03.png){#fig:001 width=90%}

4. Введя команду ~/bin/hugo new post/last_week1, создаю новый пост на тему о прошедшей неделе (рис. @fig:001).

![Создание поста](image/04.png){#fig:001 width=90%}


5. Затем заполняю созданный пост информацией о прошедшей неделе. Далее проверяю изменения на локальном сайте, ссылку на который я получил в начале с помощью команды ~/bin/hugo server (рис. @fig:001) (рис. @fig:001).

![Пост 1](image/05.png){#fig:001 width=90%}

![Проверка поста 1](image/06.png){#fig:001 width=90%}


6. Создаю второй пост markdown, вновь используя команду ~/bin/hugo new post/markdown. Далее заполняю пост необходимой информацие. Проверяю изменения на локальном сайте, ссылку на который я получил в начале с помощью команды ~/bin/hugo server (рис. @fig:001) (рис. @fig:001).

![Пост 2](image/07.png){#fig:001 width=90%}

![Проверка поста 2](image/08.png){#fig:001 width=90%}


7. Затем в каталоге blog выполняю ~/bin/hugo (рис. @fig:001).

![~/bin/hugo](image/09.png){#fig:001 width=90%}

Затем отправляю изменения на сервер.

# Выводы

В ходе выполнения третьего этапа индивидуального проекта я добавил к сайту информацию о навыках, достижениях и опыте, а также разместил несколько постов.

