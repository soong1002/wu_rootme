![image](../image/24.1.png)
start chall lên nào, vô endpoint /key xem sao
nó nhả ra 1 list public key
![image](../image/24.2.png)

giờ hãy thử vào endpoint /auth và /admin với method POST
nó yêu cầu thêm header với giá trị JWT token

![image](../image/24.3.png)


google search mình biết rằng nó là mã hóa bất đối xứng, nghĩa là cần private key để mã hóa, còn public key để giải mã 

câu hỏi mình đặt ra: liệu có thể lừa nó mã và giải mã bằng public key không =)), nghe có vẻ không khả thi lắm, nhưng vẫn nên pentest để xem thế nào, biết đâu =))) 

đúng như dự đoán, nó sử dụng thuật toán RS256 là thuật toán bất đối xứng sử dụng 2 khóa để kí và authen
![image](../image/24.4.png)

![image](../image/24.5.png)

mình đã exploit bằng extension JWT editor trog burp suite ở 1 bài wu khác, mình để link ở [đây](https://github.com/soong1002/portswigger/blob/main/JWT/jwt_confusion_alg.md)

ở bài viết này mình sẽ dùng tool jwt_tool, ae gõ google là ra, down và chạy như mình nhé

![image](../image/24.6.png)
![image](../image/24.7.png)
![image](../image/24.8.png)

nhiều bước thế kia để chỉnh thằng username thành admin đó mà, vì nếu vào endpoint /auth rồi thêm username:admin nó sẽ méo tạo cho mình token đâu, chịu khó tí nhé ae :v

![image](../image/24.9.png)

bài này viết thì gọn nhưng chỗ sử dụng thằng tool rách việc lắm, mình ngồi mò 2 tiếng để chơi cái tool này, cayyy vc

`soong1002`


