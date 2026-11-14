<a id="top"></a>

<p align="center">
  <img src="assets/hero.svg" alt="BLACKSITE — NETWORK // UNDERGROUND. System online. Network engineering, Linux, security. Illustration of a vintage CRT terminal with network cables and chips." width="100%">
</p>

<p align="center">
  <a href="#overview"><img src="assets/nav/nav-overview.svg" alt="A — Overview" width="150"></a>
  <a href="#network"><img src="assets/nav/nav-network.svg" alt="B — Network" width="150"></a>
  <a href="#roadmap"><img src="assets/nav/nav-roadmap.svg" alt="C — Roadmap" width="150"></a>
  <a href="#lab"><img src="assets/nav/nav-lab.svg" alt="D — Laboratory" width="150"></a>
  <a href="#archive"><img src="assets/nav/nav-archive.svg" alt="E — Archive" width="150"></a>
</p>

<a id="overview"></a>

<p align="center">
  <img src="assets/overview.svg" alt="System overview: networking, Linux, security and laboratory." width="100%">
</p>

<a id="network"></a>

<p align="center">
  <img src="assets/network-path.svg" alt="Packet path: workstation, switch, router, internet, server — with documentation IP addresses and the OSI layers each device handles." width="100%"><br>
  <img src="assets/tcpip-stack.svg" alt="TCP/IP stack as five hardware boards, the Ethernet frame encapsulation and a real IPv4 header in hex." width="100%">
</p>

<a id="roadmap"></a>

<p align="center">
  <img src="assets/roadmap/roadmap-head.svg" alt="Learning roadmap — 0 of 8 modules completed. Notes are templates, labs are empty." width="100%"><br>
  <a href="notes/01-basics.md"><img src="assets/roadmap/card-01.svg" alt="01 BASICS — OSI, TCP/IP. Open notes/01-basics.md" width="100%"></a><br>
  <a href="notes/02-physical-link.md"><img src="assets/roadmap/card-02.svg" alt="02 LINK — Ethernet, MAC, switches, VLAN. Open notes/02-physical-link.md" width="100%"></a><br>
  <a href="notes/03-ip.md"><img src="assets/roadmap/card-03.svg" alt="03 IP — addressing, subnets, routing. Open notes/03-ip.md" width="100%"></a><br>
  <a href="notes/04-transport.md"><img src="assets/roadmap/card-04.svg" alt="04 TRANSPORT — TCP, UDP, ports. Open notes/04-transport.md" width="100%"></a><br>
  <a href="notes/05-app-protocols.md"><img src="assets/roadmap/card-05.svg" alt="05 APP — DNS, DHCP, HTTP/HTTPS, TLS. Open notes/05-app-protocols.md" width="100%"></a><br>
  <a href="notes/06-nat-firewall.md"><img src="assets/roadmap/card-06.svg" alt="06 PERIMETER — NAT, firewall, VPN. Open notes/06-nat-firewall.md" width="100%"></a><br>
  <a href="notes/07-wifi.md"><img src="assets/roadmap/card-07.svg" alt="07 AIR — Wi-Fi. Open notes/07-wifi.md" width="100%"></a><br>
  <a href="notes/08-tools.md"><img src="assets/roadmap/card-08.svg" alt="08 ARSENAL — ping, traceroute, dig, curl, tcpdump. Open notes/08-tools.md" width="100%"></a>
</p>

<a id="lab"></a>

<p align="center">
  <img src="assets/laboratory.svg" alt="Laboratory terminal with example commands: ping, traceroute, dig, curl, tcpdump. Output is not shown." width="100%">
</p>

<details>
<summary><b>▸ copy-paste the lab commands</b></summary>

```console
ping -c 4 192.0.2.1
traceroute -n 203.0.113.80
dig example.com A +short
curl -v https://example.com
sudo tcpdump -i en0 -nn 'tcp port 443'
```

`192.0.2.1` и `203.0.113.80` — адреса из блоков для документации (RFC 5737): на них ничего не отвечает. Для реальной практики подставь свой роутер или `example.com`. Результаты и дампы складывай в [`labs/`](labs/).

</details>

<details>
<summary><b>▸ method: read → write → hack → break → repeat</b></summary>

1. **READ** — прочитал тему.
2. **WRITE** — записал главное своими словами в [`notes/`](notes/).
3. **HACK** — повторил руками в терминале → [`labs/`](labs/).
4. **BREAK** — сломал, посмотрел в `tcpdump` / Wireshark, понял почему.
5. **REPEAT** — непонятное → раздел «Вопросы» конспекта, вернуться позже.

Проверять всё только в **собственной сети или лабораторной среде**. Чужие сети без разрешения владельца не трогаем.

</details>

<details>
<summary><b>▸ primary sources: RFC</b></summary>

| RFC | Тема |
|---|---|
| [RFC 791](https://www.rfc-editor.org/rfc/rfc791) | IP |
| [RFC 792](https://www.rfc-editor.org/rfc/rfc792) | ICMP (ping) |
| [RFC 793](https://www.rfc-editor.org/rfc/rfc793) | TCP |
| [RFC 768](https://www.rfc-editor.org/rfc/rfc768) | UDP |
| [RFC 1034](https://www.rfc-editor.org/rfc/rfc1034) / [1035](https://www.rfc-editor.org/rfc/rfc1035) | DNS |
| [RFC 5737](https://www.rfc-editor.org/rfc/rfc5737) | адреса для документации |

</details>

<a id="archive"></a>

<p align="center">
  <img src="assets/cypherpunk.svg" alt="Cypherpunk archive: Bitcoin genesis block header in hex with its verified hash, a public/private key diagram and a decentralised mesh." width="100%">
</p>

<p align="center">
  <img src="assets/final.svg" alt="Connection terminated. End of transmission." width="100%"><br>
  <a href="#top"><img src="assets/nav/back-to-top.svg" alt="Back to top" width="200"></a>
</p>
