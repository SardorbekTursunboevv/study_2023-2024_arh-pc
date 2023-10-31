---
## Front matter
title: "лабораторная работа №3 "
subtitle: "Простейший вариант"
author: "Турсунбоев Сардорбек Кахрамон Угли"

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
mainfont: PT Sans
romanfont: PT Sans
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
  - \usepackage{caption}
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Целью данной Лабораторной работы является освоение процедур оформление отчетов с помощью легковесного языкаразметки Мarkdown.

# Задание

1.Установка необходимого ПО
2.Заполнеие отчета по лабораторной работе №4 с помощью языковой разметки Markdown
3.Задание на самостаятельная работу 


# Выполнение лабораторной работы  
Открываю терминал .Перехожу в каталог курса , сформированный при выполнении последней лабораторной работы
 

![Рисунок 1 переход в католог курса](image/Lab1.png) 

Обновляю локалный репозиторий ,скачивая изменения из удаленного репозиторя с помощью команды git pull
![Рисунок 2 команда git pull] (image/lab2.png)
Перехожу в каталог с шаблоном отчета по лабораторной работе №4 с помощью компакт-диска 
![Рисунок 3 переход в католог] (image/lab3.png) 
Компилирую шаблон с использованием Мakefile , вводя команду make
![Рисунок 4 ] (image/lab4.png) 
Удаляю полученные файлы с помощью Makefile ,  вводя команду make clean с помощью ls проверяю удалилисьли созданные файлы 
![Рисунок 5] (image/lab5.png) 
Открываю файл с помощью редактора 
![Рисунок 6] (image/lab6.png)

# Выводы

Я научился работать с Markdown

# Список литературы{.unnumbered}

::: {#refs}
:::
