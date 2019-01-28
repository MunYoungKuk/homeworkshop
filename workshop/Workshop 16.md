# Workshop 16

```sql
ALTER TABLE bands
ADD members INTEGER;

UPDATE bands
SET members=4
WHERE id=1;

UPDATE bands
SET members=5
WHERE id=2;

UPDATE bands
SET members=6
WHERE id=3;

UPDATE bands
SET members=3
WHERE id=3;

DELETE FROM bands
WHERE id=2;
```

