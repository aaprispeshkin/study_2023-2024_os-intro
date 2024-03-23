---
## Front matter
title: "Индивидуальный проект"
subtitle: "Первый этап"
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

Научится размещать страницы на Github pages. Начать реализацию индивидуального проекта.

# Задание

1. Скачать шаблон сайта
2. Разместить его на git 
3. Установить параметры URL сайта
4. Разместить сайт на Github pages

# Выполнение лабораторной работы

Создаём репозиторий сайта на основе шаблона(Pис.1)

![Создание репозитория на основе шаблона](image/lab1.png)

Клонируем репозиторий в рабочий каталог 

![Клонирование репозитория в рабочий каталог](image/lab2.png)

Запустим Hugo(Рис.3)

![Первый запуск Hugo](image/lab3.png)

Удалим папку public созданную в ходе работы Hugo(Рис.4)

![Удаление папки public в Midnight Commander](image/lab4.png)

Запустим Hugo server для создания локальной версии шаблона сайта(Рис.5)

![Работа Hugo server](image/lab5.png)

Создадим новый репозиторий который будет адресом нашего сайта(Рис.6)

![Создание нового репозитория](image/lab6.png)

Перейдём в созданный нами каталог нового репозитория, создадим там ветку main и файл README(Рис.7)

![Создание ветки main и файла README](image/lab7.png)

Изменим содержание файла .gitignore в каталоге шаблона, для успешного слияния двух наших каталогов(Рис.8)

![Изменение .gitignore](image/lab8.png)

Произведём слияние наших репозиториев(Рис.9)

![Слияние репозиториев](image/lab9.png)

Ещё раз запустим Hugo, в этот раз с уже созданной нами заранее папкой public(Рис.10)

![Второй запуск Hugo](image/lab10.png)

Проверим то что наша папка public может достичь сервера и сохраним наши изменения с помощью git commit(Рис.11)

![Проверка и сохранение изменений](image/lab11.png)

# Выводы

Я научился размещать сайты на Github pages тем самым выполнив первый этап реализации проекта.

