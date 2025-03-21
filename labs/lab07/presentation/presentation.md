---
## Front matter
lang: ru-RU
title: Лабораторная работа 7. Модель $M |M |1|∞$
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
 - '\makeatletter'
 - '\makeatother'
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

Используя xcos, реализовать модель  $M |M |1|∞$.

# Задания 

1. Реализовать модель $M |M |1|∞$ в xcos с использованием суперблоков.

# Выполнение лабораторной работы

## Реализация модели в xcos

![Установка контекста](image/1.png){#fig:001 width=50%}

## Реализация модели в xcos

![Суперблок, моделирующий поступление заявок](image/2.png){#fig:002 width=50%}

## Реализация модели в xcos

![Суперблок, моделирующий обработку заявок](image/3.png){#fig:003 width=50%}

## Реализация модели в xcos

![Модель $M |M |1|∞$ в xcos](image/4.png){#fig:004 width=50%}

## Реализация модели в xcos

![Поступление ( — ) и обработка (– · · – ) заявок](image/5.png){#fig:005 width=85%}

## Реализация модели в xcos

![Динамика размера очереди](image/6.png){#fig:006 width=85%}

# Выводы

Во время выполнения данной лабораторной работы я реализовала модель $M |M |1|∞$ в xcos с использованием суперблоков.
