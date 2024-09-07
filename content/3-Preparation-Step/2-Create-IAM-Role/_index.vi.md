+++
title = "Tạo IAM Role"
date = 2024
weight = 2
chapter = false
pre = "<b>3.2 </b>"
+++

#### Tạo IAM role chung cho các dịch vụ

1. Nhập và tìm kiếm **IAM** ở thanh tìm kiếm, sau đó ấn chọn vào **IAM**.
![Image](/images/3/3-2/1.png?width=40pc)

2. Ở thanh điều hướng bên trái chọn **Roles** để truy cập vào bảng điều khiển **Roles**.
![Image](/images/3/3-2/2.png?width=20pc)

3. Ấn vào **Create role** để tạo **role**
![Image](/images/3/3-2/3.png?width=40pc)

4. Chọn **AWS Service** và điền **Glue** vào **Service or use case** để chọn **Glue**. Chọn **Next** để qua bước tiếp theo.
![Image](/images/3/3-2/4.png?width=40pc)

5. Tìm và chọn **AdministratorAccess** sau đó ấn **Next** để qua bước tiếp theo.
![Image](/images/3/3-2/5-1.png?width=40pc)
![Image](/images/3/3-2/5-2.png?width=40pc)

6. Ở bước này bạn chỉ việc điền tên và ấn **Create role**, các **step** khác vẫn để mặc định.
![Image](/images/3/3-2/6-1.png?width=40pc)
![Image](/images/3/3-2/6-2.png?width=40pc)

7. Sau khi tạo **role** xong bạn có thể kiểm tra xem mình có tạo được chưa trong danh sách các **role**, ở đây mình đã tạo thành công như ô khoanh màu đỏ
![Image](/images/3/3-2/7.png?width=40pc)