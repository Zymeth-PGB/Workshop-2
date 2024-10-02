+++
title = "Tạo các database để chứa dữ liệu"
date = 2024
weight = 3
chapter = false
pre = "<b>3.3 </b>"
+++

#### Tạo Database

1. Nhập và tìm kiếm **Glue** ở thanh tìm kiếm sau đó ấn chọn.
![Image](/Workshop-2/images/3/3-3/1.png?width=40pc)

2. Ở thanh điều hướng bên trái chọn **Database** ở mục **Data Catalog**.
![Image](/Workshop-2/images/3/3-3/2.png?width=20pc)

3. Chọn **Add Database** để thêm **database**.
![Image](/Workshop-2/images/3/3-3/3.png?width=40pc)

4. Nhập tên sau đó chọn **Create Database** để tạo **database**.
![Image](/Workshop-2/images/3/3-3/4.png?width=40pc)

5. Khi tạo thành công sẽ xuất hiện các **database** đã tạo ở phần khung đỏ
![Image](/Workshop-2/images/3/3-3/5.png?width=40pc)

{{% notice note %}}
Trong bước thứ **5** bạn có thể thấy ở đây khoanh vùng 2 **database** là do trong **workshop** này ta sẽ sử dụng 1 **database** cho việc lấy dữ liệu từ **S3** và cái thứ 2 là để đưa dữ liệu sau khi **transform** vào **Redshift**. Cho nên bạn phải tạo 2 **database** như hình trên.
{{% /notice %}}