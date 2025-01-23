# Row Level Security
ROW LEVEL Security

https://canvas.sunderland.ac.uk/courses/75411/files/14951982?wrap=1

^ (SQL FILE FOR THIS STUFF)

views on the db are listed in biews tab

to see what polices are linked to a table look at RLS policies table on the table

`===============================================`

`//creates the view to put policys in and to store attributes`

`CREATE VIEW staff_branches`

`//give view to role`

`GRANT SELECT ON staff_branches TO manager`

`===============================================`

`RLS eg:`

`// what this does is that the only row that the user can see is their own, their username is stored in staff_no`

`// everything after the with check statment is satying that these are the conditions they can insert  / update / delete to`

`ALTER TABLE table ENABLE ROW LEVEL SECURITY`

`CREATE POLICY name ON table TO role USING (CURRENT_USER = 'u'||staff_no) WITH CHECK (CURRENT_USER = 'u'||staff_no);`

`===============================================`

`RLS eg:`

`//can see rows in which i am a manager of that branch`

`CREATE POLICY manager_policy ON staff TO manager`

`USING (branch_no = (SELECT branch_no FROM staff_branches));`

`===============================================`