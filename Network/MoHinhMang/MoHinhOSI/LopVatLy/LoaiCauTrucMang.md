# Các loại cấu trúc mạng
Cấu trúc mạng là sự sắp xếp các thiết bị (nút) và các kết nối (liên kết) trong một mạng máy tính. Nó thể hiện cách các máy tính, máy chủ và các thiết bị khác được kết nối và cách dữ liệu truyền giữa chúng. Việc lựa chọn cấu trúc mạng phù hợp rất quan trọng vì nó ảnh hưởng đến hiệu suất, chi phí, độ tin cậy và bảo mật của mạng. Có hai loại cấu trúc mạng chính:

+ **Cấu trúc vật lý:** Cách bố trí vật lý thực tế của cáp và thiết bị.
+ **Cấu trúc logic:** Cách dữ liệu di chuyển trên mạng, bất kể bố cục vật lý.

Tất cả các cấu trúc mạng sau (Bus, Star, Mesh, Ring, Tree, Hybrid) đều là cấu trúc mạng vật lý. Cấu trúc mạng logic đề cập đến cách dữ liệu truyền trong mạng, chẳng hạn như CSMA/CD trong Ethernet hoặc truyền token trong mạng vòng.

## 1. Cấu trúc liên kết điểm-điểm (Point to Point)
Cấu trúc liên kết điểm-điểm là một loại cấu trúc liên kết hoạt động dựa trên chức năng của bên gửi và bên nhận. Đây là hình thức giao tiếp đơn giản nhất giữa hai nút, trong đó một nút là bên gửi và nút kia là bên nhận. Cấu trúc liên kết điểm-điểm cung cấp băng thông cao.

**Thuận lợi**
+ Đơn giản và dễ cài đặt
+ Tốc độ truyền dữ liệu cao (đường truyền chuyên dụng)
+ Giao tiếp an toàn (kết nối trực tiếp)
+ Xác suất xảy ra xung đột dữ liệu thấp.

**Nhược điểm**
+ Không phù hợp với mạng lưới lớn.
+ Sẽ tốn kém nếu nhiều thiết bị cần kết nối.
+ Khả năng mở rộng hạn chế
+ Lỗi kết nối làm gián đoạn liên lạc.

## 2. Cấu trúc lưới (Mesh)
Trong cấu trúc mạng lưới (mesh topology), mỗi thiết bị được kết nối với thiết bị khác thông qua một kênh cụ thể. Mỗi thiết bị được kết nối với nhau thông qua các kênh chuyên dụng. Các kênh này được gọi là các liên kết (link). Cấu trúc mạng lưới không phụ thuộc vào các giao thức cụ thể; nó tập trung vào các kết nối trực tiếp giữa các thiết bị.

Ví dụ: Giả sử có N thiết bị được kết nối với nhau theo cấu trúc mạng lưới, tổng số cổng mà mỗi thiết bị cần là
N−1.Nếu có 6 thiết bị được kết nối với nhau, do đó tổng số cổng cần thiết cho mỗi thiết bị là 5.

**Thuận lợi**
+ Quá trình truyền thông giữa các nút diễn ra rất nhanh.
+ Cấu trúc lưới (Mesh Topology) rất mạnh mẽ.
+ Lỗi được chẩn đoán dễ dàng. Dữ liệu đáng tin cậy vì dữ liệu được truyền giữa các thiết bị thông qua các kênh hoặc liên kết chuyên dụng.
+ Đảm bảo an ninh và quyền riêng tư.

**Nhược điểm**
+ Việc cài đặt và cấu hình rất khó khăn.
+ Chi phí cáp cao do cần phải đi dây số lượng lớn, do đó chỉ phù hợp với số lượng thiết bị ít.
+ Chi phí bảo trì rất cao.

## 3. Cấu trúc hình sao (star)

Trong cấu trúc mạng hình sao (Star Topology), tất cả các thiết bị được kết nối với một bộ điều khiển trung tâm (hub) thông qua cáp. Hub này là nút trung tâm và tất cả các nút khác được kết nối với nút trung tâm. Hub có thể là loại thụ động, tức là không phải hub thông minh như các thiết bị phát sóng, đồng thời cũng có thể là hub thông minh, được gọi là hub chủ động. Hub chủ động thường có các bộ khuếch đại tín hiệu (repeater) bên trong.

**Thuận lợi**
+ Nếu N thiết bị được kết nối với nhau theo cấu trúc hình sao, thì số lượng cáp cần thiết để kết nối chúng là N. Vì vậy, việc thiết lập rất dễ dàng.
+ Mỗi thiết bị chỉ cần 1 cổng để kết nối với hub, do đó tổng số cổng cần thiết là N.
+ Hệ thống rất mạnh mẽ. Nếu một liên kết bị lỗi, chỉ liên kết đó sẽ bị ảnh hưởng chứ không ảnh hưởng đến các liên kết khác.
+ Dễ dàng xác định và khoanh vùng lỗi.
Cấu trúc mạng hình sao tiết kiệm chi phí vì sử dụng cáp đồng trục giá rẻ.

**Nhược điểm**
+ Nếu bộ tập trung (trung tâm) mà toàn bộ cấu trúc mạng phụ thuộc vào bị lỗi, toàn bộ hệ thống sẽ sụp đổ.
+ Chi phí lắp đặt rất cao.
+ Hiệu suất được tính dựa trên một bộ tập trung duy nhất, tức là trung tâm điều khiển.

**Lưu ý:** Một ví dụ phổ biến về cấu trúc liên kết hình sao là mạng cục bộ (LAN) trong văn phòng, nơi tất cả các máy tính được kết nối với một bộ chia trung tâm. Cấu trúc liên kết này cũng được sử dụng trong mạng không dây, nơi tất cả các thiết bị được kết nối với một điểm truy cập không dây.

## 4. Cấu trúc mạng bus
Mạng Bus Topology là một loại mạng trong đó mọi máy tính và thiết bị mạng được kết nối với một cáp duy nhất. Nó là mạng hai chiều. Đây là kết nối đa điểm và là một cấu trúc liên kết không mạnh mẽ vì nếu đường trục chính gặp sự cố, toàn bộ cấu trúc liên kết sẽ sụp đổ. Ethernet sử dụng cấu trúc liên kết IBus chỉ sử dụng giao thức MAC CSMA/CD. TDMA, CDMA, Pure ALOHA và Slotted ALOHA chưa bao giờ được sử dụng trong Ethernet.

**Thuận lợi**
+ Nếu N thiết bị được kết nối với nhau theo cấu trúc liên kết dạng bus, thì số lượng cáp cần thiết để kết nối chúng là 1, được gọi là cáp trục chính, và cần N đường dây nhánh.
+ Cáp đồng trục hoặc cáp xoắn đôi chủ yếu được sử dụng trong các mạng dựa trên bus hỗ trợ tốc độ lên đến 10 Mbps.
+ So với các cấu trúc mạng khác, chi phí của loại cáp này thấp hơn, nhưng nó chỉ được sử dụng để xây dựng các mạng nhỏ.
+ Cấu trúc mạng bus là một công nghệ quen thuộc vì các kỹ thuật cài đặt và khắc phục sự cố đã được biết đến rộng rãi.
+ CSMA/CD là phương thức MAC duy nhất được sử dụng trong Ethernet bus truyền thống. Ethernet chuyển mạch hiện đại không sử dụng CSMA/CD vì hoạt động song công toàn phần loại bỏ các xung đột.

**Nhược điểm**
+ Cấu trúc mạng dạng bus đơn giản hơn nhiều, nhưng vẫn cần rất nhiều dây cáp.
+ Nếu cáp chung bị hỏng, toàn bộ hệ thống sẽ sụp đổ.
+ Nếu lưu lượng mạng lớn, nó sẽ làm tăng số lượng xung đột trong mạng. Để tránh điều này, nhiều giao thức khác nhau được sử dụng ở lớp MAC, được biết đến như Pure Aloha, Slotted Aloha, CSMA/CD, v.v.
+ Việc thêm thiết bị mới vào mạng sẽ làm chậm mạng.
Mức độ an ninh rất thấp.

**Lưu ý:** Một ví dụ phổ biến về cấu trúc mạng dạng bus là mạng LAN Ethernet, trong đó tất cả các thiết bị được kết nối với một cáp đồng trục hoặc cáp xoắn đôi duy nhất. Cấu trúc mạng này cũng được sử dụng trong các mạng truyền hình cáp.

## 5. Cấu trúc vòng (ring)
Trong cấu trúc liên kết vòng (Ring Topology), các thiết bị được kết nối với nhau thành một vòng tròn, mỗi vòng tròn cách nhau chính xác hai thiết bị lân cận. Một số bộ khuếch đại tín hiệu (repeater) được sử dụng cho cấu trúc liên kết vòng có số lượng nút lớn, bởi vì nếu ai đó muốn gửi dữ liệu đến nút cuối cùng trong cấu trúc liên kết vòng có 100 nút, thì dữ liệu sẽ phải đi qua 99 nút để đến được nút thứ 100. Do đó, để ngăn ngừa mất dữ liệu, các bộ khuếch đại tín hiệu được sử dụng trong mạng.

**Lưu ý:** Ở đây, dữ liệu chỉ chảy theo một chiều, nhưng có thể được chuyển đổi thành dữ liệu hai chiều bằng cách thiết lập 2 kết nối giữa mỗi nút mạng, cấu trúc này được gọi là cấu trúc liên kết vòng kép (Dual Ring Topology).

**Hoạt động**
+ Một trạm được gọi là trạm giám sát, chịu trách nhiệm toàn bộ việc thực hiện các hoạt động.
+ Để truyền dữ liệu, trạm phải giữ mã thông báo. Sau khi quá trình truyền hoàn tất, mã thông báo sẽ được giải phóng để các trạm khác sử dụng.
+ Khi không có trạm nào đang truyền dữ liệu, thì token sẽ lưu thông trong vòng tròn.

**Thuận lợi**
+ Việc truyền dữ liệu diễn ra với tốc độ cao.
+ Khả năng va chạm là tối thiểu trong loại cấu trúc liên kết này.
+ Chi phí lắp đặt và mở rộng thấp.

**Nhược điểm**
+ Sự cố của một nút mạng duy nhất có thể khiến toàn bộ mạng bị lỗi.
+ Việc khắc phục sự cố rất khó khăn trong cấu trúc mạng này.
+ Kém an toàn hơn.

## 6. Cấu trúc cây (tree)
Cấu trúc mạng dạng cây là một biến thể của cấu trúc mạng dạng sao. Cấu trúc mạng này có luồng dữ liệu theo thứ bậc. Trong cấu trúc mạng dạng cây, các giao thức như DHCP và SAC (Cấu hình tự động tiêu chuẩn) được sử dụng.

+ Tại đây, nhiều trạm trung chuyển phụ được kết nối với trạm trung tâm chứa bộ khuếch đại tín hiệu.
+ Luồng dữ liệu này diễn ra từ trên xuống dưới, tức là từ trung tâm điều khiển đến trung tâm điều khiển thứ cấp rồi đến các thiết bị, hoặc từ dưới lên trên, tức là từ các thiết bị đến trung tâm điều khiển thứ cấp rồi đến trung tâm điều khiển chính. 
+ Đây là kết nối đa điểm và là cấu trúc liên kết không ổn định vì nếu đường trục chính gặp sự cố, toàn bộ cấu trúc liên kết sẽ sụp đổ.

**Thuận lợi**
+ Nó cho phép kết nối nhiều thiết bị hơn với một trung tâm điều khiển duy nhất, do đó làm giảm khoảng cách truyền tín hiệu đến các thiết bị.
+ Nó cho phép mạng được cách ly và ưu tiên truy cập từ các máy tính khác nhau.
+ Chúng ta có thể thêm các thiết bị mới vào mạng hiện có.

**Nhược điểm**
+ Nếu bộ điều khiển trung tâm gặp sự cố, toàn bộ hệ thống sẽ ngừng hoạt động.
+ Chi phí cao là do hệ thống dây cáp.
+ Nếu thêm thiết bị mới, việc cấu hình lại sẽ trở nên khó khăn hơn.

**Lưu ý:** Một ví dụ phổ biến về cấu trúc cây là hệ thống phân cấp trong một tổ chức lớn. Giám đốc điều hành (CEO) là gốc, được kết nối với các phòng ban khác nhau (các nút con) của công ty, các nhà quản lý giám sát các nhóm khác nhau (các nút cháu) và các thành viên nhóm (các nút lá) nằm ở đáy của hệ thống phân cấp.

## 7. Cấu trúc liên kết lai (Hybrid)
Cấu trúc liên kết lai (Hybrid Topology) là sự kết hợp của tất cả các loại cấu trúc liên kết mà chúng ta đã nghiên cứu ở trên. Cấu trúc liên kết lai được sử dụng khi các nút có thể tự do tạo thành bất kỳ hình dạng nào. Điều này có nghĩa là chúng có thể là các nút riêng lẻ như cấu trúc liên kết vòng (Ring topology) hoặc cấu trúc liên kết hình sao (Star topology) hoặc có thể là sự kết hợp của nhiều loại cấu trúc liên kết khác nhau đã thấy ở trên. Mỗi cấu trúc liên kết riêng lẻ sử dụng giao thức đã được thảo luận trước đó.

**Thuận lợi**
+ Cấu trúc này rất linh hoạt.
+ Quy mô của mạng có thể dễ dàng được mở rộng bằng cách thêm các thiết bị mới.

**Nhược điểm**
+ Việc thiết kế kiến ​​trúc của Mạng lai là một thách thức.
+ Các thiết bị trung tâm (hub) được sử dụng trong cấu trúc mạng này rất đắt tiền.
+ Chi phí cơ sở hạ tầng rất cao vì mạng lai đòi hỏi rất nhiều cáp và thiết bị mạng.

**Lưu ý:** Một ví dụ phổ biến về cấu trúc mạng lai là mạng lưới khuôn viên trường đại học. Mạng lưới này có thể có trục chính dạng hình sao, với mỗi tòa nhà được kết nối với trục chính thông qua một bộ chuyển mạch hoặc bộ định tuyến. Bên trong mỗi tòa nhà, có thể có cấu trúc mạng dạng bus hoặc vòng kết nối các phòng và văn phòng khác nhau.