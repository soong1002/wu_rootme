vào luôn vấn đề nào
![image](../image/13.1.png)

có chức năng upload file lên, chỉ cho mình up file có extension như trên, mục tiêu cần up shell để đọc file .passwd
![image](../image/13.2.png)
bypass khá cơ bản
nhưng mà =))

![image](../image/13.3.png)
mình GET thì nó méo return phpinfo =))), éo hiểu nhắm

nhưng khi mình thay đổi filename thành `a.php.png` thì 
![image](../image/13.4.png)

trôn rồi, mình dự đoán dev code lỗi do đặt extension trong 1 mảng và check mảng ở vị trí cuối là `png`, do đó bypass được. còn code php nhả ra bình thường vì nó lấy extension ở vị trí mảng 1 để xác định có cho modphp xử lí không
NOTE: lập luận trên là cá nhân mình dự đoán vì không có source code của chall nhé, sai sót là có thể xảy ra mong ae chỉ dạy mình thêm

exploit .passwd
ae upload file shell với `system($_GET[cmd])` xong truyền cho nó para cmd là được nhé
`soong1002`