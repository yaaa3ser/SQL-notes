# Day 3

1. if you need to capitalize a field (upper first letter and lower the rest) ===> 
you can use string functions like 
    ```SQL
    CONCAT    UPPER,LOWER   SUBSTRING   LENGTH
    ```
    and it will be like 
    `CONCAT(UPPER(substring(...,1,1)), LOWER(substring(...,2,length(...))))`

2. if I need to find for each **date** the number of *different* ... and their names for example. 

    `COUNT` return the number of ...

    `GROUP_CONCAT` returns the row values in the comma separated fashion.

    so it will be like: 

    ```SQL
    select
    COUNT(DISTINCT ...) as ... 
    ,GROUP_CONCAT(DISTINCT name) as ...
    from ...
    GROUP BY date
    ```

3. use LIKE 
    - [see day2 note3](https://github.com/yaaa3ser/SQL-notes/tree/main/Day%202)

    





