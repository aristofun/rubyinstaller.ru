---
layout: downloads
title: Загрузить
permalink: /downloads/
---
### Какую версию загружать?

Если вы не знаете, какую версию RubyInstaller установить и только начинаете работать с Ruby, то используйте
установщик <b>Ruby+DevKit 2.5.x (x64)</b>. Он содержит наибольшее количество совместимых гемов и устанавливает
MSYS2-DevKit вместе с Ruby, потому гемы с расширением C скомпилируются сразу же. 32-битную (x86) версию советуем,
только если приходится работать с пользовательскими 32-битными встроенными DLL- или COM-объектами.

### Как обновлять?

Обновите Ruby до свежего патча (например, с версии 2.4.1 до 2.4.4), запустив соответствующую версию установщика.
Существующие гемы не перезапишутся и будут стабильно работать с новыми версиями. Используйте RubyInstaller
(без DevKit), чтобы обновить установки. Сам DevKit обновляйте отдельно с помощью команды `ridk install`.

Если вы загружаете версию Ruby из другой стабильной ветки (2.5.x, например), используйте новую директорию для этого.
То есть не следует обновлять RubyInstaller-2.4.x до версии 2.5.x, так как гемы с расширением C несовместимы между
Ruby 2.4 и 2.5. Больше информации об этом в разделе [FAQ](https://github.com/oneclick/rubyinstaller2/wiki/FAQ#user-content-update-install).

### Какую версию Development Kit выбрать?

Для Ruby 2.4.0 и новее в качестве комплекта разработки используется [пакет MSYS2](http://www.msys2.org). Он входит в
состав <b>Ruby+DevKit</b> как компонент по выбору, чтобы не было нужды скачивать/устанавливать MSYS2 дополнительно.
Если используете Ruby без DevKit, то MSYS2 DevKit устанавливайте отдельно командой `ridk install`

MSYS2 требуется, чтобы компилировать дополнения на C/C++ для Ruby. Он необходим также для [Ruby on Rails](http://rubyonrails.org/). 
Более того, MSYS2 позволяет загружать и использовать [сотни Open Source библиотек](https://github.com/Alexpux/MINGW-packages), 
от которых могут зависеть некоторые гемы.

Среду разработки MSYS2 запускайте в консоли с помощью `ridk enable`. Она добавляет команды `make`, `gcc`, `pacman` 
или `sh` к пути поиска. Больше информации в [вики](https://github.com/oneclick/rubyinstaller2/wiki/The-ridk-tool).

### Скорость и  удобство

RubyInstaller компилируется с помощью GCC в дату выхода. Установленный Ruby — это нативное Windows-приложение,
которое работает вкупе с функциональным дистрибутивом [MSYS2](http://www.msys2.org) и
[MINGW-библиотеками](https://github.com/Alexpux/MINGW-packages).

Ищите больше о RubyInstaller и его альтернативах [здесь]({{ "/about/comparison" | relative_url }}).

### Документация

Основы и документация стандартной библиотеки Ruby входит в установочный пакет. Мы рекомендуем почитать ещё и
[online-вариант](https://ruby-doc.org/) или HTML-версию, которую можно скачать на [ruby-doc.org](https://ruby-doc.org/downloads/).

### Поддержка

Делитесь вашим мнением о RubyInstaller или предлагайте улучшения в нашей дружелюбной и полезной 
[Google Группе](http://groups.google.com/group/rubyinstaller). Счастливого программирования на Ruby!