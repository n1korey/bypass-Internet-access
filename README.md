# Решение проблемы с доступом к YouTube, Discord, X, etc.
Если не хотите использовать VPN, чтобы пользоваться всеми благами интернета, можно воспользоваться другими способами, которые описаны здесь.
# Использование туннеля через AmneziaWG
> Слегка влияет на качество сетевого трафика
* Скачиваем: [amneziawg-amd64-1.0.0.msi](https://github.com/amnezia-vpn/amneziawg-windows-client/releases)\
(Есть приложение в Apple Store & Google Play "AmneziaWG")

### С помощью AmneziaWG через GitHub

> На данный момент может перестать работать

* Регистрируемся на [GitHub](https://github.com/)
* Переходим в [codespaces](https://github.com/codespaces)
и нажимаем в блоке `Blank` -> `Use this template`, ждём загрузки терминал

* Вставляем в терминал команду: `curl -sSL https://raw.githubusercontent.com/ImMALWARE/bash-warp-generator/main/warp_generator.sh | bash`
* Переходим по ссылке, которую дадут снизу сообщения (там где "Скачать конфиг файлом"), скачиваем файл `WARP.conf`
* Переносим этот файл в приложение AmneziaWG и подключаемся
* 
### С помощью AmneziaWG через Google Shell

> На данный момент может перестать работать

* Переходим в консоль [Google](https://shell.cloud.google.com/?pli=1&show=ide%2Cterminal)

* Вставляем в терминал команду: `curl -sSL https://raw.githubusercontent.com/ImMALWARE/bash-warp-generator/main/warp_generator.sh | bash`
* В консоли появится ссылка, на файл `WARP.conf` — скачиваем
* Переносим этот файл в приложение AmneziaWG и подключаемся

> На данный момент Google Shell может плохо работать из-за нагрузки

### Дополнительный способ через WireSock VPN + WireSockUI

> Может не сработать

* Скачиваем [WireSock VPN Client](https://www.wiresock.net/sdc_download/1066/?key=7dgnyow9g0nju36l7to4wtlwy3zpca)
* Вместе с ним скачиваем [WireSockUI](https://github.com/wiresock/WireSockUI/releases/download/v0.2.8/WireSockUI-v0.2.8-AnyCPU-no-uwp.zip)

- Устанавливем WireSock VPN Client
- WireSockUI необходимо разархивировать

* Переходим либо в [codespaces](https://github.com/codespaces) (в блоке `Blank` -> `Use this template`, ждём загрузки терминал),
* Либо в [Google](https://shell.cloud.google.com/?pli=1&show=ide%2Cterminal) как из способов выше

- Вставляем команду: `curl -sSL https://raw.githubusercontent.com/ImMALWARE/bash-warp-generator/main/warp_generator.sh | bash`

* Скачиваем файл `WARP.conf`, который дадут нам в консоли
* Открываем этот файл любым способом (Блокнот, VSCode и т.д), вставляем в самый конец файла: `AllowedApps = Discord`

- Открываем файл `WireSockUI.exe`, из папки, куда мы переместили (or разархивировали) программу
- Ищем кнопку `Add Tunnel` и добавляем файл `WARP.conf`
- Далее `Activate`

# Использование zapret-wins (dpi+udp+tcp)
> Самый эффективный, поскольку не влияет на пинг (only windows)
- Способ от Flowseal [zapret-discord-youtube](https://github.com/Flowseal/zapret-discord-youtube) либо:

* Скачиваем архив [zapret-win-bundle](https://github.com/bol-van/zapret-win-bundle/archive/refs/heads/master.zip)
* Разархивируем, переходим по пути `zapret-win-bundle-master\zapret-winws`
* Перекидываем в эту папку файлы из этого репозитория
* Запускаем файл `preset_my.cmd`

> Антивирусы могут ругаться на файл WinDivert
