__PROBLEM__

we're given sure2click.apk file..

`file sure2click.apk`

```
sure2click.apk: Zip archive data, at least v2.0 to extract
```

__HINT__

get the flag (format is 47uRKr34T1f{something})

__ANSWER__

we know already that it's not using right extension file, so 

`mv sure2click.apk sure2clik.zip`

and unzip the file.. we got 

```
AndroidManifest.xml  classes.dex  META-INF  res  resources.arsc
```

`strings classes.dex | grep 47uRKr34T1f`

_Flag : 47uRKr34T1f{why_Cl1ck_Th3_Butt0n}_
