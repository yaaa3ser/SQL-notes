# Day 10

- **It is all about using `HAVING`**
    - `having` is like `where` but used with `GROUP BY` 
    
    - ![](../media/having%20vs.%20where.png)

---------------------------------------------------------------
1. [1050. Actors and Directors Who Cooperated At Least Three Times](https://leetcode.com/problemsactors-and-directors-who-cooperated-at-least-three-times/?envType=study-plan&id=sql-i)

    ```SQL
    select actor_id, director_id from ActorDirector
    group by actor_id, director_id having count(*)>2
    ```

2. [1587. Bank Account Summary II](https://leetcode.com/problems/bank-account-summary-ii/?envType=study-plan&id=sql-i)
    ```SQL
    select name, sum(amount) as 'balance' from Users, Transactions 
    where Users.account = Transactions.account
    group by name having balance>10000
    ```

-------------------------------------------------------------------------------------------------------------------------
