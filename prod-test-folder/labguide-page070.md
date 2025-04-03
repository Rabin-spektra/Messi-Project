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


  
