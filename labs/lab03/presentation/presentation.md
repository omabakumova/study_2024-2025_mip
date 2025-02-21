---
## Front matter
lang: ru-RU
title: Лабораторная работа 3. Моделирование стохастических процессов
author:
  - Абакумова О. М.
institute:
  - Российский университет дружбы народов, Москва, Россия


## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
mainfont: Open Sans Light
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Абакумова Олеся Максимовна
  * Студентка
  * Российский университет дружбы народов
  * 1132220832@pfur.ru
  * <https://github.com/omabakumova>

:::
::: {.column width="30%"}

![](./image/abakumova.png)

:::
::::::::::::::

# Цель работы

Приобретение навыков моделирования сетей передачи данных с помощью средства имитационного моделирования NS-2, а также анализ полученных результатов
моделирования.

# Задания 

- Реализовать модель на NS-2
- Построить график в GNUplot

# Выполнение лабораторной работы

## Реализация модели на NS-2

![Код stohast.tcl(1 часть)](image/1.png){#fig:001 width=40%}

## Реализация модели на NS-2

![Код stohast.tcl(2 часть)](image/2.png){#fig:002 width=25%}

## Реализация модели на NS-2

![Код stohast.tcl(3 часть)](image/3.png){#fig:003 width=30%}

## Реализация модели на NS-2

![Код stohast.tcl(4 часть)](image/4.png){#fig:004 width=70%}

## Реализация модели на NS-2

![Результат запуска stohast.tcl](image/5.png){#fig:005 width=70%}

## График в GNUplot

![Создание graph_plot](image/6.png){#fig:006 width=70%}

## График в GNUplot

![Листинг graph_plot](image/7.png){#fig:007 width=70%}

## График в GNUplot

![Файл стал исполняемым и мы его запустили](image/8.png){#fig:008 width=70%}

## График в GNUplot

![Результат запуска graph_plot(График поведения длины очереди)](image/9.png){#fig:009 width=65%}


# Выводы

Во время выполнения данной лабораторной работы я приобрела навыки моделирования стохастических процессов, используя NS-2 и построила график, используя в качестве инструмента GNUplot.

