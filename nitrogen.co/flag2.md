__PROBLEM__

Get flag2

__HINT__

Find flag2.txt somewhere on the WEB SERVER. 

Most common mistake on the development site. 

Maybe need a little bruteforcing on the web server but not bruteforcing username n password.

__ANSWER__

by using dirb, we identify that there is robots.txt with `User-agent: * Disallow: /openvpn-admin/ Disallow: /flag1/`

hence using dirb on openvpn-admin, i identify that there's a git folder.. so using gitTools to extract and dump the git content..

we got the creadential.bak with the flag2 in it..

```
mysql user	: root
mysql password  : P@ssw0rd


will be commit on private repo later.

#### flag2 #####
_flag{7d86ac83800991a0d8d3c113b389e16e}_
```
