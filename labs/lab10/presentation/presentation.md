---
## Front matter
lang: ru-RU
title: "Презентация к лабораторной работе 10"
subtitle: Программирование в командном процессоре ОС UNIX. Командные файлы
author:
  - Сидорова Н.А.
institute:
  - Российский университет дружбы народов, Москва, Россия
  - Объединённый институт ядерных исследований, Дубна, Россия
date: 13 апреля 2023

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
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

## Цель работы

Изучить основы программирования в оболочке ОС UNIX/Linux. Научиться писать
небольшие командные файлы.

## Скрипт1
Написать скрипт, который при запуске будет делать резервную копию самого себя (то есть файла, в котором содержится его исходный код) в другую директорию backup в вашем домашнем каталоге. При этом файл должен архивироваться одним из архиваторов на выбор zip, bzip2 или tar.

![скрипт 1](image/fig:001.jpg){#fig:001 width=70%}

## Скрипт1 работа 

![Работа скрипта 1](image/fig:002.jpg){#fig:002 width=70%}

## Скрипт2
Написать пример командного файла, обрабатывающего любое произвольное число аргументов командной строки, в том числе превышающее десять. Например, скрипт может последовательно распечатывать значения всех переданных аргументов. 

![скрипт 2](image/fig:003.jpg){#fig:003 width=70%}

## Скрипт2 работа 

![Работа скрипта 2](image/fig:004.jpg){#fig:004 width=70%}

## Скрипт3
Написать командный файл — аналог команды ls (без использования самой этой команды и команды dir). Требуется, чтобы он выдавал информацию о нужном каталоге и выводил информацию о возможностях доступа к файлам этого каталога. 

![скрипт 3](image/fig:005.jpg){#fig:005 width=70%}

## Скрипт3 работа 

![Работа скрипта 3](image/fig:006.jpg){#fig:006 width=70%}

## Скрипт4
Написать командный файл, который получает в качестве аргумента командной строки формат файла (.txt, .doc, .jpg, .pdf и т.д.) и вычисляет количество таких файлов в указанной директории. Путь к директории также передаётся в виде аргумента командной строки. 

![скрипт 4](image/fig:007.jpg){#fig:007 width=70%}

## Скрипт4 работа 

![Работа скрипта ](image/fig:008.jpg){#fig:008 width=70%}

##Выводы

В ходе выполнения лабораторной работы я изучила основы программирования в оболочке ОС UNIX/Linux. Научилась писать небольшие командные файлы.
