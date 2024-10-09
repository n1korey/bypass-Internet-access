# Решение проблемы с доступом к YouTube, Discord, X, etc.
Если не хотите использовать VPN, чтобы пользоваться всеми благами интернета, можно воспользоваться другими способами, которые описаны здесь.
# Использование туннеля через AmneziaWG
> Слегка влияет на качество сетевого трафика
* Скачиваем: [amneziawg-amd64-1.0.0.msi](https://github.com/amnezia-vpn/amneziawg-windows-client/releases)\
(Есть приложение в Apple Store & Google Play "AmneziaWG")

### С помощью AmneziaWG через GitHub

* Регистрируемся на [GitHub](https://github.com/)
* Переходим в [codespaces](https://github.com/codespaces)
и нажимаем в блоке `Blank` -> `Use this template`, ждём загрузки терминал

* Вставляем в терминал команду: `curl -sSL https://raw.githubusercontent.com/ImMALWARE/bash-warp-generator/main/warp_generator.sh | bash`
* Переходим по ссылке, которую дадут снизу сообщения (там где "Скачать конфиг файлом"), скачиваем файл
* Переносим этот файл в приложение AmneziaWG и подключаемся
### С помощью AmneziaWG через Google Shell

* Переходим в консоль [Google](https://shell.cloud.google.com/?pli=1&show=ide%2Cterminal)

* Вставляем в терминал команду: `curl -sSL https://raw.githubusercontent.com/ImMALWARE/bash-warp-generator/main/warp_generator.sh | bash`
* В консоли появится ссылка, на файл WARP.conf — скачиваем
* Переносим этот файл в приложение AmneziaWG и подключаемся

> На данный момент Google Shell может плохо работать из-за нагрузки


# Использование zapret-wins (dpi+udp+tcp) (only windows)
> Самый эффективный, поскольку не влияет на пинг
- Способ от Flowseal [zapret-discord-youtube](https://github.com/Flowseal/zapret-discord-youtube) либо:

* Скачиваем архив [zapret-win-bundle](https://github.com/bol-van/zapret-win-bundle/archive/refs/heads/master.zip)
* Разархивируем, переходим по пути `zapret-win-bundle-master\zapret-winws`
* Перекидываем в эту папку файлы из этого репозитория

> Антивирусы могут ругаться на файл WinDivert
