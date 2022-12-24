---
## Front matter
title: "Отчёт по лабораторной работе №4"
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

Освоить процедуры компиляции и сборки программ,
написанных на ассемблере NASM.

# Задание

# Теоретическое введение

# Выполнение лабораторной работы
1. Создам каталог для работы с программами на языке ассемблера NASM:
[рис.1](image/1.jpg){ #fig:001 width=90% }
2. Перейду в созданный каталог, создам текстовый файл с именем hello.asm
touch hello.asm, открою этот файл с помощью текстового редактора gedit:
[рис.2](image/2.jpg){ #fig:002 width=90% }
3. Введу указанный текст:
[рис.3](image/3.jpg){ #fig:003 width=90% }
4. Скомпиллирую исходный файл hello.asm в obj.o. С помощью команды ls
проверю, что файлы были созданы:
[рис.4](image/4.jpg){ #fig:004 width=90% }
Все создано.
5. Передам объектный файл на обработку компоновщику. С помощью
команды ls проверю, что исполняемый файл hello был создан:
[рис.5](image/5.jpg){ #fig:005 width=90% }
Все создано.
6. Выполню следующую команду:
[рис.6](image/6.jpg){ #fig:006 width=90% }
Исполняемый файл называется main, а объектный файл из которого собран
этот исполняемый файл obj.o.
7. Запущу на выполнение созданный исполняемый файл, находящийся в
текущем каталоге:
[рис.7](image/7.jpg){ #fig:007 width=90% }
Успешно
8. Выполнение самостоятельной работы:
[рис.8](image/8.jpg){ #fig:008 width=90% }

# Выводы

Я освоила процедуры компиляции и сборки программ, написанных на
ассемблере NASM.

# Список литературы{.unnumbered}

::: {#refs}
:::
