+++
title = "Chuẩn bị một quy trình ETL"
date = 2024
weight = 6
chapter = false
pre = "<b>3.6 </b>"
+++

#### Sử dụng Glue để thực hiện ETL

1. Nhập và tìm **Glue** ở thanh tìm kiếm.
![Image](/images/3/3-6/1.png?width=40pc)

2. Ở thanh điều hướng bên trái chọn **ETL jobs**.
![Image](/images/3/3-6/2.png?width=20pc)

3. Chọn **Visual ETL** để tạo một quy trình **ETL**.
![Image](/images/3/3-6/3.png?width=40pc)

4. Trong tab **Visual** chọn phần **Sources** để chọn nguồn dữ liệu, ở đây ta chọn **S3**.
![Image](/images/3/3-6/4.png?width=40pc)

5. Chuyển qua phần kế là **Transforms** ta sẽ chọn **Change Schema** để thực hiện các thay đổi trên dữ liệu.
![Image](/images/3/3-6/5.png?width=40pc)

6. Ở phần **Target** ta chọn **Redshift** để load dữ liệu vào.
![Image](/images/3/3-6/6.png?width=40pc)

7. Sau khi chọn xong các thành phần cho quy trình **ETL** thì ta sẽ cấu hình ở từng phần như các hình sau:
   - **S3**
![Image](/images/3/3-6/7.png?width=40pc)

   - **Change Schema**
     - Ta sẽ **Drop** các trường dữ liệu sau : **count, country, state, lat long, latitude, longitude, cltv**.
     - Đối với các trường dữ liệu có tên tên là 2 chữ như **"zip code"** thì ta sẽ đổi lại thành **"zip_code"**. Áp dụng cho tất cả các trường dữ liệu có tên dài.
![Image](/images/3/3-6/8.png?width=40pc)

   - **Redshift**
![Image](/images/3/3-6/9.png?width=40pc)

8. Ta thay đổi tên của job và **save** job lại.
![Image](/images/3/3-6/10.png?width=40pc)

9. Chuyển qua phần **Job details** và gán **IAM role** cho job này là **role** được tạo trong bước 2.
![Image](/images/3/3-6/11.png?width=40pc)

10. Sau khi thực hiện xong quay lại màn hình quản lý các job ta sẽ thấy được job mới được tạo như hình.
![Image](/images/3/3-6/12.png?width=40pc)