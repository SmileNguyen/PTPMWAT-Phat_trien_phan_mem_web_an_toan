# 📝 BÁO CÁO CHUYÊN ĐỀ HỌC PHẦN
# PHÁT TRIẺN PHẦN MỀM WEB AN TOÀN

---

### **📄Thông tin đề tài**

- **Tên đề tài :** CHỐNG CLICKJACKING BẰNG COTENT SECURITY POLICY (CSP) & X-FRAME-OPTIONS – DEMO TẤN CÔNG VÀ CÁCH FIX
- **Giảng viên hướng dẫn :** CẤN ĐỨC ĐIỆP
- **Ngành :** CÔNG NGHỆ THÔNG TIN
- **Chuyên ngành :** CÔNG NGHỆ PHẦN MỀM
- **Lớp :** D19CNTT1B
- **Khóa :** 2024-2027

---

### **🧑‍💻 Thông tin các thành viên trong nhóm**

- **Nhóm trưởng :** Nguyễn Trần Tài
- **Thành viên 1 :** Hoàng Đức Anh
- **Thành viên 2 :** Nguyễn Danh Thái
- **Thành viên 3 :** Trần Thiên Thành
- **Thành viên 4 :** Nguyễn Vũ Thái
  
### **🔎 Nhiệm vụ của từng thành viên**

| Tên thành viên | Nhiệm vụ chính |
|-----------------|----------------|
| Nguyễn Trần Tài  | Lập trình, thiết kế trang web, chuẩn bị máy ảo cho Demo chương trình và đưa ra báo cáo cho nhóm |
| Hoàng Đức Anh    | Xây dựng, thiết kế, chỉnh sửa và hoàn thiện báo cáo của nhóm |
| Nguyễn Danh Thái | [ Đang sắp xếp ] |
| Trần Thiên Thành | [ Đang sắp xếp ] |
| Nguyễn Vũ Thái   | [ Đang sắp xếp ] |

---

### **🖥️ Môi trường sử dụng**

| Thành phần | Phiên bản sử dụng |
|-----------------|----------------|
| Ubuntu    | Ubuntu 20.04 LTS |
| Apache    | 2.4 |
| Browser   | Microsoft Edge |
| IDE       | VS Code |
| VMware    | Workstation 17 Pro (17.5.0 build-22583795) |
| HTML      | HTML5 |
| CSS       | CSS3 |

---

### **📑 Danh sách công việc thực hiện **

- [x] 1. Nghiên cứu lý thuyết: Tìm hiểu khái niệm Clickjacking, phân tích nguyên nhân và cơ chế hoạt động của Clickjacking, tìm hiểu các phương pháp phòng chống:
- [x] 2. Chuẩn bị môi trường thực nghiệm: Cài đặt Ubuntu Server trên VMware Workstation, Cài đặt Apache2 Web Server, Thiết lập mạng giữa máy Windows và Ubuntu, Kiểm tra khả năng truy cập Website.
- [x] 3. Xây dựng Website nạn nhân (Victim Website): Thiết kế giao diện HTML, Tạo Form nhập thông tin, Viết JavaScript xử lý dữ liệu nhập, Đưa Website lên Apache.
- [x] Chỉnh sửa nội dung của một công việc.
- [x] 4. Xây dựng Website tấn công: Tạo Website Attacker, Nhúng Website nạn nhân bằng thẻ <iframe>, Thiết kế giao diện giả mạo, Thực hiện mô phỏng Clickjacking.
- [x] 5. Thực hiện tấn công Clickjacking: Chạy Website Victim, Chạy Website Attacker, Kiểm tra khả năng nhúng Website, Chụp ảnh minh họa quá trình tấn công.
- [x] 6. Triển khai biện pháp phòng chống: Kích hoạt module headers của Apache, Cấu hình Header: X-Frame-Options: DENY, Khởi động lại Apache.
- [x] 7. Kiểm tra sau khi cấu hình: Kiểm tra HTTP Response Header, Xác nhận trình duyệt từ chối iframe, Chụp ảnh kết quả sau khi cấu hình.
- [x] 8. Phân tích và đánh giá: So sánh trước và sau khi áp dụng X-Frame-Options, Đánh giá hiệu quả của giải pháp, So sánh X-Frame-Options với CSP frame-ancestors, Rút ra ưu điểm, nhược điểm.
- [x] 9. Hoàn thiện báo cáo: Viết báo cáo, Chèn hình ảnh minh họa, Trình bày mã nguồn, Viết kết luận và tài liệu tham khảo.

---

### **🖼️ Danh sách hình ảnh trong đề tài**

**Hình 1: Sơ đồ mô hình hệ thống demo Clickjacking:**
![Sơ đồ mô hình](./scrs/sodo.png)

=

**Hình 2: Website nạn nhân:**
![Website nạn nhân](./scrs/H1.png)

=

**Hình 3: Website bị nhúng trong iframe:**
![Website bị nhúng trong iframe](./scrs/H2.png)

=

**Hình 4: Mô phỏng Clickjacking:**
![Mô phỏng Clickjacking](./scrs/H3.png)

=

**Hình 5: Header X-Frame-Options:**
![Header X-Frame-Options](./scrs/H4.png)

=

**Hình 6: Trình duyệt Microsoft Edge thực thi chỉ thị DENY và chặn đứng hoàn toàn mã độc nhúng trang:**
![Trình duyệt Microsoft Edge thực thi](./scrs/H5.png)

---



















