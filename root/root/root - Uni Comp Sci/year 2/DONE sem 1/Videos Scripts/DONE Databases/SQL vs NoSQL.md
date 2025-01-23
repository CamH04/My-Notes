# SQL vs NoSQL
Key Value Based NoSQL system vs SQL based systems

What is a document store db. A db that stores / retrieves data as documents, much like a text document with multiple key value pairs within a document

I also prefer a document store model compared to a key value system as it allows for the storage of embedded documents 

**Referance:**

> Khan, W.; Kumar, T.; Zhang, C.; Raj, K.; Roy, A.M.; Luo, B.  
> SQL and NoSQL Database Software Architecture Performance Analysis and Assessments—A Systematic Literature Review.  
> Big Data Cogn. Comput. 2023, 7, 97.

[_https://doi.org/10.3390/bdcc7020097_](https://doi.org/10.3390/bdcc7020097)

^  
SQL and NoSQL Database Software Architecture Performance Analysis and Assessments—A Systematic Literature Review  
Litreture Review on studys based on NoSQl vs SQL

1.  Mongo Db dwarf usage (43) , 2nd highest being mySQL (22)
2.  Sql v noSQl isnt about relational v non relational. Its about the debate of the importatnce of ACID properties wihtin a DBMS (atomism, consistency, isolation, and durability.)NoSQl says its useless and provides the CAP theory insted as proposed by Professor Eric Brewer (consistency, availability, and partition tolerance)
3.  I think that the CAP theroy is much more relevent in todays world due to the persistance of big data  
    and its important role in socity,
4.  CAP lends itself to big data much more effectivly due to its relative flexibility especialy when compared  
    to the extreamly constrictive nature of a SQL / Relational System due to them utalising acid transaction systems

> Ali, Wajid & Majeed, Muhammad & Raza, Ali & Shafique, Muhammad Usman. (2019).  
> Comparison between SQL and NoSQL Databases and Their Relationship with Big Data Analytics. Asian Journal of Computer > Science and Information Technology. 4. 1-10. 10.9734/AJRCOS/2019/v4i230108.

[_https://www.researchgate.net/publication/336686999\_Comparison\_between\_SQL\_and\_NoSQL\_Databases\_and\_Their\_Relationship\_with\_Big\_Data\_Analytics_](https://www.researchgate.net/publication/336686999_Comparison_between_SQL_and_NoSQL_Databases_and_Their_Relationship_with_Big_Data_Analytics)

In Conclution Pharagraph:  
5\. These NoSQL data models are understandable and simple to execute and do not involve complicated methods for SQL optimization in Big Data analysis  
6\. ^ this point is especily one to take into consideration due to the importance of optimisation of the database in a big data system

1.  But this all leads back to the point that ACID transactions do provide more security esspecialy in which the situations reqire alot less of a complex data store model than big data databases
2.  Due to document / key value based systems not having a standered query language , data lookup can become obtuse within smaller systems
3.  But document / key value store NoSQL database systems allow for nested documents and arrays without having to worry about data redundency

> Hiyane, Y. & Benmakhlouf, Amine & Marzouk, A.. (2020).  
> Storing Data in A Document-oriented Database and Implemented from A Structured Nesting Logical Model. International > Journal of Database Management Systems. 12. 17-23. 10.5121/ijdms.2020.12202.  
> [_https://www.researchgate.net/publication/341242076\_Storing\_Data\_in\_A\_Document-oriented\_Database\_and\_Implemented\_from\_A\_Structured\_Nesting\_Logical\_Model_](https://www.researchgate.net/publication/341242076_Storing_Data_in_A_Document-oriented_Database_and_Implemented_from_A_Structured_Nesting_Logical_Model)

So for such an example i would use an sql database due to its security in data redundancy and duplication when properly implemented.