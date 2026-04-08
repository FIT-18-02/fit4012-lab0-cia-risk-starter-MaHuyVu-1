# Lab 01 Answers
## CIA & Risk: Hệ thống lưu điểm

**Họ và tên:** Ma Huy Vũ

**MSSV:** 1871020669

**Lớp/Nhóm:** CNTT-1802

---

## 1. Assets
Liệt kê ít nhất 2 assets cần bảo vệ.

- Asset 1:Cơ sở dữ liệu người dùng (thông tin cá nhân, tài khoản, mật khẩu)
- Asset 2:Dữ liệu giao dịch (đơn hàng, hóa đơn, thanh toán)
- Asset 3 (nếu có):Hệ thống máy chủ (server, API, source code)

---

## 2. Mapping CIA
Ghép từng sự cố với CIA.

- Sự cố A -> Confidentiality (Bảo mật)
- Sự cố B -> Integrity (Toàn vẹn)
- Sự cố C -> Availability (Sẵn sàng)

---

## 3. Phân tích sự cố B
- Threat:Hacker tấn công, thay đổi dữ liệu trong database
- Vulnerability:Không kiểm tra đầu vào (SQL Injection)
                Thiếu phân quyền người dùng
                Không mã hóa dữ liệu quan trọng
- Mitigation:Sử dụng Prepared Statement để chống SQL Injection
             Áp dụng phân quyền (Role-based Access Control)
             Ghi log và kiểm tra thay đổi dữ liệu
             Sao lưu dữ liệu thường xuyên

---

## 4. Reflection
Viết 5-7 dòng.

Qua bài này, em hiểu rõ hơn tầm quan trọng của việc bảo mật hệ thống thông tin. Mỗi hệ thống đều có các tài sản quan trọng cần được bảo vệ như dữ liệu người dùng và dữ liệu giao dịch. Việc áp dụng mô hình CIA giúp phân loại các rủi ro một cách rõ ràng hơn. Đồng thời, em nhận ra rằng các lỗ hổng như SQL Injection hay thiếu phân quyền có thể gây hậu quả nghiêm trọng. Vì vậy, khi phát triển phần mềm, cần chú trọng đến bảo mật ngay từ đầu. Điều này giúp hệ thống an toàn và đáng tin cậy hơn.

---

## 5. Bonus Flag
`FIT4012{A-?-B-?-C-?}`

Flag của em:FIT4012{A-C-B-I-C-A}
