# Networking Analysis

## Traceroute

1. The appropriate command or tool to perform a traceroute to a specified website or IP address
A traceroute works by sending Internet Control Message Protocol (ICMP) packets, and every router involved in transferring the data gets these packets. The ICMP packets provide information about whether the routers used in the transmission are able to effectively transfer the data.
An Internet Protocol (IP) tracer is helpful for figuring out the routing hops data has to go through, as well as response delays as it travels across nodes, which are what send the data toward its destination.

> tracert github.com

```
Трассировка маршрута к github.com [140.82.121.4]
  1     1 ms     1 ms    <1 мс  192.168.0.1
  2     1 ms     1 ms     1 ms  dynamicip-3-78-95-252.pppoe.chelny.ertelecom.ru [95.78.3.252]
  3     1 ms     1 ms     8 ms  lag-6-435.bbr01.nn.ertelecom.ru [91.144.153.98]
  4    29 ms    27 ms    27 ms  ertelekom-ic-317530.ip.twelve99-cust.net [62.115.148.175]
  5    37 ms    33 ms    33 ms  sap-b3-link.ip.twelve99.net [62.115.148.174]
  6    39 ms    42 ms    39 ms  s-bb2-link.ip.twelve99.net [80.91.250.99]
  7    63 ms    60 ms    59 ms  ffm-bb2-link.ip.twelve99.net [62.115.138.105]
  8    59 ms    60 ms    59 ms  ffm-b11-link.ip.twelve99.net [62.115.124.119]
  9    62 ms    64 ms    63 ms  github-ic-350972.ip.twelve99-cust.net [62.115.182.171]
 10     *        *        *     Превышен интервал ожидания для запроса.
 11     *        *        *     Превышен интервал ожидания для запроса.
 12    60 ms    59 ms    62 ms  lb-140-82-121-4-fra.github.com [140.82.121.4]
```
 
## Dig

1. The appropriate command or tool to perform a DNS lookup for a specified domain name

> C:\Users\ROMMAX>nslookup www.github.com

```

╤хЁтхЁ:  DC-SHIRAZ.moskvich.ru
Address:  172.19.39.1

Не заслуживающий доверия ответ:
╚ь :     github.com
Address:  140.82.121.4
Aliases:  www.github.com
```

Syntax

> nslookup [exit | finger | help | ls | lserver | root | server | set | view] [options]

https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/nslookup

> nslookup -type=any gosuslugi.ru

Display all DNS records in the domain zone

```
C:\Users\ROMMAX>nslookup -type=any gosuslugi.ru
╤хЁтхЁ:  DC-SHIRAZ.moskvich.ru
Address:  172.19.39.1

Не заслуживающий доверия ответ:
gosuslugi.ru    internet address = 213.59.253.7
gosuslugi.ru    internet address = 213.59.254.7
gosuslugi.ru    nameserver = ns1.gosuslugi.ru
gosuslugi.ru    nameserver = ns8-l2.nic.ru
gosuslugi.ru    nameserver = ns2.gosuslugi.ru
gosuslugi.ru    nameserver = ns4-l2.nic.ru
gosuslugi.ru    MX preference = 20, mail exchanger = mx68.gosuslugi.ru
gosuslugi.ru    MX preference = 10, mail exchanger = mx.gosuslugi.ru

mx68.gosuslugi.ru       internet address = 213.59.254.2
mx.gosuslugi.ru internet address = 109.207.1.100
```