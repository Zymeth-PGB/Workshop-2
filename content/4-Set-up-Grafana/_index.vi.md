+++
title = "Cài đặt và kết nối với Grafana"
date = 2024
weight = 4
chapter = false
pre = "<b>4. </b>"
+++

#### Cài đặt Grafana

Có 2 cách để cài đặt **Grafana** là cài trực tiếp vào máy hoặc cài thông qua **Docker**.

1. Cài **Grafana** trực tiếp vào máy
   
    1.1. Truy cập vào trang [download Grafana](https://grafana.com/grafana/download).

    1.2. Lựa chọn phiên bản phù hợp với hệ điều hành máy tính của bạn và tiến hành cài đặt.

2. Cài **Grafana** sử dụng **Docker**

    2.1. Truy cập vào **Docker hub** và tìm [Grafana image](https://hub.docker.com/r/grafana/grafana).

    2.2. Sau đó mở **terminal** và chạy lệnh sau: 
    ```
    docker run -d --name=grafana -p 3000:3000 grafana/grafana
    ```

    2.3. Kiểm tra xem đã cài đặt hay chưa sử dụng lệnh:
    ```
    docker ps
    ```

#### Kết nối Grafana tới Redshift

1. Truy cập vào **Grafana** thông qua **localhost** với **port** là **3000**.
2. **Username** và **password** mặc định là **admin** và **admin** cho lần đầu đăng nhập. Nếu muốn thay đổi bạn có thể truy cập vào **Profile** và thực hiện thay đổi mật khẩu.
3. Sau khi đăng nhập thành công ta sẽ thực hiện kết nối tới **Redshift** như sau:
   - Ở thanh điều hướng bên trái chọn **connection**.
![Image](/images/4/1.png?width=40pc)

   - Nhập và tìm kiếm **Redshift** ở thanh tìm kiếm.
![Image](/images/4/2.png?width=40pc)

   - Chọn **Install** để thêm **connection** tới **Redshift**.
![Image](/images/4/3.png?width=40pc)

   - Sau khi cài đặt thành công chọn **Add new data source** để thêm data đã **transforms** để thực hiện tạo **Dashboard** theo nhu cầu.
![Image](/images/4/4.png?width=40pc)