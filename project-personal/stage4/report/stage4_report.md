---
## Front matter
title: "Отчет по четвертому этапу индивидуального проекта"
subtitle: "Дисциплина: Основы информационной безопасности"
author: "Иванов Сергей Владимирович, НПИбд-01-23"

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

Просканировать веб-приложение используя сканер nikto.

# Задание

1. Использовать nikto

# Выполнение лабораторной работы

Для начала запустим веб приложение DVWA. Для этого необходимо запустить mysql и apache2. (рис. 1).

![Запуск DVWA](image/1.png){#fig:001 width=70%}

Захожу на сайт DVWA и перехожу во вкладку DWVA Security. Выбираю низкий уровень безопасности. (рис. 2)

![Выбор уровня безопасности](image/2.png){#fig:002 width=70%}

Запускаю сканер nikto. (рис. 3)

![Запуск nikto](image/3.png){#fig:003 width=70%}

Запускаю сканирование веб приложения вводя URL адрес. (рис. 4)

![Сканирование](image/4.png){#fig:004 width=70%}

Запускаю сканирование вводя номер порта и адрес порта. (рис. 5)

![Сканирование](image/5.png){#fig:005 width=70%}

# Выводы

Получены практические навыки по использованию nikto для сканирования веб приложений.
