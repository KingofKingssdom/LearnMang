# I. Giao thức Http và Https

## II. Cookies 
- Là một tập tin nhỏ mà website gửi để trình duyệt lưu trữ hoặc lưu trong bộ nhớ máy tính
để trình duyệt biết bạn là ai
<br/>
Ví dụ truy cập vào webiste đó trình duyệt sẽ không biết là ai đang xem, nên khi login thì gửi dữ liệu lưu vào cookie trình duyệt sẽ biết bạn là ai và có quyền làm gì 
- Cookie được lưu trữ và gửi trong Header của giao thức Http
- HttpResponse sẽ cookie tên là Set-Cookie: và có các thông số như mang giá trị key-value như sau

|Key|Value|ý nghĩa|
|---|---|---|
|Token|mã token|Cái này là một số key và value được đưa vào để gửi đi kèm cookie do mình đặt|
|Expires|Ngày tháng theo định dạng HTTP-date:Wdy, DD Mon YYYY HH:MM:SS GMT(Ví dụ: Wed, 21 Oct 2026 07:28:00 GMT)| Thời điểm hết hạn chính xác của cookie. Sau thời gian này trình duyệt sẽ tự xóa. Nếu không có cả Expires và Max-Age, cookie sẽ biến mất khi đóng trình duyệt (Session Cookie)|
|Max-Age|Số nguyên tính bằng giây(Ví dụ: Max-Age=3600 cho 1 giờ)| Thời gian sống của cookie kể từ lúc nhận. Nếu có cả Expires và Max-Age, thì Max-Age sẽ được ưu tiên|
|Domain|Tên miền hợp lệ(Ví dụ: Domain=example.com)| Phạm vi tên miền mà cookie được phép gửi kèm theo. Nếu đặt là example.com, cookie cũng sẽ được gửi đến các subdomain như ://example.com. Nếu bỏ trống, mặc định chỉ áp dụng cho domain hiện tại (không bao gồm subdomain)|
|Path| Đường dẫn thư mục (Ví dụ: Path=/dashboard)| Phạm vi đường dẫn trên URL. Trình duyệt chỉ gửi cookie này lên nếu URL bắt đầu bằng đường dẫn đã cấu hình. Mặc định là / (toàn bộ website)|
|SameSite| Strict hoặc Lax hoặc None| Kiểm soát cookie trong các yêu cầu liên kết trang (Cross-Site) <br/> + Strict: Chỉ gửi cookie khi người dùng đang ở chính trang đó. <br/> + Lax: Gửi cookie khi chuyển hướng từ trang khác sang (mặc định của trình duyệt hiện đại). <br/> + None: Gửi trong mọi trường hợp (bắt buộc phải đi kèm thuộc tính Secure)|
|Secure| (Chỉ ghi chữ Secure, không có giá trị)| Bảo mật kết nối. Trình duyệt sẽ chỉ gửi cookie này lên qua giao thức mã hóa HTTPS, không gửi qua HTTP thường.|
|HttpOnly|(Chỉ ghi chữ HttpOnly, không có giá trị)|Bảo mật mã độc. Ngăn không cho các đoạn mã JavaScript (như document.cookie) tiếp cận cookie này, giúp chống tấn công XSS|

Ví dụ thực tế: <br/>
Set-Cookie: user_token=aB9_kL291mZ; Expires=Sat, 31 Oct 2026 00:00:00 GMT; Max-Age=172800; Domain=://example.com; Path=/cart; Secure; HttpOnly; SameSite=Lax

- HttpCookie Request sẽ có tên là Cookie: nằm trong header gửi kèm
- Đối với request thì cookie sẽ chỉ có dạng key và value gửi đi thôi
<br/>

Ví dụ thực tế:
Cookie: token=abxyzegawgag1023; theme=dark;