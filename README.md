# Computer-networks-CiscoPacketTracer 04.12.2023
## Ниже представлены 6 настроенных компьютерных сетей в Cisco Packet Tracer, в которых реализованы базовые сетевые протоколы
### 1. Ограничение доступа сетей друг-другу с помощью VLAN
![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/aa970181-9bd2-489c-a918-f93bc034b357)

### 2. Настройка статической маршрутизации с помощью ip route
![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/f7ff7748-8863-47db-911a-875ada4b0f11)

### 3. Настройка динамической маршрутизации с помощью протоколов EIGRP и OSPF
2 простые сети, использующие протоколы EIGRP и OSPF:

![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/29350dd0-4633-4e2b-9037-ba88015f0d3b)

Усложненный вид, использующий OSPF-протокол для динамической маршрутизации и доступом к веб-серверу

![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/a30ca7f0-10eb-4bd1-8d3d-9b6ae3cd271b)

### 4. Настройка динамического и статического NAT
На коммутаторах внутренней сети настроены VLAN и динамическая маршрутизация OSPF

Перегруженный NAT на edgeRouter. edgeRouter являетсяя основным шлюзом для всех маршрутизаторов внутренней сети.

Статический NAT на edgeRouter. При запросе веб-страницы из глобальной сети, запрос перенаправляется на in-web-server.

![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/382fa40d-1d3d-40e8-b8a9-7d0e7d5f7ad1)
![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/44c689ad-e168-43f5-a6cf-8fbd842456fe)

### 5. Настройка беспроводного маршрутизатора и клиента, получение ip с помощью DHTP
![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/ea07ec7b-b6e1-462a-8e3b-00d5dcd8b03a)

Для сети __помеченной зеленым__ работает динамическая раздача ip адресов с внутреннего сервера

Запрос на получение ip адреса перенаправляется из __edgeRunners__ на IN-WEB-SERVER, DHTP
> [Конфигурация маршруторизаторе внутренней сети (edgeRunners)](edgeRunners_5_startup-config.txt)

![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/8cad9f4c-4f93-45e2-a54b-02a6622e989f)

Перегруженный NAT на edgeRouter настроен так, что сеть __помеченной красным__ не имеет доступ в глобальную сеть.

Возможно получение веб-страницы c ex-web-server и с in-web-server из внутренней сети (кроме красной).

external user может просматривать сайт с сервера in-web-server (обращаясь к внешнему порту edgeRouter).

### 6. Настройка ACL-списков
На маршруторизаторе внутренней сети настроены ACL-списки, создающие ограничения доступа. Все условия ACL указанны на скриншоте.
> [Конфигурация маршруторизаторе внутренней сети (edgeRunners)](edgeRunners_6_startup-config.txt)

![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/be2ce7e6-e93c-4fd0-b32b-6a9fb2a2c457)
