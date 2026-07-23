# Mô hình TCP/IP
## 1. Khái niệm
Mô hình TCP/IP là một khung mạng phân lớp giải thích cách dữ liệu được truyền giữa các thiết bị trên mạng bằng cách sử dụng các giao thức tiêu chuẩn để đảm bảo truyền tải đáng tin cậy và hiệu quả.

+ Được định nghĩa là kiến ​​trúc bốn lớp bao gồm các lớp Ứng dụng, Vận chuyển, Internet và Truy cập mạng.
+ Được tiêu chuẩn hóa bởi RFC 1122, trong đó quy định cấu trúc và hoạt động của nó.
+ Đơn giản và thiết thực hơn so với mô hình OSI bảy lớp.
+ Nó đóng vai trò là khung sườn cốt lõi của Internet hiện đại và các hệ thống mạng.

## 2. Nguyên lý hoạt động
Nguyên lý hoạt động của TCP/IP

**Khi gửi dữ liệu (Từ người gửi đến người nhận)**
+ **Lớp ứng dụng:** Phần mềm của người dùng (như trình duyệt web hoặc ứng dụng email) tạo ra dữ liệu và chuyển tiếp dữ liệu đó đến lớp tiếp theo.
+ **Lớp vận chuyển:** Dữ liệu được chia thành các phân đoạn, và TCP hoặc UDP sẽ thêm thông tin điều khiển để đảm bảo việc truyền tải đáng tin cậy hoặc tốc độ truyền nhanh.
+ **Lớp Internet:** Mỗi phân đoạn được đóng gói vào các gói dữ liệu có địa chỉ IP để có thể được định tuyến qua mạng đến thiết bị đích.
+ **Lớp truy cập mạng (lớp liên kết):** Các gói dữ liệu được chuyển đổi thành các khung phù hợp với mạng vật lý (Ethernet, Wi-Fi) và được truyền qua cáp hoặc tín hiệu không dây.

**Khi nhận dữ liệu (tại đích đến)**
+ **Lớp truy cập mạng:** Các khung dữ liệu được nhận từ phương tiện vật lý và được kiểm tra lỗi.
+ **Lớp Internet:** Các khung dữ liệu được giải nén để trích xuất các gói tin và sử dụng địa chỉ IP để đảm bảo chúng đến đúng thiết bị.
+ **Lớp vận chuyển:** Các phân đoạn được lắp ráp lại thành thông điệp gốc, và mọi dữ liệu bị thiếu hoặc bị hỏng sẽ được sửa chữa (nếu sử dụng TCP).
+ **Lớp ứng dụng:** Toàn bộ dữ liệu được chuyển đến ứng dụng của người dùng (ví dụ như trình duyệt hiển thị trang web hoặc ứng dụng email hiển thị tin nhắn).