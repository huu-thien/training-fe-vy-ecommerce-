# Yêu cầu dự án Front-End: Website Thương Mại Điện Tử

## Mô tả chung
Website thương mại điện tử cho phép người dùng mua hàng và admin quản lý các chức năng liên quan đến sản phẩm, người dùng và doanh thu. Website sẽ có giao diện đẹp mắt, dễ sử dụng và trải nghiệm mượt mà. Backend sẽ được giả lập bằng `json-server` để cung cấp dữ liệu tạm thời cho ứng dụng.

## Công nghệ sử dụng
- **React** / **Next.js** (framework React)
- **TypeScript**
- **CSS** (hoặc **Tailwind CSS** để dễ dàng tạo giao diện đẹp mắt)
- **json-server** để fake dữ liệu backend

## Các tính năng yêu cầu

### 1. Giao diện người dùng (User Interface)
- **Giao diện đẹp mắt**, thân thiện và dễ sử dụng.
- **Responsive design**: Tương thích với tất cả các loại thiết bị (PC, tablet, mobile).
- Màu sắc, font chữ và bố cục được lựa chọn để tạo cảm giác chuyên nghiệp và hiện đại.

### 2. Tính năng cho người mua hàng
- **Đăng ký tài khoản**:
  - Người dùng có thể tạo tài khoản mới với các thông tin cơ bản: Tên, email, mật khẩu.
- **Đăng nhập**:
  - Người dùng có thể đăng nhập vào tài khoản đã tạo.
  - Xử lý xác thực (Validation) và hiển thị thông báo lỗi nếu thông tin không chính xác.
- **Tìm kiếm sản phẩm**:
  - Cung cấp thanh tìm kiếm để người dùng tìm sản phẩm theo tên hoặc mô tả.
  - Tìm kiếm nhanh qua API giả lập từ `json-server`.
- **Lọc sản phẩm**:
  - Cho phép lọc sản phẩm theo các tiêu chí như: Giá, danh mục sản phẩm, đánh giá, v.v.
- **Xem chi tiết sản phẩm**:
  - Người dùng có thể xem thông tin chi tiết của từng sản phẩm: hình ảnh, mô tả, giá, thông tin bổ sung, và các đánh giá.
- **Đặt hàng**:
  - Người dùng có thể chọn sản phẩm, thêm vào giỏ hàng và tiến hành đặt hàng.
- **Thanh toán**:
  - Giả lập quá trình thanh toán và hiển thị thông báo khi giao dịch hoàn tất.
- **Lịch sử mua hàng**:
  - Người dùng có thể xem lại các đơn hàng đã đặt trong quá khứ.
- **Bình luận sản phẩm**:
  - Cho phép người dùng viết bình luận, đánh giá sản phẩm đã mua.

### 3. Tính năng cho Admin
- **Quản lý doanh thu**:
  - Admin có thể xem tổng doanh thu của cửa hàng theo ngày, tuần, tháng.
- **Quản lý danh mục sản phẩm**:
  - Admin có thể tạo, sửa, xoá các danh mục sản phẩm (Ví dụ: điện thoại, laptop, giày dép, v.v).
- **Quản lý sản phẩm**:
  - Admin có thể thêm mới, sửa đổi hoặc xóa các sản phẩm. Mỗi sản phẩm sẽ có thông tin như tên, mô tả, giá, ảnh, danh mục.
- **Quản lý người dùng**:
  - Admin có thể xem danh sách người dùng, sửa đổi thông tin người dùng, hoặc khoá tài khoản.

### 4. Quản lý giao diện
- **Trang chủ**:
  - Hiển thị danh sách các sản phẩm mới nhất, sản phẩm bán chạy, khuyến mãi, v.v.
  - Để người dùng dễ dàng duyệt qua các sản phẩm.
- **Trang chi tiết sản phẩm**:
  - Cung cấp đầy đủ thông tin về sản phẩm, bao gồm ảnh, mô tả chi tiết, thông tin kỹ thuật.
  - Hiển thị các đánh giá và bình luận của khách hàng đã mua.
- **Giỏ hàng và thanh toán**:
  - Giao diện giỏ hàng giúp người dùng có thể xem lại các sản phẩm đã chọn.
  - Cung cấp chức năng nhập địa chỉ giao hàng và chọn phương thức thanh toán.
- **Trang quản lý cho admin**:
  - Giao diện cho phép admin quản lý các chức năng như sản phẩm, danh mục, người dùng, doanh thu.

### 5. Các yêu cầu khác
- **Quản lý lỗi và thông báo**:
  - Thông báo rõ ràng cho người dùng khi có lỗi, ví dụ: khi không thể đăng nhập, thanh toán thất bại, v.v.
- **Dữ liệu giả lập**:
  - Sử dụng `json-server` để fake các API của Backend như: sản phẩm, danh mục, người dùng, đơn hàng.

### 6. Cấu trúc thư mục
- `/public`: Các tài nguyên công khai (hình ảnh, favicon, v.v).
- `/src/components`: Các component tái sử dụng.
- `/src/pages`: Các trang của ứng dụng (Trang chủ, trang sản phẩm, trang quản lý, v.v).
- `/src/services`: Các dịch vụ để kết nối với API giả lập.
- `/src/styles`: Các file CSS hoặc sử dụng Tailwind CSS.


## Quy trình làm việc
1. **Quản lý task**: 
   - Sử dụng **Notion** để quản lý và theo dõi tiến độ công việc. (có thể lấy template sau : [template](https://www.notion.so/f1fb8cb6f4ec483fb9a58e2bd90f7a99?v=ab4b607ab7d9476aa89689c326a55b14))
   - Mỗi task sẽ được phân công cụ thể và cập nhật trạng thái liên tục.
   - Mọi thông tin và ghi chú về tiến độ đều sẽ được ghi nhận trên Notion.
2. **Thời gian làm việc**:
   - Tối thiểu **2 giờ mỗi ngày** để phát triển và hoàn thiện các tính năng.
   - Đảm bảo chất lượng và tiến độ công việc.
3. **Daily Report**:
   - Cung cấp báo cáo tiến độ mỗi ngày qua Notion hoặc GitHub.
   - Báo cáo bao gồm các công việc đã hoàn thành, công việc tiếp theo và các vấn đề gặp phải trong ngày.
4. **Quy trình phát triển Git**:
   - Khi đẩy pull request (PR), **không cần đợi review** trước khi tiếp tục làm việc.
   - **Checkout sang nhánh khác** để tiếp tục công việc sau khi đẩy PR.
   - Học cách giải quyết **conflict** nếu có xung đột khi merge nhánh.
5. **Giao diện tham khảo**:
   - Tham khảo giao diện của các trang web nổi tiếng như **Canifa** (khuyến khích clone Canifa vì có đầy đủ chức năng và giao diện hiện đại)

## Tài liệu tham khảo
- [React Documentation](https://reactjs.org/docs/getting-started.html)
- [Next.js Documentation](https://nextjs.org/docs)
- [json-server Documentation](https://github.com/typicode/json-server)
