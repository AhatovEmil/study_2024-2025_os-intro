---
## Front matter
lang: ru-RU
title: Лабораторная работа №2
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

Изучить идеологию и применение средств контроля версий.
Освоить умения по работе с git.

## Задание

1. Создать базовую конфигурацию для работы с git.
2. Создать ключ SSH.
3. Создать ключ PGP.
4. Настроить подписи git.
5. Зарегистрироваться на Github.
6. Создать локальный каталог для выполнения заданий по предмету.

## установка git

Установливаю git: dnf install git

![установка](image/1.png){ #fig:001 width=70% }

## установка gh

Устанавливаю gh: dnf install gh

![установка](image/2.png){ #fig:002 width=70% }

## Настройка git

Базовая настройка git

Зададаю имя и email для моего репозитория:
git config --global user.name "Emil Ahatov"
git config --global user.email "ahatovemil48@gmail"
Настраиваю utf-8 в выводе сообщений git:
git config --global core.quotepath false
Настраиваю верификацию и подписание коммитов git
Зададаю имя начальной ветки (будем называть её master):
git config --global init.defaultBranch master
Параметр autocrlf:
git config --global core.autocrlf input
Параметр safecrlf:
git config --global core.safecrlf warn

![базовая настройка git](image/3.png){ #fig:003 width=70% }

## Создание ключей

Создаю ключи ssh по алгоритму rsa с ключём размером 4096 бит:
ssh-keygen -t rsa -b 4096
по алгоритму ed25519:
ssh-keygen -t ed25519
Создаю ключи pgp
Генерируем ключ gpg --full-generate-key

![создание ключей](image/4.png){ #fig:004 width=70% }

## Создание ключей

![окно подтверждения](image/5.png){ #fig:005 width=70% }

## Создание ключей

![ключ](image/6.png){ #fig:006 width=70% }

## Добавление ключей

Выводим список ключей и копируем отпечаток приватного ключа.Cкопировал сгенерированный PGP ключ в буфер обмена:

gpg --armor --export <PGP Fingerprint> | xclip -sel clip

Перехожу в настройки GitHub , нажмимаю на кнопку New GPG key и вставьте полученный ключ в поле ввода.

![копирование ключа](image/7.png){ #fig:007 width=70% }

## Создание ключей

![добавление ключа](image/8.png){ #fig:008 width=70% }

## авторизация

Авторизуюсь через браузер

![авторизация](image/9.png){ #fig:009 width=70% }

## Создание репозитория

создание репозитория курса на основе шаблона
прописываю комнды для создания репозитория:

mkdir -p ~/work/study/2022-2023/"Операционные системы"
cd ~/work/study/2022-2023/"Операционные системы"
gh repo create study_2022-2023_os-intro --template=yamadharma/course-directory-student-template --public
git clone --recursive git@github.com:<owner>/study_2024-2025_os-intro.git os-intro

![создание репозитория](image/10.png){ #fig:010 width=70% }

## Настройка каталога курса

Перехожу в каталог курса:

cd ~/work/study/2022-2023/"Операционные системы"/os-intro

Удаляю лишние файлы:

rm package.json

Создаю необходимые каталоги:

echo os-intro > COURSE
make

Отправляю файлы на сервер:

git add .
git commit -am 'feat(main): make course structure'
git push

![отправка на сервер](image/11.png){ #fig:011 width=70% }

## Выводы

Я изучил идеологию и применение средств контроля версий.
Освоил умения по работе с git.
