---
## Front matter
lang: ru-RU
title: Презентация к лабораторной работе 5
subtitle: Анализ файловой системы Linux. Команды для работы с файлами и каталогами
author:
  - Сидорова Н.А.
institute:
  - Российский университет дружбы народов, Москва, Россия
  - Объединённый институт ядерных исследований, Дубна, Россия
date: 05 марта 2023

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

Ознакомление с файловой системой Linux, её структурой, именами и содержанием
каталогов. Приобретение практических навыков по применению команд для работы
с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

## Теоретическое введение

Для создания текстового файла можно использовать команду touch.
Для просмотра файлов небольшого размера можно использовать команду cat.
Для просмотра файлов постранично удобнее использовать команду less.
Команда head выводит по умолчанию первые 10 строк файла.
Команда tail выводит умолчанию 10 последних строк файла.
Команда cp используется для копирования файлов и каталогов.
Команды mv и mvdir предназначены для перемещения и переименования файлов
и каталогов.

## Теоретическое введение
Каждый файл или каталог имеет права доступа.
В сведениях о файле или каталоге указываются:
– тип файла (символ (-) обозначает файл, а символ (d) — каталог);
– права для владельца файла (r — разрешено чтение, w — разрешена запись, x — разрешено выполнение, - — право доступа отсутствует);
– права для членов группы (r — разрешено чтение, w — разрешена запись, x — разрешено
выполнение, - — право доступа отсутствует);
– права для всех остальных (r — разрешено чтение, w — разрешена запись, x — разрешено
выполнение, - — право доступа отсутствует).
Права доступа к файлу или каталогу можно изменить, воспользовавшись командой
chmod. Сделать это может владелец файла (или каталога) или пользователь с правами
администратора.

## Теоретическое введение
Файловая система в Linux состоит из фалов и каталогов. Каждому физическому носителю соответствует своя файловая система.
Существует несколько типов файловых систем. Перечислим наиболее часто встречающиеся типы:
– ext2fs (second extended filesystem);
– ext2fs (third extended file system);
– ext4 (fourth extended file system);
– ReiserFS;
– xfs;
– fat (file allocation table);
– ntfs (new technology file system).
Для просмотра используемых в операционной системе файловых систем можно воспользоваться командой mount без параметров.
С помощью команды fsck можно проверить (а в ряде случаев восстановить) целостность файловой системы.

## Выполнение примеров из первой части лабораторной
С помощью команды touch создала файл file_name, затем удалила его командой rm
С помощью команды cat посмотрела содержимое файла Makefile
С помощью команды less постранично посмотрела содержимое файла Makefile
С помощью команд head и tail посмотрела начало и конец файла соответственно

## Создание файлов и директорий, их перемещение и переименование
Скопировала файл /usr/include/sys/io.h в домашний каталог и назвала его equipment
В домашнем каталоге создала директорию ~/ski.plases и переместила файл equipment в каталог ~/ski.plases
Переименовала файл ~/ski.plases/equipment в ~/ski.plases/equiplist, создала в домашнем каталоге файл abc1 и скопировала его в каталог ~/ski.plases, назвала его equiplist2, создала каталог с именем equipment в каталоге ~/ski.plases,
переместила файлы ~/ski.plases/equiplist и equiplist2 в каталог ~/ski.plases/equipment, создала и переместила каталог ~/newdir в каталог ~/ski.plases и назвала его plans

## Присваивание прав доступа файлам и директориям
пределила необходимые опции команды chmod, присвоила перечисленным ниже файлам выделенные права доступа, считая, что в начале таких прав
нет:
3.1. drwxr--r-- ... australia
3.2. drwx--x--x ... play
3.3. -r-xr--r-- ... my_os
3.4. -rw-rw-r-- ... feathers
Создала нужные файлы и директории

## Действия с файлами, каталогами и правами доступа
Просмотрела содержимое файла /etc/password
Скопировала файл ~/feathers в файл ~/file.old, переместила файл ~/file.old в каталог ~/play
Скопировала каталог ~/play в каталог ~/fun, переместила каталог ~/fun в каталог ~/play и назвала его games, лишила владельца файла ~/feathers права на чтение, попыталась просмотреть файл ~/feathers командой cat и файл не удалось посмотреть, попыталась скопировать файл ~/feathers и получилось это сделать, дала владельцу файла ~/feathers право на чтение, лишила владельца каталога ~/play права на выполнение, перешла в каталог ~/play и ничего не произошло, дала владельцу каталога ~/play право на выполнение

## Опции по командам mount, fsck, mkfs, kill
Прочитала man по данным командам и изучила некоторые опции.
mount: опция -l добавляет ярлыки к этому списку
fsck: опция -Т не показывает название при запуске
mkfs: опция -V показывает версию для печати и выхода
kill: опция -s дает сигнал для отправки, это может быть указано имя или номер


## Выводы

В ходе проделанной работы я ознакомилась с файловой системой Linux, её структурой, именами и содержанием каталогов, приобрела практические навыки по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы. 


:::

