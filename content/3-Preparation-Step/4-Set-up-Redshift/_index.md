+++
title = "Set up and connect to Redshift"
date = 2024
weight = 4
chapter = false
pre = "<b>3.4 </b>"
+++

#### Create Redshift Cluster

1. Enter and search for **Redshift** in the search bar, then select **Redshift**.
![Image](../../images/3/3-4/1.png?width=40pc)

2. In the left navigation pane, select **Cluster**.
![Image](../../images/3/3-4/2.png?width=20pc)

3. Choose **Create Cluster** to create a new **Cluster**.
![Image](../../images/3/3-4/3.png?width=40pc)

4. Enter a **Cluster** name and choose the options as shown in the image. Since the goal is to learn, select **ra3.xlplus** to save costs.
![Image](../../images/3/3-4/4.png?width=40pc)

5. Enter a name for the **Admin User** and select the manual password option to set your password.
{{% notice note %}}
This **Username** and **password** will be used to create a connection to the **Query Editor**, so remember them to connect to the **Query Editor**.
{{% /notice %}}

![Image](../../images/3/3-4/5.png?width=40pc)

6. Use the default additional settings and click **Create Cluster** to create the **Cluster**.
![Image](../../images/3/3-4/6.png?width=40pc)

7. Once the **Cluster** is created, look at the left navigation pane and select **Query Editor V2**.
![Image](../../images/3/3-4/7.png?width=20pc)

8. On the **Query Editor** screen, click the three dots, then select **Create connection** to establish a connection to the **Query Editor**.
![Image](../../images/3/3-4/8.png?width=40pc)

9. When **Create connection** is selected, the screen will display options to link to the **Query Editor**. Select the options as shown in the image, and enter the previously created **Username** and **password**.
![Image](../../images/3/3-4/9.png?width=40pc)

10. After successfully connecting to the **Query Editor**, paste the pre-made **SQL Script** from [Github](https://github.com/Zymeth-PGB/AWS-Basic-Data-Pipeline) and click **run** to create a **table** with fields suitable for the data to be **loaded**.
![Image](../../images/3/3-4/1-0.png?width=40pc)

11. After successfully creating the **table**, go back to the left-hand panel of **Glue** and select **Connection**.
![Image](../../images/3/3-4/1-1.png?width=20pc)

12. Select **Create connection** to create a connection to **Redshift**.
![Image](../../images/3/3-4/1-2.png?width=40pc)

13. In the first step, search for the **data source** as **Redshift**, select it, and click **next**.
![Image](../../images/3/3-4/1-3.png?width=40pc)

14. Choose **Database instances** as the **cluster** you just created, enter the **Username** and **password**, then select **next**.
![Image](../../images/3/3-4/1-4.png?width=40pc)

15. Name the **connection** and select **next**.
![Image](../../images/3/3-4/1-5.png?width=40pc)

16. Review the settings to ensure they are correct, and select **Create connection**.
![Image](../../images/3/3-4/1-6.png?width=40pc)

17. Once done, you will have a **connection** to **Redshift** as shown in the image.
![Image](../../images/3/3-4/1-7.png?width=40pc)