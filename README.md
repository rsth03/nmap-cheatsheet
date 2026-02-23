TCP SYN/ACK pings
```
sudo nmap -PS22,80,443 -PA80,443 <IP> -sn -n
```

Slower/quieter SYN scan
```
sudo nmap -vv -T2 --top-ports=20 -sS <IP> -Pn -n --disable-arp-ping
```

UDP probe
```
sudo nmap -vv -sU -p <PORT> <IP> -Pn -n
```

Basic DNS enum
```
dig @<IP> CH TXT version.bind +time=2 +tries=1
```
