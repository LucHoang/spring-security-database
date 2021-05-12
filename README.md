# spring-security-database
Mục tiêu:
Luyện tập tích hợp Spring Security vào trong ứng dụng Spring MVC.

Mô tả:
Trong bài viết lần này, mình sẽ hướng dẫn các bạn xây dựng các chức năng sau:

Đăng nhập

Đăng xuất

Phân quyền

Người dùng được chia là 3 nhóm:

Khách (guest)

Thành viên (member), có quyền ROLE_MEMBER

Quản trị viên (admin), có cả quyền ROLE_MEMBER và ROLE_ADMIN

Ứng dụng của chúng ta sẽ gồm có 4 trang:


Trang đăng nhập /login

Trang chủ /: chỉ cho phép ROLE_MEMBER truy cập

Trang admin /admin: chỉ cho ROLE_ADMIN truy cập

Trang 403 /403: nếu ROLE_MEMBER vào trang admin, sẽ bị redirect về trang này
