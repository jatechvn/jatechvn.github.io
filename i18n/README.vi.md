# 🤖 Cổng Điều Phối JA-HUB & Không Gian Làm Việc

<p align="center">
  <a href="https://jatechvn.github.io/">
    <img src="../assets/logo.png" alt="JA-HUB Logo" width="120" height="120" style="border-radius: 20px; box-shadow: 0 8px 24px rgba(0, 169, 201, 0.25);">
  </a>
</p>

<p align="center">
  <i>Trang chủ chính thức và cổng điều phối hệ thống tự động hóa của <b>Johnny (jatechvn)</b>, được xây dựng dựa trên kiến trúc <b>JA-HUB</b>.</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Tr%E1%BA%A1ng_th%C3%A1i-Online-00ff87.svg?style=flat-square&logo=statuspage" alt="System Status">
  <img src="https://img.shields.io/badge/Giao_di%E1%BB%87n-Obsidian_BilloDesign-00AFCD.svg?style=flat-square&logo=tailwindcss" alt="Theme">
  <img src="https://img.shields.io/badge/C%C3%B4ng_ngh%E1%BB%87-HTML5_/_CSS3_/_ES6-purple.svg?style=flat-square&logo=javascript" alt="Technology">
  <img src="https://img.shields.io/badge/Tri%E1%BB%83n_khai-GitHub_Pages-orange.svg?style=flat-square&logo=github" alt="Deployment">
  <img src="https://img.shields.io/badge/Gi%E1%BA%A5y_ph%C3%A9p-MIT-yellow.svg?style=flat-square" alt="License">
</p>

<p align="center">
  <a href="#giới-thiệu">🚀 Giới thiệu</a> • 
  <a href="#giao-diện-gốm-obsidian-billodesign">🎨 Hệ thống Giao diện</a> • 
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

## 🎨 Giao diện Gốm Obsidian BilloDesign

Được truyền cảm hứng từ phong cách thiết kế cyber-minimalism tối giản nhưng cao cấp của [billodesign.webflow.io](https://billodesign.webflow.io/), cổng thông tin được lột xác với hệ thống giao diện **Kính Obsidian**:

*   **Quả cầu 3D tương tác Spline**: Nền của khu vực giới thiệu được trang bị quả cầu thủy tinh 3D WebGL tương tác động. Nó sẽ xoay và nghiêng theo chuyển động di chuột thực tế của người dùng, mang lại trải nghiệm tương lai cao cấp.
*   **Màn hình chờ rèm che Preloader**: Khi tải trang, rèm tối màu sẽ tạm thời khóa cuộn màn hình và hiển thị hiệu ứng gõ chữ chào mừng `"Welcome to JA-HUB"` cùng thanh chạy tải trang phát sáng, sau đó rèm sẽ tự động trượt mở sang hai bên.
*   **Đường viền xoay phát sáng (Rotating Borders)**: Tất cả các bảng chức năng (Player, Map, Terminal, Projects) và nút hành động chính đều sở hữu đường viền sáng xoay tròn liên tục bằng CSS nâng cao (`@property --angle` kết hợp mặt nạ `linear-gradient`).
*   **Điểm chấm nhấp nháy hệ thống**: Tích hợp các đèn LED nhấp nháy phát sáng (`pulse-status-indicator`) kế bên tiêu đề các panel để báo hiệu các luồng dữ liệu đang kết nối online.
*   **Chế độ Sáng & Tối tương thích**:
    *   **Chế độ Tối (Dark - Mặc định)**: Màu đen Obsidian `#010101` chủ đạo, các tấm kính mờ với viền sáng xanh cyan tinh tế, font chữ kỹ thuật cao.
    *   **Chế độ Sáng (Light)**: Các tấm kính trắng mờ phủ sương nhẹ (`rgba(245, 245, 247, 0.85)`), chữ xám đen tương phản cao (`#111111`) và các đường biên tối thanh lịch.
*   **Phối hợp Font chữ Hài hòa**: Kết hợp font chữ hiển thị tiêu đề `Lato` với font chữ chuyên viết code `IBM Plex Mono` / `JetBrains Mono` cho các khối hiển thị dữ liệu kỹ thuật.

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

### 4. Trình phát nhạc Apple Music (iOS 16 style)
Trình phát nhạc giao diện kính mờ Liquid Glass được ghim ở cột sidebar trái:
*   **Trích xuất Album Art Động**: Tích hợp CDN `jsmediatags` để tự động giải mã dữ liệu metadata nhúng bên trong tệp `.mp3` đang phát, lấy ảnh album và hiển thị dưới dạng đĩa nhạc tròn xoay sinh động.
*   **Bảng Điều Khiển Âm Lượng Thu Gọn**: Nút loa điều khiển chính hỗ trợ nhấn để mở rộng/thu gọn bảng thanh trượt âm lượng iOS chuyên nghiệp bên dưới, có đầy đủ các tính năng như tắt/mở tiếng nhanh (Mute) và chỉnh âm lượng tối đa 100%.
*   **Khởi Chạy Thông Minh & Autoplay**: Mã nguồn được tối ưu hóa chạy các tiến trình dựng giao diện tĩnh trước, bảo đảm trang web không bị treo do các chính sách chặn CORS của trình duyệt trên giao thức cục bộ `file:///`, kèm cơ chế phát tự động thông minh.

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
│   ├── logo.png               # Brand icon (Lobster AI co-pilot logo)
│   ├── images/                # Thư mục tài nguyên hình ảnh hệ thống
│   │   └── icon.ico           # Biểu tượng trang web (favicon)
│   └── sounds/                # Thư mục âm thanh phát nhạc và ảnh trích xuất
│       ├── *.mp3              # Danh sách bài hát MP3
│       └── *.jpg              # Ảnh album trích xuất từ file nhạc
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
