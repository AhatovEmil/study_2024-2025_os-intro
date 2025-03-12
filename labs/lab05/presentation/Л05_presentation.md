---
## Front matter
lang: ru-RU
title: Лабораторная работа №5
subtitle: Операционные сисетмы
author:
  - Ахатов Э. Э.
institute:
  - Российский университет дружбы народов, Москва, Россия
  - Объединённый институт ядерных исследований, Дубна, Россия
date: 01 января 1970

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
---

## Цель работы

Познакомиться с pass, gopass, native messaging, chezmoi. Научиться пользоваться этими утилитами, синхронизировать их с гит.

## Задание

1. Установить дополнительное ПО
2. Установить и настроить pass
3. Настроить интерфейс с браузером
4. Сохранить пароль
5. Установить и настроить chezmoi
6. Настроить chezmoi на новой машине
7. Выполнить ежедневные операции с chezmoi

## Устанавливаем pass и gopass 

![Установка](image/1.png){ #fig:001 width=70% }

![Установка](image/2.png){ #fig:002 width=70% }

## Просмотрим список ключей. Инициализируем хранилище. Синхронизируемс git Создадим структуру git.

![список ключей](image/3.png){ #fig:003 width=70% }

![список ключей](image/4.png){ #fig:004 width=70% }

![инициализация](image/5.png){ #fig:005 width=70% }

## Для синхронизации выполняется следующая команда: pass git pull pass git push

![синхронизация](image/6.png){ #fig:006 width=70% }

![синхронизация](image/7.png){ #fig:007 width=70% }

## Для взаимодействия с броузером используем интерфейс native messaging.

![установка](image/8.png){ #fig:008 width=70% }

![установка](image/9.png){ #fig:009 width=70% }

## Добавим новый пароль. Отобразим пароль для указанного имени файла. Заменим существующий пароль

![добавление пароля](image/10.png){ #fig:010 width=70% }

![добавление пароля](image/11.png){ #fig:011 width=70% }

## Установим дополнительное программное обеспечение. Установим шрифты.

![установка](image/12.png){ #fig:012 width=70% }

![установка](image/13.png){ #fig:013 width=70% }

## Установим бинарный файл. Создадим собственный репозиторий с помощью утилит

![установка](image/14.png){ #fig:014 width=70% }

![установка](image/15.png){ #fig:015 width=70% }

## На второй машине инициализируем chezmoi с репозиторием dotfiles. Проверим, какие изменения внесёт chezmoi в домашний каталог.

![инициализация](image/16.png){ #fig:016 width=70% }

## добавим в файл конфигурации ~/.config/chezmoi/chezmoi.toml следущие строки

![инициализация](image/17.png){ #fig:017 width=70% }

## Вывод 

Мы познакомились с pass, gopass, native messaging, chezmoi. Научились пользоваться этими утилитами, синхронизировали их с гит.


