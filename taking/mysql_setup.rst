Cài đặt
=====
apt-get install mysql-server mysql-client

Tạo user
=====
Tên của user phải trùng với tên 1 user trên server của bạn

Dùng PHPMyadmin

Chọn mục "privileges" ->  Add a new User
Điền vào các ô:
User name: điền 1 user giống 1 user trên server của bạn
Host: chọn local

Phần Database for user
Chọn 
Grant all privileges on wildcard name (username\_%) để người dùng có thể tạo database với prefix là user của họ.

Bấm create User -> Xong 

Dùng dòng lệnh:

gõ 
mysql -u root -p
__gõ pass__

CREATE USER 'tester'@'localhost' IDENTIFIED BY 'password_cua_ban';

GRANT USAGE ON * . * TO 'tester'@'localhost' IDENTIFIED BY '***' WITH MAX_QUERIES_PER_HOUR 0 MAX_CONNECTIONS_PER_HOUR 0 MAX_UPDATES_PER_HOUR 0 MAX_USER_CONNECTIONS 0 ;

GRANT ALL PRIVILEGES ON `tester\_%` . * TO 'tester'@'localhost';


