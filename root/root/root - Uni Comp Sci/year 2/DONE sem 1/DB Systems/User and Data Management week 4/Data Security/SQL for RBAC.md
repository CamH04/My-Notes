# SQL for RBAC
Allow a privilege to a user 

`GRANT <privilege> ON <object> TO <user(s)/role>;`

Remove a privilege to a user 

`REVOKE <privilege> ON <object> FROM <user(s)/role>;`

Common privileges are:

*   ALL, SELECT, INSERT, UPDATE, DELETE

Objects can be

*   Tables, columns, views

EGS

Privileges can be granted to users or roles, e.g:  
`CREATE ROLE admin_role;`  
`GRANT INSERT ON my_table TO admin_role;`  
`GRANT admin_role TO fred;`  
 

To revoke/remove roles:  
`REVOKE admin_role FROM barney;`  
`DROP ROLE admin_role;`