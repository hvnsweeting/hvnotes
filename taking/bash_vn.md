BASH
=====
The shell is a command interpreter.

Bash là tên của 1 Linux shell, đồng thời cũng là 1 script language.

Bash là phiên bản cải tiến của sh.
Các linux shell được đánh giá có tính năng tốt hơn bash là zsh và fish (vd như khả năng auto complete của zsh ngon hơn của bash nhiều :D, fish thì tớ chưa dùng).

Script languages
-----
Bash được đặt tên ngang hàng cùng với các script language khác như python, ruby, perl, tcl, javascript, lua.

Bash scripting 
-----
Bash có 1 ưu điểm vượt trội hơn cả so với các ngôn ngữ còn lại đó là tính phổ biến. Nó có mặt ở mọi hệ điều hành UNIX/linux/bsd

Bash for sysadmin
-----
Không có các khái niệm lập trình như OOP, không có các cấu trúc dữ liệu xịn như array, list, dict. Bash đơn giản chỉ là 1 ngôn ngữ đóng vai trò glue code (kết dính các chương trình lại). 
* Bash cung cấp cú pháp để điều khiển chương trình (while for if else switch) và xử lý logic.
* Gọi các chương trình command line 1 cách trực tiếp, pipeline luồn dữ liệu từ chương trình này sang chương trình khác. 
* Đọc ghi file dễ dàng. 

Có thể so sánh đơn giản với các ngôn ngữ khác, bạn sẽ thấy bash có những thứ mà mọi ngôn ngữ khác đều có. Ưu điểm lớn nhất của nó có lẽ là khả năng gọi các chương trình khác trực tiếp và khả năng pipeline output của chương trình này làm input của chương trình khác một cách dễ dàng.

Bash for programmer
-----
Khi các bash script chủ yếu phục vụ mục đích tự động hóa các công việc lặp lại nhàm chán, bash không phải 1 ngôn ngữ hỗ trợ cho việc tạo ra các chương trình lớn, có kiến trúc phức tạp.

No programming language is perfect. There is not even a single best language; there are only languages well suited or perhaps poorly suited for particular purposes.

--Herbert Mayer

When to use bash?
-----
và bash rất hợp để viết nhanh các script nhỏ/ vừa, logic không quá phức tạp.

một hướng sử dụng bash khác là để prototype 1 chương trình phức tạp. Định hướng rõ ràng hơn cho lập trình viên về chương trình định viết. Sau đó, chương trình sẽ được viết lại bằng 1 ngôn ngữ khác như python, c , c++, java, perl...

When not?
-----
link này chứa 1 loạt các trường hợp không nên dùng bash
http://tldp.org/LDP/abs/html/why-shell.html

Compare Bash, Python, TCL for scripting
-----

