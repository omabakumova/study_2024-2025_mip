---
## Front matter
title: "Упражнение на построение фигур Лиссажу с помощью xcos"
author: "Абакумова Олеся Максимовна, НФИбд-02-22"

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

Используя Scilab и xcos, построить фигуры Лиссажу по заданным параметрам.

## Теоретическое введение

Общее математическое выражение для кривой Лиссажу:

$$
\begin{cases}
  x(t) = A \cdot \sin(at + \delta) \\
  y(t) = B \cdot \sin(bt) \\
\end{cases}
$$

где A, B — амплитуды колебаний, a, b — частоты, $\delta$ — сдвиг фаз.

# Задание

1. Построить в xcos фигуры Лиссажу со следующими параметрами:
   - $A = B = 1, a = 2, b = 2, \delta = 0; \pi/4;\pi/2;3\pi/4;\pi$;
   - $A = B = 1, a = 2, b = 4, \delta = 0; \pi/4;\pi/2;3\pi/4;\pi$;
   - $A = B = 1, a = 2, b = 6, \delta = 0; \pi/4;\pi/2;3\pi/4;\pi$;
   - $A = B = 1, a = 2, b = 3, \delta = 0; \pi/4;\pi/2;3\pi/4;\pi$;



# Выполнение лабораторной работы
## Упражнение.

Для построения последующих фигур построим модель вида (рис. [-@fig:001]):

![Модель для построения различных фигур Лиссажу](image/1.png){#fig:001 width=70%}

Для начала построим фигуры со следующими параметрами:

1. $A = B = 1, a = 2, b = 2, \delta = 0$ (рис. [-@fig:002]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 2, \delta = 0$ ](image/2.png){#fig:002 width=70%}

2. $A = B = 1, a = 2, b = 2, \delta = \pi/4$ (рис. [-@fig:003]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 2, \delta = \pi/4$ ](image/3.png){#fig:003 width=70%}

3. $A = B = 1, a = 2, b = 2, \delta = \pi/2$ (рис. [-@fig:004]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 2, \delta = \pi/2$ ](image/4.png){#fig:004 width=70%}

4. $A = B = 1, a = 2, b = 2, \delta = 3\pi/4$ (рис. [-@fig:005]):


![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 2, \delta = 3\pi/4$ ](image/5.png){#fig:005 width=70%}

4. $A = B = 1, a = 2, b = 2, \delta = \pi$ (рис. [-@fig:006]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 2, \delta = \pi$ ](image/6.png){#fig:006 width=70%}

Аналогичным образом построим фигуры Лиссажу с другими параметрами,в данном случае у нас будут различны друг от друга параметры частот:

1. $A = B = 1, a = 2, b = 4, \delta = 0$ (рис. [-@fig:007]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 4, \delta = 0$ ](image/7.png){#fig:007 width=70%}

2. $A = B = 1, a = 2, b = 4, \delta = \pi/4$ (рис. [-@fig:008]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 4, \delta = \pi/4$ ](image/8.png){#fig:008 width=70%}

3. $A = B = 1, a = 2, b = 4, \delta = \pi/2$ (рис. [-@fig:009]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 4, \delta = \pi/2$ ](image/9.png){#fig:009 width=70%}

4. $A = B = 1, a = 2, b = 2, \delta = 3\pi/4$ (рис. [-@fig:010]):


![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 4, \delta = 3\pi/4$ ](image/10.png){#fig:010 width=70%}

4. $A = B = 1, a = 2, b = 4, \delta = \pi$ (рис. [-@fig:011]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 4, \delta = \pi$ ](image/11.png){#fig:011 width=70%}

Далее рассмотрим фигуры со следующим параметром частоты:

1. $A = B = 1, a = 2, b = 6, \delta = 0$ (рис. [-@fig:012]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 6, \delta = 0$ ](image/12.png){#fig:012 width=70%}

2. $A = B = 1, a = 2, b = 6, \delta = \pi/4$ (рис. [-@fig:013]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 6, \delta = \pi/4$ ](image/13.png){#fig:013 width=70%}

3. $A = B = 1, a = 2, b = 6, \delta = \pi/2$ (рис. [-@fig:014]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 6, \delta = \pi/2$ ](image/14.png){#fig:014 width=70%}

4. $A = B = 1, a = 2, b = 6, \delta = 3\pi/4$ (рис. [-@fig:015]):


![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 6, \delta = 3\pi/4$ ](image/15.png){#fig:015 width=70%}

4. $A = B = 1, a = 2, b = 6, \delta = \pi$ (рис. [-@fig:016]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 6, \delta = \pi$ ](image/16.png){#fig:016 width=70%}

В последнем пункте задания также поменяем только частоту на уже нечетное значение и посмотрим какие фигуры мы получим:

1. $A = B = 1, a = 2, b = 3, \delta = 0$ (рис. [-@fig:017]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 3, \delta = 0$ ](image/17.png){#fig:017 width=70%}

2. $A = B = 1, a = 2, b = 3, \delta = \pi/4$ (рис. [-@fig:018]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 3, \delta = \pi/4$ ](image/18.png){#fig:018 width=70%}

3. $A = B = 1, a = 2, b = 3, \delta = \pi/2$ (рис. [-@fig:019]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 3, \delta = \pi/2$ ](image/19.png){#fig:019 width=70%}

4. $A = B = 1, a = 2, b = 3, \delta = 3\pi/4$ (рис. [-@fig:020]):


![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 3, \delta = 3\pi/4$ ](image/20.png){#fig:020 width=70%}

4. $A = B = 1, a = 2, b = 3, \delta = \pi$ (рис. [-@fig:021]):

![Фигура Лиссажу с параметрами $A = B = 1, a = 2, b = 3, \delta = \pi$ ](image/21.png){#fig:021 width=70%}


# Выводы

Во время выполнения данной лабораторной работы я применила, приобретенные навыки работы с Scilab и подсистемой xcos, и реализовала ряд фигур Лиссажу по заданным параметрам.

