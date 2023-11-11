---
## Front matter
title: "Лабораторная работа №6"
subtitle: "Основы работы c Midnight Commander. Структура программ на языке ассемблера NASM. Системные вызовы в OC GNU Linux"
author: "Турсунбоев Сардорбек"

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

Целью данной лабораторной работы является приобретение навыков работы с программой Midnight Commander и освоение инструкций mov и int в языке ассемблера NASM.

# Задание

1. Основы работы в Midnight Commander
2. Структура программ на языке ассемблера NASM
3. Использование внешних файлов в языке ассемблера NASM
4. 

# Выполнение лабораторной работы

Открою Midnight Commander через терминал командой mc(Рис.1).

![Открытие Midnight Commander через терминал](image/lab1.png)

Перейду в созданный мной в ходе лабораторной работы №4 каталог arch-pc(Рис.2).

![Переход в каталог arch-pc](image/lab2.png)

В Midnight Commander создам новый каталог lab05(Рис.3). 

![Создание каталога в Midnight Commander](image/lab3.png)

Перейду в созданный мной каталог(Рис.4).

![Переход в созданный нами каталог](image/lab4.png)

Утилитой touch создам файл lab5-1.asm(Рис.5).

![Создание файла lab5-1.asm](image/lab5.png)

Убеждаюсь что файл действительно создан(Рис.6).

![Проверка правильности создания файла](image/lab6.png)

Открою файл lab5-1.asm во встроенный редакторе mcedit(Рис.7).

![Открытие файла в редакторе mcedit](image/lab7.png)

Напишу код по образцу(Рис.8).

![Код, написанный по образцу](image/lab8.png)

В Midnight Commander открою файл для просмотра и удостоверюсь что правильно написали код(Рис.9).

![Файл, открытый для просмотра](image/lab9.png)

Оттранслирую и отправлю на компоновку lab5-1.asm, затем запущу полученный файл для проверки его работоспособности(Рис.10).

![Трансляция, компоновка и запуск lab5-1.asm](image/lab10.png)

Скопирую файл lab5-1.asm в этот же каталог и назову его lab5-2.asm(Рис.11).

![Копирование файла в Midnight Commander](image/lab11.png)

Убеждаюсь в правильности копирования файла(Рис.12).

![Файл lab5-2.asm в рабочем каталоге](image/lab12.png)

По образцу напишу код, включу в него внешний файл in_out.asm и использую доступныe подпрограммами(Рис.13).

![Код, написанный по образцу с использованием подпрограмм из внешнего файла in_out.asm](image/lab13.png)

Оттранслирую, отправлю на компоновку и запущу получившийся файл(Рис.14).

![Работа файла lab5-2.asm](image/lab14.png)

Заменим в файле lab5-2.asm подпрограмму sprintLF на sprint(Рис.15).

![Замена подпрограммы sprintLF на sprint](image/lab15.png)

Проверю результат и замечу, что результат отличается. Это вызвано тем, что sprintLF переводит строку, а sprint нет(Рис.16).

![Результат работы lab5-2.asm после замены sprintLF на sprint](image/lab16.png)

Скопирую файл lab5-1.asm и напишу там код для написания строки, запроса ввода от пользователя и вывода введёной строки на экран, без использования подпрограмм(Рис.17).

![Код в файле lab5-1.asm](image/lab17.png)

Проверю его работоспособность(Рис.18).

![Проверка работоспособности кода](image/lab18.png)

Скопирую файл lab5-2.asm и напишу там код для написания строки, запроса ввода от пользователя и вывода введёной строки на экран, в этот раз пользуясь подпрограммами из in_out.asm(Рис.19)

![Написанный в lab5-2.asm код](image/lab19.png)

Проверю работоспособность  кода(Рис.20).

![Проверка работоспособности lab5-2.asm](image/lab20.png)

# Выводы

Я научился работать с программой Midnight Commander
