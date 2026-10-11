<div align="center">

# ✦ 3D Login Interface

### Giao diện đăng nhập kính mờ với hiệu ứng chuyển động 3D

Một trang đăng nhập gọn nhẹ, nổi bật với nền gradient chuyển động, thẻ kính mờ và hiệu ứng nghiêng theo con trỏ. Mở trực tiếp trên trình duyệt — không cần cài đặt thư viện hay công cụ build.

<p>
  <img src="https://img.shields.io/badge/HTML5-structure-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-visuals-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-interactions-F7DF1E?style=for-the-badge&logo=javascript&logoColor=222" alt="JavaScript">
  <img src="https://img.shields.io/badge/Dependencies-None-2EA44F?style=for-the-badge" alt="Không phụ thuộc thư viện">
</p>

**Tác giả: Lê Phú An**

</div>

---

## ✨ Tổng quan

**3D Login Interface** là giao diện đăng nhập front-end theo phong cách hiện đại, tập trung vào cảm giác chiều sâu và chuyển động tinh tế. Nội dung nằm trong một thẻ đăng nhập ở giữa màn hình, nổi trên nền xanh tím với các vùng sáng gradient mềm mại.

> Đây là **bản demo giao diện**. Biểu mẫu hiện chỉ mô phỏng trạng thái gửi thành công, chưa xác thực tài khoản và chưa kết nối máy chủ.

## 🎨 Điểm nổi bật

- **Nền gradient nhiều lớp:** phối màu xanh dương, tím và hồng; hai quầng sáng mờ chuyển động nhẹ nhàng.
- **Thẻ đăng nhập kiểu glassmorphism:** nền bán trong suốt, hiệu ứng blur, viền sáng và đổ bóng tạo chiều sâu.
- **Hiệu ứng nghiêng 3D:** thẻ phản hồi theo vị trí con trỏ và trở về vị trí cân bằng khi rê chuột ra ngoài.
- **Nhãn nổi cho ô nhập:** nhãn email và mật khẩu dịch chuyển khi ô được focus hoặc có nội dung.
- **Nút đăng nhập có điểm nhấn:** gradient, hiệu ứng ánh sáng quét khi hover và phản hồi khi nhấn.
- **Trạng thái gửi mô phỏng:** nút lần lượt hiển thị “Signing in...” và “✓ Success!”, sau đó tự trở về trạng thái ban đầu.
- **Bố cục thích ứng:** thẻ thu hẹp trên màn hình nhỏ.
- **Không dùng framework:** HTML, CSS và JavaScript thuần; không cần cài package.

## 🖥️ Giao diện gồm những gì?

| Khu vực | Nội dung và hành vi |
| --- | --- |
| Nền trang | Gradient xanh tím toàn màn hình, hai quầng sáng chuyển động |
| Tiêu đề | “Welcome Back” cùng dòng mô tả “Sign in to continue” |
| Email | Trường nhập kiểu `email`, bắt buộc nhập theo kiểm tra cơ bản của trình duyệt |
| Mật khẩu | Trường nhập kiểu `password`, bắt buộc nhập |
| Tùy chọn | Checkbox “Remember me” và liên kết “Forgot password?” |
| Nút gửi | “Sign In”, có trạng thái loading và thông báo thành công mô phỏng |
| Đăng ký | Dòng “Don't have an account? Sign up” ở cuối thẻ |

Các nhãn, nội dung và nút trong giao diện hiện được viết bằng **tiếng Anh**.

## 🚀 Bắt đầu nhanh

### Mở trực tiếp

1. Tải hoặc sao chép thư mục dự án về máy.
2. Mở `index.html` bằng trình duyệt hiện đại.
3. Nhập email và mật khẩu bất kỳ để xem hiệu ứng gửi biểu mẫu.

### Mở bằng VS Code

Mở thư mục dự án trong VS Code, sau đó mở `index.html` bằng tiện ích Live Server nếu muốn chạy qua máy chủ phát triển cục bộ.

**Không cần** `npm install`, bước build hay cấu hình môi trường.

## 🧭 Cách sử dụng

1. Nhập email hợp lệ theo kiểm tra HTML của trình duyệt.
2. Nhập mật khẩu.
3. Có thể bật “Remember me” — trong bản demo, lựa chọn này chưa được lưu hoặc xử lý.
4. Nhấn **Sign In** để xem trạng thái loading và thông báo thành công giả lập.
5. Di chuyển con trỏ trên thẻ để trải nghiệm hiệu ứng nghiêng 3D.

> Các liên kết “Forgot password?” và “Sign up” hiện dùng `href="#"`, chưa điều hướng đến trang chức năng.

## 🧰 Công nghệ

- **HTML5:** cấu trúc trang, biểu mẫu và kiểm tra trường bắt buộc.
- **CSS3:** gradient, glassmorphism, animation, chuyển động hover và media query.
- **JavaScript thuần:** hiệu ứng parallax theo chuột và trạng thái gửi biểu mẫu.

## 📁 Cấu trúc thư mục

```text
3d-login/
├── index.html   # Trang demo hiện tại; CSS và JavaScript được viết trực tiếp trong file
├── style.css    # Tệp CSS riêng, hiện chưa được index.html nạp
├── script.js    # Tệp JavaScript riêng, hiện chưa được index.html nạp
└── README.md    # Tài liệu dự án
```

### Lưu ý về các tệp CSS và JavaScript riêng

Giao diện được mô tả trong README này là phiên bản nằm trực tiếp trong `index.html`. Tệp `style.css` và `script.js` là các tệp riêng hiện có trong thư mục nhưng **chưa được liên kết** từ trang HTML; các selector và ID trong chúng cũng không trùng hoàn toàn với markup hiện tại. Vì vậy, trình duyệt không dùng chúng khi mở trang demo. Nếu muốn chuyển sang cấu trúc CSS/JS tách file, cần đồng bộ selector và phần tử HTML trước.

## ⚙️ Chi tiết kỹ thuật

- Thẻ đăng nhập được đặt giữa màn hình bằng Flexbox.
- Nền dùng các lớp gradient và pseudo-element `::before` / `::after` kết hợp animation `float`.
- Hiệu ứng parallax tính vị trí con trỏ tương đối với tâm thẻ rồi áp dụng `rotateX` và `rotateY`.
- Biểu mẫu chặn thao tác gửi mặc định; trạng thái thành công chỉ thay đổi nội dung và màu nút trong thời gian ngắn.
- Media query tại `max-width: 480px` điều chỉnh chiều rộng và khoảng đệm của thẻ.

## 🔒 Giới hạn của bản demo

- Không có backend, API đăng nhập, xác thực danh tính hay tạo phiên người dùng.
- Không kiểm tra thông tin đăng nhập với tài khoản thật.
- Không có chức năng khôi phục mật khẩu hoặc đăng ký thực tế.
- Checkbox “Remember me” chưa lưu trạng thái.
- Trạng thái “Success” chỉ là minh họa giao diện; không chứng minh đăng nhập thành công.
- Không nhập hoặc sử dụng mật khẩu thật trên bản demo này.

## 🗺️ Hướng phát triển

- Tách CSS và JavaScript thành các tệp được nạp thực sự từ `index.html`.
- Kết nối form với API xác thực và xử lý lỗi đăng nhập.
- Bổ sung luồng đăng ký và khôi phục mật khẩu.
- Hoàn thiện khả năng truy cập bằng nhãn biểu mẫu, trạng thái focus bàn phím và thông báo trạng thái phù hợp.
- Cải thiện hỗ trợ thiết bị cảm ứng và tùy chọn giảm chuyển động.

## 📄 Giấy phép

Chưa khai báo giấy phép sử dụng trong repository.

---

<div align="center">

Được thiết kế và xây dựng bởi **Lê Phú An** · *3D Login Interface*

</div>
