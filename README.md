# Discord Rich Presence

Этот скрипт на Python использует библиотеку `pypresence` для отображения информации о системе в Discord Rich Presence.

## Подготовка
- Python 3.x
- Библиотека `pypresence`
- Библиотека `psutil`

## Установка
1. Клонируйте или загрузите репозиторий.
2. Установите необходимые библиотеки, выполнив следующую команду:
   
   ```sh
   pip install pypresence psutil
   ```
   
3. Замените переменную `client_id` на ваш реальный идентификатор клиента, полученный из Discord Developer Portal.

## Использование
1. Запустите скрипт с помощью следующей команды:
   
   ```sh
   python main.py
   ```
   
2. Скрипт будет непрерывно обновлять Discord Rich Presence с текущим использованием оперативной памяти и ЦП.
3. Он также будет отображать большое изображение плюшевой лисички.

## Автор
- [pypresence](https://github.com/qwertyquerty/pypresence) - библиотека от qwertyquerty
- [psutil](https://github.com/giampaolo/psutil) - библиотека от giampaolo

## Лицензия
Этот проект распространяется под [лицензией MIT](LICENSE).
