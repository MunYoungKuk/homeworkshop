# Workshop 15

## Problem 01

```sql
CREATE TABLE bands(
id INTEGER,name TEXT,debut INTEGER
);
INSERT INTO bands(id,name,debut)
VALUES(1,"Queen",1973);
INSERT INTO bands(id,name,debut)
VALUES(2,"Coldplay",1998);
INSERT INTO bands(id,name,debut)
VALUES(3,"MCR",2001);
```

## Problem 02

```sql
SELECT id,name FROM bands;
```

## Problem 03

```sql
SELECT name
FROM bands
WHERE debut<2000;
```





