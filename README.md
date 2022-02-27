# Crack-Soga version 2.0.6 full việt hóa
Phiên bản crack của chương trình phụ trợ soga v2ray

> Phiên bản crack có thể có nhiều rủi ro không xác định khác nhau. Vui lòng sử dụng nó sau khi nhận định của riêng bạn. Tôi không chịu trách nhiệm về các hậu quả khác nhau của việc sử dụng phần mềm này.
 
 Chỉ hack cho vui thôi, dự án này sẽ vĩnh viễn ngừng cập nhật, mong các bạn ủng hộ bản chính chủ, hãy chú ý theo dõi XrayR trong thời gian tới
 
[XrayR là một khung công tác back-end dựa trên Xray mã nguồn mở và miễn phí, hỗ trợ các giao thức V2ay, Trojan, Shadowsocks, cực kỳ dễ mở rộng và hỗ trợ kết nối nhiều bảng điều khiển](https://github.com/XrayR-project/XrayR)

Phiên bản này là phiên bản crack bẩn, các bạn tự học cách sử dụng, mong các bạn ủng hộ phiên bản gốc

[soga backend là một chương trình phụ trợ hỗ trợ v2ray, Trojan, Shadowsocks cùng lúc, phiên bản cộng đồng hỗ trợ tối đa 88 người dùng và tối ưu hóa việc sử dụng bộ nhớ lâu dài.](https://github.com/sprov065/soga)

# ~~Crack địa chỉ tải xuống tệp nhị phân: [release](https://github.com/RManLuo/crack-soga-v2ray/releases)~~

## LÀM THẾ NÀO ĐỂ CRACK

[Cách bẻ khóa chương trình phụ trợ soga](https://www.rman.top/2021/02/07/crack-soga/)

## Cài đặt 
```
bash <(curl -Ls https://raw.githubusercontent.com/DauDau432/crack-soga/main/install.sh)
```
## Đồng bộ thời gian 

Nút v2ray cần được đồng bộ hóa thời gian. Nếu thời gian quá khác với thời gian của máy khách, kết nối sẽ không thể thực hiện được.

- CentOS 
```
yum install -y ntp
systemctl enable ntpd
ntpdate -q 0.rhel.pool.ntp.org
systemctl restart ntpd
```
- Debian / Ubuntu
```
apt-get install -y ntp
systemctl enable ntp
systemctl restart ntp
```
## Cấu hình soga
```   
vi /etc/soga/soga.conf
```
Sau đây là các thông số cấu hình chi tiết, có thể được sửa đổi theo tài liệu tham khảo sau

Vui lòng làm theo hướng dẫn tương ứng để cấu hình: https://github.com/sprov065/soga/wiki

Điền đầy đủ những dòng dưới đây:
```
type = v2board                      # Cái này là bắt buộc
server_type = v2ray                 # Cái này là bắt buộc
node_id = 8                         # Điền vào bảng để thêm số ID tương ứng với nút
soga_key =                          # Khóa ủy quyền, không cần điền vào phiên bản cộng đồng, hỗ trợ tối đa 88 người dùng, phiên bản thương mại không giới hạn
webapi_url = https: //www.xxxx.com/ # Đây là địa chỉ bảng điều khiển để điền vào đế cắm
webapi_mukey = xxxxxx               # Đây là chìa khóa để giao tiếp giữa bảng điều khiển V2board và máy chủ
cert_mode = http                    # ứng dụng chế độ (nếu tls không được sử dụng, dòng này có thể được xóa)
cert_domain = x5.test.com           # IP VPS
default_dns = 8.8.8.8,1.1.1.1       # Định cấu hình dns mặc định, nơi bạn có thể định cấu hình dns để mở khóa phương tiện truyền trực tuyến, được phân tách bằng dấu phẩy
```
# Hướng dẫn bẻ khóa

- phiên bản cộng đồng sẽ giới hạn 88 người dùng
- phiên bản thương mại, không giới hạn người dùng
## Các vấn đề đã biết

Phiên bản này không phải là một bản crack hoàn chỉnh và sẽ có quá trình khởi động lại trong chu kỳ từ nửa giờ đến 1 ngày. Vui lòng xem xét cẩn thận tác động của sự cố này.

## cho phép bẻ khóa

Để kích hoạt phiên bản crack, bạn chỉ cần nhập một ký tự bất kỳ tại dòng `soga_key = # Khóa ủy quyền`, nếu để trống thì đó là phiên bản cộng đồng gốc.

# Tài liệu
- [V2board bảng điều khiển v2ray hướng dẫn gắn nút phụ trợ phương pháp cấu hình tập lệnh soga](https://ivpsr.com/235.html)
- [Cài đặt phụ trợ SOGA](https://v2rayn.net/19.html)

# Video demo
[Tại đây](https://youtu.be/3mNSUUpBiMY)
