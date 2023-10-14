---
## Front matter
title: "Отчет по лабораторной работе №2"
subtitle: "Дисциплина: Архитектура вычислительных систем"
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

Целью работы является изучить идеологию и применение средств контроля версии. Приобрести практические навыки по работе с системой git.

# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. @tbl:std-dir приведено краткое описание стандартных каталогов Unix.

: Описание некоторых каталогов файловой системы GNU Linux {#tbl:std-dir}

| Имя каталога | Описание каталога                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| `/`          | Корневая директория, содержащая всю файловую                                                                               |
| `/bin `      | Основные системные утилиты, необходимые как в однопользовательском режиме, так и при обычной работе всем пользователям     |
| `/etc`       | Общесистемные конфигурационные файлы и файлы конфигурации установленных программ                                           |
| `/home`      | Содержит домашние директории пользователей, которые, в свою очередь, содержат персональные настройки и данные пользователя |
| `/media`     | Точки монтирования для сменных носителей                                                                                   |
| `/root`      | Домашняя директория пользователя  `root`                                                                                   |
| `/tmp`       | Временные файлы                                                                                                            |
| `/usr`       | Вторичная иерархия для данных пользователя                                                                                 |

# Выполнение лабораторной работы

Необходимо произвести базовую настройку git, указав имя и email владельца репозитория (рис. @fig:001).

![Рис 1.1 – Базовая настройка git](image/1.jpg){#fig:001 width=70%}

Далее воспользуемся core.autocrlf(настройка в Git, которая предназначена для приведения переводов строк текстовых файлов в главном репозитории к единому виду)

![Рис 1.2 – Применение core.autocrlf](image/2.jpg){#fig:002 width=70%}

Теперь воспользуемся core.safecrlf с параметром warn(команда проверяет является ли процесс обратимым, если нет, то высылает предупреждение)

![Рис 1.3 – Применение core.safecrlf с параметром warn](image/3.jpg){#fig:003 width=70%}

Теперь необходимо создать SHH-ключ, для идентификации на сервере репозиториев

![Рис 2.1 – Генерация приватного и открытого ключа](image/4.png){#fig:004 width=70%}

Необходимо создать рабочее пространство на основе шаблона
Часть работы уже предоставлена нам в готовом виде, требуется лишь создать каталог “Архитектура компьютера”

![Рис 2.2 – Создание каталога “Архитектура компьютера” с помощью команды mkdir](image/5.jpg){#fig:005 width=70%}

Создание репозитория курса на основе шаблона Создание репозитория возможно через web-версию

![Рис 3.1 – Создание репозитория](image/6.jpg){#fig:006 width=70%}

Перед клонированием необходимо перейти в каталог курса

![Рис 3.2 - Переход в каталог курса, копирование ссылки для клонирования](image/7.jpg){#fig:007 width=70%}

Переходим к настройке каталога курса, которая состоит из удаления ненужных файлов и создания необходимых каталогов

![Рис 4.1 – Создание необходимых каталогов, отправка файлов на сервер](image/8.jpg){#fig:008 width=70%}

# Выводы

Выполняя лабораторную работу, я приобрел практические навыки работы с системой git. Разобрался в основных командах, настройке git, идентификации пользователя на сервере репозиториев и в создании, настройке каталога курса.

# Список литературы{.unnumbered}

::: {#refs}
:::
