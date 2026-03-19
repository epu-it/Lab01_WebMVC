# Lab01_WebMVC

BÀI TẬP: HỆ THỐNG BÁN HÀNG + BLOG SẢN PHẨM

## Chức năng cần xây dựng
| # | Chức năng | Kỹ thuật | Mô tả |
| :--- | :--- | :--- | :--- |
| 1 | Đăng ký / Đăng nhập | Identity + Cookie | Register, Login, Logout, Lockout |
| 2 | Danh mục & Sản phẩm | EF Core, Razor, Paging | Trang công khai xem sản phẩm |
| 3 | Giỏ hàng | Session | Thêm/xóa/sửa số lượng, không cần đăng nhập |
| 4 | Đặt hàng | EF Core Transaction | Tạo Order từ Cart, trừ tồn kho |
| 5 | Blog sản phẩm | Razor, Rich content | Bài viết giới thiệu, gắn với sản phẩm |
| 6 | Upload hình ảnh | IFormFile | Ảnh sản phẩm, ảnh blog |
| 7 | Admin Panel | `[Authorize(Roles)]` | CRUD product, blog, xem order |
| 8 | Cache & Session | IMemoryCache | Cache menu, session giỏ hàng, lịch sử xem |

## Các gói cần cài đặt
### EF Core + SQLite
dotnet add package Microsoft.EntityFrameworkCore.Sqlite  
dotnet add package Microsoft.EntityFrameworkCore.Design  
dotnet add package Microsoft.EntityFrameworkCore.Tools

### Identity
dotnet add package Microsoft.AspNetCore.Identity.EntityFrameworkCore

### AutoMapper (tùy chọn – giúp map ViewModel)
dotnet add package AutoMapper.Extensions.Microsoft.DependencyInjection

### EF Tool (cài 1 lần dùng mãi)
dotnet tool install --global dotnet-ef

