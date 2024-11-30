# JavaNC-thayHa
1. Mục tiêu của hệ thống
+ Cung cấp nền tảng mua sắm trực tuyến: Cho phép người dùng duyệt sản phẩm, thêm vào giỏ hàng và thực hiện thanh toán.
+ Tạo trải nghiệm người dùng thân thiện: Giao diện dễ sử dụng, giúp người dùng dễ dàng tìm kiếm và mua sản phẩm.
2. Phạm vi hệ thống
+ Người dùng: Có thể là khách hàng không đăng ký và người dùng đã đăng ký.
+ Quản trị viên: Quản lý sản phẩm, đơn hàng và người dùng.
  
3. Yêu cầu chức năng
- Chức năng cho người dùng:
+ Đăng ký và đăng nhập.
+ Duyệt list sản phẩm.
+ Thêm sản phẩm vào giỏ hàng.
+ Xem giỏ hàng và chỉnh sửa số lượng sản phẩm.
+ thanh toán.
+ Xem lịch sử đơn hàng.

- Chức năng cho quản trị viên:
+ đăng nhập (3 lần sai --> recaptcha)
+ Quản lý sản phẩm (CRUD).
+ Quản lý đơn hàng (CRUD).
+ Quản lý người dùng (CRUD).

4. Thiết kế hệ thống
Kiến trúc hệ thống:
+ Frontend: HTML, CSS, JavaScript.
+ Backend: Sử dụng Java (Spring Boot).
+ Cơ sở dữ liệu: Sql server.
+ Mô hình dữ liệu:
Bảng sản phẩm: (ID, tên, mô tả, giá, hình ảnh).
Bảng người dùng: (ID, tên, email, mật khẩu).
Bảng đơn hàng: (ID, ID người dùng, tổng giá trị, trạng thái).

5. Quy trình hoạt động
+ Viewer truy cập trang web: Duyệt sản phẩm và thêm vào giỏ hàng.
+ User xem giỏ hàng (update số lượng/xóa sản phẩm)
+ Thanh toán: Người dùng nhập thông tin thanh toán và xác nhận đơn hàng.
+ Quản trị viên xử lý đơn hàng: Quản lý và theo dõi trạng thái đơn hàng.
6. Bảo mật
+ Xác thực người dùng: Sử dụng mã hóa mật khẩu và xác thực phiên làm việc.
+ Bảo vệ dữ liệu: Đảm bảo an toàn cho thông tin người dùng và giao dịch.
