# Database ![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)
## Functional Dependency
- If, A -> B we get a definite value of B for each A

Example: for functional dependency to exists,for each a from A, if a1 == a2 then b1 == b2 (b1,b2 from B)
- Example of not a functional dependency: <br />

| A | B |
| :------------- | :----------: |
| a | 1 |
| a | 2 |
| b | 3 |
| c | 4 |

Checking functional dependency:
- Check if all records are unique or not. it they are unique then, no need to check. They are functionaly independent
## Normalization
- Removes repition of similar data on multiple places
- Data redundancy uses extra spaces
- Resundancy also leads to insertion, update and deletion anomaly
- Aim is to minimize data redundancy
- Sample table: <br />

| Roll no       | Name     | Age     | Roll ID     | Dept     | HOD Name     | HOD Phone     | 
| :------------- | :----------: |  :----------: |  :----------: |  :----------: |  :----------: |  :----------: | 
|1 | A | 20 | 101  | CSE  | John Doe | 01800000000|
|2 | B | 22 | 102  | CSE  | John Doe | 01800000000|

## 1NF
- Each column should contain atomic value
<img src="img/1nf-1.png" style="width:200px;height: 200px; display:block; margin: 0 auto"> 
- Each column should contain values that are of the same type
<img src="img/1nf-2.png" style="width:200px;height: 200px; display:block; margin: 0 auto"> 
- Each column should have a unique name
<img src="img/1nf-3.png" style="width:200px;height: 200px; display:block; margin: 0 auto">

## 2NF 
- Must be in 1NF
- No pratial dependency on the table
### Partial dependency
<img src="img/2nf-1.png" style=" display:block; margin: 0 auto">

**Solution**
<img src="img/2nf-2.png" style=" display:block; margin: 0 auto">

## 3NF
- Must be in 1NF and 2NF
- No transitive dependency
### Transitive dependency
- Attributes on table depends on non-prime attribute which depends on prime attribute 
<img src="img/3nf-1.png" style=" display:block; margin: 0 auto">
**Solution:**
<img src="img/3nf-2.png" style=" display:block; margin: 0 auto">

**Anomaly:**
- Insertion anomaly: whenever we try to update one record, we need to add duplicate data
- Deletion anomaly: Deletion of all CSE students will lead to complete annihilation of all CSE department data
- Update anomaly: If the HOD of CSE get's changed then we need to update every CSE record
## Fan Trap
### Problem
<img src="img/fan-trap-1.png" style=" display:block; margin: 0 auto">

### Solution
<img src="img/fan-trap-2.png" style=" display:block; margin: 0 auto">

## Relational Algebra
<img src="img/relational-algebra-1.png" style=" display:block; margin: 0 auto">


## Data model
### Conceptual Model
![](img/conceptual.png)
- Highly abstract
- Only Entities are visible
- Abstract relationship


### Logical Data Model
![](img/logical.png)
- Presence of attributes for each entity
- Key attributes and Non-key attributes
- Database agnostic (doesn't depend on any specific database)

### Physical Data Model
![](img/physical.png)
- Entities are referred to as Tables
- Attributes are refferred to as Columns
- Database compatible table names
- Data type
- Will inlcude indexes, constraints, triggers and other data objects

## phpMyAdmin
### Foriegn Key
- Table must be of innoDB engine

# Oracle SQL
## AUTO INCREMENT 
- [Identity column](https://www.oracletutorial.com/oracle-basics/oracle-identity-column/)


## Resources used
- [Relational Algebra](https://www.youtube.com/watch?v=tii7xcFilOA)
- [Normalization - KNOWLEDGE GATE](https://youtu.be/oylHRgBDfNc)
- https://youtu.be/RJ9TpkWKyU0
- [Normalization](https://www.youtube.com/playlist?list=PLLGlmW7jT-nTr1ory9o2MgsOmmx2w8FB3)
