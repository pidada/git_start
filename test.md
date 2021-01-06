### 查询数据库中的表信息

下面的语句是查询数据库中表的信息

```sql
-- 查询表及注释
select 
	TABLE_NAME
	,TABLE_COMMENT
FROM INFORMATION_SCHEMA.TABLES
WHERE TABLE_SCHEMA = '库名'
```



### 查询表中字段信息

下面的语句是查询某个表中字段相关信息

```sql
-- 查看字段及注释
SELECT 
	COLUMN_NAME
	,COLUMN_COMMENT
FROM INFORMATION_SCHEMA.COLUMNS
WHERE TABLE_NAME = '表名'
AND TABLE_SCHEMA = '库名';
```


