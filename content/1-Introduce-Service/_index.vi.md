+++
title = "Giới thiệu các dịch vụ và công cụ"
date = 2024
weight = 1
chapter = false
pre = "<b>1. </b>"
+++

#### Các dịch vụ và công cụ được sử dụng

1. **Amazon S3 (Simple Storage Service)** là một dịch vụ lưu trữ đối tượng trên đám mây của **Amazon Web Services (AWS)**, cho phép bạn lưu trữ và truy xuất bất kỳ lượng dữ liệu nào, từ bất kỳ đâu trên web, vào bất kỳ thời điểm nào. **S3** được thiết kế để cung cấp khả năng lưu trữ có độ bền cao, dễ dàng mở rộng quy mô
![Image](../images/1/S3.png?width=5pc)

2. **AWS Glue** là một dịch vụ **ETL (Extract, Transform, Load)** không máy chủ của **Amazon Web Services (AWS)**, giúp bạn chuẩn bị và xử lý dữ liệu một cách dễ dàng. **AWS Glue** tự động hóa quy trình trích xuất dữ liệu từ các nguồn khác nhau, biến đổi dữ liệu và tải chúng vào các kho lưu trữ dữ liệu hoặc dịch vụ phân tích khác.
![Image](../images/1/glue.png?width=5pc)

3. **Amazon Athena** là một dịch vụ truy vấn **SQL** không máy chủ do **Amazon Web Services (AWS)** cung cấp, cho phép người dùng phân tích dữ liệu trực tiếp trên **Amazon S3** bằng cách sử dụng ngôn ngữ **SQL** chuẩn mà không cần phải thiết lập hoặc quản lý cơ sở hạ tầng. **AWS Athena** đặc biệt phù hợp cho việc phân tích dữ liệu lớn được lưu trữ trong **S3** mà không cần phải tải hoặc di chuyển dữ liệu sang một hệ thống khác.
![Image](../images/1/athena.png?width=5pc)

4. **Amazon Redshift** là một dịch vụ kho dữ liệu đám mây **(cloud data warehouse)** của **Amazon Web Services (AWS)**, được thiết kế để phân tích dữ liệu quy mô lớn và hỗ trợ truy vấn **SQL** với tốc độ cao. **Redshift** cho phép bạn lưu trữ và phân tích dữ liệu từ nhiều nguồn khác nhau, từ đó giúp doanh nghiệp xây dựng các hệ thống phân tích, báo cáo và hỗ trợ ra quyết định.
![Image](../images/1/redshift.png?width=5pc)

5. **AWS IAM (Identity and Access Management)** là một dịch vụ của **Amazon Web Services (AWS)** giúp quản lý quyền và kiểm soát truy cập cho các tài nguyên và dịch vụ trong **AWS**. **IAM** cho phép bạn kiểm soát ai có thể truy cập vào tài nguyên **AWS** (người dùng, nhóm người dùng hoặc dịch vụ) và những hành động nào họ có thể thực hiện trên các tài nguyên đó.
![Image](../images/1/IAM.png?width=5pc)

6. **Grafana** là một công cụ mã nguồn mở dùng để giám sát, trực quan hóa dữ liệu và tạo các bảng điều khiển (**dashboard**) tương tác từ nhiều nguồn dữ liệu khác nhau. **Grafana** thường được sử dụng để theo dõi hiệu suất hệ thống, phân tích log, và hiển thị các số liệu theo thời gian thực, cho phép người dùng dễ dàng tạo ra các biểu đồ và bảng điều khiển trực quan nhằm giúp phân tích và giám sát dữ liệu một cách hiệu quả.
![Image](../images/1/grafana.png?width=5pc)