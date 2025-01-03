```sql
--- basics selectors
select <name> -- slected information for output table

from <tableName> -- imports a table

(INNER) JOIN <table> -- Returns records that have matching values in both tables
LEFT (OUTER) JOIN <table> -- Returns all records from the left table, and the matched records from the right table
RIGHT (OUTER) JOIN <table> -- Returns all records from the right table, and the matched records from the left table DO NOT USE THIS OFTEN
FULL (OUTER) JOIN <table> -- Returns all records when there is a match in either left or right table
CROSS JOIN <table> -- returns a table with all possible permuations of rows from each table

ON <condition> -- select where to join tables on
where <condition> -- select conditions to select
group by <param> -- group the rows by the given param
```

```sql 
--- Operators
AND -- has both conditions
OR -- has either conditions
NOT, IS NOT -- doesn't have the condition
ANY -- TRUE if any of the subquery values meet the condition	
EXISTS -- TRUE if the subquery returns one or more records
IN -- TRUE if the operand is equal to one of a list of expressions
LIKE -- TRUE if the operand matches a pattern (good for regex)
SOME -- TRUE if any of the subquery values meet the condition

=,>,>=,<,<= -- self explanatory
<> -- not equals to
```

```
-- classes
Date -- used for denoting dates
DATEDIFF(<date1>,<date2>) -- returns the differences between dates
```

## Good problems:
* Joins:
	* [1280. Student and Examinations](https://leetcode.com/problems/students-and-examinations/description/?envType=study-plan-v2&envId=top-sql-50)
* Case typing
	* [1251. Average Selling Price](https://leetcode.com/problems/average-selling-price/description/?envType=study-plan-v2&envId=top-sql-50)
	