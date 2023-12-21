---
## Front matter
title: "Архитектура компьютера"
subtitle: "Лаюораторная работа 7"
author: "Буценко Варвара Алексеевна"

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

Изучение команд условного и безусловного переходов. Приобретение навыков написания программ с использованием переходов. Знакомство с назначением и структурой файла листинга.

# Задание

Здесь приводится описание задания в соответствии с рекомендациями
методического пособия и выданным вариантом.

# Теоретическое введение

                                                  |

Более подробно об Unix см. в [@gnu-doc:bash;@newham:2005:bash;@zarrelli:2017:bash;@robbins:2013:bash;@tannenbaum:arch-pc:ru;@tannenbaum:modern-os:ru].

# Выполнение лабораторной работы

Создала каталог для программам лабораторной работы No 7, перешла в него и создала файл lab7-1.asm. Ввела в файл lab7-1.asm текст программы из листинга 7.1. (рис. @fig:001).

![1](image/1.png){#fig:001 width=70%}

Изменила текст программы, создала файл и проверила его работу. (рис. @fig:002).

![2](image/2.png){#fig:002 width=70%}

Создала файл lab7-2.asm в каталоге ~/work/arch-pc/lab07. Ввела текст программы в lab7-2.asm (рис. @fig:003).

![3](image/3.png){#fig:003 width=70%}

Создала файл листинга для программы из файла lab7-2.asm
Открыла файл листинга lab7-2.lst с помощью текстового редактора.
mcedit lab7-2.lst

(рис. @fig:004).

В начале в регистр ecx записывается значение регистра eax (4). В регистр eax записывается символ 4, в регистр ebx 1. 

![4](image/5.png){#fig:004 width=70%}

Открыла файл с программой lab7-2.asm и удалить один операнд. Выполнила трансляцию с получением файла листинга. (рис. @fig:005).

![5](image/4.png){#fig:005 width=70%}

# Выводы

Изучила команды условного и безусловного перехода, приобрела навыки написания программы с использованием переходов. Познакомилась с назначением и структурой файла листинга.

# Список литературы{.unnumbered}

::: {#refs}
:::
