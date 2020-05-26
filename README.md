# docker_mysql


Disable ONLY_FULL_GROUP_BY (https://stackoverflow.com/questions/23921117/disable-only-full-group-by)
```sql
SET GLOBAL sql_mode=(SELECT REPLACE(@@sql_mode,'ONLY_FULL_GROUP_BY',''));
```
