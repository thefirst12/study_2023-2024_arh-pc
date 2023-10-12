---
## Front matter
title: "Отчет по лабораторной работе №3"
subtitle: "Дисциплина: архитектура компьютера"
author: "Литвинов Максим Андреевич"

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

Целью работы является изучить принцип оформления отчетов с помощью легковесного языка разметки Markdown.

# Выполнение лабораторной работы

Переход в каталог курса с шаблоном отчета по Лабораторной работе №3, обновление локального репозитория с помощью команды git pull (рис. [-@fig:001]).

![Переход в каталог курса и обновления локального репозитория](image/1.png){ #fig:001 width=70% } 

Компиляция шаблона при помощи команды make (рис. [-@fig:002]).

![Компиляция шаблона](image/2.png){ #fig:002 width=70% }

Удаление полученных файлов и проверка факта удаления (рис. [-@fig:003]).

![Удаление файлов с использованием команды make clean](image/3.png){ #fig:003 width=70% }

Открытие файла report.md в текстовом редакторе (рис. [-@fig:004]).

![Открытие файла с шаблоном отчета при помощи команды gedit](image/4.png){ #fig:004 width=70% }

Отчет заполнен и скомпилирован (рис. [-@fig:005]).

![Готовый отчет](image/5.png){ #fig:005 width=70% }

# Выводы

Выполняя лабораторную работу, я приобрел практические навыки работы с языком разметки Markdown, при оформлении отчетов.

# Список литературы{.unnumbered}

::: {#refs}
:::
