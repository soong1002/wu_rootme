![image](../image/7.1.png)

chall cho ta 2 future, mình check qua login với các inject xem nó có báo syntax error không, có vẻ không được, mình focus vào feature còn lại

![image](../image/7.2.png)

để ý url mình thấy nó check parameter action và `news_id`
dùng burpsuite chặn bắt nào

![image](../image/7.3.png)
đúng như mình dự đoán, dính lỗi ở param news_id
okey, exploit thôi nào

![image](../image/7.4.png)
thử sai tiếp tục thay đổi số cột 
![image](../image/7.5.png)
-> nó có 3 cột trả về

![image](../image/7.6.png)
mình xem được tên bảng là `users`

![image](../image/7.7.png)
làm xong mới nhớ mình có thể dùng `sql_master`, cái này để xem lệnh tạo bảng và các cột trong nó =))

get password
![image](../image/7.8.png)

quên mất là nó filter dấu nháy `'`
google search mình chơi kiểu `group_concat` để gộp các cột lại thành 1 dòng

![image](../image/7.9.png)

Hoặc
![image](../image/7.10.png)

`soong1002khocvc`
