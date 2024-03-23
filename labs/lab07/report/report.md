---
## Front matter
title: "Лабораторная работа №7"
subtitle: "Анализ файловой системы Linux. Команды для работы с файлами и каталогами"
author: "Приспешкин Андрей Андреевич"

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

Ознакомление с файловой системой Linux, её структурой, именами и содержанием
каталогов. Приобретение практических навыков по применению команд для работы
с файлами и каталогами, по управлению процессами (и работами), по проверке исполь-
зования диска и обслуживанию файловой системы.

# Задание

    Выполнить все примеры из лабораторной работы
    Выполнить команды по копированию, созданию и перемещению файлов и каталогов
    Определить опции команды chmod
    Изменить права доступа к файлам
    Прочитать документацию о командах mount, fsck, mkfs, kill

# Выполнение лабораторной работы

Создадим файл abc1 и скопируем из него два новых файла april и may(Рис.1)

![Копирование файлов april и may](image/1.png)

Создадим каталог monthly и скопируем туда файлы april и may(Рис.2)

![Копирование файлов в каталог](image/2.png)

Переименум may в june(Рис.3)

![Переименование may в june](image/3.png)

Рекурсивно скопируем каталог monthly.00 в каталог /tmp(Рис.4)

![Рекурсивное копирование каталога](image/4.png)

Переименуем april в july и переместим july в каталоге monthly.00(Рис.5)

![Переименование и перемещение файла](image/5.png)

Создадим каталог reports и переместим туда каталог monthly.01, затем переименуем monthly.01 в monthly(Рис.6)

![Создание и переименование каталога](image/6.png)

Создадим файл may, проверим его права доступа, и добавим право на выполнение(Рис.7)

![Проверка и изменение прав доступа](image/7.png)

Затем уберём у файла may право на выполнение(Рис.8)

![Отмена прав на выполнение](image/8.png)

Копируем файл io.h из каталога /usr/include/sys в домашний каталог и переименуем его в equipment, затем создадим каталог ski.plases и переместим туда скопированный нами файл(Рис.9)

![Копирование файла io.h и создание каталога ski.plases](image/9.png)

Переместим файлы equiplist1 и equiplist2 в каталог ski.plases/equipment(Рис.10)

![Перемещение файлов](image/10.png)

Создадим каталог newdir и переместим его в ski.plases дав ему название plans(Рис.11)

![Перемещние каталога с новым именем](image/11.png)

Утилитой cat выведем в командную строку содержимое файла /etc/passwd(Рис.12)

![Вывод содержимого на экран](image/12.png)

Создадим файл feathers, переименуем его с копированием в файл file.old, создадим каталог play и переместим туда file.old, затем создадим каталог fun и рекурсивно копируем в него каталог play(Рис.13)

![Создание файла, копирование и рекурсивное копирование каталогов](image/13.png)

Заберём у файла feathers право на чтение и попытаемся вывести на экран его содержимое, заметим что нам отказано в доступе. Затем попробуем скопировать файл feathers в feathers1, заметим что ошибка повторяется. Вернём файлу feathers право на чтение.

![Пример попыток работы с файлами без права на чтение](image/14.png)

Заберём у каталога play право на выполнение и попробуем перейти в него, заметим что нам отказано в доступе(Рис.15)

![Попытка перейти в каталог без права на выполнение](image/15.png)

Прочитай мануалы к командам mount, fsck и kill(Рис.16)

![Команда для вывода на экран мануалов](image/16.png)

# Выводы

Я ознакомился с файловой системой Linux и приобрёл практические навыки по применению команд для работы с файлами и каталогами


