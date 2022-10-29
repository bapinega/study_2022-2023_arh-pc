---
## Front matter
title: "Отчёт по лабораторной работе №2"
subtitle: "Архитектура вычислительных систем"
author: "Пинега Белла Александровна"

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

Изучить идеологию и применение средств контроля версий.
Приобрести практические навыки по работе с системой git.

# Задание



# Теоретическое введение


# Выполнение лабораторной работы
1. Настрою git: задам предварительную конфигурацию git, настрою utf-8, задам имя начальной ветки, парамтеры autocrlf и safecrlf:
[рис.1](image/7.1.png){ #fig:001 width=90% }
Базовые настройки git заданы.
2. С помощью «ssh-keygen -C "Имя Фамилия "» сгенерирую ключи. А затем
введу «cat ~/.ssh/id_rsa.pub | xclip -sel clip», и полученные в буфере обмена ключи, вставлю на github в окно, находящееся во вкладке «new ssh key»:
[рис.2](image/7.2.png){ #fig:002 width=90% }
3. Создам каталог для предмета архитектуры компьютера:
[рис.3](image/7.3.png){ #fig:003 width=90% }
4. Создам репозиторий, затем перейду в каталог курса и клонирую созданный репозиторий:
[рис.4.1](image/7.4.png){ #fig:004 width=90% }
[рис.4.2](image/7.5.png){ #fig:005 width=90% }
5. Удалю лишние файлы:
[рис.5](image/7.6.png){ #fig:006 width=90% }
Удаление прошло успешно.
6. Создам каталоги и отправлю файлы на сервер:
[рис.6.1](image/7.7.png){ #fig:007 width=90% }
[рис.6.2](image/7.8.png){ #fig:008 width=90% }
7. Проверю правильность создания иерархии в репозитории и на github:
[рис.7.1](image/7.9.png){ #fig:009 width=90% }
[рис.7.2](image/8.png){ #fig:010 width=90% }
Все верно.
8. Создаю отчет по выполнению текущей лабораторной No2 в соответствующий каталог github lab2:
[рис.8](image/8.1.png){ #fig:011 width=90% }
Затем копирую отчет предыдущей работы No1 в lab1:
[рис.9](image/8.2.png){ #fig:012 width=90% }
Загружаю все файлы на github


# Выводы

В ходе выполнения лабораторной работы я изучила идеологию и
применение средств контроля версий, у меня появились практические навыки по работе с системой git и платформой github.

# Список литературы{.unnumbered}

::: {#refs}
:::
