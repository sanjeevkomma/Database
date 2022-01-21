* Highest Salary in each department
```sql
SELECT EmpID , Name, Salary, DeptId FROM Employee 
where ( DeptId,Salary ) in ( select DeptId, max(salary) from Employee group by DeptId )
```
