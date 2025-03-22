---
## Front matter
title: "Отчёт по лабораторной работе"
subtitle: "Лабораторная №3 по математическом моделированию"
author: "Дзахмишев Камбулат Заурович"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Между страной Х и страной У идет война. Численность состава войск
исчисляется от начала войны, и являются временными функциями( )x t и( )y t . В
начальный момент времени страна Х имеет армию численностью 32 888 человек, а
в распоряжении страны У армия численностью в 17 777 человек. Для упрощения
модели считаем, что коэффициенты, , ,a b c h постоянны. Также считаем( )P t и( )Q t
непрерывные функции.

# Цель работы

Постройте графики изменения численности войск армии Х и армии У для
следующих случаев:
1. Модель боевых действий между регулярными войсками: dx/dy = 0,55x(t) - 0,77y(t) + 1,5sin(3t + 1);
dy/dt = 0,66x(t) - 0,44y(t) + 1,2cos(t + 1)

2. Модель ведение боевых действий с участием регулярных войск и
партизанских отрядов: dx/dt = -0,27x(t) - 0,88y(t) + sin(20t);
dy/dt = -0,68x(t)y(t) - 0,37y(t) + cos(10t) + 1

# Выполнение лабораторной работы

![Часть кода по первому случаю.](/home/kambulat/work/study/2024-2025/Математическое моделирование/mathmod/labs/lab3/1/1.png){#fig:001 width=70%}

# Выполнение лабораторной работы

![Часть кода по второму случаю.](/home/kambulat/work/study/2024-2025/Математическое моделирование/mathmod/labs/lab3/1/2.png){#fig:002 width=70%}

# Выполнение лабораторной работы

![Первый график (модель боевых действий между регулярными войсками).](/home/kambulat/work/study/2024-2025/Математическое моделирование/mathmod/labs/lab3/1/3.png){#fig:003 width=70%}

# Выполнение лабораторной работы

![Второй график (модель боевых действий с участием регулярных войск и партизанских отрядов).](/home/kambulat/work/study/2024-2025/Математическое моделирование/mathmod/labs/lab3/1/4.png){#fig:004 width=70%}

# Вывод

В ходе данной лабораторной работы построил модель ведения боевых действий и увидел, что с начального момента времени численномть армии У начала убывать по мере увеличения численности армии Х для первого случая. Во втором случае почему-то сразу видно резкое уменьшение численности войск армии У.

# Список литературы{.unnumbered}

::: {#refs}
:::
