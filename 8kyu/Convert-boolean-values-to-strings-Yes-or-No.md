Complete the method that takes a boolean value and return a `"Yes"` string for `true`, or a `"No"` string for `false.`

-- # write your SQL statement here: you are given a table 'booltoword' 
-- with column 'bool', return a table with column 'bool' and your result in a column 
-- named 'res'.

```sql
SELECT bool,
  CASE "bool" 
    WHEN true THEN 'Yes'
    WHEN false THEN 'No'
  END res
from booltoword
```