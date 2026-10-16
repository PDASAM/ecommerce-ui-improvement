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
