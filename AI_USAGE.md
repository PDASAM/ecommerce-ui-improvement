# AI Usage Log

## 1. Công cụ AI
Google Gemini (phương án và mã nguồn đầu tiên); ChatGPT (hỗ trợ rà soát mã và chuẩn bị bản chạy thử).

## 2. Mục đích
Phân tích UX, đề xuất bố cục thẻ sản phẩm, tạo mã HTML5/CSS3, ảnh SVG minh họa, hỗ trợ giải thích và gợi ý kiểm thử.

## 3. Prompt đã sử dụng
Xem prompt Nhiệm vụ 3 trong báo cáo Google Docs; chèn nguyên văn prompt thực tế vào đây trước khi nộp.

## 4. Kết quả AI đề xuất
Trang demo 4 Product Card, Grid/Flexbox responsive, thông số `details/summary`, style CSS tách riêng.

## 5. Kiểm tra và điều chỉnh
- Bản mã Gemini ban đầu có 8 liên kết `href="#demo-link"` không có đích tương ứng. Phiên bản này thay nút CTA giả bằng điều khiển `details` để mở/đóng thông số, đồng thời bỏ liên kết giả tại tên sản phẩm.
- Chú thích giá và hình minh họa rõ hơn, không nhầm với dữ liệu bán hàng thực.
- **Sau khi tự chạy, bổ sung lỗi tự phát hiện, cách sửa và bằng chứng trước/sau của chính sinh viên.**

## 6. Phần có thể giải thích
- Grid `.product-grid` và Media Queries thay số cột.
- Flexbox trong `.product-card`, `.product-body` căn cấu trúc dọc.
- `details/summary` mở rộng cấu hình không JavaScript.
- `:focus-visible`, `alt`, nhãn giá cũ `<del>` hỗ trợ UX/a11y.

## AI Usage Log – Bài tập cá nhân Buổi 2

### Công cụ sử dụng

ChatGPT – hỗ trợ phân tích, giải thích và đề xuất cải thiện mã HTML5/CSS3.

### Lần 1 – Phân tích mã nguồn hiện tại

**Nội dung yêu cầu:** Phân tích giao diện danh sách sản phẩm laptop hiện có, xác định các vấn đề về cấu trúc HTML, trình bày CSS và đề xuất hướng cải thiện.

**Kết quả AI đề xuất:** Cải thiện phản hồi tương tác của nút xem cấu hình, rà soát cách đặt tên class và kiểm tra bố cục responsive.

**Đánh giá:** Các đề xuất được đối chiếu với mã nguồn hiện tại. Chỉ lựa chọn những nội dung phù hợp với phạm vi bài tập cá nhân, không xây dựng lại website.

### Lần 2 – Cải thiện hover và focus

**Nội dung yêu cầu:** Bổ sung hiệu ứng hover và focus cho khu vực xem cấu hình chi tiết của thẻ sản phẩm bằng CSS3, không sử dụng JavaScript.

**Đề xuất của AI:** Sử dụng các pseudo-class `:hover`, `:focus-visible` kết hợp `transition`.

**Cách áp dụng:** Bổ sung các quy tắc CSS cho `.accordion-header`, kế thừa màu sắc từ hệ thống biến CSS của website.

**Kết quả:** Đã kiểm tra các trạng thái tương tác trên trình duyệt và xác nhận hoạt động đạt yêu cầu.

### Lần 3 – Kiểm tra responsive

**Nội dung yêu cầu:** Kiểm tra cách bố trí các thẻ sản phẩm ở độ rộng 1366px, 768px và 390px.

**Kết quả:** Giao diện sử dụng CSS Grid và media query để chuyển số cột theo kích thước màn hình. Sau khi thử nghiệm, bố cục được xác nhận đạt yêu cầu tại ba kích thước kiểm tra.

### Nhận xét

Việc sử dụng AI giúp xác định các vị trí mã nguồn cần xem xét, đồng thời hỗ trợ hiểu rõ hơn về CSS selector, Box Model, Flexbox, Grid và các trạng thái tương tác.

Các đề xuất cần được kiểm tra bằng trình duyệt trước khi đưa vào phiên bản hoàn thiện.