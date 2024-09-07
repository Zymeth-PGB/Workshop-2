+++
title = "Thiết lập và kết nối tới Redshift"
date = 2024
weight = 4
chapter = false
pre = "<b>3.4 </b>"
+++

#### Tạo Redshift Cluster

1. Nhập và tìm kiếm **Redshift** trong thanh tìm kiếm sau đó ấn chọn **Redshift**.
![Image](/images/3/3-4/1.png?width=40pc)

2. Ở thanh điều hướng bên trái chọn **Cluster**.
![Image](/images/3/3-4/2.png?width=20pc)

3. Chọn **Create Cluster** để tạo một **Cluster** mới.
![Image](/images/3/3-4/3.png?width=40pc)

4. Nhập tên **Cluster** và chọn các tùy chọn như hình, do mục tiêu là làm để tìm hiểu nên ta chọn **ra3.xlplus** để tiết kiệm chi phí.
![Image](/images/3/3-4/4.png?width=40pc)

5. Nhập tên cho **Admin User** và chọn nhập mật khẩu thủ công để đặt mật khẩu của bạn.
{{% notice note %}}
**Username** và **password** này được sử dụng để tạo kết nối tới **Query Editor** nên bạn cần ghi nhớ để có thể kết nối đến **Query Editor**.
{{% /notice %}}

![Image](/images/3/3-4/5.png?width=40pc)

6. Sử dụng các cài đặt bổ sung mặc định và ấn **Create Cluster** để tạo **Cluster**.
![Image](/images/3/3-4/6.png?width=40pc)

7. Sau khi tạo xong **Cluster**, nhìn vào thanh điều hướng bên trái và chọn **Query Editor V2**.
![Image](/images/3/3-4/7.png?width=20pc)

8. Tại màn hình **Query Editor** chọn vào dấu 3 chấm sau đó chọn **Create connection** để tạo kết nối tới **Query Editor**.
![Image](/images/3/3-4/8.png?width=40pc)

9. Khi chọn **Create connection** sẽ hiển thị lên màn hình các lựa chọn để liên kết đến **Query Editor**, ta chọn như hình và điền **Username**, **password** đã tạo trước đó vào.
![Image](/images/3/3-4/9.png?width=40pc)

10.  Sau khi tạo kết nối đến **Query Editor** thành công ta sẽ dán **Script SQL** được tạo sẵn ở [Github](https://github.com/Zymeth-PGB/AWS-Basic-Data-Pipeline) và ấn **run** để tạo ra **table** có các trường dữ liệu phù hơp với dữ liệu sẽ được **load** vào.
![Image](/images/3/3-4/1-0.png?width=40pc)

11.  Tạo thành công **table** thì ta sẽ quay trở lại thanh điều khiển bên trái của **Glue** và chọn **connection**.
![Image](/images/3/3-4/1-1.png?width=20pc)

12.  Chọn **Create connection** để tạo **connection** tới **Redshift**.
![Image](/images/3/3-4/1-2.png?width=40pc)

13.  Ở bước đầu tiên tìm kiếm **data source** là **Redshift** sau đó ấn chọn và ấn **next**.
![Image](/images/3/3-4/1-3.png?width=40pc)

14.  Chọn **Database instances** là **cluster** vừa tạo và nhập **Username** **password**, sau đó chọn **next**.
![Image](/images/3/3-4/1-4.png?width=40pc)

15.  Đặt tên cho **connection** và chọn **next**.
![Image](/images/3/3-4/1-5.png?width=40pc)

16.  Kiểm tra lại các cài đặt đã đúng chưa và chọn **Creation connection**.
![Image](/images/3/3-4/1-6.png?width=40pc)

17.  Tạo xong sẽ có **connection** tới **Redshift** như hình.
![Image](/images/3/3-4/1-7.png?width=40pc)