---
## Front matter
title: "Лаюораторная работа 5"
subtitle: "Архитектура компьютера 5"
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

Приобретение практических навыков работы в Midnight Commander. Освоение инструкций
языка ассемблера mov и int.

# Задание

Здесь приводится описание задания в соответствии с рекомендациями
методического пособия и выданным вариантом.

# Теоретическое введение

См. теорию в лабораторной 5.

# Выполнение лабораторной работы

Открыла Midnight Commander. Пользуясь стрелочками и enter перешла в каталог ~/work/arch-pc и создала папку lab5. Пользуясь строкой ввода и командой touch создайте файл lab5-1.asm (рис. @fig:001).

![1](image/30-11-2023.png){#fig:001 width=70%}

С помощью клавиши f4 открыла файл lab5-1.asm и ввела текст програмы из листинга 5.1. Убедилась, что файл содержит текст программы. (рис. @fig:002).

![2](image/2-30-11-2023.png){#fig:002 width=70%}

Программа вывела "введите строчку", ввела свои ФИО. (рис. @fig:003).

![2](image/3-30-11-2023.png){#fig:003 width=70%}

Скачала файл со страницы курса, файл лежит в том же каталоге, что и файл с программой, в которой он используется. Заменила текст программы и создала файл. (рис. @fig:004).

![2](image/33.png){#fig:004 width=70%}


# Выводы

Смогла приобрети практические навыки работы в Midnight Commander и освоила инструкции языка ассемблера nov и int

# Список литературы{.unnumbered}

::: {#refs}
:::
