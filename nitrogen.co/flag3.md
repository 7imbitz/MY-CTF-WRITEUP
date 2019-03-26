__PROBLEM__

Get flag3

__HINT__

Find flag3.txt somewhere on the server.

Found something on flag2 before? Used it. Thanks me later. Reminder : Do not find flag3.txt first, but find the way to get flag3.txt.

__ANSWER__

use the credential we got from flag2 for `192.168.0.11/phpmyadmin`, scroll through the db and we got the ssh cred.

`user:securessh pw:securesshpassword**123`

login to the ssh using the cred and we got flag3.txt

_flag{d41d8cd98f00b204e9800998ecf8427e}_
