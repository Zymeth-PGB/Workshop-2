+++
title = "Thiết lập và query với Athena"
date = 2024
weight = 7
chapter = false
pre = "<b>3.7 </b>"
+++

#### Thiết lập Athena

1. Nhập và tìm kiếm **Athena** trong thanh tìm kiếm.
![Image](/images/3/3-7/1.png?width=40pc)

2. Trong màn hình **Query Editor** của **Athena** chọn **Data Source** như hình. Phần **Database** sẽ hiển thị **Database** trước khi **Transforms** và sau khi **Transforms**, bạn có thể chọn bất kì cái nào tùy vào mục đích sử dụng, khi chọn xong thì ở phần **Tables** sẽ xuất hiện các **Table** của **Database** đã chọn.
![Image](/images/3/3-7/2.png?width=40pc)

3. Để có thể chạy được các **query** thì ta cần phải cài đặt thêm vị trí của các kết quả **query**. Ở đây ta chọn phần **Settings** và chọn **Manage**.
![Image](/images/3/3-7/3.png?width=40pc)

4. Trước khi chọn đường dẫn đến **S3** thì ta phải quay lại **S3** và tạo 1 **Bucket** phục vụ cho việc chứa kết quả **query**. Sau khi tạo xong thì chọn đường dẫn đến **Bucket** đó và chọn **Save**.
![Image](/images/3/3-7/4.png?width=40pc)