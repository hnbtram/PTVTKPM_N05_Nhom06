<div align="center">

  # 🍿 HỆ THỐNG QUẢN LÝ RẠP CHIẾU PHIM BETA CINEMAS 🎬
  
  **Đồ án môn học: Phân tích và Thiết kế Phần mềm**
  
  [![University](https://img.shields.io/badge/Tr%C6%B0%E1%BB%9Dng-%C4%90%E1%BA%A1i%20h%E1%BB%8Dc%20Phenikaa-blue?style=for-the-badge)](https://phenikaa-uni.edu.vn/)
  [![Course](https://img.shields.io/badge/M%C3%B4n%20h%E1%BB%8Dc-Ph%C3%A2n%20t%C3%ADch%20%26%20Thi%E1%BA%BFt%20k%E1%BA%BF%20PM-orange?style=for-the-badge)]()
  [![Class](https://img.shields.io/badge/L%E1%BB%9Bp-N05%20--%20Nh%C3%B3m%2006-success?style=for-the-badge)]()
  
  **Giảng viên hướng dẫn:** TS. Trương Đức Phương
  
</div>

---

## 📖 Giới thiệu dự án

Dự án tập trung vào việc **phân tích và thiết kế** hệ thống website đặt vé xem phim trực tuyến cho chuỗi rạp Beta Cinemas. Hệ thống được xây dựng nhằm giải quyết bài toán quản lý và đặt vé cho hơn **21 cụm rạp**, phục vụ hàng triệu khách hàng mỗi năm.

Báo cáo đi sâu vào việc xác định yêu cầu, mô hình hóa hệ thống bằng ngôn ngữ **UML**, thiết kế kiến trúc phần mềm (**MVC**, **BCE**), thiết kế cơ sở dữ liệu quan hệ và thiết kế giao diện người dùng.

---

## ✨ Chức năng chính

Hệ thống được thiết kế phục vụ 3 nhóm tác nhân chính:

<details open>
<summary><b>👤 1. Khách hàng (Customer)</b></summary>
<br>

*   **Quản lý tài khoản:** Đăng ký, đăng nhập, cập nhật thông tin cá nhân.
*   **Khám phá phim & rạp:** Xem danh sách phim (đang chiếu, sắp chiếu), chi tiết phim, lịch chiếu theo rạp, giá vé, tin tức & ưu đãi.
*   **Đặt vé trực tuyến:** Chọn suất chiếu, chọn ghế (giữ ghế 10 phút), áp dụng voucher, thanh toán qua cổng trực tuyến (VNPAY, MoMo...).
*   **Quản lý vé:** Xem lịch sử đặt vé, nhận vé điện tử (mã QR).
</details>

<details open>
<summary><b>🛡️ 2. Quản trị viên (Administrator)</b></summary>
<br>

*   **Quản lý danh mục:** Tài khoản, Phim, Rạp, Phòng chiếu, Ghế, Lịch chiếu, Giá vé.
*   **Quản lý kinh doanh:** Đơn đặt vé, Thanh toán, Voucher, Phản hồi khách hàng, Tin tức & Nhượng quyền.
*   **Báo cáo & Thống kê:** Thống kê doanh thu, thống kê vé theo thời gian/phim/rạp.
</details>

---

## 🏗️ Kiến trúc & Thiết kế hệ thống

| Thành phần | Chi tiết thiết kế |
| :--- | :--- |
| 🏛️ **Kiến trúc phần mềm** | Multi-tier / N-tier kết hợp mô hình **MVC** (Model-View-Controller) và **DAO** (Data Access Object). |
| 📐 **Mô hình phân tích** | **BCE** (Boundary - Control - Entity) trực quan hóa bằng UML. |
| 🗄️ **Cơ sở dữ liệu** | CSDL quan hệ gồm **18 bảng** (SQL Server / PostgreSQL / MySQL), đảm bảo toàn vẹn dữ liệu, chống trùng ghế và trùng lịch chiếu. |
| 🔌 **Tích hợp bên thứ 3** | Cổng thanh toán (VNPAY, MoMo, ATM/VISA), Email/SMS, Google Maps API. |

---

## 📂 Cấu trúc tài liệu trong Repo

Repository này lưu trữ toàn bộ quá trình phân tích và thiết kế hệ thống:

```text
📦 Beta-Cinemas-System
 ┣ 📂 docs/               # 📄 Báo cáo chi tiết (File Word/PDF)
 ┣ 📂 diagrams/           # 📊 Biểu đồ UML
 ┃ ┣ 📜 Use_Cases/        # (Tổng quát & Chi tiết)
 ┃ ┣ 📜 Sequence/         # (29 Use Case)
 ┃ ┣ 📜 Activity/         # (29 Use Case)
 ┃ ┗ 📜 Class_Diagrams/   # (Class Diagrams & BCE Diagrams)
 ┣ 📂 database/           # 🗄️ Thiết kế CSDL (ERD & Script tạo bảng)
 ┗ 📂 ui-ux/              # 🎨 Thiết kế giao diện (Wireframe / Mockup)
```
## 👥 Thành viên nhóm thực hiện

| STT | Họ và Tên | MSSV | Vai trò |
| :---: | :--- | :---: | :--- |
| 1 | **Hoàng Nhật Bảo Trâm** | `24100260` | 👑 Nhóm trưởng |
| 2 | **Nguyễn Thùy Dương** | `24107946` | 👨‍💻 Thành viên |
| 3 | **Tô Quý Đạt** | `24100312` | 👨‍💻 Thành viên |
| 4 | **Hoàng Quốc Khánh** | `24100019` | 👨‍💻 Thành viên |
| 5 | **Nguyễn Bảo Nam** | `24100179` | 👨‍💻 Thành viên |

---

## 📚 Tài liệu tham khảo

1. **Object Management Group (OMG)**, *OMG Unified Modeling Language (UML), Version 2.5.1*, 2017.
   🔗 [Truy cập tại đây](https://www.omg.org/spec/UML/2.5.1)
2. **Martin Fowler**, *UML Distilled: A Brief Guide to the Standard Object Modeling Language*, 3rd Edition, Addison-Wesley Professional, 2003.
3. **Ian Sommerville**, *Software Engineering*, 10th Edition, Pearson, 2015.
4. **Beta Cinemas**, *Website chính thức Beta Cinemas*.
   🔗 [Truy cập tại đây](https://betacinemas.vn/)
