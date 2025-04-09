---
## Front matter
title: "Отчет по лабораторной работе №9 "
subtitle: "Дисциплина архитектура компьютера"
author: "Ахатов Эмиль Эрнстович"

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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Освоение основных возможностей командной оболочки Midnight Commander. Приоб-
ретение навыков практической работы по просмотру каталогов и файлов; манипуляций
с ними.



# Выполнение лабораторной работы

Сначала скачиваю через консольную команду mc и после создаю файл для будущей работы

![скачивание](image/1.png){ #fig:001 width=70% }

открыл файл в редакторе

![открытие](image/2.png){ #fig:002 width=70% }

Вставил рандомный текст

![вставка текста](image/3.png){ #fig:003 width=70% }

Удаление строки:

Ctrl + Y — удалить текущую строку.

![удаление](image/4.png){ #fig:004 width=70% }

Выделение:

Ctrl + \ → стрелками выделите текст → Enter.

Копирование:

F5 → Enter.

![копирование](image/5.png){ #fig:005 width=70% }

Сохранение:

F2.

![сохранение](image/6.png){ #fig:006 width=70% }

Отмена действия:

Ctrl + U.

![отмена](image/7.png){ #fig:007 width=70% }

. Переход в конец файла + текст:

Ctrl + End

![переход](image/8.png){ #fig:008 width=70% }

Переход в начало файла + текст:

Ctrl + Home

![текст](image/9.png){ #fig:009 width=70% }

Сохранение и выход:

F2 → F10

![выход](image/10.png){ #fig:010 width=70% }



# Выводы

Работа позволяет приобрести практические навыки редактирования файлов в mc, что полезно при администрировании серверов и работе в Linux без графической оболочки
