__PROBLEM__

we're given [jangan spam la ngok.doc](https://github.com/Adib7/MY-CTF-WRITEUP/blob/master/aturkreatif(USIM)/jangan%20spam%20la%20ngok.doc) file..

`file jangan spam la ngok.doc`

```
jangan spam la ngok.doc: data
```

__HINT__

get the flag (format is 47uRKr34T1f{something})

__ANSWER__

`strings jangan\ spam\ la\ ngok.doc`

```
Dear Colleague ; You made the right decision when you
signed up for our club ! If you are not interested
in our publications and wish to be removed from our
lists, simply do NOT respond and ignore this mail .
This mail is being sent in compliance with Senate bill
2516 , Title 2 ; Section 308 . This is a ligitimate
business proposal ! Why work for somebody else when
you can become rich within 19 WEEKS ! Have you ever
noticed more people than ever are surfing the web plus
how long the line-ups are at bank machines . Well,
now is your chance to capitalize on this . We will
help you SELL MORE & turn your business into an E-BUSINESS
. You are guaranteed to succeed because we take all
the risk . But don't believe us ! Prof Jones of California
tried us and says "I was skeptical but it worked for
me" ! We assure you that we operate within all applicable
laws ! You will blame yourself forever if you don't
order now ! Sign up a friend and your friend will be
rich too . Thanks . Dear E-Commerce professional ,
We know you are interested in receiving red-hot news
. We will comply with all removal requests ! This mail
is being sent in compliance with Senate bill 1623 ,
Title 8 , Section 303 . This is NOT unsolicited bulk
mail . Why work for somebody else when you can become
rich inside 51 days . Have you ever noticed nobody
is getting any younger plus nearly every commercial
on television has a .com on in it . Well, now is your
chance to capitalize on this . We will help you turn
your business into an E-BUSINESS & SELL MORE . The
best thing about our system is that it is absolutely
risk free for you ! But don't believe us . Mrs Simpson
of New Mexico tried us and says "I was skeptical but
it worked for me" . We are licensed to operate in all
states ! You will blame yourself forever if you don't
order now ! Sign up a friend and you'll get a discount
of 70% . Thank-you for your serious consideration of
our offer . Dear Professional ; This letter was specially
selected to be sent to you ! If you are not interested
in our publications and wish to be removed from our
lists, simply do NOT respond and ignore this mail !
This mail is being sent in compliance with Senate bill
2316 ; Title 6 , Section 308 ! This is not a get rich
scheme ! Why work for somebody else when you can become
rich in 39 days ! Have you ever noticed nobody is getting
any younger and society seems to be moving faster and
faster . Well, now is your chance to capitalize on
this ! WE will help YOU turn your business into an
E-BUSINESS and increase customer response by 200% .
The best thing about our system is that it is absolutely
risk free for you . But don't believe us . Mr Jones
of New York tried us and says "I was skeptical but
it worked for me" . We assure you that we operate within
all applicable laws ! If not for you then for your
LOVED ONES - act now ! Sign up a friend and you'll
get a discount of 80% ! Thank-you for your serious
consideration of our offer .
```

decode using http://www.spammimic.com/ and we got the flag 

_47uRKr34T1f{SPAMtakdeLogoHalalJAKIM}_
