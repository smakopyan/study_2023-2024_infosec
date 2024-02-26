---
## Front matter
title: "индивидуальный проект"
subtitle: "1 этап"
author: "Акопян Сатеник Манвеловна"

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
monofont: PT Sans
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

Целью данной лабораторной работы является установка Kali Linux


# Выполнение лабораторной работы

1. Устанавливаем образ операционной системы

![рисунок 1](image/1.jpg){#fig:001 width=70%}

2. Следует создать новую виртуальную машину. Для этого в VirtualBox выбираем: машина -> создать. Указываем имя виртуальной машины тип операционной системы, а также размер оперативной памяти, конфигурацию жесткого диска и его размер.

![рисунок 2](image/2.jpg){#fig:002 width=70%}

![рисунок 3](image/3.jpg){#fig:003 width=70%}

![рисунок 4](image/4.jpg){#fig:004 width=70%}

![рисунок 5](image/5.jpg){#fig:005 width=70%}

3. Выбираем 1 пункт установки

![рисунок 6](image/6.jpg){#fig:006 width=70%}

4. Выбираем локацию и язык, а также способ переключения клавиатуры

![рисунок 7](image/7.jpg){#fig:007 width=70%}

![рисунок 8](image/8.jpg){#fig:008 width=70%} 

![рисунок 9](image/9.jpg){#fig:009 width=70%}

![рисунок 10](image/10.jpg){#fig:010 width=70%}

5. Вводим имя хоста и пользователя, а также пароль

![рисунок 11](image/13.jpg){#fig:011 width=70%}

![рисунок 12](image/15.jpg){#fig:012 width=70%}

![рисунок 13](image/16.jpg){#fig:013 width=70%}

6. Выбираем нужный часовой пояс

![рисунок 14](image/17.jpg){#fig:014 width=70%}

7. Делаем последние настройки и перезапускаем систему

![рисунок 15](image/18.jpg){#fig:015 width=70%}

![рисунок 16](image/19.jpg){#fig:016 width=70%}

![рисунок 17](image/20.jpg){#fig:017 width=70%}

![рисунок 18](image/21.jpg){#fig:018 width=70%}

![рисунок 19](image/22.jpg){#fig:019 width=70%}

![рисунок 20](image/23.jpg){#fig:020 width=70%}

8. Заходим в систему под заданным именем пользователя и паролем

![рисунок 21](image/24.jpg){#fig:021 width=70%}

![рисунок 22](image/25.jpg){#fig:022 width=70%}

# Выводы

В результате данной лабораторной работы я установила Kali Linux

# Список литературы{.unnumbered}

::: {#refs}
:::
