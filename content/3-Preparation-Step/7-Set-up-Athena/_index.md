+++
title = "Setup and Query with Athena"
date = 2024
weight = 7
chapter = false
pre = "<b>3.7 </b>"
+++

#### Set Up Athena

1. Enter and search for **Athena** in the search bar.
![Image](../../images/3/3-7/1.png?width=40pc)

2. In the **Query Editor** screen of **Athena**, select the **Data Source** as shown. The **Database** section will display the **Database** before and after **Transforms**. You can choose either one based on your use case; once selected, the **Tables** section will show the **Tables** of the chosen **Database**.
![Image](../../images/3/3-7/2.png?width=40pc)

3. To run queries, you need to set up a location for the query results. Here, select **Settings** and then choose **Manage**.
![Image](../../images/3/3-7/3.png?width=40pc)

4. Before selecting the path to **S3**, you need to go back to **S3** and create a **Bucket** to store the query results. After creating it, select the path to that **Bucket** and click **Save**.
![Image](../../images/3/3-7/4.png?width=40pc)