# Fix corrupt sqlite3 database

One day, I got the below error when I want to write to my sqlite database

```
sqlalchemy.exc.DatabaseError: (sqlite3.DatabaseError) database disk image is malformed
```

With the guidance in [this SO post](https://stackoverflow.com/questions/5274202/sqlite3-database-or-disk-is-full-the-database-disk-image-is-malformed), I was able to fix the corrupt database file.

```bash
cd $DATABASE_LOCATION
echo '.dump'|sqlite3 $DB_NAME|sqlite3 repaired_$DB_NAME
mv $DB_NAME corrupt_$DB_NAME
mv repaired_$DB_NAME $DB_NAME
```