+++
title = "Install and connect to Grafana"
date = 2024
weight = 4
chapter = false
pre = "<b>4. </b>"
+++

#### Install Grafana

There are two ways to install **Grafana**: directly on your machine or using **Docker**.

1. **Install Grafana Directly on Your Machine**
   
    1.1. Go to the [download Grafana](https://grafana.com/grafana/download) page.

    1.2. Choose the version that matches your operating system and proceed with the installation.

2. **Install Grafana Using Docker**

    2.1. Visit **Docker Hub** and search for the [Grafana image](https://hub.docker.com/r/grafana/grafana).

    2.2. Then, open your **terminal** and run the following command: 
    ```
    docker run -d --name=grafana -p 3000:3000 grafana/grafana
    ```

    2.3. Check if it is installed using the command:
    ```
    docker ps
    ```

#### Connect Grafana to Redshift

1. Access **Grafana** via **localhost** on **port** **3000**.
2. The default **Username** and **password** are **admin** for the first login. If you want to change it, you can go to **Profile** and change your password.
3. After successfully logging in, connect to **Redshift** as follows:
   - In the left navigation pane, select **Connection**.
![Image](../images/4/1.png?width=40pc)

   - Enter and search for **Redshift** in the search bar.
![Image](../images/4/2.png?width=40pc)

   - Select **Install** to add the connection to **Redshift**.
![Image](../images/4/3.png?width=40pc)

   - After successful installation, select **Add new data source** to add the transformed data for creating dashboards as needed.
![Image](../images/4/4.png?width=40pc)