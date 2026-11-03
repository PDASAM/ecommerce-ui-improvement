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

## Bài tập cá nhân Buổi 2 – HTML5 & CSS3

### 1. Giới thiệu

Dự án tiếp tục phát triển giao diện cải tiến thẻ sản phẩm laptop trên website CellphoneS từ bài tập cá nhân Buổi 1, thuộc học phần Phát triển ứng dụng WEB/TMĐT.

Bài tập tập trung vào việc củng cố cấu trúc HTML5, sử dụng CSS3 để trình bày giao diện và cải thiện khả năng tương tác của khu vực danh sách sản phẩm.

### 2. Khu vực được cải thiện

Khu vực lựa chọn là danh sách bốn sản phẩm laptop trên trang `index.html`.

Trong Buổi 2, nội dung cải thiện tập trung vào hiệu ứng tương tác của nút xem cấu hình chi tiết, kiểm tra cách trình bày các thẻ sản phẩm và khả năng thích ứng với các kích thước màn hình.

### 3. Công nghệ và kỹ thuật sử dụng

| Công nghệ | Ứng dụng |
|---|---|
| HTML5 | Sử dụng header, main, section, article, figure, details, summary và footer |
| CSS Selector | Định dạng các phần tử và class |
| CSS Box Model | Điều chỉnh margin, padding, border và border-radius |
| Flexbox | Căn chỉnh thông tin và các thành phần trong thẻ sản phẩm |
| CSS Grid | Bố trí danh sách sản phẩm thành nhiều cột |
| Media Query | Điều chỉnh bố cục theo kích thước màn hình |
| Hover và Focus | Cải thiện phản hồi tương tác của giao diện |

### 4. Những thay đổi trong Buổi 2

Bổ sung hiệu ứng hover và focus-visible cho khu vực xem cấu hình chi tiết. Các thay đổi được thực hiện trong `css/style.css`, sử dụng bảng màu đỏ hiện có của dự án nhằm bảo đảm tính nhất quán.

Giao diện tiếp tục sử dụng CSS Grid và Flexbox, đồng thời được kiểm tra tại các độ rộng 1366px, 768px và 390px.

### 5. Hướng dẫn chạy website

Mở thư mục dự án bằng Visual Studio Code, sau đó mở file `index.html` bằng Live Server.

Website sử dụng HTML5 và CSS3 thuần, không yêu cầu cài đặt backend hoặc cơ sở dữ liệu.

### 6. Kiểm thử

Giao diện đã được kiểm thử trên các kích thước màn hình máy tính, máy tính bảng và điện thoại.

Hiệu ứng hover và focus của khu vực xem cấu hình cũng được kiểm tra thông qua thao tác chuột và bàn phím.

### 7. Sử dụng AI

AI được sử dụng để hỗ trợ phân tích mã HTML/CSS hiện tại, đề xuất các cải tiến giao diện và giải thích các thuộc tính CSS.

Các đề xuất được xem xét trước khi áp dụng và kiểm tra trực tiếp trên trình duyệt. Nội dung chi tiết được ghi nhận trong `AI_USAGE.md`.

### 8. Repository

https://github.com/PDASAM/ecommerce-ui-improvement