# Lớp vật lý (Physical Player)
## 1. Khái niệm
Lớp vật lý là lớp thấp nhất trong mô hình OSI, chịu trách nhiệm truyền tải các bit dữ liệu thô thông qua phần cứng mạng vật lý.

+ Xử lý việc truyền dữ liệu vật lý và điện.
+ Bao gồm dây cáp, đầu nối, phích cắm và bộ thu.
+ Truyền tải dữ liệu thô giữa các thiết bị.
+ Xác định các tiêu chuẩn phần cứng và các loại tín hiệu.

## 2. Chức năng của lớp vật lý
+ Lớp vật lý chịu trách nhiệm gửi dữ liệu thô dưới dạng bit qua môi trường vật lý.
+ Nó chuyển đổi dữ liệu thành tín hiệu có thể truyền qua dây dẫn, cáp quang hoặc kênh không dây (mã hóa) và chuyển đổi các tín hiệu này trở lại thành dữ liệu tại bộ thu (giải mã).
+ Nó đảm bảo tín hiệu được truyền tải chính xác và sử dụng các kỹ thuật như điều chế để chuẩn bị dữ liệu cho việc truyền tải và giải điều chế để thu hồi dữ liệu ở đầu bên kia.
+ Lớp này cũng quyết định cách dữ liệu truyền tải (một chiều, hai chiều luân phiên hoặc đồng thời) thông qua các chế độ truyền dẫn và kiểm soát tốc độ cũng như thời gian truyền dữ liệu để đảm bảo mọi thứ hoạt động trơn tru.
## 3. Cấu trúc vật lý
Cấu trúc mạng vật lý mô tả cách bố trí vật lý của các thiết bị và cáp trong mạng. Dưới đây là các cấu trúc mạng khác nhau được sử dụng trong mạng máy tính.

**Cấu hình đường dây**
+ **Cấu hình điểm-đến-điểm:** Trong cấu hình điểm-đến-điểm, có một đường truyền (liên kết) được dành riêng hoàn toàn để truyền dữ liệu giữa hai thiết bị.
+ **Cấu hình đa điểm:** Trong cấu hình đa điểm, có một đường dây (liên kết) thông qua đó nhiều thiết bị được kết nối.
## 4. Các giao thức ở lớp vật lý
Thông thường, lớp vật lý là sự kết hợp giữa lập trình phần cứng và phần mềm. Nó bao gồm một số giao thức kiểm soát việc truyền dữ liệu trên mạng. Sau đây là một số ví dụ về các giao thức lớp 1:

+ **Ethernet (IEEE 802.3):** Được sử dụng rộng rãi cho các mạng có dây.
+ **Wi-Fi (IEEE 802.11):** Dùng để liên lạc không dây.
Bluetooth (IEEE 802.15.1) : Giao tiếp không dây tầm ngắn.
+ **USB (Universal Serial Bus):** Dùng để kết nối các thiết bị ở khoảng cách ngắn.

## 5. Sự cần thiết của lớp vật lý trong bảo mật
Trong bảo mật, lớp vật lý đóng vai trò thiết yếu vì nhiều cuộc tấn công có thể xảy ra trước khi bất kỳ phần mềm nào được kích hoạt. Các mối đe dọa ở cấp độ này nhắm vào phần cứng hoặc phương tiện truyền dẫn thực tế.

+ **Nghe lén cáp:** Tin tặc có thể chặn dữ liệu bằng cách kết nối trực tiếp với cáp mạng.
+ **Truy cập vật lý:** Nếu ai đó vào phòng máy chủ hoặc khu vực phần cứng mà không được phép, họ có thể đánh cắp hoặc làm hỏng thiết bị.
+ **Chặn tín hiệu không dây:** Kẻ tấn công có thể thu tín hiệu Wi-Fi từ bên ngoài bằng các công cụ đặc biệt.
+ **Thao túng phần cứng:** Ai đó có thể can thiệp vào các thiết bị vật lý như bộ định tuyến hoặc cổng USB để bí mật cài đặt phần mềm độc hại.

## 6. Ứng dụng
+ Nó đảm bảo các thiết bị có thể truyền và nhận dữ liệu thô qua các phương tiện vật lý.
+ Nó cung cấp các tiêu chuẩn chung cho cáp, đầu nối và tín hiệu, đảm bảo khả năng tương thích.
+ **Hỗ trợ nhiều loại phương tiện:** Hoạt động với cả công nghệ có dây (ví dụ: Ethernet) và không dây (ví dụ: Wi-Fi).