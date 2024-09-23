+++
title = "Prepare an ETL process"
date = 2024
weight = 6
chapter = false
pre = "<b>3.6 </b>"
+++

#### Using Glue for ETL

1. Enter and search for **Glue** in the search bar.
![Image](../../images/3/3-6/1.png?width=40pc)

2. In the left navigation pane, select **ETL jobs**.
![Image](../../images/3/3-6/2.png?width=20pc)

3. Choose **Visual ETL** to create an **ETL** process.
![Image](../../images/3/3-6/3.png?width=40pc)

4. In the **Visual** tab, select the **Sources** section to choose the data source; here, we select **S3**.
![Image](../../images/3/3-6/4.png?width=40pc)

5. Move to the next section, **Transforms**, and select **Change Schema** to make changes to the data.
![Image](../../images/3/3-6/5.png?width=40pc)

6. In the **Target** section, choose **Redshift** to load the data.
![Image](../../images/3/3-6/6.png?width=40pc)

7. After selecting all the components for the **ETL** process, we will configure each part as follows:
   - **S3**
![Image](../../images/3/3-6/7.png?width=40pc)

   - **Change Schema**
     - We will **Drop** the following fields: **count, country, state, lat long, latitude, longitude, cltv**.
     - For fields with two-word names like **"zip code,"** we will change them to **"zip_code."** This applies to all fields with long names.
![Image](../../images/3/3-6/8.png?width=40pc)

   - **Redshift**
![Image](../../images/3/3-6/9.png?width=40pc)

8. Change the name of the job and **save** the job.
![Image](../../images/3/3-6/10.png?width=40pc)

9. Move to the **Job details** section and assign the **IAM role** for this job as the **role** created in step 2.
![Image](../../images/3/3-6/11.png?width=40pc)

10. After completing the setup, return to the job management screen, and you will see the newly created job as shown.
![Image](../../images/3/3-6/12.png?width=40pc)