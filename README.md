# Database ![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)
## Functional Dependency
- If, A -> B we get a definite value of B for each A

Example: for each a from A, if a1 != a2 then b1 != b2 (b1,b2 from B)
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
Sample table: <br />
| Roll no       | Name     | Age     | Roll ID     | Dept     | HOD Name     | HOD Phone     | 
| :------------- | :----------: |  :----------: |  :----------: |  :----------: |  :----------: |  :----------: | 
|1 | A | 20 | 101  | CSE  | John Doe | 01800000000|
|2 | B | 22 | 102  | CSE  | John Doe | 01800000000|

**Anomaly:**
- Insertion anomaly: whenever we try to update one record, we need to add duplicate data
- Deletion anomaly: Deletion of all CSE students will lead to complete annihilation of all CSE department data
- Update anomaly: If the HOD of CSE get's changed then we need to update every CSE record


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



## Resources used
- [Normalization - KNOWLEDGE GATE](https://youtu.be/oylHRgBDfNc)
- https://youtu.be/RJ9TpkWKyU0
