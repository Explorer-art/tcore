# TCORE
TCORE — это ядро для серверов в игре Warnament. Это улучшенная версия официального ядра сервера, в которой добавлено множество различных новый функций.

# 🚀 Функции

- Добавлено множество новых команд, например: /civ, /op, /deop, /p, /ignore, /msgtoggle, /prefix и т.д.
- Функция выдачи/снятия ролей игрокам которых нет на сервере по их никнейму
- Функция бана и мута игроков которых нет на сервере по их никнейму
- Добавлена роль "Оператор" у которой есть полный доступ ко всем командам
- Консоль в которой можно выполнять команды от имени администратора не заходя на сервер
- Менеджер плагинов
- Теперь не обязательно перезапускать сервер что бы обновить плагин
- Полностью переработана структура базы данных игроков
- Созданы удобные конфигурационные файлы в которых вы можете легко редактировать права ролей, сообщения в чате и т.д.
- Автоматические сообщения в чате и по середине экрана, которые выводятся через определённое количество секунд
- Вы можете создавать свои кастомные плагины и модули ядра

# ✅ Установка
### Установка файлов

```
sudo apt update
sudo apt upgrade
sudo apt install git -y
git clone https://github.com/Explorer-art/tcore.git
```

### Установка Docker
```
sudo apt install -y docker-compose
sudo apt install -y apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
sudo apt install -y docker-ce
sudo docker build -t warnament-server WarnamentServer
```

Что бы запустить сервер введите команду:
```
docker-compose up
```

Что бы запустить сервер без вывода логов в консоль введите команду:
```
docker-compose up -d
```

Что бы выключить сервер нажмите Ctrl+C или введите команду
```
docker-compose down
```

# Вики
Для ядра TCORE создана отдельная [документация](https://github.com/Explorer-art/tcore/wiki). Там вы можете найти более подробную информацию о ядре, о том как установить и запустить свой сервер, о его настройки и многое другое.
