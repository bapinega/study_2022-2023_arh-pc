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

Освоение арифметических инструкций языка ассемблера NASM.

# Задание

# Теоретическое введение

# Выполнение лабораторной работы
1. Создаю каталог для программам лабораторной работы, перехожу в него и создаю файл lab7-1.asm: 
[рис.1](image/1.jpg){ #fig:001 width=90% }
2. С помощью команды gedit открываю файл и ввожу листинг:
[рис.2](image/2.jpg){ #fig:002 width=90% }
3. Создаю исполняемый файл и запускаю:
[рис.3](image/3.jpg){ #fig:003 width=90% }
4. Заменяю строки в соответствии с заданием и на выводе получаю следующее:
[рис.4](image/4.jpg){ #fig:004 width=90% }
Код 10 соответсвует символу перевода строки LF, \n.
5. Создаю файл lab7-2.asm в каталоге ~/work/arch-pc/lab07, ввожу в него текст программы из листинга и запускаю:
[рис.5](image/5.jpg){ #fig:005 width=90% }
На вывод получаю 106
6. Заменю символы на числа:
[рис.6](image/6.jpg){ #fig:006 width=90% }
Получен результат 10.
7. Заменю функцию iprintLF на iprint, создам исполняемый файл и запущу его:
[рис.7](image/7.jpg){ #fig:007 width=90% }
Отличаются  iprintLF и iprint тем, что при iprint не переносится строка.
8. Создам файл lab7-3.asm, изучу текст программы из листинга и введу в lab7-3.asm. Создам исполняемый файл и запущу его:
[рис.8](image/8.jpg){ #fig:008 width=90% }
Результат совпал.
9. Изменю текст программы, создам исполняемый файл и проверю его работу:
[рис.9](image/9.jpg){ #fig:009 width=90% }
10. Создам файл variant.asm, изучу текст программы из листинга 7.4 и введу в файл variant.asm. Создам исполняемый файл и запущу:
[рис.10](image/10.jpg){ #fig:010 width=90% }
Строки 24 и 25 отвечают за вывод на экран сообщения ‘Ваш вариант:’. Инстуркции nasm mov ecx, x mov edx, 80 call sread используются для объявления неизвестной переменной (переменной для ввода)и использования условия (до 80). Инструкция “call atoi” используется для вызова неизвестной переменной (переменной для ввода). Строки 13-17 листинга 7.4 отвечают за вычисление варианта. Остаток от деления при выполнении инструкции “div ebx” записывается в регистр al. Инструкция “inc edx” используется для увеличения регистра на 1. Строки 18-28 листинга 7.4 отвечают за вывод на экран результата вычислений.
11.Выполнение самостоятельной работы 2 варианта:
Создам файл, введу программу для нужной функции, создам исполняемый файл и запущу. По условию задачи проверю работу программы на значениях 1 и 6:
[рис.11](image/11.jpg){ #fig:011 width=90% }
[рис.12](image/12.jpg){ #fig:012 width=90% }
[рис.13](image/13.jpg){ #fig:013 width=90% }
Всё работает корректно.

# Выводы

Я освоила арифметические инструкции языка ассемблер NASM.

# Список литературы{.unnumbered}

::: {#refs}
:::
