# Databases-Assignment_7

## Exercise 1

### *Mention which violation(s) there are to:*

**First normal form:** None, because we can use *customerNumber* as the primary key.

**Second normal form:** None, beacuse the table is in the first normal form, and nothing seems to imply that a compound key is being used, so every column depends on the whole key (*customerNumber*).

**Third normal form:** Transitive dependencies – *city* depends on *postalCode*.



## Exercise 2
### *Assume we did not include the customerNumber in the table. What could be a key, and do we get the same violations of the normal forms?*

*customerName* could be a good alternative to the primary key, but the violations would stay the same.



## Exercise 3
### *1. Write a safe update statement that change the repPhone column from oldNumber (say 12345678) to newNumber (say 87654321).*
```sql
UPDATE CustomerOverview SET repPhone=87654321 WHERE repPhone=12345678
```
### *2. Write an update of repEmail which do not update properly (do not update it everywhere it should).*
```sql
UPDATE CustomerOverview SET repPhone=87654321
```



## Exercise 4
### *Draw a representation of of the B+ tree with index and leaf nodes, as well as the actual table data.*
