+++
title = "Clean up"
date = 2024
weight = 5
chapter = false
pre = "<b>5. </b>"
+++

We will clean up the resources in the following order:

**Delete S3 Bucket:**
   - Access the **Buckets** management section.
   - Select the **Buckets** created in the **Workshop**.
   - Click **Delete** and re-enter the **Bucket** name as requested to delete the **Bucket**.

**Delete IAM Role:**
   - Access the **IAM** console and select the **Roles** section.
   - Click on the **Role** created in the **Workshop** and select **Delete**.
   - Re-enter the **Role** name and complete the **Delete** process.

**Delete Databases in Glue:**
   - Access the **Glue** console.
   - Select **Databases** and choose the **Databases** created in the **Workshop**.
   - Click **Delete** to remove the **Databases**.

**Delete Redshift Cluster and Connection:**
   - **Delete Cluster**
     - Access the **Redshift** console.
     - Select **View all clusters** to see all clusters.
     - Choose the cluster created and select **Action** to perform **Delete**.
     - After selecting **Delete** in **Action**, uncheck **Create final snapshot** and enter **delete** in the box to complete the **Delete cluster**.

   - **Delete Connection**
     - Access the **Glue** console.
     - Select **Connections** in the left navigation pane.
     - Choose the **connection** created in the **Workshop** and select **Action** to perform **Delete**.
     - After selecting **Delete** in **Action**, confirm the **Delete** to remove it.

**Delete Crawler:**
   - Access the **Glue** console.
   - Select **Crawlers** in the left navigation pane.
   - Choose the **crawler** created in the **Workshop** and select **Action** to perform **Delete**.
   - After selecting **Delete** in **Action**, confirm the **Delete** to remove it.

**Delete ETL Job:**
   - Access the **Glue** console.
   - Select **ETL jobs** in the left navigation pane.
   - Choose the **job** created in the **Workshop** and select **Action** to perform **Delete**.
   - After selecting **Delete** in **Action**, confirm the **Delete** to remove it.