### Task 2: Manage Permissions on Your Table

As the original table creator, youre the table owner, and you can grant other users permission to read or write to the table. You can even transfer ownership, but we wont do that here. For more information about the Unity Catalog privileges and permissions model, see [Manage privileges in Unity Catalog](https://docs.databricks.com/en/data-governance/unity-catalog/manage-privileges.html).

#### Grant Permissions Using the UI

To give users permissions on your table using the UI:

1. Click the table name in **Catalog Explorer** to open the **table details page**, and go to the **Permissions** tab.
2. Click **Grant**.
3. In the **Grant** dialog:
   - **Select** the users and groups you want to give permission to.
   - **Choose** the privileges you want to grant.  
   - For this example, assign the **SELECT (read)** privilege and click **Grant**.


