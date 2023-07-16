#  Show databases
``` show databases 
```
# to create new db
```
use test
```
# for all collections
```
show collections
```
# for inserting new 
```
db.users.insert({ id: 1,name:"terst",age:24 })
```
# Drop database
```db.dropDatabase(test)  ```
# Know your current selected database
```
db
```
# create backup (Linux)
```
sudo mongodump --db newdb --out /var/backups/mongobackups/$(date +'%m-%d-%y')
```

# Resotore database (Linux)
```
sudo mongorestore --db newdb --drop /var/backups/mongobackups/10-29-20/newdb/
```
# create backup (Windows)
```
mongodump -d AmeliaFinalDB2023 -o "C:\DBBackup"
```
# Resotore database (Windows)

```
mongorestore -d AmeliaFinalDB2023 D:\DBBackup\DB2023
```