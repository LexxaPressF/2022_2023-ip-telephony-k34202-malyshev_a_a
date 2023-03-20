University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [IP Telephony](https://github.com/itmo-ict-faculty/ip-telephony)
Year: 2022/2023
Group: K34202
Author: Malyshev Alexey Andreevich
Lab: Lab2
Date of create: 19.03.2023
Date of finished: 20.03.2023

##### Цель работы: 
Изучить построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960.

Отчет поделен на 2 части - работа с первой схемой и второй.

#### I часть
Создана схема, подключены все устройства, настроен CMERouter (название, отключен синтаксис ввода слов от DNS серверов и заданы пароли для защиты маршрутизатора). Схема с настройкой показаны на рисуноке 1.

![1](https://user-images.githubusercontent.com/57321062/226312511-81a7892c-d697-4fee-a0f9-bb5d1e877707.png)
Рисунок 1 - первоначальная настройка

Настроен DHCP сервера для передачи голоса и данных на CMERouter (рисунок 2).

![2](https://user-images.githubusercontent.com/57321062/226312546-27a55fbf-03af-4fd8-ad30-0c585fc7bbb5.png)
Рисунок 2 - настройка DHCP

Настроен Cisco CallManager Express на CMERouter (рисунок 3).

Р![3](https://user-images.githubusercontent.com/57321062/226312597-18010a8d-b06a-4621-be28-8cd74e00e51e.png)
исунок 3 - настройка CCE

Настроены интерфейсы Cisco коммутаторы для работы через vlan (рисунок 4).

![4](https://user-images.githubusercontent.com/57321062/226312635-75fc16d8-8ad7-4dcc-8407-c056d39fd6a2.png)
Рисунок 4 - настройка vlan

Настроены номера для телефонов (рисунок 5).

![5](https://user-images.githubusercontent.com/57321062/226312654-d1aeff4a-499c-45fc-a64b-1b3bcbee0264.png)
Рисунок 5 - настройка телефонов

Все телефоны подключены успешно (рисунок 6)

![6](https://user-images.githubusercontent.com/57321062/226312665-6de3bdc7-7e54-4afa-9e05-478a012c7665.png)
Рисунок 6 - вывод консоли

Выполнен прозвон с одного телефона на другой для проверки работоспособности системы (рисунок 7).

![7](https://user-images.githubusercontent.com/57321062/226312675-935fd503-0656-4553-8969-df0f0e94262a.png)
Рисунок 7 - прозвон с телефона 22 на 11

#### II часть
Создана новая схема (рисунок 8).

![8](https://user-images.githubusercontent.com/57321062/226312692-65ad406f-68e4-4cd1-b217-a657c2fcced3.png)
Рисунок 8 - новая рабочая схема

Затем настроены vlan на свитче (рисунок 9).

![9](https://user-images.githubusercontent.com/57321062/226312709-3ad2a8ea-ee67-48a4-a74c-de5f8eda2e31.png)
Рисунок 9 - настройка vlan

Даллее настроен vlan 99 (риснок 10).

![10](https://user-images.githubusercontent.com/57321062/226312722-67e98188-439a-49b3-ad3c-7b72ec086cec.png)
Рисунок 10 - настройка работы vlan 99

А также 10 и 20 (рисунок 11).

![11](https://user-images.githubusercontent.com/57321062/226312733-1f89ba2e-631a-4a76-a3cc-28009b12f98d.png)
Рисунок 11 - настройка vlan 10 и 20

> vlan 99 смотрит в сторону роутера, а vlan 10 и 20 смотрят в сторону оконечных устройств

На CMERouter созданы логические подынтерфейсы для vlan 10, vlan 20 и vlan 99 (роутер 12).

![12](https://user-images.githubusercontent.com/57321062/226312744-84a25069-7927-4e4e-a8da-47fd7349b643.png)
Рисунок 12 - настройка подынтерфейсов

На CMERouter также прописаны настройки DHCP сервера (рисунок 13).

![13](https://user-images.githubusercontent.com/57321062/226312753-0b38cd37-1b78-4ae3-9565-086af462a01a.png)
Рисунок 13 - настройка DHCP

Все также на роутере настроен телефонный сервис и номера телефонов (рисунок 14).

![14](https://user-images.githubusercontent.com/57321062/226312760-c4a6efd7-e6a2-48f6-9000-c2e1547ad5f0.png)
Рисунок 14 - настройка телефонного сервиса

Ну и наконец настроены ip адресса виртуальных телефонов (рисунок 15).

![15](https://user-images.githubusercontent.com/57321062/226312822-750d6c4f-e3f5-481d-b03c-fc44cb24f3df.png)
Рисунок 15 - настройка ephones

Последнее --- проверка (рисунок 16).

![16](https://user-images.githubusercontent.com/57321062/226312829-e44c0b6e-b8ed-4a36-8ebf-549078bfdc69.png)
Рисунок 16 - прозвон

Вывод: Изучено построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960.
