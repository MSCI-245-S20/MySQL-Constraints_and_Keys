{Check It!|assessment}(test-1960107837)

|||info
### Reset challenge database
If you make a mistake while editing the `college` database in this challenge or just want to reset the database back to its original state, return to this page and click the “Reset Challenge Database” button below.

{Reset Challenge Database}(node --no-warnings .guides/sqltests/fw-sql-reset-college-2.js)
|||
---

|||guidance

### Correct answers: 

`USE college;`

Single line statement:

``` 
ALTER TABLE students ADD COLUMN classroom_id INT(3) UNSIGNED NULL, ADD CONSTRAINT FOREIGN KEY (classroom_id) REFERENCES classrooms(id);
```

Multi-line statement:

```
mysql> ALTER TABLE students
    -> ADD COLUMN classroom_id INT(3) UNSIGNED NULL,
    -> ADD CONSTRAINT FOREIGN KEY (classroom_id)
    -> REFERENCES classrooms(id);
```

|||
