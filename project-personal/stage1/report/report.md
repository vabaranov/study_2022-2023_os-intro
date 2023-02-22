---
## Front matter
title: "Индивидуальный проект."
subtitle: "Этап 1."
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

Приобрести практические навыки создания заготовки персонального сайта.

# Выполнение лабораторной работы

1. Скачиваю файл hugo_extended_0.110.0_Linux-64bit.tar.gz и клонирую файл hugo в папку bin (рис. @fig:001).

![Клонирование.](image/01.png){#fig:001 width=90%}

2. Открыва. сайт (рис. @fig:002).

![Сайт.](image/02.png){#fig:002 width=90%}

3. Cоздаю репозиторий blog (рис. @fig:003).

![Новый репозиторий.](image/03.png){#fig:003 width=90%}

4. Клонирую новый репозиторий (рис. @fig:004)

![Клонирование.](image/04.png){#fig:004 width=90%}

5. Создаю main ветку (рис. @fig:005)

![переключение на ветку main.](image/05.png){#fig:005 width=90%}

6. Cоздаю еще один репозиторий vabaranov.github.io(рис. @fig:006)

![Новый репозиторий 2.0.](image/06.png){#fig:006 width=90%}

7. Подключение репозитория к папке public (рис. @fig:007)

![Подключение.](image/07.png){#fig:007 width=90%}

8. Исправляю ошибку и делаю это еще раз (рис. @fig:008)

![Переподключение.](image/08.png){#fig:008 width=90%}

9. Командой bin hugo cоздаю в папке файлы (рис. @fig:009)

![терминал](image/09.png){#fig:009 width=90%}

10. Пушу на гитхаб созданные файлы (рис. @fig:010)

![Загрузка.](image/10.png){#fig:010 width=70%}

11. Мой сайт (рис. @fig:011)

![Сайт.](image/11.png){#fig:011 width=90%}


# Выводы

В ходе данной работы я приобрел практические навыки создания заготовки персонального сайта.
:::
