# Chế độ truyền tải
Chế độ truyền dẫn mô tả cách dữ liệu được trao đổi giữa hai thiết bị qua kênh truyền thông. Chúng quy định liệu thông tin di chuyển theo một chiều hay cả hai chiều, và liệu các thiết bị có thể truyền dữ liệu cùng lúc hay không.

+ Xác định mô hình giao tiếp
+ Xác định vai trò người gửi và người nhận
+ Ảnh hưởng đến tốc độ và hiệu suất
+ Được sử dụng trong các hệ thống mạng và viễn thông.

## 1. Chế độ song công (simplex)
Chế độ Simplex là chế độ truyền dẫn trong đó việc giao tiếp chỉ diễn ra theo một chiều, từ người gửi đến người nhận, mà không có khả năng truyền dữ liệu ngược lại.

+ Một thiết bị chỉ đóng vai trò là bộ phát.
+ Thiết bị còn lại chỉ đóng vai trò là thiết bị thu.
+ Không hỗ trợ phản hồi hoặc xác nhận.

Ví dụ: Bàn phím và màn hình truyền thống. Bàn phím chỉ có thể nhập dữ liệu, màn hình chỉ có thể xuất dữ liệu. 

**Thuận lợi**
+ Đơn giản và dễ thực hiện
+ Chi phí lắp đặt và bảo trì thấp hơn
+ Sử dụng toàn bộ băng thông để gửi dữ liệu.
+ Thích hợp cho các ứng dụng phát sóng.

**Nhược điểm**
+ Không có báo cáo lỗi nào từ bộ thu.
+ Không phù hợp với các hệ thống tương tác
+ Không thể xác nhận giao hàng thành công.
+ Ứng dụng hạn chế trong các hệ thống liên lạc hai chiều hiện đại.

## 2. Chế độ  bán song công (Half-Duplex) 
Chế độ bán song công là chế độ truyền dẫn trong đó việc giao tiếp có thể diễn ra theo cả hai hướng, nhưng chỉ một thiết bị có thể truyền dữ liệu tại một thời điểm. Các thiết bị lần lượt gửi và nhận dữ liệu trên cùng một kênh.

+ Hỗ trợ giao tiếp hai chiều
+ Sử dụng một kênh liên lạc chung duy nhất
+ Quá trình truyền dữ liệu diễn ra luân phiên giữa các thiết bị.

Ví dụ: Máy bộ đàm, trong đó tin nhắn được gửi từng tin một và tin nhắn được gửi theo cả hai chiều. 

**Thuận lợi**
+ Linh hoạt hơn so với giao tiếp một chiều
+ Hiệu quả về chi phí so với các hệ thống song công toàn phần.
+ Sử dụng hiệu quả một kênh duy nhất
+ Thích hợp cho môi trường giao tiếp được kiểm soát.

**Nhược điểm**
+ Không thể gửi và nhận đồng thời
+ Có thể xảy ra sự chậm trễ do hệ thống truyền động theo lượt.
+ Hiệu năng giảm khi lưu lượng truy cập cao.
+ Nguy cơ va chạm nếu cơ chế điều khiển bị lỗi

## 3. Chế độ song công toàn phần (Full-Duplex)
Chế độ song công toàn phần là chế độ truyền dẫn trong đó quá trình giao tiếp diễn ra đồng thời theo cả hai hướng. Cả hai thiết bị được kết nối có thể truyền và nhận dữ liệu đồng thời mà không cần chờ đợi thiết bị kia.

+ Cho phép trao đổi dữ liệu hai chiều đồng thời.
+ Sử dụng các kênh riêng biệt hoặc băng thông được chia nhỏ
+ Thường gặp trong các hệ thống liên lạc thời gian thực

Ví dụ: Mạng điện thoại, trong đó có sự liên lạc giữa hai người thông qua đường dây điện thoại, cho phép cả hai cùng nói và nghe đồng thời. 

**Thuận lợi**
+ Tốc độ truyền dữ liệu nhanh hơn
+ Không có thời gian chờ giữa các lần truyền dữ liệu.
+ Hiệu quả giao tiếp được cải thiện
+ Thích hợp cho các ứng dụng tương tác

**Nhược điểm**
+ Chi phí lắp đặt cao hơn
+ Yêu cầu phần cứng phức tạp hơn
+ Yêu cầu băng thông lớn hơn
+ Tăng độ phức tạp của cấu hình hệ thống