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
---

## BÀI TẬP CÁ NHÂN BUỔI 2 – HTML5 & CSS3

### 1. Giới thiệu

Bài tập tiếp tục phát triển giao diện cải tiến thẻ sản phẩm laptop của website CellphoneS từ Buổi 1, thuộc học phần Phát triển ứng dụng WEB/TMĐT tại UEH.

Trong Buổi 2, nội dung thực hành tập trung vào việc rà soát cấu trúc HTML5, củng cố CSS selector và Box Model, kiểm tra Flexbox/CSS Grid và cải thiện hiệu ứng tương tác của khu vực danh sách sản phẩm.

### 2. Website tham khảo và phạm vi cải thiện

- **Website tham khảo:** CellphoneS.
- **Khu vực được chọn:** Danh sách bốn sản phẩm laptop.
- **File HTML:** `index.html`.
- **File CSS:** `css/style.css`.
- **Phạm vi:** Cải thiện giao diện hiện có, không xây dựng lại website hoặc bổ sung chức năng thương mại điện tử thực tế.

Bốn sản phẩm minh họa gồm ASUS Vivobook 14, Apple MacBook Air M2, MSI Cyborg 15 và HP OmniBook 5 AI.

### 3. Các kỹ thuật HTML5/CSS3 đã thực hành

| Kỹ thuật | Ứng dụng trong dự án |
|---|---|
| HTML5 Semantic | Sử dụng `header`, `main`, `section`, `article`, `figure`, `details`, `summary`, `footer` |
| CSS Selector | Định dạng phần tử, class và phần tử con |
| CSS Box Model | Điều chỉnh `margin`, `padding`, `border`, `border-radius` |
| Flexbox | Căn chỉnh header, nhãn thông số và các thành phần trong thẻ sản phẩm |
| CSS Grid | Bố trí danh sách sản phẩm thành các cột |
| Media Query | Điều chỉnh bố cục theo độ rộng màn hình |
| Hover và Focus | Cải thiện phản hồi khi tương tác với nút xem cấu hình |

### 4. Những cải tiến trong Buổi 2

**4.1. Rà soát cấu trúc HTML**

Kiểm tra các thẻ HTML semantic, thuộc tính `alt` của hình ảnh và cách tổ chức nội dung trong từng thẻ sản phẩm.

Điều chỉnh cách đặt tên class hiển thị tên sản phẩm để phù hợp với vai trò văn bản, tránh gây nhầm lẫn với liên kết điều hướng.

**4.2. Cải thiện hiệu ứng tương tác**

Bổ sung trạng thái `:hover`, `:focus-visible` và `transition` cho khu vực “Xem cấu hình chi tiết (Demo)”.

Các hiệu ứng sử dụng hệ thống màu đỏ thương hiệu có sẵn trong CSS nhằm duy trì tính nhất quán của giao diện.

**4.3. Điều chỉnh khoảng cách thông số kỹ thuật**

Thực hành điều chỉnh thuộc tính `gap` trong `.specs-pills` từ 6px thành 8px, quan sát sự thay đổi khoảng cách giữa các nhãn thông số và kiểm tra khả năng hiển thị trên thiết bị nhỏ.

**4.4. Kiểm tra responsive**

Giao diện được kiểm tra ở ba độ rộng màn hình:

- 1366px: Danh sách sản phẩm hiển thị 4 cột.
- 768px: Danh sách sản phẩm hiển thị 2 cột.
- 390px: Danh sách sản phẩm hiển thị 1 cột.

Kết quả kiểm thử được ghi nhận đạt yêu cầu về bố cục và khả năng sử dụng.

### 5. Hướng dẫn chạy website

1. Clone repository về máy hoặc tải mã nguồn từ GitHub.
2. Mở thư mục dự án bằng Visual Studio Code.
3. Mở file `index.html` bằng Live Server.
4. Sử dụng trình duyệt để xem giao diện và thử các thành phần tương tác.
5. Sử dụng Responsive Design Mode/DevTools để kiểm tra trên các kích thước màn hình khác nhau.

Website sử dụng HTML5 và CSS3 thuần, không yêu cầu backend, cơ sở dữ liệu hoặc cài đặt framework.

### 6. Kiểm thử và minh chứng

Nội dung kiểm thử bao gồm khả năng mở trang HTML, liên kết CSS, hiển thị hình ảnh sản phẩm, bố cục responsive và trạng thái hover/focus.

Ảnh trước và sau cải thiện, ảnh giao diện sau hoàn thiện và bảng kiểm thử được trình bày trong báo cáo Google Docs của bài cá nhân Buổi 2.

### 7. Sử dụng AI

ChatGPT được sử dụng để hỗ trợ rà soát mã nguồn, đề xuất cải thiện HTML/CSS, giải thích các thuộc tính và hướng dẫn kiểm thử.

Các đề xuất được đối chiếu với mã nguồn hiện có và kiểm tra trên trình duyệt trước khi áp dụng. Quá trình sử dụng AI được ghi nhận chi tiết trong `AI_USAGE.md`.

### 8. Hạn chế và hướng phát triển

Website hiện tập trung mô phỏng giao diện danh sách sản phẩm, chưa triển khai tìm kiếm, giỏ hàng, đặt hàng hoặc thanh toán.

Ở các buổi tiếp theo, có thể bổ sung JavaScript để phát triển những chức năng tương tác phù hợp với yêu cầu môn học.

### 9. Repository

https://github.com/PDASAM/ecommerce-ui-improvement