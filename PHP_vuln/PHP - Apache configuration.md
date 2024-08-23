![image](../image/30.1.png)

1 bài về `.htaccess`, ae đọc về .htaccess trước khi đọc bài này vì mình sẽ không giải thích lại
goal: đọc file `/private/flag.txt`

![image](../image/30.2.png)

nó không cho upload file .php hay gì :v càng cấm càng làm kaka

![image](../image/30.3.png)
để ý cái cookie, đó là đường dẫn path tới file mà mình upload lên, mình lợi dụng cái này có thể dính lỗi path traversal. 
tiến hành exploit

![image](../image/30.4.png)
upload .htaccess với extension .khiem sẽ được xử lí như .php

![image](../image/30.5.png)
payload file `xxx.khiem` 

và đây là kết quả
![image](../image/30.6.png)

mấy bài này mình làm qua rồi, giờ ngồi viết lại wu lên không lấy flag nữa, ae chịu khó tự ngồi viết code php lấy flag ở private/flag.txt nhé. Tks ae

`soong1002`



