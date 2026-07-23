# Các loại mạng máy tính
Mạng máy tính là một nhóm gồm hai hoặc nhiều máy tính và thiết bị độc lập được kết nối với nhau để chia sẻ dữ liệu, tài nguyên và dịch vụ. Các kết nối này có thể được thiết lập bằng phương tiện có dây hoặc công nghệ không dây. Các loại mạng máy tính được phân loại dựa trên một số yếu tố:

+ Khu vực địa lý
+ Phương tiện truyền dẫn
+ Quyền sở hữu và quyền truy cập

## I. Phân loại dựa trên  khu vực địa lý
Phân loại mạng máy tính theo khoảng cách vật lý hoặc khu vực mà chúng bao phủ, từ không gian cá nhân nhỏ đến các khu vực toàn cầu rộng lớn. Dựa trên khu vực địa lý, mạng máy tính chủ yếu được chia thành năm loại:

### 1.  Mạng cá nhân (Personal Area Network-PAN)

Là mạng kết nối các thiết bị cá nhân trong phạm vi rất ngắn xung quanh một người dùng duy nhất.

+ **Phạm vi phủ sóng:** 1–10 mét
+ **Các công nghệ chính:** Bluetooth, NFC, Hồng ngoại
+ **Ví dụ thực tế:** Điện thoại thông minh kết nối với tai nghe không dây.
+ **Khi nào nên sử dụng:** Để liên lạc tầm ngắn giữa các thiết bị cá nhân.

### 2. Mạng cục bộ (Local Area Network-LAN)

Là mạng kết nối các máy tính và thiết bị trong một khu vực giới hạn, chẳng hạn như nhà riêng, văn phòng hoặc tòa nhà.

+ **Phạm vi phủ sóng:** Một phòng, tòa nhà hoặc khuôn viên nhỏ.
+ **Các công nghệ chính:** Ethernet, Wi-Fi
+ **Ví dụ thực tế:** Mạng Wi-Fi tại nhà hoặc văn phòng
+ **Khi nào nên sử dụng:** Để liên lạc nhanh chóng và an toàn trong phạm vi một khu vực nhất định.

### 3. Mạng lưới khu vực khuôn viên trường (Campus Area Network-CAN)

Là mạng kết nối nhiều mạng LAN trong khuôn viên trường hoặc một nhóm các tòa nhà gần nhau.

+ **Phạm vi phủ sóng:** Khuôn viên trường đại học hoặc doanh nghiệp.
+ **Các công nghệ chính:** Ethernet, cáp quang
+ **Ví dụ thực tế:** Mạng lưới khuôn viên trường đại học hoặc doanh nghiệp
+ **Khi nào nên sử dụng:** Để kết nối các mạng LAN trong toàn khuôn viên trường thuộc cùng một tổ chức.

### 4.  Mạng lưới khu vực đô thị (Metropolitan Area Network-MAN)

Là mạng kết nối nhiều mạng lưới trong một thành phố hoặc khu vực đô thị

+ **Phạm vi phủ sóng:** Thành phố hoặc thị trấn lớn
+ **Các công nghệ chính:** Cáp quang, Vi sóng, Ethernet đô thị
+ **Ví dụ thực tế:** Mạng ISP toàn thành phố
+ **Khi nào nên sử dụng:** Để cung cấp kết nối tốc độ cao trên toàn thành phố

### 5. Mạng diện rộng (Wide Area Network-WAN)

Mạng WAN kết nối các mạng lưới trên các khu vực địa lý rộng lớn như quốc gia hoặc châu lục

+ **Phạm vi phủ sóng:** Quốc gia, châu lục hoặc toàn cầu
+ **Các công nghệ chính:** Đường truyền thuê riêng, liên kết vệ tinh, Internet
+ **Ví dụ thực tế:** Internet
+ **Khi nào nên sử dụng:** Để hỗ trợ liên lạc đường dài và toàn cầu.

## II. Phân loại dựa trên phương tiện truyền dẫn

### 1. Mạng lưới phát sóng (Broadcast Network)

Mạng này sử dụng một phương tiện truyền thông chung giữa tất cả các thiết bị được kết nối.
+ Dữ liệu được truyền từ một nút sẽ được tất cả các nút khác trong mạng nhận được.
+ Mỗi gói dữ liệu chứa một địa chỉ đích, và chỉ thiết bị được chỉ định mới xử lý nó
+ Việc giao tiếp tuân theo mô hình một-nhiều
+ Không có đường dẫn vật lý riêng biệt nào giữa người gửi và người nhận.

Ví dụ: 

+ Ethernet (dựa trên bus)
+ Mạng LAN không dây (Wi-Fi)

### 2. Mạng điểm-đến-điểm (Point to Point)
Phương pháp này sử dụng các liên kết chuyên dụng giữa các thiết bị giao tiếp.

+ Dữ liệu được truyền trực tiếp từ nút này sang nút khác.
+ Việc giao tiếp diễn ra theo mô hình một đối một.
+ Dữ liệu có thể đi qua các thiết bị trung gian (bộ định tuyến hoặc bộ chuyển mạch).
+ Cần có các thuật toán định tuyến để xác định đường đi tối ưu nhất.

Ví dụ:

+ internet
+ Mạng đường truyền thuê bao
+ Mạng điện thoại

## III. Phân loại dựa trên quyền sở hữu và quyền truy cập

### 1. Mạng riêng (Private Network)
Loại mạng này thuộc sở hữu và được quản lý bởi một cá nhân, tổ chức hoặc cơ quan.
+ Chỉ những người dùng được ủy quyền mới có thể truy cập.
+ Yêu cầu xác thực bằng các phương thức như tên người dùng, mật khẩu, VPN hoặc mã truy cập.
+ Chủ yếu được sử dụng cho giao tiếp nội bộ
+ Cung cấp mức độ bảo mật, quyền riêng tư và khả năng kiểm soát cao hơn.

Ví dụ: 
+ Mạng nội bộ công ty
+ Mạng LAN văn phòng
+ Mạng đám mây riêng

### 2. Mạng lưới công cộng (public Network)
Loại mạng này thuộc sở hữu của các nhà cung cấp dịch vụ hoặc chính quyền.
+ Dễ tiếp cận với công chúng
+ Yêu cầu rất ít hoặc không cần xác thực để kết nối
+ Cung cấp khả năng truy cập rộng rãi nhưng bảo mật thấp hơn
+ Thường được chia sẻ bởi một số lượng lớn người dùng.
+ Có thể hoạt động trên cả phương tiện có dây và không dây.

Ví dụ: 
+ internet
+ Mạng Wi-Fi công cộng
+ Mạng di động

### 3. Mạng lai (Hybrid Network)
Loại mạng này là sự kết hợp giữa mạng riêng và mạng công cộng.
+ Một số phần của mạng bị hạn chế truy cập, trong khi những phần khác có thể truy cập công khai.
+ Cho phép các tổ chức duy trì an ninh nội bộ đồng thời cung cấp khả năng kết nối bên ngoài.
+ Thường gặp trong các hệ thống doanh nghiệp và điện toán đám mây hiện đại.

Ví dụ: 
+ Mạng lưới doanh nghiệp được kết nối với Internet.
+ Mạng đám mây doanh nghiệp
+ Hệ thống ngân hàng trực tuyến

## Mạng Internet
Mạng liên kết (internetwork) là tập hợp gồm hai hoặc nhiều mạng độc lập được kết nối với nhau để hoạt động như một mạng logic duy nhất.
+ Nó cho phép giao tiếp giữa các thiết bị trên các mạng khác nhau.
+ Chính Internet là ví dụ lớn nhất về một mạng lưới liên kết
+ Nó bao gồm nhiều mạng lưới, chứ không chỉ là các máy tính riêng lẻ.
+ Sử dụng các thiết bị mạng để kết nối các mạng với nhau.

### 1. Mạng nôi bộ (Intranet)
Mạng nội bộ (intranet) là một mạng riêng được sử dụng trong phạm vi một tổ chức. Chỉ những người dùng được ủy quyền, chẳng hạn như nhân viên, mới có thể truy cập vào mạng này.
+ Thuộc sở hữu và kiểm soát bởi một tổ chức duy nhất
+ Quyền truy cập bị hạn chế bằng thông tin đăng nhập.
+ Được sử dụng cho giao tiếp và hợp tác nội bộ.
+ Cải thiện việc chia sẻ thông tin trong nội bộ tổ chức.

**Công dụng**
+ Cổng thông tin nhân viên
+ Email và tin nhắn nội bộ
+ Chia sẻ chính sách và tài liệu của công ty.
+ Các ứng dụng nội bộ (nhân sự, tiền lương, quản lý dự án)

Ví dụ:
+ Trang web nội bộ của công ty
+ Cổng thông tin khuôn viên trường đại học
+ Hệ thống nội bộ của cơ quan chính phủ

### 2. Mạng ngoại bộ (Extranet)
Extranet là phần mở rộng của intranet cho phép người dùng bên ngoài truy cập với quyền hạn chế. Nó kết nối mạng nội bộ của tổ chức với các bên ngoài đáng tin cậy.
+ Mạng riêng một phần
+ Quyền truy cập được cung cấp cho các đối tác, nhà cung cấp, nhà thầu hoặc khách hàng.
+ Yêu cầu xác thực và ủy quyền
+ Thường được triển khai bằng cách sử dụng VPN hoặc truy cập web an toàn.

**Công dụng**
+ Giao tiếp giữa doanh nghiệp với doanh nghiệp (B2B)
+ Quản lý chuỗi cung ứng
+ Cổng thông tin khách hàng
+ Nền tảng hợp tác đối tác

Ví dụ:
+ Hệ thống quản lý nhà cung cấp
+ Cổng ngân hàng trực tuyến
+ Cổng truy cập nhà cung cấp