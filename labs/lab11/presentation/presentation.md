---
## Front matter
lang: ru-RU
title: Лабораторная работа 11. Модель системы массового обслуживания M |M |1
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

# Задание

1. Построить модель задачи cистемы массового ослуживания $M|M|1$

2. Построить график

# Теоретическое введение

 В систему поступает поток заявок двух типов, распределённый по пуассоновскому
закону. Заявки поступают в очередь сервера на обработку. Дисциплина очереди -
FIFO. Если сервер находится в режиме ожидания (нет заявок на сервере), то заявка
поступает на обработку сервером.


# Выполнение лабораторной работы
## Построение модели с помощью CPNTools

![Граф сети системы обработки заявок в очереди](image/1.png){#fig:001 width=70%}

## Построение модели с помощью CPNTools

![Граф генератора заявок системы](image/2.png){#fig:002 width=70%}

## Построение модели с помощью CPNTools

![Граф процесса обработки заявок на сервере системы](image/3.png){#fig:003 width=70%}

## Построение модели с помощью CPNTools

![Задание деклараций системы](image/4.png){#fig:004 width=25%}

## Построение модели с помощью CPNTools

![Параметры элементов основного графа системы обработки заявок в очереди](image/5.png){#fig:005 width=70%}

## Построение модели с помощью CPNTools


![Параметры элементов генератора заявок системы](image/6.png){#fig:006 width=70%}

## Построение модели с помощью CPNTools

![Параметры элементов обработчика заявок системы](image/7.png){#fig:007 width=70%}

## Мониторинг параметров моделируемой системы

![Функция Predicate монитора Ostanovka](image/8.png){#fig:008 width=45%}

## Мониторинг параметров моделируемой системы

![Функция Observer монитора Queue Delay](image/9.png){#fig:009 width=45%}

## Мониторинг параметров моделируемой системы

![Файл Queue_Delay.log](image/10.png){#fig:010 width=70%}

## Мониторинг параметров моделируемой системы

![Содержание Queue_Delay.log](image/11.png){#fig:011 width=30%}

## Мониторинг параметров моделируемой системы

```
#!/usr/bin/gnuplot -persist

set encoding utf8
set term pngcairo font "Helvetica,9"

# задаём выходной файл графика
set out 'window_1.png'
plot "Queue_Delay.log" using ($4):($1) with lines
```

## Мониторинг параметров моделируемой системы

![График изменения задержки в очереди](image/12.png){#fig:012 width=70%}

## Мониторинг параметров моделируемой системы

![Функция Observer монитора Queue Delay Real](image/13.png){#fig:013 width=70%}

## Мониторинг параметров моделируемой системы

![Содержимое Queue_Delay_Real.log](image/14.png){#fig:014 width=70%}

## Мониторинг параметров моделируемой системы

![Функция Observer монитора Long Delay Time](image/15.png){#fig:015 width=70%}

## Мониторинг параметров моделируемой системы

![Определение longdelaytime в декларациях](image/16.png){#fig:016 width=70%}

## Мониторинг параметров моделируемой системы

![Содержимое Long_Delay_Time.log](image/17.png){#fig:017 width=70%}

## Мониторинг параметров моделируемой системы


```
#!/usr/bin/gnuplot -persist

set encoding utf8
set term pngcairo font "Helvetica,9"

# задаём выходной файл графика
set out 'window_1.png'
set style line 2
plot [0:] [0:1.2] "Long_Delay_Time.log" using ($4):($1) with lines
```

## Мониторинг параметров моделируемой системы

![Периоды времени, когда значения задержки в очереди превышали заданное значение](image/18.png){#fig:018 width=70%}



# Выводы

В процессе выполнения данной лабораторной работы я реализовала модель
системы массового обслуживания $M|M|1$ в CPN Tools.
