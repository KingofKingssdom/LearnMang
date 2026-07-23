# Mô hình OSI
## 1. Khái niệm
- Mô hình OSI (Open Systems Interconnection) là một khung tham chiếu chuẩn giúp chuẩn hóa cách các hệ thống máy tính giao tiếp với nhau qua mạng
- Gồm 7 lớp
    + Lớp vật lý
    + Lớp liên kết dữ liệu
    + Lớp mạng
    + Lớp vận chuyển
    + Lớp phiên
    + Lớp Trình bày
    + Lớp ứng dụng

## 2. Luồng dữ liệu trong mô hình OSI
Khi chúng ta truyền thông tin từ thiết bị này sang thiết bị khác, thông tin đó sẽ đi qua 7 lớp của mô hình OSI. Đầu tiên, dữ liệu di chuyển từ lớp 7 đến lớp 1 từ phía người gửi và sau đó quay trở lại từ lớp 1 đến  lớp 7 ở phía người nhận. Dữ liệu di chuyển qua mô hình OSI theo từng bước:
+ **Lớp ứng dụng:** Các ứng dụng tạo ra dữ liệu.
+ **Lớp trình bày:** Dữ liệu được định dạng và mã hóa.
+ **Lớp phiên:** Các kết nối được thiết lập và quản lý.
+ **Lớp vận chuyển:** Dữ liệu được chia thành các phân đoạn để đảm bảo truyền tải đáng tin cậy.
+ **Lớp mạng:** Các phân đoạn được đóng gói thành các gói dữ liệu và được định tuyến.
+ **Lớp liên kết dữ liệu:** Các gói dữ liệu được đóng khung và gửi đến thiết bị tiếp theo.
+ **Lớp vật lý:** Các khung dữ liệu được chuyển đổi thành bit và truyền tải về mặt vật lý.

Ví dụ: 
Người A gửi email cho bạn mình là Người B.
+ **Bước 1:** Người A tương tác với ứng dụng email như Gmail, Outlook, v.v. Soạn email để gửi. (Điều này diễn ra ở Lớp ứng dụng).
+ **Bước 2:** Ở lớp trình bày, ứng dụng thư điện tử chuẩn bị cho việc truyền dữ liệu bằng cách mã hóa dữ liệu và định dạng dữ liệu để truyền tải.
+ **Bước 3:** Ở lớp phiên, một kết nối được thiết lập giữa người gửi và người nhận trên internet.
+ **Bước 4:** Ở lớp vận chuyển, dữ liệu email được chia thành các phân đoạn nhỏ hơn. Nó bổ sung số thứ tự và thông tin kiểm tra lỗi để duy trì độ tin cậy của thông tin.
+ **Bước 5:** Ở lớp mạng, việc định địa chỉ cho các gói tin được thực hiện để tìm ra tuyến đường tốt nhất cho việc truyền tải.
+ **Bước 6:** Ở lớp liên kết dữ liệu, các gói dữ liệu được đóng gói vào khung, sau đó địa chỉ MAC được thêm vào cho các thiết bị cục bộ và tiếp theo là kiểm tra lỗi bằng cơ chế phát hiện lỗi.
+ **Bước 7:** Ở lớp vật lý, các khung dữ liệu được truyền dưới dạng tín hiệu điện/quang qua môi trường mạng vật lý như cáp Ethernet hoặc WiFi.

Sau khi email đến tay người nhận, tức là Người B, quá trình sẽ đảo ngược và giải mã nội dung email. Cuối cùng, email sẽ hiển thị trên ứng dụng email của Người B.
