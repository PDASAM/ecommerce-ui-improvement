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
---

## AI USAGE LOG – BÀI TẬP CÁ NHÂN BUỔI 2

### 1. Công cụ AI sử dụng

- **Công cụ:** ChatGPT (OpenAI).
- **Mục đích:** Phân tích HTML/CSS, đề xuất cải thiện giao diện, giải thích mã nguồn và hỗ trợ kiểm thử.
- **Phạm vi:** Giao diện danh sách bốn sản phẩm laptop mô phỏng CellphoneS.
- **Nguyên tắc:** Không thay thế toàn bộ mã nguồn, chỉ điều chỉnh những phần cần thiết và kiểm tra kết quả trên trình duyệt.

### 2. Quá trình sử dụng AI

#### Lần 1 – Phân tích mã nguồn hiện tại

**Nội dung trao đổi với AI:**

Cung cấp mã HTML, CSS và ảnh giao diện hiện tại của dự án, yêu cầu AI phân tích các thành phần đã có, xác định ba vấn đề cần cải thiện và đề xuất hướng xử lý phù hợp với bài tập Buổi 2.

**Đề xuất của AI:**

1. Cải thiện trạng thái hover và focus của nút xem cấu hình.
2. Xem xét cách đặt tên class `.product-link` vì tên sản phẩm đang sử dụng thẻ `span`.
3. Kiểm tra khả năng hiển thị của lưới sản phẩm trên các kích thước màn hình khác nhau.

**Đánh giá:**

Các đề xuất tập trung vào những thành phần đã tồn tại trong mã nguồn. Việc kiểm tra responsive được xem là bước xác minh, không mặc định coi bố cục hiện tại có lỗi.

#### Lần 2 – Cải thiện cấu trúc HTML và CSS

**Nội dung trao đổi với AI:**

Yêu cầu hướng dẫn thực hành HTML5 có ngữ nghĩa, CSS selector, Box Model và Flexbox dựa trên mã nguồn hiện tại, không tạo lại website.

**Đề xuất của AI:**

Điều chỉnh tên class hiển thị tên sản phẩm, kiểm tra các phần tử HTML semantic và thử nghiệm thay đổi khoảng cách `gap` giữa những nhãn thông số kỹ thuật.

**Cách thực hiện:**

Rà soát cấu trúc của từng thẻ sản phẩm và thực hành chỉnh sửa CSS tại khu vực `.specs-pills`.

**Nhận xét:**

Việc chỉnh sửa được giới hạn ở những thành phần có liên quan nhằm giữ nguyên nội dung và bố cục chính của website.

#### Lần 3 – Bổ sung hiệu ứng hover và focus

**Nội dung trao đổi với AI:**

Yêu cầu hướng dẫn bổ sung hiệu ứng tương tác cho khu vực “Xem cấu hình chi tiết (Demo)” bằng CSS3, không sử dụng JavaScript và không làm thay đổi đáng kể bố cục.

**Đề xuất của AI:**

Sử dụng các pseudo-class `:hover`, `:focus-visible` kết hợp `transition` cho `.accordion-header`.

**Cách điều chỉnh và áp dụng:**

Sử dụng các màu có sẵn trong hệ thống CSS của website, gồm `--primary-color` và `--primary-hover`, thay vì sử dụng bảng màu mới không liên quan.

**Kết quả kiểm tra:**

Đã kiểm tra các trạng thái tương tác bằng thao tác chuột và bàn phím. Hiệu ứng hoạt động đạt yêu cầu theo kết quả thử nghiệm.

#### Lần 4 – Kiểm thử responsive

**Nội dung trao đổi với AI:**

Yêu cầu hướng dẫn kiểm tra giao diện bằng công cụ responsive của trình duyệt, đánh giá khả năng hiển thị của danh sách sản phẩm trên máy tính, máy tính bảng và điện thoại.

**Đề xuất của AI:**

Kiểm thử tại các độ rộng 1366px, 768px và 390px; kiểm tra số cột, kích thước hình ảnh, khả năng đọc nội dung và hiện tượng tràn ngang.

**Cách thực hiện:**

Sử dụng Responsive Design Mode của trình duyệt và quan sát trực tiếp giao diện tại từng kích thước.

**Kết quả kiểm tra:**

Giao diện đáp ứng yêu cầu kiểm thử. CSS Grid và media query cho phép danh sách chuyển giữa bố cục 4 cột, 2 cột và 1 cột tùy kích thước màn hình.

### 3. Ví dụ về việc kiểm tra và điều chỉnh đề xuất AI

| Nội dung | Mô tả |
|---|---|
| Đề xuất AI | Bổ sung hover và focus cho `.accordion-header` |
| Mục đích | Cải thiện khả năng nhận biết thành phần tương tác |
| Điều chỉnh | Sử dụng màu đỏ thương hiệu đã được khai báo trong CSS |
| Cách kiểm tra | Thử rê chuột, nhấn mở cấu hình và điều hướng bằng phím Tab |
| Kết quả | Hiệu ứng hoạt động, không cần bổ sung JavaScript |
| Bài học | Cần đối chiếu đề xuất AI với mã nguồn và kiểm tra thực tế trước khi áp dụng |

### 4. Nhận xét và bài học rút ra

AI hỗ trợ xác định nhanh những vị trí mã nguồn cần xem xét và giải thích ý nghĩa các thuộc tính HTML/CSS.

Tuy nhiên, không phải đề xuất nào cũng cần áp dụng. Những vấn đề như khả năng hiển thị responsive phải được kiểm tra trực tiếp trước khi kết luận là lỗi.

Qua quá trình thực hành, em hiểu rõ hơn cách sử dụng CSS selector, Box Model, Flexbox, Grid, pseudo-class và media query trong một giao diện thương mại điện tử thực tế.

Việc tự điều chỉnh thuộc tính CSS và quan sát kết quả giúp em hiểu mã nguồn thay vì chỉ sao chép các đoạn code được AI đề xuất.