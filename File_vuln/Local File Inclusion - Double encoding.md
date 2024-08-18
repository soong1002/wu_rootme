![image](../image/19.1.png)
start chall lên nào
![image](../image/19.2.png)

mình focus vào các giá trị param
payload phổ thông cho tấn công về file
![image](../image/19.3.3.png)


![image](../image/19.3.png)

có thê thấy bypass được filter ../
thêm nữa nó dùng hàm `include()` rất nguy hiểm nếu hacker kiểm soát được input đầu vào mà không filter hoặc filter chưa đủ mạnh

mình thấy nó tự động thêm vào đuôi .inc.php. Đuôi inc

search content về LFI mình biết thêm về PHP Wrappers 
![image](../image/19.4.png)

oke, tiến hành exploit nào

payload:
`php://filter/convert.base64-encode/resource=home`
nhớ double encode url

![image](../image/19.5.png)
decode nó ra thôi
![image](../image/19.6.png)
có vẻ nó include thêm thằng `conf.inc.php`, thay đổi payload để đọc conf.inc.php
![image](../image/19.7.png)

done `soong1002`

