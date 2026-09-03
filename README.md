# Chuyển Ảnh Sang Dạng PNG/WebP/JPG

> **Tác giả:** Dương Tấn Chánh  
> **Nền tảng:** Single-page Web Application (100% Vanilla HTML5 / CSS3 / JavaScript thuần)

---

## 📖 Giới thiệu

**Chuyển Ảnh Sang Dạng PNG/WebP/JPG** là công cụ chuyển đổi, tối ưu hoá và nén dung lượng hình ảnh hàng loạt chạy trực tiếp trên trình duyệt máy khách (Client-side). 

Ứng dụng được xây dựng hoàn toàn bằng **HTML, CSS và JavaScript thuần**, không sử dụng bất kỳ thư viện ngoài nào (Zero Dependencies), bảo mật quyền riêng tư tuyệt đối vì tập tin không bao giờ bị tải lên máy chủ và có thể chạy hoàn toàn ngoại tuyến (Offline).

---

## ✨ Tính năng nổi bật

### 1. Đa dạng định dạng & Xử lý hàng loạt
* **Đầu vào hỗ trợ:** `PNG`, `JPG/JPEG`, `WEBP`, `BMP`, `SVG`, `GIF` (khung hình đầu), `ICO`, `AVIF`.
* **Đầu ra tuỳ chọn:** `WEBP` (tối ưu dung lượng), `JPG` (tương thích phổ biến), `PNG` (bảo toàn chất lượng Lossless).
* **Nạp ảnh linh hoạt:** 
  * Chọn cùng lúc nhiều tập tin từ thiết bị.
  * Kéo & thả (Drag and Drop) mượt mà, chống chớp nháy màn hình.
  * Dán trực tiếp từ bộ nhớ tạm (`Ctrl + V`).

### 2. Tăng tốc phần cứng đa luồng ngầm (CPU & GPU)
* **Xử lý đa luồng song song:** Tự động điều phối công việc theo số nhân CPU logic của thiết bị, giúp tăng tốc độ nén hàng loạt nhanh gấp nhiều lần mà không chiếm dụng đột biến tài nguyên máy.
* **Giải mã phần cứng GPU:** Tận dụng bộ xử lý đồ hoạ GPU thông qua Canvas 2D để kết xuất ảnh sắc nét và giữ giao diện luôn mượt mà.

### 3. Tối ưu chất lượng & Bảo toàn dữ liệu ảnh
* **Chất lượng mặc định 93%:** Chuẩn nén tối ưu quang học, giữ màu sắc trung thực và chi tiết biên nét căng.
* **Khống chế kích thước (No Upscale):** Tuyệt đối không phóng to vượt kích thước gốc; hỗ trợ thu nhỏ nhanh theo tỉ lệ 100% (Gốc), 75%, 50%, 25% hoặc giới hạn chiều rộng tối đa.
* **Tự động xử lý nền trong suốt:** Tự động lót nền trắng phẳng mịn khi chuyển đổi ảnh trong suốt sang JPG, chống hiện tượng lem vệt đen.
* **Tự động chống lỗi xoay ảnh 2 lần:** Tự động phân tích nhị phân EXIF để chuẩn hoá cờ hướng xoay về chuẩn, đảm bảo ảnh chụp từ điện thoại luôn hiển thị đúng chiều trên mọi thiết bị.

### 4. Kính lúp soi chi tiết chuyên sâu (Fullscreen Deep Zoom)
* **Bấm trực tiếp vào ảnh thu nhỏ** để mở cửa sổ soi chi tiết toàn màn hình.
* **Chuẩn điểm ảnh màn hình thật (Hardware Screen Pixel):** Ánh xạ 1:1 điểm ảnh của ảnh vào đúng 1 bóng bán dẫn của màn hình, triệt tiêu hiện tượng mờ do tỉ lệ thu phóng của hệ điều hành.
* **Các mức zoom chuẩn cấp số nhân:** `100%`, `200%`, `400%`, `800%`, `1600%`.
* **Thuật toán Zoom to Cursor (Phóng to theo vị trí chuột):** Điểm ảnh dưới đầu chuột đứng yên tuyệt đối khi lăn chuột, không để ảnh bị trôi dạt hoặc văng khỏi màn hình.
* **Nút công tắc duy nhất `[ Ảnh Nén / Ảnh Gốc ]`:** Chuyển đổi qua lại tức thì tại đúng toạ độ đang soi để so sánh chất lượng nén.

### 5. Thiết kế thân thiện & Tối ưu cho thiết bị di động
* Giao diện tối giản, loại bỏ các thuật ngữ kỹ thuật phức tạp đối với người dùng phổ thông.
* Tự động bẻ dòng an toàn với các tên tập tin máy tạo dài dằng dặc, không gây vỡ khung hay tràn lề.
* Hỗ trợ đầy đủ thao tác cảm ứng vuốt chạm kéo rê (Pointer Events) và tối ưu tỉ lệ hiển thị trên màn hình điện thoại.

---

## 🛠️ Công nghệ sử dụng

* **HTML5:** Semantic Elements, Canvas API 2D, File API, Drag & Drop API, Clipboard API.
* **CSS3:** Flexbox & CSS Grid, CSS Custom Properties (Variables), Responsive Web Design, hoàn toàn không dùng `!important` và không có style inline.
* **Vanilla JavaScript (ES6+):** Bất đồng bộ (`async/await`), xử lý mảng nhị phân (`ArrayBuffer`, `DataView`, `Blob`), giải phóng bộ nhớ chủ động (`URL.revokeObjectURL`).

---

## 🔒 Quyền riêng tư & An toàn dữ liệu

* **100% Client-side:** Toàn bộ quá trình xử lý diễn ra cục bộ trực tiếp trên trình duyệt của người dùng.
* Tuyệt đối không gửi hay lưu trữ bất kỳ hình ảnh nào lên máy chủ bên ngoài.

---

## 👤 Tác giả

**Dương Tấn Chánh**  
* Chuyên mục: Lập trình ứng dụng web Single-page (Vanilla HTML/CSS/JS thuần).

---

## 📄 Giấy phép (License)

Dự án được phát hành theo giấy phép [MIT License](LICENSE).
