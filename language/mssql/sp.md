# 특정문자열이 포함된 SP검색
```sql
SELECT 'EXEC sp_helptext [' + SCHEMA_NAME(SCHEMA_ID) + '.' + OBJECT_NAME(object_id) + ']',
OBJECT_DEFINITION(object_id)
FROM sys.procedures
WHERE OBJECT_DEFINITION(object_id) LIKE '%검색어%'
```
