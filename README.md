XML (saved with -oX) to HTML
```
xsltproc scan.xml -o scan.html
```

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
nmap -vv -sU -p <PORT> <IP> -Pn -n
```

Basic DNS enum
```
nmap -script=dns-nsid <IP>
```
