# 🤖 Cổng Điều Phối JA-HUB & Không Gian Làm Việc

<p align="center">
  <a href="https://jatechvn.github.io/">
    <img src="../assets/logo.png" alt="JA-HUB Logo" width="120" height="120" style="border-radius: 20px; box-shadow: 0 8px 24px rgba(0, 240, 255, 0.25);">
  </a>
</p>

<p align="center">
  <i>Trang chủ chính thức và cổng điều phối hệ thống tự động hóa của <b>Johnny (jatechvn)</b>, được xây dựng dựa trên kiến trúc <b>JA-HUB</b>.</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Tr%E1%BA%A1ng_th%C3%A1i-Online-00ff87.svg?style=flat-square&logo=statuspage" alt="System Status">
  <img src="https://img.shields.io/badge/Giao_di%E1%BB%87n-Liquid_Glass-00f0ff.svg?style=flat-square&logo=tailwindcss" alt="Theme">
  <img src="https://img.shields.io/badge/C%C3%B4ng_ngh%E1%BB%87-HTML5_/_CSS3_/_ES6-purple.svg?style=flat-square&logo=javascript" alt="Technology">
  <img src="https://img.shields.io/badge/Tri%E1%BB%83n_khai-GitHub_Pages-orange.svg?style=flat-square&logo=github" alt="Deployment">
  <img src="https://img.shields.io/badge/Gi%E1%BA%A5y_ph%C3%A9p-MIT-yellow.svg?style=flat-square" alt="License">
</p>

<p align="center">
  <a href="#giới-thiệu">🚀 Giới thiệu</a> • 
  <a href="#giao-diện-liquid-glass">🎨 Hệ thống Giao diện</a> • 
  <a href="#tính-năng-nổi-bật">💡 Tính năng Nổi bật</a> • 
  <a href="#kiến-trúc-hệ-thống">🏗️ Sơ đồ Kiến trúc</a> • 
  <a href="https://jatechvn.github.io/">🌐 Ghé thăm Cổng Portal</a>
</p>

<p align="center">
  <a href="../README.md">🇺🇸 English Version</a>
</p>

---

## 🚀 Giới thiệu

> *"Trong hệ sinh thái JA-HUB, không có dòng code nào hoạt động đơn độc. AHK là đôi tay, Python là trí tuệ, và Node.js là ý chí của người kiến trúc sư."* 🦞

**jatechvn.github.io** là cổng dashboard điều phối trung tâm được thiết kế để giám sát, quản lý và trình bày toàn bộ hệ sinh thái tự động hóa đa công nghệ của Johnny (**JA-HUB**). Thay vì chỉ hiển thị các dự án dưới dạng thẻ tĩnh, cổng thông tin này hoạt động như một trình khám phá cấu trúc hệ thống trực quan, cung cấp cái nhìn toàn diện về tất cả các kịch bản và máy chủ đang chạy trên các máy trạm local cũng như máy chủ ảo VPS cloud.

---

## 🎨 Giao diện Liquid Glass

Được truyền cảm hứng từ phong cách thiết kế kính mờ nguyên bản trên các ứng dụng PySide6 Python của Johnny (như `JA_AUTO_GIT`), cổng thông tin tích hợp một bộ máy giao diện **Liquid Glass**:

*   **Các tấm kính mờ linh hoạt (Glassmorphism)**: Các bộ lọc làm mờ hậu cảnh (backdrop blur) và độ trong suốt tạo nên các panel tinh tế kết hợp hiệu ứng neon phát sáng màu xanh cyan và cam.
*   **Chế độ Sáng & Tối tương thích**:
    *   **Chế độ Tối (Dark - Mặc định)**: Màu sắc mang hơi hướng cyber-punk, làm nổi bật sơ đồ kết nối và bảng ghi nhận hoạt động (console) màu xanh lục bảo.
    *   **Chế độ Sáng (Light)**: Các tấm kính trắng mờ (`rgba(240, 240, 240, 0.75)`), chữ xám đen độ tương phản cao (`#111111`) và các đường viền tối màu thanh lịch.
*   **Đồng bộ cấu hình thiết bị**: Tự động nhận diện thiết lập giao diện của hệ điều hành (`prefers-color-scheme`) để điều chỉnh độ sáng phù hợp nhất, đi kèm với nút chuyển đổi Mặt Trời/Mặt Trăng thủ công.

---

## 💡 Tính năng Nổi bật

### 1. Sơ đồ Kiến trúc SVG Tương tác
Biểu đồ vector trực quan hóa mối liên kết giữa **JA-HUB (Bộ não trung tâm)** và các Worker. Di chuột qua các worker để kích hoạt các đường truyền dữ liệu động phát sáng và hiển thị thông tin mô tả chi tiết của từng phân mục.

### 2. Trình duyệt khám phá Project
Khám phá tất cả các thư mục dự án tự động hóa:
*   **Bộ lọc Công nghệ**: Phân nhóm theo ngôn ngữ và nền tảng (Python, AHK, Node.js, PowerShell, Windows Batch, C#, Cấu hình VPS).
*   **Tìm kiếm Thời gian thực**: Hỗ trợ tìm kiếm theo tên dự án, thư viện sử dụng, mô tả và các đường dẫn tệp tin bên trong.
*   **Cây thư mục nguồn (Source Tree)**: Hộp thoại (modal) hiển thị cấu trúc tệp tin của từng project, cho phép thu gọn/mở rộng thư mục trực quan.

### 3. Khung điều khiển Sandbox Terminal
Bảng điều khiển giả lập dòng lệnh Unix ở cuối trang cho phép chạy các tác vụ chuẩn đoán:
*   `help`: Xem danh sách câu lệnh.
*   `status`: Quét trạng thái kết nối và kiểm tra hoạt động của các Worker (Watchdog logs).
*   `list`: Liệt kê các mắt xích công nghệ (Spokes) trong hệ thống.
*   `about`: Hiển thị triết lý thiết kế và thông tin kiến trúc sư Johnny.
*   `clear`: Dọn sạch màn hình console.

---

## 🏗️ Kiến trúc Hệ thống

| Mắt xích (Spokes) | Công nghệ | Vai trò hoạt động | Dự án tiêu biểu |
| :--- | :--- | :--- | :--- |
| **JA-HUB (Brain)** | Node.js / WS | Điều phối tác vụ chính, Quản lý APIs & Websockets | `server.js`, `web_ui` |
| **Python Spokes** | Python 3.13 | Xử lý logic nặng, phân tích log, chạy AI model, GUI tools | `JA_AUTO_GIT`, `JA_KEY_CREATOR` |
| **AHK Spokes** | AutoHotkey v1/v2 | Đôi tay hệ thống: Click UI, hook phần cứng, khay hệ thống | `TRAYSYSTEM.ahk`, `USB_Debug_detect` |
| **PowerShell** | WinRM / PS1 | Quản trị sâu Windows, quét cổng mạng LAN | `Network_Scanner.ps1` |
| **Batch Spokes** | Command Scripts | Setup nhanh môi trường phát triển, bypass phân quyền | `NSudo_8.2` |
| **C# Core** | C# / Sockets | Xử lý TCP socket đa luồng tốc độ cao cho máy test | `LVI_LX_RETEST_CHECK` |
| **VPS Spoke** | CentOS 7 | Định tuyến RouterOS, cấu hình bảo mật SFTP và backup | `backup_agent.sh` |

---

## 📦 Cấu trúc Thư mục

```text
jatechvn.github.io/
├── index.html                 # Điểm vào chính (Trang Dashboard)
├── README.md                  # Hướng dẫn chính (Tiếng Anh)
├── ABOUT.txt                  # Thẻ thông tin rút gọn
├── LICENSE                    # Giấy phép phần mềm MIT
│
├── assets/                    # Thư mục tài nguyên
│   └── logo.png               # Brand icon (Lobster AI co-pilot logo)
│
└── i18n/                      # Thư mục đa ngôn ngữ
    ├── README.vi.md           # Bản tiếng Việt (Tệp tin này)
    ├── README.zh-CN.md        # Bản tiếng Trung
    └── README.ja-JP.md        # Bản tiếng Nhật
```

---

## 🌐 Chạy thử nghiệm Local

Để mở trang dashboard trên trình duyệt máy tính của bạn:

1.  Nhấp đúp chuột trực tiếp vào tệp [index.html](index.html), hoặc chạy một HTTP Server nhẹ bằng Python trong thư mục dự án:
    ```bash
    python -m http.server 8000
    ```
2.  Mở trình duyệt bất kỳ và truy cập đường dẫn:
    ```text
    http://localhost:8000
    ```

---

## 📄 Giấy phép sử dụng

Dự án này được cấp phép theo các điều khoản của **MIT License**. Chi tiết xem tại tệp [LICENSE](../LICENSE).
