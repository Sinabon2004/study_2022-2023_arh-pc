---
## Front matter
title: "Отчёт по лабораторной работе №4"
subtitle: "Язык разметки Markdown"
author: "Чесноков Артемий Павлович НПИбд-02-22"

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



# Выполнение лабораторной работы

Установили программы pandoc и TexLive по указаниям в лабораторной работе. 

1. Открываем терминал

2. Переходим в каталог курса сформированный при выполнении лабораторной работы №3:
Обновим локальный репозиторий, скачав изменения из удаленного репозитория.

3. Перейдём в каталог с шаблоном отчета по лабораторной работе № 4

4. Проведем компиляцию шаблона с использованием Makefile. 
Для этого введём команду make.
При успешной компиляции должны сгенерироваться файлы report.pdf и
report.docx. Откроем и проверим корректность полученных файлов. (рис. [-@fig:001], [-@fig:002], [-@fig:003])

![Команда компиляции](image/01.png){ #fig:001 width=70%, height=70% }

![Файл отчета в docx](image/02.png){ #fig:002 width=70%, height=70% }

![Файл отчета в pdf](image/03.png){ #fig:003 width=70%, height=70% }


5. Удалим полученные файлы с использованием Makefile. Для этого введем команду make clean
Проверим, что после этой команды файлы report.pdf и report.docx были удалены. (рис. [-@fig:004])

![Удалены файлы шаблона](image/04.png){ #fig:004 width=70%, height=70% }

6. Теперь откроем файл report.md c помощью любого текстового редактора, например gedit
 (рис. [-@fig:005])

![Структура шаблона](image/05.png){ #fig:005 width=70%, height=70% }

7. Заполняем и компилируем  отчет с использованием Makefile. 
Проверяем корректность полученных файлов. (рис. [-@fig:006])
(Обращаем внимание, что для корректного отображения скриншотов они должны быть размещены в каталоге image)

![Заполняем шаблон](image/06.png){ #fig:006 width=70%, height=70% }

8. Выгружаем файлы файлы на Github.

# Выводы

Изучили как работать с языком разметки Markdown и как создавать отчёт из шаблона.

