---
## Front matter
title: "Шаблон отчёта по лабораторной работе 3"
subtitle: "Простейший вариант"
author: "Белла Александровна Пинега"

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

Нужно понять, как происходит процедура оформления отчетов
с помощью легковесного языка разметки Markdown.

Цель данного шаблона --- максимально упростить подготовку отчётов по
лабораторным работам.  Модифицируя данный шаблон, студенты смогут без
труда подготовить отчёт по лабораторным работам, а также познакомиться
с основными возможностями разметки Markdown.

# Задание

Здесь приводится описание задания в соответствии с рекомендациями
методического пособия и выданным вариантом.

# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. [-@tbl:std-dir] приведено краткое описание стандартных каталогов Unix.

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

Более подробно об Unix см. в [@gnu-doc:bash;@newham:2005:bash;@zarrelli:2017:bash;@robbins:2013:bash;@tannenbaum:arch-pc:ru;@tannenbaum:modern-os:ru].

# Выполнение лабораторной работы

Задание 3.4.
1. Открою терминал.
2. Перейду в каталог курса сформированный при выполнении лабораторной
работы No3 (arch-pc) с помощью команды cd (сменить директорию); обновлю
локальный репозиторий, скачав изменения из удаленного репозитория с
помощью команды git pull(см.рис.1):
![рис.1](image/1.1.png){ #fig:001 width=90% }
3. Перехожу в каталог с шаблоном отчета по лабораторной работе No 4(см.рис.2):![рис.2](image/1.2.png){ #fig:002 width=90% }
4. Проведу компиляцию шаблона с использованием Makefile при помощи
команды make(см.рис.3):![рис.3](image/6.1.png){ #fig:003 width=90% }
Успешно.
5. Удалю полученные файлы с использованием Makefile при помощи команды
make clean(см.рис.4):![рис.4](image/6.2.png){ #fig:004 width=90% }
Удалено.
6. Открою файл report.md c помощью текстового редактора, изучу структуру
этого файла(см.рис.5):![рис.5](image/6.3.png){ #fig:005 width=90% }
6. Загружу файлы на github.

# Выводы

Я научилась оформлять отчеты с помощью легковесного языка
разметки Markdown.

# Список литературы{.unnumbered}

::: {#refs}
:::
