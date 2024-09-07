+++
title = "Dọn dẹp tài nguyên"
date = 2024
weight = 5
chapter = false
pre = "<b>5. </b>"
+++

Chúng ta sẽ dọn dẹp tài nguyên theo thứ tự như sau:
Xóa **Bucket S3**:
   - Truy cập vào mục quản lý **Buckets**.
   - Chọn **Buckets** đã tạo trong **Workshop**.
   - Chọn **Delete** và nhập lại tên **Bucket** như yêu cầu để xóa **Bucket**.

Xóa **IAM role**:
   - Truy cập **console** của **IAM** chọn phần **Roles**.
   - Chọn vào **Role** đã tạo trong **Workshop** và chọn **Delete**.
   - Nhập lại tên **Role** và hoàn thành **Delete**.

Xóa **Databases** trong **Glue**:
   - Truy cập vào **console Glue**.
   - Chọn **Databases** và chọn các **Databases** đã tạo trong **Workshop**.
   - Chọn **Delete** để xóa các **Databases**.

Xóa **Redshift cluster** và **connection Redshift**:
   - Xóa **cluster**
     - Truy cập vào **console Redshift**.
     - Chọn **View all clusters** để xem tất cả các **cluster**.
     - Chọn **cluster** đã tạo và chọn **Action** để thực hiện **Delete**.
     - Sau khi chọn **Delete** trong **Action** ta bỏ chọn **Create final snapshot** và điền **delete** vào ô để hoàn thành **Delete cluster**.

   - Xóa **connection**
     - Truy cập vào **console Glue**.
     - Chọn **connections** ở thanh điều hướng bên trái.
     - Chọn **connection** đã tạo trong **Workshop** và chọn **Action** để thực hiện **Delete**.
     - Sau khi chọn **Delete** trong **Action** tiếp tục xác nhận **Delete** để xóa.

Xóa **Crawler**:
   - Truy cập vào **console Glue**.
   - Chọn **crawlers** ở thanh điều hướng bên trái.
   - Chọn **crawler** đã tạo trong **Workshop** và chọn **Action** để thực hiện **Delete**.
   - Sau khi chọn **Delete** trong **Action** tiếp tục xác nhận **Delete** để xóa.

Xóa **ETL job**:
   - Truy cập vào **console Glue**.
   - Chọn **ETL jobs** ở thanh điều hướng bên trái.
   - Chọn **job** đã tạo trong **Workshop** và chọn **Action** để thực hiện **Delete**.
   - Sau khi chọn **Delete** trong **Action** tiếp tục xác nhận **Delete** để xóa.