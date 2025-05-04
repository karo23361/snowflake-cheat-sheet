# ❄️ Snowflake Cheat Sheet ❄️

⭐ Purpose of this Repo is to gather basic / advanced commands while taking Snowlake Course to make a little Cheat Sheet for someone who is starting adventure with Snowflake. ⭐  

# COMMANDS CHEET SHEET #

Snowflake basic commands:

Datbase creation:
```sql
CREATE OR REPLACE DATABASE <database_name>;
```
Schema creation:
```sql
CREATE OR REPLAC SCHEMA <database_name>.<schema_name>;
```
Table creation:
```sql
CREATE OR REPLACE TABLE <database_name>.<schema_name>.<table_name> (
  column1 INT,
  columnt2 varchar(15)); 
```
Warehouse creation:
```sql
CREATE OR REPLACE WAREHOUSE <name>
WITH WAREHOUSE_SIZE = <size>
AUTO_SUSPEND = 311
AUTO_RESUME = TRUE
INITIALLY_SUSPENDED = FALSE
COMMENT = 'This is the comment for the warehouse';
```

| Available size |
| -------- |
| XSMALL  |
| SMALL |
| MEDIUM    |
| LARGE    |
| XLARGE    |
| .....    |

Stage Creation 
```sql
CREATE OR REPLACE STAGE <database_name>.<schema_name>.<stage_nam>
    url='s3://bucketsnowflakes3'; 
```

Copying data into table from bucket
```sql
COPY INTO <database_name>.<schema_name>.<table_name>
    FROM @<stage_name>
    file_format= (type = csv field_delimiter= ',' skip_header= 1)
    pattern='.*example.*';
```

Listing all files in a stage
```sql
LIST @<database_name>.<schema_name>.<stage_name>;
```




📝 (Repo will be continuously updated) 📝
