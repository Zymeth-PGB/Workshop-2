+++
title = "Create Crawler"
date = 2024
weight = 5
chapter = false
pre = "<b>3.5 </b>"
+++

#### Create Crawlers

{{% notice note %}}
We will create 2 **crawlers** to serve the purpose of retrieving **schemas** from **S3** and from the **Redshift** created in the previous step. Therefore, some similar steps will only show one image, while the steps that differ will have instructions for each **crawler**.
{{% /notice %}}

1. Enter and search for **Glue** in the search bar.
![Image](../../images/3/3-5/1.png?width=40pc)

2. In the left navigation pane, select **Crawler**.
![Image](../../images/3/3-5/2.png?width=20pc)

3. After selecting **Crawler**, a list of crawlers and other options will appear. Choose **Create crawler** to create a new **crawler**.
![Image](../../images/3/3-5/3.png?width=40pc)

4. Enter a name for each **Crawler** that matches its function, indicating where it retrieves the **schema** from.
![Image](../../images/3/3-5/4.png?width=40pc)

5. In Step 2, select **Not yet** and add a **data source**.
![Image](../../images/3/3-5/5.png?width=40pc)

6. Each **Crawler** will have different options for selecting the **data source** as follows:
   - For the **Crawler** that retrieves the **schema** from **S3**, select as shown:
     - The path to **S3** will choose the **bucket** created in step [1](../1-Create-S3/).
![Image](../../images/3/3-5/6-1.png?width=40pc)

   - For the **Crawler** that retrieves the **schema** from **Redshift**, select as shown:
     - In the **Include Path** section, add the path to the **table** created in the previous step in the **Query Editor**.
![Image](../../images/3/3-5/6-2.png?width=40pc)

7. After selecting the **data source**, you will see the **data sources** as shown in the two images below. Choose **next** to proceed to the next step.
   - **Crawler S3**
![Image](../../images/3/3-5/7-1.png?width=40pc)

   - **Crawler Redshift**
![Image](../../images/3/3-5/7-2.png?width=40pc)

8. Select the **IAM role** created in step [2](../2-create-iam-role/).
![Image](../../images/3/3-5/8.png?width=40pc)

9. Choose the appropriate **database** for each **Crawler** created in step [3](../3-create-table/):
   - **Crawler S3**
![Image](../../images/3/3-5/9-1.png?width=40pc)

   - **Crawler Redshift**
![Image](../../images/3/3-5/9-2.png?width=40pc)

10. Review the selections, and if everything is fine, choose **Create crawler**:
   - **Crawler S3**
![Image](../../images/3/3-5/10-1.png?width=40pc)

   - **Crawler Redshift**
![Image](../../images/3/3-5/10-2.png?width=40pc)

11. Once successfully created, you will have 2 **crawlers** with a **State** of **Ready**, as shown.
![Image](../../images/3/3-5/11.png?width=40pc)