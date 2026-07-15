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
| Nguyễn Trần Tài  | Lập trình, thiết kế trang web, chuẩn bị máy ảo cho Demo chương trình và đưa ra báo cáo cho nhóm, push và chỉnh sửa link github của nhóm |
| Hoàng Đức Anh    | Xây dựng, thiết kế, chỉnh sửa và hoàn thiện báo cáo của nhóm |
| Nguyễn Danh Thái | [ Đang sắp xếp ] |
| Trần Thiên Thành | [ Đang sắp xếp ] |
| Nguyễn Vũ Thái   | [ Đang sắp xếp ] |

---

### **📒 Giới thiệu đề tài**

**1. Giới thiệu**

- Trong thời đại chuyển đổi số, các ứng dụng web ngày càng được sử dụng rộng rãi trong nhiều lĩnh vực như thương mại điện tử, ngân hàng, giáo dục, y tế và các dịch vụ công trực tuyến. Cùng với sự phát triển đó, vấn đề bảo mật ứng dụng web ngày càng trở nên quan trọng nhằm bảo vệ thông tin người dùng và đảm bảo hệ thống hoạt động an toàn trước các cuộc tấn công trên Internet.

- Một trong những hình thức tấn công phổ biến nhưng thường bị xem nhẹ là Clickjacking. Đây là kỹ thuật tấn công lợi dụng khả năng nhúng một trang web hợp pháp vào bên trong một trang web độc hại bằng thẻ iframe, sau đó sử dụng các kỹ thuật che giấu hoặc tạo giao diện giả nhằm đánh lừa người dùng thực hiện các thao tác ngoài ý muốn như nhấn nút, xác nhận giao dịch, thay đổi thông tin tài khoản hoặc cấp quyền truy cập. Người dùng thường không nhận biết được mình đang tương tác với trang web thật hay một lớp giao diện giả được tạo ra bởi kẻ tấn công.

- Để phòng chống Clickjacking, các máy chủ web hiện nay thường sử dụng hai cơ chế bảo mật quan trọng là HTTP Header X-Frame-Options và Content Security Policy (CSP) với chỉ thị frame-ancestors. Các cơ chế này cho phép máy chủ kiểm soát việc trang web có được phép hiển thị bên trong iframe của các website khác hay không, từ đó ngăn chặn hiệu quả các cuộc tấn công Clickjacking.

- Trong đề tài này, nhóm em tiến hành xây dựng một môi trường mô phỏng gồm máy chủ Ubuntu chạy Apache Web Server trên VMware, xây dựng website nạn nhân (Victim Website) và website tấn công (Attacker Website) để minh họa cơ chế hoạt động của Clickjacking. Sau đó tiến hành cấu hình các Header bảo mật trên Apache nhằm ngăn chặn việc nhúng website vào iframe và đánh giá hiệu quả của giải pháp thông qua quá trình kiểm thử thực tế.

- Thông qua đề tài, nhóm em có cơ hội tìm hiểu nguyên lý hoạt động của lỗ hổng Clickjacking, cách triển khai các biện pháp phòng chống trên máy chủ Apache cũng như nâng cao kiến thức về bảo mật ứng dụng web theo các khuyến nghị của OWASP và các tiêu chuẩn bảo mật hiện đại.

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**2. Lý do chọn đề tài**

Đề tài "Chống Clickjacking bằng Content Security Policy (CSP) và X-Frame-Options – Demo tấn công và cách khắc phục" được nhóm em lựa chọn vì những lý do sau:

- Clickjacking là một lỗ hổng bảo mật phổ biến, có thể gây ảnh hưởng nghiêm trọng đến người dùng và các ứng dụng web.
- Các biện pháp phòng chống như X-Frame-Options và Content Security Policy (CSP) tương đối dễ triển khai nhưng mang lại hiệu quả bảo vệ cao.
- Đề tài có thể xây dựng mô hình thực nghiệm đơn giản bằng Apache và VMware mà không yêu cầu hạ tầng phức tạp.
- Phù hợp với nội dung môn học về phát triển phần mềm an toàn và bảo mật ứng dụng web.
- Giúp người học tiếp cận quy trình từ mô phỏng tấn công, phát hiện lỗ hổng đến triển khai và đánh giá giải pháp phòng chống.

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**3. Mục tiêu của đề tài**

Đề tài nhóm em hướng đến các mục tiêu sau:

- Tìm hiểu nguyên lý hoạt động của tấn công Clickjacking.
- Xây dựng môi trường mô phỏng cuộc tấn công bằng Apache Web Server trên Ubuntu.
- Thực hiện mô phỏng Clickjacking bằng kỹ thuật iframe.
- Triển khai cơ chế phòng chống bằng X-Frame-Options và giới thiệu Content Security Policy (CSP).
- Kiểm tra và đánh giá hiệu quả của các biện pháp bảo mật sau khi áp dụng.
- Rút ra kinh nghiệm và đề xuất các khuyến nghị nhằm nâng cao an toàn cho các ứng dụng web.


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

### 📟 Hướng dẫn chạy chương trình 

**1. Chuẩn bị môi trường**

**Phần cứng**
- Máy tính cài Windows 10/11.
- RAM tối thiểu: 8 GB (khuyến nghị 16 GB).
- VMware Workstation.

**Phần mềm**

-VMware Workstation
-Ubuntu Server 20.04 hoặc 22.04
-Apache2
-Google Chrome hoặc Microsoft Edge
-Visual Studio Code (để chỉnh sửa mã nguồn)

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**2. Khởi động máy ảo Ubuntu**

Mở VMware Workstation.

Khởi động máy ảo Ubuntu.

Đăng nhập tài khoản Ubuntu.

Kiểm tra địa chỉ IP:

 ```bash
hostname -I
```

Ví dụ:

 ```bash
192.168.1.224
```

Địa chỉ IP này sẽ được sử dụng để truy cập Website từ máy Windows.

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**3. Khởi động Apache**

Kiểm tra trạng thái Apache:

 ```bash
sudo systemctl status apache2
```

Nếu Apache chưa chạy:

 ```bash
sudo systemctl start apache2
```

Hoặc:

```bash
sudo systemctl restart apache2
```

Kiểm tra:

```bash
active (running)
```

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**4. Kiểm tra Website Victim**

Trên Windows mở trình duyệt.

Truy cập:

```bash
http://192.168.1.224
```

Nếu cấu hình đúng sẽ xuất hiện Website:

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**5. Chạy Website Attacker**

Mở thư mục chứa Website tấn công.

Ví dụ:

```bash
Attack/index.html
```

Mở bằng Google Chrome.

Hoặc chạy bằng VS Code Live Server.

Website sẽ hiển thị:

```bash
🎁 ĐIỀN THÔNG TIN ĐỂ NHẬN QUÀ MIỄN PHÍ 🎁
```

và nhúng Website Victim bằng iframe.

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**6. Thực hiện mô phỏng Clickjacking**
Người dùng truy cập Website Attacker.

Website Victim được tải bên trong:

```bash
<iframe src="http://192.168.1.224"></iframe>
```

Người dùng tưởng rằng đang thao tác trên Website Attacker nhưng thực tế lại đang nhấp chuột lên Website Victim.

Điều này mô phỏng thành công cuộc tấn công Clickjacking.

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**7. Cấu hình chống Clickjacking**

Mở file cấu hình Apache:

```bash
sudo nano /etc/apache2/sites-available/000-default.conf
```

Thêm:

```bash
Header always set X-Frame-Options "DENY"
```

Ví dụ:

```bash
<VirtualHost *:80>

DocumentRoot /var/www/html

Header always set X-Frame-Options "DENY"

</VirtualHost>
```

Lưu file.

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**8. Khởi động lại Apache**

```bash
sudo systemctl restart apache2
```

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**9. Kiểm tra Header**

Nếu chưa cài curl:

```bash
sudo apt update
sudo apt install curl -y
```

Sau đó:

```bash
curl -I http://localhost
```

Kết quả mong muốn:

```bash
HTTP/1.1 200 OK
X-Frame-Options: DENY
```

Điều này chứng minh máy chủ đã gửi Header chống Clickjacking.






 

---





### **🖼️ Danh sách hình ảnh trong đề tài**

**Hình 1: Sơ đồ mô hình hệ thống demo Clickjacking:**
![Sơ đồ mô hình](./scrs/sodo.png)

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**Hình 2: Website nạn nhân:**
![Website nạn nhân](./scrs/H1.png)

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**Hình 3: Website bị nhúng trong iframe:**
![Website bị nhúng trong iframe](./scrs/H2.png)

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**Hình 4: Mô phỏng Clickjacking:**
![Mô phỏng Clickjacking](./scrs/H3.png)

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**Hình 5: Header X-Frame-Options:**
![Header X-Frame-Options](./scrs/H4.png)

⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀ ⠀

**Hình 6: Trình duyệt Microsoft Edge thực thi chỉ thị DENY và chặn đứng hoàn toàn mã độc nhúng trang:**
![Trình duyệt Microsoft Edge thực thi](./scrs/H5.png)

---



















