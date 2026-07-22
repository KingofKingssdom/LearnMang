# Thiết bị mạng
## I. Khái niệm
Thiết bị mạng là các thiết bị vật lý cần thiết cho việc giao tiếp và tương tác giữa các máy tính trên mạng máy tính
+ Cho phép giao tiếp bằng cách truyền và nhận dữ liệu giữa các thiết bị
+ Cho phép các thiết bị kết nối với mạng một cách hiệu quả và an toàn
+ Mở rộng phạm vi phủ sóng mạng và giải quyết các vấn đề mất tín hiệu hoặc suy giảm tín hiệu.
## II. Các thiết bị mạng
Các thiết bị mạng sẽ được chia ra theo môt hình OSI theo từng lớp 
### 1. Thiết bị nằm trên lớp vật lý
**a. Hub**

Đây là điểm kết nối trung tâm cho các thiết bị trong mạng LAN.
+ Nó nhận tín hiệu đến từ một cổng và phát tán tín hiệu đó một cách mù quáng đến tất cả các cổng khác mà không cần biết người nhận là ai.
+ Xung đột lưu lượng mạng cao và rủi ro bảo mật (mọi người đều có thể xem dữ liệu của nhau)
+ Đây là thiết bị lỗi thời, đã được thay thế bằng các thiết bị chuyển mạch (Switch).

Ví dụ
Máy tính sẽ có 1-2 cổng vật lý cắm dây mạng, nếu máy A cắm dây mạng nối vào cổng vật lý 1 của hub (thường 1 hub sẽ có 4 hoặc 8 hoặc 16 hoặc 24 cổng) thì toàn bộ dữ liệu các cổng đều nhận được và phát đi, nên các máy đang cắm chỉ cần chung 1 hub là có thể nhận được dữ liệu

**b. Repeater**

Nó tái tạo tín hiệu để mở rộng phạm vi của mạng
+ Nó nhận tín hiệu yếu (do suy hao trên các dây cáp dài), khuếch đại tín hiệu đó và phát lại.
+ Mở rộng phạm vi phủ sóng WiFi hoặc cáp Ethernet vượt quá 100 mét.

**c. Modem (Bộ điều chế - Bộ giải điều chế)**

Điều này giúp thu hẹp khoảng cách giữa dữ liệu máy tính kỹ thuật số và tín hiệu tương tự, cho phép các thiết bị kết nối với internet thông qua đường dây điện thoại, cáp hoặc cáp quang.
+ Kết nối mạng gia đình của bạn với nhà cung cấp dịch vụ Internet (ISP).
+ Chuyển đổi tín hiệu số từ máy tính của bạn thành tín hiệu tương tự cho đường dây điện thoại/cáp (Điều chế) và ngược lại (Giải điều chế).

Ví dụ: Dữ liệu chạy trên máy tính và điện thoại, ... là tín hiệu số dạng 0 1, tín hiệu này là tín hiệu ổn định kh bị nhiễu nhưng lại không truyền đi xa được và còn tín hiệu tương tự là tín hiệu sẽ truyền đi xa được nhưng dễ bị nhiễu. Modem có tác dụng như trung gian đứng ra để biến tín hiệu số từ máy tính thành tín hiệu tương tự để truyền trên dây dẫn ra nhà cung cấp mạng

### 2. Thiết bị nằm trên lớp liên kết dữ liệu

**a. Switch**

Switch là thiết bị mạng tốc độ cao dùng để kết nối các thiết bị (máy tính, máy in, máy chủ) trong mạng cục bộ (LAN).

+ Không giống như hub, switch học địa chỉ MAC của mọi thiết bị được kết nối.
+ Nó chỉ gửi dữ liệu đến cổng cụ thể mà thiết bị đích được kết nối
+ Giảm va chạm, cải thiện an ninh và tốc độ.

Ví dụ: Mỗi thiết bị đều có một card mạng kèm với một con số đia chỉ MAC duy nhất, khi dữ liệu từ máy tính A đóng gói gửi kèm với MAC đến thiết bị nhận, dữ liệu sang thì đi qua cổng vật lý switch, vì switch thông minh nó nằm ở lớp liên kết dữ liệu nên nó sẽ biết đọc được gói tin đó có địa chỉ MAC nào cần nhận nó sẽ mở port mà có kết nối đến thiết bị có địa chỉ MAC đó mà không đụng gì đến các port các của switch

Cách thực hiện thực tế

**Bước 1: Đặt IP tĩnh cho 2 máy**

Vì không có Internet (không có thiết bị Cấp IP tự động), bạn cần gán cho mỗi máy một "số nhà" nội bộ:

**1. Trên máy A**
+ Bấm phím Windows + R, gõ ncpa.cpl rồi nhấn Enter
+ Nhấp chuột phải vào biểu tượng Ethernet (Mạng dây) -> chọn Properties.
+ Nhấp kép vào dòng Internet Protocol Version 4 (TCP/IPv4).
+ Chọn Use the following IP address và nhập: 
    
    + IP address: 192.168.1.1
    + Subnet mask: 255.255.255.0 (Click chuột vào dòng này nó sẽ tự hiện)
+ Bấm OK

**2. Trên máy B**
+ Làm y hệt máy A nhưng đổi địa chỉ IP lại

    + IP address: 192.168.1.2
    + Subnet mask: 255.255.255.0

**Bước 2: Bật tính năng chia sẻ và gửi file**

**Trên máy B (Máy nhận file)**
+ Tạo một thư mục ngoài màn hình tên là FileNhan
+ Nhấp chuột phải vào thư mục FileNhan -> chọn Properties -> chọn thẻ Sharing -> bấm nút Share...
+ Chọn Everyone trong danh sách -> bấm Add -> ở cột Permission Level chọn Read/Write -> Bấm Share.

**Từ máy A (Máy gửi file):**
+ Bấm phím Windows + R, gõ: \\\192.168.1.2 (đây là địa chỉ IP của máy B) rồi nhấn Enter.
+ Màn hình sẽ hiện ra thư mục FileNhan của máy B.
+ Bạn chỉ cần copy file Word từ máy A rồi dán (Paste) vào thư mục đó là xong!

**b. Bridge**

Giúp kết nối hai phân đoạn mạng LAN riêng biệt để chúng hoạt động như một mạng duy nhất.
+ Lọc lưu lượng truy cập dựa trên địa chỉ MAC để giữ lưu lượng truy cập cục bộ trong phạm vi nội bộ, giảm tắc nghẽn.
+ Đã được thay thế phần lớn bằng các thiết bị chuyển mạch (về cơ bản là các cầu nối đa cổng).

**c. Access Point (AP)**

Đây là một thiết bị phần cứng mạng cho phép các thiết bị hỗ trợ Wi-Fi, chẳng hạn như máy tính xách tay và điện thoại thông minh, kết nối với mạng có dây.
+ Hoạt động như một cầu nối giữa các thiết bị Ethernet có dây và các thiết bị Wi-Fi không dây.
+ AP chỉ cung cấp tín hiệu Wi-Fi và không định tuyến lưu lượng truy cập hoặc gán địa chỉ IP.

Ví dụ: Access Point này bắt buộc một đầu phải nhận vào một tín hiệu là có dây, trong thực tế sử dụng là có tòa nhà rộng 4 lầu. Router phát Wi-Fi thì lầu 1 và lầu 2 dùng tốt nhưng lên lầu 3 và 4 thì yếu. Sử dụng Access Point này đặt ở lầu 3 đi dây từ router nối vào nó và từ đó lầu 3 và 4 có Wi-Fi mạnh mà kh bị rào cản
đia hình

## 3.Thiết bị nằm trên lớp mạng

Các thiết bị này hoạt động với địa chỉ IP (địa chỉ logic) và kết nối các mạng khác nhau với nhau.

**a. Router (bộ định tuyến)**

Đây là một thiết bị mạng kết nối nhiều mạng với nhau và định hướng các gói dữ liệu giữa chúng bằng cách sử dụng địa chỉ IP
+ Nó sử dụng địa chỉ IP để xác định đường dẫn tốt nhất cho các gói dữ liệu.
+ Nó duy trì một Bảng Định tuyến để đưa ra những quyết định này.

Ví dụ:

    - Kết nối nhiều mạng với nhau và định hướng các gói dữ liệu giữa chúng"
    + Bản chất: Nhà bạn có nhiều thiết bị (điện thoại, laptop, tivi) kết nối lại thành 1 Mạng nội bộ (LAN). Internet bên ngoài là 1 Mạng diện rộng (WAN) khác.
    + Hai mạng này dùng "ngôn ngữ" và quy tắc quản lý khác nhau. Laptop của bạn không thể tự nối thẳng ra Google được
    + Vai trò của Router: Nó đứng ở giữa, một tay nắm mạng nhà bạn, một tay nắm mạng Internet. Khi bạn bấm xem một video Youtube, Router nhận "gói dữ liệu" yêu cầu từ laptop của bạn, kiểm tra xem nó muốn đi đâu, rồi chuyển tiếp gói dữ liệu đó sang mạng Internet

    - Sử dụng địa chỉ IP để xác định đường dẫn tốt nhất
    + Mỗi trang web (Google, Facebook) hay mỗi thiết bị trong nhà bạn đều có một địa chỉ IP riêng
    + Khi bạn gửi dữ liệu đi, gói tin sẽ dán nhãn: Địa chỉ Nguồn (IP nhà bạn) -> Địa chỉ Đích (IP của server Google)
    + Router đọc địa chỉ IP đích này, tính toán các tuyến đường cáp quang trên thế giới xem đường nào đang trống, đường nào ngắn nhất để đẩy gói tin đi theo đường nhanh nhất

    - Nó duy trì một Bảng Định tuyến (Routing Table) để đưa ra quyết định
    + Bảng định tuyến (Routing Table) giống như một "Cuốn bản đồ chỉ đường" hay "Bảng hướng dẫn chuyến xe" được lưu bên trong bộ nhớ của Router
    + Bảng này ghi rõ các quy tắc dạng
        => Nếu gói tin muốn đến địa chỉ IP của Google -> Đẩy qua cổng dây cáp Viettel/FPT.
        => Nếu gói tin muốn đến địa chỉ IP 192.168.1.5 (Máy in trong nhà) $\to$ Đẩy sang cổng LAN số 2
    + Nhờ có bảng này, Router không phải "suy nghĩ lại từ đầu" mỗi khi có một gói tin chạy qua, giúp mạng đạt tốc độ cực nhanh

    -Bộ định tuyến chặn lưu lượng phát sóng (Broadcast), cô lập các mạng với nhau
    + Router chặn lại như thế nào? Router đóng vai trò như một "Bức tường cách âm":
        => Mọi tiếng "la lớn" (Broadcast) nội bộ ở nhà bạn chỉ chạy quẩn quanh trong nhà bạn. Khi chạm tới Router, Router sẽ chặn đứng lại (Drop), không cho tràn ra ngoài Internet.
        => Nhờ vậy, mạng nhà bạn được "cô lập" an toàn, bảo mật, và mạng Internet ngoài kia cũng không bị quá tải.
