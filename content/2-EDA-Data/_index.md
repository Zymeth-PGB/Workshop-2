+++
title = "Chuẩn bị dữ liệu"
date = 2024
weight = 2
chapter = false
pre = "<b>2. </b>"
+++

#### Nguồn dữ liệu

Dữ liệu được sử dụng trong workshop này có ngữ cảnh là Một công ty viễn thông hư cấu đã cung cấp dịch vụ điện thoại gia đình và Internet cho 7043 khách hàng ở California trong quý 3.

Có thể tìm và tải dữ liệu ở đây : [Telco customer churn: IBM dataset](https://www.kaggle.com/datasets/yeanzc/telco-customer-churn-ibm-dataset)

#### Khám phá dữ liệu

Mô tả các trường dữ liệu :
- **CustomerID**: Một **ID** duy nhất xác định từng khách hàng.
- **Count**: Một giá trị được sử dụng trong báo cáo/bảng thông tin để tổng hợp số lượng khách hàng trong một tập hợp đã lọc.
- **Country**: Quốc gia nơi cư trú chính của khách hàng.
- **State**: Tiểu bang nơi cư trú chính của khách hàng.
- **City**: Thành phố nơi cư trú chính của khách hàng.
- **Zip Code**: Mã bưu chính nơi cư trú chính của khách hàng.
- **Lat Long**: Vĩ độ và kinh độ kết hợp của nơi cư trú chính của khách hàng.
- **Latitude**: Vĩ độ của nơi cư trú chính của khách hàng.
- **Longitude**: Kinh độ của nơi cư trú chính của khách hàng.
- **Gender**: Giới tính của khách hàng: **Male**, **Female**
- **Senior Citizen**: Chỉ ra nếu khách hàng từ 65 tuổi trở lên: **Yes**, **No**
- **Partner**: Chỉ ra nếu khách hàng có đối tác: **Yes**, **No**
- **Dependents**: Chỉ ra nếu khách hàng sống với bất kỳ người phụ thuộc nào: **Yes**, **No**. Người phụ thuộc có thể là con cái, cha mẹ, ông bà, v.v.
- **Tenure Months**: Chỉ ra tổng số tháng mà khách hàng đã làm việc cho công ty vào cuối quý được chỉ định ở trên.
- **Phone Service**: Chỉ ra nếu khách hàng đăng ký dịch vụ điện thoại gia đình với công ty: **Yes**, **No**
- **Multiple Lines**: Chỉ ra nếu khách hàng đăng ký nhiều đường dây điện thoại với công ty: **Yes**, **No**
- **Internet Service**: Chỉ ra nếu khách hàng đăng ký dịch vụ Internet với công ty: **No**, **DSL**, **Fiber** **Optic**, **Cable**.
- **Online Security**: Chỉ ra liệu khách hàng có đăng ký dịch vụ bảo mật trực tuyến bổ sung do công ty cung cấp hay không: **Yes**, **No**
- **Online Backup**: Chỉ ra liệu khách hàng có đăng ký dịch vụ sao lưu trực tuyến bổ sung do công ty cung cấp hay không: **Yes**, **No**
- **Device Protection**: Chỉ ra liệu khách hàng có đăng ký gói bảo vệ thiết bị bổ sung cho thiết bị Internet do công ty cung cấp hay không: **Yes**, **No**
- **Tech Support**: Chỉ ra liệu khách hàng có đăng ký gói hỗ trợ kỹ thuật bổ sung từ công ty với thời gian chờ được rút ngắn hay không: **Yes**, **No**
- **Streaming TV**: Chỉ ra liệu khách hàng có sử dụng dịch vụ Internet của mình để truyền phát chương trình truyền hình từ nhà cung cấp bên thứ ba hay không: **Yes**, **No**. Công ty không tính thêm phí cho dịch vụ này.
- **Streaming Movies**: Chỉ ra liệu khách hàng có sử dụng dịch vụ Internet của mình để truyền phát phim từ nhà cung cấp bên thứ ba hay không: **Yes**, **No**. Công ty không tính thêm phí cho dịch vụ này.
- **Contract**: Chỉ ra loại hợp đồng hiện tại của khách hàng: **Month-to-Month**, **One Year**, **Two Year**.
- **Paperless Billing**: Chỉ ra nếu khách hàng đã chọn thanh toán không cần giấy tờ: **Yes**, **No**
- **Payment Method**: Chỉ ra cách khách hàng thanh toán hóa đơn của họ: **Bank Withdrawal**, **Credit Card**, **Mailed Check**
- **Monthly Charge**: Chỉ ra tổng phí hàng tháng hiện tại của khách hàng cho tất cả các dịch vụ của công ty.
- **Total Charges**: Chỉ ra tổng phí của khách hàng, được tính đến cuối quý được chỉ định ở trên.
- **Churn Label**: **Yes** = khách hàng đã rời công ty trong quý này. **No** = khách hàng vẫn tiếp tục gắn bó với công ty. Có liên quan trực tiếp đến **Churn Value**.
- **Churn Value**: **1** = khách hàng đã rời công ty trong quý này. **0** = khách hàng vẫn tiếp tục gắn bó với công ty. Có liên quan trực tiếp đến **Churn Label**.
- **Churn Score**: Giá trị từ **0-100** được tính bằng công cụ dự đoán **IBM SPSS Modeler**. Mô hình kết hợp nhiều yếu tố được biết là nguyên nhân gây ra tình trạng **churn**. Điểm càng cao thì khả năng khách hàng **churn** càng cao.
- **CLTV**: Giá trị trọn đời của khách hàng. **CLTV** dự đoán được tính bằng cách sử dụng các công thức của công ty và dữ liệu hiện có. Giá trị càng cao, khách hàng càng có giá trị. Khách hàng có giá trị cao nên được theo dõi để biết tình trạng **churn**.
- **Churn Reason**: Lý do cụ thể của khách hàng khi rời khỏi công ty. Liên quan trực tiếp đến **Churn Category**.

Bộ dữ liệu được mô tả chi tiết hơn ở đây : [Telco customer churn](https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113)