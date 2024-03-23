---
## Front matter
title: "Лабораторная работа №3"
subtitle: "Markdown"
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

1. Получение базовых навыков работы с Markdown

# Задание

Написание отчёта по выполнению лабораторной работы №2

# Выполнение лабораторной работы

Откроем шаблон отчёта в текстовом редакторе neovim(Рис.1)

![Открытие шаблона командой nvim](image/lab1.png)

Изменим название, подзаголовок и авторство на подходящие нам(Рис.2)

![Изменение заголовка, подзаголовка и авторства](image/lab2.png)

Напишем цель нашей работы(Рис.3)

![Цель работы](image/lab3.png)

Напишем задания в нашей лабораторной работе(Рис.4)

![Задания](image/lab4.png)

Опишем выполнение лабораторной работы с иллюстрациями(Рис.5)

![Описание выполнения лабораторной работы](image/lab5.png)

Напишем ответы на контрольные вопросы(Рис.6)

![Ответы на контрольные вопросы](image/lab6.png)

Напишем вывод(Рис.7)

![Вывод](image/lab7.png)

# Выводы

Я научился работать с Markdown


