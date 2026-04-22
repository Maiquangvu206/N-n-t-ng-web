
# Câu A1

## a. Ý 1

1. **DNS Lookup**: Trình duyệt hỏi nhà cung cấp DNS để tìm địa chỉ IP của `shopee.vn` (giống như tra cứu số điện thoại từ danh bạ).

2. **Gửi HTTP Request**: Trình duyệt (client) gửi yêu cầu tới máy chủ để lấy trang chủ.

3. **Server xử lý**: Máy chủ tiếp nhận yêu cầu, truy vấn cơ sở dữ liệu và chuẩn bị nội dung trả về.

4. **Trả về HTTP Response**: Server gửi lại các file HTML, CSS, JS và/hoặc dữ liệu API.

5. **Browser Rendering**: Trình duyệt nhận tài nguyên và kết xuất giao diện (render) cho người dùng.

## b. Ý 2

**Tab Network** là công cụ giúp giám sát hoạt động truyền tải giữa trình duyệt và máy chủ; nó hiển thị:

- Danh sách file được tải về (HTML, CSS, JS, ảnh, API).
- Trạng thái phản hồi (thành công hay lỗi).
- Kích thước file và loại file.
- Thời gian tải từng tài nguyên.

# Câu A2
    Trang web dưới đây bị Google đánh giá SEO thấp vì lạm dụng <div>.
    Lỗi 1: Không dùng <header> cho phần đầu trang mà dùng <div>: <div class="header">
    Lỗi 2: Không dùng <nav> cho menu mà dùng <div class="menu">
    Lỗi 3: Không dùng <main> cho nội dung chính mà dùng <div class="main">
    Lỗi 4: Không dùng <article> cho sản phẩm mà dùng  <div class="product">
    Dùng <p> để chứa 1 đoạn văn thay vì <div class="price">25.990.000đ</div>
    Nên dùng <footer> thay vì <div class="footer">© 2026 ShopTLU</div>
    Sửa lại:
    <header>
        <div class="logo">ShopTLU</div>
        <nav>
            <a href="/">Trang chủ</a>
            <a href="/products">Sản phẩm</a>
        </nav>
    </header>

    <main>
       <article class="product">
        <h1>iPhone 16 Pro</h1>
        <p class="price">25.990.000đ</p>
        <img src="iphone.jpg" alt= "iPhone 16 Pro">
       </article>
    </main>

    <footer>
        <p>© 2026 ShopTLU</p>
    </footer>

# Câu A3
    Do thẻ <div> là thẻ block, chiếm cả dòng nên khi đóng thẻ </div> thì sẽ phải xuống dòng mới để viết, còn các thẻ <span> và <strong> là các thẻ inline, chỉ chiếm phần nội dung nằm trong thẻ nên khí đóng 2 thẻ này vẫn có thể viết tiếp nội dung nằm cạnh nhau trên dòng đó hoặc xuống dòng mới để viết.
    Text art:
        Hộp 1
        Text A Text B
        Hộp 2
        Text C Text D
        Hộp 3

# Câu A4
    <thead>: Là phần đầu bảng, chứa tiêu đề cột
    <tbody>: Là phần nội dung chính của bảng, dùng để chứa dữ liệu chính của bảng
    <tfoot>: Là phần cuối bảng dùng để chứa các kết luận, thống kê, tổng kết của bảng
    KHÔNG NÊN dùng table để tạo layout trang web vì:
    - Accessibility: Screen reader và trợ năng kỳ vọng cấu trúc tabular; dùng table cho layout gây hiểu lầm nội dung, làm khó điều hướng cho người dùng khuyết tật.
    - Semantic & SEO: Tables biểu thị dữ liệu có hàng-cột; lạm dụng làm layout phá nghĩa ngữ nghĩa DOM, ảnh hưởng tới SEO và khả năng hiểu nội dung của bot/assistive tech.
    - Responsiveness / Flexibility: Table cố định theo lưới, khó responsive; CSS Grid/Flexbox cung cấp cách bố cục linh hoạt và dễ điều chỉnh cho nhiều kích thước màn hình.
    - Hiệu năng & Bảo trì: Bảng lớn gây reflow nặng khi thay đổi nội dung; code layout bằng table thường phức tạp, khó maintain và kém tách bạch giữa cấu trúc & trình bày.

# Câu B3
    Lỗi 1 — Dòng 1 — <!DOCTYPE> không đầy đủ; nên dùng <!DOCTYPE html> — Sửa thành <!DOCTYPE html>.
    Lỗi 2 — Dòng 5 — Thẻ <title> chưa đóng trước khi chèn <meta>; meta nằm bên trong title — Đóng </title> rồi chèn <meta charset="utf-8"> ở dòng tiếp theo.
    Lỗi 3 — Dòng 6 — meta charset="utf8" không chuẩn (thiếu dấu nối) — Đổi thành meta charset="utf-8".
    Lỗi 4 — Dòng 10 — Thẻ <h1> mở hai lần, thiếu </h1> đóng — Thay <h1>Welcome to ShopTLU<h1> bằng <h1>Welcome to ShopTLU</h1>.
    Lỗi 5 — Dòng 14 — Các thẻ <a> trong nav không được đóng đúng (<a>...<a> thay vì </a>) — Đóng mỗi anchor bằng </a> (ví dụ <a href="home">Trang chủ</a>).
    Lỗi 6 — Dòng 14,15 — Giá trị href="home"/"products" có thể không đúng (nên là đường dẫn file hoặc anchor) — Đổi thành href="#home" hoặc href="#index"
    Lỗi 7 — Dòng 22 — img src=iphone.jpg thiếu dấu ngoặc kép quanh giá trị và không có alt — Viết img src="iphone.jpg" alt="iPhone 16 Pro">.
    Lỗi 8 — Dòng 24 — Thẻ <b> và </p> bị lồng sai: <p>Giá: <b>25.990.000đ</p></b> — Sửa thứ tự đóng: <p>Giá: <b>25.990.000đ</b></p>.
    Lỗi 9 — Dòng 19,42 — Có hai thẻ <main>; chỉ nên có một main chính — Đổi thẻ phụ thành <aside> hoặc một section cho sidebar.
    Lỗi 10 — Dòng 47 — Thẻ <footer> chứa <p> nhưng không đóng </p> — Thêm </p> trước </footer>.
    Lỗi 11 — Dòng 2- end — Không có thuộc tính lang cho thẻ <html> — Thêm lang="vi" (hoặc en) vào <html>.
    Lỗi 12 — Toàn file — Indentation & cấu trúc thụt lề lộn xộn, làm giảm đọc hiểu — Canh lại indent và format file để readable.