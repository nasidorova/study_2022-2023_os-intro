---
## Front matter
lang: ru-RU
title: Презентация к лабораторной работе 1
subtitle: Установка ОС Linux
author:
  - Сидорова Н.А.
institute:
  - Российский университет дружбы народов, Москва, Россия
  - Объединённый институт ядерных исследований, Дубна, Россия
date: 18 февраля 2023

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
Приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

## Техническое обеспечение
Лабораторная работа подразумевает установку на виртуальную машину VirtualBox (https://www.virtualbox.org/) операционной системы Linux (дистрибутив Fedora).
Для установки в виртуальную машину используется дистрибутив Linux Fedora (https://getfedora.org), вариант с менеджером окон i3 (https://spins.fedoraproject.org/i3/).

## Соглашения об именовании
При выполнении работ следует придерживаться следующих правил именования:
1. Пользователь внутри виртуальной машины должен иметь имя, совпадающее с учётной записью студента, выполняющего лабораторную работу.
2. Имя хоста вашей виртуальной машины должно совпадать с учётной записью студента, выполняющего лабораторную работу.
3. Имя виртуальной машины должно совпадать с учётной записью студента, выполняющего лабораторную работу.

## Задание
1. Запуск VirtualBox и создание новой виртуальной машины
2. Настройка установки операционной системы
3. Подключение образа диска дополнений гостевой ОС
4. Выполнение домашнего задания

## Создание виртуальной машины
Имя виртуальной машины - мой логин
Размер основной памяти виртуальной машины — 2048 МБ
Размер нового виртуального жесткого диска — 80 ГБ
Новый оптический привод - образ Fedora

## Установка операционной системы
1. Запустила приложение для установки системы
2. Затем установила систему на диск 
3. Создала аккаунт администратора и пользователя
4. Задала сетевое имя для компьютера

## После установки
1. Обновила все пакеты
2. Установила программы для удобства работы в консоли
3. Подключила автоматическое обновление
4. Отключила систему безопасности SELinux

## Установка драйверов для VirtualBox
1. Установила пакет DKMS
2. Подключила образ диска дополнений гостевой ОС
3. Подмонтировала диск
4. Установила драйвера

## Установка программного обеспечения для создания документации
1. Установила pandoc с необходимыми расширениями
2. Установила дистрибутив TeXlive

## Выполнение домашнего задания
С помощью команды dmesg | grep -i "то, что ищем" получила информацию о 
1. Версии ядра Linux (Linux version).
2. Частоте процессора (Detected Mhz processor).
3. Модели процессора (CPU0).
4. Объёме доступной оперативной памяти (Memory available).
5. Типе обнаруженного гипервизора (Hypervisor detected).
6. Типе файловой системы корневого раздела.
7. Последовательности монтирования файловых систем.

## Вывод 
В ходе выполнения лабораторной работы я приобрела навыки установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

:::

