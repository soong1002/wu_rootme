## PHP - preg_replace()

![image](../image/36.1.png)
start chall lên nào

![image](../image/36.2.png)

tiếp tục google cho preg_replace() thôi

![image](../image/36.3.png)
preg_replace nhận vào 3 tham số
1. pattern dùng làm biểu thức chính quy cho subject check
2. replacement sẽ thay thế chuỗi mà subject match trong pattern
3. subject để tìm xem trong pattern có chứa chuỗi mà value subject đang có hay không
![image](../image/36.4.png)

có thêm hint về `/e modifier` , nếu sử dụng \e thì nó sẽ execute php

tiến hành exploit
![image](../image/36.5.png)
![image](../image/36.6.png)

`soong1002`