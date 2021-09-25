# Кастомные eggs для панели Pterodactyl

На данный момент здесь имеются 3 самых популярных лаунчера - sashok724, его форк от KeeperJerry и GravitLauncher.

## Получение обновлений

Все файлы скачиваются только с официальных репозиториев лаунчеров, поэтому мои конфиги не придётся обновлять слишком часто.

## Немного о GravitLauncher
:warning: Все создаваемые инсталлятором гиперссылки пришлось заменить на копирование из-за некоторых проблем. Также, из-за вырезанной совместимости с Java 8 в новых версиях, мне пришлось сделать форк репозитория с Dockerfile для создания контейнера с полной версией Java 11 от BellSoft (чтобы не было проблем с JavaFX). Если же вы мне не доверяете, можете сами форкнуть [мой репозиторий с Dockerfile](https://github.com/alexeylesin/pterodactyl-core), залить его на DockerHub и сменить ссылку в настройках.

## Процесс установки

1. Переходим в админ-панель
![](https://i.imgur.com/LUTz4Co.jpg)
2. В левой панели выбираем "Nests" и нажимаем на "Import Egg"
![](https://i.imgur.com/wCC3Whu.jpg)
3. Далее делаем всё как показано на скрине
![](https://i.imgur.com/qQrgHK5.jpg)
4. Перезагружаем демон панели командой ```systemctl restart wings```

## Использование

Во время создания сервера, в разделе "Nest" выбираем "Minecraft", а в "Egg" - название лаунчера.
