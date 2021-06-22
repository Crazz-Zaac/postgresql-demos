## Creating database through terminal (for postgres)
1. Creating a user 'postgres' : 
``` sudo -u postgres -i 
```
2. Creating a user 'student' within the postgres: 
``` createuser student 
```
3. Creating a database: 
``` createdb studentdb 
```
4. Accesing the postgres Shell: 
```psql
```
5. Providing the privileges to the postgres user
```$ alter user student with encrypted password 'student';
$ grant all privileges on database studentdb to student;

```
6. To allow the user 'student' to create database. 
```alter user student createdb;
```
If this is not done, you won't be able to create any databases and prompt you with 
an error, `Permission denied...`

## 

