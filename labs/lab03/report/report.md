---
## Front matter
title: "Отчет по лабораторной работе №3"
subtitle: "Архитектура вычислительных систем"
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

Нужно понять, как происходит процедура оформления отчетов с помощью легковесного языка разметки Markdown.

# Задание

1. В соответствующем каталоге сделайте отчёт по лабораторной работе No 3
в формате Markdown. В качестве отчёта необходимо предоставить отчёты
в 3 форматах: pdf, docx и md.
2. Загрузите файлы на github.

# Теоретическое введение


# Выполнение лабораторной работы

   1. Открою терминал.
   2. Перейду в каталог курса сформированный при выполнении лабораторной работы No3 (arch-pc) с помощью команды cd (сменить директорию); обновлю локальный репозиторий, скачав изменения из удаленного репозитория с помощью команды git pull(см.рис.[-@fig:001]): [1](image/1.1.png){ #fig:001 width=90% }
   3. Перехожу в каталог с шаблоном отчета по лабораторной работе No 4(см.рис.[-@fig:002]):[2](image/1.2.png){ #fig:002 width=90% }
   4. Проведу компиляцию шаблона с использованием Makefile при помощи команды make(см.рис.[-@fig:003]):[3](image/6.1.png){ #fig:003 width=90% } Успешно.
   5. Удалю полученные файлы с использованием Makefile при помощи команды make clean(см.рис.[-@fig:004]):[4](image/6.2.png){ #fig:004 width=90% } Удалено.
   6. Открою файл report.md c помощью текстового редактора, изучу структуру этого файла(см.рис.5[-@fig:005]):[5](image/6/3.png){ #fig:005 width=90% }
   7. Загружу файлы на github.


# Выводы

Я научилась оформлять отчеты с помощью легковесного языка разметки Markdown.

# Список литературы{.unnumbered}

::: {#refs}
:::
