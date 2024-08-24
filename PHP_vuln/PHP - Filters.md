![image](../image/31.1.png)

một bài về filter, có lẽ nhiều thứ phải bypass
start chall lên trước đã

![image](../image/31.2.png)
phải login mới xem được file, để ý ở url có para `inc` để include file, mình thử inject `../`

![image](../image/31.3.png)

nó đang sử dụng `open_basedir` để giới hạn mình truy cập vào các file ngoài thư mục nó cho phép

mình suy nghĩ tới wrappers vì nó có thằng `php://filter`, thử truyền payload này vô xem
`php://filter/convert.base64-encode/resource=login.php`

![image](../image/31.4.png)
decode base64 thôi

![image](../image/31.5.png)
nó lại include tiếp `config.php`, mình đọc tiếp config.php

![image](../image/31.6.png)
và đây là password admin

`soong1002`
