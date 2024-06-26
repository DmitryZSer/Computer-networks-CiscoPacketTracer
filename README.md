# Computer-networks-CiscoPacketTracer 04.12.2023
## Ниже представлены 6 настроенных компьютерных сетей в Cisco Packet Tracer, в которых реализованы базовые сетевые протоколы
### 1. Ограничение доступа сетей друг-другу с помощью VLAN
![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/aa970181-9bd2-489c-a918-f93bc034b357)
### 2. Настройка динамической маршрутизации с помощью протоколов EIGRP и OSPF
2 простые сети, использующие протоколы EIGRP и OSPF:
![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/29350dd0-4633-4e2b-9037-ba88015f0d3b)
Усложненный вид, использующий OSPF-протокол для динамической маршрутизации и доступом к веб-серверу
![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/a30ca7f0-10eb-4bd1-8d3d-9b6ae3cd271b)
### 3. Настройка динамического и статического NAT
На коммутаторах внутренней сети настроены VLAN и динамическая маршрутизация OSPF

Перегруженный NAT на edgeRouter. edgeRouter являетсяя основным шлюзом для всех маршрутизаторов внутренней сети.

Статический NAT на edgeRouter. При запросе веб-страницы из глобальной сети, запрос перенаправляется на in-web-server.
![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/382fa40d-1d3d-40e8-b8a9-7d0e7d5f7ad1)
![image](https://github.com/DmitryZSer/Computer-networks-CiscoPacketTracer/assets/128312523/44c689ad-e168-43f5-a6cf-8fbd842456fe)
