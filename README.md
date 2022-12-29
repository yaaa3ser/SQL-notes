# SQL-notes
**SQL notes from leetcode SQL-study plan**
</br></br>


# Day 1
- to return fields from table ===> ```select ..., ..., ... from ... where ... or/and ....```
- to return a field = null ===> ```where ...``` *```is ```* ```null (not = null xxx)```
- to return a field != 5 ===> ```where ... <> 5 (or !=5)```
- to return a field from a table but not in another table (there is a **fk** between the 2 tables) ===> Ex.: id

    ``` select ... from ... where id not in (select customerId from ...)```
------------------------------------------------------------------------------------------------------------------
# Day 2 
- 