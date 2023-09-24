# 577.-Employee-Bonus
Problem Link:
https://leetcode.com/problems/employee-bonus/description/?envType=study-plan-v2&envId=top-sql-50

## Solution

```sql
SELECT e.name,b.bonus
FROM Employee e
LEFT JOIN Bonus b ON b.empId=e.empId
where ISNULL(b.bonus,0) <1000
