<div align="center">

```
 ███╗   ██╗███████╗████████╗██╗    ██╗ ██████╗ ██████╗ ██╗  ██╗
 ████╗  ██║██╔════╝╚══██╔══╝██║    ██║██╔═══██╗██╔══██╗██║ ██╔╝
 ██╔██╗ ██║█████╗     ██║   ██║ █╗ ██║██║   ██║██████╔╝█████╔╝
 ██║╚██╗██║██╔══╝     ██║   ██║███╗██║██║   ██║██╔══██╗██╔═██╗
 ██║ ╚████║███████╗   ██║   ╚███╔███╔╝╚██████╔╝██║  ██║██║  ██╗
 ╚═╝  ╚═══╝╚══════╝   ╚═╝    ╚══╝╚══╝  ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝
```

**`[ TCP/IP :: FROM WIRE TO PACKET :: LEARNING LOG ]`**

`> "The network is the computer."`

</div>

```
NETWORK(7)                  Learning Manual                  NETWORK(7)
```

## NAME

`network` — личный дневник по изучению компьютерных сетей: от кабеля до пакета.

## SYNOPSIS

```console
$ git clone https://github.com/Doosi41/network.git
$ cd network
$ cat readme.md
```

## DESCRIPTION

Никакой магии. Любая сеть — это байты, провода и договорённости (протоколы).
Цель: понять, что происходит между нажатием Enter и ответом сервера, и уметь
увидеть это своими глазами через `tcpdump` и Wireshark.

```
  [ you ]──►[ app ]──►[ TCP ]──►[ IP ]──►[ ETH ]═══ wire ═══►[ ??? ]
   curl      HTTP      port      route     MAC                  :)
```

## LAYOUT

```
network/
├── readme.md     ← ты здесь (man page)
├── notes/        ← конспекты: теория своими словами
└── labs/         ← практика: команды, скрипты, дампы, схемы
```

## ROADMAP

```
[ ] 01  Основы ............... OSI, TCP/IP, что вообще такое сеть
[ ] 02  L1/L2 ................ Ethernet, MAC, коммутаторы, VLAN
[ ] 03  L3 ................... IP, подсети, маршрутизация
[ ] 04  L4 ................... TCP, UDP, порты, рукопожатие
[ ] 05  L7 ................... DNS, DHCP, HTTP/HTTPS, TLS
[ ] 06  Периметр ............. NAT, firewall, VPN
[ ] 07  Эфир ................. Wi-Fi и беспроводные сети
[ ] 08  Арсенал .............. ping, traceroute, dig, curl, tcpdump, Wireshark
```

| # | Тема | Конспект |
|---|------|----------|
| 01 | Основы: OSI и TCP/IP | [notes/01-basics.md](notes/01-basics.md) |
| 02 | Физический и канальный уровень | [notes/02-physical-link.md](notes/02-physical-link.md) |
| 03 | IP, подсети, маршрутизация | [notes/03-ip.md](notes/03-ip.md) |
| 04 | TCP, UDP, порты | [notes/04-transport.md](notes/04-transport.md) |
| 05 | DNS, DHCP, HTTP/HTTPS, TLS | [notes/05-app-protocols.md](notes/05-app-protocols.md) |
| 06 | NAT, firewall, VPN | [notes/06-nat-firewall.md](notes/06-nat-firewall.md) |
| 07 | Wi-Fi | [notes/07-wifi.md](notes/07-wifi.md) |
| 08 | Инструменты | [notes/08-tools.md](notes/08-tools.md) |

## METHOD

```
1. READ     прочитал тему
2. WRITE    записал главное своими словами  → notes/
3. HACK     повторил руками в терминале     → labs/
4. BREAK    сломал, посмотрел в tcpdump, понял почему
5. REPEAT   непонятное → раздел «Вопросы», вернуться позже
```

## EXAMPLES

```console
$ ping -c 3 1.1.1.1              # живой ли хост (ICMP)
$ traceroute 1.1.1.1             # путь пакета по маршрутизаторам
$ dig example.com +short         # кто такой example.com (DNS)
$ curl -v https://example.com    # весь HTTP/TLS разговор
$ sudo tcpdump -i en0 -n port 53 # подслушать DNS-запросы
```

## SEE ALSO

- RFC 791 (IP), RFC 793 (TCP), RFC 1034/1035 (DNS) — первоисточники
- `man ping`, `man tcpdump`, `man dig`
- _добавляй сюда книги, курсы, видео_

## STATUS

```
[##........] 0/8 тем пройдено    uptime: day 1
```

```
$ _
```
