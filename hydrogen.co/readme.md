# HYDROGEN

__PROBLEM__

The ip address was 192.168.0.10

__SOLUTION__

So let's start with NMAP tools to the ip address 
`nmap -A -v 192.168.0.10`
and we got the following output
```
Starting Nmap 7.60 ( https://nmap.org ) at 2019-03-15 03:16 UTC
PORT   STATE SERVICE VERSION
21/tcp open  ftp     ProFTPD 1.2.6
| ftp-anon: Anonymous FTP login allowed (FTP code 230)
| -rw-r--r--   1 ftp      ftp           472 Jan 19 12:36 email.txt
|_-r--------   1 ftp      ftp            39 Jan 18 16:31 flag1.txt
|_ftp-bounce: server forbids bouncing to low ports <1025
22/tcp open  ssh     OpenSSH 6.0p1 Debian 4+deb7u7 (protocol 2.0)
| ssh-hostkey:
|   1024 24:04:bf:3c:02:c8:ac:cd:5e:41:e8:5e:c8:47:96:76 (DSA)
|   2048 28:fd:24:7b:a5:9a:b6:62:ad:d6:3f:b0:4e:7e:ea:e9 (RSA)
|_  256 eb:b8:37:33:af:eb:a2:a7:4a:84:27:6e:35:65:d4:a6 (ECDSA)
80/tcp open  http    nginx 1.2.1
| http-methods:
|_  Supported Methods: GET HEAD
| http-robots.txt: 1 disallowed entry
|_/phpmyadmin
|_http-server-header: nginx/1.2.1
|_http-title: Hydrogen Co
Service Info: OSs: Unix, Linux; CPE: cpe:/o:linux:linux_kernel

NSE: Script Post-scanning.
Initiating NSE at 03:16
Completed NSE at 03:16, 0.00s elapsed
Initiating NSE at 03:16
Completed NSE at 03:16, 0.00s elapsed
Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 7.29 seconds
```

__PROBLEM__

How many services running on Hydrogencorp

__HINT__

Give me a sum of running services on hydrogencorp.

__ANSWER__

3

__PROBLEM__

On the port for file transfer service, what is the version for the application?

__HINT__

Give me the application version number. (e.g 1.2.6)

__ANSWER__

1.2.6

__PROBLEM__

What is the software name running on port 80?

__HINT__

Give me the software name running on port 80 on this host. (e.g. IIS)

__ANSWER__

nginx 1.2.1

__PROBLEM__

What is the software and version running on port 22?

__HINT__

Give me the software and version running on port 22. (e.g. ProFTPD and 1.4.5

__ANSWER__

OpenSSH and 6.0p1

__PROBLEM__

What is the software and version running on port 22?

__HINT__

Give me the software and version running on port 22. (e.g. ProFTPD and 1.4.5)

__ANSWER__

OpenSSH and 6.0p1

__PROBLEM__

Get flag1

__HINT__

Find flag1 on the host and submit the the whole content of it.

__ANSWER__

As we can see at the ftp service, we can see the flag1.txt..
went to the `ftp://192.168.0.10` through browser and we can get the content of it
flag{a173c6cb236d6fe768ad94a6df400874}

__PROBLEM__

What is the domain name of the application?

__HINT__

Find the domain name of this host. (e.g. example.com)

__ANSWER__

There are also email.txt in ftp service, we check the content and we can see the domain.
```To: John <john@hydrogen.co>
From: Alice <alice@ymail.com>
Date: 19 August 2016
Subject: Applicant for Junior System Administration

---------------------------------------------------

Dear Hiring Manager,

I interested to apply the posting job on your blog.
If I can provide you with any further information on
my background and qualifications, please let me know.

I look Forward to hearing from you. Thank you for your
consideration.

Sincerely,

Alice
alice@ymail.com
```

hydrogen.co




