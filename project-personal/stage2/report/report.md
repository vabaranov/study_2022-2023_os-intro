---
## Front matter
title: "Индивидуальный проект"
subtitle: "Этап 2"
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

Добавить к сайту данные о себе, а также разместить несколько постов.

# Задание

Разместить фотографию владельца сайта.

Разместить краткое описание владельца сайта (Biography).

Добавить информацию об интересах (Interests).

Добавить информацию об образовании (Education).

Сделать пост по прошедшей неделе.

Добавить пост на тему по выбору:

   - Управление версиями. Git.
   
   - Непрерывная интеграция и непрерывное развертывание (CI/CD).

# Выполнение лабораторной работы

1. Размещаю фотографию владельца сайта, для этого заменяю фото из шаблона на свое (рис. @fig:001).

![Замена фото.](image/1.png){#fig:001 width=90%}

2. Размещаю основную информацию: мое имя, название университета и ссылка на сайт, краткое описание владельца сайта, добавляю информацию об интересах и об образовании (рис. @fig:002).

![Основная информация.](image/2.png){#fig:002 width=90%}

3. Получив ссылку на локальный сайт с помощью ~/bin/hugo server, проверяю изменения содержимого (рис. @fig:003).

![Проверка содержимого.](image/3.png){#fig:003 width=90%}

4. Создаю пост о прошедшей неделе, размещая необходимую информацию. Для этого выполняю команду ~/bin/hugo new post/last_week и заполняю пост информацией, проверяю содержимое на сайте (рис. @fig:005) (рис. @fig:004).

![Пост 1.](image/5.png){#fig:005 width=90%}

![Пост 1(проверка).](image/4.png){#fig:004 width=90%}

5. Затем создаю пост на тему Аналогично пункту 3 выполняю команду ~/bin/hugo new post/Git и заполняю пост информацией (рис. @fig:006).

![Пост 2.](image/6.png){#fig:006 width=90%}

6. Затем я проверяю публичный сайт. Убеждаюсь, что все выполнилось корректно (рис. @fig:007).

![Пост 2(проверка).](image/7.png){#fig:007 width=90%}

# Выводы

В ходе выполнения второго этапа индивидуального проекта я добавил к сайту данные о себе, а также разместил несколько постов.

::: {#refs}
:::
