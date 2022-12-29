
# Day 2 
1. order by a field ===> `select ... from ... order by ...`

2. o return a field based on a **condition**Ex. ==> 
`calculate the bonus of each employee. The bonus of an employee is 100% of their salary if the ID of the employee is an odd number, else it is 0.` ===>
    ```SQL
    select case 
    when (condition) then ...
    else ...
    end as '...'
    from ...  
    ```
3. LIKE
    - if I need a field starts with 's' for example ===>`... like 's%'`

    - if I need a field ends with 's' for example ===>`... like '%s'`

    - a field has 's' for example in any position ===>`... like '%s%'`

    - a field has 's' in the second position ===> `... like '_s%'`

    - start with 's' and has at least 3 characters ===>`... LIKE 'a__%'`
4. UPDATE ===> `UPDATE table set field = ... where ...`
5. UPDATE based on a **codition** ===>
    ```SQL
    update ...
    set ... = case 
                    when (condition) then (result)
                    else (result)
               end
    ```
6. DELETE ===> `DELETE from ... where ...`

7. If I need to delete duplicate emails from table Student for example using the DELETE statement ===>  `I should make 2 Students and delete based on condition like that:`
    ```SQL
    Delete S1 from Student as S1, Student as S2
    where S1.email = S2.email and S1.id > S2.id
    ```
    **Here I keep the one with the smallest id**
------------------------------------------------------------------------------------------------------------------






