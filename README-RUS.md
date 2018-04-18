Докеризированный Dante socks5-сервер для работы с мессенджером telegram
=======================================================================

**УСТАРЕВШАЯ ВЕРСИЯ. ИСПОЛЬЗУЙТЕ** [https://hub.docker.com/r/schors/tgdante2/](https://hub.docker.com/r/schors/tgdante2/)

[ENGLISH Version](README.md)

Преимущества
------------
* Docker, Docker Compose
* Скрипты для добавления/удаления пользователей и смены паролей
* Ограничение для использования только с telegram

Требования
----------

* [Docker](https://www.docker.com/docker-community) для контейнеров
* [Docker Compose](https://docs.docker.com/compose/) - программа для запуска и управления контейнерами
* [apg](http://www.adel.nursat.kz/apg/) - программа для генерации паролей

Использование
-------------

* Клонируйте репозиторий
* Отредактируйте dante/sockd.conf при необходимости:
  * external: адрес, который будет использоваться для исходящих соединений. Это может быть IP-адрес или имя интерфейса.
  * Раскоментируйте соответствующие строки для поддержки IPv6
* Отредактируйте dante/Dockerfile при необходимости:
  * Строка `ENV WORKERS 50` отвечает за количество предзапущенных процессов
* Запустите `docker-compose up -d`
* Используйте скрипты в папке `scripts` для добавления/удаления пользователей и смены паролей

На орехи
--------

* PayPal https://www.paypal.me/schors
* Яндекс.Деньги http://yasobe.ru/na/schors
* BTC:17V94QS4vaBwec1Qwqp2ow5b3tbrRGGcne

Ссылки
------

* [Telegram](https://telegram.org/) мессенджер
* [Dante](https://www.inet.no/dante/index.html) свободнораспространяемый SOCKS-сервер

* [Неугомонный Фил](https://2018.schors.spb.ru) Неугомонный Фил :tm:
* [Роскомнадзор](http://rkn.gov.ru) Федеральная служба по надзору в сфере связи, информационных технологий и массовых коммуникаций


---
[![UNLICENSE](noc.png)](UNLICENSE)
