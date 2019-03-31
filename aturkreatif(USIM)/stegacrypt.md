__PROBLEM__

we're given Whoami.jpg file..

`file Whoami.jpg`

```
Whoami.jpg: JPEG image data, JFIF standard 1.01, aspect ratio, density 1x1, 
segment length 16, baseline, precision 8, 647x404, components 3
```

__HINT__

get the flag (format is 47uRKr34T1f{something})

__ANSWER__

`strings Whoami.jpg`

```
JFIF
"!&+7/&)4)!"0A149;>>>%.DIC<H7=>;
;("(;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
$3br
%&'()*456789:CDEFGHIJSTUVWXYZcdefghijstuvwxyz
        #3R
&'()*56789:CDEFGHIJSTUVWXYZcdefghijstuvwxyz
&p2i
Gz`8c=h8
SNORi@
dPE)
r=hq
h,rF(c
....cont..
```

`steghide extract -sf Whoami.jpg`

`passphrase:` _caesar_

`wrote extracted data to "s3cret.txt".`

open s3cret.txt containing `opnzop esp glwfp "yoo1fvejxkcfxhk7okydjkmex190xq9kykyyypyjpil3qb==" lyo rpe esp qwlr`

paste it on https://learncryptography.com/tools/caesar-cipher we got 

`decode the value "ndd1uktymzrumwz7dznsyzbtm190mf9znznnnenyexa3fq==" and get the flag`

decode it using base64 and we got nothing.. hahahahah
