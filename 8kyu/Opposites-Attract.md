## Opposites Attract
```sql
-- # write your SQL statement here: you are given a table 
-- 'love' with columns 'flower1' and 'flower2', 
-- return a table with all the columns and your result
-- in a column named 'res'.

SELECT
  flower1,
  flower2,
  CASE 
    WHEN MOD(flower1, 2) = 0 AND MOD(flower2, 2) = 1 THEN true
    WHEN MOD(flower2, 2) = 0 AND MOD(flower1, 2) = 1 THEN true
    ELSE false
  END res
FROM 
  love;
```