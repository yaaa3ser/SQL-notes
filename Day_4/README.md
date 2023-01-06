# Day 4

- `UNION` is used to combine the result-set of two or more SELECT statements.
    ```SQL
    SELECT ... FROM ...
    UNION / UNION ALL
    SELECT ... FROM ...
    ```
        `UNION ALL` doesn't remove dublicates 

- `JOIN` is used to combine rows from two or more tables, based on a related column between them.

    - (INNER) JOIN: Returns records that have matching values in both tables
    - LEFT (OUTER) JOIN: Returns all records from the left table, and the matched records from the right table
    - RIGHT (OUTER) JOIN: Returns all records from the right table, and the matched records from the left table
    - FULL (OUTER) JOIN: Returns all records when there is a match in either left or right table
    - [SELF JOIN](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_join_self)
    

    ```SQL
    SELECT Orders.OrderID, Customers.CustomerName
    FROM Orders
    (INNER / ....) JOIN Customers ON Orders.CustomerID=Customers.CustomerID;
    ```

- to find **Second** Highest/LOWEST ... ===> `we find the one that is the max but less than than the origin max`
    ```SQL
    select max(a) as '...' from ...
    where a < (select max(a) from ...)

    ```

    **Nice and EASY questions**
    1. [1795. Rearrange Products Table](https://leetcode.com/problems/rearrange-products-table/?envType=study-plan&id=sql-i)

    2. [608. Tree Node](https://leetcode.com/problems/tree-node/?envType=study-plan&id=sql-i)
            




