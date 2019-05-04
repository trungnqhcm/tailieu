# 1. Giới thiệu

>Bài hướng dẫn này sẽ chỉ bạn các bước cơ bản để tạo một Web API sử dụng ASP.net Core của Microsoft.
>
Tưởng tượng bạn đang làm việc cho một công ty bán bán đồ cho Thú cưng. Quản lý yêu cầu bạn phát triển một RESTful dịch vụ quản lý hàng cho cửa hàng Online của công ty. Dịch vụ API yêu cầu cần có hỗ trợ `Thêm` ` Xoá` `Sửa` `Xem chi tiết`  các sản phẩm ( Là hoạt động cơ bản của HTTP có thể gọi là `Read` `Update` `Delete` - **CRUD** )

Bài này sẽ hướng dẫn tạo nên một `cross-platform` RESTful với `ASP.NET Core web API` viết bằng `.NET core` và `C#`. Chúng ta cũng sẽ được học cách làm việc Database. `Entity Framework` (EF) sẽ được sử dụng như **O**bject-**R**elational **M**apper (O/RM) (Chuyển đổi CSDL giưã các hệ thống).

Chuỗi bài này sẽ [.NET Core CLI](https://docs.microsoft.com/dotnet/core/tools/) để hướng dẫn phát triển một Web API. Sau khi hoàn thành chuỗi đề Hướng dẫn này, bạn có thể áp dụng để phát triển ở các môi trường khác như `Visual Studio` (Window), `Visual Studio for Mac`(MacOS) hoặc `Visual Studio Code` (Windows, Linux, & macOS).

## Mục tiêu
Trong chuỗi bài này bạn sẽ được học:
- [ ] Sử dụng .NET Core CLI để tạo một project ASP.NET Core web API.
- [ ] Tạo Database sản phẩm
- [ ] Thêm CRUD vào web API
- [ ] Test Web API

## Điều kiện tiên quyết
- Nắm được cơ bản về C#
- Nắm kiến thức về RESTful và HTTP

# 2. Tạo project web API
Sử dụng .NET core CLI là cách đơn giản nhất để tạo ASP.NET Core web API. CLI đã được tích hợp sẵn vào trong Azure Cloud Shell, nên rất thuận tiện trong việc phát triện trên Azure.
## Tạo mới Project
### Khung sườn và mổ xẻ thành phần
1. Chạy dòng .NET Core CLI command trên CMD
```
dotnet new webapi -o contoso-pets/src/ContosoPets.Api
```
Như vậy Prject API mới đã được khởi tạo.
Dòng lệnh trên khởi tạo dựa trên khung mẫu sẵn của ASP.NET Core. `webapi` dựng sẵn viết bằng  *C#*. `contoso-pets/src/ContosoPets.Api` là đường dẫn khởi tạo. Tên của Project này là `ContosoPets.Api` được thể hiện trong đường dẫn.

2. Chạy dòng lệnh
```
cd ./contoso-pets/src/ContosoPets.Api
``` 
`cd` vào thư mục chưa project
 
 3. Chạy dòng lệnh
```
code .
```
Project `ContosoPets.Api` sẽ được mở trực tiếp ở editor.

4. Phân tích cấu trúc file
Name | Decription
-------- | -----
*_Controllers/_* | $1600
Phone | $12
Pipe | $1
> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI0NDI1NTAzOCwtMTQ5MzIzOTAzMCwtNj
gxMjk4MjQxLC0xOTAyNTYwMzMzLDI2Mzk5Mjg2Ml19
-->