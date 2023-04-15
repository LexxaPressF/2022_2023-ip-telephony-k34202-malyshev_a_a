University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [IP Telephony](https://github.com/itmo-ict-faculty/ip-telephony)
Year: 2022/2023
Group: K34202
Author: Malyshev Alexey Andreevich
Lab: Lab4
Date of create: 14.04.2023
Date of finished: 15.04.2023

##### Цель работы: 
Изучить построение сети IP-телефонии между удаленными филиалами с помощью маршрутизаторов Cisco 2811 и коммутаторов Cisco 2950Т. Изучить построение сети IP-телефонии между удаленными филиалами с помощью маршрутизаторов Cisco 2811 и Cisco 2600XM.

В работе выполняется только первая часть.

#### I часть

Настроены интерфейсы fa0/0 и s0/3/0 на маршрутизаторах Cisco 2811.

![1](https://user-images.githubusercontent.com/57321062/232224007-675a7c2f-3722-4986-960a-77f8912bfff8.png)
![2](https://user-images.githubusercontent.com/57321062/232224016-19aaca4c-8c0c-4e3b-9374-76c59ab9ec52.png)


Настроены также как и в лабораторной №2: 
- Маршрутизатор Cisco 2811; 
- Коммутатор Cisco 3950Т; 
- IP-телефоны.

Настроен серверы DHCP на маршрутизаторах для передачи голоса и данных между ними.

![3](https://user-images.githubusercontent.com/57321062/232224023-68a28442-535c-4847-9d15-90381d4d5021.png)

Настроена динамическая маршрутизация RIP между маршрутизаторами.

![4](https://user-images.githubusercontent.com/57321062/232224032-11180376-8cc4-4534-ad3e-0d8b2d0e6274.png)

Настроены услуги телефонии Cisco CallManager Express (количество телефонов, порты переадрессация) на маршрутизаторе 2811.

![5](https://user-images.githubusercontent.com/57321062/232224046-0f36ba7c-681d-4c7b-b4d9-8c8702ca3652.png)

Настроены порты коммутатора:
- Явно указаны порты доступа (команда switchport mode access);
- Указана VLAN через который используется для передачи голоса;

![6](https://user-images.githubusercontent.com/57321062/232224059-f47f4dec-ef99-4219-a605-3a7d6c748b8e.png)

Проверка прозвоном между удаленными IP-телефонами:

![7](https://user-images.githubusercontent.com/57321062/232224076-0cc9e57b-79bb-48fb-88e2-7d920b8e60a6.png)

Вывод: Изучено построение сети IP-телефонии между удаленными филиалами с на базе маршрутизаторов Cisco 2811 и коммутаторов Cisco 2950Т, а также на базе маршрутизаторов Cisco 2811 и Cisco 2600XM.
