# NuxOS11 Creator

**NuxOS11 Creator** là công cụ xây dựng (image builder) dùng để tạo ra các bản **Windows 11 tùy biến nhẹ, ổn định và minh bạch**, phục vụ cho dự án **NuxOS**.

Dự án hướng tới người dùng:
- Cần một hệ điều hành Windows **gọn nhẹ**
- Ưu tiên **ổn định lâu dài (LTSC mindset)**
- Không thích telemetry, bloatware
- Muốn hiểu rõ hệ điều hành của mình đã bị thay đổi những gì

> NuxOS11 Creator **không phải là một bản Windows bẻ khóa** và **không tự động kích hoạt Windows**.

---

## 🎯 Mục tiêu dự án

- Tạo nền tảng build Windows 11 **nhẹ – sạch – an toàn**
- Tôn trọng cấu trúc gốc của Windows
- Không phá vỡ:
  - Windows Update
  - Windows Defender
- Minh bạch mọi thay đổi được thực hiện

Triết lý của dự án chịu ảnh hưởng từ:
- Linux LTSC / Enterprise (Debian, RHEL, Alma, Rocky)
- NixOS (tính tái lập, kiểm soát cấu hình)
- *“less is more”*

---

## 🧩 NuxOS11 Creator làm được gì?

- Tự động:
  - Gỡ bỏ ứng dụng không cần thiết (AppX / UWP)
  - Tinh giản thành phần không ảnh hưởng Update & Defender
  - Tối ưu trải nghiệm người dùng
- Cho phép:
  - Tùy chỉnh sâu bằng MSMG Toolkit / NTLite
  - Tạo bản Windows dùng cho Enterprise / Server / Low-end PC
- Giữ nguyên:
  - Kernel gốc
  - Cơ chế cập nhật
  - Bảo mật nền tảng

---

## 🚫 NuxOS11 Creator **KHÔNG** làm gì?

- ❌ Không tích hợp tool kích hoạt Windows
- ❌ Không tự động chạy MAS hay script kích hoạt
- ❌ Không chỉnh sửa bản quyền
- ❌ Không che giấu hành vi hệ thống
- ❌ Không thêm backdoor / malware / telemetry lạ

Người dùng **tự chịu trách nhiệm** về bản quyền Windows.

---

## 📦 Yêu cầu

- Windows 10 / Windows 11
- PowerShell 5.1+
- Quyền Administrator
- ISO Windows 11 hợp lệ (khuyến nghị:
  - Windows 11 LTSC
  - Windows 11 Consumer
  - Windows 11 Enterprise / IoT Enterprise)

---

## 🛠️ Cách sử dụng (tổng quát)

1. Chuẩn bị ISO Windows 11 gốc
2. Chạy script `NuxOS11 Creator`
3. Dán lệnh này vào Powershell: Set-ExecutionPolicy Bypass -Scope Process
4. Chạy scripts: C:/path/to/your/nuxos11/script.ps1 -ISO <letter> -SCRATCH <letter>
5. Chọn:
   - Phiên bản
   - Thành phần cần loại bỏ
6. Build image
7. Tinh chỉnh thêm bằng:
   - MSMG Toolkit
   - NTLite (nếu cần)

> NuxOS11 Creator được thiết kế làm **nền tảng build**, không phải công cụ “1-click”.

---

## 🔐 Bảo mật & Minh bạch

- Mọi script đều ở dạng **plain text**
- Không mã hóa, không obfuscate
- Người dùng có thể:
  - Đọc
  - Kiểm tra
  - Chỉnh sửa

Dự án hướng tới:
- Niềm tin cộng đồng
- Không đánh đổi bảo mật lấy sự tiện lợi

---

## 📜 Giấy phép & pháp lý

- NuxOS11 Creator **không phân phối Windows**
- Không vi phạm EULA của Microsoft nếu:
  - Người dùng có giấy phép hợp lệ
  - Không phân phối ISO đã kích hoạt

Mục đích dự án là **nghiên cứu – tối ưu – triển khai nội bộ**.

---

## 🤝 Đóng góp

Hiện tại dự án:
- Được phát triển bởi **một cá nhân**
- Hoạt động vì cộng đồng
- Không có tài trợ

Mọi đóng góp:
- Bug report
- Ý kiến kỹ thuật
- Đề xuất cải tiến  
đều được hoan nghênh.

---

## 🌌 Về NuxOS

**NuxOS** là dự án tối ưu Windows theo tư duy Linux:
- Ổn định
- Dễ kiểm soát
- Phù hợp Enterprise
- Không chạy theo xu hướng

> *“Hệ điều hành không cần hào nhoáng – chỉ cần đáng tin.”*

---

## 📎 Liên kết

- Website: https://nuxproject.my.canva.site/
- Tài liệu: (đang cập nhật)
- Issue / Feedback: GitHub Repository

---

**NuxOS11 Creator**  
*Built with care, not shortcuts.*
