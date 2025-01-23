# Paramatised Views
PARAMATISED VIEWS

[https://canvas.sunderland.ac.uk/courses/75411/files/14951981?wrap=1](https://canvas.sunderland.ac.uk/courses/75411/files/14951981?wrap=1) 

^ (SQL FILE FOR THIS STUFF)

/`/can see all of the data from SELECT between 12 and 5 o-clock in real life`

`CREATE VIEW view_name AS`

`SELECT t.tennant_no , t.t_forenames , t.t_surnames`

`FROM tennant t`

`WHERE EXTRACT (HOUR FROM CURRENT_TIME) >= 12`

`AND EXTRACT (HOUR FROM CURRENT_TIME) < 17;`