# DONE Databases
1.  Show old er diagram
    1.  (Assuming each bank only has 1 sort code,  
        new banks table,  
        Changes to data inserted into payment)
2.  Explain my rationale behind the conversion from SQL to NoSQL db 
    1.  I dont need a bank accounts table because i can have the details within an object array of documents within the document of customers
    2.  each shop can also have an array of documents which contain the items stored at a shop
3.  run the database from nothing
4.  talk about any issues encountered in development 
    1.  json syntax / javascript, error messages were vague at best making debugging an issue, especially on last aggregation where the squiggly brackets were really annoying
5.  SQL VS NoSQL