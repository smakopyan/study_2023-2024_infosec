---
## Front matter
title: "Лабораторная работа № 2"
subtitle: "Дискреционное
разграничение прав в Linux. Основные
атрибуты"
author: "Акопян Сатеник"

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

Получение практических навыков работы в консоли с атрибутами фай-
лов, закрепление теоретических основ дискреционного разграничения до-
ступа в современных системах с открытым кодом на базе ОС Linux1

# Выполнение лабораторной работы

1. В установленной при выполнении предыдущей лабораторной работы
операционной системе создайте учётную запись пользователя guest (ис-
пользую учётную запись администратора). Задайте пароль для пользователя guest (использую учётную запись администратора):

![рисунок 1](image/1.jpg){#fig:001 width=70%}

2. Войдите в систему от имени пользователя guest (команда su). Определите директорию, в которой вы находитесь, командой pwd. 

![рисунок 2](image/3.jpg){#fig:002 width=70%}

3. Уточните имя вашего пользователя командой whoami

![рисунок 3](image/4.jpg){#fig:003 width=70%}

4. Уточните имя вашего пользователя, его группу, а также группы, куда входит пользователь, командой id. Выведенные значения uid, gid и др. запомните. Сравните вывод id с выводом команды groups.

![рисунок 4](image/5.jpg){#fig:004 width=70%}

5. Просмотрите файл /etc/passwd командой cat /etc/passwd

![рисунок 5](image/6.jpg){#fig:005 width=70%}

![рисунок 6](image/7.jpg){#fig:006 width=70%}

6. Определите существующие в системе директории командой
ls -l /home/
Удалось ли вам получить список поддиректорий директории /home?(да) Ка-
кие права установлены на директориях? (Создание файла, Удаление файла, запись в файл, чтение файла, смена директории, просмотр файлов в директории, переименование файла, смена атрибутов файла)

![рисунок 7](image/8.jpg){#fig:007 width=70%}

7. Проверьте, какие расширенные атрибуты установлены на поддиректориях, находящихся в директории /home, командой: lsattr /home Удалось ли вам увидеть расширенные атрибуты директории (нет)?Удалось ли вам увидеть расширенные атрибуты директорий других пользователей (нет)

![рисунок 8](image/9.jpg){#fig:008 width=70%}

8. Создайте в домашней директории поддиректорию dir1 командой mkdir dir1

![рисунок 9](image/9.jpg){#fig:009 width=70%}

9. Снимите с директории dir1 все атрибуты командой chmod 000 dir1 и проверьте с её помощью правильность выполнения команды ls -l

![рисунок 10](image/10.jpg){#fig:010 width=70%}

10. Попытайтесь создать в директории dir1 файл file1 командой
echo "test" > /home/guest/dir1/file1
Объясните, почему вы получили отказ в выполнении операции по созда-
нию файла (так как на предыдущем этапе сняли все атрибуты с директории)?
Оцените, как сообщение об ошибке отразилось на создании файла? Про-
верьте командой (файл не создался)

![рисунок 11](image/11.jpg){#fig:011 width=70%}

# Выводы
В результате данной лабораторной работы я получила практические навыки работы в консоли с атрибутами фай-
лов, закрепила теоретические основы дискреционного разграничения доступа в современных системах с открытым кодом на базе ОС Linux

# Список литературы{.unnumbered}

::: {#refs}
:::
