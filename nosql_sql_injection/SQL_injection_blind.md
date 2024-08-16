---
title: SQL_injection_blind

---

![image](../image/2.1.png)
![image](../image/2.2.png)
![image](../image/2.3.png)


tiêu đề cho ta thấy là sqli blind nên tôi thử luôn payload admin'--

pass login trả về welcome back admin! nhưng không có password để nộp bài =))), tất nhiên rồi vì là blind mà :v 

đến đây theo kinh nghiệm thôi, ae phải biết được nên làm gì tiếp theo, vì password là blind nên có thể thử với payload như sau:

`admin'and password like 'a%' --xxx`

giải thích thêm 1 chút thì a% có nghĩa là nó sẽ check nếu password bắt đầu bằng kí tự 'a' thì nó sẽ true(bypass được), còn không thì ngược lại. Nôm na là dấu % nó sẽ không quan tâm những kí tự sau nữa

ô đến đây thì ae nghĩ ra rồi chứ =))), việc cần làm bây giờ chỉ còn đơn giản là brute force password với điều kiện đúng trả về là `'Welcome back admin !'` 

Tôi rcm ae dùng intruder trong burp suite hoặc ae có thể viết script python để request.post tới, ae nên viết python nhé. luyện tập dần cho quen tay python

trick lỏ nữa cho ae là ae có thể dùng extensions copy as python trong burp suite để chuyển request sang python, chỉnh sửa 1 tí là được tool rồi.

![image](../image/2.4.png)


mất công viết thì đến tận răng cho ae luôn =))), nhưng nên tập viết trước khi xem code nhé, tks aee
