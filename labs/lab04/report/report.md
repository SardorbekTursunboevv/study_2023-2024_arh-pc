---
## Front matter
title: "Лабораторная работа №4"
subtitle: "Создание и процесс обработки программ на языке ассемблера NASM"
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

Цель данной лабораторной работы -- базовая ознакомление с языком NASM, а также освоить процедуры компиляции и сборки программ написаных на этом языке.

# Задание

1. Создание программы Hello world на языке NASM
2. Работа с транслятором NASM
3. Работа с компоновщиком LD
4. Запуск исполняемого файла
5. Задания для самостоятельной работы

# Выполнение лабораторной работы

Cоздам в рабочем каталоге work подкаталог в котором будет выполняться лабораторная работа(Рис.1).

![Рис. 1 Создание нового подкаталога](image/lab01.png)

Перейду в созданный нами подкаталог(Рис.2).

![Рис. 2 Переход в созданный подкаталог](image/lab02.png)

создам файл hello.asm утилитой touch(Рис.3).

![Рис. 3 Создание файла hello.asm](image/lab03.png)

Редактировать файл буду в текстовом редакторе gedit(Рис.4).

![Рис. 4 Открою файл hello.asm в текстовом редакторе gedit](image/lab04.png)

Вставлю пример кода из лабораторной работы в текстовый редактор(Рис.5).

![Рис. 5 Пример кода в текстовом редакторе](image/lab05.png)

Переведу текст программы hello.asm в объектный код с помощью транслятора(Рис.6).

![Рис. 6 Работа транслятора](image/lab06.png)

Введу команду которая скомпилирует файл hello.asm в файл obj.o, так же использую ключом -g и с помощью ключа -l создам файл листинга list.lst(Рис.7).

![Рис.7 Компиляция программы с расширенным синтаксисом](image/lab07.png)

Передаю файл hello.o компоновщику ld, задам имя создаваемого файла с помощью ключа -o(Рис.8).

![Рис. 8 Работа компоновщика ld](image/lab08.png)

Передаю файл obj.o компоновщику. Файл будет иметь имя main, так как оно было указано после ключа -o(Рис.9).

![Рис.9 Передача файла obj.o компоновщику и проверка его работы](image/lab09.png)

Запущу сделанную нами программу hello(Рис.10).

![Рис. 10 Запуск программы hello](image/lab10.png)

Утилитой cp создам копию hello.asm и назовём её lab4.asm. Проверим правильность копирования утилитой ls(Рис.11).

![Рис. 11 Копирование файла hello.asm](image/lab11.png)

Открою файл lab4.asm в текстовом редакторе gedit(Рис.12).

![Рис.12 Oткрытие файла lab4.asm](image/lab12.png)

Вношу изменения в код так, чтобы программа lab4.asm выводила мои имя и фамилию(Рис.13).

![Рис.13 Код с внесёнными изменениями](image/lab13.png)

Скомпилирую получившийся код в объектный файл lab4.o(Рис.14).

![Рис.14 Компиляция программы lab4.asm](image/lab14.png)

Отправлю объектный код компоновщику для создания файла lab(Рис.15).

![Рис.15 Создание файла lab](image/lab15.png)

Запущу для проверки программу lab(Рис.16).

![Рис.16 Результат работы программы lab](image/lab16.png)

Скопирую программы созданные в ходе этой лабораторной работы в рабочий каталог(Рис.17).

![Рис. 17 Использование утилиты cp для копирования программ в рабочий каталог](image/lab17.png)

# Выводы

В ходе данной лабораторной работы я познакомился с языком NASM и научился работать с компилятором и компоновщиком

