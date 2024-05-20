# acti
ACTi cameras (including those using firmware version A1D-505-S2.10.03-AC) have a web application that uses the GET method to handle requests containing sensitive information such as user account names and passwords, which can be accessed through the browser's History, referrers, web logs, and other sources expose this information.

<img width="609" alt="image" src="https://github.com/W-Shaoye/acti/assets/24892698/c162cd64-86c3-4bbe-a6c8-68e3e3a5ebdb">



POC

GET /cgi-bin/cmd/system?GUEST_PREVIEW=0&ACCOUNT_ROOT=admin,XXXXXXXX&ACCOUNT_USER_1=XXXX,XXXXXXXX&ACCOUNT_USER_2=,&ACCOUNT_USER_3=,&ACCOUNT_USER_4=,&ACCOUNT_USER_5=,&ACCOUNT_USER_6=,&ACCOUNT_USER_7=,&ACCOUNT_USER_8=,&ACCOUNT_USER_9=,&ACCOUNT_USER_10=, HTTP/1.1

Host: 127.0.0.1

Authorization: Digest username="admin".........

Pragma: no-cache

Cache-Control: no-cache

User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.6367.118 Safari/537.36

Content-Type: text/plain;charset=utf-8

Accept: */*

Referer: http://127.0.0.1/setup/setup_user_user-account_level.html

Accept-Encoding: gzip, deflate, br

Accept-Language: zh-TW,zh;q=0.9,en-US;q=0.8,en;q=0.7

Cookie: User=; Pwd=; ViewSize_S1=640%2C360

Connection: close

<img width="530" alt="image" src="https://github.com/W-Shaoye/acti/assets/24892698/294343e5-6911-48b2-8109-2e9a89320be3">

