---
## Front matter
title: "Архитектура компьютера"
subtitle: "Лабораторная работа №6"
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

Освоение арифметических инструкций языка ассемблера NASM.

# Задание

Здесь приводится описание задания в соответствии с рекомендациями
методического пособия и выданным вариантом.

# Теоретическое введение                                                                    |

Более подробно об Unix см. в [@gnu-doc:bash;@newham:2005:bash;@zarrelli:2017:bash;@robbins:2013:bash;@tannenbaum:arch-pc:ru;@tannenbaum:modern-os:ru].

# Выполнение лабораторной работы

Создала каталог для программам лабораторной работы No 6, перешла в него и создала файл lab6-1.asm Ввела в файл lab6-1.asm текст программы из листинга 6.1. Создала иполняемый файл и запустила его (вывелось j). Далее замнила текст программы, вывелся дополнительный пробел. (рис. @fig:001).

![1](image/1.png){#fig:001 width=70%}

Создайла файл lab6-2.asm в каталоге ~/work/arch-pc/lab06 и ввела в него текст программы из листинга 6.2. Создала файл и запустила его, результат 106. Затем заменила строки, в результате вывелось 10. 

printLF и iprint по разному вывели ответ. С переносом и без. (рис. @fig:002).

![2](image/3.png){#fig:002 width=70%}

Создала файл lab6-3.asm в каталоге ~/work/arch-pc/lab06:
Ввела текст программы в lab6-3.asm. Создала исполняемый файл и запустила его. Результат остаток от деления 1 и результат 4. Поменяла текст программы, результат 5. (рис. @fig:003).

![3](image/4.png){#fig:003 width=70%}

Создала файл variant.asm в каталоге ~/work/arch-pc/lab06:
Ввела текст программы в файл variant.asm.
Создайте исполняемый файл и запустите его. Результат 8. (рис. @fig:004).

![4](image/5.png){#fig:003 width=70%}

1. Какие строки листинга 6.4 отвечают за вывод на экран сообщения ‘Ваш вариант:’?

mov eax,rem
call sprint

2. Для чего используется следующие инструкции?
mov ecx, x
mov edx, 80
call sread

Записывает значение в регистры и вызывает sread.

3. Для чего используется инструкция “call atoi”?

ASCII кода в число, `eax=x`

4. Какие строки листинга 6.4 отвечают за вычисления варианта?

or edx,edx
mov ebx,20
div ebx
inc edx

5. В какой регистр записывается остаток от деления при выполнении инструкции “div
ebx”?

exb 

6. Для чего используется инструкция “inc edx”?

Уменьшает значение регистра ax на 1

7. Какие строки листинга 6.4 отвечают за вывод на экран результата вычислений?

mov eax,rem
call sprint
mov eax,edx
call iprintLF
call quit

# Выводы

Освоила арифметические функции языка ассемблера NASM.

# Список литературы{.unnumbered}

::: {#refs}
:::
