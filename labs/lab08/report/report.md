---
## Front matter
title: "Отчёт по лабораторной работе 8"
author: "Гиршфельд Александр Евгеньевич"

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

Получение навыков по организации циклов и работе со стеком на языке NASM.


# Выполнение лабораторной работы

Создадим все рабочие файлы и директории, напишем программу. Ее рабо-
та (рис. @fig:001).

![Цикл, выводящий цифры от 10 до 1](image/1.png){#fig:001 width=70%}

Далее попытаемся уменьшить изначальный индекс на 1. Получим результат,
отличный от ожидаемого(рис. @fig:002).Получим N/2 значений.

![Цикл, выводящий нечетные, меньшие 10](image/2.png){#fig:002 width=70%}

Чтобы получить нужный результат, воспользуемся коммандами push и pop.
Веведется как раз N значений.(рис. @fig:003).

![Цикл, выводящий цифры от 9 до 0](image/3.png){#fig:003 width=70%}

написали программу и все аргументы были обработаны(рис. @fig:004).

![работа програмы](image/4.png){#fig:004 width=70%}

Работа программы, которая складывает числа, введенные пользоваталем(рис. @fig:005).

![Сложение чисел](image/5.png){#fig:005 width=70%}

программы, которая умножает числа, введенные пользоваталем(рис. @fig:006).

![умножение чисел](image/6.png){#fig:006 width=70%}

Работа программы, которая умножает числа, введенные пользоваталем(рис. @fig:007).

![умножение чисел](image/7.png){#fig:007 width=70%}


Задание для самостоятельной работы

вариант 16

программа и ее работа, которая складывает значения формулы.(рис. @fig:008)(рис. @fig:009).

![программа](image/8.png){#fig:008 width=70%}
![работа программы](image/9.png){#fig:009 width=70%}


# Выводы

Были получены по организации циклов и работе со стеком на языке NASM.


