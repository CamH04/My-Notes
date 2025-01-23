# SQL for User Managment
Create new user

`CREATE USER <userid> PASSWORD ‘newpassword’ CREATEDB;`

Gives connect privilege to user

`GRANT CONNECT ON DATABASE <dbname> TO <userid>;`

Drop User

`DROP USER <userid>;`