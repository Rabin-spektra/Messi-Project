# Databricks UC Hands-on  
## Create your first table and grant privileges  

This hands-on provides a quick walkthrough of creating a table and granting privileges in Databricks using the Unity Catalog.

# Prerequisites  

In order to perform this hands-on, you must have access to:  
- **Databricks workspace ENV with UC enabled**  




# Task 1: Create Your First Table  

Unity Catalog includes a three-level namespace for data objects: **catalog.schema.table**.  
In this example, youll run a notebook that creates a table named **department** in the **workspace catalog** and **default schema (database)**.  

The **workspace catalog** is the default catalog created with your workspace that all users have access to. It shares a name with your workspace.  

You can define access to tables declaratively using **SQL** or the **Databricks Explorer UI**:  

### Steps:  

1. In the sidebar, click **+New > Notebook**.  


![Picture1.png](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabs-AI/Lab-Guide/main/50444Hp6LnYDC/images/Picture1.png?token=8b2t1Sg45N8JBe8QNwBlyhJq)


2. Select **SQL** as your notebook language.  


![Picture2.png](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabs-AI/Lab-Guide/main/50444Hp6LnYDC/images/Picture2.png?token=8b2t1Sg45N8JBe8QNwBlyhJq)






3. Click **Connect** and attach the notebook to a compute resource.  
4. Add the following commands to the notebook and run them (replace `<workspace-catalog>` with the name of your workspace catalog):  

```sql
USE CATALOG <workspace-catalog>;

CREATE TABLE IF NOT EXISTS default.department
(
   deptcode   INT,
   deptname   STRING,
   location   STRING
);

INSERT INTO default.department VALUES
  (10, 'FINANCE', 'EDINBURGH'),
  (20, 'SOFTWARE', 'PADDINGTON');
  
```

5. In the sidebar, click **Catalog**, then search for the **workspace catalog (workspace-name)** and the **default schema**, where youll find your new **department** table.


![Picture3.png](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabs-AI/Lab-Guide/main/50444Hp6LnYDC/images/Picture3.png?token=8b2t1Sg45N8JBe8QNwBlyhJq)




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

#### Grant Permissions Using SQL Statements

You can also grant those permissions using the following SQL statement in a Databricks notebook or the SQL query editor.  
In this example, you give a group with group ID **125560464292541** (Find out the group name for this ID) permission on your table:



```sql
GRANT SELECT ON default.department TO `<your group>`;
```