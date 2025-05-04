# ❄️ Snowflake Cheat Sheet ❄️

⭐ Purpose of this Repo is to gather basic / advanced commands while taking Snowlake Course to make a little Cheat Sheet for someone who is starting adventure with Snowflake. ⭐  

# COMMANDS CHEET SHEET #

Snowflake basic commands:

Datbase creation:
```sql
CREATE OR REPLACE DATABASE <database_name>;
```
Table creation:
```sql
CREATE OR REPLACE TABLE <table_name> (
column1 INT,
columnt2 varchar(15)
); 
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
Schema creation:
```sql
CREATE OR REPLAC SCHEMA <schema_name>;
```
| Available size |
| -------- |
| XSMALL  |
| SMALL |
| MEDIUM    |
| LARGE    |
| XLARGE    |
| .....    |







📝 (Repo will be continuously updated) 📝
