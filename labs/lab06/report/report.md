---
## Front matter
title: "Лабараторная работа 6"
subtitle: "Поиск файлов.Перенаправление ввода-вывода.Просмотр запущенных процессов."
author: "Баранов Владимир Андреевич"

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

Ознакомление с инструментами поиска файлов и фильтрации текстовых данных. Приобретение практических навыков: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

# Задание



    Осуществите вход в систему, используя соответствующее имя пользователя.

    Запишите в файл file.txt названия файлов, содержащихся в каталоге /etc. Допишите в этот же файл названия файлов, содержащихся в вашем домашнем каталоге.

    Выведите имена всех файлов из file.txt, имеющих расширение .conf, после чего запишите их в новый текстовой файл conf.txt.

    Определите, какие файлы в вашем домашнем каталоге имеют имена, начинавшиеся с символа c? Предложите несколько вариантов, как это сделать.

    Выведите на экран (по странично) имена файлов из каталога /etc, начинающиеся с символа h.

    Запустите в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log.

    Удалите файл ~/logfile.

    Запустите из консоли в фоновом режиме редактор gedit.

    Определите идентификатор процесса gedit, используя команду ps, конвейер и фильтр grep. Как ещё можно определить идентификатор процесса?

    Прочтите справку (man) команды kill, после чего используйте её для завершения процесса gedit.

    Выполните команды df и du, предварительно получив более подробную информацию об этих командах, с помощью команды man.

    Воспользовавшись справкой команды find, выведите имена всех директорий, имеющихся в вашем домашнем каталоге.


# Теоретическое введение

Перенаправление ввода-вывода — возможность командной оболочки ряда операционных систем перенаправлять стандартные потоки в определённое пользователем место.

Команда find используется для поиска и отображения на экран имён файлов, соответствующих заданной строке символов. Формат команды: find путь [-опции]

Любой команде, выполняемой в системе, присваивается идентификатор процесса (process ID). Получить информацию о процессе и управлять им, пользуясь идентификатором процесса, можно из любого окна командного интерпретатора.

# Выполнение лабораторной работы
1. Осуществляю вход в систему, используя соответствующее имя пользователя.

2. Записываю в файл file.txt названия файлов, содержащихся в каталоге /etc. Затем дописываю в этот же файл названия файлов, содержащихся в моем домашнем каталоге (рис. @fig:001).

![Запись и добавление.](image/01.png){#fig:001 width=90%}

3. Вывожу имена всех файлов из file.txt, имеющих расширение .conf, и записываю их в новый текстовой файл conf.txt (рис. @fig:002).

![Вывод имен.](image/02.png){#fig:002 width=90%}

4. Определяю, какие файлы в домашнем каталоге имеют имена, начинавшиеся с символа c, используя grep и find(рис. @fig:003).

![Использоапние grep и find](image/03.png){#fig:003 width=90%}

5. Вывожу на экран имена файлов из каталога /etc, начинающиеся с символа h, используя команду find (рис. @fig:004).

![find](image/04.png){#fig:004 width=90%}

6. Запускаю в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log, для этого в конце команды ставлю & (рис. @fig:005).

![Запуск процесса.](image/05.png){#fig:005 width=90%}

7. Удаляю файл ~/logfile, используя команду rm (рис. @fig:006).

![Удаление файла.](image/06.png){#fig:006 width=90%}

8. Запускаю из консоли в фоновом режиме редактор gedit (рис. @fig:007).

![Запуск gedit](image/07.png){#fig:007 width=90%}

9. Определяю идентификатор процесса gedit, используя команду ps, конвейер и фильтр grep, также определяю идентефикаторы всех запущенных процессов с помощью команды ps (рис. @fig:008)  (рис. @fig:009).

![ps](image/08.png){#fig:008 width=90%}

![ps](image/09.png){#fig:009 width=90%}

10. Получаю справку команды kill с помощью команды man, после чего ипользую её для завершения процесса gedit (рис. @fig:010).

![kill](image/10.png){#fig:010 width=90%}

11. Выполняю команду df, предварительно получив более подробную информацию о ней с помощью команды man (рис. @fig:011).

![df](image/11.png){#fig:011 width=90%}

12. Воспользовавшись справкой команды find, вывожу имена всех директорий, имеющихся в домашнем каталоге (рис. @fig:012).

![find](image/12.png){#fig:012 width=90%}

# Выводы

Я ознакомилcя с инструментами поиска файлов и фильтрации текстовых данных, а также приобрел практические навыки по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

# Контрольные вопросы 

1. Какие потоки ввода вывода вы знаете?

– stdin — стандартный поток ввода (по умолчанию: клавиатура), файловый дескриптор 0;

– stdout — стандартный поток вывода (по умолчанию: консоль), файловый дескриптор 1;

– stderr — стандартный поток вывод сообщений об ошибках (по умолчанию: консоль), файловый дескриптор 2.

2. Объясните разницу между операцией > и >>.

“>” - это открывает файл на перезапись, когда “>>” открывает файл на дозапись.

3. Что такое конвейер?

Конвейер – это направление вывода на вход для следующей команды.

4. Что такое процесс? Чем это понятие отличается от программы?

Процесс - это исполняемая программа. Программа - это набор инструкций, которые выполняют определенную задачу при выполнении компьютером, в то время как процесс является экземпляром выполняемой компьютерной программы. Таким образом, в этом главное отличие программы и процесса.

5. Что такое PID и GID?

PID: это идентификатор процесса (PID) процесса, который вы вызываете. GID: идентификатор группы. Все группы Linux определяются GID (идентификаторами групп). GID хранятся в файле / etc / groups.

6. Что такое задачи и какая команда позволяет ими управлять?

Любую выполняющуюся в консоли команду или внешнюю программу можно запустить в фоновом режиме. Для этого следует в конце имени команды указать знак амперсанда &. Например: gedit &

7. Найдите информацию об утилитах top и htop. Каковы их функции?

Top - отобразить запущенные процессы, используемые ими ресурсы и другую полезную информацию (с автоматическим обновлением данных).

Htop - показывает динамический список системных процессов, список обычно выравнивается по использованию ЦПУ. В отличие от top, htop показывает все процессы в системе. Также показывает время непрерывной работы, использование процессоров и памяти. Htop часто применяется в тех случаях, когда информации даваемой утилитой top недостаточно, например при поиске утечек памяти в процессах.

8. Назовите и дайте характеристику команде поиска файлов. Приведите примеры использования этой команды.

Команда find используется для поиска и отображения на экран имён файлов, соответствующих заданной строке символов. Формат команды: find путь

9. Можно ли по контексту (содержанию) найти файл? Если да, то как?

Да, воспользовавшись командой grep. Формат команды: grep строка имя_файла.

10. Как определить объем свободной памяти на жёстком диске?

Для определения объёма свободного пространства на файловой системе можно воспользоваться командой df, которая выведет на экран список всех файловых систем в соответствии с именами устройств, с указанием размера и точки монтирования.

11. Как определить объем вашего домашнего каталога?

Команда du показывает число килобайт, используемое каждым файлом или каталогом.

12. Как удалить зависший процесс?

Команда kill служит для завершения процесса.


::: {#refs}
:::
