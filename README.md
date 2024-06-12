
# Kiểm tra hiệu năng trang web W3Schools Online Web Tutorials
Tạo một User (Thread Group). Ở User sẽ xác định số lượng người dùng ảo (threads), thời gian khởi động (ramp-up period) và số lần lặp lại (loop count) cho lần thử nghiệm.
Tiếp theo, trong User, thêm một HTTP để xác định các yêu cầu HTTP sẽ được gửi tới trang web. Đặt "Server Name or IP" là "www.w3schools.com" và "Path" là "/" để gửi yêu cầu tới trang chủ.
<img width="960" alt="Screenshot 2024-05-30 093420" src="https://github.com/NTHong0242/jmeter/assets/96609863/2cf7a7ab-15ca-4a5b-9063-ebdc2991e895">
# Kiểm tra hiệu năng API
Lựa chọn một API đơn giản là API thời tiết.
GET đến API thời tiết "api.weatherapi.com/v1/current.json" với 2 tham số: "key" và "q". Tham số "key" chứa khóa "API key" và tham số "q" chứa tên thành phố "London".
<img width="960" alt="Screenshot 2024-06-02 001927" src="https://github.com/NTHong0242/jmeter/assets/96609863/1e395395-0be3-4297-896b-bded8559d086">
Cài đặt User (Thread Group) để thực hiện kiểm tra hiệu suất của API với 4 người dùng giả lập, thời gian khởi động trong  giây và mỗi người dùng thực hiện các yêu cầu 2 lần.
<img width="960" alt="Screenshot 2024-06-02 002143" src="https://github.com/NTHong0242/jmeter/assets/96609863/2741dac4-1b9f-461b-8ea8-99a60aedd04c">
Tạo Response Assertion để kiểm tra mã phản hồi của API.
Nếu Response Code bằng 200 thì yêu cầu thực hiện thành công, còn nếu không thì yêu cầu thực hiện thất bại.
<img width="960" alt="Screenshot 2024-06-02 002355" src="https://github.com/NTHong0242/jmeter/assets/96609863/a285fbe6-ff77-4e5e-91fe-1b0a7b3f0c9a">


Phân tích kết quả kiểm tra:
    Tên: User 1-1
    Thời gian tải:670ms.
    Thời gian kết nối: 305 ms.
    Độ trễ: 654 ms.
    Kích thước: 1459 byte.
    Byte đã gửi: 179 byte.
    Kích thước tiêu đề: 652 byte.
    Kích thước nội dung: 807 byte.
    Số lương mẫu: 1.
    Đếm lần lỗi: 0.
    Loại dữ liệu ("text"|"bin"|""): text.
    Mã phản hồi: 200.
    Thông báo phản : OK.
<img width="960" alt="Screenshot 2024-06-02 003037" src="https://github.com/NTHong0242/jmeter/assets/96609863/6e4b940a-bc6f-4610-81f3-d7704fe0e034">

So sánh hiệu năng của hai trang web hoặc API:
<img width="960" alt="Screenshot 2024-06-02 004318" src="https://github.com/NTHong0242/jmeter/assets/96609863/dbcbd21f-41e1-4429-9f7b-50e5f29edc81">



