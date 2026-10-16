# E-commerce UI Improvement – Laptop Product Cards

## Giới thiệu
Bài thực hành HTML5/CSS3 cải tiến thẻ sản phẩm trên trang danh mục laptop, tham khảo cách trình bày của CellphoneS. **Đây là giao diện mô phỏng không liên kết với CellphoneS và không có chức năng đặt hàng.** Giá, hình SVG và thông số được dùng để minh họa.

## Website tham khảo
- CellphoneS: https://cellphones.com.vn/
- Khu vực khảo sát: Trang chủ, Danh mục Laptop, Chi tiết sản phẩm, Tìm kiếm, Giỏ hàng.

## Thành phần & công nghệ
- HTML5 Semantic: `header`, `main`, `section`, `article`, `details`, `summary`.
- CSS3 riêng trong `css/style.css`, dùng Grid, Flexbox và Media Queries.
- 4 sản phẩm minh họa bằng SVG tự tạo.
- Thẻ `details` mở/đóng cấu hình thực tế, không cần JavaScript.
- Responsive: desktop 4 cột, tablet 2 cột, mobile 1 cột.

## Chạy thử
Mở `index.html` bằng trình duyệt hoặc VS Code + Live Server. Để thử responsive, mở DevTools (`F12`) rồi bật chế độ thiết bị (`Ctrl+Shift+M`).

## Cải tiến UI
Nhấn mạnh tên, thông số và giá, tách ưu đãi có điều kiện, giảm nhãn quảng cáo, dùng một thao tác xem cấu hình khả dụng thay cho liên kết demo không tồn tại.

## Sử dụng AI
Google Gemini hỗ trợ đề xuất phương án và sinh mã nguồn. Bản mã đã được chỉnh sửa để loại bỏ các liên kết `#demo-link` không hoạt động, chuyển sang điều khiển `<details>` có thể mở/đóng. Xem `AI_USAGE.md`; bổ sung nhật ký kiểm thử thực tế sau khi chạy.
