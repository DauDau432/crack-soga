# Crack-Soga full việt hóa

# Cài đặt 
```
bash <(curl -Ls https://raw.githubusercontent.com/DauDau432/crack-soga/main/install.sh)
```
# Cấu hình soga
```   
vi /etc/soga/soga.conf
```
Sau đây là các thông số cấu hình chi tiết, có thể được sửa đổi theo tài liệu tham khảo sau

Vui lòng làm theo hướng dẫn tương ứng để cấu hình: https://github.com/sprov065/soga/wiki
```
type = v2board # Cái này là bắt buộc
server_type = v2ray # Cái này là bắt buộc
api = webapi # webapi hoặc db, cho biết docking webapi hoặc docking cơ sở dữ liệu

webapi_url = https: //www.xxxx.com/ # Đây là địa chỉ bảng điều khiển để điền vào đế cắm
webapi_mukey = xxxxxx # Đây là chìa khóa để giao tiếp giữa bảng điều khiển V2board và máy chủ

db_host = db.xxxx.com # địa chỉ cơ sở dữ liệu         
db_port = 3306 # cổng cơ sở dữ liệu
db_name = 123 # tên cơ sở dữ liệu
db_user = 123 # tên người dùng cơ sở dữ liệu
db_password = 123456 # Mật khẩu cơ sở dữ liệu

node_id = 8 # Điền vào bảng để thêm số ID tương ứng với nút
soga_key = # Khóa ủy quyền, không cần điền vào phiên bản cộng đồng, hỗ trợ tối đa 88 người dùng, phiên bản thương mại không giới hạn

cert_domain = x5.test.com # tls được sử dụng ở đây, sử dụng tên miền của ứng dụng chứng chỉ   (nếu tls không được sử dụng, dòng này có thể bị xóa) 
cert_mode = http # ứng dụng chế độ    (nếu tls không được sử dụng, dòng này có thể được xóa) 
cert_key_length = ec-256 # Để trống để đăng ký chứng chỉ RSA, điền vào ec-256 hoặc ec-384 để đăng ký chứng chỉ ECC (nếu TLS không được sử dụng, dòng này có thể bị xóa)

user_conn_limit = 0 # Giới hạn số lượng kết nối của người dùng, 0 có nghĩa là không giới hạn, v2board là bắt buộc! ! !
user_speed_limit = 0 # Giới hạn tốc độ người dùng, 0 có nghĩa là không giới hạn, tính bằng Mbps, v2board là bắt buộc! ! !
check_interval = 100 # Khoảng thời gian (giây) để đồng bộ hóa người dùng giao diện người dùng và thông tin máy chủ báo cáo, giá trị gần đúng

force_close_ssl = false # Đặt thành true để buộc đóng tls, ngay cả khi giao diện người dùng mở tls, soga sẽ không mở tls, điều này thuận tiện cho người dùng sử dụng nginx, caddy, v.v.
Cấm_bit_torrent = true # Đặt thành true để tắt tải xuống torrent

default_dns = 8.8.8.8,1.1.1.1 # Định cấu hình dns mặc định, nơi bạn có thể định cấu hình dns để mở khóa phương tiện truyền trực tuyến, được phân tách bằng dấu phẩy
```
# Hướng dẫn crack
tại ô `soga_key = # Khóa ủy quyền`
- nếu các bạn muốn dùng bản cộng đồng thì k cần điền vào ô này, nó sẽ như bản gốc và giới hạn 88 người dùng
- nếu các bạn muốn sử dụng bản thương mại, không giới hạn giới dùng thì điền kí tự bất kì vào rồi khởi động lại `soga`

# Tài liệu
[V2board bảng điều khiển v2ray hướng dẫn gắn nút phụ trợ phương pháp cấu hình tập lệnh soga](https://ivpsr.com/235.html)

[Cài đặt phụ trợ SOGA](https://v2rayn.net/19.html)

[Cách bẻ khóa chương trình phụ trợ soga](https://www.rman.top/2021/02/07/crack-soga/)
