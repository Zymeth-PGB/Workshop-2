+++
title = "Tạo Crawler"
date = 2024
weight = 5
chapter = false
pre = "<b>3.5 </b>"
+++

#### Tạo các Crawler

{{% notice note %}}
Ta sẽ tạo 2 **crawler** để phục vụ cho mục tiêu lấy **schema** từ **S3** và lấy **schema** từ **Redshift** đã tạo ở bước trước. Nên một số bước giống nhau sẽ chỉ để 1 ảnh còn những bước có khác biệt sẽ có hướng dẫn mỗi **crawler** nên làm như thế nào.
{{% /notice %}}

1. Nhập và tìm kiêm **Glue** trên thanh tìm kiếm.
![Image](../../images/3/3-5/1.png?width=40pc)

2. Ở thanh điều hướng bên trái chọn **Crawler**.
![Image](../../images/3/3-5/2.png?width=20pc)

3. Sau khi chọn **Crawler** sẽ hiện ra danh sách các **Crawler** và các tùy chọn khác. Ta chọn **Create crawler** để tạo **crawler** mới.
![Image](../../images/3/3-5/3.png?width=40pc)

4. Nhập tên cho mỗi **Crawler** phù hợp với chức năng của nó là lấy **schema** từ đâu.
![Image](../../images/3/3-5/4.png?width=40pc)

5. Bước 2 chọn **Not yet** và sẽ thêm một **data source** vào.
![Image](../../images/3/3-5/5.png?width=40pc)

6. Ở mỗi **Crawler** sẽ có cách lựa chọn **data source** khác nhau như sau: 
   - Đối với **Crawler** lấy **schema** từ **S3** thì chọn như hình:
     - Đường dẫn đến **S3** ta sẽ chọn **bucket** được tạo ở bước [số 1](../1-Create-S3/)
![Image](../../images/3/3-5/6-1.png?width=40pc)

   - Đối với **Crawler** lấy **schema** từ **Redshift** thì chọn như hình:
     - Ở mục **Include Path** thì ta sẽ thêm đường dẫn đến **table** ta đã tạo ở bước trước trong **Query Editor**.
![Image](../../images/3/3-5/6-2.png?width=40pc)

7. Sau khi lựa chọn **data source** xong ta sẽ được **data source** như 2 hình bên dưới. Chọn **next** để đến với bước tiếp theo.
   - **Crawler S3**
![Image](../../images/3/3-5/7-1.png?width=40pc)

   - **Crawler Redshift**
![Image](../../images/3/3-5/7-2.png?width=40pc)

8. Chọn **IAM role** đã tạo ở bước [số 2](../2-create-iam-role/).
![Image](../../images/3/3-5/8.png?width=40pc)

9. Chọn **database** phù hợp cho mỗi **Crawler** đã được tạo ở bước [số 3](../3-create-table/):
   - **Crawler S3**
![Image](../../images/3/3-5/9-1.png?width=40pc)

   - **Crawler Redshift**
![Image](../../images/3/3-5/9-2.png?width=40pc)

10.  Kiểm tra lại các lựa chọn nếu ổn thì chọn **Create crawler**:
    - **Crawler S3**
![Image](../../images/3/3-5/10-1.png?width=40pc)

    - **Crawler Redshift**
![Image](../../images/3/3-5/10-2.png?width=40pc)

11.  Khi tạo thành công thì sẽ được 2 **crawler** có **State** là **Ready** như hình.
![Image](../../images/3/3-5/11.png?width=40pc)