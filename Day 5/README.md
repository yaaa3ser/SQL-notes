# Day 5

- `GROUP BY` groups rows that have the same values into summary rows, like "find the number of customers in each country".
    - It is often used with aggregate functions (COUNT(), MAX(), MIN(), SUM(), AVG()) to group the result-set by one or more columns.
    ```SQL
    SELECT ... FROM ... WHERE condition
    GROUP BY column_name
    ```

- `JOIN` is used to combine rows from two or more tables, based on a related column between them.

    - (INNER) JOIN: Returns records that have matching values in both tables
    - LEFT (OUTER) JOIN: Returns all records from the left table, and the matched records from the right table
    - RIGHT (OUTER) JOIN: Returns all records from the right table, and the matched records from the left table
    - FULL (OUTER) JOIN: Returns all records when there is a match in either left or right table
    - [SELF JOIN](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_join_self)
    
-----------------------------------------------------------------------------------------------------------------------------

1. [175. Combine Two Tables](https://leetcode.com/problems/combine-two-tables/?envType=study-plan&id=sql-i)
    - easy, just `LEFT JOIN`


2. [1581. Customer Who Visited but Did Not Make Any Transactions](https://leetcode.com/problems/customer-who-visited-but-did-not-make-any-transactions/?envType=study-plan&id=sql-i)
    - nice and new idea using `GROUP BY`
    

3. [1148. Article Views I](https://leetcode.com/problems/article-views-i/?envType=study-plan&id=sql-i)
    - very easy
            




