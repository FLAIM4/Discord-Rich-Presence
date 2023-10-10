## Discord Rich Presence

Ниже приведен код на Python для реализации функционала Discord Rich Presence с использованием библиотеки pypresence. Этот код отображает информацию о текущем использовании оперативной памяти (RAM) и процессора (CPU) на вашей системе, а также добавляет изображение в качестве большой обложки.

python
from pypresence import Presence
import time
import psutil

client_id = "id"
RPC = Presence(client_id)
RPC.connect()

while True:
    time.sleep(1)
    ram1 = psutil.virtual_memory().percent
    cpu1 = psutil.cpu_percent()
    RPC.update(
        details=f"RAM: {ram1}% CPU: {cpu1}%",
        large_image='https://media.tenor.com/sKSw-rqsFxQAAAAi/foxy-foxplushy.gif',
    )
Установка модулей
Перед запуском кода необходимо установить следующие модули Python:

pypresence
psutil
Вы можете установить их, используя менеджер пакетов pip, выполнив следующие команды:

pip install pypresence
pip install psutil
Запуск кода
После установки модулей выполните код на Python. Он будет обновлять информацию о состоянии оперативной памяти и процессора каждую секунду и отображать ее в Discord с указанным в коде изображением в качестве большой обложки.

Убедитесь, что заменили значение client_id на свой собственный. Вы можете получить этот идентификатор, создав приложение на Discord Developer Portal.

Надеюсь, это поможет! Если у вас возникнут дополнительные вопросы, не стесняйтесь задавать.
