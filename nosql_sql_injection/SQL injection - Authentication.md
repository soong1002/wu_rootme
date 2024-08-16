![image](../image/4.1.png)

start chall lên mình thấy 1 form login, theo tên của chall mình tiến hành inject cơ bản nhất của lỗi SQL injection: `admin'`

![image](../image/4.2.png))

báo lỗi systax biết nó sử dụng SQLite để truy vấn, dự đoán nó không filter character
mình truyền payload `admin'--a`

![image](../image/4.3.png))

view source là có password của admin

![image](../image/4.4.png))
`soong1002dm`







