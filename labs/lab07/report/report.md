---
## Front matter
title: "Отчет по лабораторной работе №7"
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

Изучить основы работы комманд усовного и безусловного перехода в assembler.


# Выполнение лабораторной работы

Создадим рабочую папку и рабочий файл (рис. @fig:001).

![создание папки и файла](image/1.png){#fig:001 width=70%}

Запишем в файл код, проассемблируем его, запустим(рис. @fig:002)

![запуск файла](image/2.png){#fig:002 width=70%}

зменим программу так, чтобы она выводила второе,затем первое сообщение и завершала работу. Её код (рис. @fig:003) и работа (рис. @fig:004)

![код програмы](image/3.png){#fig:003 width=70%}
![работа програмы](image/4.png){#fig:004 width=70%}

Еще напишем программу, выводящую сообщения в обратном порядке(рис. @fig:005) (рис. @fig:006)

![код програмы](image/5.png){#fig:005 width=70%}
![работа програмы](image/6.png){#fig:006 width=70%}

Напишем программу с условным переходом(рис. @fig:007)

![работа програмы](image/7.png){#fig:007 width=70%}

Рассмотрим файл листинга одной из программ(рис. @fig:008)
 ![Часть файла листинга](image/8.png){ #fig:008 width=70% }

в строке 9 содержится собственно номер сторки [9], адресс [00000003], машинный код [803800] и содержимое строки кода [cmp byte [eax], 0] в строке 11 содержится номер сторки [11], адресс [00000008], машинный код [40] и содержимое строки кода [inc eax] в строке 24 содержится номер сторки [24], адресс [0000000F], машинный код [52] и содержимое строки кода [push edx]

Если в коде появляется ошибка, то ее описание появится в файле листинга

Задания для самостоятельной работы

вариант 16

программа для сравнения трех заранее известных чисел(рис. @fig:009) и ее работа(рис. @fig:010)

![програма](image/9.png){ #fig:009 width=70% }
![работа програмы](image/10.png){ #fig:010 width=70% }

Программа для вычисления выражения в зависимости от условия на одну из вводимых переменных(рис. @fig:011) (рис. @fig:012)и ее работа(рис. @fig:013)

![програма](image/11.png){ #fig:011 width=70% }
![програма](image/12.png){ #fig:012 width=70% }
![работа програмы](image/13.png){ #fig:013 width=70% }


# Выводы

Были изучены основные принципы работы с условным и безусловным переходом в assembler и изучены основы чтения файлов листинга.

