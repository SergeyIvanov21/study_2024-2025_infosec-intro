---
## Front matter
title: "Отчет по третьему этапу индивидуального проекта"
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

Получить практические навыки по использованию Hydra для брутфорса паролей.

# Задание

1. Взломать логин и пароль с помощью Hydra.

# Выполнение лабораторной работы

Для брутфорса паролей необходим список частоиспользуемых паролей. Использую стандартный список rockyou.txt для Kali Linux. Распаковываю его. (рис. 1).

![Распаковка архива с паролями](image/1.png){#fig:001 width=70%}

Захожу на сайт DVWA и перехожу во вкладку Brute Force. (рис. 2)

![Сайт DVWA](image/2.png){#fig:002 width=70%}

Необходимо получить параметры cookie с сайта. Использую специальное расширение. (рис. 3)

![Получение параметров cookie](image/3.png){#fig:003 width=70%}

Далее ввожу запрос в Hydra. Подбираем пароль для пользователя admin, используем get запрос и параметры cookie. (рис. 4)

![Запрос в Hydra](image/4.png){#fig:004 width=70%}

Hedra выдала результат запроса. (рис. 5)

![Результат запроса](image/5.png){#fig:005 width=70%}

Вводим полученные логин и пароль на сайт. Видим, что авторизация выполнена успешно. (рис. 6)

![Результат](image/6.png){#fig:006 width=70%}

# Выводы

Получены практические навыки по использованию Hydra для брутфорса паролей.
