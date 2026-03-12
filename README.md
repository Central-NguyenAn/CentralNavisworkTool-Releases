<p align="center">
  <img src="images/icon.png" alt="CentralTool Logo" width="80"/>
</p>

<h1 align="center">CentralTool Plugin</h1>

<p align="center">
  <strong>Plugin mở rộng cho Autodesk Navisworks Manage</strong><br/>
  Bộ công cụ tự động hóa quy trình BIM — Search Sets, WBS Matching, Quantification & hơn thế nữa.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-Navisworks%20Manage-0696D7?style=for-the-badge&logo=autodesk&logoColor=white" alt="Platform"/>
  <img src="https://img.shields.io/badge/versions-2023%20%7C%202024-green?style=for-the-badge" alt="Versions"/>
  <img src="https://img.shields.io/badge/.NET%20Framework-4.8-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" alt=".NET"/>
  <img src="https://img.shields.io/badge/license-MIT-brightgreen?style=for-the-badge" alt="License"/>
</p>

---

## 📥 Tải về (Download)

👉 **[Tải phiên bản mới nhất tại đây](https://github.com/Central-NguyenAn/CentralTool-Plugin/releases/latest)**

| File | Mô tả |
|---|---|
| `CentralTool.bundle.zip` | Plugin đầy đủ cho cả Navisworks 2023 & 2024 |

---

## 💻 Yêu cầu hệ thống

| Thành phần | Yêu cầu |
|---|---|
| **Hệ điều hành** | Windows 10/11 (64-bit) |
| **Phần mềm** | Autodesk Navisworks Manage **2023** hoặc **2024** |
| **.NET Framework** | 4.8 (thường đã có sẵn trên Windows 10/11) |

---

## 📦 Hướng dẫn cài đặt

### Bước 1: Tải file

Vào trang [**Releases**](https://github.com/Central-NguyenAn/CentralTool-Plugin/releases/latest) và tải file `CentralTool.bundle.zip`.

### Bước 2: Giải nén

Giải nén file `.zip`, bạn sẽ được thư mục `CentralTool.bundle` có cấu trúc:

```
CentralTool.bundle/
├── PackageContents.xml
└── Contents/
    ├── 2023/          ← cho Navisworks 2023
    │   ├── CentralTool.dll
    │   ├── MiniExcel.dll
    │   └── Images/
    └── 2024/          ← cho Navisworks 2024
        ├── CentralTool.dll
        ├── MiniExcel.dll
        └── Images/
```

### Bước 3: Copy vào thư mục Plugin

Copy **toàn bộ** thư mục `CentralTool.bundle` vào:

```
%AppData%\Autodesk\ApplicationPlugins\
```

> 💡 **Mẹo**: Mở File Explorer, dán đường dẫn trên vào thanh địa chỉ và nhấn Enter.

### Bước 4: Khởi động Navisworks

Mở **Navisworks Manage** → Tab **"Central"** sẽ xuất hiện trên thanh Ribbon.

---

## ✨ Tính năng

### 🔍 Search Set Manager
Quản lý và tạo **Search Sets** trực quan qua giao diện WPF:
- Tạo và chỉnh sửa điều kiện tìm kiếm
- Quản lý toán tử so sánh
- Xử lý giá trị rỗng và điều kiện đặc biệt

### 🏗️ Trợ lý WBS (WBS Matcher)
Tự động đối chiếu và ánh xạ **Work Breakdown Structure** với đối tượng trong mô hình:
- Data Inspector kiểm tra dữ liệu
- Dịch vụ khớp nối WBS tự động
- Giao diện quản lý trực quan

### 📐 Auto Formula (Quantification Formula)
Tự động áp dụng **công thức tính khối lượng** trong Navisworks:
- Kiểm tra cấu trúc DB Quantification
- Ánh xạ công thức tự động

### 📊 Quantification Updater
Cập nhật dữ liệu Quantification hàng loạt.

---

## 🚀 Sử dụng

Sau khi cài đặt, mở **Navisworks Manage** và tìm tab **"Central"** trên thanh Ribbon:

| Nút | Chức năng |
|---|---|
| **Search Sets** | Mở cửa sổ quản lý Search Sets |
| **Trợ lý WBS** | Mở công cụ khớp nối WBS |
| **Auto Formula** | Mở công cụ tự động áp dụng công thức Quantification |

---

## 🔄 Cập nhật

Để cập nhật plugin:
1. Tải phiên bản mới từ [Releases](https://github.com/Central-NguyenAn/CentralTool-Plugin/releases/latest)
2. **Đóng Navisworks**
3. Xóa thư mục `CentralTool.bundle` cũ trong `%AppData%\Autodesk\ApplicationPlugins\`
4. Giải nén và copy thư mục mới vào

---

## ❓ Câu hỏi thường gặp (FAQ)

<details>
<summary><strong>Tab "Central" không xuất hiện sau khi cài đặt?</strong></summary>

- Đảm bảo bạn đang dùng **Navisworks Manage** (không phải Simulate hay Freedom)
- Kiểm tra thư mục `CentralTool.bundle` nằm đúng trong `%AppData%\Autodesk\ApplicationPlugins\`
- Kiểm tra file `PackageContents.xml` nằm ở thư mục gốc `CentralTool.bundle\`
- Thử khởi động lại Navisworks

</details>

<details>
<summary><strong>Plugin có hoạt động với Navisworks Simulate hay Freedom không?</strong></summary>

Không. CentralTool chỉ hỗ trợ **Navisworks Manage** do sử dụng các API chỉ có trong phiên bản Manage.

</details>

<details>
<summary><strong>Có cần cài thêm gì không?</strong></summary>

Không. Plugin chỉ cần .NET Framework 4.8 (đã có sẵn trên Windows 10/11). Tất cả dependencies đã được đóng gói sẵn.

</details>

---

## 📝 Ghi chú phiên bản (Changelog)

Xem chi tiết tại trang [Releases](https://github.com/Central-NguyenAn/CentralTool-Plugin/releases).

---

## 📧 Liên hệ & Báo lỗi

Nếu gặp vấn đề khi sử dụng, vui lòng tạo [Issue](https://github.com/Central-NguyenAn/CentralTool-Plugin/issues/new) trên GitHub.

---

<p align="center">
  <sub>Built with ❤️ for BIM Engineers</sub>
</p>
