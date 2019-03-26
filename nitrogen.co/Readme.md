# NITROGEN

__PROBLEM__

GuDLuck IP = 192.168.0.11

__SOLUTION__

So let's start with NMAP tools to the ip address 
`nmap -A -v 192.168.0.11`
and we got the following output
```
Starting Nmap 7.60 ( https://nmap.org ) at 2019-03-26 01:34 UTC
Nmap scan report for 192.168.0.11
Host is up (0.00024s latency).
Not shown: 998 closed ports
PORT   STATE SERVICE VERSION
22/tcp open  ssh     OpenSSH 7.2p2 Ubuntu 4ubuntu2.4 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey:
|   2048 49:4a:79:a8:32:7f:b9:4d:6c:83:a2:1e:7b:5d:c7:f1 (RSA)
|   256 f2:20:e8:52:84:bf:f7:57:e1:21:48:3e:e4:94:a8:f6 (ECDSA)
|_  256 5e:2e:d1:13:72:b7:33:5f:fe:cc:48:db:fc:44:24:a3 (EdDSA)
80/tcp open  http    Apache httpd 2.4.18 ((Ubuntu))
| http-methods:
|_  Supported Methods: OPTIONS GET HEAD POST
| http-robots.txt: 2 disallowed entries
|_/openvpn-admin/ /flag1/
|_http-server-header: Apache/2.4.18 (Ubuntu)
|_http-title: Site Maintenance NITR0GEN
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

NSE: Script Post-scanning.
Initiating NSE at 01:34
Completed NSE at 01:34, 0.00s elapsed
Initiating NSE at 01:34
Completed NSE at 01:34, 0.00s elapsed
Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 7.11 seconds
```

__PROBLEM__

How many port open on Nitrogen

__ANSWER__

2


