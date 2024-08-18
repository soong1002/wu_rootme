start chall lên
![image](../image/17.1.png)

goal: Get in the admin section
click vào admin sẽ bắt login

ae nên tìm hiểu trước về LFI hoặc path traversal vuln nhé
ở đây mình sẽ tiến hành exploit luôn

ae để ý url với parameter trong ảnh trên, mình có thế lợi dụng ../ để thoát ra khỏi thư mục làm việc hiện tại để về thư mục cha
Ở đây mình thay ../ cho `coding` vì thay cho parameter `f` nó báo lỗi như này
![image](../image/17.2.png)

câu từ khá khó để giải thích cho ae hiểu tại sao phải thay ../ vào coding mà không phải para f, đại loại ae hình dung para f không cho phép để trống là được, vì khi dùng ../ nó sẽ back ra 1 level từ folder hiện tại

![image](../image/17.3.png)
vào admin thôi
![image](../image/17.4.png)
có file index.php, mở ra đọc là lấy được password admin!
[image](../image/17.5.png)

`soong1002`
NOTE: ../





