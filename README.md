# Authenticate with OTP code through LinOTP software for OpenVPN
Mục tiêu: cải thiện tính bảo mật của việc kết nối các máy khách VPN

Giải pháp: triển khai một lớp bảo mật bổ sung dựa trên xác thực hai yếu tố (OTP) bằng LinOTP
Phương pháp để sử dụng OTP với OpenVPN:
- Xác thực bằng một RADIUS Server được connect tới LinOTP:
  - OpenVPN plugin: openvpn-auth-radius
  - PAM: libpam-radius-auth
- Xác thực bằng PAM thông qua LinOTP web API:
               -   PAM python modul: pam_linotp.py
               -   PAM C modul: pam_linotp
# Tính năng
- Xác thực được chứng nhận OATH và xử lý token
- Framework chính sách mở rộng cho phép định nghĩa chi tiết vai trò của quản trị viên, quy tắc xác thực, token,…
- Hỗ trợ nhiều loại database: MySQL, MariaDB, PostgreSQL, SQLite, Oracle,…
- Cung cấp các API cho việc quản lí, xác thực, user ID resolver, audit log,…
- Hỗ trợ PKCS11 / HSM cho các Mô-đun bảo mật phần cứng như SafeNet Luna SA
# Mô hình triển khai
![image](https://user-images.githubusercontent.com/93479388/184076305-713cb240-5a0b-4e04-af87-69d09707ca9b.png)
![image](https://user-images.githubusercontent.com/93479388/184076339-5fac649d-cd8f-4a71-babd-c4a3196526b8.png)

# Demo 
Link video demo: https://youtu.be/Nxwxxvw3sQ0, https://youtu.be/O1LZkVxBDYE, https://youtu.be/LzVasLMssDc

   

