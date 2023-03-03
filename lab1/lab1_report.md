University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [IP Telephony](https://github.com/itmo-ict-faculty/ip-telephony)
Year: 2022/2023
Group: K34202
Author: Malyshev Alexey Andreevich
Lab: Lab1
Date of create: 02.03.2023
Date of finished: 02.03.2023

##### Цель работы: 
Изучить рабочую среду Cisco Packet Tracer, ознакомить- ся с интерфейсами основных устройств, типами кабелей, научиться собирать топологию. Изучить построение сети IP-телефонии с помощью маршрутизатора, коммутатора и IP телефонов Cisco 7960 в среде Packet tracer.
Отчет поделен на 2 части - работа с первой схемой и второй.

#### I часть

Схема изучена и собрана в Cisko Packet (рисунок 1).

Рисунок 1 - созданная схема

Далее компьютерам были назначены адреса в сети. На рисунке 2 показан терминал PC0 и назначенный ему IP адресс.

Рисунок 2 - настройка PC0

После настройки всех IP-адресов, выполнена проверка работоспособности сети (рисунок 3).

Рисунок 3 - пинги от PC0 к остальным компьютерам

#### II часть

Собрана новая схема сети, в котором сразу изменено название для одного из роутеров (рисунок 4).

Рисунок 4 - Схема сети 
> Заметка: нужно использовать именно маршрутизатор 2811, потому что другие не поддерживают нужные функции

Перед настройкой CMERouter следует включить питание в установленых телефонах (рисунок 5).

Рисунок 5 - включение телефонов

Для CMERouter открыт терминал настройки. В нем настроен IP-адрес для порта f0/0, DHCP-сервер для передачи голоса и данных на маршрутизаторе, а также параметры VoIP (рисунки 6-7).

Рисунок 6 - настройка IP и DHCP

Рисунок 7 - настройка параметров VoIP

Также необходимо настройть vlan у коммутатора для работы с VoIP (рисунок 8).

Рисунок 8 - настройка vlan для работы с VoIP

Последний штрих -- осталось задать телефонные номера для подключенных устройств (рисунок 9)

Рисунок 9 - команды для задания номеров

Для проверки позвоним с телефонов

Рисунок 10 - прозвон с телефона 01 на 02

Рисунок 11 - прозвон с телефона 02 на 01

#### Вывод
В результате выполнения лабораторной работы смоделировано несколько сетей в Cisco Packet Tracer, а также изучен принцип работы сетей VoIP.
