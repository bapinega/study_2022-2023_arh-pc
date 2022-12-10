---
## Front matter
title: "Отчёт по лабораторной работе 5"
subtitle: "НБИбд-02-22"
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

Приобретение практических навыков работы в Midnight Commander. Освоение инструкций языка ассемблера mov и int.

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
1. Открою Midnight Commander:
2. Перехожу в каталог ~/work/arch-pc:
![рис.1](image/1.1.png){ #fig:001 width=90% }
3. С помощью клавиши F7 создаю папку lab06:![рис.2](image/1.2.png){ #fig:002 width=90% }
4. Пользуясь строкой ввода и командой touch создаю файл lab6-1.asm. С помощью клавиши F4 открою файл lab6-1.asm:![рис.3](image/6.1.png){ #fig:003 width=90% }
Успешно.
5. Введу текст программы 6.1. С помощью клавиши F3 откройте файл lab6-1.asm убеждаюсь, что файл содержит текст программы:![рис.4](image/6.2.png){ #fig:004 width=90% }
Удалено.
6. Выполняю компоновку объектного файла и запускаю получившийся исполняемый![рис.5](image/6.3.png){ #fig:005 width=90% }
7. С помощью клавиши F6 создаю копию файла lab6- 1.asm с именем lab6-2.asm:[рис.6](image/6.4.png){ #fig:006 width=90% }
8. Заменяю подпрограмму sprintLF на sprint:[рис.7](image/6.5.png){ #fig:006 width=90% }
9. Создаю копию файла lab6-1.asm. Вношу изменения, так чтобы она работала по алгоритму:[рис.8](image/6.6.png){ #fig:007 width=90% }
10. Проверяю работу: [рис.5](image/6.7.png){ #fig:008 width=90% }

# Выводы

Я научислась работать в Midnight Commander. И освоила инструкции языка ассемблера mov и int.

# Список литературы{.unnumbered}

::: {#refs}
:::
